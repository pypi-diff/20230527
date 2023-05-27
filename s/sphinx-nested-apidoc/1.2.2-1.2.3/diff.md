# Comparing `tmp/sphinx_nested_apidoc-1.2.2.tar.gz` & `tmp/sphinx_nested_apidoc-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_nested_apidoc-1.2.2.tar", max compression
+gzip compressed data, was "sphinx_nested_apidoc-1.2.3.tar", max compression
```

## Comparing `sphinx_nested_apidoc-1.2.2.tar` & `sphinx_nested_apidoc-1.2.3.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1073 2022-12-26 06:54:54.480290 sphinx_nested_apidoc-1.2.2/LICENSE
--rw-r--r--   0        0        0    10887 2022-12-26 06:54:54.480290 sphinx_nested_apidoc-1.2.2/README.rst
--rw-r--r--   0        0        0     2146 2022-12-26 06:54:54.480290 sphinx_nested_apidoc-1.2.2/pyproject.toml
--rw-r--r--   0        0        0      730 2022-12-26 06:54:54.480290 sphinx_nested_apidoc-1.2.2/src/sphinx_nested_apidoc/__init__.py
--rw-r--r--   0        0        0     4045 2022-12-26 06:54:54.480290 sphinx_nested_apidoc-1.2.2/src/sphinx_nested_apidoc/__main__.py
--rw-r--r--   0        0        0     3051 2022-12-26 06:54:54.480290 sphinx_nested_apidoc-1.2.2/src/sphinx_nested_apidoc/_ext.py
--rw-r--r--   0        0        0    11318 2022-12-26 06:54:54.480290 sphinx_nested_apidoc-1.2.2/src/sphinx_nested_apidoc/core.py
--rw-r--r--   0        0        0    12133 1970-01-01 00:00:00.000000 sphinx_nested_apidoc-1.2.2/setup.py
--rw-r--r--   0        0        0    12148 1970-01-01 00:00:00.000000 sphinx_nested_apidoc-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-27 14:48:23.868826 sphinx_nested_apidoc-1.2.3/LICENSE
+-rw-r--r--   0        0        0    10887 2023-05-27 14:48:23.868826 sphinx_nested_apidoc-1.2.3/README.rst
+-rw-r--r--   0        0        0     2321 2023-05-27 14:48:23.868826 sphinx_nested_apidoc-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0      730 2023-05-27 14:48:23.868826 sphinx_nested_apidoc-1.2.3/src/sphinx_nested_apidoc/__init__.py
+-rw-r--r--   0        0        0     4088 2023-05-27 14:48:23.868826 sphinx_nested_apidoc-1.2.3/src/sphinx_nested_apidoc/__main__.py
+-rw-r--r--   0        0        0     3145 2023-05-27 14:48:23.868826 sphinx_nested_apidoc-1.2.3/src/sphinx_nested_apidoc/_ext.py
+-rw-r--r--   0        0        0    10848 2023-05-27 14:48:23.868826 sphinx_nested_apidoc-1.2.3/src/sphinx_nested_apidoc/core.py
+-rw-r--r--   0        0        0    11949 1970-01-01 00:00:00.000000 sphinx_nested_apidoc-1.2.3/PKG-INFO
```

### Comparing `sphinx_nested_apidoc-1.2.2/LICENSE` & `sphinx_nested_apidoc-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_nested_apidoc-1.2.2/README.rst` & `sphinx_nested_apidoc-1.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_nested_apidoc-1.2.2/pyproject.toml` & `sphinx_nested_apidoc-1.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinx-nested-apidoc"
-version = "1.2.2"
+version = "1.2.3"
 description = "sphinx-nested-apidoc: When flattened is not enough"
 authors = ["Arunanshu Biswas <mydellpc07@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 scripts = {sphinx-nested-apidoc = "sphinx_nested_apidoc.__main__:main"}
 repository = "https://github.com/arunanshub/sphinx-nested-apidoc"
 classifiers = [
@@ -20,66 +20,87 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/arunanshub/sphinx-nested-apidoc/issues"
 "Changelog" = "https://github.com/arunanshub/sphinx-nested-apidoc/blob/master/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-Sphinx = "^5.0.0"
+Sphinx = "^6.0.0"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^2.20.0"
+pre-commit = "^3.0.0"
+mypy = "^1.3.0"
 
 [tool.poetry.group.test.dependencies]
 hypothesis = "^6.56.1"
 pytest = "^7.1.3"
 pytest-xdist = "^3.0.0"
 pytest-cov = "^4.0.0"
 hypothesis-fspaths = "^0.1"
 pytest-mock = "^3.10.0"
 
 [tool.poetry.group.docs.dependencies]
 furo = ">=2022.9.29"
-sphinxext-opengraph = "^0.7.2"
+sphinxext-opengraph = "^0.8.0"
 sphinx-copybutton = "^0.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool]
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.2.2"
+version = "1.2.3"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 annotated_tag = true
 changelog_start_rev = "v0.3.1"
 version_files = [
     "pyproject.toml",
     "src/sphinx_nested_apidoc/__init__.py",
 ]
 
-[tool.pycln]
-all = true
-
 [tool.black]
 line-length = 79
 target-verson = "py38"
 
-[tool.isort]
-multi_line_output = 3
-include_trailing_comma = true
-line_length = 79
-profile = "black"
-add_imports = ["from __future__ import annotations"]
-
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING",
     "if typing.TYPE_CHECKING",
 ]
 
 [tool.pytest.ini_options]
 addopts = "--strict-config --strict-markers"
+
+[tool.ruff]
+line-length = 79
+target-version = "py38"
+exclude = [
+    "docs",
+    "tests",
+]
+ignore = [
+    "ANN101",
+    "ANN102",
+    "ANN401",
+    "B024",
+]
+select = [
+  "ANN",
+  "B",
+  "E",
+  "F",
+  "W",
+  "I",
+  "RET",
+  "EM",
+  "UP",
+  "C90",
+  "PTH",
+  "SIM",
+]
+
+[tool.ruff.isort]
+required-imports = ["from __future__ import annotations"]
```

### Comparing `sphinx_nested_apidoc-1.2.2/src/sphinx_nested_apidoc/__init__.py` & `sphinx_nested_apidoc-1.2.3/src/sphinx_nested_apidoc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 LOGGER_FORMAT = "[{levelname}: {filename}:{lineno}]: {message}"
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 
 
 def start_logging(
     level: int | str = logging.DEBUG,
     fmt: str = LOGGER_FORMAT,
 ) -> logging.Handler:
     """
```

### Comparing `sphinx_nested_apidoc-1.2.2/src/sphinx_nested_apidoc/__main__.py` & `sphinx_nested_apidoc-1.2.3/src/sphinx_nested_apidoc/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import argparse
 import logging
+from pathlib import Path
 
 from . import __version__, start_logging
 from .core import feed_sphinx_apidoc, rename_files, sanitize_path
 
 logger = logging.getLogger(__name__)
 
 APP_NAME = "sphinx-nested-apidoc"
@@ -128,18 +129,18 @@
     )
 
     if is_help:
         ps.exit(0)
 
     try:
         rename_files(
-            args.destdir,
-            args.module_path,
+            Path(args.destdir),
+            Path(args.module_path),
             package_name=(
-                sanitize_path(args.package_name)
+                sanitize_path(Path(args.package_name))
                 if args.package_name is not None
                 else None
             ),
             extension=args.suffix,
             implicit_namespaces=args.implicit_namespaces,
             dry_run=args.dry_run,
             force=args.force,
```

### Comparing `sphinx_nested_apidoc-1.2.2/src/sphinx_nested_apidoc/_ext.py` & `sphinx_nested_apidoc-1.2.3/src/sphinx_nested_apidoc/_ext.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from __future__ import annotations
 
 import typing
+from pathlib import Path
 
 if typing.TYPE_CHECKING:
     from sphinx.application import Sphinx
 
 from . import __version__
 from .core import feed_sphinx_apidoc, rename_files, sanitize_path
 
 
 def _execute(
-    package_dir: str,
-    doc_dir: str,
-    package_name: str | None,
+    package_dir: Path,
+    doc_dir: Path,
+    package_name: Path | None,
     suffix: str,
     excluded_files: typing.Iterable[str],
     module_first: bool,
     implicit_namespaces: bool,
 ) -> None:
     extra_args = []
     if module_first:
         extra_args.append("--module-first")
 
     feed_sphinx_apidoc(
-        doc_dir,
-        package_dir,
+        str(doc_dir),
+        str(package_dir),
         "--full",  # without `full` sphinx-build cannot find `index.rst`
         *extra_args,
         suffix=suffix,
         implicit_namespaces=implicit_namespaces,
     )
 
     rename_files(
@@ -40,24 +41,24 @@
         excluded_files=excluded_files,
     )
 
 
 def _builder_inited(app: Sphinx) -> None:
     config = app.config
     docdir = app.srcdir
-    package_dir = config.sphinx_nested_apidoc_package_dir
-    package_name = config.sphinx_nested_apidoc_package_name
-    suffix = config.sphinx_nested_apidoc_suffix
-    excluded_files = config.sphinx_nested_apidoc_excluded_files
-    module_first = config.sphinx_nested_apidoc_module_first
-    implicit_namespaces = config.sphinx_nested_apidoc_implicit_namespaces
+    package_dir: str = config.sphinx_nested_apidoc_package_dir
+    package_name: str = config.sphinx_nested_apidoc_package_name
+    suffix: str = config.sphinx_nested_apidoc_suffix
+    excluded_files: list[str] = config.sphinx_nested_apidoc_excluded_files
+    module_first: bool = config.sphinx_nested_apidoc_module_first
+    implicit_namespaces: bool = config.sphinx_nested_apidoc_implicit_namespaces
     _execute(
-        package_dir,
-        docdir,
-        package_name,
+        Path(package_dir),
+        Path(docdir),
+        Path(package_name),
         suffix,
         excluded_files,
         module_first,
         implicit_namespaces,
     )
```

### Comparing `sphinx_nested_apidoc-1.2.2/src/sphinx_nested_apidoc/core.py` & `sphinx_nested_apidoc-1.2.3/src/sphinx_nested_apidoc/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 from __future__ import annotations
 
 import functools
-import glob
 import logging
-import os
-import shutil
 import sys
 from contextlib import redirect_stdout
 from os import path
+from pathlib import Path
 from typing import Iterable, Iterator
 
 from sphinx.ext import apidoc
 
 logger = logging.getLogger(__name__)
 
 
 @functools.lru_cache
-def _safe_makedirs(name: str, mode: int = 0o755) -> bool:
+def _safe_makedirs(name: Path, mode: int = 0o755) -> bool:
     """
-    The same ``os.makedirs``, except that it caches its arguments and returns
+    The same ``Path.mkdir``, except that it caches its arguments and returns
     boolean instead of raising an exception.
 
     Args:
         name: The name of the directory to create.
         mode: The creation mode.
 
     Returns:
         ``True`` if directory is created, ``False`` otherwise.
     """
     try:
-        os.makedirs(name, mode, exist_ok=False)
+        name.mkdir(mode, True, False)
     except FileExistsError:
         return False
 
     logger.debug("Create directory %s", name)
     return True
 
 
@@ -43,37 +41,37 @@
     short_flag: str | None,
     flag: str,
 ) -> None:
     if cond and (flag not in arg or short_flag not in arg):
         arg.append(flag)
 
 
-def sanitize_path(p: str) -> str:
+def sanitize_path(path_: Path) -> Path:
     """
     Eliminates double slashes and relative path nastiness from the given path
     by treating them as relative to root path.
 
     Args:
-        p: A string representing the path to be sanitized.
+        path_: A string representing the path to be sanitized.
 
     Returns:
         Sanitized path as string.
 
     Note:
         On Windows, if the path contains a different drive letter, it will
         return an empty string.
     """
     try:
-        sanitized = path.relpath(path.join(path.sep, p), path.sep)
+        sanitized = (path.sep / path_).relative_to("/")
     except ValueError:
         # Windows issue: given path is a different drive. Since it is invalid
         # anyway, we return empty string.
-        return ""
+        return Path()
 
-    return "" if sanitized == "." else sanitized
+    return Path() if sanitized == "." else sanitized
 
 
 def feed_sphinx_apidoc(
     output_dir: str,
     module_path: str,
     *sphinx_arguments: str,
     implicit_namespaces: bool = False,
@@ -147,78 +145,77 @@
     with redirect_stdout(stdout):
         apidoc.main(arguments)
 
     return is_help
 
 
 def yield_source_files(
-    source_dir: str,
+    source_dir: Path,
     extension: str = "rst",
-) -> Iterator[str]:
+) -> Iterator[Path]:
     """Yields files from source directory that end with the given extension.
 
     Args:
         source_dir: The directory where the files are located.
         extension: The extension of the file, without the "." prefix.
 
     Yields:
         Path to file that end with ``extension``.
 
     Raises:
         ValueError: If extension starts with a ".".
     """
     if extension.startswith("."):
-        raise ValueError("extension must not start with '.'")
+        msg = "extension must not start with '.'"
+        raise ValueError(msg)
 
-    pattern = path.join(
-        path.normpath(source_dir),
-        f"*{path.extsep}{extension}",
+    yield from filter(
+        Path.is_file, source_dir.glob(f"*{path.extsep}{extension}")
     )
-    yield from filter(path.isfile, glob.iglob(pattern))
 
 
-def get_nested_dir_filename(sphinx_source_file: str) -> str:
+def get_nested_dir_filename(sphinx_source_file: Path) -> Path:
     """
     Convert a ``sphinx-apidoc`` based source file name into a nested directory
     based path.
 
     Args:
         sphinx_source_file: A ``sphinx-apidoc`` generated file.
-        dest_dir: The destination directory where the new fill will be stored.
 
     Returns:
         A string representing the path of the file.
 
     Note:
         It does not handle the case where the source file is actually an index
-        for a module, ie. It does not rename "a.b.module.rst" to
+        for a module, i.e. It does not rename "a.b.module.rst" to
         "some/path/a/b/module/index.rst". Use
         :py:func:`get_destination_filename` for that.
     """
-    src_filename = path.basename(sphinx_source_file)
-    src_filename, ext = path.splitext(src_filename)
-    return src_filename.replace(".", path.sep) + ext
+    return Path(
+        sphinx_source_file.stem.replace(".", path.sep)
+        + sphinx_source_file.suffix
+    )
 
 
 @functools.lru_cache
-def is_packagedir(directory: str) -> bool:
+def is_packagedir(directory: Path) -> bool:
     """Checks if given directory is a package.
 
     This function caches its input to improve performance.
     """
-    return any("__init__" in name for name in os.listdir(directory))
+    return any(directory.glob("__init__*"))
 
 
 def get_destination_filename(
-    sphinx_source_file: str,
-    package_dir: str,
+    sphinx_source_file: Path,
+    package_dir: Path,
     extension: str = "rst",
     implicit_namespaces: bool = False,
-    package_name: str | None = None,
-) -> str:
+    package_name: Path | None = None,
+) -> Path:
     """
     Convert a ``sphinx-apidoc`` generated source file name into a nested
     directory based path, and rename to "index" files where necessary.
 
     Args:
         sphinx_source_file: Path to the ``sphinx-apidoc`` generated file.
         package_dir:
@@ -233,44 +230,40 @@
             ``docs/myproj/a/b/c.rst`` to ``docs/newname/a/b/c.rst``, where
             ``newname`` is the new name of the directory. If ``None``, the name
             is derived from ``package_dir`` and sphinx source file.
 
     Returns:
         A string representing the path of the file.
     """
-    package_dir = path.normpath(package_dir)
-
-    # determine the source dir component that will be used to derive the
-    # package directory from the sphinx-apidoc generated files.
     if is_packagedir(package_dir) or implicit_namespaces:
-        root_module_name = path.basename(package_dir)
-        source_dir_component = package_dir.rsplit(root_module_name, 1)[0]
+        # /some/path/src => /some/path
+        source_dir_component = package_dir.parent
     else:
+        # /some/path/src/package remains same
         source_dir_component = package_dir
 
-    nested_dir_path = dest_name = get_nested_dir_filename(sphinx_source_file)
-    # determine the original directory path
-    package_dir_path = path.splitext(nested_dir_path)[0]
-    # check whether the package directory exists
-    if path.exists(path.join(source_dir_component, package_dir_path)):
-        dest_name = path.join(
-            package_dir_path,
-            f"index{path.extsep}{extension}",
-        )
+    # package.a.b.rst => package/a/b.rst
+    dest_name = get_nested_dir_filename(sphinx_source_file)
+    # package/a/b.rst => package/a/b
+    package_dir_path = dest_name.with_suffix("")
+    # does /some/path/src/package/a/b exist?
+    if (source_dir_component / package_dir_path).exists():
+        # package/a/b => package/a/b/index.rst
+        dest_name = package_dir_path / f"index{path.extsep}{extension}"
 
-    # "docs/package/b/c/d.rst" => "docs/renamed/b/c/d.rst"
+    # package/a/b.rst => newname/a/b.rst
     if package_name is not None:
-        dest_name = path.join(package_name, dest_name.split(path.sep, 1)[-1])
+        dest_name = package_name / str(dest_name).split(path.sep, 1)[-1]
     return dest_name
 
 
 def rename_files(
-    sphinx_source_dir: str,
-    package_dir: str,
-    package_name: str | None = None,
+    sphinx_source_dir: Path,
+    package_dir: Path,
+    package_name: Path | None = None,
     extension: str = "rst",
     implicit_namespaces: bool = False,
     dry_run: bool = False,
     force: bool = False,
     excluded_files: Iterable[str] = ("index", "modules"),
 ) -> None:
     """
@@ -298,40 +291,40 @@
             Name of files (**without extension**) that should not be
             renamed/modified. By default, it excludes ``index`` and
             ``modules``.
     """
     for source_file in yield_source_files(sphinx_source_dir, extension):
         # ignore `index` and `modules` files by default. `modules` is generated
         # when `sphinx-apidoc --full` is not used.
-        # file_name: /a/b/c/docs/index.ext => index.ext => index
-        file_name = path.splitext(path.basename(source_file))[0]
+        # file_name: /a/b/c/docs/index.ext => index
+        file_name = source_file.stem
         if file_name in excluded_files:
             logger.debug("Skipping excluded file: %s", source_file)
             continue
 
         nested_dir_path = get_destination_filename(
             source_file,
             package_dir,
             extension,
             implicit_namespaces,
             package_name,
         )
-        dest_path = path.join(sphinx_source_dir, nested_dir_path)
-        dest_dir = path.split(dest_path)[0]
+        dest_path = sphinx_source_dir / nested_dir_path
+        dest_dir = dest_path.parent
 
         if dry_run:
             logger.info("%s would be changed to %s", source_file, dest_path)
             continue
 
         # create the directories.
         # NOTE: We can create the directories beforehand by filtering out the
         # dirs from the destination filename.
         if not _safe_makedirs(dest_dir, mode=0o755):
             logger.debug("makedirs: %s already exists", dest_dir)
 
-        if path.exists(dest_path) and not force:
-            os.remove(source_file)  # remove leftover source files.
+        if dest_path.exists() and not force:
+            source_file.unlink()  # remove leftover source files.
             logger.warning("%s already exists. Skipping.", dest_path)
             continue
 
-        shutil.move(source_file, dest_path)
+        source_file.rename(dest_path)
         logger.info("%s -> %s", source_file, dest_path)
```

### Comparing `sphinx_nested_apidoc-1.2.2/setup.py` & `sphinx_nested_apidoc-1.2.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,331 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: sphinx-nested-apidoc
+Version: 1.2.3
+Summary: sphinx-nested-apidoc: When flattened is not enough
+Home-page: https://github.com/arunanshub/sphinx-nested-apidoc
+License: MIT
+Author: Arunanshu Biswas
+Author-email: mydellpc07@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Documentation :: Sphinx
+Requires-Dist: Sphinx (>=6.0.0,<7.0.0)
+Project-URL: Bug Tracker, https://github.com/arunanshub/sphinx-nested-apidoc/issues
+Project-URL: Changelog, https://github.com/arunanshub/sphinx-nested-apidoc/blob/master/CHANGELOG.md
+Project-URL: Repository, https://github.com/arunanshub/sphinx-nested-apidoc
+Description-Content-Type: text/x-rst
 
-package_dir = \
-{'': 'src'}
+sphinx-nested-apidoc
+====================
 
-packages = \
-['sphinx_nested_apidoc']
+When flattened is not enough.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Sphinx>=5.0.0,<6.0.0']
-
-entry_points = \
-{'console_scripts': ['sphinx-nested-apidoc = '
-                     'sphinx_nested_apidoc.__main__:main']}
-
-setup_kwargs = {
-    'name': 'sphinx-nested-apidoc',
-    'version': '1.2.2',
-    'description': 'sphinx-nested-apidoc: When flattened is not enough',
-    'long_description': 'sphinx-nested-apidoc\n====================\n\nWhen flattened is not enough.\n\n.. image:: https://github.com/arunanshub/sphinx-nested-apidoc/actions/workflows/ci.yml/badge.svg\n   :alt: CI\n   :target: https://github.com/arunanshub/sphinx-nested-apidoc/actions/workflows/ci.yml\n\n.. image:: https://coveralls.io/repos/github/arunanshub/sphinx-nested-apidoc/badge.svg?branch=master\n   :target: https://coveralls.io/github/arunanshub/sphinx-nested-apidoc?branch=master\n   :alt: Coverage\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :alt: Black\n   :target: https://github.com/psf/black\n\n.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336\n   :alt: isort\n   :target: https://pycqa.github.io/isort\n\n.. image:: https://img.shields.io/pypi/pyversions/sphinx-nested-apidoc\n   :target: https://pypi.org/project/sphinx-nested-apidoc\n   :alt: PyPI - Python Version\n\n.. image:: https://readthedocs.org/projects/sphinx-nested-apidoc/badge/?version=latest\n   :target: https://sphinx-nested-apidoc.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n\nInstallation\n++++++++++++\n\nUse ``pip`` or ``pip3`` to install ``sphinx-nested-apidoc``\n\n.. code-block:: bash\n\n   pip install sphinx-nested-apidoc\n\nor\n\n.. code-block:: bash\n\n   pip3 install sphinx-nested-apidoc\n\nIntroduction\n++++++++++++\n\n``sphinx-apidoc`` is a great tool for generating documentation, but it does not\nreplicate the directory structure of your package. ``sphinx-nested-apidoc``\naims to solve that problem.\n\nTutorial\n++++++++\n\nLet\'s say we have the following directory structure of our package:\n\n.. code-block:: text\n\n   mymodule/\n   ├── fruits/\n   │   ├── __init__.py\n   │   ├── mango.py\n   │   ├── pear.py\n   ├── animals/\n   │   ├── special/\n   │   │   ├── __init__.py\n   │   │   ├── doggo.py\n   │   │   └── catto.py\n   │   ├── __init__.py\n   │   ├── monke.py\n   │   └── chimp.py\n   ├── __init__.py\n   ├── base.py\n   └── exceptions.py\n\nAnd we want to generate documentation for this package in some directory ``docs/``.\n\nLet\'s see the difference.\n\nUsing ``sphinx-apidoc`` we get\n------------------------------\n\nWe use the following command:\n\n.. code-block:: bash\n\n   sphinx-apidoc -o docs/ mymodule/ -e\n\nIt generates:\n\n.. code-block:: text\n\n   docs/\n   ├── modules.rst\n   ├── mymodule.animals.chimp.rst\n   ├── mymodule.animals.monke.rst\n   ├── mymodule.animals.rst\n   ├── mymodule.animals.special.catto.rst\n   ├── mymodule.animals.special.doggo.rst\n   ├── mymodule.animals.special.rst\n   ├── mymodule.base.rst\n   ├── mymodule.exceptions.rst\n   ├── mymodule.fruits.mango.rst\n   ├── mymodule.fruits.pear.rst\n   ├── mymodule.fruits.rst\n   └── mymodule.rst\n\nThis is not very clean, obviously.\n\nUsing ``sphinx-nested-apidoc`` we get\n-------------------------------------\n\nWe use the following command:\n\n.. code-block:: bash\n\n   sphinx-nested-apidoc -o docs/ mymodule/\n\nIt generates:\n\n.. code-block:: text\n\n   docs/\n   ├── modules.rst\n   └── mymodule/\n       ├── animals/\n       │   ├── chimp.rst\n       │   ├── index.rst\n       │   ├── monke.rst\n       │   └── special/\n       │       ├── catto.rst\n       │       ├── doggo.rst\n       │       └── index.rst\n       ├── base.rst\n       ├── exceptions.rst\n       ├── fruits/\n       │   ├── mango.rst\n       │   ├── pear.rst\n       │   └── index.rst\n       └── index.rst\n\nLooks clean!\n\nWant to name the package something else?\n----------------------------------------\n\n.. code-block:: bash\n\n   sphinx-nested-apidoc --package-name src -o docs/ mymodule/\n\nIt generates:\n\n.. code-block:: text\n\n   docs/\n   ├── modules.rst\n   └── src/\n       ├── animals/\n       │   ├── chimp.rst\n       │   ├── index.rst\n       │   ├── monke.rst\n       │   └── special/\n       │       ├── catto.rst\n       │       ├── doggo.rst\n       │       └── index.rst\n       ├── base.rst\n       ├── exceptions.rst\n       ├── fruits/\n       │   ├── mango.rst\n       │   ├── pear.rst\n       │   └── index.rst\n       └── index.rst\n\nNote that ``mymodule`` has been renamed to ``src``.\n\nAs a Sphinx Extension\n---------------------\n\nYou can also use this as a sphinx extension.\n\nCreate a file called ``docs/conf.py`` and configure it like this:\n\n.. code-block:: python\n\n   # ...\n   extensions = [\n       "sphinx_nested_apidoc",\n       # ...other extensions\n   ]\n\n   # Name of the package directory.\n   sphinx_nested_apidoc_package_dir = "packagename"\n   # Name of the folder to put all the package documentation in. By default it is\n   # the name of the package itself.\n   sphinx_nested_apidoc_package_name = "src"\n   # ...\n\nAnd then run:\n\n.. code-block:: bash\n\n   sphinx-build docs docs/_build\n\nUsage Details\n+++++++++++++\n\n.. code-block:: text\n\n   usage: sphinx-nested-apidoc [-h] [-v | -q] [--version] [-f] [-n] -o DESTDIR\n                               [--package-name PACKAGE_NAME] [-s SUFFIX]\n                               [--implicit-namespaces]\n                               module_path ...\n\nGenerates nested directory from sphinx-apidoc\'s flattened files. It is simply a\nwrapper over sphinx-apidoc and you can pass additional arguments to it for\nextended configuration.\n\npositional arguments:\n   ``module_path``\n      Path to package to document.\n   ``...``\n      Commands and flags to supply to sphinx-apidoc. Note that some arguments\n      like `--dry-run` are ignored.\n\noptions:\n   -h, --help\n      show this help message and exit\n   -v, --verbose\n      Increase application verbosity. This option is repeatable and will\n      increase verbosity each time it is repeated. This option cannot be used\n      when -q/--quiet is used. (default: 3)\n   -q, --quiet\n      Disable logging. This option cannot be used when -v/--verbose is used.\n      (default: False)\n   --version\n      show program\'s version number and exit\n   -f, --force\n      Replace existing files. (default: False)\n   -n, --dry-run\n      Run the script without creating files (default: False)\n   -o, --output-dir\n      directory to place all output (default: None)\n   --package-name\n      Name of the directory to put the package documentation in. By default it\n      is the name of the package itself. (default: None)\n\n``sphinx-apidoc`` options:\n   -s, --suffix\n      file suffix (default: rst)\n   --implicit-namespaces\n      interpret module paths according to PEP-0420 implicit namespaces\n      specification (default: False)\n\nSphinx Extension Configuration\n++++++++++++++++++++++++++++++\n\nThe following configuration values are used:\n\n+-----------------------------------------------+------------------------------------------------------------------------------------------------------------------+-------------------------+------------+\n| Option Name                                   | Description                                                                                                      | Default                 | Required?  |\n+===============================================+==================================================================================================================+=========================+============+\n| ``sphinx_nested_apidoc_package_dir``          | This is where the package to document resides.                                                                   |                         | **YES**    |\n+-----------------------------------------------+------------------------------------------------------------------------------------------------------------------+-------------------------+------------+\n| ``sphinx_nested_apidoc_package_name``         | Name of the directory to put all the package documentation in. By default it is the name of the package itself.  | ``None``                |            |\n+-----------------------------------------------+------------------------------------------------------------------------------------------------------------------+-------------------------+------------+\n| ``sphinx_nested_apidoc_suffix``               | The suffix of the generated documentation files.                                                                 | ``rst``                 |            |\n+-----------------------------------------------+------------------------------------------------------------------------------------------------------------------+-------------------------+------------+\n| ``sphinx_nested_apidoc_excluded_files``       | List of files (without extension) to exclude from modification/renaming.                                         | ``index``, ``modules``  |            |\n+-----------------------------------------------+------------------------------------------------------------------------------------------------------------------+-------------------------+------------+\n| ``sphinx_nested_apidoc_module_first``         | put module documentation before submodule documentation.                                                         | ``False``               |            |\n+-----------------------------------------------+------------------------------------------------------------------------------------------------------------------+-------------------------+------------+\n| ``sphinx_nested_apidoc_implicit_namespaces``  | interpret module paths according to PEP-0420 implicit namespaces specification.                                  | ``False``               |            |\n+-----------------------------------------------+------------------------------------------------------------------------------------------------------------------+-------------------------+------------+\n\nSome additional details\n+++++++++++++++++++++++\n\nWhat it does\n------------\n\n- As you saw earlier, it generates a nested directory from a flattened one.\n- Under the hood, it uses ``sphinx-apidoc``. More on this below.\n\nAs stated above, ``sphinx-nested-apidoc`` uses ``sphinx-apidoc`` internally.\nThis means, you can configure ``sphinx-apidoc`` from ``sphinx-nested-apidoc``.\nFor example:\n\n.. code-block:: bash\n\n   # You can pass arguments like this:\n   sphinx-nested-apidoc -o docs/ mymodule/ -- -M -F --ext-githubpages\n   # or you can simply omit the \'--\'.\n\nEverything after the required positional argument of ``sphinx-nested-apidoc``\nis passed to ``sphinx-apidoc``.\n\nWhat it does not do\n-------------------\n\n- It does not modify the contents of the file. It just renames (or moves) them.\n- It is not a standalone tool. It requires ``sphinx-apidoc`` for its work.\n\nLicense\n+++++++\n\n`MIT <https://choosealicense.com/licenses/mit/>`_\n',
-    'author': 'Arunanshu Biswas',
-    'author_email': 'mydellpc07@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/arunanshub/sphinx-nested-apidoc',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+.. image:: https://github.com/arunanshub/sphinx-nested-apidoc/actions/workflows/ci.yml/badge.svg
+   :alt: CI
+   :target: https://github.com/arunanshub/sphinx-nested-apidoc/actions/workflows/ci.yml
 
+.. image:: https://coveralls.io/repos/github/arunanshub/sphinx-nested-apidoc/badge.svg?branch=master
+   :target: https://coveralls.io/github/arunanshub/sphinx-nested-apidoc?branch=master
+   :alt: Coverage
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :alt: Black
+   :target: https://github.com/psf/black
+
+.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+   :alt: isort
+   :target: https://pycqa.github.io/isort
+
+.. image:: https://img.shields.io/pypi/pyversions/sphinx-nested-apidoc
+   :target: https://pypi.org/project/sphinx-nested-apidoc
+   :alt: PyPI - Python Version
+
+.. image:: https://readthedocs.org/projects/sphinx-nested-apidoc/badge/?version=latest
+   :target: https://sphinx-nested-apidoc.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
+
+Installation
+++++++++++++
+
+Use ``pip`` or ``pip3`` to install ``sphinx-nested-apidoc``
+
+.. code-block:: bash
+
+   pip install sphinx-nested-apidoc
+
+or
+
+.. code-block:: bash
+
+   pip3 install sphinx-nested-apidoc
+
+Introduction
+++++++++++++
+
+``sphinx-apidoc`` is a great tool for generating documentation, but it does not
+replicate the directory structure of your package. ``sphinx-nested-apidoc``
+aims to solve that problem.
+
+Tutorial
+++++++++
+
+Let's say we have the following directory structure of our package:
+
+.. code-block:: text
+
+   mymodule/
+   ├── fruits/
+   │   ├── __init__.py
+   │   ├── mango.py
+   │   ├── pear.py
+   ├── animals/
+   │   ├── special/
+   │   │   ├── __init__.py
+   │   │   ├── doggo.py
+   │   │   └── catto.py
+   │   ├── __init__.py
+   │   ├── monke.py
+   │   └── chimp.py
+   ├── __init__.py
+   ├── base.py
+   └── exceptions.py
+
+And we want to generate documentation for this package in some directory ``docs/``.
+
+Let's see the difference.
+
+Using ``sphinx-apidoc`` we get
+------------------------------
+
+We use the following command:
+
+.. code-block:: bash
+
+   sphinx-apidoc -o docs/ mymodule/ -e
+
+It generates:
+
+.. code-block:: text
+
+   docs/
+   ├── modules.rst
+   ├── mymodule.animals.chimp.rst
+   ├── mymodule.animals.monke.rst
+   ├── mymodule.animals.rst
+   ├── mymodule.animals.special.catto.rst
+   ├── mymodule.animals.special.doggo.rst
+   ├── mymodule.animals.special.rst
+   ├── mymodule.base.rst
+   ├── mymodule.exceptions.rst
+   ├── mymodule.fruits.mango.rst
+   ├── mymodule.fruits.pear.rst
+   ├── mymodule.fruits.rst
+   └── mymodule.rst
+
+This is not very clean, obviously.
+
+Using ``sphinx-nested-apidoc`` we get
+-------------------------------------
+
+We use the following command:
+
+.. code-block:: bash
+
+   sphinx-nested-apidoc -o docs/ mymodule/
+
+It generates:
+
+.. code-block:: text
+
+   docs/
+   ├── modules.rst
+   └── mymodule/
+       ├── animals/
+       │   ├── chimp.rst
+       │   ├── index.rst
+       │   ├── monke.rst
+       │   └── special/
+       │       ├── catto.rst
+       │       ├── doggo.rst
+       │       └── index.rst
+       ├── base.rst
+       ├── exceptions.rst
+       ├── fruits/
+       │   ├── mango.rst
+       │   ├── pear.rst
+       │   └── index.rst
+       └── index.rst
+
+Looks clean!
+
+Want to name the package something else?
+----------------------------------------
+
+.. code-block:: bash
+
+   sphinx-nested-apidoc --package-name src -o docs/ mymodule/
+
+It generates:
+
+.. code-block:: text
+
+   docs/
+   ├── modules.rst
+   └── src/
+       ├── animals/
+       │   ├── chimp.rst
+       │   ├── index.rst
+       │   ├── monke.rst
+       │   └── special/
+       │       ├── catto.rst
+       │       ├── doggo.rst
+       │       └── index.rst
+       ├── base.rst
+       ├── exceptions.rst
+       ├── fruits/
+       │   ├── mango.rst
+       │   ├── pear.rst
+       │   └── index.rst
+       └── index.rst
+
+Note that ``mymodule`` has been renamed to ``src``.
+
+As a Sphinx Extension
+---------------------
+
+You can also use this as a sphinx extension.
+
+Create a file called ``docs/conf.py`` and configure it like this:
+
+.. code-block:: python
+
+   # ...
+   extensions = [
+       "sphinx_nested_apidoc",
+       # ...other extensions
+   ]
+
+   # Name of the package directory.
+   sphinx_nested_apidoc_package_dir = "packagename"
+   # Name of the folder to put all the package documentation in. By default it is
+   # the name of the package itself.
+   sphinx_nested_apidoc_package_name = "src"
+   # ...
+
+And then run:
+
+.. code-block:: bash
+
+   sphinx-build docs docs/_build
+
+Usage Details
++++++++++++++
+
+.. code-block:: text
+
+   usage: sphinx-nested-apidoc [-h] [-v | -q] [--version] [-f] [-n] -o DESTDIR
+                               [--package-name PACKAGE_NAME] [-s SUFFIX]
+                               [--implicit-namespaces]
+                               module_path ...
+
+Generates nested directory from sphinx-apidoc's flattened files. It is simply a
+wrapper over sphinx-apidoc and you can pass additional arguments to it for
+extended configuration.
+
+positional arguments:
+   ``module_path``
+      Path to package to document.
+   ``...``
+      Commands and flags to supply to sphinx-apidoc. Note that some arguments
+      like `--dry-run` are ignored.
+
+options:
+   -h, --help
+      show this help message and exit
+   -v, --verbose
+      Increase application verbosity. This option is repeatable and will
+      increase verbosity each time it is repeated. This option cannot be used
+      when -q/--quiet is used. (default: 3)
+   -q, --quiet
+      Disable logging. This option cannot be used when -v/--verbose is used.
+      (default: False)
+   --version
+      show program's version number and exit
+   -f, --force
+      Replace existing files. (default: False)
+   -n, --dry-run
+      Run the script without creating files (default: False)
+   -o, --output-dir
+      directory to place all output (default: None)
+   --package-name
+      Name of the directory to put the package documentation in. By default it
+      is the name of the package itself. (default: None)
+
+``sphinx-apidoc`` options:
+   -s, --suffix
+      file suffix (default: rst)
+   --implicit-namespaces
+      interpret module paths according to PEP-0420 implicit namespaces
+      specification (default: False)
+
+Sphinx Extension Configuration
+++++++++++++++++++++++++++++++
+
+The following configuration values are used:
+
++-----------------------------------------------+------------------------------------------------------------------------------------------------------------------+-------------------------+------------+
+| Option Name                                   | Description                                                                                                      | Default                 | Required?  |
++===============================================+==================================================================================================================+=========================+============+
+| ``sphinx_nested_apidoc_package_dir``          | This is where the package to document resides.                                                                   |                         | **YES**    |
++-----------------------------------------------+------------------------------------------------------------------------------------------------------------------+-------------------------+------------+
+| ``sphinx_nested_apidoc_package_name``         | Name of the directory to put all the package documentation in. By default it is the name of the package itself.  | ``None``                |            |
++-----------------------------------------------+------------------------------------------------------------------------------------------------------------------+-------------------------+------------+
+| ``sphinx_nested_apidoc_suffix``               | The suffix of the generated documentation files.                                                                 | ``rst``                 |            |
++-----------------------------------------------+------------------------------------------------------------------------------------------------------------------+-------------------------+------------+
+| ``sphinx_nested_apidoc_excluded_files``       | List of files (without extension) to exclude from modification/renaming.                                         | ``index``, ``modules``  |            |
++-----------------------------------------------+------------------------------------------------------------------------------------------------------------------+-------------------------+------------+
+| ``sphinx_nested_apidoc_module_first``         | put module documentation before submodule documentation.                                                         | ``False``               |            |
++-----------------------------------------------+------------------------------------------------------------------------------------------------------------------+-------------------------+------------+
+| ``sphinx_nested_apidoc_implicit_namespaces``  | interpret module paths according to PEP-0420 implicit namespaces specification.                                  | ``False``               |            |
++-----------------------------------------------+------------------------------------------------------------------------------------------------------------------+-------------------------+------------+
+
+Some additional details
++++++++++++++++++++++++
+
+What it does
+------------
+
+- As you saw earlier, it generates a nested directory from a flattened one.
+- Under the hood, it uses ``sphinx-apidoc``. More on this below.
+
+As stated above, ``sphinx-nested-apidoc`` uses ``sphinx-apidoc`` internally.
+This means, you can configure ``sphinx-apidoc`` from ``sphinx-nested-apidoc``.
+For example:
+
+.. code-block:: bash
+
+   # You can pass arguments like this:
+   sphinx-nested-apidoc -o docs/ mymodule/ -- -M -F --ext-githubpages
+   # or you can simply omit the '--'.
+
+Everything after the required positional argument of ``sphinx-nested-apidoc``
+is passed to ``sphinx-apidoc``.
+
+What it does not do
+-------------------
+
+- It does not modify the contents of the file. It just renames (or moves) them.
+- It is not a standalone tool. It requires ``sphinx-apidoc`` for its work.
+
+License
++++++++
+
+`MIT <https://choosealicense.com/licenses/mit/>`_
 
-setup(**setup_kwargs)
```

