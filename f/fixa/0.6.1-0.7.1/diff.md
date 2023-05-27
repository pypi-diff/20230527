# Comparing `tmp/fixa-0.6.1.tar.gz` & `tmp/fixa-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixa-0.6.1.tar", last modified: Fri May 26 17:33:49 2023, max compression
+gzip compressed data, was "fixa-0.7.1.tar", last modified: Sat May 27 19:11:38 2023, max compression
```

## Comparing `fixa-0.6.1.tar` & `fixa-0.7.1.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 17:33:49.302509 fixa-0.6.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-06 00:03:13.000000 fixa-0.6.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1114 2023-05-06 00:03:13.000000 fixa-0.6.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      312 2023-05-06 00:03:13.000000 fixa-0.6.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-26 17:33:49.302368 fixa-0.6.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2986 2023-05-06 00:03:13.000000 fixa-0.6.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 17:33:49.298437 fixa-0.6.1/fixa/
--rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-05-06 00:03:13.000000 fixa-0.6.1/fixa/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-26 17:22:04.000000 fixa-0.6.1/fixa/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4137 2023-05-08 06:09:51.000000 fixa-0.6.1/fixa/better_enum.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      533 2023-05-06 03:13:06.000000 fixa-0.6.1/fixa/better_pathlib.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6675 2023-05-06 00:03:13.000000 fixa-0.6.1/fixa/binarysearch.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3225 2023-05-26 17:28:21.000000 fixa-0.6.1/fixa/build_dist.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1333 2023-05-06 03:12:23.000000 fixa-0.6.1/fixa/dataclass_dataframe.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 17:33:49.299376 fixa-0.6.1/fixa/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-06 00:03:13.000000 fixa-0.6.1/fixa/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2383 2023-05-06 03:09:12.000000 fixa-0.6.1/fixa/git_cli.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5877 2023-05-06 00:03:13.000000 fixa-0.6.1/fixa/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    12219 2023-05-06 01:55:53.000000 fixa-0.6.1/fixa/iterable.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-05-12 16:53:54.000000 fixa-0.6.1/fixa/nest_logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      469 2023-05-06 03:18:07.000000 fixa-0.6.1/fixa/os_platform.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-06 05:18:39.000000 fixa-0.6.1/fixa/pytest_cov_helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3145 2023-05-06 01:57:52.000000 fixa-0.6.1/fixa/rnd.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1933 2023-05-06 03:17:46.000000 fixa-0.6.1/fixa/runtime.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 17:33:49.299607 fixa-0.6.1/fixa/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      539 2023-05-06 05:18:39.000000 fixa-0.6.1/fixa/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4757 2023-05-06 00:03:13.000000 fixa-0.6.1/fixa/timer.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 17:33:49.299260 fixa-0.6.1/fixa.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-26 17:33:49.000000 fixa-0.6.1/fixa.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      923 2023-05-26 17:33:49.000000 fixa-0.6.1/fixa.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-26 17:33:49.000000 fixa-0.6.1/fixa.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-05-26 17:33:49.000000 fixa-0.6.1/fixa.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        5 2023-05-26 17:33:49.000000 fixa-0.6.1/fixa.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      706 2023-05-26 17:22:09.000000 fixa-0.6.1/pyproject.toml
--rw-r--r--   0 sanhehu    (501) staff       (20)     2541 2023-05-26 17:22:50.000000 fixa-0.6.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-05-06 00:03:13.000000 fixa-0.6.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-26 17:19:20.000000 fixa-0.6.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-06 00:03:13.000000 fixa-0.6.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-06 00:03:13.000000 fixa-0.6.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-26 17:33:49.302554 fixa-0.6.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7699 2023-05-06 00:03:13.000000 fixa-0.6.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 17:33:49.302088 fixa-0.6.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3858 2023-05-08 05:53:35.000000 fixa-0.6.1/tests/test_better_enum.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      663 2023-05-06 02:16:38.000000 fixa-0.6.1/tests/test_better_pathlib.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1633 2023-05-06 01:48:18.000000 fixa-0.6.1/tests/test_binarysearch.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      692 2023-05-06 01:42:50.000000 fixa-0.6.1/tests/test_dataclass_dataframe.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      740 2023-05-06 03:08:57.000000 fixa-0.6.1/tests/test_git_cli.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2178 2023-05-06 01:48:41.000000 fixa-0.6.1/tests/test_hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-05-06 01:48:59.000000 fixa-0.6.1/tests/test_import.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6529 2023-05-06 01:56:07.000000 fixa-0.6.1/tests/test_iterable.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4127 2023-05-12 03:29:46.000000 fixa-0.6.1/tests/test_nest_logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      661 2023-05-06 01:58:16.000000 fixa-0.6.1/tests/test_rnd.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3432 2023-05-06 02:03:21.000000 fixa-0.6.1/tests/test_timer.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 19:11:38.085145 fixa-0.7.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-06 00:03:13.000000 fixa-0.7.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1114 2023-05-06 00:03:13.000000 fixa-0.7.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      312 2023-05-06 00:03:13.000000 fixa-0.7.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-27 19:11:38.084988 fixa-0.7.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2986 2023-05-06 00:03:13.000000 fixa-0.7.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 19:11:38.062302 fixa-0.7.1/fixa/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-05-06 00:03:13.000000 fixa-0.7.1/fixa/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-27 19:11:06.000000 fixa-0.7.1/fixa/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4137 2023-05-08 06:09:51.000000 fixa-0.7.1/fixa/better_enum.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      650 2023-05-27 18:21:44.000000 fixa-0.7.1/fixa/better_pathlib.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6675 2023-05-06 00:03:13.000000 fixa-0.7.1/fixa/binarysearch.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3225 2023-05-26 17:28:21.000000 fixa-0.7.1/fixa/build_dist.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1333 2023-05-06 03:12:23.000000 fixa-0.7.1/fixa/dataclass_dataframe.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 19:11:38.081551 fixa-0.7.1/fixa/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-06 00:03:13.000000 fixa-0.7.1/fixa/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2998 2023-05-27 18:40:26.000000 fixa-0.7.1/fixa/git_cli.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-05-27 18:23:51.000000 fixa-0.7.1/fixa/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    12219 2023-05-06 01:55:53.000000 fixa-0.7.1/fixa/iterable.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-05-12 16:53:54.000000 fixa-0.7.1/fixa/nest_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       82 2023-05-27 18:41:51.000000 fixa-0.7.1/fixa/nested_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      469 2023-05-06 03:18:07.000000 fixa-0.7.1/fixa/os_platform.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-06 05:18:39.000000 fixa-0.7.1/fixa/pytest_cov_helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3145 2023-05-06 01:57:52.000000 fixa-0.7.1/fixa/rnd.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1933 2023-05-06 03:17:46.000000 fixa-0.7.1/fixa/runtime.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 19:11:38.081858 fixa-0.7.1/fixa/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      539 2023-05-06 05:18:39.000000 fixa-0.7.1/fixa/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4757 2023-05-06 00:03:13.000000 fixa-0.7.1/fixa/timer.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 19:11:38.063067 fixa-0.7.1/fixa.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-27 19:11:38.000000 fixa-0.7.1/fixa.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      945 2023-05-27 19:11:38.000000 fixa-0.7.1/fixa.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-27 19:11:38.000000 fixa-0.7.1/fixa.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-05-27 19:11:38.000000 fixa-0.7.1/fixa.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        5 2023-05-27 19:11:38.000000 fixa-0.7.1/fixa.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      706 2023-05-26 17:22:09.000000 fixa-0.7.1/pyproject.toml
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2889 2023-05-27 18:40:37.000000 fixa-0.7.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-05-06 00:03:13.000000 fixa-0.7.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-26 17:19:20.000000 fixa-0.7.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-06 00:03:13.000000 fixa-0.7.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-06 00:03:13.000000 fixa-0.7.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-27 19:11:38.085189 fixa-0.7.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7699 2023-05-06 00:03:13.000000 fixa-0.7.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 19:11:38.084690 fixa-0.7.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3858 2023-05-08 05:53:35.000000 fixa-0.7.1/tests/test_better_enum.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      758 2023-05-27 18:22:18.000000 fixa-0.7.1/tests/test_better_pathlib.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1633 2023-05-06 01:48:18.000000 fixa-0.7.1/tests/test_binarysearch.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      692 2023-05-06 01:42:50.000000 fixa-0.7.1/tests/test_dataclass_dataframe.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      926 2023-05-27 18:39:25.000000 fixa-0.7.1/tests/test_git_cli.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2892 2023-05-27 18:21:55.000000 fixa-0.7.1/tests/test_hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-05-06 01:48:59.000000 fixa-0.7.1/tests/test_import.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6529 2023-05-06 01:56:07.000000 fixa-0.7.1/tests/test_iterable.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4127 2023-05-12 03:29:46.000000 fixa-0.7.1/tests/test_nest_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      661 2023-05-06 01:58:16.000000 fixa-0.7.1/tests/test_rnd.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3432 2023-05-06 02:03:21.000000 fixa-0.7.1/tests/test_timer.py
```

### Comparing `fixa-0.6.1/LICENSE.txt` & `fixa-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/PKG-INFO` & `fixa-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fixa
-Version: 0.6.1
+Version: 0.7.1
 Summary: Like the Ikea FIXA, it is my toolbox to fix things.
 Home-page: https://github.com/MacHu-GWU/fixa-project
-Download-URL: https://pypi.python.org/pypi/fixa/0.6.1#downloads
+Download-URL: https://pypi.python.org/pypi/fixa/0.7.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `fixa-0.6.1/README.rst` & `fixa-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/fixa/better_enum.py` & `fixa-0.7.1/fixa/better_enum.py`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/fixa/binarysearch.py` & `fixa-0.7.1/fixa/binarysearch.py`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/fixa/build_dist.py` & `fixa-0.7.1/fixa/build_dist.py`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/fixa/dataclass_dataframe.py` & `fixa-0.7.1/fixa/dataclass_dataframe.py`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/fixa/git_cli.py` & `fixa-0.7.1/fixa/git_cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,27 +12,49 @@
 
 
 @contextlib.contextmanager
 def temp_cwd(path: T.Union[str, Path]):  # pragma: no cover
     """
     Temporarily set the current working directory (CWD) and automatically
     switch back when it's done.
+
+    Example:
+
+    .. code-block:: python
+
+        with temp_cwd(Path("/path/to/target/working/directory")):
+            # do something
     """
+    path = Path(path).absolute()
+    if not path.is_dir():
+        raise NotADirectoryError(f"{path} is not a dir!")
     cwd = os.getcwd()
     os.chdir(str(path))
     try:
         yield path
     finally:
         os.chdir(cwd)
 
 
 class GitCLIError(Exception):
     pass
 
 
+def locate_dir_repo(path: Path) -> Path:
+    """
+    Locate the directory of the git repository. Similar to the effect of
+    ``git rev-parse --show-toplevel``.
+    """
+    if path.joinpath(".git").exists():
+        return path
+    if path.parent == path:
+        raise FileNotFoundError("Cannot find the .git folder!")
+    return locate_dir_repo(path.parent)
+
+
 def get_git_branch_from_git_cli(dir_repo: T.Union[str, Path]) -> str:
     """
     Use ``git`` CLI to get the current git branch.
 
     Run:
 
     .. code-block:: bash
```

### Comparing `fixa-0.6.1/fixa/hashes.py` & `fixa-0.7.1/fixa/hashes.py`

 * *Files 24% similar despite different names*

```diff
@@ -217,9 +217,58 @@
             while True:
                 data = f.read(chunk_size)
                 if not data:
                     break
                 m.update(data)
         return self._digest(m, hexdigest)
 
+    def of_folder(
+        self,
+        abspath: T.Union[str, Path, T.Any],
+        algo: T.Optional[HashAlgoEnum] = None,
+        hexdigest: T.Optional[bool] = None,
+    ) -> str:
+        """
+        Return hash value of a folder. It is based on the concatenation of
+        the hash values of all files in the folder. The order of the files
+        are sorted by their paths.
+        """
+        path = Path(abspath)
+        if not path.is_dir():
+            raise NotADirectoryError(f"{path} is not a folder!")
+        hashes = list()
+        for p in sorted(path.glob("**/*"), key=lambda x: str(x)):
+            if p.is_file():
+                hashes.append(self.of_file(p, algo=algo, hexdigest=hexdigest))
+        return self.of_str(
+            s="".join(hashes),
+            algo=algo,
+            hexdigest=hexdigest,
+        )
+
+    def of_paths(
+        self,
+        paths: T.List[T.Union[str, Path, T.Any]],
+        algo: T.Optional[HashAlgoEnum] = None,
+        hexdigest: T.Optional[bool] = None,
+    ) -> str:
+        """
+        Return hash value of a list of paths. It is based on the concatenation of
+        the hash values of all files and folders.
+        """
+        hashes = list()
+        for path in paths:
+            path = Path(path)
+            if path.is_dir():
+                hashes.append(self.of_folder(path, algo=algo, hexdigest=hexdigest))
+            elif path.is_file():
+                hashes.append(self.of_file(path, algo=algo, hexdigest=hexdigest))
+            else:  # pragma: no cover
+                pass
+        return self.of_str(
+            s="".join(hashes),
+            algo=algo,
+            hexdigest=hexdigest,
+        )
+
 
 hashes = Hashes()
```

### Comparing `fixa-0.6.1/fixa/iterable.py` & `fixa-0.7.1/fixa/iterable.py`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/fixa/nest_logger.py` & `fixa-0.7.1/fixa/nest_logger.py`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/fixa/pytest_cov_helper.py` & `fixa-0.7.1/fixa/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/fixa/rnd.py` & `fixa-0.7.1/fixa/rnd.py`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/fixa/runtime.py` & `fixa-0.7.1/fixa/runtime.py`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/fixa/tests/__init__.py` & `fixa-0.7.1/fixa/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/fixa/timer.py` & `fixa-0.7.1/fixa/timer.py`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/fixa.egg-info/PKG-INFO` & `fixa-0.7.1/fixa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fixa
-Version: 0.6.1
+Version: 0.7.1
 Summary: Like the Ikea FIXA, it is my toolbox to fix things.
 Home-page: https://github.com/MacHu-GWU/fixa-project
-Download-URL: https://pypi.python.org/pypi/fixa/0.6.1#downloads
+Download-URL: https://pypi.python.org/pypi/fixa/0.7.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `fixa-0.6.1/fixa.egg-info/SOURCES.txt` & `fixa-0.7.1/fixa.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 fixa/binarysearch.py
 fixa/build_dist.py
 fixa/dataclass_dataframe.py
 fixa/git_cli.py
 fixa/hashes.py
 fixa/iterable.py
 fixa/nest_logger.py
+fixa/nested_logger.py
 fixa/os_platform.py
 fixa/pytest_cov_helper.py
 fixa/rnd.py
 fixa/runtime.py
 fixa/timer.py
 fixa.egg-info/PKG-INFO
 fixa.egg-info/SOURCES.txt
```

### Comparing `fixa-0.6.1/pyproject.toml` & `fixa-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/release-history.rst` & `fixa-0.7.1/release-history.rst`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,30 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.7.1 (2023-05-27)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- add ``hashes.Hashes.of_folder`` and ``hashes.Hashes.of_paths``.
+- add ``git_cli.locate_dir_repo``.
+
+**Minor Improvements**
+
+- add edge case handling for ``better_pathlib.temp_cwd``.
+
+**Bugfixes**
+
+**Miscellaneous**
+
+
 0.6.1 (2023-05-26)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - add ``build_dist`` module to build the source distribution of Python.
```

### Comparing `fixa-0.6.1/requirements-doc.txt` & `fixa-0.7.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/setup.py` & `fixa-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/tests/test_better_enum.py` & `fixa-0.7.1/tests/test_better_enum.py`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/tests/test_better_pathlib.py` & `fixa-0.7.1/tests/test_better_pathlib.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,12 +17,16 @@
     assert Path.cwd() != p
     with temp_cwd(p):
         assert Path.cwd() == p
         with pytest.raises(Exception):
             raise Exception()
     assert Path.cwd() != p
 
+    with pytest.raises(NotADirectoryError):
+        with temp_cwd(__file__):
+            pass
+
 
 if __name__ == "__main__":
     from fixa.tests import run_cov_test
 
     run_cov_test(__file__, "fixa.better_pathlib", preview=False)
```

### Comparing `fixa-0.6.1/tests/test_binarysearch.py` & `fixa-0.7.1/tests/test_binarysearch.py`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/tests/test_dataclass_dataframe.py` & `fixa-0.7.1/tests/test_dataclass_dataframe.py`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/tests/test_hashes.py` & `fixa-0.7.1/tests/test_hashes.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,14 +43,40 @@
 
     id1 = hashes.of_file(a_file)
     with open(a_file, "rb") as f:
         id2 = hashes.of_file_object(f)
     assert id1 == id2
 
 
+def test_hash_folder():
+    hashes.use_sha256().use_hexdigesst()
+
+    dir_project_root = Path(__file__).absolute().parent.parent
+    dir_fixa = dir_project_root / "fixa"
+    dir_tests = dir_project_root / "tests"
+    path_readme = dir_project_root / "README.rst"
+
+    with pytest.raises(NotADirectoryError):
+        hashes.of_folder(path_readme)
+
+    id1 = hashes.of_folder(dir_fixa)
+    id2 = hashes.of_folder(dir_fixa)
+    assert id1 == id2
+
+    id3 = hashes.of_folder(dir_tests)
+    id4 = hashes.of_folder(dir_tests)
+    assert id3 == id4
+
+    assert id1 != id3
+
+    id5 = hashes.of_paths([dir_fixa, dir_tests, path_readme])
+    id6 = hashes.of_paths([dir_fixa, dir_tests, path_readme])
+    assert id5 == id6
+
+
 def test_hash_anything():
     """
     This test may failed in different operation system.
     """
     hashes.use_sha256().use_hexdigesst()
 
     a_bytes = b"hello world"
```

### Comparing `fixa-0.6.1/tests/test_iterable.py` & `fixa-0.7.1/tests/test_iterable.py`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/tests/test_nest_logger.py` & `fixa-0.7.1/tests/test_nest_logger.py`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/tests/test_rnd.py` & `fixa-0.7.1/tests/test_rnd.py`

 * *Files identical despite different names*

### Comparing `fixa-0.6.1/tests/test_timer.py` & `fixa-0.7.1/tests/test_timer.py`

 * *Files identical despite different names*

