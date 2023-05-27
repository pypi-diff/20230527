# Comparing `tmp/lndb_storage-0.3.0.tar.gz` & `tmp/lndb_storage-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb_storage-0.3.0.tar", last modified: Tue May 23 16:02:13 2023, max compression
+gzip compressed data, was "lndb_storage-0.3.1.tar", last modified: Sat May 27 16:11:15 2023, max compression
```

## Comparing `lndb_storage-0.3.0.tar` & `lndb_storage-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     3181 2023-04-10 13:55:12.337864 lndb_storage-0.3.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-03-29 20:45:21.388328 lndb_storage-0.3.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-03-29 20:45:21.388401 lndb_storage-0.3.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2023-03-29 20:45:21.388463 lndb_storage-0.3.0/.gitignore
--rw-r--r--   0        0        0     1765 2023-04-24 16:53:24.500304 lndb_storage-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-03-29 20:45:21.388633 lndb_storage-0.3.0/LICENSE
--rw-r--r--   0        0        0      124 2023-03-29 20:45:21.388936 lndb_storage-0.3.0/README.md
--rw-r--r--   0        0        0     3250 2023-05-23 16:01:47.084797 lndb_storage-0.3.0/docs/changelog.md
--rw-r--r--   0        0        0     9684 2023-04-23 22:03:51.292643 lndb_storage-0.3.0/docs/guide/add-replace-stage.ipynb
--rw-r--r--   0        0        0       88 2023-04-09 22:14:23.875135 lndb_storage-0.3.0/docs/guide/index.md
--rw-r--r--   0        0        0     3976 2023-04-08 09:43:17.308905 lndb_storage-0.3.0/docs/guide/iris.csv
--rw-r--r--   0        0        0     4550 2023-04-08 09:43:17.309082 lndb_storage-0.3.0/docs/guide/iris.data
--rw-r--r--   0        0        0     4349 2023-04-23 22:03:51.292792 lndb_storage-0.3.0/docs/guide/new_iris.csv
--rw-r--r--   0        0        0     4615 2023-04-10 12:49:18.628116 lndb_storage-0.3.0/docs/guide/serialize-cache.ipynb
--rw-r--r--   0        0        0     4069 2023-04-24 16:53:24.501276 lndb_storage-0.3.0/docs/guide/stream.ipynb
--rw-r--r--   0        0        0     7566 2023-04-10 10:36:19.544617 lndb_storage-0.3.0/docs/guide/upload.ipynb
--rw-r--r--   0        0        0      122 2023-04-10 13:20:18.123402 lndb_storage-0.3.0/docs/index.md
--rw-r--r--   0        0        0       60 2023-04-09 20:42:44.949390 lndb_storage-0.3.0/docs/reference.md
--rw-r--r--   0        0        0      160 2023-03-29 20:45:21.390164 lndb_storage-0.3.0/lamin-project.yaml
--rw-r--r--   0        0        0      579 2023-05-23 16:01:34.728417 lndb_storage-0.3.0/lndb_storage/__init__.py
--rw-r--r--   0        0        0     3337 2023-04-18 11:35:08.919567 lndb_storage-0.3.0/lndb_storage/_file.py
--rw-r--r--   0        0        0      492 2023-04-16 20:58:33.198299 lndb_storage-0.3.0/lndb_storage/_h5ad.py
--rw-r--r--   0        0        0      204 2023-03-29 20:45:21.390606 lndb_storage-0.3.0/lndb_storage/_images.py
--rw-r--r--   0        0        0     2307 2023-03-29 20:45:21.390671 lndb_storage-0.3.0/lndb_storage/_subset.py
--rw-r--r--   0        0        0     2764 2023-04-09 20:42:44.950408 lndb_storage-0.3.0/lndb_storage/_zarr.py
--rw-r--r--   0        0        0      317 2023-03-29 20:45:21.390956 lndb_storage-0.3.0/lndb_storage/object/__init__.py
--rw-r--r--   0        0        0      945 2023-04-16 20:58:33.198732 lndb_storage-0.3.0/lndb_storage/object/_anndata.py
--rw-r--r--   0        0        0      730 2023-03-29 20:45:21.391077 lndb_storage-0.3.0/lndb_storage/object/_anndata_sizes.py
--rw-r--r--   0        0        0      900 2023-03-29 20:45:21.391132 lndb_storage-0.3.0/lndb_storage/object/_core.py
--rw-r--r--   0        0        0     4116 2023-03-29 20:45:21.391201 lndb_storage-0.3.0/lndb_storage/object/_lazy_field.py
--rw-r--r--   0        0        0     4853 2023-05-23 14:42:49.806479 lndb_storage-0.3.0/lndb_storage/object/_subset_anndata.py
--rw-r--r--   0        0        0      919 2023-04-24 16:53:24.501654 lndb_storage-0.3.0/noxfile.py
--rw-r--r--   0        0        0     1108 2023-05-23 14:40:16.493381 lndb_storage-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      484 2023-05-23 14:40:16.493813 lndb_storage-0.3.0/tests/test_notebooks.py
--rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 lndb_storage-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3181 2023-04-10 13:55:12.337864 lndb_storage-0.3.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-03-29 20:45:21.388328 lndb_storage-0.3.1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-03-29 20:45:21.388401 lndb_storage-0.3.1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2023-03-29 20:45:21.388463 lndb_storage-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1765 2023-04-24 16:53:24.500304 lndb_storage-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-03-29 20:45:21.388633 lndb_storage-0.3.1/LICENSE
+-rw-r--r--   0        0        0      124 2023-03-29 20:45:21.388936 lndb_storage-0.3.1/README.md
+-rw-r--r--   0        0        0     3430 2023-05-27 16:10:58.877632 lndb_storage-0.3.1/docs/changelog.md
+-rw-r--r--   0        0        0     9684 2023-04-23 22:03:51.292643 lndb_storage-0.3.1/docs/guide/add-replace-stage.ipynb
+-rw-r--r--   0        0        0       88 2023-04-09 22:14:23.875135 lndb_storage-0.3.1/docs/guide/index.md
+-rw-r--r--   0        0        0     3976 2023-04-08 09:43:17.308905 lndb_storage-0.3.1/docs/guide/iris.csv
+-rw-r--r--   0        0        0     4550 2023-04-08 09:43:17.309082 lndb_storage-0.3.1/docs/guide/iris.data
+-rw-r--r--   0        0        0     4349 2023-04-23 22:03:51.292792 lndb_storage-0.3.1/docs/guide/new_iris.csv
+-rw-r--r--   0        0        0     4615 2023-04-10 12:49:18.628116 lndb_storage-0.3.1/docs/guide/serialize-cache.ipynb
+-rw-r--r--   0        0        0     5600 2023-05-27 16:08:47.046588 lndb_storage-0.3.1/docs/guide/stream.ipynb
+-rw-r--r--   0        0        0     7566 2023-04-10 10:36:19.544617 lndb_storage-0.3.1/docs/guide/upload.ipynb
+-rw-r--r--   0        0        0      122 2023-04-10 13:20:18.123402 lndb_storage-0.3.1/docs/index.md
+-rw-r--r--   0        0        0       60 2023-04-09 20:42:44.949390 lndb_storage-0.3.1/docs/reference.md
+-rw-r--r--   0        0        0      160 2023-03-29 20:45:21.390164 lndb_storage-0.3.1/lamin-project.yaml
+-rw-r--r--   0        0        0      579 2023-05-27 16:10:40.280665 lndb_storage-0.3.1/lndb_storage/__init__.py
+-rw-r--r--   0        0        0     3337 2023-04-18 11:35:08.919567 lndb_storage-0.3.1/lndb_storage/_file.py
+-rw-r--r--   0        0        0      492 2023-04-16 20:58:33.198299 lndb_storage-0.3.1/lndb_storage/_h5ad.py
+-rw-r--r--   0        0        0      204 2023-03-29 20:45:21.390606 lndb_storage-0.3.1/lndb_storage/_images.py
+-rw-r--r--   0        0        0     2307 2023-03-29 20:45:21.390671 lndb_storage-0.3.1/lndb_storage/_subset.py
+-rw-r--r--   0        0        0     2764 2023-04-09 20:42:44.950408 lndb_storage-0.3.1/lndb_storage/_zarr.py
+-rw-r--r--   0        0        0      317 2023-03-29 20:45:21.390956 lndb_storage-0.3.1/lndb_storage/object/__init__.py
+-rw-r--r--   0        0        0      945 2023-04-16 20:58:33.198732 lndb_storage-0.3.1/lndb_storage/object/_anndata.py
+-rw-r--r--   0        0        0    11730 2023-05-27 16:08:47.046772 lndb_storage-0.3.1/lndb_storage/object/_anndata_accessor.py
+-rw-r--r--   0        0        0      730 2023-03-29 20:45:21.391077 lndb_storage-0.3.1/lndb_storage/object/_anndata_sizes.py
+-rw-r--r--   0        0        0      900 2023-03-29 20:45:21.391132 lndb_storage-0.3.1/lndb_storage/object/_core.py
+-rw-r--r--   0        0        0     4116 2023-03-29 20:45:21.391201 lndb_storage-0.3.1/lndb_storage/object/_lazy_field.py
+-rw-r--r--   0        0        0     3991 2023-05-27 16:08:47.047268 lndb_storage-0.3.1/lndb_storage/object/_subset_anndata.py
+-rw-r--r--   0        0        0      933 2023-05-27 16:08:47.047494 lndb_storage-0.3.1/noxfile.py
+-rw-r--r--   0        0        0     1108 2023-05-23 14:40:16.493381 lndb_storage-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      484 2023-05-23 14:40:16.493813 lndb_storage-0.3.1/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 lndb_storage-0.3.1/PKG-INFO
```

### Comparing `lndb_storage-0.3.0/.github/workflows/build.yml` & `lndb_storage-0.3.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/.github/workflows/latest-changes.yml` & `lndb_storage-0.3.1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/.gitignore` & `lndb_storage-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/.pre-commit-config.yaml` & `lndb_storage-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/LICENSE` & `lndb_storage-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/docs/changelog.md` & `lndb_storage-0.3.1/docs/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+✨ `AnnDataAccessor` for access to cloud AnnData attributes | [32](https://github.com/laminlabs/lndb-storage/pull/32) | [Koncopd](https://github.com/Koncopd) | 2023-05-27 | 0.3.1
 ✅ Use nbproject-test directly in test_notebooks.py | [31](https://github.com/laminlabs/lndb-storage/pull/31) | [Koncopd](https://github.com/Koncopd) | 2023-05-04 | 0.3.0
 ♻️ Refactor CloudAnnData | [29](https://github.com/laminlabs/lndb-storage/pull/29) | [Koncopd](https://github.com/Koncopd) | 2023-05-04 |
 🦺 Check that obs and var are dataframes in subset | [28](https://github.com/laminlabs/lndb-storage/pull/28) | [Koncopd](https://github.com/Koncopd) | 2023-05-04 |
 ✨ Add `CloudAnnData` | [26](https://github.com/laminlabs/lndb-storage/pull/26) | [falexwolf](https://github.com/falexwolf) | 2023-04-24 | 0.2rc6
 📝 Drastically simplify streaming guide | [25](https://github.com/laminlabs/lndb-storage/pull/25) | [falexwolf](https://github.com/falexwolf) | 2023-04-24 |
 ✅ Add additional tests for replace | [24](https://github.com/laminlabs/lndb-storage/pull/24) | [Koncopd](https://github.com/Koncopd) | 2023-04-23 |
 ✅ Check add with key | [20](https://github.com/laminlabs/lndb-storage/pull/20) | [Koncopd](https://github.com/Koncopd) | 2023-04-16 | 0.2rc5
```

### Comparing `lndb_storage-0.3.0/docs/guide/add-replace-stage.ipynb` & `lndb_storage-0.3.1/docs/guide/add-replace-stage.ipynb`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/docs/guide/iris.csv` & `lndb_storage-0.3.1/docs/guide/iris.csv`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/docs/guide/iris.data` & `lndb_storage-0.3.1/docs/guide/iris.data`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/docs/guide/new_iris.csv` & `lndb_storage-0.3.1/docs/guide/new_iris.csv`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/docs/guide/serialize-cache.ipynb` & `lndb_storage-0.3.1/docs/guide/serialize-cache.ipynb`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/docs/guide/stream.ipynb` & `lndb_storage-0.3.1/docs/guide/stream.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9600908251231527%*

 * *Differences: {"'cells'": "{insert: [(16, OrderedDict([('cell_type', 'code'), ('execution_count', None), "*

 * *            "('metadata', OrderedDict()), ('outputs', []), ('source', ['adata_subset'])])), (17, "*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count', None), ('metadata', "*

 * *            "OrderedDict()), ('outputs', []), ('source', "*

 * *            "['adata_subset.obs.cell_type.value_counts()'])])), (18, OrderedDict([('cell_type', "*

 * *            '\'markdown\'), (\'metadata\', OrderedDict()), (\'source\',  […]*

```diff
@@ -154,14 +154,90 @@
                 "adata_subset.obs.cell_type.value_counts()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "It is also possible to access AnnData objects' attributes and subset them directly through `file.backed()` withouth loading the full objects into memory:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "adata"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Note that the object above is an AnnDataAccessor object, not an AnnData object"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Check the reference to `.X`:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "adata.X"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Get a subset of the object, attributes are loaded only on explicit access:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "obs_idx = adata.obs.cell_type.isin([\"Dendritic cells\", \"CD14+ Monocytes\"]) & (\n",
+                "    adata.obs.percent_mito <= 0.05\n",
+                ")\n",
+                "adata_subset = adata[obs_idx]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "adata_subset"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "adata_subset.obs.cell_type.value_counts()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "You can do the same with a zarr object:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -186,15 +262,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.9.12"
         },
         "nbproject": {
             "id": "YVUCtH4GfQOy",
             "parent": null,
             "pypackage": null,
             "time_init": "2023-01-23T08:28:32.097943+00:00",
             "user_handle": "testuser1",
```

### Comparing `lndb_storage-0.3.0/docs/guide/upload.ipynb` & `lndb_storage-0.3.1/docs/guide/upload.ipynb`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/lndb_storage/__init__.py` & `lndb_storage-0.3.1/lndb_storage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
    :toctree: .
 
    store_object
    store_png
    delete_storage
 """
 
-__version__ = "0.3.0"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.3.1"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 from lndb.dev.upath import UPath
 from lndb.dev.upath import infer_filesystem as _infer_filesystem
 
 from ._file import delete_storage, load_to_memory, store_object
 from ._h5ad import h5ad_to_anndata
 from ._images import store_png
```

### Comparing `lndb_storage-0.3.0/lndb_storage/_file.py` & `lndb_storage-0.3.1/lndb_storage/_file.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/lndb_storage/_subset.py` & `lndb_storage-0.3.1/lndb_storage/_subset.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/lndb_storage/_zarr.py` & `lndb_storage-0.3.1/lndb_storage/_zarr.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/lndb_storage/object/_anndata.py` & `lndb_storage-0.3.1/lndb_storage/object/_anndata.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/lndb_storage/object/_anndata_sizes.py` & `lndb_storage-0.3.1/lndb_storage/object/_anndata_sizes.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/lndb_storage/object/_core.py` & `lndb_storage-0.3.1/lndb_storage/object/_core.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/lndb_storage/object/_lazy_field.py` & `lndb_storage-0.3.1/lndb_storage/object/_lazy_field.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/lndb_storage/object/_subset_anndata.py` & `lndb_storage-0.3.1/lndb_storage/object/_subset_anndata.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,47 @@
-from functools import cached_property
 from typing import Optional, Union
 
 import h5py
-import pandas as pd
 import zarr
 from anndata import AnnData
+from anndata._io.h5ad import read_dataframe_legacy as read_dataframe_legacy_h5
 from anndata._io.specs.methods import _read_partial
 from anndata._io.specs.registry import read_elem, read_elem_partial
+from anndata._io.zarr import read_dataframe_legacy as read_dataframe_legacy_zarr
 from lndb.dev.upath import infer_filesystem as _infer_filesystem
 from lnschema_core import File
 from lnschema_core._core import filepath_from_file_or_folder
 
 from ._lazy_field import LazySelector
 
 
+def _read_dataframe(elem: Union[zarr.Array, h5py.Dataset, zarr.Group, h5py.Group]):
+    if isinstance(elem, zarr.Array):
+        return read_dataframe_legacy_zarr(elem)
+    elif isinstance(elem, h5py.Dataset):
+        return read_dataframe_legacy_h5(elem)
+    else:
+        return read_elem(elem)
+
+
 def _indices(base_indices, select_indices):
     if len(base_indices) == len(select_indices):
         return slice(None)
     else:
         return list(base_indices.get_indexer(select_indices))
 
 
-def _to_df(val):
-    if isinstance(val, pd.DataFrame):
-        return val
-    # is array
-    elif "index" in val.dtype.fields:
-        return pd.DataFrame.from_records(val, index="index")
-    else:
-        return pd.DataFrame.from_records(val)
-
-
 def _subset_adata_storage(
     storage: Union[zarr.Group, h5py.File],
     query_obs: Optional[Union[str, LazySelector]] = None,
     query_var: Optional[Union[str, LazySelector]] = None,
 ) -> Union[AnnData, None]:
     with storage as access:
-        obs = _to_df(read_elem(access["obs"]))
-        var = _to_df(read_elem(access["var"]))
+        obs = _read_dataframe(access["obs"])
+        var = _read_dataframe(access["var"])
 
         if query_obs is not None:
             if hasattr(query_obs, "evaluate"):
                 obs_result = obs[query_obs.evaluate(obj=obs)]  # type: ignore
             else:
                 obs_result = obs.query(query_obs)
         else:
@@ -104,37 +103,7 @@
             adata = _subset_adata_storage(storage, query_obs, query_var)
     elif file.suffix == ".zarr":
         mapper = fs.get_mapper(file_path_str, check=True)
         storage = zarr.open(mapper, mode="r")
         adata = _subset_adata_storage(storage, query_obs, query_var)
 
     return adata
-
-
-class CloudAnnData:
-    def __init__(self, file: File):
-        fs, file_path_str = _infer_filesystem(filepath_from_file_or_folder(file))
-        if file.suffix == ".h5ad":
-            self._conn = fs.open(file_path_str, mode="rb")
-            self.storage = h5py.File(self._conn, mode="r")
-        elif file.suffix in (".zarr", ".zrad"):
-            self._conn = None
-            mapper = fs.get_mapper(file_path_str, check=True)
-            self.storage = zarr.open(mapper, mode="r")
-        else:
-            raise ValueError(
-                f"file should have .h5ad, .zarr or .zrad suffix, not {file.suffix}."
-            )
-
-    def __del__(self):
-        """Closes the connection."""
-        if self._conn is not None:
-            self.storage.close()
-            self._conn.close()
-
-    @cached_property
-    def obs(self) -> pd.DataFrame:
-        return _to_df(read_elem(self.storage["obs"]))
-
-    @cached_property
-    def var(self) -> pd.DataFrame:
-        return _to_df(read_elem(self.storage["var"]))
```

### Comparing `lndb_storage-0.3.0/noxfile.py` & `lndb_storage-0.3.1/noxfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     run_pre_commit(session)
 
 
 @nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
 def build(session):
     login_testuser1(session)
     session.install(".[dev,test]")
-    response = requests.get("https://github.com/laminlabs/lamindb/tree/cloud")
+    response = requests.get("https://github.com/laminlabs/lamindb/tree/adata_access")
     if response.status_code < 400:
-        session.install("git+https://github.com/laminlabs/lamindb@cloud")
+        session.install("git+https://github.com/laminlabs/lamindb@adata_access")
     else:
         session.install("git+https://github.com/laminlabs/lamindb")
     run_pytest(session)
     build_docs(session)
     upload_docs_artifact()
     move_built_docs_to_docs_slash_project_slug()
```

### Comparing `lndb_storage-0.3.0/pyproject.toml` & `lndb_storage-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.3.0/PKG-INFO` & `lndb_storage-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lndb_storage
-Version: 0.3.0
+Version: 0.3.1
 Summary: Storage → object.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core
 Requires-Dist: lndb>=0.41.0
 Requires-Dist: lamin_logger>=0.3.0
 Requires-Dist: nbproject
```

