# Comparing `tmp/lnschema_lamin1-0.17a1.tar.gz` & `tmp/lnschema_lamin1-0.17a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnschema_lamin1-0.17a1.tar", last modified: Thu May 25 22:09:04 2023, max compression
+gzip compressed data, was "lnschema_lamin1-0.17a2.tar", last modified: Sat May 27 05:11:31 2023, max compression
```

## Comparing `lnschema_lamin1-0.17a1.tar` & `lnschema_lamin1-0.17a2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     3577 2023-04-22 05:28:10.791442 lnschema_lamin1-0.17a1/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-04-22 03:48:17.570277 lnschema_lamin1-0.17a1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-04-22 03:48:17.570464 lnschema_lamin1-0.17a1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1416 2023-04-22 03:51:54.773184 lnschema_lamin1-0.17a1/.gitignore
--rw-r--r--   0        0        0     1795 2023-04-24 17:49:33.167540 lnschema_lamin1-0.17a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      154 2023-05-25 15:48:48.190697 lnschema_lamin1-0.17a1/README.md
--rw-r--r--   0        0        0     1069 2023-05-25 21:06:40.200485 lnschema_lamin1-0.17a1/docs/changelog.md
--rw-r--r--   0        0        0     5015 2023-04-24 17:39:09.187958 lnschema_lamin1-0.17a1/docs/guide/01-get-started.ipynb
--rw-r--r--   0        0        0     2190 2023-04-24 17:39:09.199540 lnschema_lamin1-0.17a1/docs/guide/02-orms.ipynb
--rw-r--r--   0        0        0     5397 2023-04-24 17:39:09.201311 lnschema_lamin1-0.17a1/docs/guide/10-migrate.ipynb
--rw-r--r--   0        0        0       65 2023-04-22 04:06:04.615921 lnschema_lamin1-0.17a1/docs/guide/index.md
--rw-r--r--   0        0        0      122 2023-04-22 03:48:11.331800 lnschema_lamin1-0.17a1/docs/index.md
--rw-r--r--   0        0        0       63 2023-04-22 03:51:55.148920 lnschema_lamin1-0.17a1/docs/reference.md
--rw-r--r--   0        0        0      163 2023-04-22 04:44:31.557229 lnschema_lamin1-0.17a1/lamin-project.yaml
--rw-r--r--   0        0        0      641 2023-05-25 21:06:29.118991 lnschema_lamin1-0.17a1/lnschema_lamin1/__init__.py
--rw-r--r--   0        0        0     4310 2023-05-25 21:05:50.419914 lnschema_lamin1-0.17a1/lnschema_lamin1/_core.py
--rw-r--r--   0        0        0     2902 2023-05-25 21:05:50.420200 lnschema_lamin1-0.17a1/lnschema_lamin1/_link.py
--rw-r--r--   0        0        0      259 2023-05-25 15:48:48.191950 lnschema_lamin1-0.17a1/lnschema_lamin1/dev/__init__.py
--rw-r--r--   0        0        0      119 2023-04-22 03:48:17.441295 lnschema_lamin1-0.17a1/lnschema_lamin1/dev/_id.py
--rw-r--r--   0        0        0      346 2023-05-25 15:48:48.192035 lnschema_lamin1-0.17a1/lnschema_lamin1/dev/_type.py
--rw-r--r--   0        0        0     1145 2023-04-22 03:56:14.122435 lnschema_lamin1-0.17a1/lnschema_lamin1/dev/_versions.py
--rw-r--r--   0        0        0       31 2023-04-22 03:48:17.441214 lnschema_lamin1-0.17a1/lnschema_lamin1/dev/id.py
--rw-r--r--   0        0        0      156 2023-05-25 15:48:48.192133 lnschema_lamin1-0.17a1/lnschema_lamin1/dev/type.py
--rw-r--r--   0        0        0      426 2023-05-25 15:48:48.192250 lnschema_lamin1-0.17a1/lnschema_lamin1/link.py
--rw-r--r--   0        0        0     1063 2023-04-24 17:49:33.169471 lnschema_lamin1-0.17a1/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py
--rw-r--r--   0        0        0     4097 2023-05-25 15:48:48.192371 lnschema_lamin1-0.17a1/lnschema_lamin1/migrations/versions/2023-05-15-a0867fc8d6e5-v0_16_2.py
--rw-r--r--   0        0        0     2251 2023-05-25 15:48:48.192464 lnschema_lamin1-0.17a1/lnschema_lamin1/migrations/versions/2023-05-23-f9f58cf3ab38-v0_16_3.py
--rw-r--r--   0        0        0     4920 2023-05-25 21:05:50.420445 lnschema_lamin1-0.17a1/lnschema_lamin1/migrations/versions/2023-05-25-c3f38ffe9e05-v0_17_0.py
--rw-r--r--   0        0        0      776 2023-04-24 16:11:06.697345 lnschema_lamin1-0.17a1/noxfile.py
--rw-r--r--   0        0        0      655 2023-05-25 21:25:20.217756 lnschema_lamin1-0.17a1/pyproject.toml
--rw-r--r--   0        0        0      811 2023-04-22 04:38:14.658100 lnschema_lamin1-0.17a1/tests/test_migrations.py
--rw-r--r--   0        0        0      481 2023-04-22 03:48:11.224317 lnschema_lamin1-0.17a1/tests/test_notebooks.py
--rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 lnschema_lamin1-0.17a1/PKG-INFO
+-rw-r--r--   0        0        0     3577 2023-04-22 05:28:10.791442 lnschema_lamin1-0.17a2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-04-22 03:48:17.570277 lnschema_lamin1-0.17a2/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-04-22 03:48:17.570464 lnschema_lamin1-0.17a2/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1416 2023-04-22 03:51:54.773184 lnschema_lamin1-0.17a2/.gitignore
+-rw-r--r--   0        0        0     1795 2023-04-24 17:49:33.167540 lnschema_lamin1-0.17a2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      154 2023-05-25 15:48:48.190697 lnschema_lamin1-0.17a2/README.md
+-rw-r--r--   0        0        0     1069 2023-05-27 05:11:12.141464 lnschema_lamin1-0.17a2/docs/changelog.md
+-rw-r--r--   0        0        0     5015 2023-04-24 17:39:09.187958 lnschema_lamin1-0.17a2/docs/guide/01-get-started.ipynb
+-rw-r--r--   0        0        0     2190 2023-04-24 17:39:09.199540 lnschema_lamin1-0.17a2/docs/guide/02-orms.ipynb
+-rw-r--r--   0        0        0     5397 2023-04-24 17:39:09.201311 lnschema_lamin1-0.17a2/docs/guide/10-migrate.ipynb
+-rw-r--r--   0        0        0       65 2023-04-22 04:06:04.615921 lnschema_lamin1-0.17a2/docs/guide/index.md
+-rw-r--r--   0        0        0      122 2023-04-22 03:48:11.331800 lnschema_lamin1-0.17a2/docs/index.md
+-rw-r--r--   0        0        0       63 2023-04-22 03:51:55.148920 lnschema_lamin1-0.17a2/docs/reference.md
+-rw-r--r--   0        0        0      163 2023-04-22 04:44:31.557229 lnschema_lamin1-0.17a2/lamin-project.yaml
+-rw-r--r--   0        0        0      684 2023-05-27 05:11:02.526940 lnschema_lamin1-0.17a2/lnschema_lamin1/__init__.py
+-rw-r--r--   0        0        0     4310 2023-05-25 21:05:50.419914 lnschema_lamin1-0.17a2/lnschema_lamin1/_core.py
+-rw-r--r--   0        0        0     2902 2023-05-25 21:05:50.420200 lnschema_lamin1-0.17a2/lnschema_lamin1/_link.py
+-rw-r--r--   0        0        0      259 2023-05-25 15:48:48.191950 lnschema_lamin1-0.17a2/lnschema_lamin1/dev/__init__.py
+-rw-r--r--   0        0        0      119 2023-04-22 03:48:17.441295 lnschema_lamin1-0.17a2/lnschema_lamin1/dev/_id.py
+-rw-r--r--   0        0        0      346 2023-05-25 15:48:48.192035 lnschema_lamin1-0.17a2/lnschema_lamin1/dev/_type.py
+-rw-r--r--   0        0        0     1145 2023-04-22 03:56:14.122435 lnschema_lamin1-0.17a2/lnschema_lamin1/dev/_versions.py
+-rw-r--r--   0        0        0       31 2023-04-22 03:48:17.441214 lnschema_lamin1-0.17a2/lnschema_lamin1/dev/id.py
+-rw-r--r--   0        0        0      156 2023-05-25 15:48:48.192133 lnschema_lamin1-0.17a2/lnschema_lamin1/dev/type.py
+-rw-r--r--   0        0        0      426 2023-05-25 15:48:48.192250 lnschema_lamin1-0.17a2/lnschema_lamin1/link.py
+-rw-r--r--   0        0        0     1063 2023-04-24 17:49:33.169471 lnschema_lamin1-0.17a2/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py
+-rw-r--r--   0        0        0     4097 2023-05-25 15:48:48.192371 lnschema_lamin1-0.17a2/lnschema_lamin1/migrations/versions/2023-05-15-a0867fc8d6e5-v0_16_2.py
+-rw-r--r--   0        0        0     2251 2023-05-25 15:48:48.192464 lnschema_lamin1-0.17a2/lnschema_lamin1/migrations/versions/2023-05-23-f9f58cf3ab38-v0_16_3.py
+-rw-r--r--   0        0        0     4920 2023-05-25 21:05:50.420445 lnschema_lamin1-0.17a2/lnschema_lamin1/migrations/versions/2023-05-25-c3f38ffe9e05-v0_17_0.py
+-rw-r--r--   0        0        0      776 2023-04-24 16:11:06.697345 lnschema_lamin1-0.17a2/noxfile.py
+-rw-r--r--   0        0        0      663 2023-05-26 15:20:03.193182 lnschema_lamin1-0.17a2/pyproject.toml
+-rw-r--r--   0        0        0      811 2023-04-22 04:38:14.658100 lnschema_lamin1-0.17a2/tests/test_migrations.py
+-rw-r--r--   0        0        0      481 2023-04-22 03:48:11.224317 lnschema_lamin1-0.17a2/tests/test_notebooks.py
+-rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 lnschema_lamin1-0.17a2/PKG-INFO
```

### Comparing `lnschema_lamin1-0.17a1/.github/workflows/build.yml` & `lnschema_lamin1-0.17a2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a1/.github/workflows/latest-changes.yml` & `lnschema_lamin1-0.17a2/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a1/.gitignore` & `lnschema_lamin1-0.17a2/.gitignore`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a1/.pre-commit-config.yaml` & `lnschema_lamin1-0.17a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a1/docs/changelog.md` & `lnschema_lamin1-0.17a2/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-🏗️ Remove SQL-level schema modules | [9](https://github.com/laminlabs/lnschema-lamin1/pull/9) | [falexwolf](https://github.com/falexwolf) | 2023-05-25 | 0.17a1
+🏗️ Remove SQL-level schema modules | [9](https://github.com/laminlabs/lnschema-lamin1/pull/9) | [falexwolf](https://github.com/falexwolf) | 2023-05-25 | 0.17a2
 🎨 Add `Well` table, File.cell_lines | [8](https://github.com/laminlabs/lnschema-lamin1/pull/8) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-23 | 0.16.3
 💚 Removed treatment relationships | [4](https://github.com/laminlabs/lnschema-lamin1/pull/4) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-15 | 0.16.2
 ✨ Added `Treatment` table | [3](https://github.com/laminlabs/lnschema-lamin1/pull/3) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-15 |
 🚚 Link `CellType` to `File` | [2](https://github.com/laminlabs/lnschema-lamin1/pull/2) | [falexwolf](https://github.com/falexwolf) | 2023-04-24 | 0.16.1
 🎉 Move content from `lnschema-wetlab` here | [1](https://github.com/laminlabs/lnschema-lamin1/pull/1) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.15.1
```

### Comparing `lnschema_lamin1-0.17a1/docs/guide/01-get-started.ipynb` & `lnschema_lamin1-0.17a2/docs/guide/01-get-started.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a1/docs/guide/02-orms.ipynb` & `lnschema_lamin1-0.17a2/docs/guide/02-orms.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a1/docs/guide/10-migrate.ipynb` & `lnschema_lamin1-0.17a2/docs/guide/10-migrate.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a1/lnschema_lamin1/__init__.py` & `lnschema_lamin1-0.17a2/lnschema_lamin1/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,31 +10,39 @@
    :toctree: .
 
    Experiment
    ExperimentType
    Biosample
    Techsample
    Treatment
+   Well
 
 Development tools:
 
 .. autosummary::
    :toctree: .
 
    dev
    link
 
 """
 
 _schema_id = "tvhn"
 _name = "lamin1"
-_migration = "f9f58cf3ab38"
-__version__ = "0.17a1"
+_migration = "c3f38ffe9e05"
+__version__ = "0.17a2"
 
 # prints warning of python versions
 from lamin_logger import py_version_warning
 
 py_version_warning("3.8", "3.10")
 
 
 from . import dev, link
-from ._core import Biosample, Experiment, ExperimentType, Techsample, Treatment  # noqa
+from ._core import (  # noqa
+    Biosample,
+    Experiment,
+    ExperimentType,
+    Techsample,
+    Treatment,
+    Well,
+)
```

### Comparing `lnschema_lamin1-0.17a1/lnschema_lamin1/_core.py` & `lnschema_lamin1-0.17a2/lnschema_lamin1/_core.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a1/lnschema_lamin1/_link.py` & `lnschema_lamin1-0.17a2/lnschema_lamin1/_link.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a1/lnschema_lamin1/dev/_versions.py` & `lnschema_lamin1-0.17a2/lnschema_lamin1/dev/_versions.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a1/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py` & `lnschema_lamin1-0.17a2/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a1/lnschema_lamin1/migrations/versions/2023-05-15-a0867fc8d6e5-v0_16_2.py` & `lnschema_lamin1-0.17a2/lnschema_lamin1/migrations/versions/2023-05-15-a0867fc8d6e5-v0_16_2.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a1/lnschema_lamin1/migrations/versions/2023-05-23-f9f58cf3ab38-v0_16_3.py` & `lnschema_lamin1-0.17a2/lnschema_lamin1/migrations/versions/2023-05-23-f9f58cf3ab38-v0_16_3.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a1/lnschema_lamin1/migrations/versions/2023-05-25-c3f38ffe9e05-v0_17_0.py` & `lnschema_lamin1-0.17a2/lnschema_lamin1/migrations/versions/2023-05-25-c3f38ffe9e05-v0_17_0.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a1/noxfile.py` & `lnschema_lamin1-0.17a2/noxfile.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a1/pyproject.toml` & `lnschema_lamin1-0.17a2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "lnschema_lamin1"
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
-    "lamindb[bionty,biolab]",
+    "lamindb[bionty,biolab]>=0.41a2",
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/lnschema-lamin1"
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `lnschema_lamin1-0.17a1/tests/test_migrations.py` & `lnschema_lamin1-0.17a2/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.17a1/PKG-INFO` & `lnschema_lamin1-0.17a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lnschema_lamin1
-Version: 0.17a1
+Version: 0.17a2
 Summary: Lamin's `lamin1` lab schema (`tvhn`).
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
-Requires-Dist: lamindb[bionty,biolab]
+Requires-Dist: lamindb[bionty,biolab]>=0.41a2
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: nbproject_test>=0.4.1 ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lnschema-lamin1
 Provides-Extra: dev
```

