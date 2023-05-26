# Comparing `tmp/littlefs-python-0.4.0.tar.gz` & `tmp/littlefs-python-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "littlefs-python-0.4.0.tar", last modified: Tue Nov 15 23:03:31 2022, max compression
+gzip compressed data, was "littlefs-python-0.5.0.tar", last modified: Fri May 26 23:21:06 2023, max compression
```

## Comparing `littlefs-python-0.4.0.tar` & `littlefs-python-0.5.0.tar`

### file list

```diff
@@ -1,112 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.867162 littlefs-python-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.863162 littlefs-python-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.863162 littlefs-python-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1449 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5494 2022-11-15 23:03:31.867162 littlefs-python-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3868 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.863162 littlefs-python-0.4.0/ci/
--rwxr-xr-x   0 runner    (1001) docker     (121)      860 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/ci/build-wheels.sh
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/ci/download_release_files.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.863162 littlefs-python-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.863162 littlefs-python-0.4.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/docs/doc8.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.863162 littlefs-python-0.4.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     4344 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/docs/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.863162 littlefs-python-0.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/examples/mkfsimg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/examples/walk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.863162 littlefs-python-0.4.0/littlefs/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/.git
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.859162 littlefs-python-0.4.0/littlefs/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.863162 littlefs-python-0.4.0/littlefs/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/.github/workflows/post-release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     9209 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/.github/workflows/status.yml
--rw-r--r--   0 runner    (1001) docker     (121)    14511 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    96233 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/DESIGN.md
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     2137 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    10265 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    30716 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/SPEC.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.863162 littlefs-python-0.4.0/littlefs/bd/
--rw-r--r--   0 runner    (1001) docker     (121)     6635 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/bd/lfs_filebd.c
--rw-r--r--   0 runner    (1001) docker     (121)     1845 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/bd/lfs_filebd.h
--rw-r--r--   0 runner    (1001) docker     (121)     4882 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/bd/lfs_rambd.c
--rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/bd/lfs_rambd.h
--rw-r--r--   0 runner    (1001) docker     (121)    10229 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/bd/lfs_testbd.c
--rw-r--r--   0 runner    (1001) docker     (121)     3974 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/bd/lfs_testbd.h
--rw-r--r--   0 runner    (1001) docker     (121)   160700 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/lfs.c
--rw-r--r--   0 runner    (1001) docker     (121)    23096 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/lfs.h
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/lfs_util.c
--rw-r--r--   0 runner    (1001) docker     (121)     7233 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/lfs_util.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.863162 littlefs-python-0.4.0/littlefs/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     7644 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/scripts/code.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9706 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/scripts/coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11448 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/scripts/explode_asserts.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1864 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/scripts/prefix.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      858 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/scripts/readblock.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11347 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/scripts/readmdir.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6357 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/scripts/readtree.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    30736 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/scripts/test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.867162 littlefs-python-0.4.0/littlefs/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    21227 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/tests/test_alloc.toml
--rw-r--r--   0 runner    (1001) docker     (121)    11995 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/tests/test_attrs.toml
--rw-r--r--   0 runner    (1001) docker     (121)     7486 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/tests/test_badblocks.toml
--rw-r--r--   0 runner    (1001) docker     (121)    27874 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/tests/test_dirs.toml
--rw-r--r--   0 runner    (1001) docker     (121)    21933 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/tests/test_entries.toml
--rw-r--r--   0 runner    (1001) docker     (121)    10179 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/tests/test_evil.toml
--rw-r--r--   0 runner    (1001) docker     (121)    15554 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/tests/test_exhaustion.toml
--rw-r--r--   0 runner    (1001) docker     (121)    16158 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/tests/test_files.toml
--rw-r--r--   0 runner    (1001) docker     (121)     7720 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/tests/test_interspersed.toml
--rw-r--r--   0 runner    (1001) docker     (121)    69418 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/tests/test_move.toml
--rw-r--r--   0 runner    (1001) docker     (121)     4221 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/tests/test_orphans.toml
--rw-r--r--   0 runner    (1001) docker     (121)     9813 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/tests/test_paths.toml
--rw-r--r--   0 runner    (1001) docker     (121)    11149 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/tests/test_relocations.toml
--rw-r--r--   0 runner    (1001) docker     (121)    13029 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/tests/test_seek.toml
--rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/tests/test_superblocks.toml
--rw-r--r--   0 runner    (1001) docker     (121)    14895 2022-11-15 23:03:25.000000 littlefs-python-0.4.0/littlefs/tests/test_truncate.toml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-15 23:03:31.867162 littlefs-python-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1774 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.859162 littlefs-python-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.867162 littlefs-python-0.4.0/src/littlefs/
--rw-r--r--   0 runner    (1001) docker     (121)    12278 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/src/littlefs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2228 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/src/littlefs/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/src/littlefs/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)   666461 2022-11-15 23:03:31.000000 littlefs-python-0.4.0/src/littlefs/lfs.c
--rw-r--r--   0 runner    (1001) docker     (121)     5182 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/src/littlefs/lfs.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2809 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/src/littlefs/lfs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9951 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/src/littlefs/lfs.pyx
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/src/littlefs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.867162 littlefs-python-0.4.0/src/littlefs_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5494 2022-11-15 23:03:31.000000 littlefs-python-0.4.0/src/littlefs_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2273 2022-11-15 23:03:31.000000 littlefs-python-0.4.0/src/littlefs_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 23:03:31.000000 littlefs-python-0.4.0/src/littlefs_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 23:03:31.000000 littlefs-python-0.4.0/src/littlefs_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-15 23:03:31.000000 littlefs-python-0.4.0/src/littlefs_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.867162 littlefs-python-0.4.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:03:31.867162 littlefs-python-0.4.0/test/lfs/
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/test/lfs/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/test/lfs/test_dir_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3452 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/test/lfs/test_file_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/test/lfs/test_fs_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/test/test_directories.py
--rw-r--r--   0 runner    (1001) docker     (121)     5225 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/test/test_files.py
--rw-r--r--   0 runner    (1001) docker     (121)     2392 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/test/test_remove_rename.py
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-11-15 23:03:24.000000 littlefs-python-0.4.0/test/test_walk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.322197 littlefs-python-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.310197 littlefs-python-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.310197 littlefs-python-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-26 23:21:06.322197 littlefs-python-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.310197 littlefs-python-0.5.0/ci/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      860 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/ci/build-wheels.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/ci/download_release_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.310197 littlefs-python-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.310197 littlefs-python-0.5.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/docs/doc8.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.314197 littlefs-python-0.5.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/docs/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.314197 littlefs-python-0.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/examples/mkfsimg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/examples/walk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.314197 littlefs-python-0.5.0/littlefs/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/.git
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.310197 littlefs-python-0.5.0/littlefs/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.314197 littlefs-python-0.5.0/littlefs/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/.github/workflows/post-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/.github/workflows/status.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    26975 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    96233 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/DESIGN.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    33650 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/SPEC.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.314197 littlefs-python-0.5.0/littlefs/bd/
+-rw-r--r--   0 runner    (1001) docker     (123)    20342 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/bd/lfs_emubd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/bd/lfs_emubd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/bd/lfs_filebd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/bd/lfs_filebd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/bd/lfs_rambd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/bd/lfs_rambd.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.314197 littlefs-python-0.5.0/littlefs/benches/
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/benches/bench_dir.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/benches/bench_file.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/benches/bench_superblock.toml
+-rw-r--r--   0 runner    (1001) docker     (123)   184603 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/lfs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23801 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/lfs.h
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/lfs_util.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/lfs_util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.314197 littlefs-python-0.5.0/littlefs/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)    67872 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/runners/bench_runner.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/runners/bench_runner.h
+-rw-r--r--   0 runner    (1001) docker     (123)    91607 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/runners/test_runner.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/runners/test_runner.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.318197 littlefs-python-0.5.0/littlefs/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    52054 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/bench.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5401 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/changeprefix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23095 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/code.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27397 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/cov.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22943 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45193 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/perf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44308 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/perfbd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54030 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    41869 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/plotmpl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15011 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/prettyasserts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/readblock.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12631 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/readmdir.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6357 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/readtree.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24367 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/stack.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21064 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/structs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25393 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/summary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5275 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/tailpipe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1993 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/teepipe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54598 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31069 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/tracebd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8135 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.318197 littlefs-python-0.5.0/littlefs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    22638 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_alloc.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_attrs.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_badblocks.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_bd.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    41114 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_compat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    32864 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_dirs.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    22546 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_entries.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_evil.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_exhaustion.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    17120 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_files.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_interspersed.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    70817 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_move.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_orphans.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_paths.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_powerloss.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_relocations.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_seek.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_superblocks.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    17457 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_truncate.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 23:21:06.322197 littlefs-python-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.310197 littlefs-python-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.322197 littlefs-python-0.5.0/src/littlefs/
+-rw-r--r--   0 runner    (1001) docker     (123)    12278 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/src/littlefs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/src/littlefs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/src/littlefs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   667029 2023-05-26 23:21:06.000000 littlefs-python-0.5.0/src/littlefs/lfs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/src/littlefs/lfs.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/src/littlefs/lfs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/src/littlefs/lfs.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/src/littlefs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.322197 littlefs-python-0.5.0/src/littlefs_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-26 23:21:06.000000 littlefs-python-0.5.0/src/littlefs_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-26 23:21:06.000000 littlefs-python-0.5.0/src/littlefs_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 23:21:06.000000 littlefs-python-0.5.0/src/littlefs_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 23:21:06.000000 littlefs-python-0.5.0/src/littlefs_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 23:21:06.000000 littlefs-python-0.5.0/src/littlefs_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.322197 littlefs-python-0.5.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.322197 littlefs-python-0.5.0/test/lfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/test/lfs/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/test/lfs/test_dir_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/test/lfs/test_file_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/test/lfs/test_fs_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/test/test_directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/test/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/test/test_remove_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/test/test_walk.py
```

### Comparing `littlefs-python-0.4.0/.github/workflows/deploy.yml` & `littlefs-python-0.5.0/.github/workflows/deploy.yml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     steps:
       - uses: actions/checkout@v3
         with:
           submodules: 'recursive'
 
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.11.2
+        uses: pypa/cibuildwheel@v2.12.1
 
       - uses: actions/upload-artifact@v3
         with:
           path: ./wheelhouse/*.whl
 
   build_sdist:
     name: Build source distribution
@@ -49,11 +49,11 @@
     # if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags/')
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: artifact
           path: dist
       
-      - uses: pypa/gh-action-pypi-publish@v1.5.1
+      - uses: pypa/gh-action-pypi-publish@v1.8.4
         with:
           user: __token__
           password: ${{ secrets.pypi_api_token }}
```

### Comparing `littlefs-python-0.4.0/.github/workflows/run-tests.yml` & `littlefs-python-0.5.0/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/LICENSE` & `littlefs-python-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/PKG-INFO` & `littlefs-python-0.5.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,143 +1,159 @@
 Metadata-Version: 2.1
 Name: littlefs-python
-Version: 0.4.0
+Version: 0.5.0
 Summary: A python wrapper for littlefs
 Home-page: https://github.com/jrast/littlefs-python
 Author: Jürg Rast
 Author-email: juergr@gmail.com
 License: UNKNOWN
-Description: ===================
-        littlefs for Python
-        ===================
-        
-        .. image:: https://readthedocs.org/projects/littlefs-python/badge/?version=latest
-            :target: https://littlefs-python.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://badge.fury.io/py/littlefs-python.svg
-            :target: https://badge.fury.io/py/littlefs-python
-        
-        littlefs-python provides a thin wrapper around littlefs_, a filesystem targeted for
-        small embedded systems.
-        The wrapper provides a pythonic interface to the filesystem and allows the creation,
-        inspection and modification of the filesystem or individual files.
-        Even if this package uses Cython_, the goal is not to provide a high performance
-        implementation. Cython was chosen as an easy method is offered to generate the binding
-        and the littlefs library in one step.
-        
-        Quick Examples
-        ==============
-        Let's create a image ready to transfer to a flash memory using the pythonic interface:
-        
-        .. code:: python
-        
-            from littlefs import LittleFS
-        
-            # Initialize the File System according to your specifications
-            fs = LittleFS(block_size=512, block_count=256)
-        
-            # Open a file and write some content
-            with fs.open('first-file.txt', 'w') as fh:
-                fh.write('Some text to begin with\n')
-        
-            # Dump the filesystem content to a file
-            with open('FlashMemory.bin', 'wb') as fh:
-                fh.write(fs.context.buffer)
-        
-        The same can be done by using the more verbose C-Style API, which closely resembles the
-        steps which must be performed in C:
-        
-        .. code:: python
-        
-            from littlefs import lfs
-        
-            cfg = lfs.LFSConfig(block_size=512, block_count=256)
-            fs = lfs.LFSFilesystem()
-        
-            # Format and mount the filesystem
-            lfs.format(fs, cfg)
-            lfs.mount(fs, cfg)
-        
-            # Open a file and write some content
-            fh = lfs.file_open(fs, 'first-file.txt', 'w')
-            lfs.file_write(fs, fh, b'Some text to begin with\n')
-            lfs.file_close(fs, fh)
-        
-            # Dump the filesystem content to a file
-            with open('FlashMemory.bin', 'wb') as fh:
-                fh.write(cfg.user_context.buffer)
-        
-        
-        Installation
-        ============
-        
-        This is as simple as it can be::
-        
-            pip install littlefs-python
-        
-        At the moment wheels (which require no build) are provided for the following platforms,
-        on other platforms the source package is used and a compiler is required:
-        
-         - Linux: Python 3.6 - 3.10 / 32- & 64-bit
-         - Windows: Python 3.6 - 3.10 / 32- & 64-bit
-        
-        
-        Development Setup
-        =================
-        
-        Start by checking out the source repository of littlefs-python::
-        
-            git clone https://github.com/jrast/littlefs-python.git
-        
-        The source code for littlefs is included as a submodule which must be
-        checked out after the clone::
-        
-            cd <littlefs-python>
-            git submodule update --init
-        
-        this ensures that the correct version of littlefs_ is cloned into
-        the littlefs folder. As a next step install the dependencies and install
-        the package::
-        
-            pip install -r requirements.txt
-            pip install -e .
-        
-        .. note::
-            It's highly recommended to install the package in a virtual environment!
-        
-        
-        Development Hints
-        -----------------
-        
-        - Test should be run before commiting: `pytest test`
-        - Mypy is used for typechecking. Run it also on the tests to catch more issues:
-          `mypy src test test/lfs`
-        - Mypy stubs can be generated with `stubgen src`. This will create a `out` direcotry
-          containing the generated stub files.
-        
-        
-        Creating a new release
-        ======================
-        
-        - Make sure the master branch is in the state you want it.
-        - Create a tag with the new version number
-        - Wait until all builds are completed. A new release should be created
-          automatically on github.
-        - Build the source distribution with `python setup.py sdist`
-        - Download all assets (using `ci/download_release_files.py`)
-        - Upload to pypi using twine: `twine upload dist/*`
-        
-        
-        
-        .. _littlefs: https://github.com/littlefs-project/littlefs
-        .. _Cython: http://docs.cython.org/en/latest/index.html
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Filesystems
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+===================
+littlefs for Python
+===================
+
+.. image:: https://readthedocs.org/projects/littlefs-python/badge/?version=latest
+    :target: https://littlefs-python.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://badge.fury.io/py/littlefs-python.svg
+    :target: https://badge.fury.io/py/littlefs-python
+
+littlefs-python provides a thin wrapper around littlefs_, a filesystem targeted for
+small embedded systems.
+The wrapper provides a pythonic interface to the filesystem and allows the creation,
+inspection and modification of the filesystem or individual files.
+Even if this package uses Cython_, the goal is not to provide a high performance
+implementation. Cython was chosen as an easy method is offered to generate the binding
+and the littlefs library in one step.
+
+Quick Examples
+==============
+Let's create a image ready to transfer to a flash memory using the pythonic interface:
+
+.. code:: python
+
+    from littlefs import LittleFS
+
+    # Initialize the File System according to your specifications
+    fs = LittleFS(block_size=512, block_count=256)
+
+    # Open a file and write some content
+    with fs.open('first-file.txt', 'w') as fh:
+        fh.write('Some text to begin with\n')
+
+    # Dump the filesystem content to a file
+    with open('FlashMemory.bin', 'wb') as fh:
+        fh.write(fs.context.buffer)
+
+The same can be done by using the more verbose C-Style API, which closely resembles the
+steps which must be performed in C:
+
+.. code:: python
+
+    from littlefs import lfs
+
+    cfg = lfs.LFSConfig(block_size=512, block_count=256)
+    fs = lfs.LFSFilesystem()
+
+    # Format and mount the filesystem
+    lfs.format(fs, cfg)
+    lfs.mount(fs, cfg)
+
+    # Open a file and write some content
+    fh = lfs.file_open(fs, 'first-file.txt', 'w')
+    lfs.file_write(fs, fh, b'Some text to begin with\n')
+    lfs.file_close(fs, fh)
+
+    # Dump the filesystem content to a file
+    with open('FlashMemory.bin', 'wb') as fh:
+        fh.write(cfg.user_context.buffer)
+
+
+Installation
+============
+
+.. note::
+    As littlefs_ is bundled with the package you will need to install the correct version of
+    this package in successfully read or create images for your embedded system. If you start
+    from scratch the latest version is recommeded.
+
+    .. csv-table::
+        :header: "Package Version", "LittleFS Version", "LittleFS File System Version"
+
+        0.6.0, 2.6.1, 2.1
+        0.5.0, 2.4.1, 2.0
+        0.4.0, 2.2.1, 2.0
+
+
+This is as simple as it can be::
+
+    pip install littlefs-python
+
+At the moment wheels (which require no build) are provided for the following platforms,
+on other platforms the source package is used and a compiler is required:
+
+ - Linux: Python 3.6 - 3.10 / 32- & 64-bit
+ - Windows: Python 3.6 - 3.10 / 32- & 64-bit
+
+
+Development Setup
+=================
+
+Start by checking out the source repository of littlefs-python::
+
+    git clone https://github.com/jrast/littlefs-python.git
+
+The source code for littlefs is included as a submodule which must be
+checked out after the clone::
+
+    cd <littlefs-python>
+    git submodule update --init
+
+this ensures that the correct version of littlefs_ is cloned into
+the littlefs folder. As a next step install the dependencies and install
+the package::
+
+    pip install -r requirements.txt
+    pip install -e .
+
+.. note::
+    It's highly recommended to install the package in a virtual environment!
+
+
+Development Hints
+-----------------
+
+- Test should be run before commiting: `pytest test`
+- Mypy is used for typechecking. Run it also on the tests to catch more issues:
+  `mypy src test test/lfs`
+- Mypy stubs can be generated with `stubgen src`. This will create a `out` direcotry
+  containing the generated stub files.
+
+
+Creating a new release
+======================
+
+- Make sure the master branch is in the state you want it.
+- Create a tag with the new version number
+- Wait until all builds are completed. A new release should be created
+  automatically on github.
+- Build the source distribution with `python setup.py sdist`
+- Download all assets (using `ci/download_release_files.py`)
+- Upload to pypi using twine: `twine upload dist/*`
+
+
+
+.. _littlefs: https://github.com/littlefs-project/littlefs
+.. _Cython: http://docs.cython.org/en/latest/index.html
+
+
```

### Comparing `littlefs-python-0.4.0/README.rst` & `littlefs-python-0.5.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -59,14 +59,27 @@
     with open('FlashMemory.bin', 'wb') as fh:
         fh.write(cfg.user_context.buffer)
 
 
 Installation
 ============
 
+.. note::
+    As littlefs_ is bundled with the package you will need to install the correct version of
+    this package in successfully read or create images for your embedded system. If you start
+    from scratch the latest version is recommeded.
+
+    .. csv-table::
+        :header: "Package Version", "LittleFS Version", "LittleFS File System Version"
+
+        0.6.0, 2.6.1, 2.1
+        0.5.0, 2.4.1, 2.0
+        0.4.0, 2.2.1, 2.0
+
+
 This is as simple as it can be::
 
     pip install littlefs-python
 
 At the moment wheels (which require no build) are provided for the following platforms,
 on other platforms the source package is used and a compiler is required:
```

### Comparing `littlefs-python-0.4.0/ci/build-wheels.sh` & `littlefs-python-0.5.0/ci/build-wheels.sh`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/ci/download_release_files.py` & `littlefs-python-0.5.0/ci/download_release_files.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/docs/Makefile` & `littlefs-python-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/docs/conf.py` & `littlefs-python-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/docs/examples/index.rst` & `littlefs-python-0.5.0/docs/examples/index.rst`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/docs/make.bat` & `littlefs-python-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/docs/usage.rst` & `littlefs-python-0.5.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/examples/mkfsimg.py` & `littlefs-python-0.5.0/examples/mkfsimg.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/examples/walk.py` & `littlefs-python-0.5.0/examples/walk.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/littlefs/.github/workflows/post-release.yml` & `littlefs-python-0.5.0/littlefs/.github/workflows/post-release.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 name: post-release
 on:
   release:
     branches: [master]
     types: [released]
 
+defaults:
+  run:
+    shell: bash -euv -o pipefail {0}
+
 jobs:
   post-release:
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-22.04
     steps:
       # trigger post-release in dependency repo, this indirection allows the
       # dependency repo to be updated often without affecting this repo. At
       # the time of this comment, the dependency repo is responsible for
       # creating PRs for other dependent repos post-release.
       - name: trigger-post-release
         continue-on-error: true
         run: |
           curl -sS -X POST -H "authorization: token ${{secrets.BOT_TOKEN}}" \
             "$GITHUB_API_URL/repos/${{secrets.POST_RELEASE_REPO}}/dispatches" \
             -d "$(jq -n '{
               event_type: "post-release",
               client_payload: {
                 repo: env.GITHUB_REPOSITORY,
-                version: "${{github.event.release.tag_name}}"}}' \
-              | tee /dev/stderr)"
+                version: "${{github.event.release.tag_name}}",
+              },
+            }' | tee /dev/stderr)"
```

### Comparing `littlefs-python-0.4.0/littlefs/.github/workflows/release.yml` & `littlefs-python-0.5.0/littlefs/.github/workflows/release.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 name: release
 on:
   workflow_run:
     workflows: [test]
     branches: [master]
     types: [completed]
 
+defaults:
+  run:
+    shell: bash -euv -o pipefail {0}
+
 jobs:
   release:
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-22.04
 
     # need to manually check for a couple things
     # - tests passed?
     # - we are the most recent commit on master?
     if: ${{github.event.workflow_run.conclusion == 'success' &&
       github.event.workflow_run.head_sha == github.sha}}
 
@@ -27,16 +31,30 @@
 
       # try to get results from tests
       - uses: dawidd6/action-download-artifact@v2
         continue-on-error: true
         with:
           workflow: ${{github.event.workflow_run.name}}
           run_id: ${{github.event.workflow_run.id}}
-          name: results
-          path: results
+          name: sizes
+          path: sizes
+      - uses: dawidd6/action-download-artifact@v2
+        continue-on-error: true
+        with:
+          workflow: ${{github.event.workflow_run.name}}
+          run_id: ${{github.event.workflow_run.id}}
+          name: cov
+          path: cov
+      - uses: dawidd6/action-download-artifact@v2
+        continue-on-error: true
+        with:
+          workflow: ${{github.event.workflow_run.name}}
+          run_id: ${{github.event.workflow_run.id}}
+          name: bench
+          path: bench
 
       - name: find-version
         run: |
           # rip version from lfs.h
           LFS_VERSION="$(grep -o '^#define LFS_VERSION .*$' lfs.h \
             | awk '{print $3}')"
           LFS_VERSION_MAJOR="$((0xffff & ($LFS_VERSION >> 16)))"
@@ -64,106 +82,127 @@
         continue-on-error: true
         run: |
           LFS_PREV_VERSION="$(git describe --tags --abbrev=0 --match 'v*')"
           echo "LFS_PREV_VERSION=$LFS_PREV_VERSION"
           echo "LFS_PREV_VERSION=$LFS_PREV_VERSION" >> $GITHUB_ENV
 
       # try to find results from tests
-      - name: collect-results
+      - name: create-table
         run: |
           # previous results to compare against?
           [ -n "$LFS_PREV_VERSION" ] && curl -sS \
-            "$GITHUB_API_URL/repos/$GITHUB_REPOSITORY/`
-              `status/$LFS_PREV_VERSION" \
+            "$GITHUB_API_URL/repos/$GITHUB_REPOSITORY/status/$LFS_PREV_VERSION`
+              `?per_page=100" \
             | jq -re 'select(.sha != env.GITHUB_SHA) | .statuses[]' \
-            >> prev-results.json \
+            >> prev-status.json \
             || true
 
-          # unfortunately these each have their own format
-          [ -e results/code-thumb.csv ] && ( \
-            export PREV="$(jq -re '
-                  select(.context == "results / code").description
-                  | capture("Code size is (?<result>[0-9]+)").result' \
-                prev-results.json || echo 0)"
-            ./scripts/code.py -u results/code-thumb.csv -s | awk '
-              NR==2 {printf "Code size,%d B",$2}
-              NR==2 && ENVIRON["PREV"]+0 != 0 {
-                printf " (%+.1f%%)",100*($2-ENVIRON["PREV"])/ENVIRON["PREV"]}
-              NR==2 {printf "\n"}' \
-            >> results.csv)
-          [ -e results/code-thumb-readonly.csv ] && ( \
-            export PREV="$(jq -re '
-                  select(.context == "results / code (readonly)").description
-                  | capture("Code size is (?<result>[0-9]+)").result' \
-                prev-results.json || echo 0)"
-            ./scripts/code.py -u results/code-thumb-readonly.csv -s | awk '
-              NR==2 {printf "Code size<br/>(readonly),%d B",$2}
-              NR==2 && ENVIRON["PREV"]+0 != 0 {
-                printf " (%+.1f%%)",100*($2-ENVIRON["PREV"])/ENVIRON["PREV"]}
-              NR==2 {printf "\n"}' \
-            >> results.csv)
-          [ -e results/code-thumb-threadsafe.csv ] && ( \
-            export PREV="$(jq -re '
-                  select(.context == "results / code (threadsafe)").description
-                  | capture("Code size is (?<result>[0-9]+)").result' \
-                prev-results.json || echo 0)"
-            ./scripts/code.py -u results/code-thumb-threadsafe.csv -s | awk '
-              NR==2 {printf "Code size<br/>(threadsafe),%d B",$2}
-              NR==2 && ENVIRON["PREV"]+0 != 0 {
-                printf " (%+.1f%%)",100*($2-ENVIRON["PREV"])/ENVIRON["PREV"]}
-              NR==2 {printf "\n"}' \
-            >> results.csv)
-          [ -e results/code-thumb-migrate.csv ] && ( \
-            export PREV="$(jq -re '
-                  select(.context == "results / code (migrate)").description
-                  | capture("Code size is (?<result>[0-9]+)").result' \
-                prev-results.json || echo 0)"
-            ./scripts/code.py -u results/code-thumb-migrate.csv -s | awk '
-              NR==2 {printf "Code size<br/>(migrate),%d B",$2}
-              NR==2 && ENVIRON["PREV"]+0 != 0 {
-                printf " (%+.1f%%)",100*($2-ENVIRON["PREV"])/ENVIRON["PREV"]}
-              NR==2 {printf "\n"}' \
-            >> results.csv)
-          [ -e results/code-thumb-error-asserts.csv ] && ( \
-            export PREV="$(jq -re '
-                  select(.context == "results / code (error-asserts)").description
-                  | capture("Code size is (?<result>[0-9]+)").result' \
-                prev-results.json || echo 0)"
-            ./scripts/code.py -u results/code-thumb-error-asserts.csv -s | awk '
-              NR==2 {printf "Code size<br/>(error-asserts),%d B",$2}
-              NR==2 && ENVIRON["PREV"]+0 != 0 {
-                printf " (%+.1f%%)",100*($2-ENVIRON["PREV"])/ENVIRON["PREV"]}
-              NR==2 {printf "\n"}' \
-            >> results.csv)
-          [ -e results/coverage.csv ] && ( \
-            export PREV="$(jq -re '
-                  select(.context == "results / coverage").description
-                  | capture("Coverage is (?<result>[0-9\\.]+)").result' \
-                prev-results.json || echo 0)"
-            ./scripts/coverage.py -u results/coverage.csv -s | awk -F '[ /%]+' '
-              NR==2 {printf "Coverage,%.1f%% of %d lines",$4,$3}
-              NR==2 && ENVIRON["PREV"]+0 != 0 {
-                printf " (%+.1f%%)",$4-ENVIRON["PREV"]}
-              NR==2 {printf "\n"}' \
-            >> results.csv)
-
-          # transpose to GitHub table
-          [ -e results.csv ] || exit 0
-          awk -F ',' '
-            {label[NR]=$1; value[NR]=$2}
-            END {
-              for (r=1; r<=NR; r++) {printf "| %s ",label[r]}; printf "|\n";
-              for (r=1; r<=NR; r++) {printf "|:--"}; printf "|\n";
-              for (r=1; r<=NR; r++) {printf "| %s ",value[r]}; printf "|\n"}' \
-            results.csv > results.txt
-          echo "RESULTS:"
-          cat results.txt
+          # build table for GitHub
+          declare -A table
+
+          # sizes table
+          i=0
+          j=0
+          for c in "" readonly threadsafe migrate error-asserts
+          do
+            # per-config results
+            c_or_default=${c:-default}
+            c_camel=${c_or_default^}
+            table[$i,$j]=$c_camel
+            ((j+=1))
+
+            for s in code stack struct
+            do
+              f=sizes/thumb${c:+-$c}.$s.csv
+              [ -e $f ] && table[$i,$j]=$( \
+                export PREV="$(jq -re '
+                    select(.context == "'"sizes (thumb${c:+, $c}) / $s"'").description
+                    | capture("(?<prev>[0-9∞]+)").prev' \
+                  prev-status.json || echo 0)"
+                ./scripts/summary.py $f --max=stack_limit -Y \
+                  | awk '
+                    NR==2 {$1=0; printf "%s B",$NF}
+                    NR==2 && ENVIRON["PREV"]+0 != 0 {
+                      printf " (%+.1f%%)",100*($NF-ENVIRON["PREV"])/ENVIRON["PREV"]
+                    }' \
+                  | sed -e 's/ /\&nbsp;/g')
+              ((j+=1))
+            done
+            ((j=0, i+=1))
+          done
+
+          # coverage table
+          i=0
+          j=4
+          for s in lines branches
+          do
+            table[$i,$j]=${s^}
+            ((j+=1))
+
+            f=cov/cov.csv
+            [ -e $f ] && table[$i,$j]=$( \
+              export PREV="$(jq -re '
+                  select(.context == "'"cov / $s"'").description
+                  | capture("(?<prev_a>[0-9]+)/(?<prev_b>[0-9]+)")
+                  | 100*((.prev_a|tonumber) / (.prev_b|tonumber))' \
+                prev-status.json || echo 0)"
+              ./scripts/cov.py -u $f -f$s -Y \
+                | awk -F '[ /%]+' -v s=$s '
+                  NR==2 {$1=0; printf "%d/%d %s",$2,$3,s}
+                  NR==2 && ENVIRON["PREV"]+0 != 0 {
+                    printf " (%+.1f%%)",$4-ENVIRON["PREV"]
+                  }' \
+                | sed -e 's/ /\&nbsp;/g')
+            ((j=4, i+=1))
+          done
+
+          # benchmark table
+          i=3
+          j=4
+          for s in readed proged erased
+          do
+            table[$i,$j]=${s^}
+            ((j+=1))
+
+            f=bench/bench.csv
+            [ -e $f ] && table[$i,$j]=$( \
+              export PREV="$(jq -re '
+                  select(.context == "'"bench / $s"'").description
+                  | capture("(?<prev>[0-9]+)").prev' \
+                prev-status.json || echo 0)"
+              ./scripts/summary.py $f -f$s=bench_$s -Y \
+                | awk '
+                  NR==2 {$1=0; printf "%s B",$NF}
+                  NR==2 && ENVIRON["PREV"]+0 != 0 {
+                    printf " (%+.1f%%)",100*($NF-ENVIRON["PREV"])/ENVIRON["PREV"]
+                  }' \
+                | sed -e 's/ /\&nbsp;/g')
+            ((j=4, i+=1))
+          done
+
+          # build the actual table
+          echo "|   | Code | Stack | Structs |   | Coverage |" >> table.txt
+          echo "|:--|-----:|------:|--------:|:--|---------:|" >> table.txt
+          for ((i=0; i<6; i++))
+          do
+            echo -n "|" >> table.txt
+            for ((j=0; j<6; j++))
+            do
+              echo -n " " >> table.txt
+              [[ i -eq 2 && j -eq 5 ]] && echo -n "**Benchmarks**" >> table.txt
+              echo -n "${table[$i,$j]:-}" >> table.txt
+              echo -n " |" >> table.txt
+            done
+            echo >> table.txt
+          done
+
+          cat table.txt
 
       # find changes from history
-      - name: collect-changes
+      - name: create-changes
         run: |
           [ -n "$LFS_PREV_VERSION" ] || exit 0
           # use explicit link to github commit so that release notes can
           # be copied elsewhere
           git log "$LFS_PREV_VERSION.." \
             --grep='^Merge' --invert-grep \
             --format="format:[\`%h\`](`
@@ -179,15 +218,15 @@
           git branch "v$LFS_VERSION_MAJOR" HEAD
 
           # create major prefix branch
           git config user.name ${{secrets.BOT_USER}}
           git config user.email ${{secrets.BOT_EMAIL}}
           git fetch "https://github.com/$GITHUB_REPOSITORY.git" \
             "v$LFS_VERSION_MAJOR-prefix" || true
-          ./scripts/prefix.py "lfs$LFS_VERSION_MAJOR"
+          ./scripts/changeprefix.py --git "lfs" "lfs$LFS_VERSION_MAJOR"
           git branch "v$LFS_VERSION_MAJOR-prefix" $( \
             git commit-tree $(git write-tree) \
               $(git rev-parse --verify -q FETCH_HEAD | sed -e 's/^/-p /') \
               -p HEAD \
               -m "Generated v$LFS_VERSION_MAJOR prefixes")
           git reset --hard
 
@@ -197,19 +236,22 @@
             "v$LFS_VERSION_MAJOR-prefix"
 
       # build release notes
       - name: create-release
         run: |
           # create release and patch version tag (vN.N.N)
           # only draft if not a patch release
-          [ -e results.txt ] && export RESULTS="$(cat results.txt)"
-          [ -e changes.txt ] && export CHANGES="$(cat changes.txt)"
+          [ -e table.txt ] && cat table.txt >> release.txt
+          echo >> release.txt
+          [ -e changes.txt ] && cat changes.txt >> release.txt
+          cat release.txt
+
           curl -sS -X POST -H "authorization: token ${{secrets.BOT_TOKEN}}" \
             "$GITHUB_API_URL/repos/$GITHUB_REPOSITORY/releases" \
-            -d "$(jq -n '{
+            -d "$(jq -n --rawfile release release.txt '{
               tag_name: env.LFS_VERSION,
               name: env.LFS_VERSION | rtrimstr(".0"),
               target_commitish: "${{github.event.workflow_run.head_sha}}",
               draft: env.LFS_VERSION | endswith(".0"),
-              body: [env.RESULTS, env.CHANGES | select(.)] | join("\n\n")}' \
-              | tee /dev/stderr)"
+              body: $release,
+            }' | tee /dev/stderr)"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `littlefs-python-0.4.0/littlefs/DESIGN.md` & `littlefs-python-0.5.0/littlefs/DESIGN.md`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/littlefs/LICENSE.md` & `littlefs-python-0.5.0/littlefs/LICENSE.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+Copyright (c) 2022, The littlefs authors.  
 Copyright (c) 2017, Arm Limited. All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 -  Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `littlefs-python-0.4.0/littlefs/README.md` & `littlefs-python-0.5.0/littlefs/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -222,14 +222,21 @@
   want this, but it is handy for demos.  You can see it in action
   [here][littlefs-js-demo].
   
 - [littlefs-python] - A Python wrapper for littlefs. The project allows you
   to create images of the filesystem on your PC. Check if littlefs will fit
   your needs, create images for a later download to the target memory or
   inspect the content of a binary image of the target memory.
+  
+- [littlefs2-rust] - A Rust wrapper for littlefs. This project allows you
+  to use littlefs in a Rust-friendly API, reaping the benefits of Rust's memory
+  safety and other guarantees.
+
+- [littlefs-disk-img-viewer] - A memory-efficient web application for viewing
+  littlefs disk images in your web browser.
 
 - [mklfs] - A command line tool built by the [Lua RTOS] guys for making
   littlefs images from a host PC. Supports Windows, Mac OS, and Linux.
 
 - [Mbed OS] - The easiest way to get started with littlefs is to jump into Mbed
   which already has block device drivers for most forms of embedded storage.
   littlefs is available in Mbed OS as the [LittleFileSystem] class.
@@ -239,20 +246,26 @@
   likely outperform littlefs on small memories such as the internal flash on
   microcontrollers.
 
 - [Dhara] - An interesting NAND flash translation layer designed for small
   MCUs. It offers static wear-leveling and power-resilience with only a fixed
   _O(|address|)_ pointer structure stored on each block and in RAM.
 
+- [chamelon] - A pure-OCaml implementation of (most of) littlefs, designed for
+  use with the MirageOS library operating system project. It is interoperable
+  with the reference implementation, with some caveats.
 
 [BSD-3-Clause]: https://spdx.org/licenses/BSD-3-Clause.html
+[littlefs-disk-img-viewer]: https://github.com/tniessen/littlefs-disk-img-viewer
 [littlefs-fuse]: https://github.com/geky/littlefs-fuse
 [FUSE]: https://github.com/libfuse/libfuse
 [littlefs-js]: https://github.com/geky/littlefs-js
 [littlefs-js-demo]:http://littlefs.geky.net/demo.html
 [mklfs]: https://github.com/whitecatboard/Lua-RTOS-ESP32/tree/master/components/mklfs/src
 [Lua RTOS]: https://github.com/whitecatboard/Lua-RTOS-ESP32
 [Mbed OS]: https://github.com/armmbed/mbed-os
-[LittleFileSystem]: https://os.mbed.com/docs/mbed-os/v5.12/apis/littlefilesystem.html
+[LittleFileSystem]: https://os.mbed.com/docs/mbed-os/latest/apis/littlefilesystem.html
 [SPIFFS]: https://github.com/pellepl/spiffs
 [Dhara]: https://github.com/dlbeer/dhara
 [littlefs-python]: https://pypi.org/project/littlefs-python/
+[littlefs2-rust]: https://crates.io/crates/littlefs2
+[chamelon]: https://github.com/yomimono/chamelon
```

### Comparing `littlefs-python-0.4.0/littlefs/SPEC.md` & `littlefs-python-0.5.0/littlefs/SPEC.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## littlefs technical specification
 
-This is the technical specification of the little filesystem. This document
-covers the technical details of how the littlefs is stored on disk for
-introspection and tooling. This document assumes you are familiar with the
-design of the littlefs, for more info on how littlefs works check
-out [DESIGN.md](DESIGN.md).
+This is the technical specification of the little filesystem with on-disk
+version lfs2.1. This document covers the technical details of how the littlefs
+is stored on disk for introspection and tooling. This document assumes you are
+familiar with the design of the littlefs, for more info on how littlefs works
+check out [DESIGN.md](DESIGN.md).
 
 ```
    | | |     .---._____
   .-----.   |          |
 --|o    |---| littlefs |
 --|     |---|          |
   '-----'   '----------'
@@ -129,20 +129,14 @@
 |       data C      |                    |       data C      |      |
 |                   |                    |                   |    tag C
 |                   |                    |                   |
 |                   |                    |                   |
 '-------------------'                    '-------------------'
 ```
 
-One last thing to note before we get into the details around tag encoding. Each
-tag contains a valid bit used to indicate if the tag and containing commit is
-valid. This valid bit is the first bit found in the tag and the commit and can
-be used to tell if we've attempted to write to the remaining space in the
-block.
-
 Here's a more complete example of metadata block containing 4 entries:
 
 ```
   .---------------------------------------.
 .-|  revision count   |      tag ~A       |        \
 | |-------------------+-------------------|        |
 | |                 data A                |        |
@@ -187,14 +181,61 @@
 | '---------------------------------------'  ||||
 '---------------------------------------'    |||'- most recent A
                                              ||'-- most recent B
                                              |'--- most recent C
                                              '---- most recent D
 ```
 
+Two things to note before we get into the details around tag encoding:
+
+1. Each tag contains a valid bit used to indicate if the tag and containing
+   commit is valid. After XORing, this bit should always be zero.
+
+   At the end of each commit, the valid bit of the previous tag is XORed
+   with the lowest bit in the type field of the CRC tag. This allows
+   the CRC tag to force the next commit to fail the valid bit test if it
+   has not yet been written to.
+
+2. The valid bit alone is not enough info to know if the next commit has been
+   erased. We don't know the order bits will be programmed in a program block,
+   so it's possible that the next commit had an attempted program that left the
+   valid bit unchanged.
+
+   To ensure we only ever program erased bytes, each commit can contain an
+   optional forward-CRC (FCRC). An FCRC contains a checksum of some amount of
+   bytes in the next commit at the time it was erased.
+
+   ```
+   .-------------------. \      \
+   |  revision count   | |      |
+   |-------------------| |      |
+   |     metadata      | |      |
+   |                   | +---.  +-- current commit
+   |                   | |   |  |
+   |-------------------| |   |  |
+   |       FCRC       ---|-. |  |
+   |-------------------| / | |  |
+   |        CRC       -----|-'  /
+   |-------------------|   |
+   |      padding      |   |        padding (does't need CRC)
+   |                   |   |
+   |-------------------| \ |    \
+   |      erased?      | +-'    |
+   |         |         | |      +-- next commit
+   |         v         | /      |
+   |                   |        /
+   |                   |
+   '-------------------'
+   ```
+
+   If the FCRC is missing or the checksum does not match, we must assume a
+   commit was attempted but failed due to power-loss.
+
+   Note that end-of-block commits do not need an FCRC.
+
 ## Metadata tags
 
 So in littlefs, 32-bit tags describe every type of metadata. And this means
 _every_ type of metadata, including file entries, directory fields, and
 global state. Even the CRCs used to mark the end of commits get their own tag.
 
 Because of this, the tag format contains some densely packed information. Note
@@ -229,27 +270,27 @@
 
 1. **Valid bit (1-bit)** - Indicates if the tag is valid.
 
 2. **Type3 (11-bits)** - Type of the tag. This field is broken down further
    into a 3-bit abstract type and an 8-bit chunk field. Note that the value
    `0x000` is invalid and not assigned a type.
 
-3. **Type1 (3-bits)** - Abstract type of the tag. Groups the tags into
-   8 categories that facilitate bitmasked lookups.
+    1. **Type1 (3-bits)** - Abstract type of the tag. Groups the tags into
+       8 categories that facilitate bitmasked lookups.
 
-4. **Chunk (8-bits)** - Chunk field used for various purposes by the different
-   abstract types.  type1+chunk+id form a unique identifier for each tag in the
-   metadata block.
+    2. **Chunk (8-bits)** - Chunk field used for various purposes by the different
+       abstract types.  type1+chunk+id form a unique identifier for each tag in the
+       metadata block.
 
-5. **Id (10-bits)** - File id associated with the tag. Each file in a metadata
+3. **Id (10-bits)** - File id associated with the tag. Each file in a metadata
    block gets a unique id which is used to associate tags with that file. The
    special value `0x3ff` is used for any tags that are not associated with a
    file, such as directory and global metadata.
 
-6. **Length (10-bits)** - Length of the data in bytes. The special value
+4. **Length (10-bits)** - Length of the data in bytes. The special value
    `0x3ff` indicates that this tag has been deleted.
 
 ## Metadata types
 
 What follows is an exhaustive list of metadata in littlefs.
 
 ---
@@ -781,7 +822,45 @@
 2. **CRC (32-bits)** - CRC-32 with a polynomial of `0x04c11db7` initialized
    with `0xffffffff`.
 
 3. **Padding** - Padding to the next program-aligned boundary. No guarantees
    are made about the contents.
 
 ---
+#### `0x5ff` LFS_TYPE_FCRC
+
+Added in lfs2.1, the optional FCRC tag contains a checksum of some amount of
+bytes in the next commit at the time it was erased. This allows us to ensure
+that we only ever program erased bytes, even if a previous commit failed due
+to power-loss.
+
+When programming a commit, the FCRC size must be at least as large as the
+program block size. However, the program block is not saved on disk, and can
+change between mounts, so the FCRC size on disk may be different than the
+current program block size.
+
+If the FCRC is missing or the checksum does not match, we must assume a
+commit was attempted but failed due to power-loss.
+
+Layout of the FCRC tag:
+
+```
+        tag                          data
+[--      32      --][--      32      --|--      32      --]
+[1|- 11 -| 10 | 10 ][--      32      --|--      32      --]
+ ^    ^     ^    ^            ^- fcrc size       ^- fcrc
+ |    |     |    '- size (8)
+ |    |     '------ id (0x3ff)
+ |    '------------ type (0x5ff)
+ '----------------- valid bit
+```
+
+FCRC fields:
+
+1. **FCRC size (32-bits)** - Number of bytes after this commit's CRC tag's
+   padding to include in the FCRC.
+
+2. **FCRC (32-bits)** - CRC of the bytes after this commit's CRC tag's padding
+   when erased. Like the CRC tag, this uses a CRC-32 with a polynomial of
+   `0x04c11db7` initialized with `0xffffffff`.
+
+---
```

### Comparing `littlefs-python-0.4.0/littlefs/bd/lfs_filebd.c` & `littlefs-python-0.5.0/littlefs/bd/lfs_filebd.c`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,54 @@
 /*
  * Block device emulated in a file
  *
+ * Copyright (c) 2022, The littlefs authors.
  * Copyright (c) 2017, Arm Limited. All rights reserved.
  * SPDX-License-Identifier: BSD-3-Clause
  */
 #include "bd/lfs_filebd.h"
 
 #include <fcntl.h>
 #include <unistd.h>
 #include <errno.h>
 
-int lfs_filebd_createcfg(const struct lfs_config *cfg, const char *path,
-        const struct lfs_filebd_config *bdcfg) {
-    LFS_FILEBD_TRACE("lfs_filebd_createcfg(%p {.context=%p, "
+#ifdef _WIN32
+#include <windows.h>
+#endif
+
+int lfs_filebd_create(const struct lfs_config *cfg, const char *path) {
+    LFS_FILEBD_TRACE("lfs_filebd_create(%p {.context=%p, "
                 ".read=%p, .prog=%p, .erase=%p, .sync=%p, "
                 ".read_size=%"PRIu32", .prog_size=%"PRIu32", "
                 ".block_size=%"PRIu32", .block_count=%"PRIu32"}, "
-                "\"%s\", "
-                "%p {.erase_value=%"PRId32"})",
+                "\"%s\")",
             (void*)cfg, cfg->context,
             (void*)(uintptr_t)cfg->read, (void*)(uintptr_t)cfg->prog,
             (void*)(uintptr_t)cfg->erase, (void*)(uintptr_t)cfg->sync,
             cfg->read_size, cfg->prog_size, cfg->block_size, cfg->block_count,
             path, (void*)bdcfg, bdcfg->erase_value);
     lfs_filebd_t *bd = cfg->context;
-    bd->cfg = bdcfg;
 
     // open file
+    #ifdef _WIN32
+    bd->fd = open(path, O_RDWR | O_CREAT | O_BINARY, 0666);
+    #else
     bd->fd = open(path, O_RDWR | O_CREAT, 0666);
+    #endif
+
     if (bd->fd < 0) {
         int err = -errno;
-        LFS_FILEBD_TRACE("lfs_filebd_createcfg -> %d", err);
+        LFS_FILEBD_TRACE("lfs_filebd_create -> %d", err);
         return err;
     }
 
-    LFS_FILEBD_TRACE("lfs_filebd_createcfg -> %d", 0);
+    LFS_FILEBD_TRACE("lfs_filebd_create -> %d", 0);
     return 0;
 }
 
-int lfs_filebd_create(const struct lfs_config *cfg, const char *path) {
-    LFS_FILEBD_TRACE("lfs_filebd_create(%p {.context=%p, "
-                ".read=%p, .prog=%p, .erase=%p, .sync=%p, "
-                ".read_size=%"PRIu32", .prog_size=%"PRIu32", "
-                ".block_size=%"PRIu32", .block_count=%"PRIu32"}, "
-                "\"%s\")",
-            (void*)cfg, cfg->context,
-            (void*)(uintptr_t)cfg->read, (void*)(uintptr_t)cfg->prog,
-            (void*)(uintptr_t)cfg->erase, (void*)(uintptr_t)cfg->sync,
-            cfg->read_size, cfg->prog_size, cfg->block_size, cfg->block_count,
-            path);
-    static const struct lfs_filebd_config defaults = {.erase_value=-1};
-    int err = lfs_filebd_createcfg(cfg, path, &defaults);
-    LFS_FILEBD_TRACE("lfs_filebd_create -> %d", err);
-    return err;
-}
-
 int lfs_filebd_destroy(const struct lfs_config *cfg) {
     LFS_FILEBD_TRACE("lfs_filebd_destroy(%p)", (void*)cfg);
     lfs_filebd_t *bd = cfg->context;
     int err = close(bd->fd);
     if (err < 0) {
         err = -errno;
         LFS_FILEBD_TRACE("lfs_filebd_destroy -> %d", err);
@@ -72,22 +62,21 @@
         lfs_off_t off, void *buffer, lfs_size_t size) {
     LFS_FILEBD_TRACE("lfs_filebd_read(%p, "
                 "0x%"PRIx32", %"PRIu32", %p, %"PRIu32")",
             (void*)cfg, block, off, buffer, size);
     lfs_filebd_t *bd = cfg->context;
 
     // check if read is valid
+    LFS_ASSERT(block < cfg->block_count);
     LFS_ASSERT(off  % cfg->read_size == 0);
     LFS_ASSERT(size % cfg->read_size == 0);
-    LFS_ASSERT(block < cfg->block_count);
+    LFS_ASSERT(off+size <= cfg->block_size);
 
-    // zero for reproducability (in case file is truncated)
-    if (bd->cfg->erase_value != -1) {
-        memset(buffer, bd->cfg->erase_value, size);
-    }
+    // zero for reproducibility (in case file is truncated)
+    memset(buffer, 0, size);
 
     // read
     off_t res1 = lseek(bd->fd,
             (off_t)block*cfg->block_size + (off_t)off, SEEK_SET);
     if (res1 < 0) {
         int err = -errno;
         LFS_FILEBD_TRACE("lfs_filebd_read -> %d", err);
@@ -103,45 +92,24 @@
 
     LFS_FILEBD_TRACE("lfs_filebd_read -> %d", 0);
     return 0;
 }
 
 int lfs_filebd_prog(const struct lfs_config *cfg, lfs_block_t block,
         lfs_off_t off, const void *buffer, lfs_size_t size) {
-    LFS_FILEBD_TRACE("lfs_filebd_prog(%p, 0x%"PRIx32", %"PRIu32", %p, %"PRIu32")",
+    LFS_FILEBD_TRACE("lfs_filebd_prog(%p, "
+                "0x%"PRIx32", %"PRIu32", %p, %"PRIu32")",
             (void*)cfg, block, off, buffer, size);
     lfs_filebd_t *bd = cfg->context;
 
     // check if write is valid
+    LFS_ASSERT(block < cfg->block_count);
     LFS_ASSERT(off  % cfg->prog_size == 0);
     LFS_ASSERT(size % cfg->prog_size == 0);
-    LFS_ASSERT(block < cfg->block_count);
-
-    // check that data was erased? only needed for testing
-    if (bd->cfg->erase_value != -1) {
-        off_t res1 = lseek(bd->fd,
-                (off_t)block*cfg->block_size + (off_t)off, SEEK_SET);
-        if (res1 < 0) {
-            int err = -errno;
-            LFS_FILEBD_TRACE("lfs_filebd_prog -> %d", err);
-            return err;
-        }
-
-        for (lfs_off_t i = 0; i < size; i++) {
-            uint8_t c;
-            ssize_t res2 = read(bd->fd, &c, 1);
-            if (res2 < 0) {
-                int err = -errno;
-                LFS_FILEBD_TRACE("lfs_filebd_prog -> %d", err);
-                return err;
-            }
-
-            LFS_ASSERT(c == bd->cfg->erase_value);
-        }
-    }
+    LFS_ASSERT(off+size <= cfg->block_size);
 
     // program data
     off_t res1 = lseek(bd->fd,
             (off_t)block*cfg->block_size + (off_t)off, SEEK_SET);
     if (res1 < 0) {
         int err = -errno;
         LFS_FILEBD_TRACE("lfs_filebd_prog -> %d", err);
@@ -156,48 +124,37 @@
     }
 
     LFS_FILEBD_TRACE("lfs_filebd_prog -> %d", 0);
     return 0;
 }
 
 int lfs_filebd_erase(const struct lfs_config *cfg, lfs_block_t block) {
-    LFS_FILEBD_TRACE("lfs_filebd_erase(%p, 0x%"PRIx32")", (void*)cfg, block);
-    lfs_filebd_t *bd = cfg->context;
+    LFS_FILEBD_TRACE("lfs_filebd_erase(%p, 0x%"PRIx32" (%"PRIu32"))",
+            (void*)cfg, block, cfg->block_size);
 
     // check if erase is valid
     LFS_ASSERT(block < cfg->block_count);
 
-    // erase, only needed for testing
-    if (bd->cfg->erase_value != -1) {
-        off_t res1 = lseek(bd->fd, (off_t)block*cfg->block_size, SEEK_SET);
-        if (res1 < 0) {
-            int err = -errno;
-            LFS_FILEBD_TRACE("lfs_filebd_erase -> %d", err);
-            return err;
-        }
-
-        for (lfs_off_t i = 0; i < cfg->block_size; i++) {
-            ssize_t res2 = write(bd->fd, &(uint8_t){bd->cfg->erase_value}, 1);
-            if (res2 < 0) {
-                int err = -errno;
-                LFS_FILEBD_TRACE("lfs_filebd_erase -> %d", err);
-                return err;
-            }
-        }
-    }
+    // erase is a noop
+    (void)block;
 
     LFS_FILEBD_TRACE("lfs_filebd_erase -> %d", 0);
     return 0;
 }
 
 int lfs_filebd_sync(const struct lfs_config *cfg) {
     LFS_FILEBD_TRACE("lfs_filebd_sync(%p)", (void*)cfg);
+
     // file sync
     lfs_filebd_t *bd = cfg->context;
+    #ifdef _WIN32
+    int err = FlushFileBuffers((HANDLE) _get_osfhandle(bd->fd)) ? 0 : -1;
+    #else
     int err = fsync(bd->fd);
+    #endif
     if (err) {
         err = -errno;
         LFS_FILEBD_TRACE("lfs_filebd_sync -> %d", 0);
         return err;
     }
 
     LFS_FILEBD_TRACE("lfs_filebd_sync -> %d", 0);
```

### Comparing `littlefs-python-0.4.0/littlefs/bd/lfs_filebd.h` & `littlefs-python-0.5.0/littlefs/bd/lfs_rambd.h`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 /*
- * Block device emulated in a file
+ * Block device emulated in RAM
  *
+ * Copyright (c) 2022, The littlefs authors.
  * Copyright (c) 2017, Arm Limited. All rights reserved.
  * SPDX-License-Identifier: BSD-3-Clause
  */
-#ifndef LFS_FILEBD_H
-#define LFS_FILEBD_H
+#ifndef LFS_RAMBD_H
+#define LFS_RAMBD_H
 
 #include "lfs.h"
 #include "lfs_util.h"
 
 #ifdef __cplusplus
 extern "C"
 {
 #endif
 
 
 // Block device specific tracing
-#ifdef LFS_FILEBD_YES_TRACE
-#define LFS_FILEBD_TRACE(...) LFS_TRACE(__VA_ARGS__)
+#ifndef LFS_RAMBD_TRACE
+#ifdef LFS_RAMBD_YES_TRACE
+#define LFS_RAMBD_TRACE(...) LFS_TRACE(__VA_ARGS__)
 #else
-#define LFS_FILEBD_TRACE(...)
+#define LFS_RAMBD_TRACE(...)
+#endif
 #endif
 
-// filebd config (optional)
-struct lfs_filebd_config {
-    // 8-bit erase value to use for simulating erases. -1 does not simulate
-    // erases, which can speed up testing by avoiding all the extra block-device
-    // operations to store the erase value.
-    int32_t erase_value;
+// rambd config (optional)
+struct lfs_rambd_config {
+    // Optional statically allocated buffer for the block device.
+    void *buffer;
 };
 
-// filebd state
-typedef struct lfs_filebd {
-    int fd;
-    const struct lfs_filebd_config *cfg;
-} lfs_filebd_t;
+// rambd state
+typedef struct lfs_rambd {
+    uint8_t *buffer;
+    const struct lfs_rambd_config *cfg;
+} lfs_rambd_t;
 
 
-// Create a file block device using the geometry in lfs_config
-int lfs_filebd_create(const struct lfs_config *cfg, const char *path);
-int lfs_filebd_createcfg(const struct lfs_config *cfg, const char *path,
-        const struct lfs_filebd_config *bdcfg);
+// Create a RAM block device using the geometry in lfs_config
+int lfs_rambd_create(const struct lfs_config *cfg);
+int lfs_rambd_createcfg(const struct lfs_config *cfg,
+        const struct lfs_rambd_config *bdcfg);
 
 // Clean up memory associated with block device
-int lfs_filebd_destroy(const struct lfs_config *cfg);
+int lfs_rambd_destroy(const struct lfs_config *cfg);
 
 // Read a block
-int lfs_filebd_read(const struct lfs_config *cfg, lfs_block_t block,
+int lfs_rambd_read(const struct lfs_config *cfg, lfs_block_t block,
         lfs_off_t off, void *buffer, lfs_size_t size);
 
 // Program a block
 //
 // The block must have previously been erased.
-int lfs_filebd_prog(const struct lfs_config *cfg, lfs_block_t block,
+int lfs_rambd_prog(const struct lfs_config *cfg, lfs_block_t block,
         lfs_off_t off, const void *buffer, lfs_size_t size);
 
 // Erase a block
 //
 // A block must be erased before being programmed. The
 // state of an erased block is undefined.
-int lfs_filebd_erase(const struct lfs_config *cfg, lfs_block_t block);
+int lfs_rambd_erase(const struct lfs_config *cfg, lfs_block_t block);
 
 // Sync the block device
-int lfs_filebd_sync(const struct lfs_config *cfg);
+int lfs_rambd_sync(const struct lfs_config *cfg);
 
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #endif
```

### Comparing `littlefs-python-0.4.0/littlefs/bd/lfs_rambd.c` & `littlefs-python-0.5.0/littlefs/bd/lfs_rambd.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,59 @@
 /*
  * Block device emulated in RAM
  *
+ * Copyright (c) 2022, The littlefs authors.
  * Copyright (c) 2017, Arm Limited. All rights reserved.
  * SPDX-License-Identifier: BSD-3-Clause
  */
 #include "bd/lfs_rambd.h"
 
 int lfs_rambd_createcfg(const struct lfs_config *cfg,
         const struct lfs_rambd_config *bdcfg) {
     LFS_RAMBD_TRACE("lfs_rambd_createcfg(%p {.context=%p, "
                 ".read=%p, .prog=%p, .erase=%p, .sync=%p, "
                 ".read_size=%"PRIu32", .prog_size=%"PRIu32", "
                 ".block_size=%"PRIu32", .block_count=%"PRIu32"}, "
-                "%p {.erase_value=%"PRId32", .buffer=%p})",
+                "%p {.buffer=%p})",
             (void*)cfg, cfg->context,
             (void*)(uintptr_t)cfg->read, (void*)(uintptr_t)cfg->prog,
             (void*)(uintptr_t)cfg->erase, (void*)(uintptr_t)cfg->sync,
             cfg->read_size, cfg->prog_size, cfg->block_size, cfg->block_count,
-            (void*)bdcfg, bdcfg->erase_value, bdcfg->buffer);
+            (void*)bdcfg, bdcfg->buffer);
     lfs_rambd_t *bd = cfg->context;
     bd->cfg = bdcfg;
 
     // allocate buffer?
     if (bd->cfg->buffer) {
         bd->buffer = bd->cfg->buffer;
     } else {
         bd->buffer = lfs_malloc(cfg->block_size * cfg->block_count);
         if (!bd->buffer) {
             LFS_RAMBD_TRACE("lfs_rambd_createcfg -> %d", LFS_ERR_NOMEM);
             return LFS_ERR_NOMEM;
         }
     }
 
-    // zero for reproducability?
-    if (bd->cfg->erase_value != -1) {
-        memset(bd->buffer, bd->cfg->erase_value,
-                cfg->block_size * cfg->block_count);
-    }
+    // zero for reproducibility
+    memset(bd->buffer, 0, cfg->block_size * cfg->block_count);
 
     LFS_RAMBD_TRACE("lfs_rambd_createcfg -> %d", 0);
     return 0;
 }
 
 int lfs_rambd_create(const struct lfs_config *cfg) {
     LFS_RAMBD_TRACE("lfs_rambd_create(%p {.context=%p, "
                 ".read=%p, .prog=%p, .erase=%p, .sync=%p, "
                 ".read_size=%"PRIu32", .prog_size=%"PRIu32", "
                 ".block_size=%"PRIu32", .block_count=%"PRIu32"})",
             (void*)cfg, cfg->context,
             (void*)(uintptr_t)cfg->read, (void*)(uintptr_t)cfg->prog,
             (void*)(uintptr_t)cfg->erase, (void*)(uintptr_t)cfg->sync,
             cfg->read_size, cfg->prog_size, cfg->block_size, cfg->block_count);
-    static const struct lfs_rambd_config defaults = {.erase_value=-1};
+    static const struct lfs_rambd_config defaults = {0};
     int err = lfs_rambd_createcfg(cfg, &defaults);
     LFS_RAMBD_TRACE("lfs_rambd_create -> %d", err);
     return err;
 }
 
 int lfs_rambd_destroy(const struct lfs_config *cfg) {
     LFS_RAMBD_TRACE("lfs_rambd_destroy(%p)", (void*)cfg);
@@ -72,17 +70,18 @@
         lfs_off_t off, void *buffer, lfs_size_t size) {
     LFS_RAMBD_TRACE("lfs_rambd_read(%p, "
                 "0x%"PRIx32", %"PRIu32", %p, %"PRIu32")",
             (void*)cfg, block, off, buffer, size);
     lfs_rambd_t *bd = cfg->context;
 
     // check if read is valid
+    LFS_ASSERT(block < cfg->block_count);
     LFS_ASSERT(off  % cfg->read_size == 0);
     LFS_ASSERT(size % cfg->read_size == 0);
-    LFS_ASSERT(block < cfg->block_count);
+    LFS_ASSERT(off+size <= cfg->block_size);
 
     // read data
     memcpy(buffer, &bd->buffer[block*cfg->block_size + off], size);
 
     LFS_RAMBD_TRACE("lfs_rambd_read -> %d", 0);
     return 0;
 }
@@ -91,50 +90,42 @@
         lfs_off_t off, const void *buffer, lfs_size_t size) {
     LFS_RAMBD_TRACE("lfs_rambd_prog(%p, "
                 "0x%"PRIx32", %"PRIu32", %p, %"PRIu32")",
             (void*)cfg, block, off, buffer, size);
     lfs_rambd_t *bd = cfg->context;
 
     // check if write is valid
+    LFS_ASSERT(block < cfg->block_count);
     LFS_ASSERT(off  % cfg->prog_size == 0);
     LFS_ASSERT(size % cfg->prog_size == 0);
-    LFS_ASSERT(block < cfg->block_count);
-
-    // check that data was erased? only needed for testing
-    if (bd->cfg->erase_value != -1) {
-        for (lfs_off_t i = 0; i < size; i++) {
-            LFS_ASSERT(bd->buffer[block*cfg->block_size + off + i] ==
-                    bd->cfg->erase_value);
-        }
-    }
+    LFS_ASSERT(off+size <= cfg->block_size);
 
     // program data
     memcpy(&bd->buffer[block*cfg->block_size + off], buffer, size);
 
     LFS_RAMBD_TRACE("lfs_rambd_prog -> %d", 0);
     return 0;
 }
 
 int lfs_rambd_erase(const struct lfs_config *cfg, lfs_block_t block) {
-    LFS_RAMBD_TRACE("lfs_rambd_erase(%p, 0x%"PRIx32")", (void*)cfg, block);
-    lfs_rambd_t *bd = cfg->context;
+    LFS_RAMBD_TRACE("lfs_rambd_erase(%p, 0x%"PRIx32" (%"PRIu32"))",
+            (void*)cfg, block, cfg->block_size);
 
     // check if erase is valid
     LFS_ASSERT(block < cfg->block_count);
 
-    // erase, only needed for testing
-    if (bd->cfg->erase_value != -1) {
-        memset(&bd->buffer[block*cfg->block_size],
-                bd->cfg->erase_value, cfg->block_size);
-    }
+    // erase is a noop
+    (void)block;
 
     LFS_RAMBD_TRACE("lfs_rambd_erase -> %d", 0);
     return 0;
 }
 
 int lfs_rambd_sync(const struct lfs_config *cfg) {
     LFS_RAMBD_TRACE("lfs_rambd_sync(%p)", (void*)cfg);
-    // sync does nothing because we aren't backed by anything real
+
+    // sync is a noop
     (void)cfg;
+
     LFS_RAMBD_TRACE("lfs_rambd_sync -> %d", 0);
     return 0;
 }
```

### Comparing `littlefs-python-0.4.0/littlefs/lfs.c` & `littlefs-python-0.5.0/littlefs/lfs.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,37 @@
 /*
  * The little filesystem
  *
+ * Copyright (c) 2022, The littlefs authors.
  * Copyright (c) 2017, Arm Limited. All rights reserved.
  * SPDX-License-Identifier: BSD-3-Clause
  */
 #include "lfs.h"
 #include "lfs_util.h"
 
+
+// some constants used throughout the code
 #define LFS_BLOCK_NULL ((lfs_block_t)-1)
 #define LFS_BLOCK_INLINE ((lfs_block_t)-2)
 
+enum {
+    LFS_OK_RELOCATED = 1,
+    LFS_OK_DROPPED   = 2,
+    LFS_OK_ORPHANED  = 3,
+};
+
+enum {
+    LFS_CMP_EQ = 0,
+    LFS_CMP_LT = 1,
+    LFS_CMP_GT = 2,
+};
+
+
 /// Caching block device operations ///
+
 static inline void lfs_cache_drop(lfs_t *lfs, lfs_cache_t *rcache) {
     // do not zero, cheaper if cache is readonly or only going to be
     // written with identical data (during relocates)
     (void)lfs;
     rcache->block = LFS_BLOCK_NULL;
 }
 
@@ -103,47 +120,62 @@
             return err;
         }
     }
 
     return 0;
 }
 
-enum {
-    LFS_CMP_EQ = 0,
-    LFS_CMP_LT = 1,
-    LFS_CMP_GT = 2,
-};
-
 static int lfs_bd_cmp(lfs_t *lfs,
         const lfs_cache_t *pcache, lfs_cache_t *rcache, lfs_size_t hint,
         lfs_block_t block, lfs_off_t off,
         const void *buffer, lfs_size_t size) {
     const uint8_t *data = buffer;
     lfs_size_t diff = 0;
 
     for (lfs_off_t i = 0; i < size; i += diff) {
         uint8_t dat[8];
 
         diff = lfs_min(size-i, sizeof(dat));
-        int res = lfs_bd_read(lfs,
+        int err = lfs_bd_read(lfs,
                 pcache, rcache, hint-i,
                 block, off+i, &dat, diff);
-        if (res) {
-            return res;
+        if (err) {
+            return err;
         }
 
-        res = memcmp(dat, data + i, diff);
+        int res = memcmp(dat, data + i, diff);
         if (res) {
             return res < 0 ? LFS_CMP_LT : LFS_CMP_GT;
         }
     }
 
     return LFS_CMP_EQ;
 }
 
+static int lfs_bd_crc(lfs_t *lfs,
+        const lfs_cache_t *pcache, lfs_cache_t *rcache, lfs_size_t hint,
+        lfs_block_t block, lfs_off_t off, lfs_size_t size, uint32_t *crc) {
+    lfs_size_t diff = 0;
+
+    for (lfs_off_t i = 0; i < size; i += diff) {
+        uint8_t dat[8];
+        diff = lfs_min(size-i, sizeof(dat));
+        int err = lfs_bd_read(lfs,
+                pcache, rcache, hint-i,
+                block, off+i, &dat, diff);
+        if (err) {
+            return err;
+        }
+
+        *crc = lfs_crc(*crc, &dat, diff);
+    }
+
+    return 0;
+}
+
 #ifndef LFS_READONLY
 static int lfs_bd_flush(lfs_t *lfs,
         lfs_cache_t *pcache, lfs_cache_t *rcache, bool validate) {
     if (pcache->block != LFS_BLOCK_NULL && pcache->block != LFS_BLOCK_INLINE) {
         LFS_ASSERT(pcache->block < lfs->cfg->block_count);
         lfs_size_t diff = lfs_alignup(pcache->size, lfs->cfg->prog_size);
         int err = lfs->cfg->prog(lfs->cfg, pcache->block,
@@ -264,30 +296,32 @@
 static inline int lfs_pair_cmp(
         const lfs_block_t paira[2],
         const lfs_block_t pairb[2]) {
     return !(paira[0] == pairb[0] || paira[1] == pairb[1] ||
              paira[0] == pairb[1] || paira[1] == pairb[0]);
 }
 
-static inline bool lfs_pair_sync(
+static inline bool lfs_pair_issync(
         const lfs_block_t paira[2],
         const lfs_block_t pairb[2]) {
     return (paira[0] == pairb[0] && paira[1] == pairb[1]) ||
            (paira[0] == pairb[1] && paira[1] == pairb[0]);
 }
 
 static inline void lfs_pair_fromle32(lfs_block_t pair[2]) {
     pair[0] = lfs_fromle32(pair[0]);
     pair[1] = lfs_fromle32(pair[1]);
 }
 
+#ifndef LFS_READONLY
 static inline void lfs_pair_tole32(lfs_block_t pair[2]) {
     pair[0] = lfs_tole32(pair[0]);
     pair[1] = lfs_tole32(pair[1]);
 }
+#endif
 
 // operations on 32-bit entry tags
 typedef uint32_t lfs_tag_t;
 typedef int32_t lfs_stag_t;
 
 #define LFS_MKTAG(type, id, size) \
     (((lfs_tag_t)(type) << 20) | ((lfs_tag_t)(id) << 10) | (lfs_tag_t)(size))
@@ -306,14 +340,18 @@
     return ((int32_t)(tag << 22) >> 22) == -1;
 }
 
 static inline uint16_t lfs_tag_type1(lfs_tag_t tag) {
     return (tag & 0x70000000) >> 20;
 }
 
+static inline uint16_t lfs_tag_type2(lfs_tag_t tag) {
+    return (tag & 0x78000000) >> 20;
+}
+
 static inline uint16_t lfs_tag_type3(lfs_tag_t tag) {
     return (tag & 0x7ff00000) >> 20;
 }
 
 static inline uint8_t lfs_tag_chunk(lfs_tag_t tag) {
     return (tag & 0x0ff00000) >> 20;
 }
@@ -361,42 +399,68 @@
         if (((uint32_t*)a)[i] != 0) {
             return false;
         }
     }
     return true;
 }
 
+#ifndef LFS_READONLY
 static inline bool lfs_gstate_hasorphans(const lfs_gstate_t *a) {
     return lfs_tag_size(a->tag);
 }
 
 static inline uint8_t lfs_gstate_getorphans(const lfs_gstate_t *a) {
-    return lfs_tag_size(a->tag);
+    return lfs_tag_size(a->tag) & 0x1ff;
 }
 
 static inline bool lfs_gstate_hasmove(const lfs_gstate_t *a) {
     return lfs_tag_type1(a->tag);
 }
 
+static inline bool lfs_gstate_needssuperblock(const lfs_gstate_t *a) {
+    return lfs_tag_size(a->tag) >> 9;
+}
+#endif
+
 static inline bool lfs_gstate_hasmovehere(const lfs_gstate_t *a,
         const lfs_block_t *pair) {
     return lfs_tag_type1(a->tag) && lfs_pair_cmp(a->pair, pair) == 0;
 }
 
 static inline void lfs_gstate_fromle32(lfs_gstate_t *a) {
     a->tag     = lfs_fromle32(a->tag);
     a->pair[0] = lfs_fromle32(a->pair[0]);
     a->pair[1] = lfs_fromle32(a->pair[1]);
 }
 
+#ifndef LFS_READONLY
 static inline void lfs_gstate_tole32(lfs_gstate_t *a) {
     a->tag     = lfs_tole32(a->tag);
     a->pair[0] = lfs_tole32(a->pair[0]);
     a->pair[1] = lfs_tole32(a->pair[1]);
 }
+#endif
+
+// operations on forward-CRCs used to track erased state
+struct lfs_fcrc {
+    lfs_size_t size;
+    uint32_t crc;
+};
+
+static void lfs_fcrc_fromle32(struct lfs_fcrc *fcrc) {
+    fcrc->size = lfs_fromle32(fcrc->size);
+    fcrc->crc = lfs_fromle32(fcrc->crc);
+}
+
+#ifndef LFS_READONLY
+static void lfs_fcrc_tole32(struct lfs_fcrc *fcrc) {
+    fcrc->size = lfs_tole32(fcrc->size);
+    fcrc->crc = lfs_tole32(fcrc->crc);
+}
+#endif
 
 // other endianness operations
 static void lfs_ctz_fromle32(struct lfs_ctz *ctz) {
     ctz->head = lfs_fromle32(ctz->head);
     ctz->size = lfs_fromle32(ctz->size);
 }
 
@@ -412,22 +476,24 @@
     superblock->block_size  = lfs_fromle32(superblock->block_size);
     superblock->block_count = lfs_fromle32(superblock->block_count);
     superblock->name_max    = lfs_fromle32(superblock->name_max);
     superblock->file_max    = lfs_fromle32(superblock->file_max);
     superblock->attr_max    = lfs_fromle32(superblock->attr_max);
 }
 
+#ifndef LFS_READONLY
 static inline void lfs_superblock_tole32(lfs_superblock_t *superblock) {
     superblock->version     = lfs_tole32(superblock->version);
     superblock->block_size  = lfs_tole32(superblock->block_size);
     superblock->block_count = lfs_tole32(superblock->block_count);
     superblock->name_max    = lfs_tole32(superblock->name_max);
     superblock->file_max    = lfs_tole32(superblock->file_max);
     superblock->attr_max    = lfs_tole32(superblock->attr_max);
 }
+#endif
 
 #ifndef LFS_NO_ASSERT
 static bool lfs_mlist_isopen(struct lfs_mlist *head,
         struct lfs_mlist *node) {
     for (struct lfs_mlist **p = &head; *p; p = &(*p)->next) {
         if (*p == (struct lfs_mlist*)node) {
             return true;
@@ -456,40 +522,43 @@
 /// Internal operations predeclared here ///
 #ifndef LFS_READONLY
 static int lfs_dir_commit(lfs_t *lfs, lfs_mdir_t *dir,
         const struct lfs_mattr *attrs, int attrcount);
 static int lfs_dir_compact(lfs_t *lfs,
         lfs_mdir_t *dir, const struct lfs_mattr *attrs, int attrcount,
         lfs_mdir_t *source, uint16_t begin, uint16_t end);
-
+static lfs_ssize_t lfs_file_flushedwrite(lfs_t *lfs, lfs_file_t *file,
+        const void *buffer, lfs_size_t size);
 static lfs_ssize_t lfs_file_rawwrite(lfs_t *lfs, lfs_file_t *file,
         const void *buffer, lfs_size_t size);
 static int lfs_file_rawsync(lfs_t *lfs, lfs_file_t *file);
 static int lfs_file_outline(lfs_t *lfs, lfs_file_t *file);
 static int lfs_file_flush(lfs_t *lfs, lfs_file_t *file);
 
+static int lfs_fs_deorphan(lfs_t *lfs, bool powerloss);
+static void lfs_fs_prepsuperblock(lfs_t *lfs, bool needssuperblock);
 static int lfs_fs_preporphans(lfs_t *lfs, int8_t orphans);
 static void lfs_fs_prepmove(lfs_t *lfs,
         uint16_t id, const lfs_block_t pair[2]);
 static int lfs_fs_pred(lfs_t *lfs, const lfs_block_t dir[2],
         lfs_mdir_t *pdir);
 static lfs_stag_t lfs_fs_parent(lfs_t *lfs, const lfs_block_t dir[2],
         lfs_mdir_t *parent);
-static int lfs_fs_relocate(lfs_t *lfs,
-        const lfs_block_t oldpair[2], lfs_block_t newpair[2]);
 static int lfs_fs_forceconsistency(lfs_t *lfs);
 #endif
 
 #ifdef LFS_MIGRATE
 static int lfs1_traverse(lfs_t *lfs,
         int (*cb)(void*, lfs_block_t), void *data);
 #endif
 
 static int lfs_dir_rawrewind(lfs_t *lfs, lfs_dir_t *dir);
 
+static lfs_ssize_t lfs_file_flushedread(lfs_t *lfs, lfs_file_t *file,
+        void *buffer, lfs_size_t size);
 static lfs_ssize_t lfs_file_rawread(lfs_t *lfs, lfs_file_t *file,
         void *buffer, lfs_size_t size);
 static int lfs_file_rawclose(lfs_t *lfs, lfs_file_t *file);
 static lfs_soff_t lfs_file_rawsize(lfs_t *lfs, lfs_file_t *file);
 
 static lfs_ssize_t lfs_fs_rawsize(lfs_t *lfs);
 static int lfs_fs_rawtraverse(lfs_t *lfs,
@@ -722,120 +791,250 @@
 
     // check for redundancy
     if ((mask & tag) == (mask & *filtertag) ||
             lfs_tag_isdelete(*filtertag) ||
             (LFS_MKTAG(0x7ff, 0x3ff, 0) & tag) == (
                 LFS_MKTAG(LFS_TYPE_DELETE, 0, 0) |
                     (LFS_MKTAG(0, 0x3ff, 0) & *filtertag))) {
+        *filtertag = LFS_MKTAG(LFS_FROM_NOOP, 0, 0);
         return true;
     }
 
     // check if we need to adjust for created/deleted tags
     if (lfs_tag_type1(tag) == LFS_TYPE_SPLICE &&
             lfs_tag_id(tag) <= lfs_tag_id(*filtertag)) {
         *filtertag += LFS_MKTAG(0, lfs_tag_splice(tag), 0);
     }
 
     return false;
 }
 #endif
 
 #ifndef LFS_READONLY
+// maximum recursive depth of lfs_dir_traverse, the deepest call:
+//
+// traverse with commit
+// '-> traverse with move
+//     '-> traverse with filter
+//
+#define LFS_DIR_TRAVERSE_DEPTH 3
+
+struct lfs_dir_traverse {
+    const lfs_mdir_t *dir;
+    lfs_off_t off;
+    lfs_tag_t ptag;
+    const struct lfs_mattr *attrs;
+    int attrcount;
+
+    lfs_tag_t tmask;
+    lfs_tag_t ttag;
+    uint16_t begin;
+    uint16_t end;
+    int16_t diff;
+
+    int (*cb)(void *data, lfs_tag_t tag, const void *buffer);
+    void *data;
+
+    lfs_tag_t tag;
+    const void *buffer;
+    struct lfs_diskoff disk;
+};
+
 static int lfs_dir_traverse(lfs_t *lfs,
         const lfs_mdir_t *dir, lfs_off_t off, lfs_tag_t ptag,
         const struct lfs_mattr *attrs, int attrcount,
         lfs_tag_t tmask, lfs_tag_t ttag,
         uint16_t begin, uint16_t end, int16_t diff,
         int (*cb)(void *data, lfs_tag_t tag, const void *buffer), void *data) {
+    // This function in inherently recursive, but bounded. To allow tool-based
+    // analysis without unnecessary code-cost we use an explicit stack
+    struct lfs_dir_traverse stack[LFS_DIR_TRAVERSE_DEPTH-1];
+    unsigned sp = 0;
+    int res;
+
     // iterate over directory and attrs
+    lfs_tag_t tag;
+    const void *buffer;
+    struct lfs_diskoff disk;
     while (true) {
-        lfs_tag_t tag;
-        const void *buffer;
-        struct lfs_diskoff disk;
-        if (off+lfs_tag_dsize(ptag) < dir->off) {
-            off += lfs_tag_dsize(ptag);
-            int err = lfs_bd_read(lfs,
-                    NULL, &lfs->rcache, sizeof(tag),
-                    dir->pair[0], off, &tag, sizeof(tag));
-            if (err) {
-                return err;
-            }
-
-            tag = (lfs_frombe32(tag) ^ ptag) | 0x80000000;
-            disk.block = dir->pair[0];
-            disk.off = off+sizeof(lfs_tag_t);
-            buffer = &disk;
-            ptag = tag;
-        } else if (attrcount > 0) {
-            tag = attrs[0].tag;
-            buffer = attrs[0].buffer;
-            attrs += 1;
-            attrcount -= 1;
-        } else {
-            return 0;
-        }
-
-        lfs_tag_t mask = LFS_MKTAG(0x7ff, 0, 0);
-        if ((mask & tmask & tag) != (mask & tmask & ttag)) {
-            continue;
-        }
+        {
+            if (off+lfs_tag_dsize(ptag) < dir->off) {
+                off += lfs_tag_dsize(ptag);
+                int err = lfs_bd_read(lfs,
+                        NULL, &lfs->rcache, sizeof(tag),
+                        dir->pair[0], off, &tag, sizeof(tag));
+                if (err) {
+                    return err;
+                }
 
-        // do we need to filter? inlining the filtering logic here allows
-        // for some minor optimizations
-        if (lfs_tag_id(tmask) != 0) {
-            // scan for duplicates and update tag based on creates/deletes
-            int filter = lfs_dir_traverse(lfs,
-                    dir, off, ptag, attrs, attrcount,
-                    0, 0, 0, 0, 0,
-                    lfs_dir_traverse_filter, &tag);
-            if (filter < 0) {
-                return filter;
+                tag = (lfs_frombe32(tag) ^ ptag) | 0x80000000;
+                disk.block = dir->pair[0];
+                disk.off = off+sizeof(lfs_tag_t);
+                buffer = &disk;
+                ptag = tag;
+            } else if (attrcount > 0) {
+                tag = attrs[0].tag;
+                buffer = attrs[0].buffer;
+                attrs += 1;
+                attrcount -= 1;
+            } else {
+                // finished traversal, pop from stack?
+                res = 0;
+                break;
             }
 
-            if (filter) {
+            // do we need to filter?
+            lfs_tag_t mask = LFS_MKTAG(0x7ff, 0, 0);
+            if ((mask & tmask & tag) != (mask & tmask & ttag)) {
                 continue;
             }
 
-            // in filter range?
-            if (!(lfs_tag_id(tag) >= begin && lfs_tag_id(tag) < end)) {
+            if (lfs_tag_id(tmask) != 0) {
+                LFS_ASSERT(sp < LFS_DIR_TRAVERSE_DEPTH);
+                // recurse, scan for duplicates, and update tag based on
+                // creates/deletes
+                stack[sp] = (struct lfs_dir_traverse){
+                    .dir        = dir,
+                    .off        = off,
+                    .ptag       = ptag,
+                    .attrs      = attrs,
+                    .attrcount  = attrcount,
+                    .tmask      = tmask,
+                    .ttag       = ttag,
+                    .begin      = begin,
+                    .end        = end,
+                    .diff       = diff,
+                    .cb         = cb,
+                    .data       = data,
+                    .tag        = tag,
+                    .buffer     = buffer,
+                    .disk       = disk,
+                };
+                sp += 1;
+
+                tmask = 0;
+                ttag = 0;
+                begin = 0;
+                end = 0;
+                diff = 0;
+                cb = lfs_dir_traverse_filter;
+                data = &stack[sp-1].tag;
                 continue;
             }
         }
 
+popped:
+        // in filter range?
+        if (lfs_tag_id(tmask) != 0 &&
+                !(lfs_tag_id(tag) >= begin && lfs_tag_id(tag) < end)) {
+            continue;
+        }
+
         // handle special cases for mcu-side operations
         if (lfs_tag_type3(tag) == LFS_FROM_NOOP) {
             // do nothing
         } else if (lfs_tag_type3(tag) == LFS_FROM_MOVE) {
+            // Without this condition, lfs_dir_traverse can exhibit an
+            // extremely expensive O(n^3) of nested loops when renaming.
+            // This happens because lfs_dir_traverse tries to filter tags by
+            // the tags in the source directory, triggering a second
+            // lfs_dir_traverse with its own filter operation.
+            //
+            // traverse with commit
+            // '-> traverse with filter
+            //     '-> traverse with move
+            //         '-> traverse with filter
+            //
+            // However we don't actually care about filtering the second set of
+            // tags, since duplicate tags have no effect when filtering.
+            //
+            // This check skips this unnecessary recursive filtering explicitly,
+            // reducing this runtime from O(n^3) to O(n^2).
+            if (cb == lfs_dir_traverse_filter) {
+                continue;
+            }
+
+            // recurse into move
+            stack[sp] = (struct lfs_dir_traverse){
+                .dir        = dir,
+                .off        = off,
+                .ptag       = ptag,
+                .attrs      = attrs,
+                .attrcount  = attrcount,
+                .tmask      = tmask,
+                .ttag       = ttag,
+                .begin      = begin,
+                .end        = end,
+                .diff       = diff,
+                .cb         = cb,
+                .data       = data,
+                .tag        = LFS_MKTAG(LFS_FROM_NOOP, 0, 0),
+            };
+            sp += 1;
+
             uint16_t fromid = lfs_tag_size(tag);
             uint16_t toid = lfs_tag_id(tag);
-            int err = lfs_dir_traverse(lfs,
-                    buffer, 0, 0xffffffff, NULL, 0,
-                    LFS_MKTAG(0x600, 0x3ff, 0),
-                    LFS_MKTAG(LFS_TYPE_STRUCT, 0, 0),
-                    fromid, fromid+1, toid-fromid+diff,
-                    cb, data);
-            if (err) {
-                return err;
-            }
+            dir = buffer;
+            off = 0;
+            ptag = 0xffffffff;
+            attrs = NULL;
+            attrcount = 0;
+            tmask = LFS_MKTAG(0x600, 0x3ff, 0);
+            ttag = LFS_MKTAG(LFS_TYPE_STRUCT, 0, 0);
+            begin = fromid;
+            end = fromid+1;
+            diff = toid-fromid+diff;
         } else if (lfs_tag_type3(tag) == LFS_FROM_USERATTRS) {
             for (unsigned i = 0; i < lfs_tag_size(tag); i++) {
                 const struct lfs_attr *a = buffer;
-                int err = cb(data, LFS_MKTAG(LFS_TYPE_USERATTR + a[i].type,
+                res = cb(data, LFS_MKTAG(LFS_TYPE_USERATTR + a[i].type,
                         lfs_tag_id(tag) + diff, a[i].size), a[i].buffer);
-                if (err) {
-                    return err;
+                if (res < 0) {
+                    return res;
+                }
+
+                if (res) {
+                    break;
                 }
             }
         } else {
-            int err = cb(data, tag + LFS_MKTAG(0, diff, 0), buffer);
-            if (err) {
-                return err;
+            res = cb(data, tag + LFS_MKTAG(0, diff, 0), buffer);
+            if (res < 0) {
+                return res;
+            }
+
+            if (res) {
+                break;
             }
         }
     }
+
+    if (sp > 0) {
+        // pop from the stack and return, fortunately all pops share
+        // a destination
+        dir         = stack[sp-1].dir;
+        off         = stack[sp-1].off;
+        ptag        = stack[sp-1].ptag;
+        attrs       = stack[sp-1].attrs;
+        attrcount   = stack[sp-1].attrcount;
+        tmask       = stack[sp-1].tmask;
+        ttag        = stack[sp-1].ttag;
+        begin       = stack[sp-1].begin;
+        end         = stack[sp-1].end;
+        diff        = stack[sp-1].diff;
+        cb          = stack[sp-1].cb;
+        data        = stack[sp-1].data;
+        tag         = stack[sp-1].tag;
+        buffer      = stack[sp-1].buffer;
+        disk        = stack[sp-1].disk;
+        sp -= 1;
+        goto popped;
+    } else {
+        return res;
+    }
 }
 #endif
 
 static lfs_stag_t lfs_dir_fetchmatch(lfs_t *lfs,
         lfs_mdir_t *dir, const lfs_block_t pair[2],
         lfs_tag_t fmask, lfs_tag_t ftag, uint16_t *id,
         int (*cb)(void *data, lfs_tag_t tag, const void *buffer), void *data) {
@@ -878,66 +1077,67 @@
         lfs_tag_t ptag = 0xffffffff;
 
         uint16_t tempcount = 0;
         lfs_block_t temptail[2] = {LFS_BLOCK_NULL, LFS_BLOCK_NULL};
         bool tempsplit = false;
         lfs_stag_t tempbesttag = besttag;
 
+        // assume not erased until proven otherwise
+        bool maybeerased = false;
+        bool hasfcrc = false;
+        struct lfs_fcrc fcrc;
+
         dir->rev = lfs_tole32(dir->rev);
         uint32_t crc = lfs_crc(0xffffffff, &dir->rev, sizeof(dir->rev));
         dir->rev = lfs_fromle32(dir->rev);
 
         while (true) {
             // extract next tag
             lfs_tag_t tag;
             off += lfs_tag_dsize(ptag);
             int err = lfs_bd_read(lfs,
                     NULL, &lfs->rcache, lfs->cfg->block_size,
                     dir->pair[0], off, &tag, sizeof(tag));
             if (err) {
                 if (err == LFS_ERR_CORRUPT) {
                     // can't continue?
-                    dir->erased = false;
                     break;
                 }
                 return err;
             }
 
             crc = lfs_crc(crc, &tag, sizeof(tag));
             tag = lfs_frombe32(tag) ^ ptag;
 
-            // next commit not yet programmed or we're not in valid range
+            // next commit not yet programmed?
             if (!lfs_tag_isvalid(tag)) {
-                dir->erased = (lfs_tag_type1(ptag) == LFS_TYPE_CRC &&
-                        dir->off % lfs->cfg->prog_size == 0);
+                maybeerased = true;
                 break;
+            // out of range?
             } else if (off + lfs_tag_dsize(tag) > lfs->cfg->block_size) {
-                dir->erased = false;
                 break;
             }
 
             ptag = tag;
 
-            if (lfs_tag_type1(tag) == LFS_TYPE_CRC) {
+            if (lfs_tag_type2(tag) == LFS_TYPE_CCRC) {
                 // check the crc attr
                 uint32_t dcrc;
                 err = lfs_bd_read(lfs,
                         NULL, &lfs->rcache, lfs->cfg->block_size,
                         dir->pair[0], off+sizeof(tag), &dcrc, sizeof(dcrc));
                 if (err) {
                     if (err == LFS_ERR_CORRUPT) {
-                        dir->erased = false;
                         break;
                     }
                     return err;
                 }
                 dcrc = lfs_fromle32(dcrc);
 
                 if (crc != dcrc) {
-                    dir->erased = false;
                     break;
                 }
 
                 // reset the next bit if we need to
                 ptag ^= (lfs_tag_t)(lfs_tag_chunk(tag) & 1U) << 31;
 
                 // toss our crc into the filesystem seed for
@@ -956,29 +1156,27 @@
                 dir->split = tempsplit;
 
                 // reset crc
                 crc = 0xffffffff;
                 continue;
             }
 
+            // fcrc is only valid when last tag was a crc
+            hasfcrc = false;
+
             // crc the entry first, hopefully leaving it in the cache
-            for (lfs_off_t j = sizeof(tag); j < lfs_tag_dsize(tag); j++) {
-                uint8_t dat;
-                err = lfs_bd_read(lfs,
-                        NULL, &lfs->rcache, lfs->cfg->block_size,
-                        dir->pair[0], off+j, &dat, 1);
-                if (err) {
-                    if (err == LFS_ERR_CORRUPT) {
-                        dir->erased = false;
-                        break;
-                    }
-                    return err;
+            err = lfs_bd_crc(lfs,
+                    NULL, &lfs->rcache, lfs->cfg->block_size,
+                    dir->pair[0], off+sizeof(tag),
+                    lfs_tag_dsize(tag)-sizeof(tag), &crc);
+            if (err) {
+                if (err == LFS_ERR_CORRUPT) {
+                    break;
                 }
-
-                crc = lfs_crc(crc, &dat, 1);
+                return err;
             }
 
             // directory modification tags?
             if (lfs_tag_type1(tag) == LFS_TYPE_NAME) {
                 // increase count of files if necessary
                 if (lfs_tag_id(tag) >= tempcount) {
                     tempcount = lfs_tag_id(tag) + 1;
@@ -997,28 +1195,40 @@
                 tempsplit = (lfs_tag_chunk(tag) & 1);
 
                 err = lfs_bd_read(lfs,
                         NULL, &lfs->rcache, lfs->cfg->block_size,
                         dir->pair[0], off+sizeof(tag), &temptail, 8);
                 if (err) {
                     if (err == LFS_ERR_CORRUPT) {
-                        dir->erased = false;
                         break;
                     }
+                    return err;
                 }
                 lfs_pair_fromle32(temptail);
+            } else if (lfs_tag_type3(tag) == LFS_TYPE_FCRC) {
+                err = lfs_bd_read(lfs,
+                        NULL, &lfs->rcache, lfs->cfg->block_size,
+                        dir->pair[0], off+sizeof(tag),
+                        &fcrc, sizeof(fcrc));
+                if (err) {
+                    if (err == LFS_ERR_CORRUPT) {
+                        break;
+                    }
+                }
+
+                lfs_fcrc_fromle32(&fcrc);
+                hasfcrc = true;
             }
 
             // found a match for our fetcher?
             if ((fmask & tag) == (fmask & ftag)) {
                 int res = cb(data, tag, &(struct lfs_diskoff){
                         dir->pair[0], off+sizeof(tag)});
                 if (res < 0) {
                     if (res == LFS_ERR_CORRUPT) {
-                        dir->erased = false;
                         break;
                     }
                     return res;
                 }
 
                 if (res == LFS_CMP_EQ) {
                     // found a match
@@ -1032,43 +1242,62 @@
                         lfs_tag_id(tag) <= lfs_tag_id(tempbesttag)) {
                     // found a greater match, keep track to keep things sorted
                     tempbesttag = tag | 0x80000000;
                 }
             }
         }
 
-        // consider what we have good enough
-        if (dir->off > 0) {
-            // synthetic move
-            if (lfs_gstate_hasmovehere(&lfs->gdisk, dir->pair)) {
-                if (lfs_tag_id(lfs->gdisk.tag) == lfs_tag_id(besttag)) {
-                    besttag |= 0x80000000;
-                } else if (besttag != -1 &&
-                        lfs_tag_id(lfs->gdisk.tag) < lfs_tag_id(besttag)) {
-                    besttag -= LFS_MKTAG(0, 1, 0);
-                }
+        // found no valid commits?
+        if (dir->off == 0) {
+            // try the other block?
+            lfs_pair_swap(dir->pair);
+            dir->rev = revs[(r+1)%2];
+            continue;
+        }
+
+        // did we end on a valid commit? we may have an erased block
+        dir->erased = false;
+        if (maybeerased && hasfcrc && dir->off % lfs->cfg->prog_size == 0) {
+            // check for an fcrc matching the next prog's erased state, if
+            // this failed most likely a previous prog was interrupted, we
+            // need a new erase
+            uint32_t fcrc_ = 0xffffffff;
+            int err = lfs_bd_crc(lfs,
+                    NULL, &lfs->rcache, lfs->cfg->block_size,
+                    dir->pair[0], dir->off, fcrc.size, &fcrc_);
+            if (err && err != LFS_ERR_CORRUPT) {
+                return err;
             }
 
-            // found tag? or found best id?
-            if (id) {
-                *id = lfs_min(lfs_tag_id(besttag), dir->count);
-            }
-
-            if (lfs_tag_isvalid(besttag)) {
-                return besttag;
-            } else if (lfs_tag_id(besttag) < dir->count) {
-                return LFS_ERR_NOENT;
-            } else {
-                return 0;
+            // found beginning of erased part?
+            dir->erased = (fcrc_ == fcrc.crc);
+        }
+
+        // synthetic move
+        if (lfs_gstate_hasmovehere(&lfs->gdisk, dir->pair)) {
+            if (lfs_tag_id(lfs->gdisk.tag) == lfs_tag_id(besttag)) {
+                besttag |= 0x80000000;
+            } else if (besttag != -1 &&
+                    lfs_tag_id(lfs->gdisk.tag) < lfs_tag_id(besttag)) {
+                besttag -= LFS_MKTAG(0, 1, 0);
             }
         }
 
-        // failed, try the other block?
-        lfs_pair_swap(dir->pair);
-        dir->rev = revs[(r+1)%2];
+        // found tag? or found best id?
+        if (id) {
+            *id = lfs_min(lfs_tag_id(besttag), dir->count);
+        }
+
+        if (lfs_tag_isvalid(besttag)) {
+            return besttag;
+        } else if (lfs_tag_id(besttag) < dir->count) {
+            return LFS_ERR_NOENT;
+        } else {
+            return 0;
+        }
     }
 
     LFS_ERROR("Corrupted dir pair at {0x%"PRIx32", 0x%"PRIx32"}",
             dir->pair[0], dir->pair[1]);
     return LFS_ERR_CORRUPT;
 }
 
@@ -1334,109 +1563,142 @@
 
     commit->ptag = tag & 0x7fffffff;
     return 0;
 }
 #endif
 
 #ifndef LFS_READONLY
+
 static int lfs_dir_commitcrc(lfs_t *lfs, struct lfs_commit *commit) {
     // align to program units
-    const lfs_off_t end = lfs_alignup(commit->off + 2*sizeof(uint32_t),
+    //
+    // this gets a bit complex as we have two types of crcs:
+    // - 5-word crc with fcrc to check following prog (middle of block)
+    // - 2-word crc with no following prog (end of block)
+    const lfs_off_t end = lfs_alignup(
+            lfs_min(commit->off + 5*sizeof(uint32_t), lfs->cfg->block_size),
             lfs->cfg->prog_size);
 
     lfs_off_t off1 = 0;
     uint32_t crc1 = 0;
 
     // create crc tags to fill up remainder of commit, note that
     // padding is not crced, which lets fetches skip padding but
     // makes committing a bit more complicated
     while (commit->off < end) {
-        lfs_off_t off = commit->off + sizeof(lfs_tag_t);
-        lfs_off_t noff = lfs_min(end - off, 0x3fe) + off;
+        lfs_off_t noff = (
+                lfs_min(end - (commit->off+sizeof(lfs_tag_t)), 0x3fe)
+                + (commit->off+sizeof(lfs_tag_t)));
+        // too large for crc tag? need padding commits
         if (noff < end) {
-            noff = lfs_min(noff, end - 2*sizeof(uint32_t));
+            noff = lfs_min(noff, end - 5*sizeof(uint32_t));
         }
 
-        // read erased state from next program unit
-        lfs_tag_t tag = 0xffffffff;
-        int err = lfs_bd_read(lfs,
-                NULL, &lfs->rcache, sizeof(tag),
-                commit->block, noff, &tag, sizeof(tag));
-        if (err && err != LFS_ERR_CORRUPT) {
-            return err;
+        // space for fcrc?
+        uint8_t eperturb = -1;
+        if (noff >= end && noff <= lfs->cfg->block_size - lfs->cfg->prog_size) {
+            // first read the leading byte, this always contains a bit
+            // we can perturb to avoid writes that don't change the fcrc
+            int err = lfs_bd_read(lfs,
+                    NULL, &lfs->rcache, lfs->cfg->prog_size,
+                    commit->block, noff, &eperturb, 1);
+            if (err && err != LFS_ERR_CORRUPT) {
+                return err;
+            }
+
+            // find the expected fcrc, don't bother avoiding a reread
+            // of the eperturb, it should still be in our cache
+            struct lfs_fcrc fcrc = {.size=lfs->cfg->prog_size, .crc=0xffffffff};
+            err = lfs_bd_crc(lfs,
+                    NULL, &lfs->rcache, lfs->cfg->prog_size,
+                    commit->block, noff, fcrc.size, &fcrc.crc);
+            if (err && err != LFS_ERR_CORRUPT) {
+                return err;
+            }
+
+            lfs_fcrc_tole32(&fcrc);
+            err = lfs_dir_commitattr(lfs, commit,
+                    LFS_MKTAG(LFS_TYPE_FCRC, 0x3ff, sizeof(struct lfs_fcrc)),
+                    &fcrc);
+            if (err) {
+                return err;
+            }
         }
 
-        // build crc tag
-        bool reset = ~lfs_frombe32(tag) >> 31;
-        tag = LFS_MKTAG(LFS_TYPE_CRC + reset, 0x3ff, noff - off);
-
-        // write out crc
-        uint32_t footer[2];
-        footer[0] = lfs_tobe32(tag ^ commit->ptag);
-        commit->crc = lfs_crc(commit->crc, &footer[0], sizeof(footer[0]));
-        footer[1] = lfs_tole32(commit->crc);
-        err = lfs_bd_prog(lfs,
+        // build commit crc
+        struct {
+            lfs_tag_t tag;
+            uint32_t crc;
+        } ccrc;
+        lfs_tag_t ntag = LFS_MKTAG(
+                LFS_TYPE_CCRC + (((uint8_t)~eperturb) >> 7), 0x3ff,
+                noff - (commit->off+sizeof(lfs_tag_t)));
+        ccrc.tag = lfs_tobe32(ntag ^ commit->ptag);
+        commit->crc = lfs_crc(commit->crc, &ccrc.tag, sizeof(lfs_tag_t));
+        ccrc.crc = lfs_tole32(commit->crc);
+
+        int err = lfs_bd_prog(lfs,
                 &lfs->pcache, &lfs->rcache, false,
-                commit->block, commit->off, &footer, sizeof(footer));
+                commit->block, commit->off, &ccrc, sizeof(ccrc));
         if (err) {
             return err;
         }
 
         // keep track of non-padding checksum to verify
         if (off1 == 0) {
-            off1 = commit->off + sizeof(uint32_t);
+            off1 = commit->off + sizeof(lfs_tag_t);
             crc1 = commit->crc;
         }
 
-        commit->off += sizeof(tag)+lfs_tag_size(tag);
-        commit->ptag = tag ^ ((lfs_tag_t)reset << 31);
-        commit->crc = 0xffffffff; // reset crc for next "commit"
+        commit->off = noff;
+        // perturb valid bit?
+        commit->ptag = ntag ^ ((0x80UL & ~eperturb) << 24);
+        // reset crc for next commit
+        commit->crc = 0xffffffff;
+
+        // manually flush here since we don't prog the padding, this confuses
+        // the caching layer
+        if (noff >= end || noff >= lfs->pcache.off + lfs->cfg->cache_size) {
+            // flush buffers
+            int err = lfs_bd_sync(lfs, &lfs->pcache, &lfs->rcache, false);
+            if (err) {
+                return err;
+            }
+        }
     }
 
-    // flush buffers
-    int err = lfs_bd_sync(lfs, &lfs->pcache, &lfs->rcache, false);
+    // successful commit, check checksums to make sure
+    //
+    // note that we don't need to check padding commits, worst
+    // case if they are corrupted we would have had to compact anyways
+    lfs_off_t off = commit->begin;
+    uint32_t crc = 0xffffffff;
+    int err = lfs_bd_crc(lfs,
+            NULL, &lfs->rcache, off1+sizeof(uint32_t),
+            commit->block, off, off1-off, &crc);
     if (err) {
         return err;
     }
 
-    // successful commit, check checksums to make sure
-    lfs_off_t off = commit->begin;
-    lfs_off_t noff = off1;
-    while (off < end) {
-        uint32_t crc = 0xffffffff;
-        for (lfs_off_t i = off; i < noff+sizeof(uint32_t); i++) {
-            // check against written crc, may catch blocks that
-            // become readonly and match our commit size exactly
-            if (i == off1 && crc != crc1) {
-                return LFS_ERR_CORRUPT;
-            }
-
-            // leave it up to caching to make this efficient
-            uint8_t dat;
-            err = lfs_bd_read(lfs,
-                    NULL, &lfs->rcache, noff+sizeof(uint32_t)-i,
-                    commit->block, i, &dat, 1);
-            if (err) {
-                return err;
-            }
-
-            crc = lfs_crc(crc, &dat, 1);
-        }
+    // check non-padding commits against known crc
+    if (crc != crc1) {
+        return LFS_ERR_CORRUPT;
+    }
 
-        // detected write error?
-        if (crc != 0) {
-            return LFS_ERR_CORRUPT;
-        }
+    // make sure to check crc in case we happen to pick
+    // up an unrelated crc (frozen block?)
+    err = lfs_bd_crc(lfs,
+            NULL, &lfs->rcache, sizeof(uint32_t),
+            commit->block, off1, sizeof(uint32_t), &crc);
+    if (err) {
+        return err;
+    }
 
-        // skip padding
-        off = lfs_min(end - noff, 0x3fe) + noff;
-        if (off < end) {
-            off = lfs_min(off, end - 2*sizeof(uint32_t));
-        }
-        noff = off + sizeof(uint32_t);
+    if (crc != 0) {
+        return LFS_ERR_CORRUPT;
     }
 
     return 0;
 }
 #endif
 
 #ifndef LFS_READONLY
@@ -1445,15 +1707,15 @@
     for (int i = 0; i < 2; i++) {
         int err = lfs_alloc(lfs, &dir->pair[(i+1)%2]);
         if (err) {
             return err;
         }
     }
 
-    // zero for reproducability in case initial block is unreadable
+    // zero for reproducibility in case initial block is unreadable
     dir->rev = 0;
 
     // rather than clobbering one of the blocks we just pretend
     // the revision may be valid
     int err = lfs_bd_read(lfs,
             NULL, &lfs->rcache, sizeof(dir->rev),
             dir->pair[0], 0, &dir->rev, sizeof(dir->rev));
@@ -1504,29 +1766,29 @@
 }
 #endif
 
 #ifndef LFS_READONLY
 static int lfs_dir_split(lfs_t *lfs,
         lfs_mdir_t *dir, const struct lfs_mattr *attrs, int attrcount,
         lfs_mdir_t *source, uint16_t split, uint16_t end) {
-    // create tail directory
-    lfs_alloc_ack(lfs);
+    // create tail metadata pair
     lfs_mdir_t tail;
     int err = lfs_dir_alloc(lfs, &tail);
     if (err) {
         return err;
     }
 
     tail.split = dir->split;
     tail.tail[0] = dir->tail[0];
     tail.tail[1] = dir->tail[1];
 
-    err = lfs_dir_compact(lfs, &tail, attrs, attrcount, source, split, end);
-    if (err) {
-        return err;
+    // note we don't care about LFS_OK_RELOCATED
+    int res = lfs_dir_compact(lfs, &tail, attrs, attrcount, source, split, end);
+    if (res < 0) {
+        return res;
     }
 
     dir->tail[0] = tail.pair[0];
     dir->tail[1] = tail.pair[1];
     dir->split = true;
 
     // update root if needed
@@ -1560,114 +1822,52 @@
 static int lfs_dir_commit_commit(void *p, lfs_tag_t tag, const void *buffer) {
     struct lfs_dir_commit_commit *commit = p;
     return lfs_dir_commitattr(commit->lfs, commit->commit, tag, buffer);
 }
 #endif
 
 #ifndef LFS_READONLY
+static bool lfs_dir_needsrelocation(lfs_t *lfs, lfs_mdir_t *dir) {
+    // If our revision count == n * block_cycles, we should force a relocation,
+    // this is how littlefs wear-levels at the metadata-pair level. Note that we
+    // actually use (block_cycles+1)|1, this is to avoid two corner cases:
+    // 1. block_cycles = 1, which would prevent relocations from terminating
+    // 2. block_cycles = 2n, which, due to aliasing, would only ever relocate
+    //    one metadata block in the pair, effectively making this useless
+    return (lfs->cfg->block_cycles > 0
+            && ((dir->rev + 1) % ((lfs->cfg->block_cycles+1)|1) == 0));
+}
+#endif
+
+#ifndef LFS_READONLY
 static int lfs_dir_compact(lfs_t *lfs,
         lfs_mdir_t *dir, const struct lfs_mattr *attrs, int attrcount,
         lfs_mdir_t *source, uint16_t begin, uint16_t end) {
     // save some state in case block is bad
-    const lfs_block_t oldpair[2] = {dir->pair[0], dir->pair[1]};
     bool relocated = false;
-    bool tired = false;
-
-    // should we split?
-    while (end - begin > 1) {
-        // find size
-        lfs_size_t size = 0;
-        int err = lfs_dir_traverse(lfs,
-                source, 0, 0xffffffff, attrs, attrcount,
-                LFS_MKTAG(0x400, 0x3ff, 0),
-                LFS_MKTAG(LFS_TYPE_NAME, 0, 0),
-                begin, end, -begin,
-                lfs_dir_commit_size, &size);
-        if (err) {
-            return err;
-        }
-
-        // space is complicated, we need room for tail, crc, gstate,
-        // cleanup delete, and we cap at half a block to give room
-        // for metadata updates.
-        if (end - begin < 0xff &&
-                size <= lfs_min(lfs->cfg->block_size - 36,
-                    lfs_alignup((lfs->cfg->metadata_max ?
-                            lfs->cfg->metadata_max : lfs->cfg->block_size)/2,
-                        lfs->cfg->prog_size))) {
-            break;
-        }
-
-        // can't fit, need to split, we should really be finding the
-        // largest size that fits with a small binary search, but right now
-        // it's not worth the code size
-        uint16_t split = (end - begin) / 2;
-        err = lfs_dir_split(lfs, dir, attrs, attrcount,
-                source, begin+split, end);
-        if (err) {
-            // if we fail to split, we may be able to overcompact, unless
-            // we're too big for even the full block, in which case our
-            // only option is to error
-            if (err == LFS_ERR_NOSPC && size <= lfs->cfg->block_size - 36) {
-                break;
-            }
-            return err;
-        }
-
-        end = begin + split;
-    }
+    bool tired = lfs_dir_needsrelocation(lfs, dir);
 
     // increment revision count
     dir->rev += 1;
-    // If our revision count == n * block_cycles, we should force a relocation,
-    // this is how littlefs wear-levels at the metadata-pair level. Note that we
-    // actually use (block_cycles+1)|1, this is to avoid two corner cases:
-    // 1. block_cycles = 1, which would prevent relocations from terminating
-    // 2. block_cycles = 2n, which, due to aliasing, would only ever relocate
-    //    one metadata block in the pair, effectively making this useless
-    if (lfs->cfg->block_cycles > 0 &&
-            (dir->rev % ((lfs->cfg->block_cycles+1)|1) == 0)) {
-        if (lfs_pair_cmp(dir->pair, (const lfs_block_t[2]){0, 1}) == 0) {
-            // oh no! we're writing too much to the superblock,
-            // should we expand?
-            lfs_ssize_t res = lfs_fs_rawsize(lfs);
-            if (res < 0) {
-                return res;
-            }
-
-            // do we have extra space? littlefs can't reclaim this space
-            // by itself, so expand cautiously
-            if ((lfs_size_t)res < lfs->cfg->block_count/2) {
-                LFS_DEBUG("Expanding superblock at rev %"PRIu32, dir->rev);
-                int err = lfs_dir_split(lfs, dir, attrs, attrcount,
-                        source, begin, end);
-                if (err && err != LFS_ERR_NOSPC) {
-                    return err;
-                }
 
-                // welp, we tried, if we ran out of space there's not much
-                // we can do, we'll error later if we've become frozen
-                if (!err) {
-                    end = begin;
-                }
-            }
+    // do not proactively relocate blocks during migrations, this
+    // can cause a number of failure states such: clobbering the
+    // v1 superblock if we relocate root, and invalidating directory
+    // pointers if we relocate the head of a directory. On top of
+    // this, relocations increase the overall complexity of
+    // lfs_migration, which is already a delicate operation.
 #ifdef LFS_MIGRATE
-        } else if (lfs->lfs1) {
-            // do not proactively relocate blocks during migrations, this
-            // can cause a number of failure states such: clobbering the
-            // v1 superblock if we relocate root, and invalidating directory
-            // pointers if we relocate the head of a directory. On top of
-            // this, relocations increase the overall complexity of
-            // lfs_migration, which is already a delicate operation.
+    if (lfs->lfs1) {
+        tired = false;
+    }
 #endif
-        } else {
-            // we're writing too much, time to relocate
-            tired = true;
-            goto relocate;
-        }
+
+    if (tired && lfs_pair_cmp(dir->pair, (const lfs_block_t[2]){0, 1}) != 0) {
+        // we're writing too much, time to relocate
+        goto relocate;
     }
 
     // begin loop to commit compaction to blocks until a compact sticks
     while (true) {
         {
             // setup commit state
             struct lfs_commit commit = {
@@ -1803,52 +2003,131 @@
             return err;
         }
 
         tired = false;
         continue;
     }
 
-    if (relocated) {
-        // update references if we relocated
-        LFS_DEBUG("Relocating {0x%"PRIx32", 0x%"PRIx32"} "
-                    "-> {0x%"PRIx32", 0x%"PRIx32"}",
-                oldpair[0], oldpair[1], dir->pair[0], dir->pair[1]);
-        int err = lfs_fs_relocate(lfs, oldpair, dir->pair);
-        if (err) {
-            return err;
-        }
-    }
-
-    return 0;
+    return relocated ? LFS_OK_RELOCATED : 0;
 }
 #endif
 
 #ifndef LFS_READONLY
-static int lfs_dir_commit(lfs_t *lfs, lfs_mdir_t *dir,
-        const struct lfs_mattr *attrs, int attrcount) {
-    // check for any inline files that aren't RAM backed and
-    // forcefully evict them, needed for filesystem consistency
-    for (lfs_file_t *f = (lfs_file_t*)lfs->mlist; f; f = f->next) {
-        if (dir != &f->m && lfs_pair_cmp(f->m.pair, dir->pair) == 0 &&
-                f->type == LFS_TYPE_REG && (f->flags & LFS_F_INLINE) &&
-                f->ctz.size > lfs->cfg->cache_size) {
-            int err = lfs_file_outline(lfs, f);
+static int lfs_dir_splittingcompact(lfs_t *lfs, lfs_mdir_t *dir,
+        const struct lfs_mattr *attrs, int attrcount,
+        lfs_mdir_t *source, uint16_t begin, uint16_t end) {
+    while (true) {
+        // find size of first split, we do this by halving the split until
+        // the metadata is guaranteed to fit
+        //
+        // Note that this isn't a true binary search, we never increase the
+        // split size. This may result in poorly distributed metadata but isn't
+        // worth the extra code size or performance hit to fix.
+        lfs_size_t split = begin;
+        while (end - split > 1) {
+            lfs_size_t size = 0;
+            int err = lfs_dir_traverse(lfs,
+                    source, 0, 0xffffffff, attrs, attrcount,
+                    LFS_MKTAG(0x400, 0x3ff, 0),
+                    LFS_MKTAG(LFS_TYPE_NAME, 0, 0),
+                    split, end, -split,
+                    lfs_dir_commit_size, &size);
             if (err) {
                 return err;
             }
 
-            err = lfs_file_flush(lfs, f);
-            if (err) {
+            // space is complicated, we need room for:
+            //
+            // - tail:         4+2*4 = 12 bytes
+            // - gstate:       4+3*4 = 16 bytes
+            // - move delete:  4     = 4 bytes
+            // - crc:          4+4   = 8 bytes
+            //                 total = 40 bytes
+            //
+            // And we cap at half a block to avoid degenerate cases with
+            // nearly-full metadata blocks.
+            //
+            if (end - split < 0xff
+                    && size <= lfs_min(
+                        lfs->cfg->block_size - 40,
+                        lfs_alignup(
+                            (lfs->cfg->metadata_max
+                                ? lfs->cfg->metadata_max
+                                : lfs->cfg->block_size)/2,
+                            lfs->cfg->prog_size))) {
+                break;
+            }
+
+            split = split + ((end - split) / 2);
+        }
+
+        if (split == begin) {
+            // no split needed
+            break;
+        }
+
+        // split into two metadata pairs and continue
+        int err = lfs_dir_split(lfs, dir, attrs, attrcount,
+                source, split, end);
+        if (err && err != LFS_ERR_NOSPC) {
+            return err;
+        }
+
+        if (err) {
+            // we can't allocate a new block, try to compact with degraded
+            // performance
+            LFS_WARN("Unable to split {0x%"PRIx32", 0x%"PRIx32"}",
+                    dir->pair[0], dir->pair[1]);
+            break;
+        } else {
+            end = split;
+        }
+    }
+
+    if (lfs_dir_needsrelocation(lfs, dir)
+            && lfs_pair_cmp(dir->pair, (const lfs_block_t[2]){0, 1}) == 0) {
+        // oh no! we're writing too much to the superblock,
+        // should we expand?
+        lfs_ssize_t size = lfs_fs_rawsize(lfs);
+        if (size < 0) {
+            return size;
+        }
+
+        // do we have extra space? littlefs can't reclaim this space
+        // by itself, so expand cautiously
+        if ((lfs_size_t)size < lfs->cfg->block_count/2) {
+            LFS_DEBUG("Expanding superblock at rev %"PRIu32, dir->rev);
+            int err = lfs_dir_split(lfs, dir, attrs, attrcount,
+                    source, begin, end);
+            if (err && err != LFS_ERR_NOSPC) {
                 return err;
             }
+
+            if (err) {
+                // welp, we tried, if we ran out of space there's not much
+                // we can do, we'll error later if we've become frozen
+                LFS_WARN("Unable to expand superblock");
+            } else {
+                end = begin;
+            }
         }
     }
 
+    return lfs_dir_compact(lfs, dir, attrs, attrcount, source, begin, end);
+}
+#endif
+
+#ifndef LFS_READONLY
+static int lfs_dir_relocatingcommit(lfs_t *lfs, lfs_mdir_t *dir,
+        const lfs_block_t pair[2],
+        const struct lfs_mattr *attrs, int attrcount,
+        lfs_mdir_t *pdir) {
+    int state = 0;
+
     // calculate changes to the directory
-    lfs_mdir_t olddir = *dir;
     bool hasdelete = false;
     for (int i = 0; i < attrcount; i++) {
         if (lfs_tag_type3(attrs[i].tag) == LFS_TYPE_CREATE) {
             dir->count += 1;
         } else if (lfs_tag_type3(attrs[i].tag) == LFS_TYPE_DELETE) {
             LFS_ASSERT(dir->count > 0);
             dir->count -= 1;
@@ -1859,31 +2138,27 @@
             dir->split = (lfs_tag_chunk(attrs[i].tag) & 1);
             lfs_pair_fromle32(dir->tail);
         }
     }
 
     // should we actually drop the directory block?
     if (hasdelete && dir->count == 0) {
-        lfs_mdir_t pdir;
-        int err = lfs_fs_pred(lfs, dir->pair, &pdir);
+        LFS_ASSERT(pdir);
+        int err = lfs_fs_pred(lfs, dir->pair, pdir);
         if (err && err != LFS_ERR_NOENT) {
-            *dir = olddir;
             return err;
         }
 
-        if (err != LFS_ERR_NOENT && pdir.split) {
-            err = lfs_dir_drop(lfs, &pdir, dir);
-            if (err) {
-                *dir = olddir;
-                return err;
-            }
+        if (err != LFS_ERR_NOENT && pdir->split) {
+            state = LFS_OK_DROPPED;
+            goto fixmlist;
         }
     }
 
-    if (dir->erased || dir->count >= 0xff) {
+    if (dir->erased) {
         // try to commit
         struct lfs_commit commit = {
             .block = dir->pair[0],
             .off = dir->off,
             .ptag = dir->etag,
             .crc = 0xffffffff,
 
@@ -1900,119 +2175,333 @@
                 lfs_dir_commit_commit, &(struct lfs_dir_commit_commit){
                     lfs, &commit});
         lfs_pair_fromle32(dir->tail);
         if (err) {
             if (err == LFS_ERR_NOSPC || err == LFS_ERR_CORRUPT) {
                 goto compact;
             }
-            *dir = olddir;
             return err;
         }
 
         // commit any global diffs if we have any
         lfs_gstate_t delta = {0};
         lfs_gstate_xor(&delta, &lfs->gstate);
         lfs_gstate_xor(&delta, &lfs->gdisk);
         lfs_gstate_xor(&delta, &lfs->gdelta);
         delta.tag &= ~LFS_MKTAG(0, 0, 0x3ff);
         if (!lfs_gstate_iszero(&delta)) {
             err = lfs_dir_getgstate(lfs, dir, &delta);
             if (err) {
-                *dir = olddir;
                 return err;
             }
 
             lfs_gstate_tole32(&delta);
             err = lfs_dir_commitattr(lfs, &commit,
                     LFS_MKTAG(LFS_TYPE_MOVESTATE, 0x3ff,
                         sizeof(delta)), &delta);
             if (err) {
                 if (err == LFS_ERR_NOSPC || err == LFS_ERR_CORRUPT) {
                     goto compact;
                 }
-                *dir = olddir;
                 return err;
             }
         }
 
         // finalize commit with the crc
         err = lfs_dir_commitcrc(lfs, &commit);
         if (err) {
             if (err == LFS_ERR_NOSPC || err == LFS_ERR_CORRUPT) {
                 goto compact;
             }
-            *dir = olddir;
             return err;
         }
 
         // successful commit, update dir
         LFS_ASSERT(commit.off % lfs->cfg->prog_size == 0);
         dir->off = commit.off;
         dir->etag = commit.ptag;
         // and update gstate
         lfs->gdisk = lfs->gstate;
         lfs->gdelta = (lfs_gstate_t){0};
-    } else {
+
+        goto fixmlist;
+    }
+
 compact:
-        // fall back to compaction
-        lfs_cache_drop(lfs, &lfs->pcache);
+    // fall back to compaction
+    lfs_cache_drop(lfs, &lfs->pcache);
 
-        int err = lfs_dir_compact(lfs, dir, attrs, attrcount,
-                dir, 0, dir->count);
-        if (err) {
-            *dir = olddir;
-            return err;
-        }
+    state = lfs_dir_splittingcompact(lfs, dir, attrs, attrcount,
+            dir, 0, dir->count);
+    if (state < 0) {
+        return state;
     }
 
+    goto fixmlist;
+
+fixmlist:;
     // this complicated bit of logic is for fixing up any active
     // metadata-pairs that we may have affected
     //
     // note we have to make two passes since the mdir passed to
     // lfs_dir_commit could also be in this list, and even then
     // we need to copy the pair so they don't get clobbered if we refetch
     // our mdir.
+    lfs_block_t oldpair[2] = {pair[0], pair[1]};
     for (struct lfs_mlist *d = lfs->mlist; d; d = d->next) {
-        if (&d->m != dir && lfs_pair_cmp(d->m.pair, olddir.pair) == 0) {
+        if (lfs_pair_cmp(d->m.pair, oldpair) == 0) {
             d->m = *dir;
-            for (int i = 0; i < attrcount; i++) {
-                if (lfs_tag_type3(attrs[i].tag) == LFS_TYPE_DELETE &&
-                        d->id == lfs_tag_id(attrs[i].tag)) {
-                    d->m.pair[0] = LFS_BLOCK_NULL;
-                    d->m.pair[1] = LFS_BLOCK_NULL;
-                } else if (lfs_tag_type3(attrs[i].tag) == LFS_TYPE_DELETE &&
-                        d->id > lfs_tag_id(attrs[i].tag)) {
-                    d->id -= 1;
-                    if (d->type == LFS_TYPE_DIR) {
-                        ((lfs_dir_t*)d)->pos -= 1;
-                    }
-                } else if (lfs_tag_type3(attrs[i].tag) == LFS_TYPE_CREATE &&
-                        d->id >= lfs_tag_id(attrs[i].tag)) {
-                    d->id += 1;
-                    if (d->type == LFS_TYPE_DIR) {
-                        ((lfs_dir_t*)d)->pos += 1;
+            if (d->m.pair != pair) {
+                for (int i = 0; i < attrcount; i++) {
+                    if (lfs_tag_type3(attrs[i].tag) == LFS_TYPE_DELETE &&
+                            d->id == lfs_tag_id(attrs[i].tag)) {
+                        d->m.pair[0] = LFS_BLOCK_NULL;
+                        d->m.pair[1] = LFS_BLOCK_NULL;
+                    } else if (lfs_tag_type3(attrs[i].tag) == LFS_TYPE_DELETE &&
+                            d->id > lfs_tag_id(attrs[i].tag)) {
+                        d->id -= 1;
+                        if (d->type == LFS_TYPE_DIR) {
+                            ((lfs_dir_t*)d)->pos -= 1;
+                        }
+                    } else if (lfs_tag_type3(attrs[i].tag) == LFS_TYPE_CREATE &&
+                            d->id >= lfs_tag_id(attrs[i].tag)) {
+                        d->id += 1;
+                        if (d->type == LFS_TYPE_DIR) {
+                            ((lfs_dir_t*)d)->pos += 1;
+                        }
                     }
                 }
             }
-        }
-    }
 
-    for (struct lfs_mlist *d = lfs->mlist; d; d = d->next) {
-        if (lfs_pair_cmp(d->m.pair, olddir.pair) == 0) {
             while (d->id >= d->m.count && d->m.split) {
                 // we split and id is on tail now
                 d->id -= d->m.count;
                 int err = lfs_dir_fetch(lfs, &d->m, d->m.tail);
                 if (err) {
                     return err;
                 }
             }
         }
     }
 
+    return state;
+}
+#endif
+
+#ifndef LFS_READONLY
+static int lfs_dir_orphaningcommit(lfs_t *lfs, lfs_mdir_t *dir,
+        const struct lfs_mattr *attrs, int attrcount) {
+    // check for any inline files that aren't RAM backed and
+    // forcefully evict them, needed for filesystem consistency
+    for (lfs_file_t *f = (lfs_file_t*)lfs->mlist; f; f = f->next) {
+        if (dir != &f->m && lfs_pair_cmp(f->m.pair, dir->pair) == 0 &&
+                f->type == LFS_TYPE_REG && (f->flags & LFS_F_INLINE) &&
+                f->ctz.size > lfs->cfg->cache_size) {
+            int err = lfs_file_outline(lfs, f);
+            if (err) {
+                return err;
+            }
+
+            err = lfs_file_flush(lfs, f);
+            if (err) {
+                return err;
+            }
+        }
+    }
+
+    lfs_block_t lpair[2] = {dir->pair[0], dir->pair[1]};
+    lfs_mdir_t ldir = *dir;
+    lfs_mdir_t pdir;
+    int state = lfs_dir_relocatingcommit(lfs, &ldir, dir->pair,
+            attrs, attrcount, &pdir);
+    if (state < 0) {
+        return state;
+    }
+
+    // update if we're not in mlist, note we may have already been
+    // updated if we are in mlist
+    if (lfs_pair_cmp(dir->pair, lpair) == 0) {
+        *dir = ldir;
+    }
+
+    // commit was successful, but may require other changes in the
+    // filesystem, these would normally be tail recursive, but we have
+    // flattened them here avoid unbounded stack usage
+
+    // need to drop?
+    if (state == LFS_OK_DROPPED) {
+        // steal state
+        int err = lfs_dir_getgstate(lfs, dir, &lfs->gdelta);
+        if (err) {
+            return err;
+        }
+
+        // steal tail, note that this can't create a recursive drop
+        lpair[0] = pdir.pair[0];
+        lpair[1] = pdir.pair[1];
+        lfs_pair_tole32(dir->tail);
+        state = lfs_dir_relocatingcommit(lfs, &pdir, lpair, LFS_MKATTRS(
+                    {LFS_MKTAG(LFS_TYPE_TAIL + dir->split, 0x3ff, 8),
+                        dir->tail}),
+                NULL);
+        lfs_pair_fromle32(dir->tail);
+        if (state < 0) {
+            return state;
+        }
+
+        ldir = pdir;
+    }
+
+    // need to relocate?
+    bool orphans = false;
+    while (state == LFS_OK_RELOCATED) {
+        LFS_DEBUG("Relocating {0x%"PRIx32", 0x%"PRIx32"} "
+                    "-> {0x%"PRIx32", 0x%"PRIx32"}",
+                lpair[0], lpair[1], ldir.pair[0], ldir.pair[1]);
+        state = 0;
+
+        // update internal root
+        if (lfs_pair_cmp(lpair, lfs->root) == 0) {
+            lfs->root[0] = ldir.pair[0];
+            lfs->root[1] = ldir.pair[1];
+        }
+
+        // update internally tracked dirs
+        for (struct lfs_mlist *d = lfs->mlist; d; d = d->next) {
+            if (lfs_pair_cmp(lpair, d->m.pair) == 0) {
+                d->m.pair[0] = ldir.pair[0];
+                d->m.pair[1] = ldir.pair[1];
+            }
+
+            if (d->type == LFS_TYPE_DIR &&
+                    lfs_pair_cmp(lpair, ((lfs_dir_t*)d)->head) == 0) {
+                ((lfs_dir_t*)d)->head[0] = ldir.pair[0];
+                ((lfs_dir_t*)d)->head[1] = ldir.pair[1];
+            }
+        }
+
+        // find parent
+        lfs_stag_t tag = lfs_fs_parent(lfs, lpair, &pdir);
+        if (tag < 0 && tag != LFS_ERR_NOENT) {
+            return tag;
+        }
+
+        bool hasparent = (tag != LFS_ERR_NOENT);
+        if (tag != LFS_ERR_NOENT) {
+            // note that if we have a parent, we must have a pred, so this will
+            // always create an orphan
+            int err = lfs_fs_preporphans(lfs, +1);
+            if (err) {
+                return err;
+            }
+
+            // fix pending move in this pair? this looks like an optimization but
+            // is in fact _required_ since relocating may outdate the move.
+            uint16_t moveid = 0x3ff;
+            if (lfs_gstate_hasmovehere(&lfs->gstate, pdir.pair)) {
+                moveid = lfs_tag_id(lfs->gstate.tag);
+                LFS_DEBUG("Fixing move while relocating "
+                        "{0x%"PRIx32", 0x%"PRIx32"} 0x%"PRIx16"\n",
+                        pdir.pair[0], pdir.pair[1], moveid);
+                lfs_fs_prepmove(lfs, 0x3ff, NULL);
+                if (moveid < lfs_tag_id(tag)) {
+                    tag -= LFS_MKTAG(0, 1, 0);
+                }
+            }
+
+            lfs_block_t ppair[2] = {pdir.pair[0], pdir.pair[1]};
+            lfs_pair_tole32(ldir.pair);
+            state = lfs_dir_relocatingcommit(lfs, &pdir, ppair, LFS_MKATTRS(
+                        {LFS_MKTAG_IF(moveid != 0x3ff,
+                            LFS_TYPE_DELETE, moveid, 0), NULL},
+                        {tag, ldir.pair}),
+                    NULL);
+            lfs_pair_fromle32(ldir.pair);
+            if (state < 0) {
+                return state;
+            }
+
+            if (state == LFS_OK_RELOCATED) {
+                lpair[0] = ppair[0];
+                lpair[1] = ppair[1];
+                ldir = pdir;
+                orphans = true;
+                continue;
+            }
+        }
+
+        // find pred
+        int err = lfs_fs_pred(lfs, lpair, &pdir);
+        if (err && err != LFS_ERR_NOENT) {
+            return err;
+        }
+        LFS_ASSERT(!(hasparent && err == LFS_ERR_NOENT));
+
+        // if we can't find dir, it must be new
+        if (err != LFS_ERR_NOENT) {
+            if (lfs_gstate_hasorphans(&lfs->gstate)) {
+                // next step, clean up orphans
+                err = lfs_fs_preporphans(lfs, -hasparent);
+                if (err) {
+                    return err;
+                }
+            }
+
+            // fix pending move in this pair? this looks like an optimization
+            // but is in fact _required_ since relocating may outdate the move.
+            uint16_t moveid = 0x3ff;
+            if (lfs_gstate_hasmovehere(&lfs->gstate, pdir.pair)) {
+                moveid = lfs_tag_id(lfs->gstate.tag);
+                LFS_DEBUG("Fixing move while relocating "
+                        "{0x%"PRIx32", 0x%"PRIx32"} 0x%"PRIx16"\n",
+                        pdir.pair[0], pdir.pair[1], moveid);
+                lfs_fs_prepmove(lfs, 0x3ff, NULL);
+            }
+
+            // replace bad pair, either we clean up desync, or no desync occured
+            lpair[0] = pdir.pair[0];
+            lpair[1] = pdir.pair[1];
+            lfs_pair_tole32(ldir.pair);
+            state = lfs_dir_relocatingcommit(lfs, &pdir, lpair, LFS_MKATTRS(
+                        {LFS_MKTAG_IF(moveid != 0x3ff,
+                            LFS_TYPE_DELETE, moveid, 0), NULL},
+                        {LFS_MKTAG(LFS_TYPE_TAIL + pdir.split, 0x3ff, 8),
+                            ldir.pair}),
+                    NULL);
+            lfs_pair_fromle32(ldir.pair);
+            if (state < 0) {
+                return state;
+            }
+
+            ldir = pdir;
+        }
+    }
+
+    return orphans ? LFS_OK_ORPHANED : 0;
+}
+#endif
+
+#ifndef LFS_READONLY
+static int lfs_dir_commit(lfs_t *lfs, lfs_mdir_t *dir,
+        const struct lfs_mattr *attrs, int attrcount) {
+    int orphans = lfs_dir_orphaningcommit(lfs, dir, attrs, attrcount);
+    if (orphans < 0) {
+        return orphans;
+    }
+
+    if (orphans) {
+        // make sure we've removed all orphans, this is a noop if there
+        // are none, but if we had nested blocks failures we may have
+        // created some
+        int err = lfs_fs_deorphan(lfs, false);
+        if (err) {
+            return err;
+        }
+    }
+
     return 0;
 }
 #endif
 
 
 /// Top level directory operations ///
 #ifndef LFS_READONLY
@@ -2059,15 +2548,15 @@
     err = lfs_dir_commit(lfs, &dir, LFS_MKATTRS(
             {LFS_MKTAG(LFS_TYPE_SOFTTAIL, 0x3ff, 8), pred.tail}));
     lfs_pair_fromle32(pred.tail);
     if (err) {
         return err;
     }
 
-    // current block end of list?
+    // current block not end of list?
     if (cwd.m.split) {
         // update tails, this creates a desync
         err = lfs_fs_preporphans(lfs, +1);
         if (err) {
             return err;
         }
 
@@ -2219,31 +2708,31 @@
     dir->pos = lfs_min(2, off);
     off -= dir->pos;
 
     // skip superblock entry
     dir->id = (off > 0 && lfs_pair_cmp(dir->head, lfs->root) == 0);
 
     while (off > 0) {
-        int diff = lfs_min(dir->m.count - dir->id, off);
-        dir->id += diff;
-        dir->pos += diff;
-        off -= diff;
-
         if (dir->id == dir->m.count) {
             if (!dir->m.split) {
                 return LFS_ERR_INVAL;
             }
 
             err = lfs_dir_fetch(lfs, &dir->m, dir->m.tail);
             if (err) {
                 return err;
             }
 
             dir->id = 0;
         }
+
+        int diff = lfs_min(dir->m.count - dir->id, off);
+        dir->id += diff;
+        dir->pos += diff;
+        off -= diff;
     }
 
     return 0;
 }
 
 static lfs_soff_t lfs_dir_rawtell(lfs_t *lfs, lfs_dir_t *dir) {
     (void)lfs;
@@ -2509,16 +2998,19 @@
         }
 
         // get next slot and create entry to remember name
         err = lfs_dir_commit(lfs, &file->m, LFS_MKATTRS(
                 {LFS_MKTAG(LFS_TYPE_CREATE, file->id, 0), NULL},
                 {LFS_MKTAG(LFS_TYPE_REG, file->id, nlen), path},
                 {LFS_MKTAG(LFS_TYPE_INLINESTRUCT, file->id, 0), NULL}));
+
+        // it may happen that the file name doesn't fit in the metadata blocks, e.g., a 256 byte file name will
+        // not fit in a 128 byte block.
+        err = (err == LFS_ERR_NOSPC) ? LFS_ERR_NAMETOOLONG : err;
         if (err) {
-            err = LFS_ERR_NAMETOOLONG;
             goto cleanup;
         }
 
         tag = LFS_MKTAG(LFS_TYPE_INLINESTRUCT, 0, 0);
     } else if (flags & LFS_O_EXCL) {
         err = LFS_ERR_EXIST;
         goto cleanup;
@@ -2615,20 +3107,22 @@
 #ifndef LFS_READONLY
     file->flags |= LFS_F_ERRED;
 #endif
     lfs_file_rawclose(lfs, file);
     return err;
 }
 
+#ifndef LFS_NO_MALLOC
 static int lfs_file_rawopen(lfs_t *lfs, lfs_file_t *file,
         const char *path, int flags) {
     static const struct lfs_file_config defaults = {0};
     int err = lfs_file_rawopencfg(lfs, file, path, flags, &defaults);
     return err;
 }
+#endif
 
 static int lfs_file_rawclose(lfs_t *lfs, lfs_file_t *file) {
 #ifndef LFS_READONLY
     int err = lfs_file_rawsync(lfs, file);
 #else
     int err = 0;
 #endif
@@ -2726,23 +3220,23 @@
     }
 
     file->flags &= ~LFS_F_INLINE;
     return 0;
 }
 #endif
 
-#ifndef LFS_READONLY
 static int lfs_file_flush(lfs_t *lfs, lfs_file_t *file) {
     if (file->flags & LFS_F_READING) {
         if (!(file->flags & LFS_F_INLINE)) {
             lfs_cache_drop(lfs, &file->cache);
         }
         file->flags &= ~LFS_F_READING;
     }
 
+#ifndef LFS_READONLY
     if (file->flags & LFS_F_WRITING) {
         lfs_off_t pos = file->pos;
 
         if (!(file->flags & LFS_F_INLINE)) {
             // copy over anything after current branch
             lfs_file_t orig = {
                 .ctz.head = file->ctz.head,
@@ -2753,20 +3247,20 @@
             };
             lfs_cache_drop(lfs, &lfs->rcache);
 
             while (file->pos < file->ctz.size) {
                 // copy over a byte at a time, leave it up to caching
                 // to make this efficient
                 uint8_t data;
-                lfs_ssize_t res = lfs_file_rawread(lfs, &orig, &data, 1);
+                lfs_ssize_t res = lfs_file_flushedread(lfs, &orig, &data, 1);
                 if (res < 0) {
                     return res;
                 }
 
-                res = lfs_file_rawwrite(lfs, file, &data, 1);
+                res = lfs_file_flushedwrite(lfs, file, &data, 1);
                 if (res < 0) {
                     return res;
                 }
 
                 // keep our reference to the rcache in sync
                 if (lfs->rcache.block != LFS_BLOCK_NULL) {
                     lfs_cache_drop(lfs, &orig.cache);
@@ -2801,18 +3295,18 @@
         file->ctz.head = file->block;
         file->ctz.size = file->pos;
         file->flags &= ~LFS_F_WRITING;
         file->flags |= LFS_F_DIRTY;
 
         file->pos = pos;
     }
+#endif
 
     return 0;
 }
-#endif
 
 #ifndef LFS_READONLY
 static int lfs_file_rawsync(lfs_t *lfs, lfs_file_t *file) {
     if (file->flags & LFS_F_ERRED) {
         // it's not safe to do anything if our file errored
         return 0;
     }
@@ -2859,31 +3353,19 @@
         file->flags &= ~LFS_F_DIRTY;
     }
 
     return 0;
 }
 #endif
 
-static lfs_ssize_t lfs_file_rawread(lfs_t *lfs, lfs_file_t *file,
+static lfs_ssize_t lfs_file_flushedread(lfs_t *lfs, lfs_file_t *file,
         void *buffer, lfs_size_t size) {
-    LFS_ASSERT((file->flags & LFS_O_RDONLY) == LFS_O_RDONLY);
-
     uint8_t *data = buffer;
     lfs_size_t nsize = size;
 
-#ifndef LFS_READONLY
-    if (file->flags & LFS_F_WRITING) {
-        // flush out any writes
-        int err = lfs_file_flush(lfs, file);
-        if (err) {
-            return err;
-        }
-    }
-#endif
-
     if (file->pos >= file->ctz.size) {
         // eof if past end
         return 0;
     }
 
     size = lfs_min(size, file->ctz.size - file->pos);
     nsize = size;
@@ -2932,51 +3414,37 @@
         data += diff;
         nsize -= diff;
     }
 
     return size;
 }
 
-#ifndef LFS_READONLY
-static lfs_ssize_t lfs_file_rawwrite(lfs_t *lfs, lfs_file_t *file,
-        const void *buffer, lfs_size_t size) {
-    LFS_ASSERT((file->flags & LFS_O_WRONLY) == LFS_O_WRONLY);
-
-    const uint8_t *data = buffer;
-    lfs_size_t nsize = size;
+static lfs_ssize_t lfs_file_rawread(lfs_t *lfs, lfs_file_t *file,
+        void *buffer, lfs_size_t size) {
+    LFS_ASSERT((file->flags & LFS_O_RDONLY) == LFS_O_RDONLY);
 
-    if (file->flags & LFS_F_READING) {
-        // drop any reads
+#ifndef LFS_READONLY
+    if (file->flags & LFS_F_WRITING) {
+        // flush out any writes
         int err = lfs_file_flush(lfs, file);
         if (err) {
             return err;
         }
     }
+#endif
 
-    if ((file->flags & LFS_O_APPEND) && file->pos < file->ctz.size) {
-        file->pos = file->ctz.size;
-    }
-
-    if (file->pos + size > lfs->file_max) {
-        // Larger than file limit?
-        return LFS_ERR_FBIG;
-    }
+    return lfs_file_flushedread(lfs, file, buffer, size);
+}
 
-    if (!(file->flags & LFS_F_WRITING) && file->pos > file->ctz.size) {
-        // fill with zeros
-        lfs_off_t pos = file->pos;
-        file->pos = file->ctz.size;
 
-        while (file->pos < pos) {
-            lfs_ssize_t res = lfs_file_rawwrite(lfs, file, &(uint8_t){0}, 1);
-            if (res < 0) {
-                return res;
-            }
-        }
-    }
+#ifndef LFS_READONLY
+static lfs_ssize_t lfs_file_flushedwrite(lfs_t *lfs, lfs_file_t *file,
+        const void *buffer, lfs_size_t size) {
+    const uint8_t *data = buffer;
+    lfs_size_t nsize = size;
 
     if ((file->flags & LFS_F_INLINE) &&
             lfs_max(file->pos+nsize, file->ctz.size) >
             lfs_min(0x3fe, lfs_min(
                 lfs->cfg->cache_size,
                 (lfs->cfg->metadata_max ?
                     lfs->cfg->metadata_max : lfs->cfg->block_size) / 8))) {
@@ -2993,15 +3461,15 @@
         if (!(file->flags & LFS_F_WRITING) ||
                 file->off == lfs->cfg->block_size) {
             if (!(file->flags & LFS_F_INLINE)) {
                 if (!(file->flags & LFS_F_WRITING) && file->pos > 0) {
                     // find out which block we're extending from
                     int err = lfs_ctz_find(lfs, NULL, &file->cache,
                             file->ctz.head, file->ctz.size,
-                            file->pos-1, &file->block, &file->off);
+                            file->pos-1, &file->block, &(lfs_off_t){0});
                     if (err) {
                         file->flags |= LFS_F_ERRED;
                         return err;
                     }
 
                     // mark cache as dirty since we may have read data into it
                     lfs_cache_zero(lfs, &file->cache);
@@ -3050,48 +3518,118 @@
         file->off += diff;
         data += diff;
         nsize -= diff;
 
         lfs_alloc_ack(lfs);
     }
 
-    file->flags &= ~LFS_F_ERRED;
     return size;
 }
+
+static lfs_ssize_t lfs_file_rawwrite(lfs_t *lfs, lfs_file_t *file,
+        const void *buffer, lfs_size_t size) {
+    LFS_ASSERT((file->flags & LFS_O_WRONLY) == LFS_O_WRONLY);
+
+    if (file->flags & LFS_F_READING) {
+        // drop any reads
+        int err = lfs_file_flush(lfs, file);
+        if (err) {
+            return err;
+        }
+    }
+
+    if ((file->flags & LFS_O_APPEND) && file->pos < file->ctz.size) {
+        file->pos = file->ctz.size;
+    }
+
+    if (file->pos + size > lfs->file_max) {
+        // Larger than file limit?
+        return LFS_ERR_FBIG;
+    }
+
+    if (!(file->flags & LFS_F_WRITING) && file->pos > file->ctz.size) {
+        // fill with zeros
+        lfs_off_t pos = file->pos;
+        file->pos = file->ctz.size;
+
+        while (file->pos < pos) {
+            lfs_ssize_t res = lfs_file_flushedwrite(lfs, file, &(uint8_t){0}, 1);
+            if (res < 0) {
+                return res;
+            }
+        }
+    }
+
+    lfs_ssize_t nsize = lfs_file_flushedwrite(lfs, file, buffer, size);
+    if (nsize < 0) {
+        return nsize;
+    }
+
+    file->flags &= ~LFS_F_ERRED;
+    return nsize;
+}
 #endif
 
 static lfs_soff_t lfs_file_rawseek(lfs_t *lfs, lfs_file_t *file,
         lfs_soff_t off, int whence) {
     // find new pos
     lfs_off_t npos = file->pos;
     if (whence == LFS_SEEK_SET) {
         npos = off;
     } else if (whence == LFS_SEEK_CUR) {
-        npos = file->pos + off;
+        if ((lfs_soff_t)file->pos + off < 0) {
+            return LFS_ERR_INVAL;
+        } else {
+            npos = file->pos + off;
+        }
     } else if (whence == LFS_SEEK_END) {
-        npos = lfs_file_rawsize(lfs, file) + off;
+        lfs_soff_t res = lfs_file_rawsize(lfs, file) + off;
+        if (res < 0) {
+            return LFS_ERR_INVAL;
+        } else {
+            npos = res;
+        }
     }
 
     if (npos > lfs->file_max) {
         // file position out of range
         return LFS_ERR_INVAL;
     }
 
     if (file->pos == npos) {
         // noop - position has not changed
         return npos;
     }
 
+    // if we're only reading and our new offset is still in the file's cache
+    // we can avoid flushing and needing to reread the data
+    if (
 #ifndef LFS_READONLY
+        !(file->flags & LFS_F_WRITING)
+#else
+        true
+#endif
+            ) {
+        int oindex = lfs_ctz_index(lfs, &(lfs_off_t){file->pos});
+        lfs_off_t noff = npos;
+        int nindex = lfs_ctz_index(lfs, &noff);
+        if (oindex == nindex
+                && noff >= file->cache.off
+                && noff < file->cache.off + file->cache.size) {
+            file->pos = npos;
+            file->off = noff;
+            return npos;
+        }
+    }
+
     // write out everything beforehand, may be noop if rdonly
     int err = lfs_file_flush(lfs, file);
     if (err) {
         return err;
     }
-#endif
 
     // update pos
     file->pos = npos;
     return npos;
 }
 
 #ifndef LFS_READONLY
@@ -3101,34 +3639,63 @@
     if (size > LFS_FILE_MAX) {
         return LFS_ERR_INVAL;
     }
 
     lfs_off_t pos = file->pos;
     lfs_off_t oldsize = lfs_file_rawsize(lfs, file);
     if (size < oldsize) {
-        // need to flush since directly changing metadata
-        int err = lfs_file_flush(lfs, file);
-        if (err) {
-            return err;
-        }
+        // revert to inline file?
+        if (size <= lfs_min(0x3fe, lfs_min(
+                lfs->cfg->cache_size,
+                (lfs->cfg->metadata_max ?
+                    lfs->cfg->metadata_max : lfs->cfg->block_size) / 8))) {
+            // flush+seek to head
+            lfs_soff_t res = lfs_file_rawseek(lfs, file, 0, LFS_SEEK_SET);
+            if (res < 0) {
+                return (int)res;
+            }
 
-        // lookup new head in ctz skip list
-        err = lfs_ctz_find(lfs, NULL, &file->cache,
-                file->ctz.head, file->ctz.size,
-                size, &file->block, &file->off);
-        if (err) {
-            return err;
-        }
+            // read our data into rcache temporarily
+            lfs_cache_drop(lfs, &lfs->rcache);
+            res = lfs_file_flushedread(lfs, file,
+                    lfs->rcache.buffer, size);
+            if (res < 0) {
+                return (int)res;
+            }
 
-        // need to set pos/block/off consistently so seeking back to
-        // the old position does not get confused
-        file->pos = size;
-        file->ctz.head = file->block;
-        file->ctz.size = size;
-        file->flags |= LFS_F_DIRTY | LFS_F_READING;
+            file->ctz.head = LFS_BLOCK_INLINE;
+            file->ctz.size = size;
+            file->flags |= LFS_F_DIRTY | LFS_F_READING | LFS_F_INLINE;
+            file->cache.block = file->ctz.head;
+            file->cache.off = 0;
+            file->cache.size = lfs->cfg->cache_size;
+            memcpy(file->cache.buffer, lfs->rcache.buffer, size);
+
+        } else {
+            // need to flush since directly changing metadata
+            int err = lfs_file_flush(lfs, file);
+            if (err) {
+                return err;
+            }
+
+            // lookup new head in ctz skip list
+            err = lfs_ctz_find(lfs, NULL, &file->cache,
+                    file->ctz.head, file->ctz.size,
+                    size-1, &file->block, &(lfs_off_t){0});
+            if (err) {
+                return err;
+            }
+
+            // need to set pos/block/off consistently so seeking back to
+            // the old position does not get confused
+            file->pos = size;
+            file->ctz.head = file->block;
+            file->ctz.size = size;
+            file->flags |= LFS_F_DIRTY | LFS_F_READING;
+        }
     } else if (size > oldsize) {
         // flush+seek if not already at end
         lfs_soff_t res = lfs_file_rawseek(lfs, file, 0, LFS_SEEK_END);
         if (res < 0) {
             return (int)res;
         }
 
@@ -3377,15 +3944,16 @@
         if (err) {
             lfs->mlist = prevdir.next;
             return err;
         }
     }
 
     lfs->mlist = prevdir.next;
-    if (prevtag != LFS_ERR_NOENT && lfs_tag_type3(prevtag) == LFS_TYPE_DIR) {
+    if (prevtag != LFS_ERR_NOENT
+            && lfs_tag_type3(prevtag) == LFS_TYPE_DIR) {
         // fix orphan
         err = lfs_fs_preporphans(lfs, -1);
         if (err) {
             return err;
         }
 
         err = lfs_fs_pred(lfs, prevdir.m.pair, &newcwd);
@@ -3479,27 +4047,36 @@
 
 
 /// Filesystem operations ///
 static int lfs_init(lfs_t *lfs, const struct lfs_config *cfg) {
     lfs->cfg = cfg;
     int err = 0;
 
+    // check that bool is a truthy-preserving type
+    //
+    // note the most common reason for this failure is a before-c99 compiler,
+    // which littlefs currently does not support
+    LFS_ASSERT((bool)0x80000000);
+
     // validate that the lfs-cfg sizes were initiated properly before
     // performing any arithmetic logics with them
     LFS_ASSERT(lfs->cfg->read_size != 0);
     LFS_ASSERT(lfs->cfg->prog_size != 0);
     LFS_ASSERT(lfs->cfg->cache_size != 0);
 
     // check that block size is a multiple of cache size is a multiple
     // of prog and read sizes
     LFS_ASSERT(lfs->cfg->cache_size % lfs->cfg->read_size == 0);
     LFS_ASSERT(lfs->cfg->cache_size % lfs->cfg->prog_size == 0);
     LFS_ASSERT(lfs->cfg->block_size % lfs->cfg->cache_size == 0);
 
-    // check that the block size is large enough to fit ctz pointers
+    // check that the block size is large enough to fit all ctz pointers
+    LFS_ASSERT(lfs->cfg->block_size >= 128);
+    // this is the exact calculation for all ctz pointers, if this fails
+    // and the simpler assert above does not, math must be broken
     LFS_ASSERT(4*lfs_npw2(0xffffffff / (lfs->cfg->block_size-2*4))
             <= lfs->cfg->block_size);
 
     // block_cycles = 0 is no longer supported.
     //
     // block_cycles is the number of erase cycles before littlefs evicts
     // metadata logs as a part of wear leveling. Suggested values are in the
@@ -3675,22 +4252,31 @@
     int err = lfs_init(lfs, cfg);
     if (err) {
         return err;
     }
 
     // scan directory blocks for superblock and any global updates
     lfs_mdir_t dir = {.tail = {0, 1}};
-    lfs_block_t cycle = 0;
+    lfs_block_t tortoise[2] = {LFS_BLOCK_NULL, LFS_BLOCK_NULL};
+    lfs_size_t tortoise_i = 1;
+    lfs_size_t tortoise_period = 1;
     while (!lfs_pair_isnull(dir.tail)) {
-        if (cycle >= lfs->cfg->block_count/2) {
-            // loop detected
+        // detect cycles with Brent's algorithm
+        if (lfs_pair_issync(dir.tail, tortoise)) {
+            LFS_WARN("Cycle detected in tail list");
             err = LFS_ERR_CORRUPT;
             goto cleanup;
         }
-        cycle += 1;
+        if (tortoise_i == tortoise_period) {
+            tortoise[0] = dir.tail[0];
+            tortoise[1] = dir.tail[1];
+            tortoise_i = 0;
+            tortoise_period *= 2;
+        }
+        tortoise_i += 1;
 
         // fetch next block in tail list
         lfs_stag_t tag = lfs_dir_fetchmatch(lfs, &dir, dir.tail,
                 LFS_MKTAG(0x7ff, 0x3ff, 0),
                 LFS_MKTAG(LFS_TYPE_SUPERBLOCK, 0, 8),
                 NULL,
                 lfs_dir_find_match, &(struct lfs_dir_find_match){
@@ -3718,20 +4304,37 @@
             lfs_superblock_fromle32(&superblock);
 
             // check version
             uint16_t major_version = (0xffff & (superblock.version >> 16));
             uint16_t minor_version = (0xffff & (superblock.version >>  0));
             if ((major_version != LFS_DISK_VERSION_MAJOR ||
                  minor_version > LFS_DISK_VERSION_MINOR)) {
-                LFS_ERROR("Invalid version v%"PRIu16".%"PRIu16,
-                        major_version, minor_version);
+                LFS_ERROR("Invalid version "
+                        "v%"PRIu16".%"PRIu16" != v%"PRIu16".%"PRIu16,
+                        major_version, minor_version,
+                        LFS_DISK_VERSION_MAJOR, LFS_DISK_VERSION_MINOR);
                 err = LFS_ERR_INVAL;
                 goto cleanup;
             }
 
+            // found older minor version? set an in-device only bit in the
+            // gstate so we know we need to rewrite the superblock before
+            // the first write
+            if (minor_version < LFS_DISK_VERSION_MINOR) {
+                LFS_DEBUG("Found older minor version "
+                        "v%"PRIu16".%"PRIu16" < v%"PRIu16".%"PRIu16,
+                        major_version, minor_version,
+                        LFS_DISK_VERSION_MAJOR, LFS_DISK_VERSION_MINOR);
+            #ifndef LFS_READONLY
+                // note this bit is reserved on disk, so fetching more gstate
+                // will not interfere here
+                lfs_fs_prepsuperblock(lfs, true);
+            #endif
+            }
+
             // check superblock configuration
             if (superblock.name_max) {
                 if (superblock.name_max > lfs->name_max) {
                     LFS_ERROR("Unsupported name_max (%"PRIu32" > %"PRIu32")",
                             superblock.name_max, lfs->name_max);
                     err = LFS_ERR_INVAL;
                     goto cleanup;
@@ -3757,14 +4360,28 @@
                             superblock.attr_max, lfs->attr_max);
                     err = LFS_ERR_INVAL;
                     goto cleanup;
                 }
 
                 lfs->attr_max = superblock.attr_max;
             }
+
+            if (superblock.block_count != lfs->cfg->block_count) {
+                LFS_ERROR("Invalid block count (%"PRIu32" != %"PRIu32")",
+                        superblock.block_count, lfs->cfg->block_count);
+                err = LFS_ERR_INVAL;
+                goto cleanup;
+            }
+
+            if (superblock.block_size != lfs->cfg->block_size) {
+                LFS_ERROR("Invalid block size (%"PRIu32" != %"PRIu32")",
+                        superblock.block_size, lfs->cfg->block_size);
+                err = LFS_ERR_INVAL;
+                goto cleanup;
+            }
         }
 
         // has gstate?
         err = lfs_dir_getgstate(lfs, &dir, &lfs->gstate);
         if (err) {
             goto cleanup;
         }
@@ -3819,21 +4436,30 @@
         }
 
         dir.tail[0] = lfs->root[0];
         dir.tail[1] = lfs->root[1];
     }
 #endif
 
-    lfs_block_t cycle = 0;
+    lfs_block_t tortoise[2] = {LFS_BLOCK_NULL, LFS_BLOCK_NULL};
+    lfs_size_t tortoise_i = 1;
+    lfs_size_t tortoise_period = 1;
     while (!lfs_pair_isnull(dir.tail)) {
-        if (cycle >= lfs->cfg->block_count/2) {
-            // loop detected
+        // detect cycles with Brent's algorithm
+        if (lfs_pair_issync(dir.tail, tortoise)) {
+            LFS_WARN("Cycle detected in tail list");
             return LFS_ERR_CORRUPT;
         }
-        cycle += 1;
+        if (tortoise_i == tortoise_period) {
+            tortoise[0] = dir.tail[0];
+            tortoise[1] = dir.tail[1];
+            tortoise_i = 0;
+            tortoise_period *= 2;
+        }
+        tortoise_i += 1;
 
         for (int i = 0; i < 2; i++) {
             int err = cb(data, dir.tail[i]);
             if (err) {
                 return err;
             }
         }
@@ -3904,21 +4530,30 @@
 
 #ifndef LFS_READONLY
 static int lfs_fs_pred(lfs_t *lfs,
         const lfs_block_t pair[2], lfs_mdir_t *pdir) {
     // iterate over all directory directory entries
     pdir->tail[0] = 0;
     pdir->tail[1] = 1;
-    lfs_block_t cycle = 0;
+    lfs_block_t tortoise[2] = {LFS_BLOCK_NULL, LFS_BLOCK_NULL};
+    lfs_size_t tortoise_i = 1;
+    lfs_size_t tortoise_period = 1;
     while (!lfs_pair_isnull(pdir->tail)) {
-        if (cycle >= lfs->cfg->block_count/2) {
-            // loop detected
+        // detect cycles with Brent's algorithm
+        if (lfs_pair_issync(pdir->tail, tortoise)) {
+            LFS_WARN("Cycle detected in tail list");
             return LFS_ERR_CORRUPT;
         }
-        cycle += 1;
+        if (tortoise_i == tortoise_period) {
+            tortoise[0] = pdir->tail[0];
+            tortoise[1] = pdir->tail[1];
+            tortoise_i = 0;
+            tortoise_period *= 2;
+        }
+        tortoise_i += 1;
 
         if (lfs_pair_cmp(pdir->tail, pair) == 0) {
             return 0;
         }
 
         int err = lfs_dir_fetch(lfs, pdir, pdir->tail);
         if (err) {
@@ -3960,21 +4595,30 @@
 
 #ifndef LFS_READONLY
 static lfs_stag_t lfs_fs_parent(lfs_t *lfs, const lfs_block_t pair[2],
         lfs_mdir_t *parent) {
     // use fetchmatch with callback to find pairs
     parent->tail[0] = 0;
     parent->tail[1] = 1;
-    lfs_block_t cycle = 0;
+    lfs_block_t tortoise[2] = {LFS_BLOCK_NULL, LFS_BLOCK_NULL};
+    lfs_size_t tortoise_i = 1;
+    lfs_size_t tortoise_period = 1;
     while (!lfs_pair_isnull(parent->tail)) {
-        if (cycle >= lfs->cfg->block_count/2) {
-            // loop detected
+        // detect cycles with Brent's algorithm
+        if (lfs_pair_issync(parent->tail, tortoise)) {
+            LFS_WARN("Cycle detected in tail list");
             return LFS_ERR_CORRUPT;
         }
-        cycle += 1;
+        if (tortoise_i == tortoise_period) {
+            tortoise[0] = parent->tail[0];
+            tortoise[1] = parent->tail[1];
+            tortoise_i = 0;
+            tortoise_period *= 2;
+        }
+        tortoise_i += 1;
 
         lfs_stag_t tag = lfs_dir_fetchmatch(lfs, parent, parent->tail,
                 LFS_MKTAG(0x7ff, 0, 0x3ff),
                 LFS_MKTAG(LFS_TYPE_DIRSTRUCT, 0, 8),
                 NULL,
                 lfs_fs_parent_match, &(struct lfs_fs_parent_match){
                     lfs, {pair[0], pair[1]}});
@@ -3984,119 +4628,24 @@
     }
 
     return LFS_ERR_NOENT;
 }
 #endif
 
 #ifndef LFS_READONLY
-static int lfs_fs_relocate(lfs_t *lfs,
-        const lfs_block_t oldpair[2], lfs_block_t newpair[2]) {
-    // update internal root
-    if (lfs_pair_cmp(oldpair, lfs->root) == 0) {
-        lfs->root[0] = newpair[0];
-        lfs->root[1] = newpair[1];
-    }
-
-    // update internally tracked dirs
-    for (struct lfs_mlist *d = lfs->mlist; d; d = d->next) {
-        if (lfs_pair_cmp(oldpair, d->m.pair) == 0) {
-            d->m.pair[0] = newpair[0];
-            d->m.pair[1] = newpair[1];
-        }
-
-        if (d->type == LFS_TYPE_DIR &&
-                lfs_pair_cmp(oldpair, ((lfs_dir_t*)d)->head) == 0) {
-            ((lfs_dir_t*)d)->head[0] = newpair[0];
-            ((lfs_dir_t*)d)->head[1] = newpair[1];
-        }
-    }
-
-    // find parent
-    lfs_mdir_t parent;
-    lfs_stag_t tag = lfs_fs_parent(lfs, oldpair, &parent);
-    if (tag < 0 && tag != LFS_ERR_NOENT) {
-        return tag;
-    }
-
-    if (tag != LFS_ERR_NOENT) {
-        // update disk, this creates a desync
-        int err = lfs_fs_preporphans(lfs, +1);
-        if (err) {
-            return err;
-        }
-
-        // fix pending move in this pair? this looks like an optimization but
-        // is in fact _required_ since relocating may outdate the move.
-        uint16_t moveid = 0x3ff;
-        if (lfs_gstate_hasmovehere(&lfs->gstate, parent.pair)) {
-            moveid = lfs_tag_id(lfs->gstate.tag);
-            LFS_DEBUG("Fixing move while relocating "
-                    "{0x%"PRIx32", 0x%"PRIx32"} 0x%"PRIx16"\n",
-                    parent.pair[0], parent.pair[1], moveid);
-            lfs_fs_prepmove(lfs, 0x3ff, NULL);
-            if (moveid < lfs_tag_id(tag)) {
-                tag -= LFS_MKTAG(0, 1, 0);
-            }
-        }
-
-        lfs_pair_tole32(newpair);
-        err = lfs_dir_commit(lfs, &parent, LFS_MKATTRS(
-                {LFS_MKTAG_IF(moveid != 0x3ff,
-                    LFS_TYPE_DELETE, moveid, 0), NULL},
-                {tag, newpair}));
-        lfs_pair_fromle32(newpair);
-        if (err) {
-            return err;
-        }
-
-        // next step, clean up orphans
-        err = lfs_fs_preporphans(lfs, -1);
-        if (err) {
-            return err;
-        }
-    }
-
-    // find pred
-    int err = lfs_fs_pred(lfs, oldpair, &parent);
-    if (err && err != LFS_ERR_NOENT) {
-        return err;
-    }
-
-    // if we can't find dir, it must be new
-    if (err != LFS_ERR_NOENT) {
-        // fix pending move in this pair? this looks like an optimization but
-        // is in fact _required_ since relocating may outdate the move.
-        uint16_t moveid = 0x3ff;
-        if (lfs_gstate_hasmovehere(&lfs->gstate, parent.pair)) {
-            moveid = lfs_tag_id(lfs->gstate.tag);
-            LFS_DEBUG("Fixing move while relocating "
-                    "{0x%"PRIx32", 0x%"PRIx32"} 0x%"PRIx16"\n",
-                    parent.pair[0], parent.pair[1], moveid);
-            lfs_fs_prepmove(lfs, 0x3ff, NULL);
-        }
-
-        // replace bad pair, either we clean up desync, or no desync occured
-        lfs_pair_tole32(newpair);
-        err = lfs_dir_commit(lfs, &parent, LFS_MKATTRS(
-                {LFS_MKTAG_IF(moveid != 0x3ff,
-                    LFS_TYPE_DELETE, moveid, 0), NULL},
-                {LFS_MKTAG(LFS_TYPE_TAIL + parent.split, 0x3ff, 8), newpair}));
-        lfs_pair_fromle32(newpair);
-        if (err) {
-            return err;
-        }
-    }
-
-    return 0;
+static void lfs_fs_prepsuperblock(lfs_t *lfs, bool needssuperblock) {
+    lfs->gstate.tag = (lfs->gstate.tag & ~LFS_MKTAG(0, 0, 0x200))
+            | (uint32_t)needssuperblock << 9;
 }
 #endif
 
 #ifndef LFS_READONLY
 static int lfs_fs_preporphans(lfs_t *lfs, int8_t orphans) {
-    LFS_ASSERT(lfs_tag_size(lfs->gstate.tag) > 0 || orphans >= 0);
+    LFS_ASSERT(lfs_tag_size(lfs->gstate.tag) > 0x000 || orphans >= 0);
+    LFS_ASSERT(lfs_tag_size(lfs->gstate.tag) < 0x1ff || orphans <= 0);
     lfs->gstate.tag += orphans;
     lfs->gstate.tag = ((lfs->gstate.tag & ~LFS_MKTAG(0x800, 0, 0)) |
             ((uint32_t)lfs_gstate_hasorphans(&lfs->gstate) << 31));
 
     return 0;
 }
 #endif
@@ -4108,25 +4657,68 @@
             ((id != 0x3ff) ? LFS_MKTAG(LFS_TYPE_DELETE, id, 0) : 0));
     lfs->gstate.pair[0] = (id != 0x3ff) ? pair[0] : 0;
     lfs->gstate.pair[1] = (id != 0x3ff) ? pair[1] : 0;
 }
 #endif
 
 #ifndef LFS_READONLY
+static int lfs_fs_desuperblock(lfs_t *lfs) {
+    if (!lfs_gstate_needssuperblock(&lfs->gstate)) {
+        return 0;
+    }
+
+    LFS_DEBUG("Rewriting superblock {0x%"PRIx32", 0x%"PRIx32"}",
+            lfs->root[0],
+            lfs->root[1]);
+
+    lfs_mdir_t root;
+    int err = lfs_dir_fetch(lfs, &root, lfs->root);
+    if (err) {
+        return err;
+    }
+
+    // write a new superblock
+    lfs_superblock_t superblock = {
+        .version     = LFS_DISK_VERSION,
+        .block_size  = lfs->cfg->block_size,
+        .block_count = lfs->cfg->block_count,
+        .name_max    = lfs->name_max,
+        .file_max    = lfs->file_max,
+        .attr_max    = lfs->attr_max,
+    };
+
+    lfs_superblock_tole32(&superblock);
+    err = lfs_dir_commit(lfs, &root, LFS_MKATTRS(
+            {LFS_MKTAG(LFS_TYPE_INLINESTRUCT, 0, sizeof(superblock)),
+                &superblock}));
+    if (err) {
+        return err;
+    }
+
+    lfs_fs_prepsuperblock(lfs, false);
+    return 0;
+}
+#endif
+
+#ifndef LFS_READONLY
 static int lfs_fs_demove(lfs_t *lfs) {
     if (!lfs_gstate_hasmove(&lfs->gdisk)) {
         return 0;
     }
 
     // Fix bad moves
     LFS_DEBUG("Fixing move {0x%"PRIx32", 0x%"PRIx32"} 0x%"PRIx16,
             lfs->gdisk.pair[0],
             lfs->gdisk.pair[1],
             lfs_tag_id(lfs->gdisk.tag));
 
+    // no other gstate is supported at this time, so if we found something else
+    // something most likely went wrong in gstate calculation
+    LFS_ASSERT(lfs_tag_type3(lfs->gdisk.tag) == LFS_TYPE_DELETE);
+
     // fetch and delete the moved entry
     lfs_mdir_t movedir;
     int err = lfs_dir_fetch(lfs, &movedir, lfs->gdisk.pair);
     if (err) {
         return err;
     }
 
@@ -4140,104 +4732,195 @@
     }
 
     return 0;
 }
 #endif
 
 #ifndef LFS_READONLY
-static int lfs_fs_deorphan(lfs_t *lfs) {
+static int lfs_fs_deorphan(lfs_t *lfs, bool powerloss) {
     if (!lfs_gstate_hasorphans(&lfs->gstate)) {
         return 0;
     }
 
-    // Fix any orphans
-    lfs_mdir_t pdir = {.split = true, .tail = {0, 1}};
-    lfs_mdir_t dir;
+    // Check for orphans in two separate passes:
+    // - 1 for half-orphans (relocations)
+    // - 2 for full-orphans (removes/renames)
+    //
+    // Two separate passes are needed as half-orphans can contain outdated
+    // references to full-orphans, effectively hiding them from the deorphan
+    // search.
+    //
+    int pass = 0;
+    while (pass < 2) {
+        // Fix any orphans
+        lfs_mdir_t pdir = {.split = true, .tail = {0, 1}};
+        lfs_mdir_t dir;
+        bool moreorphans = false;
+
+        // iterate over all directory directory entries
+        while (!lfs_pair_isnull(pdir.tail)) {
+            int err = lfs_dir_fetch(lfs, &dir, pdir.tail);
+            if (err) {
+                return err;
+            }
 
-    // iterate over all directory directory entries
-    while (!lfs_pair_isnull(pdir.tail)) {
-        int err = lfs_dir_fetch(lfs, &dir, pdir.tail);
-        if (err) {
-            return err;
-        }
+            // check head blocks for orphans
+            if (!pdir.split) {
+                // check if we have a parent
+                lfs_mdir_t parent;
+                lfs_stag_t tag = lfs_fs_parent(lfs, pdir.tail, &parent);
+                if (tag < 0 && tag != LFS_ERR_NOENT) {
+                    return tag;
+                }
 
-        // check head blocks for orphans
-        if (!pdir.split) {
-            // check if we have a parent
-            lfs_mdir_t parent;
-            lfs_stag_t tag = lfs_fs_parent(lfs, pdir.tail, &parent);
-            if (tag < 0 && tag != LFS_ERR_NOENT) {
-                return tag;
-            }
+                if (pass == 0 && tag != LFS_ERR_NOENT) {
+                    lfs_block_t pair[2];
+                    lfs_stag_t state = lfs_dir_get(lfs, &parent,
+                            LFS_MKTAG(0x7ff, 0x3ff, 0), tag, pair);
+                    if (state < 0) {
+                        return state;
+                    }
+                    lfs_pair_fromle32(pair);
 
-            if (tag == LFS_ERR_NOENT) {
-                // we are an orphan
-                LFS_DEBUG("Fixing orphan {0x%"PRIx32", 0x%"PRIx32"}",
-                        pdir.tail[0], pdir.tail[1]);
+                    if (!lfs_pair_issync(pair, pdir.tail)) {
+                        // we have desynced
+                        LFS_DEBUG("Fixing half-orphan "
+                                "{0x%"PRIx32", 0x%"PRIx32"} "
+                                "-> {0x%"PRIx32", 0x%"PRIx32"}",
+                                pdir.tail[0], pdir.tail[1], pair[0], pair[1]);
+
+                        // fix pending move in this pair? this looks like an
+                        // optimization but is in fact _required_ since
+                        // relocating may outdate the move.
+                        uint16_t moveid = 0x3ff;
+                        if (lfs_gstate_hasmovehere(&lfs->gstate, pdir.pair)) {
+                            moveid = lfs_tag_id(lfs->gstate.tag);
+                            LFS_DEBUG("Fixing move while fixing orphans "
+                                    "{0x%"PRIx32", 0x%"PRIx32"} 0x%"PRIx16"\n",
+                                    pdir.pair[0], pdir.pair[1], moveid);
+                            lfs_fs_prepmove(lfs, 0x3ff, NULL);
+                        }
 
-                err = lfs_dir_drop(lfs, &pdir, &dir);
-                if (err) {
-                    return err;
+                        lfs_pair_tole32(pair);
+                        state = lfs_dir_orphaningcommit(lfs, &pdir, LFS_MKATTRS(
+                                {LFS_MKTAG_IF(moveid != 0x3ff,
+                                    LFS_TYPE_DELETE, moveid, 0), NULL},
+                                {LFS_MKTAG(LFS_TYPE_SOFTTAIL, 0x3ff, 8),
+                                    pair}));
+                        lfs_pair_fromle32(pair);
+                        if (state < 0) {
+                            return state;
+                        }
+
+                        // did our commit create more orphans?
+                        if (state == LFS_OK_ORPHANED) {
+                            moreorphans = true;
+                        }
+
+                        // refetch tail
+                        continue;
+                    }
                 }
 
-                // refetch tail
-                continue;
-            }
+                // note we only check for full orphans if we may have had a
+                // power-loss, otherwise orphans are created intentionally
+                // during operations such as lfs_mkdir
+                if (pass == 1 && tag == LFS_ERR_NOENT && powerloss) {
+                    // we are an orphan
+                    LFS_DEBUG("Fixing orphan {0x%"PRIx32", 0x%"PRIx32"}",
+                            pdir.tail[0], pdir.tail[1]);
 
-            lfs_block_t pair[2];
-            lfs_stag_t res = lfs_dir_get(lfs, &parent,
-                    LFS_MKTAG(0x7ff, 0x3ff, 0), tag, pair);
-            if (res < 0) {
-                return res;
-            }
-            lfs_pair_fromle32(pair);
+                    // steal state
+                    err = lfs_dir_getgstate(lfs, &dir, &lfs->gdelta);
+                    if (err) {
+                        return err;
+                    }
 
-            if (!lfs_pair_sync(pair, pdir.tail)) {
-                // we have desynced
-                LFS_DEBUG("Fixing half-orphan {0x%"PRIx32", 0x%"PRIx32"} "
-                            "-> {0x%"PRIx32", 0x%"PRIx32"}",
-                        pdir.tail[0], pdir.tail[1], pair[0], pair[1]);
-
-                lfs_pair_tole32(pair);
-                err = lfs_dir_commit(lfs, &pdir, LFS_MKATTRS(
-                        {LFS_MKTAG(LFS_TYPE_SOFTTAIL, 0x3ff, 8), pair}));
-                lfs_pair_fromle32(pair);
-                if (err) {
-                    return err;
-                }
+                    // steal tail
+                    lfs_pair_tole32(dir.tail);
+                    int state = lfs_dir_orphaningcommit(lfs, &pdir, LFS_MKATTRS(
+                            {LFS_MKTAG(LFS_TYPE_TAIL + dir.split, 0x3ff, 8),
+                                dir.tail}));
+                    lfs_pair_fromle32(dir.tail);
+                    if (state < 0) {
+                        return state;
+                    }
 
-                // refetch tail
-                continue;
+                    // did our commit create more orphans?
+                    if (state == LFS_OK_ORPHANED) {
+                        moreorphans = true;
+                    }
+
+                    // refetch tail
+                    continue;
+                }
             }
+
+            pdir = dir;
         }
 
-        pdir = dir;
+        pass = moreorphans ? 0 : pass+1;
     }
 
     // mark orphans as fixed
     return lfs_fs_preporphans(lfs, -lfs_gstate_getorphans(&lfs->gstate));
 }
 #endif
 
 #ifndef LFS_READONLY
 static int lfs_fs_forceconsistency(lfs_t *lfs) {
-    int err = lfs_fs_demove(lfs);
+    int err = lfs_fs_desuperblock(lfs);
+    if (err) {
+        return err;
+    }
+
+    err = lfs_fs_demove(lfs);
     if (err) {
         return err;
     }
 
-    err = lfs_fs_deorphan(lfs);
+    err = lfs_fs_deorphan(lfs, true);
     if (err) {
         return err;
     }
 
     return 0;
 }
 #endif
 
+#ifndef LFS_READONLY
+int lfs_fs_rawmkconsistent(lfs_t *lfs) {
+    // lfs_fs_forceconsistency does most of the work here
+    int err = lfs_fs_forceconsistency(lfs);
+    if (err) {
+        return err;
+    }
+
+    // do we have any pending gstate?
+    lfs_gstate_t delta = {0};
+    lfs_gstate_xor(&delta, &lfs->gdisk);
+    lfs_gstate_xor(&delta, &lfs->gstate);
+    if (!lfs_gstate_iszero(&delta)) {
+        // lfs_dir_commit will implicitly write out any pending gstate
+        lfs_mdir_t root;
+        err = lfs_dir_fetch(lfs, &root, lfs->root);
+        if (err) {
+            return err;
+        }
+
+        err = lfs_dir_commit(lfs, &root, NULL, 0);
+        if (err) {
+            return err;
+        }
+    }
+
+    return 0;
+}
+#endif
+
 static int lfs_fs_size_count(void *p, lfs_block_t block) {
     (void)block;
     lfs_size_t *size = p;
     *size += 1;
     return 0;
 }
 
@@ -5078,14 +5761,15 @@
 
     LFS_TRACE("lfs_removeattr -> %d", err);
     LFS_UNLOCK(lfs->cfg);
     return err;
 }
 #endif
 
+#ifndef LFS_NO_MALLOC
 int lfs_file_open(lfs_t *lfs, lfs_file_t *file, const char *path, int flags) {
     int err = LFS_LOCK(lfs->cfg);
     if (err) {
         return err;
     }
     LFS_TRACE("lfs_file_open(%p, %p, \"%s\", %x)",
             (void*)lfs, (void*)file, path, flags);
@@ -5093,14 +5777,15 @@
 
     err = lfs_file_rawopen(lfs, file, path, flags);
 
     LFS_TRACE("lfs_file_open -> %d", err);
     LFS_UNLOCK(lfs->cfg);
     return err;
 }
+#endif
 
 int lfs_file_opencfg(lfs_t *lfs, lfs_file_t *file,
         const char *path, int flags,
         const struct lfs_file_config *cfg) {
     int err = LFS_LOCK(lfs->cfg);
     if (err) {
         return err;
@@ -5393,14 +6078,30 @@
     err = lfs_fs_rawtraverse(lfs, cb, data, true);
 
     LFS_TRACE("lfs_fs_traverse -> %d", err);
     LFS_UNLOCK(lfs->cfg);
     return err;
 }
 
+#ifndef LFS_READONLY
+int lfs_fs_mkconsistent(lfs_t *lfs) {
+    int err = LFS_LOCK(lfs->cfg);
+    if (err) {
+        return err;
+    }
+    LFS_TRACE("lfs_fs_mkconsistent(%p)", (void*)lfs);
+
+    err = lfs_fs_rawmkconsistent(lfs);
+
+    LFS_TRACE("lfs_fs_mkconsistent -> %d", err);
+    LFS_UNLOCK(lfs->cfg);
+    return err;
+}
+#endif
+
 #ifdef LFS_MIGRATE
 int lfs_migrate(lfs_t *lfs, const struct lfs_config *cfg) {
     int err = LFS_LOCK(cfg);
     if (err) {
         return err;
     }
     LFS_TRACE("lfs_migrate(%p, %p {.context=%p, "
```

### Comparing `littlefs-python-0.4.0/littlefs/lfs.h` & `littlefs-python-0.5.0/littlefs/lfs.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 /*
  * The little filesystem
  *
+ * Copyright (c) 2022, The littlefs authors.
  * Copyright (c) 2017, Arm Limited. All rights reserved.
  * SPDX-License-Identifier: BSD-3-Clause
  */
 #ifndef LFS_H
 #define LFS_H
 
-#include <stdint.h>
-#include <stdbool.h>
 #include "lfs_util.h"
 
 #ifdef __cplusplus
 extern "C"
 {
 #endif
 
 
 /// Version info ///
 
 // Software library version
 // Major (top-nibble), incremented on backwards incompatible changes
 // Minor (bottom-nibble), incremented on feature additions
-#define LFS_VERSION 0x00020004
+#define LFS_VERSION 0x00020006
 #define LFS_VERSION_MAJOR (0xffff & (LFS_VERSION >> 16))
 #define LFS_VERSION_MINOR (0xffff & (LFS_VERSION >>  0))
 
 // Version of On-disk data structures
 // Major (top-nibble), incremented on backwards incompatible changes
 // Minor (bottom-nibble), incremented on feature additions
-#define LFS_DISK_VERSION 0x00020000
+#define LFS_DISK_VERSION 0x00020001
 #define LFS_DISK_VERSION_MAJOR (0xffff & (LFS_DISK_VERSION >> 16))
 #define LFS_DISK_VERSION_MINOR (0xffff & (LFS_DISK_VERSION >>  0))
 
 
 /// Definitions ///
 
 // Type definitions
@@ -109,14 +108,16 @@
     LFS_TYPE_SUPERBLOCK     = 0x0ff,
     LFS_TYPE_DIRSTRUCT      = 0x200,
     LFS_TYPE_CTZSTRUCT      = 0x202,
     LFS_TYPE_INLINESTRUCT   = 0x201,
     LFS_TYPE_SOFTTAIL       = 0x600,
     LFS_TYPE_HARDTAIL       = 0x601,
     LFS_TYPE_MOVESTATE      = 0x7ff,
+    LFS_TYPE_CCRC           = 0x500,
+    LFS_TYPE_FCRC           = 0x5ff,
 
     // internal chip sources
     LFS_FROM_NOOP           = 0x000,
     LFS_FROM_MOVE           = 0x101,
     LFS_FROM_USERATTRS      = 0x102,
 };
 
@@ -155,75 +156,75 @@
 
 // Configuration provided during initialization of the littlefs
 struct lfs_config {
     // Opaque user provided context that can be used to pass
     // information to the block device operations
     void *context;
 
-    // Read a region in a block. Negative error codes are propogated
+    // Read a region in a block. Negative error codes are propagated
     // to the user.
     int (*read)(const struct lfs_config *c, lfs_block_t block,
             lfs_off_t off, void *buffer, lfs_size_t size);
 
     // Program a region in a block. The block must have previously
-    // been erased. Negative error codes are propogated to the user.
+    // been erased. Negative error codes are propagated to the user.
     // May return LFS_ERR_CORRUPT if the block should be considered bad.
     int (*prog)(const struct lfs_config *c, lfs_block_t block,
             lfs_off_t off, const void *buffer, lfs_size_t size);
 
     // Erase a block. A block must be erased before being programmed.
     // The state of an erased block is undefined. Negative error codes
-    // are propogated to the user.
+    // are propagated to the user.
     // May return LFS_ERR_CORRUPT if the block should be considered bad.
     int (*erase)(const struct lfs_config *c, lfs_block_t block);
 
     // Sync the state of the underlying block device. Negative error codes
-    // are propogated to the user.
+    // are propagated to the user.
     int (*sync)(const struct lfs_config *c);
 
 #ifdef LFS_THREADSAFE
     // Lock the underlying block device. Negative error codes
-    // are propogated to the user.
+    // are propagated to the user.
     int (*lock)(const struct lfs_config *c);
 
     // Unlock the underlying block device. Negative error codes
-    // are propogated to the user.
+    // are propagated to the user.
     int (*unlock)(const struct lfs_config *c);
 #endif
 
-    // Minimum size of a block read. All read operations will be a
+    // Minimum size of a block read in bytes. All read operations will be a
     // multiple of this value.
     lfs_size_t read_size;
 
-    // Minimum size of a block program. All program operations will be a
-    // multiple of this value.
+    // Minimum size of a block program in bytes. All program operations will be
+    // a multiple of this value.
     lfs_size_t prog_size;
 
-    // Size of an erasable block. This does not impact ram consumption and
-    // may be larger than the physical erase size. However, non-inlined files
-    // take up at minimum one block. Must be a multiple of the read
-    // and program sizes.
+    // Size of an erasable block in bytes. This does not impact ram consumption
+    // and may be larger than the physical erase size. However, non-inlined
+    // files take up at minimum one block. Must be a multiple of the read and
+    // program sizes.
     lfs_size_t block_size;
 
     // Number of erasable blocks on the device.
     lfs_size_t block_count;
 
     // Number of erase cycles before littlefs evicts metadata logs and moves
     // the metadata to another block. Suggested values are in the
     // range 100-1000, with large values having better performance at the cost
     // of less consistent wear distribution.
     //
     // Set to -1 to disable block-level wear-leveling.
     int32_t block_cycles;
 
-    // Size of block caches. Each cache buffers a portion of a block in RAM.
-    // The littlefs needs a read cache, a program cache, and one additional
+    // Size of block caches in bytes. Each cache buffers a portion of a block in
+    // RAM. The littlefs needs a read cache, a program cache, and one additional
     // cache per file. Larger caches can improve performance by storing more
-    // data and reducing the number of disk accesses. Must be a multiple of
-    // the read and program sizes, and a factor of the block size.
+    // data and reducing the number of disk accesses. Must be a multiple of the
+    // read and program sizes, and a factor of the block size.
     lfs_size_t cache_size;
 
     // Size of the lookahead buffer in bytes. A larger lookahead buffer
     // increases the number of blocks found during an allocation pass. The
     // lookahead buffer is stored as a compact bitmap, so each byte of RAM
     // can track 8 blocks. Must be a multiple of 8.
     lfs_size_t lookahead_size;
@@ -481,15 +482,15 @@
 // the buffer, it will be padded with zeros. If the stored attribute is larger,
 // then it will be silently truncated. If no attribute is found, the error
 // LFS_ERR_NOATTR is returned and the buffer is filled with zeros.
 //
 // Returns the size of the attribute, or a negative error code on failure.
 // Note, the returned size is the size of the attribute on disk, irrespective
 // of the size of the buffer. This can be used to dynamically allocate a buffer
-// or check for existance.
+// or check for existence.
 lfs_ssize_t lfs_getattr(lfs_t *lfs, const char *path,
         uint8_t type, void *buffer, lfs_size_t size);
 
 #ifndef LFS_READONLY
 // Set custom attributes
 //
 // Custom attributes are uniquely identified by an 8-bit type and limited
@@ -509,31 +510,36 @@
 // Returns a negative error code on failure.
 int lfs_removeattr(lfs_t *lfs, const char *path, uint8_t type);
 #endif
 
 
 /// File operations ///
 
+#ifndef LFS_NO_MALLOC
 // Open a file
 //
 // The mode that the file is opened in is determined by the flags, which
 // are values from the enum lfs_open_flags that are bitwise-ored together.
 //
 // Returns a negative error code on failure.
 int lfs_file_open(lfs_t *lfs, lfs_file_t *file,
         const char *path, int flags);
 
+// if LFS_NO_MALLOC is defined, lfs_file_open() will fail with LFS_ERR_NOMEM
+// thus use lfs_file_opencfg() with config.buffer set.
+#endif
+
 // Open a file with extra configuration
 //
 // The mode that the file is opened in is determined by the flags, which
 // are values from the enum lfs_open_flags that are bitwise-ored together.
 //
 // The config struct provides additional config options per file as described
-// above. The config struct must be allocated while the file is open, and the
-// config struct must be zeroed for defaults and backwards compatibility.
+// above. The config struct must remain allocated while the file is open, and
+// the config struct must be zeroed for defaults and backwards compatibility.
 //
 // Returns a negative error code on failure.
 int lfs_file_opencfg(lfs_t *lfs, lfs_file_t *file,
         const char *path, int flags,
         const struct lfs_file_config *config);
 
 // Close a file
@@ -667,14 +673,26 @@
 // currently in use by the filesystem. This can be used to determine which
 // blocks are in use or how much of the storage is available.
 //
 // Returns a negative error code on failure.
 int lfs_fs_traverse(lfs_t *lfs, int (*cb)(void*, lfs_block_t), void *data);
 
 #ifndef LFS_READONLY
+// Attempt to make the filesystem consistent and ready for writing
+//
+// Calling this function is not required, consistency will be implicitly
+// enforced on the first operation that writes to the filesystem, but this
+// function allows the work to be performed earlier and without other
+// filesystem changes.
+//
+// Returns a negative error code on failure.
+int lfs_fs_mkconsistent(lfs_t *lfs);
+#endif
+
+#ifndef LFS_READONLY
 #ifdef LFS_MIGRATE
 // Attempts to migrate a previous version of littlefs
 //
 // Behaves similarly to the lfs_format function. Attempts to mount
 // the previous version of littlefs and update the filesystem so it can be
 // mounted with the current version of littlefs.
 //
```

### Comparing `littlefs-python-0.4.0/littlefs/lfs_util.h` & `littlefs-python-0.5.0/littlefs/lfs_util.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 /*
  * lfs utility functions
  *
+ * Copyright (c) 2022, The littlefs authors.
  * Copyright (c) 2017, Arm Limited. All rights reserved.
  * SPDX-License-Identifier: BSD-3-Clause
  */
 #ifndef LFS_UTIL_H
 #define LFS_UTIL_H
 
 // Users can override lfs_util.h with their own configuration by defining
@@ -162,18 +163,17 @@
 // between a and b ignoring overflow
 static inline int lfs_scmp(uint32_t a, uint32_t b) {
     return (int)(unsigned)(a - b);
 }
 
 // Convert between 32-bit little-endian and native order
 static inline uint32_t lfs_fromle32(uint32_t a) {
-#if !defined(LFS_NO_INTRINSICS) && ( \
-    (defined(  BYTE_ORDER  ) && defined(  ORDER_LITTLE_ENDIAN  ) &&   BYTE_ORDER   ==   ORDER_LITTLE_ENDIAN  ) || \
+#if (defined(  BYTE_ORDER  ) && defined(  ORDER_LITTLE_ENDIAN  ) &&   BYTE_ORDER   ==   ORDER_LITTLE_ENDIAN  ) || \
     (defined(__BYTE_ORDER  ) && defined(__ORDER_LITTLE_ENDIAN  ) && __BYTE_ORDER   == __ORDER_LITTLE_ENDIAN  ) || \
-    (defined(__BYTE_ORDER__) && defined(__ORDER_LITTLE_ENDIAN__) && __BYTE_ORDER__ == __ORDER_LITTLE_ENDIAN__))
+    (defined(__BYTE_ORDER__) && defined(__ORDER_LITTLE_ENDIAN__) && __BYTE_ORDER__ == __ORDER_LITTLE_ENDIAN__)
     return a;
 #elif !defined(LFS_NO_INTRINSICS) && ( \
     (defined(  BYTE_ORDER  ) && defined(  ORDER_BIG_ENDIAN  ) &&   BYTE_ORDER   ==   ORDER_BIG_ENDIAN  ) || \
     (defined(__BYTE_ORDER  ) && defined(__ORDER_BIG_ENDIAN  ) && __BYTE_ORDER   == __ORDER_BIG_ENDIAN  ) || \
     (defined(__BYTE_ORDER__) && defined(__ORDER_BIG_ENDIAN__) && __BYTE_ORDER__ == __ORDER_BIG_ENDIAN__))
     return __builtin_bswap32(a);
 #else
@@ -191,18 +191,17 @@
 // Convert between 32-bit big-endian and native order
 static inline uint32_t lfs_frombe32(uint32_t a) {
 #if !defined(LFS_NO_INTRINSICS) && ( \
     (defined(  BYTE_ORDER  ) && defined(  ORDER_LITTLE_ENDIAN  ) &&   BYTE_ORDER   ==   ORDER_LITTLE_ENDIAN  ) || \
     (defined(__BYTE_ORDER  ) && defined(__ORDER_LITTLE_ENDIAN  ) && __BYTE_ORDER   == __ORDER_LITTLE_ENDIAN  ) || \
     (defined(__BYTE_ORDER__) && defined(__ORDER_LITTLE_ENDIAN__) && __BYTE_ORDER__ == __ORDER_LITTLE_ENDIAN__))
     return __builtin_bswap32(a);
-#elif !defined(LFS_NO_INTRINSICS) && ( \
-    (defined(  BYTE_ORDER  ) && defined(  ORDER_BIG_ENDIAN  ) &&   BYTE_ORDER   ==   ORDER_BIG_ENDIAN  ) || \
+#elif (defined(  BYTE_ORDER  ) && defined(  ORDER_BIG_ENDIAN  ) &&   BYTE_ORDER   ==   ORDER_BIG_ENDIAN  ) || \
     (defined(__BYTE_ORDER  ) && defined(__ORDER_BIG_ENDIAN  ) && __BYTE_ORDER   == __ORDER_BIG_ENDIAN  ) || \
-    (defined(__BYTE_ORDER__) && defined(__ORDER_BIG_ENDIAN__) && __BYTE_ORDER__ == __ORDER_BIG_ENDIAN__))
+    (defined(__BYTE_ORDER__) && defined(__ORDER_BIG_ENDIAN__) && __BYTE_ORDER__ == __ORDER_BIG_ENDIAN__)
     return a;
 #else
     return (((uint8_t*)&a)[0] << 24) |
            (((uint8_t*)&a)[1] << 16) |
            (((uint8_t*)&a)[2] <<  8) |
            (((uint8_t*)&a)[3] <<  0);
 #endif
```

### Comparing `littlefs-python-0.4.0/littlefs/scripts/code.py` & `littlefs-python-0.5.0/littlefs/scripts/watch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,214 +1,265 @@
 #!/usr/bin/env python3
 #
-# Script to find code size at the function level. Basically just a bit wrapper
-# around nm with some extra conveniences for comparing builds. Heavily inspired
-# by Linux's Bloat-O-Meter.
+# Traditional watch command, but with higher resolution updates and a bit
+# different options/output format
+#
+# Example:
+# ./scripts/watch.py -s0.1 date
+#
+# Copyright (c) 2022, The littlefs authors.
+# SPDX-License-Identifier: BSD-3-Clause
 #
 
+import collections as co
+import errno
+import fcntl
+import io
 import os
-import glob
-import itertools as it
-import subprocess as sp
-import shlex
+import pty
 import re
-import csv
-import collections as co
-
+import shutil
+import struct
+import subprocess as sp
+import sys
+import termios
+import time
+
+try:
+    import inotify_simple
+except ModuleNotFoundError:
+    inotify_simple = None
 
-OBJ_PATHS = ['*.o', 'bd/*.o']
 
-def collect(paths, **args):
-    results = co.defaultdict(lambda: 0)
-    pattern = re.compile(
-        '^(?P<size>[0-9a-fA-F]+)' +
-        ' (?P<type>[%s])' % re.escape(args['type']) +
-        ' (?P<func>.+?)$')
-    for path in paths:
-        # note nm-tool may contain extra args
-        cmd = args['nm_tool'] + ['--size-sort', path]
-        if args.get('verbose'):
-            print(' '.join(shlex.quote(c) for c in cmd))
-        proc = sp.Popen(cmd,
-            stdout=sp.PIPE,
-            stderr=sp.PIPE if not args.get('verbose') else None,
-            universal_newlines=True)
-        for line in proc.stdout:
-            m = pattern.match(line)
-            if m:
-                results[(path, m.group('func'))] += int(m.group('size'), 16)
-        proc.wait()
-        if proc.returncode != 0:
-            if not args.get('verbose'):
-                for line in proc.stderr:
-                    sys.stdout.write(line)
-            sys.exit(-1)
-
-    flat_results = []
-    for (file, func), size in results.items():
-        # map to source files
-        if args.get('build_dir'):
-            file = re.sub('%s/*' % re.escape(args['build_dir']), '', file)
-        # discard internal functions
-        if func.startswith('__'):
-            continue
-        # discard .8449 suffixes created by optimizer
-        func = re.sub('\.[0-9]+', '', func)
-        flat_results.append((file, func, size))
-
-    return flat_results
-
-def main(**args):
-    # find sizes
-    if not args.get('use', None):
-        # find .o files
-        paths = []
-        for path in args['obj_paths']:
-            if os.path.isdir(path):
-                path = path + '/*.o'
-
-            for path in glob.glob(path):
-                paths.append(path)
-
-        if not paths:
-            print('no .obj files found in %r?' % args['obj_paths'])
-            sys.exit(-1)
-
-        results = collect(paths, **args)
-    else:
-        with open(args['use']) as f:
-            r = csv.DictReader(f)
-            results = [
-                (   result['file'],
-                    result['function'],
-                    int(result['size']))
-                for result in r]
-
-    total = 0
-    for _, _, size in results:
-        total += size
-
-    # find previous results?
-    if args.get('diff'):
-        with open(args['diff']) as f:
-            r = csv.DictReader(f)
-            prev_results = [
-                (   result['file'],
-                    result['function'],
-                    int(result['size']))
-                for result in r]
-
-        prev_total = 0
-        for _, _, size in prev_results:
-            prev_total += size
-
-    # write results to CSV
-    if args.get('output'):
-        with open(args['output'], 'w') as f:
-            w = csv.writer(f)
-            w.writerow(['file', 'function', 'size'])
-            for file, func, size in sorted(results):
-                w.writerow((file, func, size))
-
-    # print results
-    def dedup_entries(results, by='function'):
-        entries = co.defaultdict(lambda: 0)
-        for file, func, size in results:
-            entry = (file if by == 'file' else func)
-            entries[entry] += size
-        return entries
-
-    def diff_entries(olds, news):
-        diff = co.defaultdict(lambda: (0, 0, 0, 0))
-        for name, new in news.items():
-            diff[name] = (0, new, new, 1.0)
-        for name, old in olds.items():
-            _, new, _, _ = diff[name]
-            diff[name] = (old, new, new-old, (new-old)/old if old else 1.0)
-        return diff
-
-    def print_header(by=''):
-        if not args.get('diff'):
-            print('%-36s %7s' % (by, 'size'))
+def openio(path, mode='r', buffering=-1):
+    # allow '-' for stdin/stdout
+    if path == '-':
+        if mode == 'r':
+            return os.fdopen(os.dup(sys.stdin.fileno()), mode, buffering)
         else:
-            print('%-36s %7s %7s %7s' % (by, 'old', 'new', 'diff'))
+            return os.fdopen(os.dup(sys.stdout.fileno()), mode, buffering)
+    else:
+        return open(path, mode, buffering)
 
-    def print_entries(by='function'):
-        entries = dedup_entries(results, by=by)
+def inotifywait(paths):
+    # wait for interesting events
+    inotify = inotify_simple.INotify()
+    flags = (inotify_simple.flags.ATTRIB
+        | inotify_simple.flags.CREATE
+        | inotify_simple.flags.DELETE
+        | inotify_simple.flags.DELETE_SELF
+        | inotify_simple.flags.MODIFY
+        | inotify_simple.flags.MOVED_FROM
+        | inotify_simple.flags.MOVED_TO
+        | inotify_simple.flags.MOVE_SELF)
 
-        if not args.get('diff'):
-            print_header(by=by)
-            for name, size in sorted(entries.items()):
-                print("%-36s %7d" % (name, size))
-        else:
-            prev_entries = dedup_entries(prev_results, by=by)
-            diff = diff_entries(prev_entries, entries)
-            print_header(by='%s (%d added, %d removed)' % (by,
-                sum(1 for old, _, _, _ in diff.values() if not old),
-                sum(1 for _, new, _, _ in diff.values() if not new)))
-            for name, (old, new, diff, ratio) in sorted(diff.items(),
-                    key=lambda x: (-x[1][3], x)):
-                if ratio or args.get('all'):
-                    print("%-36s %7s %7s %+7d%s" % (name,
-                        old or "-",
-                        new or "-",
-                        diff,
-                        ' (%+.1f%%)' % (100*ratio) if ratio else ''))
-
-    def print_totals():
-        if not args.get('diff'):
-            print("%-36s %7d" % ('TOTAL', total))
+    # recurse into directories
+    for path in paths:
+        if os.path.isdir(path):
+            for dir, _, files in os.walk(path):
+                inotify.add_watch(dir, flags)
+                for f in files:
+                    inotify.add_watch(os.path.join(dir, f), flags)
         else:
-            ratio = (total-prev_total)/prev_total if prev_total else 1.0
-            print("%-36s %7s %7s %+7d%s" % (
-                'TOTAL',
-                prev_total if prev_total else '-',
-                total if total else '-',
-                total-prev_total,
-                ' (%+.1f%%)' % (100*ratio) if ratio else ''))
+            inotify.add_watch(path, flags)
 
-    if args.get('quiet'):
+    # wait for event
+    inotify.read()
+
+class LinesIO:
+    def __init__(self, maxlen=None):
+        self.maxlen = maxlen
+        self.lines = co.deque(maxlen=maxlen)
+        self.tail = io.StringIO()
+
+        # trigger automatic sizing
+        if maxlen == 0:
+            self.resize(0)
+
+    def write(self, s):
+        # note using split here ensures the trailing string has no newline
+        lines = s.split('\n')
+
+        if len(lines) > 1 and self.tail.getvalue():
+            self.tail.write(lines[0])
+            lines[0] = self.tail.getvalue()
+            self.tail = io.StringIO()
+
+        self.lines.extend(lines[:-1])
+
+        if lines[-1]:
+            self.tail.write(lines[-1])
+
+    def resize(self, maxlen):
+        self.maxlen = maxlen
+        if maxlen == 0:
+            maxlen = shutil.get_terminal_size((80, 5))[1]
+        if maxlen != self.lines.maxlen:
+            self.lines = co.deque(self.lines, maxlen=maxlen)
+
+    canvas_lines = 1
+    def draw(self):
+        # did terminal size change?
+        if self.maxlen == 0:
+            self.resize(0)
+
+        # first thing first, give ourself a canvas
+        while LinesIO.canvas_lines < len(self.lines):
+            sys.stdout.write('\n')
+            LinesIO.canvas_lines += 1
+
+        # clear the bottom of the canvas if we shrink
+        shrink = LinesIO.canvas_lines - len(self.lines)
+        if shrink > 0:
+            for i in range(shrink):
+                sys.stdout.write('\r')
+                if shrink-1-i > 0:
+                    sys.stdout.write('\x1b[%dA' % (shrink-1-i))
+                sys.stdout.write('\x1b[K')
+                if shrink-1-i > 0:
+                    sys.stdout.write('\x1b[%dB' % (shrink-1-i))
+            sys.stdout.write('\x1b[%dA' % shrink)
+            LinesIO.canvas_lines = len(self.lines)
+
+        for i, line in enumerate(self.lines):
+            # move cursor, clear line, disable/reenable line wrapping
+            sys.stdout.write('\r')
+            if len(self.lines)-1-i > 0:
+                sys.stdout.write('\x1b[%dA' % (len(self.lines)-1-i))
+            sys.stdout.write('\x1b[K')
+            sys.stdout.write('\x1b[?7l')
+            sys.stdout.write(line)
+            sys.stdout.write('\x1b[?7h')
+            if len(self.lines)-1-i > 0:
+                sys.stdout.write('\x1b[%dB' % (len(self.lines)-1-i))
+        sys.stdout.flush()
+
+
+def main(command, *,
+        lines=0,
+        cat=False,
+        sleep=None,
+        keep_open=False,
+        keep_open_paths=None,
+        exit_on_error=False):
+    returncode = 0
+    try:
+        while True:
+            # reset ring each run
+            if cat:
+                ring = sys.stdout
+            else:
+                ring = LinesIO(lines)
+
+            try:
+                # run the command under a pseudoterminal 
+                mpty, spty = pty.openpty()
+
+                # forward terminal size
+                w, h = shutil.get_terminal_size((80, 5))
+                if lines:
+                    h = lines
+                fcntl.ioctl(spty, termios.TIOCSWINSZ,
+                    struct.pack('HHHH', h, w, 0, 0))
+
+                proc = sp.Popen(command,
+                    stdout=spty,
+                    stderr=spty,
+                    close_fds=False)
+                os.close(spty)
+                mpty = os.fdopen(mpty, 'r', 1)
+
+                while True:
+                    try:
+                        line = mpty.readline()
+                    except OSError as e:
+                        if e.errno != errno.EIO:
+                            raise
+                        break
+                    if not line:
+                        break
+
+                    ring.write(line)
+                    if not cat:
+                        ring.draw()
+
+                mpty.close()
+                proc.wait()
+                if exit_on_error and proc.returncode != 0:
+                    returncode = proc.returncode
+                    break
+            except OSError as e:
+                if e.errno != errno.ETXTBSY:
+                    raise
+                pass
+
+            # try to inotifywait
+            if keep_open and inotify_simple is not None:
+                if keep_open_paths:
+                    paths = set(keep_paths)
+                else:
+                    # guess inotify paths from command
+                    paths = set()
+                    for p in command:
+                        for p in {
+                                p,
+                                re.sub('^-.', '', p),
+                                re.sub('^--[^=]+=', '', p)}:
+                            if p and os.path.exists(p):
+                                paths.add(p)
+                ptime = time.time()
+                inotifywait(paths)
+                # sleep for a minimum amount of time, this helps issues around
+                # rapidly updating files
+                time.sleep(max(0, (sleep or 0.1) - (time.time()-ptime)))
+            else:
+                time.sleep(sleep or 0.1)
+    except KeyboardInterrupt:
         pass
-    elif args.get('summary'):
-        print_header()
-        print_totals()
-    elif args.get('files'):
-        print_entries(by='file')
-        print_totals()
-    else:
-        print_entries(by='function')
-        print_totals()
+
+    if not cat:
+        sys.stdout.write('\n')
+    sys.exit(returncode)
+
 
 if __name__ == "__main__":
-    import argparse
     import sys
+    import argparse
     parser = argparse.ArgumentParser(
-        description="Find code size at the function level.")
-    parser.add_argument('obj_paths', nargs='*', default=OBJ_PATHS,
-        help="Description of where to find *.o files. May be a directory \
-            or a list of paths. Defaults to %r." % OBJ_PATHS)
-    parser.add_argument('-v', '--verbose', action='store_true',
-        help="Output commands that run behind the scenes.")
-    parser.add_argument('-o', '--output',
-        help="Specify CSV file to store results.")
-    parser.add_argument('-u', '--use',
-        help="Don't compile and find code sizes, instead use this CSV file.")
-    parser.add_argument('-d', '--diff',
-        help="Specify CSV file to diff code size against.")
-    parser.add_argument('-a', '--all', action='store_true',
-        help="Show all functions, not just the ones that changed.")
-    parser.add_argument('--files', action='store_true',
-        help="Show file-level code sizes. Note this does not include padding! "
-            "So sizes may differ from other tools.")
-    parser.add_argument('-s', '--summary', action='store_true',
-        help="Only show the total code size.")
-    parser.add_argument('-q', '--quiet', action='store_true',
-        help="Don't show anything, useful with -o.")
-    parser.add_argument('--type', default='tTrRdDbB',
-        help="Type of symbols to report, this uses the same single-character "
-            "type-names emitted by nm. Defaults to %(default)r.")
-    parser.add_argument('--nm-tool', default=['nm'], type=lambda x: x.split(),
-        help="Path to the nm tool to use.")
-    parser.add_argument('--build-dir',
-        help="Specify the relative build directory. Used to map object files \
-            to the correct source files.")
-    sys.exit(main(**vars(parser.parse_args())))
+        description="Traditional watch command, but with higher resolution "
+            "updates and a bit different options/output format.",
+        allow_abbrev=False)
+    parser.add_argument(
+        'command',
+        nargs=argparse.REMAINDER,
+        help="Command to run.")
+    parser.add_argument(
+        '-n', '--lines',
+        nargs='?',
+        type=lambda x: int(x, 0),
+        const=0,
+        help="Show this many lines of history. 0 uses the terminal height. "
+            "Defaults to 0.")
+    parser.add_argument(
+        '-z', '--cat',
+        action='store_true',
+        help="Pipe directly to stdout.")
+    parser.add_argument(
+        '-s', '--sleep',
+        type=float,
+        help="Seconds to sleep between runs. Defaults to 0.1.")
+    parser.add_argument(
+        '-k', '--keep-open',
+        action='store_true',
+        help="Try to use inotify to wait for changes.")
+    parser.add_argument(
+        '-K', '--keep-open-path',
+        dest='keep_open_paths',
+        action='append',
+        help="Use this path for inotify. Defaults to guessing.")
+    parser.add_argument(
+        '-e', '--exit-on-error',
+        action='store_true',
+        help="Exit on error.")
+    sys.exit(main(**{k: v
+        for k, v in vars(parser.parse_args()).items()
+        if v is not None}))
```

### Comparing `littlefs-python-0.4.0/littlefs/scripts/readblock.py` & `littlefs-python-0.5.0/littlefs/scripts/readblock.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/littlefs/scripts/readmdir.py` & `littlefs-python-0.5.0/littlefs/scripts/readmdir.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     'userattr':     (0x700, 0x300),
     'tail':         (0x700, 0x600),
     'softtail':     (0x7ff, 0x600),
     'hardtail':     (0x7ff, 0x601),
     'gstate':       (0x700, 0x700),
     'movestate':    (0x7ff, 0x7ff),
     'crc':          (0x700, 0x500),
+    'ccrc':         (0x780, 0x500),
+    'fcrc':         (0x7ff, 0x5ff),
 }
 
 class Tag:
     def __init__(self, *args):
         if len(args) == 1:
             self.tag = args[0]
         elif len(args) == 3:
@@ -95,45 +97,60 @@
         return self.type & 0xff
 
     @property
     def schunk(self):
         return struct.unpack('b', struct.pack('B', self.chunk))[0]
 
     def is_(self, type):
-        return (self.type & TAG_TYPES[type][0]) == TAG_TYPES[type][1]
+        try:
+            if ' ' in type:
+                type1, type3 = type.split()
+                return (self.is_(type1) and
+                    (self.type & ~TAG_TYPES[type1][0]) == int(type3, 0))
+
+            return self.type == int(type, 0)
+
+        except (ValueError, KeyError):
+            return (self.type & TAG_TYPES[type][0]) == TAG_TYPES[type][1]
 
     def mkmask(self):
         return Tag(
             0x700 if self.isunique else 0x7ff,
             0x3ff if self.isattr else 0,
             0)
 
     def chid(self, nid):
         ntag = Tag(self.type, nid, self.size)
-        if hasattr(self, 'off'):  ntag.off  = self.off
-        if hasattr(self, 'data'): ntag.data = self.data
-        if hasattr(self, 'crc'):  ntag.crc  = self.crc
+        if hasattr(self, 'off'):    ntag.off    = self.off
+        if hasattr(self, 'data'):   ntag.data   = self.data
+        if hasattr(self, 'ccrc'):   ntag.crc    = self.crc
+        if hasattr(self, 'erased'): ntag.erased = self.erased
         return ntag
 
     def typerepr(self):
-        if self.is_('crc') and getattr(self, 'crc', 0xffffffff) != 0xffffffff:
-            return 'crc (bad)'
+        if (self.is_('ccrc')
+                and getattr(self, 'ccrc', 0xffffffff) != 0xffffffff):
+            crc_status = ' (bad)'
+        elif self.is_('fcrc') and getattr(self, 'erased', False):
+            crc_status = ' (era)'
+        else:
+            crc_status = ''
 
         reverse_types = {v: k for k, v in TAG_TYPES.items()}
         for prefix in range(12):
             mask = 0x7ff & ~((1 << prefix)-1)
             if (mask, self.type & mask) in reverse_types:
                 type = reverse_types[mask, self.type & mask]
                 if prefix > 0:
-                    return '%s %#0*x' % (
-                        type, prefix//4, self.type & ((1 << prefix)-1))
+                    return '%s %#x%s' % (
+                        type, self.type & ((1 << prefix)-1), crc_status)
                 else:
-                    return type
+                    return '%s%s' % (type, crc_status)
         else:
-            return '%02x' % self.type
+            return '%02x%s' % (self.type, crc_status)
 
     def idrepr(self):
         return repr(self.id) if self.id != 0x3ff else '.'
 
     def sizerepr(self):
         return repr(self.size) if self.size != 0x3ff else 'x'
 
@@ -168,46 +185,61 @@
 
         self.pair = [self]
         self.data = blocks[0]
         block = self.data
 
         self.rev, = struct.unpack('<I', block[0:4])
         crc = binascii.crc32(block[0:4])
+        fcrctag = None
+        fcrcdata = None
 
         # parse tags
         corrupt = False
         tag = Tag(0xffffffff)
         off = 4
         self.log = []
         self.all_ = []
         while len(block) - off >= 4:
             ntag, = struct.unpack('>I', block[off:off+4])
 
-            tag = Tag(int(tag) ^ ntag)
+            tag = Tag((int(tag) ^ ntag) & 0x7fffffff)
             tag.off = off + 4
             tag.data = block[off+4:off+tag.dsize]
-            if tag.is_('crc'):
-                crc = binascii.crc32(block[off:off+4+4], crc)
+            if tag.is_('ccrc'):
+                crc = binascii.crc32(block[off:off+2*4], crc)
             else:
                 crc = binascii.crc32(block[off:off+tag.dsize], crc)
             tag.crc = crc
             off += tag.dsize
 
             self.all_.append(tag)
 
-            if tag.is_('crc'):
+            if tag.is_('fcrc') and len(tag.data) == 8:
+                fcrctag = tag
+                fcrcdata = struct.unpack('<II', tag.data)
+            elif tag.is_('ccrc'):
                 # is valid commit?
                 if crc != 0xffffffff:
                     corrupt = True
                 if not corrupt:
                     self.log = self.all_.copy()
+                    # end of commit?
+                    if fcrcdata:
+                        fcrcsize, fcrc = fcrcdata
+                        fcrc_ = 0xffffffff ^ binascii.crc32(
+                            block[off:off+fcrcsize])
+                        if fcrc_ == fcrc:
+                            fcrctag.erased = True
+                            corrupt = True
 
                 # reset tag parsing
                 crc = 0
                 tag = Tag(int(tag) ^ ((tag.type & 1) << 31))
+                fcrctag = None
+                fcrcdata = None
 
         # find active ids
         self.ids = list(it.takewhile(
             lambda id: Tag('name', id, 0) in self,
             it.count()))
 
         # find most recent tags
@@ -276,15 +308,15 @@
         f.write("%-8s  %-8s  %-13s %4s %4s" % (
             'off', 'tag', 'type', 'id', 'len'))
         if truncate:
             f.write('  data (truncated)')
         f.write('\n')
 
         for tag in tags:
-            f.write("%08x: %08x  %-13s %4s %4s" % (
+            f.write("%08x: %08x  %-14s %3s %4s" % (
                 tag.off, tag,
                 tag.typerepr(), tag.idrepr(), tag.sizerepr()))
             if truncate:
                 f.write("  %-23s  %-8s\n" % (
                     ' '.join('%02x' % c for c in tag.data[:8]),
                     ''.join(c if c >= ' ' and c <= '~' else '.'
                         for c in map(chr, tag.data[:8]))))
```

### Comparing `littlefs-python-0.4.0/littlefs/scripts/readtree.py` & `littlefs-python-0.5.0/littlefs/scripts/readtree.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/littlefs/scripts/test.py` & `littlefs-python-0.5.0/littlefs/scripts/tracebd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,857 +1,1002 @@
 #!/usr/bin/env python3
-
-# This script manages littlefs tests, which are configured with
-# .toml files stored in the tests directory.
+#
+# Display operations on block devices based on trace output
+#
+# Example:
+# ./scripts/tracebd.py trace
+#
+# Copyright (c) 2022, The littlefs authors.
+# SPDX-License-Identifier: BSD-3-Clause
 #
 
-import toml
-import glob
-import re
-import os
+import collections as co
+import functools as ft
 import io
 import itertools as it
-import collections.abc as abc
-import subprocess as sp
-import base64
-import sys
-import copy
-import shlex
-import pty
-import errno
-import signal
-
-TEST_PATHS = 'tests'
-RULES = """
-# add block devices to sources
-TESTSRC ?= $(SRC) $(wildcard bd/*.c)
-
-define FLATTEN
-%(path)s%%$(subst /,.,$(target)): $(target)
-    ./scripts/explode_asserts.py $$< -o $$@
-endef
-$(foreach target,$(TESTSRC),$(eval $(FLATTEN)))
-
--include %(path)s*.d
-.SECONDARY:
-
-%(path)s.test: %(path)s.test.o \\
-        $(foreach t,$(subst /,.,$(TESTSRC:.c=.o)),%(path)s.$t)
-    $(CC) $(CFLAGS) $^ $(LFLAGS) -o $@
-
-# needed in case builddir is different
-%(path)s%%.o: %(path)s%%.c
-    $(CC) -c -MMD $(CFLAGS) $< -o $@
-"""
-COVERAGE_RULES = """
-%(path)s.test: override CFLAGS += -fprofile-arcs -ftest-coverage
-
-# delete lingering coverage
-%(path)s.test: | %(path)s.info.clean
-.PHONY: %(path)s.info.clean
-%(path)s.info.clean:
-    rm -f %(path)s*.gcda
-
-# accumulate coverage info
-.PHONY: %(path)s.info
-%(path)s.info:
-    $(strip $(LCOV) -c \\
-        $(addprefix -d ,$(wildcard %(path)s*.gcda)) \\
-        --rc 'geninfo_adjust_src_path=$(shell pwd)' \\
-        -o $@)
-    $(LCOV) -e $@ $(addprefix /,$(SRC)) -o $@
-ifdef COVERAGETARGET
-    $(strip $(LCOV) -a $@ \\
-        $(addprefix -a ,$(wildcard $(COVERAGETARGET))) \\
-        -o $(COVERAGETARGET))
-endif
-"""
-GLOBALS = """
-//////////////// AUTOGENERATED TEST ////////////////
-#include "lfs.h"
-#include "bd/lfs_testbd.h"
-#include <stdio.h>
-extern const char *lfs_testbd_path;
-extern uint32_t lfs_testbd_cycles;
-"""
-DEFINES = {
-    'LFS_READ_SIZE': 16,
-    'LFS_PROG_SIZE': 'LFS_READ_SIZE',
-    'LFS_BLOCK_SIZE': 512,
-    'LFS_BLOCK_COUNT': 1024,
-    'LFS_BLOCK_CYCLES': -1,
-    'LFS_CACHE_SIZE': '(64 % LFS_PROG_SIZE == 0 ? 64 : LFS_PROG_SIZE)',
-    'LFS_LOOKAHEAD_SIZE': 16,
-    'LFS_ERASE_VALUE': 0xff,
-    'LFS_ERASE_CYCLES': 0,
-    'LFS_BADBLOCK_BEHAVIOR': 'LFS_TESTBD_BADBLOCK_PROGERROR',
-}
-PROLOGUE = """
-    // prologue
-    __attribute__((unused)) lfs_t lfs;
-    __attribute__((unused)) lfs_testbd_t bd;
-    __attribute__((unused)) lfs_file_t file;
-    __attribute__((unused)) lfs_dir_t dir;
-    __attribute__((unused)) struct lfs_info info;
-    __attribute__((unused)) char path[1024];
-    __attribute__((unused)) uint8_t buffer[1024];
-    __attribute__((unused)) lfs_size_t size;
-    __attribute__((unused)) int err;
-    
-    __attribute__((unused)) const struct lfs_config cfg = {
-        .context        = &bd,
-        .read           = lfs_testbd_read,
-        .prog           = lfs_testbd_prog,
-        .erase          = lfs_testbd_erase,
-        .sync           = lfs_testbd_sync,
-        .read_size      = LFS_READ_SIZE,
-        .prog_size      = LFS_PROG_SIZE,
-        .block_size     = LFS_BLOCK_SIZE,
-        .block_count    = LFS_BLOCK_COUNT,
-        .block_cycles   = LFS_BLOCK_CYCLES,
-        .cache_size     = LFS_CACHE_SIZE,
-        .lookahead_size = LFS_LOOKAHEAD_SIZE,
-    };
-
-    __attribute__((unused)) const struct lfs_testbd_config bdcfg = {
-        .erase_value        = LFS_ERASE_VALUE,
-        .erase_cycles       = LFS_ERASE_CYCLES,
-        .badblock_behavior  = LFS_BADBLOCK_BEHAVIOR,
-        .power_cycles       = lfs_testbd_cycles,
-    };
-
-    lfs_testbd_createcfg(&cfg, lfs_testbd_path, &bdcfg) => 0;
-"""
-EPILOGUE = """
-    // epilogue
-    lfs_testbd_destroy(&cfg) => 0;
-"""
-PASS = '\033[32m✓\033[0m'
-FAIL = '\033[31m✗\033[0m'
-
-class TestFailure(Exception):
-    def __init__(self, case, returncode=None, stdout=None, assert_=None):
-        self.case = case
-        self.returncode = returncode
-        self.stdout = stdout
-        self.assert_ = assert_
-
-class TestCase:
-    def __init__(self, config, filter=filter,
-            suite=None, caseno=None, lineno=None, **_):
-        self.config = config
-        self.filter = filter
-        self.suite = suite
-        self.caseno = caseno
-        self.lineno = lineno
-
-        self.code = config['code']
-        self.code_lineno = config['code_lineno']
-        self.defines = config.get('define', {})
-        self.if_ = config.get('if', None)
-        self.in_ = config.get('in', None)
-
-        self.result = None
-
-    def __str__(self):
-        if hasattr(self, 'permno'):
-            if any(k not in self.case.defines for k in self.defines):
-                return '%s#%d#%d (%s)' % (
-                    self.suite.name, self.caseno, self.permno, ', '.join(
-                        '%s=%s' % (k, v) for k, v in self.defines.items()
-                        if k not in self.case.defines))
+import math as m
+import os
+import re
+import shutil
+import threading as th
+import time
+
+
+CHARS = 'rpe.'
+COLORS = ['42', '45', '44', '']
+
+WEAR_CHARS = '0123456789'
+WEAR_CHARS_SUBSCRIPTS = '.₁₂₃₄₅₆789'
+WEAR_COLORS = ['', '', '', '', '', '', '', '35', '35', '1;31']
+
+CHARS_DOTS = " .':"
+COLORS_DOTS = ['32', '35', '34', '']
+CHARS_BRAILLE = (
+    '⠀⢀⡀⣀⠠⢠⡠⣠⠄⢄⡄⣄⠤⢤⡤⣤' '⠐⢐⡐⣐⠰⢰⡰⣰⠔⢔⡔⣔⠴⢴⡴⣴'
+    '⠂⢂⡂⣂⠢⢢⡢⣢⠆⢆⡆⣆⠦⢦⡦⣦' '⠒⢒⡒⣒⠲⢲⡲⣲⠖⢖⡖⣖⠶⢶⡶⣶'
+    '⠈⢈⡈⣈⠨⢨⡨⣨⠌⢌⡌⣌⠬⢬⡬⣬' '⠘⢘⡘⣘⠸⢸⡸⣸⠜⢜⡜⣜⠼⢼⡼⣼'
+    '⠊⢊⡊⣊⠪⢪⡪⣪⠎⢎⡎⣎⠮⢮⡮⣮' '⠚⢚⡚⣚⠺⢺⡺⣺⠞⢞⡞⣞⠾⢾⡾⣾'
+    '⠁⢁⡁⣁⠡⢡⡡⣡⠅⢅⡅⣅⠥⢥⡥⣥' '⠑⢑⡑⣑⠱⢱⡱⣱⠕⢕⡕⣕⠵⢵⡵⣵'
+    '⠃⢃⡃⣃⠣⢣⡣⣣⠇⢇⡇⣇⠧⢧⡧⣧' '⠓⢓⡓⣓⠳⢳⡳⣳⠗⢗⡗⣗⠷⢷⡷⣷'
+    '⠉⢉⡉⣉⠩⢩⡩⣩⠍⢍⡍⣍⠭⢭⡭⣭' '⠙⢙⡙⣙⠹⢹⡹⣹⠝⢝⡝⣝⠽⢽⡽⣽'
+    '⠋⢋⡋⣋⠫⢫⡫⣫⠏⢏⡏⣏⠯⢯⡯⣯' '⠛⢛⡛⣛⠻⢻⡻⣻⠟⢟⡟⣟⠿⢿⡿⣿')
+
+
+def openio(path, mode='r', buffering=-1):
+    # allow '-' for stdin/stdout
+    if path == '-':
+        if mode == 'r':
+            return os.fdopen(os.dup(sys.stdin.fileno()), mode, buffering)
+        else:
+            return os.fdopen(os.dup(sys.stdout.fileno()), mode, buffering)
+    else:
+        return open(path, mode, buffering)
+
+class LinesIO:
+    def __init__(self, maxlen=None):
+        self.maxlen = maxlen
+        self.lines = co.deque(maxlen=maxlen)
+        self.tail = io.StringIO()
+
+        # trigger automatic sizing
+        if maxlen == 0:
+            self.resize(0)
+
+    def write(self, s):
+        # note using split here ensures the trailing string has no newline
+        lines = s.split('\n')
+
+        if len(lines) > 1 and self.tail.getvalue():
+            self.tail.write(lines[0])
+            lines[0] = self.tail.getvalue()
+            self.tail = io.StringIO()
+
+        self.lines.extend(lines[:-1])
+
+        if lines[-1]:
+            self.tail.write(lines[-1])
+
+    def resize(self, maxlen):
+        self.maxlen = maxlen
+        if maxlen == 0:
+            maxlen = shutil.get_terminal_size((80, 5))[1]
+        if maxlen != self.lines.maxlen:
+            self.lines = co.deque(self.lines, maxlen=maxlen)
+
+    canvas_lines = 1
+    def draw(self):
+        # did terminal size change?
+        if self.maxlen == 0:
+            self.resize(0)
+
+        # first thing first, give ourself a canvas
+        while LinesIO.canvas_lines < len(self.lines):
+            sys.stdout.write('\n')
+            LinesIO.canvas_lines += 1
+
+        # clear the bottom of the canvas if we shrink
+        shrink = LinesIO.canvas_lines - len(self.lines)
+        if shrink > 0:
+            for i in range(shrink):
+                sys.stdout.write('\r')
+                if shrink-1-i > 0:
+                    sys.stdout.write('\x1b[%dA' % (shrink-1-i))
+                sys.stdout.write('\x1b[K')
+                if shrink-1-i > 0:
+                    sys.stdout.write('\x1b[%dB' % (shrink-1-i))
+            sys.stdout.write('\x1b[%dA' % shrink)
+            LinesIO.canvas_lines = len(self.lines)
+
+        for i, line in enumerate(self.lines):
+            # move cursor, clear line, disable/reenable line wrapping
+            sys.stdout.write('\r')
+            if len(self.lines)-1-i > 0:
+                sys.stdout.write('\x1b[%dA' % (len(self.lines)-1-i))
+            sys.stdout.write('\x1b[K')
+            sys.stdout.write('\x1b[?7l')
+            sys.stdout.write(line)
+            sys.stdout.write('\x1b[?7h')
+            if len(self.lines)-1-i > 0:
+                sys.stdout.write('\x1b[%dB' % (len(self.lines)-1-i))
+        sys.stdout.flush()
+
+
+# space filling Hilbert-curve
+#
+# note we memoize the last curve since this is a bit expensive
+#
+@ft.lru_cache(1)
+def hilbert_curve(width, height):
+    # based on generalized Hilbert curves:
+    # https://github.com/jakubcerveny/gilbert
+    #
+    def hilbert_(x, y, a_x, a_y, b_x, b_y):
+        w = abs(a_x+a_y)
+        h = abs(b_x+b_y)
+        a_dx = -1 if a_x < 0 else +1 if a_x > 0 else 0
+        a_dy = -1 if a_y < 0 else +1 if a_y > 0 else 0
+        b_dx = -1 if b_x < 0 else +1 if b_x > 0 else 0
+        b_dy = -1 if b_y < 0 else +1 if b_y > 0 else 0
+
+        # trivial row
+        if h == 1:
+            for _ in range(w):
+                yield (x,y)
+                x, y = x+a_dx, y+a_dy
+            return
+
+        # trivial column
+        if w == 1:
+            for _ in range(h):
+                yield (x,y)
+                x, y = x+b_dx, y+b_dy
+            return
+
+        a_x_, a_y_ = a_x//2, a_y//2
+        b_x_, b_y_ = b_x//2, b_y//2
+        w_ = abs(a_x_+a_y_)
+        h_ = abs(b_x_+b_y_)
+
+        if 2*w > 3*h:
+            # prefer even steps
+            if w_ % 2 != 0 and w > 2:
+                a_x_, a_y_ = a_x_+a_dx, a_y_+a_dy
+
+            # split in two
+            yield from hilbert_(x, y, a_x_, a_y_, b_x, b_y)
+            yield from hilbert_(x+a_x_, y+a_y_, a_x-a_x_, a_y-a_y_, b_x, b_y)
+        else:
+            # prefer even steps
+            if h_ % 2 != 0 and h > 2:
+                b_x_, b_y_ = b_x_+b_dx, b_y_+b_dy
+
+            # split in three
+            yield from hilbert_(x, y, b_x_, b_y_, a_x_, a_y_)
+            yield from hilbert_(x+b_x_, y+b_y_, a_x, a_y, b_x-b_x_, b_y-b_y_)
+            yield from hilbert_(
+                x+(a_x-a_dx)+(b_x_-b_dx), y+(a_y-a_dy)+(b_y_-b_dy),
+                -b_x_, -b_y_, -(a_x-a_x_), -(a_y-a_y_))
+
+    if width >= height:
+        curve = hilbert_(0, 0, +width, 0, 0, +height)
+    else:
+        curve = hilbert_(0, 0, 0, +height, +width, 0)
+
+    return list(curve)
+
+# space filling Z-curve/Lebesgue-curve
+#
+# note we memoize the last curve since this is a bit expensive
+#
+@ft.lru_cache(1)
+def lebesgue_curve(width, height):
+    # we create a truncated Z-curve by simply filtering out the points
+    # that are outside our region
+    curve = []
+    for i in range(2**(2*m.ceil(m.log2(max(width, height))))):
+        # we just operate on binary strings here because it's easier
+        b = '{:0{}b}'.format(i, 2*m.ceil(m.log2(i+1)/2))
+        x = int(b[1::2], 2) if b[1::2] else 0
+        y = int(b[0::2], 2) if b[0::2] else 0
+        if x < width and y < height:
+            curve.append((x, y))
+
+    return curve
+
+
+class Block(int):
+    __slots__ = ()
+    def __new__(cls, state=0, *,
+            wear=0,
+            readed=False,
+            proged=False,
+            erased=False):
+        return super().__new__(cls,
+            state
+            | (wear << 3)
+            | (1 if readed else 0)
+            | (2 if proged else 0)
+            | (4 if erased else 0))
+
+    @property
+    def wear(self):
+        return self >> 3
+
+    @property
+    def readed(self):
+        return (self & 1) != 0
+
+    @property
+    def proged(self):
+        return (self & 2) != 0
+
+    @property
+    def erased(self):
+        return (self & 4) != 0
+
+    def read(self):
+        return Block(int(self) | 1)
+
+    def prog(self):
+        return Block(int(self) | 2)
+
+    def erase(self):
+        return Block((int(self) | 4) + 8)
+
+    def clear(self):
+        return Block(int(self) & ~7)
+
+    def __or__(self, other):
+        return Block(
+            (int(self) | int(other)) & 7,
+            wear=max(self.wear, other.wear))
+
+    def worn(self, max_wear, *,
+            block_cycles=None,
+            wear_chars=None,
+            **_):
+        if wear_chars is None:
+            wear_chars = WEAR_CHARS
+
+        if block_cycles:
+            return self.wear / block_cycles
+        else:
+            return self.wear / max(max_wear, len(wear_chars))
+
+    def draw(self, max_wear, char=None, *,
+            read=True,
+            prog=True,
+            erase=True,
+            wear=False,
+            block_cycles=None,
+            color=True,
+            subscripts=False,
+            dots=False,
+            braille=False,
+            chars=None,
+            wear_chars=None,
+            colors=None,
+            wear_colors=None,
+            **_):
+        # fallback to default chars/colors
+        if chars is None:
+            chars = CHARS
+        if len(chars) < len(CHARS):
+            chars = chars + CHARS[len(chars):]
+
+        if colors is None:
+            if braille or dots:
+                colors = COLORS_DOTS
             else:
-                return '%s#%d#%d' % (
-                    self.suite.name, self.caseno, self.permno)
+                colors = COLORS
+        if len(colors) < len(COLORS):
+            colors = colors + COLORS[len(colors):]
+
+        if wear_chars is None:
+            if subscripts:
+                wear_chars = WEAR_CHARS_SUBSCRIPTS
+            else:
+                wear_chars = WEAR_CHARS
+
+        if wear_colors is None:
+            wear_colors = WEAR_COLORS
+
+        # compute char/color
+        c = chars[3]
+        f = [colors[3]]
+
+        if wear:
+            w = min(
+                self.worn(
+                    max_wear,
+                    block_cycles=block_cycles,
+                    wear_chars=wear_chars),
+                1)
+
+            c = wear_chars[int(w * (len(wear_chars)-1))]
+            f.append(wear_colors[int(w * (len(wear_colors)-1))])
+
+        if erase and self.erased:
+            c = chars[2]
+            f.append(colors[2])
+        elif prog and self.proged:
+            c = chars[1]
+            f.append(colors[1])
+        elif read and self.readed:
+            c = chars[0]
+            f.append(colors[0])
+
+        # override char?
+        if char:
+            c = char
+
+        # apply colors
+        if f and color:
+            c = '%s%s\x1b[m' % (
+                ''.join('\x1b[%sm' % f_ for f_ in f),
+                c)
+
+        return c
+
+
+class Bd:
+    def __init__(self, *,
+            size=1,
+            count=1,
+            width=None,
+            height=1,
+            blocks=None):
+        if width is None:
+            width = count
+
+        if blocks is None:
+            self.blocks = [Block() for _ in range(width*height)]
         else:
-            return '%s#%d' % (
-                self.suite.name, self.caseno)
+            self.blocks = blocks
+        self.size = size
+        self.count = count
+        self.width = width
+        self.height = height
+
+    def _op(self, f, block=None, off=None, size=None):
+        if block is None:
+            range_ = range(len(self.blocks))
+        else:
+            if off is None:
+                off, size = 0, self.size
+            elif size is None:
+                off, size = 0, off
+
+            # update our geometry? this will do nothing if we haven't changed
+            self.resize(
+                size=max(self.size, off+size),
+                count=max(self.count, block+1))
+
+            # map to our block space
+            start = (block*self.size + off) / (self.size*self.count)
+            stop = (block*self.size + off+size) / (self.size*self.count)
+
+            range_ = range(
+                m.floor(start*len(self.blocks)),
+                m.ceil(stop*len(self.blocks)))
+
+        # apply the op
+        for i in range_:
+            self.blocks[i] = f(self.blocks[i])
+
+    def read(self, block=None, off=None, size=None):
+        self._op(Block.read, block, off, size)
+
+    def prog(self, block=None, off=None, size=None):
+        self._op(Block.prog, block, off, size)
+
+    def erase(self, block=None, off=None, size=None):
+        self._op(Block.erase, block, off, size)
+
+    def clear(self, block=None, off=None, size=None):
+        self._op(Block.clear, block, off, size)
+
+    def copy(self):
+        return Bd(
+            blocks=self.blocks.copy(),
+            size=self.size,
+            count=self.count,
+            width=self.width,
+            height=self.height)
+
+    def resize(self, *,
+            size=None,
+            count=None,
+            width=None,
+            height=None):
+        size = size if size is not None else self.size
+        count = count if count is not None else self.count
+        width = width if width is not None else self.width
+        height = height if height is not None else self.height
+
+        if (size == self.size
+                and count == self.count
+                and width == self.width
+                and height == self.height):
+            return
+
+        # transform our blocks
+        blocks = []
+        for x in range(width*height):
+            # map from new bd space
+            start = m.floor(x * (size*count)/(width*height))
+            stop = m.ceil((x+1) * (size*count)/(width*height))
+            start_block = start // size
+            start_off = start % size
+            stop_block = stop // size
+            stop_off = stop % size
+            # map to old bd space
+            start = start_block*self.size + start_off
+            stop = stop_block*self.size + stop_off
+            start = m.floor(start * len(self.blocks)/(self.size*self.count))
+            stop = m.ceil(stop * len(self.blocks)/(self.size*self.count))
+
+            # aggregate state
+            blocks.append(ft.reduce(
+                Block.__or__,
+                self.blocks[start:stop],
+                Block()))
+            
+        self.size = size
+        self.count = count
+        self.width = width
+        self.height = height
+        self.blocks = blocks
+
+    def draw(self, row, *,
+            read=False,
+            prog=False,
+            erase=False,
+            wear=False,
+            hilbert=False,
+            lebesgue=False,
+            dots=False,
+            braille=False,
+            **args):
+        # find max wear?
+        max_wear = None
+        if wear:
+            max_wear = max(b.wear for b in self.blocks)
+
+        # fold via a curve?
+        if hilbert:
+            grid = [None]*(self.width*self.height)
+            for (x,y), b in zip(
+                    hilbert_curve(self.width, self.height),
+                    self.blocks):
+                grid[x + y*self.width] = b
+        elif lebesgue:
+            grid = [None]*(self.width*self.height)
+            for (x,y), b in zip(
+                    lebesgue_curve(self.width, self.height),
+                    self.blocks):
+                grid[x + y*self.width] = b
+        else:
+            grid = self.blocks
 
-    def permute(self, class_=None, defines={}, permno=None, **_):
-        ncase = (class_ or type(self))(self.config)
-        for k, v in self.__dict__.items():
-            setattr(ncase, k, v)
-        ncase.case = self
-        ncase.perms = [ncase]
-        ncase.permno = permno
-        ncase.defines = defines
-        return ncase
-
-    def build(self, f, **_):
-        # prologue
-        for k, v in sorted(self.defines.items()):
-            if k not in self.suite.defines:
-                f.write('#define %s %s\n' % (k, v))
-
-        f.write('void test_case%d(%s) {' % (self.caseno, ','.join(
-            '\n'+8*' '+'__attribute__((unused)) intmax_t %s' % k
-            for k in sorted(self.perms[0].defines)
-            if k not in self.defines)))
-
-        f.write(PROLOGUE)
-        f.write('\n')
-        f.write(4*' '+'// test case %d\n' % self.caseno)
-        f.write(4*' '+'#line %d "%s"\n' % (self.code_lineno, self.suite.path))
-
-        # test case goes here
-        f.write(self.code)
-
-        # epilogue
-        f.write(EPILOGUE)
-        f.write('}\n')
-
-        for k, v in sorted(self.defines.items()):
-            if k not in self.suite.defines:
-                f.write('#undef %s\n' % k)
-
-    def shouldtest(self, **args):
-        if (self.filter is not None and
-                len(self.filter) >= 1 and
-                self.filter[0] != self.caseno):
-            return False
-        elif (self.filter is not None and
-                len(self.filter) >= 2 and
-                self.filter[1] != self.permno):
+        # need to wait for more trace output before rendering
+        #
+        # this is sort of a hack that knows the output is going to a terminal
+        if (braille and self.height < 4) or (dots and self.height < 2):
+            needed_height = 4 if braille else 2
+
+            self.history = getattr(self, 'history', [])
+            self.history.append(grid)
+
+            if len(self.history)*self.height < needed_height:
+                # skip for now
+                return None
+
+            grid = list(it.chain.from_iterable(
+                # did we resize?
+                it.islice(it.chain(h, it.repeat(Block())),
+                    self.width*self.height)
+                for h in self.history))
+            self.history = []
+
+        line = []
+        if braille:
+            # encode into a byte
+            for x in range(0, self.width, 2):
+                byte_b = 0
+                best_b = Block()
+                for i in range(2*4):
+                    b = grid[x+(2-1-(i%2)) + ((row*4)+(4-1-(i//2)))*self.width]
+                    best_b |= b
+                    if ((read and b.readed)
+                            or (prog and b.proged)
+                            or (erase and b.erased)
+                            or (not read and not prog and not erase
+                                and wear and b.worn(max_wear, **args) >= 0.7)):
+                        byte_b |= 1 << i
+
+                line.append(best_b.draw(
+                    max_wear,
+                    CHARS_BRAILLE[byte_b],
+                    braille=True,
+                    read=read,
+                    prog=prog,
+                    erase=erase,
+                    wear=wear,
+                    **args))
+        elif dots:
+            # encode into a byte
+            for x in range(self.width):
+                byte_b = 0
+                best_b = Block()
+                for i in range(2):
+                    b = grid[x + ((row*2)+(2-1-i))*self.width]
+                    best_b |= b
+                    if ((read and b.readed)
+                            or (prog and b.proged)
+                            or (erase and b.erased)
+                            or (not read and not prog and not erase
+                                and wear and b.worn(max_wear, **args) >= 0.7)):
+                        byte_b |= 1 << i
+
+                line.append(best_b.draw(
+                    max_wear,
+                    CHARS_DOTS[byte_b],
+                    dots=True,
+                    read=read,
+                    prog=prog,
+                    erase=erase,
+                    wear=wear,
+                    **args))
+        else:
+            for x in range(self.width):
+                line.append(grid[x + row*self.width].draw(
+                    max_wear,
+                    read=read,
+                    prog=prog,
+                    erase=erase,
+                    wear=wear,
+                    **args))
+
+        return ''.join(line)
+
+
+
+def main(path='-', *,
+        read=False,
+        prog=False,
+        erase=False,
+        wear=False,
+        block=(None,None),
+        off=(None,None),
+        block_size=None,
+        block_count=None,
+        block_cycles=None,
+        reset=False,
+        color='auto',
+        dots=False,
+        braille=False,
+        width=None,
+        height=None,
+        lines=None,
+        cat=False,
+        hilbert=False,
+        lebesgue=False,
+        coalesce=None,
+        sleep=None,
+        keep_open=False,
+        **args):
+    # figure out what color should be
+    if color == 'auto':
+        color = sys.stdout.isatty()
+    elif color == 'always':
+        color = True
+    else:
+        color = False
+
+    # exclusive wear or read/prog/erase by default
+    if not read and not prog and not erase and not wear:
+        read = True
+        prog = True
+        erase = True
+
+    # assume a reasonable lines/height if not specified
+    #
+    # note that we let height = None if neither hilbert or lebesgue
+    # are specified, this is a bit special as the default may be less
+    # than one character in height.
+    if height is None and (hilbert or lebesgue):
+        if lines is not None:
+            height = lines
+        else:
+            height = 5
+
+    if lines is None:
+        if height is not None:
+            lines = height
+        else:
+            lines = 5
+
+    # allow ranges for blocks/offs
+    block_start = block[0]
+    block_stop = block[1] if len(block) > 1 else block[0]+1
+    off_start = off[0]
+    off_stop = off[1] if len(off) > 1 else off[0]+1
+
+    if block_start is None:
+        block_start = 0
+    if block_stop is None and block_count is not None:
+        block_stop = block_count
+    if off_start is None:
+        off_start = 0
+    if off_stop is None and block_size is not None:
+        off_stop = block_size
+
+    # create a block device representation
+    bd = Bd()
+
+    def resize(*, size=None, count=None):
+        nonlocal bd
+
+        # size may be overriden by cli args
+        if block_size is not None:
+            size = block_size
+        elif off_stop is not None:
+            size = off_stop-off_start
+
+        if block_count is not None:
+            count = block_count
+        elif block_stop is not None:
+            count = block_stop-block_start
+
+        # figure out best width/height
+        if width is None:
+            width_ = min(80, shutil.get_terminal_size((80, 5))[0])
+        elif width:
+            width_ = width
+        else:
+            width_ = shutil.get_terminal_size((80, 5))[0]
+
+        if height is None:
+            height_ = 0
+        elif height:
+            height_ = height
+        else:
+            height_ = shutil.get_terminal_size((80, 5))[1]
+
+        bd.resize(
+            size=size,
+            count=count,
+            # scale if we're printing with dots or braille
+            width=2*width_ if braille else width_,
+            height=max(1,
+                4*height_ if braille
+                else 2*height_ if dots
+                else height_))
+    resize()
+
+    # parse a line of trace output
+    pattern = re.compile(
+        '^(?P<file>[^:]*):(?P<line>[0-9]+):trace:.*?bd_(?:'
+            '(?P<create>create\w*)\('
+                '(?:'
+                    'block_size=(?P<block_size>\w+)'
+                    '|' 'block_count=(?P<block_count>\w+)'
+                    '|' '.*?' ')*' '\)'
+            '|' '(?P<read>read)\('
+                '\s*(?P<read_ctx>\w+)' '\s*,'
+                '\s*(?P<read_block>\w+)' '\s*,'
+                '\s*(?P<read_off>\w+)' '\s*,'
+                '\s*(?P<read_buffer>\w+)' '\s*,'
+                '\s*(?P<read_size>\w+)' '\s*\)'
+            '|' '(?P<prog>prog)\('
+                '\s*(?P<prog_ctx>\w+)' '\s*,'
+                '\s*(?P<prog_block>\w+)' '\s*,'
+                '\s*(?P<prog_off>\w+)' '\s*,'
+                '\s*(?P<prog_buffer>\w+)' '\s*,'
+                '\s*(?P<prog_size>\w+)' '\s*\)'
+            '|' '(?P<erase>erase)\('
+                '\s*(?P<erase_ctx>\w+)' '\s*,'
+                '\s*(?P<erase_block>\w+)'
+                '\s*\(\s*(?P<erase_size>\w+)\s*\)' '\s*\)'
+            '|' '(?P<sync>sync)\('
+                '\s*(?P<sync_ctx>\w+)' '\s*\)' ')\s*$')
+    def parse(line):
+        nonlocal bd
+
+        # string searching is much faster than the regex here, and this
+        # actually has a big impact given how much trace output comes
+        # through here
+        if 'trace' not in line or 'bd' not in line:
             return False
-        elif args.get('no_internal') and self.in_ is not None:
+        m = pattern.match(line)
+        if not m:
             return False
-        elif self.if_ is not None:
-            if_ = self.if_
-            while True:
-                for k, v in sorted(self.defines.items(),
-                        key=lambda x: len(x[0]), reverse=True):
-                    if k in if_:
-                        if_ = if_.replace(k, '(%s)' % v)
-                        break
-                else:
-                    break
-            if_ = (
-                re.sub('(\&\&|\?)', ' and ',
-                re.sub('(\|\||:)', ' or ',
-                re.sub('!(?!=)', ' not ', if_))))
-            return eval(if_)
-        else:
+
+        if m.group('create'):
+            # update our block size/count
+            size = int(m.group('block_size'), 0)
+            count = int(m.group('block_count'), 0)
+
+            resize(size=size, count=count)
+            if reset:
+                bd = Bd(
+                    size=bd.size,
+                    count=bd.count,
+                    width=bd.width,
+                    height=bd.height)
             return True
 
-    def test(self, exec=[], persist=False, cycles=None,
-            gdb=False, failure=None, disk=None, **args):
-        # build command
-        cmd = exec + ['./%s.test' % self.suite.path,
-            repr(self.caseno), repr(self.permno)]
-
-        # persist disk or keep in RAM for speed?
-        if persist:
-            if not disk:
-                disk = self.suite.path + '.disk'
-            if persist != 'noerase':
-                try:
-                    with open(disk, 'w') as f:
-                        f.truncate(0)
-                    if args.get('verbose'):
-                        print('truncate --size=0', disk)
-                except FileNotFoundError:
-                    pass
-
-            cmd.append(disk)
-
-        # simulate power-loss after n cycles?
-        if cycles:
-            cmd.append(str(cycles))
-
-        # failed? drop into debugger?
-        if gdb and failure:
-            ncmd = ['gdb']
-            if gdb == 'assert':
-                ncmd.extend(['-ex', 'r'])
-                if failure.assert_:
-                    ncmd.extend(['-ex', 'up 2'])
-            elif gdb == 'main':
-                ncmd.extend([
-                    '-ex', 'b %s:%d' % (self.suite.path, self.code_lineno),
-                    '-ex', 'r'])
-            ncmd.extend(['--args'] + cmd)
-
-            if args.get('verbose'):
-                print(' '.join(shlex.quote(c) for c in ncmd))
-            signal.signal(signal.SIGINT, signal.SIG_IGN)
-            sys.exit(sp.call(ncmd))
-
-        # run test case!
-        mpty, spty = pty.openpty()
-        if args.get('verbose'):
-            print(' '.join(shlex.quote(c) for c in cmd))
-        proc = sp.Popen(cmd, stdout=spty, stderr=spty)
-        os.close(spty)
-        mpty = os.fdopen(mpty, 'r', 1)
-        stdout = []
-        assert_ = None
-        try:
-            while True:
-                try:
-                    line = mpty.readline()
-                except OSError as e:
-                    if e.errno == errno.EIO:
-                        break
-                    raise
-                if not line:
-                    break;
-                stdout.append(line)
-                if args.get('verbose'):
-                    sys.stdout.write(line)
-                # intercept asserts
-                m = re.match(
-                    '^{0}([^:]+):(\d+):(?:\d+:)?{0}{1}:{0}(.*)$'
-                    .format('(?:\033\[[\d;]*.| )*', 'assert'),
-                    line)
-                if m and assert_ is None:
-                    try:
-                        with open(m.group(1)) as f:
-                            lineno = int(m.group(2))
-                            line = (next(it.islice(f, lineno-1, None))
-                                .strip('\n'))
-                        assert_ = {
-                            'path': m.group(1),
-                            'line': line,
-                            'lineno': lineno,
-                            'message': m.group(3)}
-                    except:
-                        pass
-        except KeyboardInterrupt:
-            raise TestFailure(self, 1, stdout, None)
-        proc.wait()
-
-        # did we pass?
-        if proc.returncode != 0:
-            raise TestFailure(self, proc.returncode, stdout, assert_)
-        else:
-            return PASS
-
-class ValgrindTestCase(TestCase):
-    def __init__(self, config, **args):
-        self.leaky = config.get('leaky', False)
-        super().__init__(config, **args)
-
-    def shouldtest(self, **args):
-        return not self.leaky and super().shouldtest(**args)
-
-    def test(self, exec=[], **args):
-        verbose = args.get('verbose')
-        uninit = (self.defines.get('LFS_ERASE_VALUE', None) == -1)
-        exec = [
-            'valgrind',
-            '--leak-check=full',
-            ] + (['--undef-value-errors=no'] if uninit else []) + [
-            ] + (['--track-origins=yes'] if not uninit else []) + [
-            '--error-exitcode=4',
-            '--error-limit=no',
-            ] + (['--num-callers=1'] if not verbose else []) + [
-            '-q'] + exec
-        return super().test(exec=exec, **args)
-
-class ReentrantTestCase(TestCase):
-    def __init__(self, config, **args):
-        self.reentrant = config.get('reentrant', False)
-        super().__init__(config, **args)
-
-    def shouldtest(self, **args):
-        return self.reentrant and super().shouldtest(**args)
-
-    def test(self, persist=False, gdb=False, failure=None, **args):
-        for cycles in it.count(1):
-            # clear disk first?
-            if cycles == 1 and persist != 'noerase':
-                persist = 'erase'
-            else:
-                persist = 'noerase'
+        elif m.group('read') and read:
+            block = int(m.group('read_block'), 0)
+            off = int(m.group('read_off'), 0)
+            size = int(m.group('read_size'), 0)
+
+            if block_stop is not None and block >= block_stop:
+                return False
+            block -= block_start
+            if off_stop is not None:
+                if off >= off_stop:
+                    return False
+                size = min(size, off_stop-off)
+            off -= off_start
 
-            # exact cycle we should drop into debugger?
-            if gdb and failure and failure.cycleno == cycles:
-                return super().test(gdb=gdb, persist=persist, cycles=cycles,
-                    failure=failure, **args)
-
-            # run tests, but kill the program after prog/erase has
-            # been hit n cycles. We exit with a special return code if the
-            # program has not finished, since this isn't a test failure.
-            try:
-                return super().test(persist=persist, cycles=cycles, **args)
-            except TestFailure as nfailure:
-                if nfailure.returncode == 33:
-                    continue
-                else:
-                    nfailure.cycleno = cycles
-                    raise
-
-class TestSuite:
-    def __init__(self, path, classes=[TestCase], defines={},
-            filter=None, **args):
-        self.name = os.path.basename(path)
-        if self.name.endswith('.toml'):
-            self.name = self.name[:-len('.toml')]
-        if args.get('build_dir'):
-            self.toml = path
-            self.path = args['build_dir'] + '/' + path
-        else:
-            self.toml = path
-            self.path = path
-        self.classes = classes
-        self.defines = defines.copy()
-        self.filter = filter
-
-        with open(self.toml) as f:
-            # load tests
-            config = toml.load(f)
-
-            # find line numbers
-            f.seek(0)
-            linenos = []
-            code_linenos = []
-            for i, line in enumerate(f):
-                if re.match(r'\[\[\s*case\s*\]\]', line):
-                    linenos.append(i+1)
-                if re.match(r'code\s*=\s*(\'\'\'|""")', line):
-                    code_linenos.append(i+2)
-
-            code_linenos.reverse()
-
-        # grab global config
-        for k, v in config.get('define', {}).items():
-            if k not in self.defines:
-                self.defines[k] = v
-        self.code = config.get('code', None)
-        if self.code is not None:
-            self.code_lineno = code_linenos.pop()
-
-        # create initial test cases
-        self.cases = []
-        for i, (case, lineno) in enumerate(zip(config['case'], linenos)):
-            # code lineno?
-            if 'code' in case:
-                case['code_lineno'] = code_linenos.pop()
-            # merge conditions if necessary
-            if 'if' in config and 'if' in case:
-                case['if'] = '(%s) && (%s)' % (config['if'], case['if'])
-            elif 'if' in config:
-                case['if'] = config['if']
-            # initialize test case
-            self.cases.append(TestCase(case, filter=filter,
-                suite=self, caseno=i+1, lineno=lineno, **args))
-
-    def __str__(self):
-        return self.name
-
-    def __lt__(self, other):
-        return self.name < other.name
-
-    def permute(self, **args):
-        for case in self.cases:
-            # lets find all parameterized definitions, in one of [args.D,
-            # suite.defines, case.defines, DEFINES]. Note that each of these
-            # can be either a dict of defines, or a list of dicts, expressing
-            # an initial set of permutations.
-            pending = [{}]
-            for inits in [self.defines, case.defines, DEFINES]:
-                if not isinstance(inits, list):
-                    inits = [inits]
-
-                npending = []
-                for init, pinit in it.product(inits, pending):
-                    ninit = pinit.copy()
-                    for k, v in init.items():
-                        if k not in ninit:
-                            try:
-                                ninit[k] = eval(v)
-                            except:
-                                ninit[k] = v
-                    npending.append(ninit)
-
-                pending = npending
-
-            # expand permutations
-            pending = list(reversed(pending))
-            expanded = []
-            while pending:
-                perm = pending.pop()
-                for k, v in sorted(perm.items()):
-                    if not isinstance(v, str) and isinstance(v, abc.Iterable):
-                        for nv in reversed(v):
-                            nperm = perm.copy()
-                            nperm[k] = nv
-                            pending.append(nperm)
-                        break
-                else:
-                    expanded.append(perm)
-
-            # generate permutations
-            case.perms = []
-            for i, (class_, defines) in enumerate(
-                    it.product(self.classes, expanded)):
-                case.perms.append(case.permute(
-                    class_, defines, permno=i+1, **args))
-
-            # also track non-unique defines
-            case.defines = {}
-            for k, v in case.perms[0].defines.items():
-                if all(perm.defines[k] == v for perm in case.perms):
-                    case.defines[k] = v
-
-        # track all perms and non-unique defines
-        self.perms = []
-        for case in self.cases:
-            self.perms.extend(case.perms)
-
-        self.defines = {}
-        for k, v in self.perms[0].defines.items():
-            if all(perm.defines.get(k, None) == v for perm in self.perms):
-                self.defines[k] = v
-
-        return self.perms
-
-    def build(self, **args):
-        # build test files
-        tf = open(self.path + '.test.tc', 'w')
-        tf.write(GLOBALS)
-        if self.code is not None:
-            tf.write('#line %d "%s"\n' % (self.code_lineno, self.path))
-            tf.write(self.code)
-
-        tfs = {None: tf}
-        for case in self.cases:
-            if case.in_ not in tfs:
-                tfs[case.in_] = open(self.path+'.'+
-                    re.sub('(\.c)?$', '.tc', case.in_.replace('/', '.')), 'w')
-                tfs[case.in_].write('#line 1 "%s"\n' % case.in_)
-                with open(case.in_) as f:
-                    for line in f:
-                        tfs[case.in_].write(line)
-                tfs[case.in_].write('\n')
-                tfs[case.in_].write(GLOBALS)
-
-            tfs[case.in_].write('\n')
-            case.build(tfs[case.in_], **args)
-
-        tf.write('\n')
-        tf.write('const char *lfs_testbd_path;\n')
-        tf.write('uint32_t lfs_testbd_cycles;\n')
-        tf.write('int main(int argc, char **argv) {\n')
-        tf.write(4*' '+'int case_         = (argc > 1) ? atoi(argv[1]) : 0;\n')
-        tf.write(4*' '+'int perm          = (argc > 2) ? atoi(argv[2]) : 0;\n')
-        tf.write(4*' '+'lfs_testbd_path   = (argc > 3) ? argv[3] : NULL;\n')
-        tf.write(4*' '+'lfs_testbd_cycles = (argc > 4) ? atoi(argv[4]) : 0;\n')
-        for perm in self.perms:
-            # test declaration
-            tf.write(4*' '+'extern void test_case%d(%s);\n' % (
-                perm.caseno, ', '.join(
-                    'intmax_t %s' % k for k in sorted(perm.defines)
-                    if k not in perm.case.defines)))
-            # test call
-            tf.write(4*' '+
-                'if (argc < 3 || (case_ == %d && perm == %d)) {'
-                ' test_case%d(%s); '
-                '}\n' % (perm.caseno, perm.permno, perm.caseno, ', '.join(
-                    str(v) for k, v in sorted(perm.defines.items())
-                    if k not in perm.case.defines)))
-        tf.write('}\n')
-
-        for tf in tfs.values():
-            tf.close()
-
-        # write makefiles
-        with open(self.path + '.mk', 'w') as mk:
-            mk.write(RULES.replace(4*' ', '\t') % dict(path=self.path))
-            mk.write('\n')
-
-            # add coverage hooks?
-            if args.get('coverage'):
-                mk.write(COVERAGE_RULES.replace(4*' ', '\t') % dict(
-                    path=self.path))
-                mk.write('\n')
-
-            # add truely global defines globally
-            for k, v in sorted(self.defines.items()):
-                mk.write('%s.test: override CFLAGS += -D%s=%r\n'
-                    % (self.path, k, v))
-
-            for path in tfs:
-                if path is None:
-                    mk.write('%s: %s | %s\n' % (
-                        self.path+'.test.c',
-                        self.toml,
-                        self.path+'.test.tc'))
-                else:
-                    mk.write('%s: %s %s | %s\n' % (
-                        self.path+'.'+path.replace('/', '.'),
-                        self.toml,
-                        path,
-                        self.path+'.'+re.sub('(\.c)?$', '.tc',
-                            path.replace('/', '.'))))
-                mk.write('\t./scripts/explode_asserts.py $| -o $@\n')
-
-        self.makefile = self.path + '.mk'
-        self.target = self.path + '.test'
-        return self.makefile, self.target
-
-    def test(self, **args):
-        # run test suite!
-        if not args.get('verbose', True):
-            sys.stdout.write(self.name + ' ')
-            sys.stdout.flush()
-        for perm in self.perms:
-            if not perm.shouldtest(**args):
-                continue
-
-            try:
-                result = perm.test(**args)
-            except TestFailure as failure:
-                perm.result = failure
-                if not args.get('verbose', True):
-                    sys.stdout.write(FAIL)
-                    sys.stdout.flush()
-                if not args.get('keep_going'):
-                    if not args.get('verbose', True):
-                        sys.stdout.write('\n')
-                    raise
-            else:
-                perm.result = PASS
-                if not args.get('verbose', True):
-                    sys.stdout.write(PASS)
-                    sys.stdout.flush()
+            bd.read(block, off, size)
+            return True
 
-        if not args.get('verbose', True):
-            sys.stdout.write('\n')
+        elif m.group('prog') and prog:
+            block = int(m.group('prog_block'), 0)
+            off = int(m.group('prog_off'), 0)
+            size = int(m.group('prog_size'), 0)
+
+            if block_stop is not None and block >= block_stop:
+                return False
+            block -= block_start
+            if off_stop is not None:
+                if off >= off_stop:
+                    return False
+                size = min(size, off_stop-off)
+            off -= off_start
 
-def main(**args):
-    # figure out explicit defines
-    defines = {}
-    for define in args['D']:
-        k, v, *_ = define.split('=', 2) + ['']
-        defines[k] = v
-
-    # and what class of TestCase to run
-    classes = []
-    if args.get('normal'):
-        classes.append(TestCase)
-    if args.get('reentrant'):
-        classes.append(ReentrantTestCase)
-    if args.get('valgrind'):
-        classes.append(ValgrindTestCase)
-    if not classes:
-        classes = [TestCase]
-
-    suites = []
-    for testpath in args['test_paths']:
-        # optionally specified test case/perm
-        testpath, *filter = testpath.split('#')
-        filter = [int(f) for f in filter]
-
-        # figure out the suite's toml file
-        if os.path.isdir(testpath):
-            testpath = testpath + '/*.toml'
-        elif os.path.isfile(testpath):
-            testpath = testpath
-        elif testpath.endswith('.toml'):
-            testpath = TEST_PATHS + '/' + testpath
-        else:
-            testpath = TEST_PATHS + '/' + testpath + '.toml'
-
-        # find tests
-        for path in glob.glob(testpath):
-            suites.append(TestSuite(path, classes, defines, filter, **args))
-
-    # sort for reproducability
-    suites = sorted(suites)
-
-    # generate permutations
-    for suite in suites:
-        suite.permute(**args)
-
-    # build tests in parallel
-    print('====== building ======')
-    makefiles = []
-    targets = []
-    for suite in suites:
-        makefile, target = suite.build(**args)
-        makefiles.append(makefile)
-        targets.append(target)
-
-    cmd = (['make', '-f', 'Makefile'] +
-        list(it.chain.from_iterable(['-f', m] for m in makefiles)) +
-        [target for target in targets])
-    mpty, spty = pty.openpty()
-    if args.get('verbose'):
-        print(' '.join(shlex.quote(c) for c in cmd))
-    proc = sp.Popen(cmd, stdout=spty, stderr=spty)
-    os.close(spty)
-    mpty = os.fdopen(mpty, 'r', 1)
-    stdout = []
-    while True:
-        try:
-            line = mpty.readline()
-        except OSError as e:
-            if e.errno == errno.EIO:
-                break
-            raise
-        if not line:
-            break;
-        stdout.append(line)
-        if args.get('verbose'):
-            sys.stdout.write(line)
-        # intercept warnings
-        m = re.match(
-            '^{0}([^:]+):(\d+):(?:\d+:)?{0}{1}:{0}(.*)$'
-            .format('(?:\033\[[\d;]*.| )*', 'warning'),
-            line)
-        if m and not args.get('verbose'):
-            try:
-                with open(m.group(1)) as f:
-                    lineno = int(m.group(2))
-                    line = next(it.islice(f, lineno-1, None)).strip('\n')
-                sys.stdout.write(
-                    "\033[01m{path}:{lineno}:\033[01;35mwarning:\033[m "
-                    "{message}\n{line}\n\n".format(
-                        path=m.group(1), line=line, lineno=lineno,
-                        message=m.group(3)))
-            except:
-                pass
-    proc.wait()
-    if proc.returncode != 0:
-        if not args.get('verbose'):
-            for line in stdout:
-                sys.stdout.write(line)
-        sys.exit(-1)
+            bd.prog(block, off, size)
+            return True
+
+        elif m.group('erase') and (erase or wear):
+            block = int(m.group('erase_block'), 0)
+            size = int(m.group('erase_size'), 0)
+
+            if block_stop is not None and block >= block_stop:
+                return False
+            block -= block_start
+            if off_stop is not None:
+                size = min(size, off_stop)
+            off = -off_start
+
+            bd.erase(block, off, size)
+            return True
 
-    print('built %d test suites, %d test cases, %d permutations' % (
-        len(suites),
-        sum(len(suite.cases) for suite in suites),
-        sum(len(suite.perms) for suite in suites)))
-
-    total = 0
-    for suite in suites:
-        for perm in suite.perms:
-            total += perm.shouldtest(**args)
-    if total != sum(len(suite.perms) for suite in suites):
-        print('filtered down to %d permutations' % total)
-
-    # only requested to build?
-    if args.get('build'):
-        return 0
+        else:
+            return False
+
+    # print trace output
+    def draw(f):
+        def writeln(s=''):
+            f.write(s)
+            f.write('\n')
+        f.writeln = writeln
+
+        # don't forget we've scaled this for braille/dots!
+        for row in range(
+                m.ceil(bd.height/4) if braille
+                else m.ceil(bd.height/2) if dots
+                else bd.height):
+            line = bd.draw(row,
+                read=read,
+                prog=prog,
+                erase=erase,
+                wear=wear,
+                block_cycles=block_cycles,
+                color=color,
+                dots=dots,
+                braille=braille,
+                hilbert=hilbert,
+                lebesgue=lebesgue,
+                **args)
+            if line:
+                f.writeln(line)
+
+        bd.clear()
+        resize()
+
+
+    # read/parse/coalesce operations
+    if cat:
+        ring = sys.stdout
+    else:
+        ring = LinesIO(lines)
+
+    # if sleep print in background thread to avoid getting stuck in a read call
+    event = th.Event()
+    lock = th.Lock()
+    if sleep:
+        done = False
+        def background():
+            while not done:
+                event.wait()
+                event.clear()
+                with lock:
+                    draw(ring)
+                    if not cat:
+                        ring.draw()
+                time.sleep(sleep or 0.01)
+        th.Thread(target=background, daemon=True).start()
 
-    print('====== testing ======')
     try:
-        for suite in suites:
-            suite.test(**args)
-    except TestFailure:
+        while True:
+            with openio(path) as f:
+                changed = 0
+                for line in f:
+                    with lock:
+                        changed += parse(line)
+
+                        # need to redraw?
+                        if changed and (not coalesce or changed >= coalesce):
+                            if sleep:
+                                event.set()
+                            else:
+                                draw(ring)
+                                if not cat:
+                                    ring.draw()
+                            changed = 0
+
+            if not keep_open:
+                break
+            # don't just flood open calls
+            time.sleep(sleep or 0.1)
+    except FileNotFoundError as e:
+        print("error: file not found %r" % path)
+        sys.exit(-1)
+    except KeyboardInterrupt:
         pass
 
-    print('====== results ======')
-    passed = 0
-    failed = 0
-    for suite in suites:
-        for perm in suite.perms:
-            if perm.result == PASS:
-                passed += 1
-            elif isinstance(perm.result, TestFailure):
-                sys.stdout.write(
-                    "\033[01m{path}:{lineno}:\033[01;31mfailure:\033[m "
-                    "{perm} failed\n".format(
-                        perm=perm, path=perm.suite.path, lineno=perm.lineno,
-                        returncode=perm.result.returncode or 0))
-                if perm.result.stdout:
-                    if perm.result.assert_:
-                        stdout = perm.result.stdout[:-1]
-                    else:
-                        stdout = perm.result.stdout
-                    for line in stdout[-5:]:
-                        sys.stdout.write(line)
-                if perm.result.assert_:
-                    sys.stdout.write(
-                        "\033[01m{path}:{lineno}:\033[01;31massert:\033[m "
-                        "{message}\n{line}\n".format(
-                            **perm.result.assert_))
-                sys.stdout.write('\n')
-                failed += 1
-
-    if args.get('coverage'):
-        # collect coverage info
-        # why -j1? lcov doesn't work in parallel because of gcov limitations
-        cmd = (['make', '-j1', '-f', 'Makefile'] +
-            list(it.chain.from_iterable(['-f', m] for m in makefiles)) +
-            (['COVERAGETARGET=%s' % args['coverage']]
-                if isinstance(args['coverage'], str) else []) +
-            [suite.path + '.info' for suite in suites
-                if any(perm.result == PASS for perm in suite.perms)])
-        if args.get('verbose'):
-            print(' '.join(shlex.quote(c) for c in cmd))
-        proc = sp.Popen(cmd,
-            stdout=sp.PIPE if not args.get('verbose') else None,
-            stderr=sp.STDOUT if not args.get('verbose') else None,
-            universal_newlines=True)
-        proc.wait()
-        if proc.returncode != 0:
-            if not args.get('verbose'):
-                for line in proc.stdout:
-                    sys.stdout.write(line)
-            sys.exit(-1)
-
-    if args.get('gdb'):
-        failure = None
-        for suite in suites:
-            for perm in suite.perms:
-                if isinstance(perm.result, TestFailure):
-                    failure = perm.result
-        if failure is not None:
-            print('======= gdb ======')
-            # drop into gdb
-            failure.case.test(failure=failure, **args)
-            sys.exit(0)
-
-    print('tests passed %d/%d (%.2f%%)' % (passed, total,
-        100*(passed/total if total else 1.0)))
-    print('tests failed %d/%d (%.2f%%)' % (failed, total,
-        100*(failed/total if total else 1.0)))
-    return 1 if failed > 0 else 0
+    if sleep:
+        done = True
+        lock.acquire() # avoids https://bugs.python.org/issue42717
+    if not cat:
+        sys.stdout.write('\n')
+
 
 if __name__ == "__main__":
+    import sys
     import argparse
     parser = argparse.ArgumentParser(
-        description="Run parameterized tests in various configurations.")
-    parser.add_argument('test_paths', nargs='*', default=[TEST_PATHS],
-        help="Description of test(s) to run. By default, this is all tests \
-            found in the \"{0}\" directory. Here, you can specify a different \
-            directory of tests, a specific file, a suite by name, and even \
-            specific test cases and permutations. For example \
-            \"test_dirs#1\" or \"{0}/test_dirs.toml#1#1\".".format(TEST_PATHS))
-    parser.add_argument('-D', action='append', default=[],
-        help="Overriding parameter definitions.")
-    parser.add_argument('-v', '--verbose', action='store_true',
-        help="Output everything that is happening.")
-    parser.add_argument('-k', '--keep-going', action='store_true',
-        help="Run all tests instead of stopping on first error. Useful for CI.")
-    parser.add_argument('-p', '--persist', choices=['erase', 'noerase'],
-        nargs='?', const='erase',
-        help="Store disk image in a file.")
-    parser.add_argument('-b', '--build', action='store_true',
-        help="Only build the tests, do not execute.")
-    parser.add_argument('-g', '--gdb', choices=['init', 'main', 'assert'],
-        nargs='?', const='assert',
-        help="Drop into gdb on test failure.")
-    parser.add_argument('--no-internal', action='store_true',
-        help="Don't run tests that require internal knowledge.")
-    parser.add_argument('-n', '--normal', action='store_true',
-        help="Run tests normally.")
-    parser.add_argument('-r', '--reentrant', action='store_true',
-        help="Run reentrant tests with simulated power-loss.")
-    parser.add_argument('--valgrind', action='store_true',
-        help="Run non-leaky tests under valgrind to check for memory leaks.")
-    parser.add_argument('--exec', default=[], type=lambda e: e.split(),
-        help="Run tests with another executable prefixed on the command line.")
-    parser.add_argument('--disk',
-        help="Specify a file to use for persistent/reentrant tests.")
-    parser.add_argument('--coverage', type=lambda x: x if x else True,
-        nargs='?', const='',
-        help="Collect coverage information during testing. This uses lcov/gcov \
-            to accumulate coverage information into *.info files. May also \
-            a path to a *.info file to accumulate coverage info into.")
-    parser.add_argument('--build-dir',
-        help="Build relative to the specified directory instead of the \
-            current directory.")
-
-    sys.exit(main(**vars(parser.parse_args())))
+        description="Display operations on block devices based on "
+            "trace output.",
+        allow_abbrev=False)
+    parser.add_argument(
+        'path',
+        nargs='?',
+        help="Path to read from.")
+    parser.add_argument(
+        '-r', '--read',
+        action='store_true',
+        help="Render reads.")
+    parser.add_argument(
+        '-p', '--prog',
+        action='store_true',
+        help="Render progs.")
+    parser.add_argument(
+        '-e', '--erase',
+        action='store_true',
+        help="Render erases.")
+    parser.add_argument(
+        '-w', '--wear',
+        action='store_true',
+        help="Render wear.")
+    parser.add_argument(
+        '-b', '--block',
+        type=lambda x: tuple(
+            int(x, 0) if x.strip() else None
+            for x in x.split(',')),
+        help="Show a specific block or range of blocks.")
+    parser.add_argument(
+        '-i', '--off',
+        type=lambda x: tuple(
+            int(x, 0) if x.strip() else None
+            for x in x.split(',')),
+        help="Show a specific offset or range of offsets.")
+    parser.add_argument(
+        '-B', '--block-size',
+        type=lambda x: int(x, 0),
+        help="Assume a specific block size.")
+    parser.add_argument(
+        '--block-count',
+        type=lambda x: int(x, 0),
+        help="Assume a specific block count.")
+    parser.add_argument(
+        '-C', '--block-cycles',
+        type=lambda x: int(x, 0),
+        help="Assumed maximum number of erase cycles when measuring wear.")
+    parser.add_argument(
+        '-R', '--reset',
+        action='store_true',
+        help="Reset wear on block device initialization.")
+    parser.add_argument(
+        '--color',
+        choices=['never', 'always', 'auto'],
+        default='auto',
+        help="When to use terminal colors. Defaults to 'auto'.")
+    parser.add_argument(
+        '--subscripts',
+        action='store_true',
+        help="Use unicode subscripts for showing wear.")
+    parser.add_argument(
+        '-:', '--dots',
+        action='store_true',
+        help="Use 1x2 ascii dot characters.")
+    parser.add_argument(
+        '-⣿', '--braille',
+        action='store_true',
+        help="Use 2x4 unicode braille characters. Note that braille characters "
+            "sometimes suffer from inconsistent widths.")
+    parser.add_argument(
+        '--chars',
+        help="Characters to use for read, prog, erase, noop operations.")
+    parser.add_argument(
+        '--wear-chars',
+        help="Characters to use for showing wear.")
+    parser.add_argument(
+        '--colors',
+        type=lambda x: [x.strip() for x in x.split(',')],
+        help="Colors to use for read, prog, erase, noop operations.")
+    parser.add_argument(
+        '--wear-colors',
+        type=lambda x: [x.strip() for x in x.split(',')],
+        help="Colors to use for showing wear.")
+    parser.add_argument(
+        '-W', '--width',
+        nargs='?',
+        type=lambda x: int(x, 0),
+        const=0,
+        help="Width in columns. 0 uses the terminal width. Defaults to "
+            "min(terminal, 80).")
+    parser.add_argument(
+        '-H', '--height',
+        nargs='?',
+        type=lambda x: int(x, 0),
+        const=0,
+        help="Height in rows. 0 uses the terminal height. Defaults to 1.")
+    parser.add_argument(
+        '-n', '--lines',
+        nargs='?',
+        type=lambda x: int(x, 0),
+        const=0,
+        help="Show this many lines of history. 0 uses the terminal height. "
+            "Defaults to 5.")
+    parser.add_argument(
+        '-z', '--cat',
+        action='store_true',
+        help="Pipe directly to stdout.")
+    parser.add_argument(
+        '-U', '--hilbert',
+        action='store_true',
+        help="Render as a space-filling Hilbert curve.")
+    parser.add_argument(
+        '-Z', '--lebesgue',
+        action='store_true',
+        help="Render as a space-filling Z-curve.")
+    parser.add_argument(
+        '-c', '--coalesce',
+        type=lambda x: int(x, 0),
+        help="Number of operations to coalesce together.")
+    parser.add_argument(
+        '-s', '--sleep',
+        type=float,
+        help="Time in seconds to sleep between reads, coalescing operations.")
+    parser.add_argument(
+        '-k', '--keep-open',
+        action='store_true',
+        help="Reopen the pipe on EOF, useful when multiple "
+            "processes are writing.")
+    sys.exit(main(**{k: v
+        for k, v in vars(parser.parse_intermixed_args()).items()
+        if v is not None}))
```

### Comparing `littlefs-python-0.4.0/littlefs/tests/test_alloc.toml` & `littlefs-python-0.5.0/littlefs/tests/test_alloc.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,205 +1,239 @@
 # allocator tests
 # note for these to work there are a number constraints on the device geometry
-if = 'LFS_BLOCK_CYCLES == -1'
+if = 'BLOCK_CYCLES == -1'
 
-[[case]] # parallel allocation test
-define.FILES = 3
-define.SIZE = '(((LFS_BLOCK_SIZE-8)*(LFS_BLOCK_COUNT-6)) / FILES)'
+# parallel allocation test
+[cases.test_alloc_parallel]
+defines.FILES = 3
+defines.SIZE = '(((BLOCK_SIZE-8)*(BLOCK_COUNT-6)) / FILES)'
 code = '''
-    const char *names[FILES] = {"bacon", "eggs", "pancakes"};
+    const char *names[] = {"bacon", "eggs", "pancakes"};
     lfs_file_t files[FILES];
 
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "breakfast") => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int n = 0; n < FILES; n++) {
+        char path[1024];
         sprintf(path, "breakfast/%s", names[n]);
         lfs_file_open(&lfs, &files[n], path,
                 LFS_O_WRONLY | LFS_O_CREAT | LFS_O_APPEND) => 0;
     }
     for (int n = 0; n < FILES; n++) {
-        size = strlen(names[n]);
+        size_t size = strlen(names[n]);
         for (lfs_size_t i = 0; i < SIZE; i += size) {
             lfs_file_write(&lfs, &files[n], names[n], size) => size;
         }
     }
     for (int n = 0; n < FILES; n++) {
         lfs_file_close(&lfs, &files[n]) => 0;
     }
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int n = 0; n < FILES; n++) {
+        char path[1024];
         sprintf(path, "breakfast/%s", names[n]);
+        lfs_file_t file;
         lfs_file_open(&lfs, &file, path, LFS_O_RDONLY) => 0;
-        size = strlen(names[n]);
+        size_t size = strlen(names[n]);
         for (lfs_size_t i = 0; i < SIZE; i += size) {
+            uint8_t buffer[1024];
             lfs_file_read(&lfs, &file, buffer, size) => size;
             assert(memcmp(buffer, names[n], size) == 0);
         }
         lfs_file_close(&lfs, &file) => 0;
     }
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # serial allocation test
-define.FILES = 3
-define.SIZE = '(((LFS_BLOCK_SIZE-8)*(LFS_BLOCK_COUNT-6)) / FILES)'
-code = '''
-    const char *names[FILES] = {"bacon", "eggs", "pancakes"};
-
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+# serial allocation test
+[cases.test_alloc_serial]
+defines.FILES = 3
+defines.SIZE = '(((BLOCK_SIZE-8)*(BLOCK_COUNT-6)) / FILES)'
+code = '''
+    const char *names[] = {"bacon", "eggs", "pancakes"};
+
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "breakfast") => 0;
     lfs_unmount(&lfs) => 0;
 
     for (int n = 0; n < FILES; n++) {
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
+        char path[1024];
         sprintf(path, "breakfast/%s", names[n]);
+        lfs_file_t file;
         lfs_file_open(&lfs, &file, path,
                 LFS_O_WRONLY | LFS_O_CREAT | LFS_O_APPEND) => 0;
-        size = strlen(names[n]);
+        size_t size = strlen(names[n]);
+        uint8_t buffer[1024];
         memcpy(buffer, names[n], size);
         for (int i = 0; i < SIZE; i += size) {
             lfs_file_write(&lfs, &file, buffer, size) => size;
         }
         lfs_file_close(&lfs, &file) => 0;
         lfs_unmount(&lfs) => 0;
     }
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int n = 0; n < FILES; n++) {
+        char path[1024];
         sprintf(path, "breakfast/%s", names[n]);
+        lfs_file_t file;
         lfs_file_open(&lfs, &file, path, LFS_O_RDONLY) => 0;
-        size = strlen(names[n]);
+        size_t size = strlen(names[n]);
         for (int i = 0; i < SIZE; i += size) {
+            uint8_t buffer[1024];
             lfs_file_read(&lfs, &file, buffer, size) => size;
             assert(memcmp(buffer, names[n], size) == 0);
         }
         lfs_file_close(&lfs, &file) => 0;
     }
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # parallel allocation reuse test
-define.FILES = 3
-define.SIZE = '(((LFS_BLOCK_SIZE-8)*(LFS_BLOCK_COUNT-6)) / FILES)'
-define.CYCLES = [1, 10]
+# parallel allocation reuse test
+[cases.test_alloc_parallel_reuse]
+defines.FILES = 3
+defines.SIZE = '(((BLOCK_SIZE-8)*(BLOCK_COUNT-6)) / FILES)'
+defines.CYCLES = [1, 10]
 code = '''
-    const char *names[FILES] = {"bacon", "eggs", "pancakes"};
+    const char *names[] = {"bacon", "eggs", "pancakes"};
     lfs_file_t files[FILES];
 
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
     for (int c = 0; c < CYCLES; c++) {
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         lfs_mkdir(&lfs, "breakfast") => 0;
         lfs_unmount(&lfs) => 0;
 
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         for (int n = 0; n < FILES; n++) {
+            char path[1024];
             sprintf(path, "breakfast/%s", names[n]);
             lfs_file_open(&lfs, &files[n], path,
                     LFS_O_WRONLY | LFS_O_CREAT | LFS_O_APPEND) => 0;
         }
         for (int n = 0; n < FILES; n++) {
-            size = strlen(names[n]);
+            size_t size = strlen(names[n]);
             for (int i = 0; i < SIZE; i += size) {
                 lfs_file_write(&lfs, &files[n], names[n], size) => size;
             }
         }
         for (int n = 0; n < FILES; n++) {
             lfs_file_close(&lfs, &files[n]) => 0;
         }
         lfs_unmount(&lfs) => 0;
 
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         for (int n = 0; n < FILES; n++) {
+            char path[1024];
             sprintf(path, "breakfast/%s", names[n]);
+            lfs_file_t file;
             lfs_file_open(&lfs, &file, path, LFS_O_RDONLY) => 0;
-            size = strlen(names[n]);
+            size_t size = strlen(names[n]);
             for (int i = 0; i < SIZE; i += size) {
+                uint8_t buffer[1024];
                 lfs_file_read(&lfs, &file, buffer, size) => size;
                 assert(memcmp(buffer, names[n], size) == 0);
             }
             lfs_file_close(&lfs, &file) => 0;
         }
         lfs_unmount(&lfs) => 0;
 
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         for (int n = 0; n < FILES; n++) {
+            char path[1024];
             sprintf(path, "breakfast/%s", names[n]);
             lfs_remove(&lfs, path) => 0;
         }
         lfs_remove(&lfs, "breakfast") => 0;
         lfs_unmount(&lfs) => 0;
     }
 '''
 
-[[case]] # serial allocation reuse test
-define.FILES = 3
-define.SIZE = '(((LFS_BLOCK_SIZE-8)*(LFS_BLOCK_COUNT-6)) / FILES)'
-define.CYCLES = [1, 10]
+# serial allocation reuse test
+[cases.test_alloc_serial_reuse]
+defines.FILES = 3
+defines.SIZE = '(((BLOCK_SIZE-8)*(BLOCK_COUNT-6)) / FILES)'
+defines.CYCLES = [1, 10]
 code = '''
-    const char *names[FILES] = {"bacon", "eggs", "pancakes"};
+    const char *names[] = {"bacon", "eggs", "pancakes"};
 
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
     for (int c = 0; c < CYCLES; c++) {
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         lfs_mkdir(&lfs, "breakfast") => 0;
         lfs_unmount(&lfs) => 0;
 
         for (int n = 0; n < FILES; n++) {
-            lfs_mount(&lfs, &cfg) => 0;
+            lfs_mount(&lfs, cfg) => 0;
+            char path[1024];
             sprintf(path, "breakfast/%s", names[n]);
+            lfs_file_t file;
             lfs_file_open(&lfs, &file, path,
                     LFS_O_WRONLY | LFS_O_CREAT | LFS_O_APPEND) => 0;
-            size = strlen(names[n]);
+            size_t size = strlen(names[n]);
+            uint8_t buffer[1024];
             memcpy(buffer, names[n], size);
             for (int i = 0; i < SIZE; i += size) {
                 lfs_file_write(&lfs, &file, buffer, size) => size;
             }
             lfs_file_close(&lfs, &file) => 0;
             lfs_unmount(&lfs) => 0;
         }
 
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         for (int n = 0; n < FILES; n++) {
+            char path[1024];
             sprintf(path, "breakfast/%s", names[n]);
+            lfs_file_t file;
             lfs_file_open(&lfs, &file, path, LFS_O_RDONLY) => 0;
-            size = strlen(names[n]);
+            size_t size = strlen(names[n]);
             for (int i = 0; i < SIZE; i += size) {
+                uint8_t buffer[1024];
                 lfs_file_read(&lfs, &file, buffer, size) => size;
                 assert(memcmp(buffer, names[n], size) == 0);
             }
             lfs_file_close(&lfs, &file) => 0;
         }
         lfs_unmount(&lfs) => 0;
 
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         for (int n = 0; n < FILES; n++) {
+            char path[1024];
             sprintf(path, "breakfast/%s", names[n]);
             lfs_remove(&lfs, path) => 0;
         }
         lfs_remove(&lfs, "breakfast") => 0;
         lfs_unmount(&lfs) => 0;
     }
 '''
 
-[[case]] # exhaustion test
+# exhaustion test
+[cases.test_alloc_exhaustion]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "exhaustion", LFS_O_WRONLY | LFS_O_CREAT);
-    size = strlen("exhaustion");
+    size_t size = strlen("exhaustion");
+    uint8_t buffer[1024];
     memcpy(buffer, "exhaustion", size);
     lfs_file_write(&lfs, &file, buffer, size) => size;
     lfs_file_sync(&lfs, &file) => 0;
 
     size = strlen("blahblahblahblah");
     memcpy(buffer, "blahblahblahblah", size);
     lfs_ssize_t res;
@@ -212,32 +246,36 @@
         res => size;
     }
     res => LFS_ERR_NOSPC;
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "exhaustion", LFS_O_RDONLY);
     size = strlen("exhaustion");
     lfs_file_size(&lfs, &file) => size;
     lfs_file_read(&lfs, &file, buffer, size) => size;
     memcmp(buffer, "exhaustion", size) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # exhaustion wraparound test
-define.SIZE = '(((LFS_BLOCK_SIZE-8)*(LFS_BLOCK_COUNT-4)) / 3)'
-code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+# exhaustion wraparound test
+[cases.test_alloc_exhaustion_wraparound]
+defines.SIZE = '(((BLOCK_SIZE-8)*(BLOCK_COUNT-4)) / 3)'
+code = '''
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "padding", LFS_O_WRONLY | LFS_O_CREAT);
-    size = strlen("buffering");
+    size_t size = strlen("buffering");
+    uint8_t buffer[1024];
     memcpy(buffer, "buffering", size);
     for (int i = 0; i < SIZE; i += size) {
         lfs_file_write(&lfs, &file, buffer, size) => size;
     }
     lfs_file_close(&lfs, &file) => 0;
     lfs_remove(&lfs, "padding") => 0;
 
@@ -259,36 +297,41 @@
         res => size;
     }
     res => LFS_ERR_NOSPC;
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "exhaustion", LFS_O_RDONLY);
     size = strlen("exhaustion");
     lfs_file_size(&lfs, &file) => size;
     lfs_file_read(&lfs, &file, buffer, size) => size;
     memcmp(buffer, "exhaustion", size) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_remove(&lfs, "exhaustion") => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # dir exhaustion test
+# dir exhaustion test
+[cases.test_alloc_dir_exhaustion]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     // find out max file size
     lfs_mkdir(&lfs, "exhaustiondir") => 0;
-    size = strlen("blahblahblahblah");
+    size_t size = strlen("blahblahblahblah");
+    uint8_t buffer[1024];
     memcpy(buffer, "blahblahblahblah", size);
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "exhaustion", LFS_O_WRONLY | LFS_O_CREAT);
     int count = 0;
+    int err;
     while (true) {
         err = lfs_file_write(&lfs, &file, buffer, size);
         if (err < 0) {
             break;
         }
 
         count += 1;
@@ -319,69 +362,73 @@
 
     lfs_mkdir(&lfs, "exhaustiondir") => LFS_ERR_NOSPC;
 
     lfs_remove(&lfs, "exhaustion") => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # what if we have a bad block during an allocation scan?
+# what if we have a bad block during an allocation scan?
+[cases.test_alloc_bad_blocks]
 in = "lfs.c"
-define.LFS_ERASE_CYCLES = 0xffffffff
-define.LFS_BADBLOCK_BEHAVIOR = 'LFS_TESTBD_BADBLOCK_READERROR'
+defines.ERASE_CYCLES = 0xffffffff
+defines.BADBLOCK_BEHAVIOR = 'LFS_EMUBD_BADBLOCK_READERROR'
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     // first fill to exhaustion to find available space
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "pacman", LFS_O_WRONLY | LFS_O_CREAT) => 0;
+    uint8_t buffer[1024];
     strcpy((char*)buffer, "waka");
-    size = strlen("waka");
+    size_t size = strlen("waka");
     lfs_size_t filesize = 0;
     while (true) {
         lfs_ssize_t res = lfs_file_write(&lfs, &file, buffer, size);
         assert(res == (lfs_ssize_t)size || res == LFS_ERR_NOSPC);
         if (res == LFS_ERR_NOSPC) {
             break;
         }
         filesize += size;
     }
     lfs_file_close(&lfs, &file) => 0;
     // now fill all but a couple of blocks of the filesystem with data
-    filesize -= 3*LFS_BLOCK_SIZE;
+    filesize -= 3*BLOCK_SIZE;
     lfs_file_open(&lfs, &file, "pacman", LFS_O_WRONLY | LFS_O_CREAT) => 0;
     strcpy((char*)buffer, "waka");
     size = strlen("waka");
     for (lfs_size_t i = 0; i < filesize/size; i++) {
         lfs_file_write(&lfs, &file, buffer, size) => size;
     }
     lfs_file_close(&lfs, &file) => 0;
     // also save head of file so we can error during lookahead scan
     lfs_block_t fileblock = file.ctz.head;
     lfs_unmount(&lfs) => 0;
 
     // remount to force an alloc scan
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     // but mark the head of our file as a "bad block", this is force our
     // scan to bail early
-    lfs_testbd_setwear(&cfg, fileblock, 0xffffffff) => 0;
+    lfs_emubd_setwear(cfg, fileblock, 0xffffffff) => 0;
     lfs_file_open(&lfs, &file, "ghost", LFS_O_WRONLY | LFS_O_CREAT) => 0;
     strcpy((char*)buffer, "chomp");
     size = strlen("chomp");
     while (true) {
         lfs_ssize_t res = lfs_file_write(&lfs, &file, buffer, size);
         assert(res == (lfs_ssize_t)size || res == LFS_ERR_CORRUPT);
         if (res == LFS_ERR_CORRUPT) {
             break;
         }
     }
     lfs_file_close(&lfs, &file) => 0;
 
     // now reverse the "bad block" and try to write the file again until we
     // run out of space
-    lfs_testbd_setwear(&cfg, fileblock, 0) => 0;
+    lfs_emubd_setwear(cfg, fileblock, 0) => 0;
     lfs_file_open(&lfs, &file, "ghost", LFS_O_WRONLY | LFS_O_CREAT) => 0;
     strcpy((char*)buffer, "chomp");
     size = strlen("chomp");
     while (true) {
         lfs_ssize_t res = lfs_file_write(&lfs, &file, buffer, size);
         assert(res == (lfs_ssize_t)size || res == LFS_ERR_NOSPC);
         if (res == LFS_ERR_NOSPC) {
@@ -389,15 +436,15 @@
         }
     }
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_unmount(&lfs) => 0;
 
     // check that the disk isn't hurt
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "pacman", LFS_O_RDONLY) => 0;
     strcpy((char*)buffer, "waka");
     size = strlen("waka");
     for (lfs_size_t i = 0; i < filesize/size; i++) {
         uint8_t rbuffer[4];
         lfs_file_read(&lfs, &file, rbuffer, size) => size;
         assert(memcmp(rbuffer, buffer, size) == 0);
@@ -407,58 +454,65 @@
 '''
 
 
 # Below, I don't like these tests. They're fragile and depend _heavily_
 # on the geometry of the block device. But they are valuable. Eventually they
 # should be removed and replaced with generalized tests.
 
-[[case]] # chained dir exhaustion test
-define.LFS_BLOCK_SIZE = 512
-define.LFS_BLOCK_COUNT = 1024
-if = 'LFS_BLOCK_SIZE == 512 && LFS_BLOCK_COUNT == 1024'
-code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+# chained dir exhaustion test
+[cases.test_alloc_chained_dir_exhaustion]
+if = 'BLOCK_SIZE == 512'
+defines.BLOCK_COUNT = 1024
+code = '''
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     // find out max file size
     lfs_mkdir(&lfs, "exhaustiondir") => 0;
     for (int i = 0; i < 10; i++) {
+        char path[1024];
         sprintf(path, "dirwithanexhaustivelylongnameforpadding%d", i);
         lfs_mkdir(&lfs, path) => 0;
     }
-    size = strlen("blahblahblahblah");
+    size_t size = strlen("blahblahblahblah");
+    uint8_t buffer[1024];
     memcpy(buffer, "blahblahblahblah", size);
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "exhaustion", LFS_O_WRONLY | LFS_O_CREAT);
     int count = 0;
+    int err;
     while (true) {
         err = lfs_file_write(&lfs, &file, buffer, size);
         if (err < 0) {
             break;
         }
 
         count += 1;
     }
     err => LFS_ERR_NOSPC;
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_remove(&lfs, "exhaustion") => 0;
     lfs_remove(&lfs, "exhaustiondir") => 0;
     for (int i = 0; i < 10; i++) {
+        char path[1024];
         sprintf(path, "dirwithanexhaustivelylongnameforpadding%d", i);
         lfs_remove(&lfs, path) => 0;
     }
 
     // see that chained dir fails
     lfs_file_open(&lfs, &file, "exhaustion", LFS_O_WRONLY | LFS_O_CREAT);
     for (int i = 0; i < count+1; i++) {
         lfs_file_write(&lfs, &file, buffer, size) => size;
     }
     lfs_file_sync(&lfs, &file) => 0;
 
     for (int i = 0; i < 10; i++) {
+        char path[1024];
         sprintf(path, "dirwithanexhaustivelylongnameforpadding%d", i);
         lfs_mkdir(&lfs, path) => 0;
     }
 
     lfs_mkdir(&lfs, "exhaustiondir") => LFS_ERR_NOSPC;
 
     // shorten file to try a second chained dir
@@ -478,167 +532,177 @@
 
     lfs_mkdir(&lfs, "exhaustiondir2") => LFS_ERR_NOSPC;
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # split dir test
-define.LFS_BLOCK_SIZE = 512
-define.LFS_BLOCK_COUNT = 1024
-if = 'LFS_BLOCK_SIZE == 512 && LFS_BLOCK_COUNT == 1024'
-code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+# split dir test
+[cases.test_alloc_split_dir]
+if = 'BLOCK_SIZE == 512'
+defines.BLOCK_COUNT = 1024
+code = '''
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     // create one block hole for half a directory
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "bump", LFS_O_WRONLY | LFS_O_CREAT) => 0;
-    for (lfs_size_t i = 0; i < cfg.block_size; i += 2) {
+    for (lfs_size_t i = 0; i < cfg->block_size; i += 2) {
+        uint8_t buffer[1024];
         memcpy(&buffer[i], "hi", 2);
     }
-    lfs_file_write(&lfs, &file, buffer, cfg.block_size) => cfg.block_size;
+    uint8_t buffer[1024];
+    lfs_file_write(&lfs, &file, buffer, cfg->block_size) => cfg->block_size;
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_file_open(&lfs, &file, "exhaustion", LFS_O_WRONLY | LFS_O_CREAT);
-    size = strlen("blahblahblahblah");
+    size_t size = strlen("blahblahblahblah");
     memcpy(buffer, "blahblahblahblah", size);
     for (lfs_size_t i = 0;
-            i < (cfg.block_count-4)*(cfg.block_size-8);
+            i < (cfg->block_count-4)*(cfg->block_size-8);
             i += size) {
         lfs_file_write(&lfs, &file, buffer, size) => size;
     }
     lfs_file_close(&lfs, &file) => 0;
 
     // remount to force reset of lookahead
     lfs_unmount(&lfs) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     // open hole
     lfs_remove(&lfs, "bump") => 0;
 
     lfs_mkdir(&lfs, "splitdir") => 0;
     lfs_file_open(&lfs, &file, "splitdir/bump",
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
-    for (lfs_size_t i = 0; i < cfg.block_size; i += 2) {
+    for (lfs_size_t i = 0; i < cfg->block_size; i += 2) {
         memcpy(&buffer[i], "hi", 2);
     }
-    lfs_file_write(&lfs, &file, buffer, 2*cfg.block_size) => LFS_ERR_NOSPC;
+    lfs_file_write(&lfs, &file, buffer, 2*cfg->block_size) => LFS_ERR_NOSPC;
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # outdated lookahead test
-define.LFS_BLOCK_SIZE = 512
-define.LFS_BLOCK_COUNT = 1024
-if = 'LFS_BLOCK_SIZE == 512 && LFS_BLOCK_COUNT == 1024'
+# outdated lookahead test
+[cases.test_alloc_outdated_lookahead]
+if = 'BLOCK_SIZE == 512'
+defines.BLOCK_COUNT = 1024
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     // fill completely with two files
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "exhaustion1",
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
-    size = strlen("blahblahblahblah");
+    size_t size = strlen("blahblahblahblah");
+    uint8_t buffer[1024];
     memcpy(buffer, "blahblahblahblah", size);
     for (lfs_size_t i = 0;
-            i < ((cfg.block_count-2)/2)*(cfg.block_size-8);
+            i < ((cfg->block_count-2)/2)*(cfg->block_size-8);
             i += size) {
         lfs_file_write(&lfs, &file, buffer, size) => size;
     }
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_file_open(&lfs, &file, "exhaustion2",
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
     size = strlen("blahblahblahblah");
     memcpy(buffer, "blahblahblahblah", size);
     for (lfs_size_t i = 0;
-            i < ((cfg.block_count-2+1)/2)*(cfg.block_size-8);
+            i < ((cfg->block_count-2+1)/2)*(cfg->block_size-8);
             i += size) {
         lfs_file_write(&lfs, &file, buffer, size) => size;
     }
     lfs_file_close(&lfs, &file) => 0;
 
     // remount to force reset of lookahead
     lfs_unmount(&lfs) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     // rewrite one file
     lfs_file_open(&lfs, &file, "exhaustion1",
             LFS_O_WRONLY | LFS_O_TRUNC) => 0;
     lfs_file_sync(&lfs, &file) => 0;
     size = strlen("blahblahblahblah");
     memcpy(buffer, "blahblahblahblah", size);
     for (lfs_size_t i = 0;
-            i < ((cfg.block_count-2)/2)*(cfg.block_size-8);
+            i < ((cfg->block_count-2)/2)*(cfg->block_size-8);
             i += size) {
         lfs_file_write(&lfs, &file, buffer, size) => size;
     }
     lfs_file_close(&lfs, &file) => 0;
 
     // rewrite second file, this requires lookahead does not
     // use old population
     lfs_file_open(&lfs, &file, "exhaustion2",
             LFS_O_WRONLY | LFS_O_TRUNC) => 0;
     lfs_file_sync(&lfs, &file) => 0;
     size = strlen("blahblahblahblah");
     memcpy(buffer, "blahblahblahblah", size);
     for (lfs_size_t i = 0;
-            i < ((cfg.block_count-2+1)/2)*(cfg.block_size-8);
+            i < ((cfg->block_count-2+1)/2)*(cfg->block_size-8);
             i += size) {
         lfs_file_write(&lfs, &file, buffer, size) => size;
     }
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # outdated lookahead and split dir test
-define.LFS_BLOCK_SIZE = 512
-define.LFS_BLOCK_COUNT = 1024
-if = 'LFS_BLOCK_SIZE == 512 && LFS_BLOCK_COUNT == 1024'
-code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+# outdated lookahead and split dir test
+[cases.test_alloc_outdated_lookahead_split_dir]
+if = 'BLOCK_SIZE == 512'
+defines.BLOCK_COUNT = 1024
+code = '''
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     // fill completely with two files
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "exhaustion1",
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
-    size = strlen("blahblahblahblah");
+    size_t size = strlen("blahblahblahblah");
+    uint8_t buffer[1024];
     memcpy(buffer, "blahblahblahblah", size);
     for (lfs_size_t i = 0;
-            i < ((cfg.block_count-2)/2)*(cfg.block_size-8);
+            i < ((cfg->block_count-2)/2)*(cfg->block_size-8);
             i += size) {
         lfs_file_write(&lfs, &file, buffer, size) => size;
     }
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_file_open(&lfs, &file, "exhaustion2",
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
     size = strlen("blahblahblahblah");
     memcpy(buffer, "blahblahblahblah", size);
     for (lfs_size_t i = 0;
-            i < ((cfg.block_count-2+1)/2)*(cfg.block_size-8);
+            i < ((cfg->block_count-2+1)/2)*(cfg->block_size-8);
             i += size) {
         lfs_file_write(&lfs, &file, buffer, size) => size;
     }
     lfs_file_close(&lfs, &file) => 0;
 
     // remount to force reset of lookahead
     lfs_unmount(&lfs) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     // rewrite one file with a hole of one block
     lfs_file_open(&lfs, &file, "exhaustion1",
             LFS_O_WRONLY | LFS_O_TRUNC) => 0;
     lfs_file_sync(&lfs, &file) => 0;
     size = strlen("blahblahblahblah");
     memcpy(buffer, "blahblahblahblah", size);
     for (lfs_size_t i = 0;
-            i < ((cfg.block_count-2)/2 - 1)*(cfg.block_size-8);
+            i < ((cfg->block_count-2)/2 - 1)*(cfg->block_size-8);
             i += size) {
         lfs_file_write(&lfs, &file, buffer, size) => size;
     }
     lfs_file_close(&lfs, &file) => 0;
 
     // try to allocate a directory, should fail!
     lfs_mkdir(&lfs, "split") => LFS_ERR_NOSPC;
```

### Comparing `littlefs-python-0.4.0/littlefs/tests/test_attrs.toml` & `littlefs-python-0.5.0/littlefs/tests/test_attrs.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-[[case]] # set/get attribute
+[cases.test_attrs_get_set]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "hello") => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "hello/hello", LFS_O_WRONLY | LFS_O_CREAT) => 0;
     lfs_file_write(&lfs, &file, "hello", strlen("hello")) => strlen("hello");
     lfs_file_close(&lfs, &file);
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    uint8_t buffer[1024];
     memset(buffer, 0, sizeof(buffer));
     lfs_setattr(&lfs, "hello", 'A', "aaaa",   4) => 0;
     lfs_setattr(&lfs, "hello", 'B', "bbbbbb", 6) => 0;
     lfs_setattr(&lfs, "hello", 'C', "ccccc",  5) => 0;
     lfs_getattr(&lfs, "hello", 'A', buffer,    4) => 4;
     lfs_getattr(&lfs, "hello", 'B', buffer+4,  6) => 6;
     lfs_getattr(&lfs, "hello", 'C', buffer+10, 5) => 5;
@@ -56,15 +59,15 @@
     lfs_setattr(&lfs, "hello", 'B', "fffffffff", 9) => 0;
     lfs_getattr(&lfs, "hello", 'A', buffer,    4) => 4;
     lfs_getattr(&lfs, "hello", 'B', buffer+4,  6) => 9;
     lfs_getattr(&lfs, "hello", 'C', buffer+10, 5) => 5;
 
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     memset(buffer, 0, sizeof(buffer));
     lfs_getattr(&lfs, "hello", 'A', buffer,    4) => 4;
     lfs_getattr(&lfs, "hello", 'B', buffer+4,  9) => 9;
     lfs_getattr(&lfs, "hello", 'C', buffer+13, 5) => 5;
     memcmp(buffer,    "aaaa",      4) => 0;
     memcmp(buffer+4,  "fffffffff", 9) => 0;
     memcmp(buffer+13, "ccccc",     5) => 0;
@@ -72,25 +75,28 @@
     lfs_file_open(&lfs, &file, "hello/hello", LFS_O_RDONLY) => 0;
     lfs_file_read(&lfs, &file, buffer, sizeof(buffer)) => strlen("hello");
     memcmp(buffer, "hello", strlen("hello")) => 0;
     lfs_file_close(&lfs, &file);
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # set/get root attribute
+[cases.test_attrs_get_set_root]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "hello") => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "hello/hello", LFS_O_WRONLY | LFS_O_CREAT) => 0;
     lfs_file_write(&lfs, &file, "hello", strlen("hello")) => strlen("hello");
     lfs_file_close(&lfs, &file);
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    uint8_t buffer[1024];
     memset(buffer, 0, sizeof(buffer));
     lfs_setattr(&lfs, "/", 'A', "aaaa",   4) => 0;
     lfs_setattr(&lfs, "/", 'B', "bbbbbb", 6) => 0;
     lfs_setattr(&lfs, "/", 'C', "ccccc",  5) => 0;
     lfs_getattr(&lfs, "/", 'A', buffer,    4) => 4;
     lfs_getattr(&lfs, "/", 'B', buffer+4,  6) => 6;
     lfs_getattr(&lfs, "/", 'C', buffer+10, 5) => 5;
@@ -133,15 +139,15 @@
     lfs_setattr(&lfs, "/", 'A', buffer, LFS_ATTR_MAX+1) => LFS_ERR_NOSPC;
     lfs_setattr(&lfs, "/", 'B', "fffffffff", 9) => 0;
     lfs_getattr(&lfs, "/", 'A', buffer,    4) => 4;
     lfs_getattr(&lfs, "/", 'B', buffer+4,  6) => 9;
     lfs_getattr(&lfs, "/", 'C', buffer+10, 5) => 5;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     memset(buffer, 0, sizeof(buffer));
     lfs_getattr(&lfs, "/", 'A', buffer,    4) => 4;
     lfs_getattr(&lfs, "/", 'B', buffer+4,  9) => 9;
     lfs_getattr(&lfs, "/", 'C', buffer+13, 5) => 5;
     memcmp(buffer,    "aaaa",      4) => 0;
     memcmp(buffer+4,  "fffffffff", 9) => 0;
     memcmp(buffer+13, "ccccc",     5) => 0;
@@ -149,25 +155,28 @@
     lfs_file_open(&lfs, &file, "hello/hello", LFS_O_RDONLY) => 0;
     lfs_file_read(&lfs, &file, buffer, sizeof(buffer)) => strlen("hello");
     memcmp(buffer, "hello", strlen("hello")) => 0;
     lfs_file_close(&lfs, &file);
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # set/get file attribute
+[cases.test_attrs_get_set_file]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "hello") => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "hello/hello", LFS_O_WRONLY | LFS_O_CREAT) => 0;
     lfs_file_write(&lfs, &file, "hello", strlen("hello")) => strlen("hello");
     lfs_file_close(&lfs, &file);
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    uint8_t buffer[1024];
     memset(buffer, 0, sizeof(buffer));
     struct lfs_attr attrs1[] = {
         {'A', buffer,    4},
         {'B', buffer+4,  6},
         {'C', buffer+10, 5},
     };
     struct lfs_file_config cfg1 = {.attrs=attrs1, .attr_count=3};
@@ -234,15 +243,15 @@
     lfs_file_close(&lfs, &file) => 0;
     attrs1[0].size = 4;
     lfs_file_opencfg(&lfs, &file, "hello/hello", LFS_O_RDONLY, &cfg1) => 0;
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     memset(buffer, 0, sizeof(buffer));
     struct lfs_attr attrs3[] = {
         {'A', buffer,    4},
         {'B', buffer+4,  9},
         {'C', buffer+13, 5},
     };
     struct lfs_file_config cfg3 = {.attrs=attrs3, .attr_count=3};
@@ -256,28 +265,31 @@
     lfs_file_open(&lfs, &file, "hello/hello", LFS_O_RDONLY) => 0;
     lfs_file_read(&lfs, &file, buffer, sizeof(buffer)) => strlen("hello");
     memcmp(buffer, "hello", strlen("hello")) => 0;
     lfs_file_close(&lfs, &file);
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # deferred file attributes
+[cases.test_attrs_deferred_file]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "hello") => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "hello/hello", LFS_O_WRONLY | LFS_O_CREAT) => 0;
     lfs_file_write(&lfs, &file, "hello", strlen("hello")) => strlen("hello");
     lfs_file_close(&lfs, &file);
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_setattr(&lfs, "hello/hello", 'B', "fffffffff",  9) => 0;
     lfs_setattr(&lfs, "hello/hello", 'C', "ccccc",      5) => 0;
 
+    uint8_t buffer[1024];
     memset(buffer, 0, sizeof(buffer));
     struct lfs_attr attrs1[] = {
         {'B', "gggg", 4},
         {'C', "",     0},
         {'D', "hhhh", 4},
     };
     struct lfs_file_config cfg1 = {.attrs=attrs1, .attr_count=3};
```

### Comparing `littlefs-python-0.4.0/littlefs/tests/test_badblocks.toml` & `littlefs-python-0.5.0/littlefs/tests/test_badblocks.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,241 +1,260 @@
 # bad blocks with block cycles should be tested in test_relocations
-if = 'LFS_BLOCK_CYCLES == -1'
+if = '(int32_t)BLOCK_CYCLES == -1'
 
-[[case]] # single bad blocks
-define.LFS_BLOCK_COUNT = 256 # small bd so test runs faster
-define.LFS_ERASE_CYCLES = 0xffffffff
-define.LFS_ERASE_VALUE = [0x00, 0xff, -1]
-define.LFS_BADBLOCK_BEHAVIOR = [
-    'LFS_TESTBD_BADBLOCK_PROGERROR',
-    'LFS_TESTBD_BADBLOCK_ERASEERROR',
-    'LFS_TESTBD_BADBLOCK_READERROR',
-    'LFS_TESTBD_BADBLOCK_PROGNOOP',
-    'LFS_TESTBD_BADBLOCK_ERASENOOP',
+[cases.test_badblocks_single]
+defines.BLOCK_COUNT = 256 # small bd so test runs faster
+defines.ERASE_CYCLES = 0xffffffff
+defines.ERASE_VALUE = [0x00, 0xff, -1]
+defines.BADBLOCK_BEHAVIOR = [
+    'LFS_EMUBD_BADBLOCK_PROGERROR',
+    'LFS_EMUBD_BADBLOCK_ERASEERROR',
+    'LFS_EMUBD_BADBLOCK_READERROR',
+    'LFS_EMUBD_BADBLOCK_PROGNOOP',
+    'LFS_EMUBD_BADBLOCK_ERASENOOP',
 ]
-define.NAMEMULT = 64
-define.FILEMULT = 1
+defines.NAMEMULT = 64
+defines.FILEMULT = 1
 code = '''
-    for (lfs_block_t badblock = 2; badblock < LFS_BLOCK_COUNT; badblock++) {
-        lfs_testbd_setwear(&cfg, badblock-1, 0) => 0;
-        lfs_testbd_setwear(&cfg, badblock, 0xffffffff) => 0;
-        
-        lfs_format(&lfs, &cfg) => 0;
+    for (lfs_block_t badblock = 2; badblock < BLOCK_COUNT; badblock++) {
+        lfs_emubd_setwear(cfg, badblock-1, 0) => 0;
+        lfs_emubd_setwear(cfg, badblock, 0xffffffff) => 0;
+
+        lfs_t lfs;
+        lfs_format(&lfs, cfg) => 0;
 
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         for (int i = 1; i < 10; i++) {
+            uint8_t buffer[1024];
             for (int j = 0; j < NAMEMULT; j++) {
                 buffer[j] = '0'+i;
             }
             buffer[NAMEMULT] = '\0';
             lfs_mkdir(&lfs, (char*)buffer) => 0;
 
             buffer[NAMEMULT] = '/';
             for (int j = 0; j < NAMEMULT; j++) {
                 buffer[j+NAMEMULT+1] = '0'+i;
             }
             buffer[2*NAMEMULT+1] = '\0';
+            lfs_file_t file;
             lfs_file_open(&lfs, &file, (char*)buffer,
                     LFS_O_WRONLY | LFS_O_CREAT) => 0;
             
-            size = NAMEMULT;
+            lfs_size_t size = NAMEMULT;
             for (int j = 0; j < i*FILEMULT; j++) {
                 lfs_file_write(&lfs, &file, buffer, size) => size;
             }
 
             lfs_file_close(&lfs, &file) => 0;
         }
         lfs_unmount(&lfs) => 0;
 
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         for (int i = 1; i < 10; i++) {
+            uint8_t buffer[1024];
             for (int j = 0; j < NAMEMULT; j++) {
                 buffer[j] = '0'+i;
             }
             buffer[NAMEMULT] = '\0';
+            struct lfs_info info;
             lfs_stat(&lfs, (char*)buffer, &info) => 0;
             info.type => LFS_TYPE_DIR;
 
             buffer[NAMEMULT] = '/';
             for (int j = 0; j < NAMEMULT; j++) {
                 buffer[j+NAMEMULT+1] = '0'+i;
             }
             buffer[2*NAMEMULT+1] = '\0';
+            lfs_file_t file;
             lfs_file_open(&lfs, &file, (char*)buffer, LFS_O_RDONLY) => 0;
             
-            size = NAMEMULT;
+            int size = NAMEMULT;
             for (int j = 0; j < i*FILEMULT; j++) {
                 uint8_t rbuffer[1024];
                 lfs_file_read(&lfs, &file, rbuffer, size) => size;
                 memcmp(buffer, rbuffer, size) => 0;
             }
 
             lfs_file_close(&lfs, &file) => 0;
         }
         lfs_unmount(&lfs) => 0;
     }
 '''
 
-[[case]] # region corruption (causes cascading failures)
-define.LFS_BLOCK_COUNT = 256 # small bd so test runs faster
-define.LFS_ERASE_CYCLES = 0xffffffff
-define.LFS_ERASE_VALUE = [0x00, 0xff, -1]
-define.LFS_BADBLOCK_BEHAVIOR = [
-    'LFS_TESTBD_BADBLOCK_PROGERROR',
-    'LFS_TESTBD_BADBLOCK_ERASEERROR',
-    'LFS_TESTBD_BADBLOCK_READERROR',
-    'LFS_TESTBD_BADBLOCK_PROGNOOP',
-    'LFS_TESTBD_BADBLOCK_ERASENOOP',
+[cases.test_badblocks_region_corruption] # (causes cascading failures)
+defines.BLOCK_COUNT = 256 # small bd so test runs faster
+defines.ERASE_CYCLES = 0xffffffff
+defines.ERASE_VALUE = [0x00, 0xff, -1]
+defines.BADBLOCK_BEHAVIOR = [
+    'LFS_EMUBD_BADBLOCK_PROGERROR',
+    'LFS_EMUBD_BADBLOCK_ERASEERROR',
+    'LFS_EMUBD_BADBLOCK_READERROR',
+    'LFS_EMUBD_BADBLOCK_PROGNOOP',
+    'LFS_EMUBD_BADBLOCK_ERASENOOP',
 ]
-define.NAMEMULT = 64
-define.FILEMULT = 1
+defines.NAMEMULT = 64
+defines.FILEMULT = 1
 code = '''
-    for (lfs_block_t i = 0; i < (LFS_BLOCK_COUNT-2)/2; i++) {
-        lfs_testbd_setwear(&cfg, i+2, 0xffffffff) => 0;
+    for (lfs_block_t i = 0; i < (BLOCK_COUNT-2)/2; i++) {
+        lfs_emubd_setwear(cfg, i+2, 0xffffffff) => 0;
     }
-    
-    lfs_format(&lfs, &cfg) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+
+    lfs_mount(&lfs, cfg) => 0;
     for (int i = 1; i < 10; i++) {
+        uint8_t buffer[1024];
         for (int j = 0; j < NAMEMULT; j++) {
             buffer[j] = '0'+i;
         }
         buffer[NAMEMULT] = '\0';
         lfs_mkdir(&lfs, (char*)buffer) => 0;
 
         buffer[NAMEMULT] = '/';
         for (int j = 0; j < NAMEMULT; j++) {
             buffer[j+NAMEMULT+1] = '0'+i;
         }
         buffer[2*NAMEMULT+1] = '\0';
+        lfs_file_t file;
         lfs_file_open(&lfs, &file, (char*)buffer,
                 LFS_O_WRONLY | LFS_O_CREAT) => 0;
         
-        size = NAMEMULT;
+        lfs_size_t size = NAMEMULT;
         for (int j = 0; j < i*FILEMULT; j++) {
             lfs_file_write(&lfs, &file, buffer, size) => size;
         }
 
         lfs_file_close(&lfs, &file) => 0;
     }
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int i = 1; i < 10; i++) {
+        uint8_t buffer[1024];
         for (int j = 0; j < NAMEMULT; j++) {
             buffer[j] = '0'+i;
         }
         buffer[NAMEMULT] = '\0';
+        struct lfs_info info;
         lfs_stat(&lfs, (char*)buffer, &info) => 0;
         info.type => LFS_TYPE_DIR;
 
         buffer[NAMEMULT] = '/';
         for (int j = 0; j < NAMEMULT; j++) {
             buffer[j+NAMEMULT+1] = '0'+i;
         }
         buffer[2*NAMEMULT+1] = '\0';
+        lfs_file_t file;
         lfs_file_open(&lfs, &file, (char*)buffer, LFS_O_RDONLY) => 0;
         
-        size = NAMEMULT;
+        lfs_size_t size = NAMEMULT;
         for (int j = 0; j < i*FILEMULT; j++) {
             uint8_t rbuffer[1024];
             lfs_file_read(&lfs, &file, rbuffer, size) => size;
             memcmp(buffer, rbuffer, size) => 0;
         }
 
         lfs_file_close(&lfs, &file) => 0;
     }
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # alternating corruption (causes cascading failures)
-define.LFS_BLOCK_COUNT = 256 # small bd so test runs faster
-define.LFS_ERASE_CYCLES = 0xffffffff
-define.LFS_ERASE_VALUE = [0x00, 0xff, -1]
-define.LFS_BADBLOCK_BEHAVIOR = [
-    'LFS_TESTBD_BADBLOCK_PROGERROR',
-    'LFS_TESTBD_BADBLOCK_ERASEERROR',
-    'LFS_TESTBD_BADBLOCK_READERROR',
-    'LFS_TESTBD_BADBLOCK_PROGNOOP',
-    'LFS_TESTBD_BADBLOCK_ERASENOOP',
+[cases.test_badblocks_alternating_corruption] # (causes cascading failures)
+defines.BLOCK_COUNT = 256 # small bd so test runs faster
+defines.ERASE_CYCLES = 0xffffffff
+defines.ERASE_VALUE = [0x00, 0xff, -1]
+defines.BADBLOCK_BEHAVIOR = [
+    'LFS_EMUBD_BADBLOCK_PROGERROR',
+    'LFS_EMUBD_BADBLOCK_ERASEERROR',
+    'LFS_EMUBD_BADBLOCK_READERROR',
+    'LFS_EMUBD_BADBLOCK_PROGNOOP',
+    'LFS_EMUBD_BADBLOCK_ERASENOOP',
 ]
-define.NAMEMULT = 64
-define.FILEMULT = 1
+defines.NAMEMULT = 64
+defines.FILEMULT = 1
 code = '''
-    for (lfs_block_t i = 0; i < (LFS_BLOCK_COUNT-2)/2; i++) {
-        lfs_testbd_setwear(&cfg, (2*i) + 2, 0xffffffff) => 0;
+    for (lfs_block_t i = 0; i < (BLOCK_COUNT-2)/2; i++) {
+        lfs_emubd_setwear(cfg, (2*i) + 2, 0xffffffff) => 0;
     }
-    
-    lfs_format(&lfs, &cfg) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+
+    lfs_mount(&lfs, cfg) => 0;
     for (int i = 1; i < 10; i++) {
+        uint8_t buffer[1024];
         for (int j = 0; j < NAMEMULT; j++) {
             buffer[j] = '0'+i;
         }
         buffer[NAMEMULT] = '\0';
         lfs_mkdir(&lfs, (char*)buffer) => 0;
 
         buffer[NAMEMULT] = '/';
         for (int j = 0; j < NAMEMULT; j++) {
             buffer[j+NAMEMULT+1] = '0'+i;
         }
         buffer[2*NAMEMULT+1] = '\0';
+        lfs_file_t file;
         lfs_file_open(&lfs, &file, (char*)buffer,
                 LFS_O_WRONLY | LFS_O_CREAT) => 0;
         
-        size = NAMEMULT;
+        lfs_size_t size = NAMEMULT;
         for (int j = 0; j < i*FILEMULT; j++) {
             lfs_file_write(&lfs, &file, buffer, size) => size;
         }
 
         lfs_file_close(&lfs, &file) => 0;
     }
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int i = 1; i < 10; i++) {
+        uint8_t buffer[1024];
         for (int j = 0; j < NAMEMULT; j++) {
             buffer[j] = '0'+i;
         }
         buffer[NAMEMULT] = '\0';
+        struct lfs_info info;
         lfs_stat(&lfs, (char*)buffer, &info) => 0;
         info.type => LFS_TYPE_DIR;
 
         buffer[NAMEMULT] = '/';
         for (int j = 0; j < NAMEMULT; j++) {
             buffer[j+NAMEMULT+1] = '0'+i;
         }
         buffer[2*NAMEMULT+1] = '\0';
+        lfs_file_t file;
         lfs_file_open(&lfs, &file, (char*)buffer, LFS_O_RDONLY) => 0;
         
-        size = NAMEMULT;
+        lfs_size_t size = NAMEMULT;
         for (int j = 0; j < i*FILEMULT; j++) {
             uint8_t rbuffer[1024];
             lfs_file_read(&lfs, &file, rbuffer, size) => size;
             memcmp(buffer, rbuffer, size) => 0;
         }
 
         lfs_file_close(&lfs, &file) => 0;
     }
     lfs_unmount(&lfs) => 0;
 '''
 
 # other corner cases
-[[case]] # bad superblocks (corrupt 1 or 0)
-define.LFS_ERASE_CYCLES = 0xffffffff
-define.LFS_ERASE_VALUE = [0x00, 0xff, -1]
-define.LFS_BADBLOCK_BEHAVIOR = [
-    'LFS_TESTBD_BADBLOCK_PROGERROR',
-    'LFS_TESTBD_BADBLOCK_ERASEERROR',
-    'LFS_TESTBD_BADBLOCK_READERROR',
-    'LFS_TESTBD_BADBLOCK_PROGNOOP',
-    'LFS_TESTBD_BADBLOCK_ERASENOOP',
+[cases.test_badblocks_superblocks] # (corrupt 1 or 0)
+defines.ERASE_CYCLES = 0xffffffff
+defines.ERASE_VALUE = [0x00, 0xff, -1]
+defines.BADBLOCK_BEHAVIOR = [
+    'LFS_EMUBD_BADBLOCK_PROGERROR',
+    'LFS_EMUBD_BADBLOCK_ERASEERROR',
+    'LFS_EMUBD_BADBLOCK_READERROR',
+    'LFS_EMUBD_BADBLOCK_PROGNOOP',
+    'LFS_EMUBD_BADBLOCK_ERASENOOP',
 ]
 code = '''
-    lfs_testbd_setwear(&cfg, 0, 0xffffffff) => 0;
-    lfs_testbd_setwear(&cfg, 1, 0xffffffff) => 0;
+    lfs_emubd_setwear(cfg, 0, 0xffffffff) => 0;
+    lfs_emubd_setwear(cfg, 1, 0xffffffff) => 0;
 
-    lfs_format(&lfs, &cfg) => LFS_ERR_NOSPC;
-    lfs_mount(&lfs, &cfg) => LFS_ERR_CORRUPT;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => LFS_ERR_NOSPC;
+    lfs_mount(&lfs, cfg) => LFS_ERR_CORRUPT;
 '''
```

### Comparing `littlefs-python-0.4.0/littlefs/tests/test_dirs.toml` & `littlefs-python-0.5.0/littlefs/tests/test_dirs.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,193 +1,223 @@
-[[case]] # root
+[cases.test_dirs_root]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
     lfs_dir_open(&lfs, &dir, "/") => 0;
+    struct lfs_info info;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # many directory creation
-define.N = 'range(0, 100, 3)'
+[cases.test_dirs_many_creation]
+defines.N = 'range(3, 100, 3)'
+if = 'N < BLOCK_COUNT/2'
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "dir%03d", i);
         lfs_mkdir(&lfs, path) => 0;
     }
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
     lfs_dir_open(&lfs, &dir, "/") => 0;
+    struct lfs_info info;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "dir%03d", i);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(info.type == LFS_TYPE_DIR);
         assert(strcmp(info.name, path) == 0);
     }
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # many directory removal
-define.N = 'range(3, 100, 11)'
+[cases.test_dirs_many_removal]
+defines.N = 'range(3, 100, 11)'
+if = 'N < BLOCK_COUNT/2'
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "removeme%03d", i);
         lfs_mkdir(&lfs, path) => 0;
     }
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
     lfs_dir_open(&lfs, &dir, "/") => 0;
+    struct lfs_info info;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "removeme%03d", i);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(info.type == LFS_TYPE_DIR);
         assert(strcmp(info.name, path) == 0);
     }
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs);
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "removeme%03d", i);
         lfs_remove(&lfs, path) => 0;
     }
     lfs_unmount(&lfs);
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_dir_open(&lfs, &dir, "/") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # many directory rename
-define.N = 'range(3, 100, 11)'
+[cases.test_dirs_many_rename]
+defines.N = 'range(3, 100, 11)'
+if = 'N < BLOCK_COUNT/2'
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "test%03d", i);
         lfs_mkdir(&lfs, path) => 0;
     }
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
     lfs_dir_open(&lfs, &dir, "/") => 0;
+    struct lfs_info info;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "test%03d", i);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(info.type == LFS_TYPE_DIR);
         assert(strcmp(info.name, path) == 0);
     }
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs);
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int i = 0; i < N; i++) {
         char oldpath[128];
         char newpath[128];
         sprintf(oldpath, "test%03d", i);
         sprintf(newpath, "tedd%03d", i);
         lfs_rename(&lfs, oldpath, newpath) => 0;
     }
     lfs_unmount(&lfs);
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_dir_open(&lfs, &dir, "/") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "tedd%03d", i);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(info.type == LFS_TYPE_DIR);
         assert(strcmp(info.name, path) == 0);
     }
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs);
 '''
 
-[[case]] # reentrant many directory creation/rename/removal
-define.N = [5, 11]
+[cases.test_dirs_many_reentrant]
+defines.N = [5, 11]
+if = 'BLOCK_COUNT >= 4*N'
 reentrant = true
 code = '''
-    err = lfs_mount(&lfs, &cfg);
+    lfs_t lfs;
+    int err = lfs_mount(&lfs, cfg);
     if (err) {
-        lfs_format(&lfs, &cfg) => 0;
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_format(&lfs, cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
     }
 
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "hi%03d", i);
         err = lfs_mkdir(&lfs, path);
         assert(err == 0 || err == LFS_ERR_EXIST);
     }
 
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "hello%03d", i);
         err = lfs_remove(&lfs, path);
         assert(err == 0 || err == LFS_ERR_NOENT);
     }
 
+    lfs_dir_t dir;
     lfs_dir_open(&lfs, &dir, "/") => 0;
+    struct lfs_info info;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "hi%03d", i);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(info.type == LFS_TYPE_DIR);
         assert(strcmp(info.name, path) == 0);
     }
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
@@ -205,23 +235,25 @@
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "hello%03d", i);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(info.type == LFS_TYPE_DIR);
         assert(strcmp(info.name, path) == 0);
     }
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
 
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "hello%03d", i);
         lfs_remove(&lfs, path) => 0;
     }
 
     lfs_dir_open(&lfs, &dir, "/") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
@@ -230,190 +262,221 @@
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # file creation
-define.N = 'range(3, 100, 11)'
+[cases.test_dirs_file_creation]
+defines.N = 'range(3, 100, 11)'
+if = 'N < BLOCK_COUNT/2'
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "file%03d", i);
+        lfs_file_t file;
         lfs_file_open(&lfs, &file, path,
                 LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => 0;
         lfs_file_close(&lfs, &file) => 0;
     }
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
     lfs_dir_open(&lfs, &dir, "/") => 0;
+    struct lfs_info info;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "file%03d", i);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(info.type == LFS_TYPE_REG);
         assert(strcmp(info.name, path) == 0);
     }
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs);
 '''
 
-[[case]] # file removal
-define.N = 'range(0, 100, 3)'
+[cases.test_dirs_file_removal]
+defines.N = 'range(3, 100, 11)'
+if = 'N < BLOCK_COUNT/2'
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "removeme%03d", i);
+        lfs_file_t file;
         lfs_file_open(&lfs, &file, path,
                 LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => 0;
         lfs_file_close(&lfs, &file) => 0;
     }
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
     lfs_dir_open(&lfs, &dir, "/") => 0;
+    struct lfs_info info;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "removeme%03d", i);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(info.type == LFS_TYPE_REG);
         assert(strcmp(info.name, path) == 0);
     }
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs);
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "removeme%03d", i);
         lfs_remove(&lfs, path) => 0;
     }
     lfs_unmount(&lfs);
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_dir_open(&lfs, &dir, "/") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # file rename
-define.N = 'range(0, 100, 3)'
+[cases.test_dirs_file_rename]
+defines.N = 'range(3, 100, 11)'
+if = 'N < BLOCK_COUNT/2'
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "test%03d", i);
+        lfs_file_t file;
         lfs_file_open(&lfs, &file, path,
                 LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => 0;
         lfs_file_close(&lfs, &file) => 0;
     }
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
     lfs_dir_open(&lfs, &dir, "/") => 0;
+    struct lfs_info info;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "test%03d", i);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(info.type == LFS_TYPE_REG);
         assert(strcmp(info.name, path) == 0);
     }
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs);
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int i = 0; i < N; i++) {
         char oldpath[128];
         char newpath[128];
         sprintf(oldpath, "test%03d", i);
         sprintf(newpath, "tedd%03d", i);
         lfs_rename(&lfs, oldpath, newpath) => 0;
     }
     lfs_unmount(&lfs);
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_dir_open(&lfs, &dir, "/") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "tedd%03d", i);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(info.type == LFS_TYPE_REG);
         assert(strcmp(info.name, path) == 0);
     }
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs);
 '''
 
-[[case]] # reentrant file creation/rename/removal
-define.N = [5, 25]
+[cases.test_dirs_file_reentrant]
+defines.N = [5, 25]
+if = 'N < BLOCK_COUNT/2'
 reentrant = true
 code = '''
-    err = lfs_mount(&lfs, &cfg);
+    lfs_t lfs;
+    int err = lfs_mount(&lfs, cfg);
     if (err) {
-        lfs_format(&lfs, &cfg) => 0;
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_format(&lfs, cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
     }
 
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "hi%03d", i);
+        lfs_file_t file;
         lfs_file_open(&lfs, &file, path, LFS_O_CREAT | LFS_O_WRONLY) => 0;
         lfs_file_close(&lfs, &file) => 0;
     }
 
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "hello%03d", i);
         err = lfs_remove(&lfs, path);
         assert(err == 0 || err == LFS_ERR_NOENT);
     }
 
+    lfs_dir_t dir;
     lfs_dir_open(&lfs, &dir, "/") => 0;
+    struct lfs_info info;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "hi%03d", i);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(info.type == LFS_TYPE_REG);
         assert(strcmp(info.name, path) == 0);
     }
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
@@ -431,23 +494,25 @@
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "hello%03d", i);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(info.type == LFS_TYPE_REG);
         assert(strcmp(info.name, path) == 0);
     }
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
 
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "hello%03d", i);
         lfs_remove(&lfs, path) => 0;
     }
 
     lfs_dir_open(&lfs, &dir, "/") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
@@ -456,32 +521,36 @@
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # nested directories
+[cases.test_dirs_nested]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "potato") => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "burito",
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "potato/baked") => 0;
     lfs_mkdir(&lfs, "potato/sweet") => 0;
     lfs_mkdir(&lfs, "potato/fried") => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
     lfs_dir_open(&lfs, &dir, "potato") => 0;
+    struct lfs_info info;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, ".") == 0);
     info.type => LFS_TYPE_DIR;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "..") == 0);
     info.type => LFS_TYPE_DIR;
     lfs_dir_read(&lfs, &dir, &info) => 1;
@@ -494,37 +563,37 @@
     assert(strcmp(info.name, "sweet") == 0);
     info.type => LFS_TYPE_DIR;
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
 
     // try removing?
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_remove(&lfs, "potato") => LFS_ERR_NOTEMPTY;
     lfs_unmount(&lfs) => 0;
 
     // try renaming?
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_rename(&lfs, "potato", "coldpotato") => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_rename(&lfs, "coldpotato", "warmpotato") => 0;
     lfs_rename(&lfs, "warmpotato", "hotpotato") => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_remove(&lfs, "potato") => LFS_ERR_NOENT;
     lfs_remove(&lfs, "coldpotato") => LFS_ERR_NOENT;
     lfs_remove(&lfs, "warmpotato") => LFS_ERR_NOENT;
     lfs_remove(&lfs, "hotpotato") => LFS_ERR_NOTEMPTY;
     lfs_unmount(&lfs) => 0;
 
     // try cross-directory renaming
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "coldpotato") => 0;
     lfs_rename(&lfs, "hotpotato/baked", "coldpotato/baked") => 0;
     lfs_rename(&lfs, "coldpotato", "hotpotato") => LFS_ERR_NOTEMPTY;
     lfs_remove(&lfs, "coldpotato") => LFS_ERR_NOTEMPTY;
     lfs_remove(&lfs, "hotpotato") => LFS_ERR_NOTEMPTY;
     lfs_rename(&lfs, "hotpotato/fried", "coldpotato/fried") => 0;
     lfs_rename(&lfs, "coldpotato", "hotpotato") => LFS_ERR_NOTEMPTY;
@@ -532,15 +601,15 @@
     lfs_remove(&lfs, "hotpotato") => LFS_ERR_NOTEMPTY;
     lfs_rename(&lfs, "hotpotato/sweet", "coldpotato/sweet") => 0;
     lfs_rename(&lfs, "coldpotato", "hotpotato") => 0;
     lfs_remove(&lfs, "coldpotato") => LFS_ERR_NOENT;
     lfs_remove(&lfs, "hotpotato") => LFS_ERR_NOTEMPTY;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_dir_open(&lfs, &dir, "hotpotato") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, ".") == 0);
     info.type => LFS_TYPE_DIR;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "..") == 0);
     info.type => LFS_TYPE_DIR;
@@ -554,25 +623,25 @@
     assert(strcmp(info.name, "sweet") == 0);
     info.type => LFS_TYPE_DIR;
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
     
     // final remove
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_remove(&lfs, "hotpotato") => LFS_ERR_NOTEMPTY;
     lfs_remove(&lfs, "hotpotato/baked") => 0;
     lfs_remove(&lfs, "hotpotato") => LFS_ERR_NOTEMPTY;
     lfs_remove(&lfs, "hotpotato/fried") => 0;
     lfs_remove(&lfs, "hotpotato") => LFS_ERR_NOTEMPTY;
     lfs_remove(&lfs, "hotpotato/sweet") => 0;
     lfs_remove(&lfs, "hotpotato") => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_dir_open(&lfs, &dir, "/") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, ".") == 0);
     info.type => LFS_TYPE_DIR;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "..") == 0);
     info.type => LFS_TYPE_DIR;
@@ -580,89 +649,99 @@
     assert(strcmp(info.name, "burito") == 0);
     info.type => LFS_TYPE_REG;
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # recursive remove
-define.N = [10, 100]
-code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+[cases.test_dirs_recursive_remove]
+defines.N = [10, 100]
+if = 'N < BLOCK_COUNT/2'
+code = '''
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "prickly-pear") => 0;
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "prickly-pear/cactus%03d", i);
         lfs_mkdir(&lfs, path) => 0;
     }
+    lfs_dir_t dir;
     lfs_dir_open(&lfs, &dir, "prickly-pear") => 0;
+    struct lfs_info info;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "cactus%03d", i);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(info.type == LFS_TYPE_DIR);
         assert(strcmp(info.name, path) == 0);
     }
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs);
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_remove(&lfs, "prickly-pear") => LFS_ERR_NOTEMPTY;
 
     lfs_dir_open(&lfs, &dir, "prickly-pear") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     for (int i = 0; i < N; i++) {
+        char path[1024];
         sprintf(path, "cactus%03d", i);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(info.type == LFS_TYPE_DIR);
         assert(strcmp(info.name, path) == 0);
         sprintf(path, "prickly-pear/%s", info.name);
         lfs_remove(&lfs, path) => 0;
     }
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
 
     lfs_remove(&lfs, "prickly-pear") => 0;
     lfs_remove(&lfs, "prickly-pear") => LFS_ERR_NOENT;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_remove(&lfs, "prickly-pear") => LFS_ERR_NOENT;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # other error cases
+[cases.test_dirs_other_errors]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "potato") => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "burito",
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     lfs_mkdir(&lfs, "potato") => LFS_ERR_EXIST;
     lfs_mkdir(&lfs, "burito") => LFS_ERR_EXIST;
     lfs_file_open(&lfs, &file, "burito",
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => LFS_ERR_EXIST;
     lfs_file_open(&lfs, &file, "potato",
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => LFS_ERR_EXIST;
+    lfs_dir_t dir;
     lfs_dir_open(&lfs, &dir, "tomato") => LFS_ERR_NOENT;
     lfs_dir_open(&lfs, &dir, "burito") => LFS_ERR_NOTDIR;
     lfs_file_open(&lfs, &file, "tomato", LFS_O_RDONLY) => LFS_ERR_NOENT;
     lfs_file_open(&lfs, &file, "potato", LFS_O_RDONLY) => LFS_ERR_ISDIR;
     lfs_file_open(&lfs, &file, "tomato", LFS_O_WRONLY) => LFS_ERR_NOENT;
     lfs_file_open(&lfs, &file, "potato", LFS_O_WRONLY) => LFS_ERR_ISDIR;
     lfs_file_open(&lfs, &file, "potato",
@@ -674,14 +753,15 @@
     lfs_file_open(&lfs, &file, "/", LFS_O_RDONLY) => LFS_ERR_ISDIR;
     lfs_file_open(&lfs, &file, "/", LFS_O_WRONLY) => LFS_ERR_ISDIR;
     lfs_file_open(&lfs, &file, "/",
             LFS_O_WRONLY | LFS_O_CREAT) => LFS_ERR_ISDIR;
 
     // check that errors did not corrupt directory
     lfs_dir_open(&lfs, &dir, "/") => 0;
+    struct lfs_info info;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
@@ -692,15 +772,15 @@
     assert(strcmp(info.name, "potato") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
 
     lfs_unmount(&lfs) => 0;
 
     // or on disk
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_dir_open(&lfs, &dir, "/") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "..") == 0);
@@ -711,54 +791,61 @@
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, "potato") == 0);
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # directory seek
-define.COUNT = [4, 128, 132]
-code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+[cases.test_dirs_seek]
+defines.COUNT = [4, 128, 132]
+if = 'COUNT < BLOCK_COUNT/2'
+code = '''
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "hello") => 0;
     for (int i = 0; i < COUNT; i++) {
+        char path[1024];
         sprintf(path, "hello/kitty%03d", i);
         lfs_mkdir(&lfs, path) => 0;
     }
     lfs_unmount(&lfs) => 0;
 
-    for (int j = 2; j < COUNT; j++) {
-        lfs_mount(&lfs, &cfg) => 0;
+    // try seeking to each dir entry
+    for (int j = 0; j < COUNT; j++) {
+        lfs_mount(&lfs, cfg) => 0;
+        lfs_dir_t dir;
         lfs_dir_open(&lfs, &dir, "hello") => 0;
+        struct lfs_info info;
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(strcmp(info.name, ".") == 0);
         assert(info.type == LFS_TYPE_DIR);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(strcmp(info.name, "..") == 0);
         assert(info.type == LFS_TYPE_DIR);
 
-        lfs_soff_t pos;
         for (int i = 0; i < j; i++) {
+            char path[1024];
             sprintf(path, "kitty%03d", i);
             lfs_dir_read(&lfs, &dir, &info) => 1;
             assert(strcmp(info.name, path) == 0);
             assert(info.type == LFS_TYPE_DIR);
-            pos = lfs_dir_tell(&lfs, &dir);
-            assert(pos >= 0);
         }
+        lfs_soff_t pos = lfs_dir_tell(&lfs, &dir);
+        assert(pos >= 0);
 
         lfs_dir_seek(&lfs, &dir, pos) => 0;
+        char path[1024];
         sprintf(path, "kitty%03d", j);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(strcmp(info.name, path) == 0);
         assert(info.type == LFS_TYPE_DIR);
 
         lfs_dir_rewind(&lfs, &dir) => 0;
-        sprintf(path, "kitty%03d", 0);
+        sprintf(path, "kitty%03u", 0);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(strcmp(info.name, ".") == 0);
         assert(info.type == LFS_TYPE_DIR);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(strcmp(info.name, "..") == 0);
         assert(info.type == LFS_TYPE_DIR);
         lfs_dir_read(&lfs, &dir, &info) => 1;
@@ -770,55 +857,107 @@
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(strcmp(info.name, path) == 0);
         assert(info.type == LFS_TYPE_DIR);
 
         lfs_dir_close(&lfs, &dir) => 0;
         lfs_unmount(&lfs) => 0;
     }
+
+    // try seeking to end of dir
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
+    lfs_dir_open(&lfs, &dir, "hello") => 0;
+    struct lfs_info info;
+    lfs_dir_read(&lfs, &dir, &info) => 1;
+    assert(strcmp(info.name, ".") == 0);
+    assert(info.type == LFS_TYPE_DIR);
+    lfs_dir_read(&lfs, &dir, &info) => 1;
+    assert(strcmp(info.name, "..") == 0);
+    assert(info.type == LFS_TYPE_DIR);
+
+    for (int i = 0; i < COUNT; i++) {
+        char path[1024];
+        sprintf(path, "kitty%03d", i);
+        lfs_dir_read(&lfs, &dir, &info) => 1;
+        assert(strcmp(info.name, path) == 0);
+        assert(info.type == LFS_TYPE_DIR);
+    }
+    lfs_soff_t pos = lfs_dir_tell(&lfs, &dir);
+    assert(pos >= 0);
+
+    lfs_dir_read(&lfs, &dir, &info) => 0;
+
+    lfs_dir_seek(&lfs, &dir, pos) => 0;
+    lfs_dir_read(&lfs, &dir, &info) => 0;
+
+    lfs_dir_rewind(&lfs, &dir) => 0;
+    char path[1024];
+    sprintf(path, "kitty%03d", 0);
+    lfs_dir_read(&lfs, &dir, &info) => 1;
+    assert(strcmp(info.name, ".") == 0);
+    assert(info.type == LFS_TYPE_DIR);
+    lfs_dir_read(&lfs, &dir, &info) => 1;
+    assert(strcmp(info.name, "..") == 0);
+    assert(info.type == LFS_TYPE_DIR);
+    lfs_dir_read(&lfs, &dir, &info) => 1;
+    assert(strcmp(info.name, path) == 0);
+    assert(info.type == LFS_TYPE_DIR);
+
+    lfs_dir_seek(&lfs, &dir, pos) => 0;
+    lfs_dir_read(&lfs, &dir, &info) => 0;
+
+    lfs_dir_close(&lfs, &dir) => 0;
+    lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # root seek
-define.COUNT = [4, 128, 132]
+[cases.test_dirs_toot_seek]
+defines.COUNT = [4, 128, 132]
+if = 'COUNT < BLOCK_COUNT/2'
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int i = 0; i < COUNT; i++) {
+        char path[1024];
         sprintf(path, "hi%03d", i);
         lfs_mkdir(&lfs, path) => 0;
     }
     lfs_unmount(&lfs) => 0;
 
-    for (int j = 2; j < COUNT; j++) {
-        lfs_mount(&lfs, &cfg) => 0;
+    for (int j = 0; j < COUNT; j++) {
+        lfs_mount(&lfs, cfg) => 0;
+        lfs_dir_t dir;
         lfs_dir_open(&lfs, &dir, "/") => 0;
+        struct lfs_info info;
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(strcmp(info.name, ".") == 0);
         assert(info.type == LFS_TYPE_DIR);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(strcmp(info.name, "..") == 0);
         assert(info.type == LFS_TYPE_DIR);
 
-        lfs_soff_t pos;
         for (int i = 0; i < j; i++) {
+            char path[1024];
             sprintf(path, "hi%03d", i);
             lfs_dir_read(&lfs, &dir, &info) => 1;
             assert(strcmp(info.name, path) == 0);
             assert(info.type == LFS_TYPE_DIR);
-            pos = lfs_dir_tell(&lfs, &dir);
-            assert(pos >= 0);
         }
+        lfs_soff_t pos = lfs_dir_tell(&lfs, &dir);
+        assert(pos >= 0);
 
         lfs_dir_seek(&lfs, &dir, pos) => 0;
+        char path[1024];
         sprintf(path, "hi%03d", j);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(strcmp(info.name, path) == 0);
         assert(info.type == LFS_TYPE_DIR);
 
         lfs_dir_rewind(&lfs, &dir) => 0;
-        sprintf(path, "hi%03d", 0);
+        sprintf(path, "hi%03u", 0);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(strcmp(info.name, ".") == 0);
         assert(info.type == LFS_TYPE_DIR);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(strcmp(info.name, "..") == 0);
         assert(info.type == LFS_TYPE_DIR);
         lfs_dir_read(&lfs, &dir, &info) => 1;
@@ -830,9 +969,55 @@
         lfs_dir_read(&lfs, &dir, &info) => 1;
         assert(strcmp(info.name, path) == 0);
         assert(info.type == LFS_TYPE_DIR);
 
         lfs_dir_close(&lfs, &dir) => 0;
         lfs_unmount(&lfs) => 0;
     }
+
+    // try seeking to end of dir
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
+    lfs_dir_open(&lfs, &dir, "/") => 0;
+    struct lfs_info info;
+    lfs_dir_read(&lfs, &dir, &info) => 1;
+    assert(strcmp(info.name, ".") == 0);
+    assert(info.type == LFS_TYPE_DIR);
+    lfs_dir_read(&lfs, &dir, &info) => 1;
+    assert(strcmp(info.name, "..") == 0);
+    assert(info.type == LFS_TYPE_DIR);
+
+    for (int i = 0; i < COUNT; i++) {
+        char path[1024];
+        sprintf(path, "hi%03d", i);
+        lfs_dir_read(&lfs, &dir, &info) => 1;
+        assert(strcmp(info.name, path) == 0);
+        assert(info.type == LFS_TYPE_DIR);
+    }
+    lfs_soff_t pos = lfs_dir_tell(&lfs, &dir);
+    assert(pos >= 0);
+
+    lfs_dir_read(&lfs, &dir, &info) => 0;
+
+    lfs_dir_seek(&lfs, &dir, pos) => 0;
+    lfs_dir_read(&lfs, &dir, &info) => 0;
+
+    lfs_dir_rewind(&lfs, &dir) => 0;
+    char path[1024];
+    sprintf(path, "hi%03d", 0);
+    lfs_dir_read(&lfs, &dir, &info) => 1;
+    assert(strcmp(info.name, ".") == 0);
+    assert(info.type == LFS_TYPE_DIR);
+    lfs_dir_read(&lfs, &dir, &info) => 1;
+    assert(strcmp(info.name, "..") == 0);
+    assert(info.type == LFS_TYPE_DIR);
+    lfs_dir_read(&lfs, &dir, &info) => 1;
+    assert(strcmp(info.name, path) == 0);
+    assert(info.type == LFS_TYPE_DIR);
+
+    lfs_dir_seek(&lfs, &dir, pos) => 0;
+    lfs_dir_read(&lfs, &dir, &info) => 0;
+
+    lfs_dir_close(&lfs, &dir) => 0;
+    lfs_unmount(&lfs) => 0;
 '''
```

### Comparing `littlefs-python-0.4.0/littlefs/tests/test_entries.toml` & `littlefs-python-0.5.0/littlefs/tests/test_entries.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # These tests are for some specific corner cases with neighboring inline files.
 # Note that these tests are intended for 512 byte inline sizes. They should
 # still pass with other inline sizes but wouldn't be testing anything.
 
-define.LFS_CACHE_SIZE = 512
-if = 'LFS_CACHE_SIZE % LFS_PROG_SIZE == 0 && LFS_CACHE_SIZE == 512'
+defines.CACHE_SIZE = 512
+if = 'CACHE_SIZE % PROG_SIZE == 0 && CACHE_SIZE == 512'
 
-[[case]] # entry grow test
+[cases.test_entries_grow]
 code = '''
     uint8_t wbuffer[1024];
     uint8_t rbuffer[1024];
 
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     // write hi0 20
+    char path[1024];
+    lfs_size_t size;
     sprintf(path, "hi0"); size = 20;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, path,
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_TRUNC) => 0;
     memset(wbuffer, 'c', size);
     lfs_file_write(&lfs, &file, wbuffer, size) => size;
     lfs_file_size(&lfs, &file) => size;
     lfs_file_close(&lfs, &file) => 0;
     // write hi1 20
@@ -90,24 +94,28 @@
     lfs_file_read(&lfs, &file, rbuffer, size) => size;
     memcmp(rbuffer, wbuffer, size) => 0;
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # entry shrink test
+[cases.test_entries_shrink]
 code = '''
     uint8_t wbuffer[1024];
     uint8_t rbuffer[1024];
 
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     // write hi0 20
+    char path[1024];
+    lfs_size_t size;
     sprintf(path, "hi0"); size = 20;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, path,
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_TRUNC) => 0;
     memset(wbuffer, 'c', size);
     lfs_file_write(&lfs, &file, wbuffer, size) => size;
     lfs_file_size(&lfs, &file) => size;
     lfs_file_close(&lfs, &file) => 0;
     // write hi1 200
@@ -179,24 +187,28 @@
     lfs_file_read(&lfs, &file, rbuffer, size) => size;
     memcmp(rbuffer, wbuffer, size) => 0;
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # entry spill test
+[cases.test_entries_spill]
 code = '''
     uint8_t wbuffer[1024];
     uint8_t rbuffer[1024];
 
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     // write hi0 200
+    char path[1024];
+    lfs_size_t size;
     sprintf(path, "hi0"); size = 200;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, path,
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_TRUNC) => 0;
     memset(wbuffer, 'c', size);
     lfs_file_write(&lfs, &file, wbuffer, size) => size;
     lfs_file_size(&lfs, &file) => size;
     lfs_file_close(&lfs, &file) => 0;
     // write hi1 200
@@ -252,24 +264,28 @@
     lfs_file_read(&lfs, &file, rbuffer, size) => size;
     memcmp(rbuffer, wbuffer, size) => 0;
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # entry push spill test
+[cases.test_entries_push_spill]
 code = '''
     uint8_t wbuffer[1024];
     uint8_t rbuffer[1024];
 
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     // write hi0 200
+    char path[1024];
+    lfs_size_t size;
     sprintf(path, "hi0"); size = 200;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, path,
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_TRUNC) => 0;
     memset(wbuffer, 'c', size);
     lfs_file_write(&lfs, &file, wbuffer, size) => size;
     lfs_file_size(&lfs, &file) => size;
     lfs_file_close(&lfs, &file) => 0;
     // write hi1 20
@@ -341,24 +357,28 @@
     lfs_file_read(&lfs, &file, rbuffer, size) => size;
     memcmp(rbuffer, wbuffer, size) => 0;
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # entry push spill two test
+[cases.test_entries_push_spill_two]
 code = '''
     uint8_t wbuffer[1024];
     uint8_t rbuffer[1024];
 
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     // write hi0 200
+    char path[1024];
+    lfs_size_t size;
     sprintf(path, "hi0"); size = 200;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, path,
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_TRUNC) => 0;
     memset(wbuffer, 'c', size);
     lfs_file_write(&lfs, &file, wbuffer, size) => size;
     lfs_file_size(&lfs, &file) => size;
     lfs_file_close(&lfs, &file) => 0;
     // write hi1 20
@@ -445,24 +465,28 @@
     lfs_file_read(&lfs, &file, rbuffer, size) => size;
     memcmp(rbuffer, wbuffer, size) => 0;
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # entry drop test
+[cases.test_entries_drop]
 code = '''
     uint8_t wbuffer[1024];
     uint8_t rbuffer[1024];
 
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     // write hi0 200
+    char path[1024];
+    lfs_size_t size;
     sprintf(path, "hi0"); size = 200;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, path,
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_TRUNC) => 0;
     memset(wbuffer, 'c', size);
     lfs_file_write(&lfs, &file, wbuffer, size) => size;
     lfs_file_size(&lfs, &file) => size;
     lfs_file_close(&lfs, &file) => 0;
     // write hi1 200
@@ -487,14 +511,15 @@
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_TRUNC) => 0;
     memset(wbuffer, 'c', size);
     lfs_file_write(&lfs, &file, wbuffer, size) => size;
     lfs_file_size(&lfs, &file) => size;
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_remove(&lfs, "hi1") => 0;
+    struct lfs_info info;
     lfs_stat(&lfs, "hi1", &info) => LFS_ERR_NOENT;
     // read hi0 200
     sprintf(path, "hi0"); size = 200;
     lfs_file_open(&lfs, &file, path, LFS_O_RDONLY) => 0;
     lfs_file_size(&lfs, &file) => size;
     lfs_file_read(&lfs, &file, rbuffer, size) => size;
     memcmp(rbuffer, wbuffer, size) => 0;
@@ -543,23 +568,26 @@
 
     lfs_remove(&lfs, "hi0") => 0;
     lfs_stat(&lfs, "hi0", &info) => LFS_ERR_NOENT;
 
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # create too big
+[cases.test_entries_create_too_big]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    char path[1024];
     memset(path, 'm', 200);
     path[200] = '\0';
 
-    size = 400;
+    lfs_size_t size = 400;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, path,
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_TRUNC) => 0;
     uint8_t wbuffer[1024];
     memset(wbuffer, 'c', size);
     lfs_file_write(&lfs, &file, wbuffer, size) => size;
     lfs_file_close(&lfs, &file) => 0;
 
@@ -568,23 +596,26 @@
     uint8_t rbuffer[1024];
     lfs_file_read(&lfs, &file, rbuffer, size) => size;
     memcmp(rbuffer, wbuffer, size) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # resize too big
+[cases.test_entries_resize_too_big]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    char path[1024];
     memset(path, 'm', 200);
     path[200] = '\0';
 
-    size = 40;
+    lfs_size_t size = 40;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, path,
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_TRUNC) => 0;
     uint8_t wbuffer[1024];
     memset(wbuffer, 'c', size);
     lfs_file_write(&lfs, &file, wbuffer, size) => size;
     lfs_file_close(&lfs, &file) => 0;
```

### Comparing `littlefs-python-0.4.0/littlefs/tests/test_evil.toml` & `littlefs-python-0.5.0/littlefs/tests/test_evil.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 # Tests for recovering from conditions which shouldn't normally
 # happen during normal operation of littlefs
 
 # invalid pointer tests (outside of block_count)
 
-[[case]] # invalid tail-pointer test
-define.TAIL_TYPE = ['LFS_TYPE_HARDTAIL', 'LFS_TYPE_SOFTTAIL']
-define.INVALSET = [0x3, 0x1, 0x2]
+[cases.test_evil_invalid_tail_pointer]
+defines.TAIL_TYPE = ['LFS_TYPE_HARDTAIL', 'LFS_TYPE_SOFTTAIL']
+defines.INVALSET = [0x3, 0x1, 0x2]
 in = "lfs.c"
 code = '''
     // create littlefs
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
     // change tail-pointer to invalid pointers
-    lfs_init(&lfs, &cfg) => 0;
+    lfs_init(&lfs, cfg) => 0;
     lfs_mdir_t mdir;
     lfs_dir_fetch(&lfs, &mdir, (lfs_block_t[2]){0, 1}) => 0;
     lfs_dir_commit(&lfs, &mdir, LFS_MKATTRS(
             {LFS_MKTAG(LFS_TYPE_HARDTAIL, 0x3ff, 8),
                 (lfs_block_t[2]){
                     (INVALSET & 0x1) ? 0xcccccccc : 0,
                     (INVALSET & 0x2) ? 0xcccccccc : 0}})) => 0;
     lfs_deinit(&lfs) => 0;
 
     // test that mount fails gracefully
-    lfs_mount(&lfs, &cfg) => LFS_ERR_CORRUPT;
+    lfs_mount(&lfs, cfg) => LFS_ERR_CORRUPT;
 '''
 
-[[case]] # invalid dir pointer test
-define.INVALSET = [0x3, 0x1, 0x2]
+[cases.test_evil_invalid_dir_pointer]
+defines.INVALSET = [0x3, 0x1, 0x2]
 in = "lfs.c"
 code = '''
     // create littlefs
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
     // make a dir
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "dir_here") => 0;
     lfs_unmount(&lfs) => 0;
 
     // change the dir pointer to be invalid
-    lfs_init(&lfs, &cfg) => 0;
+    lfs_init(&lfs, cfg) => 0;
     lfs_mdir_t mdir;
     lfs_dir_fetch(&lfs, &mdir, (lfs_block_t[2]){0, 1}) => 0;
     // make sure id 1 == our directory
+    uint8_t buffer[1024];
     lfs_dir_get(&lfs, &mdir,
             LFS_MKTAG(0x700, 0x3ff, 0),
             LFS_MKTAG(LFS_TYPE_NAME, 1, strlen("dir_here")), buffer)
                 => LFS_MKTAG(LFS_TYPE_DIR, 1, strlen("dir_here"));
     assert(memcmp((char*)buffer, "dir_here", strlen("dir_here")) == 0);
     // change dir pointer
     lfs_dir_commit(&lfs, &mdir, LFS_MKATTRS(
@@ -53,196 +56,210 @@
                 (lfs_block_t[2]){
                     (INVALSET & 0x1) ? 0xcccccccc : 0,
                     (INVALSET & 0x2) ? 0xcccccccc : 0}})) => 0;
     lfs_deinit(&lfs) => 0;
 
     // test that accessing our bad dir fails, note there's a number
     // of ways to access the dir, some can fail, but some don't
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    struct lfs_info info;
     lfs_stat(&lfs, "dir_here", &info) => 0;
     assert(strcmp(info.name, "dir_here") == 0);
     assert(info.type == LFS_TYPE_DIR);
 
+    lfs_dir_t dir;
     lfs_dir_open(&lfs, &dir, "dir_here") => LFS_ERR_CORRUPT;
     lfs_stat(&lfs, "dir_here/file_here", &info) => LFS_ERR_CORRUPT;
     lfs_dir_open(&lfs, &dir, "dir_here/dir_here") => LFS_ERR_CORRUPT;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "dir_here/file_here",
             LFS_O_RDONLY) => LFS_ERR_CORRUPT;
     lfs_file_open(&lfs, &file, "dir_here/file_here",
             LFS_O_WRONLY | LFS_O_CREAT) => LFS_ERR_CORRUPT;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # invalid file pointer test
+[cases.test_evil_invalid_file_pointer]
 in = "lfs.c"
-define.SIZE = [10, 1000, 100000] # faked file size
+defines.SIZE = [10, 1000, 100000] # faked file size
 code = '''
     // create littlefs
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
     // make a file
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "file_here",
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
     // change the file pointer to be invalid
-    lfs_init(&lfs, &cfg) => 0;
+    lfs_init(&lfs, cfg) => 0;
     lfs_mdir_t mdir;
     lfs_dir_fetch(&lfs, &mdir, (lfs_block_t[2]){0, 1}) => 0;
     // make sure id 1 == our file
+    uint8_t buffer[1024];
     lfs_dir_get(&lfs, &mdir,
             LFS_MKTAG(0x700, 0x3ff, 0),
             LFS_MKTAG(LFS_TYPE_NAME, 1, strlen("file_here")), buffer)
                 => LFS_MKTAG(LFS_TYPE_REG, 1, strlen("file_here"));
     assert(memcmp((char*)buffer, "file_here", strlen("file_here")) == 0);
     // change file pointer
     lfs_dir_commit(&lfs, &mdir, LFS_MKATTRS(
             {LFS_MKTAG(LFS_TYPE_CTZSTRUCT, 1, sizeof(struct lfs_ctz)),
                 &(struct lfs_ctz){0xcccccccc, lfs_tole32(SIZE)}})) => 0;
     lfs_deinit(&lfs) => 0;
 
     // test that accessing our bad file fails, note there's a number
     // of ways to access the dir, some can fail, but some don't
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    struct lfs_info info;
     lfs_stat(&lfs, "file_here", &info) => 0;
     assert(strcmp(info.name, "file_here") == 0);
     assert(info.type == LFS_TYPE_REG);
     assert(info.size == SIZE);
 
     lfs_file_open(&lfs, &file, "file_here", LFS_O_RDONLY) => 0;
     lfs_file_read(&lfs, &file, buffer, SIZE) => LFS_ERR_CORRUPT;
     lfs_file_close(&lfs, &file) => 0;
 
     // any allocs that traverse CTZ must unfortunately must fail
-    if (SIZE > 2*LFS_BLOCK_SIZE) {
+    if (SIZE > 2*BLOCK_SIZE) {
         lfs_mkdir(&lfs, "dir_here") => LFS_ERR_CORRUPT;
     }
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # invalid pointer in CTZ skip-list test
-define.SIZE = ['2*LFS_BLOCK_SIZE', '3*LFS_BLOCK_SIZE', '4*LFS_BLOCK_SIZE']
+[cases.test_evil_invalid_ctz_pointer] # invalid pointer in CTZ skip-list test
+defines.SIZE = ['2*BLOCK_SIZE', '3*BLOCK_SIZE', '4*BLOCK_SIZE']
 in = "lfs.c"
 code = '''
     // create littlefs
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
     // make a file
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "file_here",
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
     for (int i = 0; i < SIZE; i++) {
         char c = 'c';
         lfs_file_write(&lfs, &file, &c, 1) => 1;
     }
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
     // change pointer in CTZ skip-list to be invalid
-    lfs_init(&lfs, &cfg) => 0;
+    lfs_init(&lfs, cfg) => 0;
     lfs_mdir_t mdir;
     lfs_dir_fetch(&lfs, &mdir, (lfs_block_t[2]){0, 1}) => 0;
     // make sure id 1 == our file and get our CTZ structure
+    uint8_t buffer[4*BLOCK_SIZE];
     lfs_dir_get(&lfs, &mdir,
             LFS_MKTAG(0x700, 0x3ff, 0),
             LFS_MKTAG(LFS_TYPE_NAME, 1, strlen("file_here")), buffer)
                 => LFS_MKTAG(LFS_TYPE_REG, 1, strlen("file_here"));
     assert(memcmp((char*)buffer, "file_here", strlen("file_here")) == 0);
     struct lfs_ctz ctz;
     lfs_dir_get(&lfs, &mdir,
             LFS_MKTAG(0x700, 0x3ff, 0),
             LFS_MKTAG(LFS_TYPE_STRUCT, 1, sizeof(struct lfs_ctz)), &ctz)
                 => LFS_MKTAG(LFS_TYPE_CTZSTRUCT, 1, sizeof(struct lfs_ctz));
     lfs_ctz_fromle32(&ctz);
     // rewrite block to contain bad pointer
-    uint8_t bbuffer[LFS_BLOCK_SIZE];
-    cfg.read(&cfg, ctz.head, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
+    uint8_t bbuffer[BLOCK_SIZE];
+    cfg->read(cfg, ctz.head, 0, bbuffer, BLOCK_SIZE) => 0;
     uint32_t bad = lfs_tole32(0xcccccccc);
     memcpy(&bbuffer[0], &bad, sizeof(bad));
     memcpy(&bbuffer[4], &bad, sizeof(bad));
-    cfg.erase(&cfg, ctz.head) => 0;
-    cfg.prog(&cfg, ctz.head, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
+    cfg->erase(cfg, ctz.head) => 0;
+    cfg->prog(cfg, ctz.head, 0, bbuffer, BLOCK_SIZE) => 0;
     lfs_deinit(&lfs) => 0;
 
     // test that accessing our bad file fails, note there's a number
     // of ways to access the dir, some can fail, but some don't
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    struct lfs_info info;
     lfs_stat(&lfs, "file_here", &info) => 0;
     assert(strcmp(info.name, "file_here") == 0);
     assert(info.type == LFS_TYPE_REG);
     assert(info.size == SIZE);
 
     lfs_file_open(&lfs, &file, "file_here", LFS_O_RDONLY) => 0;
     lfs_file_read(&lfs, &file, buffer, SIZE) => LFS_ERR_CORRUPT;
     lfs_file_close(&lfs, &file) => 0;
 
     // any allocs that traverse CTZ must unfortunately must fail
-    if (SIZE > 2*LFS_BLOCK_SIZE) {
+    if (SIZE > 2*BLOCK_SIZE) {
         lfs_mkdir(&lfs, "dir_here") => LFS_ERR_CORRUPT;
     }
     lfs_unmount(&lfs) => 0;
 '''
 
 
-[[case]] # invalid gstate pointer
-define.INVALSET = [0x3, 0x1, 0x2]
+[cases.test_evil_invalid_gstate_pointer]
+defines.INVALSET = [0x3, 0x1, 0x2]
 in = "lfs.c"
 code = '''
     // create littlefs
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
     // create an invalid gstate
-    lfs_init(&lfs, &cfg) => 0;
+    lfs_init(&lfs, cfg) => 0;
     lfs_mdir_t mdir;
     lfs_dir_fetch(&lfs, &mdir, (lfs_block_t[2]){0, 1}) => 0;
     lfs_fs_prepmove(&lfs, 1, (lfs_block_t [2]){
             (INVALSET & 0x1) ? 0xcccccccc : 0,
             (INVALSET & 0x2) ? 0xcccccccc : 0});
     lfs_dir_commit(&lfs, &mdir, NULL, 0) => 0;
     lfs_deinit(&lfs) => 0;
 
     // test that mount fails gracefully
     // mount may not fail, but our first alloc should fail when
     // we try to fix the gstate
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "should_fail") => LFS_ERR_CORRUPT;
     lfs_unmount(&lfs) => 0;
 '''
 
 # cycle detection/recovery tests
 
-[[case]] # metadata-pair threaded-list loop test
+[cases.test_evil_mdir_loop] # metadata-pair threaded-list loop test
 in = "lfs.c"
 code = '''
     // create littlefs
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
     // change tail-pointer to point to ourself
-    lfs_init(&lfs, &cfg) => 0;
+    lfs_init(&lfs, cfg) => 0;
     lfs_mdir_t mdir;
     lfs_dir_fetch(&lfs, &mdir, (lfs_block_t[2]){0, 1}) => 0;
     lfs_dir_commit(&lfs, &mdir, LFS_MKATTRS(
             {LFS_MKTAG(LFS_TYPE_HARDTAIL, 0x3ff, 8),
                 (lfs_block_t[2]){0, 1}})) => 0;
     lfs_deinit(&lfs) => 0;
 
     // test that mount fails gracefully
-    lfs_mount(&lfs, &cfg) => LFS_ERR_CORRUPT;
+    lfs_mount(&lfs, cfg) => LFS_ERR_CORRUPT;
 '''
 
-[[case]] # metadata-pair threaded-list 2-length loop test
+[cases.test_evil_mdir_loop2] # metadata-pair threaded-list 2-length loop test
 in = "lfs.c"
 code = '''
     // create littlefs with child dir
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "child") => 0;
     lfs_unmount(&lfs) => 0;
 
     // find child
-    lfs_init(&lfs, &cfg) => 0;
+    lfs_init(&lfs, cfg) => 0;
     lfs_mdir_t mdir;
     lfs_block_t pair[2];
     lfs_dir_fetch(&lfs, &mdir, (lfs_block_t[2]){0, 1}) => 0;
     lfs_dir_get(&lfs, &mdir,
             LFS_MKTAG(0x7ff, 0x3ff, 0),
             LFS_MKTAG(LFS_TYPE_DIRSTRUCT, 1, sizeof(pair)), pair)
                 => LFS_MKTAG(LFS_TYPE_DIRSTRUCT, 1, sizeof(pair));
@@ -251,28 +268,29 @@
     lfs_dir_fetch(&lfs, &mdir, pair) => 0;
     lfs_dir_commit(&lfs, &mdir, LFS_MKATTRS(
             {LFS_MKTAG(LFS_TYPE_HARDTAIL, 0x3ff, 8),
                 (lfs_block_t[2]){0, 1}})) => 0;
     lfs_deinit(&lfs) => 0;
 
     // test that mount fails gracefully
-    lfs_mount(&lfs, &cfg) => LFS_ERR_CORRUPT;
+    lfs_mount(&lfs, cfg) => LFS_ERR_CORRUPT;
 '''
 
-[[case]] # metadata-pair threaded-list 1-length child loop test
+[cases.test_evil_mdir_loop_child] # metadata-pair threaded-list 1-length child loop test
 in = "lfs.c"
 code = '''
     // create littlefs with child dir
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "child") => 0;
     lfs_unmount(&lfs) => 0;
 
     // find child
-    lfs_init(&lfs, &cfg) => 0;
+    lfs_init(&lfs, cfg) => 0;
     lfs_mdir_t mdir;
     lfs_block_t pair[2];
     lfs_dir_fetch(&lfs, &mdir, (lfs_block_t[2]){0, 1}) => 0;
     lfs_dir_get(&lfs, &mdir,
             LFS_MKTAG(0x7ff, 0x3ff, 0),
             LFS_MKTAG(LFS_TYPE_DIRSTRUCT, 1, sizeof(pair)), pair)
                 => LFS_MKTAG(LFS_TYPE_DIRSTRUCT, 1, sizeof(pair));
@@ -280,9 +298,9 @@
     // change tail-pointer to point to ourself
     lfs_dir_fetch(&lfs, &mdir, pair) => 0;
     lfs_dir_commit(&lfs, &mdir, LFS_MKATTRS(
             {LFS_MKTAG(LFS_TYPE_HARDTAIL, 0x3ff, 8), pair})) => 0;
     lfs_deinit(&lfs) => 0;
 
     // test that mount fails gracefully
-    lfs_mount(&lfs, &cfg) => LFS_ERR_CORRUPT;
+    lfs_mount(&lfs, cfg) => LFS_ERR_CORRUPT;
 '''
```

### Comparing `littlefs-python-0.4.0/littlefs/tests/test_exhaustion.toml` & `littlefs-python-0.5.0/littlefs/tests/test_exhaustion.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,465 +1,505 @@
-[[case]] # test running a filesystem to exhaustion
-define.LFS_ERASE_CYCLES = 10
-define.LFS_BLOCK_COUNT = 256 # small bd so test runs faster
-define.LFS_BLOCK_CYCLES = 'LFS_ERASE_CYCLES / 2'
-define.LFS_BADBLOCK_BEHAVIOR = [
-    'LFS_TESTBD_BADBLOCK_PROGERROR',
-    'LFS_TESTBD_BADBLOCK_ERASEERROR',
-    'LFS_TESTBD_BADBLOCK_READERROR',
-    'LFS_TESTBD_BADBLOCK_PROGNOOP',
-    'LFS_TESTBD_BADBLOCK_ERASENOOP',
+# test running a filesystem to exhaustion
+[cases.test_exhaustion_normal]
+defines.ERASE_CYCLES = 10
+defines.BLOCK_COUNT = 256 # small bd so test runs faster
+defines.BLOCK_CYCLES = 'ERASE_CYCLES / 2'
+defines.BADBLOCK_BEHAVIOR = [
+    'LFS_EMUBD_BADBLOCK_PROGERROR',
+    'LFS_EMUBD_BADBLOCK_ERASEERROR',
+    'LFS_EMUBD_BADBLOCK_READERROR',
+    'LFS_EMUBD_BADBLOCK_PROGNOOP',
+    'LFS_EMUBD_BADBLOCK_ERASENOOP',
 ]
-define.FILES = 10
+defines.FILES = 10
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "roadrunner") => 0;
     lfs_unmount(&lfs) => 0;
 
     uint32_t cycle = 0;
     while (true) {
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         for (uint32_t i = 0; i < FILES; i++) {
             // chose name, roughly random seed, and random 2^n size
+            char path[1024];
             sprintf(path, "roadrunner/test%d", i);
-            srand(cycle * i);
-            size = 1 << ((rand() % 10)+2);
+            uint32_t prng = cycle * i;
+            lfs_size_t size = 1 << ((TEST_PRNG(&prng) % 10)+2);
 
+            lfs_file_t file;
             lfs_file_open(&lfs, &file, path,
                     LFS_O_WRONLY | LFS_O_CREAT | LFS_O_TRUNC) => 0;
 
             for (lfs_size_t j = 0; j < size; j++) {
-                char c = 'a' + (rand() % 26);
+                char c = 'a' + (TEST_PRNG(&prng) % 26);
                 lfs_ssize_t res = lfs_file_write(&lfs, &file, &c, 1);
                 assert(res == 1 || res == LFS_ERR_NOSPC);
                 if (res == LFS_ERR_NOSPC) {
-                    err = lfs_file_close(&lfs, &file);
+                    int err = lfs_file_close(&lfs, &file);
                     assert(err == 0 || err == LFS_ERR_NOSPC);
                     lfs_unmount(&lfs) => 0;
                     goto exhausted;
                 }
             }
 
-            err = lfs_file_close(&lfs, &file);
+            int err = lfs_file_close(&lfs, &file);
             assert(err == 0 || err == LFS_ERR_NOSPC);
             if (err == LFS_ERR_NOSPC) {
                 lfs_unmount(&lfs) => 0;
                 goto exhausted;
             }
         }
 
         for (uint32_t i = 0; i < FILES; i++) {
             // check for errors
+            char path[1024];
             sprintf(path, "roadrunner/test%d", i);
-            srand(cycle * i);
-            size = 1 << ((rand() % 10)+2);
+            uint32_t prng = cycle * i;
+            lfs_size_t size = 1 << ((TEST_PRNG(&prng) % 10)+2);
 
+            lfs_file_t file;
             lfs_file_open(&lfs, &file, path, LFS_O_RDONLY) => 0;
             for (lfs_size_t j = 0; j < size; j++) {
-                char c = 'a' + (rand() % 26);
+                char c = 'a' + (TEST_PRNG(&prng) % 26);
                 char r;
                 lfs_file_read(&lfs, &file, &r, 1) => 1;
                 assert(r == c);
             }
 
             lfs_file_close(&lfs, &file) => 0;
         }
         lfs_unmount(&lfs) => 0;
 
         cycle += 1;
     }
 
 exhausted:
     // should still be readable
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (uint32_t i = 0; i < FILES; i++) {
         // check for errors
+        char path[1024];
         sprintf(path, "roadrunner/test%d", i);
+        struct lfs_info info;
         lfs_stat(&lfs, path, &info) => 0;
     }
     lfs_unmount(&lfs) => 0;
 
     LFS_WARN("completed %d cycles", cycle);
 '''
 
-[[case]] # test running a filesystem to exhaustion
-         # which also requires expanding superblocks
-define.LFS_ERASE_CYCLES = 10
-define.LFS_BLOCK_COUNT = 256 # small bd so test runs faster
-define.LFS_BLOCK_CYCLES = 'LFS_ERASE_CYCLES / 2'
-define.LFS_BADBLOCK_BEHAVIOR = [
-    'LFS_TESTBD_BADBLOCK_PROGERROR',
-    'LFS_TESTBD_BADBLOCK_ERASEERROR',
-    'LFS_TESTBD_BADBLOCK_READERROR',
-    'LFS_TESTBD_BADBLOCK_PROGNOOP',
-    'LFS_TESTBD_BADBLOCK_ERASENOOP',
+# test running a filesystem to exhaustion
+# which also requires expanding superblocks
+[cases.test_exhaustion_superblocks]
+defines.ERASE_CYCLES = 10
+defines.BLOCK_COUNT = 256 # small bd so test runs faster
+defines.BLOCK_CYCLES = 'ERASE_CYCLES / 2'
+defines.BADBLOCK_BEHAVIOR = [
+    'LFS_EMUBD_BADBLOCK_PROGERROR',
+    'LFS_EMUBD_BADBLOCK_ERASEERROR',
+    'LFS_EMUBD_BADBLOCK_READERROR',
+    'LFS_EMUBD_BADBLOCK_PROGNOOP',
+    'LFS_EMUBD_BADBLOCK_ERASENOOP',
 ]
-define.FILES = 10
+defines.FILES = 10
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
     uint32_t cycle = 0;
     while (true) {
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         for (uint32_t i = 0; i < FILES; i++) {
             // chose name, roughly random seed, and random 2^n size
+            char path[1024];
             sprintf(path, "test%d", i);
-            srand(cycle * i);
-            size = 1 << ((rand() % 10)+2);
+            uint32_t prng = cycle * i;
+            lfs_size_t size = 1 << ((TEST_PRNG(&prng) % 10)+2);
 
+            lfs_file_t file;
             lfs_file_open(&lfs, &file, path,
                     LFS_O_WRONLY | LFS_O_CREAT | LFS_O_TRUNC) => 0;
 
             for (lfs_size_t j = 0; j < size; j++) {
-                char c = 'a' + (rand() % 26);
+                char c = 'a' + (TEST_PRNG(&prng) % 26);
                 lfs_ssize_t res = lfs_file_write(&lfs, &file, &c, 1);
                 assert(res == 1 || res == LFS_ERR_NOSPC);
                 if (res == LFS_ERR_NOSPC) {
-                    err = lfs_file_close(&lfs, &file);
+                    int err = lfs_file_close(&lfs, &file);
                     assert(err == 0 || err == LFS_ERR_NOSPC);
                     lfs_unmount(&lfs) => 0;
                     goto exhausted;
                 }
             }
 
-            err = lfs_file_close(&lfs, &file);
+            int err = lfs_file_close(&lfs, &file);
             assert(err == 0 || err == LFS_ERR_NOSPC);
             if (err == LFS_ERR_NOSPC) {
                 lfs_unmount(&lfs) => 0;
                 goto exhausted;
             }
         }
 
         for (uint32_t i = 0; i < FILES; i++) {
             // check for errors
+            char path[1024];
             sprintf(path, "test%d", i);
-            srand(cycle * i);
-            size = 1 << ((rand() % 10)+2);
+            uint32_t prng = cycle * i;
+            lfs_size_t size = 1 << ((TEST_PRNG(&prng) % 10)+2);
 
+            lfs_file_t file;
             lfs_file_open(&lfs, &file, path, LFS_O_RDONLY) => 0;
             for (lfs_size_t j = 0; j < size; j++) {
-                char c = 'a' + (rand() % 26);
+                char c = 'a' + (TEST_PRNG(&prng) % 26);
                 char r;
                 lfs_file_read(&lfs, &file, &r, 1) => 1;
                 assert(r == c);
             }
 
             lfs_file_close(&lfs, &file) => 0;
         }
         lfs_unmount(&lfs) => 0;
 
         cycle += 1;
     }
 
 exhausted:
     // should still be readable
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (uint32_t i = 0; i < FILES; i++) {
         // check for errors
+        char path[1024];
+        struct lfs_info info;
         sprintf(path, "test%d", i);
         lfs_stat(&lfs, path, &info) => 0;
     }
     lfs_unmount(&lfs) => 0;
 
     LFS_WARN("completed %d cycles", cycle);
 '''
 
 # These are a sort of high-level litmus test for wear-leveling. One definition
 # of wear-leveling is that increasing a block device's space translates directly
 # into increasing the block devices lifetime. This is something we can actually
 # check for.
 
-[[case]] # wear-level test running a filesystem to exhaustion
-define.LFS_ERASE_CYCLES = 20
-define.LFS_BLOCK_COUNT = 256 # small bd so test runs faster
-define.LFS_BLOCK_CYCLES = 'LFS_ERASE_CYCLES / 2'
-define.FILES = 10
+# wear-level test running a filesystem to exhaustion
+[cases.test_exhuastion_wear_leveling]
+defines.ERASE_CYCLES = 20
+defines.BLOCK_COUNT = 256 # small bd so test runs faster
+defines.BLOCK_CYCLES = 'ERASE_CYCLES / 2'
+defines.FILES = 10
 code = '''
     uint32_t run_cycles[2];
-    const uint32_t run_block_count[2] = {LFS_BLOCK_COUNT/2, LFS_BLOCK_COUNT};
+    const uint32_t run_block_count[2] = {BLOCK_COUNT/2, BLOCK_COUNT};
 
     for (int run = 0; run < 2; run++) {
-        for (lfs_block_t b = 0; b < LFS_BLOCK_COUNT; b++) {
-            lfs_testbd_setwear(&cfg, b,
-                    (b < run_block_count[run]) ? 0 : LFS_ERASE_CYCLES) => 0;
+        for (lfs_block_t b = 0; b < BLOCK_COUNT; b++) {
+            lfs_emubd_setwear(cfg, b,
+                    (b < run_block_count[run]) ? 0 : ERASE_CYCLES) => 0;
         }
 
-        lfs_format(&lfs, &cfg) => 0;
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_t lfs;
+        lfs_format(&lfs, cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         lfs_mkdir(&lfs, "roadrunner") => 0;
         lfs_unmount(&lfs) => 0;
 
         uint32_t cycle = 0;
         while (true) {
-            lfs_mount(&lfs, &cfg) => 0;
+            lfs_mount(&lfs, cfg) => 0;
             for (uint32_t i = 0; i < FILES; i++) {
                 // chose name, roughly random seed, and random 2^n size
+                char path[1024];
                 sprintf(path, "roadrunner/test%d", i);
-                srand(cycle * i);
-                size = 1 << ((rand() % 10)+2);
+                uint32_t prng = cycle * i;
+                lfs_size_t size = 1 << ((TEST_PRNG(&prng) % 10)+2);
 
+                lfs_file_t file;
                 lfs_file_open(&lfs, &file, path,
                         LFS_O_WRONLY | LFS_O_CREAT | LFS_O_TRUNC) => 0;
 
                 for (lfs_size_t j = 0; j < size; j++) {
-                    char c = 'a' + (rand() % 26);
+                    char c = 'a' + (TEST_PRNG(&prng) % 26);
                     lfs_ssize_t res = lfs_file_write(&lfs, &file, &c, 1);
                     assert(res == 1 || res == LFS_ERR_NOSPC);
                     if (res == LFS_ERR_NOSPC) {
-                        err = lfs_file_close(&lfs, &file);
+                        int err = lfs_file_close(&lfs, &file);
                         assert(err == 0 || err == LFS_ERR_NOSPC);
                         lfs_unmount(&lfs) => 0;
                         goto exhausted;
                     }
                 }
 
-                err = lfs_file_close(&lfs, &file);
+                int err = lfs_file_close(&lfs, &file);
                 assert(err == 0 || err == LFS_ERR_NOSPC);
                 if (err == LFS_ERR_NOSPC) {
                     lfs_unmount(&lfs) => 0;
                     goto exhausted;
                 }
             }
 
             for (uint32_t i = 0; i < FILES; i++) {
                 // check for errors
+                char path[1024];
                 sprintf(path, "roadrunner/test%d", i);
-                srand(cycle * i);
-                size = 1 << ((rand() % 10)+2);
+                uint32_t prng = cycle * i;
+                lfs_size_t size = 1 << ((TEST_PRNG(&prng) % 10)+2);
 
+                lfs_file_t file;
                 lfs_file_open(&lfs, &file, path, LFS_O_RDONLY) => 0;
                 for (lfs_size_t j = 0; j < size; j++) {
-                    char c = 'a' + (rand() % 26);
+                    char c = 'a' + (TEST_PRNG(&prng) % 26);
                     char r;
                     lfs_file_read(&lfs, &file, &r, 1) => 1;
                     assert(r == c);
                 }
 
                 lfs_file_close(&lfs, &file) => 0;
             }
             lfs_unmount(&lfs) => 0;
 
             cycle += 1;
         }
 
 exhausted:
         // should still be readable
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         for (uint32_t i = 0; i < FILES; i++) {
             // check for errors
+            char path[1024];
+            struct lfs_info info;
             sprintf(path, "roadrunner/test%d", i);
             lfs_stat(&lfs, path, &info) => 0;
         }
         lfs_unmount(&lfs) => 0;
 
         run_cycles[run] = cycle;
         LFS_WARN("completed %d blocks %d cycles",
                 run_block_count[run], run_cycles[run]);
     }
 
     // check we increased the lifetime by 2x with ~10% error
     LFS_ASSERT(run_cycles[1]*110/100 > 2*run_cycles[0]);
 '''
 
-[[case]] # wear-level test + expanding superblock
-define.LFS_ERASE_CYCLES = 20
-define.LFS_BLOCK_COUNT = 256 # small bd so test runs faster
-define.LFS_BLOCK_CYCLES = 'LFS_ERASE_CYCLES / 2'
-define.FILES = 10
+# wear-level test + expanding superblock
+[cases.test_exhaustion_wear_leveling_superblocks]
+defines.ERASE_CYCLES = 20
+defines.BLOCK_COUNT = 256 # small bd so test runs faster
+defines.BLOCK_CYCLES = 'ERASE_CYCLES / 2'
+defines.FILES = 10
 code = '''
     uint32_t run_cycles[2];
-    const uint32_t run_block_count[2] = {LFS_BLOCK_COUNT/2, LFS_BLOCK_COUNT};
+    const uint32_t run_block_count[2] = {BLOCK_COUNT/2, BLOCK_COUNT};
 
     for (int run = 0; run < 2; run++) {
-        for (lfs_block_t b = 0; b < LFS_BLOCK_COUNT; b++) {
-            lfs_testbd_setwear(&cfg, b,
-                    (b < run_block_count[run]) ? 0 : LFS_ERASE_CYCLES) => 0;
+        for (lfs_block_t b = 0; b < BLOCK_COUNT; b++) {
+            lfs_emubd_setwear(cfg, b,
+                    (b < run_block_count[run]) ? 0 : ERASE_CYCLES) => 0;
         }
 
-        lfs_format(&lfs, &cfg) => 0;
+        lfs_t lfs;
+        lfs_format(&lfs, cfg) => 0;
 
         uint32_t cycle = 0;
         while (true) {
-            lfs_mount(&lfs, &cfg) => 0;
+            lfs_mount(&lfs, cfg) => 0;
             for (uint32_t i = 0; i < FILES; i++) {
                 // chose name, roughly random seed, and random 2^n size
+                char path[1024];
                 sprintf(path, "test%d", i);
-                srand(cycle * i);
-                size = 1 << ((rand() % 10)+2);
+                uint32_t prng = cycle * i;
+                lfs_size_t size = 1 << ((TEST_PRNG(&prng) % 10)+2);
 
+                lfs_file_t file;
                 lfs_file_open(&lfs, &file, path,
                         LFS_O_WRONLY | LFS_O_CREAT | LFS_O_TRUNC) => 0;
 
                 for (lfs_size_t j = 0; j < size; j++) {
-                    char c = 'a' + (rand() % 26);
+                    char c = 'a' + (TEST_PRNG(&prng) % 26);
                     lfs_ssize_t res = lfs_file_write(&lfs, &file, &c, 1);
                     assert(res == 1 || res == LFS_ERR_NOSPC);
                     if (res == LFS_ERR_NOSPC) {
-                        err = lfs_file_close(&lfs, &file);
+                        int err = lfs_file_close(&lfs, &file);
                         assert(err == 0 || err == LFS_ERR_NOSPC);
                         lfs_unmount(&lfs) => 0;
                         goto exhausted;
                     }
                 }
 
-                err = lfs_file_close(&lfs, &file);
+                int err = lfs_file_close(&lfs, &file);
                 assert(err == 0 || err == LFS_ERR_NOSPC);
                 if (err == LFS_ERR_NOSPC) {
                     lfs_unmount(&lfs) => 0;
                     goto exhausted;
                 }
             }
 
             for (uint32_t i = 0; i < FILES; i++) {
                 // check for errors
+                char path[1024];
                 sprintf(path, "test%d", i);
-                srand(cycle * i);
-                size = 1 << ((rand() % 10)+2);
+                uint32_t prng = cycle * i;
+                lfs_size_t size = 1 << ((TEST_PRNG(&prng) % 10)+2);
 
+                lfs_file_t file;
                 lfs_file_open(&lfs, &file, path, LFS_O_RDONLY) => 0;
                 for (lfs_size_t j = 0; j < size; j++) {
-                    char c = 'a' + (rand() % 26);
+                    char c = 'a' + (TEST_PRNG(&prng) % 26);
                     char r;
                     lfs_file_read(&lfs, &file, &r, 1) => 1;
                     assert(r == c);
                 }
 
                 lfs_file_close(&lfs, &file) => 0;
             }
             lfs_unmount(&lfs) => 0;
 
             cycle += 1;
         }
 
 exhausted:
         // should still be readable
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         for (uint32_t i = 0; i < FILES; i++) {
             // check for errors
+            char path[1024];
+            struct lfs_info info;
             sprintf(path, "test%d", i);
             lfs_stat(&lfs, path, &info) => 0;
         }
         lfs_unmount(&lfs) => 0;
 
         run_cycles[run] = cycle;
         LFS_WARN("completed %d blocks %d cycles",
                 run_block_count[run], run_cycles[run]);
     }
 
     // check we increased the lifetime by 2x with ~10% error
     LFS_ASSERT(run_cycles[1]*110/100 > 2*run_cycles[0]);
 '''
 
-[[case]] # test that we wear blocks roughly evenly
-define.LFS_ERASE_CYCLES = 0xffffffff
-define.LFS_BLOCK_COUNT = 256 # small bd so test runs faster
-define.LFS_BLOCK_CYCLES = [5, 4, 3, 2, 1]
-define.CYCLES = 100
-define.FILES = 10
-if = 'LFS_BLOCK_CYCLES < CYCLES/10'
+# test that we wear blocks roughly evenly
+[cases.test_exhaustion_wear_distribution]
+defines.ERASE_CYCLES = 0xffffffff
+defines.BLOCK_COUNT = 256 # small bd so test runs faster
+defines.BLOCK_CYCLES = [5, 4, 3, 2, 1]
+defines.CYCLES = 100
+defines.FILES = 10
+if = 'BLOCK_CYCLES < CYCLES/10'
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "roadrunner") => 0;
     lfs_unmount(&lfs) => 0;
 
     uint32_t cycle = 0;
     while (cycle < CYCLES) {
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         for (uint32_t i = 0; i < FILES; i++) {
             // chose name, roughly random seed, and random 2^n size
+            char path[1024];
             sprintf(path, "roadrunner/test%d", i);
-            srand(cycle * i);
-            size = 1 << 4; //((rand() % 10)+2);
+            uint32_t prng = cycle * i;
+            lfs_size_t size = 1 << 4; //((TEST_PRNG(&prng) % 10)+2);
 
+            lfs_file_t file;
             lfs_file_open(&lfs, &file, path,
                     LFS_O_WRONLY | LFS_O_CREAT | LFS_O_TRUNC) => 0;
 
             for (lfs_size_t j = 0; j < size; j++) {
-                char c = 'a' + (rand() % 26);
+                char c = 'a' + (TEST_PRNG(&prng) % 26);
                 lfs_ssize_t res = lfs_file_write(&lfs, &file, &c, 1);
                 assert(res == 1 || res == LFS_ERR_NOSPC);
                 if (res == LFS_ERR_NOSPC) {
-                    err = lfs_file_close(&lfs, &file);
+                    int err = lfs_file_close(&lfs, &file);
                     assert(err == 0 || err == LFS_ERR_NOSPC);
                     lfs_unmount(&lfs) => 0;
                     goto exhausted;
                 }
             }
 
-            err = lfs_file_close(&lfs, &file);
+            int err = lfs_file_close(&lfs, &file);
             assert(err == 0 || err == LFS_ERR_NOSPC);
             if (err == LFS_ERR_NOSPC) {
                 lfs_unmount(&lfs) => 0;
                 goto exhausted;
             }
         }
 
         for (uint32_t i = 0; i < FILES; i++) {
             // check for errors
+            char path[1024];
             sprintf(path, "roadrunner/test%d", i);
-            srand(cycle * i);
-            size = 1 << 4; //((rand() % 10)+2);
+            uint32_t prng = cycle * i;
+            lfs_size_t size = 1 << 4; //((TEST_PRNG(&prng) % 10)+2);
 
+            lfs_file_t file;
             lfs_file_open(&lfs, &file, path, LFS_O_RDONLY) => 0;
             for (lfs_size_t j = 0; j < size; j++) {
-                char c = 'a' + (rand() % 26);
+                char c = 'a' + (TEST_PRNG(&prng) % 26);
                 char r;
                 lfs_file_read(&lfs, &file, &r, 1) => 1;
                 assert(r == c);
             }
 
             lfs_file_close(&lfs, &file) => 0;
         }
         lfs_unmount(&lfs) => 0;
 
         cycle += 1;
     }
 
 exhausted:
     // should still be readable
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (uint32_t i = 0; i < FILES; i++) {
         // check for errors
+        char path[1024];
+        struct lfs_info info;
         sprintf(path, "roadrunner/test%d", i);
         lfs_stat(&lfs, path, &info) => 0;
     }
     lfs_unmount(&lfs) => 0;
 
     LFS_WARN("completed %d cycles", cycle);
 
     // check the wear on our block device
-    lfs_testbd_wear_t minwear = -1;
-    lfs_testbd_wear_t totalwear = 0;
-    lfs_testbd_wear_t maxwear = 0;
+    lfs_emubd_wear_t minwear = -1;
+    lfs_emubd_wear_t totalwear = 0;
+    lfs_emubd_wear_t maxwear = 0;
     // skip 0 and 1 as superblock movement is intentionally avoided
-    for (lfs_block_t b = 2; b < LFS_BLOCK_COUNT; b++) {
-        lfs_testbd_wear_t wear = lfs_testbd_getwear(&cfg, b);
+    for (lfs_block_t b = 2; b < BLOCK_COUNT; b++) {
+        lfs_emubd_wear_t wear = lfs_emubd_wear(cfg, b);
         printf("%08x: wear %d\n", b, wear);
         assert(wear >= 0);
         if (wear < minwear) {
             minwear = wear;
         }
         if (wear > maxwear) {
             maxwear = wear;
         }
         totalwear += wear;
     }
-    lfs_testbd_wear_t avgwear = totalwear / LFS_BLOCK_COUNT;
+    lfs_emubd_wear_t avgwear = totalwear / BLOCK_COUNT;
     LFS_WARN("max wear: %d cycles", maxwear);
-    LFS_WARN("avg wear: %d cycles", totalwear / LFS_BLOCK_COUNT);
+    LFS_WARN("avg wear: %d cycles", totalwear / (int)BLOCK_COUNT);
     LFS_WARN("min wear: %d cycles", minwear);
 
     // find standard deviation^2
-    lfs_testbd_wear_t dev2 = 0;
-    for (lfs_block_t b = 2; b < LFS_BLOCK_COUNT; b++) {
-        lfs_testbd_wear_t wear = lfs_testbd_getwear(&cfg, b);
+    lfs_emubd_wear_t dev2 = 0;
+    for (lfs_block_t b = 2; b < BLOCK_COUNT; b++) {
+        lfs_emubd_wear_t wear = lfs_emubd_wear(cfg, b);
         assert(wear >= 0);
-        lfs_testbd_swear_t diff = wear - avgwear;
+        lfs_emubd_swear_t diff = wear - avgwear;
         dev2 += diff*diff;
     }
     dev2 /= totalwear;
     LFS_WARN("std dev^2: %d", dev2);
     assert(dev2 < 8);
 '''
```

### Comparing `littlefs-python-0.4.0/littlefs/tests/test_files.toml` & `littlefs-python-0.5.0/littlefs/tests/test_files.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,480 +1,510 @@
 
-[[case]] # simple file test
+[cases.test_files_simple]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "hello",
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => 0;
-    size = strlen("Hello World!")+1;
+    lfs_size_t size = strlen("Hello World!")+1;
+    uint8_t buffer[1024];
     strcpy((char*)buffer, "Hello World!");
     lfs_file_write(&lfs, &file, buffer, size) => size;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "hello", LFS_O_RDONLY) => 0;
     lfs_file_read(&lfs, &file, buffer, size) => size;
     assert(strcmp((char*)buffer, "Hello World!") == 0);
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # larger files
-define.SIZE = [32, 8192, 262144, 0, 7, 8193]
-define.CHUNKSIZE = [31, 16, 33, 1, 1023]
+[cases.test_files_large]
+defines.SIZE = [32, 8192, 262144, 0, 7, 8193]
+defines.CHUNKSIZE = [31, 16, 33, 1, 1023]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
     // write
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "avacado",
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => 0;
-    srand(1);
+    uint32_t prng = 1;
+    uint8_t buffer[1024];
     for (lfs_size_t i = 0; i < SIZE; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE-i);
         for (lfs_size_t b = 0; b < chunk; b++) {
-            buffer[b] = rand() & 0xff;
+            buffer[b] = TEST_PRNG(&prng) & 0xff;
         }
         lfs_file_write(&lfs, &file, buffer, chunk) => chunk;
     }
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
     // read
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "avacado", LFS_O_RDONLY) => 0;
     lfs_file_size(&lfs, &file) => SIZE;
-    srand(1);
+    prng = 1;
     for (lfs_size_t i = 0; i < SIZE; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE-i);
         lfs_file_read(&lfs, &file, buffer, chunk) => chunk;
         for (lfs_size_t b = 0; b < chunk; b++) {
-            assert(buffer[b] == (rand() & 0xff));
+            assert(buffer[b] == (TEST_PRNG(&prng) & 0xff));
         }
     }
     lfs_file_read(&lfs, &file, buffer, CHUNKSIZE) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # rewriting files
-define.SIZE1 = [32, 8192, 131072, 0, 7, 8193]
-define.SIZE2 = [32, 8192, 131072, 0, 7, 8193]
-define.CHUNKSIZE = [31, 16, 1]
+[cases.test_files_rewrite]
+defines.SIZE1 = [32, 8192, 131072, 0, 7, 8193]
+defines.SIZE2 = [32, 8192, 131072, 0, 7, 8193]
+defines.CHUNKSIZE = [31, 16, 1]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
     // write
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
+    uint8_t buffer[1024];
     lfs_file_open(&lfs, &file, "avacado",
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => 0;
-    srand(1);
+    uint32_t prng = 1;
     for (lfs_size_t i = 0; i < SIZE1; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE1-i);
         for (lfs_size_t b = 0; b < chunk; b++) {
-            buffer[b] = rand() & 0xff;
+            buffer[b] = TEST_PRNG(&prng) & 0xff;
         }
         lfs_file_write(&lfs, &file, buffer, chunk) => chunk;
     }
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
     // read
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "avacado", LFS_O_RDONLY) => 0;
     lfs_file_size(&lfs, &file) => SIZE1;
-    srand(1);
+    prng = 1;
     for (lfs_size_t i = 0; i < SIZE1; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE1-i);
         lfs_file_read(&lfs, &file, buffer, chunk) => chunk;
         for (lfs_size_t b = 0; b < chunk; b++) {
-            assert(buffer[b] == (rand() & 0xff));
+            assert(buffer[b] == (TEST_PRNG(&prng) & 0xff));
         }
     }
     lfs_file_read(&lfs, &file, buffer, CHUNKSIZE) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
     // rewrite
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "avacado", LFS_O_WRONLY) => 0;
-    srand(2);
+    prng = 2;
     for (lfs_size_t i = 0; i < SIZE2; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE2-i);
         for (lfs_size_t b = 0; b < chunk; b++) {
-            buffer[b] = rand() & 0xff;
+            buffer[b] = TEST_PRNG(&prng) & 0xff;
         }
         lfs_file_write(&lfs, &file, buffer, chunk) => chunk;
     }
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
     // read
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "avacado", LFS_O_RDONLY) => 0;
     lfs_file_size(&lfs, &file) => lfs_max(SIZE1, SIZE2);
-    srand(2);
+    prng = 2;
     for (lfs_size_t i = 0; i < SIZE2; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE2-i);
         lfs_file_read(&lfs, &file, buffer, chunk) => chunk;
         for (lfs_size_t b = 0; b < chunk; b++) {
-            assert(buffer[b] == (rand() & 0xff));
+            assert(buffer[b] == (TEST_PRNG(&prng) & 0xff));
         }
     }
     if (SIZE1 > SIZE2) {
-        srand(1);
+        prng = 1;
         for (lfs_size_t b = 0; b < SIZE2; b++) {
-            rand();
+            TEST_PRNG(&prng);
         }
         for (lfs_size_t i = SIZE2; i < SIZE1; i += CHUNKSIZE) {
             lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE1-i);
             lfs_file_read(&lfs, &file, buffer, chunk) => chunk;
             for (lfs_size_t b = 0; b < chunk; b++) {
-                assert(buffer[b] == (rand() & 0xff));
+                assert(buffer[b] == (TEST_PRNG(&prng) & 0xff));
             }
         }
     }
     lfs_file_read(&lfs, &file, buffer, CHUNKSIZE) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # appending files
-define.SIZE1 = [32, 8192, 131072, 0, 7, 8193]
-define.SIZE2 = [32, 8192, 131072, 0, 7, 8193]
-define.CHUNKSIZE = [31, 16, 1]
+[cases.test_files_append]
+defines.SIZE1 = [32, 8192, 131072, 0, 7, 8193]
+defines.SIZE2 = [32, 8192, 131072, 0, 7, 8193]
+defines.CHUNKSIZE = [31, 16, 1]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
     // write
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
+    uint8_t buffer[1024];
     lfs_file_open(&lfs, &file, "avacado",
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => 0;
-    srand(1);
+    uint32_t prng = 1;
     for (lfs_size_t i = 0; i < SIZE1; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE1-i);
         for (lfs_size_t b = 0; b < chunk; b++) {
-            buffer[b] = rand() & 0xff;
+            buffer[b] = TEST_PRNG(&prng) & 0xff;
         }
         lfs_file_write(&lfs, &file, buffer, chunk) => chunk;
     }
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
     // read
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "avacado", LFS_O_RDONLY) => 0;
     lfs_file_size(&lfs, &file) => SIZE1;
-    srand(1);
+    prng = 1;
     for (lfs_size_t i = 0; i < SIZE1; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE1-i);
         lfs_file_read(&lfs, &file, buffer, chunk) => chunk;
         for (lfs_size_t b = 0; b < chunk; b++) {
-            assert(buffer[b] == (rand() & 0xff));
+            assert(buffer[b] == (TEST_PRNG(&prng) & 0xff));
         }
     }
     lfs_file_read(&lfs, &file, buffer, CHUNKSIZE) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
     // append
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "avacado", LFS_O_WRONLY | LFS_O_APPEND) => 0;
-    srand(2);
+    prng = 2;
     for (lfs_size_t i = 0; i < SIZE2; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE2-i);
         for (lfs_size_t b = 0; b < chunk; b++) {
-            buffer[b] = rand() & 0xff;
+            buffer[b] = TEST_PRNG(&prng) & 0xff;
         }
         lfs_file_write(&lfs, &file, buffer, chunk) => chunk;
     }
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
     // read
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "avacado", LFS_O_RDONLY) => 0;
     lfs_file_size(&lfs, &file) => SIZE1 + SIZE2;
-    srand(1);
+    prng = 1;
     for (lfs_size_t i = 0; i < SIZE1; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE1-i);
         lfs_file_read(&lfs, &file, buffer, chunk) => chunk;
         for (lfs_size_t b = 0; b < chunk; b++) {
-            assert(buffer[b] == (rand() & 0xff));
+            assert(buffer[b] == (TEST_PRNG(&prng) & 0xff));
         }
     }
-    srand(2);
+    prng = 2;
     for (lfs_size_t i = 0; i < SIZE2; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE2-i);
         lfs_file_read(&lfs, &file, buffer, chunk) => chunk;
         for (lfs_size_t b = 0; b < chunk; b++) {
-            assert(buffer[b] == (rand() & 0xff));
+            assert(buffer[b] == (TEST_PRNG(&prng) & 0xff));
         }
     }
     lfs_file_read(&lfs, &file, buffer, CHUNKSIZE) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # truncating files
-define.SIZE1 = [32, 8192, 131072, 0, 7, 8193]
-define.SIZE2 = [32, 8192, 131072, 0, 7, 8193]
-define.CHUNKSIZE = [31, 16, 1]
+[cases.test_files_truncate]
+defines.SIZE1 = [32, 8192, 131072, 0, 7, 8193]
+defines.SIZE2 = [32, 8192, 131072, 0, 7, 8193]
+defines.CHUNKSIZE = [31, 16, 1]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
     // write
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
+    uint8_t buffer[1024];
     lfs_file_open(&lfs, &file, "avacado",
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => 0;
-    srand(1);
+    uint32_t prng = 1;
     for (lfs_size_t i = 0; i < SIZE1; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE1-i);
         for (lfs_size_t b = 0; b < chunk; b++) {
-            buffer[b] = rand() & 0xff;
+            buffer[b] = TEST_PRNG(&prng) & 0xff;
         }
         lfs_file_write(&lfs, &file, buffer, chunk) => chunk;
     }
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
     // read
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "avacado", LFS_O_RDONLY) => 0;
     lfs_file_size(&lfs, &file) => SIZE1;
-    srand(1);
+    prng = 1;
     for (lfs_size_t i = 0; i < SIZE1; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE1-i);
         lfs_file_read(&lfs, &file, buffer, chunk) => chunk;
         for (lfs_size_t b = 0; b < chunk; b++) {
-            assert(buffer[b] == (rand() & 0xff));
+            assert(buffer[b] == (TEST_PRNG(&prng) & 0xff));
         }
     }
     lfs_file_read(&lfs, &file, buffer, CHUNKSIZE) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
     // truncate
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "avacado", LFS_O_WRONLY | LFS_O_TRUNC) => 0;
-    srand(2);
+    prng = 2;
     for (lfs_size_t i = 0; i < SIZE2; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE2-i);
         for (lfs_size_t b = 0; b < chunk; b++) {
-            buffer[b] = rand() & 0xff;
+            buffer[b] = TEST_PRNG(&prng) & 0xff;
         }
         lfs_file_write(&lfs, &file, buffer, chunk) => chunk;
     }
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
     // read
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "avacado", LFS_O_RDONLY) => 0;
     lfs_file_size(&lfs, &file) => SIZE2;
-    srand(2);
+    prng = 2;
     for (lfs_size_t i = 0; i < SIZE2; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE2-i);
         lfs_file_read(&lfs, &file, buffer, chunk) => chunk;
         for (lfs_size_t b = 0; b < chunk; b++) {
-            assert(buffer[b] == (rand() & 0xff));
+            assert(buffer[b] == (TEST_PRNG(&prng) & 0xff));
         }
     }
     lfs_file_read(&lfs, &file, buffer, CHUNKSIZE) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # reentrant file writing
-define.SIZE = [32, 0, 7, 2049]
-define.CHUNKSIZE = [31, 16, 65]
+[cases.test_files_reentrant_write]
+defines.SIZE = [32, 0, 7, 2049]
+defines.CHUNKSIZE = [31, 16, 65]
 reentrant = true
 code = '''
-    err = lfs_mount(&lfs, &cfg);
+    lfs_t lfs;
+    int err = lfs_mount(&lfs, cfg);
     if (err) {
-        lfs_format(&lfs, &cfg) => 0;
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_format(&lfs, cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
     }
 
+    lfs_file_t file;
+    uint8_t buffer[1024];
     err = lfs_file_open(&lfs, &file, "avacado", LFS_O_RDONLY);
     assert(err == LFS_ERR_NOENT || err == 0);
     if (err == 0) {
         // can only be 0 (new file) or full size
-        size = lfs_file_size(&lfs, &file);
+        lfs_size_t size = lfs_file_size(&lfs, &file);
         assert(size == 0 || size == SIZE);
         lfs_file_close(&lfs, &file) => 0;
     }
 
     // write
     lfs_file_open(&lfs, &file, "avacado", LFS_O_WRONLY | LFS_O_CREAT) => 0;
-    srand(1);
+    uint32_t prng = 1;
     for (lfs_size_t i = 0; i < SIZE; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE-i);
         for (lfs_size_t b = 0; b < chunk; b++) {
-            buffer[b] = rand() & 0xff;
+            buffer[b] = TEST_PRNG(&prng) & 0xff;
         }
         lfs_file_write(&lfs, &file, buffer, chunk) => chunk;
     }
     lfs_file_close(&lfs, &file) => 0;
 
     // read
     lfs_file_open(&lfs, &file, "avacado", LFS_O_RDONLY) => 0;
     lfs_file_size(&lfs, &file) => SIZE;
-    srand(1);
+    prng = 1;
     for (lfs_size_t i = 0; i < SIZE; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE-i);
         lfs_file_read(&lfs, &file, buffer, chunk) => chunk;
         for (lfs_size_t b = 0; b < chunk; b++) {
-            assert(buffer[b] == (rand() & 0xff));
+            assert(buffer[b] == (TEST_PRNG(&prng) & 0xff));
         }
     }
     lfs_file_read(&lfs, &file, buffer, CHUNKSIZE) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # reentrant file writing with syncs
-define = [
+[cases.test_files_reentrant_write_sync]
+defines = [
     # append (O(n))
     {MODE='LFS_O_APPEND',   SIZE=[32, 0, 7, 2049],  CHUNKSIZE=[31, 16, 65]},
     # truncate (O(n^2))
     {MODE='LFS_O_TRUNC',    SIZE=[32, 0, 7, 200],   CHUNKSIZE=[31, 16, 65]},
     # rewrite (O(n^2))
     {MODE=0,                SIZE=[32, 0, 7, 200],   CHUNKSIZE=[31, 16, 65]},
 ]
 reentrant = true
 code = '''
-    err = lfs_mount(&lfs, &cfg);
+    lfs_t lfs;
+    int err = lfs_mount(&lfs, cfg);
     if (err) {
-        lfs_format(&lfs, &cfg) => 0;
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_format(&lfs, cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
     }
 
+    lfs_file_t file;
+    uint8_t buffer[1024];
     err = lfs_file_open(&lfs, &file, "avacado", LFS_O_RDONLY);
     assert(err == LFS_ERR_NOENT || err == 0);
     if (err == 0) {
         // with syncs we could be any size, but it at least must be valid data
-        size = lfs_file_size(&lfs, &file);
+        lfs_size_t size = lfs_file_size(&lfs, &file);
         assert(size <= SIZE);
-        srand(1);
+        uint32_t prng = 1;
         for (lfs_size_t i = 0; i < size; i += CHUNKSIZE) {
             lfs_size_t chunk = lfs_min(CHUNKSIZE, size-i);
             lfs_file_read(&lfs, &file, buffer, chunk) => chunk;
             for (lfs_size_t b = 0; b < chunk; b++) {
-                assert(buffer[b] == (rand() & 0xff));
+                assert(buffer[b] == (TEST_PRNG(&prng) & 0xff));
             }
         }
         lfs_file_close(&lfs, &file) => 0;
     }
 
     // write
     lfs_file_open(&lfs, &file, "avacado",
         LFS_O_WRONLY | LFS_O_CREAT | MODE) => 0;
-    size = lfs_file_size(&lfs, &file);
+    lfs_size_t size = lfs_file_size(&lfs, &file);
     assert(size <= SIZE);
-    srand(1);
+    uint32_t prng = 1;
     lfs_size_t skip = (MODE == LFS_O_APPEND) ? size : 0;
     for (lfs_size_t b = 0; b < skip; b++) {
-        rand();
+        TEST_PRNG(&prng);
     }
     for (lfs_size_t i = skip; i < SIZE; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE-i);
         for (lfs_size_t b = 0; b < chunk; b++) {
-            buffer[b] = rand() & 0xff;
+            buffer[b] = TEST_PRNG(&prng) & 0xff;
         }
         lfs_file_write(&lfs, &file, buffer, chunk) => chunk;
         lfs_file_sync(&lfs, &file) => 0;
     }
     lfs_file_close(&lfs, &file) => 0;
 
     // read
     lfs_file_open(&lfs, &file, "avacado", LFS_O_RDONLY) => 0;
     lfs_file_size(&lfs, &file) => SIZE;
-    srand(1);
+    prng = 1;
     for (lfs_size_t i = 0; i < SIZE; i += CHUNKSIZE) {
         lfs_size_t chunk = lfs_min(CHUNKSIZE, SIZE-i);
         lfs_file_read(&lfs, &file, buffer, chunk) => chunk;
         for (lfs_size_t b = 0; b < chunk; b++) {
-            assert(buffer[b] == (rand() & 0xff));
+            assert(buffer[b] == (TEST_PRNG(&prng) & 0xff));
         }
     }
     lfs_file_read(&lfs, &file, buffer, CHUNKSIZE) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # many files
-define.N = 300
+[cases.test_files_many]
+defines.N = 300
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
     // create N files of 7 bytes
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int i = 0; i < N; i++) {
+        lfs_file_t file;
+        char path[1024];
         sprintf(path, "file_%03d", i);
         lfs_file_open(&lfs, &file, path,
                 LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => 0;
         char wbuffer[1024];
-        size = 7;
-        snprintf(wbuffer, size, "Hi %03d", i);
+        lfs_size_t size = 7;
+        sprintf(wbuffer, "Hi %03d", i);
         lfs_file_write(&lfs, &file, wbuffer, size) => size;
         lfs_file_close(&lfs, &file) => 0;
 
         char rbuffer[1024];
         lfs_file_open(&lfs, &file, path, LFS_O_RDONLY) => 0;
         lfs_file_read(&lfs, &file, rbuffer, size) => size;
         assert(strcmp(rbuffer, wbuffer) == 0);
         lfs_file_close(&lfs, &file) => 0;
     }
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # many files with power cycle
-define.N = 300
+[cases.test_files_many_power_cycle]
+defines.N = 300
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
     // create N files of 7 bytes
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int i = 0; i < N; i++) {
+        lfs_file_t file;
+        char path[1024];
         sprintf(path, "file_%03d", i);
         lfs_file_open(&lfs, &file, path,
                 LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => 0;
         char wbuffer[1024];
-        size = 7;
-        snprintf(wbuffer, size, "Hi %03d", i);
+        lfs_size_t size = 7;
+        sprintf(wbuffer, "Hi %03d", i);
         lfs_file_write(&lfs, &file, wbuffer, size) => size;
         lfs_file_close(&lfs, &file) => 0;
         lfs_unmount(&lfs) => 0;
 
         char rbuffer[1024];
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         lfs_file_open(&lfs, &file, path, LFS_O_RDONLY) => 0;
         lfs_file_read(&lfs, &file, rbuffer, size) => size;
         assert(strcmp(rbuffer, wbuffer) == 0);
         lfs_file_close(&lfs, &file) => 0;
     }
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # many files with power loss
-define.N = 300
+[cases.test_files_many_power_loss]
+defines.N = 300
 reentrant = true
 code = '''
-    err = lfs_mount(&lfs, &cfg);
+    lfs_t lfs;
+    int err = lfs_mount(&lfs, cfg);
     if (err) {
-        lfs_format(&lfs, &cfg) => 0;
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_format(&lfs, cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
     }
     // create N files of 7 bytes
     for (int i = 0; i < N; i++) {
+        lfs_file_t file;
+        char path[1024];
         sprintf(path, "file_%03d", i);
         err = lfs_file_open(&lfs, &file, path, LFS_O_WRONLY | LFS_O_CREAT);
         char wbuffer[1024];
-        size = 7;
-        snprintf(wbuffer, size, "Hi %03d", i);
+        lfs_size_t size = 7;
+        sprintf(wbuffer, "Hi %03d", i);
         if ((lfs_size_t)lfs_file_size(&lfs, &file) != size) {
             lfs_file_write(&lfs, &file, wbuffer, size) => size;
         }
         lfs_file_close(&lfs, &file) => 0;
 
         char rbuffer[1024];
         lfs_file_open(&lfs, &file, path, LFS_O_RDONLY) => 0;
```

### Comparing `littlefs-python-0.4.0/littlefs/tests/test_interspersed.toml` & `littlefs-python-0.5.0/littlefs/tests/test_orphans.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,244 +1,273 @@
+[cases.test_orphans_normal]
+in = "lfs.c"
+if = 'PROG_SIZE <= 0x3fe' # only works with one crc per commit
+code = '''
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_mkdir(&lfs, "parent") => 0;
+    lfs_mkdir(&lfs, "parent/orphan") => 0;
+    lfs_mkdir(&lfs, "parent/child") => 0;
+    lfs_remove(&lfs, "parent/orphan") => 0;
+    lfs_unmount(&lfs) => 0;
 
-[[case]] # interspersed file test
-define.SIZE = [10, 100]
-define.FILES = [4, 10, 26] 
-code = '''
-    lfs_file_t files[FILES];
-    const char alphas[] = "abcdefghijklmnopqrstuvwxyz";
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
-    for (int j = 0; j < FILES; j++) {
-        sprintf(path, "%c", alphas[j]);
-        lfs_file_open(&lfs, &files[j], path,
-                LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => 0;
-    }
+    // corrupt the child's most recent commit, this should be the update
+    // to the linked-list entry, which should orphan the orphan. Note this
+    // makes a lot of assumptions about the remove operation.
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
+    lfs_dir_open(&lfs, &dir, "parent/child") => 0;
+    lfs_block_t block = dir.m.pair[0];
+    lfs_dir_close(&lfs, &dir) => 0;
+    lfs_unmount(&lfs) => 0;
+    uint8_t buffer[BLOCK_SIZE];
+    cfg->read(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    int off = BLOCK_SIZE-1;
+    while (off >= 0 && buffer[off] == ERASE_VALUE) {
+        off -= 1;
+    }
+    memset(&buffer[off-3], BLOCK_SIZE, 3);
+    cfg->erase(cfg, block) => 0;
+    cfg->prog(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    cfg->sync(cfg) => 0;
+
+    lfs_mount(&lfs, cfg) => 0;
+    struct lfs_info info;
+    lfs_stat(&lfs, "parent/orphan", &info) => LFS_ERR_NOENT;
+    lfs_stat(&lfs, "parent/child", &info) => 0;
+    lfs_fs_size(&lfs) => 8;
+    lfs_unmount(&lfs) => 0;
 
-    for (int i = 0; i < SIZE; i++) {
-        for (int j = 0; j < FILES; j++) {
-            lfs_file_write(&lfs, &files[j], &alphas[j], 1) => 1;
-        }
-    }
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_stat(&lfs, "parent/orphan", &info) => LFS_ERR_NOENT;
+    lfs_stat(&lfs, "parent/child", &info) => 0;
+    lfs_fs_size(&lfs) => 8;
+    // this mkdir should both create a dir and deorphan, so size
+    // should be unchanged
+    lfs_mkdir(&lfs, "parent/otherchild") => 0;
+    lfs_stat(&lfs, "parent/orphan", &info) => LFS_ERR_NOENT;
+    lfs_stat(&lfs, "parent/child", &info) => 0;
+    lfs_stat(&lfs, "parent/otherchild", &info) => 0;
+    lfs_fs_size(&lfs) => 8;
+    lfs_unmount(&lfs) => 0;
 
-    for (int j = 0; j < FILES; j++) {
-        lfs_file_close(&lfs, &files[j]);
-    }
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_stat(&lfs, "parent/orphan", &info) => LFS_ERR_NOENT;
+    lfs_stat(&lfs, "parent/child", &info) => 0;
+    lfs_stat(&lfs, "parent/otherchild", &info) => 0;
+    lfs_fs_size(&lfs) => 8;
+    lfs_unmount(&lfs) => 0;
+'''
 
-    lfs_dir_open(&lfs, &dir, "/") => 0;
-    lfs_dir_read(&lfs, &dir, &info) => 1;
-    assert(strcmp(info.name, ".") == 0);
-    assert(info.type == LFS_TYPE_DIR);
-    lfs_dir_read(&lfs, &dir, &info) => 1;
-    assert(strcmp(info.name, "..") == 0);
-    assert(info.type == LFS_TYPE_DIR);
-    for (int j = 0; j < FILES; j++) {
-        sprintf(path, "%c", alphas[j]);
-        lfs_dir_read(&lfs, &dir, &info) => 1;
-        assert(strcmp(info.name, path) == 0);
-        assert(info.type == LFS_TYPE_REG);
-        assert(info.size == SIZE);
-    }
-    lfs_dir_read(&lfs, &dir, &info) => 0;
-    lfs_dir_close(&lfs, &dir) => 0;
+# test that we only run deorphan once per power-cycle
+[cases.test_orphans_no_orphans]
+in = 'lfs.c'
+code = '''
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
-    for (int j = 0; j < FILES; j++) {
-        sprintf(path, "%c", alphas[j]);
-        lfs_file_open(&lfs, &files[j], path, LFS_O_RDONLY) => 0;
-    }
+    lfs_mount(&lfs, cfg) => 0;
+    // mark the filesystem as having orphans
+    lfs_fs_preporphans(&lfs, +1) => 0;
+    lfs_mdir_t mdir;
+    lfs_dir_fetch(&lfs, &mdir, (lfs_block_t[2]){0, 1}) => 0;
+    lfs_dir_commit(&lfs, &mdir, NULL, 0) => 0;
 
-    for (int i = 0; i < 10; i++) {
-        for (int j = 0; j < FILES; j++) {
-            lfs_file_read(&lfs, &files[j], buffer, 1) => 1;
-            assert(buffer[0] == alphas[j]);
-        }
-    }
+    // we should have orphans at this state
+    assert(lfs_gstate_hasorphans(&lfs.gstate));
+    lfs_unmount(&lfs) => 0;
+
+    // mount
+    lfs_mount(&lfs, cfg) => 0;
+    // we should detect orphans
+    assert(lfs_gstate_hasorphans(&lfs.gstate));
+    // force consistency
+    lfs_fs_forceconsistency(&lfs) => 0;
+    // we should no longer have orphans
+    assert(!lfs_gstate_hasorphans(&lfs.gstate));
 
-    for (int j = 0; j < FILES; j++) {
-        lfs_file_close(&lfs, &files[j]);
-    }
-    
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # interspersed remove file test
-define.SIZE = [10, 100]
-define.FILES = [4, 10, 26]
-code = '''
-    const char alphas[] = "abcdefghijklmnopqrstuvwxyz";
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
-    for (int j = 0; j < FILES; j++) {
-        sprintf(path, "%c", alphas[j]);
-        lfs_file_open(&lfs, &file, path,
-                LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => 0;
-        for (int i = 0; i < SIZE; i++) {
-            lfs_file_write(&lfs, &file, &alphas[j], 1) => 1;
-        }
-        lfs_file_close(&lfs, &file);
-    }
-    lfs_unmount(&lfs) => 0;
+[cases.test_orphans_one_orphan]
+in = 'lfs.c'
+code = '''
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
-    lfs_file_open(&lfs, &file, "zzz", LFS_O_WRONLY | LFS_O_CREAT) => 0;
-    for (int j = 0; j < FILES; j++) {
-        lfs_file_write(&lfs, &file, (const void*)"~", 1) => 1;
-        lfs_file_sync(&lfs, &file) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    // create an orphan
+    lfs_mdir_t orphan;
+    lfs_alloc_ack(&lfs);
+    lfs_dir_alloc(&lfs, &orphan) => 0;
+    lfs_dir_commit(&lfs, &orphan, NULL, 0) => 0;
+
+    // append our orphan and mark the filesystem as having orphans
+    lfs_fs_preporphans(&lfs, +1) => 0;
+    lfs_mdir_t mdir;
+    lfs_dir_fetch(&lfs, &mdir, (lfs_block_t[2]){0, 1}) => 0;
+    lfs_pair_tole32(orphan.pair);
+    lfs_dir_commit(&lfs, &mdir, LFS_MKATTRS(
+            {LFS_MKTAG(LFS_TYPE_SOFTTAIL, 0x3ff, 8), orphan.pair})) => 0;
 
-        sprintf(path, "%c", alphas[j]);
-        lfs_remove(&lfs, path) => 0;
-    }
-    lfs_file_close(&lfs, &file);
+    // we should have orphans at this state
+    assert(lfs_gstate_hasorphans(&lfs.gstate));
+    lfs_unmount(&lfs) => 0;
 
-    lfs_dir_open(&lfs, &dir, "/") => 0;
-    lfs_dir_read(&lfs, &dir, &info) => 1;
-    assert(strcmp(info.name, ".") == 0);
-    assert(info.type == LFS_TYPE_DIR);
-    lfs_dir_read(&lfs, &dir, &info) => 1;
-    assert(strcmp(info.name, "..") == 0);
-    assert(info.type == LFS_TYPE_DIR);
-    lfs_dir_read(&lfs, &dir, &info) => 1;
-    assert(strcmp(info.name, "zzz") == 0);
-    assert(info.type == LFS_TYPE_REG);
-    assert(info.size == FILES);
-    lfs_dir_read(&lfs, &dir, &info) => 0;
-    lfs_dir_close(&lfs, &dir) => 0;
+    // mount
+    lfs_mount(&lfs, cfg) => 0;
+    // we should detect orphans
+    assert(lfs_gstate_hasorphans(&lfs.gstate));
+    // force consistency
+    lfs_fs_forceconsistency(&lfs) => 0;
+    // we should no longer have orphans
+    assert(!lfs_gstate_hasorphans(&lfs.gstate));
 
-    lfs_file_open(&lfs, &file, "zzz", LFS_O_RDONLY) => 0;
-    for (int i = 0; i < FILES; i++) {
-        lfs_file_read(&lfs, &file, buffer, 1) => 1;
-        assert(buffer[0] == '~');
-    }
-    lfs_file_close(&lfs, &file);
-    
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # remove inconveniently test
-define.SIZE = [10, 100]
+# test that we can persist gstate with lfs_fs_mkconsistent
+[cases.test_orphans_mkconsistent_no_orphans]
+in = 'lfs.c'
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
-    lfs_file_t files[3];
-    lfs_file_open(&lfs, &files[0], "e", LFS_O_WRONLY | LFS_O_CREAT) => 0;
-    lfs_file_open(&lfs, &files[1], "f", LFS_O_WRONLY | LFS_O_CREAT) => 0;
-    lfs_file_open(&lfs, &files[2], "g", LFS_O_WRONLY | LFS_O_CREAT) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 
-    for (int i = 0; i < SIZE/2; i++) {
-        lfs_file_write(&lfs, &files[0], (const void*)"e", 1) => 1;
-        lfs_file_write(&lfs, &files[1], (const void*)"f", 1) => 1;
-        lfs_file_write(&lfs, &files[2], (const void*)"g", 1) => 1;
-    }
+    lfs_mount(&lfs, cfg) => 0;
+    // mark the filesystem as having orphans
+    lfs_fs_preporphans(&lfs, +1) => 0;
+    lfs_mdir_t mdir;
+    lfs_dir_fetch(&lfs, &mdir, (lfs_block_t[2]){0, 1}) => 0;
+    lfs_dir_commit(&lfs, &mdir, NULL, 0) => 0;
 
-    lfs_remove(&lfs, "f") => 0;
+    // we should have orphans at this state
+    assert(lfs_gstate_hasorphans(&lfs.gstate));
+    lfs_unmount(&lfs) => 0;
 
-    for (int i = 0; i < SIZE/2; i++) {
-        lfs_file_write(&lfs, &files[0], (const void*)"e", 1) => 1;
-        lfs_file_write(&lfs, &files[1], (const void*)"f", 1) => 1;
-        lfs_file_write(&lfs, &files[2], (const void*)"g", 1) => 1;
-    }
+    // mount
+    lfs_mount(&lfs, cfg) => 0;
+    // we should detect orphans
+    assert(lfs_gstate_hasorphans(&lfs.gstate));
+    // force consistency
+    lfs_fs_mkconsistent(&lfs) => 0;
+    // we should no longer have orphans
+    assert(!lfs_gstate_hasorphans(&lfs.gstate));
 
-    lfs_file_close(&lfs, &files[0]);
-    lfs_file_close(&lfs, &files[1]);
-    lfs_file_close(&lfs, &files[2]);
-
-    lfs_dir_open(&lfs, &dir, "/") => 0;
-    lfs_dir_read(&lfs, &dir, &info) => 1;
-    assert(strcmp(info.name, ".") == 0);
-    assert(info.type == LFS_TYPE_DIR);
-    lfs_dir_read(&lfs, &dir, &info) => 1;
-    assert(strcmp(info.name, "..") == 0);
-    assert(info.type == LFS_TYPE_DIR);
-    lfs_dir_read(&lfs, &dir, &info) => 1;
-    assert(strcmp(info.name, "e") == 0);
-    assert(info.type == LFS_TYPE_REG);
-    assert(info.size == SIZE);
-    lfs_dir_read(&lfs, &dir, &info) => 1;
-    assert(strcmp(info.name, "g") == 0);
-    assert(info.type == LFS_TYPE_REG);
-    assert(info.size == SIZE);
-    lfs_dir_read(&lfs, &dir, &info) => 0;
-    lfs_dir_close(&lfs, &dir) => 0;
+    // remount
+    lfs_unmount(&lfs) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    // we should still have no orphans
+    assert(!lfs_gstate_hasorphans(&lfs.gstate));
+    lfs_unmount(&lfs) => 0;
+'''
 
-    lfs_file_open(&lfs, &files[0], "e", LFS_O_RDONLY) => 0;
-    lfs_file_open(&lfs, &files[1], "g", LFS_O_RDONLY) => 0;
-    for (int i = 0; i < SIZE; i++) {
-        lfs_file_read(&lfs, &files[0], buffer, 1) => 1;
-        assert(buffer[0] == 'e');
-        lfs_file_read(&lfs, &files[1], buffer, 1) => 1;
-        assert(buffer[0] == 'g');
-    }
-    lfs_file_close(&lfs, &files[0]);
-    lfs_file_close(&lfs, &files[1]);
-    
+[cases.test_orphans_mkconsistent_one_orphan]
+in = 'lfs.c'
+code = '''
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+
+    lfs_mount(&lfs, cfg) => 0;
+    // create an orphan
+    lfs_mdir_t orphan;
+    lfs_alloc_ack(&lfs);
+    lfs_dir_alloc(&lfs, &orphan) => 0;
+    lfs_dir_commit(&lfs, &orphan, NULL, 0) => 0;
+
+    // append our orphan and mark the filesystem as having orphans
+    lfs_fs_preporphans(&lfs, +1) => 0;
+    lfs_mdir_t mdir;
+    lfs_dir_fetch(&lfs, &mdir, (lfs_block_t[2]){0, 1}) => 0;
+    lfs_pair_tole32(orphan.pair);
+    lfs_dir_commit(&lfs, &mdir, LFS_MKATTRS(
+            {LFS_MKTAG(LFS_TYPE_SOFTTAIL, 0x3ff, 8), orphan.pair})) => 0;
+
+    // we should have orphans at this state
+    assert(lfs_gstate_hasorphans(&lfs.gstate));
+    lfs_unmount(&lfs) => 0;
+
+    // mount
+    lfs_mount(&lfs, cfg) => 0;
+    // we should detect orphans
+    assert(lfs_gstate_hasorphans(&lfs.gstate));
+    // force consistency
+    lfs_fs_mkconsistent(&lfs) => 0;
+    // we should no longer have orphans
+    assert(!lfs_gstate_hasorphans(&lfs.gstate));
+
+    // remount
+    lfs_unmount(&lfs) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    // we should still have no orphans
+    assert(!lfs_gstate_hasorphans(&lfs.gstate));
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # reentrant interspersed file test
-define.SIZE = [10, 100]
-define.FILES = [4, 10, 26] 
+# reentrant testing for orphans, basically just spam mkdir/remove
+[cases.test_orphans_reentrant]
 reentrant = true
+# TODO fix this case, caused by non-DAG trees
+if = '!(DEPTH == 3 && CACHE_SIZE != 64)'
+defines = [
+    {FILES=6,  DEPTH=1, CYCLES=20},
+    {FILES=26, DEPTH=1, CYCLES=20},
+    {FILES=3,  DEPTH=3, CYCLES=20},
+]
 code = '''
-    lfs_file_t files[FILES];
-    const char alphas[] = "abcdefghijklmnopqrstuvwxyz";
-
-    err = lfs_mount(&lfs, &cfg);
+    lfs_t lfs;
+    int err = lfs_mount(&lfs, cfg);
     if (err) {
-        lfs_format(&lfs, &cfg) => 0;
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_format(&lfs, cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
     }
 
-    for (int j = 0; j < FILES; j++) {
-        sprintf(path, "%c", alphas[j]);
-        lfs_file_open(&lfs, &files[j], path,
-                LFS_O_WRONLY | LFS_O_CREAT | LFS_O_APPEND) => 0;
-    }
-
-    for (int i = 0; i < SIZE; i++) {
-        for (int j = 0; j < FILES; j++) {
-            size = lfs_file_size(&lfs, &files[j]);
-            assert((int)size >= 0);
-            if ((int)size <= i) {
-                lfs_file_write(&lfs, &files[j], &alphas[j], 1) => 1;
-                lfs_file_sync(&lfs, &files[j]) => 0;
-            }
+    uint32_t prng = 1;
+    const char alpha[] = "abcdefghijklmnopqrstuvwxyz";
+    for (unsigned i = 0; i < CYCLES; i++) {
+        // create random path
+        char full_path[256];
+        for (unsigned d = 0; d < DEPTH; d++) {
+            sprintf(&full_path[2*d], "/%c", alpha[TEST_PRNG(&prng) % FILES]);
         }
-    }
 
-    for (int j = 0; j < FILES; j++) {
-        lfs_file_close(&lfs, &files[j]);
-    }
-
-    lfs_dir_open(&lfs, &dir, "/") => 0;
-    lfs_dir_read(&lfs, &dir, &info) => 1;
-    assert(strcmp(info.name, ".") == 0);
-    assert(info.type == LFS_TYPE_DIR);
-    lfs_dir_read(&lfs, &dir, &info) => 1;
-    assert(strcmp(info.name, "..") == 0);
-    assert(info.type == LFS_TYPE_DIR);
-    for (int j = 0; j < FILES; j++) {
-        sprintf(path, "%c", alphas[j]);
-        lfs_dir_read(&lfs, &dir, &info) => 1;
-        assert(strcmp(info.name, path) == 0);
-        assert(info.type == LFS_TYPE_REG);
-        assert(info.size == SIZE);
-    }
-    lfs_dir_read(&lfs, &dir, &info) => 0;
-    lfs_dir_close(&lfs, &dir) => 0;
+        // if it does not exist, we create it, else we destroy
+        struct lfs_info info;
+        int res = lfs_stat(&lfs, full_path, &info);
+        if (res == LFS_ERR_NOENT) {
+            // create each directory in turn, ignore if dir already exists
+            for (unsigned d = 0; d < DEPTH; d++) {
+                char path[1024];
+                strcpy(path, full_path);
+                path[2*d+2] = '\0';
+                err = lfs_mkdir(&lfs, path);
+                assert(!err || err == LFS_ERR_EXIST);
+            }
 
-    for (int j = 0; j < FILES; j++) {
-        sprintf(path, "%c", alphas[j]);
-        lfs_file_open(&lfs, &files[j], path, LFS_O_RDONLY) => 0;
-    }
+            for (unsigned d = 0; d < DEPTH; d++) {
+                char path[1024];
+                strcpy(path, full_path);
+                path[2*d+2] = '\0';
+                lfs_stat(&lfs, path, &info) => 0;
+                assert(strcmp(info.name, &path[2*d+1]) == 0);
+                assert(info.type == LFS_TYPE_DIR);
+            }
+        } else {
+            // is valid dir?
+            assert(strcmp(info.name, &full_path[2*(DEPTH-1)+1]) == 0);
+            assert(info.type == LFS_TYPE_DIR);
+
+            // try to delete path in reverse order, ignore if dir is not empty
+            for (int d = DEPTH-1; d >= 0; d--) {
+                char path[1024];
+                strcpy(path, full_path);
+                path[2*d+2] = '\0';
+                err = lfs_remove(&lfs, path);
+                assert(!err || err == LFS_ERR_NOTEMPTY);
+            }
 
-    for (int i = 0; i < 10; i++) {
-        for (int j = 0; j < FILES; j++) {
-            lfs_file_read(&lfs, &files[j], buffer, 1) => 1;
-            assert(buffer[0] == alphas[j]);
+            lfs_stat(&lfs, full_path, &info) => LFS_ERR_NOENT;
         }
     }
-
-    for (int j = 0; j < FILES; j++) {
-        lfs_file_close(&lfs, &files[j]);
-    }
-    
     lfs_unmount(&lfs) => 0;
 '''
+
```

### Comparing `littlefs-python-0.4.0/littlefs/tests/test_move.toml` & `littlefs-python-0.5.0/littlefs/tests/test_move.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-[[case]] # move file
+[cases.test_move_file]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "a") => 0;
     lfs_mkdir(&lfs, "b") => 0;
     lfs_mkdir(&lfs, "c") => 0;
     lfs_mkdir(&lfs, "d") => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "a/hello", LFS_O_CREAT | LFS_O_WRONLY) => 0;
     lfs_file_write(&lfs, &file, "hola\n", 5) => 5;
     lfs_file_write(&lfs, &file, "bonjour\n", 8) => 8;
     lfs_file_write(&lfs, &file, "ohayo\n", 6) => 6;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_rename(&lfs, "a/hello", "c/hello") => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
+    struct lfs_info info;
     lfs_dir_open(&lfs, &dir, "a") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, ".") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "..") == 0);
     assert(info.type == LFS_TYPE_DIR);
@@ -40,79 +44,86 @@
     assert(info.size == 5+8+6);
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
 
     lfs_file_open(&lfs, &file, "a/hello", LFS_O_RDONLY) => LFS_ERR_NOENT;
     lfs_file_open(&lfs, &file, "b/hello", LFS_O_RDONLY) => LFS_ERR_NOENT;
     lfs_file_open(&lfs, &file, "c/hello", LFS_O_RDONLY) => 0;
+    uint8_t buffer[1024];
     lfs_file_read(&lfs, &file, buffer, 5) => 5;
     memcmp(buffer, "hola\n", 5) => 0;
     lfs_file_read(&lfs, &file, buffer, 8) => 8;
     memcmp(buffer, "bonjour\n", 8) => 0;
     lfs_file_read(&lfs, &file, buffer, 6) => 6;
     memcmp(buffer, "ohayo\n", 6) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_file_open(&lfs, &file, "d/hello", LFS_O_RDONLY) => LFS_ERR_NOENT;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # noop move, yes this is legal
+[cases.test_move_nop] # yes this is legal
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "hi") => 0;
     lfs_rename(&lfs, "hi", "hi") => 0;
     lfs_mkdir(&lfs, "hi/hi") => 0;
     lfs_rename(&lfs, "hi/hi", "hi/hi") => 0;
     lfs_mkdir(&lfs, "hi/hi/hi") => 0;
     lfs_rename(&lfs, "hi/hi/hi", "hi/hi/hi") => 0;
+    struct lfs_info info;
     lfs_stat(&lfs, "hi/hi/hi", &info) => 0;
     assert(strcmp(info.name, "hi") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # move file corrupt source
+[cases.test_move_file_corrupt_source]
 in = "lfs.c"
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "a") => 0;
     lfs_mkdir(&lfs, "b") => 0;
     lfs_mkdir(&lfs, "c") => 0;
     lfs_mkdir(&lfs, "d") => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "a/hello", LFS_O_CREAT | LFS_O_WRONLY) => 0;
     lfs_file_write(&lfs, &file, "hola\n", 5) => 5;
     lfs_file_write(&lfs, &file, "bonjour\n", 8) => 8;
     lfs_file_write(&lfs, &file, "ohayo\n", 6) => 6;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_rename(&lfs, "a/hello", "c/hello") => 0;
     lfs_unmount(&lfs) => 0;
 
     // corrupt the source
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
+    struct lfs_info info;
     lfs_dir_open(&lfs, &dir, "a") => 0;
     lfs_block_t block = dir.m.pair[0];
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
-    uint8_t bbuffer[LFS_BLOCK_SIZE];
-    cfg.read(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    int off = LFS_BLOCK_SIZE-1;
-    while (off >= 0 && bbuffer[off] == LFS_ERASE_VALUE) {
+    uint8_t buffer[BLOCK_SIZE];
+    cfg->read(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    int off = BLOCK_SIZE-1;
+    while (off >= 0 && buffer[off] == ERASE_VALUE) {
         off -= 1;
     }
-    memset(&bbuffer[off-3], LFS_BLOCK_SIZE, 3);
-    cfg.erase(&cfg, block) => 0;
-    cfg.prog(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    cfg.sync(&cfg) => 0;
+    memset(&buffer[off-3], BLOCK_SIZE, 3);
+    cfg->erase(cfg, block) => 0;
+    cfg->prog(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    cfg->sync(cfg) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_dir_open(&lfs, &dir, "a") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, ".") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "..") == 0);
     assert(info.type == LFS_TYPE_DIR);
@@ -142,69 +153,74 @@
     lfs_file_read(&lfs, &file, buffer, 6) => 6;
     memcmp(buffer, "ohayo\n", 6) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_file_open(&lfs, &file, "d/hello", LFS_O_RDONLY) => LFS_ERR_NOENT;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # move file corrupt source and dest
+# move file corrupt source and dest
+[cases.test_move_file_corrupt_source_dest]
 in = "lfs.c"
-if = 'LFS_PROG_SIZE <= 0x3fe' # only works with one crc per commit
+if = 'PROG_SIZE <= 0x3fe' # only works with one crc per commit
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "a") => 0;
     lfs_mkdir(&lfs, "b") => 0;
     lfs_mkdir(&lfs, "c") => 0;
     lfs_mkdir(&lfs, "d") => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "a/hello", LFS_O_CREAT | LFS_O_WRONLY) => 0;
     lfs_file_write(&lfs, &file, "hola\n", 5) => 5;
     lfs_file_write(&lfs, &file, "bonjour\n", 8) => 8;
     lfs_file_write(&lfs, &file, "ohayo\n", 6) => 6;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_rename(&lfs, "a/hello", "c/hello") => 0;
     lfs_unmount(&lfs) => 0;
 
     // corrupt the source
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
+    struct lfs_info info;
     lfs_dir_open(&lfs, &dir, "a") => 0;
     lfs_block_t block = dir.m.pair[0];
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
-    uint8_t bbuffer[LFS_BLOCK_SIZE];
-    cfg.read(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    int off = LFS_BLOCK_SIZE-1;
-    while (off >= 0 && bbuffer[off] == LFS_ERASE_VALUE) {
+    uint8_t buffer[BLOCK_SIZE];
+    cfg->read(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    int off = BLOCK_SIZE-1;
+    while (off >= 0 && buffer[off] == ERASE_VALUE) {
         off -= 1;
     }
-    memset(&bbuffer[off-3], LFS_BLOCK_SIZE, 3);
-    cfg.erase(&cfg, block) => 0;
-    cfg.prog(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    cfg.sync(&cfg) => 0;
+    memset(&buffer[off-3], BLOCK_SIZE, 3);
+    cfg->erase(cfg, block) => 0;
+    cfg->prog(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    cfg->sync(cfg) => 0;
 
     // corrupt the destination
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_dir_open(&lfs, &dir, "c") => 0;
     block = dir.m.pair[0];
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
-    cfg.read(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    off = LFS_BLOCK_SIZE-1;
-    while (off >= 0 && bbuffer[off] == LFS_ERASE_VALUE) {
+    cfg->read(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    off = BLOCK_SIZE-1;
+    while (off >= 0 && buffer[off] == ERASE_VALUE) {
         off -= 1;
     }
-    memset(&bbuffer[off-3], LFS_BLOCK_SIZE, 3);
-    cfg.erase(&cfg, block) => 0;
-    cfg.prog(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    cfg.sync(&cfg) => 0;
+    memset(&buffer[off-3], BLOCK_SIZE, 3);
+    cfg->erase(cfg, block) => 0;
+    cfg->prog(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    cfg->sync(cfg) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_dir_open(&lfs, &dir, "a") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, ".") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "..") == 0);
     assert(info.type == LFS_TYPE_DIR);
@@ -234,74 +250,78 @@
     lfs_file_close(&lfs, &file) => 0;
     lfs_file_open(&lfs, &file, "b/hello", LFS_O_RDONLY) => LFS_ERR_NOENT;
     lfs_file_open(&lfs, &file, "c/hello", LFS_O_RDONLY) => LFS_ERR_NOENT;
     lfs_file_open(&lfs, &file, "d/hello", LFS_O_RDONLY) => LFS_ERR_NOENT;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # move file after corrupt
+[cases.test_move_file_after_corrupt]
 in = "lfs.c"
-if = 'LFS_PROG_SIZE <= 0x3fe' # only works with one crc per commit
+if = 'PROG_SIZE <= 0x3fe' # only works with one crc per commit
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "a") => 0;
     lfs_mkdir(&lfs, "b") => 0;
     lfs_mkdir(&lfs, "c") => 0;
     lfs_mkdir(&lfs, "d") => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "a/hello", LFS_O_CREAT | LFS_O_WRONLY) => 0;
     lfs_file_write(&lfs, &file, "hola\n", 5) => 5;
     lfs_file_write(&lfs, &file, "bonjour\n", 8) => 8;
     lfs_file_write(&lfs, &file, "ohayo\n", 6) => 6;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_rename(&lfs, "a/hello", "c/hello") => 0;
     lfs_unmount(&lfs) => 0;
 
     // corrupt the source
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
+    struct lfs_info info;
     lfs_dir_open(&lfs, &dir, "a") => 0;
     lfs_block_t block = dir.m.pair[0];
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
-    uint8_t bbuffer[LFS_BLOCK_SIZE];
-    cfg.read(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    int off = LFS_BLOCK_SIZE-1;
-    while (off >= 0 && bbuffer[off] == LFS_ERASE_VALUE) {
+    uint8_t buffer[BLOCK_SIZE];
+    cfg->read(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    int off = BLOCK_SIZE-1;
+    while (off >= 0 && buffer[off] == ERASE_VALUE) {
         off -= 1;
     }
-    memset(&bbuffer[off-3], LFS_BLOCK_SIZE, 3);
-    cfg.erase(&cfg, block) => 0;
-    cfg.prog(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    cfg.sync(&cfg) => 0;
+    memset(&buffer[off-3], BLOCK_SIZE, 3);
+    cfg->erase(cfg, block) => 0;
+    cfg->prog(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    cfg->sync(cfg) => 0;
 
     // corrupt the destination
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_dir_open(&lfs, &dir, "c") => 0;
     block = dir.m.pair[0];
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
-    cfg.read(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    off = LFS_BLOCK_SIZE-1;
-    while (off >= 0 && bbuffer[off] == LFS_ERASE_VALUE) {
+    cfg->read(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    off = BLOCK_SIZE-1;
+    while (off >= 0 && buffer[off] == ERASE_VALUE) {
         off -= 1;
     }
-    memset(&bbuffer[off-3], LFS_BLOCK_SIZE, 3);
-    cfg.erase(&cfg, block) => 0;
-    cfg.prog(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    cfg.sync(&cfg) => 0;
+    memset(&buffer[off-3], BLOCK_SIZE, 3);
+    cfg->erase(cfg, block) => 0;
+    cfg->prog(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    cfg->sync(cfg) => 0;
 
     // continue move
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_rename(&lfs, "a/hello", "c/hello") => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_dir_open(&lfs, &dir, "a") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, ".") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "..") == 0);
     assert(info.type == LFS_TYPE_DIR);
@@ -331,36 +351,38 @@
     lfs_file_read(&lfs, &file, buffer, 6) => 6;
     memcmp(buffer, "ohayo\n", 6) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_file_open(&lfs, &file, "d/hello", LFS_O_RDONLY) => LFS_ERR_NOENT;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # simple reentrant move file
+[cases.test_move_reentrant_file]
 reentrant = true
 code = '''
-    err = lfs_mount(&lfs, &cfg);
+    lfs_t lfs;
+    int err = lfs_mount(&lfs, cfg);
     if (err) {
-        lfs_format(&lfs, &cfg) => 0;
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_format(&lfs, cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
     }
     err = lfs_mkdir(&lfs, "a");
     assert(!err || err == LFS_ERR_EXIST);
     err = lfs_mkdir(&lfs, "b");
     assert(!err || err == LFS_ERR_EXIST);
     err = lfs_mkdir(&lfs, "c");
     assert(!err || err == LFS_ERR_EXIST);
     err = lfs_mkdir(&lfs, "d");
     assert(!err || err == LFS_ERR_EXIST);
     lfs_unmount(&lfs) => 0;
 
     while (true) {
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         // there should never exist _2_ hello files
         int count = 0;
+        struct lfs_info info;
         if (lfs_stat(&lfs, "a/hello", &info) == 0) {
             assert(strcmp(info.name, "hello") == 0);
             assert(info.type == LFS_TYPE_REG);
             assert(info.size == 5+8+6 || info.size == 0);
             count += 1;
         }
         if (lfs_stat(&lfs, "b/hello", &info) == 0) {
@@ -380,38 +402,41 @@
             assert(info.type == LFS_TYPE_REG);
             assert(info.size == 5+8+6);
             count += 1;
         }
         assert(count <= 1);
         lfs_unmount(&lfs) => 0;
 
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         if (lfs_stat(&lfs, "a/hello", &info) == 0 && info.size > 0) {
             lfs_rename(&lfs, "a/hello", "b/hello") => 0;
         } else if (lfs_stat(&lfs, "b/hello", &info) == 0) {
             lfs_rename(&lfs, "b/hello", "c/hello") => 0;
         } else if (lfs_stat(&lfs, "c/hello", &info) == 0) {
             lfs_rename(&lfs, "c/hello", "d/hello") => 0;
         } else if (lfs_stat(&lfs, "d/hello", &info) == 0) {
             // success
             lfs_unmount(&lfs) => 0;
             break;
         } else {
             // create file
+            lfs_file_t file;
             lfs_file_open(&lfs, &file, "a/hello",
                     LFS_O_WRONLY | LFS_O_CREAT) => 0;
             lfs_file_write(&lfs, &file, "hola\n", 5) => 5;
             lfs_file_write(&lfs, &file, "bonjour\n", 8) => 8;
             lfs_file_write(&lfs, &file, "ohayo\n", 6) => 6;
             lfs_file_close(&lfs, &file) => 0;
         }
         lfs_unmount(&lfs) => 0;
     }
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
+    struct lfs_info info;
     lfs_dir_open(&lfs, &dir, "a") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, ".") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "..") == 0);
     assert(info.type == LFS_TYPE_DIR);
@@ -427,47 +452,52 @@
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "hello") == 0);
     assert(info.type == LFS_TYPE_REG);
     assert(info.size == 5+8+6);
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
 
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "a/hello", LFS_O_RDONLY) => LFS_ERR_NOENT;
     lfs_file_open(&lfs, &file, "b/hello", LFS_O_RDONLY) => LFS_ERR_NOENT;
     lfs_file_open(&lfs, &file, "c/hello", LFS_O_RDONLY) => LFS_ERR_NOENT;
     lfs_file_open(&lfs, &file, "d/hello", LFS_O_RDONLY) => 0;
+    uint8_t buffer[1024];
     lfs_file_read(&lfs, &file, buffer, 5) => 5;
     memcmp(buffer, "hola\n", 5) => 0;
     lfs_file_read(&lfs, &file, buffer, 8) => 8;
     memcmp(buffer, "bonjour\n", 8) => 0;
     lfs_file_read(&lfs, &file, buffer, 6) => 6;
     memcmp(buffer, "ohayo\n", 6) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # move dir
+[cases.test_move_dir]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "a") => 0;
     lfs_mkdir(&lfs, "b") => 0;
     lfs_mkdir(&lfs, "c") => 0;
     lfs_mkdir(&lfs, "d") => 0;
     lfs_mkdir(&lfs, "a/hi") => 0;
     lfs_mkdir(&lfs, "a/hi/hola") => 0;
     lfs_mkdir(&lfs, "a/hi/bonjour") => 0;
     lfs_mkdir(&lfs, "a/hi/ohayo") => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_rename(&lfs, "a/hi", "c/hi") => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
+    struct lfs_info info;
     lfs_dir_open(&lfs, &dir, "a") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, ".") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "..") == 0);
     assert(info.type == LFS_TYPE_DIR);
@@ -506,51 +536,54 @@
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_dir_open(&lfs, &dir, "d/hi") => LFS_ERR_NOENT;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # move dir corrupt source
+[cases.test_move_dir_corrupt_source]
 in = "lfs.c"
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "a") => 0;
     lfs_mkdir(&lfs, "b") => 0;
     lfs_mkdir(&lfs, "c") => 0;
     lfs_mkdir(&lfs, "d") => 0;
     lfs_mkdir(&lfs, "a/hi") => 0;
     lfs_mkdir(&lfs, "a/hi/hola") => 0;
     lfs_mkdir(&lfs, "a/hi/bonjour") => 0;
     lfs_mkdir(&lfs, "a/hi/ohayo") => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_rename(&lfs, "a/hi", "c/hi") => 0;
     lfs_unmount(&lfs) => 0;
 
     // corrupt the source
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
+    struct lfs_info info;
     lfs_dir_open(&lfs, &dir, "a") => 0;
     lfs_block_t block = dir.m.pair[0];
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
-    uint8_t bbuffer[LFS_BLOCK_SIZE];
-    cfg.read(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    int off = LFS_BLOCK_SIZE-1;
-    while (off >= 0 && bbuffer[off] == LFS_ERASE_VALUE) {
+    uint8_t buffer[BLOCK_SIZE];
+    cfg->read(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    int off = BLOCK_SIZE-1;
+    while (off >= 0 && buffer[off] == ERASE_VALUE) {
         off -= 1;
     }
-    memset(&bbuffer[off-3], LFS_BLOCK_SIZE, 3);
-    cfg.erase(&cfg, block) => 0;
-    cfg.prog(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    cfg.sync(&cfg) => 0;
+    memset(&buffer[off-3], BLOCK_SIZE, 3);
+    cfg->erase(cfg, block) => 0;
+    cfg->prog(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    cfg->sync(cfg) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_dir_open(&lfs, &dir, "a") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, ".") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "..") == 0);
     assert(info.type == LFS_TYPE_DIR);
@@ -589,68 +622,71 @@
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_dir_open(&lfs, &dir, "d/hi") => LFS_ERR_NOENT;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # move dir corrupt source and dest
+[cases.test_move_dir_corrupt_source_dest]
 in = "lfs.c"
-if = 'LFS_PROG_SIZE <= 0x3fe' # only works with one crc per commit
+if = 'PROG_SIZE <= 0x3fe' # only works with one crc per commit
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "a") => 0;
     lfs_mkdir(&lfs, "b") => 0;
     lfs_mkdir(&lfs, "c") => 0;
     lfs_mkdir(&lfs, "d") => 0;
     lfs_mkdir(&lfs, "a/hi") => 0;
     lfs_mkdir(&lfs, "a/hi/hola") => 0;
     lfs_mkdir(&lfs, "a/hi/bonjour") => 0;
     lfs_mkdir(&lfs, "a/hi/ohayo") => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_rename(&lfs, "a/hi", "c/hi") => 0;
     lfs_unmount(&lfs) => 0;
 
     // corrupt the source
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
+    struct lfs_info info;
     lfs_dir_open(&lfs, &dir, "a") => 0;
     lfs_block_t block = dir.m.pair[0];
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
-    uint8_t bbuffer[LFS_BLOCK_SIZE];
-    cfg.read(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    int off = LFS_BLOCK_SIZE-1;
-    while (off >= 0 && bbuffer[off] == LFS_ERASE_VALUE) {
+    uint8_t buffer[BLOCK_SIZE];
+    cfg->read(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    int off = BLOCK_SIZE-1;
+    while (off >= 0 && buffer[off] == ERASE_VALUE) {
         off -= 1;
     }
-    memset(&bbuffer[off-3], LFS_BLOCK_SIZE, 3);
-    cfg.erase(&cfg, block) => 0;
-    cfg.prog(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    cfg.sync(&cfg) => 0;
+    memset(&buffer[off-3], BLOCK_SIZE, 3);
+    cfg->erase(cfg, block) => 0;
+    cfg->prog(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    cfg->sync(cfg) => 0;
 
     // corrupt the destination
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_dir_open(&lfs, &dir, "c") => 0;
     block = dir.m.pair[0];
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
-    cfg.read(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    off = LFS_BLOCK_SIZE-1;
-    while (off >= 0 && bbuffer[off] == LFS_ERASE_VALUE) {
+    cfg->read(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    off = BLOCK_SIZE-1;
+    while (off >= 0 && buffer[off] == ERASE_VALUE) {
         off -= 1;
     }
-    memset(&bbuffer[off-3], LFS_BLOCK_SIZE, 3);
-    cfg.erase(&cfg, block) => 0;
-    cfg.prog(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    cfg.sync(&cfg) => 0;
+    memset(&buffer[off-3], BLOCK_SIZE, 3);
+    cfg->erase(cfg, block) => 0;
+    cfg->prog(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    cfg->sync(cfg) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_dir_open(&lfs, &dir, "a") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, ".") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "..") == 0);
     assert(info.type == LFS_TYPE_DIR);
@@ -689,73 +725,76 @@
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_dir_open(&lfs, &dir, "b/hi") => LFS_ERR_NOENT;
     lfs_dir_open(&lfs, &dir, "c/hi") => LFS_ERR_NOENT;
     lfs_dir_open(&lfs, &dir, "d/hi") => LFS_ERR_NOENT;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # move dir after corrupt
+[cases.test_move_dir_after_corrupt]
 in = "lfs.c"
-if = 'LFS_PROG_SIZE <= 0x3fe' # only works with one crc per commit
+if = 'PROG_SIZE <= 0x3fe' # only works with one crc per commit
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "a") => 0;
     lfs_mkdir(&lfs, "b") => 0;
     lfs_mkdir(&lfs, "c") => 0;
     lfs_mkdir(&lfs, "d") => 0;
     lfs_mkdir(&lfs, "a/hi") => 0;
     lfs_mkdir(&lfs, "a/hi/hola") => 0;
     lfs_mkdir(&lfs, "a/hi/bonjour") => 0;
     lfs_mkdir(&lfs, "a/hi/ohayo") => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_rename(&lfs, "a/hi", "c/hi") => 0;
     lfs_unmount(&lfs) => 0;
 
     // corrupt the source
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
+    struct lfs_info info;
     lfs_dir_open(&lfs, &dir, "a") => 0;
     lfs_block_t block = dir.m.pair[0];
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
-    uint8_t bbuffer[LFS_BLOCK_SIZE];
-    cfg.read(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    int off = LFS_BLOCK_SIZE-1;
-    while (off >= 0 && bbuffer[off] == LFS_ERASE_VALUE) {
+    uint8_t buffer[BLOCK_SIZE];
+    cfg->read(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    int off = BLOCK_SIZE-1;
+    while (off >= 0 && buffer[off] == ERASE_VALUE) {
         off -= 1;
     }
-    memset(&bbuffer[off-3], LFS_BLOCK_SIZE, 3);
-    cfg.erase(&cfg, block) => 0;
-    cfg.prog(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    cfg.sync(&cfg) => 0;
+    memset(&buffer[off-3], BLOCK_SIZE, 3);
+    cfg->erase(cfg, block) => 0;
+    cfg->prog(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    cfg->sync(cfg) => 0;
 
     // corrupt the destination
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_dir_open(&lfs, &dir, "c") => 0;
     block = dir.m.pair[0];
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
-    cfg.read(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    off = LFS_BLOCK_SIZE-1;
-    while (off >= 0 && bbuffer[off] == LFS_ERASE_VALUE) {
+    cfg->read(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    off = BLOCK_SIZE-1;
+    while (off >= 0 && buffer[off] == ERASE_VALUE) {
         off -= 1;
     }
-    memset(&bbuffer[off-3], LFS_BLOCK_SIZE, 3);
-    cfg.erase(&cfg, block) => 0;
-    cfg.prog(&cfg, block, 0, bbuffer, LFS_BLOCK_SIZE) => 0;
-    cfg.sync(&cfg) => 0;
+    memset(&buffer[off-3], BLOCK_SIZE, 3);
+    cfg->erase(cfg, block) => 0;
+    cfg->prog(cfg, block, 0, buffer, BLOCK_SIZE) => 0;
+    cfg->sync(cfg) => 0;
 
     // continue move
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_rename(&lfs, "a/hi", "c/hi") => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_dir_open(&lfs, &dir, "a") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, ".") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "..") == 0);
     assert(info.type == LFS_TYPE_DIR);
@@ -794,36 +833,38 @@
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_dir_open(&lfs, &dir, "d/hi") => LFS_ERR_NOENT;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # simple reentrant move dir
+[cases.test_reentrant_dir]
 reentrant = true
 code = '''
-    err = lfs_mount(&lfs, &cfg);
+    lfs_t lfs;
+    int err = lfs_mount(&lfs, cfg);
     if (err) {
-        lfs_format(&lfs, &cfg) => 0;
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_format(&lfs, cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
     }
     err = lfs_mkdir(&lfs, "a");
     assert(!err || err == LFS_ERR_EXIST);
     err = lfs_mkdir(&lfs, "b");
     assert(!err || err == LFS_ERR_EXIST);
     err = lfs_mkdir(&lfs, "c");
     assert(!err || err == LFS_ERR_EXIST);
     err = lfs_mkdir(&lfs, "d");
     assert(!err || err == LFS_ERR_EXIST);
     lfs_unmount(&lfs) => 0;
 
     while (true) {
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         // there should never exist _2_ hi directories
         int count = 0;
+        struct lfs_info info;
         if (lfs_stat(&lfs, "a/hi", &info) == 0) {
             assert(strcmp(info.name, "hi") == 0);
             assert(info.type == LFS_TYPE_DIR);
             count += 1;
         }
         if (lfs_stat(&lfs, "b/hi", &info) == 0) {
             assert(strcmp(info.name, "hi") == 0);
@@ -839,15 +880,15 @@
             assert(strcmp(info.name, "hi") == 0);
             assert(info.type == LFS_TYPE_DIR);
             count += 1;
         }
         assert(count <= 1);
         lfs_unmount(&lfs) => 0;
 
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         if (lfs_stat(&lfs, "a/hi", &info) == 0) {
             lfs_rename(&lfs, "a/hi", "b/hi") => 0;
         } else if (lfs_stat(&lfs, "b/hi", &info) == 0) {
             lfs_rename(&lfs, "b/hi", "c/hi") => 0;
         } else if (lfs_stat(&lfs, "c/hi", &info) == 0) {
             lfs_rename(&lfs, "c/hi", "d/hi") => 0;
         } else if (lfs_stat(&lfs, "d/hi", &info) == 0) {
@@ -864,15 +905,17 @@
             err = lfs_mkdir(&lfs, "temp/ohayo");
             assert(!err || err == LFS_ERR_EXIST);
             lfs_rename(&lfs, "temp", "a/hi") => 0;
         }
         lfs_unmount(&lfs) => 0;
     }
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
+    struct lfs_info info;
     lfs_dir_open(&lfs, &dir, "a") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, ".") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "..") == 0);
     assert(info.type == LFS_TYPE_DIR);
@@ -911,59 +954,63 @@
     assert(strcmp(info.name, "ohayo") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # move state stealing
+[cases.test_move_state_stealing]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "a") => 0;
     lfs_mkdir(&lfs, "b") => 0;
     lfs_mkdir(&lfs, "c") => 0;
     lfs_mkdir(&lfs, "d") => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "a/hello", LFS_O_CREAT | LFS_O_WRONLY) => 0;
     lfs_file_write(&lfs, &file, "hola\n", 5) => 5;
     lfs_file_write(&lfs, &file, "bonjour\n", 8) => 8;
     lfs_file_write(&lfs, &file, "ohayo\n", 6) => 6;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_rename(&lfs, "a/hello", "b/hello") => 0;
     lfs_unmount(&lfs) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_rename(&lfs, "b/hello", "c/hello") => 0;
     lfs_unmount(&lfs) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_rename(&lfs, "c/hello", "d/hello") => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "a/hello", LFS_O_RDONLY) => LFS_ERR_NOENT;
     lfs_file_open(&lfs, &file, "b/hello", LFS_O_RDONLY) => LFS_ERR_NOENT;
     lfs_file_open(&lfs, &file, "c/hello", LFS_O_RDONLY) => LFS_ERR_NOENT;
     lfs_file_open(&lfs, &file, "d/hello", LFS_O_RDONLY) => 0;
+    uint8_t buffer[1024];
     lfs_file_read(&lfs, &file, buffer, 5) => 5;
     memcmp(buffer, "hola\n", 5) => 0;
     lfs_file_read(&lfs, &file, buffer, 8) => 8;
     memcmp(buffer, "bonjour\n", 8) => 0;
     lfs_file_read(&lfs, &file, buffer, 6) => 6;
     memcmp(buffer, "ohayo\n", 6) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_remove(&lfs, "b") => 0;
     lfs_remove(&lfs, "c") => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    struct lfs_info info;
     lfs_stat(&lfs, "a", &info) => 0;
     lfs_stat(&lfs, "b", &info) => LFS_ERR_NOENT;
     lfs_stat(&lfs, "c", &info) => LFS_ERR_NOENT;
     lfs_stat(&lfs, "d", &info) => 0;
     lfs_file_open(&lfs, &file, "a/hello", LFS_O_RDONLY) => LFS_ERR_NOENT;
     lfs_file_open(&lfs, &file, "b/hello", LFS_O_RDONLY) => LFS_ERR_NOENT;
     lfs_file_open(&lfs, &file, "c/hello", LFS_O_RDONLY) => LFS_ERR_NOENT;
@@ -975,20 +1022,24 @@
     lfs_file_read(&lfs, &file, buffer, 6) => 6;
     memcmp(buffer, "ohayo\n", 6) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
 # Other specific corner cases
-[[case]] # create + delete in same commit with neighbors
+
+# create + delete in same commit with neighbors
+[cases.test_move_create_delete_same]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     // littlefs keeps files sorted, so we know the order these will be in
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "/1.move_me",
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_file_open(&lfs, &file, "/0.before",
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
     lfs_file_write(&lfs, &file, "test.1", 7) => 7;
@@ -1020,14 +1071,16 @@
     lfs_rename(&lfs, "/1.move_me", "/3.move_me") => 0;
 
     lfs_file_close(&lfs, &files[0]) => 0;
     lfs_file_close(&lfs, &files[1]) => 0;
     lfs_file_close(&lfs, &files[2]) => 0;
 
     // check that nothing was corrupted
+    lfs_dir_t dir;
+    struct lfs_info info;
     lfs_dir_open(&lfs, &dir, "/") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, ".") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "..") == 0);
     assert(info.type == LFS_TYPE_DIR);
@@ -1047,14 +1100,15 @@
     assert(strcmp(info.name, "4.after") == 0);
     assert(info.type == LFS_TYPE_REG);
     assert(info.size == 7);
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
 
     lfs_file_open(&lfs, &file, "/0.before", LFS_O_RDONLY) => 0;
+    uint8_t buffer[1024];
     lfs_file_read(&lfs, &file, buffer, 7) => 7;
     assert(strcmp((char*)buffer, "test.4") == 0);
     lfs_file_close(&lfs, &file) => 0;
     lfs_file_open(&lfs, &file, "/2.in_between", LFS_O_RDONLY) => 0;
     lfs_file_read(&lfs, &file, buffer, 7) => 7;
     assert(strcmp((char*)buffer, "test.5") == 0);
     lfs_file_close(&lfs, &file) => 0;
@@ -1120,21 +1174,23 @@
     lfs_file_open(&lfs, &file, "/4.after", LFS_O_RDONLY) => 0;
     lfs_file_read(&lfs, &file, buffer, 7) => 7;
     assert(strcmp((char*)buffer, "test.9") == 0);
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-# Other specific corner cases
-[[case]] # create + delete + delete in same commit with neighbors
+# create + delete + delete in same commit with neighbors
+[cases.test_move_create_delete_delete_same]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     // littlefs keeps files sorted, so we know the order these will be in
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "/1.move_me",
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_file_open(&lfs, &file, "/3.move_me",
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
     lfs_file_write(&lfs, &file, "remove me",
             sizeof("remove me")) => sizeof("remove me");
@@ -1171,14 +1227,16 @@
     lfs_rename(&lfs, "/1.move_me", "/3.move_me") => 0;
 
     lfs_file_close(&lfs, &files[0]) => 0;
     lfs_file_close(&lfs, &files[1]) => 0;
     lfs_file_close(&lfs, &files[2]) => 0;
 
     // check that nothing was corrupted
+    lfs_dir_t dir;
+    struct lfs_info info;
     lfs_dir_open(&lfs, &dir, "/") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, ".") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "..") == 0);
     assert(info.type == LFS_TYPE_DIR);
@@ -1198,14 +1256,15 @@
     assert(strcmp(info.name, "4.after") == 0);
     assert(info.type == LFS_TYPE_REG);
     assert(info.size == 7);
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
 
     lfs_file_open(&lfs, &file, "/0.before", LFS_O_RDONLY) => 0;
+    uint8_t buffer[1024];
     lfs_file_read(&lfs, &file, buffer, 7) => 7;
     assert(strcmp((char*)buffer, "test.4") == 0);
     lfs_file_close(&lfs, &file) => 0;
     lfs_file_open(&lfs, &file, "/2.in_between", LFS_O_RDONLY) => 0;
     lfs_file_read(&lfs, &file, buffer, 7) => 7;
     assert(strcmp((char*)buffer, "test.5") == 0);
     lfs_file_close(&lfs, &file) => 0;
@@ -1277,22 +1336,25 @@
     lfs_file_open(&lfs, &file, "/4.after", LFS_O_RDONLY) => 0;
     lfs_file_read(&lfs, &file, buffer, 7) => 7;
     assert(strcmp((char*)buffer, "test.9") == 0);
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # create + delete in different dirs with neighbors
+# create + delete in different dirs with neighbors
+[cases.test_move_create_delete_different]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     // littlefs keeps files sorted, so we know the order these will be in
     lfs_mkdir(&lfs, "/dir.1") => 0;
     lfs_mkdir(&lfs, "/dir.2") => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "/dir.1/1.move_me",
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_file_open(&lfs, &file, "/dir.2/1.move_me",
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
     lfs_file_write(&lfs, &file, "remove me",
             sizeof("remove me")) => sizeof("remove me");
@@ -1336,14 +1398,16 @@
 
     lfs_file_close(&lfs, &files[0]) => 0;
     lfs_file_close(&lfs, &files[1]) => 0;
     lfs_file_close(&lfs, &files[2]) => 0;
     lfs_file_close(&lfs, &files[3]) => 0;
 
     // check that nothing was corrupted
+    lfs_dir_t dir;
+    struct lfs_info info;
     lfs_dir_open(&lfs, &dir, "/") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, ".") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "..") == 0);
     assert(info.type == LFS_TYPE_DIR);
@@ -1393,14 +1457,15 @@
     assert(strcmp(info.name, "2.after") == 0);
     assert(info.type == LFS_TYPE_REG);
     assert(info.size == 7);
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
 
     lfs_file_open(&lfs, &file, "/dir.1/0.before", LFS_O_RDONLY) => 0;
+    uint8_t buffer[1024];
     lfs_file_read(&lfs, &file, buffer, 7) => 7;
     assert(strcmp((char*)buffer, "test.5") == 0);
     lfs_file_close(&lfs, &file) => 0;
     lfs_file_open(&lfs, &file, "/dir.1/2.after", LFS_O_RDONLY) => 0;
     lfs_file_read(&lfs, &file, buffer, 7) => 7;
     assert(strcmp((char*)buffer, "test.6") == 0);
     lfs_file_close(&lfs, &file) => 0;
@@ -1514,25 +1579,28 @@
     lfs_file_open(&lfs, &file, "/dir.2/2.after", LFS_O_RDONLY) => 0;
     lfs_file_read(&lfs, &file, buffer, 7) => 7;
     assert(strcmp((char*)buffer, "test.c") == 0);
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # move fix in relocation
+# move fix in relocation
+[cases.test_move_fix_relocation]
 in = "lfs.c"
-define.RELOCATIONS = 'range(0x3+1)'
-define.LFS_ERASE_CYCLES = 0xffffffff
+defines.RELOCATIONS = 'range(4)'
+defines.ERASE_CYCLES = 0xffffffff
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     lfs_mkdir(&lfs, "/parent") => 0;
     lfs_mkdir(&lfs, "/parent/child") => 0;
 
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "/parent/1.move_me",
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
     lfs_file_write(&lfs, &file, "move me",
             sizeof("move me")) => sizeof("move me");
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_file_open(&lfs, &file, "/parent/0.before",
@@ -1564,23 +1632,25 @@
     lfs_file_write(&lfs, &files[0], "test.5", 7) => 7;
     lfs_file_write(&lfs, &files[1], "test.6", 7) => 7;
     lfs_file_write(&lfs, &files[2], "test.7", 7) => 7;
     lfs_file_write(&lfs, &files[3], "test.8", 7) => 7;
 
     // force specific directories to relocate
     if (RELOCATIONS & 0x1) {
+        lfs_dir_t dir;
         lfs_dir_open(&lfs, &dir, "/parent");
-        lfs_testbd_setwear(&cfg, dir.m.pair[0], 0xffffffff) => 0;
-        lfs_testbd_setwear(&cfg, dir.m.pair[1], 0xffffffff) => 0;
+        lfs_emubd_setwear(cfg, dir.m.pair[0], 0xffffffff) => 0;
+        lfs_emubd_setwear(cfg, dir.m.pair[1], 0xffffffff) => 0;
         lfs_dir_close(&lfs, &dir) => 0;
     }
     if (RELOCATIONS & 0x2) {
+        lfs_dir_t dir;
         lfs_dir_open(&lfs, &dir, "/parent/child");
-        lfs_testbd_setwear(&cfg, dir.m.pair[0], 0xffffffff) => 0;
-        lfs_testbd_setwear(&cfg, dir.m.pair[1], 0xffffffff) => 0;
+        lfs_emubd_setwear(cfg, dir.m.pair[0], 0xffffffff) => 0;
+        lfs_emubd_setwear(cfg, dir.m.pair[1], 0xffffffff) => 0;
         lfs_dir_close(&lfs, &dir) => 0;
     }
 
     // ok, now we move the file, this creates a move that needs to be
     // fixed, possibly in a metadata-pair that needs to be relocated
     //
     // the worst case is if we need to relocate and we need to implicit
@@ -1589,14 +1659,16 @@
 
     lfs_file_close(&lfs, &files[0]) => 0;
     lfs_file_close(&lfs, &files[1]) => 0;
     lfs_file_close(&lfs, &files[2]) => 0;
     lfs_file_close(&lfs, &files[3]) => 0;
 
     // check that nothing was corrupted
+    lfs_dir_t dir;
+    struct lfs_info info;
     lfs_dir_open(&lfs, &dir, "/parent") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, ".") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "..") == 0);
     assert(info.type == LFS_TYPE_DIR);
@@ -1633,14 +1705,15 @@
     assert(strcmp(info.name, "2.after") == 0);
     assert(info.type == LFS_TYPE_REG);
     assert(info.size == 7);
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
 
     lfs_file_open(&lfs, &file, "/parent/0.before", LFS_O_RDONLY) => 0;
+    uint8_t buffer[1024];
     lfs_file_read(&lfs, &file, buffer, 7) => 7;
     assert(strcmp((char*)buffer, "test.5") == 0);
     lfs_file_close(&lfs, &file) => 0;
     lfs_file_open(&lfs, &file, "/parent/2.after", LFS_O_RDONLY) => 0;
     lfs_file_read(&lfs, &file, buffer, 7) => 7;
     assert(strcmp((char*)buffer, "test.6") == 0);
     lfs_file_close(&lfs, &file) => 0;
@@ -1651,26 +1724,29 @@
     lfs_file_open(&lfs, &file, "/parent/child/2.after", LFS_O_RDONLY) => 0;
     lfs_file_read(&lfs, &file, buffer, 7) => 7;
     assert(strcmp((char*)buffer, "test.8") == 0);
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # move fix in relocation with predecessor
+# move fix in relocation with predecessor
+[cases.test_move_fix_relocation_predecessor]
 in = "lfs.c"
-define.RELOCATIONS = 'range(0x7+1)'
-define.LFS_ERASE_CYCLES = 0xffffffff
+defines.RELOCATIONS = 'range(8)'
+defines.ERASE_CYCLES = 0xffffffff
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     lfs_mkdir(&lfs, "/parent") => 0;
     lfs_mkdir(&lfs, "/parent/child") => 0;
     lfs_mkdir(&lfs, "/parent/sibling") => 0;
 
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "/parent/sibling/1.move_me",
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
     lfs_file_write(&lfs, &file, "move me",
             sizeof("move me")) => sizeof("move me");
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_file_open(&lfs, &file, "/parent/sibling/0.before",
@@ -1702,29 +1778,32 @@
     lfs_file_write(&lfs, &files[0], "test.5", 7) => 7;
     lfs_file_write(&lfs, &files[1], "test.6", 7) => 7;
     lfs_file_write(&lfs, &files[2], "test.7", 7) => 7;
     lfs_file_write(&lfs, &files[3], "test.8", 7) => 7;
 
     // force specific directories to relocate
     if (RELOCATIONS & 0x1) {
+        lfs_dir_t dir;
         lfs_dir_open(&lfs, &dir, "/parent");
-        lfs_testbd_setwear(&cfg, dir.m.pair[0], 0xffffffff) => 0;
-        lfs_testbd_setwear(&cfg, dir.m.pair[1], 0xffffffff) => 0;
+        lfs_emubd_setwear(cfg, dir.m.pair[0], 0xffffffff) => 0;
+        lfs_emubd_setwear(cfg, dir.m.pair[1], 0xffffffff) => 0;
         lfs_dir_close(&lfs, &dir) => 0;
     }
     if (RELOCATIONS & 0x2) {
+        lfs_dir_t dir;
         lfs_dir_open(&lfs, &dir, "/parent/sibling");
-        lfs_testbd_setwear(&cfg, dir.m.pair[0], 0xffffffff) => 0;
-        lfs_testbd_setwear(&cfg, dir.m.pair[1], 0xffffffff) => 0;
+        lfs_emubd_setwear(cfg, dir.m.pair[0], 0xffffffff) => 0;
+        lfs_emubd_setwear(cfg, dir.m.pair[1], 0xffffffff) => 0;
         lfs_dir_close(&lfs, &dir) => 0;
     }
     if (RELOCATIONS & 0x4) {
+        lfs_dir_t dir;
         lfs_dir_open(&lfs, &dir, "/parent/child");
-        lfs_testbd_setwear(&cfg, dir.m.pair[0], 0xffffffff) => 0;
-        lfs_testbd_setwear(&cfg, dir.m.pair[1], 0xffffffff) => 0;
+        lfs_emubd_setwear(cfg, dir.m.pair[0], 0xffffffff) => 0;
+        lfs_emubd_setwear(cfg, dir.m.pair[1], 0xffffffff) => 0;
         lfs_dir_close(&lfs, &dir) => 0;
     }
 
     // ok, now we move the file, this creates a move that needs to be
     // fixed, possibly in a metadata-pair that needs to be relocated
     //
     // and now relocations can force us to need to fix our move in either
@@ -1735,14 +1814,16 @@
 
     lfs_file_close(&lfs, &files[0]) => 0;
     lfs_file_close(&lfs, &files[1]) => 0;
     lfs_file_close(&lfs, &files[2]) => 0;
     lfs_file_close(&lfs, &files[3]) => 0;
 
     // check that nothing was corrupted
+    lfs_dir_t dir;
+    struct lfs_info info;
     lfs_dir_open(&lfs, &dir, "/parent") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, ".") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(strcmp(info.name, "..") == 0);
     assert(info.type == LFS_TYPE_DIR);
@@ -1792,14 +1873,15 @@
     assert(strcmp(info.name, "2.after") == 0);
     assert(info.type == LFS_TYPE_REG);
     assert(info.size == 7);
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
 
     lfs_file_open(&lfs, &file, "/parent/sibling/0.before", LFS_O_RDONLY) => 0;
+    uint8_t buffer[1024];
     lfs_file_read(&lfs, &file, buffer, 7) => 7;
     assert(strcmp((char*)buffer, "test.5") == 0);
     lfs_file_close(&lfs, &file) => 0;
     lfs_file_open(&lfs, &file, "/parent/sibling/2.after", LFS_O_RDONLY) => 0;
     lfs_file_read(&lfs, &file, buffer, 7) => 7;
     assert(strcmp((char*)buffer, "test.6") == 0);
     lfs_file_close(&lfs, &file) => 0;
```

### Comparing `littlefs-python-0.4.0/littlefs/tests/test_paths.toml` & `littlefs-python-0.5.0/littlefs/tests/test_paths.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 
-[[case]] # simple path test
+# simple path test
+[cases.test_paths_normal]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "tea") => 0;
     lfs_mkdir(&lfs, "tea/hottea") => 0;
     lfs_mkdir(&lfs, "tea/warmtea") => 0;
     lfs_mkdir(&lfs, "tea/coldtea") => 0;
 
+    struct lfs_info info;
     lfs_stat(&lfs, "tea/hottea", &info) => 0;
     assert(strcmp(info.name, "hottea") == 0);
     lfs_stat(&lfs, "/tea/hottea", &info) => 0;
     assert(strcmp(info.name, "hottea") == 0);
 
     lfs_mkdir(&lfs, "/milk") => 0;
     lfs_stat(&lfs, "/milk", &info) => 0;
     assert(strcmp(info.name, "milk") == 0);
     lfs_stat(&lfs, "milk", &info) => 0;
     assert(strcmp(info.name, "milk") == 0);
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # redundant slashes
+# redundant slashes
+[cases.test_paths_redundant_slashes]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "tea") => 0;
     lfs_mkdir(&lfs, "tea/hottea") => 0;
     lfs_mkdir(&lfs, "tea/warmtea") => 0;
     lfs_mkdir(&lfs, "tea/coldtea") => 0;
 
+    struct lfs_info info;
     lfs_stat(&lfs, "/tea/hottea", &info) => 0;
     assert(strcmp(info.name, "hottea") == 0);
     lfs_stat(&lfs, "//tea//hottea", &info) => 0;
     assert(strcmp(info.name, "hottea") == 0);
     lfs_stat(&lfs, "///tea///hottea", &info) => 0;
     assert(strcmp(info.name, "hottea") == 0);
 
@@ -41,23 +47,26 @@
     lfs_stat(&lfs, "////milk", &info) => 0;
     assert(strcmp(info.name, "milk") == 0);
     lfs_stat(&lfs, "milk", &info) => 0;
     assert(strcmp(info.name, "milk") == 0);
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # dot path test
+# dot path test
+[cases.test_paths_dot]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "tea") => 0;
     lfs_mkdir(&lfs, "tea/hottea") => 0;
     lfs_mkdir(&lfs, "tea/warmtea") => 0;
     lfs_mkdir(&lfs, "tea/coldtea") => 0;
 
+    struct lfs_info info;
     lfs_stat(&lfs, "./tea/hottea", &info) => 0;
     assert(strcmp(info.name, "hottea") == 0);
     lfs_stat(&lfs, "/./tea/hottea", &info) => 0;
     assert(strcmp(info.name, "hottea") == 0);
     lfs_stat(&lfs, "/././tea/hottea", &info) => 0;
     assert(strcmp(info.name, "hottea") == 0);
     lfs_stat(&lfs, "/./tea/./hottea", &info) => 0;
@@ -67,27 +76,30 @@
     lfs_stat(&lfs, "/./milk", &info) => 0;
     assert(strcmp(info.name, "milk") == 0);
     lfs_stat(&lfs, "milk", &info) => 0;
     assert(strcmp(info.name, "milk") == 0);
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # dot dot path test
+# dot dot path test
+[cases.test_paths_dot_dot]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "tea") => 0;
     lfs_mkdir(&lfs, "tea/hottea") => 0;
     lfs_mkdir(&lfs, "tea/warmtea") => 0;
     lfs_mkdir(&lfs, "tea/coldtea") => 0;
     lfs_mkdir(&lfs, "coffee") => 0;
     lfs_mkdir(&lfs, "coffee/hotcoffee") => 0;
     lfs_mkdir(&lfs, "coffee/warmcoffee") => 0;
     lfs_mkdir(&lfs, "coffee/coldcoffee") => 0;
 
+    struct lfs_info info;
     lfs_stat(&lfs, "coffee/../tea/hottea", &info) => 0;
     assert(strcmp(info.name, "hottea") == 0);
     lfs_stat(&lfs, "tea/coldtea/../hottea", &info) => 0;
     assert(strcmp(info.name, "hottea") == 0);
     lfs_stat(&lfs, "coffee/coldcoffee/../../tea/hottea", &info) => 0;
     assert(strcmp(info.name, "hottea") == 0);
     lfs_stat(&lfs, "coffee/../coffee/../tea/hottea", &info) => 0;
@@ -97,113 +109,133 @@
     lfs_stat(&lfs, "coffee/../milk", &info) => 0;
     strcmp(info.name, "milk") => 0;
     lfs_stat(&lfs, "milk", &info) => 0;
     strcmp(info.name, "milk") => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # trailing dot path test
+# trailing dot path test
+[cases.test_paths_trailing_dot]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "tea") => 0;
     lfs_mkdir(&lfs, "tea/hottea") => 0;
     lfs_mkdir(&lfs, "tea/warmtea") => 0;
     lfs_mkdir(&lfs, "tea/coldtea") => 0;
 
+    struct lfs_info info;
     lfs_stat(&lfs, "tea/hottea/", &info) => 0;
     assert(strcmp(info.name, "hottea") == 0);
     lfs_stat(&lfs, "tea/hottea/.", &info) => 0;
     assert(strcmp(info.name, "hottea") == 0);
     lfs_stat(&lfs, "tea/hottea/./.", &info) => 0;
     assert(strcmp(info.name, "hottea") == 0);
     lfs_stat(&lfs, "tea/hottea/..", &info) => 0;
     assert(strcmp(info.name, "tea") == 0);
     lfs_stat(&lfs, "tea/hottea/../.", &info) => 0;
     assert(strcmp(info.name, "tea") == 0);
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # leading dot path test
+# leading dot path test
+[cases.test_paths_leading_dot]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, ".milk") => 0;
+    struct lfs_info info;
     lfs_stat(&lfs, ".milk", &info) => 0;
     strcmp(info.name, ".milk") => 0;
     lfs_stat(&lfs, "tea/.././.milk", &info) => 0;
     strcmp(info.name, ".milk") => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # root dot dot path test
+# root dot dot path test
+[cases.test_paths_root_dot_dot]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "tea") => 0;
     lfs_mkdir(&lfs, "tea/hottea") => 0;
     lfs_mkdir(&lfs, "tea/warmtea") => 0;
     lfs_mkdir(&lfs, "tea/coldtea") => 0;
     lfs_mkdir(&lfs, "coffee") => 0;
     lfs_mkdir(&lfs, "coffee/hotcoffee") => 0;
     lfs_mkdir(&lfs, "coffee/warmcoffee") => 0;
     lfs_mkdir(&lfs, "coffee/coldcoffee") => 0;
 
+    struct lfs_info info;
     lfs_stat(&lfs, "coffee/../../../../../../tea/hottea", &info) => 0;
     strcmp(info.name, "hottea") => 0;
 
     lfs_mkdir(&lfs, "coffee/../../../../../../milk") => 0;
     lfs_stat(&lfs, "coffee/../../../../../../milk", &info) => 0;
     strcmp(info.name, "milk") => 0;
     lfs_stat(&lfs, "milk", &info) => 0;
     strcmp(info.name, "milk") => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # invalid path tests
+# invalid path tests
+[cases.test_paths_invalid]
 code = '''
-    lfs_format(&lfs, &cfg);
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg);
+    lfs_mount(&lfs, cfg) => 0;
+    struct lfs_info info;
     lfs_stat(&lfs, "dirt", &info) => LFS_ERR_NOENT;
     lfs_stat(&lfs, "dirt/ground", &info) => LFS_ERR_NOENT;
     lfs_stat(&lfs, "dirt/ground/earth", &info) => LFS_ERR_NOENT;
 
     lfs_remove(&lfs, "dirt") => LFS_ERR_NOENT;
     lfs_remove(&lfs, "dirt/ground") => LFS_ERR_NOENT;
     lfs_remove(&lfs, "dirt/ground/earth") => LFS_ERR_NOENT;
 
     lfs_mkdir(&lfs, "dirt/ground") => LFS_ERR_NOENT;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "dirt/ground", LFS_O_WRONLY | LFS_O_CREAT)
             => LFS_ERR_NOENT;
     lfs_mkdir(&lfs, "dirt/ground/earth") => LFS_ERR_NOENT;
     lfs_file_open(&lfs, &file, "dirt/ground/earth", LFS_O_WRONLY | LFS_O_CREAT)
             => LFS_ERR_NOENT;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # root operations
+# root operations
+[cases.test_paths_root]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    struct lfs_info info;
     lfs_stat(&lfs, "/", &info) => 0;
     assert(strcmp(info.name, "/") == 0);
     assert(info.type == LFS_TYPE_DIR);
 
     lfs_mkdir(&lfs, "/") => LFS_ERR_EXIST;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "/", LFS_O_WRONLY | LFS_O_CREAT)
             => LFS_ERR_ISDIR;
 
     lfs_remove(&lfs, "/") => LFS_ERR_INVAL;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # root representations
+# root representations
+[cases.test_paths_root_reprs]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    struct lfs_info info;
     lfs_stat(&lfs, "/", &info) => 0;
     assert(strcmp(info.name, "/") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_stat(&lfs, "", &info) => 0;
     assert(strcmp(info.name, "/") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_stat(&lfs, ".", &info) => 0;
@@ -217,67 +249,78 @@
     assert(info.type == LFS_TYPE_DIR);
     lfs_stat(&lfs, "./", &info) => 0;
     assert(strcmp(info.name, "/") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # superblock conflict test
+# superblock conflict test
+[cases.test_paths_superblock_conflict]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    struct lfs_info info;
     lfs_stat(&lfs, "littlefs", &info) => LFS_ERR_NOENT;
     lfs_remove(&lfs, "littlefs") => LFS_ERR_NOENT;
 
     lfs_mkdir(&lfs, "littlefs") => 0;
     lfs_stat(&lfs, "littlefs", &info) => 0;
     assert(strcmp(info.name, "littlefs") == 0);
     assert(info.type == LFS_TYPE_DIR);
     lfs_remove(&lfs, "littlefs") => 0;
     lfs_stat(&lfs, "littlefs", &info) => LFS_ERR_NOENT;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # max path test
+# max path test
+[cases.test_paths_max]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "coffee") => 0;
     lfs_mkdir(&lfs, "coffee/hotcoffee") => 0;
     lfs_mkdir(&lfs, "coffee/warmcoffee") => 0;
     lfs_mkdir(&lfs, "coffee/coldcoffee") => 0;
 
+    char path[1024];
     memset(path, 'w', LFS_NAME_MAX+1);
     path[LFS_NAME_MAX+1] = '\0';
     lfs_mkdir(&lfs, path) => LFS_ERR_NAMETOOLONG;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, path, LFS_O_WRONLY | LFS_O_CREAT)
             => LFS_ERR_NAMETOOLONG;
 
     memcpy(path, "coffee/", strlen("coffee/"));
     memset(path+strlen("coffee/"), 'w', LFS_NAME_MAX+1);
     path[strlen("coffee/")+LFS_NAME_MAX+1] = '\0';
     lfs_mkdir(&lfs, path) => LFS_ERR_NAMETOOLONG;
     lfs_file_open(&lfs, &file, path, LFS_O_WRONLY | LFS_O_CREAT)
             => LFS_ERR_NAMETOOLONG;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # really big path test
+# really big path test
+[cases.test_paths_really_big]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_mkdir(&lfs, "coffee") => 0;
     lfs_mkdir(&lfs, "coffee/hotcoffee") => 0;
     lfs_mkdir(&lfs, "coffee/warmcoffee") => 0;
     lfs_mkdir(&lfs, "coffee/coldcoffee") => 0;
 
+    char path[1024];
     memset(path, 'w', LFS_NAME_MAX);
     path[LFS_NAME_MAX] = '\0';
     lfs_mkdir(&lfs, path) => 0;
     lfs_remove(&lfs, path) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, path,
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_remove(&lfs, path) => 0;
 
     memcpy(path, "coffee/", strlen("coffee/"));
     memset(path+strlen("coffee/"), 'w', LFS_NAME_MAX);
```

### Comparing `littlefs-python-0.4.0/littlefs/tests/test_relocations.toml` & `littlefs-python-0.5.0/littlefs/tests/test_relocations.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,104 +1,123 @@
 # specific corner cases worth explicitly testing for
-[[case]] # dangling split dir test
-define.ITERATIONS = 20
-define.COUNT = 10
-define.LFS_BLOCK_CYCLES = [8, 1]
+[cases.test_relocations_dangling_split_dir]
+defines.ITERATIONS = 20
+defines.COUNT = 10
+defines.BLOCK_CYCLES = [8, 1]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
     // fill up filesystem so only ~16 blocks are left
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "padding", LFS_O_CREAT | LFS_O_WRONLY) => 0;
+    uint8_t buffer[512];
     memset(buffer, 0, 512);
-    while (LFS_BLOCK_COUNT - lfs_fs_size(&lfs) > 16) {
+    while (BLOCK_COUNT - lfs_fs_size(&lfs) > 16) {
         lfs_file_write(&lfs, &file, buffer, 512) => 512;
     }
     lfs_file_close(&lfs, &file) => 0;
     // make a child dir to use in bounded space
     lfs_mkdir(&lfs, "child") => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
-    for (int j = 0; j < ITERATIONS; j++) {
-        for (int i = 0; i < COUNT; i++) {
+    lfs_mount(&lfs, cfg) => 0;
+    for (unsigned j = 0; j < ITERATIONS; j++) {
+        for (unsigned i = 0; i < COUNT; i++) {
+            char path[1024];
             sprintf(path, "child/test%03d_loooooooooooooooooong_name", i);
             lfs_file_open(&lfs, &file, path, LFS_O_CREAT | LFS_O_WRONLY) => 0;
             lfs_file_close(&lfs, &file) => 0;
         }
 
+        lfs_dir_t dir;
+        struct lfs_info info;
         lfs_dir_open(&lfs, &dir, "child") => 0;
         lfs_dir_read(&lfs, &dir, &info) => 1;
         lfs_dir_read(&lfs, &dir, &info) => 1;
-        for (int i = 0; i < COUNT; i++) {
+        for (unsigned i = 0; i < COUNT; i++) {
+            char path[1024];
             sprintf(path, "test%03d_loooooooooooooooooong_name", i);
             lfs_dir_read(&lfs, &dir, &info) => 1;
             strcmp(info.name, path) => 0;
         }
         lfs_dir_read(&lfs, &dir, &info) => 0;
         lfs_dir_close(&lfs, &dir) => 0;
 
-        if (j == ITERATIONS-1) {
+        if (j == (unsigned)ITERATIONS-1) {
             break;
         }
 
-        for (int i = 0; i < COUNT; i++) {
+        for (unsigned i = 0; i < COUNT; i++) {
+            char path[1024];
             sprintf(path, "child/test%03d_loooooooooooooooooong_name", i);
             lfs_remove(&lfs, path) => 0;
         }
     }
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_dir_t dir;
+    struct lfs_info info;
     lfs_dir_open(&lfs, &dir, "child") => 0;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     lfs_dir_read(&lfs, &dir, &info) => 1;
-    for (int i = 0; i < COUNT; i++) {
+    for (unsigned i = 0; i < COUNT; i++) {
+        char path[1024];
         sprintf(path, "test%03d_loooooooooooooooooong_name", i);
         lfs_dir_read(&lfs, &dir, &info) => 1;
         strcmp(info.name, path) => 0;
     }
     lfs_dir_read(&lfs, &dir, &info) => 0;
     lfs_dir_close(&lfs, &dir) => 0;
-    for (int i = 0; i < COUNT; i++) {
+    for (unsigned i = 0; i < COUNT; i++) {
+        char path[1024];
         sprintf(path, "child/test%03d_loooooooooooooooooong_name", i);
         lfs_remove(&lfs, path) => 0;
     }
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # outdated head test
-define.ITERATIONS = 20
-define.COUNT = 10
-define.LFS_BLOCK_CYCLES = [8, 1]
+[cases.test_relocations_outdated_head]
+defines.ITERATIONS = 20
+defines.COUNT = 10
+defines.BLOCK_CYCLES = [8, 1]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
     // fill up filesystem so only ~16 blocks are left
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "padding", LFS_O_CREAT | LFS_O_WRONLY) => 0;
+    uint8_t buffer[512];
     memset(buffer, 0, 512);
-    while (LFS_BLOCK_COUNT - lfs_fs_size(&lfs) > 16) {
+    while (BLOCK_COUNT - lfs_fs_size(&lfs) > 16) {
         lfs_file_write(&lfs, &file, buffer, 512) => 512;
     }
     lfs_file_close(&lfs, &file) => 0;
     // make a child dir to use in bounded space
     lfs_mkdir(&lfs, "child") => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
-    for (int j = 0; j < ITERATIONS; j++) {
-        for (int i = 0; i < COUNT; i++) {
+    lfs_mount(&lfs, cfg) => 0;
+    for (unsigned j = 0; j < ITERATIONS; j++) {
+        for (unsigned i = 0; i < COUNT; i++) {
+            char path[1024];
             sprintf(path, "child/test%03d_loooooooooooooooooong_name", i);
             lfs_file_open(&lfs, &file, path, LFS_O_CREAT | LFS_O_WRONLY) => 0;
             lfs_file_close(&lfs, &file) => 0;
         }
 
+        lfs_dir_t dir;
+        struct lfs_info info;
         lfs_dir_open(&lfs, &dir, "child") => 0;
         lfs_dir_read(&lfs, &dir, &info) => 1;
         lfs_dir_read(&lfs, &dir, &info) => 1;
-        for (int i = 0; i < COUNT; i++) {
+        for (unsigned i = 0; i < COUNT; i++) {
+            char path[1024];
             sprintf(path, "test%03d_loooooooooooooooooong_name", i);
             lfs_dir_read(&lfs, &dir, &info) => 1;
             strcmp(info.name, path) => 0;
             info.size => 0;
 
             sprintf(path, "child/test%03d_loooooooooooooooooong_name", i);
             lfs_file_open(&lfs, &file, path, LFS_O_WRONLY) => 0;
@@ -106,15 +125,16 @@
             lfs_file_close(&lfs, &file) => 0;
         }
         lfs_dir_read(&lfs, &dir, &info) => 0;
 
         lfs_dir_rewind(&lfs, &dir) => 0;
         lfs_dir_read(&lfs, &dir, &info) => 1;
         lfs_dir_read(&lfs, &dir, &info) => 1;
-        for (int i = 0; i < COUNT; i++) {
+        for (unsigned i = 0; i < COUNT; i++) {
+            char path[1024];
             sprintf(path, "test%03d_loooooooooooooooooong_name", i);
             lfs_dir_read(&lfs, &dir, &info) => 1;
             strcmp(info.name, path) => 0;
             info.size => 2;
 
             sprintf(path, "child/test%03d_loooooooooooooooooong_name", i);
             lfs_file_open(&lfs, &file, path, LFS_O_WRONLY) => 0;
@@ -122,179 +142,197 @@
             lfs_file_close(&lfs, &file) => 0;
         }
         lfs_dir_read(&lfs, &dir, &info) => 0;
 
         lfs_dir_rewind(&lfs, &dir) => 0;
         lfs_dir_read(&lfs, &dir, &info) => 1;
         lfs_dir_read(&lfs, &dir, &info) => 1;
-        for (int i = 0; i < COUNT; i++) {
+        for (unsigned i = 0; i < COUNT; i++) {
+            char path[1024];
             sprintf(path, "test%03d_loooooooooooooooooong_name", i);
             lfs_dir_read(&lfs, &dir, &info) => 1;
             strcmp(info.name, path) => 0;
             info.size => 2;
         }
         lfs_dir_read(&lfs, &dir, &info) => 0;
         lfs_dir_close(&lfs, &dir) => 0;
 
-        for (int i = 0; i < COUNT; i++) {
+        for (unsigned i = 0; i < COUNT; i++) {
+            char path[1024];
             sprintf(path, "child/test%03d_loooooooooooooooooong_name", i);
             lfs_remove(&lfs, path) => 0;
         }
     }
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # reentrant testing for relocations, this is the same as the
-         # orphan testing, except here we also set block_cycles so that
-         # almost every tree operation needs a relocation
+# reentrant testing for relocations, this is the same as the
+# orphan testing, except here we also set block_cycles so that
+# almost every tree operation needs a relocation
+[cases.test_relocations_reentrant]
 reentrant = true
 # TODO fix this case, caused by non-DAG trees
-if = '!(DEPTH == 3 && LFS_CACHE_SIZE != 64)'
-define = [
-    {FILES=6,  DEPTH=1, CYCLES=20, LFS_BLOCK_CYCLES=1},
-    {FILES=26, DEPTH=1, CYCLES=20, LFS_BLOCK_CYCLES=1},
-    {FILES=3,  DEPTH=3, CYCLES=20, LFS_BLOCK_CYCLES=1},
+# NOTE the second condition is required
+if = '!(DEPTH == 3 && CACHE_SIZE != 64) && 2*FILES < BLOCK_COUNT'
+defines = [
+    {FILES=6,  DEPTH=1, CYCLES=20, BLOCK_CYCLES=1},
+    {FILES=26, DEPTH=1, CYCLES=20, BLOCK_CYCLES=1},
+    {FILES=3,  DEPTH=3, CYCLES=20, BLOCK_CYCLES=1},
 ]
 code = '''
-    err = lfs_mount(&lfs, &cfg);
+    lfs_t lfs;
+    int err = lfs_mount(&lfs, cfg);
     if (err) {
-        lfs_format(&lfs, &cfg) => 0;
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_format(&lfs, cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
     }
 
-    srand(1);
+    uint32_t prng = 1;
     const char alpha[] = "abcdefghijklmnopqrstuvwxyz";
-    for (int i = 0; i < CYCLES; i++) {
+    for (unsigned i = 0; i < CYCLES; i++) {
         // create random path
         char full_path[256];
-        for (int d = 0; d < DEPTH; d++) {
-            sprintf(&full_path[2*d], "/%c", alpha[rand() % FILES]);
+        for (unsigned d = 0; d < DEPTH; d++) {
+            sprintf(&full_path[2*d], "/%c", alpha[TEST_PRNG(&prng) % FILES]);
         }
 
         // if it does not exist, we create it, else we destroy
+        struct lfs_info info;
         int res = lfs_stat(&lfs, full_path, &info);
         if (res == LFS_ERR_NOENT) {
             // create each directory in turn, ignore if dir already exists
-            for (int d = 0; d < DEPTH; d++) {
+            for (unsigned d = 0; d < DEPTH; d++) {
+                char path[1024];
                 strcpy(path, full_path);
                 path[2*d+2] = '\0';
                 err = lfs_mkdir(&lfs, path);
                 assert(!err || err == LFS_ERR_EXIST);
             }
 
-            for (int d = 0; d < DEPTH; d++) {
+            for (unsigned d = 0; d < DEPTH; d++) {
+                char path[1024];
                 strcpy(path, full_path);
                 path[2*d+2] = '\0';
                 lfs_stat(&lfs, path, &info) => 0;
                 assert(strcmp(info.name, &path[2*d+1]) == 0);
                 assert(info.type == LFS_TYPE_DIR);
             }
         } else {
             // is valid dir?
             assert(strcmp(info.name, &full_path[2*(DEPTH-1)+1]) == 0);
             assert(info.type == LFS_TYPE_DIR);
 
             // try to delete path in reverse order, ignore if dir is not empty
-            for (int d = DEPTH-1; d >= 0; d--) {
+            for (unsigned d = DEPTH-1; d+1 > 0; d--) {
+                char path[1024];
                 strcpy(path, full_path);
                 path[2*d+2] = '\0';
                 err = lfs_remove(&lfs, path);
                 assert(!err || err == LFS_ERR_NOTEMPTY);
             }
 
             lfs_stat(&lfs, full_path, &info) => LFS_ERR_NOENT;
         }
     }
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # reentrant testing for relocations, but now with random renames!
+# reentrant testing for relocations, but now with random renames!
+[cases.test_relocations_reentrant_renames]
 reentrant = true
 # TODO fix this case, caused by non-DAG trees
-if = '!(DEPTH == 3 && LFS_CACHE_SIZE != 64)'
-define = [
-    {FILES=6,  DEPTH=1, CYCLES=20, LFS_BLOCK_CYCLES=1},
-    {FILES=26, DEPTH=1, CYCLES=20, LFS_BLOCK_CYCLES=1},
-    {FILES=3,  DEPTH=3, CYCLES=20, LFS_BLOCK_CYCLES=1},
+# NOTE the second condition is required
+if = '!(DEPTH == 3 && CACHE_SIZE != 64) && 2*FILES < BLOCK_COUNT'
+defines = [
+    {FILES=6,  DEPTH=1, CYCLES=20, BLOCK_CYCLES=1},
+    {FILES=26, DEPTH=1, CYCLES=20, BLOCK_CYCLES=1},
+    {FILES=3,  DEPTH=3, CYCLES=20, BLOCK_CYCLES=1},
 ]
 code = '''
-    err = lfs_mount(&lfs, &cfg);
+    lfs_t lfs;
+    int err = lfs_mount(&lfs, cfg);
     if (err) {
-        lfs_format(&lfs, &cfg) => 0;
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_format(&lfs, cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
     }
 
-    srand(1);
+    uint32_t prng = 1;
     const char alpha[] = "abcdefghijklmnopqrstuvwxyz";
-    for (int i = 0; i < CYCLES; i++) {
+    for (unsigned i = 0; i < CYCLES; i++) {
         // create random path
         char full_path[256];
-        for (int d = 0; d < DEPTH; d++) {
-            sprintf(&full_path[2*d], "/%c", alpha[rand() % FILES]);
+        for (unsigned d = 0; d < DEPTH; d++) {
+            sprintf(&full_path[2*d], "/%c", alpha[TEST_PRNG(&prng) % FILES]);
         }
 
         // if it does not exist, we create it, else we destroy
+        struct lfs_info info;
         int res = lfs_stat(&lfs, full_path, &info);
         assert(!res || res == LFS_ERR_NOENT);
         if (res == LFS_ERR_NOENT) {
             // create each directory in turn, ignore if dir already exists
-            for (int d = 0; d < DEPTH; d++) {
+            for (unsigned d = 0; d < DEPTH; d++) {
+                char path[1024];
                 strcpy(path, full_path);
                 path[2*d+2] = '\0';
                 err = lfs_mkdir(&lfs, path);
                 assert(!err || err == LFS_ERR_EXIST);
             }
 
-            for (int d = 0; d < DEPTH; d++) {
+            for (unsigned d = 0; d < DEPTH; d++) {
+                char path[1024];
                 strcpy(path, full_path);
                 path[2*d+2] = '\0';
                 lfs_stat(&lfs, path, &info) => 0;
                 assert(strcmp(info.name, &path[2*d+1]) == 0);
                 assert(info.type == LFS_TYPE_DIR);
             }
         } else {
             assert(strcmp(info.name, &full_path[2*(DEPTH-1)+1]) == 0);
             assert(info.type == LFS_TYPE_DIR);
 
             // create new random path
             char new_path[256];
-            for (int d = 0; d < DEPTH; d++) {
-                sprintf(&new_path[2*d], "/%c", alpha[rand() % FILES]);
+            for (unsigned d = 0; d < DEPTH; d++) {
+                sprintf(&new_path[2*d], "/%c", alpha[TEST_PRNG(&prng) % FILES]);
             }
 
             // if new path does not exist, rename, otherwise destroy
             res = lfs_stat(&lfs, new_path, &info);
             assert(!res || res == LFS_ERR_NOENT);
             if (res == LFS_ERR_NOENT) {
                 // stop once some dir is renamed
-                for (int d = 0; d < DEPTH; d++) {
+                for (unsigned d = 0; d < DEPTH; d++) {
+                    char path[1024];
                     strcpy(&path[2*d], &full_path[2*d]);
                     path[2*d+2] = '\0';
                     strcpy(&path[128+2*d], &new_path[2*d]);
                     path[128+2*d+2] = '\0';
                     err = lfs_rename(&lfs, path, path+128);
                     assert(!err || err == LFS_ERR_NOTEMPTY);
                     if (!err) {
                         strcpy(path, path+128);
                     }
                 }
 
-                for (int d = 0; d < DEPTH; d++) {
+                for (unsigned d = 0; d < DEPTH; d++) {
+                    char path[1024];
                     strcpy(path, new_path);
                     path[2*d+2] = '\0';
                     lfs_stat(&lfs, path, &info) => 0;
                     assert(strcmp(info.name, &path[2*d+1]) == 0);
                     assert(info.type == LFS_TYPE_DIR);
                 }
                 
                 lfs_stat(&lfs, full_path, &info) => LFS_ERR_NOENT;
             } else {
                 // try to delete path in reverse order,
                 // ignore if dir is not empty
-                for (int d = DEPTH-1; d >= 0; d--) {
+                for (unsigned d = DEPTH-1; d+1 > 0; d--) {
+                    char path[1024];
                     strcpy(path, full_path);
                     path[2*d+2] = '\0';
                     err = lfs_remove(&lfs, path);
                     assert(!err || err == LFS_ERR_NOTEMPTY);
                 }
 
                 lfs_stat(&lfs, full_path, &info) => LFS_ERR_NOENT;
```

### Comparing `littlefs-python-0.4.0/littlefs/tests/test_seek.toml` & `littlefs-python-0.5.0/littlefs/tests/test_seek.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 
-[[case]] # simple file seek
-define = [
+# simple file seek
+[cases.test_seek_read]
+defines = [
     {COUNT=132, SKIP=4},
     {COUNT=132, SKIP=128},
     {COUNT=200, SKIP=10},
     {COUNT=200, SKIP=100},
     {COUNT=4,   SKIP=1},
     {COUNT=4,   SKIP=2},
 ]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "kitty",
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_APPEND) => 0;
-    size = strlen("kittycatcat");
+    size_t size = strlen("kittycatcat");
+    uint8_t buffer[1024];
     memcpy(buffer, "kittycatcat", size);
     for (int j = 0; j < COUNT; j++) {
         lfs_file_write(&lfs, &file, buffer, size);
     }
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "kitty", LFS_O_RDONLY) => 0;
 
     lfs_soff_t pos = -1;
     size = strlen("kittycatcat");
     for (int i = 0; i < SKIP; i++) {
         lfs_file_read(&lfs, &file, buffer, size) => size;
         memcmp(buffer, "kittycatcat", size) => 0;
@@ -64,37 +68,41 @@
     size = lfs_file_size(&lfs, &file);
     lfs_file_seek(&lfs, &file, 0, LFS_SEEK_CUR) => size;
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # simple file seek and write
-define = [
+# simple file seek and write
+[cases.test_seek_write]
+defines = [
     {COUNT=132, SKIP=4},
     {COUNT=132, SKIP=128},
     {COUNT=200, SKIP=10},
     {COUNT=200, SKIP=100},
     {COUNT=4,   SKIP=1},
     {COUNT=4,   SKIP=2},
 ]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "kitty",
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_APPEND) => 0;
-    size = strlen("kittycatcat");
+    size_t size = strlen("kittycatcat");
+    uint8_t buffer[1024];
     memcpy(buffer, "kittycatcat", size);
     for (int j = 0; j < COUNT; j++) {
         lfs_file_write(&lfs, &file, buffer, size);
     }
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "kitty", LFS_O_RDWR) => 0;
 
     lfs_soff_t pos = -1;
     size = strlen("kittycatcat");
     for (int i = 0; i < SKIP; i++) {
         lfs_file_read(&lfs, &file, buffer, size) => size;
         memcmp(buffer, "kittycatcat", size) => 0;
@@ -125,35 +133,38 @@
     size = lfs_file_size(&lfs, &file);
     lfs_file_seek(&lfs, &file, 0, LFS_SEEK_CUR) => size;
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # boundary seek and writes
-define.COUNT = 132
-define.OFFSETS = '"{512, 1020, 513, 1021, 511, 1019, 1441}"'
+# boundary seek and writes
+[cases.test_seek_boundary_write]
+defines.COUNT = 132
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "kitty",
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_APPEND) => 0;
-    size = strlen("kittycatcat");
+    size_t size = strlen("kittycatcat");
+    uint8_t buffer[1024];
     memcpy(buffer, "kittycatcat", size);
     for (int j = 0; j < COUNT; j++) {
         lfs_file_write(&lfs, &file, buffer, size);
     }
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "kitty", LFS_O_RDWR) => 0;
 
     size = strlen("hedgehoghog");
-    const lfs_soff_t offsets[] = OFFSETS;
+    const lfs_soff_t offsets[] = {512, 1020, 513, 1021, 511, 1019, 1441};
 
     for (unsigned i = 0; i < sizeof(offsets) / sizeof(offsets[0]); i++) {
         lfs_soff_t off = offsets[i];
         memcpy(buffer, "hedgehoghog", size);
         lfs_file_seek(&lfs, &file, off, LFS_SEEK_SET) => off;
         lfs_file_write(&lfs, &file, buffer, size) => size;
         lfs_file_seek(&lfs, &file, off, LFS_SEEK_SET) => off;
@@ -179,36 +190,40 @@
         memcmp(buffer, "hedgehoghog", size) => 0;
     }
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # out of bounds seek
-define = [
+# out of bounds seek
+[cases.test_seek_out_of_bounds]
+defines = [
     {COUNT=132, SKIP=4},
     {COUNT=132, SKIP=128},
     {COUNT=200, SKIP=10},
     {COUNT=200, SKIP=100},
     {COUNT=4,   SKIP=2},
     {COUNT=4,   SKIP=3},
 ]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "kitty",
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_APPEND) => 0;
-    size = strlen("kittycatcat");
+    size_t size = strlen("kittycatcat");
+    uint8_t buffer[1024];
     memcpy(buffer, "kittycatcat", size);
     for (int j = 0; j < COUNT; j++) {
         lfs_file_write(&lfs, &file, buffer, size);
     }
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "kitty", LFS_O_RDWR) => 0;
 
     size = strlen("kittycatcat");
     lfs_file_size(&lfs, &file) => COUNT*size;
     lfs_file_seek(&lfs, &file, (COUNT+SKIP)*size,
             LFS_SEEK_SET) => (COUNT+SKIP)*size;
     lfs_file_read(&lfs, &file, buffer, size) => 0;
@@ -234,24 +249,28 @@
             LFS_SEEK_END) => LFS_ERR_INVAL;
     lfs_file_tell(&lfs, &file) => (COUNT+1)*size;
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # inline write and seek
-define.SIZE = [2, 4, 128, 132]
+# inline write and seek
+[cases.test_seek_inline_write]
+defines.SIZE = [2, 4, 128, 132]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "tinykitty",
             LFS_O_RDWR | LFS_O_CREAT) => 0;
     int j = 0;
     int k = 0;
 
+    uint8_t buffer[1024];
     memcpy(buffer, "abcdefghijklmnopqrstuvwxyz", 26);
     for (unsigned i = 0; i < SIZE; i++) {
         lfs_file_write(&lfs, &file, &buffer[j++ % 26], 1) => 1;
         lfs_file_tell(&lfs, &file) => i+1;
         lfs_file_size(&lfs, &file) => i+1;
     }
 
@@ -301,24 +320,28 @@
     lfs_file_tell(&lfs, &file) => SIZE;
     lfs_file_size(&lfs, &file) => SIZE;
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # file seek and write with power-loss
+# file seek and write with power-loss
+[cases.test_seek_reentrant_write]
 # must be power-of-2 for quadratic probing to be exhaustive
-define.COUNT = [4, 64, 128]
+defines.COUNT = [4, 64, 128]
 reentrant = true
 code = '''
-    err = lfs_mount(&lfs, &cfg);
+    lfs_t lfs;
+    int err = lfs_mount(&lfs, cfg);
     if (err) {
-        lfs_format(&lfs, &cfg) => 0;
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_format(&lfs, cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
     }
+    lfs_file_t file;
+    uint8_t buffer[1024];
     err = lfs_file_open(&lfs, &file, "kitty", LFS_O_RDONLY);
     assert(!err || err == LFS_ERR_NOENT);
     if (!err) {
         if (lfs_file_size(&lfs, &file) != 0) {
             lfs_file_size(&lfs, &file) => 11*COUNT;
             for (int j = 0; j < COUNT; j++) {
                 memset(buffer, 0, 11+1);
@@ -330,22 +353,22 @@
         lfs_file_close(&lfs, &file) => 0;
     }
 
     lfs_file_open(&lfs, &file, "kitty", LFS_O_WRONLY | LFS_O_CREAT) => 0;
     if (lfs_file_size(&lfs, &file) == 0) {
         for (int j = 0; j < COUNT; j++) {
             strcpy((char*)buffer, "kittycatcat");
-            size = strlen((char*)buffer);
+            size_t size = strlen((char*)buffer);
             lfs_file_write(&lfs, &file, buffer, size) => size;
         }
     }
     lfs_file_close(&lfs, &file) => 0;
 
     strcpy((char*)buffer, "doggodogdog");
-    size = strlen((char*)buffer);
+    size_t size = strlen((char*)buffer);
 
     lfs_file_open(&lfs, &file, "kitty", LFS_O_RDWR) => 0;
     lfs_file_size(&lfs, &file) => COUNT*size;
     // seek and write using quadratic probing to touch all
     // 11-byte words in the file
     lfs_off_t off = 0;
     for (int j = 0; j < COUNT; j++) {
```

### Comparing `littlefs-python-0.4.0/littlefs/tests/test_superblocks.toml` & `littlefs-python-0.5.0/littlefs/tests/test_superblocks.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,127 +1,151 @@
-[[case]] # simple formatting test
+# simple formatting test
+[cases.test_superblocks_format]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
 '''
 
-[[case]] # mount/unmount
+# mount/unmount
+[cases.test_superblocks_mount]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # reentrant format
+# reentrant format
+[cases.test_superblocks_reentrant_format]
 reentrant = true
 code = '''
-    err = lfs_mount(&lfs, &cfg);
+    lfs_t lfs;
+    int err = lfs_mount(&lfs, cfg);
     if (err) {
-        lfs_format(&lfs, &cfg) => 0;
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_format(&lfs, cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
     }
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # invalid mount
+# invalid mount
+[cases.test_superblocks_invalid_mount]
 code = '''
-    lfs_mount(&lfs, &cfg) => LFS_ERR_CORRUPT;
+    lfs_t lfs;
+    lfs_mount(&lfs, cfg) => LFS_ERR_CORRUPT;
 '''
 
-[[case]] # expanding superblock
-define.LFS_BLOCK_CYCLES = [32, 33, 1]
-define.N = [10, 100, 1000]
+# expanding superblock
+[cases.test_superblocks_expand]
+defines.BLOCK_CYCLES = [32, 33, 1]
+defines.N = [10, 100, 1000]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     for (int i = 0; i < N; i++) {
+        lfs_file_t file;
         lfs_file_open(&lfs, &file, "dummy",
                 LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => 0;
         lfs_file_close(&lfs, &file) => 0;
+        struct lfs_info info;
         lfs_stat(&lfs, "dummy", &info) => 0;
         assert(strcmp(info.name, "dummy") == 0);
         assert(info.type == LFS_TYPE_REG);
         lfs_remove(&lfs, "dummy") => 0;
     }
     lfs_unmount(&lfs) => 0;
 
     // one last check after power-cycle
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "dummy",
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => 0;
     lfs_file_close(&lfs, &file) => 0;
+    struct lfs_info info;
     lfs_stat(&lfs, "dummy", &info) => 0;
     assert(strcmp(info.name, "dummy") == 0);
     assert(info.type == LFS_TYPE_REG);
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # expanding superblock with power cycle
-define.LFS_BLOCK_CYCLES = [32, 33, 1]
-define.N = [10, 100, 1000]
+# expanding superblock with power cycle
+[cases.test_superblocks_expand_power_cycle]
+defines.BLOCK_CYCLES = [32, 33, 1]
+defines.N = [10, 100, 1000]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
     for (int i = 0; i < N; i++) {
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
         // remove lingering dummy?
-        err = lfs_stat(&lfs, "dummy", &info);
+        struct lfs_info info;
+        int err = lfs_stat(&lfs, "dummy", &info);
         assert(err == 0 || (err == LFS_ERR_NOENT && i == 0));
         if (!err) {
             assert(strcmp(info.name, "dummy") == 0);
             assert(info.type == LFS_TYPE_REG);
             lfs_remove(&lfs, "dummy") => 0;
         }
 
+        lfs_file_t file;
         lfs_file_open(&lfs, &file, "dummy",
                 LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => 0;
         lfs_file_close(&lfs, &file) => 0;
         lfs_stat(&lfs, "dummy", &info) => 0;
         assert(strcmp(info.name, "dummy") == 0);
         assert(info.type == LFS_TYPE_REG);
         lfs_unmount(&lfs) => 0;
     }
 
     // one last check after power-cycle
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    struct lfs_info info;
     lfs_stat(&lfs, "dummy", &info) => 0;
     assert(strcmp(info.name, "dummy") == 0);
     assert(info.type == LFS_TYPE_REG);
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # reentrant expanding superblock
-define.LFS_BLOCK_CYCLES = [2, 1]
-define.N = 24
+# reentrant expanding superblock
+[cases.test_superblocks_reentrant_expand]
+defines.BLOCK_CYCLES = [2, 1]
+defines.N = 24
 reentrant = true
 code = '''
-    err = lfs_mount(&lfs, &cfg);
+    lfs_t lfs;
+    int err = lfs_mount(&lfs, cfg);
     if (err) {
-        lfs_format(&lfs, &cfg) => 0;
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_format(&lfs, cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
     }
 
     for (int i = 0; i < N; i++) {
         // remove lingering dummy?
+        struct lfs_info info;
         err = lfs_stat(&lfs, "dummy", &info);
         assert(err == 0 || (err == LFS_ERR_NOENT && i == 0));
         if (!err) {
             assert(strcmp(info.name, "dummy") == 0);
             assert(info.type == LFS_TYPE_REG);
             lfs_remove(&lfs, "dummy") => 0;
         }
 
+        lfs_file_t file;
         lfs_file_open(&lfs, &file, "dummy",
                 LFS_O_WRONLY | LFS_O_CREAT | LFS_O_EXCL) => 0;
         lfs_file_close(&lfs, &file) => 0;
         lfs_stat(&lfs, "dummy", &info) => 0;
         assert(strcmp(info.name, "dummy") == 0);
         assert(info.type == LFS_TYPE_REG);
     }
 
     lfs_unmount(&lfs) => 0;
 
     // one last check after power-cycle
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    struct lfs_info info;
     lfs_stat(&lfs, "dummy", &info) => 0;
     assert(strcmp(info.name, "dummy") == 0);
     assert(info.type == LFS_TYPE_REG);
     lfs_unmount(&lfs) => 0;
 '''
```

### Comparing `littlefs-python-0.4.0/littlefs/tests/test_truncate.toml` & `littlefs-python-0.5.0/littlefs/tests/test_truncate.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,110 +1,129 @@
-[[case]] # simple truncate
-define.MEDIUMSIZE = [32, 2048]
-define.LARGESIZE = 8192
+# simple truncate
+[cases.test_truncate_simple]
+defines.MEDIUMSIZE = [31, 32, 33, 511, 512, 513, 2047, 2048, 2049]
+defines.LARGESIZE = [32, 33, 512, 513, 2048, 2049, 8192, 8193]
+if = 'MEDIUMSIZE < LARGESIZE'
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "baldynoop",
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
 
+    uint8_t buffer[1024];
     strcpy((char*)buffer, "hair");
-    size = strlen((char*)buffer);
+    size_t size = strlen((char*)buffer);
     for (lfs_off_t j = 0; j < LARGESIZE; j += size) {
-        lfs_file_write(&lfs, &file, buffer, size) => size;
+        lfs_file_write(&lfs, &file, buffer, lfs_min(size, LARGESIZE-j))
+                => lfs_min(size, LARGESIZE-j);
     }
     lfs_file_size(&lfs, &file) => LARGESIZE;
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
     
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "baldynoop", LFS_O_RDWR) => 0;
     lfs_file_size(&lfs, &file) => LARGESIZE;
 
     lfs_file_truncate(&lfs, &file, MEDIUMSIZE) => 0;
     lfs_file_size(&lfs, &file) => MEDIUMSIZE;
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "baldynoop", LFS_O_RDONLY) => 0;
     lfs_file_size(&lfs, &file) => MEDIUMSIZE;
 
     size = strlen("hair");
     for (lfs_off_t j = 0; j < MEDIUMSIZE; j += size) {
-        lfs_file_read(&lfs, &file, buffer, size) => size;
-        memcmp(buffer, "hair", size) => 0;
+        lfs_file_read(&lfs, &file, buffer, lfs_min(size, MEDIUMSIZE-j))
+                => lfs_min(size, MEDIUMSIZE-j);
+        memcmp(buffer, "hair", lfs_min(size, MEDIUMSIZE-j)) => 0;
     }
     lfs_file_read(&lfs, &file, buffer, size) => 0;
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # truncate and read
-define.MEDIUMSIZE = [32, 2048]
-define.LARGESIZE = 8192
+# truncate and read
+[cases.test_truncate_read]
+defines.MEDIUMSIZE = [31, 32, 33, 511, 512, 513, 2047, 2048, 2049]
+defines.LARGESIZE = [32, 33, 512, 513, 2048, 2049, 8192, 8193]
+if = 'MEDIUMSIZE < LARGESIZE'
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "baldyread",
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
 
+    uint8_t buffer[1024];
     strcpy((char*)buffer, "hair");
-    size = strlen((char*)buffer);
+    size_t size = strlen((char*)buffer);
     for (lfs_off_t j = 0; j < LARGESIZE; j += size) {
-        lfs_file_write(&lfs, &file, buffer, size) => size;
+        lfs_file_write(&lfs, &file, buffer, lfs_min(size, LARGESIZE-j))
+                => lfs_min(size, LARGESIZE-j);
     }
     lfs_file_size(&lfs, &file) => LARGESIZE;
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "baldyread", LFS_O_RDWR) => 0;
     lfs_file_size(&lfs, &file) => LARGESIZE;
 
     lfs_file_truncate(&lfs, &file, MEDIUMSIZE) => 0;
     lfs_file_size(&lfs, &file) => MEDIUMSIZE;
 
     size = strlen("hair");
     for (lfs_off_t j = 0; j < MEDIUMSIZE; j += size) {
-        lfs_file_read(&lfs, &file, buffer, size) => size;
-        memcmp(buffer, "hair", size) => 0;
+        lfs_file_read(&lfs, &file, buffer, lfs_min(size, MEDIUMSIZE-j))
+                => lfs_min(size, MEDIUMSIZE-j);
+        memcmp(buffer, "hair", lfs_min(size, MEDIUMSIZE-j)) => 0;
     }
     lfs_file_read(&lfs, &file, buffer, size) => 0;
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "baldyread", LFS_O_RDONLY) => 0;
     lfs_file_size(&lfs, &file) => MEDIUMSIZE;
 
     size = strlen("hair");
     for (lfs_off_t j = 0; j < MEDIUMSIZE; j += size) {
-        lfs_file_read(&lfs, &file, buffer, size) => size;
-        memcmp(buffer, "hair", size) => 0;
+        lfs_file_read(&lfs, &file, buffer, lfs_min(size, MEDIUMSIZE-j))
+                => lfs_min(size, MEDIUMSIZE-j);
+        memcmp(buffer, "hair", lfs_min(size, MEDIUMSIZE-j)) => 0;
     }
     lfs_file_read(&lfs, &file, buffer, size) => 0;
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # write, truncate, and read
+# write, truncate, and read
+[cases.test_truncate_write_read]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "sequence",
             LFS_O_RDWR | LFS_O_CREAT | LFS_O_TRUNC) => 0;
 
-    size = lfs_min(lfs.cfg->cache_size, sizeof(buffer)/2);
+    uint8_t buffer[1024];
+    size_t size = lfs_min(lfs.cfg->cache_size, sizeof(buffer)/2);
     lfs_size_t qsize = size / 4;
     uint8_t *wb = buffer;
     uint8_t *rb = buffer + size;
     for (lfs_off_t j = 0; j < size; ++j) {
         wb[j] = j;
     }
 
@@ -132,146 +151,169 @@
     lfs_file_tell(&lfs, &file) => qsize;
 
     /* Chop to 1/2 */
     trunc -= qsize;
     lfs_file_truncate(&lfs, &file, trunc) => 0;
     lfs_file_tell(&lfs, &file) => qsize;
     lfs_file_size(&lfs, &file) => trunc;
-    
+
     /* Read should produce second quarter */
     lfs_file_read(&lfs, &file, rb, size) => trunc - qsize;
     memcmp(rb, wb + qsize, trunc - qsize) => 0;
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # truncate and write
-define.MEDIUMSIZE = [32, 2048]
-define.LARGESIZE = 8192
+# truncate and write
+[cases.test_truncate_write]
+defines.MEDIUMSIZE = [31, 32, 33, 511, 512, 513, 2047, 2048, 2049]
+defines.LARGESIZE = [32, 33, 512, 513, 2048, 2049, 8192, 8193]
+if = 'MEDIUMSIZE < LARGESIZE'
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "baldywrite",
             LFS_O_WRONLY | LFS_O_CREAT) => 0;
 
+    uint8_t buffer[1024];
     strcpy((char*)buffer, "hair");
-    size = strlen((char*)buffer);
+    size_t size = strlen((char*)buffer);
     for (lfs_off_t j = 0; j < LARGESIZE; j += size) {
-        lfs_file_write(&lfs, &file, buffer, size) => size;
+        lfs_file_write(&lfs, &file, buffer, lfs_min(size, LARGESIZE-j))
+                => lfs_min(size, LARGESIZE-j);
     }
     lfs_file_size(&lfs, &file) => LARGESIZE;
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "baldywrite", LFS_O_RDWR) => 0;
     lfs_file_size(&lfs, &file) => LARGESIZE;
 
+    /* truncate */
     lfs_file_truncate(&lfs, &file, MEDIUMSIZE) => 0;
     lfs_file_size(&lfs, &file) => MEDIUMSIZE;
 
+    /* and write */
     strcpy((char*)buffer, "bald");
     size = strlen((char*)buffer);
     for (lfs_off_t j = 0; j < MEDIUMSIZE; j += size) {
-        lfs_file_write(&lfs, &file, buffer, size) => size;
+        lfs_file_write(&lfs, &file, buffer, lfs_min(size, MEDIUMSIZE-j))
+                => lfs_min(size, MEDIUMSIZE-j);
     }
     lfs_file_size(&lfs, &file) => MEDIUMSIZE;
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "baldywrite", LFS_O_RDONLY) => 0;
     lfs_file_size(&lfs, &file) => MEDIUMSIZE;
 
     size = strlen("bald");
     for (lfs_off_t j = 0; j < MEDIUMSIZE; j += size) {
-        lfs_file_read(&lfs, &file, buffer, size) => size;
-        memcmp(buffer, "bald", size) => 0;
+        lfs_file_read(&lfs, &file, buffer, lfs_min(size, MEDIUMSIZE-j))
+                => lfs_min(size, MEDIUMSIZE-j);
+        memcmp(buffer, "bald", lfs_min(size, MEDIUMSIZE-j)) => 0;
     }
     lfs_file_read(&lfs, &file, buffer, size) => 0;
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # truncate write under powerloss
-define.SMALLSIZE = [4, 512]
-define.MEDIUMSIZE = [32, 1024]
-define.LARGESIZE = 2048
+# truncate write under powerloss
+[cases.test_truncate_reentrant_write]
+defines.SMALLSIZE = [4, 512]
+defines.MEDIUMSIZE = [0, 3, 4, 5, 31, 32, 33, 511, 512, 513, 1023, 1024, 1025]
+defines.LARGESIZE = 2048
 reentrant = true
 code = '''
-    err = lfs_mount(&lfs, &cfg);
+    lfs_t lfs;
+    int err = lfs_mount(&lfs, cfg);
     if (err) {
-        lfs_format(&lfs, &cfg) => 0;
-        lfs_mount(&lfs, &cfg) => 0;
+        lfs_format(&lfs, cfg) => 0;
+        lfs_mount(&lfs, cfg) => 0;
     }
+    lfs_file_t file;
     err = lfs_file_open(&lfs, &file, "baldy", LFS_O_RDONLY);
     assert(!err || err == LFS_ERR_NOENT);
     if (!err) {
-        size = lfs_file_size(&lfs, &file);
+        size_t size = lfs_file_size(&lfs, &file);
         assert(size == 0 ||
-                size == LARGESIZE ||
-                size == MEDIUMSIZE ||
-                size == SMALLSIZE);
+                size == (size_t)LARGESIZE ||
+                size == (size_t)MEDIUMSIZE ||
+                size == (size_t)SMALLSIZE);
         for (lfs_off_t j = 0; j < size; j += 4) {
-            lfs_file_read(&lfs, &file, buffer, 4) => 4;
-            assert(memcmp(buffer, "hair", 4) == 0 ||
-                   memcmp(buffer, "bald", 4) == 0 ||
-                   memcmp(buffer, "comb", 4) == 0);
+            uint8_t buffer[1024];
+            lfs_file_read(&lfs, &file, buffer, lfs_min(4, size-j))
+                    => lfs_min(4, size-j);
+            assert(memcmp(buffer, "hair", lfs_min(4, size-j)) == 0 ||
+                   memcmp(buffer, "bald", lfs_min(4, size-j)) == 0 ||
+                   memcmp(buffer, "comb", lfs_min(4, size-j)) == 0);
         }
         lfs_file_close(&lfs, &file) => 0;
     }
 
     lfs_file_open(&lfs, &file, "baldy",
             LFS_O_WRONLY | LFS_O_CREAT | LFS_O_TRUNC) => 0;
     lfs_file_size(&lfs, &file) => 0;
+    uint8_t buffer[1024];
     strcpy((char*)buffer, "hair");
-    size = strlen((char*)buffer);
+    size_t size = strlen((char*)buffer);
     for (lfs_off_t j = 0; j < LARGESIZE; j += size) {
-        lfs_file_write(&lfs, &file, buffer, size) => size;
+        lfs_file_write(&lfs, &file, buffer, lfs_min(size, LARGESIZE-j))
+                => lfs_min(size, LARGESIZE-j);
     }
     lfs_file_size(&lfs, &file) => LARGESIZE;
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_file_open(&lfs, &file, "baldy", LFS_O_RDWR) => 0;
     lfs_file_size(&lfs, &file) => LARGESIZE;
+    /* truncate */
     lfs_file_truncate(&lfs, &file, MEDIUMSIZE) => 0;
     lfs_file_size(&lfs, &file) => MEDIUMSIZE;
+    /* and write */
     strcpy((char*)buffer, "bald");
     size = strlen((char*)buffer);
     for (lfs_off_t j = 0; j < MEDIUMSIZE; j += size) {
-        lfs_file_write(&lfs, &file, buffer, size) => size;
+        lfs_file_write(&lfs, &file, buffer, lfs_min(size, MEDIUMSIZE-j))
+                => lfs_min(size, MEDIUMSIZE-j);
     }
     lfs_file_size(&lfs, &file) => MEDIUMSIZE;
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_file_open(&lfs, &file, "baldy", LFS_O_RDWR) => 0;
     lfs_file_size(&lfs, &file) => MEDIUMSIZE;
     lfs_file_truncate(&lfs, &file, SMALLSIZE) => 0;
     lfs_file_size(&lfs, &file) => SMALLSIZE;
     strcpy((char*)buffer, "comb");
     size = strlen((char*)buffer);
     for (lfs_off_t j = 0; j < SMALLSIZE; j += size) {
-        lfs_file_write(&lfs, &file, buffer, size) => size;
+        lfs_file_write(&lfs, &file, buffer, lfs_min(size, SMALLSIZE-j))
+                => lfs_min(size, SMALLSIZE-j);
     }
     lfs_file_size(&lfs, &file) => SMALLSIZE;
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # more aggressive general truncation tests
-define.CONFIG = 'range(6)'
-define.SMALLSIZE = 32
-define.MEDIUMSIZE = 2048
-define.LARGESIZE = 8192
+# more aggressive general truncation tests
+[cases.test_truncate_aggressive]
+defines.CONFIG = 'range(6)'
+defines.SMALLSIZE = 32
+defines.MEDIUMSIZE = 2048
+defines.LARGESIZE = 8192
 code = '''
+    lfs_t lfs;
     #define COUNT 5
     const struct {
         lfs_off_t startsizes[COUNT];
         lfs_off_t startseeks[COUNT];
         lfs_off_t hotsizes[COUNT];
         lfs_off_t coldsizes[COUNT];
     } configs[] = {
@@ -308,24 +350,27 @@
     };
 
     const lfs_off_t *startsizes = configs[CONFIG].startsizes;
     const lfs_off_t *startseeks = configs[CONFIG].startseeks;
     const lfs_off_t *hotsizes   = configs[CONFIG].hotsizes;
     const lfs_off_t *coldsizes  = configs[CONFIG].coldsizes;
 
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     for (unsigned i = 0; i < COUNT; i++) {
+        char path[1024];
         sprintf(path, "hairyhead%d", i);
+        lfs_file_t file;
         lfs_file_open(&lfs, &file, path,
                 LFS_O_WRONLY | LFS_O_CREAT | LFS_O_TRUNC) => 0;
 
+        uint8_t buffer[1024];
         strcpy((char*)buffer, "hair");
-        size = strlen((char*)buffer);
+        size_t size = strlen((char*)buffer);
         for (lfs_off_t j = 0; j < startsizes[i]; j += size) {
             lfs_file_write(&lfs, &file, buffer, size) => size;
         }
         lfs_file_size(&lfs, &file) => startsizes[i];
 
         if (startseeks[i] != startsizes[i]) {
             lfs_file_seek(&lfs, &file,
@@ -336,104 +381,119 @@
         lfs_file_size(&lfs, &file) => hotsizes[i];
 
         lfs_file_close(&lfs, &file) => 0;
     }
 
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     for (unsigned i = 0; i < COUNT; i++) {
+        char path[1024];
         sprintf(path, "hairyhead%d", i);
+        lfs_file_t file;
         lfs_file_open(&lfs, &file, path, LFS_O_RDWR) => 0;
         lfs_file_size(&lfs, &file) => hotsizes[i];
 
-        size = strlen("hair");
+        size_t size = strlen("hair");
         lfs_off_t j = 0;
         for (; j < startsizes[i] && j < hotsizes[i]; j += size) {
+            uint8_t buffer[1024];
             lfs_file_read(&lfs, &file, buffer, size) => size;
             memcmp(buffer, "hair", size) => 0;
         }
 
         for (; j < hotsizes[i]; j += size) {
+            uint8_t buffer[1024];
             lfs_file_read(&lfs, &file, buffer, size) => size;
             memcmp(buffer, "\0\0\0\0", size) => 0;
         }
 
         lfs_file_truncate(&lfs, &file, coldsizes[i]) => 0;
         lfs_file_size(&lfs, &file) => coldsizes[i];
 
         lfs_file_close(&lfs, &file) => 0;
     }
 
     lfs_unmount(&lfs) => 0;
 
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
 
     for (unsigned i = 0; i < COUNT; i++) {
+        char path[1024];
         sprintf(path, "hairyhead%d", i);
+        lfs_file_t file;
         lfs_file_open(&lfs, &file, path, LFS_O_RDONLY) => 0;
         lfs_file_size(&lfs, &file) => coldsizes[i];
 
-        size = strlen("hair");
+        size_t size = strlen("hair");
         lfs_off_t j = 0;
         for (; j < startsizes[i] && j < hotsizes[i] && j < coldsizes[i];
                 j += size) {
+            uint8_t buffer[1024];
             lfs_file_read(&lfs, &file, buffer, size) => size;
             memcmp(buffer, "hair", size) => 0;
         }
 
         for (; j < coldsizes[i]; j += size) {
+            uint8_t buffer[1024];
             lfs_file_read(&lfs, &file, buffer, size) => size;
             memcmp(buffer, "\0\0\0\0", size) => 0;
         }
 
         lfs_file_close(&lfs, &file) => 0;
     }
 
     lfs_unmount(&lfs) => 0;
 '''
 
-[[case]] # noop truncate
-define.MEDIUMSIZE = [32, 2048]
+# noop truncate
+[cases.test_truncate_nop]
+defines.MEDIUMSIZE = [32, 33, 512, 513, 2048, 2049, 8192, 8193]
 code = '''
-    lfs_format(&lfs, &cfg) => 0;
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
+    lfs_file_t file;
     lfs_file_open(&lfs, &file, "baldynoop",
             LFS_O_RDWR | LFS_O_CREAT) => 0;
 
+    uint8_t buffer[1024];
     strcpy((char*)buffer, "hair");
-    size = strlen((char*)buffer);
+    size_t size = strlen((char*)buffer);
     for (lfs_off_t j = 0; j < MEDIUMSIZE; j += size) {
-        lfs_file_write(&lfs, &file, buffer, size) => size;
+        lfs_file_write(&lfs, &file, buffer, lfs_min(size, MEDIUMSIZE-j))
+                => lfs_min(size, MEDIUMSIZE-j);
 
         // this truncate should do nothing
-        lfs_file_truncate(&lfs, &file, j+size) => 0;
+        lfs_file_truncate(&lfs, &file, j+lfs_min(size, MEDIUMSIZE-j)) => 0;
     }
     lfs_file_size(&lfs, &file) => MEDIUMSIZE;
 
     lfs_file_seek(&lfs, &file, 0, LFS_SEEK_SET) => 0;
     // should do nothing again
     lfs_file_truncate(&lfs, &file, MEDIUMSIZE) => 0;
     lfs_file_size(&lfs, &file) => MEDIUMSIZE;
 
     for (lfs_off_t j = 0; j < MEDIUMSIZE; j += size) {
-        lfs_file_read(&lfs, &file, buffer, size) => size;
-        memcmp(buffer, "hair", size) => 0;
+        lfs_file_read(&lfs, &file, buffer, lfs_min(size, MEDIUMSIZE-j))
+                => lfs_min(size, MEDIUMSIZE-j);
+        memcmp(buffer, "hair", lfs_min(size, MEDIUMSIZE-j)) => 0;
     }
     lfs_file_read(&lfs, &file, buffer, size) => 0;
 
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 
     // still there after reboot?
-    lfs_mount(&lfs, &cfg) => 0;
+    lfs_mount(&lfs, cfg) => 0;
     lfs_file_open(&lfs, &file, "baldynoop", LFS_O_RDWR) => 0;
     lfs_file_size(&lfs, &file) => MEDIUMSIZE;
     for (lfs_off_t j = 0; j < MEDIUMSIZE; j += size) {
-        lfs_file_read(&lfs, &file, buffer, size) => size;
-        memcmp(buffer, "hair", size) => 0;
+        lfs_file_read(&lfs, &file, buffer, lfs_min(size, MEDIUMSIZE-j))
+                => lfs_min(size, MEDIUMSIZE-j);
+        memcmp(buffer, "hair", lfs_min(size, MEDIUMSIZE-j)) => 0;
     }
     lfs_file_read(&lfs, &file, buffer, size) => 0;
     lfs_file_close(&lfs, &file) => 0;
     lfs_unmount(&lfs) => 0;
 '''
```

### Comparing `littlefs-python-0.4.0/setup.py` & `littlefs-python-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     )
 ]
 
 
 
 setup_requires = [
     'setuptools_scm>=3.3.3',
-    'Cython>=0.29.13',
 ]
 
 HERE = path.abspath(path.dirname(__file__))
 with open(path.join(HERE, 'README.rst'), encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
```

### Comparing `littlefs-python-0.4.0/src/littlefs/__init__.py` & `littlefs-python-0.5.0/src/littlefs/__init__.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/src/littlefs/context.py` & `littlefs-python-0.5.0/src/littlefs/context.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/src/littlefs/errors.py` & `littlefs-python-0.5.0/src/littlefs/errors.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/src/littlefs/lfs.c` & `littlefs-python-0.5.0/src/littlefs/lfs.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "LFS_NO_DEBUG",
@@ -42,16 +42,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -111,24 +111,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -236,15 +240,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -275,15 +279,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -585,35 +589,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1281,26 +1285,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -9500,15 +9504,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_8littlefs_3lfs_LFSFilesystem(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -9598,15 +9602,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_8littlefs_3lfs_LFSFile(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -9705,15 +9709,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_8littlefs_3lfs_LFSDirectory(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -9803,15 +9807,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_8littlefs_3lfs___pyx_scope_struct__file_open *__pyx_freelist_8littlefs_3lfs___pyx_scope_struct__file_open[8];
 static int __pyx_freecount_8littlefs_3lfs___pyx_scope_struct__file_open = 0;
 
@@ -9921,15 +9925,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_8littlefs_3lfs___pyx_scope_struct_1_genexpr *__pyx_freelist_8littlefs_3lfs___pyx_scope_struct_1_genexpr[8];
 static int __pyx_freecount_8littlefs_3lfs___pyx_scope_struct_1_genexpr = 0;
 
@@ -10038,15 +10042,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -10700,15 +10704,15 @@
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   __pyx_umethod_PyDict_Type_get.type = (PyObject*)&PyDict_Type;
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_8 = PyInt_FromLong(8); if (unlikely(!__pyx_int_8)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_64 = PyInt_FromLong(64); if (unlikely(!__pyx_int_64)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_128 = PyInt_FromLong(128); if (unlikely(!__pyx_int_128)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
@@ -11004,15 +11008,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_littlefs__lfs) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -11947,17 +11951,15 @@
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
 #ifdef WITH_THREAD
     PyGILState_STATE state;
     if (nogil)
         state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
-#endif
+    else state = (PyGILState_STATE)0;
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
     if (full_traceback) {
         Py_XINCREF(old_exc);
         Py_XINCREF(old_val);
         Py_XINCREF(old_tb);
@@ -12265,28 +12267,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -12497,19 +12499,19 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg) {
     if (likely(cfunc->func)) {
         int flag = cfunc->flag;
         if (flag == METH_O) {
             return (*(cfunc->func))(self, arg);
         } else if (PY_VERSION_HEX >= 0x030600B1 && flag == METH_FASTCALL) {
-            if (PY_VERSION_HEX >= 0x030700A0) {
+            #if PY_VERSION_HEX >= 0x030700A0
                 return (*(__Pyx_PyCFunctionFast)(void*)(PyCFunction)cfunc->func)(self, &arg, 1);
-            } else {
+            #else
                 return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
-            }
+            #endif
         } else if (PY_VERSION_HEX >= 0x030700A0 && flag == (METH_FASTCALL | METH_KEYWORDS)) {
             return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
         }
     }
     return __Pyx__CallUnboundCMethod1(cfunc, self, arg);
 }
 #endif
@@ -13051,15 +13053,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -13550,15 +13552,15 @@
     }
     Py_XDECREF(owned_metaclass);
     return result;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -13973,15 +13975,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -14169,15 +14171,15 @@
                         } else if (8 * sizeof(uint32_t) >= 4 * PyLong_SHIFT) {
                             return (uint32_t) (((((((((uint32_t)digits[3]) << PyLong_SHIFT) | (uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -14365,15 +14367,15 @@
                         } else if (8 * sizeof(int32_t) >= 4 * PyLong_SHIFT) {
                             return (int32_t) (((((((((int32_t)digits[3]) << PyLong_SHIFT) | (int32_t)digits[2]) << PyLong_SHIFT) | (int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -14637,15 +14639,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -16006,15 +16008,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
```

### Comparing `littlefs-python-0.4.0/src/littlefs/lfs.pxd` & `littlefs-python-0.5.0/src/littlefs/lfs.pxd`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/src/littlefs/lfs.pyi` & `littlefs-python-0.5.0/src/littlefs/lfs.pyi`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/src/littlefs/lfs.pyx` & `littlefs-python-0.5.0/src/littlefs/lfs.pyx`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/src/littlefs_python.egg-info/PKG-INFO` & `littlefs-python-0.5.0/src/littlefs_python.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,143 +1,159 @@
 Metadata-Version: 2.1
 Name: littlefs-python
-Version: 0.4.0
+Version: 0.5.0
 Summary: A python wrapper for littlefs
 Home-page: https://github.com/jrast/littlefs-python
 Author: Jürg Rast
 Author-email: juergr@gmail.com
 License: UNKNOWN
-Description: ===================
-        littlefs for Python
-        ===================
-        
-        .. image:: https://readthedocs.org/projects/littlefs-python/badge/?version=latest
-            :target: https://littlefs-python.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://badge.fury.io/py/littlefs-python.svg
-            :target: https://badge.fury.io/py/littlefs-python
-        
-        littlefs-python provides a thin wrapper around littlefs_, a filesystem targeted for
-        small embedded systems.
-        The wrapper provides a pythonic interface to the filesystem and allows the creation,
-        inspection and modification of the filesystem or individual files.
-        Even if this package uses Cython_, the goal is not to provide a high performance
-        implementation. Cython was chosen as an easy method is offered to generate the binding
-        and the littlefs library in one step.
-        
-        Quick Examples
-        ==============
-        Let's create a image ready to transfer to a flash memory using the pythonic interface:
-        
-        .. code:: python
-        
-            from littlefs import LittleFS
-        
-            # Initialize the File System according to your specifications
-            fs = LittleFS(block_size=512, block_count=256)
-        
-            # Open a file and write some content
-            with fs.open('first-file.txt', 'w') as fh:
-                fh.write('Some text to begin with\n')
-        
-            # Dump the filesystem content to a file
-            with open('FlashMemory.bin', 'wb') as fh:
-                fh.write(fs.context.buffer)
-        
-        The same can be done by using the more verbose C-Style API, which closely resembles the
-        steps which must be performed in C:
-        
-        .. code:: python
-        
-            from littlefs import lfs
-        
-            cfg = lfs.LFSConfig(block_size=512, block_count=256)
-            fs = lfs.LFSFilesystem()
-        
-            # Format and mount the filesystem
-            lfs.format(fs, cfg)
-            lfs.mount(fs, cfg)
-        
-            # Open a file and write some content
-            fh = lfs.file_open(fs, 'first-file.txt', 'w')
-            lfs.file_write(fs, fh, b'Some text to begin with\n')
-            lfs.file_close(fs, fh)
-        
-            # Dump the filesystem content to a file
-            with open('FlashMemory.bin', 'wb') as fh:
-                fh.write(cfg.user_context.buffer)
-        
-        
-        Installation
-        ============
-        
-        This is as simple as it can be::
-        
-            pip install littlefs-python
-        
-        At the moment wheels (which require no build) are provided for the following platforms,
-        on other platforms the source package is used and a compiler is required:
-        
-         - Linux: Python 3.6 - 3.10 / 32- & 64-bit
-         - Windows: Python 3.6 - 3.10 / 32- & 64-bit
-        
-        
-        Development Setup
-        =================
-        
-        Start by checking out the source repository of littlefs-python::
-        
-            git clone https://github.com/jrast/littlefs-python.git
-        
-        The source code for littlefs is included as a submodule which must be
-        checked out after the clone::
-        
-            cd <littlefs-python>
-            git submodule update --init
-        
-        this ensures that the correct version of littlefs_ is cloned into
-        the littlefs folder. As a next step install the dependencies and install
-        the package::
-        
-            pip install -r requirements.txt
-            pip install -e .
-        
-        .. note::
-            It's highly recommended to install the package in a virtual environment!
-        
-        
-        Development Hints
-        -----------------
-        
-        - Test should be run before commiting: `pytest test`
-        - Mypy is used for typechecking. Run it also on the tests to catch more issues:
-          `mypy src test test/lfs`
-        - Mypy stubs can be generated with `stubgen src`. This will create a `out` direcotry
-          containing the generated stub files.
-        
-        
-        Creating a new release
-        ======================
-        
-        - Make sure the master branch is in the state you want it.
-        - Create a tag with the new version number
-        - Wait until all builds are completed. A new release should be created
-          automatically on github.
-        - Build the source distribution with `python setup.py sdist`
-        - Download all assets (using `ci/download_release_files.py`)
-        - Upload to pypi using twine: `twine upload dist/*`
-        
-        
-        
-        .. _littlefs: https://github.com/littlefs-project/littlefs
-        .. _Cython: http://docs.cython.org/en/latest/index.html
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Filesystems
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+===================
+littlefs for Python
+===================
+
+.. image:: https://readthedocs.org/projects/littlefs-python/badge/?version=latest
+    :target: https://littlefs-python.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://badge.fury.io/py/littlefs-python.svg
+    :target: https://badge.fury.io/py/littlefs-python
+
+littlefs-python provides a thin wrapper around littlefs_, a filesystem targeted for
+small embedded systems.
+The wrapper provides a pythonic interface to the filesystem and allows the creation,
+inspection and modification of the filesystem or individual files.
+Even if this package uses Cython_, the goal is not to provide a high performance
+implementation. Cython was chosen as an easy method is offered to generate the binding
+and the littlefs library in one step.
+
+Quick Examples
+==============
+Let's create a image ready to transfer to a flash memory using the pythonic interface:
+
+.. code:: python
+
+    from littlefs import LittleFS
+
+    # Initialize the File System according to your specifications
+    fs = LittleFS(block_size=512, block_count=256)
+
+    # Open a file and write some content
+    with fs.open('first-file.txt', 'w') as fh:
+        fh.write('Some text to begin with\n')
+
+    # Dump the filesystem content to a file
+    with open('FlashMemory.bin', 'wb') as fh:
+        fh.write(fs.context.buffer)
+
+The same can be done by using the more verbose C-Style API, which closely resembles the
+steps which must be performed in C:
+
+.. code:: python
+
+    from littlefs import lfs
+
+    cfg = lfs.LFSConfig(block_size=512, block_count=256)
+    fs = lfs.LFSFilesystem()
+
+    # Format and mount the filesystem
+    lfs.format(fs, cfg)
+    lfs.mount(fs, cfg)
+
+    # Open a file and write some content
+    fh = lfs.file_open(fs, 'first-file.txt', 'w')
+    lfs.file_write(fs, fh, b'Some text to begin with\n')
+    lfs.file_close(fs, fh)
+
+    # Dump the filesystem content to a file
+    with open('FlashMemory.bin', 'wb') as fh:
+        fh.write(cfg.user_context.buffer)
+
+
+Installation
+============
+
+.. note::
+    As littlefs_ is bundled with the package you will need to install the correct version of
+    this package in successfully read or create images for your embedded system. If you start
+    from scratch the latest version is recommeded.
+
+    .. csv-table::
+        :header: "Package Version", "LittleFS Version", "LittleFS File System Version"
+
+        0.6.0, 2.6.1, 2.1
+        0.5.0, 2.4.1, 2.0
+        0.4.0, 2.2.1, 2.0
+
+
+This is as simple as it can be::
+
+    pip install littlefs-python
+
+At the moment wheels (which require no build) are provided for the following platforms,
+on other platforms the source package is used and a compiler is required:
+
+ - Linux: Python 3.6 - 3.10 / 32- & 64-bit
+ - Windows: Python 3.6 - 3.10 / 32- & 64-bit
+
+
+Development Setup
+=================
+
+Start by checking out the source repository of littlefs-python::
+
+    git clone https://github.com/jrast/littlefs-python.git
+
+The source code for littlefs is included as a submodule which must be
+checked out after the clone::
+
+    cd <littlefs-python>
+    git submodule update --init
+
+this ensures that the correct version of littlefs_ is cloned into
+the littlefs folder. As a next step install the dependencies and install
+the package::
+
+    pip install -r requirements.txt
+    pip install -e .
+
+.. note::
+    It's highly recommended to install the package in a virtual environment!
+
+
+Development Hints
+-----------------
+
+- Test should be run before commiting: `pytest test`
+- Mypy is used for typechecking. Run it also on the tests to catch more issues:
+  `mypy src test test/lfs`
+- Mypy stubs can be generated with `stubgen src`. This will create a `out` direcotry
+  containing the generated stub files.
+
+
+Creating a new release
+======================
+
+- Make sure the master branch is in the state you want it.
+- Create a tag with the new version number
+- Wait until all builds are completed. A new release should be created
+  automatically on github.
+- Build the source distribution with `python setup.py sdist`
+- Download all assets (using `ci/download_release_files.py`)
+- Upload to pypi using twine: `twine upload dist/*`
+
+
+
+.. _littlefs: https://github.com/littlefs-project/littlefs
+.. _Cython: http://docs.cython.org/en/latest/index.html
+
+
```

### Comparing `littlefs-python-0.4.0/src/littlefs_python.egg-info/SOURCES.txt` & `littlefs-python-0.5.0/src/littlefs_python.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitattributes
 .gitignore
 .gitmodules
 LICENSE
 MANIFEST.in
 README.rst
 mypy.ini
+pyproject.toml
 requirements.txt
 setup.py
 .github/dependabot.yml
 .github/workflows/deploy.yml
 .github/workflows/run-tests.yml
 ci/build-wheels.sh
 ci/download_release_files.py
@@ -19,54 +20,78 @@
 docs/make.bat
 docs/usage.rst
 docs/api/index.rst
 docs/examples/index.rst
 examples/mkfsimg.py
 examples/walk.py
 littlefs/.git
+littlefs/.gitattributes
 littlefs/.gitignore
 littlefs/DESIGN.md
 littlefs/LICENSE.md
 littlefs/Makefile
 littlefs/README.md
 littlefs/SPEC.md
 littlefs/lfs.c
 littlefs/lfs.h
 littlefs/lfs_util.c
 littlefs/lfs_util.h
 littlefs/.github/workflows/post-release.yml
 littlefs/.github/workflows/release.yml
 littlefs/.github/workflows/status.yml
 littlefs/.github/workflows/test.yml
+littlefs/bd/lfs_emubd.c
+littlefs/bd/lfs_emubd.h
 littlefs/bd/lfs_filebd.c
 littlefs/bd/lfs_filebd.h
 littlefs/bd/lfs_rambd.c
 littlefs/bd/lfs_rambd.h
-littlefs/bd/lfs_testbd.c
-littlefs/bd/lfs_testbd.h
+littlefs/benches/bench_dir.toml
+littlefs/benches/bench_file.toml
+littlefs/benches/bench_superblock.toml
+littlefs/runners/bench_runner.c
+littlefs/runners/bench_runner.h
+littlefs/runners/test_runner.c
+littlefs/runners/test_runner.h
+littlefs/scripts/bench.py
+littlefs/scripts/changeprefix.py
 littlefs/scripts/code.py
-littlefs/scripts/coverage.py
-littlefs/scripts/explode_asserts.py
-littlefs/scripts/prefix.py
+littlefs/scripts/cov.py
+littlefs/scripts/data.py
+littlefs/scripts/perf.py
+littlefs/scripts/perfbd.py
+littlefs/scripts/plot.py
+littlefs/scripts/plotmpl.py
+littlefs/scripts/prettyasserts.py
 littlefs/scripts/readblock.py
 littlefs/scripts/readmdir.py
 littlefs/scripts/readtree.py
+littlefs/scripts/stack.py
+littlefs/scripts/structs.py
+littlefs/scripts/summary.py
+littlefs/scripts/tailpipe.py
+littlefs/scripts/teepipe.py
 littlefs/scripts/test.py
+littlefs/scripts/tracebd.py
+littlefs/scripts/watch.py
 littlefs/tests/test_alloc.toml
 littlefs/tests/test_attrs.toml
 littlefs/tests/test_badblocks.toml
+littlefs/tests/test_bd.toml
+littlefs/tests/test_compat.toml
 littlefs/tests/test_dirs.toml
 littlefs/tests/test_entries.toml
 littlefs/tests/test_evil.toml
 littlefs/tests/test_exhaustion.toml
 littlefs/tests/test_files.toml
 littlefs/tests/test_interspersed.toml
 littlefs/tests/test_move.toml
 littlefs/tests/test_orphans.toml
 littlefs/tests/test_paths.toml
+littlefs/tests/test_powerloss.toml
 littlefs/tests/test_relocations.toml
 littlefs/tests/test_seek.toml
 littlefs/tests/test_superblocks.toml
 littlefs/tests/test_truncate.toml
 src/littlefs/__init__.py
 src/littlefs/context.py
 src/littlefs/errors.py
```

### Comparing `littlefs-python-0.4.0/test/lfs/conftest.py` & `littlefs-python-0.5.0/test/lfs/conftest.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/test/lfs/test_dir_functions.py` & `littlefs-python-0.5.0/test/lfs/test_dir_functions.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/test/lfs/test_file_functions.py` & `littlefs-python-0.5.0/test/lfs/test_file_functions.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/test/lfs/test_fs_functions.py` & `littlefs-python-0.5.0/test/lfs/test_fs_functions.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/test/test_directories.py` & `littlefs-python-0.5.0/test/test_directories.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/test/test_files.py` & `littlefs-python-0.5.0/test/test_files.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/test/test_remove_rename.py` & `littlefs-python-0.5.0/test/test_remove_rename.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.4.0/test/test_walk.py` & `littlefs-python-0.5.0/test/test_walk.py`

 * *Files identical despite different names*

