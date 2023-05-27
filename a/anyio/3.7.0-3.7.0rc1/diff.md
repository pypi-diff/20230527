# Comparing `tmp/anyio-3.7.0.tar.gz` & `tmp/anyio-3.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyio-3.7.0.tar", last modified: Sat May 27 11:12:31 2023, max compression
+gzip compressed data, was "anyio-3.7.0rc1.tar", last modified: Thu May 18 16:06:13 2023, max compression
```

## Comparing `anyio-3.7.0.tar` & `anyio-3.7.0rc1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:31.510136 anyio-3.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:31.498136 anyio-3.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:31.498136 anyio-3.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-27 11:12:17.000000 anyio-3.7.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-27 11:12:17.000000 anyio-3.7.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-27 11:12:17.000000 anyio-3.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-27 11:12:17.000000 anyio-3.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-27 11:12:17.000000 anyio-3.7.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-27 11:12:17.000000 anyio-3.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-27 11:12:31.510136 anyio-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-27 11:12:17.000000 anyio-3.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:31.502136 anyio-3.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/cancellation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/fileio.rst
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/networking.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/signals.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/streams.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/subprocesses.rst
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/support.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/synchronization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/tasks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/threads.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/typedattrs.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34211 2023-05-27 11:12:17.000000 anyio-3.7.0/docs/versionhistory.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-27 11:12:17.000000 anyio-3.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 11:12:31.510136 anyio-3.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:31.498136 anyio-3.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:31.502136 anyio-3.7.0/src/anyio/
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:31.506136 anyio-3.7.0/src/anyio/_backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67056 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/_backends/_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    30035 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/_backends/_trio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:31.506136 anyio-3.7.0/src/anyio/_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/_core/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/_core/_eventloop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/_core/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18026 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/_core/_fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/_core/_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/_core/_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    20667 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/_core/_sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/_core/_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/_core/_subprocesses.py
--rw-r--r--   0 runner    (1001) docker     (123)    16729 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/_core/_synchronization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/_core/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/_core/_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/_core/_typedattr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:31.506136 anyio-3.7.0/src/anyio/abc/
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/abc/_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/abc/_sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/abc/_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/abc/_subprocesses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/abc/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/abc/_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    16435 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/from_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/lowlevel.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/pytest_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:31.506136 anyio-3.7.0/src/anyio/streams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/streams/buffered.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/streams/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/streams/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/streams/stapled.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/streams/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/streams/tls.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/to_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-27 11:12:17.000000 anyio-3.7.0/src/anyio/to_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:31.502136 anyio-3.7.0/src/anyio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-27 11:12:31.000000 anyio-3.7.0/src/anyio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-27 11:12:31.000000 anyio-3.7.0/src/anyio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:12:31.000000 anyio-3.7.0/src/anyio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-27 11:12:31.000000 anyio-3.7.0/src/anyio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-27 11:12:31.000000 anyio-3.7.0/src/anyio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 11:12:31.000000 anyio-3.7.0/src/anyio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:31.510136 anyio-3.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:31.510136 anyio-3.7.0/tests/streams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/streams/test_buffered.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/streams/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/streams/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/streams/test_stapled.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/streams/test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    18830 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/streams/test_tls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/test_debugging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/test_eventloop.py
--rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/test_fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/test_from_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/test_lowlevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/test_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    51369 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/test_sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/test_subprocesses.py
--rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/test_synchronization.py
--rw-r--r--   0 runner    (1001) docker     (123)    34173 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/test_taskgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/test_to_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-05-27 11:12:17.000000 anyio-3.7.0/tests/test_to_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.609362 anyio-3.7.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.597363 anyio-3.7.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.597363 anyio-3.7.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-18 16:06:13.609362 anyio-3.7.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.601363 anyio-3.7.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/cancellation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/fileio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/networking.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/signals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/streams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/subprocesses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/support.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/synchronization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/tasks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/threads.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/typedattrs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34214 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/versionhistory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 16:06:13.609362 anyio-3.7.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.597363 anyio-3.7.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.601363 anyio-3.7.0rc1/src/anyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.601363 anyio-3.7.0rc1/src/anyio/_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67067 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_backends/_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30046 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_backends/_trio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.605363 anyio-3.7.0rc1/src/anyio/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18026 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20667 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_subprocesses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16754 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_typedattr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.605363 anyio-3.7.0rc1/src/anyio/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/_subprocesses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16435 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/from_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/lowlevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/pytest_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.605363 anyio-3.7.0rc1/src/anyio/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/buffered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/stapled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/to_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/to_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.601363 anyio-3.7.0rc1/src/anyio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-18 16:06:13.000000 anyio-3.7.0rc1/src/anyio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-18 16:06:13.000000 anyio-3.7.0rc1/src/anyio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:06:13.000000 anyio-3.7.0rc1/src/anyio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-18 16:06:13.000000 anyio-3.7.0rc1/src/anyio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-18 16:06:13.000000 anyio-3.7.0rc1/src/anyio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 16:06:13.000000 anyio-3.7.0rc1/src/anyio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.605363 anyio-3.7.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.609362 anyio-3.7.0rc1/tests/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/test_buffered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/test_stapled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18830 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/test_tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_debugging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_from_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_lowlevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51369 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_subprocesses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34173 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_taskgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_to_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_to_thread.py
```

### Comparing `anyio-3.7.0/.github/workflows/publish.yml` & `anyio-3.7.0rc1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/.github/workflows/test.yml` & `anyio-3.7.0rc1/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
       run: pyright --verifytypes anyio
 
   test:
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", pypy-3.9]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", pypy-3.8]
         include:
         - os: macos-latest
           python-version: "3.7"
         - os: macos-latest
           python-version: "3.11"
         - os: windows-latest
           python-version: "3.7"
@@ -41,19 +41,18 @@
     runs-on: ${{ matrix.os }}
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
-        allow-prereleases: true
         cache: pip
         cache-dependency-path: setup.cfg
     - name: Install dependencies
-      run: pip install -e .[test] coveralls
+      run: pip install .[test,trio] coveralls
     - name: Test with pytest
       run: coverage run -m pytest -v
       timeout-minutes: 5
       env:
         PYTEST_DISABLE_PLUGIN_AUTOLOAD: 1
     - name: Upload Coverage
       run: coveralls --service=github
```

### Comparing `anyio-3.7.0/.pre-commit-config.yaml` & `anyio-3.7.0rc1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,25 @@
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [ "--fix=lf" ]
       - id: trailing-whitespace
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.270
+    rev: v0.0.265
     hooks:
       - id: ruff
         args: [--fix, --show-fixes]
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.3.0
+    rev: v1.2.0
     hooks:
       - id: mypy
         additional_dependencies:
           - pytest
           - trio-typing >= 0.8.0
           - packaging
```

### Comparing `anyio-3.7.0/LICENSE` & `anyio-3.7.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/PKG-INFO` & `anyio-3.7.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: anyio
-Version: 3.7.0
+Version: 3.7.0rc1
 Summary: High level compatibility layer for multiple asynchronous event loop implementations
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://anyio.readthedocs.io/en/latest/
 Project-URL: Changelog, https://anyio.readthedocs.io/en/stable/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/anyio
 Project-URL: Issue tracker, https://github.com/agronholm/anyio/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: AnyIO
-Classifier: Typing :: Typed
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `anyio-3.7.0/README.rst` & `anyio-3.7.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/docs/api.rst` & `anyio-3.7.0rc1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/docs/basics.rst` & `anyio-3.7.0rc1/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/docs/cancellation.rst` & `anyio-3.7.0rc1/docs/cancellation.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/docs/conf.py` & `anyio-3.7.0rc1/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from packaging.version import parse
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx_autodoc_typehints",
-    "sphinxcontrib.jquery",
 ]
 
 templates_path = ["_templates"]
 source_suffix = ".rst"
 master_doc = "index"
 project = "AnyIO"
 author = "Alex Grönholm"
@@ -24,14 +23,13 @@
 release = v.public
 
 language = "en"
 
 exclude_patterns = ["_build"]
 pygments_style = "sphinx"
 autodoc_default_options = {"members": True, "show-inheritance": True}
-autodoc_mock_imports = ["_typeshed"]
 todo_include_todos = False
 
 html_theme = "sphinx_rtd_theme"
 htmlhelp_basename = "anyiodoc"
 
 intersphinx_mapping = {"python": ("https://docs.python.org/3/", None)}
```

### Comparing `anyio-3.7.0/docs/contributing.rst` & `anyio-3.7.0rc1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/docs/faq.rst` & `anyio-3.7.0rc1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/docs/fileio.rst` & `anyio-3.7.0rc1/docs/fileio.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/docs/migration.rst` & `anyio-3.7.0rc1/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/docs/networking.rst` & `anyio-3.7.0rc1/docs/networking.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/docs/signals.rst` & `anyio-3.7.0rc1/docs/signals.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/docs/streams.rst` & `anyio-3.7.0rc1/docs/streams.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/docs/subprocesses.rst` & `anyio-3.7.0rc1/docs/subprocesses.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/docs/support.rst` & `anyio-3.7.0rc1/docs/support.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/docs/synchronization.rst` & `anyio-3.7.0rc1/docs/synchronization.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/docs/tasks.rst` & `anyio-3.7.0rc1/docs/tasks.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/docs/testing.rst` & `anyio-3.7.0rc1/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/docs/threads.rst` & `anyio-3.7.0rc1/docs/threads.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/docs/typedattrs.rst` & `anyio-3.7.0rc1/docs/typedattrs.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/docs/versionhistory.rst` & `anyio-3.7.0rc1/docs/versionhistory.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Version history
 ===============
 
 This library adheres to `Semantic Versioning 2.0 <http://semver.org/>`_.
 
-**3.7.0**
+**3.7.0rc1**
 
 - Dropped support for Python 3.6
 - Improved type annotations:
 
   - Several functions and methods that were previously annotated as accepting
     ``Coroutine[Any, Any, Any]`` as the return type of the callable have been amended to
     accept ``Awaitable[Any]`` instead, to allow a slightly broader set of coroutine-like
```

### Comparing `anyio-3.7.0/pyproject.toml` & `anyio-3.7.0rc1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 authors = [{name = "Alex Grönholm", email = "alex.gronholm@nextday.fi"}]
 license = {text = "MIT"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Framework :: AnyIO",
-    "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -47,21 +46,20 @@
     "mock >= 4; python_version < '3.8'",
     "coverage[toml] >= 4.5",
     "hypothesis >= 4.0",
     "psutil >= 5.9",
     "pytest >= 7.0",
     "pytest-mock >= 3.6.1",
     "trustme",
-    "uvloop >= 0.17; python_version < '3.12' and platform_python_implementation == 'CPython' and platform_system != 'Windows'",
+    "uvloop >= 0.17; platform_python_implementation == 'CPython' and platform_system != 'Windows'",
 ]
 doc = [
     "packaging",
     "Sphinx >= 6.1.0",
     "sphinx_rtd_theme",
-    "sphinxcontrib-jquery",
     "sphinx-autodoc-typehints >= 1.2.0",
 ]
 
 [project.entry-points]
 pytest11 = {anyio = "anyio.pytest_plugin"}
 
 [tool.setuptools_scm]
@@ -99,17 +97,14 @@
 addopts = "-rsx --tb=short --strict-config --strict-markers -p anyio -p no:asyncio -p no:trio"
 testpaths = ["tests"]
 # Ignore resource warnings due to a CPython/Windows bug (https://bugs.python.org/issue44428)
 filterwarnings = [
     "error",
     "ignore:unclosed <socket.socket.*:ResourceWarning",
     "ignore:unclosed transport <_ProactorSocketTransport.*:ResourceWarning",
-    "ignore:ast.Str is deprecated:DeprecationWarning",
-    "ignore:Attribute s is deprecated:DeprecationWarning",
-    "ignore:ast.NameConstant is deprecated:DeprecationWarning",
     # Workaround for Python 3.9.7 (see https://bugs.python.org/issue45097)
     "ignore:The loop argument is deprecated since Python 3\\.8, and scheduled for removal in Python 3\\.10\\.:DeprecationWarning:asyncio",
 ]
 markers = [
     "network: marks tests as requiring Internet access",
 ]
 
@@ -119,33 +114,36 @@
 
 [tool.coverage.report]
 show_missing = true
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
+minversion = 4.0.0
 envlist = pre-commit, py37, py38, py39, py310, py311, pypy3
 skip_missing_interpreters = true
-minversion = 4.4.3
 
 [testenv]
 depends = pre-commit
 package = editable
 commands = coverage run -m pytest {posargs}
-extras = test
+extras =
+    test
+    trio
 
 [testenv:pre-commit]
 depends =
 basepython = python3
 package = skip
 deps = pre-commit
 commands = pre-commit run --all-files
 
 [testenv:pyright]
 deps = pyright
 commands = pyright --verifytypes anyio
+package = editable
 
 [testenv:docs]
 depends =
 extras = doc
-commands = sphinx-build -W -n docs build/sphinx
+commands = sphinx-build docs build/sphinx
 """
```

### Comparing `anyio-3.7.0/src/anyio/__init__.py` & `anyio-3.7.0rc1/src/anyio/__init__.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/_backends/_asyncio.py` & `anyio-3.7.0rc1/src/anyio/_backends/_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     IO,
     Any,
     AsyncGenerator,
     Awaitable,
     Callable,
     Collection,
     Coroutine,
+    Deque,
     Generator,
     Iterable,
     Mapping,
     Optional,
     Sequence,
     Tuple,
     TypeVar,
@@ -755,15 +756,15 @@
 class WorkerThread(Thread):
     MAX_IDLE_TIME = 10  # seconds
 
     def __init__(
         self,
         root_task: asyncio.Task,
         workers: set[WorkerThread],
-        idle_workers: deque[WorkerThread],
+        idle_workers: Deque[WorkerThread],
     ):
         super().__init__(name="AnyIO worker thread")
         self.root_task = root_task
         self.workers = workers
         self.idle_workers = idle_workers
         self.loop = root_task._loop
         self.queue: Queue[
@@ -821,15 +822,15 @@
         self.workers.discard(self)
         try:
             self.idle_workers.remove(self)
         except ValueError:
             pass
 
 
-_threadpool_idle_workers: RunVar[deque[WorkerThread]] = RunVar(
+_threadpool_idle_workers: RunVar[Deque[WorkerThread]] = RunVar(
     "_threadpool_idle_workers"
 )
 _threadpool_workers: RunVar[set[WorkerThread]] = RunVar("_threadpool_workers")
 
 
 async def run_sync_in_worker_thread(
     func: Callable[..., T_Retval],
@@ -1109,15 +1110,15 @@
 
 #
 # Sockets and networking
 #
 
 
 class StreamProtocol(asyncio.Protocol):
-    read_queue: deque[bytes]
+    read_queue: Deque[bytes]
     read_event: asyncio.Event
     write_event: asyncio.Event
     exception: Exception | None = None
 
     def connection_made(self, transport: asyncio.BaseTransport) -> None:
         self.read_queue = deque()
         self.read_event = asyncio.Event()
@@ -1145,15 +1146,15 @@
         self.write_event = asyncio.Event()
 
     def resume_writing(self) -> None:
         self.write_event.set()
 
 
 class DatagramProtocol(asyncio.DatagramProtocol):
-    read_queue: deque[tuple[bytes, IPSockAddrType]]
+    read_queue: Deque[tuple[bytes, IPSockAddrType]]
     read_event: asyncio.Event
     write_event: asyncio.Event
     exception: Exception | None = None
 
     def connection_made(self, transport: asyncio.BaseTransport) -> None:
         self.read_queue = deque(maxlen=100)  # arbitrary value
         self.read_event = asyncio.Event()
@@ -1920,15 +1921,15 @@
 #
 
 
 class _SignalReceiver(DeprecatedAsyncContextManager["_SignalReceiver"]):
     def __init__(self, signals: tuple[int, ...]):
         self._signals = signals
         self._loop = get_running_loop()
-        self._signal_queue: deque[int] = deque()
+        self._signal_queue: Deque[int] = deque()
         self._future: asyncio.Future = asyncio.Future()
         self._handled_signals: set[int] = set()
 
     def _deliver(self, signum: int) -> None:
         self._signal_queue.append(signum)
         if not self._future.done():
             self._future.set_result(None)
```

### Comparing `anyio-3.7.0/src/anyio/_backends/_trio.py` & `anyio-3.7.0rc1/src/anyio/_backends/_trio.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     Any,
     AsyncGenerator,
     AsyncIterator,
     Awaitable,
     Callable,
     Collection,
     Coroutine,
+    Deque,
     Generic,
     Iterable,
     Mapping,
     NoReturn,
     Sequence,
     TypeVar,
     cast,
@@ -904,15 +905,15 @@
 
 class TestRunner(abc.TestRunner):
     def __init__(self, **options: Any) -> None:
         from collections import deque
         from queue import Queue
 
         self._call_queue: Queue[Callable[..., object]] = Queue()
-        self._result_queue: deque[Outcome] = deque()
+        self._result_queue: Deque[Outcome] = deque()
         self._stop_event: trio.Event | None = None
         self._nursery: trio.Nursery | None = None
         self._options = options
 
     async def _trio_main(self) -> None:
         self._stop_event = trio.Event()
         async with trio.open_nursery() as self._nursery:
```

### Comparing `anyio-3.7.0/src/anyio/_core/_compat.py` & `anyio-3.7.0rc1/src/anyio/_core/_compat.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/_core/_eventloop.py` & `anyio-3.7.0rc1/src/anyio/_core/_eventloop.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/_core/_exceptions.py` & `anyio-3.7.0rc1/src/anyio/_core/_exceptions.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/_core/_fileio.py` & `anyio-3.7.0rc1/src/anyio/_core/_fileio.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/_core/_signals.py` & `anyio-3.7.0rc1/src/anyio/_core/_signals.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/_core/_sockets.py` & `anyio-3.7.0rc1/src/anyio/_core/_sockets.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/_core/_streams.py` & `anyio-3.7.0rc1/src/anyio/_core/_streams.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/_core/_subprocesses.py` & `anyio-3.7.0rc1/src/anyio/_core/_subprocesses.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/_core/_synchronization.py` & `anyio-3.7.0rc1/src/anyio/_core/_synchronization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from collections import deque
 from dataclasses import dataclass
 from types import TracebackType
+from typing import Deque
 from warnings import warn
 
 from ..lowlevel import cancel_shielded_checkpoint, checkpoint, checkpoint_if_cancelled
 from ._compat import DeprecatedAwaitable
 from ._eventloop import get_asynclib
 from ._exceptions import BusyResourceError, WouldBlock
 from ._tasks import CancelScope
@@ -100,15 +101,15 @@
         raise NotImplementedError
 
 
 class Lock:
     _owner_task: TaskInfo | None = None
 
     def __init__(self) -> None:
-        self._waiters: deque[tuple[TaskInfo, Event]] = deque()
+        self._waiters: Deque[tuple[TaskInfo, Event]] = deque()
 
     async def __aenter__(self) -> None:
         await self.acquire()
 
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
@@ -188,15 +189,15 @@
 
 
 class Condition:
     _owner_task: TaskInfo | None = None
 
     def __init__(self, lock: Lock | None = None):
         self._lock = lock or Lock()
-        self._waiters: deque[Event] = deque()
+        self._waiters: Deque[Event] = deque()
 
     async def __aenter__(self) -> None:
         await self.acquire()
 
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
@@ -290,15 +291,15 @@
             if max_value < initial_value:
                 raise ValueError(
                     "max_value must be equal to or higher than initial_value"
                 )
 
         self._value = initial_value
         self._max_value = max_value
-        self._waiters: deque[Event] = deque()
+        self._waiters: Deque[Event] = deque()
 
     async def __aenter__(self) -> Semaphore:
         await self.acquire()
         return self
 
     async def __aexit__(
         self,
```

### Comparing `anyio-3.7.0/src/anyio/_core/_tasks.py` & `anyio-3.7.0rc1/src/anyio/_core/_tasks.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/_core/_testing.py` & `anyio-3.7.0rc1/src/anyio/_core/_testing.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/_core/_typedattr.py` & `anyio-3.7.0rc1/src/anyio/_core/_typedattr.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/abc/__init__.py` & `anyio-3.7.0rc1/src/anyio/abc/__init__.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/abc/_resources.py` & `anyio-3.7.0rc1/src/anyio/abc/_resources.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/abc/_sockets.py` & `anyio-3.7.0rc1/src/anyio/abc/_sockets.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/abc/_streams.py` & `anyio-3.7.0rc1/src/anyio/abc/_streams.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/abc/_subprocesses.py` & `anyio-3.7.0rc1/src/anyio/abc/_subprocesses.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/abc/_tasks.py` & `anyio-3.7.0rc1/src/anyio/abc/_tasks.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/abc/_testing.py` & `anyio-3.7.0rc1/src/anyio/abc/_testing.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/from_thread.py` & `anyio-3.7.0rc1/src/anyio/from_thread.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/lowlevel.py` & `anyio-3.7.0rc1/src/anyio/lowlevel.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/pytest_plugin.py` & `anyio-3.7.0rc1/src/anyio/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/streams/buffered.py` & `anyio-3.7.0rc1/src/anyio/streams/buffered.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/streams/file.py` & `anyio-3.7.0rc1/src/anyio/streams/file.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/streams/memory.py` & `anyio-3.7.0rc1/src/anyio/streams/memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from collections import OrderedDict, deque
 from dataclasses import dataclass, field
 from types import TracebackType
-from typing import Generic, NamedTuple, TypeVar
+from typing import Deque, Generic, NamedTuple, TypeVar
 
 from .. import (
     BrokenResourceError,
     ClosedResourceError,
     EndOfStream,
     WouldBlock,
     get_cancelled_exc_class,
@@ -31,15 +31,15 @@
     #: number of tasks blocked on :meth:`MemoryObjectReceiveStream.receive`
     tasks_waiting_receive: int
 
 
 @dataclass(eq=False)
 class MemoryObjectStreamState(Generic[T_Item]):
     max_buffer_size: float = field()
-    buffer: deque[T_Item] = field(init=False, default_factory=deque)
+    buffer: Deque[T_Item] = field(init=False, default_factory=deque)
     open_send_channels: int = field(init=False, default=0)
     open_receive_channels: int = field(init=False, default=0)
     waiting_receivers: OrderedDict[Event, list[T_Item]] = field(
         init=False, default_factory=OrderedDict
     )
     waiting_senders: OrderedDict[Event, T_Item] = field(
         init=False, default_factory=OrderedDict
```

### Comparing `anyio-3.7.0/src/anyio/streams/stapled.py` & `anyio-3.7.0rc1/src/anyio/streams/stapled.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/streams/text.py` & `anyio-3.7.0rc1/src/anyio/streams/text.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/streams/tls.py` & `anyio-3.7.0rc1/src/anyio/streams/tls.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio/to_process.py` & `anyio-3.7.0rc1/src/anyio/to_process.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 import os
 import pickle
 import subprocess
 import sys
 from collections import deque
 from importlib.util import module_from_spec, spec_from_file_location
-from typing import Callable, TypeVar, cast
+from typing import Callable, Deque, TypeVar, cast
 
 from ._core._eventloop import current_time, get_asynclib, get_cancelled_exc_class
 from ._core._exceptions import BrokenWorkerProcess
 from ._core._subprocesses import open_process
 from ._core._synchronization import CapacityLimiter
 from ._core._tasks import CancelScope, fail_after
 from .abc import ByteReceiveStream, ByteSendStream, Process
 from .lowlevel import RunVar, checkpoint_if_cancelled
 from .streams.buffered import BufferedByteReceiveStream
 
 WORKER_MAX_IDLE_TIME = 300  # 5 minutes
 
 T_Retval = TypeVar("T_Retval")
 _process_pool_workers: RunVar[set[Process]] = RunVar("_process_pool_workers")
-_process_pool_idle_workers: RunVar[deque[tuple[Process, float]]] = RunVar(
+_process_pool_idle_workers: RunVar[Deque[tuple[Process, float]]] = RunVar(
     "_process_pool_idle_workers"
 )
 _default_process_limiter: RunVar[CapacityLimiter] = RunVar("_default_process_limiter")
 
 
 async def run_sync(
     func: Callable[..., T_Retval],
```

### Comparing `anyio-3.7.0/src/anyio/to_thread.py` & `anyio-3.7.0rc1/src/anyio/to_thread.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/src/anyio.egg-info/PKG-INFO` & `anyio-3.7.0rc1/src/anyio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: anyio
-Version: 3.7.0
+Version: 3.7.0rc1
 Summary: High level compatibility layer for multiple asynchronous event loop implementations
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://anyio.readthedocs.io/en/latest/
 Project-URL: Changelog, https://anyio.readthedocs.io/en/stable/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/anyio
 Project-URL: Issue tracker, https://github.com/agronholm/anyio/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: AnyIO
-Classifier: Typing :: Typed
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `anyio-3.7.0/src/anyio.egg-info/SOURCES.txt` & `anyio-3.7.0rc1/src/anyio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/conftest.py` & `anyio-3.7.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/streams/test_buffered.py` & `anyio-3.7.0rc1/tests/streams/test_buffered.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/streams/test_file.py` & `anyio-3.7.0rc1/tests/streams/test_file.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/streams/test_memory.py` & `anyio-3.7.0rc1/tests/streams/test_memory.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/streams/test_stapled.py` & `anyio-3.7.0rc1/tests/streams/test_stapled.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from collections import deque
 from dataclasses import InitVar, dataclass, field
-from typing import Iterable, TypeVar
+from typing import Deque, Iterable, TypeVar
 
 import pytest
 
 from anyio import ClosedResourceError, EndOfStream
 from anyio.abc import (
     ByteReceiveStream,
     ByteSendStream,
@@ -99,15 +99,15 @@
 
 T_Item = TypeVar("T_Item")
 
 
 @dataclass
 class DummyObjectReceiveStream(ObjectReceiveStream[T_Item]):
     data: InitVar[Iterable[T_Item]]
-    buffer: deque[T_Item] = field(init=False)
+    buffer: Deque[T_Item] = field(init=False)
     _closed: bool = field(init=False, default=False)
 
     def __post_init__(self, data: Iterable[T_Item]) -> None:
         self.buffer = deque(data)
 
     async def receive(self) -> T_Item:
         if self._closed:
```

### Comparing `anyio-3.7.0/tests/streams/test_text.py` & `anyio-3.7.0rc1/tests/streams/test_text.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/streams/test_tls.py` & `anyio-3.7.0rc1/tests/streams/test_tls.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/test_compat.py` & `anyio-3.7.0rc1/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/test_debugging.py` & `anyio-3.7.0rc1/tests/test_debugging.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/test_eventloop.py` & `anyio-3.7.0rc1/tests/test_eventloop.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/test_fileio.py` & `anyio-3.7.0rc1/tests/test_fileio.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/test_from_thread.py` & `anyio-3.7.0rc1/tests/test_from_thread.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/test_lowlevel.py` & `anyio-3.7.0rc1/tests/test_lowlevel.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/test_pytest_plugin.py` & `anyio-3.7.0rc1/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/test_signals.py` & `anyio-3.7.0rc1/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/test_sockets.py` & `anyio-3.7.0rc1/tests/test_sockets.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/test_subprocesses.py` & `anyio-3.7.0rc1/tests/test_subprocesses.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/test_synchronization.py` & `anyio-3.7.0rc1/tests/test_synchronization.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/test_taskgroups.py` & `anyio-3.7.0rc1/tests/test_taskgroups.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/test_to_process.py` & `anyio-3.7.0rc1/tests/test_to_process.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0/tests/test_to_thread.py` & `anyio-3.7.0rc1/tests/test_to_thread.py`

 * *Files identical despite different names*

