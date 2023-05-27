# Comparing `tmp/trepan3k-1.2.8.tar.gz` & `tmp/trepan3k-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trepan3k-1.2.8.tar", last modified: Sat Nov  6 00:30:45 2021, max compression
+gzip compressed data, was "trepan3k-1.2.9.tar", last modified: Sat May 27 13:31:12 2023, max compression
```

## Comparing `trepan3k-1.2.8.tar` & `trepan3k-1.2.9.tar`

### file list

```diff
@@ -1,421 +1,422 @@
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:45.195601 trepan3k-1.2.8/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    35147 2015-04-05 01:14:05.000000 trepan3k-1.2.8/COPYING
--rw-rw-r--   0 rocky     (1000) rocky     (1000)   136815 2021-11-06 00:20:14.000000 trepan3k-1.2.8/ChangeLog
--rw-r--r--   0 rocky     (1000) rocky     (1000)      452 2020-04-21 18:39:42.000000 trepan3k-1.2.8/MANIFEST.in
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2844 2020-06-28 17:08:41.000000 trepan3k-1.2.8/Makefile
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    17345 2021-11-06 00:26:11.000000 trepan3k-1.2.8/NEWS.md
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    17457 2021-11-06 00:30:45.195601 trepan3k-1.2.8/PKG-INFO
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    13808 2021-08-21 16:21:41.000000 trepan3k-1.2.8/README.rst
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3729 2021-11-06 00:26:11.000000 trepan3k-1.2.8/__pkginfo__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)       23 2015-12-25 20:52:45.000000 trepan3k-1.2.8/requirements-dev.txt
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      832 2021-11-06 00:30:45.195601 trepan3k-1.2.8/setup.cfg
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1849 2021-11-06 00:30:04.000000 trepan3k-1.2.8/setup.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.847603 trepan3k-1.2.8/test/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      140 2013-03-29 21:23:19.000000 trepan3k-1.2.8/test/Makefile
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.851603 trepan3k-1.2.8/test/data/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      471 2019-04-17 00:56:26.000000 trepan3k-1.2.8/test/data/highlight-38.right
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      471 2017-05-21 16:21:13.000000 trepan3k-1.2.8/test/data/highlight-pyp35.right
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      471 2017-08-16 11:02:27.000000 trepan3k-1.2.8/test/data/highlight-pypy.right
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      207 2015-10-17 01:37:14.000000 trepan3k-1.2.8/test/data/highlight.cmd
--rw-r--r--   0 rocky     (1000) rocky     (1000)      450 2019-04-17 00:57:53.000000 trepan3k-1.2.8/test/data/highlight.right
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)      942 2017-11-02 19:38:09.000000 trepan3k-1.2.8/test/data/macro-pypy.right
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      248 2017-05-21 16:21:13.000000 trepan3k-1.2.8/test/data/macro-pypy35.right
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      248 2015-10-17 02:13:29.000000 trepan3k-1.2.8/test/data/macro.cmd
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      875 2017-11-02 19:38:09.000000 trepan3k-1.2.8/test/data/macro.right
--rw-rw-r--   0 rocky     (1000) rocky     (1000)       31 2017-08-16 11:02:30.000000 trepan3k-1.2.8/test/data/noscript-pypy.right
--rw-rw-r--   0 rocky     (1000) rocky     (1000)       34 2015-10-17 02:13:22.000000 trepan3k-1.2.8/test/data/noscript.cmd
--rw-rw-r--   0 rocky     (1000) rocky     (1000)       31 2015-04-05 01:14:05.000000 trepan3k-1.2.8/test/data/noscript.right
--rw-r--r--   0 rocky     (1000) rocky     (1000)      523 2019-04-17 01:05:56.000000 trepan3k-1.2.8/test/data/step-38.right
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1303 2017-08-16 11:05:16.000000 trepan3k-1.2.8/test/data/step-pypy.right
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      168 2015-10-17 02:14:16.000000 trepan3k-1.2.8/test/data/step.cmd
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      503 2017-04-08 10:30:30.000000 trepan3k-1.2.8/test/data/step.right
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.851603 trepan3k-1.2.8/test/example/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      117 2015-05-17 15:52:27.000000 trepan3k-1.2.8/test/example/bug.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)       45 2015-05-15 23:41:10.000000 trepan3k-1.2.8/test/example/eval.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      175 2015-12-01 06:41:35.000000 trepan3k-1.2.8/test/example/fib.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1076 2015-12-19 03:55:56.000000 trepan3k-1.2.8/test/example/gcd-dbgcall.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1022 2015-12-22 03:02:06.000000 trepan3k-1.2.8/test/example/gcd.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)      705 2015-04-05 01:14:05.000000 trepan3k-1.2.8/test/example/hanoi.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)      189 2020-06-14 22:55:31.000000 trepan3k-1.2.8/test/example/multi-line.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3083 2015-04-21 13:40:13.000000 trepan3k-1.2.8/test/example/tail.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.851603 trepan3k-1.2.8/test/functional/
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.847603 trepan3k-1.2.8/test/functional/.eggs/
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.847603 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.855603 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      404 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/__init__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      144 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/__main__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    13224 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/case.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     6316 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/commands.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    25282 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/config.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    13071 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/core.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      376 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/exc.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.855603 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/ext/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)       33 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/ext/__init__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    88107 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/ext/dtcompat.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1273 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/failure.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     5978 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/importer.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     7042 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/inspector.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    25578 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/loader.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.855603 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     6291 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/__init__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1720 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/allmodules.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     9709 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/attrib.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    26058 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/base.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1021 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/builtin.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3364 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/capture.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3156 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/collect.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    11677 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/cover.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2272 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/debug.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1551 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/deprecated.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    17478 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/doctests.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     7275 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/errorclass.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1635 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/failuredetail.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3756 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/isolate.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     9358 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/logcapture.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    15577 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/manager.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    35286 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/multiprocess.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    13533 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/plugintest.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     5357 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/prof.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2142 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/skip.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     9917 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/testid.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    11645 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/xunit.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     6879 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/proxy.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     7454 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/pyversion.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     6741 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/result.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     8985 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/selector.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.855603 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/sphinx/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)        5 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/sphinx/__init__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     5638 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/sphinx/pluginopts.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    22405 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/suite.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.859603 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/tools/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      436 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/tools/__init__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     4170 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/tools/nontrivial.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1184 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/tools/trivial.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     5540 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/twistedtools.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    20334 2021-07-17 19:51:55.000000 trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/util.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2206 2015-04-06 08:02:19.000000 trepan3k-1.2.8/test/functional/fn_helper.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)      417 2015-04-06 15:13:13.000000 trepan3k-1.2.8/test/functional/setup.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     4455 2015-04-06 08:04:18.000000 trepan3k-1.2.8/test/functional/stringarray.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     2122 2015-04-05 01:14:05.000000 trepan3k-1.2.8/test/functional/test-break.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1351 2015-04-05 01:14:05.000000 trepan3k-1.2.8/test/functional/test-finish.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1126 2015-04-06 09:30:51.000000 trepan3k-1.2.8/test/functional/test-jump.py
--rwxr-xr-x   0 rocky     (1000) rocky     (1000)     2364 2015-04-21 13:37:05.000000 trepan3k-1.2.8/test/functional/test-next.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     2982 2015-04-05 01:14:05.000000 trepan3k-1.2.8/test/functional/test-sig.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1401 2015-04-21 01:58:39.000000 trepan3k-1.2.8/test/functional/test-skip.py
--rwxr-xr-x   0 rocky     (1000) rocky     (1000)     5911 2015-04-21 01:57:05.000000 trepan3k-1.2.8/test/functional/test-step.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.859603 trepan3k-1.2.8/test/integration/
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.847603 trepan3k-1.2.8/test/integration/.eggs/
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.847603 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.859603 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      404 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/__init__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      144 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/__main__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    13224 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/case.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     6316 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/commands.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    25282 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/config.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    13071 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/core.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      376 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/exc.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.859603 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/ext/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)       33 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/ext/__init__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    88107 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/ext/dtcompat.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1273 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/failure.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     5978 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/importer.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     7042 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/inspector.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    25578 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/loader.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.939603 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     6291 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/__init__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1720 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/allmodules.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     9709 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/attrib.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    26058 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/base.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1021 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/builtin.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3364 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/capture.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3156 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/collect.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    11677 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/cover.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2272 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/debug.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1551 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/deprecated.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    17478 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/doctests.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     7275 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/errorclass.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1635 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/failuredetail.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3756 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/isolate.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     9358 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/logcapture.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    15577 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/manager.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    35286 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/multiprocess.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    13533 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/plugintest.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     5357 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/prof.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2142 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/skip.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     9917 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/testid.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    11645 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/xunit.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     6879 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/proxy.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     7454 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/pyversion.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     6741 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/result.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     8985 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/selector.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.939603 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/sphinx/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)        5 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/sphinx/__init__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     5638 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/sphinx/pluginopts.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    22405 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/suite.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.939603 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/tools/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      436 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/tools/__init__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     4170 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/tools/nontrivial.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1184 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/tools/trivial.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     5540 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/twistedtools.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    20334 2021-07-17 19:51:56.000000 trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/util.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2094 2020-05-08 23:54:32.000000 trepan3k-1.2.8/test/integration/helper.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)      417 2015-04-06 15:13:13.000000 trepan3k-1.2.8/test/integration/setup.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)      774 2019-04-17 01:08:01.000000 trepan3k-1.2.8/test/integration/test-general.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)      810 2019-04-17 01:05:37.000000 trepan3k-1.2.8/test/integration/test-highlight.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)      539 2015-04-05 14:01:28.000000 trepan3k-1.2.8/test/integration/test-noscript.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.943603 trepan3k-1.2.8/test/unit/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      226 2015-04-05 14:01:28.000000 trepan3k-1.2.8/test/unit/cmdhelper.py
--rwxr-xr-x   0 rocky     (1000) rocky     (1000)     3505 2020-06-18 10:55:05.000000 trepan3k-1.2.8/test/unit/test-break.py
--rwxr-xr-x   0 rocky     (1000) rocky     (1000)     3386 2020-06-14 02:56:20.000000 trepan3k-1.2.8/test/unit/test-brkpt.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1228 2017-08-16 11:08:40.000000 trepan3k-1.2.8/test/unit/test-bytecode.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1419 2015-04-05 14:01:28.000000 trepan3k-1.2.8/test/unit/test-clifns.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     2458 2015-04-05 22:56:16.000000 trepan3k-1.2.8/test/unit/test-cmd-alias.py
--rwxr-xr-x   0 rocky     (1000) rocky     (1000)     2881 2020-06-18 10:54:29.000000 trepan3k-1.2.8/test/unit/test-cmdbreak.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     2471 2015-05-16 19:16:43.000000 trepan3k-1.2.8/test/unit/test-cmdfns.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     4640 2018-05-18 23:47:35.000000 trepan3k-1.2.8/test/unit/test-cmdproc.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     4176 2020-06-18 00:52:10.000000 trepan3k-1.2.8/test/unit/test-completion.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1107 2017-05-07 06:31:11.000000 trepan3k-1.2.8/test/unit/test-core.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     2568 2017-11-02 19:38:09.000000 trepan3k-1.2.8/test/unit/test-disassemble.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)      530 2015-04-05 14:01:28.000000 trepan3k-1.2.8/test/unit/test-except.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)      996 2015-04-05 14:01:28.000000 trepan3k-1.2.8/test/unit/test-fifo.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)      803 2015-05-16 19:17:16.000000 trepan3k-1.2.8/test/unit/test-finish.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     2145 2015-04-05 15:15:49.000000 trepan3k-1.2.8/test/unit/test-help.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1572 2015-04-05 14:01:28.000000 trepan3k-1.2.8/test/unit/test-info-files.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)      688 2015-04-05 21:55:08.000000 trepan3k-1.2.8/test/unit/test-inout-input.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)      987 2017-05-07 06:31:11.000000 trepan3k-1.2.8/test/unit/test-kill.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     2254 2020-06-14 02:49:42.000000 trepan3k-1.2.8/test/unit/test-lib-complete.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1170 2015-04-05 14:01:28.000000 trepan3k-1.2.8/test/unit/test-lib-display.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)      861 2020-10-26 21:45:02.000000 trepan3k-1.2.8/test/unit/test-lib-eval.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1031 2017-05-07 06:31:11.000000 trepan3k-1.2.8/test/unit/test-lib-file.py
--rwxr-xr-x   0 rocky     (1000) rocky     (1000)     3175 2020-05-10 23:15:25.000000 trepan3k-1.2.8/test/unit/test-lib-format.py
--rwxr-xr-x   0 rocky     (1000) rocky     (1000)      877 2016-01-13 01:56:52.000000 trepan3k-1.2.8/test/unit/test-lib-pp.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)      798 2015-04-06 02:00:40.000000 trepan3k-1.2.8/test/unit/test-lib-printing.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     2094 2015-04-05 23:35:30.000000 trepan3k-1.2.8/test/unit/test-lib-sig.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1455 2015-04-05 23:50:30.000000 trepan3k-1.2.8/test/unit/test-lib-thread.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     3876 2020-06-18 10:59:50.000000 trepan3k-1.2.8/test/unit/test-list.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1096 2015-04-05 14:01:28.000000 trepan3k-1.2.8/test/unit/test-misc.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1074 2021-08-21 16:06:05.000000 trepan3k-1.2.8/test/unit/test-print.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1630 2015-04-05 14:01:28.000000 trepan3k-1.2.8/test/unit/test-processor.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)      604 2015-04-05 14:01:28.000000 trepan3k-1.2.8/test/unit/test-quit.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)      612 2015-04-05 22:59:05.000000 trepan3k-1.2.8/test/unit/test-run.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)      864 2015-04-06 00:12:45.000000 trepan3k-1.2.8/test/unit/test-stack.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1033 2015-04-05 14:01:28.000000 trepan3k-1.2.8/test/unit/test-step.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     2133 2015-05-16 19:17:26.000000 trepan3k-1.2.8/test/unit/test-subcmd.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1364 2017-11-02 19:38:09.000000 trepan3k-1.2.8/test/unit/test-tcp.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1021 2020-05-10 11:25:11.000000 trepan3k-1.2.8/test/unit/test-user.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.943603 trepan3k-1.2.8/trepan/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     6913 2021-03-15 19:32:04.000000 trepan3k-1.2.8/trepan/__init__.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)    10554 2021-07-17 20:00:44.000000 trepan3k-1.2.8/trepan/__main__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     9203 2021-08-22 13:18:02.000000 trepan3k-1.2.8/trepan/api.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     7454 2020-05-22 00:00:22.000000 trepan3k-1.2.8/trepan/bwcli.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.943603 trepan3k-1.2.8/trepan/bwprocessor/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      709 2018-08-04 18:11:20.000000 trepan3k-1.2.8/trepan/bwprocessor/__init__.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.943603 trepan3k-1.2.8/trepan/bwprocessor/command/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1574 2015-04-06 08:36:44.000000 trepan3k-1.2.8/trepan/bwprocessor/command/__init__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3566 2015-06-12 09:21:38.000000 trepan3k-1.2.8/trepan/bwprocessor/command/base_cmd.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3764 2015-04-05 14:01:28.000000 trepan3k-1.2.8/trepan/bwprocessor/command/mock.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2708 2015-04-05 14:01:28.000000 trepan3k-1.2.8/trepan/bwprocessor/command/quit.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2619 2015-04-06 08:39:49.000000 trepan3k-1.2.8/trepan/bwprocessor/command/step.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3826 2015-04-06 08:35:14.000000 trepan3k-1.2.8/trepan/bwprocessor/location.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)    18061 2016-01-13 06:45:18.000000 trepan3k-1.2.8/trepan/bwprocessor/main.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1084 2015-04-06 08:35:06.000000 trepan3k-1.2.8/trepan/bwprocessor/msg.py
--rwxr-xr-x   0 rocky     (1000) rocky     (1000)     4922 2021-03-15 19:06:06.000000 trepan3k-1.2.8/trepan/client.py
--rwxr-xr-x   0 rocky     (1000) rocky     (1000)     3297 2020-05-09 22:53:35.000000 trepan3k-1.2.8/trepan/clifns.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    14734 2021-08-22 13:15:51.000000 trepan3k-1.2.8/trepan/debugger.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1377 2020-05-10 11:37:44.000000 trepan3k-1.2.8/trepan/exception.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.947603 trepan3k-1.2.8/trepan/inout/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      278 2018-08-04 18:12:22.000000 trepan3k-1.2.8/trepan/inout/__init__.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     5375 2020-05-14 16:43:09.000000 trepan3k-1.2.8/trepan/inout/base.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     4693 2020-04-23 00:22:52.000000 trepan3k-1.2.8/trepan/inout/fifoclient.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     4851 2015-04-05 14:01:28.000000 trepan3k-1.2.8/trepan/inout/fifoserver.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     5332 2018-07-28 23:13:20.000000 trepan3k-1.2.8/trepan/inout/input.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3004 2020-12-18 23:01:17.000000 trepan3k-1.2.8/trepan/inout/output.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2672 2015-04-05 18:56:20.000000 trepan3k-1.2.8/trepan/inout/scriptin.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     4456 2015-04-05 14:01:28.000000 trepan3k-1.2.8/trepan/inout/stringarray.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     4314 2017-08-10 11:59:32.000000 trepan3k-1.2.8/trepan/inout/tcpclient.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1519 2021-05-08 07:51:11.000000 trepan3k-1.2.8/trepan/inout/tcpfns.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     6486 2017-08-10 11:59:32.000000 trepan3k-1.2.8/trepan/inout/tcpserver.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2839 2018-07-28 18:10:01.000000 trepan3k-1.2.8/trepan/interface.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.947603 trepan3k-1.2.8/trepan/interfaces/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      789 2016-10-09 17:01:53.000000 trepan3k-1.2.8/trepan/interfaces/__init__.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     2551 2021-07-16 09:55:55.000000 trepan3k-1.2.8/trepan/interfaces/bullwinkle.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2873 2017-08-10 11:59:32.000000 trepan3k-1.2.8/trepan/interfaces/client.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1012 2015-04-05 01:14:05.000000 trepan3k-1.2.8/trepan/interfaces/comcodes.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     3927 2015-04-05 18:48:30.000000 trepan3k-1.2.8/trepan/interfaces/script.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     4861 2017-08-10 11:59:32.000000 trepan3k-1.2.8/trepan/interfaces/server.py
--rwxrwxr-x   0 rocky     (1000) rocky     (1000)     5831 2020-12-18 23:01:17.000000 trepan3k-1.2.8/trepan/interfaces/user.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.947603 trepan3k-1.2.8/trepan/lib/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      922 2018-08-04 18:12:47.000000 trepan3k-1.2.8/trepan/lib/__init__.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)    12381 2020-07-01 02:21:03.000000 trepan3k-1.2.8/trepan/lib/breakpoint.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     4186 2020-05-09 22:54:13.000000 trepan3k-1.2.8/trepan/lib/bytecode.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     3777 2020-05-09 20:16:32.000000 trepan3k-1.2.8/trepan/lib/complete.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)    17867 2020-10-12 00:38:55.000000 trepan3k-1.2.8/trepan/lib/core.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     5854 2021-08-29 12:44:38.000000 trepan3k-1.2.8/trepan/lib/default.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3459 2021-10-24 05:13:17.000000 trepan3k-1.2.8/trepan/lib/deparse.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    12497 2021-11-06 00:30:04.000000 trepan3k-1.2.8/trepan/lib/disassemble.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     4764 2020-05-09 20:12:06.000000 trepan3k-1.2.8/trepan/lib/display.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2469 2020-10-26 21:45:02.000000 trepan3k-1.2.8/trepan/lib/eval.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3957 2020-05-21 23:54:28.000000 trepan3k-1.2.8/trepan/lib/file.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    13861 2020-08-23 21:52:33.000000 trepan3k-1.2.8/trepan/lib/format.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3965 2021-07-17 20:00:44.000000 trepan3k-1.2.8/trepan/lib/pp.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     4182 2020-05-14 16:43:09.000000 trepan3k-1.2.8/trepan/lib/printing.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)    20001 2016-01-13 06:46:34.000000 trepan3k-1.2.8/trepan/lib/sighandler.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    14788 2021-10-30 09:53:22.000000 trepan3k-1.2.8/trepan/lib/stack.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2939 2020-05-09 20:08:59.000000 trepan3k-1.2.8/trepan/lib/thred.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2361 2021-06-17 13:36:06.000000 trepan3k-1.2.8/trepan/misc.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)    13920 2018-08-20 07:21:37.000000 trepan3k-1.2.8/trepan/options.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     7438 2017-11-02 19:38:09.000000 trepan3k-1.2.8/trepan/post_mortem.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:44.947603 trepan3k-1.2.8/trepan/processor/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)        0 2020-05-09 19:25:16.000000 trepan3k-1.2.8/trepan/processor/__init__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     6247 2020-05-11 19:25:31.000000 trepan3k-1.2.8/trepan/processor/cmd_addrlist.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     5998 2020-07-01 17:39:14.000000 trepan3k-1.2.8/trepan/processor/cmdbreak.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     7344 2021-07-17 20:00:44.000000 trepan3k-1.2.8/trepan/processor/cmdfns.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     6503 2020-06-13 07:48:11.000000 trepan3k-1.2.8/trepan/processor/cmdlist.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    43072 2021-08-22 13:19:50.000000 trepan3k-1.2.8/trepan/processor/cmdproc.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:45.111601 trepan3k-1.2.8/trepan/processor/command/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1506 2021-01-30 06:01:07.000000 trepan3k-1.2.8/trepan/processor/command/__init__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3199 2020-06-28 00:22:39.000000 trepan3k-1.2.8/trepan/processor/command/alias.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     5139 2020-06-08 00:51:15.000000 trepan3k-1.2.8/trepan/processor/command/backtrace.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     4965 2021-07-17 20:00:44.000000 trepan3k-1.2.8/trepan/processor/command/base_cmd.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     6742 2020-06-09 10:38:06.000000 trepan3k-1.2.8/trepan/processor/command/base_subcmd.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     9195 2021-10-30 09:53:22.000000 trepan3k-1.2.8/trepan/processor/command/base_submgr.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     4123 2020-06-09 10:49:22.000000 trepan3k-1.2.8/trepan/processor/command/bpython.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     4601 2020-06-18 10:47:44.000000 trepan3k-1.2.8/trepan/processor/command/break.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1742 2020-06-28 00:29:59.000000 trepan3k-1.2.8/trepan/processor/command/cd.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     2410 2020-06-09 10:44:53.000000 trepan3k-1.2.8/trepan/processor/command/clear.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     2535 2020-08-23 22:10:08.000000 trepan3k-1.2.8/trepan/processor/command/condition.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3053 2020-12-19 12:03:57.000000 trepan3k-1.2.8/trepan/processor/command/continue.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3327 2020-06-27 23:18:24.000000 trepan3k-1.2.8/trepan/processor/command/debug.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2279 2020-06-08 01:53:13.000000 trepan3k-1.2.8/trepan/processor/command/delete.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     7386 2021-10-30 09:53:22.000000 trepan3k-1.2.8/trepan/processor/command/deparse.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3048 2021-07-17 20:00:44.000000 trepan3k-1.2.8/trepan/processor/command/deval.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2054 2020-06-08 02:07:48.000000 trepan3k-1.2.8/trepan/processor/command/disable.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     8894 2021-11-06 00:30:04.000000 trepan3k-1.2.8/trepan/processor/command/disassemble.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     3493 2020-06-09 10:38:06.000000 trepan3k-1.2.8/trepan/processor/command/display.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     2118 2020-06-09 10:38:06.000000 trepan3k-1.2.8/trepan/processor/command/down.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2718 2020-06-13 07:58:59.000000 trepan3k-1.2.8/trepan/processor/command/edit.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2075 2020-06-08 02:09:09.000000 trepan3k-1.2.8/trepan/processor/command/enable.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3126 2020-10-26 21:45:02.000000 trepan3k-1.2.8/trepan/processor/command/eval.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2021 2020-06-13 07:02:56.000000 trepan3k-1.2.8/trepan/processor/command/examine.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     2009 2020-06-09 10:53:31.000000 trepan3k-1.2.8/trepan/processor/command/exit.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     3223 2020-06-07 23:52:05.000000 trepan3k-1.2.8/trepan/processor/command/finish.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     8829 2020-06-27 20:24:38.000000 trepan3k-1.2.8/trepan/processor/command/frame.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2643 2020-06-28 00:27:18.000000 trepan3k-1.2.8/trepan/processor/command/handle.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:45.111601 trepan3k-1.2.8/trepan/processor/command/help/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)        4 2015-06-12 09:10:07.000000 trepan3k-1.2.8/trepan/processor/command/help/.gitignore
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      327 2020-05-08 23:23:05.000000 trepan3k-1.2.8/trepan/processor/command/help/README.md
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      924 2017-11-02 19:38:09.000000 trepan3k-1.2.8/trepan/processor/command/help/arange.rst
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2328 2015-06-12 09:10:07.000000 trepan3k-1.2.8/trepan/processor/command/help/command.rst
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      336 2020-05-10 13:57:19.000000 trepan3k-1.2.8/trepan/processor/command/help/examples.rst
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      454 2015-06-12 09:10:07.000000 trepan3k-1.2.8/trepan/processor/command/help/filename.rst
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     4192 2017-11-02 19:38:09.000000 trepan3k-1.2.8/trepan/processor/command/help/location.rst
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1421 2017-11-02 19:38:09.000000 trepan3k-1.2.8/trepan/processor/command/help/range.rst
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      517 2015-06-12 09:10:07.000000 trepan3k-1.2.8/trepan/processor/command/help/suffixes.rst
--rw-r--r--   0 rocky     (1000) rocky     (1000)     9754 2020-06-07 23:52:05.000000 trepan3k-1.2.8/trepan/processor/command/help.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1453 2020-06-07 23:52:05.000000 trepan3k-1.2.8/trepan/processor/command/info.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:45.111601 trepan3k-1.2.8/trepan/processor/command/info_subcmd/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1548 2018-08-04 18:17:08.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/__init__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2566 2016-01-09 01:15:52.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/args.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     4108 2020-06-14 02:21:04.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/break.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2176 2015-05-27 13:44:41.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/builtins.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     4704 2015-12-26 18:41:24.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/code.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1780 2015-05-15 23:15:58.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/display.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     5563 2020-06-18 01:11:47.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/files.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     4635 2015-12-27 10:27:28.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/frame.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2683 2018-03-11 14:22:50.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/globals.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     5167 2020-06-14 22:55:31.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/line.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     5002 2020-08-29 23:19:55.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/lines.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     4984 2020-07-29 05:41:43.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/locals.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     2806 2017-06-04 01:27:49.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/macro.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     3133 2020-06-18 00:48:10.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/offsets.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     3381 2020-05-28 02:33:29.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/pc.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     3431 2020-05-28 02:33:29.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/program.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1983 2020-05-28 02:33:29.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/return.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2200 2015-05-27 13:44:41.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/signals.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1351 2015-04-06 07:36:04.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/source.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     7188 2015-06-03 17:26:44.000000 trepan3k-1.2.8/trepan/processor/command/info_subcmd/threads.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     6554 2020-06-08 01:48:34.000000 trepan3k-1.2.8/trepan/processor/command/ipython.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2889 2020-06-09 11:37:53.000000 trepan3k-1.2.8/trepan/processor/command/jump.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     5968 2020-06-07 23:52:05.000000 trepan3k-1.2.8/trepan/processor/command/kill.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     7447 2021-01-25 02:33:50.000000 trepan3k-1.2.8/trepan/processor/command/list.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3916 2020-06-28 00:24:53.000000 trepan3k-1.2.8/trepan/processor/command/macro.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     3916 2020-06-07 23:52:05.000000 trepan3k-1.2.8/trepan/processor/command/mock.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     3161 2020-06-07 23:52:05.000000 trepan3k-1.2.8/trepan/processor/command/next.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2450 2020-06-08 00:50:13.000000 trepan3k-1.2.8/trepan/processor/command/p.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1998 2020-06-27 21:39:33.000000 trepan3k-1.2.8/trepan/processor/command/pp.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     6432 2020-06-07 23:52:05.000000 trepan3k-1.2.8/trepan/processor/command/python.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     4621 2020-06-07 23:52:05.000000 trepan3k-1.2.8/trepan/processor/command/quit.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     2540 2020-06-10 10:16:51.000000 trepan3k-1.2.8/trepan/processor/command/restart.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1878 2020-06-13 06:52:18.000000 trepan3k-1.2.8/trepan/processor/command/run.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1410 2020-06-07 23:52:05.000000 trepan3k-1.2.8/trepan/processor/command/set.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:45.191601 trepan3k-1.2.8/trepan/processor/command/set_subcmd/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      682 2020-05-19 09:30:37.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/__demo_helper__.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1529 2020-05-12 12:50:00.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/__init__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2641 2021-01-25 02:40:06.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/asmfmt.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2280 2015-04-06 07:46:57.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/autoeval.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2177 2020-05-13 04:45:41.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/autolist.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1941 2020-05-13 04:58:08.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/autopc.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1956 2015-06-07 00:55:56.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/autopython.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1412 2016-06-22 03:50:08.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/basename.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1315 2015-04-06 08:45:16.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/cmdtrace.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1456 2015-10-17 02:35:09.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/confirm.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2092 2015-04-06 07:57:23.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/dbg_trepan.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     2179 2020-05-28 18:08:00.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/different.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     2574 2020-09-06 00:03:09.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/events.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     3919 2020-05-12 17:36:53.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/highlight.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1573 2020-05-19 09:31:33.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/listsize.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1556 2020-09-06 00:03:09.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/maxstring.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1775 2020-10-12 00:43:00.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/patsub.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1748 2015-06-16 18:10:56.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/skip.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1963 2020-09-06 00:07:18.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/style.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1875 2021-07-17 20:00:44.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/substitute.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1255 2021-01-25 03:16:56.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/tempdir.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1431 2015-06-07 00:55:59.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/trace.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)      923 2020-05-28 02:33:29.000000 trepan3k-1.2.8/trepan/processor/command/set_subcmd/width.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1435 2020-06-07 23:52:05.000000 trepan3k-1.2.8/trepan/processor/command/show.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:45.195601 trepan3k-1.2.8/trepan/processor/command/show_subcmd/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      676 2015-04-05 14:01:28.000000 trepan3k-1.2.8/trepan/processor/command/show_subcmd/__demo_helper__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1447 2018-08-04 18:16:43.000000 trepan3k-1.2.8/trepan/processor/command/show_subcmd/__init__.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     2613 2015-06-03 17:26:55.000000 trepan3k-1.2.8/trepan/processor/command/show_subcmd/aliases.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1427 2015-04-06 09:42:03.000000 trepan3k-1.2.8/trepan/processor/command/show_subcmd/args.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1606 2020-06-23 11:50:47.000000 trepan3k-1.2.8/trepan/processor/command/show_subcmd/asmfmt.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1196 2015-06-07 00:55:59.000000 trepan3k-1.2.8/trepan/processor/command/show_subcmd/autoeval.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1219 2020-05-13 04:52:21.000000 trepan3k-1.2.8/trepan/processor/command/show_subcmd/autolist.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1238 2021-10-30 09:53:22.000000 trepan3k-1.2.8/trepan/processor/command/show_subcmd/autopc.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1289 2015-04-06 07:51:46.000000 trepan3k-1.2.8/trepan/processor/command/show_subcmd/autopython.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1266 2015-04-05 14:01:28.000000 trepan3k-1.2.8/trepan/processor/command/show_subcmd/basename.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1204 2015-06-07 00:56:02.000000 trepan3k-1.2.8/trepan/processor/command/show_subcmd/confirm.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)      341 2015-06-07 00:56:02.000000 trepan3k-1.2.8/trepan/processor/command/show_subcmd/dbg_trepan.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1721 2015-06-07 00:56:06.000000 trepan3k-1.2.8/trepan/processor/command/show_subcmd/highlight.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1078 2015-06-07 00:56:06.000000 trepan3k-1.2.8/trepan/processor/command/show_subcmd/listsize.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1205 2020-10-25 11:27:16.000000 trepan3k-1.2.8/trepan/processor/command/show_subcmd/style.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)      937 2021-01-25 02:39:14.000000 trepan3k-1.2.8/trepan/processor/command/show_subcmd/tempdir.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3269 2020-06-10 10:15:21.000000 trepan3k-1.2.8/trepan/processor/command/skip.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     3010 2020-06-07 23:52:05.000000 trepan3k-1.2.8/trepan/processor/command/source.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     5078 2020-06-15 16:43:55.000000 trepan3k-1.2.8/trepan/processor/command/step.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3653 2020-12-19 12:03:57.000000 trepan3k-1.2.8/trepan/processor/command/tbreak.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     1887 2020-06-07 23:52:05.000000 trepan3k-1.2.8/trepan/processor/command/unalias.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2610 2020-06-28 00:28:35.000000 trepan3k-1.2.8/trepan/processor/command/undisplay.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     2434 2020-06-09 10:38:06.000000 trepan3k-1.2.8/trepan/processor/command/up.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     4455 2020-06-27 20:24:38.000000 trepan3k-1.2.8/trepan/processor/command/whatis.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     6142 2020-06-09 10:38:06.000000 trepan3k-1.2.8/trepan/processor/complete.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3537 2017-11-02 19:38:09.000000 trepan3k-1.2.8/trepan/processor/frame.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     9451 2021-11-06 00:30:04.000000 trepan3k-1.2.8/trepan/processor/location.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:45.195601 trepan3k-1.2.8/trepan/processor/parse/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)        0 2017-11-02 19:38:09.000000 trepan3k-1.2.8/trepan/processor/parse/__init__.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     7825 2020-06-14 16:46:55.000000 trepan3k-1.2.8/trepan/processor/parse/parser.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)     4810 2020-06-14 16:46:55.000000 trepan3k-1.2.8/trepan/processor/parse/scanner.py
--rw-r--r--   0 rocky     (1000) rocky     (1000)    13068 2020-06-14 16:46:55.000000 trepan3k-1.2.8/trepan/processor/parse/semantics.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1426 2017-11-02 19:38:09.000000 trepan3k-1.2.8/trepan/processor/parse/tok.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     5614 2016-01-13 06:49:48.000000 trepan3k-1.2.8/trepan/processor/subcmd.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2066 2015-04-06 08:40:40.000000 trepan3k-1.2.8/trepan/processor/trace.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      255 2021-11-06 00:26:11.000000 trepan3k-1.2.8/trepan/version.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2916 2020-05-09 16:29:56.000000 trepan3k-1.2.8/trepan/vprocessor.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2021-11-06 00:30:45.195601 trepan3k-1.2.8/trepan3k.egg-info/
--rw-r--r--   0 rocky     (1000) rocky     (1000)    17457 2021-11-06 00:30:44.000000 trepan3k-1.2.8/trepan3k.egg-info/PKG-INFO
--rw-r--r--   0 rocky     (1000) rocky     (1000)    15341 2021-11-06 00:30:44.000000 trepan3k-1.2.8/trepan3k.egg-info/SOURCES.txt
--rw-r--r--   0 rocky     (1000) rocky     (1000)        1 2021-11-06 00:30:44.000000 trepan3k-1.2.8/trepan3k.egg-info/dependency_links.txt
--rw-r--r--   0 rocky     (1000) rocky     (1000)       82 2021-11-06 00:30:44.000000 trepan3k-1.2.8/trepan3k.egg-info/entry_points.txt
--rw-r--r--   0 rocky     (1000) rocky     (1000)        1 2020-06-07 23:00:37.000000 trepan3k-1.2.8/trepan3k.egg-info/not-zip-safe
--rw-r--r--   0 rocky     (1000) rocky     (1000)      172 2021-11-06 00:30:44.000000 trepan3k-1.2.8/trepan3k.egg-info/requires.txt
--rw-r--r--   0 rocky     (1000) rocky     (1000)        7 2021-11-06 00:30:44.000000 trepan3k-1.2.8/trepan3k.egg-info/top_level.txt
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.428597 trepan3k-1.2.9/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    35147 2015-04-05 01:14:05.000000 trepan3k-1.2.9/COPYING
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)   149367 2023-05-27 13:20:02.000000 trepan3k-1.2.9/ChangeLog
+-rw-r--r--   0 rocky     (1000) rocky     (1000)      452 2020-04-21 18:39:42.000000 trepan3k-1.2.9/MANIFEST.in
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2895 2023-05-27 08:41:28.000000 trepan3k-1.2.9/Makefile
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    17796 2023-05-27 13:15:35.000000 trepan3k-1.2.9/NEWS.md
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    15032 2023-05-27 13:31:12.428597 trepan3k-1.2.9/PKG-INFO
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    13797 2023-05-27 12:54:52.000000 trepan3k-1.2.9/README.rst
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3845 2023-05-27 13:30:49.000000 trepan3k-1.2.9/__pkginfo__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)       23 2015-12-25 20:52:45.000000 trepan3k-1.2.9/requirements-dev.txt
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      832 2023-05-27 13:31:12.432597 trepan3k-1.2.9/setup.cfg
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1849 2023-05-27 13:30:49.000000 trepan3k-1.2.9/setup.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.196598 trepan3k-1.2.9/test/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      140 2013-03-29 21:23:19.000000 trepan3k-1.2.9/test/Makefile
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.200598 trepan3k-1.2.9/test/data/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      471 2019-04-17 00:56:26.000000 trepan3k-1.2.9/test/data/highlight-38.right
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      471 2017-05-21 16:21:13.000000 trepan3k-1.2.9/test/data/highlight-pyp35.right
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      471 2017-08-16 11:02:27.000000 trepan3k-1.2.9/test/data/highlight-pypy.right
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      207 2015-10-17 01:37:14.000000 trepan3k-1.2.9/test/data/highlight.cmd
+-rw-r--r--   0 rocky     (1000) rocky     (1000)      450 2019-04-17 00:57:53.000000 trepan3k-1.2.9/test/data/highlight.right
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)      942 2017-11-02 19:38:09.000000 trepan3k-1.2.9/test/data/macro-pypy.right
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      248 2017-05-21 16:21:13.000000 trepan3k-1.2.9/test/data/macro-pypy35.right
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      248 2015-10-17 02:13:29.000000 trepan3k-1.2.9/test/data/macro.cmd
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      875 2017-11-02 19:38:09.000000 trepan3k-1.2.9/test/data/macro.right
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)       31 2017-08-16 11:02:30.000000 trepan3k-1.2.9/test/data/noscript-pypy.right
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)       34 2015-10-17 02:13:22.000000 trepan3k-1.2.9/test/data/noscript.cmd
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)       31 2015-04-05 01:14:05.000000 trepan3k-1.2.9/test/data/noscript.right
+-rw-r--r--   0 rocky     (1000) rocky     (1000)      523 2019-04-17 01:05:56.000000 trepan3k-1.2.9/test/data/step-38.right
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1303 2017-08-16 11:05:16.000000 trepan3k-1.2.9/test/data/step-pypy.right
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      168 2015-10-17 02:14:16.000000 trepan3k-1.2.9/test/data/step.cmd
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      503 2017-04-08 10:30:30.000000 trepan3k-1.2.9/test/data/step.right
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.200598 trepan3k-1.2.9/test/example/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      117 2015-05-17 15:52:27.000000 trepan3k-1.2.9/test/example/bug.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)       45 2015-05-15 23:41:10.000000 trepan3k-1.2.9/test/example/eval.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      175 2015-12-01 06:41:35.000000 trepan3k-1.2.9/test/example/fib.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1076 2015-12-19 03:55:56.000000 trepan3k-1.2.9/test/example/gcd-dbgcall.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1022 2015-12-22 03:02:06.000000 trepan3k-1.2.9/test/example/gcd.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)      705 2015-04-05 01:14:05.000000 trepan3k-1.2.9/test/example/hanoi.py
+-rw-r--r--   0 rocky     (1000) rocky     (1000)      189 2020-06-14 22:55:31.000000 trepan3k-1.2.9/test/example/multi-line.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3083 2015-04-21 13:40:13.000000 trepan3k-1.2.9/test/example/tail.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.200598 trepan3k-1.2.9/test/functional/
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.192598 trepan3k-1.2.9/test/functional/.eggs/
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.192598 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.204598 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      404 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      144 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/__main__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    13224 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/case.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     6316 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/commands.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    25282 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/config.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    13071 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/core.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      376 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/exc.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.204598 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/ext/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)       33 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/ext/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    88107 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/ext/dtcompat.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1273 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/failure.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5978 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/importer.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     7042 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/inspector.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    25578 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/loader.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.208598 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     6291 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1720 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/allmodules.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     9709 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/attrib.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    26058 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/base.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1021 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/builtin.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3364 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/capture.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3156 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/collect.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    11677 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/cover.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2272 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/debug.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1551 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/deprecated.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    17478 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/doctests.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     7275 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/errorclass.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1635 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/failuredetail.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3756 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/isolate.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     9358 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/logcapture.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    15577 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/manager.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    35286 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/multiprocess.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    13533 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/plugintest.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5357 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/prof.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2142 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/skip.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     9917 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/testid.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    11645 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/xunit.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     6879 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/proxy.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     7454 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/pyversion.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     6741 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/result.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     8985 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/selector.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.208598 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/sphinx/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)        5 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/sphinx/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5638 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/sphinx/pluginopts.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    22405 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/suite.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.208598 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/tools/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      436 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/tools/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4170 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/tools/nontrivial.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1184 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/tools/trivial.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5540 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/twistedtools.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    20334 2021-07-17 19:51:55.000000 trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/util.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2206 2015-04-06 08:02:19.000000 trepan3k-1.2.9/test/functional/fn_helper.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)      417 2015-04-06 15:13:13.000000 trepan3k-1.2.9/test/functional/setup.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4455 2015-04-06 08:04:18.000000 trepan3k-1.2.9/test/functional/stringarray.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     2122 2015-04-05 01:14:05.000000 trepan3k-1.2.9/test/functional/test-break.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1351 2015-04-05 01:14:05.000000 trepan3k-1.2.9/test/functional/test-finish.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1126 2015-04-06 09:30:51.000000 trepan3k-1.2.9/test/functional/test-jump.py
+-rwxr-xr-x   0 rocky     (1000) rocky     (1000)     2364 2015-04-21 13:37:05.000000 trepan3k-1.2.9/test/functional/test-next.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     2982 2015-04-05 01:14:05.000000 trepan3k-1.2.9/test/functional/test-sig.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1401 2015-04-21 01:58:39.000000 trepan3k-1.2.9/test/functional/test-skip.py
+-rwxr-xr-x   0 rocky     (1000) rocky     (1000)     5911 2015-04-21 01:57:05.000000 trepan3k-1.2.9/test/functional/test-step.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.208598 trepan3k-1.2.9/test/integration/
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.196598 trepan3k-1.2.9/test/integration/.eggs/
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.196598 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.208598 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      404 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      144 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/__main__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    13224 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/case.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     6316 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/commands.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    25282 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/config.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    13071 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/core.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      376 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/exc.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.208598 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/ext/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)       33 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/ext/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    88107 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/ext/dtcompat.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1273 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/failure.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5978 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/importer.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     7042 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/inspector.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    25578 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/loader.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.280598 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     6291 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1720 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/allmodules.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     9709 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/attrib.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    26058 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/base.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1021 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/builtin.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3364 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/capture.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3156 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/collect.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    11677 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/cover.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2272 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/debug.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1551 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/deprecated.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    17478 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/doctests.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     7275 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/errorclass.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1635 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/failuredetail.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3756 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/isolate.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     9358 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/logcapture.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    15577 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/manager.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    35286 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/multiprocess.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    13533 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/plugintest.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5357 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/prof.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2142 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/skip.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     9917 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/testid.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    11645 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/xunit.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     6879 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/proxy.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     7454 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/pyversion.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     6741 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/result.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     8985 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/selector.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.280598 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/sphinx/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)        5 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/sphinx/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5638 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/sphinx/pluginopts.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    22405 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/suite.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.280598 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/tools/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      436 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/tools/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4170 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/tools/nontrivial.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1184 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/tools/trivial.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5540 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/twistedtools.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    20334 2021-07-17 19:51:56.000000 trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/util.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2094 2020-05-08 23:54:32.000000 trepan3k-1.2.9/test/integration/helper.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)      417 2015-04-06 15:13:13.000000 trepan3k-1.2.9/test/integration/setup.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)      774 2023-05-27 13:30:49.000000 trepan3k-1.2.9/test/integration/test-general.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)      810 2023-05-27 13:30:49.000000 trepan3k-1.2.9/test/integration/test-highlight.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)      539 2015-04-05 14:01:28.000000 trepan3k-1.2.9/test/integration/test-noscript.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.284598 trepan3k-1.2.9/test/unit/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      226 2015-04-05 14:01:28.000000 trepan3k-1.2.9/test/unit/cmdhelper.py
+-rwxr-xr-x   0 rocky     (1000) rocky     (1000)     3505 2020-06-18 10:55:05.000000 trepan3k-1.2.9/test/unit/test-break.py
+-rwxr-xr-x   0 rocky     (1000) rocky     (1000)     3386 2020-06-14 02:56:20.000000 trepan3k-1.2.9/test/unit/test-brkpt.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1067 2023-05-27 12:22:16.000000 trepan3k-1.2.9/test/unit/test-bytecode.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1419 2015-04-05 14:01:28.000000 trepan3k-1.2.9/test/unit/test-clifns.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     2458 2015-04-05 22:56:16.000000 trepan3k-1.2.9/test/unit/test-cmd-alias.py
+-rwxr-xr-x   0 rocky     (1000) rocky     (1000)     2881 2020-06-18 10:54:29.000000 trepan3k-1.2.9/test/unit/test-cmdbreak.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     2471 2015-05-16 19:16:43.000000 trepan3k-1.2.9/test/unit/test-cmdfns.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     4640 2018-05-18 23:47:35.000000 trepan3k-1.2.9/test/unit/test-cmdproc.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     4176 2020-06-18 00:52:10.000000 trepan3k-1.2.9/test/unit/test-completion.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1107 2017-05-07 06:31:11.000000 trepan3k-1.2.9/test/unit/test-core.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     2568 2017-11-02 19:38:09.000000 trepan3k-1.2.9/test/unit/test-disassemble.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)      530 2015-04-05 14:01:28.000000 trepan3k-1.2.9/test/unit/test-except.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)      996 2015-04-05 14:01:28.000000 trepan3k-1.2.9/test/unit/test-fifo.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)      803 2015-05-16 19:17:16.000000 trepan3k-1.2.9/test/unit/test-finish.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     2145 2015-04-05 15:15:49.000000 trepan3k-1.2.9/test/unit/test-help.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1572 2015-04-05 14:01:28.000000 trepan3k-1.2.9/test/unit/test-info-files.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)      688 2015-04-05 21:55:08.000000 trepan3k-1.2.9/test/unit/test-inout-input.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)      995 2023-05-27 01:10:05.000000 trepan3k-1.2.9/test/unit/test-kill.py
+-rw-r--r--   0 rocky     (1000) rocky     (1000)     2254 2020-06-14 02:49:42.000000 trepan3k-1.2.9/test/unit/test-lib-complete.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1170 2015-04-05 14:01:28.000000 trepan3k-1.2.9/test/unit/test-lib-display.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)      861 2020-10-26 21:45:02.000000 trepan3k-1.2.9/test/unit/test-lib-eval.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1031 2017-05-07 06:31:11.000000 trepan3k-1.2.9/test/unit/test-lib-file.py
+-rwxr-xr-x   0 rocky     (1000) rocky     (1000)     3175 2020-05-10 23:15:25.000000 trepan3k-1.2.9/test/unit/test-lib-format.py
+-rwxr-xr-x   0 rocky     (1000) rocky     (1000)      877 2016-01-13 01:56:52.000000 trepan3k-1.2.9/test/unit/test-lib-pp.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)      798 2015-04-06 02:00:40.000000 trepan3k-1.2.9/test/unit/test-lib-printing.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     2101 2023-05-27 01:10:05.000000 trepan3k-1.2.9/test/unit/test-lib-sig.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1455 2015-04-05 23:50:30.000000 trepan3k-1.2.9/test/unit/test-lib-thread.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     3876 2020-06-18 10:59:50.000000 trepan3k-1.2.9/test/unit/test-list.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1096 2015-04-05 14:01:28.000000 trepan3k-1.2.9/test/unit/test-misc.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1074 2021-08-21 16:06:05.000000 trepan3k-1.2.9/test/unit/test-print.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1630 2015-04-05 14:01:28.000000 trepan3k-1.2.9/test/unit/test-processor.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)      604 2015-04-05 14:01:28.000000 trepan3k-1.2.9/test/unit/test-quit.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)      612 2015-04-05 22:59:05.000000 trepan3k-1.2.9/test/unit/test-run.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)      864 2015-04-06 00:12:45.000000 trepan3k-1.2.9/test/unit/test-stack.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1033 2015-04-05 14:01:28.000000 trepan3k-1.2.9/test/unit/test-step.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     2133 2015-05-16 19:17:26.000000 trepan3k-1.2.9/test/unit/test-subcmd.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1364 2017-11-02 19:38:09.000000 trepan3k-1.2.9/test/unit/test-tcp.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     1021 2020-05-10 11:25:11.000000 trepan3k-1.2.9/test/unit/test-user.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.284598 trepan3k-1.2.9/trepan/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     6950 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/__init__.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)    10910 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/__main__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     9491 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/api.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     7648 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/bwcli.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.288598 trepan3k-1.2.9/trepan/bwprocessor/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      709 2018-08-04 18:11:20.000000 trepan3k-1.2.9/trepan/bwprocessor/__init__.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.344597 trepan3k-1.2.9/trepan/bwprocessor/command/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1550 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/bwprocessor/command/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3558 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/bwprocessor/command/base_cmd.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3672 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/bwprocessor/command/mock.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2726 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/bwprocessor/command/quit.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2646 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/bwprocessor/command/step.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3742 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/bwprocessor/location.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    17955 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/bwprocessor/main.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1074 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/bwprocessor/msg.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     4907 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/client.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     3329 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/clifns.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    14719 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/debugger.py
+-rw-r--r--   0 rocky     (1000) rocky     (1000)     1377 2020-05-10 11:37:44.000000 trepan3k-1.2.9/trepan/exception.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.344597 trepan3k-1.2.9/trepan/inout/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      279 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/inout/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5380 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/inout/base.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4590 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/inout/fifoclient.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4775 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/inout/fifoserver.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5303 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/inout/input.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3017 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/inout/output.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2655 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/inout/scriptin.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4434 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/inout/stringarray.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4179 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/inout/tcpclient.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1519 2021-05-08 07:51:11.000000 trepan3k-1.2.9/trepan/inout/tcpfns.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     6394 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/inout/tcpserver.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2855 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/interface.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.348597 trepan3k-1.2.9/trepan/interfaces/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      789 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/interfaces/__init__.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     2534 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/interfaces/bullwinkle.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2898 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/interfaces/client.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      964 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/interfaces/comcodes.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     3798 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/interfaces/script.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4813 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/interfaces/server.py
+-rwxrwxr-x   0 rocky     (1000) rocky     (1000)     5907 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/interfaces/user.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.348597 trepan3k-1.2.9/trepan/lib/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      923 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/lib/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    12777 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/lib/breakpoint.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4228 2023-05-27 13:30:49.000000 trepan3k-1.2.9/trepan/lib/bytecode.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3784 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/lib/complete.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    17905 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/lib/core.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5871 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/lib/default.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3515 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/lib/deparse.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    12555 2023-05-27 13:30:49.000000 trepan3k-1.2.9/trepan/lib/disassemble.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4784 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/lib/display.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2499 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/lib/eval.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3982 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/lib/file.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    13988 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/lib/format.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3965 2021-07-17 20:00:44.000000 trepan3k-1.2.9/trepan/lib/pp.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4235 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/lib/printing.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    20059 2023-05-27 13:30:49.000000 trepan3k-1.2.9/trepan/lib/sighandler.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    14869 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/lib/stack.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2939 2020-05-09 20:08:59.000000 trepan3k-1.2.9/trepan/lib/thred.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2361 2021-06-17 13:36:06.000000 trepan3k-1.2.9/trepan/misc.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    13565 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/options.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     7499 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/post_mortem.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.352597 trepan3k-1.2.9/trepan/processor/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)        0 2020-05-09 19:25:16.000000 trepan3k-1.2.9/trepan/processor/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     6487 2023-05-27 13:30:49.000000 trepan3k-1.2.9/trepan/processor/cmd_addrlist.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     6111 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/cmdbreak.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     7362 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/cmdfns.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     6453 2023-05-27 13:30:49.000000 trepan3k-1.2.9/trepan/processor/cmdlist.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    43542 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/cmdproc.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.368597 trepan3k-1.2.9/trepan/processor/command/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1506 2021-01-30 06:01:07.000000 trepan3k-1.2.9/trepan/processor/command/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3259 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/alias.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5230 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/backtrace.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5031 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/processor/command/base_cmd.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     6753 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/processor/command/base_subcmd.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     9342 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/command/base_submgr.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4158 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/bpython.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4846 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/command/break.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1785 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/command/cd.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2429 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/clear.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2579 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/condition.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3162 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/continue.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3365 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/command/debug.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2306 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/delete.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     7525 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/processor/command/deparse.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3120 2023-05-27 13:30:49.000000 trepan3k-1.2.9/trepan/processor/command/deval.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2073 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/disable.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     9011 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/processor/command/disassemble.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3537 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/display.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2158 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/down.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2753 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/edit.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2094 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/enable.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3144 2023-05-27 13:30:49.000000 trepan3k-1.2.9/trepan/processor/command/eval.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2084 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/examine.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2034 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/command/exit.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3390 2023-05-27 13:30:49.000000 trepan3k-1.2.9/trepan/processor/command/finish.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     8951 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/command/frame.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2726 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/handle.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.368597 trepan3k-1.2.9/trepan/processor/command/help/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)        4 2015-06-12 09:10:07.000000 trepan3k-1.2.9/trepan/processor/command/help/.gitignore
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      327 2020-05-08 23:23:05.000000 trepan3k-1.2.9/trepan/processor/command/help/README.md
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      924 2017-11-02 19:38:09.000000 trepan3k-1.2.9/trepan/processor/command/help/arange.rst
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2326 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/processor/command/help/command.rst
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      336 2020-05-10 13:57:19.000000 trepan3k-1.2.9/trepan/processor/command/help/examples.rst
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      454 2015-06-12 09:10:07.000000 trepan3k-1.2.9/trepan/processor/command/help/filename.rst
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4192 2017-11-02 19:38:09.000000 trepan3k-1.2.9/trepan/processor/command/help/location.rst
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1421 2017-11-02 19:38:09.000000 trepan3k-1.2.9/trepan/processor/command/help/range.rst
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      517 2015-06-12 09:10:07.000000 trepan3k-1.2.9/trepan/processor/command/help/suffixes.rst
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    10049 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/command/help.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1469 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/info.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.388597 trepan3k-1.2.9/trepan/processor/command/info_subcmd/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1550 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2612 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/args.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4196 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/break.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2151 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/builtins.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4875 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/code.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1800 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/display.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5581 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/files.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4877 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/frame.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2931 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/globals.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5310 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/line.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5240 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/lines.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5111 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/locals.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2829 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/macro.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3233 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/offsets.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3390 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/pc.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3459 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/program.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2011 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/return.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2230 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/signals.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1352 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/source.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     7209 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/command/info_subcmd/threads.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     6512 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/command/ipython.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2875 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/command/jump.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     6033 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/kill.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     7808 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/command/list.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4062 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/macro.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3825 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/command/mock.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3244 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/next.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2499 2023-05-27 13:30:49.000000 trepan3k-1.2.9/trepan/processor/command/p.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2033 2023-05-27 13:30:49.000000 trepan3k-1.2.9/trepan/processor/command/pp.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     6379 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/command/python.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4666 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/quit.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2587 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/command/restart.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1901 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/run.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1430 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.424597 trepan3k-1.2.9/trepan/processor/command/set_subcmd/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      692 2023-05-27 12:37:38.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/__demo_helper__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1548 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2641 2021-01-25 02:40:06.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/asmfmt.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2362 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/autoeval.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2192 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/autolist.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1956 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/autopc.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1983 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/autopython.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1431 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/basename.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1312 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/cmdtrace.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1486 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/confirm.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2111 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/dbg_trepan.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2250 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/different.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2630 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/events.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4015 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/highlight.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1589 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/listsize.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1571 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/maxstring.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1815 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/patsub.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1785 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/skip.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2014 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/style.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1918 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/substitute.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1294 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/tempdir.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1445 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/trace.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      938 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/set_subcmd/width.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1454 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/show.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.428597 trepan3k-1.2.9/trepan/processor/command/show_subcmd/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      686 2023-05-27 12:43:48.000000 trepan3k-1.2.9/trepan/processor/command/show_subcmd/__demo_helper__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1431 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/command/show_subcmd/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2643 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/show_subcmd/aliases.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1436 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/show_subcmd/args.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1624 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/processor/command/show_subcmd/asmfmt.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1214 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/show_subcmd/autoeval.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1235 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/show_subcmd/autolist.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1238 2021-10-30 09:53:22.000000 trepan3k-1.2.9/trepan/processor/command/show_subcmd/autopc.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1295 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/show_subcmd/autopython.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1280 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/show_subcmd/basename.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1213 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/show_subcmd/confirm.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      358 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/show_subcmd/dbg_trepan.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1775 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/show_subcmd/highlight.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1095 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/show_subcmd/listsize.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1220 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/show_subcmd/style.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1767 2023-05-27 13:30:49.000000 trepan3k-1.2.9/trepan/processor/command/show_subcmd/substitute.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      952 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/processor/command/show_subcmd/tempdir.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3292 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/skip.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3028 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/source.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5193 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/step.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3721 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/command/tbreak.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1857 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/unalias.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2516 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/undisplay.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2400 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/command/up.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4544 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/command/whatis.py
+-rw-r--r--   0 rocky     (1000) rocky     (1000)     6142 2020-06-09 10:38:06.000000 trepan3k-1.2.9/trepan/processor/complete.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3532 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/frame.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     9588 2023-05-27 13:30:49.000000 trepan3k-1.2.9/trepan/processor/location.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.428597 trepan3k-1.2.9/trepan/processor/parse/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)        0 2017-11-02 19:38:09.000000 trepan3k-1.2.9/trepan/processor/parse/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     7822 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/parse/parser.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4733 2023-05-27 13:30:49.000000 trepan3k-1.2.9/trepan/processor/parse/scanner.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    13046 2023-05-27 13:30:49.000000 trepan3k-1.2.9/trepan/processor/parse/semantics.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1421 2023-05-27 01:10:05.000000 trepan3k-1.2.9/trepan/processor/parse/tok.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5784 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/processor/subcmd.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2040 2023-05-27 08:41:28.000000 trepan3k-1.2.9/trepan/processor/trace.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      255 2023-05-27 12:21:48.000000 trepan3k-1.2.9/trepan/version.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2922 2023-05-27 13:15:35.000000 trepan3k-1.2.9/trepan/vprocessor.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-05-27 13:31:12.428597 trepan3k-1.2.9/trepan3k.egg-info/
+-rw-r--r--   0 rocky     (1000) rocky     (1000)    15032 2023-05-27 13:31:12.000000 trepan3k-1.2.9/trepan3k.egg-info/PKG-INFO
+-rw-r--r--   0 rocky     (1000) rocky     (1000)    15392 2023-05-27 13:31:12.000000 trepan3k-1.2.9/trepan3k.egg-info/SOURCES.txt
+-rw-r--r--   0 rocky     (1000) rocky     (1000)        1 2023-05-27 13:31:12.000000 trepan3k-1.2.9/trepan3k.egg-info/dependency_links.txt
+-rw-r--r--   0 rocky     (1000) rocky     (1000)       81 2023-05-27 13:31:12.000000 trepan3k-1.2.9/trepan3k.egg-info/entry_points.txt
+-rw-r--r--   0 rocky     (1000) rocky     (1000)        1 2020-06-07 23:00:37.000000 trepan3k-1.2.9/trepan3k.egg-info/not-zip-safe
+-rw-r--r--   0 rocky     (1000) rocky     (1000)      172 2023-05-27 13:31:12.000000 trepan3k-1.2.9/trepan3k.egg-info/requires.txt
+-rw-r--r--   0 rocky     (1000) rocky     (1000)        7 2023-05-27 13:31:12.000000 trepan3k-1.2.9/trepan3k.egg-info/top_level.txt
```

### Comparing `trepan3k-1.2.8/COPYING` & `trepan3k-1.2.9/COPYING`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/ChangeLog` & `trepan3k-1.2.9/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,311 @@
+2023-05-27  rocky <rocky@gnu.org>
+
+	* NEWS.md, README.rst, __pkginfo__.py, trepan/api.py,
+	trepan/bwcli.py, trepan/bwprocessor/command/__init__.py,
+	trepan/bwprocessor/command/base_cmd.py, trepan/bwprocessor/msg.py,
+	trepan/client.py, trepan/debugger.py, trepan/inout/base.py,
+	trepan/inout/input.py, trepan/inout/output.py,
+	trepan/inout/stringarray.py, trepan/interface.py,
+	trepan/interfaces/client.py, trepan/interfaces/script.py,
+	trepan/interfaces/server.py, trepan/lib/default.py,
+	trepan/lib/eval.py, trepan/lib/format.py, trepan/lib/sighandler.py,
+	trepan/options.py, trepan/processor/command/base_cmd.py,
+	trepan/processor/command/base_subcmd.py,
+	trepan/processor/command/deparse.py,
+	trepan/processor/command/disassemble.py,
+	trepan/processor/command/help/command.rst,
+	trepan/processor/command/info_subcmd/code.py,
+	trepan/processor/command/show_subcmd/asmfmt.py,
+	trepan/processor/command/show_subcmd/substitute.py,
+	trepan/processor/command/show_subcmd/tempdir.py,
+	trepan/processor/location.py, trepan/processor/subcmd.py,
+	trepan/version.py, trepan/vprocessor.py: Get ready for release 1.2.9
+
+2023-05-27  rocky <rocky@gnu.org>
+
+	* trepan/processor/command/show_subcmd/substitute.py: Add "show
+	sustitute" command
+
+2023-05-27  rocky <rocky@gnu.org>
+
+	* admin-tools/setup-python-3.2.sh, test/unit/test-bytecode.py,
+	trepan/lib/bytecode.py: Sync with python 3.2 branch
+
+2023-05-27  rocky <rocky@gnu.org>
+
+	* .pre-commit-config.yaml, __pkginfo__.py, setup.py,
+	trepan/__main__.py, trepan/bwprocessor/command/__init__.py,
+	trepan/bwprocessor/command/quit.py, trepan/bwprocessor/location.py,
+	trepan/bwprocessor/main.py, trepan/bwprocessor/msg.py,
+	trepan/client.py, trepan/clifns.py, trepan/debugger.py,
+	trepan/inout/fifoclient.py, trepan/inout/fifoserver.py,
+	trepan/inout/input.py, trepan/inout/output.py,
+	trepan/inout/scriptin.py, trepan/inout/stringarray.py,
+	trepan/interfaces/bullwinkle.py, trepan/interfaces/user.py,
+	trepan/lib/breakpoint.py, trepan/lib/bytecode.py,
+	trepan/lib/complete.py, trepan/lib/core.py, trepan/lib/default.py,
+	trepan/lib/deparse.py, trepan/lib/disassemble.py,
+	trepan/lib/display.py, trepan/lib/eval.py, trepan/lib/file.py,
+	trepan/lib/format.py, trepan/lib/printing.py, trepan/lib/stack.py,
+	trepan/options.py, trepan/post_mortem.py,
+	trepan/processor/cmd_addrlist.py, trepan/processor/cmdfns.py,
+	trepan/processor/cmdproc.py, trepan/processor/command/base_cmd.py,
+	trepan/processor/command/base_subcmd.py,
+	trepan/processor/command/base_submgr.py,
+	trepan/processor/command/break.py, trepan/processor/command/cd.py,
+	trepan/processor/command/debug.py,
+	trepan/processor/command/deval.py,
+	trepan/processor/command/disassemble.py,
+	trepan/processor/command/eval.py, trepan/processor/command/exit.py,
+	trepan/processor/command/finish.py,
+	trepan/processor/command/frame.py,
+	trepan/processor/command/help.py,
+	trepan/processor/command/info_subcmd/files.py,
+	trepan/processor/command/info_subcmd/threads.py,
+	trepan/processor/command/ipython.py,
+	trepan/processor/command/jump.py, trepan/processor/command/list.py,
+	trepan/processor/command/mock.py, trepan/processor/command/p.py,
+	trepan/processor/command/pp.py, trepan/processor/command/python.py,
+	trepan/processor/command/restart.py,
+	trepan/processor/command/set_subcmd/__demo_helper__.py,
+	trepan/processor/command/show_subcmd/__demo_helper__.py,
+	trepan/processor/command/show_subcmd/__init__.py,
+	trepan/processor/command/whatis.py, trepan/processor/location.py,
+	trepan/processor/parse/scanner.py,
+	trepan/processor/parse/semantics.py, trepan/processor/subcmd.py,
+	trepan/processor/trace.py: linting ...  go over with flake8, isort and black
+
+2023-05-26  rocky <rocky@gnu.org>
+
+	* Makefile, trepan/__main__.py, trepan/api.py,
+	trepan/bwprocessor/command/mock.py, trepan/lib/format.py,
+	trepan/lib/printing.py, trepan/processor/cmdlist.py,
+	trepan/processor/command/tbreak.py: Misc lint
+
+2023-05-26  rocky <rocky@gnu.org>
+
+	* admin-tools/setup-master.sh: Bump master version
+
+2023-05-26  rocky <rocky@gnu.org>
+
+	* Makefile, trepan/bwcli.py, trepan/lib/sighandler.py,
+	trepan/processor/command/info_subcmd/__init__.py,
+	trepan/processor/command/info_subcmd/code.py,
+	trepan/processor/command/info_subcmd/frame.py,
+	trepan/processor/command/info_subcmd/line.py,
+	trepan/processor/command/info_subcmd/locals.py,
+	trepan/processor/command/info_subcmd/signals.py,
+	trepan/processor/command/set_subcmd/__init__.py: Misc pylint, isort
+	and black stuff
+
+2023-03-13  rocky <rocky@gnu.org>
+
+	* : commit a24009865cd1382bfbf0d3378e58a06866a9ab29 Author: rocky
+	<rocky@gnu.org> Date:   Tue Jan 24 21:56:14 2023 -0500
+
+2022-12-20  rocky <rocky@gnu.org>
+
+	* admin-tools/pyenv-newer-versions: Update neweset Python versions
+
+2022-11-25  rocky <rocky@gnu.org>
+
+	* .isort.cfg, test/unit/test-kill.py, test/unit/test-lib-sig.py,
+	trepan/lib/sighandler.py: Misc lint...  Add isort config
+
+2022-10-26  rocky <rocky@gnu.org>
+
+	* trepan/lib/sighandler.py: Ignore ignored signals
+
+2022-08-18  rocky <rocky@gnu.org>
+
+	* admin-tools/make-dist-newer.sh: Because of decompyle, specialize
+	wheel for version
+
+2022-06-26  R. Bernstein <rocky@users.noreply.github.com>
+
+	* : Merge pull request #42 from dev590t/feature/documentation Add tip about debug overhead
+
+2022-06-26  dev <dev@gmail.com>
+
+	* docs/commands/running.rst: Add tip about debug overhead
+
+2022-06-21  rocky <rocky@gnu.org>
+
+	* docs/install.rst: Fix incorrect tagging & update decompilation
+	info
+
+2022-06-21  R. Bernstein <rocky@users.noreply.github.com>
+
+	* : Merge pull request #41 from dev590t/feature/documentation Detail the installation instruction
+
+2022-06-21  dev <dev@gmail.com>
+
+	* docs/install.rst: Add new installation solution
+
+2022-06-21  dev <dev@gmail.com>
+
+	* docs/install.rst: Add installation requirement
+
+2022-06-19  rocky <rocky@gnu.org>
+
+	* .pre-commit-config.yaml, trepan/__main__.py, trepan/api.py,
+	trepan/bwcli.py, trepan/bwprocessor/command/__init__.py,
+	trepan/bwprocessor/command/base_cmd.py,
+	trepan/bwprocessor/command/mock.py,
+	trepan/bwprocessor/command/quit.py,
+	trepan/bwprocessor/command/step.py, trepan/bwprocessor/location.py,
+	trepan/bwprocessor/main.py, trepan/bwprocessor/msg.py,
+	trepan/clifns.py, trepan/debugger.py, trepan/inout/__init__.py,
+	trepan/inout/base.py, trepan/inout/fifoclient.py,
+	trepan/inout/fifoserver.py, trepan/inout/input.py,
+	trepan/inout/output.py, trepan/inout/scriptin.py,
+	trepan/inout/stringarray.py, trepan/inout/tcpclient.py,
+	trepan/inout/tcpserver.py, trepan/interface.py,
+	trepan/interfaces/__init__.py, trepan/interfaces/bullwinkle.py,
+	trepan/interfaces/client.py, trepan/interfaces/comcodes.py,
+	trepan/interfaces/script.py, trepan/interfaces/server.py,
+	trepan/interfaces/user.py, trepan/lib/__init__.py,
+	trepan/lib/breakpoint.py, trepan/lib/complete.py,
+	trepan/lib/core.py, trepan/lib/disassemble.py,
+	trepan/lib/format.py, trepan/lib/printing.py,
+	trepan/lib/sighandler.py, trepan/lib/stack.py, trepan/options.py,
+	trepan/post_mortem.py, trepan/processor/cmd_addrlist.py,
+	trepan/processor/cmdfns.py, trepan/processor/cmdlist.py,
+	trepan/processor/cmdproc.py, trepan/processor/command/alias.py,
+	trepan/processor/command/backtrace.py,
+	trepan/processor/command/base_cmd.py,
+	trepan/processor/command/base_subcmd.py,
+	trepan/processor/command/base_submgr.py,
+	trepan/processor/command/bpython.py,
+	trepan/processor/command/break.py, trepan/processor/command/cd.py,
+	trepan/processor/command/clear.py,
+	trepan/processor/command/condition.py,
+	trepan/processor/command/continue.py,
+	trepan/processor/command/debug.py,
+	trepan/processor/command/delete.py,
+	trepan/processor/command/deparse.py,
+	trepan/processor/command/deval.py,
+	trepan/processor/command/disable.py,
+	trepan/processor/command/disassemble.py,
+	trepan/processor/command/display.py,
+	trepan/processor/command/down.py, trepan/processor/command/edit.py,
+	trepan/processor/command/enable.py,
+	trepan/processor/command/examine.py,
+	trepan/processor/command/exit.py,
+	trepan/processor/command/finish.py,
+	trepan/processor/command/frame.py,
+	trepan/processor/command/handle.py,
+	trepan/processor/command/help.py, trepan/processor/command/info.py,
+	trepan/processor/command/info_subcmd/__init__.py,
+	trepan/processor/command/info_subcmd/args.py,
+	trepan/processor/command/info_subcmd/break.py,
+	trepan/processor/command/info_subcmd/builtins.py,
+	trepan/processor/command/info_subcmd/code.py,
+	trepan/processor/command/info_subcmd/display.py,
+	trepan/processor/command/info_subcmd/files.py,
+	trepan/processor/command/info_subcmd/frame.py,
+	trepan/processor/command/info_subcmd/globals.py,
+	trepan/processor/command/info_subcmd/line.py,
+	trepan/processor/command/info_subcmd/lines.py,
+	trepan/processor/command/info_subcmd/locals.py,
+	trepan/processor/command/info_subcmd/macro.py,
+	trepan/processor/command/info_subcmd/offsets.py,
+	trepan/processor/command/info_subcmd/pc.py,
+	trepan/processor/command/info_subcmd/program.py,
+	trepan/processor/command/info_subcmd/return.py,
+	trepan/processor/command/info_subcmd/signals.py,
+	trepan/processor/command/info_subcmd/source.py,
+	trepan/processor/command/info_subcmd/threads.py,
+	trepan/processor/command/ipython.py,
+	trepan/processor/command/jump.py, trepan/processor/command/kill.py,
+	trepan/processor/command/list.py,
+	trepan/processor/command/macro.py,
+	trepan/processor/command/next.py, trepan/processor/command/p.py,
+	trepan/processor/command/pp.py, trepan/processor/command/python.py,
+	trepan/processor/command/quit.py,
+	trepan/processor/command/restart.py,
+	trepan/processor/command/run.py, trepan/processor/command/set.py,
+	trepan/processor/command/set_subcmd/__demo_helper__.py,
+	trepan/processor/command/set_subcmd/autoeval.py,
+	trepan/processor/command/set_subcmd/autolist.py,
+	trepan/processor/command/set_subcmd/autopc.py,
+	trepan/processor/command/set_subcmd/autopython.py,
+	trepan/processor/command/set_subcmd/basename.py,
+	trepan/processor/command/set_subcmd/cmdtrace.py,
+	trepan/processor/command/set_subcmd/confirm.py,
+	trepan/processor/command/set_subcmd/dbg_trepan.py,
+	trepan/processor/command/set_subcmd/different.py,
+	trepan/processor/command/set_subcmd/events.py,
+	trepan/processor/command/set_subcmd/highlight.py,
+	trepan/processor/command/set_subcmd/listsize.py,
+	trepan/processor/command/set_subcmd/maxstring.py,
+	trepan/processor/command/set_subcmd/patsub.py,
+	trepan/processor/command/set_subcmd/skip.py,
+	trepan/processor/command/set_subcmd/style.py,
+	trepan/processor/command/set_subcmd/substitute.py,
+	trepan/processor/command/set_subcmd/tempdir.py,
+	trepan/processor/command/set_subcmd/trace.py,
+	trepan/processor/command/set_subcmd/width.py,
+	trepan/processor/command/show.py,
+	trepan/processor/command/show_subcmd/__demo_helper__.py,
+	trepan/processor/command/show_subcmd/__init__.py,
+	trepan/processor/command/show_subcmd/aliases.py,
+	trepan/processor/command/show_subcmd/args.py,
+	trepan/processor/command/show_subcmd/asmfmt.py,
+	trepan/processor/command/show_subcmd/autoeval.py,
+	trepan/processor/command/show_subcmd/autolist.py,
+	trepan/processor/command/show_subcmd/autopython.py,
+	trepan/processor/command/show_subcmd/basename.py,
+	trepan/processor/command/show_subcmd/confirm.py,
+	trepan/processor/command/show_subcmd/dbg_trepan.py,
+	trepan/processor/command/show_subcmd/highlight.py,
+	trepan/processor/command/show_subcmd/listsize.py,
+	trepan/processor/command/show_subcmd/style.py,
+	trepan/processor/command/show_subcmd/tempdir.py,
+	trepan/processor/command/skip.py,
+	trepan/processor/command/source.py,
+	trepan/processor/command/step.py,
+	trepan/processor/command/tbreak.py,
+	trepan/processor/command/unalias.py,
+	trepan/processor/command/undisplay.py,
+	trepan/processor/command/up.py, trepan/processor/command/whatis.py,
+	trepan/processor/frame.py, trepan/processor/location.py,
+	trepan/processor/parse/parser.py,
+	trepan/processor/parse/scanner.py,
+	trepan/processor/parse/semantics.py, trepan/processor/parse/tok.py,
+	trepan/processor/subcmd.py, trepan/processor/trace.py,
+	trepan/vprocessor.py: reformat via black version 22.3.0
+
+2022-06-05  rocky <rocky@gnu.org>
+
+	* trepan/processor/cmdbreak.py: Squelch traceback on break in
+	unparsable file
+
+2022-03-10  rocky <rocky@gnu.org>
+
+	* trepan/__init__.py, trepan/lib/deparse.py: Misc lint
+
+2022-01-02  rocky <rocky@gnu.org>
+
+	* __pkginfo__.py, trepan/__main__.py: Misc small bugs and tweaks
+
+2021-11-25  rocky <rocky@gnu.org>
+
+	* admin-tools/pyenv-newer-versions, trepan/processor/cmdfns.py: 
+	Remove PYTHON_VERSION
+
+2021-11-19  rocky <rocky@gnu.org>
+
+	* __pkginfo__.py, trepan/version.py: Bump decompyle version to 3.8.0
+
 2021-11-05  rocky <rocky@gnu.org>
 
-	* __pkginfo__.py, trepan/version.py: Get ready for release 1.2.8
+	* NEWS.md, __pkginfo__.py, trepan/version.py: Get ready for release
+	1.2.8
 
 2021-11-01  rocky <rocky@gnu.org>
 
 	* __pkginfo__.py: Admnistrivia
 
 2021-10-30  rocky <rocky@gnu.org>
```

### Comparing `trepan3k-1.2.8/Makefile` & `trepan3k-1.2.9/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 	$(PYTHON) setup.py --long-description | ./rst2html.py > python3-trepan.html
 
 #: Lint program
 flake8:
 	flake8 trepan
 
 #: Run all tests: unit, functional and integration verbosely
-check: test-unit test-functional test-integration # flake8
+# check: test-unit test-functional test-integration # flake8
+check: test-unit test-integration # flake8
 
 #: Run unit (white-box) tests
 test-unit:
 	$(PYTHON) ./setup.py nosetests
 
 #: Run unit (white-box) tests
 test-unit-short:
@@ -61,15 +62,15 @@
 
 #: Clean up temporary files
 clean:
 	$(PYTHON) ./setup.py $@
 
 #: Create source (tarball) and binary (egg) distribution
 dist: check-rst
-	bash ./admin-tools/make-dist.sh
+	bash ./admin-tools/make-dist-newer.sh
 
 #: Create source tarball
 sdist: check-rst
 	$(PYTHON) ./setup.py sdist
 
 #: Style check. Set env var LINT to pyflakes, flake, or flake8
 lint:
```

### Comparing `trepan3k-1.2.8/NEWS.md` & `trepan3k-1.2.9/NEWS.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+1.2.9 2023-05-27
+================
+
+Commands that are useful in remote envionments and docker:
+
+* Add "set tempdir" to set location of TEMPDIR (useful docker)
+* Add "set/show substitute"
+
+Other changes:
+
+* Blacken, and isort, codespell, and lint many files
+* ignore ignored signal
+* specialize decompiler to decompyle for 3.7 and 3.8
+* fix incorrect tagging in install doc and update decompilation info
+* Squelch traceback on break in unparsable file
+
 1.2.8 2021-11-05
 ================
 
 * Convert to use newer xdis (which handles 3.10)
 * sphinx doc updates
 * Generalize subcmdmgr for use in trepan-xpy trepan-xpy has a new class of subcommands Vmstack.
   So we need to be aable to allow it to set trepanxpy as a base directory to look for
```

### Comparing `trepan3k-1.2.8/PKG-INFO` & `trepan3k-1.2.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,342 +1,344 @@
 Metadata-Version: 2.1
 Name: trepan3k
-Version: 1.2.8
+Version: 1.2.9
 Summary: GDB-like Python Debugger in the Trepan family
 Home-page: http://github.com/rocky/python3-trepan/
 Author: Rocky Bernstein
 Author-email: rocky@gnu.org
 License: GPL3
-Description: |TravisCI| |CircleCI| |Pypi Installs| |license| |Supported Python Versions|
-        
-        |packagestatus|
-        
-        .. contents:: :local:
-        
-        Abstract
-        ========
-        
-        This is a gdb-like debugger for Python. It is a rewrite of *pdb* from
-        the ground up. It is both a high-level debugger as well as a
-        lower-level bytecode debugger. By lower-level debugger, I mean that it
-        understands a lot about byte code and will try to make use of that in
-        its normal higher-level instructions.
-        
-        A command-line interface (CLI) is provided as well as an remote access
-        interface over TCP/IP.
-        
-        See the Tutorial_ for how to use. See ipython-trepan_ for using this
-        in *ipython* or an *ipython notebook*.
-        
-        This package is for Python 3.2 and above. See trepan2_ for the same code
-        modified to work with Python 2.
-        
-        Features
-        ========
-        
-        Since this debugger is similar to other_ trepanning_ debuggers_ and *gdb*
-        in general, knowledge gained by learning this is transferable to those
-        debuggers and vice versa.
-        
-        There's a lot of cool stuff here that's not in the stock
-        Python debugger *pdb*, or in any other Python debugger that I know about.
-        
-        
-        More Exact location information
-        -------------------------------
-        
-        Python reports line information on the granularity of a line. To get
-        more precise information, we can (de)parse into Python the byte code
-        around a bytecode offset such as the place you are stopped at.
-        
-        So far as I know, there is no other debugger that decompile code at runtime.
-        
-        See the deparse_ command for details.
-        
-        We use information in the line number table in byte to understand
-        which lines are breakpointable, and in which module or function the
-        line appears in. Use info_line_ to see this information.
-        
-        In the future we may allow specifiying an offset to indicate which
-        offset to stop at when there are several choices for a given line
-        number.
-        
-        
-        Debugging Python bytecode (no source available)
-        -----------------------------------------------
-        
-        You can pass the debugger the name of Python bytecode and many times,
-        the debugger will merrily proceed.  This debugger tries very hard find
-        the source code. Either by using the current executable search path
-        (e.g. ``PATH``) or for some by looking inside the bytecode for a
-        filename in the main code object (``co_filename``) and applying that
-        with a search path which takes into account directory where the
-        bytecode lives.
-        
-        Failing to find source code this way, and in other situations where
-        source code can't be found, the debugger will decompile the bytecode
-        and use that for showing source test. *This allows us to debug `eval`'d
-        or `exec''d code.*
-        
-        But if you happen to know where the source code is located, you can
-        associate a file source code with the current name listed in the
-        bytecode. See the set_substitute_ command for details here.
-        
-        Source-code Syntax Colorization
-        -------------------------------
-        
-        Terminal source code is colorized via pygments_ . And with that you
-        can set the pygments color style, e.g. "colorful", "paraiso-dark". See
-        set_style_ . Furthermore, we make use of terminal bold and emphasized
-        text in debugger output and help text. Of course, you can also turn
-        this off. You can use your own
-        pygments_style_, provided you have a terminal that supports 256
-        colors. If your terminal supports the basic ANSI color sequences only,
-        we support that too in both dark and light themes.
-        
-        
-        Command Completion
-        ------------------
-        
-        GNU readline command completion is available. Command completion is
-        not just a simple static list, but varies depending on the
-        context. For example, for frame-changing commands which take optional
-        numbers, on the list of *valid numbers* is considered.
-        
-        Terminal Handling
-        -----------------
-        
-        We can adjust debugger output depending on the line width of your
-        terminal. If it changes, or you want to adjust it, see set_width_ .
-        
-        Smart Eval
-        ----------
-        
-        If you want to evaluate the current source line before it is run in
-        the code, use ``eval``. To evaluate text of a common fragment of line,
-        such as the expression part of an *if* statement, you can do that with
-        ``eval?``. See eval_ for more information.
-        
-        Function Breakpoints
-        ---------------------
-        
-        Many Python debuggers only allow setting a breakpoint at a line event
-        and functions are treated like line numbers. But functions and lines
-        are fundamentally different. If I write::
-        
-             def five(): return 5
-        
-        this line means has three different kinds of things. First there is
-        the code in Python that defines function ``five()`` for the first
-        time. Then there is the function itself, and then there is some code
-        inside that function.
-        
-        In this debugger, you can give the name of a *function* by surrounding
-        adding ``()`` at the end::
-        
-            break five()
-        
-        Also ``five`` could be a method of an object that is currently defined when the
-        ``breakpoint`` command is given::
-        
-            self.five()
-        
-        More Stepping Control
-        ---------------------
-        
-        Sometimes you want small steps, and sometimes large stepping.
-        
-        This fundamental issue is handled in a couple ways:
-        
-        Step Granularity
-        ................
-        
-        There are now ``step`` *event* and ``next`` *event* commands with
-        aliases to ``s+``, ``s>`` and so on. The plus-suffixed commands force
-        a different line on a subsequent stop, the dash-suffixed commands
-        don't.  Suffixes ``>``, ``<``, and ``!`` specify ``call``, ``return``
-        and ``exception`` events respectively. And without a suffix you get
-        the default; this is set by the ``set different`` command.
-        
-        Event Filtering and Tracing
-        ...........................
-        
-        By default the debugger stops at every event: ``call``, ``return``,
-        ``line``, ``exception``, ``c-call``, ``c-exception``. If you just want
-        to stop at ``line`` events (which is largely what you happens in
-        *pdb*) you can. If however you just want to stop at calls and returns,
-        that's possible too. Or pick some combination.
-        
-        In conjunction with handling *all* events by default, the event status is shown when stopped. The reason for stopping is also available via ``info program``.
-        
-        Event Tracing of Calls and Returns
-        ----------------------------------
-        
-        I'm not sure why this was not done before. Probably because of the
-        lack of the ability to set and move by different granularities,
-        tracing calls and returns lead to too many uninteresting stops (such
-        as at the same place you just were at). Also, stopping on function
-        definitions probably also added to this tedium.
-        
-        Because we're really handling return events, we can show you the return value. (*pdb* has an "undocumented" *retval* command that doesn't seem to work.)
-        
-        Debugger Macros via Python Lambda expressions
-        ---------------------------------------------
-        
-        There are debugger macros.  In *gdb*, there is a *macro* debugger
-        command to extend debugger commands.
-        
-        However Python has its own rich programming language so it seems silly
-        to recreate the macro language that is in *gdb*. Simpler and more
-        powerful is just to use Python here. A debugger macro here is just a
-        lambda expression which returns a string or a list of strings. Each
-        string returned should be a debugger command.
-        
-        We also have *aliases* for the extremely simple situation where you
-        want to give an alias to an existing debugger command. But beware:
-        some commands, like step_ inspect command suffixes and change their
-        behavior accordingly.
-        
-        We also envision a number of other ways to allow extension of this
-        debugger either through additional modules, or user-supplied debugger
-        command directories.
-        
-        Byte-code Instruction Introspection
-        ------------------------------------
-        
-        We do more in the way of looking at the byte codes to give better information. Through this we can provide:
-        
-        * a *skip* command. It is like the *jump* command, but you don't have
-          to deal with line numbers.
-        * disassembly of code fragments. You can now disassemble relative to
-          the stack frames you are currently stopped at.
-        * Better interpretation of where you are when inside *execfile* or
-          *exec*. (But really though this is probably a Python compiler
-          misfeature.)
-        * Check that breakpoints are set only where they make sense.
-        * A more accurate determination of if you are at a function-defining
-          *def* or *class* statements (because the caller instruction contains
-          ``MAKE_FUNCTION`` or ``BUILD_CLASS``.)
-        
-        Even without "deparsing" mentioned above, the ability to disassemble
-        where the PC is currently located (see `info pc <info_pc>`_), by line
-        number range or byte-offset range lets you tell exactly where you are
-        and code is getting run.
-        
-        Some Debugger Command Arguments can be Variables and Expressions
-        ----------------------------------------------------------------
-        
-        Commands that take integer arguments like *up*, *list*, or
-        *disassemble* allow you to use a Python expression which may include
-        local or global variables that evaluates to an integer. This
-        eliminates the need in *gdb* for special "dollar" debugger
-        variables. (Note however because of *shlex* parsing, expressions can't
-        have embedded blanks.)
-        
-        Out-of-Process Debugging
-        ------------------------
-        
-        You can now debug your program in a different process or even a different computer on a different network!
-        
-        Related, is flexible support for remapping path names from file
-        system, e.g. that inside a docker container or on a remote filesystem
-        with locally-installed files. See subst_ for more information.
-        
-        Egg, Wheel, and Tarballs
-        ------------------------
-        
-        Can be installed via the usual *pip* or *easy_install*. There is a
-        source tarball. `How To Install
-        <https://python3-trepan.readthedocs.io/en/latest/install.html>`_ has
-        full instructions and installing from git and by other means.
-        
-        Modularity
-        ----------
-        
-        The Debugger plays nice with other trace hooks. You can have several debugger objects.
-        
-        Many of the things listed below doesn't directly effect end-users, but
-        it does eventually by way of more robust and featureful code. And
-        keeping developers happy is a good thing.(TM)
-        
-        * Commands and subcommands are individual classes now, not methods in a class. This means they now have properties like the context in which they can be run, minimum abbreviation name or alias names. To add a new command you basically add a file in a directory.
-        * I/O is it's own layer. This simplifies interactive readline behavior from reading commands over a TCP socket.
-        * An interface is it's own layer. Local debugging, remote debugging, running debugger commands from a file (``source``) are different interfaces. This means, for example, that we are able to give better error reporting if a debugger command file has an error.
-        * There is an experimental Python-friendly interface for front-ends
-        * more testable. Much more unit and functional tests. More of *pydb*'s integration test will eventually be added.
-        
-        Documentation
-        -------------
-        
-        Documentation: http://python3-trepan.readthedocs.org
-        
-        See Also
-        --------
-        
-        * trepan2_ : trepan debugger for Python 2
-        * trepanxpy_ : trepan debugger for `x-python <https://pypi.python.org/pypi/x-python>`_, the bytecode interpreter written in Python
-        * pydbgr_  : previous incarnation of the Python 2 debugger
-        * pydb_ : even older incarnation of debugger (for very old Python 2)
-        * Tutorial_: Tutorial for how to use
-        * https://github.com/rocky/trepan-xpy : Python debugger using this code to support `x-python <https://pypi.python.org/pypi/x-python>`_
-        * https://pypi.python.org/pypi/uncompyle6 : Python decompiler
-        * https://pypi.python.org/pypi/decompyle3 : Python 3.7 and 3.8 decompiler
-        * https://pypi.python.org/pypi/xdis : cross-platform disassembler
-        
-        
-        .. _pygments:  http://pygments.org
-        .. _pygments_style:  http://pygments.org/docs/styles/
-        .. _howtoinstall: https://github.com/rocky/python3-trepan/wiki/How-to-Install
-        .. _pydb:  http://bashdb.sf.net/pydb
-        .. _pydbgr: https://pypi.python.org/pypi/pydbgr
-        .. _trepan2: https://pypi.python.org/pypi/trepan2
-        .. _trepan3: https://github.com/rocky/python3-trepan
-        .. _trepanxpy: https://pypi.python.org/pypi/trepanxpy
-        .. _other: https://repology.org/project/zshdb/versions
-        .. _trepanning: https://rubygems.org/gems/trepanning
-        .. _debuggers: https://metacpan.org/pod/Devel::Trepan
-        .. _this: http://bashdb.sourceforge.net/pydb/features.html
-        .. _Tutorial: http://python2-trepan.readthedocs.io/en/latest/entry-exit.html
-        .. |downloads| image:: https://img.shields.io/pypi/dd/trepan3k.svg
-           :target: https://pypi.python.org/pypi/trepan3k/
-        .. |TravisCI| image:: https://api.travis-ci.org/rocky/python3-trepan.svg
-           :target: https://travis-ci.org/rocky/python3-trepan
-        .. |CircleCI| image:: https://circleci.com/gh/rocky/python3-trepan.svg?style=svg
-           :target: https://circleci.com/gh/rocky/python3-trepan
-        .. _ipython-trepan: https://github.com/rocky/ipython-trepan
-        .. |license| image:: https://img.shields.io/pypi/l/trepan.svg
-            :target: https://pypi.python.org/pypi/trepan3k
-            :alt: License
-        .. _deparse:  https://python3-trepan.readthedocs.io/en/latest/commands/data/deparse.html
-        .. _info_line:  https://python3-trepan.readthedocs.io/en/latest/commands/info/line.html
-        .. _set_style:  https://python3-trepan.readthedocs.org/en/latest/commands/set/style.html
-        .. _set_substitute:  https://python3-trepan.readthedocs.org/en/latest/commands/set/substitute.html
-        .. _set_width:  https://python3-trepan.readthedocs.org/en/latest/commands/set/width.html
-        .. _eval: https://python3-trepan.readthedocs.org/en/latest/commands/data/eval.html
-        .. _step: https://python3-trepan.readthedocs.org/en/latest/commands/running/step.html
-        .. _subst: https://python3-trepan.readthedocs.io/en/latest/commands/set/substitute.html
-        .. _install: http://python3-trepan.readthedocs.org/en/latest/install.html
-        .. |Supported Python Versions| image:: https://img.shields.io/pypi/pyversions/trepan3k.svg
-           :target: https://pypi.python.org/pypi/trepan3k/
-        .. |Pypi Installs| image:: https://pepy.tech/badge/trepan3k
-        .. |packagestatus| image:: https://repology.org/badge/vertical-allrepos/python:trepan3k.svg
-        		 :target: https://repology.org/project/python:trepan3k/versions
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5 
-Classifier: Programming Language :: Python :: 3.6 
-Classifier: Programming Language :: Python :: 3.7 
-Classifier: Programming Language :: Python :: 3.8 
-Classifier: Programming Language :: Python :: 3.9 
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/x-rst
+License-File: COPYING
+
+|CircleCI| |Pypi Installs| |license| |Supported Python Versions|
+
+|packagestatus|
+
+.. contents:: :local:
+
+Abstract
+========
+
+This is a gdb-like debugger for Python. It is a rewrite of *pdb* from
+the ground up. It is both a high-level debugger as well as a
+lower-level bytecode debugger. By lower-level debugger, I mean that it
+understands a lot about byte code and will try to make use of that in
+its normal higher-level instructions.
+
+A command-line interface (CLI) is provided as well as an remote access
+interface over TCP/IP.
+
+See the Tutorial_ for how to use. See ipython-trepan_ for using this
+in *ipython* or an *ipython notebook*.
+
+This package is for Python 3.2 and above. See trepan2_ for the same code
+modified to work with Python 2.
+
+Features
+========
+
+Since this debugger is similar to other_ trepanning_ debuggers_ and *gdb*
+in general, knowledge gained by learning this is transferable to those
+debuggers and vice versa.
+
+There's a lot of cool stuff here that's not in the stock
+Python debugger *pdb*, or in any other Python debugger that I know about.
+
+
+More Exact location information
+-------------------------------
+
+Python reports line information on the granularity of a line. To get
+more precise information, we can (de)parse into Python the byte code
+around a bytecode offset such as the place you are stopped at.
+
+So far as I know, there is no other debugger that decompile code at runtime.
+
+See the deparse_ command for details.
+
+We use information in the line number table in byte to understand
+which lines are breakpointable, and in which module or function the
+line appears in. Use info_line_ to see this information.
+
+In the future we may allow specifiying an offset to indicate which
+offset to stop at when there are several choices for a given line
+number.
+
+
+Debugging Python bytecode (no source available)
+-----------------------------------------------
+
+You can pass the debugger the name of Python bytecode and many times,
+the debugger will merrily proceed.  This debugger tries very hard find
+the source code. Either by using the current executable search path
+(e.g. ``PATH``) or for some by looking inside the bytecode for a
+filename in the main code object (``co_filename``) and applying that
+with a search path which takes into account directory where the
+bytecode lives.
+
+Failing to find source code this way, and in other situations where
+source code can't be found, the debugger will decompile the bytecode
+and use that for showing source test. *This allows us to debug `eval`'d
+or `exec''d code.*
+
+But if you happen to know where the source code is located, you can
+associate a file source code with the current name listed in the
+bytecode. See the set_substitute_ command for details here.
+
+Source-code Syntax Colorization
+-------------------------------
+
+Terminal source code is colorized via pygments_ . And with that you
+can set the pygments color style, e.g. "colorful", "paraiso-dark". See
+set_style_ . Furthermore, we make use of terminal bold and emphasized
+text in debugger output and help text. Of course, you can also turn
+this off. You can use your own
+pygments_style_, provided you have a terminal that supports 256
+colors. If your terminal supports the basic ANSI color sequences only,
+we support that too in both dark and light themes.
+
+
+Command Completion
+------------------
+
+GNU readline command completion is available. Command completion is
+not just a simple static list, but varies depending on the
+context. For example, for frame-changing commands which take optional
+numbers, on the list of *valid numbers* is considered.
+
+Terminal Handling
+-----------------
+
+We can adjust debugger output depending on the line width of your
+terminal. If it changes, or you want to adjust it, see set_width_ .
+
+Smart Eval
+----------
+
+If you want to evaluate the current source line before it is run in
+the code, use ``eval``. To evaluate text of a common fragment of line,
+such as the expression part of an *if* statement, you can do that with
+``eval?``. See eval_ for more information.
+
+Function Breakpoints
+---------------------
+
+Many Python debuggers only allow setting a breakpoint at a line event
+and functions are treated like line numbers. But functions and lines
+are fundamentally different. If I write::
+
+     def five(): return 5
+
+this line means has three different kinds of things. First there is
+the code in Python that defines function ``five()`` for the first
+time. Then there is the function itself, and then there is some code
+inside that function.
+
+In this debugger, you can give the name of a *function* by surrounding
+adding ``()`` at the end::
+
+    break five()
+
+Also ``five`` could be a method of an object that is currently defined when the
+``breakpoint`` command is given::
+
+    self.five()
+
+More Stepping Control
+---------------------
+
+Sometimes you want small steps, and sometimes large stepping.
+
+This fundamental issue is handled in a couple ways:
+
+Step Granularity
+................
+
+There are now ``step`` *event* and ``next`` *event* commands with
+aliases to ``s+``, ``s>`` and so on. The plus-suffixed commands force
+a different line on a subsequent stop, the dash-suffixed commands
+don't.  Suffixes ``>``, ``<``, and ``!`` specify ``call``, ``return``
+and ``exception`` events respectively. And without a suffix you get
+the default; this is set by the ``set different`` command.
+
+Event Filtering and Tracing
+...........................
+
+By default the debugger stops at every event: ``call``, ``return``,
+``line``, ``exception``, ``c-call``, ``c-exception``. If you just want
+to stop at ``line`` events (which is largely what you happens in
+*pdb*) you can. If however you just want to stop at calls and returns,
+that's possible too. Or pick some combination.
+
+In conjunction with handling *all* events by default, the event status is shown when stopped. The reason for stopping is also available via ``info program``.
+
+Event Tracing of Calls and Returns
+----------------------------------
+
+I'm not sure why this was not done before. Probably because of the
+lack of the ability to set and move by different granularities,
+tracing calls and returns lead to too many uninteresting stops (such
+as at the same place you just were at). Also, stopping on function
+definitions probably also added to this tedium.
+
+Because we're really handling return events, we can show you the return value. (*pdb* has an "undocumented" *retval* command that doesn't seem to work.)
+
+Debugger Macros via Python Lambda expressions
+---------------------------------------------
+
+There are debugger macros.  In *gdb*, there is a *macro* debugger
+command to extend debugger commands.
+
+However Python has its own rich programming language so it seems silly
+to recreate the macro language that is in *gdb*. Simpler and more
+powerful is just to use Python here. A debugger macro here is just a
+lambda expression which returns a string or a list of strings. Each
+string returned should be a debugger command.
+
+We also have *aliases* for the extremely simple situation where you
+want to give an alias to an existing debugger command. But beware:
+some commands, like step_ inspect command suffixes and change their
+behavior accordingly.
+
+We also envision a number of other ways to allow extension of this
+debugger either through additional modules, or user-supplied debugger
+command directories.
+
+Byte-code Instruction Introspection
+------------------------------------
+
+We do more in the way of looking at the byte codes to give better information. Through this we can provide:
+
+* a *skip* command. It is like the *jump* command, but you don't have
+  to deal with line numbers.
+* disassembly of code fragments. You can now disassemble relative to
+  the stack frames you are currently stopped at.
+* Better interpretation of where you are when inside *execfile* or
+  *exec*. (But really though this is probably a Python compiler
+  misfeature.)
+* Check that breakpoints are set only where they make sense.
+* A more accurate determination of if you are at a function-defining
+  *def* or *class* statements (because the caller instruction contains
+  ``MAKE_FUNCTION`` or ``BUILD_CLASS``.)
+
+Even without "deparsing" mentioned above, the ability to disassemble
+where the PC is currently located (see `info pc <info_pc>`_), by line
+number range or byte-offset range lets you tell exactly where you are
+and code is getting run.
+
+Some Debugger Command Arguments can be Variables and Expressions
+----------------------------------------------------------------
+
+Commands that take integer arguments like *up*, *list*, or
+*disassemble* allow you to use a Python expression which may include
+local or global variables that evaluates to an integer. This
+eliminates the need in *gdb* for special "dollar" debugger
+variables. (Note however because of *shlex* parsing, expressions can't
+have embedded blanks.)
+
+Out-of-Process Debugging
+------------------------
+
+You can now debug your program in a different process or even a different computer on a different network!
+
+Related, is flexible support for remapping path names from file
+system, e.g. that inside a docker container or on a remote filesystem
+with locally-installed files. See subst_ for more information.
+
+Egg, Wheel, and Tarballs
+------------------------
+
+Can be installed via the usual *pip* or *easy_install*. There is a
+source tarball. `How To Install
+<https://python3-trepan.readthedocs.io/en/latest/install.html>`_ has
+full instructions and installing from git and by other means.
+
+Modularity
+----------
+
+The Debugger plays nice with other trace hooks. You can have several debugger objects.
+
+Many of the things listed below doesn't directly effect end-users, but
+it does eventually by way of more robust and featureful code. And
+keeping developers happy is a good thing.(TM)
+
+* Commands and subcommands are individual classes now, not methods in a class. This means they now have properties like the context in which they can be run, minimum abbreviation name or alias names. To add a new command you basically add a file in a directory.
+* I/O is it's own layer. This simplifies interactive readline behavior from reading commands over a TCP socket.
+* An interface is it's own layer. Local debugging, remote debugging, running debugger commands from a file (``source``) are different interfaces. This means, for example, that we are able to give better error reporting if a debugger command file has an error.
+* There is an experimental Python-friendly interface for front-ends
+* more testable. Much more unit and functional tests. More of *pydb*'s integration test will eventually be added.
+
+Documentation
+-------------
+
+Documentation: http://python3-trepan.readthedocs.org
+
+See Also
+--------
+
+* trepan2_ : trepan debugger for Python 2
+* trepanxpy_ : trepan debugger for `x-python <https://pypi.python.org/pypi/x-python>`_, the bytecode interpreter written in Python
+* pydbgr_  : previous incarnation of the Python 2 debugger
+* pydb_ : even older incarnation of debugger (for very old Python 2)
+* Tutorial_: Tutorial for how to use
+* https://github.com/rocky/trepan-xpy : Python debugger using this code to support `x-python <https://pypi.python.org/pypi/x-python>`_
+* https://pypi.python.org/pypi/uncompyle6 : Python decompiler
+* https://pypi.python.org/pypi/decompyle3 : Python 3.7 and 3.8 decompiler
+* https://pypi.python.org/pypi/xdis : cross-platform disassembler
+
+
+.. _pygments:  http://pygments.org
+.. _pygments_style:  http://pygments.org/docs/styles/
+.. _howtoinstall: https://github.com/rocky/python3-trepan/wiki/How-to-Install
+.. _pydb:  http://bashdb.sf.net/pydb
+.. _pydbgr: https://pypi.python.org/pypi/pydbgr
+.. _trepan2: https://pypi.python.org/pypi/trepan2
+.. _trepan3: https://github.com/rocky/python3-trepan
+.. _trepanxpy: https://pypi.python.org/pypi/trepanxpy
+.. _other: https://repology.org/project/zshdb/versions
+.. _trepanning: https://rubygems.org/gems/trepanning
+.. _debuggers: https://metacpan.org/pod/Devel::Trepan
+.. _this: http://bashdb.sourceforge.net/pydb/features.html
+.. _Tutorial: http://python2-trepan.readthedocs.io/en/latest/entry-exit.html
+.. |downloads| image:: https://img.shields.io/pypi/dd/trepan3k.svg
+   :target: https://pypi.python.org/pypi/trepan3k/
+.. |TravisCI| image:: https://api.travis-ci.org/rocky/python3-trepan.svg
+   :target: https://travis-ci.org/rocky/python3-trepan
+.. |CircleCI| image:: https://circleci.com/gh/rocky/python3-trepan.svg?style=svg
+   :target: https://circleci.com/gh/rocky/python3-trepan
+.. _ipython-trepan: https://github.com/rocky/ipython-trepan
+.. |license| image:: https://img.shields.io/pypi/l/trepan.svg
+    :target: https://pypi.python.org/pypi/trepan3k
+    :alt: License
+.. _deparse:  https://python3-trepan.readthedocs.io/en/latest/commands/data/deparse.html
+.. _info_line:  https://python3-trepan.readthedocs.io/en/latest/commands/info/line.html
+.. _set_style:  https://python3-trepan.readthedocs.org/en/latest/commands/set/style.html
+.. _set_substitute:  https://python3-trepan.readthedocs.org/en/latest/commands/set/substitute.html
+.. _set_width:  https://python3-trepan.readthedocs.org/en/latest/commands/set/width.html
+.. _eval: https://python3-trepan.readthedocs.org/en/latest/commands/data/eval.html
+.. _step: https://python3-trepan.readthedocs.org/en/latest/commands/running/step.html
+.. _subst: https://python3-trepan.readthedocs.io/en/latest/commands/set/substitute.html
+.. _install: http://python3-trepan.readthedocs.org/en/latest/install.html
+.. |Supported Python Versions| image:: https://img.shields.io/pypi/pyversions/trepan3k.svg
+   :target: https://pypi.python.org/pypi/trepan3k/
+.. |Pypi Installs| image:: https://pepy.tech/badge/trepan3k
+.. |packagestatus| image:: https://repology.org/badge/vertical-allrepos/python:trepan3k.svg
+		 :target: https://repology.org/project/python:trepan3k/versions
+
```

### Comparing `trepan3k-1.2.8/README.rst` & `trepan3k-1.2.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-|TravisCI| |CircleCI| |Pypi Installs| |license| |Supported Python Versions|
+|CircleCI| |Pypi Installs| |license| |Supported Python Versions|
 
 |packagestatus|
 
 .. contents:: :local:
 
 Abstract
 ========
```

### Comparing `trepan3k-1.2.8/__pkginfo__.py` & `trepan3k-1.2.9/__pkginfo__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright (C) 2013, 2015-2018, 2020-2021 Rocky Bernstein <rocky@gnu.org>
+# Copyright (C) 2013, 2015-2018, 2020-2021, 2023 Rocky Bernstein
+# <rocky@gnu.org>
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
@@ -17,53 +18,56 @@
 # To the extent possible we make this file look more like a
 # configuration file rather than code like setup.py. I find putting
 # configuration stuff in the middle of a function call in setup.py,
 # which for example requires commas in between parameters, is a little
 # less elegant than having it here with reduced code, albeit there
 # still is some room for improvement.
 
+import os.path as osp
 import sys
 
 decompiler = "uncompyle6 >= 3.8.0"
 
 SYS_VERSION = sys.version_info[0:2]
 if SYS_VERSION <= (3, 2):
     pygments_version = "== 1.6"
 else:
     pygments_version = ">= 2.2.0"
     if (3, 7) <= SYS_VERSION < (3, 9):
-        decompiler = "decompyle3 >= 3.7.7"
+        decompiler = "decompyle3 >= 3.8.0"
 
 
 # Python-version | package  | last-version |
 # ------------------------------------------
 # 3.2            | pip      | 8.1.2        |
 # 3.2            | pygments | 1.6          |
 # 3.3            | pip      | 10.0.1       |
 # 3.4            | pip      | 19.1.1       |
 
 # Things that change more often go here.
-copyright = """Copyright (C) 2013, 2015-2021 Rocky Bernstein <rocky@gnu.org>."""
+copyright = """Copyright (C) 2013, 2015-2021, 2023 Rocky Bernstein <rocky@gnu.org>."""
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Software Development :: Debuggers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3.2",
     "Programming Language :: Python :: 3.3",
     "Programming Language :: Python :: 3.4",
-    "Programming Language :: Python :: 3.5 ",
-    "Programming Language :: Python :: 3.6 ",
-    "Programming Language :: Python :: 3.7 ",
-    "Programming Language :: Python :: 3.8 ",
-    "Programming Language :: Python :: 3.9 ",
+    "Programming Language :: Python :: 3.5",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 # The rest in alphabetic order
 author = "Rocky Bernstein"
 author_email = "rocky@gnu.org"
 
 entry_points = {
@@ -84,19 +88,17 @@
     "tracer >= 0.3.2",
     "term-background >= 1.0.1",
     decompiler,
 ]
 license = "GPL3"
 mailing_list = "python-debugger@googlegroups.com"
 modname = "trepan3k"
-py_modules = None
+py_modules = []
 short_desc = "GDB-like Python Debugger in the Trepan family"
 
-import os.path as osp
-
 
 def get_srcdir():
     filename = osp.normcase(osp.dirname(osp.abspath(__file__)))
     return osp.realpath(filename)
 
 
 def read(*rnames):
```

### Comparing `trepan3k-1.2.8/setup.cfg` & `trepan3k-1.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/setup.py` & `trepan3k-1.2.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 #!/usr/bin/env python3
 import sys
 
+from setuptools import find_packages, setup
+
 SYS_VERSION = sys.version_info[0:2]
 if not ((3, 1) <= SYS_VERSION <= (3, 10)):
     mess = "Python Versions 3.1 to 3.10 are supported only in this package."
     if (2, 4) <= SYS_VERSION <= (2, 7):
         mess += "\nFor your Python, version %s, See trepan2" % sys.version[0:3]
     elif SYS_VERSION < (2, 4):
         mess += "\nFor your Python, version %s, see pydb" % sys.version[0:3]
     print(mess)
     raise Exception(mess)
 
 # Get the package information used in setup().
 from __pkginfo__ import (
+    __version__,
     author,
     author_email,
     classifiers,
     entry_points,
     install_requires,
     license,
     long_description,
     modname,
     py_modules,
     short_desc,
-    __version__,
     web,
     zip_safe,
 )
 
 __import__("pkg_resources")
 
-from setuptools import setup, find_packages
-
 packages = find_packages()
 
 setup(
     author=author,
     author_email=author_email,
     classifiers=classifiers,
     data_files=[
```

### Comparing `trepan3k-1.2.8/test/data/macro-pypy.right` & `trepan3k-1.2.9/test/data/macro-pypy.right`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/data/macro.right` & `trepan3k-1.2.9/test/data/macro.right`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/data/step-38.right` & `trepan3k-1.2.9/test/data/step-38.right`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/data/step-pypy.right` & `trepan3k-1.2.9/test/data/step-pypy.right`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/example/gcd-dbgcall.py` & `trepan3k-1.2.9/test/example/gcd-dbgcall.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/example/gcd.py` & `trepan3k-1.2.9/test/example/gcd.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/example/hanoi.py` & `trepan3k-1.2.9/test/example/hanoi.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/example/tail.py` & `trepan3k-1.2.9/test/example/tail.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/case.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/case.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/commands.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/commands.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/config.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/config.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/core.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/core.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/ext/dtcompat.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/ext/dtcompat.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/failure.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/failure.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/importer.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/importer.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/inspector.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/inspector.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/loader.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/loader.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/__init__.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/allmodules.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/allmodules.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/attrib.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/attrib.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/base.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/base.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/builtin.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/builtin.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/capture.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/capture.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/collect.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/collect.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/cover.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/cover.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/debug.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/debug.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/deprecated.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/deprecated.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/doctests.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/doctests.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/errorclass.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/errorclass.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/failuredetail.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/failuredetail.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/isolate.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/isolate.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/logcapture.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/logcapture.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/manager.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/multiprocess.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/multiprocess.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/plugintest.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/plugintest.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/prof.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/prof.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/skip.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/skip.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/testid.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/testid.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/xunit.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/xunit.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/proxy.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/proxy.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/pyversion.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/pyversion.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/result.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/result.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/selector.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/selector.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/sphinx/pluginopts.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/sphinx/pluginopts.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/suite.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/suite.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/tools/nontrivial.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/tools/nontrivial.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/tools/trivial.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/tools/trivial.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/twistedtools.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/twistedtools.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/util.py` & `trepan3k-1.2.9/test/functional/.eggs/nose-1.3.7-py3.9.egg/nose/util.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/fn_helper.py` & `trepan3k-1.2.9/test/functional/fn_helper.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/stringarray.py` & `trepan3k-1.2.9/test/functional/stringarray.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/test-break.py` & `trepan3k-1.2.9/test/functional/test-break.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/test-finish.py` & `trepan3k-1.2.9/test/functional/test-finish.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/test-jump.py` & `trepan3k-1.2.9/test/functional/test-jump.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/test-next.py` & `trepan3k-1.2.9/test/functional/test-next.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/test-sig.py` & `trepan3k-1.2.9/test/functional/test-sig.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/test-skip.py` & `trepan3k-1.2.9/test/functional/test-skip.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/functional/test-step.py` & `trepan3k-1.2.9/test/functional/test-step.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/case.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/case.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/commands.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/commands.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/config.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/config.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/core.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/core.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/ext/dtcompat.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/ext/dtcompat.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/failure.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/failure.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/importer.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/importer.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/inspector.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/inspector.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/loader.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/loader.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/__init__.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/allmodules.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/allmodules.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/attrib.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/attrib.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/base.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/base.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/builtin.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/builtin.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/capture.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/capture.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/collect.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/collect.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/cover.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/cover.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/debug.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/debug.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/deprecated.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/deprecated.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/doctests.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/doctests.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/errorclass.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/errorclass.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/failuredetail.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/failuredetail.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/isolate.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/isolate.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/logcapture.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/logcapture.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/manager.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/multiprocess.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/multiprocess.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/plugintest.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/plugintest.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/prof.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/prof.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/skip.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/skip.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/testid.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/testid.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/xunit.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/plugins/xunit.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/proxy.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/proxy.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/pyversion.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/pyversion.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/result.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/result.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/selector.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/selector.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/sphinx/pluginopts.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/sphinx/pluginopts.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/suite.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/suite.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/tools/nontrivial.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/tools/nontrivial.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/tools/trivial.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/tools/trivial.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/twistedtools.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/twistedtools.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/util.py` & `trepan3k-1.2.9/test/integration/.eggs/nose-1.3.7-py3.9.egg/nose/util.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/helper.py` & `trepan3k-1.2.9/test/integration/helper.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/test-general.py` & `trepan3k-1.2.9/test/integration/test-general.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/test-highlight.py` & `trepan3k-1.2.9/test/integration/test-highlight.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/integration/test-noscript.py` & `trepan3k-1.2.9/test/integration/test-noscript.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-break.py` & `trepan3k-1.2.9/test/unit/test-break.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-brkpt.py` & `trepan3k-1.2.9/test/unit/test-brkpt.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-bytecode.py` & `trepan3k-1.2.9/test/unit/test-bytecode.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 #!/usr/bin/env python3
-'Unit test for trepan.bytecode'
-import inspect, unittest
+"Unit test for trepan.bytecode"
+import inspect
+import unittest
+
+from xdis import IS_PYPY, PYTHON_VERSION_TRIPLE
 
 from trepan.lib import bytecode as Mcode
-from xdis import IS_PYPY, PYTHON_VERSION
 
 
 class TestByteCode(unittest.TestCase):
-
     def test_contains_make_function(self):
         def sqr(x):
             return x * x
+
         frame = inspect.currentframe()
         co = frame.f_code
         lineno = frame.f_lineno
-        self.assertTrue(Mcode.stmt_contains_opcode(co, lineno-4,
-                                                   'MAKE_FUNCTION'))
-        self.assertFalse(Mcode.stmt_contains_opcode(co, lineno,
-                                                    'MAKE_FUNCTION'))
+        self.assertFalse(Mcode.stmt_contains_opcode(co, lineno, "MAKE_FUNCTION"))
         return
 
     def test_op_at_frame(self):
         frame = inspect.currentframe()
-        if IS_PYPY or PYTHON_VERSION >= 3.7:
-            call_opcode = 'CALL_METHOD'
+        if IS_PYPY or PYTHON_VERSION_TRIPLE >= (3, 7):
+            call_opcode = "CALL_METHOD"
         else:
-            call_opcode = 'CALL_FUNCTION'
+            call_opcode = "CALL_FUNCTION"
 
         self.assertEqual(call_opcode, Mcode.op_at_frame(frame))
         return
 
     def test_is_def_frame(self):
         # Not a "def" statement because frame is wrong spot
         frame = inspect.currentframe()
-        self.assertFalse(Mcode.is_def_stmt('foo(): pass', frame))
+        self.assertFalse(Mcode.is_def_stmt("foo(): pass", frame))
         return
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `trepan3k-1.2.8/test/unit/test-clifns.py` & `trepan3k-1.2.9/test/unit/test-clifns.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-cmd-alias.py` & `trepan3k-1.2.9/test/unit/test-cmd-alias.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-cmdbreak.py` & `trepan3k-1.2.9/test/unit/test-cmdbreak.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-cmdfns.py` & `trepan3k-1.2.9/test/unit/test-cmdfns.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-cmdproc.py` & `trepan3k-1.2.9/test/unit/test-cmdproc.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-completion.py` & `trepan3k-1.2.9/test/unit/test-completion.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-core.py` & `trepan3k-1.2.9/test/unit/test-core.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-disassemble.py` & `trepan3k-1.2.9/test/unit/test-disassemble.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-except.py` & `trepan3k-1.2.9/test/unit/test-except.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-fifo.py` & `trepan3k-1.2.9/test/unit/test-fifo.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-finish.py` & `trepan3k-1.2.9/test/unit/test-finish.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-help.py` & `trepan3k-1.2.9/test/unit/test-help.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-info-files.py` & `trepan3k-1.2.9/test/unit/test-info-files.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-inout-input.py` & `trepan3k-1.2.9/test/unit/test-inout-input.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-kill.py` & `trepan3k-1.2.9/test/unit/test-kill.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         """Test processor.command.kill.KillCommand.run()"""
         signal.signal(28, self.handle)
         d, cp = dbg_setup()
         command = Mkill.KillCommand(cp)
         result = command.run(['kill', 'wrong', 'number', 'of', 'args'])
         self.assertFalse(result)
         self.assertFalse(self.signal_caught)
-        if sys.platform != 'win32':
-            result = command.run(['kill', '28'])
-            self.assertFalse(result)
-            self.assertTrue(self.signal_caught)
+        # if sys.platform != 'win32':
+        #     result = command.run(['kill', '28'])
+        #     self.assertFalse(result)
+        #     self.assertTrue(self.signal_caught)
         return
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `trepan3k-1.2.8/test/unit/test-lib-complete.py` & `trepan3k-1.2.9/test/unit/test-lib-complete.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-lib-display.py` & `trepan3k-1.2.9/test/unit/test-lib-display.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-lib-eval.py` & `trepan3k-1.2.9/test/unit/test-lib-eval.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-lib-file.py` & `trepan3k-1.2.9/test/unit/test-lib-file.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-lib-format.py` & `trepan3k-1.2.9/test/unit/test-lib-format.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-lib-pp.py` & `trepan3k-1.2.9/test/unit/test-lib-pp.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-lib-printing.py` & `trepan3k-1.2.9/test/unit/test-lib-printing.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-lib-sig.py` & `trepan3k-1.2.9/test/unit/test-lib-sig.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from trepan.lib import sighandler as Msig
 
 
 class TestLibSigHandle(unittest.TestCase):
 
     def test_YN(self):
         for expect, b in (('Yes', True), ('No', False)):
-            self.assertEqual(expect, Msig.YN(b))
+            self.assertEqual(expect, Msig.yes_or_no(b))
             pass
         return
 
     def test_canonic_signame(self):
         for expect, name_num in (('SIGTERM',  '15'),
                                  ('SIGTERM', '-15'),
                                  ('SIGTERM', 'term'),
```

### Comparing `trepan3k-1.2.8/test/unit/test-lib-thread.py` & `trepan3k-1.2.9/test/unit/test-lib-thread.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-list.py` & `trepan3k-1.2.9/test/unit/test-list.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-misc.py` & `trepan3k-1.2.9/test/unit/test-misc.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-print.py` & `trepan3k-1.2.9/test/unit/test-print.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-processor.py` & `trepan3k-1.2.9/test/unit/test-processor.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-quit.py` & `trepan3k-1.2.9/test/unit/test-quit.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-run.py` & `trepan3k-1.2.9/test/unit/test-run.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-stack.py` & `trepan3k-1.2.9/test/unit/test-stack.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-step.py` & `trepan3k-1.2.9/test/unit/test-step.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-subcmd.py` & `trepan3k-1.2.9/test/unit/test-subcmd.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-tcp.py` & `trepan3k-1.2.9/test/unit/test-tcp.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/test/unit/test-user.py` & `trepan3k-1.2.9/test/unit/test-user.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/trepan/__init__.py` & `trepan3k-1.2.9/trepan/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#  Copyright (C) 2008-2009, 2013, 2015, 2021 Rocky Bernstein <rocky@gnu.org>
+#  Copyright (C) 2008-2009, 2013, 2015, 2021-2022 Rocky Bernstein <rocky@gnu.org>
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -160,15 +160,17 @@
   running debugger commands from a file (`source`) are different interfaces.
   This means, for example, that we are able to give better error reporting
   if a debugger command file has an error.
 * There is an experimental Python-friendly interface for front-ends
 * more testable. Much more unit and functional tests. More of _pydb_'s
   integration test will eventually be added.
 
-Copyright (C) 2008-2009, 2013-2016, 2021 Rocky Bernstein <rocky@gnu.org>
+Copyright (C) 2008-2009, 2013-2016, 2021-2022 Rocky Bernstein <rocky@gnu.org>
 
 .. |Downloads| image:: https://pypip.in/download/trepan/badge.svg
 .. |Build Status| image:: https://travis-ci.org/rocky/python3-trepan.svg
 """
 __docformat__ = "restructuredtext"
 
 from trepan.version import __version__
+
+__all__ = ["__version__"]
```

### Comparing `trepan3k-1.2.8/trepan/__main__.py` & `trepan3k-1.2.9/trepan/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: iso-8859-1 -*-
-#   Copyright (C) 2008-2010, 2013-2018, 2020-2021 Rocky Bernstein
+#   Copyright (C) 2008-2010, 2013-2018, 2020-2023 Rocky Bernstein
 #   <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
@@ -13,28 +13,32 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """The command-line interface to the debugger.
 """
-import os, pyficache, sys, tempfile
+import os
 import os.path as osp
+import sys
+import tempfile
+
+import pyficache
 
 package = "trepan"
 
 # Our local modules
 import trepan.client as Mclient
 import trepan.clifns as Mclifns
 import trepan.debugger as Mdebugger
 import trepan.exception as Mexcept
-import trepan.options as Moptions
 import trepan.interfaces.server as Mserver
 import trepan.lib.file as Mfile
 import trepan.misc as Mmisc
+import trepan.options as Moptions
 
 # The name of the debugger we are currently going by.
 __title__ = package
 
 from trepan.version import __version__
 
 
@@ -84,45 +88,53 @@
         mainpyfile = sys_argv[0]  # Get script filename.
         if not osp.isfile(mainpyfile):
             mainpyfile = Mclifns.whence_file(mainpyfile)
             is_readable = Mfile.readable(mainpyfile)
             if is_readable is None:
                 print(
                     "%s: Python script file '%s' does not exist"
-                    % (__title__, mainpyfile,)
+                    % (
+                        __title__,
+                        mainpyfile,
+                    )
                 )
                 sys.exit(1)
             elif not is_readable:
                 print(
-                    "%s: Can't read Python script file '%s'" % (__title__, mainpyfile,)
+                    "%s: Can't read Python script file '%s'"
+                    % (
+                        __title__,
+                        mainpyfile,
+                    )
                 )
                 sys.exit(1)
                 return
 
         if Mfile.is_compiled_py(mainpyfile):
             try:
-                from xdis import load_module, PYTHON_VERSION, IS_PYPY
+                from xdis import IS_PYPY, PYTHON_VERSION_TRIPLE, load_module
+                from xdis.version_info import version_tuple_to_str
 
                 (
                     python_version,
                     timestamp,
                     magic_int,
                     co,
                     is_pypy,
                     source_size,
                     sip_hash,
                 ) = load_module(mainpyfile, code_objects=None, fast_load=False)
                 if is_pypy != IS_PYPY:
                     print("Bytecode is pypy %s, but we are %s." % (is_pypy, IS_PYPY))
                     print("For a cross-version debugger, use trepan-xpy with x-python.")
                     sys.exit(2)
-                if python_version != PYTHON_VERSION:
+                if python_version[:2] != PYTHON_VERSION_TRIPLE[:2]:
                     print(
                         "Bytecode is for version %s but we are version %s."
-                        % (python_version, PYTHON_VERSION)
+                        % (python_version, version_tuple_to_str())
                     )
                     print("For a cross-version debugger, use trepan-xpy with x-python.")
                     sys.exit(2)
 
                 py_file = co.co_filename
                 if osp.isabs(py_file):
                     try_file = py_file
@@ -143,15 +155,15 @@
                     # Move onto the except branch
                     raise IOError(
                         "Python file name embedded in code %s not found" % try_file
                     )
             except IOError:
                 decompiler = "uncompyle6"
                 try:
-                    if 3.7 <= PYTHON_VERSION <= 3.8:
+                    if (3, 7) <= PYTHON_VERSION_TRIPLE <= (3, 8):
                         from uncompyle6 import decompile_file
                     else:
                         from decompyle3 import decompile_file
 
                         decompiler = "decompyle3"
                 except ImportError:
                     print(
@@ -181,15 +193,15 @@
 
                 fd.file.write = write_wrapper
 
                 # from io import StringIO
                 # linemap_io = StringIO()
                 try:
                     decompile_file(mainpyfile, fd.file, mapstream=fd)
-                except:
+                except Exception:
                     print(
                         "%s: error decompiling '%s'" % (__title__, mainpyfile),
                         file=sys.stderr,
                     )
                     sys.exit(1)
                     return
 
@@ -218,15 +230,18 @@
         # If mainpyfile is an optimized Python script try to find and
         # use non-optimized alternative.
         mainpyfile_noopt = pyficache.resolve_name_to_path(mainpyfile)
         if mainpyfile != mainpyfile_noopt and Mfile.readable(mainpyfile_noopt):
             print("%s: Compiled Python script given and we can't use that." % __title__)
             print(
                 "%s: Substituting non-compiled name: %s"
-                % (__title__, mainpyfile_noopt,)
+                % (
+                    __title__,
+                    mainpyfile_noopt,
+                )
             )
             mainpyfile = mainpyfile_noopt
             pass
 
         # Replace trepan's dir with script's dir in front of
         # module search path.
         sys.path[0] = dbg.main_dirname = osp.dirname(mainpyfile)
@@ -237,15 +252,14 @@
 
     # if not mainpyfile:
     #     print('For now, you need to specify a Python script name!')
     #     sys.exit(2)
     #     pass
 
     while True:
-
         # Run the debugged script over and over again until we get it
         # right.
 
         try:
             if dbg.program_sys_argv and mainpyfile:
                 normal_termination = dbg.run_script(mainpyfile)
                 if not normal_termination:
```

### Comparing `trepan3k-1.2.8/trepan/api.py` & `trepan3k-1.2.9/trepan/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2008-2009, 2013-2017, 2019-2021 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2008-2009, 2013-2017, 2019-2021, 2023 Rocky
+#   Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -31,20 +33,20 @@
 # But this a bit cumbersome and perhaps overkill for the 2 or so
 # functions below.  (It also doesn't work once we add the exception handling
 # we see below. So for now, we'll live with the code duplication.
 
 import sys
 
 from trepan import debugger as Mdebugger
-from trepan.post_mortem import post_mortem_excepthook, uncaught_exception
 from trepan.debugger import Trepan
+from trepan.post_mortem import post_mortem_excepthook, uncaught_exception
 
 
 def debugger_on_post_mortem():
-    """Call debugger on an exeception that terminates a program"""
+    """Call debugger on an exception that terminates a program"""
     sys.excepthook = post_mortem_excepthook
     return
 
 
 def run_eval(
     expression,
     debug_opts=None,
@@ -65,15 +67,15 @@
     """
 
     dbg = Trepan(opts=debug_opts)
     try:
         return dbg.run_eval(
             expression, start_opts=start_opts, globals_=globals_, locals_=locals_
         )
-    except:
+    except Exception:
         dbg.core.trace_hook_suspend = True
         if start_opts and "tb_fn" in start_opts:
             tb_fn = start_opts["tb_fn"]
         uncaught_exception(dbg, tb_fn)
     finally:
         dbg.core.trace_hook_suspend = False
     return
@@ -88,15 +90,15 @@
     When run_call() returns, it returns whatever the function call
     returned.  The debugger prompt appears as soon as the function is
     entered."""
 
     dbg = Trepan()
     try:
         return dbg.run_call(func, *args, **kwds)
-    except:
+    except Exception:
         uncaught_exception(dbg)
         pass
     return
 
 
 def run_exec(statement, debug_opts=None, start_opts=None, globals_=None, locals_=None):
 
@@ -115,101 +117,100 @@
     module __main__ is used."""
 
     dbg = Trepan(opts=debug_opts)
     try:
         return dbg.run_exec(
             statement, start_opts=start_opts, globals_=globals_, locals_=locals_
         )
-    except:
+    except Exception:
         uncaught_exception(dbg)
         pass
     return
 
 
 def debug(dbg_opts=None, start_opts=None, post_mortem=True, step_ignore=1, level=0):
     """
-Enter the debugger.
+    Enter the debugger.
 
-Parameters
-----------
+    Parameters
+    ----------
 
-level : how many stack frames go back. Usually it will be
-the default 0. But sometimes though there may be calls in setup to the debugger
-that you may want to skip.
-
-step_ignore : how many line events to ignore after the
-debug() call. 0 means don't even wait for the debug() call to finish.
-
-param dbg_opts : is an optional "options" dictionary that gets fed
-trepan.Debugger(); `start_opts' are the optional "options"
-dictionary that gets fed to trepan.Debugger.core.start().
-
-Use like this:
-
-.. code-block:: python
-
-    ... # Possibly some Python code
-    import trepan.api # Needed only once
-    ... # Possibly some more Python code
-    trepan.api.debug() # You can wrap inside conditional logic too
-    pass  # Stop will be here.
-    # Below is code you want to use the debugger to do things.
-    ....  # more Python code
-    # If you get to a place in the program where you aren't going
-    # want to debug any more, but want to remove debugger trace overhead:
-    trepan.api.stop()
-
-Parameter "level" specifies how many stack frames go back. Usually it will be
-the default 0. But sometimes though there may be calls in setup to the debugger
-that you may want to skip.
-
-Parameter "step_ignore" specifies how many line events to ignore after the
-debug() call. 0 means don't even wait for the debug() call to finish.
-
-In situations where you want an immediate stop in the "debug" call
-rather than the statement following it ("pass" above), add parameter
-step_ignore=0 to debug() like this::
-
-    import trepan.api  # Needed only once
-    # ... as before
-    trepan.api.debug(step_ignore=0)
-    # ... as before
-
-Module variable _debugger_obj_ from module trepan.debugger is used as
-the debugger instance variable; it can be subsequently used to change
-settings or alter behavior. It should be of type Debugger (found in
-module trepan). If not, it will get changed to that type::
-
-   $ python
-   >>> from trepan.debugger import debugger_obj
-   >>> type(debugger_obj)
-   <type 'NoneType'>
-   >>> import trepan.api
-   >>> trepan.api.debug()
-   ...
-   (Trepan) c
-   >>> from trepan.debugger import debugger_obj
-   >>> debugger_obj
-   <trepan.debugger.Debugger instance at 0x7fbcacd514d0>
-   >>>
-
-If however you want your own separate debugger instance, you can
-create it from the debugger _class Debugger()_ from module
-trepan.debugger::
-
-  $ python
-  >>> from trepan.debugger import Debugger
-  >>> dbgr = Debugger()  # Add options as desired
-  >>> dbgr
-  <trepan.debugger.Debugger instance at 0x2e25320>
-
-`dbg_opts' is an optional "options" dictionary that gets fed
-trepan.Debugger(); `start_opts' are the optional "options"
-dictionary that gets fed to trepan.Debugger.core.start().
-"""
+    level : how many stack frames go back. Usually it will be
+    the default 0. But sometimes though there may be calls in setup to the debugger
+    that you may want to skip.
+
+    step_ignore : how many line events to ignore after the
+    debug() call. 0 means don't even wait for the debug() call to finish.
+
+    param dbg_opts : is an optional "options" dictionary that gets fed
+    trepan.Debugger(); `start_opts' are the optional "options"
+    dictionary that gets fed to trepan.Debugger.core.start().
+
+    Use like this:
+
+    .. code-block:: python
+
+        ... # Possibly some Python code
+        import trepan.api # Needed only once
+        ... # Possibly some more Python code
+        trepan.api.debug() # You can wrap inside conditional logic too
+        pass  # Stop will be here.
+        # Below is code you want to use the debugger to do things.
+        ....  # more Python code
+        # If you get to a place in the program where you aren't going
+        # want to debug any more, but want to remove debugger trace overhead:
+        trepan.api.stop()
+
+    Parameter "level" specifies how many stack frames go back. Usually it will be
+    the default 0. But sometimes though there may be calls in setup to the debugger
+    that you may want to skip.
+
+    Parameter "step_ignore" specifies how many line events to ignore after the
+    debug() call. 0 means don't even wait for the debug() call to finish.
+
+    In situations where you want an immediate stop in the "debug" call
+    rather than the statement following it ("pass" above), add parameter
+    step_ignore=0 to debug() like this::
+
+        import trepan.api  # Needed only once
+        # ... as before
+        trepan.api.debug(step_ignore=0)
+        # ... as before
+
+    Module variable _debugger_obj_ from module trepan.debugger is used as
+    the debugger instance variable; it can be subsequently used to change
+    settings or alter behavior. It should be of type Debugger (found in
+    module trepan). If not, it will get changed to that type::
+
+       $ python
+       >>> from trepan.debugger import debugger_obj
+       >>> type(debugger_obj)
+       <type 'NoneType'>
+       >>> import trepan.api
+       >>> trepan.api.debug()
+       ...
+       (Trepan) c
+       >>> from trepan.debugger import debugger_obj
+       >>> debugger_obj
+       <trepan.debugger.Debugger instance at 0x7fbcacd514d0>
+       >>>
+
+    If however you want your own separate debugger instance, you can
+    create it from the debugger _class Debugger()_ from module
+    trepan.debugger::
+
+      $ python
+      >>> from trepan.debugger import Debugger
+      >>> dbgr = Debugger()  # Add options as desired
+      >>> dbgr
+      <trepan.debugger.Debugger instance at 0x2e25320>
+
+    `dbg_opts' is an optional "options" dictionary that gets fed
+    trepan.Debugger(); `start_opts' are the optional "options"
+    dictionary that gets fed to trepan.Debugger.core.start()."""
     if not isinstance(Mdebugger.debugger_obj, Mdebugger.Trepan):
         Mdebugger.debugger_obj = Mdebugger.Trepan(dbg_opts)
         Mdebugger.debugger_obj.core.add_ignore(debug, stop)
         pass
     core = Mdebugger.debugger_obj.core
     frame = sys._getframe(0 + level)
     core.set_next(frame)
```

### Comparing `trepan3k-1.2.8/trepan/bwcli.py` & `trepan3k-1.2.9/trepan/bwcli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: iso-8859-1 -*-
-#   Copyright (C) 2013, 2015, 2020 Rocky Bernstein <rocky@gnu.org>
+#   Copyright (C) 2013, 2015, 2020, 2023 Rocky Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -12,39 +12,43 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """ The hairy command-line interface to the debugger.
 """
-import os, os.path as osp, sys
-
+import os.path as osp
+import sys
 from optparse import OptionParser
 
-from pyficache import resolve_name_to_path
+import pyficache
 
 # Our local modules
-from trepan import clifns as Mclifns
-from trepan import debugger as Mdebugger, exception as Mexcept, misc as Mmisc
-from trepan.lib.file import readable
+from trepan import (
+    clifns as Mclifns,
+    debugger as Mdebugger,
+    exception as Mexcept,
+    misc as Mmisc,
+)
 from trepan.interfaces.bullwinkle import BWInterface
+from trepan.lib.file import readable
 
 # The name of the debugger we are currently going by.
 __title__ = "trepan"
 
-# VERSION.py sets variable VERSION.
-from trepan.VERSION import VERSION as __version__
+# version.py sets variable __version__
+from trepan.version import __version__
 
 
 def process_options(debugger_name, pkg_version, sys_argv, option_list=None):
     """Handle debugger options. Set `option_list' if you are writing
     another main program and want to extend the existing set of debugger
     options.
 
-    The options dicionary from opt_parser is return. sys_argv is
+    The options dictionary from opt_parser is return. sys_argv is
     also updated."""
     usage_str = """%prog [debugger-options] [python-script [script-options...]]
 
        Runs the extended python debugger"""
 
     # serverChoices = ('TCP','FIFO', None)
 
@@ -82,15 +86,15 @@
     (opts, sys.argv) = optparser.parse_args()
     dbg_opts = {}
 
     return opts, dbg_opts, sys.argv
 
 
 def _postprocess_options(dbg, opts):
-    """ Handle options (`opts') that feed into the debugger (`dbg')"""
+    """Handle options (`opts') that feed into the debugger (`dbg')"""
     # Set dbg.settings['printset']
     print_events = []
     if opts.fntrace:
         print_events = ["c_call", "c_return", "call", "return"]
     # if opts.linetrace: print_events += ['line']
     if len(print_events):
         dbg.settings["printset"] = frozenset(print_events)
@@ -137,32 +141,42 @@
         mainpyfile = sys_argv[0]  # Get script filename.
         if not osp.isfile(mainpyfile):
             mainpyfile = Mclifns.whence_file(mainpyfile)
             is_readable = readable(mainpyfile)
             if is_readable is None:
                 print(
                     "%s: Python script file '%s' does not exist"
-                    % (__title__, mainpyfile,)
+                    % (
+                        __title__,
+                        mainpyfile,
+                    )
                 )
                 sys.exit(1)
             elif not is_readable:
                 print(
-                    "%s: Can't read Python script file '%s'" % (__title__, mainpyfile,)
+                    "%s: Can't read Python script file '%s'"
+                    % (
+                        __title__,
+                        mainpyfile,
+                    )
                 )
                 sys.exit(1)
                 return
 
         # If mainpyfile is an optimized Python script try to find and
         # use non-optimized alternative.
         mainpyfile_noopt = pyficache.resolve_name_to_file(mainpyfile)
         if mainpyfile != mainpyfile_noopt and readable(mainpyfile_noopt):
             print("%s: Compiled Python script given and we can't use that." % __title__)
             print(
                 "%s: Substituting non-compiled name: %s"
-                % (__title__, mainpyfile_noopt,)
+                % (
+                    __title__,
+                    mainpyfile_noopt,
+                )
             )
             mainpyfile = mainpyfile_noopt
             pass
 
         # Replace trepan's dir with script's dir in front of
         # module search path.
         sys.path[0] = dbg.main_dirname = osp.dirname(mainpyfile)
```

### Comparing `trepan3k-1.2.8/trepan/bwprocessor/__init__.py` & `trepan3k-1.2.9/trepan/bwprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/trepan/bwprocessor/command/__init__.py` & `trepan3k-1.2.9/trepan/bwprocessor/command/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,38 @@
+#  Copyright (C) 2008, 2009, 2013 Rocky Bernstein <rocky@gnu.org>
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
-# """ Copyright (C) 2008, 2009, 2013 Rocky Bernstein <rocky@gnu.org> """
-__import__('pkg_resources').declare_namespace(__name__)
+import glob
+import os
 
-import glob, os
+__import__("pkg_resources").declare_namespace(__name__)
 
 # FIXME: Is it really helpful to "privatize" variable names below?
 # The below names are not part of the standard pre-defined names like
 # __name__ or __file__ are.
 
 # Get the name of our directory.
 __command_dir__ = os.path.dirname(__file__)
 
 # A glob pattern that will get all *.py files but not __init__.py
-__py_files__    = glob.glob(os.path.join(__command_dir__, '[a-z]*.py'))
+__py_files__ = glob.glob(os.path.join(__command_dir__, "[a-z]*.py"))
 
 # Take the basename of the filename and drop off '.py'. That minus the
-# files in exclude_files and tha becomes the list of modules that
+# files in exclude_files and that becomes the list of modules that
 # commands.py will use to import
-exclude_files = ['mock.py']
-__modules__ = [ os.path.basename(filename[0:-3]) for
-                filename in __py_files__
-                if os.path.basename(filename) not in exclude_files]
-__all__ =  __modules__  + exclude_files
+exclude_files = ["mock.py"]
+__modules__ = [
+    os.path.basename(filename[0:-3])
+    for filename in __py_files__
+    if os.path.basename(filename) not in exclude_files
+]
+__all__ = __modules__ + exclude_files
```

### Comparing `trepan3k-1.2.8/trepan/bwprocessor/command/base_cmd.py` & `trepan3k-1.2.9/trepan/bwprocessor/command/base_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#  Copyright (C) 2009-2010, 2012-2013, 2015 Rocky Bernstein
+#  Copyright (C) 2009-2010, 2012-2013, 2015, 2013 Rocky Bernstein
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
@@ -16,85 +16,87 @@
 """A base class for debugger commands.
 
 This file is the one module in this directory that isn't a real command
 and commands.py needs to take care to avoid instantiating this class
 and storing it as a list of known debugger commands.
 """
 
-NotImplementedMessage = "This method must be overriden in a subclass"
+NotImplementedMessage = "This method must be overridden in a subclass"
 
-__all__ = ['DebuggerCommand']
+__all__ = ["DebuggerCommand"]
 
 
 class DebuggerCommand:
     """Base Class for Debugger commands. We pull in some helper
     functions for command from module cmdfns."""
 
-    category = 'misc'
+    category = "misc"
 
     def __init__(self, proc):
         """proc contains the command processor object that this
         command is invoked through.  A debugger field gives access to
         the stack frame and I/O."""
         self.proc = proc
 
         # Convenience class access. We don't expect that either core
         # or debugger will change over the course of the program
         # execution like errmsg(), msg(), and msg_nocr() might. (See
         # the note below on these latter 3 methods.)
         #
-        self.core     = proc.core
+        self.core = proc.core
         self.debugger = proc.debugger
         self.settings = self.debugger.settings
         return
 
     aliases = ()
-    name    = 'YourCommandName'
+    name = "YourCommandName"
 
     # Note for errmsg, msg, and msg_nocr we don't want to simply make
     # an assignment of method names like self.msg = self.debugger.intf.msg,
     # because we want to allow the interface (intf) to change
     # dynamically. That is, the value of self.debugger may change
-    # in the course of the program and if we made such an method assignemnt
+    # in the course of the program and if we made such an method assignment
     # we wouldn't pick up that change in our self.msg
     def errmsg(self, msg, opts={}):
-        """ Convenience short-hand for self.debugger.intf.errmsg """
+        """Convenience short-hand for self.debugger.intf.errmsg"""
         try:
-            return(self.debugger.intf[-1].errmsg(msg))
+            return self.debugger.intf[-1].errmsg(msg)
         except EOFError:
             # FIXME: what do we do here?
             pass
         return None
 
     def msg(self, msg, opts={}):
-        """ Convenience short-hand for self.debugger.intf.msg """
+        """Convenience short-hand for self.debugger.intf.msg"""
         try:
-            return(self.debugger.intf[-1].msg(msg))
+            return self.debugger.intf[-1].msg(msg)
         except EOFError:
             # FIXME: what do we do here?
             pass
         return None
 
     def msg_nocr(self, msg, opts={}):
-        """ Convenience short-hand for self.debugger.intf.msg_nocr """
+        """Convenience short-hand for self.debugger.intf.msg_nocr"""
         try:
-            return(self.debugger.intf[-1].msg_nocr(msg))
+            return self.debugger.intf[-1].msg_nocr(msg)
         except EOFError:
             # FIXME: what do we do here?
             pass
         return None
 
     def run(self, args):
-        """ The method that implements the debugger command.
+        """The method that implements the debugger command.
         Help on the command comes from the docstring of this method.
         """
         raise NotImplementedError(NotImplementedMessage)
 
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.bwprocessor.command import mock
+
     d, cp = mock.dbg_setup()
     dd = DebuggerCommand(cp)
     dd.msg("hi")
     dd.errmsg("Don't do that")
     pass
```

### Comparing `trepan3k-1.2.8/trepan/bwprocessor/command/mock.py` & `trepan3k-1.2.9/trepan/bwprocessor/command/mock.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,130 +11,142 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program; if not, write to the Free Software
 #    Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 #    02110-1301 USA.
-''' Not a command. A stub class used by a command in its 'main' for
-demonstrating how the command works.'''
+""" Not a command. A stub class used by a command in its 'main' for
+demonstrating how the command works."""
 
-import os, sys
+import sys
 
 from trepan.lib import breakpoint, default
 
 
 class MockIO:
-    def readline(self, prompt='', add_to_history=False):
+    def readline(self, prompt="", add_to_history=False):
         print(prompt)
-        return 'quit'
+        return "quit"
+
     pass
 
 
 class MockUserInterface:
     def __init__(self):
         self.io = MockIO()
         return
 
     def confirm(self, msg, default):
-        print('** %s' % msg)
+        print("** %s" % msg)
         # Ignore the default.
         return True
 
     def errmsg(self, msg):
-        print('** %s' % msg)
+        print("** %s" % msg)
         return
 
     def finalize(self, last_wishes=None):
         return
 
     def msg(self, msg):
         print(msg)
         return
 
     def msg_nocr(self, msg):
         sys.stdout.write(msg)
         return
+
     pass
 
+
 class MockProcessor:
     def __init__(self, core):
-        self.core         = core
-        self.debugger     = core.debugger
+        self.core = core
+        self.debugger = core.debugger
         self.continue_running = False
-        self.curframe     = None
-        self.event2short  = {}
-        self.frame        = None
-        self.intf         = core.debugger.intf
+        self.curframe = None
+        self.event2short = {}
+        self.frame = None
+        self.intf = core.debugger.intf
         self.last_command = None
-        self.stack        = []
+        self.stack = []
         return
 
-    def get_int(self, arg, min_value=0, default=1, cmdname=None,
-                    at_most=None):
+    def get_int(self, arg, min_value=0, default=1, cmdname=None, at_most=None):
         return None
 
     def undefined_cmd(self, cmd):
         self.intf[-1].errmsg('Undefined mock command: "%s' % cmd)
         return
+
     pass
 
+
 # External Egg packages
 import tracefilter
 
+
 class MockDebuggerCore:
     def __init__(self, debugger):
-        self.debugger       = debugger
-        self.execution_status = 'Pre-execution'
-        self.filename_cache  = {}
-        self.ignore_filter  = tracefilter.TraceFilter([])
-        self.bpmgr          = breakpoint.BreakpointManager()
-        self.processor      = MockProcessor(self)
-        self.step_ignore    = -1
-        self.stop_frame     = None
-        self.last_lineno    = None
-        self.last_filename  = None
+        self.debugger = debugger
+        self.execution_status = "Pre-execution"
+        self.filename_cache = {}
+        self.ignore_filter = tracefilter.TraceFilter([])
+        self.bpmgr = breakpoint.BreakpointManager()
+        self.processor = MockProcessor(self)
+        self.step_ignore = -1
+        self.stop_frame = None
+        self.last_lineno = None
+        self.last_filename = None
         self.different_line = None
         return
 
     def set_next(self, frame, step_events=None):
         pass
 
-    def stop(self): pass
+    def stop(self):
+        pass
 
     def canonic(self, filename):
         return filename
 
     def canonic_filename(self, frame):
         return frame.f_code.co_filename
 
     def filename(self, name):
         return name
 
     def is_running(self):
-        return 'Running' == self.execution_status
+        return "Running" == self.execution_status
 
     def get_file_breaks(self, filename):
         return []
+
     pass
 
 
 class MockDebugger:
     def __init__(self):
-        self.intf             = [MockUserInterface()]
-        self.core             = MockDebuggerCore(self)
-        self.settings         = default.DEBUGGER_SETTINGS
-        self.orig_sys_argv    = None
+        self.intf = [MockUserInterface()]
+        self.core = MockDebuggerCore(self)
+        self.settings = default.DEBUGGER_SETTINGS
+        self.orig_sys_argv = None
         self.program_sys_argv = []
         return
 
-    def stop(self): pass
+    def stop(self):
+        pass
+
+    def restart_argv(self):
+        return []
 
-    def restart_argv(self): return []
     pass
 
 
-def dbg_setup(d = None):
-    if d is None: d = MockDebugger()
+def dbg_setup(d=None):
+    if d is None:
+        d = MockDebugger()
     from trepan.bwprocessor import main as bwproc
+
     cp = bwproc.BWProcessor(d.core)
     return d, cp
```

### Comparing `trepan3k-1.2.8/trepan/bwprocessor/command/quit.py` & `trepan3k-1.2.9/trepan/bwprocessor/command/quit.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,81 +7,84 @@
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import os, threading
+import os
+import threading
+
+from trepan import exception as Mexcept
 
 # Our local modules
 from trepan.bwprocessor.command import base_cmd as Mbase_cmd
-from trepan import exception as Mexcept
 
 
 class QuitCommand(Mbase_cmd.DebuggerCommand):
     """Gently exit the debugger and debugged program.
 
-**Input Fields:**
+    **Input Fields:**
 
-   { command     => 'quit',
-   }
+       { command     => 'quit',
+       }
 
-The program being debugged is exited raising a *DebuggerQuit* exception.
+    The program being debugged is exited raising a *DebuggerQuit* exception.
 
-**Output Fields: **
+    **Output Fields: **
 
-   { name      => 'status',
-     event     => 'terminated',
-     [errmsg   => <error-message-array>]
-     [msg      => <message-text array>]
-  }
-"""
+       { name      => 'status',
+         event     => 'terminated',
+         [errmsg   => <error-message-array>]
+         [msg      => <message-text array>]
+      }"""
 
-    name          = os.path.basename(__file__).split('.')[0]
-    need_stack    = False
+    name = os.path.basename(__file__).split(".")[0]
+    need_stack = False
 
     def nothread_quit(self, arg):
-        """ quit command when there's just one thread. """
+        """quit command when there's just one thread."""
 
         self.debugger.core.stop()
-        self.debugger.core.execution_status = 'Quit command'
-        self.proc.response['event'] = 'terminated'
-        self.proc.response['name']  = 'status'
+        self.debugger.core.execution_status = "Quit command"
+        self.proc.response["event"] = "terminated"
+        self.proc.response["name"] = "status"
         self.proc.intf[-1].msg(self.proc.response)
         raise Mexcept.DebuggerQuit
 
     def threaded_quit(self, arg):
-        """ quit command when several threads are involved. """
+        """quit command when several threads are involved."""
         self.msg("Quit for threading not fully done yet. Try 'kill'.")
         return False
 
     def run(self, cmd_hash):
         threading_list = threading.enumerate()
-        if (len(threading_list) == 1 and
-            threading_list[0].getName() == 'MainThread'):
+        if len(threading_list) == 1 and threading_list[0].getName() == "MainThread":
             # We just have a main thread so that's safe to quit
             return self.nothread_quit(cmd_hash)
         else:
             return self.threaded_quit(cmd_hash)
         pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.bwprocessor.command import mock
+
     d, cp = mock.dbg_setup()
     command = QuitCommand(cp)
     try:
-        command.run(['quit'])
+        command.run(["quit"])
     except Mexcept.DebuggerQuit:
         print("A got 'quit' a exception. Ok, be that way - I'm going home.")
         pass
 
     class MyThread(threading.Thread):
         def run(self):
-            command.run(['quit'])
+            command.run(["quit"])
             return
+
         pass
 
     t = MyThread()
     t.start()
     t.join()
     pass
```

### Comparing `trepan3k-1.2.8/trepan/bwprocessor/command/step.py` & `trepan3k-1.2.9/trepan/bwprocessor/command/step.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,53 +17,54 @@
 
 # Our local modules
 from trepan.bwprocessor.command import base_cmd as Mbase_cmd
 
 
 class StepCommand(Mbase_cmd.DebuggerCommand):
     """
-step statements
+    step statements
 
-**Input Fields:**
+    **Input Fields:**
 
-   { command  => 'step',
-     [count   => <integer>],
-   }
+       { command  => 'step',
+         [count   => <integer>],
+       }
 
-If *count* is given, that many statements will be stepped. If it
-is not given, 1 is used, i.e. stop at the next statement.
+    If *count* is given, that many statements will be stepped. If it
+    is not given, 1 is used, i.e. stop at the next statement.
 
-**Output Fields:**
+    **Output Fields:**
 
-   { name     => 'step',
-     count    => <integer>,
-     [errmsg  => <error-message-array>]
-     [msg     => <message-text array>]
-   }
-"""
+       { name     => 'step',
+         count    => <integer>,
+         [errmsg  => <error-message-array>]
+         [msg     => <message-text array>]
+       }"""
 
-    name          = os.path.basename(__file__).split('.')[0]
-    need_stack    = True
+    name = os.path.basename(__file__).split(".")[0]
+    need_stack = True
 
     def run(self, cmd_hash):
-        if 'step_count' in cmd_hash:
-            step_count = cmd_hash['step_count'] - 1
+        if "step_count" in cmd_hash:
+            step_count = cmd_hash["step_count"] - 1
         else:
             step_count = 0
             pass
         self.proc.debugger.core.step_ignore = 0
-        self.core.stop_level       = None
-        self.core.last_frame       = None
-        self.core.stop_on_finish   = False
+        self.core.stop_level = None
+        self.core.last_frame = None
+        self.core.stop_on_finish = False
         self.proc.continue_running = True  # Break out of command read loop
-        self.proc.response['step_count'] = step_count + 1
+        self.proc.response["step_count"] = step_count + 1
         return True
+
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     # from mock import MockDebugger
     # d = MockDebugger()
     # cmd = StepCommand(d.core.processor)
     # for c in (['s', '5'],
     #           ['step', '1+2'],
     #           ['s', 'foo']):
     #     d.core.step_ignore = 0
```

### Comparing `trepan3k-1.2.8/trepan/bwprocessor/location.py` & `trepan3k-1.2.9/trepan/bwprocessor/location.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2015 Rocky Bernstein <rocky@gnu.org>
-''' Location routines'''
+#   Copyright (C) 2015, 2023 Rocky Bernstein <rocky@gnu.org>
+""" Location routines"""
+
+import linecache
+import tempfile
+
+import pyficache
 
-import pyficache, linecache, tempfile
 from trepan.lib import stack as Mstack
 
 
 def format_location(proc_obj):
     """Show where we are. GUI's and front-end interfaces often
     use this to update displays. So it is helpful to make sure
     we give at least some place that's located in a file.
@@ -25,102 +29,109 @@
     while i_stack >= 0:
         frame_lineno = proc_obj.stack[i_stack]
         i_stack -= 1
         frame, lineno = frame_lineno
 
         filename = Mstack.frame2file(core_obj, frame)
 
-        location['filename'] = filename
-        location['fn_name']  = frame.f_code.co_name
-        location['lineno']   = lineno
+        location["filename"] = filename
+        location["fn_name"] = frame.f_code.co_name
+        location["lineno"] = lineno
 
-        if '<string>' == filename and dbgr_obj.eval_string:
+        if "<string>" == filename and dbgr_obj.eval_string:
             filename = pyficache.unmap_file(filename)
-            if '<string>' == filename:
-                fd = tempfile.NamedTemporaryFile(suffix='.py',
-                                                 prefix='eval_string',
-                                                 delete=False)
-                fd.write(bytes(dbgr_obj.eval_string, 'UTF-8'))
+            if "<string>" == filename:
+                fd = tempfile.NamedTemporaryFile(
+                    suffix=".py", prefix="eval_string", delete=False
+                )
+                fd.write(bytes(dbgr_obj.eval_string, "UTF-8"))
                 fd.close()
-                pyficache.remap_file(fd.name, '<string>')
+                pyficache.remap_file(fd.name, "<string>")
                 filename = fd.name
                 pass
             pass
 
-        opts = {
-            'reload_on_change' : proc_obj.settings('reload'),
-            'output'           : 'plain'
-            }
+        opts = {"reload_on_change": proc_obj.settings("reload"), "output": "plain"}
         line = pyficache.getline(filename, lineno, opts)
         if not line:
-            line = linecache.getline(filename, lineno,
-                                     proc_obj.curframe.f_globals)
+            line = linecache.getline(filename, lineno, proc_obj.curframe.f_globals)
             pass
 
         if line and len(line.strip()) != 0:
-            location['text'] = line
+            location["text"] = line
             pass
-        if '<string>' != filename: break
+        if "<string>" != filename:
+            break
         pass
 
     return location
 
+
 def print_location(proc_obj, event=None):
     response = proc_obj.response
-    response['name'] = 'status'
-    response['location'] = format_location(proc_obj)
+    response["name"] = "status"
+    response["location"] = format_location(proc_obj)
     if event:
-        response['event'] = event
-        if event in ['return', 'exception']:
+        response["event"] = event
+        if event in ["return", "exception"]:
             val = proc_obj._saferepr(proc_obj.event_arg)
-            event['arg'] = val
+            event["arg"] = val
             pass
         pass
     proc_obj.intf[-1].msg(response)
     return
 
 
 # Demo it
-if __name__=='__main__':
+if __name__ == "__main__":
+
     class MockDebugger:
         def __init__(self):
             self.eval_string = None
+
         pass
 
     class MockProcessor:
         def __init__(self, core_obj):
             self.curindex = 0
             self.stack = []
             self.core = core_obj
             self.debugger = MockDebugger()
-            self.opts = {'highlight': 'plain', 'reload': False}
+            self.opts = {"highlight": "plain", "reload": False}
             pass
 
         def settings(self, key):
             return self.opts[key]
+
         pass
 
     class MockCore:
-        def filename(self, fn): return fn
+        def filename(self, fn):
+            return fn
+
+        def canonic_filename(self, frame):
+            return frame.f_code.co_filename
 
-        def canonic_filename(self, frame): return frame.f_code.co_filename
         pass
 
     core = MockCore()
     cmdproc = MockProcessor(core)
 
     import sys
+
     cmdproc.curframe = cmdproc.frame = sys._getframe()
     cmdproc.stack.append((sys._getframe(), 10))
 
     import pprint
+
     pp = pprint.PrettyPrinter()
     pp.pprint(format_location(cmdproc))
 
     def test(cmdproc, pp):
         cmdproc.stack[0:0] = [(sys._getframe(1), 1)]
         pp.pprint(format_location(cmdproc))
         pass
-    eval('test(cmdproc, pp)')
-    cmdproc.debugger.eval_string = 'Fooled you!'
-    eval('test(cmdproc, pp)')
+
+    eval("test(cmdproc, pp)")
+    cmdproc.debugger.eval_string = "Fooled you!"
+    eval("test(cmdproc, pp)")
     pass
```

### Comparing `trepan3k-1.2.8/trepan/bwprocessor/main.py` & `trepan3k-1.2.9/trepan/bwprocessor/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2008-2010, 2013-2016 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2008-2010, 2013-2016, 2023 Rocky Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import inspect, linecache, sys, traceback
-import pyficache
+import inspect
+import linecache
+import sys
+import traceback
 from reprlib import Repr
 
-from trepan import vprocessor as Mprocessor
-from trepan import exception as Mexcept, misc as Mmisc
-from trepan.lib import bytecode as Mbytecode, display as Mdisplay
-from trepan.lib import thred as Mthread
+import pyficache
+
+from trepan import exception as Mexcept, misc as Mmisc, vprocessor as Mprocessor
 from trepan.bwprocessor import location as Mlocation, msg as Mmsg
+from trepan.lib import bytecode as Mbytecode, display as Mdisplay, thred as Mthread
 
 
 def get_stack(f, t, botframe, proc_obj=None):
     """Return a stack of frames which the debugger will use for in
     showing backtraces and in frame switching. As such various frame
     that are really around may be excluded unless we are debugging the
     sebugger. Also we will add traceback frame on top if that
     exists."""
     exclude_frame = lambda f: False
     if proc_obj:
         settings = proc_obj.debugger.settings
-        if not settings['dbg_trepan']:
-            exclude_frame = lambda f: \
-                proc_obj.core.ignore_filter.is_included(f)
+        if not settings["dbg_trepan"]:
+            exclude_frame = lambda f: proc_obj.core.ignore_filter.is_included(f)
             pass
         pass
     stack = []
     if t and t.tb_frame is f:
         t = t.tb_next
     while f is not None:
-        if exclude_frame(f): break  # See commented alternative below
+        if exclude_frame(f):
+            break  # See commented alternative below
         stack.append((f, f.f_lineno))
         # bdb has:
         # if f is botframe: break
         f = f.f_back
         pass
     stack.reverse()
     i = max(0, len(stack) - 1)
@@ -56,89 +59,91 @@
         pass
     return stack, i
 
 
 def run_hooks(obj, hooks, *args):
     """Run each function in `hooks' with args"""
     for hook in hooks:
-        if hook(obj, *args): return True
+        if hook(obj, *args):
+            return True
         pass
     return False
 
 
 def resolve_name(obj, command_name):
     if command_name not in obj.commands:
         return None
     return command_name
 
+
 # Default settings for command processor method call
 DEFAULT_PROC_OPTS = {
     # A list of debugger initialization files to read on first command
     # loop entry.  Often this something like [~/.trepanrc] which the
     # front-end sets.
-    'initfile_list' : []
+    "initfile_list": []
 }
 
 
 class BWProcessor(Mprocessor.Processor):
-
     def __init__(self, core_obj, opts=None):
         Mprocessor.Processor.__init__(self, core_obj)
 
-        self.response = {'errs': [], 'msg': []}
-        self.continue_running = False   # True if we should leave command loop
+        self.response = {"errs": [], "msg": []}
+        self.continue_running = False  # True if we should leave command loop
 
-        self.cmd_instances    = self._populate_commands()
+        self.cmd_instances = self._populate_commands()
 
         # command name before alias or macro resolution
-        self.cmd_name         = ''
+        self.cmd_name = ""
 
         # Current command getting run
-        self.current_command  = ''
+        self.current_command = ""
 
-        self.debug_nest       = 1
-        self.display_mgr      = Mdisplay.DisplayMgr()
-        self.intf             = core_obj.debugger.intf
-        self.last_command     = None    # Initially a no-op
-        self.precmd_hooks     = []
+        self.debug_nest = 1
+        self.display_mgr = Mdisplay.DisplayMgr()
+        self.intf = core_obj.debugger.intf
+        self.last_command = None  # Initially a no-op
+        self.precmd_hooks = []
 
         # If not:
         # self.location         = lambda : print_location(self)
 
-        self.preloop_hooks    = []
-        self.postcmd_hooks    = []
+        self.preloop_hooks = []
+        self.postcmd_hooks = []
 
         self._populate_cmd_lists()
 
         # Stop only if line/file is different from last time
         self.different_line = None
 
         # These values updated on entry. Set initial values.
-        self.curframe       = None
-        self.event          = None
-        self.event_arg      = None
-        self.frame          = None
-        self.list_lineno    = 0
+        self.curframe = None
+        self.event = None
+        self.event_arg = None
+        self.frame = None
+        self.list_lineno = 0
 
         # Create a custom safe Repr instance and increase its maxstring.
         # The default of 30 truncates error messages too easily.
-        self._repr             = Repr()
-        self._repr.maxstring   = 100
-        self._repr.maxother    = 60
-        self._repr.maxset      = 10
-        self._repr.maxfrozen   = 10
-        self._repr.array       = 10
-        self._saferepr         = self._repr.repr
-        self.stack             = []
-        self.thread_name       = None
+        self._repr = Repr()
+        self._repr.maxstring = 100
+        self._repr.maxother = 60
+        self._repr.maxset = 10
+        self._repr.maxfrozen = 10
+        self._repr.array = 10
+        self._saferepr = self._repr.repr
+        self.stack = []
+        self.thread_name = None
         self.frame_thread_name = None
         return
 
-    def add_preloop_hook(self, hook, position=-1, nodups = True):
-        if hook in self.preloop_hooks: return False
+    def add_preloop_hook(self, hook, position=-1, nodups=True):
+        if hook in self.preloop_hooks:
+            return False
         self.preloop_hooks.insert(position, hook)
         return True
 
     def adjust_frame(self, pos, absolute_pos):
         """Adjust stack frame by pos positions. If absolute_pos then
         pos is an absolute number. Otherwise it is a relative number.
 
@@ -147,92 +152,92 @@
             Mmsg.errmsg(self, "No stack.")
             return
 
         # Below we remove any negativity. At the end, pos will be
         # the new value of self.curindex.
         if absolute_pos:
             if pos >= 0:
-                pos = len(self.stack)-pos-1
+                pos = len(self.stack) - pos - 1
             else:
-                pos = -pos-1
+                pos = -pos - 1
         else:
             pos += self.curindex
 
         if pos < 0:
-            Mmsg.errmsg(self,
-                        "Adjusting would put us beyond the oldest frame.")
+            Mmsg.errmsg(self, "Adjusting would put us beyond the oldest frame.")
             return
         elif pos >= len(self.stack):
-            Mmsg.errmsg(self,
-                        "Adjusting would put us beyond the newest frame.")
+            Mmsg.errmsg(self, "Adjusting would put us beyond the newest frame.")
             return
 
         self.curindex = pos
         self.curframe = self.stack[self.curindex][0]
         self.print_location()
         self.list_lineno = None
         return
 
     # To be overridden in derived debuggers
     def defaultFile(self):
         """Produce a reasonable default."""
         filename = self.curframe.f_code.co_filename
         # Consider using is_exec_stmt(). I just don't understand
         # the conditions under which the below test is true.
-        if filename == '<string>' and self.debugger.mainpyfile:
+        if filename == "<string>" and self.debugger.mainpyfile:
             filename = self.debugger.mainpyfile
             pass
         return filename
 
-    def event_processor(self, frame, event, event_arg, prompt='Trepan'):
-        'command event processor: reading a commands do something with them.'
-        self.frame     = frame
-        self.event     = event
+    def event_processor(self, frame, event, event_arg, prompt="Trepan"):
+        "command event processor: reading a commands do something with them."
+        self.frame = frame
+        self.event = event
         self.event_arg = event_arg
 
         filename = frame.f_code.co_filename
-        lineno   = frame.f_lineno
-        line     = linecache.getline(filename, lineno, frame.f_globals)
+        lineno = frame.f_lineno
+        line = linecache.getline(filename, lineno, frame.f_globals)
         if not line:
-            opts = {'output': 'plain',
-                    'reload_on_change': self.settings('reload'),
-                    'strip_nl': False}
+            opts = {
+                "output": "plain",
+                "reload_on_change": self.settings("reload"),
+                "strip_nl": False,
+            }
             line = pyficache.getline(filename, lineno, opts)
         self.current_source_text = line
-        if self.settings('skip') is not None:
+        if self.settings("skip") is not None:
             if Mbytecode.is_def_stmt(line, frame):
                 return True
             if Mbytecode.is_class_def(line, frame):
                 return True
             pass
         self.thread_name = Mthread.current_thread_name()
         self.frame_thread_name = self.thread_name
         self.process_commands()
         return True
 
     def forget(self):
-        """ Remove memory of state variables set in the command processor """
-        self.stack       = []
-        self.curindex    = 0
-        self.curframe    = None
+        """Remove memory of state variables set in the command processor"""
+        self.stack = []
+        self.curindex = 0
+        self.curframe = None
         self.thread_name = None
         self.frame_thread_name = None
         return
 
     def eval(self, arg):
         """Eval string arg in the current frame context."""
         try:
-            return eval(arg, self.curframe.f_globals,
-                        self.curframe.f_locals)
-        except:
+            return eval(arg, self.curframe.f_globals, self.curframe.f_locals)
+        except Exception:
             t, v = sys.exc_info()[:2]
             if isinstance(t, str):
                 exc_type_name = t
                 pass
-            else: exc_type_name = t.__name__
+            else:
+                exc_type_name = t.__name__
             Mmsg.errmsg(self, str("%s: %s" % (exc_type_name, arg)))
             raise
         return None  # Not reached
 
     def exec_line(self, line):
         if self.curframe:
             local_vars = self.curframe.f_locals
@@ -241,120 +246,126 @@
             local_vars = None
             # FIXME: should probably have place where the
             # user can store variables inside the debug session.
             # The setup for this should be elsewhere. Possibly
             # in interaction.
             global_vars = None
         try:
-            code = compile(line + '\n', '"%s"' % line, 'single')
+            code = compile(line + "\n", '"%s"' % line, "single")
             exec(code, global_vars, local_vars)
-        except:
+        except Exception:
             t, v = sys.exc_info()[:2]
             if isinstance(t, bytes):
                 exc_type_name = t
-            else: exc_type_name = t.__name__
-            Mmsg.errmsg(self, '%s: %s' % (str(exc_type_name), str(v)))
+            else:
+                exc_type_name = t.__name__
+            Mmsg.errmsg(self, "%s: %s" % (str(exc_type_name), str(v)))
             pass
         return
 
     def ok_for_running(self, cmd_obj, name, cmd_hash):
-        '''We separate some of the common debugger command checks here:
+        """We separate some of the common debugger command checks here:
         whether it makes sense to run the command in this execution state,
         if the command has the right number of arguments and so on.
-        '''
-        if hasattr(cmd_obj, 'execution_set'):
-            if not (self.core.execution_status in cmd_obj.execution_set):
-                part1 = ("Command '%s' is not available for execution "
-                         "status:" % name)
-                Mmsg.errmsg(self,
-                            Mmisc.
-                            wrapped_lines(part1,
-                                            self.core.execution_status,
-                                            self.debugger.settings['width']))
+        """
+        if hasattr(cmd_obj, "execution_set"):
+            if self.core.execution_status not in cmd_obj.execution_set:
+                part1 = "Command '%s' is not available for execution " "status:" % name
+                Mmsg.errmsg(
+                    self,
+                    Mmisc.wrapped_lines(
+                        part1,
+                        self.core.execution_status,
+                        self.debugger.settings["width"],
+                    ),
+                )
                 return False
             pass
         if self.frame is None and cmd_obj.need_stack:
-            self.intf[-1].errmsg("Command '%s' needs an execution stack."
-                                 % name)
+            self.intf[-1].errmsg("Command '%s' needs an execution stack." % name)
             return False
         return True
 
     def process_commands(self):
         """Handle debugger commands."""
-        if self.core.execution_status != 'No program':
+        if self.core.execution_status != "No program":
             self.setup()
             Mlocation.print_location(self, self.event)
             pass
         leave_loop = run_hooks(self, self.preloop_hooks)
         self.continue_running = False
 
         while not leave_loop:
             try:
                 run_hooks(self, self.precmd_hooks)
                 # bdb had a True return to leave loop.
                 # A more straight-forward way is to set
                 # instance variable self.continue_running.
                 leave_loop = self.process_command()
-                if leave_loop or self.continue_running: break
+                if leave_loop or self.continue_running:
+                    break
             except EOFError:
                 # If we have stacked interfaces, pop to the next
                 # one.  If this is the last one however, we'll
                 # just stick with that.  FIXME: Possibly we should
                 # check to see if we are interactive.  and not
                 # leave if that's the case. Is this the right
                 # thing?  investigate and fix.
                 if len(self.debugger.intf) > 1:
                     del self.debugger.intf[-1]
-                    self.last_command = ''
+                    self.last_command = ""
                 else:
                     if self.debugger.intf[-1].output:
-                        self.debugger.intf[-1].output.writeline('Leaving')
+                        self.debugger.intf[-1].output.writeline("Leaving")
                         raise Mexcept.DebuggerQuit
                         pass
                     break
                 pass
             pass
         return run_hooks(self, self.postcmd_hooks)
 
     def process_command(self):
         # process command
-        self.response = {'errs': [], 'msg': []}
+        self.response = {"errs": [], "msg": []}
         cmd_hash = self.intf[-1].read_command()
 
         # FIXME: put this into a routine
         if not isinstance(cmd_hash, dict):
-            Mmsg.errmsg(self, "invalid input, expecting a hash: %s" % cmd_hash,
-                        {'set_name': True})
+            Mmsg.errmsg(
+                self,
+                "invalid input, expecting a hash: %s" % cmd_hash,
+                {"set_name": True},
+            )
             self.intf[-1].msg(self.response)
             return False
-        if 'command' not in cmd_hash:
-            Mmsg.errmsg(self,
-                        "invalid input, expecting a 'command' key: %s" %
-                        cmd_hash,
-                        {'set_name': True})
+        if "command" not in cmd_hash:
+            Mmsg.errmsg(
+                self,
+                "invalid input, expecting a 'command' key: %s" % cmd_hash,
+                {"set_name": True},
+            )
             self.intf[-1].msg(self.response)
             return False
 
-        self.cmd_name = cmd_hash['command']
+        self.cmd_name = cmd_hash["command"]
         cmd_name = resolve_name(self, self.cmd_name)
         if cmd_name:
             cmd_obj = self.commands[cmd_name]
             if self.ok_for_running(cmd_obj, cmd_name, cmd_hash):
                 try:
-                    self.response['name'] = cmd_name
+                    self.response["name"] = cmd_name
                     result = cmd_obj.run(cmd_hash)
                     self.intf[-1].msg(self.response)
-                    if result: return result
-                except (Mexcept.DebuggerQuit,
-                        Mexcept.DebuggerRestart, SystemExit):
+                    if result:
+                        return result
+                except (Mexcept.DebuggerQuit, Mexcept.DebuggerRestart, SystemExit):
                     # Let these exceptions propagate through
                     raise
-                except:
-                    Mmsg.errmsg(self, "INTERNAL ERROR: " +
-                                traceback.format_exc())
+                except Exception:
+                    Mmsg.errmsg(self, "INTERNAL ERROR: " + traceback.format_exc())
                     pass
                 pass
             else:
                 self.undefined_cmd(cmd_name)
                 pass
             pass
         return False
@@ -371,120 +382,131 @@
         """Initialization done before entering the debugger-command
         loop. In particular we set up the call stack used for local
         variable lookup and frame/up/down commands.
 
         We return True if we should NOT enter the debugger-command
         loop."""
         self.forget()
-        if self.settings('dbg_trepan'):
+        if self.settings("dbg_trepan"):
             self.frame = inspect.currentframe()
             pass
-        if self.event in ['exception', 'c_exception']:
+        if self.event in ["exception", "c_exception"]:
             exc_type, exc_value, exc_traceback = self.event_arg
         else:
-            _, _, exc_traceback = (None, None, None,)  # NOQA
+            _, _, exc_traceback = (
+                None,
+                None,
+                None,
+            )  # NOQA
             pass
         if self.frame or exc_traceback:
-            self.stack, self.curindex = \
-                get_stack(self.frame, exc_traceback, None, self)
+            self.stack, self.curindex = get_stack(self.frame, exc_traceback, None, self)
             self.curframe = self.stack[self.curindex][0]
             self.thread_name = Mthread.current_thread_name()
 
         else:
-            self.stack = self.curframe = \
-                self.botframe = None
+            self.stack = self.curframe = self.botframe = None
             pass
         if self.curframe:
-            self.list_lineno = \
-                max(1, inspect.getlineno(self.curframe))
+            self.list_lineno = max(1, inspect.getlineno(self.curframe))
         else:
             self.list_lineno = None
             pass
         # if self.execRcLines()==1: return True
         return False
 
     def undefined_cmd(self, cmd):
         """Error message when a command doesn't exist"""
         Mmsg.errmsg(self, 'Undefined command: "%s". Try "help".' % cmd)
         return
 
     def _populate_commands(self):
-        """ Create an instance of each of the debugger
+        """Create an instance of each of the debugger
         commands. Commands are found by importing files in the
         directory 'command'. Some files are excluded via an array set
         in __init__.  For each of the remaining files, we import them
         and scan for class names inside those files and for each class
         name, we will create an instance of that class. The set of
         DebuggerCommand class instances form set of possible debugger
         commands."""
         cmd_instances = []
         from trepan.bwprocessor import command as Mcommand
-        eval_cmd_template = 'command_mod.%s(self)'
+
+        eval_cmd_template = "command_mod.%s(self)"
         for mod_name in Mcommand.__modules__:
             import_name = "command." + mod_name
             try:
                 command_mod = getattr(__import__(import_name), mod_name)
-            except:
-                print('Error importing %s: %s' % (mod_name, sys.exc_info()[0]))
+            except Exception:
+                print("Error importing %s: %s" % (mod_name, sys.exc_info()[0]))
                 continue
 
-            classnames = [ tup[0] for tup in
-                           inspect.getmembers(command_mod, inspect.isclass)
-                           if ('DebuggerCommand' != tup[0] and
-                               tup[0].endswith('Command')) ]
+            classnames = [
+                tup[0]
+                for tup in inspect.getmembers(command_mod, inspect.isclass)
+                if ("DebuggerCommand" != tup[0] and tup[0].endswith("Command"))
+            ]
             for classname in classnames:
                 eval_cmd = eval_cmd_template % classname
                 try:
                     instance = eval(eval_cmd)
                     cmd_instances.append(instance)
-                except:
-                    print('Error loading %s from %s: %s' %
-                          (classname, mod_name, sys.exc_info()[0]))
+                except Exception:
+                    print(
+                        "Error loading %s from %s: %s"
+                        % (classname, mod_name, sys.exc_info()[0])
+                    )
                     pass
                 pass
             pass
         return cmd_instances
 
     def _populate_cmd_lists(self):
-        """ Populate self.commands"""
+        """Populate self.commands"""
         self.commands = {}
         for cmd_instance in self.cmd_instances:
             cmd_name = cmd_instance.name
             self.commands[cmd_name] = cmd_instance
             pass
         return
 
     pass
 
+
 # Demo it
-if __name__=='__main__':
+if __name__ == "__main__":
     from trepan.interfaces import bullwinkle as Mbullwinkle
 
     class Debugger:
         def __init__(self):
             self.intf = [Mbullwinkle.BWInterface()]
-            self.settings = {'dbg_trepan': True, 'reload': False}
+            self.settings = {"dbg_trepan": True, "reload": False}
+
         pass
 
     class MockCore:
-        def filename(self, fn): return fn
+        def filename(self, fn):
+            return fn
 
-        def canonic_filename(self, frame): return frame.f_code.co_filename
+        def canonic_filename(self, frame):
+            return frame.f_code.co_filename
 
         def __init__(self):
             self.debugger = Debugger()
             return
+
         pass
+
     core = MockCore()
     bwproc = BWProcessor(core)
-    print('commands:')
+    print("commands:")
     commands = list(bwproc.commands.keys())
     commands.sort()
     print(commands)
-    print(resolve_name(bwproc, 'quit'))
+    print(resolve_name(bwproc, "quit"))
     # print('-' * 10)
     # print_source_line(sys.stdout.write, 100, 'source_line_test.py')
     # print('-' * 10)
     bwproc.frame = sys._getframe()
     bwproc.setup()
     # print()
     # print('-' * 10)
```

### Comparing `trepan3k-1.2.8/trepan/bwprocessor/msg.py` & `trepan3k-1.2.9/trepan/bwprocessor/msg.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2015 Rocky Bernstein <rocky@gnu.org>
-''' Common I/O routines'''
+#   Copyright (C) 2015, 2023 Rocky Bernstein <rocky@gnu.org>
+""" Common I/O routines"""
+
 
 # Note for errmsg, msg, and msg_nocr we don't want to simply make
 # an assignment of method names like self.msg = self.debugger.intf.msg,
 # because we want to allow the interface (intf) to change
 # dynamically. That is, the value of self.debugger may change
-# in the course of the program and if we made such an method assignemnt
+# in the course of the program and if we made such an method assignment
 # we wouldn't pick up that change in our self.msg
 def errmsg(proc_obj, message, opts={}):
     response = proc_obj.response
-    if 'set_name' in opts: response['name'] = 'error'
-    return response['errs'].append(message)
+    if "set_name" in opts:
+        response["name"] = "error"
+    return response["errs"].append(message)
 
 
 def msg(proc_obj, message, opts={}):
     response = proc_obj.response
-    return response['msg'].append(message)
+    return response["msg"].append(message)
 
 
 # Demo it
-if __name__=='__main__':
+if __name__ == "__main__":
+
     class Demo:
         def __init__(self):
-            self.response = {'errs': [],
-                             'msg' : []}
+            self.response = {"errs": [], "msg": []}
             pass
+
         pass
 
     import pprint
+
     demo = Demo()
-    msg(demo, 'hi')
+    msg(demo, "hi")
     pp = pprint.PrettyPrinter()
     pp.pprint(demo.response)
```

### Comparing `trepan3k-1.2.8/trepan/client.py` & `trepan3k-1.2.9/trepan/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2013-2017, 2021 Rocky Bernstein
+#
+#   Copyright (C) 2009, 2013-2017, 2021, 2023 Rocky Bernstein
 #
 #    This program is free software; you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation; either version 2 of the License, or
 #    (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
@@ -13,30 +14,29 @@
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program; if not, write to the Free Software
 #    Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 #    02110-1301 USA.
 
-import sys, time
+import sys
+import time
+from optparse import OptionParser
 
 # Our local modules
-from trepan.interfaces import client as Mclient
-from trepan.interfaces import comcodes as Mcomcodes
-
-from optparse import OptionParser
+from trepan.interfaces import client as Mclient, comcodes as Mcomcodes
 from trepan.version import __version__
 
 
 def process_options(pkg_version, sys_argv, option_list=None):
     """Handle debugger options. Set `option_list' if you are writing
     another main program and want to extend the existing set of debugger
     options.
 
-    The options dicionary from opt_parser is return. sys_argv is
+    The options dictionary from opt_parser is return. sys_argv is
     also updated."""
     usage_str = """%prog [debugger-options]]
 
     Client connection to an out-of-process trepan3k debugger session"""
 
     # serverChoices = ('TCP','FIFO', None) # we use PID for now.
```

### Comparing `trepan3k-1.2.8/trepan/clifns.py` & `trepan3k-1.2.9/trepan/clifns.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,95 +1,100 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2008-2009, 2013 Rocky Bernstein <rocky@gnu.org>
+#   Copyright (C) 2008-2009, 2013, 2023 Rocky Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import os, linecache
+import linecache
+import os
 import os.path as osp
 
 
 # FIXME: do a better job of this. Live parsing?
 def is_ok_line_for_breakpoint(filename, lineno, errmsg_fn):
     """Check whether specified line seems to be executable.
 
     Return `lineno` if it is, 0 if not (e.g. a docstring, comment, blank
     line or EOF). Warning: testing is not comprehensive.
     """
     line = linecache.getline(filename, lineno)
     if not line:
-        errmsg_fn('End of file')
+        errmsg_fn("End of file")
         return False
     line = line.strip()
     # Don't allow setting breakpoint at a blank line
-    if (not line or (line[0] == '#') or
-         (line[:3] == '"""') or line[:3] == "'''"):
-        errmsg_fn('Blank or comment')
+    if not line or (line[0] == "#") or (line[:3] == '"""') or line[:3] == "'''":
+        errmsg_fn("Blank or comment")
         return False
     return True
 
 
 def file2module(filename):
-    """Given a file name, extract the most likely module name. """
+    """Given a file name, extract the most likely module name."""
     basename = osp.basename(filename)
-    if '.' in basename:
-        pos = basename.rfind('.')
+    if "." in basename:
+        pos = basename.rfind(".")
         return basename[:pos]
     else:
         return basename
     return None
 
 
 def search_file(filename, directories, cdir):
     """Return a full pathname for filename if we can find one. path
     is a list of directories to prepend to filename. If no file is
     found we'll return None"""
 
     for trydir in directories:
 
         # Handle $cwd and $cdir
-        if trydir =='$cwd': trydir='.'
-        elif trydir == '$cdir': trydir = cdir
+        if trydir == "$cwd":
+            trydir = "."
+        elif trydir == "$cdir":
+            trydir = cdir
 
         tryfile = osp.realpath(osp.join(trydir, filename))
         if osp.isfile(tryfile):
             return tryfile
     return None
 
 
 def whence_file(py_script, dirnames=None):
     """Do a shell-like path lookup for py_script and return the results.
     If we can't find anything return py_script"""
     if py_script.find(os.sep) != -1:
         # Don't search since this name has path separator components
         return py_script
     if dirnames is None:
-        dirnames = os.environ['PATH'].split(os.pathsep)
+        dirnames = os.environ["PATH"].split(os.pathsep)
     for dirname in dirnames:
         py_script_try = osp.join(dirname, py_script)
         if osp.exists(py_script_try):
             return py_script_try
     # Failure
     return py_script
 
+
 def path_expanduser_abs(filename):
     return os.path.abspath(os.path.expanduser(filename))
 
+
 # Demo
-if __name__=='__main__':
+if __name__ == "__main__":
     import sys
+
     print(file2module(sys.argv[0]), sys.argv[0])
     ok = is_ok_line_for_breakpoint(__file__, 1, sys.stdout.write)
     print("\nCan stop at line 1? ", ok)
     ok = is_ok_line_for_breakpoint(__file__, 2, sys.stdout.write)
     print("\nCan stop at line 2? ", ok)
     print(path_expanduser_abs("./.trepan3krc"))
     print(path_expanduser_abs("~/.trepan3krc"))
```

### Comparing `trepan3k-1.2.8/trepan/debugger.py` & `trepan3k-1.2.9/trepan/debugger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2008-2010, 2013-2015, 2018 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2008-2010, 2013-2015, 2018, 2023 Rocky Bernstein
+#   <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -25,46 +27,52 @@
 a Python script and `core' which contains the core debugging
 start/stop and event-handling dispatcher and `client.py' which is a
 user or client-side code for connecting to server'd debugged program.
 """
 
 # Our local modules
 
-from trepan.exception import DebuggerQuit, DebuggerRestart
+# Common Python packages
+import sys
+import types
+
+import pyficache
+import tracefilter
+
+# External Egg packages
+import tracer
+
+import trepan.interfaces.user as Muser
 
 # Default settings used here
 import trepan.lib.default as Mdefault
-import trepan.interfaces.user as Muser
-from trepan.misc import option_set
 import trepan.lib.sighandler as Msig
-
-# Common Python packages
-import sys, types
-
-# External Egg packages
-import tracer, tracefilter, pyficache
+from trepan.exception import DebuggerQuit, DebuggerRestart
+from trepan.misc import option_set
 
 debugger_obj = None
 
 try:
     from readline import get_line_buffer
 except ImportError:
+
     def get_line_buffer():
         return None
+
     pass
 
-class Trepan(object):
 
+class Trepan(object):
     # The following functions have to be defined before
     # DEFAULT_INIT_OPTS which includes references to these.
 
     # FIXME DRY run, run_exec, run_eval.
 
     def run(self, cmd, start_opts=None, globals_=None, locals_=None):
-        """ Run debugger on string `cmd' using builtin function eval
+        """Run debugger on string `cmd' using builtin function eval
         and if that builtin exec.  Arguments `globals_' and `locals_'
         are the dictionaries to use for local and global variables. By
         default, the value of globals is globals(), the current global
         variables. If `locals_' is not given, it becomes a copy of
         `globals_'.
 
         Debugger.core.start settings are passed via optional
@@ -76,15 +84,15 @@
         """
         if globals_ is None:
             globals_ = globals()
         if locals_ is None:
             locals_ = globals_
         if not isinstance(cmd, types.CodeType):
             self.eval_string = cmd
-            cmd = cmd+'\n'
+            cmd = cmd + "\n"
             pass
         retval = None
         self.core.start(start_opts)
         try:
             retval = eval(cmd, globals_, locals_)
         except SyntaxError:
             try:
@@ -97,15 +105,15 @@
         except DebuggerQuit:
             pass
         finally:
             self.core.stop()
         return retval
 
     def run_exec(self, cmd, start_opts=None, globals_=None, locals_=None):
-        """ Run debugger on string `cmd' which will executed via the
+        """Run debugger on string `cmd' which will executed via the
         builtin function exec. Arguments `globals_' and `locals_' are
         the dictionaries to use for local and global variables. By
         default, the value of globals is globals(), the current global
         variables. If `locals_' is not given, it becomes a copy of
         `globals_'.
 
         Debugger.core.start settings are passed via optional
@@ -116,44 +124,44 @@
         `run_call' if you want to debug function run_call.
         """
         if globals_ is None:
             globals_ = globals()
         if locals_ is None:
             locals_ = globals_
         if not isinstance(cmd, types.CodeType):
-            cmd = cmd+'\n'
+            cmd = cmd + "\n"
             pass
         self.core.start(start_opts)
         try:
             exec(cmd, globals_, locals_)
         except DebuggerQuit:
             pass
         finally:
             self.core.stop()
         return
 
     def run_call(self, func, start_opts=None, *args, **kwds):
-        """ Run debugger on function call: `func(*args, **kwds)'
+        """Run debugger on function call: `func(*args, **kwds)'
 
         See also `run_eval' if what you want to run is an eval'able
         expression have that result returned and `run' if you want to
-        debug a statment via exec.
+        debug a statement via exec.
         """
         res = None
         self.core.start(opts=start_opts)
         try:
             res = func(*args, **kwds)
         except DebuggerQuit:
             pass
         finally:
             self.core.stop()
         return res
 
     def run_eval(self, expr, start_opts=None, globals_=None, locals_=None):
-        """ Run debugger on string `expr' which will executed via the
+        """Run debugger on string `expr' which will executed via the
         built-in Python function: eval; `globals_' and `locals_' are
         the dictionaries to use for local and global variables. If
         `globals' is not given, __main__.__dict__ (the current global
         variables) is used. If `locals_' is not given, it becomes a
         copy of `globals_'.
 
         See also `run_call' if what you to debug a function call and
@@ -161,30 +169,29 @@
         """
         if globals_ is None:
             globals_ = globals()
         if locals_ is None:
             locals_ = globals_
         if not isinstance(expr, types.CodeType):
             self.eval_string = expr
-            expr = expr+'\n'
+            expr = expr + "\n"
             pass
         retval = None
         self.core.start(start_opts)
         try:
             retval = eval(expr, globals_, locals_)
         except DebuggerQuit:
             pass
         finally:
-            pyficache.remove_remap_file('<string>')
+            pyficache.remove_remap_file("<string>")
             self.core.stop()
         return retval
 
-    def run_script(self, filename, start_opts=None, globals_=None,
-                   locals_=None):
-        """ Run debugger on Python script `filename'. The script may
+    def run_script(self, filename, start_opts=None, globals_=None, locals_=None):
+        """Run debugger on Python script `filename'. The script may
         inspect sys.argv for command arguments. `globals_' and
         `locals_' are the dictionaries to use for local and global
         variables. If `globals' is not given, globals() (the current
         global variables) is used. If `locals_' is not given, it
         becomes a copy of `globals_'.
 
         True is returned if the program terminated normally and False
@@ -198,218 +205,226 @@
         self.mainpyfile = self.core.canonic(filename)
 
         # Start with fresh empty copy of globals and locals and tell the script
         # that it's being run as __main__ to avoid scripts being able to access
         # the debugger namespace.
         if globals_ is None:
             import __main__  # NOQA
-            globals_ = {"__name__" : "__main__",
-                       "__file__" : self.mainpyfile,
-                       "__builtins__" : __builtins__
-                       }  # NOQA
+
+            globals_ = {
+                "__name__": "__main__",
+                "__file__": self.mainpyfile,
+                "__builtins__": __builtins__,
+            }  # NOQA
         if locals_ is None:
             locals_ = globals_
         retval = False
-        self.core.execution_status = 'Running'
+        self.core.execution_status = "Running"
         try:
-            compiled = compile(open(self.mainpyfile).read(),
-                               self.mainpyfile, 'exec')
-        except (SyntaxError):
+            compiled = compile(open(self.mainpyfile).read(), self.mainpyfile, "exec")
+        except SyntaxError:
             self.intf[0].errmsg("Python can't compile %s" % self.mainpyfile)
             self.intf[0].errmsg(sys.exc_info()[1])
             retval = False
             pass
         except UnicodeDecodeError:
-            self.intf[0].errmsg("File %s can't be read as a text file. Is it Python source?" % self.mainpyfile)
+            self.intf[0].errmsg(
+                "File %s can't be read as a text file. Is it Python source?"
+                % self.mainpyfile
+            )
             self.intf[0].errmsg(sys.exc_info()[1])
             retval = False
             pass
         except IOError:
             print(sys.exc_info()[1])
         except DebuggerQuit:
             retval = False
             pass
         except DebuggerRestart:
-            self.core.execution_status = 'Restart requested'
+            self.core.execution_status = "Restart requested"
             raise DebuggerRestart
         else:
             self.core.start(start_opts)
             exec(compiled, globals_, locals_)
             retval = True
         finally:
-            self.core.stop(options={'remove': True})
+            self.core.stop(options={"remove": True})
         return retval
 
     def restart_argv(self):
-        '''Return an array that would be execv-ed  to restart the program'''
+        """Return an array that would be execv-ed  to restart the program"""
         return self.orig_sys_argv or self.program_sys_argv
 
     # Note: has to come after functions listed in ignore_filter.
     DEFAULT_INIT_OPTS = {
         # What routines will we not trace into?
-        'ignore_filter': tracefilter.TraceFilter(
-            [tracer.start, tracer.stop,
-             run_eval, run_call, run_eval, run_script]),
-
+        "ignore_filter": tracefilter.TraceFilter(
+            [tracer.start, tracer.stop, run_eval, run_call, run_eval, run_script]
+        ),
         # sys.argv when not None contains sys.argv *before* debugger
         # command processing. So sys.argv contains debugger options as
         # well as debugged-program options. These options are used to
         # do a "hard" or execv() restart.
-
         # program_sys_argv is set by option save_sys_argv and contains
         # sys.argv that we see now which may have debugger options
         # stripped, or it may be that we were not called from a
         # debugger front end but from inside the running
         # program. These options are suitable for a "soft" or
         # exception-handling DebuggerRestart kind of restart.
-        'orig_sys_argv' : None,
-        'save_sys_argv' : True,
-
+        "orig_sys_argv": None,
+        "save_sys_argv": True,
         # How is I/O for this debugger handled?
-        'activate'    : False,
-        'interface'   : None,
-        'input'       : None,
-        'output'      : None,
-        'processor'   : None,
-
+        "activate": False,
+        "interface": None,
+        "input": None,
+        "output": None,
+        "processor": None,
         # Setting contains lots of debugger settings - a whole file
         # full of them!
-        'settings'    : Mdefault.DEBUGGER_SETTINGS,
-
-        'start_opts'  : Mdefault.START_OPTS,
-        'step_ignore' : 0,
-
-        'from_ipython' : False
-        }
+        "settings": Mdefault.DEBUGGER_SETTINGS,
+        "start_opts": Mdefault.START_OPTS,
+        "step_ignore": 0,
+        "from_ipython": False,
+    }
 
     def __init__(self, opts=None):
         """Create a debugger object. But depending on the value of
         key 'start' inside hash 'opts', we may or may not initially
         start debugging.
 
         See also Debugger.start and Debugger.stop.
         """
 
         import trepan.lib.core as Mcore
 
-        self.mainpyfile  = None
-        self.thread      = None
+        self.mainpyfile = None
+        self.thread = None
         self.eval_string = None
-        get_option = lambda key: option_set(opts, key,
-                                            self.DEFAULT_INIT_OPTS)
-        completer  = lambda text, state: self.complete(text, state)
+        get_option = lambda key: option_set(opts, key, self.DEFAULT_INIT_OPTS)
+        completer = lambda text, state: self.complete(text, state)
 
         # set the instance variables that come directly from options.
-        for opt in ('settings', 'orig_sys_argv', 'from_ipython'):
+        for opt in ("settings", "orig_sys_argv", "from_ipython"):
             setattr(self, opt, get_option(opt))
             pass
 
         core_opts = {}
-        for opt in ('ignore_filter', 'proc_opts', 'processor', 'step_ignore',
-                    'processor',):
+        for opt in (
+            "ignore_filter",
+            "proc_opts",
+            "processor",
+            "step_ignore",
+            "processor",
+        ):
             core_opts[opt] = get_option(opt)
             pass
 
         # How is I/O for this debugger handled? This should
         # be set before calling DebuggerCore.
-        interface_opts={
+        interface_opts = {
             "complete": completer,
             "debugger_name": "trepan3k",
         }
         # FIXME when I pass in opts=opts things break
-        interface = (get_option('interface') or
-                     Muser.UserInterface(opts=interface_opts))
+        interface = get_option("interface") or Muser.UserInterface(opts=interface_opts)
         self.intf = [interface]
 
-        inp = get_option('input')
+        inp = get_option("input")
         if inp:
             self.intf[-1].input = inp
             pass
 
-        out = get_option('output')
+        out = get_option("output")
         if out:
             self.intf[-1].output = out
             pass
 
         self.core = Mcore.TrepanCore(self, core_opts)
         self.core.add_ignore(self.core.stop)
 
         # When set True, we'll also suspend our debug-hook tracing.
         # This gives us a way to prevent or allow self debugging.
         self.core.trace_hook_suspend = False
 
-        if get_option('save_sys_argv'):
+        if get_option("save_sys_argv"):
             # Save the debugged program's sys.argv? We do this so that
             # when the debugged script munges these, we have a good
             # copy to use for an exec restart
             self.program_sys_argv = list(sys.argv)
         else:
             self.program_sys_argv = None
             pass
 
         self.sigmgr = Msig.SignalManager(self)
 
         # Were we requested to activate immediately?
-        if get_option('activate'):
-            self.core.start(get_option('start_opts'))
+        if get_option("activate"):
+            self.core.start(get_option("start_opts"))
             pass
         return
 
     def complete(self, last_token, state):
-        if hasattr(self.core.processor, 'completer'):
+        if hasattr(self.core.processor, "completer"):
             str = get_line_buffer() or last_token
             results = self.core.processor.completer(str, state)
             return results[state]
         else:
             return [None]
+
     pass
 
+
 # Demo it
-if __name__=='__main__':
+if __name__ == "__main__":
+
     def foo():
         y = 2
         for i in range(2):
-            print("%d %d" % (i, y) )
+            print("%d %d" % (i, y))
             pass
         return 3
+
     import debugger
+
     d = debugger.Trepan()
-    d.settings['trace'] = True
-    d.settings['printset'] = tracer.ALL_EVENTS
+    d.settings["trace"] = True
+    d.settings["printset"] = tracer.ALL_EVENTS
     d.core.step_ignore = -1
     print('Issuing: run_eval("1+2")')
-    print(d.run_eval('1+2'))
+    print(d.run_eval("1+2"))
     print('Issuing: run_exec("x=1; y=2")')
-    d.run_exec('x=1; y=2')
+    d.run_exec("x=1; y=2")
 
     print('Issuing: run("3*4")')
-    print(d.run('3*4'))
+    print(d.run("3*4"))
     print('Issuing: run("x=3; y=4")')
-    d.run('x=3; y=4')
+    d.run("x=3; y=4")
 
-    print('Issuing: run_call(foo)')
+    print("Issuing: run_call(foo)")
     d.run_call(foo)
     if len(sys.argv) > 1:
         while True:
             try:
-                print('started')
+                print("started")
                 d.core.step_ignore = 0
                 d.core.start()
                 x = 4
                 x = foo()
                 for i in range(2):
-                    print("%d" % (i+1)*10)
+                    print("%d" % (i + 1) * 10)
                     pass
                 d.core.stop()
 
-                def square(x): return x*x
-                print('calling: run_call(square,2)')
+                def square(x):
+                    return x * x
+
+                print("calling: run_call(square,2)")
                 d.run_call(square, 2)
             except DebuggerQuit:
                 print("That's all Folks!...")
                 break
             except DebuggerRestart:
-                print('Restarting...')
+                print("Restarting...")
                 pass
             pass
         pass
     pass
```

### Comparing `trepan3k-1.2.8/trepan/exception.py` & `trepan3k-1.2.9/trepan/exception.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/trepan/inout/base.py` & `trepan3k-1.2.9/trepan/inout/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2014-2015, 2020 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2009, 2014-2015, 2020, 2023 Rocky Bernstein
+#   <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """classes to support communication to and from the debugger.  This
-communcation might be to/from another process or another computer.
+communication might be to/from another process or another computer.
 And reading may be from a debugger command script.
 
 For example, we'd like to support Sockets, and serial lines and file
 reading, as well a readline-type input. Encryption and Authentication
 methods might decorate some of the communication channels.
 
-Some ideas originiated as part of Matt Fleming's 2006 Google Summer of
+Some ideas originated as part of Matt Fleming's 2006 Google Summer of
 Code project.
 """
 
 from abc import ABCMeta
 
 NotImplementedMessage = "This method must be overriden in a subclass"
 
@@ -43,15 +45,15 @@
             pass
         return
 
     def use_history(self):
         return False
 
     def open(self, inp, opts=None):
-        """Use this to set where to read from. """
+        """Use this to set where to read from."""
         raise NotImplementedError(NotImplementedMessage)
 
     def readline(self, use_raw=None):
         """Read a line of input. EOFError will be raised on EOF.
 
         Note that we don't support prompting first. Instead, arrange
         to call DebuggerOutput.write() first with the prompt. If
@@ -62,15 +64,15 @@
         """
         raise NotImplementedError(NotImplementedMessage)
 
     pass
 
 
 class DebuggerInOutBase(metaclass=ABCMeta):
-    """ This is an abstract class that specifies debugger output. """
+    """This is an abstract class that specifies debugger output."""
 
     def __init__(self, out=None, opts=None):
         self.output = None
         return
 
     def close(self):
         if self.output:
@@ -84,25 +86,25 @@
     def write(self, output):
         """Use this to set where to write to. output can be a
         file object or a string. This code raises IOError on error.
         """
         raise NotImplementedError(NotImplementedMessage)
 
     def writeline(self, msg):
-        """ used to write to a debugger that is connected to this
+        """used to write to a debugger that is connected to this
         server; `str' written will have a newline added to it
         """
         self.write("%s\n" % msg)
         return
 
     pass
 
 
 class TrepanInOutBase(metaclass=ABCMeta):
-    """ This is an abstract class that specifies debugger input output when
+    """This is an abstract class that specifies debugger input output when
     handled by the same channel, e.g. a socket or tty.
     """
 
     def __init__(self, inout=None, opts=None):
         self.inout = None
         return
 
@@ -112,15 +114,15 @@
             pass
         return
 
     def flush(self):
         raise NotImplementedError(NotImplementedMessage)
 
     def open(self, inp, opts=None):
-        """Use this to set where to read from. """
+        """Use this to set where to read from."""
         raise NotImplementedError(NotImplementedMessage)
 
     def readline(self, use_raw=None):
         """Read a line of input. EOFError will be raised on EOF.
 
         Note that we don't support prompting first. Instead, arrange
         to call DebuggerOutput.write() first with the prompt. If
@@ -134,15 +136,15 @@
     def write(self, output):
         """Use this to set where to write to. output can be a
         file object or a string. This code raises IOError on error.
         """
         raise NotImplementedError(NotImplementedMessage)
 
     def writeline(self, msg):
-        """ used to write to a debugger that is connected to this
+        """used to write to a debugger that is connected to this
         server; `str' written will have a newline added to it
         """
         self.write("%s\n" % msg)
         return
 
     pass
```

### Comparing `trepan3k-1.2.8/trepan/inout/fifoclient.py` & `trepan3k-1.2.9/trepan/inout/fifoclient.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2013-2015 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2009, 2013-2015, 2023 Rocky Bernstein
+#   <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -11,129 +13,133 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Debugger FIFO Input/Output interface. """
 
-import tempfile, os
+import os
+import tempfile
 
-from trepan.lib import default as Mdefault, file as Mfile
 from trepan import misc as Mmisc
 from trepan.inout.base import DebuggerInOutBase
+from trepan.lib import default as Mdefault, file as Mfile
 
 
 class FIFOClient(DebuggerInOutBase):
     """Debugger Client Input/Output Socket."""
 
-    DEFAULT_INIT_OPTS = {'open': True}
+    DEFAULT_INIT_OPTS = {"open": True}
 
     def __init__(self, inp=None, opts=None):
-        get_option = lambda key: Mmisc.option_set(opts, key,
-                                                  Mdefault.CLIENT_SOCKET_OPTS)
-        self.state = 'disconnected'
+        get_option = lambda key: Mmisc.option_set(
+            opts, key, Mdefault.CLIENT_SOCKET_OPTS
+        )
+        self.state = "disconnected"
         self.flush_after_write = True
-        self.input  = None
+        self.input = None
         self.output = None
         self.line_edit = False  # Our name for GNU readline capability
-        self.state    = 'disconnected'
-        open_pid = get_option('open')
+        self.state = "disconnected"
+        open_pid = get_option("open")
         if open_pid:
             self.open(open_pid)
             pass
         return
 
     def close(self):
-        """ Closes both input and output """
-        self.state = 'closing'
+        """Closes both input and output"""
+        self.state = "closing"
         if self.input:
             self.input.close()
             pass
         if self.output:
             self.output.close()
             pass
-        self.state = 'disconnnected'
+        self.state = "disconnnected"
         return
 
     def flush(self):
         return self.output.flush()
 
     def open(self, pid, opts=None):
 
         # Not in/out are reversed from server side
-        d              = tempfile.gettempdir()
-        self.out_name  = os.path.join(d, ('trepan-%s.in' % pid))
-        self.in_name   = os.path.join(d, ('trepan-%s.out' % pid))
+        d = tempfile.gettempdir()
+        self.out_name = os.path.join(d, ("trepan-%s.in" % pid))
+        self.in_name = os.path.join(d, ("trepan-%s.out" % pid))
         is_readable = Mfile.readable(self.out_name)
         if not is_readable:
             if is_readable is None:
-                raise IOError("output FIFO %s doesn't exist" %
-                              self.out_name)
+                raise IOError("output FIFO %s doesn't exist" % self.out_name)
             else:
-                raise IOError("output FIFO %s is not readable" %
-                              self.out_name)
+                raise IOError("output FIFO %s is not readable" % self.out_name)
             pass
         is_readable = Mfile.readable(self.in_name)
         if not is_readable:
             if is_readable is None:
-                raise IOError("input FIFO %s doesn't exist" %
-                              self.in_name)
+                raise IOError("input FIFO %s doesn't exist" % self.in_name)
             else:
-                raise IOError("input FIFO %s is not readable" %
-                              self.out_name)
+                raise IOError("input FIFO %s is not readable" % self.out_name)
             pass
-        self.state     = 'active'
+        self.state = "active"
         return
 
     def read_msg(self):
         """Read a line of input. EOFError will be raised on EOF.
 
         Note that we don't support prompting"""
         # FIXME: do we have to create and check a buffer for
         # lines?
-        if self.state == 'active':
+        if self.state == "active":
             if not self.input:
-                self.input = open(self.in_name, 'r')
+                self.input = open(self.in_name, "r")
                 pass
             line = self.input.readline()
             if not line:
-                self.state = 'disconnected'
+                self.state = "disconnected"
                 raise EOFError
             return line.encode("utf-8")
         else:
             raise IOError("readline called in state: %s." % self.state)
         return  # Not reached
 
     def write(self, msg):
-        """ This method the debugger uses to write. In contrast to
+        """This method the debugger uses to write. In contrast to
         writeline, no newline is added to the end to `str'.
         """
-        if self.state == 'active':
+        if self.state == "active":
             if not self.output:
-                self.output = open(self.out_name, 'w')
+                self.output = open(self.out_name, "w")
                 pass
             pass
         else:
             raise EOFError
         self.output.write(msg)
-        if self.flush_after_write: self.flush()
+        if self.flush_after_write:
+            self.flush()
         return
 
+
 # Demo
-if __name__=='__main__':
-    fifo = FIFOClient(opts={'open': False})
+if __name__ == "__main__":
+    fifo = FIFOClient(opts={"open": False})
     import sys
+
     if len(sys.argv) > 1:
-        print('Connecting...',)
+        print(
+            "Connecting...",
+        )
         fifo.open(sys.argv[1])
-        print('connected.')
+        print("connected.")
         while True:
             prompt = fifo.readline()
             line = input(prompt)
-            if len(line) == 0: break
+            if len(line) == 0:
+                break
             try:
                 line = fifo.writeline(line)
                 print("Got: ", fifo.readline())
             except EOFError:
                 break
             pass
         pass
```

### Comparing `trepan3k-1.2.8/trepan/inout/fifoserver.py` & `trepan3k-1.2.9/trepan/inout/fifoserver.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,124 +13,127 @@
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Debugger FIFO Input/Output interface. """
 
 import os
 
-if hasattr(os, 'mkfifo'):
-    import atexit, tempfile
+if hasattr(os, "mkfifo"):
+    import atexit
+    import tempfile
 
     from trepan import misc as Mmisc
     from trepan.inout.base import DebuggerInOutBase
 
     # FIXME: Consider using Python's socketserver/SocketServer?
     class FIFOServer(DebuggerInOutBase):
         """Debugger Server Input/Output Socket."""
 
-        DEFAULT_INIT_OPTS = {'open': True}
+        DEFAULT_INIT_OPTS = {"open": True}
 
         def __init__(self, opts=None):
-            get_option = lambda key: Mmisc.option_set(opts, key,
-                                                      self.DEFAULT_INIT_OPTS)
+            get_option = lambda key: Mmisc.option_set(opts, key, self.DEFAULT_INIT_OPTS)
             atexit.register(self.close)
             self.flush_after_write = True
             self.line_edit = False  # Our name for GNU readline capability
-            self.in_name   = None   # String: input file name
-            self.input     = None   # File Descriptor
-            self.out_name  = None   # String: output file name
-            self.output    = None   # String: output file name
-            self.state     = 'disconnected'
-            if get_option('open'):
+            self.in_name = None  # String: input file name
+            self.input = None  # File Descriptor
+            self.out_name = None  # String: output file name
+            self.output = None  # String: output file name
+            self.state = "disconnected"
+            if get_option("open"):
                 self.open(opts)
                 pass
             return
 
         def close(self):
-            """ Closes both input and output. """
-            self.state = 'closing'
+            """Closes both input and output."""
+            self.state = "closing"
             if self.input:
                 self.input.close()
                 pass
             if self.in_name and os.path.exists(self.in_name):
                 os.unlink(self.in_name)
                 pass
             if self.output:
                 self.output.close()
                 pass
             if self.out_name and os.path.exists(self.out_name):
                 os.unlink(self.out_name)
                 pass
-            self.state = 'disconnnected'
+            self.state = "disconnnected"
             return
 
         def flush(self):
             return self.output.flush()
 
         def open(self, opts=None):
-            d              = tempfile.gettempdir()
-            pid            = os.getpid()
-            self.out_name  = os.path.join(d, ('trepan-%s.out' % pid))
-            self.in_name   = os.path.join(d, ('trepan-%s.in' % pid))
+            d = tempfile.gettempdir()
+            pid = os.getpid()
+            self.out_name = os.path.join(d, ("trepan-%s.out" % pid))
+            self.in_name = os.path.join(d, ("trepan-%s.in" % pid))
             try:
                 os.mkfifo(self.in_name)
                 os.mkfifo(self.out_name)
-                self.state     = 'active'
+                self.state = "active"
             except OSError:
-                self.state = 'error'
+                self.state = "error"
                 pass
             return
 
         def read_msg(self):
             """Read a line of input. EOFError will be raised on EOF.
 
             Note that we don't support prompting"""
             # FIXME: do we have to create and check a buffer for
             # lines?
-            if self.state == 'active':
+            if self.state == "active":
                 if not self.input:
-                    self.input = open(self.in_name, 'r')
+                    self.input = open(self.in_name, "r")
                     pass
                 line = self.input.readline()
                 if not line:
-                    self.state = 'disconnected'
+                    self.state = "disconnected"
                     raise EOFError
                 return line.rstrip("\n")
             else:
                 raise EOFError
             return  # Not reached
 
         def write(self, msg):
-            """ This method the debugger uses to write. In contrast to
+            """This method the debugger uses to write. In contrast to
             writeline, no newline is added to the end to `str'.
             """
-            if self.state == 'active':
+            if self.state == "active":
                 if not self.output:
-                    self.output = open(self.out_name, 'w')
+                    self.output = open(self.out_name, "w")
                     pass
                 pass
             else:
                 raise EOFError
             self.output.write(msg)
-            if self.flush_after_write: self.flush()
+            if self.flush_after_write:
+                self.flush()
             return
+
     # Demo
-    if __name__=='__main__':
-        fifo = FIFOServer(opts={'open': False})
+    if __name__ == "__main__":
+        fifo = FIFOServer(opts={"open": False})
         import sys
+
         if len(sys.argv) > 1:
             fifo.open()
             print('Looking for input on %s"...' % fifo.in_name)
             while True:
                 try:
-                    fifo.write('nu?')
-                    fifo.writeline(' ')
+                    fifo.write("nu?")
+                    fifo.writeline(" ")
                     line = fifo.readline()
                     print(line)
-                    fifo.writeline('ack: ' + line)
+                    fifo.writeline("ack: " + line)
                 except EOFError:
                     break
                 pass
             pass
         fifo.close()
         pass
     pass
```

### Comparing `trepan3k-1.2.8/trepan/inout/input.py` & `trepan3k-1.2.9/trepan/inout/input.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009-2010, 2013-2015, 2017 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2009-2010, 2013-2015, 2017, 2023 Rocky Bernstein
+#   <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -11,49 +13,51 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Debugger input possibly attached to a user or interactive. """
 
-import io, sys
+import io
+import sys
 
 from trepan import misc as Mmisc
 from trepan.inout import base as Mbase
 
 
-def readline_importable():
+def readline_importable() -> bool:
     try:
         import readline  # NOQA
+
         return True
     except ImportError:
         return False
     return  # Not reached
 
 
 class DebuggerUserInput(Mbase.DebuggerInputBase):
     """Debugger input connected to what we think of as a end-user input
     as opposed to a relay mechanism to another process. Input could be
-    interative terminal, but it might be file input."""
+    interactive terminal, but it might be file input."""
 
     def __init__(self, inp=None, opts=None):
-        self.input     = inp or sys.stdin
+        self.input = inp or sys.stdin
         self.line_edit = None  # Our name for GNU readline capability
         self.open(self.input, opts)
         return
 
     def close(self):
         self.input.close()
         self.closed = True
         return
 
     DEFAULT_OPEN_READ_OPTS = {
-        'use_raw'      : True,
-        'try_readline' : True,
-        }
+        "use_raw": True,
+        "try_readline": True,
+    }
 
     def use_history(self):
         return self.use_raw and readline_importable()
 
     def open(self, inp, opts={}):
         """Use this to set where to read from.
 
@@ -64,36 +68,39 @@
         opts['try_readline'] is set.
 
         Set opts['use_raw'] if input should use Python's use_raw(). If
         however 'inp' is a string and opts['use_raw'] is not set, we
         will assume no raw output. Note that an individual readline
         may override the setting.
         """
-        get_option = lambda key: Mmisc.option_set(opts, key,
-                                                  self.DEFAULT_OPEN_READ_OPTS)
-        if (isinstance(inp, io.TextIOWrapper) or
-            isinstance(inp, io.StringIO) or
-            hasattr(inp, 'isatty') and inp.isatty()):
-            self.use_raw = get_option('use_raw')
-        elif isinstance(inp, 'string'.__class__):  # FIXME
+        get_option = lambda key: Mmisc.option_set(
+            opts, key, self.DEFAULT_OPEN_READ_OPTS
+        )
+        if (
+            isinstance(inp, io.TextIOWrapper)
+            or isinstance(inp, io.StringIO)
+            or hasattr(inp, "isatty")
+            and inp.isatty()
+        ):
+            self.use_raw = get_option("use_raw")
+        elif isinstance(inp, "string".__class__):  # FIXME
             if opts is None:
                 self.use_raw = False
             else:
-                self.use_raw = get_option('use_raw')
+                self.use_raw = get_option("use_raw")
                 pass
-            inp = open(inp, 'r')
+            inp = open(inp, "r")
         else:
-            raise IOError("Invalid input type (%s) for %s" % (type(inp),
-                                                                inp))
-        self.input     = inp
-        self.line_edit = get_option('try_readline') and readline_importable()
+            raise IOError("Invalid input type (%s) for %s" % (type(inp), inp))
+        self.input = inp
+        self.line_edit = get_option("try_readline") and readline_importable()
         self.closed = False
         return
 
-    def readline(self, use_raw=None, prompt=''):
+    def readline(self, use_raw=None, prompt=""):
         """Read a line of input. EOFError will be raised on EOF.
 
         Note: some user interfaces may decide to arrange to call
         DebuggerOutput.write() first with the prompt rather than pass
         it here.. If `use_raw' is set raw_input() will be used in that
         is supported by the specific input input. If this option is
         left None as is normally expected the value from the class
@@ -110,47 +117,50 @@
                 return inp
             except ValueError:
                 raise EOFError
             pass
 
         else:
             line = self.input.readline()
-            if not line: raise EOFError
+            if not line:
+                raise EOFError
             return line.rstrip("\n")
         pass
+
     pass
 
+
 # Demo
-if __name__=='__main__':
-    print('readline importable: ', readline_importable())
+if __name__ == "__main__":
+    print("readline importable: ", readline_importable())
     inp = DebuggerUserInput(__file__)
     line = inp.readline()
     print(line)
     inp.close()
-    inp.open('input.py', opts={'use_raw': False})
+    inp.open("input.py", opts={"use_raw": False})
     while True:
         try:
             inp.readline()
         except EOFError:
             break
         pass
     try:
         inp.readline()
     except EOFError:
-        print('EOF handled correctly')
+        print("EOF handled correctly")
     pass
 
     if len(sys.argv) > 1:
         inp = DebuggerUserInput()
         try:
-            print("Type some characters:", end=' ')
+            print("Type some characters:", end=" ")
             line = inp.readline()
             print("You typed: %s" % line)
-            print("Type some more characters (raw):", end=' ')
+            print("Type some more characters (raw):", end=" ")
             line = inp.readline(True)
-            print("Type even more characters (not raw):", end=' ')
+            print("Type even more characters (not raw):", end=" ")
             line = inp.readline(True)
             print("You also typed: %s" % line)
         except EOFError:
             print("Got EOF")
         pass
     pass
```

### Comparing `trepan3k-1.2.8/trepan/inout/output.py` & `trepan3k-1.2.9/trepan/inout/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2013, 2015, 2020 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2009, 2013, 2015, 2020, 2023 Rocky Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -11,22 +12,23 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Debugger output. """
 
-import io, sys
+import io
+import sys
 
 from trepan.inout.base import DebuggerInOutBase
 
 
 class DebuggerUserOutput(DebuggerInOutBase):
     """Debugger output shown directly to what we think of as end-user
-    ouptut as opposed to a relay mechanism to another process. Output
+    output as opposed to a relay mechanism to another process. Output
     could be an interactive terminal, but it might also be file output"""
 
     def __init__(self, out=None, opts=None):
 
         self.flush_after_write = False
         self.output = out or sys.stdout
         self.open(self.output, opts)
@@ -54,15 +56,15 @@
             )
             # raise IOError("Invalid output type (%s) for %s" % (type(output),
             #                                                     output))
         self.output = output
         return
 
     def write(self, msg):
-        """ This method the debugger uses to write. In contrast to
+        """This method the debugger uses to write. In contrast to
         writeline, no newline is added to the end to `str'.
         """
         if self.output.closed:
             raise IOError("writing %s on a closed file" % msg)
         self.output.write(msg)
         if self.flush_after_write:
             self.flush()
```

### Comparing `trepan3k-1.2.8/trepan/inout/scriptin.py` & `trepan3k-1.2.9/trepan/inout/scriptin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2014-2015 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2009, 2014-2015, 2023 Rocky Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -11,74 +12,77 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Debugger Script input interface. """
 
-import io, types
+import io
 
 from trepan.inout import base as Mbase
 
 
 # Do we need this?
 class ScriptInput(Mbase.DebuggerInputBase):
     """Debugger Script input - largely the same as DebuggerInput."""
 
     def __init__(self, inp, opts=None):
 
-        self.input     = None
+        self.input = None
         self.line_edit = False  # Our name for GNU readline capability
-        self.name      = None
+        self.name = None
         self.open(inp, opts)
         return
 
     def close(self):
         if self.input:
             self.input.close()
             pass
         return
 
     def open(self, inp, opts=None):
-        """Use this to set what file to read from. """
+        """Use this to set what file to read from."""
         if isinstance(inp, io.TextIOWrapper):
             self.input = inp
-        elif isinstance(inp, 'string'.__class__):  # FIXME
-            self.name  = inp
-            self.input = open(inp, 'r')
+        elif isinstance(inp, "string".__class__):  # FIXME
+            self.name = inp
+            self.input = open(inp, "r")
         else:
-            raise IOError("Invalid input type (%s) for %s" %
-                          (inp.__class__.__name__, inp))
+            raise IOError(
+                "Invalid input type (%s) for %s" % (inp.__class__.__name__, inp)
+            )
         return
 
-    def readline(self, prompt='', use_raw=None):
+    def readline(self, prompt="", use_raw=None):
         """Read a line of input. Prompt and use_raw exist to be
         compatible with other input routines and are ignored.
         EOFError will be raised on EOF.
         """
         line = self.input.readline()
-        if not line: raise EOFError
+        if not line:
+            raise EOFError
         return line.rstrip("\n")
 
+
 # Demo
-if __name__=='__main__':
+if __name__ == "__main__":
     import os
-    my_file = os.path.join(os.path.dirname(os.path.abspath(__file__)),
-                           'scriptin.py')
+
+    my_file = os.path.join(os.path.dirname(os.path.abspath(__file__)), "scriptin.py")
     inp = ScriptInput(my_file)
     line = inp.readline()
     print(line)
     inp.close()
     # Note opts below are aren't acted upon. They are there for
     # compatibility
-    inp.open(my_file, opts={'use_raw': False})
+    inp.open(my_file, opts={"use_raw": False})
     while True:
         try:
             inp.readline()
         except EOFError:
             break
         pass
     try:
         inp.readline()
     except EOFError:
-        print('EOF handled correctly')
+        print("EOF handled correctly")
     pass
```

### Comparing `trepan3k-1.2.8/trepan/inout/stringarray.py` & `trepan3k-1.2.9/trepan/inout/stringarray.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2013-2014 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2009, 2013-2014, 2023 Rocky Bernstein
+#   <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -18,133 +20,135 @@
 import types
 
 from trepan.inout import base as Mbase
 
 
 class StringArrayInput(Mbase.DebuggerInputBase):
     """Simulate I/O using an array of strings. Sort of like StringIO, but
-    even simplier. """
+    even simpler."""
 
     def __init__(self, inp=[], opts=None):
-        self.input  = inp
+        self.input = inp
         self.closed = False
         return
 
     def close(self):
-        'Interface is for compatibility'
+        "Interface is for compatibility"
         self.closed = True
         return
 
     def open(self, inp, opts=None):
-        """Use this to set where to read from.
-        """
+        """Use this to set where to read from."""
         if isinstance(inp, list):
             self.input = inp
         else:
             raise IOError("Invalid input type (%s) for %s" % (type(inp), inp))
         return
 
-    def readline(self, use_raw=None, prompt=''):
+    def readline(self, use_raw=None, prompt=""):
         """Read a line of input. EOFError will be raised on EOF.
 
         Note that we don't support prompting"""
-        if self.closed: raise ValueError
+        if self.closed:
+            raise ValueError
         if 0 == len(self.input):
             self.closed = True
             raise EOFError
         line = self.input[0]
         del self.input[0]
         return line
+
     pass
 
 
 class StringArrayOutput(Mbase.DebuggerInOutBase):
     """Simulate I/O using an array of strings. Sort of like StringIO, but
-    even simplier. """
+    even simpler."""
 
     def __init__(self, out=[], opts=None):
         self.flush_after_write = False  # For compatibility
         self.closed = False
         self.output = out
         return
 
     def close(self):
-        'Nothing to do here. Interface is for compatibility'
+        "Nothing to do here. Interface is for compatibility"
         self.closed = True
         return
 
     def flush(self):
-        'Nothing to do here. Interface is for compatibility'
+        "Nothing to do here. Interface is for compatibility"
         return
 
     def open(self, output):
         """Use this to set where to write to. output can be a
         file object or a string. This code raises IOError on error.
 
         If another file was previously open upon calling this open,
         that will be stacked and will come back into use after
         a close_write().
         """
         if isinstance(output, types.Listype):
             self.output = output
         else:
-            raise IOError("Invalid output type (%s) for %s" % (type(output),
-                                                                 output))
+            raise IOError("Invalid output type (%s) for %s" % (type(output), output))
         return
 
     def write(self, msg):
-        """ This method the debugger uses to write. In contrast to
+        """This method the debugger uses to write. In contrast to
         writeline, no newline is added to the end to `str'.
         """
-        if self.closed: raise ValueError
+        if self.closed:
+            raise ValueError
         if [] == self.output:
             self.output = [msg]
         else:
             self.output[-1] += msg
             pass
         return
 
     def writeline(self, msg):
-        """ used to write to a debugger that is connected to this
+        """used to write to a debugger that is connected to this
         server; Here, we use the null string '' as an indicator of a
         newline.
         """
         self.write(msg)
-        self.output.append('')
+        self.output.append("")
         return
 
     pass
 
+
 # Demo
-if __name__=='__main__':
-    inp= StringArrayInput(['Now is the time', 'for all good men'])
+if __name__ == "__main__":
+    inp = StringArrayInput(["Now is the time", "for all good men"])
     line = inp.readline()
     print(line)
     line = inp.readline()
     print(line)
     try:
         line = inp.readline()
     except EOFError:
-        print('EOF hit on read')
+        print("EOF hit on read")
         pass
     out = StringArrayOutput()
     print(out.output)
-#    line = io.readline("Type some more characters: ")
+    #    line = io.readline("Type some more characters: ")
     out.writeline("Hello, world!")
     print(out.output)
     out.write("Hello")
     print(out.output)
     out.writeline(", again.")
     print(out.output)
-#     io.open_write(sys.stdout)
+    #     io.open_write(sys.stdout)
     out.flush_after_write = True
     out.write("Last hello")
     out.close()
     print(out.output)
     try:
         out.writeline("You won't see me")
-    except:
+    except Exception:
         pass
     # Closing after already closed is okay
     out.close()
     inp.close()
     pass
```

### Comparing `trepan3k-1.2.8/trepan/inout/tcpclient.py` & `trepan3k-1.2.9/trepan/inout/tcpclient.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,107 +22,106 @@
 from trepan.inout.base import DebuggerInOutBase
 from trepan.misc import option_set
 
 
 class TCPClient(DebuggerInOutBase):
     """Debugger Client Input/Output Socket."""
 
-    DEFAULT_INIT_OPTS = {'open': True}
+    DEFAULT_INIT_OPTS = {"open": True}
 
     def __init__(self, inout=None, opts=None):
-        get_option = lambda key: option_set(opts, key,
-                                            Mdefault.CLIENT_SOCKET_OPTS)
+        get_option = lambda key: option_set(opts, key, Mdefault.CLIENT_SOCKET_OPTS)
         self.inout = None
         self.addr = None
-        self.buf = ''
+        self.buf = ""
         self.line_edit = False  # Our name for GNU readline capability
-        self.state = 'disconnected'
+        self.state = "disconnected"
         if inout:
             self.inout = inout
-        elif get_option('open'):
+        elif get_option("open"):
             self.open(opts)
             pass
         return
 
     def close(self):
-        """ Closes both input and output """
+        """Closes both input and output"""
         if self.inout:
             self.inout.close()
             pass
-        self.state = 'disconnnected'
+        self.state = "disconnnected"
         return
 
     def open(self, opts=None):
 
-        get_option = lambda key: option_set(opts, key,
-                                            Mdefault.CLIENT_SOCKET_OPTS)
+        get_option = lambda key: option_set(opts, key, Mdefault.CLIENT_SOCKET_OPTS)
 
-        HOST = get_option('HOST')
-        PORT = get_option('PORT')
+        HOST = get_option("HOST")
+        PORT = get_option("PORT")
         self.inout = None
-        for res in socket.getaddrinfo(HOST, PORT, socket.AF_UNSPEC,
-                                      socket.SOCK_STREAM):
+        for res in socket.getaddrinfo(HOST, PORT, socket.AF_UNSPEC, socket.SOCK_STREAM):
             af, socktype, proto, canonname, sa = res
             try:
                 self.inout = socket.socket(af, socktype, proto)
-                self.state = 'connected'
+                self.state = "connected"
             except socket.error:
                 self.inout = None
-                self.state = 'disconnected'
+                self.state = "disconnected"
                 continue
             try:
                 self.inout.connect(sa)
             except socket.error:
                 self.inout.close()
                 self.inout = None
                 continue
                 break
         if self.inout is None:
-            raise IOError('could not open client socket on port %s' %
-                          PORT)
+            raise IOError("could not open client socket on port %s" % PORT)
         return
 
     def read_msg(self):
         """Read one message unit. It's possible however that
         more than one message will be set in a receive, so we will
         have to buffer that for the next read.
         EOFError will be raised on EOF.
         """
-        if self.state == 'connected':
+        if self.state == "connected":
             if 0 == len(self.buf):
                 self.buf = self.inout.recv(Mtcpfns.TCP_MAX_PACKET)
                 if 0 == (self.buf):
-                    self.state = 'disconnected'
+                    self.state = "disconnected"
                     raise EOFError
                 pass
             self.buf, data = Mtcpfns.unpack_msg(self.buf)
-            return data.decode('utf-8')
+            return data.decode("utf-8")
         else:
             raise IOError("read_msg called in state: %s." % self.state)
 
     def write(self, msg):
-        """ This method the debugger uses to write a message unit."""
+        """This method the debugger uses to write a message unit."""
         # FIXME: do we have to check the size of msg and split output?
         return self.inout.send(Mtcpfns.pack_msg(msg))
 
     pass
 
+
 # Demo
-if __name__=='__main__':
-    inout = TCPClient(opts={'open': False})
+if __name__ == "__main__":
+    inout = TCPClient(opts={"open": False})
     import sys
+
     if len(sys.argv) > 1:
-        print('Connecting...', end=' ')
+        print("Connecting...", end=" ")
         inout.open()
-        print('connected.')
+        print("connected.")
         while True:
-            line = input('nu? ')
-            if len(line) == 0: break
+            line = input("nu? ")
+            if len(line) == 0:
+                break
             try:
                 line = inout.writeline(line)
-                print("Got: ", inout.read_msg().rstrip('\n'))
+                print("Got: ", inout.read_msg().rstrip("\n"))
             except EOFError:
                 break
             pass
         pass
     inout.close()
     pass
```

### Comparing `trepan3k-1.2.8/trepan/inout/tcpfns.py` & `trepan3k-1.2.9/trepan/inout/tcpfns.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/trepan/inout/tcpserver.py` & `trepan3k-1.2.9/trepan/inout/tcpserver.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,98 +23,104 @@
 from trepan.inout.base import DebuggerInOutBase
 
 
 # FIXME: Consider using Python's socketserver/SocketServer?
 class TCPServer(DebuggerInOutBase):
     """Debugger Server Input/Output Socket."""
 
-    DEFAULT_INIT_OPTS = {'open': True, 'socket': None}
+    DEFAULT_INIT_OPTS = {"open": True, "socket": None}
 
     def __init__(self, inout=None, opts=None):
-        get_option = lambda key: Mmisc.option_set(opts, key,
-                                                  self.DEFAULT_INIT_OPTS)
+        get_option = lambda key: Mmisc.option_set(opts, key, self.DEFAULT_INIT_OPTS)
 
         self.inout = None
         self.conn = None
         self.addr = None
-        self.remote_addr = ''
-        self.buf = ''    # Read buffer
+        self.remote_addr = ""
+        self.buf = ""  # Read buffer
         self.line_edit = False  # Our name for GNU readline capability
-        self.state = 'disconnected'
+        self.state = "disconnected"
         self.PORT = None
         self.HOST = None
         if inout:
             self.inout = inout
-        if get_option('socket'):
-            self.inout = opts['socket']
+        if get_option("socket"):
+            self.inout = opts["socket"]
             self.inout.listen(1)
-            self.state = 'listening'
-        elif get_option('open'):
+            self.state = "listening"
+        elif get_option("open"):
             self.open(opts)
             pass
         return
 
     def close(self):
-        """ Closes both socket and server connection. """
-        self.state = 'closing'
+        """Closes both socket and server connection."""
+        self.state = "closing"
         if self.inout:
             self.inout.close()
             pass
-        self.state = 'closing connection'
+        self.state = "closing connection"
         if self.conn:
             self.conn.close()
-        self.state = 'disconnected'
+        self.state = "disconnected"
         return
 
     def open(self, opts=None):
-        get_option = lambda key: Mmisc.option_set(opts, key,
-                                                  Mdefault.SERVER_SOCKET_OPTS)
-
-        self.HOST  = get_option('HOST')
-        self.PORT  = get_option('PORT')
-        self.reuse = get_option('reuse')
-        self.search_limit = get_option('search_limit')
+        get_option = lambda key: Mmisc.option_set(
+            opts, key, Mdefault.SERVER_SOCKET_OPTS
+        )
+
+        self.HOST = get_option("HOST")
+        self.PORT = get_option("PORT")
+        self.reuse = get_option("reuse")
+        self.search_limit = get_option("search_limit")
         self.inout = None
 
         this_port = self.PORT - 1
         for i in range(self.search_limit):
             this_port += 1
-            for res in socket.getaddrinfo(self.HOST, this_port, socket.AF_UNSPEC,
-                                          socket.SOCK_STREAM, 0,
-                                          socket.AI_PASSIVE):
+            for res in socket.getaddrinfo(
+                self.HOST,
+                this_port,
+                socket.AF_UNSPEC,
+                socket.SOCK_STREAM,
+                0,
+                socket.AI_PASSIVE,
+            ):
                 af, socktype, proto, canonname, sa = res
                 try:
                     self.inout = socket.socket(af, socktype, proto)
                 except socket.error:
                     self.inout = None
                     continue
                 try:
-                    if get_option('reuse'):
+                    if get_option("reuse"):
                         # The following socket option allows the OS to reclaim
                         # The address faster on termination.
-                        self.inout.setsockopt(socket.SOL_SOCKET,
-                                              socket.SO_REUSEADDR, 1)
+                        self.inout.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
                         pass
                     self.inout.bind(sa)
                     self.inout.listen(1)
-                    self.state = 'listening'
+                    self.state = "listening"
                     break
                 except socket.error as exc:
                     if exc.errno in [errno.EADDRINUSE, errno.EINVAL]:
                         self.inout.close()
                         self.inout = None
                         continue
                     raise
                 pass
-            if self.state == 'listening':
+            if self.state == "listening":
                 break
         if self.inout is None:
-            raise IOError('could not open server socket after trying ports '
-                          '%s..%s' % (self.PORT, this_port))
+            raise IOError(
+                "could not open server socket after trying ports "
+                "%s..%s" % (self.PORT, this_port)
+            )
         self.PORT = this_port
         return
 
     def read(self):
         if len(self.buf) == 0:
             self.read_msg()
             pass
@@ -122,61 +128,62 @@
 
     def read_msg(self):
         """Read one message unit. It's possible however that
         more than one message will be set in a receive, so we will
         have to buffer that for the next read.
         EOFError will be raised on EOF.
         """
-        if self.state != 'connected':
+        if self.state != "connected":
             self.wait_for_connect()
             pass
-        if self.state == 'connected':
+        if self.state == "connected":
             if 0 == len(self.buf):
                 self.buf = self.conn.recv(Mtcpfns.TCP_MAX_PACKET)
                 if 0 == len(self.buf):
-                    self.state = 'disconnected'
+                    self.state = "disconnected"
                     raise EOFError
                 pass
             self.buf, data = Mtcpfns.unpack_msg(self.buf)
-            return data.decode('utf-8')
+            return data.decode("utf-8")
         else:
             raise IOError("read_msg called in state: %s." % self.state)
 
     def wait_for_connect(self):
         self.conn, self.addr = self.inout.accept()
-        self.remote_addr = ':'.join(str(v) for v in self.addr)
-        self.state = 'connected'
+        self.remote_addr = ":".join(str(v) for v in self.addr)
+        self.state = "connected"
         return
 
     def write(self, msg):
-        """ This method the debugger uses to write. In contrast to
+        """This method the debugger uses to write. In contrast to
         writeline, no newline is added to the end to `str'. Also
         msg doesn't have to be a string.
         """
-        if self.state != 'connected':
+        if self.state != "connected":
             self.wait_for_connect()
             pass
         buffer = Mtcpfns.pack_msg(msg)
         while len(buffer) > Mtcpfns.TCP_MAX_PACKET:
-            self.conn.send(buffer[:Mtcpfns.TCP_MAX_PACKET])
-            buffer = buffer[Mtcpfns.TCP_MAX_PACKET:]
+            self.conn.send(buffer[: Mtcpfns.TCP_MAX_PACKET])
+            buffer = buffer[Mtcpfns.TCP_MAX_PACKET :]
         return self.conn.send(buffer)
 
+
 # Demo
-if __name__=='__main__':
-    inout = TCPServer(opts={'open': False})
+if __name__ == "__main__":
+    inout = TCPServer(opts={"open": False})
     import sys
+
     if len(sys.argv) > 1:
         inout.open()
-        print('Listening for connection on %s:%s' %
-              (inout.HOST, inout.PORT))
+        print("Listening for connection on %s:%s" % (inout.HOST, inout.PORT))
         while True:
             try:
-                line = inout.read_msg().rstrip('\n')
+                line = inout.read_msg().rstrip("\n")
                 print(line)
-                inout.writeline('ack: ' + line)
+                inout.writeline("ack: " + line)
             except EOFError:
                 break
             pass
         pass
     inout.close()
     pass
```

### Comparing `trepan3k-1.2.8/trepan/interface.py` & `trepan3k-1.2.9/trepan/interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2010, 2013, 2015, 2018 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2010, 2013, 2015, 2018, 2023 Rocky Bernstein
+#   <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -13,64 +15,64 @@
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """A base class for a debugger interface."""
 
 import sys
 
-NotImplementedMessage = "This method must be overriden in a subclass"
+NotImplementedMessage = "This method must be overridden in a subclass"
+
+__all__ = ["TrepanInterface"]
 
-__all__ = ['TrepanInterface']
 
 class TrepanInterface:
     """
-A debugger interface handles the communication or interaction with between
-the program and the outside portion which could be
-    - a user,
-    - a front-end that talks to a user, or
-    - another interface in another process or computer
+    A debugger interface handles the communication or interaction with between
+    the program and the outside portion which could be
+        - a user,
+        - a front-end that talks to a user, or
+        - another interface in another process or computer
     """
 
     def __init__(self, inp=None, out=None):
-        self.input  = inp or sys.stdin
+        self.input = inp or sys.stdin
         self.output = out or sys.stdout
         self.interactive = False
         return
 
     def close(self):
-        """ Closes all input and/or output """
+        """Closes all input and/or output"""
         raise NotImplementedError(NotImplementedMessage)
         return
 
     def confirm(self, prompt, default):
-        """ Called when a dangerous action is about to be done to make sure
+        """Called when a dangerous action is about to be done to make sure
         it's okay. `prompt' is printed; user response is returned."""
         raise NotImplementedError(NotImplementedMessage)
 
     def errmsg(self, str, prefix="** "):
-        """Common routine for reporting debugger error messages.
-           """
+        """Common routine for reporting debugger error messages."""
         raise NotImplementedError(NotImplementedMessage)
 
     def finalize(self, last_wishes=None):
         raise NotImplementedError(NotImplementedMessage)
 
     def msg(self, msg):
-        """ used to write to a debugger that is connected to this
+        """used to write to a debugger that is connected to this
         server; `str' written will have a newline added to it
         """
-        if hasattr(self.output, 'writeline'):
+        if hasattr(self.output, "writeline"):
             self.output.writeline(msg)
-        elif hasattr(self.output, 'writelines'):
+        elif hasattr(self.output, "writelines"):
             self.output.writelines(msg + "\n")
             pass
         return
 
     def msg_nocr(self, msg):
-        """ used to write to a debugger that is connected to this
+        """used to write to a debugger that is connected to this
         server; `str' written will not have a newline added to it
         """
         self.output.write(msg)
         return
 
     def read_command(self, prompt):
         raise NotImplementedError(NotImplementedMessage)
```

### Comparing `trepan3k-1.2.8/trepan/interfaces/__init__.py` & `trepan3k-1.2.9/trepan/interfaces/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """ Copyright (C) 2008, 2013-2014, 2016 Rocky Bernstein <rocky@gnu.org> """
-__package__ = 'trepan.interfaces'
-__docformat__ = 'restructuredtext'
+__package__ = "trepan.interfaces"
+__docformat__ = "restructuredtext"
```

### Comparing `trepan3k-1.2.8/trepan/interfaces/bullwinkle.py` & `trepan3k-1.2.9/trepan/interfaces/bullwinkle.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2013-2015 Rocky Bernstein <rocky@gnu.org>
+#   Copyright (C) 2013-2015, 2023 Rocky Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -11,71 +11,74 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Interface when communicating with the user in the same process as
     the debugged program."""
-import atexit, pprint
+import atexit
+import pprint
 
 # Our local modules
 from trepan import interface as Minterface
 from trepan.inout import input as Minput, output as Moutput
 
 
 class BWInterface(Minterface.TrepanInterface):
     """Interface when communicating with the user in the same
     process as the debugged program."""
 
     def __init__(self, inp=None, out=None, opts=None):
         atexit.register(self.finalize)
-        self.input       = inp or Minput.DebuggerUserInput()
-        self.output      = out or Moutput.DebuggerUserOutput()
-        self.pp          = pprint.PrettyPrinter()
+        self.input = inp or Minput.DebuggerUserInput()
+        self.output = out or Moutput.DebuggerUserOutput()
+        self.pp = pprint.PrettyPrinter()
         return
 
     def close(self):
-        """ Closes both input and output """
+        """Closes both input and output"""
         self.input.close()
         self.output.close()
         return
 
     def errmsg(self, msg):
-        """Common routine for reporting debugger error messages.
-           """
+        """Common routine for reporting debugger error messages."""
         return self.msg(msg)
 
     def finalize(self, last_wishes=None):
         # print exit annotation
         # save history
         self.close()
         return
 
     def msg(self, msg):
         self.output.write(self.pp.pformat(msg) + "\n")
         return
 
     def read_command(self):
-        line = self.readline('Bullwinkle read: ')
+        line = self.readline("Bullwinkle read: ")
         try:
             command = eval(line)
         except:
             return "eval error"
         pass
         return command
 
-    def readline(self, prompt=''):
+    def readline(self, prompt=""):
         return self.input.readline(prompt=prompt)
+
     pass
 
+
 # Demo
-if __name__=='__main__':
+if __name__ == "__main__":
     intf = BWInterface()
     intf.msg("Testing1, 2, 3")
     import sys
+
     if len(sys.argv) > 1:
         try:
             entry = intf.read_command()
         except EOFError:
             print("No input EOF: ")
         else:
             intf.msg(entry)
```

### Comparing `trepan3k-1.2.8/trepan/interfaces/client.py` & `trepan3k-1.2.9/trepan/interfaces/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,82 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2013-2014, 2017 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2009, 2013-2014, 2017, 2023 Rocky Bernstein
+#   <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Module for client (i.e. user to communication-device) interaction.
-The debugged program is at the other end of the communcation."""
+The debugged program is at the other end of the communication."""
+
+from trepan.inout import fifoclient as Mfifoclient, tcpclient as Mtcpclient
 
 # Our local modules
 from trepan.interfaces import user as Muser
-from trepan.inout import tcpclient as Mtcpclient, fifoclient as Mfifoclient
 
+DEFAULT_INIT_CONNECTION_OPTS = {"IO": "TCP"}
 
-DEFAULT_INIT_CONNECTION_OPTS = {'IO': 'TCP'}
 
 class ClientInterface(Muser.UserInterface):
     """Interface for a user which is attached to a debugged process
     via some sort of communication medium (e.g. socket, tty, FIFOs).
     This could be on the same computer in a different process or on
     a remote computer."""
 
-    def __init__(self, inp=None, out=None, inout=None, user_opts={},
-                 connection_opts={}):
+    def __init__(
+        self, inp=None, out=None, inout=None, user_opts={}, connection_opts={}
+    ):
 
         opts = DEFAULT_INIT_CONNECTION_OPTS.copy()
         opts.update(connection_opts)
 
         Muser.UserInterface.__init__(self, inp, out, user_opts)
 
         self.inout = None  # initialize in case assignment below fails
         if inout:
             self.inout = inout
         else:
-            self.server_type = opts['IO']
-            if 'FIFO' == self.server_type:
+            self.server_type = opts["IO"]
+            if "FIFO" == self.server_type:
                 self.inout = Mfifoclient.FIFOClient(opts=opts)
-            elif 'TCP' == self.server_type:
+            elif "TCP" == self.server_type:
                 self.inout = Mtcpclient.TCPClient(opts=opts)
             else:
-                self.errmsg("Expecting server type TCP or FIFO. Got: %s." %
-                            self.server_type)
+                self.errmsg(
+                    "Expecting server type TCP or FIFO. Got: %s." % self.server_type
+                )
                 return
             pass
         return
 
     def read_remote(self):
-        '''Send a message back to the server (in contrast to
-        the local user output channel).'''
+        """Send a message back to the server (in contrast to
+        the local user output channel)."""
         coded_line = self.inout.read_msg()
         if isinstance(coded_line, bytes):
             coded_line = coded_line.decode("utf-8")
         control = coded_line[0]
         remote_line = coded_line[1:]
         return (control, remote_line)
 
     def write_remote(self, code, msg):
-        '''Send a message back to the server (in contrast to
-        the local user output channel).'''
+        """Send a message back to the server (in contrast to
+        the local user output channel)."""
         # FIXME change into write_xxx
         return self.inout.writeline(code + msg)
+
     pass
 
+
 # Demo
-if __name__=='__main__':
+if __name__ == "__main__":
     intf = ClientInterface()
```

### Comparing `trepan3k-1.2.8/trepan/interfaces/comcodes.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/source.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2008, 2009, 2013 Rocky Bernstein <rocky@gnu.org>
+#   Copyright (C) 2008-2009, 2013, 2015 Rocky Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
-""" Communication status codes"""
-PRINT         = '.'
-COMMAND       = 'C'   # read a command
-CONFIRM_TRUE  = 'Y'
-CONFIRM_FALSE = 'N'
-CONFIRM_REPLY = '?'
-QUIT          = 'q'
-PROMPT        = 'p'
-SYNC          = 's'   # Resynchronize communication
-RESTART       = 'r'
+
+# Our local modules
+from trepan.processor.command import base_subcmd as Mbase_subcmd
+
+
+class InfoSource(Mbase_subcmd.DebuggerSubcommand):
+    """Information about the current Python file."""
+
+    min_abbrev = 1
+    need_stack = True
+    short_help = "Information about the current Python file"
+
+    def run(self, args):
+        if not self.proc.curframe:
+            self.errmsg("No current source file.")
+            return
+        filename = self.core.canonic_filename(self.proc.curframe)
+        self.msg("Current Python file is %s" % self.core.filename(filename))
+        return False
+
+    pass
```

### Comparing `trepan3k-1.2.8/trepan/interfaces/script.py` & `trepan3k-1.2.9/trepan/interfaces/script.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,96 +14,94 @@
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Module for reading debugger scripts"""
 import atexit
 
 # Our local modules
 from trepan import interface as Minterface, misc as Mmisc
-from trepan.inout import scriptin as Mscriptin, output as Moutput
+from trepan.inout import output as Moutput, scriptin as Mscriptin
+
 
 class ScriptInterface(Minterface.TrepanInterface):
     """Interface when reading debugger scripts"""
 
-    DEFAULT_INIT_OPTS = {
-        'abort_on_error' : True,
-        'confirm_val'    : False,
-        'verbose'        : False
-        }
+    DEFAULT_INIT_OPTS = {"abort_on_error": True, "confirm_val": False, "verbose": False}
 
     def __init__(self, script_name, out=None, opts=None):
-        get_option = lambda key: Mmisc.option_set(opts, key,
-                                                  self.DEFAULT_INIT_OPTS)
+        get_option = lambda key: Mmisc.option_set(opts, key, self.DEFAULT_INIT_OPTS)
 
         atexit.register(self.finalize)
-        self.script_name     = script_name
-        self.histfile        = None
-        self.input_lineno    = 0
-        self.input           = Mscriptin.ScriptInput(script_name)
-        self.interactive     = False
-        self.output          = out or Moutput.DebuggerUserOutput()
-
-        self.abort_on_error  = get_option('abort_on_error')
-        self.default_confirm = get_option('confirm_val')
-        self.verbose         = get_option('verbose')
+        self.script_name = script_name
+        self.histfile = None
+        self.input_lineno = 0
+        self.input = Mscriptin.ScriptInput(script_name)
+        self.interactive = False
+        self.output = out or Moutput.DebuggerUserOutput()
+
+        self.abort_on_error = get_option("abort_on_error")
+        self.default_confirm = get_option("confirm_val")
+        self.verbose = get_option("verbose")
 
         return
 
     def close(self):
-        """ Closes input. (We don't have an output.)"""
+        """Closes input. (We don't have an output.)"""
         self.input.close()
         return
 
     # Could look also look for interactive input and
     # use that. For now, though we'll simplify.
     def confirm(self, prompt, default):
-        """ Called when a dangerous action is about to be done, to make
-        sure it's okay. """
+        """Called when a dangerous action is about to be done, to make
+        sure it's okay."""
         return self.default_confirm
 
     def errmsg(self, msg, prefix="** "):
-        """Common routine for reporting debugger error messages.
-           """
+        """Common routine for reporting debugger error messages."""
         #  self.verbose shows lines so we don't have to duplicate info
         #  here. Perhaps there should be a 'terse' mode to never show
         #  position info.
         if not self.verbose:
-            location = ("%s:%s: Error in source command file"
-                        % (self.script_name, self.input_lineno))
-            msg = "%s%s:\n%s%s" %(prefix, location, prefix, msg)
+            location = "%s:%s: Error in source command file" % (
+                self.script_name,
+                self.input_lineno,
+            )
+            msg = "%s%s:\n%s%s" % (prefix, location, prefix, msg)
         else:
-            msg = "%s%s" %(prefix, msg)
+            msg = "%s%s" % (prefix, msg)
             pass
         self.msg(msg)
         if self.abort_on_error:
             raise EOFError
         return
 
     def finalize(self, last_wishes=None):
         # print exit annotation
         # save history
         self.close()
         return
 
-    def read_command(self, prompt=''):
-        '''Script interface to read a command. `prompt' is a parameter for
-        compatibilty and is ignored.'''
+    def read_command(self, prompt=""):
+        """Script interface to read a command. `prompt' is a parameter for
+        compatibility and is ignored."""
         self.input_lineno += 1
         line = self.readline()
         if self.verbose:
             location = "%s line %s" % (self.script_name, self.input_lineno)
-            self.msg('+ %s: %s' % (location, line))
+            self.msg("+ %s: %s" % (location, line))
             pass
         # Do something with history?
         return line
 
     # Could decide make this look for interactive input?
-    def readline(self, prompt=''):
-        '''Script interface to read a line. `prompt' is a parameter for
-        compatibilty and is ignored.'''
+    def readline(self, prompt=""):
+        """Script interface to read a line. `prompt' is a parameter for
+        compatibility and is ignored."""
         return self.input.readline()
 
+
 # Demo
-if __name__=='__main__':
-    intf = ScriptInterface('script.py')
+if __name__ == "__main__":
+    intf = ScriptInterface("script.py")
     line = intf.readline()
     print("Line read: %s" % line)
     pass
```

### Comparing `trepan3k-1.2.8/trepan/interfaces/server.py` & `trepan3k-1.2.9/trepan/interfaces/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Module for Server (i.e. program to communication-device) interaction"""
 import atexit
 
 # Our local modules
 from trepan import interface as Minterface
-from trepan.inout import tcpserver as Mtcpserver, fifoserver as Mfifoserver
+from trepan.inout import fifoserver as Mfifoserver, tcpserver as Mtcpserver
 from trepan.interfaces import comcodes as Mcomcodes
 
-DEFAULT_INIT_CONNECTION_OPTS = {'IO': 'TCP',
-                                'PORT': 1955}
+DEFAULT_INIT_CONNECTION_OPTS = {"IO": "TCP", "PORT": 1955}
+
 
 class ServerInterface(Minterface.TrepanInterface):
     """Interface for debugging a program but having user control
     reside outside of the debugged process, possibly on another
     computer."""
 
     def __init__(self, inout=None, out=None, connection_opts={}):
@@ -34,82 +34,81 @@
 
         opts = DEFAULT_INIT_CONNECTION_OPTS.copy()
         opts.update(connection_opts)
         self.inout = None  # initialize in case assignment below fails
         if inout:
             self.inout = inout
         else:
-            self.server_type = opts['IO']
-            if 'FIFO' == self.server_type:
+            self.server_type = opts["IO"]
+            if "FIFO" == self.server_type:
                 self.inout = Mfifoserver.FIFOServer()
             else:
                 self.inout = Mtcpserver.TCPServer(opts=opts)
                 pass
             pass
-        # For Compatability
+        # For Compatibility
         self.output = self.inout
-        self.input  = self.inout
+        self.input = self.inout
         self.interactive = True  # Or at least so we think initially
         self.histfile = None
         return
 
     def close(self):
-        """ Closes both input and output """
+        """Closes both input and output"""
         if self.inout:
             self.inout.close()
         return
 
     def confirm(self, prompt, default):
-        """ Called when a dangerous action is about to be done to make sure
+        """Called when a dangerous action is about to be done to make sure
         it's okay. `prompt' is printed; user response is returned."""
         while True:
             try:
                 self.write_confirm(prompt, default)
-                reply = self.readline('').strip().lower()
+                reply = self.readline("").strip().lower()
             except EOFError:
                 return default
-            if reply in ('y', 'yes'):
+            if reply in ("y", "yes"):
                 return True
-            elif reply in ('n', 'no'):
+            elif reply in ("n", "no"):
                 return False
             else:
                 self.msg("Please answer y or n.")
                 pass
             pass
         return default
 
     def errmsg(self, str, prefix="** "):
-        """Common routine for reporting debugger error messages.
-           """
-        return self.msg("%s%s" %(prefix, str))
+        """Common routine for reporting debugger error messages."""
+        return self.msg("%s%s" % (prefix, str))
 
     def finalize(self, last_wishes=Mcomcodes.QUIT):
         # print exit annotation
         if self.is_connected():
             self.inout.writeline(last_wishes)
             pass
         self.close()
         return
 
     def is_connected(self):
-        """ Return True if we are connected """
-        return self.inout and 'connected' == self.inout.state
+        """Return True if we are connected"""
+        return self.inout and "connected" == self.inout.state
 
     def msg(self, msg):
-        """ used to write to a debugger that is connected to this
+        """used to write to a debugger that is connected to this
         server; `str' written will have a newline added to it
         """
         self.inout.writeline(Mcomcodes.PRINT + msg)
         return
 
     def msg_nocr(self, msg):
-        """ used to write to a debugger that is connected to this
+        """used to write to a debugger that is connected to this
         server; `str' written will not have a newline added to it
         """
-        self.inout.write(Mcomcodes.PRINT +  msg)
+        self.inout.write(Mcomcodes.PRINT + msg)
         return
 
     def read_command(self, prompt):
         return self.readline(prompt)
 
     def read_data(self):
         return self.inout.read_data()
@@ -119,15 +118,15 @@
             self.write_prompt(prompt)
             pass
         coded_line = self.inout.read_msg()
         self.read_ctrl = coded_line[0]
         return coded_line[1:]
 
     def state(self):
-        """ Return connected """
+        """Return connected"""
         return self.inout.state
 
     def write_prompt(self, prompt):
         return self.inout.writeline(Mcomcodes.PROMPT + prompt)
 
     def write_confirm(self, prompt, default):
         if default:
@@ -135,12 +134,13 @@
         else:
             code = Mcomcodes.CONFIRM_FALSE
             pass
         return self.inout.writeline(code + prompt)
 
     pass
 
+
 # Demo
-if __name__=='__main__':
-    connection_opts={'IO': 'TCP', 'PORT': 1954}
+if __name__ == "__main__":
+    connection_opts = {"IO": "TCP", "PORT": 1954}
     intf = ServerInterface(connection_opts=connection_opts)
     pass
```

### Comparing `trepan3k-1.2.8/trepan/interfaces/user.py` & `trepan3k-1.2.9/trepan/interfaces/user.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
+#
 #   Copyright (C) 2009-2010, 2013-2015,
-#   2017-2018, 2020 Rocky Bernstein <rocky@gnu.org>
+#   2017-2018, 2020, 2023 Rocky Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -12,40 +13,45 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Interface when communicating with the user in the same process as
     the debugged program."""
-import atexit, os.path as osp
+import atexit
+import os.path as osp
 
 # Our local modules
 from trepan.interface import TrepanInterface
 
 histfile = osp.expanduser("~/.trepan3k_hist")
 # is_pypy = '__pypy__' in sys.builtin_module_names
 
 DEFAULT_USER_SETTINGS = {
     "histfile": histfile,  # Where do we save the history?
     "complete": None,  # Function which handles tab completion, or None
 }
 
 try:
-    from readline import read_history_file, set_completer, set_history_length
-    from readline import write_history_file, parse_and_bind
+    from readline import (
+        parse_and_bind,
+        read_history_file,
+        set_completer,
+        set_history_length,
+        write_history_file,
+    )
 except ImportError:
     pass
 
 
 class UserInterface(TrepanInterface):
     """Interface when communicating with the user in the same
     process as the debugged program."""
 
     def __init__(self, inp=None, out=None, opts={}):
-
         user_opts = DEFAULT_USER_SETTINGS.copy()
         user_opts.update(opts)
 
         from trepan.inout import input as Minput, output as Moutput
 
         atexit.register(self.finalize)
         self.interactive = True  # Or at least so we think initially
@@ -61,34 +67,34 @@
                 pass
             self.histfile = user_opts["histfile"]
             if self.histfile:
                 try:
                     read_history_file(histfile)
                 except IOError:
                     pass
-                except:
+                except Exception:
                     # PyPy read_history_file fails
                     return
                 set_history_length(50)
                 atexit.register(self.user_write_history_file)
                 pass
         return
 
     def user_write_history_file(self):
         try:
             write_history_file(self.histfile)
-        except:
+        except Exception:
             pass
 
     def close(self):
-        """ Closes both input and output """
+        """Closes both input and output"""
         try:
             self.input.close()
             self.output.close()
-        except:
+        except Exception:
             pass
         return
 
     def confirm(self, prompt, default):
         """Called when a dangerous action is about to be done, to make
         sure it's okay. Expect a yes/no answer to `prompt' which is printed,
         suffixed with a question mark and the default value.  The user
@@ -131,15 +137,15 @@
         return self.msg("%s%s" % (prefix, msg))
 
     def finalize(self, last_wishes=None):
         # This routine gets called multiple times.
         # We hard-code the close() function here.
         try:
             self.msg("%s: That's all, folks..." % self.debugger_name)
-        except:
+        except Exception:
             pass
         else:
             self.close()
             pass
         return
 
     def read_command(self, prompt=""):
```

### Comparing `trepan3k-1.2.8/trepan/lib/__init__.py` & `trepan3k-1.2.9/trepan/lib/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,12 +9,13 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """ Copyright (C) 2008, 2009, 2013, 2015 Rocky Bernstein <rocky@gnu.org> """
 
-__docformat__ = 'restructuredtext'
+__docformat__ = "restructuredtext"
 
 from trepan.misc import pyfiles
+
 __all__ = pyfiles(__file__)
-__package__ = 'trepan.lib'
+__package__ = "trepan.lib"
```

### Comparing `trepan3k-1.2.8/trepan/lib/breakpoint.py` & `trepan3k-1.2.9/trepan/lib/breakpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,48 +14,52 @@
 
     Breakpoints are indexed by number in the `bpbynumber' list, and
     through a (file,line) tuple which is a key in the `bplist'
     dictionary. If the breakpoint is a function it is in `fnlist' as
     well.  Note there may be more than one breakpoint per line which
     may have different conditions associated with them.
     """
+
     def __init__(self):
         self.reset()
         return
 
     def bpnumbers(self):
-        '''Returns a list of strings of breakpoint numbers'''
-        return ["%d" % bp.number for bp in self.bpbynumber if
-                bp is not None]
+        """Returns a list of strings of breakpoint numbers"""
+        return ["%d" % bp.number for bp in self.bpbynumber if bp is not None]
 
     def get_breakpoint(self, i):
         if isinstance(i, str):
             try:
                 i = int(i)
             except ValueError:
-                return(False, 'Breakpoint value %r is not a number.' % i,
-                       None)
+                return (False, "Breakpoint value %r is not a number." % i, None)
             pass
         if 1 == len(self.bpbynumber):
-            return (False, 'No breakpoints set.', None)
+            return (False, "No breakpoints set.", None)
         elif i >= len(self.bpbynumber) or i <= 0:
-            return (False, 'Breakpoint number %d out of range 1..%d.' %
-                    (i, len(self.bpbynumber)-1), None)
+            return (
+                False,
+                "Breakpoint number %d out of range 1..%d."
+                % (i, len(self.bpbynumber) - 1),
+                None,
+            )
         bp = self.bpbynumber[i]
         if bp is None:
-            return (False, 'Breakpoint %d previously deleted.' % i, None)
+            return (False, "Breakpoint %d previously deleted." % i, None)
         return (True, None, bp)
 
-    def add_breakpoint(self, filename, lineno, offset, temporary=False, condition=None,
-                       func=None):
+    def add_breakpoint(
+        self, filename, lineno, offset, temporary=False, condition=None, func=None
+    ):
 
         bpnum = len(self.bpbynumber)
-        if filename: filename  = os.path.realpath(filename)
-        brkpt = Breakpoint(bpnum, filename, lineno, temporary, condition,
-                           func, offset)
+        if filename:
+            filename = os.path.realpath(filename)
+        brkpt = Breakpoint(bpnum, filename, lineno, temporary, condition, func, offset)
         # Build the internal lists of breakpoints
         self.bpbynumber.append(brkpt)
         if (filename, lineno) in self.bplist:
             self.bplist[filename, lineno].append(brkpt)
         else:
             self.bplist[filename, lineno] = [brkpt]
             pass
@@ -71,71 +75,80 @@
         bp_list = []
         for bp in self.bpbynumber:
             if bp:
                 bp_list.append(str(bp.number))
                 self.delete_breakpoint(bp)
                 pass
         if not bp_list:
-            return 'There are no breakpoints'
+            return "There are no breakpoints"
         else:
-            return 'Deleted breakpoints %s' % ', '.join(bp_list)
+            return "Deleted breakpoints %s" % ", ".join(bp_list)
         return
 
     def delete_breakpoint(self, bp):
-        " remove breakpoint `bp'"
+        "remove breakpoint `bp'"
         bpnum = bp.number
-        self.bpbynumber[bpnum] = None   # No longer in list
+        self.bpbynumber[bpnum] = None  # No longer in list
         index = (bp.filename, bp.line)
-        if index not in self.bplist: return False
+        if index not in self.bplist:
+            return False
         self.bplist[index].remove(bp)
         if not self.bplist[index]:
             # No more breakpoints for this file:line combo
             del self.bplist[index]
         return True
 
     def delete_breakpoint_by_number(self, bpnum):
         "Remove a breakpoint given its breakpoint number."
         success, msg, bp = self.get_breakpoint(bpnum)
         if not success:
             return False, msg
         self.delete_breakpoint(bp)
-        return (True, '')
+        return (True, "")
 
-    def en_disable_all_breakpoints(self,  do_enable=True):
+    def en_disable_all_breakpoints(self, do_enable=True):
         "Enable or disable all breakpoints."
         bp_list = [bp for bp in self.bpbynumber if bp]
         bp_nums = []
         if do_enable:
-            endis = 'en'
+            endis = "en"
         else:
-            endis = 'dis'
+            endis = "dis"
             pass
         if not bp_list:
             return "No breakpoints to %sable" % endis
         for bp in bp_list:
             bp.enabled = do_enable
             bp_nums.append(str(bp.number))
             pass
-        return ("Breakpoints %sabled: %s" % (endis, ", ".join(bp_nums)))
+        return "Breakpoints %sabled: %s" % (endis, ", ".join(bp_nums))
 
     def en_disable_breakpoint_by_number(self, bpnum, do_enable=True):
         "Enable or disable a breakpoint given its breakpoint number."
         success, msg, bp = self.get_breakpoint(bpnum)
         if not success:
             return success, msg
         if do_enable:
-            endis = 'en'
+            endis = "en"
         else:
-            endis = 'dis'
+            endis = "dis"
             pass
         if bp.enabled == do_enable:
-            return (False, ('Breakpoint (%r) previously %sabled' %
-                            (str(bpnum), endis,)))
+            return (
+                False,
+                (
+                    "Breakpoint (%r) previously %sabled"
+                    % (
+                        str(bpnum),
+                        endis,
+                    )
+                ),
+            )
         bp.enabled = do_enable
-        return (True, '')
+        return (True, "")
 
     def delete_breakpoints_by_lineno(self, filename, lineno):
         """Removes all breakpoints at a give filename and line number.
         Returns a list of breakpoints numbers deleted.
         """
         if (filename, lineno) not in self.bplist:
             return []
@@ -162,55 +175,55 @@
                 continue
             # Count every hit when bp is enabled
             b.hits += 1
             if not b.condition:
                 # If unconditional, and ignoring, go on to next, else
                 # break
                 if b.ignore > 0:
-                    b.ignore = b.ignore -1
+                    b.ignore = b.ignore - 1
                     continue
                 else:
                     # breakpoint and marker that's ok to delete if
                     # temporary
                     return (b, True)
             else:
                 # Conditional bp.
                 # Ignore count applies only to those bpt hits where the
                 # condition evaluates to true.
                 try:
                     val = eval(b.condition, frame.f_globals, frame.f_locals)
                     if val:
                         if b.ignore > 0:
-                            b.ignore = b.ignore -1
+                            b.ignore = b.ignore - 1
                             # continue
                         else:
                             return (b, True)
                     # else:
                     #   continue
-                except:
+                except Exception:
                     # if eval fails, most conservative thing is to
                     # stop on breakpoint regardless of ignore count.
                     # Don't delete temporary, as another hint to user.
                     return (b, False)
                 pass
             pass
         return (None, None)
 
     def last(self):
-        return len(self.bpbynumber)-1
+        return len(self.bpbynumber) - 1
 
     def reset(self):
-        """ A list of breakpoints by breakpoint number.  Each entry is
+        """A list of breakpoints by breakpoint number.  Each entry is
         None or an instance of Breakpoint.  Index 0 is unused, except
-        for marking an effective break .... see effective(). """
+        for marking an effective break .... see effective()."""
         self.bpbynumber = [None]
 
         # A list of breakpoints indexed by (file, lineno) tuple
         self.bplist = {}
-        self.fnlist  = {}
+        self.fnlist = {}
 
         return
 
     pass  # BreakpointManager
 
 
 class Breakpoint:
@@ -220,64 +233,80 @@
     conditionals.
 
     When matching an offset, if offset is None, the offset value is not
     considered in a match. If offset is -1, we are at a "call" event;
     the first offset in bytecode is 0.
     """
 
-    def __init__(self, number, filename, line, temporary=False,
-                 condition=None, funcname=None, offset=None):
+    def __init__(
+        self,
+        number,
+        filename,
+        line,
+        temporary=False,
+        condition=None,
+        funcname=None,
+        offset=None,
+    ):
 
         self.offset = offset
         self.condition = condition
-        self.enabled   = True
+        self.enabled = True
 
-        self.filename  = filename
-        if filename: self.filename  = os.path.realpath(filename)
+        self.filename = filename
+        if filename:
+            self.filename = os.path.realpath(filename)
 
         # Needed if funcname is not None.
         self.func_first_executable_line = None
-        self.funcname  = funcname
+        self.funcname = funcname
 
         # Number of time breakpoint has been hit
-        self.hits      = 0
+        self.hits = 0
 
         # Number of times to ignore breakpoint before stopping
-        self.ignore    = 0
+        self.ignore = 0
 
-        self.line      = line
-        self.number    = number
+        self.line = line
+        self.number = number
 
         # Delete breakpoint after hitting it.
         self.temporary = temporary
         return
 
     def __str__(self):
         if self.temporary:
-            disp = 'del  '
+            disp = "del  "
         else:
-            disp = 'keep '
+            disp = "keep "
         if self.enabled:
-            disp = disp + 'yes  '
+            disp = disp + "yes  "
         else:
-            disp = disp + 'no   '
+            disp = disp + "no   "
         if self.offset is None:
             offset_str = " any"
         else:
             offset_str = "%4d" % self.offset
-        msg = '%-4dbreakpoint   %s %s at %s:%d' % (self.number, disp,
-                                                    offset_str, self.filename, self.line)
+        msg = "%-4dbreakpoint   %s %s at %s:%d" % (
+            self.number,
+            disp,
+            offset_str,
+            self.filename,
+            self.line,
+        )
         if self.condition:
-            msg += '\n\tstop only if %s' % self.condition
+            msg += "\n\tstop only if %s" % self.condition
         if self.ignore:
-            msg += msg('\n\tignore next %d hits' % self.ignore)
+            msg += msg("\n\tignore next %d hits" % self.ignore)
         if self.hits:
-            if (self.hits > 1): ss = 's'
-            else: ss = ''
-            msg +='\n\tbreakpoint already hit %d time%s' % self.hits, ss
+            if self.hits > 1:
+                ss = "s"
+            else:
+                ss = ""
+            msg += "\n\tbreakpoint already hit %d time%s" % self.hits, ss
         return msg
 
     def enable(self):
         self.enabled = True
         return self.enabled
 
     def disable(self):
@@ -286,21 +315,25 @@
 
     def icon_char(self):
         """Return a one-character "icon" giving the state of the breakpoint
         't': temporary breakpoint
         'B': enabled breakpoint
         'b': disabled breakpoint
         """
-        if self.temporary : return 't'
-        elif self.enabled:  return 'B'
-        else: return 'b'
+        if self.temporary:
+            return "t"
+        elif self.enabled:
+            return "B"
+        else:
+            return "b"
         return
 
     pass  # end of Breakpoint class
 
+
 def checkfuncname(b, frame):
     """Check whether we should break here because of `b.funcname`."""
     if not b.funcname:
         # Breakpoint was set via line number.
         if b.line != frame.f_lineno:
             # Breakpoint was set at a line with a def statement and the function
             # defined is called: don't break.
@@ -319,48 +352,57 @@
         b.func_first_executable_line = frame.f_lineno
 
     if b.func_first_executable_line != frame.f_lineno:
         # But we are not at the first line number: don't break.
         return False
     return True
 
+
 # Demo
 
-if __name__=='__main__':
+if __name__ == "__main__":
     bpmgr = BreakpointManager()
     print(bpmgr.last())
-    bp = bpmgr.add_breakpoint('foo', 0, 5)
+    bp = bpmgr.add_breakpoint("foo", 0, 5)
     print(bp.icon_char())
     print(bpmgr.last())
     print(repr(bp))
     print(str(bp))
     bp.disable()
     print(str(bp))
     for i in 10, 1:
         status, msg = bpmgr.delete_breakpoint_by_number(i)
-        print("Delete breakpoint %s: %s %s" % (i, status, msg,))
+        print(
+            "Delete breakpoint %s: %s %s"
+            % (
+                i,
+                status,
+                msg,
+            )
+        )
     import inspect
+
     frame = inspect.currentframe()
     print("Stop at bp: %s" % checkfuncname(bp, frame))
 
     def foo(bp, bpmgr):
         frame = inspect.currentframe()
         print("Stop at bp2: %s" % checkfuncname(bp, frame))
         # frame.f_lineno is constantly updated. So adjust for the
         # line difference between the add_breakpoint and the check.
-        bp3 = bpmgr.add_breakpoint('foo', 0, frame.f_lineno+1)
+        bp3 = bpmgr.add_breakpoint("foo", 0, frame.f_lineno + 1)
         print("Stop at bp3: %s" % checkfuncname(bp3, frame))
         return
 
-    bp2 = bpmgr.add_breakpoint(None, None, False, None, 'foo')
+    bp2 = bpmgr.add_breakpoint(None, None, False, None, "foo")
     foo(bp2, bpmgr)
-    bp3 = bpmgr.add_breakpoint('foo', 5, 2, temporary=True)
+    bp3 = bpmgr.add_breakpoint("foo", 5, 2, temporary=True)
     print(bp3.icon_char())
     print(bpmgr.bpnumbers())
 
-    bp = bpmgr.add_breakpoint('bar', 10, 3)
+    bp = bpmgr.add_breakpoint("bar", 10, 3)
     filename = bp.filename
     for i in range(3):
-        bp = bpmgr.add_breakpoint('bar', 2, 6)
+        bp = bpmgr.add_breakpoint("bar", 2, 6)
     print(bpmgr.delete_breakpoints_by_lineno(filename, 6))
     print(bpmgr.delete_breakpoints_by_lineno(filename, 6))
     print(bpmgr.bpnumbers())
```

### Comparing `trepan3k-1.2.8/trepan/lib/bytecode.py` & `trepan3k-1.2.9/trepan/lib/bytecode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2012-2013, 2020 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2009, 2012-2013, 2020, 2023 Rocky Bernstein
+#   <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -11,16 +13,18 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Bytecode instruction routines"""
 
-import xdis, re
-from opcode import opname, HAVE_ARGUMENT
+import re
+
+import xdis
+from opcode import HAVE_ARGUMENT, opname
 
 
 def op_at_code_loc(code, loc):
     try:
         op = code[loc]
     except IndexError:
         return "got IndexError"
@@ -61,18 +65,19 @@
             if 0 == count:
                 return linestarts[offset]
             pass
         pass
     return -1000
 
 
-def stmt_contains_opcode(co, lineno, query_opcode):
+def stmt_contains_opcode(co, lineno, query_opcode) -> bool:
     linestarts = dict(xdis.findlinestarts(co))
     code = co.co_code
     found_start = False
+    offset = 0
     for offset, start_line in list(linestarts.items()):
         if start_line == lineno:
             found_start = True
             break
         pass
     if not found_start:
         return False
```

### Comparing `trepan3k-1.2.8/trepan/lib/complete.py` & `trepan3k-1.2.9/trepan/lib/complete.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2013, 2020 Rocky Bernstein <rocky@gnu.org>
+#   Copyright (C) 2013, 2020, 2023 Rocky Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -53,15 +53,15 @@
         pass
     pass
     return sorted(result, key=lambda pair: pair[0])
 
 
 def complete_token_filtered(aliases, prefix, expanded):
     """Find all starting matches in dictionary *aliases* that start
-     with *prefix*, but filter out any matches already in *expanded*"""
+    with *prefix*, but filter out any matches already in *expanded*"""
 
     complete_ary = aliases.keys()
     return [cmd for cmd in complete_ary if cmd.startswith(prefix)]
 
 
 def complete_brkpts(bpmgr, prefix):
     return complete_token(sorted(bpmgr.bpnumbers()), prefix)
@@ -69,22 +69,22 @@
 
 def next_token(str, start_pos):
     """Find the next token in str string from start_pos, we return
     the token and the next blank position after the token or
     str.size if this is the last token. Tokens are delimited by
     white space."""
     look_at = str[start_pos:]
-    match = re.search("\S", look_at)
+    match = re.search(r"\S", look_at)
     if match:
         pos = match.start()
     else:
         pos = 0
         pass
     next_nonblank_pos = start_pos + pos
-    next_match = re.search("\s", str[next_nonblank_pos:])
+    next_match = re.search(r"\s", str[next_nonblank_pos:])
     if next_match:
         next_blank_pos = next_nonblank_pos + next_match.start()
     else:
         next_blank_pos = len(str)
         pass
     return [next_blank_pos, str[next_nonblank_pos : next_blank_pos + 1].rstrip()]
```

### Comparing `trepan3k-1.2.8/trepan/lib/core.py` & `trepan3k-1.2.9/trepan/lib/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2008-2010, 2013-2016, 2020 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2008-2010, 2013-2016, 2020 2023 Rocky Bernstein
+#   <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -19,41 +21,43 @@
 stopping trace event handling and breakpoint checking. See also
 debugger for top-level Debugger class and module routine which
 ultimately will call this. An event processor is responsible of
 handling what to do when an event is triggered."""
 
 
 # Common Python packages
-import os, sys, threading
+import os
 import os.path as osp
+import sys
+import threading
 
 # External packages
 import pyficache
 import tracer
 
+import trepan.clifns as Mclifns
+
 # Our local modules
 from trepan.lib import breakpoint, default, stack as Mstack
 from trepan.misc import option_set
-import trepan.clifns as Mclifns
-from trepan.processor import trace as Mtrace, cmdproc as Mcmdproc
+from trepan.processor import cmdproc as Mcmdproc, trace as Mtrace
 
 
 class TrepanCore(object):
-
     DEFAULT_INIT_OPTS = {
         "processor": None,
         # How many step events to skip before
         # entering event processor? Zero (0) means stop at the next one.
         # A negative number indicates no eventual stopping.
         "step_ignore": 0,
         "ignore_filter": None,  # But see debugger.py
     }
 
     def __init__(self, debugger, opts=None):
-        """ Create a debugger object. But depending on the value of
+        """Create a debugger object. But depending on the value of
         key 'start' inside hash `opts', we may or may not initially
         start tracing events (i.e. enter the debugger).
 
         See also `start' and `stop'.
         """
 
         import trepan.bwprocessor as Mbwproc
@@ -135,15 +139,15 @@
         be debugged"""
         for frame_or_fn in frames_or_fns:
             rc = self.ignore_filter.add_include(frame_or_fn)
             pass
         return rc
 
     def canonic(self, filename):
-        """ Turns `filename' into its canonic representation and returns this
+        """Turns `filename' into its canonic representation and returns this
         string. This allows a user to refer to a given file in one of several
         equivalent ways.
 
         Relative filenames need to be fully resolved, since the current working
         directory might change over the course of execution.
 
         If filename is enclosed in < ... >, then we assume it is
@@ -177,15 +181,15 @@
             self.filename_cache[filename] = canonic
         canonic = pyficache.unmap_file(canonic)
 
         return canonic
 
     def canonic_filename(self, frame):
         """Picks out the file name from `frame' and returns its
-         canonic() value, a string."""
+        canonic() value, a string."""
         return self.canonic(frame.f_code.co_filename)
 
     def filename(self, filename=None):
         """Return filename or the basename of that depending on the
         basename setting"""
         if filename is None:
             if self.debugger.mainpyfile:
@@ -209,15 +213,15 @@
 
     def remove_ignore(self, frame_or_fn):
         """Remove `frame_or_fn' to the list of functions that are not to
         be debugged"""
         return self.ignore_filter.remove_include(frame_or_fn)
 
     def start(self, opts=None):
-        """ We've already created a debugger object, but here we start
+        """We've already created a debugger object, but here we start
         debugging in earnest. We can also turn off debugging (but have
         the hooks suspended or not) using 'stop'.
 
         'opts' is a hash of every known value you might want to set when
         starting the debugger. See START_OPTS of module default.
         """
 
@@ -309,23 +313,23 @@
 
     def matches_condition(self, frame):
         # Conditional bp.
         # Ignore count applies only to those bpt hits where the
         # condition evaluates to true.
         try:
             val = eval(self.until_condition, frame.f_globals, frame.f_locals)
-        except:
+        except Exception:
             # if eval fails, most conservative thing is to
             # stop on breakpoint regardless of ignore count.
             # Don't delete temporary, as another hint to user.
             return False
         return val
 
     def is_stop_here(self, frame, event):
-        """ Does the magic to determine if we stop here and run a
+        """Does the magic to determine if we stop here and run a
         command processor or not. If so, return True and set
         self.stop_reason; if not, return False.
 
         Determining factors can be whether a breakpoint was
         encountered, whether we are stepping, next'ing, finish'ing,
         and, if so, whether there is an ignore counter.
         """
@@ -443,15 +447,15 @@
             if self.is_stop_here(frame, event) or self.is_break_here(frame):
                 # Run the event processor
                 return self.processor.event_processor(frame, self.event, arg)
             return self
         finally:
             try:
                 self.debugger_lock.release()
-            except:
+            except Exception:
                 pass
             pass
         pass
 
     pass
```

### Comparing `trepan3k-1.2.8/trepan/lib/default.py` & `trepan3k-1.2.9/trepan/lib/default.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2008-2009, 2013, 2015, 2017, 2020-2021 Rocky Bernstein
-#   <rocky@gnu.org>
+#
+#   Copyright (C) 2008-2009, 2013, 2015, 2017, 2020-2021, 2023 Rocky
+#   Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -13,17 +14,18 @@
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """ A place for the debugger default settings """
 
 # External Egg packages
-import os, tracer
-from columnize import computed_displaywidth
+import os
 
+import tracer
+from columnize import computed_displaywidth
 from term_background import is_dark_background
 
 width = computed_displaywidth()
 
 # Below are the default debugger settings. The debugger object version
 # of this may change. A setting is something a user may want to
 # change, in contrast to settings that the debugger decides to set in
@@ -37,30 +39,30 @@
 
 DEBUGGER_SETTINGS = {
     # Emacs and old-style gdb annotate level. Used to annotate output
     # to make parsing inside Emacs easier and to allow Emacs to get
     # updated information (stack, local variables) without having to
     # poll for it.
     "annotate": 0,
-    # Format style to use in showing disssembly
+    # Format style to use in showing disassembly
     "asmfmt": "extended",
     # Eval as Python the unrecognized debugger commands?
     "autoeval": True,
     # Run 'list' command every time we enter the debugger?
     "autolist": False,
     # Enter IPython every time we enter the debugger?
     # Note: only relevant if we have ipython installed. This takes
     # precedence over autopython.
     "autoipython": False,
     # Run 'info pc' command every time we enter the debugger?
     "autopc": False,
     # Enter Python every time we enter the debugger?
     "autopython": False,
     # Show basename only on filename output?
-    # This opiton is useful in integration testing and
+    # This option is useful in integration testing and
     # possibly to prepare example output for publication
     "basename": False,
     # Set echoing lines read from debugger?
     "cmdtrace": False,
     # confirm potentially dangerous operations?
     "confirm": True,
     # Debug macros?
@@ -97,16 +99,16 @@
     # has an effect if trace is set True.
     "printset": tracer.ALL_EVENTS,
     # If this is set True, debugger startup file, e.g. .trepanrc will
     # not be read/run.
     "nostartup": False,
     # Reread source file if we determine it has changed?
     "reload": False,
-    # Skip instructions that make clases, functions, and closures?
-    # (In the Python they are "class" and "def" statments)
+    # Skip instructions that make classes, functions, and closures?
+    # (In the Python they are "class" and "def" statements)
     "skip": True,
     "step_ignore": 0,
     # Location to put temporary decompiled python files.
     # If value is None, use Python's defaults
     "tempdir": None,
     # print trace output?
     "trace": False,
@@ -120,15 +122,15 @@
     "PORT": 1027,
 }  # Arbitrary non-privileged port
 
 
 SERVER_SOCKET_OPTS = {
     "HOST": None,  # Symbolic name meaning all available interfaces
     "PORT": 1027,  # Arbitrary non-privileged port
-    "reuse": "posix" == os.name,  # Allow port to be resued on close?
+    "reuse": "posix" == os.name,  # Allow port to be reused on close?
     "skew": +0,  # additional increment on socket tries
     "search_limit": 100,  # max number of ports to try
 }
 
 # Default settings on the Debugger#start() method call
 START_OPTS = {
     "add_hook_opts": tracer.DEFAULT_ADD_HOOK_OPTS,
```

### Comparing `trepan3k-1.2.8/trepan/lib/deparse.py` & `trepan3k-1.2.9/trepan/lib/deparse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # -*- coding: utf-8 -*-
 """Deparsing Routines"""
 
-import sys, tempfile
-from io import StringIO
+import sys
+import tempfile
 from hashlib import sha1
-from xdis import PYTHON_VERSION
+from io import StringIO
+
+from xdis import PYTHON_VERSION_TRIPLE
 
-if 3.7 <= PYTHON_VERSION <= 3.8:
+if (3, 7) <= PYTHON_VERSION_TRIPLE < (3, 9):
     try:
+        from decompyle3.semantics.fragments import code_deparse, deparsed_find
         from decompyle3.semantics.linemap import code_deparse_with_map
-        from decompyle3.semantics.fragments import deparsed_find, code_deparse
     except ImportError:
+        from uncompyle6.semantics.fragments import code_deparse, deparsed_find
         from uncompyle6.semantics.linemap import code_deparse_with_map
-        from uncompyle6.semantics.fragments import deparsed_find, code_deparse
 else:
     from uncompyle6.semantics.linemap import code_deparse_with_map
     from uncompyle6.semantics.fragments import deparsed_find, code_deparse
 
 import pyficache
 
 # FIXME remap filename to a short name.
@@ -27,15 +29,15 @@
 def deparse_and_cache(co, errmsg_fn, tempdir=None):
     # co = proc_obj.curframe.f_code
     out = StringIO()
     deparsed = deparse_cache.get(co, None)
     if not deparsed or not hasattr(deparsed, "source_linemap"):
         try:
             deparsed = code_deparse_with_map(co, out)
-        except:
+        except Exception:
             errmsg_fn(str(sys.exc_info()[0]))
             errmsg_fn("error in deparsing code: %s" % co.co_filename)
             return None, None
 
         deparse_cache[co] = deparsed
 
     text = out.getvalue()
@@ -66,23 +68,23 @@
     nodeInfo = None
     deparsed = deparse_cache.get(co, None)
     if not deparsed or not hasattr(deparsed, "offsets"):
         out = StringIO()
         try:
             # FIXME: cache co
             deparsed = code_deparse(co, out)
-        except:
+        except Exception:
             print(sys.exc_info()[1])
             if errmsg_fn:
                 errmsg_fn(sys.exc_info()[1])
                 errmsg_fn("error in deparsing code")
         deparse_cache[co] = deparsed
     try:
         nodeInfo = deparsed_find((name, last_i), deparsed, co)
-    except:
+    except Exception:
         if errmsg_fn:
             errmsg_fn(sys.exc_info()[1])
             errmsg_fn("error in deparsing code at offset %d" % last_i)
 
     if not nodeInfo:
         nodeInfo = deparsed_find((name, last_i), deparsed, co)
     return deparsed, nodeInfo
```

### Comparing `trepan3k-1.2.8/trepan/lib/disassemble.py` & `trepan3k-1.2.9/trepan/lib/disassemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # -*- coding: utf-8 -*-
 #   Modification of Python's Lib/dis.py
 # FIXME: see if we can use more of Lib/dis in Python3
 """Disassembly Routines"""
 
-import inspect, sys, types
+import inspect
+import sys
+import types
 
 from xdis import (
+    IS_PYPY,
     Bytecode,
     findlabels,
     findlinestarts,
     get_instructions_bytes,
     get_opcode,
-    IS_PYPY,
 )
 from xdis.std import distb
 from xdis.version_info import PYTHON_VERSION_TRIPLE
 
 from trepan.lib.format import (
     Arrow,
     Comment,
@@ -162,15 +164,19 @@
             relative_pos=relative_pos,
             highlight=highlight,
             start_offset=start_offset,
             end_offset=end_offset,
             asm_format=asm_format,
         )
     elif isinstance(x, str):  # Source code
-        return disassemble_string(msg, msg_nocr, x,)
+        return disassemble_string(
+            msg,
+            msg_nocr,
+            x,
+        )
     else:
         errmsg("Don't know how to disassemble %s objects." % type(x).__name__)
     return None, None
 
 
 def disassemble(
     msg,
```

### Comparing `trepan3k-1.2.8/trepan/lib/display.py` & `trepan3k-1.2.9/trepan/lib/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         return
 
     def add(self, frame, arg, fmt=None):
         if not frame:
             return None
         try:
             eval(arg, frame.f_globals, frame.f_locals)
-        except:
+        except Exception:
             return None
         self.next += 1
         display = Display(frame, arg, fmt, self.next)
         self.list.append(display)
         return display
 
     def all(self):
@@ -110,15 +110,15 @@
         return
 
     def to_s(self, frame):
         if not frame:
             return 'No symbol "' + self.arg + '" in current context.'
         try:
             val = eval(self.arg, frame.f_globals, frame.f_locals)
-        except:
+        except Exception:
             return 'No symbol "' + self.arg + '" in current context.'
         s = "%3d: %s" % (self.number, Mstack.print_obj(self.arg, val, self.fmt, True))
         return s
 
     def format(self, show_enabled=True):
         """format display item"""
         what = ""
```

### Comparing `trepan3k-1.2.8/trepan/lib/eval.py` & `trepan3k-1.2.9/trepan/lib/eval.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2012-2015 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2012-2015, 2023 Rocky Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -17,39 +18,39 @@
 
 # extract the "expression" part of a line of source code.
 #
 import re
 
 
 def extract_expression(text):
-    if re.search("^\s*(?:if|elif)\s+", text):
-        text = re.sub("^\s*(?:if|elif)\s+", "", text)
-        text = re.sub(":(?:\s+.*$|$)", "", text)
-    elif re.search("^\s*assert\s+.*", text):
+    if re.search(r"^\s*(?:if|elif)\s+", text):
+        text = re.sub(r"^\s*(?:if|elif)\s+", "", text)
+        text = re.sub(r":(?:\s+.*$|$)", "", text)
+    elif re.search(r"^\s*assert\s+.*", text):
         # EXPR in : assert EXPRESSION:
-        text = re.sub("^\s*assert\s+", "", text)
-    elif re.search("^\s*(?:while)\s+", text):
-        text = re.sub("^\s*(?:while)\s+", "", text)
-        text = re.sub(":(?:\s+.*$|$)", "", text)
-    elif re.search("^\s*return\s+", text):
-        # EXPRESION in: return EXPRESSION
-        text = re.sub("^\s*return\s+", "", text)
-    elif re.search("^\s*for\s+.+\s+in\s+.*:", text):
-        # EXPRESION in: for VAR in EXPRESSION:
-        text = re.sub("^\s*for\s+.+\s+in\s+", "", text)
+        text = re.sub(r"^\s*assert\s+", "", text)
+    elif re.search(r"^\s*(?:while)\s+", text):
+        text = re.sub(r"^\s*(?:while)\s+", "", text)
+        text = re.sub(r":(?:\s+.*$|$)", "", text)
+    elif re.search(r"^\s*return\s+", text):
+        # EXPRESSION in: return EXPRESSION
+        text = re.sub(r"^\s*return\s+", "", text)
+    elif re.search(r"^\s*for\s+.+\s+in\s+.*:", text):
+        # EXPRESSION in: for VAR in EXPRESSION:
+        text = re.sub(r"^\s*for\s+.+\s+in\s+", "", text)
         text = re.sub(":.*$", "", text)
-    elif re.search("^\s*and\s+.*", text):
-        # EXPRESION in: and EXPRESSION
-        text = re.sub("^\s*and\s+", "", text)
-    elif re.search("^\s*or\s+.*", text):
-        # EXPRESION in: and EXPRESSION
-        text = re.sub("^\s*or\s+", "", text)
-    elif re.search("\s*[A-Za-z_][A-Za-z0-9_\[\]]*\s*=[^=>]", text):
+    elif re.search(r"^\s*and\s+.*", text):
+        # EXPRESSION in: and EXPRESSION
+        text = re.sub(r"^\s*and\s+", "", text)
+    elif re.search(r"^\s*or\s+.*", text):
+        # EXPRESSION in: and EXPRESSION
+        text = re.sub(r"^\s*or\s+", "", text)
+    elif re.search(r"\s*[A-Za-z_][A-Za-z0-9_\[\]]*\s*=[^=>]", text):
         # RHS of an assignment statement.
-        text = re.sub("^\s*[A-Za-z_][A-Za-z0-9_\[\]]*\s*=\s*", "", text)
+        text = re.sub(r"^\s*[A-Za-z_][A-Za-z0-9_\[\]]*\s*=\s*", "", text)
         pass
     return text
 
 
 # Demo it
 if __name__ == "__main__":
     for stmt in (
```

### Comparing `trepan3k-1.2.8/trepan/lib/file.py` & `trepan3k-1.2.9/trepan/lib/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2008-2009, 2013, 2015-2017 Rocky Bernstein <rocky@gnu.org>
+#   Copyright (C) 2008-2009, 2013, 2015-2017, 2023 Rocky Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Things related to file/module status"""
-import os, pyficache, stat, sys
+import os
+import stat
+import sys
+
+import pyficache
 
 
 def file_list():
     return list(set(pyficache.cached_files() + list(pyficache.file2file_remap.keys())))
 
 
 def is_compiled_py(filename):
```

### Comparing `trepan3k-1.2.8/trepan/lib/format.py` & `trepan3k-1.2.9/trepan/lib/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2013, 2015, 2017, 2019, 2020 Rocky Bernstein <rocky@gnu.org>
+
+#   Copyright (C) 2013, 2015, 2017, 2019, 2020, 2023
+#   Rocky Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -11,15 +13,17 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Pygments-related terminal formatting"""
 
-import re, sys
+import re
+import sys
+
 import pyficache
 from pygments import highlight, lex
 from pygments.console import ansiformat
 from pygments.filter import Filter
 from pygments.formatter import Formatter
 from pygments.formatters import TerminalFormatter
 from pygments.formatters.terminal import TERMINAL_COLORS
@@ -32,32 +36,31 @@
     Number,
     Operator,
     String,
     Token,
 )
 from pygments.util import get_choice_opt
 
-
-# Set up my own color scheme with some addtional definitions
+# Set up my own color scheme with some additional definitions.
 color_scheme = TERMINAL_COLORS.copy()
 color_scheme[Generic.Strong] = ("*black*", "*white*")
 color_scheme[Name.Variable] = ("_black_", "_white_")
 
 color_scheme[Generic.Strong] = ("*black*", "*white*")
 color_scheme[Name.Variable] = ("_black_", "_white_")
 color_scheme[Generic.Emph] = color_scheme[Comment.Preproc]
 
 # Assume pygments has fixed up the horrible atom colors
-## FIXME: change some horrible colors under atom dark
-## this is a hack until I get general way to do colorstyle setting
-## color_scheme[Token.Comment]  = ('darkgray', 'white')
-## color_scheme[Token.Keyword]  = ('darkblue', 'green')
-## color_scheme[Token.Number]  = ('darkblue', 'blue')
-## color_scheme[Keyword]  = ('darkblue', 'turquoise')
-## color_scheme[Number]  = ('darkblue', 'green')
+# FIXME: change some horrible colors under atom dark
+# this is a hack until I get general way to do colorstyle setting
+# color_scheme[Token.Comment]  = ('darkgray', 'white')
+# color_scheme[Token.Keyword]  = ('darkblue', 'green')
+# color_scheme[Token.Number]  = ('darkblue', 'blue')
+# color_scheme[Keyword]  = ('darkblue', 'turquoise')
+# color_scheme[Number]  = ('darkblue', 'green')
 
 pyficache.dark_terminal_formatter.colorscheme = color_scheme
 pyficache.light_terminal_formatter.colorscheme = color_scheme
 
 
 def format_token(ttype, token, colorscheme=color_scheme, highlight="light"):
     if "plain" == highlight:
@@ -225,59 +228,66 @@
             return
         elif (
             self.verbatim == "colon-verbatim" and ttype == Token.Text and text == "\n\n"
         ):
             self.write_nl()
             self.last_was_nl = True
             return
-        elif self.verbatim == 'colon-verbatim' and ttype == Token.Text and text == '\n':
+        elif self.verbatim == "colon-verbatim" and ttype == Token.Text and text == "\n":
             self.write_nl()
             self.last_was_nl = False
             return
         last_last_nl = self.last_was_nl
-        if text == '':
+        if text == "":
             pass
-        elif text[-1] == '\n':
+        elif text[-1] == "\n":
             if self.last_was_nl:
                 self.write_nl()
                 self.write_nl()
                 text = text[:-1]
             elif self.verbatim:
                 self.write_verbatim(text)
                 self.column = 0
-                self.verbatim = len(text) >=2 and text[-2] == '\n'
+                self.verbatim = len(text) >= 2 and text[-2] == "\n"
                 self.last_was_nl = True
                 return
             else:
-                self.write(' ', color)
+                self.write(" ", color)
                 text = text[:-1]
                 pass
             self.last_was_nl = True
-            if '' == text: return
-            while text[-1] == '\n':
+            if "" == text:
+                return
+            while text[-1] == "\n":
                 self.write_nl()
                 text = text[:-1]
-                if '' == text: return
+                if "" == text:
+                    return
                 pass
             pass
         else:
             self.last_was_nl = False
             pass
         self.in_list = False
         if last_last_nl:
-            if ' * ' == text[0:3]: self.in_list = True
-            elif '  ' == text[0:2]: self.verbatim = self.verbatim or True
+            if " * " == text[0:3]:
+                self.in_list = True
+            elif "  " == text[0:2]:
+                self.verbatim = self.verbatim or True
             pass
 
         # FIXME: there may be nested lists, tables and so on.
         if self.verbatim:
             self.write_verbatim(text)
         elif self.in_list:
             # FIXME:
-            self.write(text, color,)
+            self.write(
+                text,
+                color,
+            )
         else:
             words = re.compile("[ \t]+").split(text)
             for word in words[:-1]:
                 # print "column: %d, word %s" % (self.column, word)
                 if (self.column + len(word) + 1) >= self.width:
                     self.write_nl()
                     pass
```

### Comparing `trepan3k-1.2.8/trepan/lib/pp.py` & `trepan3k-1.2.9/trepan/lib/pp.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/trepan/lib/printing.py` & `trepan3k-1.2.9/trepan/lib/printing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # -*- coding: utf-8 -*-
-#  Copyright (C) 2007-2010, 2015, 2020 Rocky Bernstein
+#
+#  Copyright (C) 2007-2010, 2015, 2020, 2023 Rocky Bernstein
 
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import inspect, types
+import inspect
+import types
 
 
 def print_dict(s, obj, title):
     if hasattr(obj, "__dict__"):
         obj = obj.__dict__
         pass
     if isinstance(obj, dict):
@@ -32,30 +34,30 @@
     return s
 
 
 def print_argspec(obj, obj_name):
     """A slightly decorated version of inspect.format_argspec"""
     try:
         return obj_name + inspect.formatargspec(*inspect.getargspec(obj))
-    except:
+    except Exception:
         return None
     return  # Not reached
 
 
 def print_obj(arg, frame, format=None, short=False):
-    """Return a string representation of an object """
+    """Return a string representation of an object"""
     try:
         if not frame:
             # ?? Should we have set up a dummy globals
             # to have persistence?
             obj = eval(arg, None, None)
         else:
             obj = eval(arg, frame.f_globals, frame.f_locals)
             pass
-    except:
+    except Exception:
         return 'No symbol "' + arg + '" in current context.'
     # format and print
     what = arg
     if format:
         what = format + " " + arg
         obj = printf(obj, format)
     s = "%s = %s" % (what, obj)
@@ -112,25 +114,25 @@
     # Strip leading '/'
     if fmt[0] == "/":
         fmt = fmt[1:]
     f = fmt[0]
     if f in pconvert.keys():
         try:
             return pconvert[f](val)
-        except:
+        except Exception:
             return str(val)
     # binary (t is from 'twos')
     if f == "t":
         try:
             res = ""
             while val:
                 res = twos[val & 0xF] + res
                 val = val >> 4
             return res
-        except:
+        except Exception:
             return str(val)
     return str(val)
 
 
 if __name__ == "__main__":
     print(print_dict("", globals(), "my globals"))
     print("-" * 40)
```

### Comparing `trepan3k-1.2.8/trepan/lib/sighandler.py` & `trepan3k-1.2.9/trepan/lib/sighandler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2013-2014, 2016 Rocky Bernstein <rocky@gnu.org>
+#   Copyright (C) 2009, 2013-2014, 2016, 2022, 2023 Rocky Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -17,122 +17,125 @@
 # TODO:
 #  - Doublecheck handle_pass and other routines.
 #  - can remove signal handler altogether when
 #         ignore=True, print=False, pass=True
 #
 #
 import signal
+from typing import Optional
 
 
-def YN(b):
+def yes_or_no(b) -> str:
     """Return 'Yes' for True and 'No' for False, and ?? for anything
     else."""
     if type(b) != bool:
         return "??"
     if b:
         return "Yes"
     return "No"
 
 
-def lookup_signame(num):
+def lookup_signame(num: int) -> Optional[str]:
     """Find the corresponding signal name for 'num'. Return None
     if 'num' is invalid."""
     signames = signal.__dict__
     num = abs(num)
     for signame in list(signames.keys()):
-        if signame.startswith('SIG') and signames[signame] == num:
+        if signame.startswith("SIG") and signames[signame] == num:
             return signame
         pass
     # Something went wrong. Should have returned above
     return None
 
 
 def lookup_signum(name):
     """Find the corresponding signal number for 'name'. Return None
     if 'name' is invalid."""
     uname = name.upper()
-    if (uname.startswith('SIG') and hasattr(signal, uname)):
+    if uname.startswith("SIG") and hasattr(signal, uname):
         return getattr(signal, uname)
     else:
-        uname = "SIG"+uname
+        uname = "SIG" + uname
         if hasattr(signal, uname):
             return getattr(signal, uname)
         return None
-    return  # Not reached
+    return  # noqa
 
 
-def canonic_signame(name_num):
+def canonic_signame(name_num) -> Optional[str]:
     """Return a signal name for a signal name or signal
     number.  Return None is name_num is an int but not a valid signal
     number and False if name_num is a not number. If name_num is a
     signal name or signal number, the canonic if name is returned."""
     signum = lookup_signum(name_num)
     if signum is None:
         # Maybe signame is a number?
         try:
             num = int(name_num)
             signame = lookup_signame(num)
             if signame is None:
                 return None
-        except:
+        except Exception:
             return False
         return signame
 
     signame = name_num.upper()
-    if not signame.startswith('SIG'): return 'SIG'+signame
+    if not signame.startswith("SIG"):
+        return "SIG" + signame
     return signame
 
-fatal_signals = ['SIGKILL', 'SIGSTOP']
+
+fatal_signals = ["SIGKILL", "SIGSTOP"]
 
 # I copied these from GDB source code.
 signal_description = {
-  "SIGHUP"    : "Hangup",
-  "SIGINT"    : "Interrupt",
-  "SIGQUIT"   : "Quit",
-  "SIGILL"    : "Illegal instruction",
-  "SIGTRAP"   : "Trace/breakpoint trap",
-  "SIGABRT"   : "Aborted",
-  "SIGEMT"    : "Emulation trap",
-  "SIGFPE"    : "Arithmetic exception",
-  "SIGKILL"   : "Killed",
-  "SIGBUS"    : "Bus error",
-  "SIGSEGV"   : "Segmentation fault",
-  "SIGSYS"    : "Bad system call",
-  "SIGPIPE"   : "Broken pipe",
-  "SIGALRM"   : "Alarm clock",
-  "SIGTERM"   : "Terminated",
-  "SIGURG"    : "Urgent I/O condition",
-  "SIGSTOP"   : "Stopped (signal)",
-  "SIGTSTP"   : "Stopped (user)",
-  "SIGCONT"   : "Continued",
-  "SIGCHLD"   : "Child status changed",
-  "SIGTTIN"   : "Stopped (tty input)",
-  "SIGTTOU"   : "Stopped (tty output)",
-  "SIGIO"     : "I/O possible",
-  "SIGXCPU"   : "CPU time limit exceeded",
-  "SIGXFSZ"   : "File size limit exceeded",
-  "SIGVTALRM" : "Virtual timer expired",
-  "SIGPROF"   : "Profiling timer expired",
-  "SIGWINCH"  : "Window size changed",
-  "SIGLOST"   : "Resource lost",
-  "SIGUSR1"   : "User-defined signal 1",
-  "SIGUSR2"   : "User-defined signal 2",
-  "SIGPWR"    : "Power fail/restart",
-  "SIGPOLL"   : "Pollable event occurred",
-  "SIGWIND"   : "SIGWIND",
-  "SIGPHONE"  : "SIGPHONE",
-  "SIGWAITING": "Process's LWPs are blocked",
-  "SIGLWP"    : "Signal LWP",
-  "SIGDANGER" : "Swap space dangerously low",
-  "SIGGRANT"  : "Monitor mode granted",
-  "SIGRETRACT": "Need to relinquish monitor mode",
-  "SIGMSG"    : "Monitor mode data available",
-  "SIGSOUND"  : "Sound completed",
-  "SIGSAK"    : "Secure attention"
-  }
+    "SIGHUP": "Hangup",
+    "SIGINT": "Interrupt",
+    "SIGQUIT": "Quit",
+    "SIGILL": "Illegal instruction",
+    "SIGTRAP": "Trace/breakpoint trap",
+    "SIGABRT": "Aborted",
+    "SIGEMT": "Emulation trap",
+    "SIGFPE": "Arithmetic exception",
+    "SIGKILL": "Killed",
+    "SIGBUS": "Bus error",
+    "SIGSEGV": "Segmentation fault",
+    "SIGSYS": "Bad system call",
+    "SIGPIPE": "Broken pipe",
+    "SIGALRM": "Alarm clock",
+    "SIGTERM": "Terminated",
+    "SIGURG": "Urgent I/O condition",
+    "SIGSTOP": "Stopped (signal)",
+    "SIGTSTP": "Stopped (user)",
+    "SIGCONT": "Continued",
+    "SIGCHLD": "Child status changed",
+    "SIGTTIN": "Stopped (tty input)",
+    "SIGTTOU": "Stopped (tty output)",
+    "SIGIO": "I/O possible",
+    "SIGXCPU": "CPU time limit exceeded",
+    "SIGXFSZ": "File size limit exceeded",
+    "SIGVTALRM": "Virtual timer expired",
+    "SIGPROF": "Profiling timer expired",
+    "SIGWINCH": "Window size changed",
+    "SIGLOST": "Resource lost",
+    "SIGUSR1": "User-defined signal 1",
+    "SIGUSR2": "User-defined signal 2",
+    "SIGPWR": "Power fail/restart",
+    "SIGPOLL": "Pollable event occurred",
+    "SIGWIND": "SIGWIND",
+    "SIGPHONE": "SIGPHONE",
+    "SIGWAITING": "Process's LWPs are blocked",
+    "SIGLWP": "Signal LWP",
+    "SIGDANGER": "Swap space dangerously low",
+    "SIGGRANT": "Monitor mode granted",
+    "SIGRETRACT": "Need to relinquish monitor mode",
+    "SIGMSG": "Monitor mode data available",
+    "SIGSOUND": "Sound completed",
+    "SIGSAK": "Secure attention",
+}
 
 
 class SignalManager:
     """Manages Signal Handling information for the debugger
 
     - Do we print/not print when signal is caught
     - Do we pass/not pass the signal to the program
@@ -143,102 +146,137 @@
     default set. Parameter default_print specifies whether or not we
     print receiving a signals that is not ignored.
 
     All the methods which change these attributes return None on error, or
     True/False if we have set the action (pass/print/stop) for a signal
     handler.
     """
+
     def __init__(self, dbgr, ignore_list=None, default_print=True):
-        self.dbgr    = dbgr
+        self.dbgr = dbgr
         # dbgr.core.add_ignore(SigHandler.handle)
-        self.sigs    = {}
+        self.sigs = {}
 
         # List of signals. Dunno why signal doesn't provide.
         self.siglist = []
 
         # Ignore signal handling initially for these known signals.
         if ignore_list is None:
-            ignore_list = ['SIGALRM',    'SIGCHLD',  'SIGURG',
-                           'SIGIO',      'SIGCLD',
-                           'SIGVTALRM'   'SIGPROF',  'SIGWINCH',  'SIGPOLL',
-                           'SIGWAITING', 'SIGLWP',   'SIGCANCEL', 'SIGTRAP',
-                           'SIGTERM',    'SIGQUIT',  'SIGILL',
-                           # Wierd stuff from 3.3
-                           'SIG_SETMASK', 'ITIMER_PROF', 'ITIMER_VIRTUAL',
-                           'ITIMER_REAL', 'ITIMER_PROF',
-                           'SIG_BLOCK', 'SIG_UNBLOCK'
-                           ]  # NOQA
+            ignore_list = [
+                "SIGALRM",
+                "SIGCHLD",
+                "SIGURG",
+                "SIGIO",
+                "SIGCLD",
+                "SIGVTALRM" "SIGPROF",
+                "SIGWINCH",
+                "SIGPOLL",
+                "SIGWAITING",
+                "SIGLWP",
+                "SIGCANCEL",
+                "SIGTRAP",
+                "SIGTERM",
+                "SIGQUIT",
+                "SIGILL",
+                # Weird stuff from 3.3
+                "SIG_SETMASK",
+                "ITIMER_PROF",
+                "ITIMER_VIRTUAL",
+                "ITIMER_REAL",
+                "ITIMER_PROF",
+                "SIG_BLOCK",
+                "SIG_UNBLOCK",
+            ]  # NOQA
         self.ignore_list = ignore_list
-        self._orig_set_signal  = signal.signal
+        self._orig_set_signal = signal.signal
         signal.signal = self.set_signal_replacement
 
-        self.info_fmt='%-14s%-4s\t%-4s\t%-5s\t%-4s\t%s'
-        self.header  = self.info_fmt % ('Signal', 'Stop', 'Print',
-                                        'Stack', 'Pass',
-                                        'Description')
+        self.info_fmt = "%-14s%-4s\t%-4s\t%-5s\t%-4s\t%s"
+        self.header = self.info_fmt % (
+            "Signal",
+            "Stop",
+            "Print",
+            "Stack",
+            "Pass",
+            "Description",
+        )
 
-        if default_print: default_print = self.dbgr.intf[-1].msg
+        if default_print:
+            default_print = self.dbgr.intf[-1].msg
 
         for signame in list(signal.__dict__.keys()):
             # Look for a signal name on this os.
-            if signame.startswith('SIG') and '_' not in signame:
+            if signame.startswith("SIG") and "_" not in signame:
                 self.siglist.append(signame)
                 self.initialize_handler(signame)
             pass
-        self.action('SIGINT stop print nostack nopass')
+        self.action("SIGINT stop print nostack nopass")
         return
 
-    def initialize_handler(self, signame):
-        if signame in fatal_signals: return False
+    def initialize_handler(self, signame: str):
+        if signame in fatal_signals:
+            return False
         signum = lookup_signum(signame)
-        if signum is None: return False
+        if signum is None:
+            return False
 
         try:
             old_handler = signal.getsignal(signum)
         except ValueError:
             # On some OS's (Redhat 8), SIGNUM's are listed (like
             # SIGRTMAX) that getsignal can't handle.
             old_handler = None
             if signame in self.sigs:
                 self.sigs.pop(signame)
                 pass
 
         if signame in self.ignore_list:
-            self.sigs[signame] = SigHandler(self.dbgr, signame, signum,
-                                            old_handler,
-                                            None, False,
-                                            print_stack=False,
-                                            pass_along=True)
+            self.sigs[signame] = SigHandler(
+                self.dbgr,
+                signame,
+                signum,
+                old_handler,
+                None,
+                False,
+                print_stack=False,
+                pass_along=True,
+            )
         else:
-            self.sigs[signame] = SigHandler(self.dbgr, signame, signum,
-                                            old_handler,
-                                            self.dbgr.intf[-1].msg,
-                                            True,
-                                            print_stack=False,
-                                            pass_along=False)
+            self.sigs[signame] = SigHandler(
+                self.dbgr,
+                signame,
+                signum,
+                old_handler,
+                self.dbgr.intf[-1].msg,
+                True,
+                print_stack=False,
+                pass_along=False,
+            )
             pass
         return True
 
-    def set_signal_replacement(self, signum, handle):
+    def set_signal_replacement(self, signum: int, handle):
         """A replacement for signal.signal which chains the signal behind
         the debugger's handler"""
         signame = lookup_signame(signum)
         if signame is None:
-            self.dbgr.intf[-1].errmsg(("%s is not a signal number"
-                                       " I know about.")  % signum)
+            self.dbgr.intf[-1].errmsg(
+                "%s is not a signal number I know about." % signum
+            )
             return False
         # Since the intent is to set a handler, we should pass this
         # signal on to the handler
-        self.sigs[signame].pass_along = True
-        if self.check_and_adjust_sighandler(signame, self.sigs):
-            self.sigs[signame].old_handler = handle
-            return True
+        if signame not in self.ignore_list:
+            self.sigs[signame].pass_along = True
+            if self.check_and_adjust_sighandler(signame, self.sigs):
+                self.sigs[signame].old_handler = handle
+                return True
         return False
 
-    def check_and_adjust_sighandler(self, signame, sigs):
+    def check_and_adjust_sighandler(self, signame: str, sigs):
         """
         Check to see if a single signal handler that we are interested
         in has changed or has not been set initially. On return
         self.sigs[signame] should have our signal handler. True is
         returned if the same or adjusted, False or None if error or
         not found.
         """
@@ -270,62 +308,69 @@
                 # May be weird keys from 3.3
                 return False
             pass
         return True
 
     def check_and_adjust_sighandlers(self):
         """Check to see if any of the signal handlers we are interested in have
-        changed or is not initially set. Change any that are not right. """
+        changed or is not initially set. Change any that are not right."""
         for signame in list(self.sigs.keys()):
             if not self.check_and_adjust_sighandler(signame, self.sigs):
                 break
             pass
         return
 
     def is_name_or_number(self, name_num):
         signame = canonic_signame(name_num)
         if signame is None:
-            self.dbgr.intf[-1].errmsg(("%s is not a signal number" +
-                                       " I know about.")  % name_num)
+            self.dbgr.intf[-1].errmsg(
+                ("%s is not a signal number" + " I know about.") % name_num
+            )
             return False
         elif not signame:
-            self.dbgr.intf[-1].errmsg(("%s is not a signal name I " +
-                                       "know about.") % name_num)
+            self.dbgr.intf[-1].errmsg(
+                ("%s is not a signal name I " + "know about.") % name_num
+            )
             return False
         return signame
 
     def print_info_signal_entry(self, signame):
         """Print status for a single signal name (signame)"""
         if signame in signal_description:
-            description=signal_description[signame]
+            description = signal_description[signame]
         else:
-            description=""
+            description = ""
             pass
         if signame not in list(self.sigs.keys()):
             # Fake up an entry as though signame were in sigs.
-            self.dbgr.intf[-1].msg(self.info_fmt
-                                   % (signame, 'No', 'No', 'No', 'Yes',
-                                      description))
+            self.dbgr.intf[-1].msg(
+                self.info_fmt % (signame, "No", "No", "No", "Yes", description)
+            )
             return
 
         sig_obj = self.sigs[signame]
-        self.dbgr.intf[-1].msg(self.info_fmt %
-                               (signame,
-                                YN(sig_obj.b_stop),
-                                YN(sig_obj.print_method is not None),
-                                YN(sig_obj.print_stack),
-                                YN(sig_obj.pass_along),
-                                description))
+        self.dbgr.intf[-1].msg(
+            self.info_fmt
+            % (
+                signame,
+                yes_or_no(sig_obj.b_stop),
+                yes_or_no(sig_obj.print_method is not None),
+                yes_or_no(sig_obj.print_stack),
+                yes_or_no(sig_obj.pass_along),
+                description,
+            )
+        )
         return
 
     def info_signal(self, args):
         """Print information about a signal"""
-        if len(args) == 0: return None
+        if len(args) == 0:
+            return None
         signame = args[0]
-        if signame in ['handle', 'signal']:
+        if signame in ["handle", "signal"]:
             # This has come from dbgr's info command
             if len(args) == 1:
                 # Show all signal handlers
                 self.dbgr.core.processor.section(self.header)
                 for signame in self.siglist:
                     self.print_info_signal_entry(signame)
                 return True
@@ -340,52 +385,54 @@
         return True
 
     def action(self, arg):
         """Delegate the actions specified in 'arg' to another
         method.
         """
         if not arg:
-            self.info_signal(['handle'])
+            self.info_signal(["handle"])
             return True
         args = arg.split()
         signame = args[0]
         signame = self.is_name_or_number(args[0])
-        if not signame: return
+        if not signame:
+            return
 
         if len(args) == 1:
             self.info_signal([signame])
             return True
         # We can display information about 'fatal' signals, but not
         # change their actions.
         if signame in fatal_signals:
             return None
 
         if signame not in list(self.sigs.keys()):
-            if not self.initialize_handler(signame): return None
+            if not self.initialize_handler(signame):
+                return None
             pass
 
         # multiple commands might be specified, i.e. 'nopass nostop'
         for attr in args[1:]:
-            if attr.startswith('no'):
+            if attr.startswith("no"):
                 on = False
                 attr = attr[2:]
             else:
                 on = True
-            if 'stop'.startswith(attr):
+            if "stop".startswith(attr):
                 self.handle_stop(signame, on)
-            elif 'print'.startswith(attr) and len(attr) >= 2:
+            elif "print".startswith(attr) and len(attr) >= 2:
                 self.handle_print(signame, on)
-            elif 'pass'.startswith(attr):
+            elif "pass".startswith(attr):
                 self.handle_pass(signame, on)
-            elif 'ignore'.startswith(attr):
+            elif "ignore".startswith(attr):
                 self.handle_ignore(signame, on)
-            elif 'stack'.startswith(attr):
+            elif "stack".startswith(attr):
                 self.handle_print_stack(signame, on)
             else:
-                self.dbgr.intf[-1].errmsg('Invalid arguments')
+                self.dbgr.intf[-1].errmsg("Invalid arguments")
                 pass
             pass
         return self.check_and_adjust_sighandler(signame, self.sigs)
 
     def handle_print_stack(self, signame, print_stack):
         """Set whether we stop or not when this signal is caught.
         If 'set_stop' is True your program will stop when this signal
@@ -394,20 +441,20 @@
         return print_stack
 
     def handle_stop(self, signame, set_stop):
         """Set whether we stop or not when this signal is caught.
         If 'set_stop' is True your program will stop when this signal
         happens."""
         if set_stop:
-            self.sigs[signame].b_stop       = True
+            self.sigs[signame].b_stop = True
             # stop keyword implies print AND nopass
             self.sigs[signame].print_method = self.dbgr.intf[-1].msg
-            self.sigs[signame].pass_along   = False
+            self.sigs[signame].pass_along = False
         else:
-            self.sigs[signame].b_stop       = False
+            self.sigs[signame].b_stop = False
             pass
         return set_stop
 
     def handle_pass(self, signame, set_pass):
         """Set whether we pass this signal to the program (or not)
         when this signal is caught. If set_pass is True, Dbgr should allow
         your program to see this signal.
@@ -429,14 +476,15 @@
         """Set whether we print or not when this signal is caught."""
         if set_print:
             self.sigs[signame].print_method = self.dbgr.intf[-1].msg
         else:
             self.sigs[signame].print_method = None
             pass
         return set_print
+
     pass
 
 
 class SigHandler:
     """Store information about what we do when we handle a signal,
 
     - Do we print/not print when signal is caught
@@ -445,103 +493,117 @@
 
     Parameters:
        signame : name of signal (e.g. SIGUSR1 or USR1)
        print_method routine to use for "print"
        stop routine to call to invoke debugger when stopping
        pass_along: True is signal is to be passed to user's handler
     """
-    def __init__(self, dbgr, signame, signum, old_handler,
-                 print_method, b_stop,
-                 print_stack=False, pass_along=True):
-
-        self.dbgr         = dbgr
-        self.old_handler  = old_handler
-        self.pass_along   = pass_along
+
+    def __init__(
+        self,
+        dbgr,
+        signame,
+        signum,
+        old_handler,
+        print_method,
+        b_stop,
+        print_stack=False,
+        pass_along=True,
+    ):
+
+        self.dbgr = dbgr
+        self.old_handler = old_handler
+        self.pass_along = pass_along
         self.print_method = print_method
-        self.print_stack  = print_stack
-        self.signame      = signame
-        self.signum       = signum
-        self.b_stop       = b_stop
+        self.print_stack = print_stack
+        self.signame = signame
+        self.signum = signum
+        self.b_stop = b_stop
         return
 
     def handle(self, signum, frame):
         """This method is called when a signal is received."""
         if self.print_method:
-            self.print_method('\nProgram received signal %s.'
-                              % self.signame)
+            self.print_method("\nProgram received signal %s." % self.signame)
         if self.print_stack:
             import traceback
+
             strings = traceback.format_stack(frame)
             for s in strings:
-                if s[-1] == '\n': s = s[0:-1]
+                if s[-1] == "\n":
+                    s = s[0:-1]
                 self.print_method(s)
                 pass
             pass
         if self.b_stop:
             core = self.dbgr.core
             old_trace_hook_suspend = core.trace_hook_suspend
             core.trace_hook_suspend = True
-            core.stop_reason = ('intercepting signal %s (%d)' %
-                                (self.signame, signum))
-            core.processor.event_processor(frame, 'signal', signum)
+            core.stop_reason = "intercepting signal %s (%d)" % (self.signame, signum)
+            core.processor.event_processor(frame, "signal", signum)
             core.trace_hook_suspend = old_trace_hook_suspend
             pass
         if self.pass_along:
             # pass the signal to the program
             if self.old_handler:
                 self.old_handler(signum, frame)
                 pass
             pass
         return
+
     pass
 
+
 # When invoked as main program, do some basic tests of a couple of functions
-if __name__=='__main__':
-    import trepan.inout
-    import trepan.processor.command
-    import trepan.interfaces
-    for b in (True, False,):
-        print('YN of %s is %s' % (repr(b), YN(b)))
+if __name__ == "__main__":
+
+    for b in (
+        True,
+        False,
+    ):
+        print("yes_or_no of %s is %s" % (repr(b), yes_or_no(b)))
         pass
     for signum in range(signal.NSIG):
         signame = lookup_signame(signum)
         if signame is not None:
-            if not signame.startswith('SIG'): continue
+            if not signame.startswith("SIG"):
+                continue
             print(signame, signum, lookup_signum(signame))
-            assert(signum == lookup_signum(signame))
+            assert signum == lookup_signum(signame)
             # Try without the SIG prefix
-            assert(signum == lookup_signum(signame[3:]))
+            assert signum == lookup_signum(signame[3:])
             pass
         pass
 
     for i in (15, -15, 300):
-        print('lookup_signame(%d): %s' % (i, lookup_signame(i)))
+        print("lookup_signame(%d): %s" % (i, lookup_signame(i)))
         pass
 
-    for i in ('term', 'TERM', 'NotThere'):
-        print('lookup_signum(%s): %s' % (i, repr(lookup_signum(i))))
+    for i in ("term", "TERM", "NotThere"):
+        print("lookup_signum(%s): %s" % (i, repr(lookup_signum(i))))
         pass
 
-    for i in ('15', '-15', 'term', 'sigterm', 'TERM', '300', 'bogus'):
-        print('canonic_signame(%s): %s' % (i, canonic_signame(i)))
+    for i in ("15", "-15", "term", "sigterm", "TERM", "300", "bogus"):
+        print("canonic_signame(%s): %s" % (i, canonic_signame(i)))
         pass
 
     from trepan import debugger as Mdebugger
+
     dbgr = Mdebugger.Trepan()
     h = SignalManager(dbgr)
     h.info_signal(["TRAP"])
     # Set to known value
-    h.action('SIGUSR1')
-    h.action('usr1 print pass stop')
-    h.info_signal(['USR1'])
+    h.action("SIGUSR1")
+    h.action("usr1 print pass stop")
+    h.info_signal(["USR1"])
     # noprint implies no stop
-    h.action('SIGUSR1 noprint')
-    h.info_signal(['USR1'])
-    h.action('foo nostop')
+    h.action("SIGUSR1 noprint")
+    h.info_signal(["USR1"])
+    h.action("foo nostop")
     # stop keyword implies print
-    h.action('SIGUSR1 stop')
-    h.info_signal(['SIGUSR1'])
-    h.action('SIGUSR1 noprint')
-    h.info_signal(['SIGUSR1'])
-    h.action('SIGUSR1 nopass stack')
-    h.info_signal(['SIGUSR1'])
+    h.action("SIGUSR1 stop")
+    h.info_signal(["SIGUSR1"])
+    h.action("SIGUSR1 noprint")
+    h.info_signal(["SIGUSR1"])
+    h.action("SIGUSR1 nopass stack")
+    h.info_signal(["SIGUSR1"])
     pass
```

### Comparing `trepan3k-1.2.8/trepan/lib/stack.py` & `trepan3k-1.2.9/trepan/lib/stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,28 +11,31 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """ Functions for working with Python frames"""
 
-import inspect, linecache, os, re, xdis
+import inspect
+import linecache
+import os
+import os.path as osp
+import re
+
+import xdis
+from xdis import IS_PYPY, get_opcode
+from xdis.version_info import PYTHON_VERSION_TRIPLE
 
 import trepan.lib.bytecode as Mbytecode
-import trepan.lib.printing as Mprint
 import trepan.lib.format as Mformat
 import trepan.lib.pp as Mpp
-
-import os.path as osp
+import trepan.lib.printing as Mprint
 from trepan.lib.deparse import deparse_offset
 from trepan.processor.cmdfns import deparse_fn
 
-from xdis import IS_PYPY, get_opcode
-from xdis.version_info import PYTHON_VERSION_TRIPLE
-
 format_token = Mformat.format_token
 
 _with_local_varname = re.compile(r"_\[[0-9+]\]")
 
 
 def count_frames(frame, count_start=0):
     "Return a count of the number of frames"
@@ -83,15 +86,15 @@
         source_text = ""
         for i, source_text in enumerate(source_lines):
             if len(source_text) > 0:
                 break
         if len(source_lines) > 1:
             source_text += "..."
         source_text = '"%s"' % source_text
-    except:
+    except Exception:
         pass
     return source_text
 
 
 def format_stack_entry(
     dbg_obj, frame_lineno, lprefix=": ", include_location=True, color="plain"
 ):
@@ -106,15 +109,19 @@
         funcname = frame.f_code.co_name
     else:
         funcname = "<lambda>"
         pass
     s = format_token(Mformat.Function, funcname, highlight=color)
 
     args, varargs, varkw, local_vars = inspect.getargvalues(frame)
-    if "<module>" == funcname and ([], None, None,) == (args, varargs, varkw,):
+    if "<module>" == funcname and ([], None, None,) == (
+        args,
+        varargs,
+        varkw,
+    ):
         is_module = True
         if is_exec_stmt(frame):
             fn_name = format_token(Mformat.Function, "exec", highlight=color)
             source_text = deparse_source_from_code(frame.f_code)
             s += " %s(%s)" % (
                 format_token(Mformat.Function, fn_name, highlight=color),
                 source_text,
@@ -129,15 +136,15 @@
                         source_text,
                     )
             pass
     else:
         is_module = False
         try:
             parms = inspect.formatargvalues(args, varargs, varkw, local_vars)
-        except:
+        except Exception:
             pass
         else:
             maxargstrsize = dbg_obj.settings["maxargstrsize"]
             if len(parms) >= maxargstrsize:
                 parms = "%s...)" % parms[0:maxargstrsize]
                 pass
             s += parms
@@ -373,31 +380,31 @@
                 pass
             pass
         pass
     return s
 
 
 def eval_print_obj(arg, frame, format=None, short=False):
-    """Return a string representation of an object """
+    """Return a string representation of an object"""
     try:
         if not frame:
             # ?? Should we have set up a dummy globals
             # to have persistence?
             val = eval(arg, None, None)
         else:
             val = eval(arg, frame.f_globals, frame.f_locals)
             pass
-    except:
+    except Exception:
         return 'No symbol "' + arg + '" in current context.'
 
     return print_obj(arg, val, format, short)
 
 
 def print_obj(arg, val, format=None, short=False):
-    """Return a string representation of an object """
+    """Return a string representation of an object"""
     what = arg
     if format:
         what = format + " " + arg
         val = Mprint.printf(val, format)
         pass
     s = "%s = %s" % (what, val)
     if not short:
```

### Comparing `trepan3k-1.2.8/trepan/lib/thred.py` & `trepan3k-1.2.9/trepan/lib/thred.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/trepan/misc.py` & `trepan3k-1.2.9/trepan/misc.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/trepan/options.py` & `trepan3k-1.2.9/trepan/options.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,278 +1,385 @@
 #!/usr/bin/env python
 # -*- coding: iso-8859-1 -*-
-#   Copyright (C) 2013-2015 Rocky Bernstein <rocky@gnu.org>
+#   Copyright (C) 2013-2015, 2023 Rocky Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import os, sys, codecs
-
+import codecs
+import os
+import sys
 from optparse import OptionParser
-from trepan import debugger as Mdebugger, api as Mapi, clifns as Mclifns
-from trepan.lib import file as Mfile
+
+from trepan import api as Mapi, clifns as Mclifns, debugger as Mdebugger
 from trepan.inout import output as Moutput
+from trepan.lib import file as Mfile
+
 
 def default_configfile(base_filename):
-    '''Return fully expanded configuration filename location for
-    base_filename. python2 and  python3 debuggers share the smae
+    """Return fully expanded configuration filename location for
+    base_filename. python2 and  python3 debuggers share the same
     directory: ~/.config/trepan.py
-    '''
-    file_dir = os.path.join(os.environ.get('HOME', '~'), '.config', 'trepanpy')
+    """
+    file_dir = os.path.join(os.environ.get("HOME", "~"), ".config", "trepanpy")
     file_dir = Mclifns.path_expanduser_abs(file_dir)
 
     if not os.path.isdir(file_dir):
         os.makedirs(file_dir, mode=0o755)
     return os.path.join(file_dir, base_filename)
 
+
 def add_startup_file(dbg_initfiles):
-    """ Read debugger startup file(s): both python code and
+    """Read debugger startup file(s): both python code and
     debugger profile to dbg_initfiles."""
 
-    startup_python_file = default_configfile('profile.py')
+    startup_python_file = default_configfile("profile.py")
 
     if Mfile.readable(startup_python_file):
-        with codecs.open(startup_python_file, 'r', encoding='utf8') as fp:
-                exec(fp.read())
+        with codecs.open(startup_python_file, "r", encoding="utf8") as fp:
+            exec(fp.read())
 
-    startup_trepan_file = default_configfile('profile')
+    startup_trepan_file = default_configfile("profile")
     if Mfile.readable(startup_trepan_file):
         if startup_trepan_file not in dbg_initfiles:
             dbg_initfiles.append(startup_trepan_file)
         pass
     return
 
+
 def process_options(debugger_name, pkg_version, sys_argv, option_list=None):
     """Handle debugger options. Set `option_list' if you are writing
     another main program and want to extend the existing set of debugger
     options.
 
-    The options dicionary from optparser is returned. sys_argv is
+    The options dictionary from optparser is returned. sys_argv is
     also updated."""
-    usage_str="""%prog [debugger-options] [python-script [script-options...]]
+    usage_str = """%prog [debugger-options] [python-script [script-options...]]
 
     Runs the extended python debugger"""
 
     # serverChoices = ('TCP','FIFO', None)
 
-    optparser = OptionParser(usage=usage_str, option_list=option_list,
-                             version="%%prog version %s" % pkg_version)
-
-    optparser.add_option("-X", "--trace", dest="linetrace",
-                         action="store_true", default=False,
-                         help="Show lines before executing them. "
-                         "This option also sets --batch")
-    optparser.add_option("-F", "--fntrace", dest="fntrace",
-                         action="store_true", default=False,
-                         help="Show functions before executing them. "
-                         "This option also sets --batch")
-    optparser.add_option("--basename", dest="basename",
-                         action="store_true", default=False,
-                         help="Filenames strip off basename, "
-                         "(e.g. for regression tests)"
-                         )
+    optparser = OptionParser(
+        usage=usage_str,
+        option_list=option_list,
+        version="%%prog version %s" % pkg_version,
+    )
+
+    optparser.add_option(
+        "-X",
+        "--trace",
+        dest="linetrace",
+        action="store_true",
+        default=False,
+        help="Show lines before executing them. " "This option also sets --batch",
+    )
+    optparser.add_option(
+        "-F",
+        "--fntrace",
+        dest="fntrace",
+        action="store_true",
+        default=False,
+        help="Show functions before executing them. " "This option also sets --batch",
+    )
+    optparser.add_option(
+        "--basename",
+        dest="basename",
+        action="store_true",
+        default=False,
+        help="Filenames strip off basename, " "(e.g. for regression tests)",
+    )
     #     optparser.add_option("--batch", dest="noninteractive",
     #                          action="store_true", default=False,
     #                          help="Don't run interactive commands shell on "+
     #                          "stops.")
-    optparser.add_option("--client", dest="client",
-                         action='store_true',
-                         help="Connect to an existing debugger process "
-                         "started with the --server option. "
-                         "See options for client.")
-    optparser.add_option("-x", "--command", dest="command",
-                         action="store", type='string', metavar='FILE',
-                         help="Execute commands from FILE.")
-    optparser.add_option("--cd", dest="cd",
-                         action="store", type='string', metavar='DIR',
-                         help="Change current directory to DIR.")
-    optparser.add_option("--confirm", dest="confirm",
-                         action="store_true", default=True,
-                         help="Confirm potentially dangerous operations")
-    optparser.add_option("--dbg_trepan", dest="dbg_trepan",
-                         action="store_true", default=False,
-                         help="Debug the debugger")
-    optparser.add_option("--different", dest="different",
-                         action="store_true", default=True,
-                         help="Consecutive stops should have "
-                         "different positions")
+    optparser.add_option(
+        "--client",
+        dest="client",
+        action="store_true",
+        help="Connect to an existing debugger process "
+        "started with the --server option. "
+        "See options for client.",
+    )
+    optparser.add_option(
+        "-x",
+        "--command",
+        dest="command",
+        action="store",
+        type="string",
+        metavar="FILE",
+        help="Execute commands from FILE.",
+    )
+    optparser.add_option(
+        "--cd",
+        dest="cd",
+        action="store",
+        type="string",
+        metavar="DIR",
+        help="Change current directory to DIR.",
+    )
+    optparser.add_option(
+        "--confirm",
+        dest="confirm",
+        action="store_true",
+        default=True,
+        help="Confirm potentially dangerous operations",
+    )
+    optparser.add_option(
+        "--dbg_trepan",
+        dest="dbg_trepan",
+        action="store_true",
+        default=False,
+        help="Debug the debugger",
+    )
+    optparser.add_option(
+        "--different",
+        dest="different",
+        action="store_true",
+        default=True,
+        help="Consecutive stops should have " "different positions",
+    )
     #     optparser.add_option("--error", dest="errors", metavar='FILE',
     #                          action="store", type='string',
     #                          help="Write debugger's error output "
     #                          + "(stderr) to FILE")
-    optparser.add_option("-e", "--exec", dest="execute", type="string",
-                         help="list of debugger commands to " +
-                         "execute. Separate the commands with ;;")
-
-    optparser.add_option("-H", "--host", dest="host", default='127.0.0.1',
-                         action="store", type='string', metavar='IP-OR-HOST',
-                         help="connect IP or host name. "
-                         "Only valid if --client option given.")
-
-    optparser.add_option("--highlight", dest="highlight",
-                         action="store", type='string',
-                         metavar='{light|dark|plain}',
-                         default='light',
-                         help="Use syntax and terminal highlight output. "
-                         "'plain' is no highlight")
-
-    optparser.add_option("--private", dest="private",
-                         action='store_true', default=False,
-                         help="Don't register this as a global debugger")
-
-    optparser.add_option("--main", dest="main",
-                         action="store_true", default=True,
-                         help="First stop should be in __main__"
-                         )
-    optparser.add_option("--no-main", dest="main",
-                         action="store_false", default=True,
-                         help="First stop should be in __main__"
-                         )
-    optparser.add_option("--post-mortem", dest="post_mortem",
-                         action='store_true', default=True,
-                         help=("Enter debugger on an uncaught (fatal) "
-                               "exception"))
-
-    optparser.add_option("--no-post-mortem", dest="post_mortem",
-                         action='store_false', default=True,
-                         help=("Don't enter debugger on an uncaught (fatal) "
-                               "exception"))
-
-    optparser.add_option("-n", "--nx", dest="noexecute",
-                         action="store_true", default=False,
-                         help=("Don't execute commands found in any "
-                               "initialization files"))
-
-    optparser.add_option("-o", "--output", dest="output", metavar='FILE',
-                         action="store", type='string',
-                         help=("Write debugger's output (stdout) "
-                               "to FILE"))
-    optparser.add_option("-P", "--port", dest="port", default=1027,
-                         action="store", type='int',
-                         help="Use TCP port number NUMBER for "
-                         "out-of-process connections.")
-
-    optparser.add_option("--server", dest="server",
-                         action='store_true',
-                         help="Out-of-process server connection mode")
+    optparser.add_option(
+        "-e",
+        "--exec",
+        dest="execute",
+        type="string",
+        help="list of debugger commands to " + "execute. Separate the commands with ;;",
+    )
+
+    optparser.add_option(
+        "-H",
+        "--host",
+        dest="host",
+        default="127.0.0.1",
+        action="store",
+        type="string",
+        metavar="IP-OR-HOST",
+        help="connect IP or host name. " "Only valid if --client option given.",
+    )
+
+    optparser.add_option(
+        "--highlight",
+        dest="highlight",
+        action="store",
+        type="string",
+        metavar="{light|dark|plain}",
+        default="light",
+        help="Use syntax and terminal highlight output. " "'plain' is no highlight",
+    )
+
+    optparser.add_option(
+        "--private",
+        dest="private",
+        action="store_true",
+        default=False,
+        help="Don't register this as a global debugger",
+    )
+
+    optparser.add_option(
+        "--main",
+        dest="main",
+        action="store_true",
+        default=True,
+        help="First stop should be in __main__",
+    )
+    optparser.add_option(
+        "--no-main",
+        dest="main",
+        action="store_false",
+        default=True,
+        help="First stop should be in __main__",
+    )
+    optparser.add_option(
+        "--post-mortem",
+        dest="post_mortem",
+        action="store_true",
+        default=True,
+        help=("Enter debugger on an uncaught (fatal) " "exception"),
+    )
+
+    optparser.add_option(
+        "--no-post-mortem",
+        dest="post_mortem",
+        action="store_false",
+        default=True,
+        help=("Don't enter debugger on an uncaught (fatal) " "exception"),
+    )
+
+    optparser.add_option(
+        "-n",
+        "--nx",
+        dest="noexecute",
+        action="store_true",
+        default=False,
+        help=("Don't execute commands found in any " "initialization files"),
+    )
+
+    optparser.add_option(
+        "-o",
+        "--output",
+        dest="output",
+        metavar="FILE",
+        action="store",
+        type="string",
+        help=("Write debugger's output (stdout) " "to FILE"),
+    )
+    optparser.add_option(
+        "-P",
+        "--port",
+        dest="port",
+        default=1027,
+        action="store",
+        type="int",
+        help="Use TCP port number NUMBER for " "out-of-process connections.",
+    )
+
+    optparser.add_option(
+        "--server",
+        dest="server",
+        action="store_true",
+        help="Out-of-process server connection mode",
+    )
 
     # optparser.add_option("--style", dest="style",
     #                      action="store", type='string',
     #                      metavar='*pygments-style*',
     #                      default=None,
     #                      help=("Pygments style; 'none' "
     #                            "uses 8-color rather than 256-color terminal"))
 
-    optparser.add_option("--sigcheck", dest="sigcheck",
-                         action="store_true", default=False,
-                         help="Set to watch for signal handler changes")
-    optparser.add_option("-t", "--target", dest="target",
-                         help=("Specify a target to connect to. Arguments"
-                               " should be of form, 'protocol address'.")),
-    optparser.add_option("--from_ipython", dest='from_ipython', action='store_true',
-                         default=False, help="Called from inside ipython")
+    optparser.add_option(
+        "--sigcheck",
+        dest="sigcheck",
+        action="store_true",
+        default=False,
+        help="Set to watch for signal handler changes",
+    )
+    optparser.add_option(
+        "-t",
+        "--target",
+        dest="target",
+        help=(
+            "Specify a target to connect to. Arguments"
+            " should be of form, 'protocol address'."
+        ),
+    ),
+    optparser.add_option(
+        "--from_ipython",
+        dest="from_ipython",
+        action="store_true",
+        default=False,
+        help="Called from inside ipython",
+    )
 
     # annotate option produces annotations, used in trepan.el for a
     # better emacs integration. Annotations are similar in purpose to
     # those of GDB (see that manual for a description), although the
     # syntax is different.  they have the following format:
     #
     # ^Z^Zannotation-name
     # <arbitrary text>
     # ^Z^Z
     #
     # where ^Z is the ctrl-Z character, and "annotname" is the name of the
     # annotation. A line with only two ^Z ends the annotation (no nesting
     # allowed). See trepan.el for the usage
-    optparser.add_option("--annotate", default=0, type="int",
-                         help="Use annotations to work inside emacs")
+    optparser.add_option(
+        "--annotate", default=0, type="int", help="Use annotations to work inside emacs"
+    )
 
     # Set up to stop on the first non-option because that's the name
     # of the script to be debugged on arguments following that are
     # that scripts options that should be left untouched.  We would
     # not want to interpret and option for the script, e.g. --help, as
     # one one of our own, e.g. --help.
 
     optparser.disable_interspersed_args()
 
     sys.argv = list(sys_argv)
     # FIXME: why does this mess up integration tests?
     # (opts, sys.argv) = optparser.parse_args(sys_argv)
     (opts, sys.argv) = optparser.parse_args()
-    dbg_opts = {'from_ipython': opts.from_ipython}
+    dbg_opts = {"from_ipython": opts.from_ipython}
 
     # Handle debugger startup command files: --nx (-n) and --command.
     dbg_initfiles = []
     if not opts.noexecute:
         add_startup_file(dbg_initfiles)
 
     # As per gdb, first we execute user initialization files and then
     # we execute any file specified via --command.
     if opts.command:
         dbg_initfiles.append(opts.command)
         pass
 
-    dbg_opts['proc_opts'] = {'initfile_list': dbg_initfiles}
+    dbg_opts["proc_opts"] = {"initfile_list": dbg_initfiles}
 
     if opts.cd:
         os.chdir(opts.cd)
         pass
 
     if opts.output:
         try:
-            dbg_opts['output'] = Moutput.DebuggerUserOutput(opts.output)
+            dbg_opts["output"] = Moutput.DebuggerUserOutput(opts.output)
         except IOError:
             _, xxx_todo_changeme, _ = sys.exc_info()
             (errno, strerror) = xxx_todo_changeme.args
             print("I/O in opening debugger output file %s" % opts.output)
             print("error(%s): %s" % (errno, strerror))
-        except:
-            print("Unexpected error in opening debugger output file %s" %
-                  opts.output)
+        except Exception:
+            print("Unexpected error in opening debugger output file %s" % opts.output)
             print(sys.exc_info()[0])
             sys.exit(2)
             pass
         pass
 
     return opts, dbg_opts, sys.argv
 
+
 def _postprocess_options(dbg, opts):
-    ''' Handle options (`opts') that feed into the debugger (`dbg')'''
+    """Handle options (`opts') that feed into the debugger (`dbg')"""
     # Set dbg.settings['printset']
     print_events = []
-    if opts.fntrace:   print_events = ['c_call', 'c_return', 'call', 'return']
-    if opts.linetrace: print_events += ['line']
+    if opts.fntrace:
+        print_events = ["c_call", "c_return", "call", "return"]
+    if opts.linetrace:
+        print_events += ["line"]
     if len(print_events):
-        dbg.settings['printset'] = frozenset(print_events)
+        dbg.settings["printset"] = frozenset(print_events)
         pass
 
-    for setting in ('annotate', 'basename', 'different'):
+    for setting in ("annotate", "basename", "different"):
         dbg.settings[setting] = getattr(opts, setting)
         pass
 
-    if getattr(opts, 'highlight'):
-        dbg.settings['highlight'] = opts.highlight
+    if getattr(opts, "highlight"):
+        dbg.settings["highlight"] = opts.highlight
     else:
-        dbg.settings['highlight'] = 'plain'
+        dbg.settings["highlight"] = "plain"
 
     # if getattr(opts, 'style') and opts.style != 'none':
     #     dbg.settings['style'] = opts.style
     # else:
     #     dbg.settings['style'] = None
-    dbg.settings['style'] = None
+    dbg.settings["style"] = None
 
     # Normally we want to set Mdebugger.debugger_obj so that one can
     # put trepan.debugger breakpoints in a program and not have more
     # than one debugger running. More than one debugger may confuse
     # users, e.g. set different might stop at the same line once for
     # each debugger.
     if not opts.private:
@@ -283,42 +390,43 @@
     #         try:
     #             dbg.stderr = open(opts.errors, 'w')
     #         except IOError, (errno, strerror):
     #             print "I/O in opening debugger output file %s" % opts.errors
     #             print "error(%s): %s" % (errno, strerror)
     #         except ValueError:
     #             print "Could not convert data to an integer."
-    #         except:
+    #         except Exception:
     #             print "Unexpected error in opening debugger output "
     #                   "file %s" % opts.errors
     #             print sys.exc_info()[0]
     #             sys.exit(2)
 
     #     if opts.execute:
     #         dbg.cmdqueue = list(opts.execute.split(';;'))
 
     if opts.post_mortem:
         Mapi.debugger_on_post_mortem()
         pass
     return
 
+
 # Demo it
-if __name__=='__main__':
+if __name__ == "__main__":
     import pprint
 
     def doit(prog, version, arg_str):
         print("options '%s'" % arg_str)
         args = arg_str.split()
-        opts, dbg_opts, sys_argv = process_options('testing', version, args)
+        opts, dbg_opts, sys_argv = process_options("testing", version, args)
         pp.pprint(vars(opts))
-        print('')
+        print("")
         return
 
     pp = pprint.PrettyPrinter(indent=4)
-    doit('testing', '1.1', '')
-    doit('testing', '1.2', 'foo bar')
-    doit('testing', '1.3', '--server')
-    doit('testing', '1.3', '--command %s bar baz' % __file__)
-    doit('testing', '1.4', '--server --client')
-    doit('testing', '1.5', '--style=emacs')
-    doit('testing', '1.6', '--help')  # exits, so must be last
+    doit("testing", "1.1", "")
+    doit("testing", "1.2", "foo bar")
+    doit("testing", "1.3", "--server")
+    doit("testing", "1.3", "--command %s bar baz" % __file__)
+    doit("testing", "1.4", "--server --client")
+    doit("testing", "1.5", "--style=emacs")
+    doit("testing", "1.6", "--help")  # exits, so must be last
     pass
```

### Comparing `trepan3k-1.2.8/trepan/post_mortem.py` & `trepan3k-1.2.9/trepan/post_mortem.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # Post-Mortem interface
 
-import inspect, os, sys, re, traceback
+import inspect
+import os
+import re
+import sys
+import traceback
 
 # Our local modules
 from trepan import debugger as Mdebugger
 from trepan.exception import DebuggerQuit, DebuggerRestart
 
 
 def get_last_or_frame_exception():
@@ -48,35 +52,37 @@
     'dbg', is an optional trepan.Trepan object.
     """
     post_mortem(get_last_or_frame_exception(), frameno, dbg=dbg)
     return
 
 
 def post_mortem_excepthook(exc_type, exc_value, exc_tb, tb_fn=None):
-    if str(exc_type) == str(DebuggerQuit): return
+    if str(exc_type) == str(DebuggerQuit):
+        return
     try:
         if str(exc_type) == str(DebuggerRestart):
-            if ( exc_value and exc_value.sys_argv and
-                 len(exc_value.sys_argv) > 0 ):
-                print("No restart handler - trying restart via execv(%s)" %
-                       repr(exc_value.sys_argv))
+            if exc_value and exc_value.sys_argv and len(exc_value.sys_argv) > 0:
+                print(
+                    "No restart handler - trying restart via execv(%s)"
+                    % repr(exc_value.sys_argv)
+                )
                 os.execvp(exc_value.sys_argv[0], exc_value.sys_argv)
             else:
                 print("No restart handler, no params registered")
                 print("Entering post-mortem debugger...")
         else:
             if tb_fn:
                 tb_fn(exc_type, exc_value, exc_tb)
             else:
                 traceback.print_exception(exc_type, exc_value, exc_tb)
             print("Uncaught exception. Entering post-mortem debugger...")
             pass
         post_mortem((exc_type, exc_value, exc_tb))
         print("Post-mortem debugger finished.")
-    except:
+    except Exception:
         pass
     return
 
 
 def post_mortem(exc=None, frameno=1, dbg=None):
     """Enter debugger read loop after your program has crashed.
 
@@ -102,30 +108,34 @@
     re_bogus_file = re.compile("^<.+>$")
 
     if exc[0] is None:
         # frameno+1 because we are about to add one more level of call
         # in get_last_or_frame_exception
         exc = get_last_or_frame_exception()
         if exc[0] is None:
-            print("Can't find traceback for post_mortem "
-                  "in sys.last_traceback or sys.exec_info()")
+            print(
+                "Can't find traceback for post_mortem "
+                "in sys.last_traceback or sys.exec_info()"
+            )
             return
         pass
     exc_type, exc_value, exc_tb = exc
-    dbg.core.execution_status = ('Terminated with unhandled exception %s'
-                                 % exc_type)
+    dbg.core.execution_status = "Terminated with unhandled exception %s" % exc_type
 
     # tb has least-recent traceback entry first. We want the most-recent
     # entry. Also we'll pick out a mainpyfile name if it hasn't previously
     # been set.
     if exc_tb is not None:
         while exc_tb.tb_next is not None:
             filename = exc_tb.tb_frame.f_code.co_filename
-            if (dbg.mainpyfile and 0 == len(dbg.mainpyfile)
-                and not re_bogus_file.match(filename)):
+            if (
+                dbg.mainpyfile
+                and 0 == len(dbg.mainpyfile)
+                and not re_bogus_file.match(filename)
+            ):
                 dbg.mainpyfile = filename
                 pass
             exc_tb = exc_tb.tb_next
             pass
         dbg.core.processor.curframe = exc_tb.tb_frame
         pass
 
@@ -140,58 +150,61 @@
     #     dbg._sys_argv[:0] = [__title__]
 
     try:
         # # FIXME: This can be called from except hook in which case we
         # # need this. Dunno why though.
         # try:
         #     _pydb_trace.set_trace(t.tb_frame)
-        # except:
+        # except Exception:
         #     pass
 
         # Possibly a bug in Python 2.5. Why f.f_lineno is
         # not always equal to t.tb_lineno, I don't know.
         f = exc_tb.tb_frame
-        if f and f.f_lineno != exc_tb.tb_lineno : f = f.f_back
-        dbg.core.processor.event_processor(f, 'exception', exc, 'Trepan3k:pm')
+        if f and f.f_lineno != exc_tb.tb_lineno:
+            f = f.f_back
+        dbg.core.processor.event_processor(f, "exception", exc, "Trepan3k:pm")
     except DebuggerRestart:
         while True:
             sys.argv = list(dbg._program_sys_argv)
-            dbg.msg("Restarting %s with arguments:\n\t%s"
-                  % (dbg.filename(dbg.mainpyfile),
-                     " ".join(dbg._program_sys_argv[1:])))
+            dbg.msg(
+                "Restarting %s with arguments:\n\t%s"
+                % (dbg.filename(dbg.mainpyfile), " ".join(dbg._program_sys_argv[1:]))
+            )
             try:
                 dbg.run_script(dbg.mainpyfile)
             except DebuggerRestart:
                 pass
             pass
     except DebuggerQuit:
         pass
     return
 
+
 def uncaught_exception(dbg, tb_fn=None):
     exc = sys.exc_info()
     exc_type, exc_value, exc_tb = exc
-    if exc_type == DebuggerQuit: return
+    if exc_type == DebuggerQuit:
+        return
     if exc_type == DebuggerRestart:
         print("restart not done yet - entering post mortem debugging")
     elif exc_tb is None:
         print("You don't seem to have an exception traceback, yet.")
         return
     else:
         if tb_fn:
             tb_fn(exc_type, exc_value, exc_tb)
         else:
             traceback.print_exception(exc_type, exc_value, exc_tb)
         print("uncaught exception. entering post mortem debugging")
         pass
-    dbg.core.execution_status = ('Terminated with unhandled exception %s'
-                                 % exc_type)
-    dbg.core.processor.event_processor(exc_tb.tb_frame, 'exception', exc,
-                                       'Trepan3k:pm')
+    dbg.core.execution_status = "Terminated with unhandled exception %s" % exc_type
+    dbg.core.processor.event_processor(exc_tb.tb_frame, "exception", exc, "Trepan3k:pm")
     print("Post mortem debugger finished.")
     return
 
-if __name__=='__main__':
+
+if __name__ == "__main__":
     if len(sys.argv) > 1:
         pm()
         pass
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/cmd_addrlist.py` & `trepan3k-1.2.9/trepan/processor/cmd_addrlist.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,42 +16,49 @@
 
 from trepan.processor.parse.semantics import build_arange, Location
 from trepan.processor.parse.parser import LocationError
 from trepan.processor.parse.scanner import ScannerError
 from trepan.processor.location import resolve_address_location
 
 INVALID_PARSE_LIST = (None, None, None, None, None, None)
+
+
 def parse_addr_list_cmd(proc, args, listsize=40):
     """Parses arguments for the "list" command and returns the tuple:
     (filename, first line number, last line number)
     or sets these to None if there was some problem."""
 
-    text = proc.current_command[len(args[0])+1:].strip()
+    text = proc.current_command[len(args[0]) + 1 :].strip()
 
-    if text in frozenset(('', '.', '+', '-')):
-        if text == '.':
-            location = resolve_address_location(proc, '.')
-            return (location.path, location.line_number, True,
-                    location.line_number + listsize, True,
-                    location.method)
+    if text in frozenset(("", ".", "+", "-")):
+        if text == ".":
+            location = resolve_address_location(proc, ".")
+            return (
+                location.path,
+                location.line_number,
+                True,
+                location.line_number + listsize,
+                True,
+                location.method,
+            )
 
         if proc.list_offset is None:
             proc.errmsg("Don't have previous list location")
             return INVALID_PARSE_LIST
 
         filename = proc.list_filename
-        if text == '+':
-            first = max(0, proc.list_offset-1)
-        elif text == '-':
+        if text == "+":
+            first = max(0, proc.list_offset - 1)
+        elif text == "-":
             # FIXME: not quite right for offsets
             if proc.list_lineno == 1 + listsize:
                 proc.errmsg("Already at start of %s." % proc.list_filename)
                 return INVALID_PARSE_LIST
-            first = max(1, proc.list_lineno - (2*listsize) - 1)
-        elif text == '':
+            first = max(1, proc.list_lineno - (2 * listsize) - 1)
+        elif text == "":
             # Continue from where we last left off
             first = proc.list_offset + 1
             last = first + listsize - 1
             return filename, first, True, last, True, proc.list_object
         last = first + listsize - 1
         return filename, first, True, last, True, proc.list_object
     else:
@@ -70,88 +77,106 @@
 
         if list_range.first is None:
             # Last must have been given
             assert isinstance(list_range.last, Location)
             location = resolve_address_location(proc, list_range.last)
             if not location:
                 return INVALID_PARSE_LIST
-            last     = location.line_number
+            last = location.line_number
             if location.is_address:
                 raise RuntimeError("We don't handle ending offsets")
             else:
-                first    = max(1, last - listsize)
+                first = max(1, last - listsize)
             return location.path, first, False, last, False, location.method
         elif isinstance(list_range.first, int):
-            first    = list_range.first
+            first = list_range.first
             location = resolve_address_location(proc, list_range.last)
             if not location:
                 return INVALID_PARSE_LIST
             filename = location.path
-            last     = location.line_number
+            last = location.line_number
 
             if not location.is_address and last < first:
                 # Treat as a count rather than an absolute location
                 last = first + last
-            return location.path, first, False, last, location.is_address, location.method
+            return (
+                location.path,
+                first,
+                False,
+                last,
+                location.is_address,
+                location.method,
+            )
         else:
             # First is location. Last may be empty or a number/address
             assert isinstance(list_range.first, Location)
             location = resolve_address_location(proc, list_range.first)
             if not location:
                 return INVALID_PARSE_LIST
-            first    = location.line_number
+            first = location.line_number
             first_is_addr = location.is_address
-            last_is_addr  = False
-            last     = list_range.last
+            last_is_addr = False
+            last = list_range.last
             if isinstance(last, str):
                 # Is an offset +number
-                assert last[0] in ('+', '*')
-                last_is_addr = last[0] == '*'
+                assert last[0] in ("+", "*")
+                last_is_addr = last[0] == "*"
                 if last_is_addr:
                     last = int(last[1:])
                 else:
                     last = first + int(last[1:])
             elif not last:
                 last_is_addr = first_is_addr
                 last = first + listsize
             elif last < first:
                 # Treat as a count rather than an absolute location
                 last = first + last
 
-            return location.path, first, first_is_addr, last, last_is_addr, location.method
+            return (
+                location.path,
+                first,
+                first_is_addr,
+                last,
+                last_is_addr,
+                location.method,
+            )
         pass
     return
 
+
 # Demo it
-if __name__=='__main__':
+if __name__ == "__main__":
     from trepan.processor.command import mock as Mmock
     from trepan.processor.cmdproc import CommandProcessor
     import sys
+
     d = Mmock.MockDebugger()
     cmdproc = CommandProcessor(d.core)
     # print '-' * 10
     # print_source_line(sys.stdout.write, 100, 'source_line_test.py')
     # print '-' * 10
     cmdproc.frame = sys._getframe()
     cmdproc.setup()
 
     def five():
         return 5
-    import os
+
+    import os  # noqa
+
     for cmd in (
-            # "disasm",
-            # "disasm +",
-            # "disasm -",
-            "disasm *5, *10",
-            "disasm *15, 10",
-            "disasm five(), *10",
-            # "disasm 9 , 5",
-            # "disasm 7 ,",
-            # "disasm '''c:\\tmp\\foo.bat''':1",
-            # 'disasm """/Users/My Documents/foo.py""":2',
-            # 'disasm build_range()',
-            # 'disasm os:1 ,',
-            ):
-        args = cmd.split(' ')
+        # "disasm",
+        # "disasm +",
+        # "disasm -",
+        "disasm *5, *10",
+        "disasm *15, 10",
+        "disasm five(), *10",
+        # "disasm 9 , 5",
+        # "disasm 7 ,",
+        # "disasm '''c:\\tmp\\foo.bat''':1",
+        # 'disasm """/Users/My Documents/foo.py""":2',
+        # 'disasm build_range()',
+        "disasm os:1 ,",
+    ):
+        args = cmd.split(" ")
         cmdproc.current_command = cmd
         print(parse_addr_list_cmd(cmdproc, args))
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/cmdbreak.py` & `trepan3k-1.2.9/trepan/processor/cmdbreak.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-#  Copyright (C) 2009-2010, 2013, 2015-2018, 2020 Rocky Bernstein
+#  Copyright (C) 2009-2010, 2013, 2015-2018, 2020, 2022 Rocky Bernstein
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -31,16 +31,17 @@
     condition,
     temporary,
     args,
     force=False,
     offset=None,
 ):
     if lineno is None and offset is None:
-        part1 = "I don't understand '%s' as a line number, offset, or function name," % " ".join(
-            args[1:]
+        part1 = (
+            "I don't understand '%s' as a line number, offset, or function name,"
+            % " ".join(args[1:])
         )
         msg = wrapped_lines(
             part1, "or file/module plus line number.", cmd_obj.settings["width"]
         )
         cmd_obj.errmsg(msg)
         return False
     if filename is None:
@@ -78,37 +79,37 @@
         pass
     bp = cmd_obj.core.bpmgr.add_breakpoint(
         filename,
         lineno=lineno,
         offset=offset,
         temporary=temporary,
         condition=condition,
-        func=func)
+        func=func,
+    )
     if func and inspect.isfunction(func):
         cmd_obj.msg(
             "Breakpoint %d set on calling function %s()" % (bp.number, func.__name__)
         )
         part1 = "Currently this is line %d of file" % lineno
         msg = wrapped_lines(
             part1, cmd_obj.core.filename(filename), cmd_obj.settings["width"]
         )
         cmd_obj.msg(msg)
     else:
-        part1 = ("Breakpoint %d set at line %d of file" %
-                 (bp.number, lineno))
+        part1 = "Breakpoint %d set at line %d of file" % (bp.number, lineno)
         msg = wrapped_lines(
             part1, cmd_obj.core.filename(filename), cmd_obj.settings["width"]
         )
         cmd_obj.msg(msg)
         if func:
             func_str = " of %s" % pretty_modfunc_name(func)
         else:
             func_str = ""
         if offset is not None and offset >= 0:
-            cmd_obj.msg("Breakpoint is at offset %d%s "% (offset, func_str))
+            cmd_obj.msg("Breakpoint is at offset %d%s " % (offset, func_str))
         pass
     return True
 
 
 INVALID_PARSE_BREAK = (None, None, None, None, None)
 
 
@@ -137,15 +138,20 @@
             proc.errmsg(e.text)
             proc.errmsg(e.text_cursor)
             return INVALID_PARSE_BREAK
 
         location = bp_expr.location
         condition = bp_expr.condition
 
-    location = resolve_location(proc, location)
+    try:
+        location = resolve_location(proc, location)
+    except ValueError as e:
+        proc.errmsg(str(e))
+        return INVALID_PARSE_BREAK
+
     if location:
         return (
             location.method,
             location.path,
             location.line_number,
             condition,
             location.offset,
```

### Comparing `trepan3k-1.2.8/trepan/processor/cmdfns.py` & `trepan3k-1.2.9/trepan/processor/cmdfns.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2013, 2015, 2017-2018, 2020-2021 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2013, 2015, 2017-2018, 2020-2021, 2023 Rocky
+#   Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -13,17 +15,18 @@
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """ Common command-parsing routines such as check command argument
 counts, to parse a string for an integer, or check a string for an
 on/off setting value.
 """
-import os, sys, tempfile
-import pyficache
-from xdis import IS_PYPY, PYTHON_VERSION
+import sys
+import tempfile
+
+from xdis import IS_PYPY, PYTHON_VERSION_TRIPLE
 
 
 def source_tempfile_remap(prefix, text, tempdir=None):
     fd = tempfile.NamedTemporaryFile(
         suffix=".py", prefix=prefix, dir=tempdir, delete=False
     )
     with fd:
@@ -31,31 +34,29 @@
         fd.close()
         pass
     return fd.name
 
 
 def deparse_fn(code):
     try:
-        if 3.7 <= PYTHON_VERSION <= 3.8:
+        if (3, 7) <= PYTHON_VERSION_TRIPLE <= (3, 8):
             from uncompyle6.semantics.linemap import (
                 deparse_code_with_fragments_and_map as deparse_code,
             )
         else:
             from decompile3.semantics.linemap import (
                 deparse_code_with_fragments_and_map as deparse_code,
             )
 
     except ImportError:
         return None
-    sys_version = sys.version[:5]
     try:
-        float_version = py_str2float(sys_version)
-        deparsed = deparse_code(float_version, code, is_pypy=IS_PYPY)
+        deparsed = deparse_code(PYTHON_VERSION_TRIPLE, code, is_pypy=IS_PYPY)
         return deparsed
-    except:
+    except Exception:
         raise
     return None
 
 
 def get_an_int(errmsg, arg, msg_on_error, min_value=None, max_value=None):
     """Another get_int() routine, this one simpler and less stylized
     than get_int(). We eval arg return it as an integer value or
@@ -127,15 +128,15 @@
         errmsg("Expecting 'on', 1, 'off', or 0. Got: %s." % str(arg))
     raise ValueError
 
 
 def get_val(curframe, errmsg, arg):
     try:
         return eval(arg, curframe.f_globals, curframe.f_locals)
-    except:
+    except Exception:
         t, v = sys.exc_info()[:2]
         if isinstance(t, str):
             exc_type_name = t
         else:
             exc_type_name = t.__name__
         errmsg(str("%s: %s" % (exc_type_name, arg)))
         raise
@@ -193,15 +194,21 @@
         return "on"
     return "off"
 
 
 def run_show_val(obj, name):
     """Generic subcommand value display"""
     val = obj.debugger.settings[obj.name]
-    obj.msg("%s is %s." % (obj.name, obj.cmd.proc._saferepr(val),))
+    obj.msg(
+        "%s is %s."
+        % (
+            obj.name,
+            obj.cmd.proc._saferepr(val),
+        )
+    )
     return False
 
 
 def want_different_line(cmd, default):
     if cmd[-1] == "-":
         return False
     elif cmd[-1] == "+":
```

### Comparing `trepan3k-1.2.8/trepan/processor/cmdlist.py` & `trepan3k-1.2.9/trepan/processor/cmdlist.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,38 +16,40 @@
 
 from trepan.processor.parse.semantics import build_location, build_range, Location
 from trepan.processor.parse.parser import LocationError
 from trepan.processor.parse.scanner import ScannerError
 from trepan.processor.location import resolve_location
 
 INVALID_PARSE_LIST = (None, None, None)
+
+
 def parse_list_cmd(proc, args, listsize=10):
     """Parses arguments for the "list" command and returns the tuple:
     (filename, first line number, last line number)
     or sets these to None if there was some problem."""
 
-    text = proc.current_command[len(args[0])+1:].strip()
+    text = proc.current_command[len(args[0]) + 1 :].strip()
 
-    if text in frozenset(('', '.', '+', '-')):
-        if text == '.':
-            location = resolve_location(proc, '.')
+    if text in frozenset(("", ".", "+", "-")):
+        if text == ".":
+            location = resolve_location(proc, ".")
             return location.path, location.line_number, listsize
         else:
             if proc.list_lineno is None:
                 proc.errmsg("Don't have previous list location")
                 return INVALID_PARSE_LIST
             filename = proc.list_filename
-            if text == '+':
+            if text == "+":
                 first = max(1, proc.list_lineno + listsize)
-            elif text == '-':
+            elif text == "-":
                 if proc.list_lineno == 1 + listsize:
                     proc.errmsg("Already at start of %s." % proc.list_filename)
                     return INVALID_PARSE_LIST
-                first = max(1, proc.list_lineno - (2*listsize) - 1)
-            elif text == '':
+                first = max(1, proc.list_lineno - (2 * listsize) - 1)
+            elif text == "":
                 # Continue from where we last left off
                 first = proc.list_lineno + 1
         last = first + listsize - 1
         return filename, first, last
     else:
         try:
             list_range = build_range(text)
@@ -64,63 +66,66 @@
 
         if list_range.first is None:
             # Last must have been given
             assert isinstance(list_range.last, Location)
             location = resolve_location(proc, list_range.last)
             if not location:
                 return INVALID_PARSE_LIST
-            last     = location.line_number
-            first    = max(1, last - listsize)
+            last = location.line_number
+            first = max(1, last - listsize)
             return location.path, first, last
         elif isinstance(list_range.first, int):
-            first    = list_range.first
+            first = list_range.first
             location = resolve_location(proc, list_range.last)
             if not location:
                 return INVALID_PARSE_LIST
             filename = location.path
-            last     = location.line_number
+            last = location.line_number
             if last < first:
                 # Treat as a count rather than an absolute location
                 last = first + last
             return location.path, first, last
         else:
             # First is location. Last may be empty or a number
             assert isinstance(list_range.first, Location)
             location = resolve_location(proc, list_range.first)
             if not location:
                 return INVALID_PARSE_LIST
-            first    = location.line_number
-            last     = list_range.last
+            first = location.line_number
+            last = list_range.last
             if location.method:
                 first -= listsize // 2
             if isinstance(last, str):
                 # Is an offset +number
-                assert last[0] == '+'
+                assert last[0] == "+"
                 last = first + int(last[1:])
             elif not last:
                 last = first + listsize
             elif last < first:
                 # Treat as a count rather than an absolute location
                 last = first + last
 
             return location.path, first, last
         pass
     return
 
+
 INVALID_PARSE_LOCATION = (None, None)
+
+
 def parse_location(proc, args):
-    text = proc.current_command[len(args[0])+1:].strip()
+    text = proc.current_command[len(args[0]) + 1 :].strip()
 
-    if text in frozenset(('', '.')):
-        if text == '.':
-            location = resolve_location(proc, '.')
+    if text in frozenset(("", ".")):
+        if text == ".":
+            location = resolve_location(proc, ".")
             return location.path, location.line_number
         else:
             filename = proc.list_filename
-            if text == '':
+            if text == "":
                 # Continue from where we last left off
                 first = proc.list_lineno + 1
         return filename, first
     else:
         try:
             location = build_location(text)
         except LocationError as e:
@@ -131,41 +136,45 @@
         except ScannerError as e:
             proc.errmsg("Lexical error in location at or around:")
             proc.errmsg(e.text)
             proc.errmsg(e.text_cursor)
             return INVALID_PARSE_LOCATION
         return location
 
+
 # Demo it
-if __name__=='__main__':
+if __name__ == "__main__":
     from trepan.processor.command import mock as Mmock
     from trepan.processor.cmdproc import CommandProcessor
     import sys
+
     d = Mmock.MockDebugger()
     cmdproc = CommandProcessor(d.core)
     # print '-' * 10
     # print_source_line(sys.stdout.write, 100, 'source_line_test.py')
     # print '-' * 10
     cmdproc.frame = sys._getframe()
     cmdproc.setup()
 
     def five():
         return 5
-    import os
+
+    import os  # noqa
+
     for cmd in (
-            # "list",
-            # "list +",
-            # "list -",
-            # "list 15, 10",
-            "list five()",
-            # "list 9 , 5",
-            # "list 7 ,",
-            # "list '''c:\\tmp\\foo.bat''':1",
-            # 'list """/Users/My Documents/foo.py""":2',
-            # 'list build_range()',
-            # 'list os:1 ,',
-            'list os.path:9 ,',
-            ):
-        args = cmd.split(' ')
+        # "list",
+        # "list +",
+        # "list -",
+        # "list 15, 10",
+        "list five()",
+        # "list 9 , 5",
+        # "list 7 ,",
+        # "list '''c:\\tmp\\foo.bat''':1",
+        # 'list """/Users/My Documents/foo.py""":2',
+        # 'list build_range()',
+        # 'list os:1 ,',
+        "list os.path:9 ,",
+    ):
+        args = cmd.split(" ")
         cmdproc.current_command = cmd
         print(parse_list_cmd(cmdproc, args))
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/cmdproc.py` & `trepan3k-1.2.9/trepan/processor/cmdproc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2008-2010, 2013-2021 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2008-2010, 2013-2021, 2023 Rocky Bernstein
+#   <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import inspect, linecache, sys, shlex, tempfile, traceback, re
-import os.path as osp
-import pyficache
 import importlib
-from trepan.processor import cmdfns
-from trepan.lib.deparse import deparse_and_cache
+import inspect
+import linecache
+import os.path as osp
+import re
+import shlex
+import sys
+import tempfile
+import traceback
 
 # Note: the module name pre 3.2 is repr
 from reprlib import Repr
 
+import pyficache
 from pygments.console import colorize
-
 from tracer import EVENT2SHORT
 
-from trepan.vprocessor import Processor
-from trepan.lib.bytecode import is_def_stmt, is_class_def
 import trepan.exception as Mexcept
 import trepan.lib.display as Mdisplay
-import trepan.misc as Mmisc
 import trepan.lib.file as Mfile
 import trepan.lib.stack as Mstack
 import trepan.lib.thred as Mthread
+import trepan.misc as Mmisc
 import trepan.processor.complete as Mcomplete
-
+from trepan.lib.bytecode import is_class_def, is_def_stmt
+from trepan.lib.deparse import deparse_and_cache
+from trepan.processor import cmdfns
 from trepan.processor.cmdfns import deparse_fn
+from trepan.vprocessor import Processor
 
 warned_file_mismatches = set()
 
 
 def get_srcdir():
     filename = osp.normcase(osp.dirname(osp.abspath(__file__)))
     return osp.realpath(filename)
@@ -77,19 +83,26 @@
 
 def get_stack(f, t, botframe, proc_obj=None):
     """Return a stack of frames which the debugger will use for in
     showing backtraces and in frame switching. As such various frame
     that are really around may be excluded unless we are debugging the
     sebugger. Also we will add traceback frame on top if that
     exists."""
-    exclude_frame = lambda f: False
+
+    def false_fn(f):
+        return false_fn
+
+    def fn_is_ignored(f):
+        return proc_obj.core.ignore_filter.is_included(f)
+
+    exclude_frame = false_fn
     if proc_obj:
         settings = proc_obj.debugger.settings
         if not settings["dbg_trepan"]:
-            exclude_frame = lambda f: proc_obj.core.ignore_filter.is_included(f)
+            exclude_frame = fn_is_ignored
             pass
         pass
     stack = []
     if t and t.tb_frame is f:
         t = t.tb_next
     while f is not None:
         if exclude_frame(f):
@@ -123,15 +136,15 @@
             command_name = obj.aliases[command_name]
             pass
         else:
             return None
         pass
     try:
         return command_name.lower()
-    except:
+    except Exception:
         return None
     return
 
 
 def print_source_line(msg, lineno, line, event_str=None):
     """Print out a source line of text , e.g. the second
     line in:
@@ -323,15 +336,15 @@
 
         try:
             match, reason = Mstack.check_path_with_frame(frame, filename)
             if not match:
                 if filename not in warned_file_mismatches:
                     proc_obj.errmsg(reason)
                     warned_file_mismatches.add(filename)
-        except:
+        except Exception:
             pass
 
         fn_name = frame.f_code.co_name
         last_i = frame.f_lasti
         print_source_location_info(
             intf_obj.msg,
             filename,
@@ -356,15 +369,15 @@
         pass
     elif (
         proc_obj.event == "call"
         and proc_obj.curframe.f_locals.get("__name__", "") != "__main__"
     ):
         try:
             proc_obj.commands["info"].run(["info", "locals"])
-        except:
+        except Exception:
             pass
     return True
 
 
 # Default settings for command processor method call
 DEFAULT_PROC_OPTS = {
     # A list of debugger initialization files to read on first command
@@ -372,15 +385,18 @@
     # front-end sets.
     "initfile_list": []
 }
 
 
 class CommandProcessor(Processor):
     def __init__(self, core_obj, opts=None):
-        get_option = lambda key: Mmisc.option_set(opts, key, DEFAULT_PROC_OPTS)
+        def get_option_fn(key):
+            return Mmisc.option_set(opts, key, DEFAULT_PROC_OPTS)
+
+        get_option = get_option_fn
         super().__init__(core_obj)
 
         self.continue_running = False  # True if we should leave command loop
         self.event2short = dict(EVENT2SHORT)
         self.event2short["signal"] = "?!"
         self.event2short["brkpt"] = "xx"
 
@@ -537,27 +553,27 @@
         self.set_prompt(prompt)
         self.process_commands()
         if filename == "<string>":
             pyficache.remove_remap_file("<string>")
         return self.event_processor
 
     def forget(self):
-        """ Remove memory of state variables set in the command processor """
+        """Remove memory of state variables set in the command processor"""
         self.stack = []
         self.curindex = 0
         self.curframe = None
         self.thread_name = None
         self.frame_thread_name = None
         return
 
     def eval(self, arg, show_error=True):
         """Eval string arg in the current frame context."""
         try:
             return eval(arg, self.curframe.f_globals, self.curframe.f_locals)
-        except:
+        except Exception:
             t, v = sys.exc_info()[:2]
             if isinstance(t, str):
                 exc_type_name = t
                 pass
             else:
                 exc_type_name = t.__name__
             if show_error:
@@ -575,15 +591,15 @@
             # user can store variables inside the debug session.
             # The setup for this should be elsewhere. Possibly
             # in interaction.
             global_vars = None
         try:
             code = compile(line + "\n", '"%s"' % line, "single")
             exec(code, global_vars, local_vars)
-        except:
+        except Exception:
             t, v = sys.exc_info()[:2]
             if type(t) == bytes:
                 exc_type_name = t
             else:
                 exc_type_name = t.__name__
             self.errmsg("%s: %s" % (str(exc_type_name), str(v)))
             pass
@@ -615,21 +631,21 @@
         return ret_value
 
     def get_int_noerr(self, arg):
         """Eval arg and it is an integer return the value. Otherwise
         return None"""
         if self.curframe:
             g = self.curframe.f_globals
-            l = self.curframe.f_locals
+            locals_dict = self.curframe.f_locals
         else:
             g = globals()
-            l = locals()
+            locals_dict = locals()
             pass
         try:
-            val = int(eval(arg, g, l))
+            val = int(eval(arg, g, locals_dict))
         except (SyntaxError, NameError, ValueError, TypeError):
             return None
         return val
 
     def get_int(self, arg, min_value=0, default=1, cmdname=None, at_most=None):
         """If no argument use the default. If arg is a an integer between
         least min_value and at_most, use that. Otherwise report an error.
@@ -677,15 +693,15 @@
         return default
 
     def getval(self, arg, locals=None):
         if not locals:
             locals = self.curframe.f_locals
         try:
             return eval(arg, self.curframe.f_globals, locals)
-        except:
+        except Exception:
             t, v = sys.exc_info()[:2]
             if isinstance(t, str):
                 exc_type_name = t
             else:
                 exc_type_name = t.__name__
             self.errmsg(str("%s: %s" % (exc_type_name, arg)))
             raise
@@ -780,15 +796,15 @@
                 self.errmsg("No previous command registered, " + "so this is a no-op.")
                 pass
             return False
         if current_command is None or current_command[0] == "#":
             return False
         try:
             args_list = arg_split(current_command)
-        except:
+        except Exception:
             self.errmsg("bad parse %s: %s" % sys.exc_info()[0:2])
             return False
 
         for args in args_list:
             if len(args):
                 while True:
                     if len(args) == 0:
@@ -855,15 +871,15 @@
                         except (
                             Mexcept.DebuggerQuit,
                             Mexcept.DebuggerRestart,
                             SystemExit,
                         ):
                             # Let these exceptions propagate through
                             raise
-                        except:
+                        except Exception:
                             self.errmsg("INTERNAL ERROR: " + traceback.format_exc())
                             pass
                         pass
                     pass
                 elif not self.settings("autoeval"):
                     self.undefined_cmd(current_command)
                 else:
@@ -982,15 +998,15 @@
                     pass
             except ImportError:
                 pass
             pass
         return
 
     def _populate_commands(self):
-        """ Create an instance of each of the debugger
+        """Create an instance of each of the debugger
         commands. Commands are found by importing files in the
         directory 'command'. Some files are excluded via an array set
         in __init__.  For each of the remaining files, we import them
         and scan for class names inside those files and for each class
         name, we will create an instance of that class. The set of
         DebuggerCommand class instances form set of possible debugger
         commands."""
@@ -1005,22 +1021,26 @@
         cmd_instances = []
         eval_cmd_template = "command_mod.%s(self)"
         for mod_name in Mcommand.__dict__.keys():
             if mod_name.startswith("__"):
                 continue
             import_name = "trepan.processor.command." + mod_name
             imp = __import__(import_name)
-            if imp.__name__ == base_name:
+            if imp.__name__ == mod_name:
                 command_mod = imp.processor.command
             else:
-                if mod_name in ("info_sub", "set_sub", "show_sub",):
+                if mod_name in (
+                    "info_sub",
+                    "set_sub",
+                    "show_sub",
+                ):
                     pass
                 try:
                     command_mod = getattr(__import__(import_name), mod_name)
-                except:
+                except Exception:
                     # Don't need to warn about optional modules
                     if mod_name not in self.optional_modules:
                         print("Error importing %s: %s" % (mod_name, sys.exc_info()[0]))
                         pass
                     continue
                 pass
 
@@ -1034,15 +1054,15 @@
                 if False:
                     instance = eval(eval_cmd)
                     cmd_instances.append(instance)
                 else:
                     try:
                         instance = eval(eval_cmd)
                         cmd_instances.append(instance)
-                    except:
+                    except Exception:
                         print(
                             "Error loading %s from %s: %s"
                             % (classname, mod_name, sys.exc_info()[0])
                         )
                         pass
                     pass
                 pass
@@ -1054,20 +1074,24 @@
         """
         Add files in filesystem to self.commands.
         If running from source or from an easy_install'd package, this is used.
         """
         cmd_instances = []
 
         for mod_name in Mcommand.__modules__:
-            if mod_name in ("info_sub", "set_sub", "show_sub",):
+            if mod_name in (
+                "info_sub",
+                "set_sub",
+                "show_sub",
+            ):
                 pass
             import_name = "%s.%s" % (Mcommand.__name__, mod_name)
             try:
                 command_mod = importlib.import_module(import_name)
-            except:
+            except Exception:
                 if mod_name not in self.optional_modules:
                     print("Error importing %s: %s" % (mod_name, sys.exc_info()[0]))
                     pass
                 continue
 
             classnames = [
                 tup[0]
@@ -1078,28 +1102,28 @@
                 if False:
                     instance = getattr(command_mod, classname)(self)
                     cmd_instances.append(instance)
                 else:
                     try:
                         instance = getattr(command_mod, classname)(self)
                         cmd_instances.append(instance)
-                    except:
+                    except Exception:
                         print(
                             "Error loading %s from %s: %s"
                             % (classname, mod_name, sys.exc_info()[0])
                         )
                         pass
                     pass
                 pass
             pass
         return cmd_instances
 
     def _populate_cmd_lists(self):
-        """ Populate self.lists and hashes:
-        self.commands, and self.aliases, self.category """
+        """Populate self.lists and hashes:
+        self.commands, and self.aliases, self.category"""
         self.commands = {}
         self.aliases = {}
         self.category = {}
         #         self.short_help = {}
         for cmd_instance in self.cmd_instances:
             if not hasattr(cmd_instance, "aliases"):
                 continue
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/__init__.py` & `trepan3k-1.2.9/trepan/processor/command/__init__.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/trepan/processor/command/alias.py` & `trepan3k-1.2.9/trepan/processor/command/alias.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,34 +16,34 @@
 # Our local modules
 from trepan.processor.command.base_cmd import DebuggerCommand
 
 
 class AliasCommand(DebuggerCommand):
     """**alias** *alias-name* *debugger-command*
 
-Add alias *alias-name* for a debugger command *debugger-command*.  You
-might do this if you want shorter command names or more commands that
-have more familiar meanings.
-
-Another related use is as a command abbreviation for a command that
-would otherwise be ambiguous. For example, by default we make `s` be
-an alias of `step` to force it to be used. Without the alias, `s`
-might be `step`, `show`, or `set` among others.
-
-Examples:
---------
-
-    alias cat list   # "cat prog.py" is the same as "list prog.py"
-    alias s   step   # "s" is now an alias for "step".
-                     # The above example is done by default.
+    Add alias *alias-name* for a debugger command *debugger-command*.  You
+    might do this if you want shorter command names or more commands that
+    have more familiar meanings.
+
+    Another related use is as a command abbreviation for a command that
+    would otherwise be ambiguous. For example, by default we make `s` be
+    an alias of `step` to force it to be used. Without the alias, `s`
+    might be `step`, `show`, or `set` among others.
+
+    Examples:
+    --------
+
+        alias cat list   # "cat prog.py" is the same as "list prog.py"
+        alias s   step   # "s" is now an alias for "step".
+                         # The above example is done by default.
 
-See also:
----------
+    See also:
+    ---------
 
-`unalias` and `show alias`.
+    `unalias` and `show alias`.
     """
 
     name = "alias"
     short_help = "Add an alias for a debugger command"
 
     DebuggerCommand.setup(locals(), category="support", max_args=2, need_stack=True)
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/backtrace.py` & `trepan3k-1.2.9/trepan/processor/command/backtrace.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,46 +20,45 @@
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.lib import stack as Mstack
 
 
 class BacktraceCommand(DebuggerCommand):
     """**backtrace** [*options*] [*count*]
 
-Print backtrace of all stack frames, or innermost *count* frames.
+    Print backtrace of all stack frames, or innermost *count* frames.
 
-With a negative argument, print outermost -*count* frames.
+    With a negative argument, print outermost -*count* frames.
 
-An arrow indicates the 'current frame'. The current frame determines
-the context used for many debugger commands such as expression
-evaluation or source-line listing.
-
-*options* are:
-
-   -d | --deparse - show deparsed call position
-   -s | --source  - show source code line
-   -f | --full    - locals of each frame
-   -h | --help    - give this help
-
-Examples:
----------
-
-   backtrace      # Print a full stack trace
-   backtrace 2    # Print only the top two entries
-   backtrace -1   # Print a stack trace except the initial (least recent) call.
-   backtrace -s   # show source lines in listing
-   backtrace -d   # show deparsed source lines in listing
-   backtrace -f   # show with locals
-   backtrace -df  # show with deparsed calls and locals
-   backtrace --deparse --full   # same as above
+    An arrow indicates the 'current frame'. The current frame determines
+    the context used for many debugger commands such as expression
+    evaluation or source-line listing.
 
-See also:
----------
+    *options* are:
 
-`frame`, `locals`, `global`, `deparse`, `list`.
-"""
+       -d | --deparse - show deparsed call position
+       -s | --source  - show source code line
+       -f | --full    - locals of each frame
+       -h | --help    - give this help
+
+    Examples:
+    ---------
+
+       backtrace      # Print a full stack trace
+       backtrace 2    # Print only the top two entries
+       backtrace -1   # Print a stack trace except the initial (least recent) call.
+       backtrace -s   # show source lines in listing
+       backtrace -d   # show deparsed source lines in listing
+       backtrace -f   # show with locals
+       backtrace -df  # show with deparsed calls and locals
+       backtrace --deparse --full   # same as above
+
+    See also:
+    ---------
+
+    `frame`, `locals`, `global`, `deparse`, `list`."""
 
     aliases = ("bt", "where")
     short_help = "Print backtrace of stack frames"
 
     DebuggerCommand.setup(locals(), category="stack", max_args=4, need_stack=True)
 
     def run(self, args):
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/base_cmd.py` & `trepan3k-1.2.9/trepan/processor/command/base_cmd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
-#  Copyright (C) 2009-2010, 2012-2013, 2015, 2021 Rocky Bernstein
+#
+#  Copyright (C) 2009-2010, 2012-2013, 2015, 2021, 2023 Rocky
+#  Bernstein
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
@@ -16,37 +18,37 @@
 """A base class for debugger commands.
 
 This file is the one module in this directory that isn't a real command
 and commands.py needs to take care to avoid instantiating this class
 and storing it as a list of known debugger commands.
 """
 
-NotImplementedMessage = "This method must be overriden in a subclass"
-
 import columnize
 from pygments.console import colorize
 
 from trepan.lib import format as Mformat
 
+NotImplementedMessage = "This method must be overridden in a subclass"
+
 __all__ = ["DebuggerCommand"]
 
 
 class DebuggerCommand:
     """Base Class for Debugger commands. We pull in some helper
     functions for command from module cmdfns."""
 
     category = "misc"
 
     @staticmethod
-    def setup(l, category="misc", min_args=0, max_args=None, need_stack=False):
-        l["name"] = l["__module__"].split(".")[-1]
-        l["category"] = category
-        l["min_args"] = min_args
-        l["max_args"] = max_args
-        l["need_stack"] = need_stack
+    def setup(local_dict, category="misc", min_args=0, max_args=None, need_stack=False):
+        local_dict["name"] = local_dict["__module__"].split(".")[-1]
+        local_dict["category"] = category
+        local_dict["min_args"] = min_args
+        local_dict["max_args"] = max_args
+        local_dict["need_stack"] = need_stack
         return
 
     def __init__(self, proc):
         """proc contains the command processor object that this
         command is invoked through.  A debugger field gives access to
         the stack frame and I/O."""
         self.proc = proc
@@ -67,43 +69,43 @@
     def columnize_commands(self, commands):
         """List commands arranged in an aligned columns"""
         commands.sort()
         width = self.debugger.settings["width"]
         return columnize.columnize(commands, displaywidth=width, lineprefix="    ")
 
     def confirm(self, msg, default=False):
-        """ Convenience short-hand for self.debugger.intf[-1].confirm """
+        """Convenience short-hand for self.debugger.intf[-1].confirm"""
         return self.debugger.intf[-1].confirm(msg, default)
 
     # Note for errmsg, msg, and msg_nocr we don't want to simply make
     # an assignment of method names like self.msg = self.debugger.intf.msg,
     # because we want to allow the interface (intf) to change
     # dynamically. That is, the value of self.debugger may change
-    # in the course of the program and if we made such an method assignemnt
+    # in the course of the program and if we made such an method assignment
     # we wouldn't pick up that change in our self.msg
     def errmsg(self, msg, opts={}):
-        """ Convenience short-hand for self.debugger.intf[-1].errmsg """
+        """Convenience short-hand for self.debugger.intf[-1].errmsg"""
         try:
             return self.debugger.intf[-1].errmsg(msg)
         except EOFError:
             # FIXME: what do we do here?
             pass
         return None
 
     def msg(self, msg, opts={}):
-        """ Convenience short-hand for self.debugger.intf[-1].msg """
+        """Convenience short-hand for self.debugger.intf[-1].msg"""
         try:
             return self.debugger.intf[-1].msg(msg)
         except EOFError:
             # FIXME: what do we do here?
             pass
         return None
 
     def msg_nocr(self, msg: str, opts={}):
-        """ Convenience short-hand for self.debugger.intf[-1].msg_nocr """
+        """Convenience short-hand for self.debugger.intf[-1].msg_nocr"""
         try:
             return self.debugger.intf[-1].msg_nocr(msg[:1000])
         except EOFError:
             # FIXME: what do we do here?
             pass
         return None
 
@@ -113,15 +115,15 @@
             text,
             "plain" == self.debugger.settings["highlight"],
             self.debugger.settings["width"],
         )
         return self.msg(text)
 
     def run(self, args):
-        """ The method that implements the debugger command.
+        """The method that implements the debugger command.
         Help on the command comes from the docstring of this method.
         """
         raise NotImplementedError(NotImplementedMessage)
 
     pass
 
     def section(self, message, opts={}):
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/base_subcmd.py` & `trepan3k-1.2.9/trepan/processor/command/base_subcmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009-2010, 2012-2013, 2015-2016, 2020 Rocky Bernstein
+#
+#   Copyright (C) 2009-2010, 2012-2013, 2015-2016, 2020, 2023 Rocky
+#   Bernstein
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -16,18 +18,24 @@
 """A base class for debugger subcommands.
 
 This file is a module in this directory that isn't a real command
 and commands.py needs to take care to avoid instantiating this class
 and storing it as a list of known debugger commands.
 """
 
-NotImplementedMessage = "This method must be overriden in a subclass"
-import columnize, re
+import re
+
+import columnize
 from pygments.console import colorize
 
+from trepan.lib.complete import complete_token
+from trepan.processor.cmdfns import run_set_bool, run_show_bool, run_show_int
+
+NotImplementedMessage = "This method must be overridden in a subclass"
+
 
 # Note: don't end classname with Command (capital C) since cmdproc
 # will think this a command name like QuitCommand
 #                                         ^
 class DebuggerSubcommand:
     """Base Class for Debugger subcommands. We pull in some helper
     functions for command from module cmdfns."""
@@ -82,44 +90,44 @@
     def columnize_commands(self, commands):
         """List commands arranged in an aligned columns"""
         commands.sort()
         width = self.debugger.settings["width"]
         return columnize.columnize(commands, displaywidth=width, lineprefix="    ")
 
     def confirm(self, msg, default=False):
-        """ Convenience short-hand for self.debugger.intf.confirm """
+        """Convenience short-hand for self.debugger.intf.confirm"""
         return self.debugger.intf[-1].confirm(msg, default)
 
     # Note for errmsg, msg, and msg_nocr we don't want to simply make
     # an assignment of method names like self.msg = self.debugger.intf.msg,
     # because we want to allow the interface (intf) to change
     # dynamically. That is, the value of self.debugger may change
-    # in the course of the program and if we made such an method assignemnt
+    # in the course of the program and if we made such an method assignment
     # we wouldn't pick up that change in our self.msg
     def errmsg(self, msg):
-        """ Convenience short-hand for self.debugger.intf[-1].errmsg """
+        """Convenience short-hand for self.debugger.intf[-1].errmsg"""
         return self.debugger.intf[-1].errmsg(msg)
 
     def msg(self, msg):
-        """ Convenience short-hand for self.debugger.intf[-1].msg """
+        """Convenience short-hand for self.debugger.intf[-1].msg"""
         return self.debugger.intf[-1].msg(msg)
 
     def msg_nocr(self, msg):
-        """ Convenience short-hand for self.debugger.intf[-1].msg_nocr """
+        """Convenience short-hand for self.debugger.intf[-1].msg_nocr"""
         return self.debugger.intf[-1].msg_nocr(msg)
 
     aliases = ()
     name = "YourCommandName"
 
     def rst_msg(self, text):
         """Convenience short-hand for self.proc.rst_msg(text)"""
         return self.proc.rst_msg(text)
 
     def run(self):
-        """ The method that implements the debugger command.
+        """The method that implements the debugger command.
         Help on the command comes from the docstring of this method.
         """
         raise NotImplementedError(NotImplementedMessage)
 
     def section(self, message, opts={}):
         if "plain" != self.settings["highlight"]:
             message = colorize("bold", message)
@@ -127,18 +135,14 @@
             message += "\n" + "-" * len(message)
             pass
         self.msg(message)
 
     pass
 
 
-from trepan.processor.cmdfns import run_set_bool, run_show_bool, run_show_int
-from trepan.lib.complete import complete_token
-
-
 class DebuggerSetBoolSubcommand(DebuggerSubcommand):
     max_args = 1
 
     def complete(self, prefix):
         result = complete_token(("on", "off"), prefix)
         return result
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/base_submgr.py` & `trepan3k-1.2.9/trepan/processor/command/base_submgr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2010, 2013, 2015, 2020-2021 Rocky Bernstein
+#
+#  Copyright (C) 2009, 2010, 2013, 2015, 2020-2021, 2023 Rocky Bernstein
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import inspect, re, sys, importlib
+import importlib
+import inspect
+import re
+import sys
 
+from trepan.lib.complete import complete_token, complete_token_with_next
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.processor.subcmd import Subcmd
-from trepan.lib.complete import complete_token, complete_token_with_next
 
 
 def abbrev_stringify(name, min_abbrev):
-    return "(%s)%s" % (name[:min_abbrev], name[min_abbrev:],)
+    return "(%s)%s" % (
+        name[:min_abbrev],
+        name[min_abbrev:],
+    )
 
 
 def capitalize(s):
     # "abcd" -> "Abcd"
     if s:
         return s[0].upper() + s[1:]
     else:  # empty string
@@ -107,15 +114,15 @@
             ]
 
             for classname in classnames:
                 eval_cmd = eval_cmd_template % classname
                 try:
                     instance = eval(eval_cmd)
                     self.cmds.add(instance)
-                except:
+                except Exception:
                     print("Error eval'ing class %s" % classname)
                     pass
                 pass
             pass
         return cmd_instances
 
     def help(self, args):
@@ -168,15 +175,19 @@
             if cmds == []:
                 self.errmsg(
                     "No %s subcommands found matching /^%s/. "
                     'Try "help".' % (self.name, subcmd_name)
                 )
             else:
                 self.section(
-                    'Subcommand(s) of "%s" matching /^%s/:' % (self.name, subcmd_name,)
+                    'Subcommand(s) of "%s" matching /^%s/:'
+                    % (
+                        self.name,
+                        subcmd_name,
+                    )
                 )
                 self.msg_nocr(self.columnize_commands(cmds))
                 pass
             pass
         return
 
     # Return an Array of subcommands that can start with +arg+. If none
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/bpython.py` & `trepan3k-1.2.9/trepan/processor/command/bpython.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,36 +14,36 @@
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 import sys
 
 # Our local modules
 from trepan.processor.command.base_cmd import DebuggerCommand
 
+
 class PythonCommand(DebuggerCommand):
     """**bpython** [**-d**]
 
-Run bpython as a command subshell. The *sys.ps1* prompt will be set to
-`trepan2 >>> `.
+    Run bpython as a command subshell. The *sys.ps1* prompt will be set to
+    `trepan2 >>> `.
 
-If *-d* is passed, you can access debugger state via local variable *debugger*.
+    If *-d* is passed, you can access debugger state via local variable *debugger*.
 
-To issue a debugger command use function *dbgr()*. For example:
+    To issue a debugger command use function *dbgr()*. For example:
 
-  dbgr('info program')
-"""
+      dbgr('info program')"""
 
-    short_help    = 'Run bpython as a command subshell'
+    short_help = "Run bpython as a command subshell"
 
     DebuggerCommand.setup(locals(), category="support", max_args=1)
 
     def dbgr(self, string):
-        '''Invoke a debugger command from inside a python shell called inside
+        """Invoke a debugger command from inside a python shell called inside
         the debugger.
-        '''
-        print('')
+        """
+        print("")
         self.proc.cmd_queue.append(string)
         self.proc.process_command()
         return
 
     def run(self, args):
 
         try:
@@ -58,64 +58,69 @@
         if have_line_edit:
             try:
                 self.proc.write_history_file()
             except IOError:
                 pass
             pass
 
-        banner_tmpl='''trepan2 python shell%s
-Use dbgr(*string*) to issue debugger command: *string*'''
+        banner_tmpl = """trepan2 python shell%s
+Use dbgr(*string*) to issue debugger command: *string*"""
 
-        debug = len(args) > 1 and args[1] == '-d'
+        debug = len(args) > 1 and args[1] == "-d"
         if debug:
-            banner_tmpl += ("\nVariable 'debugger' contains a trepan" +
-                            "debugger object.")
+            banner_tmpl += (
+                "\nVariable 'debugger' contains a trepan" + "debugger object."
+            )
             pass
-        my_locals  = {}
+        my_locals = {}
         # my_globals = None
         if self.proc.curframe:
             # my_globals = self.proc.curframe.f_globals
             if self.proc.curframe.f_locals:
                 my_locals = self.proc.curframe.f_locals
                 pass
             pass
 
         # Give python and the user a way to get access to the debugger.
-        if debug: my_locals['debugger'] = self.debugger
-        my_locals['dbgr'] = self.dbgr
+        if debug:
+            my_locals["debugger"] = self.debugger
+        my_locals["dbgr"] = self.dbgr
 
         if len(my_locals):
-            banner=(banner_tmpl % ' with locals')
+            banner = banner_tmpl % " with locals"
         else:
-            banner=(banner_tmpl % '')
+            banner = banner_tmpl % ""
             pass
 
-        sys.ps1 = 'trepan2 >>> '
+        sys.ps1 = "trepan2 >>> "
         print(banner)
         try:
             main_bpython([], my_locals)
         except SystemExit:
             pass
 
         # restore completion and our history if we can do so.
-        if hasattr(self.proc.intf[-1], 'complete'):
+        if hasattr(self.proc.intf[-1], "complete"):
             try:
                 from readline import set_completer, parse_and_bind
+
                 parse_and_bind("tab: complete")
                 set_completer(self.proc.intf[-1].complete)
             except ImportError:
                 pass
             pass
 
         if have_line_edit:
             self.proc.read_history_file()
             pass
         return
+
     pass
 
+
 # if __name__ == '__main__':
 #     from trepan import debugger as Mdebugger
 #     d = Mdebugger.Debugger()
 #     command = PythonCommand(d.core.processor)
 #     command.proc.frame = sys._getframe()
 #     command.proc.setup()
 #     if len(sys.argv) > 1:
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/break.py` & `trepan3k-1.2.9/trepan/processor/command/break.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,87 +1,95 @@
 # -*- coding: utf-8 -*-
 #
-#  Copyright (C) 2009-2010, 2013-2015, 2017-2018, 2020 Rocky Bernstein
+#  Copyright (C) 2009-2010, 2013-2015, 2017-2018, 2020, 2023 Rocky Bernstein
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from trepan.processor.cmdbreak import parse_break_cmd, set_break
+
 # Our local modules
 from trepan.processor.command.base_cmd import DebuggerCommand
-from trepan.processor.cmdbreak import parse_break_cmd, set_break
 from trepan.processor.complete import complete_break_linenumber
 
 
 class BreakCommand(DebuggerCommand):
     """**break** [*location*] [if *condition*]]
 
-Sets a breakpoint, i.e. stopping point just before the
-execution of the instruction specified by *location*.
+    Sets a breakpoint, i.e. stopping point just before the
+    execution of the instruction specified by *location*.
 
-Without arguments or an empty *location*, the breakpoint is set at the
-current stopped location.
+    Without arguments or an empty *location*, the breakpoint is set at the
+    current stopped location.
 
-See `help syntax location` for detailed information on a location.
+    See `help syntax location` for detailed information on a location.
 
-If the word `if` is given after *location*, subsequent arguments given
-Without arguments or an empty *location*, the breakpoint is set
-the current stopped location.
-
-Normally we only allow stopping at lines that we think are
-stoppable. If the command has a `!` suffix, force the breakpoint anyway.
-
-Examples:
----------
-
-   break                # Break where we are current stopped at
-   break if i < j       # Break at current line if i < j
-   break 10             # Break on line 10 of the file we are
-                        # currently stopped at
-   break! 10            # Break where we are current stopped at, even if
-                        # we don't think line 10 is stoppable
-   break os.path.join() # Break in function os.path.join
-   break x[i].fn()      # break in function specified by x[i].fn
-   break x[i].fn() if x # break in function specified by x[i].fn
-                        # if x is set
-   break os.path:45     # Break on line 45 file holding module os.path
-   break myfile.py:2    # Break on line 2 of myfile.py
-   break myfile.py:2 if i < j # Same as above but only if i < j
-   break "foo's.py":1"  # One way to specify path with a quote
-   break 'c:\\foo.bat':1      # One way to specify a Windows file name,
-   break '/My Docs/foo.py':1  # One way to specify path with blanks in it
+    If the word `if` is given after *location*, subsequent arguments given
+    Without arguments or an empty *location*, the breakpoint is set
+    the current stopped location.
+
+    Normally we only allow stopping at lines that we think are
+    stoppable. If the command has a `!` suffix, force the breakpoint anyway.
+
+    Examples:
+    ---------
+
+       break                # Break where we are current stopped at
+       break if i < j       # Break at current line if i < j
+       break 10             # Break on line 10 of the file we are
+                            # currently stopped at
+       break! 10            # Break where we are current stopped at, even if
+                            # we don't think line 10 is stoppable
+       break os.path.join() # Break in function os.path.join
+       break x[i].fn()      # break in function specified by x[i].fn
+       break x[i].fn() if x # break in function specified by x[i].fn
+                            # if x is set
+       break os.path:45     # Break on line 45 file holding module os.path
+       break myfile.py:2    # Break on line 2 of myfile.py
+       break myfile.py:2 if i < j # Same as above but only if i < j
+       break "foo's.py":1"  # One way to specify path with a quote
+       break 'c:\\foo.bat':1      # One way to specify a Windows file name,
+       break '/My Docs/foo.py':1  # One way to specify path with blanks in it
 
-See also:
----------
+    See also:
+    ---------
 
-`info break`, `tbreak`, `condition` and `help syntax location`."""
+    `info break`, `tbreak`, `condition` and `help syntax location`."""
 
     aliases = ("b", "break!", "b!")
     short_help = "Set breakpoint at specified line or function"
 
     DebuggerCommand.setup(locals(), category="breakpoints", need_stack=True)
 
     complete = complete_break_linenumber
 
     def run(self, args):
         force = True if args[0][-1] == "!" else False
 
         (func, filename, lineno, condition, offset) = parse_break_cmd(self.proc, args)
-        if not (func == None and filename == None):
+        if not (func is None and filename is None):
             set_break(
-                self, func, filename, lineno, condition, False, args, force=force,
-                offset=offset
+                self,
+                func,
+                filename,
+                lineno,
+                condition,
+                False,
+                args,
+                force=force,
+                offset=offset,
             )
         return
 
 
 if __name__ == "__main__":
 
     def do_parse(cmd, a):
@@ -92,14 +100,15 @@
     def do_run(cmd, a):
         name = "break"
         cmd.proc.current_command = name + " " + " ".join(a)
         print(a)
         cmd.run([name] + a)
 
     import sys
+
     from trepan.debugger import Trepan
 
     d = Trepan()
     command = BreakCommand(d.core.processor)
     command.proc.frame = sys._getframe()
     command.proc.setup()
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/cd.py` & `trepan3k-1.2.9/trepan/processor/command/cd.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 # -*- coding: utf-8 -*-
-#  Copyright (C) 2009, 2013-2015, 2020 Rocky Bernstein
+#  Copyright (C) 2009, 2013-2015, 2020, 2023 Rocky Bernstein
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import os, sys
+import os
+import sys
 
 from trepan.processor.command.base_cmd import DebuggerCommand
 
 
 class CDCommand(DebuggerCommand):
     """**cd** *directory*
 
-Set working directory to *directory* for debugger and program
-being debugged. """
+    Set working directory to *directory* for debugger and program
+    being debugged."""
 
     aliases = ("chdir",)
     short_help = (
         "Set working directory to DIR for debugger " "and program being debugged"
     )
 
     DebuggerCommand.setup(
-        locals(), category="files", max_args=1, min_args=1,
+        locals(),
+        category="files",
+        max_args=1,
+        min_args=1,
     )
 
     def run(self, args):
         try:
             os.chdir(args[1])
             self.msg("Working directory %s." % os.getcwd())
         except OSError:
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/clear.py` & `trepan3k-1.2.9/trepan/processor/command/clear.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,21 +20,20 @@
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.processor.complete import complete_bpnumber
 
 
 class ClearCommand(DebuggerCommand):
     """**clear** [*linenumber*]
 
-Clear some breakpoints by line number.
+    Clear some breakpoints by line number.
 
-See also:
----------
-`delete`
-
-"""
+    See also:
+    ---------
+    `delete`
+    """
 
     short_help = "Delete some breakpoints on a line"
 
     DebuggerCommand.setup(locals(), category="breakpoints", need_stack=True)
 
     complete = complete_bpnumber
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/condition.py` & `trepan3k-1.2.9/trepan/processor/command/condition.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,29 +17,29 @@
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.processor.complete import complete_bpnumber
 
 
 class ConditionCommand(DebuggerCommand):
     """**condition** *bp_number* *condition*
 
-*bp_number* is a breakpoint number. *condition* is an expression which
-must evaluate to *True* before the breakpoint is honored.  If *condition*
-is absent, any existing condition is removed; i.e., the breakpoint is
-made unconditional.
+    *bp_number* is a breakpoint number. *condition* is an expression which
+    must evaluate to *True* before the breakpoint is honored.  If *condition*
+    is absent, any existing condition is removed; i.e., the breakpoint is
+    made unconditional.
 
-Examples:
----------
+    Examples:
+    ---------
 
-   condition 5 x > 10  # Breakpoint 5 now has condition x > 10
-   condition 5         # Remove above condition
+       condition 5 x > 10  # Breakpoint 5 now has condition x > 10
+       condition 5         # Remove above condition
 
-See also:
----------
+    See also:
+    ---------
 
-`break`, `tbreak`."""
+    `break`, `tbreak`."""
 
     aliases = ("cond",)
     short_help = "Specify breakpoint number N to break only if COND is True"
 
     DebuggerCommand.setup(locals(), category="breakpoints", min_args=1)
 
     complete = complete_bpnumber
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/continue.py` & `trepan3k-1.2.9/trepan/processor/command/continue.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,36 +17,35 @@
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.processor.cmdbreak import parse_break_cmd, set_break
 
 
 class ContinueCommand(DebuggerCommand):
     """**continue** [*location*]
 
-Leave the debugger read-eval print loop and continue
-execution. Subsequent entry to the debugger however may occur via
-breakpoints or explicit calls, or exceptions.
-
-If *location* is given, a temporary breakpoint is set at that
-position before continuing.
-
-Examples:
----------
-
-    continue          # Continue execution
-    continue 5        # Continue with a one-time breakpoint at line 5
-    continue basename # Go to os.path.basename if we have basename imported
-    continue /usr/lib/python3.8/posixpath.py:110 # Possibly the same as
-                                                 # the above using file
-                                                 # and line number
+    Leave the debugger read-eval print loop and continue
+    execution. Subsequent entry to the debugger however may occur via
+    breakpoints or explicit calls, or exceptions.
+
+    If *location* is given, a temporary breakpoint is set at that
+    position before continuing.
+
+    Examples:
+    ---------
+
+        continue          # Continue execution
+        continue 5        # Continue with a one-time breakpoint at line 5
+        continue basename # Go to os.path.basename if we have basename imported
+        continue /usr/lib/python3.8/posixpath.py:110 # Possibly the same as
+                                                     # the above using file
+                                                     # and line number
 
-See also:
----------
+    See also:
+    ---------
 
-`step` `jump`, `next`, `finish` and `help syntax location`
-"""
+    `step` `jump`, `next`, `finish` and `help syntax location`"""
 
     aliases = ("c",)
     execution_set = ["Running"]
     short_help = "Continue execution of debugged program"
     DebuggerCommand.setup(locals(), category="running", max_args=1, need_stack=True)
 
     def run(self, args):
@@ -80,11 +79,14 @@
     ):
         d.core.step_ignore = 0
         cmd.continue_running = False
         result = cmd.run(c)
         print("Run result: %s" % result)
         print(
             "step_ignore %d, continue_running: %s"
-            % (d.core.step_ignore, cmd.continue_running,)
+            % (
+                d.core.step_ignore,
+                cmd.continue_running,
+            )
         )
         pass
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/debug.py` & `trepan3k-1.2.9/trepan/processor/command/debug.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 # -*- coding: utf-8 -*-
-#  Copyright (C) 2010, 2012-2015, 2020 Rocky Bernstein
+#
+#  Copyright (C) 2010, 2012-2015, 2020, 2023 Rocky Bernstein
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import sys, threading
+import sys
+import threading
+
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.processor.complete import complete_identifier
 
 
 class DebugCommand(DebuggerCommand):
     """**debug** *python-expression*
 
-Enter a nested debugger that steps through the *python-expression* argument
-which is an arbitrary expression to be executed the current
-environment."""
+    Enter a nested debugger that steps through the *python-expression* argument
+    which is an arbitrary expression to be executed the current
+    environment."""
 
     short_help = "Debug *python-expression"
 
     complete = complete_identifier
 
     DebuggerCommand.setup(locals(), category="support", min_args=1, need_stack=True)
 
@@ -59,15 +62,15 @@
 
         self.section("ENTERING NESTED DEBUGGER")
 
         self.core.step_ignore = 2  # call_tracing will stop in itself.
         try:
             ret = sys.call_tracing(eval, (arg, global_vars, local_vars))
             self.msg("R=> %s" % self.proc._saferepr(ret))
-        except:
+        except Exception:
             pass
         self.section("LEAVING NESTED DEBUGGER")
 
         self.core.debugger_lock = old_lock
         self.core.stop_level = old_stop_level
         self.core.different_line = old_different_line
         self.proc.continue_running = False
@@ -81,16 +84,17 @@
         return False
 
     pass
 
 
 if __name__ == "__main__":
     import inspect
-    from trepan.processor import cmdproc as Mcmdproc
+
     from trepan import debugger
+    from trepan.processor import cmdproc as Mcmdproc
 
     d = debugger.Trepan()
     cp = d.core.processor
     cp.curframe = inspect.currentframe()
     cp.stack, cp.curindex = Mcmdproc.get_stack(cp.curframe, None, None, cp)
     command = DebugCommand(cp)
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/delete.py` & `trepan3k-1.2.9/trepan/processor/command/delete.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,24 +18,23 @@
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.processor.complete import complete_bpnumber
 
 
 class DeleteCommand(DebuggerCommand):
     """**delete** [*bpnumber* [*bpnumber*...]]
 
-Delete some breakpoints.
+    Delete some breakpoints.
 
-Arguments are breakpoint numbers with spaces in between.  To delete
-all breakpoints, give no argument.  Without
-arguments, clear all breaks (but first ask for confirmation).
-
-See also:
----------
-`clear`
-"""
+    Arguments are breakpoint numbers with spaces in between.  To delete
+    all breakpoints, give no argument.  Without
+    arguments, clear all breaks (but first ask for confirmation).
+
+    See also:
+    ---------
+    `clear`"""
 
     aliases = ("delete!",)
     short_help = "Delete some breakpoints or auto-display expressions"
 
     complete = complete_bpnumber
 
     DebuggerCommand.setup(locals(), category="breakpoints")
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/deparse.py` & `trepan3k-1.2.9/trepan/processor/command/deparse.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,59 +21,58 @@
         try:
             from decompyle3.semantics.fragments import code_deparse
         except ImportError:
             from uncompyle6.semantics.fragments import code_deparse
     else:
         from uncompyle6.semantics.fragments import code_deparse
 
-from getopt import getopt, GetoptError
+from getopt import GetoptError, getopt
 
+from pyficache import getlines, highlight_string
 
 from trepan.lib.deparse import deparse_and_cache, deparse_offset
-from pyficache import highlight_string, getlines
 
 # Our local modules
 from trepan.processor.command.base_cmd import DebuggerCommand
 
 
 class DeparseCommand(DebuggerCommand):
     """**deparse** [options] [ . ]
 
-Options:
-------
+    Options:
+    ------
 
-    -p | --parent        show parent node
-    -t | --tree          show parse tree
-    -o | --offset [num]  show deparse of offset NUM
-    -h | --help          give this help
-
-deparse around where the program is currently stopped. If no offset is given,
-we use the current frame offset. If `-p` is given, include parent information.
-
-If an '.' argument is given, deparse the entire function or main
-program you are in.
-
-Output is colorized the same as source listing. Use `set highlight plain` to turn
-that off.
-
-Examples:
---------
-
-    deparse             # deparse current location
-    deparse --parent    # deparse current location enclosing context
-    deparse .           # deparse current function or main
-    deparse --offset 6  # deparse starting at offset 6
-    deparse --offsets   # show all exect deparsing offsets
-    deparse --tree      # deparse and show parse tree
+        -p | --parent        show parent node
+        -t | --tree          show parse tree
+        -o | --offset [num]  show deparse of offset NUM
+        -h | --help          give this help
 
-See also:
----------
+    deparse around where the program is currently stopped. If no offset is given,
+    we use the current frame offset. If `-p` is given, include parent information.
 
-`disassemble`, `list`, and `set highlight`
-"""
+    If an '.' argument is given, deparse the entire function or main
+    program you are in.
+
+    Output is colorized the same as source listing. Use `set highlight plain` to turn
+    that off.
+
+    Examples:
+    --------
+
+        deparse             # deparse current location
+        deparse --parent    # deparse current location enclosing context
+        deparse .           # deparse current function or main
+        deparse --offset 6  # deparse starting at offset 6
+        deparse --offsets   # show all exect deparsing offsets
+        deparse --tree      # deparse and show parse tree
+
+    See also:
+    ---------
+
+    `disassemble`, `list`, and `set highlight`"""
 
     short_help = "Deparse source via uncompyle6/decompyle3"
     DebuggerCommand.setup(locals(), category="data", max_args=10, need_stack=True)
 
     def print_text(self, text):
         if self.settings["highlight"] == "plain":
             self.msg(text)
@@ -82,15 +81,15 @@
 
         if "style" in self.settings:
             opts["style"] = self.settings["style"]
         self.msg(highlight_string(text, opts).strip("\n"))
 
     def run(self, args):
         if sys.version_info[:2] > (3, 8):
-            self.errmsg("Deparsing for Python greater than 3.8 not impemented")
+            self.errmsg("Deparsing for Python greater than 3.8 not implemented")
             return
         co = self.proc.curframe.f_code
         name = co.co_name
 
         try:
             opts, args = getopt(
                 args[1:],
@@ -112,15 +111,18 @@
             if o in ("-h", "--help"):
                 self.proc.commands["help"].run(["help", "deparse"])
                 return
             elif o in ("-O", "--offsets"):
                 show_offsets = True
             elif o in ("-p", "--parent"):
                 show_parent = True
-            elif o in ("-t", "--tree",):
+            elif o in (
+                "-t",
+                "--tree",
+            ):
                 show_tree = True
             elif o in ("-o", "--offset"):
                 offset = a
             else:
                 self.errmsg("unhandled option '%s'" % o)
             pass
         pass
@@ -202,14 +204,15 @@
         return
 
     pass
 
 
 if __name__ == "__main__":
     import sys
+
     from trepan import debugger
 
     d = debugger.Trepan()
     cp = d.core.processor
     command = DeparseCommand(d.core.processor)
     command.proc.frame = sys._getframe()
     command.proc.setup()
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/deval.py` & `trepan3k-1.2.9/trepan/processor/command/deval.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,32 +25,32 @@
 else:
     from uncompyle6.semantics.fragments import deparse_code
     from uncompyle6.semantics.fragments import deparsed_find
 
 
 class DEvalCommand(DebuggerCommand):
     """**deval**
-    **deval?**
+        **deval?**
 
-Run a the current deparsed expression in the context of the current
-frame. Normally we are stopped before an expression so the thing that
-corresponds to the `eval` command is running the parent
-construct. `deval?` will run just the command associated with the next
-piece of code to be run.
+    Run a the current deparsed expression in the context of the current
+    frame. Normally we are stopped before an expression so the thing that
+    corresponds to the `eval` command is running the parent
+    construct. `deval?` will run just the command associated with the next
+    piece of code to be run.
 
-Examples:
----------
+    Examples:
+    ---------
 
-    deval   # Run *parent* of current deparsed code
-    deval?  # Run current deparsed code
+        deval   # Run *parent* of current deparsed code
+        deval?  # Run current deparsed code
 
-See also:
----------
+    See also:
+    ---------
 
-`eval`
+    `eval`
 
     """
 
     aliases = ("deval?",)
     short_help = "Print value of deparsed expression"
 
     DebuggerCommand.setup(locals(), category="data", need_stack=True, max_args=0)
@@ -65,27 +65,27 @@
         sys_version = version_info[0] + (version_info[1] / 10.0)
         try:
             deparsed = deparse_code(sys_version, co, is_pypy=IS_PYPY)
             nodeInfo = deparsed_find((name, last_i), deparsed, co)
             if not nodeInfo:
                 self.errmsg("Can't find exact offset %d" % last_i)
                 return
-        except:
+        except Exception:
             self.errmsg("error in deparsing code")
             return
         if "?" == args[0][-1]:
             extractInfo = deparsed.extract_node_info(nodeInfo.node)
         else:
             extractInfo, _ = deparsed.extract_parent_info(nodeInfo.node)
         text = extractInfo.selectedText
         text = text.strip()
         self.msg("Evaluating: %s" % text)
         try:
             self.proc.exec_line(text)
-        except:
+        except Exception:
             pass
 
 
 if __name__ == "__main__":
     import inspect
     from trepan import debugger
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/disable.py` & `trepan3k-1.2.9/trepan/processor/command/disable.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,21 +18,20 @@
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.processor.complete import complete_bpnumber
 
 
 class DisableCommand(DebuggerCommand):
     """**disable** *bpnumber* [*bpnumber* ...]
 
-Disables the breakpoints given as a space separated list of breakpoint
-numbers. To disable all breakpoints, give no argument. See also `info break` to get a list.
+    Disables the breakpoints given as a space separated list of breakpoint
+    numbers. To disable all breakpoints, give no argument. See also `info break` to get a list.
 
-See also:
----------
-`enable`
-"""
+    See also:
+    ---------
+    `enable`"""
 
     short_help = "Disable some breakpoints"
 
     complete = complete_bpnumber
 
     DebuggerCommand.setup(locals(), category="breakpoints")
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/disassemble.py` & `trepan3k-1.2.9/trepan/processor/command/disassemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 # -*- coding: utf-8 -*-
-#  Copyright (C) 2009, 2012-2018, 2020 Rocky Bernstein
+#
+#  Copyright (C) 2009, 2012-2018, 2020, 2023 Rocky Bernstein
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import inspect, sys
+import inspect
 import os.path as osp
+import sys
 
-# Our local modules
-from trepan.processor.command.base_cmd import DebuggerCommand
-from trepan.lib.disassemble import dis
-import trepan.lib.file as Mfile
 from xdis.load import load_module
+
+import trepan.lib.file as Mfile
+from trepan.lib.disassemble import dis
 from trepan.processor.cmd_addrlist import parse_addr_list_cmd
 
+# Our local modules
+from trepan.processor.command.base_cmd import DebuggerCommand
+
 # From importlib.util
 DEBUG_BYTECODE_SUFFIXES = [".pyc"]
 OPTIMIZED_BYTECODE_SUFFIXES = [".pyo"]
 _PYCACHE = "__pycache__"
 
 
 def cache_from_source(path, debug_override=None):
@@ -62,73 +66,70 @@
         return osp.join(head, filename)
     return osp.join(head, _PYCACHE, filename)
 
 
 class DisassembleCommand(DebuggerCommand):
     """**disassemble** [*thing*]
 
-**disassemble** [*address-range*]
+    **disassemble** [*address-range*]
 
-Disassembles bytecode. See `help syntax range` for what can go in a list range.
+    Disassembles bytecode. See `help syntax range` for what can go in a list range.
 
-Without arguments, print lines starting from where the last list left off
-since the last entry to the debugger. We start off at the location indicated
-by the current stack.
+    Without arguments, print lines starting from where the last list left off
+    since the last entry to the debugger. We start off at the location indicated
+    by the current stack.
 
-in addition you can also use:
+    in addition you can also use:
 
-  - a '.' for the location of the current frame
+      - a '.' for the location of the current frame
 
-  - a '-' for the lines before the last list
+      - a '-' for the lines before the last list
 
-  - a '+' for the lines after the last list
+      - a '+' for the lines after the last list
 
-With a class, method, function, pyc-file, code or string argument
-disassemble that.
+    With a class, method, function, pyc-file, code or string argument
+    disassemble that.
 
-Examples:
---------
-::
+    Examples:
+    --------
+    ::
 
-   disassemble    # Possibly current frame
-   disassemble +                    # Same as above
-   disassemble os.path              # Disassemble all of os.path # xxx
-   disassemble os.path.normcase()   # Disaasemble just method os.path.normcase
-   disassemble 3                    # Disassemble starting from line 3
-   disassemble 3, 10                # Disassemble lines 3 to 10
-   disassemble *0, *10              # Disassemble offset 0..10 (10 not included)
-   disassemble myprog.pyc           # Disassemble file myprog.pyc
+       disassemble    # Possibly current frame
+       disassemble +                    # Same as above
+       disassemble os.path              # Disassemble all of os.path # xxx
+       disassemble os.path.normcase()   # Disaasemble just method os.path.normcase
+       disassemble 3                    # Disassemble starting from line 3
+       disassemble 3, 10                # Disassemble lines 3 to 10
+       disassemble *0, *10              # Disassemble offset 0..10 (10 not included)
+       disassemble myprog.pyc           # Disassemble file myprog.pyc
 
-See also:
----------
+    See also:
+    ---------
 
-`help syntax arange`, `deparse`, `list`, `info pc`.
-"""
+    `help syntax arange`, `deparse`, `list`, `info pc`."""
 
     aliases = ("disasm",)  # Note: we will have disable
     short_help = "Disassemble Python bytecode"
 
-    DebuggerCommand.setup(
-        locals(), category="data", max_args=2
-    )
+    DebuggerCommand.setup(locals(), category="data", max_args=2)
 
     def run(self, args):
         proc = self.proc
 
         # FIXME: add a setting for assembler list size
         listsize = 4
 
         opts = {
             "highlight": self.settings["highlight"],
             "start_line": 1,
             "end_line": None,
             "start_offset": None,
             "end_offset": None,
             "relative_pos": False,
-            "asm_format" : self.settings["asmfmt"]
+            "asm_format": self.settings["asmfmt"],
         }
 
         curframe = proc.curframe
         if curframe:
             line_no = inspect.getlineno(curframe)
             opts["start_line"] = line_no - 1
             opts["end_line"] = line_no + 1
@@ -137,15 +138,15 @@
         if len(args) == 2:
             if args[1].endswith("()"):
                 eval_args = args[1][:-2]
             else:
                 eval_args = args[1]
             try:
                 obj = self.proc.eval(eval_args, show_error=False)
-            except:
+            except Exception:
                 obj = None
             else:
                 if (
                     inspect.ismethod(obj)
                     or inspect.isfunction(obj)
                     or inspect.isgeneratorfunction(obj)
                     or inspect.isgenerator(obj)
@@ -201,15 +202,15 @@
             elif not curframe:
                 self.errmsg("No frame selected.")
                 return
             else:
                 try:
                     obj = self.proc.eval(args[1])
                     opts["start_line"] = -1
-                except:
+                except Exception:
                     self.errmsg(
                         ("Object '%s' is not something we can" + " disassemble.")
                         % args[1]
                     )
                     return
 
         # We now have all  information. Do the listing.
@@ -217,15 +218,14 @@
             self.msg, self.msg_nocr, self.section, self.errmsg, obj, **opts
         )
         return False
 
 
 # Demo it
 if __name__ == "__main__":
-
     # FIXME: make sure the below is in a unit test
     def doit(cmd, args):
         proc = cmd.proc
         proc.current_command = " ".join(args)
         cmd.run(args)
 
     from trepan.processor.command import mock
@@ -233,21 +233,21 @@
     d, cp = mock.dbg_setup()
 
     cp.list_object = cp.curframe = inspect.currentframe()
     command = DisassembleCommand(cp)
     prefix = "-" * 20 + " disassemble "
 
     print(prefix + "os.path")
-    doit(command, ["dissassemble", "cp.errmsg()"])
+    doit(command, ["disassemble", "cp.errmsg()"])
 
     print(prefix + "cp.errmsg()")
-    doit(command, ["dissassemble", "cp.errmsg()"])
+    doit(command, ["disassemble", "cp.errmsg()"])
 
     print(prefix + "cp.errmsg()")
-    doit(command, ["dissassemble", "cp.errmsg()"])
+    doit(command, ["disassemble", "cp.errmsg()"])
 
     # print(prefix)
     # doit(command, ['disassemble']) # no good
 
     # print(prefix + 'me')
     # doit(command, ['disassemble', 'me()']) # reports invalid function correctly
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/display.py` & `trepan3k-1.2.9/trepan/processor/command/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.processor.complete import complete_id_and_builtins
 
 
 class DisplayCommand(DebuggerCommand):
     """**display** [*format*] *expression*
 
-Print value of expression *expression* each time the program stops.
-*format* may be used before *expression* and may be one of `/c` for
-char, `/x` for hex, `/o` for octal, `/f` for float or `/s` for string.
-
-For now, display expressions are only evaluated when in the same
-code as the frame that was in effect when the display expression
-was set.  This is a departure from gdb and we may allow for more
-flexibility in the future to specify whether this should be the
-case or not.
-
-With no argument, evaluate and display all currently requested
-auto-display expressions.  Use `undisplay` to cancel display
-requests previously made."""
+    Print value of expression *expression* each time the program stops.
+    *format* may be used before *expression* and may be one of `/c` for
+    char, `/x` for hex, `/o` for octal, `/f` for float or `/s` for string.
+
+    For now, display expressions are only evaluated when in the same
+    code as the frame that was in effect when the display expression
+    was set.  This is a departure from gdb and we may allow for more
+    flexibility in the future to specify whether this should be the
+    case or not.
+
+    With no argument, evaluate and display all currently requested
+    auto-display expressions.  Use `undisplay` to cancel display
+    requests previously made."""
 
     short_help = "Display expressions when entering debugger"
 
     format_specs = ("/c", "/x", "/o", "/f", "/s")
 
     DebuggerCommand.setup(locals(), category="data")
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/down.py` & `trepan3k-1.2.9/trepan/processor/command/down.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,21 +24,21 @@
     short_help = "Move stack frame to a more recent selected frame"
 
     UpCommand.setup(locals(), category="stack", need_stack=True, max_args=1)
 
     def run(self, args):
         """**down** [*count*]
 
-Move the current frame down in the stack trace (to a newer frame). 0
-is the most recent frame. If no count is given, move down 1.
+        Move the current frame down in the stack trace (to a newer frame). 0
+        is the most recent frame. If no count is given, move down 1.
 
-See also:
----------
+        See also:
+        ---------
 
-`up` and `frame`."""
+        `up` and `frame`."""
 
         adjust_relative(self.proc, self.name, args, self.signum)
         return False
 
 
 if __name__ == "__main__":
     import inspect
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/edit.py` & `trepan3k-1.2.9/trepan/processor/command/edit.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,28 +20,29 @@
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.processor.cmdlist import parse_location
 
 
 class EditCommand(DebuggerCommand):
     """**edit** *location*
 
-Edit specified file or module.
-With no argument, edits file containing most recent line listed.
+    Edit specified file or module.
+    With no argument, edits file containing most recent line listed.
 
-See also:
----------
+    See also:
+    ---------
 
-`list`
-"""
+    `list`"""
 
     aliases = ("ed",)
     short_help = "Edit specified file or module"
 
     DebuggerCommand.setup(
-        locals(), category="files", max_args=1,
+        locals(),
+        category="files",
+        max_args=1,
     )
 
     def run(self, args):
         curframe = self.proc.curframe
         if len(args) == 1:
             if curframe is None:
                 self.errmsg(
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/enable.py` & `trepan3k-1.2.9/trepan/processor/command/enable.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,21 +18,20 @@
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.processor.complete import complete_bpnumber
 
 
 class EnableCommand(DebuggerCommand):
     """**enable** *bpnumber* [*bpnumber* ...]
 
-Enables the breakpoints given as a space separated list of breakpoint
-numbers. To enable all breakpoints, give no argument. See also `info break` to get a list.
+    Enables the breakpoints given as a space separated list of breakpoint
+    numbers. To enable all breakpoints, give no argument. See also `info break` to get a list.
 
-See also:
----------
-`disable`
-"""
+    See also:
+    ---------
+    `disable`"""
 
     aliases = ("en",)
     short_help = "Enable some breakpoints"
 
     complete = complete_bpnumber
 
     DebuggerCommand.setup(locals(), category="breakpoints")
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/eval.py` & `trepan3k-1.2.9/trepan/processor/command/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
-#  Copyright (C) 2012-2013, 2015, 2017, 2020 Rocky Bernstein
+#
+#  Copyright (C) 2012-2013, 2015, 2017, 2020, 2023 Rocky Bernstein
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
@@ -72,15 +73,15 @@
                 return
         else:
             text = self.proc.current_command[len(self.proc.cmd_name) :]
             pass
         text = text.strip()
         try:
             self.proc.exec_line(text)
-        except:
+        except Exception:
             pass
 
 
 if __name__ == "__main__":
     import inspect
     from trepan.debugger import Trepan
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/examine.py` & `trepan3k-1.2.9/trepan/processor/command/examine.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,36 +18,38 @@
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.lib.printing import print_obj
 
 
 class ExamineCommand(DebuggerCommand):
     """**examine** *expr1* [*expr2* ...]
 
-Examine value, type and object attributes of an expression.
+    Examine value, type and object attributes of an expression.
 
-In contrast to normal Python expressions, expressions should not have
-blanks which would cause shlex to see them as different tokens.
+    In contrast to normal Python expressions, expressions should not have
+    blanks which would cause shlex to see them as different tokens.
 
-Examples:
----------
+    Examples:
+    ---------
 
-    examine x+1   # ok
-    examine x + 1 # not ok
+        examine x+1   # ok
+        examine x + 1 # not ok
 
-See also:
----------
+    See also:
+    ---------
 
-`pr`, `pp`, and `whatis`.
-"""
+    `pr`, `pp`, and `whatis`."""
 
     aliases = ("x",)
     short_help = "Examine value, type, and object attributes " "of an expression"
 
     DebuggerCommand.setup(
-        locals(), category="data", need_stack=True, min_args=1,
+        locals(),
+        category="data",
+        need_stack=True,
+        min_args=1,
     )
 
     def run(self, args):
         for arg in args[1:]:
             s = print_obj(arg, self.proc.curframe)
             self.msg(s)
             pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/exit.py` & `trepan3k-1.2.9/trepan/processor/command/exit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 # -*- coding: utf-8 -*-
-#  Copyright (C) 2009, 2013, 2015, 2020 Rocky Bernstein
+#
+#  Copyright (C) 2009, 2013, 2015, 2020, 2023 Rocky Bernstein
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import os
 
 # Our local modules
 from trepan.processor.command.base_cmd import DebuggerCommand
 
 
 class ExitCommand(DebuggerCommand):
     """**exit** [*exitcode*]
 
-Hard exit of the debugged program.
+    Hard exit of the debugged program.
 
-The program being debugged is exited via *sys.exit()*. If a return code
-is given, that is the return code passed to *sys.exit()*, the
-return code that will be passed back to the OS.
+    The program being debugged is exited via *sys.exit()*. If a return code
+    is given, that is the return code passed to *sys.exit()*, the
+    return code that will be passed back to the OS.
 
-See also:
----------
+    See also:
+    ---------
 
-See `quit` and `kill`.
-"""
+    See `quit` and `kill`."""
 
     short_help = "Exit program via sys.exit()"
 
     DebuggerCommand.setup(locals(), category="support", max_args=1)
 
     def run(self, args):
         self.core.stop()
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/finish.py` & `trepan3k-1.2.9/trepan/processor/command/finish.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 # -*- coding: utf-8 -*-
-#  Copyright (C) 2009, 2013-2015, 2020 Rocky Bernstein
+#  Copyright (C) 2009, 2013-2015, 2020, 2023 Rocky Bernstein
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import os.path as osp, sys
+import sys
 
 # Our local modules
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.lib.stack import count_frames
 
 
 class FinishCommand(DebuggerCommand):
     """**finish** [*level*]
 
-Continue execution until leaving the current function. When *level* is
-specified, that many frame levels need to be popped. Note that *yield*
-and exceptions raised my reduce the number of stack frames. Also, if a
-thread is switched, we stop ignoring levels.
+    Continue execution until leaving the current function. When *level* is
+    specified, that many frame levels need to be popped. Note that *yield*
+    and exceptions raised my reduce the number of stack frames. Also, if a
+    thread is switched, we stop ignoring levels.
 
-See the `break` command if you want to stop at a particular point in a
+    See the `break` command if you want to stop at a particular point in a
 
-See also:
----------
+    See also:
+    ---------
 
-`continue`, `step`, `next`.
-"""
+    `continue`, `step`, `next`."""
 
     # FIXME: add finish [levels|fn]
     # If fn is given, that's a short-hand way of looking up how many levels
     # until that frame. However the same provisions regarding stopping,
     # exceptions, 'yield'ing and so on still apply.
 
     aliases = ("fin",)
@@ -80,19 +79,27 @@
         for c in (
             ["finish", "1"],
             ["finish", "wrong", "number", "of", "args"],
             ["finish", "5"],
             ["finish", "0*5+1"],
         ):
             cmd.continue_running = False
-            cmd.proc.stack = [(sys._getframe(0), 14,)]
+            cmd.proc.stack = [
+                (
+                    sys._getframe(0),
+                    14,
+                )
+            ]
             result = cmd.run(c)
             print("Execute result: %s" % result)
             print(
                 "stop_frame %s, continue_running: %s"
-                % (cmd.core.stop_frame, cmd.continue_running,)
+                % (
+                    cmd.core.stop_frame,
+                    cmd.continue_running,
+                )
             )
             pass
         return
 
     demo_finish(cmd)
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/frame.py` & `trepan3k-1.2.9/trepan/processor/command/frame.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,69 +1,71 @@
 # -*- coding: utf-8 -*-
-#  Copyright (C) 2009, 2013-2015, 2020 Rocky Bernstein
+#  Copyright (C) 2009, 2013-2015, 2020, 2023 Rocky Bernstein
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import inspect, sys, threading
+import inspect
+import sys
+import threading
+
+from trepan.lib import thred as Mthread
+from trepan.lib.complete import complete_token
+from trepan.processor.cmdproc import get_stack
 
 # Our local modules
 from trepan.processor.command.base_cmd import DebuggerCommand
-from trepan.processor.frame import frame_low_high, adjust_frame
-from trepan.processor.cmdproc import get_stack
-from trepan.lib.complete import complete_token
-from trepan.lib import thred as Mthread
+from trepan.processor.frame import adjust_frame, frame_low_high
 
 
 class FrameCommand(DebuggerCommand):
     """**frame** [*thread-Name*|*thread-number*] [*frame-number*]
 
-Change the current frame to frame *frame-number* if specified, or the
-current frame, 0, if no frame number specified.
+    Change the current frame to frame *frame-number* if specified, or the
+    current frame, 0, if no frame number specified.
 
-If a thread name or thread number is given, change the current frame
-to a frame in that thread. Dot (.) can be used to indicate the name of
-the current frame the debugger is stopped in.
-
-A negative number indicates the position from the other or
-least-recently-entered end.  So `frame -1` moves to the oldest frame,
-and `frame 0` moves to the newest frame. Any variable or expression
-that evaluates to a number can be used as a position, however due to
-parsing limitations, the position expression has to be seen as a single
-blank-delimited parameter. That is, the expression `(5*3)-1` is okay
-while `(5 * 3) - 1)` isn't.
-
-**Examples:**
-
-   frame     # Set current frame at the current stopping point
-   frame 0   # Same as above
-   frame 5-5 # Same as above. Note: no spaces allowed in expression 5-5
-   frame .   # Same as above. "current thread" is explicit.
-   frame . 0 # Same as above.
-   frame 1   # Move to frame 1. Same as: frame 0; up
-   frame -1  # The least-recent frame
-   frame MainThread 0 # Switch to frame 0 of thread MainThread
-   frame MainThread   # Same as above
-   frame -2434343 0   # Use a thread number instead of name
+    If a thread name or thread number is given, change the current frame
+    to a frame in that thread. Dot (.) can be used to indicate the name of
+    the current frame the debugger is stopped in.
+
+    A negative number indicates the position from the other or
+    least-recently-entered end.  So `frame -1` moves to the oldest frame,
+    and `frame 0` moves to the newest frame. Any variable or expression
+    that evaluates to a number can be used as a position, however due to
+    parsing limitations, the position expression has to be seen as a single
+    blank-delimited parameter. That is, the expression `(5*3)-1` is okay
+    while `(5 * 3) - 1)` isn't.
+
+    **Examples:**
+
+       frame     # Set current frame at the current stopping point
+       frame 0   # Same as above
+       frame 5-5 # Same as above. Note: no spaces allowed in expression 5-5
+       frame .   # Same as above. "current thread" is explicit.
+       frame . 0 # Same as above.
+       frame 1   # Move to frame 1. Same as: frame 0; up
+       frame -1  # The least-recent frame
+       frame MainThread 0 # Switch to frame 0 of thread MainThread
+       frame MainThread   # Same as above
+       frame -2434343 0   # Use a thread number instead of name
 
-See also:
----------
+    See also:
+    ---------
 
-`up`, `down`, `backtrace`, and `info threads`.
-"""
+    `up`, `down`, `backtrace`, and `info threads`."""
 
     short_help = "Select and print a stack frame"
 
     DebuggerCommand.setup(locals(), category="stack", max_args=2, need_stack=True)
 
     def complete(self, prefix):
         proc_obj = self.proc
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/handle.py` & `trepan3k-1.2.9/trepan/processor/command/handle.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,44 +17,43 @@
 # Our local modules
 from trepan.processor.command.base_cmd import DebuggerCommand
 
 
 class HandleCommand(DebuggerCommand):
     """**handle** [*signal-name* [*action1* *action2* ...]]
 
-Specify how to handle a signal *signal-name*. *signal-name* can be a
-signal name like `SIGINT` or a signal number like 2. The absolute
-value is used for numbers so -9 is the same as 9 (`SIGKILL`). When
-signal names are used, you can drop off the leading "SIG" if you want. Also
-letter case is not important either.
+    Specify how to handle a signal *signal-name*. *signal-name* can be a
+    signal name like `SIGINT` or a signal number like 2. The absolute
+    value is used for numbers so -9 is the same as 9 (`SIGKILL`). When
+    signal names are used, you can drop off the leading "SIG" if you want. Also
+    letter case is not important either.
 
-Arguments are signals and actions to apply to those signals.
-recognized actions include `stop`, `nostop`, `print`, `noprint`,
-`pass`, `nopass`, `ignore`, or `noignore`.
+    Arguments are signals and actions to apply to those signals.
+    recognized actions include `stop`, `nostop`, `print`, `noprint`,
+    `pass`, `nopass`, `ignore`, or `noignore`.
 
-`stop` means reenter debugger if this signal happens (implies `print` and
-`nopass`).
+    `stop` means reenter debugger if this signal happens (implies `print` and
+    `nopass`).
 
-`Print` means print a message if this signal happens.
+    `Print` means print a message if this signal happens.
 
-`Pass` means let program see this signal; otherwise the program see it.
+    `Pass` means let program see this signal; otherwise the program see it.
 
-`Ignore` is a synonym for `nopass`; `noignore` is a synonym for `pass`.
+    `Ignore` is a synonym for `nopass`; `noignore` is a synonym for `pass`.
 
-Without any action names the current settings are shown.
+    Without any action names the current settings are shown.
 
-**Examples:**
+    **Examples:**
 
-  handle INT         # Show current settings of SIGINT
-  handle SIGINT      # same as above
-  handle int         # same as above
-  handle 2           # Probably the same as above
-  handle -2          # the same as above
-  handle INT nostop  # Don't stop in the debugger on SIGINT
-"""
+      handle INT         # Show current settings of SIGINT
+      handle SIGINT      # same as above
+      handle int         # same as above
+      handle 2           # Probably the same as above
+      handle -2          # the same as above
+      handle INT nostop  # Don't stop in the debugger on SIGINT"""
 
     short_help = "Specify how to handle a signal"
 
     DebuggerCommand.setup(locals(), category="running", min_args=1)
 
     def run(self, args):
         if self.debugger.sigmgr.action(" ".join(args[1:])) and len(args) > 2:
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/help/arange.rst` & `trepan3k-1.2.9/trepan/processor/command/help/arange.rst`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/trepan/processor/command/help/command.rst` & `trepan3k-1.2.9/trepan/processor/command/help/command.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 =======================
 
 Command names and arguments are separated with spaces like POSIX shell
 syntax. Parenthesis around the arguments and commas between them are
 not used. If the first non-blank character of a line starts with `#`,
 the command is ignored.
 
-Commands are split at whereever `;;` appears. This process disregards
+Commands are split at wherever `;;` appears. This process disregards
 any quotes or other symbols that have meaning in Python. The strings
 after the leading command string are put back on a command queue, and
 there should be white space around ';;'.
 
 Within a single command, tokens are then white-space split. Again,
 this process disregards quotes or symbols that have meaning in Python.
 Some commands like `eval`, `macro`, and `break` have access to the
@@ -32,15 +32,15 @@
 
 3. After the above, The leading token is looked up a table of debugger
 commands. If an exact match is found, the command name and arguments
 are dispatched to that command.
 
 4. If after all of the above, we still don't find a command, the line
 may be evaluated as a Python statement in the current context of the
-program at the point it is stoppped. However this is done only if
+program at the point it is stopped. However this is done only if
 "auto evaluation" is on.  It is on by default.
 
 If `auto eval` is not set on, or if running the Python statement
 produces an error, we display an error message that the entered string
 is "undefined".
 
 If you want python-, ipython- or bpython-like shell
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/help/location.rst` & `trepan3k-1.2.9/trepan/processor/command/help/location.rst`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/trepan/processor/command/help/range.rst` & `trepan3k-1.2.9/trepan/processor/command/help/range.rst`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/trepan/processor/command/help/suffixes.rst` & `trepan3k-1.2.9/trepan/processor/command/help/suffixes.rst`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/trepan/processor/command/help.py` & `trepan3k-1.2.9/trepan/processor/command/help.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2012-2013, 2015, 2020 Rocky Bernstein
+#
+#    Copyright (C) 2009, 2012-2013, 2015, 2020, 2023 Rocky Bernstein
 #
 #    This program is free software; you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation; either version 2 of the License, or
 #    (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
@@ -11,24 +12,24 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program; if not, write to the Free Software
 #    Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 #    02110-1301 USA.
-import glob, re
-
+import glob
 import os.path as osp
+import re
 
-# Our local modules
-from trepan.processor.command.base_cmd import DebuggerCommand
-from trepan.processor import cmdproc as Mcmdproc
-from trepan.lib import complete as Mcomplete
 from trepan import misc as Mmisc
+from trepan.lib import complete as Mcomplete
+from trepan.processor import cmdproc as Mcmdproc
 
+# Our local modules
+from trepan.processor.command.base_cmd import DebuggerCommand
 
 categories = {
     "breakpoints": "Making the program stop at certain points",
     "data": "Examining data",
     "files": "Specifying and examining files",
     "running": "Running the program",
     "status": "Status inquiries",
@@ -37,45 +38,45 @@
     "syntax": "Debugger command syntax",
 }
 
 
 class HelpCommand(DebuggerCommand):
     """**help** [*command* [*subcommand*]|*expression*]
 
-Without argument, print the list of available debugger commands.
+    Without argument, print the list of available debugger commands.
 
-When an argument is given, it is first checked to see if it is command
-name.
+    When an argument is given, it is first checked to see if it is command
+    name.
 
-If the argument is an expression or object name, you get the same
-help that you would get inside a Python shell running the built-in
-*help()* command.
+    If the argument is an expression or object name, you get the same
+    help that you would get inside a Python shell running the built-in
+    *help()* command.
 
-If the environment variable *$PAGER* is defined, the file is
-piped through that command.  You'll notice this only for long help
-output.
+    If the environment variable *$PAGER* is defined, the file is
+    piped through that command.  You'll notice this only for long help
+    output.
 
-Some commands like `info`, `set`, and `show` can accept an
-additional subcommand to give help just about that particular
-subcommand. For example `help info line` give help about the
-info line command.
+    Some commands like `info`, `set`, and `show` can accept an
+    additional subcommand to give help just about that particular
+    subcommand. For example `help info line` give help about the
+    info line command.
 
-See also:
----------
+    See also:
+    ---------
 
-`examine` and `whatis`.
-"""
+    `examine` and `whatis`."""
 
     aliases = ("?",)
     short_help = "Print commands or give help for command(s)"
     HELP_DIR = osp.join(osp.dirname(__file__), "help")
     RST_EXTENSION = ".rst"
 
     DebuggerCommand.setup(
-        locals(), category="support",
+        locals(),
+        category="support",
     )
 
     def complete(self, prefix):
         proc_obj = self.proc
         matches = Mcomplete.complete_token(
             list(categories.keys()) + ["*", "all"] + list(proc_obj.commands.keys()),
             prefix,
@@ -139,15 +140,19 @@
                 ]
                 if cmds is None:
                     self.errmsg(
                         "No commands found matching /^%s/. " 'Try "help".' % cmd_name
                     )
                 elif len(cmds) == 1:
                     self.msg(
-                        "Pattern '%s' matches command %s..." % (cmd_name, cmds[0],)
+                        "Pattern '%s' matches command %s..."
+                        % (
+                            cmd_name,
+                            cmds[0],
+                        )
                     )
                     args[1] = cmds[0]
                     self.run(args)
                 else:
                     self.section("Command names matching /^%s/:" % cmd_name)
                     self.msg_nocr(self.columnize_commands(cmds))
                     pass
@@ -193,15 +198,21 @@
 
         self.msg("%s.\n" % categories[category])
         self.section("List of commands:")
         names.sort()
         for name in names:  # Foo! iteritems() doesn't do sorting
             if category != n2cmd[name].category:
                 continue
-            self.msg("%-13s -- %s" % (name, n2cmd[name].short_help,))
+            self.msg(
+                "%-13s -- %s"
+                % (
+                    name,
+                    n2cmd[name].short_help,
+                )
+            )
             pass
         return
 
     def syntax_files(self):
         path = osp.join(self.HELP_DIR, ("*%s" % self.RST_EXTENSION))
         files = glob.glob(path)
         return [osp.basename(name).split(".")[0] for name in files]
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info.py` & `trepan3k-1.2.9/trepan/processor/command/info.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 
 from trepan.processor.command.base_submgr import SubcommandMgr
 
 
 class InfoCommand(SubcommandMgr):
     """Generic command for showing things about the program being debugged.
 
-You can give unique prefix of the name of a subcommand to get
-information about just that subcommand.
+    You can give unique prefix of the name of a subcommand to get
+    information about just that subcommand.
 
-Type `info` for a list of *info* subcommands and what they do.
-Type `help info *` for just a list of *info* subcommands.
-"""
+    Type `info` for a list of *info* subcommands and what they do.
+    Type `help info *` for just a list of *info* subcommands."""
 
     aliases = ("i",)
     short_help = "Information about debugged program and its environment"
 
     SubcommandMgr.setup(locals(), category="status")
 
+
 if __name__ == "__main__":
     from trepan.processor.command import mock
 
     d, cp = mock.dbg_setup()
     command = InfoCommand(cp, "info")
     command.run(["info"])
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/__init__.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2008-2009, 2014, 2018 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2008-2009, 2014, 2018, 2023 Rocky Bernstein
+#   <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
-""" Copyright (C) 2008, 2009, 2018 Rocky Bernstein <rocky@gnu.org> """
+""" Copyright (C) 2008, 2009, 2018, 2023 Rocky Bernstein <rocky@gnu.org> """
 
-import glob, os
+import glob
+import os
 
 # FIXME: Is it really helpful to "privatize" variable names below?
 # The below names are not part of the standard pre-defined names like
 # __name__ or __file__ are.
 
 # Get the name of our directory.
 __command_dir__ = os.path.dirname(__file__)
 
 # A glob pattern that will get all *.py files but not __init__.py
-__py_files__    = glob.glob(os.path.join(__command_dir__, '[a-z]*.py'))
+__py_files__ = glob.glob(os.path.join(__command_dir__, "[a-z]*.py"))
 
 # Take the basename of the filename and drop off '.py'. That minus the
 # file exclude_file the list of modules that info.py will use to import
 exclude_files = []
-__modules__ = [ os.path.basename(filename[0:-3]) for
-                filename in __py_files__
-                if os.path.basename(filename) not in exclude_files]
+__modules__ = [
+    os.path.basename(filename[0:-3])
+    for filename in __py_files__
+    if os.path.basename(filename) not in exclude_files
+]
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/args.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/args.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 # Our local modules
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 
 
 class InfoArgs(Mbase_subcmd.DebuggerSubcommand):
     """**info args**
 
-Show parameters of the current stack frame.
+    Show parameters of the current stack frame.
 
-See also:
----------
-`info locals`, `info globals`, `info frame`"""
+    See also:
+    ---------
+    `info locals`, `info globals`, `info frame`"""
 
     min_abbrev = 1
     need_stack = True
     short_help = "Argument variables of the current stack frame"
 
     def run(self, args):
         if not self.proc.curframe:
@@ -39,45 +39,51 @@
             return False
         f = self.proc.curframe
         co = f.f_code
         # Break out display into args, varargs, keywords, and locals ?
         # args, varargs, varkw, f_locals = getargvalues(f)
         d = f.f_locals
         n = co.co_argcount
-        if co.co_flags & inspect.CO_VARARGS: n += 1
-        if co.co_flags & inspect.CO_VARKEYWORDS: n += 1
+        if co.co_flags & inspect.CO_VARARGS:
+            n += 1
+        if co.co_flags & inspect.CO_VARKEYWORDS:
+            n += 1
 
         if n == 0:
             self.msg("no parameters")
         else:
             self.section("Argument parameters")
             for i in range(n):
                 name = co.co_varnames[i]
-                self.msg_nocr("%d: %s = " % (i+1, name))
+                self.msg_nocr("%d: %s = " % (i + 1, name))
                 if name in d:
                     self.msg(str(d[name]))
                 else:
                     self.ermsg("undefined")
                     pass
                 pass
             pass
         return False
+
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command import mock, info as Minfo
+
     d, cp = mock.dbg_setup()
     i = Minfo.InfoCommand(cp)
     sub = InfoArgs(i)
     print(sub.run([]))
     cp.curframe = inspect.currentframe()
     print(sub.run([]))
 
     def nest_me(sub, cp, b=1):
         cp.curframe = inspect.currentframe()
         print(sub.run([]))
         return
-    print('-' * 10)
+
+    print("-" * 10)
     nest_me(sub, cp, 3)
-    print('-' * 10)
+    print("-" * 10)
     nest_me(sub, cp)
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/break.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/break.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,42 +18,42 @@
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 from trepan.processor import complete as Mcomplete
 
 
 class InfoBreak(Mbase_subcmd.DebuggerSubcommand):
     """**info breakpoints** [ *bp-number...* ]
 
-Show the status of specified breakpoints (or all user-settable
-breakpoints if no argument).
+    Show the status of specified breakpoints (or all user-settable
+    breakpoints if no argument).
 
-The "Disp" column contains one of "keep", or "del", to indicate the
-disposition of the breakpoint after it gets hit.  "del" means that the
-breakpoint will be deleted.  The ""Enb" column indicates if the
-breakpoint is enabled. The "Where" column indicates the file/line
-number of the breakpoint.
-
-Also shown are the number of times the breakpoint has been hit,
-when that count is at least one, and any conditions the breakpoint
-has.
-
-Example:
---------
-
-
-    (trepan3k) info break
-    Num Type          Disp Enb Off Where
-    1   breakpoint    del  n     3 at /tmp/fib.py:9
-    2   breakpoint    keep y    10 at /tmp/fib.py:4
-            breakpoint already hit 1 time
-    3   breakpoint    keep y    20 at /tmp/fib.py:6
-            stop only if x > 0
-
-See also:
----------
-`break`, `delete`, `enable`, `disable`, `condition`
+    The "Disp" column contains one of "keep", or "del", to indicate the
+    disposition of the breakpoint after it gets hit.  "del" means that the
+    breakpoint will be deleted.  The ""Enb" column indicates if the
+    breakpoint is enabled. The "Where" column indicates the file/line
+    number of the breakpoint.
+
+    Also shown are the number of times the breakpoint has been hit,
+    when that count is at least one, and any conditions the breakpoint
+    has.
+
+    Example:
+    --------
+
+
+        (trepan3k) info break
+        Num Type          Disp Enb Off Where
+        1   breakpoint    del  n     3 at /tmp/fib.py:9
+        2   breakpoint    keep y    10 at /tmp/fib.py:4
+                breakpoint already hit 1 time
+        3   breakpoint    keep y    20 at /tmp/fib.py:6
+                stop only if x > 0
+
+    See also:
+    ---------
+    `break`, `delete`, `enable`, `disable`, `condition`
 
     """
 
     min_abbrev = 1  # Min is info b
     need_stack = False
     short_help = "Status of user-settable breakpoints"
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/builtins.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/builtins.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,45 +18,48 @@
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 from trepan.lib import complete as Mcomplete
 
 
 class InfoBuiltins(Mbase_subcmd.DebuggerSubcommand):
     """**info builtins**
 
-Show the builtin-functions for the current stack frame."""
+    Show the builtin-functions for the current stack frame."""
 
-    max_args   = 1
+    max_args = 1
     min_abbrev = 2
     need_stack = True
     short_help = "Show the builtins for current stack frame"
 
     def complete(self, prefix):
-        completions = sorted(['*'] +
-                              self.proc.curframe.f_builtins.keys())
+        completions = sorted(["*"] + self.proc.curframe.f_builtins.keys())
         return Mcomplete.complete_token(completions, prefix)
 
     def run(self, args):
         if not self.proc.curframe:
             self.errmsg("No frame selected.")
             return False
         names = list(self.proc.curframe.f_builtins.keys())
-        if len(args) > 0 and args[0] == '*' :
+        if len(args) > 0 and args[0] == "*":
             self.section("builtins")
             self.msg(self.columnize_commands(names))
         elif len(args) == 0:
             if len(names) > 0:
                 self.section("builtins")
                 self.msg(self.columnize_commands(names))
         return False
+
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command import mock, info as Minfo
     from trepan import debugger as Mdebugger
+
     d = Mdebugger.Debugger()
     d, cp = mock.dbg_setup(d)
     i = Minfo.InfoCommand(cp)
     sub = InfoBuiltins(i)
     import inspect
+
     cp.curframe = inspect.currentframe()
     sub.run([])
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/code.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/code.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2015 Rocky Bernstein <rocky@gnu.org>
+#   Copyright (C) 2015, 2023 Rocky Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-# Our local modules
-from trepan.processor.command import base_subcmd as Mbase_subcmd
 from trepan.lib import complete as Mcomplete
 from trepan.processor import frame as Mframe
 
+# Our local modules
+from trepan.processor.command import base_subcmd as Mbase_subcmd
+
 
 class InfoCode(Mbase_subcmd.DebuggerSubcommand):
-    """**info code** [ *frame-number* | *pyton code object* ]
+    """**info code** [ *frame-number* | *python code object* ]
 
-Show the detailed information for the Python code object in
-*frame-number* or the current frame if *frame-number* is not specified.
+    Show the detailed information for the Python code object in
+    *frame-number* or the current frame if *frame-number* is not specified.
 
-Specific information includes:
+    Specific information includes:
 
-* the number of arguments (not including * or ** args)
+    * the number of arguments (not including * or ** args)
 
-* constants used in the bytecode
+    * constants used in the bytecode
 
-* name of file in which this code object was created
+    * name of file in which this code object was created
 
-* number of first line in Python source code
+    * number of first line in Python source code
 
-* name with which this code object was defined
+    * name with which this code object was defined
 
-See also:
----------
+    See also:
+    ---------
 
-`info frame`, `info locals`, `info file`
-"""
+    `info frame`, `info locals`, `info file`"""
 
     min_abbrev = 2
     max_args = 2
     need_stack = True
-    short_help = '''Show detailed info about the Python code object'''
+    short_help = """Show detailed info about the Python code object"""
 
     def complete(self, prefix):
         proc_obj = self.proc
         low, high = Mframe.frame_low_high(proc_obj, None)
-        ary = [str(low+i) for i in range(high-low+1)]
+        ary = [str(low + i) for i in range(high - low + 1)]
         # FIXME: add in Thread names
         return Mcomplete.complete_token(ary, prefix)
 
     def run(self, args):
         proc = self.proc
         frame = proc.curframe
         if not frame:
@@ -65,62 +65,75 @@
 
         frame_num = None
         frame_num = None
         if len(args) == 1:
             try:
                 frame_num = int(args[0])
                 i_stack = len(proc.stack)
-                if frame_num < -i_stack or frame_num > i_stack-1:
-                    self.errmsg(('a frame number number has to be in the range %d to %d.' +
-                                 ' Got: %d (%s).') % (-i_stack, i_stack-1,
-                                                      frame_num, args[0]))
+                if frame_num < -i_stack or frame_num > i_stack - 1:
+                    self.errmsg(
+                        (
+                            "a frame number number has to be in the range %d to %d."
+                            + " Got: %d (%s)."
+                        )
+                        % (-i_stack, i_stack - 1, frame_num, args[0])
+                    )
                     return False
                 frame = proc.stack[frame_num][0]
                 code = frame.f_code
-            except:
+            except Exception:
                 try:
                     code = eval(args[0], frame.f_globals, frame.f_locals)
-                except:
-                    self.errmsg('%s is not a evaluable as a code object or frame number.' %
-                                 args[0])
+                except Exception:
+                    self.errmsg(
+                        "%s is not a evaluable as a code object or frame number."
+                        % args[0]
+                    )
                     return False
                 # if not inspect.iscode(code):
                 #     self.errmsg('%s is not a code object' % code)
                 pass
 
         else:
             frame_num = proc.curindex
             code = frame.f_code
 
-        mess = 'Code for Frame %d' % frame_num if frame_num is not None else 'Code Info'
+        mess = "Code for Frame %d" % frame_num if frame_num is not None else "Code Info"
         self.section(mess)
         self.msg("  name: %s" % code.co_name)
         self.msg("  number of arguments: %d" % code.co_argcount)
         self.msg("  number of locals: %d" % code.co_nlocals)
         self.msg("  maximum stack size %s" % code.co_stacksize)
         self.msg("  first line number: %s" % code.co_firstlineno)
         self.msg("  is%s optimized" % ("" if (code.co_flags & 1) == 1 else " not"))
-        self.msg("  new local namespace? %s" % ("yes" if (code.co_flags & 2) == 1 else " no"))
+        self.msg(
+            "  new local namespace? %s" % ("yes" if (code.co_flags & 2) == 1 else " no")
+        )
         self.msg("  has%s *args" % ("" if (code.co_flags & 4) == 1 else " no"))
         self.msg("  has%s **args" % ("" if (code.co_flags & 8) == 1 else " no"))
-        maxwidth = self.settings['width'] // 2
-        for name, field in [('Constants', 'co_consts'),
-                            ('Variable names', 'co_varnames'),
-                            ('Local Variables', 'co_names')
-                            ]:
+        maxwidth = self.settings["width"] // 2
+        for name, field in [
+            ("Constants", "co_consts"),
+            ("Variable names", "co_varnames"),
+            ("Local Variables", "co_names"),
+        ]:
             vals = [proc._saferepr(x, maxwidth) for x in getattr(code, field)]
             if vals:
                 self.section(name)
                 m = self.columnize_commands(vals)
                 self.msg_nocr(m)
 
         return False
+
     pass
 
-if __name__ == '__main__':
-    from trepan.processor.command import mock, info as Minfo
+
+if __name__ == "__main__":
+    from trepan.processor.command import info as Minfo, mock
+
     d, cp = mock.dbg_setup()
     i = Minfo.InfoCommand(cp)
     sub = InfoCode(i)
     import inspect
+
     cp.curframe = inspect.currentframe()
     sub.run([])
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/display.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/display.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,41 +16,45 @@
 
 
 # Our local modules
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 
 
 class InfoDisplay(Mbase_subcmd.DebuggerSubcommand):
-    '''**info display**
+    """**info display**
 
-Show the display expression evaluated when the program stops.
+    Show the display expression evaluated when the program stops.
 
-See also:
----------
-`display`, `undisplay`'''
+    See also:
+    ---------
+    `display`, `undisplay`"""
 
     min_abbrev = 2  # info di
     need_stack = True
-    short_help = 'Expressions to display when program stops'
+    short_help = "Expressions to display when program stops"
 
     def run(self, args):
         lines = self.proc.display_mgr.all()
         if 0 == len(lines):
-            self.errmsg('There are no auto-display expressions now.')
+            self.errmsg("There are no auto-display expressions now.")
             return
         for line in lines:
             self.msg(line)
             pass
         return
+
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command import mock, info as Minfo
+
     d, cp = mock.dbg_setup()
     i = Minfo.InfoCommand(cp)
     sub = InfoDisplay(i)
     import inspect
+
     cp.curframe = inspect.currentframe()
     sub.run([])
-    sub.proc.display_mgr.add(cp.curframe, '/x i')
-    sub.proc.display_mgr.add(cp.curframe, 'd')
+    sub.proc.display_mgr.add(cp.curframe, "/x i")
+    sub.proc.display_mgr.add(cp.curframe, "d")
     sub.run([])
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/files.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/files.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,146 +1,158 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2008-2009, 2012-2013, 2015 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2008-2009, 2012-2013, 2015, 2023 Rocky Bernstein
+#   <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import columnize, inspect, pyficache, sys
+import inspect
+import sys
+
+import columnize
+import pyficache
 
-# Our local modules
-from trepan.processor.command.base_subcmd import DebuggerSubcommand
 from trepan import misc as Mmisc
 from trepan.lib import complete as Mcomplete
 from trepan.lib.file import file_list
 
+# Our local modules
+from trepan.processor.command.base_subcmd import DebuggerSubcommand
+
 
 class InfoFiles(DebuggerSubcommand):
     min_abbrev = 2
     need_stack = False
-    short_help = 'Show information about an imported or loaded Python file'
+    short_help = "Show information about an imported or loaded Python file"
 
     def complete(self, prefix):
-        completions = sorted(['.'] + file_list())
+        completions = sorted(["."] + file_list())
         return Mcomplete.complete_token(completions, prefix)
 
     def run(self, args):
         """**info files** [*filename* [**all** | **brkpts** | **lines** | **sha1** | **size**]]
 
-Show information about the current file. If no filename is
-given and the program is running then the current file associated
-with the current stack entry is used. Sub options which can be
-shown about a file are:
+        Show information about the current file. If no filename is
+        given and the program is running then the current file associated
+        with the current stack entry is used. Sub options which can be
+        shown about a file are:
 
-* **brkpts** Line numbers where there are statement boundaries. These lines can be used in breakpoint commands.
+        * **brkpts** Line numbers where there are statement boundaries. These lines can be used in breakpoint commands.
 
-* **sha1**	A SHA1 hash of the source text.
+        * **sha1**	A SHA1 hash of the source text.
 
-The following may be useful in comparing source code.
+        The following may be useful in comparing source code.
 
-* **size**	The number of lines in the file.
+        * **size**	The number of lines in the file.
 
-* **all** All of the above information.
+        * **all** All of the above information.
         """
         if len(args) == 0:
             if not self.proc.curframe:
                 self.errmsg("No frame - no default file.")
                 return False
             filename = self.proc.curframe.f_code.co_filename
         else:
             filename = args[0]
             pass
 
-        m = filename + ' is'
+        m = filename + " is"
         filename_cache = self.core.filename_cache
         if filename in filename_cache:
             m += " cached in debugger"
             if filename_cache[filename] != filename:
-                m += ' as:'
-                m = Mmisc.wrapped_lines(m, filename_cache[filename] + '.',
-                                        self.settings['width'])
+                m += " as:"
+                m = Mmisc.wrapped_lines(
+                    m, filename_cache[filename] + ".", self.settings["width"]
+                )
             else:
-                m += '.'
+                m += "."
                 pass
             self.msg(m)
         else:
-            matches = [file for file in file_list() if
-                       file.endswith(filename)]
-            if (len(matches) > 1):
+            matches = [file for file in file_list() if file.endswith(filename)]
+            if len(matches) > 1:
                 self.msg("Multiple files found ending filename string:")
                 for match_file in matches:
                     self.msg("\t%s" % match_file)
                     pass
             elif len(matches) == 1:
                 canonic_name = pyficache.unmap_file(matches[0])
-                m += " matched debugger cache file:\n  "  + canonic_name
+                m += " matched debugger cache file:\n  " + canonic_name
                 self.msg(m)
             else:
-                self.msg(m + ' not cached in debugger.')
+                self.msg(m + " not cached in debugger.")
             pass
         canonic_name = self.core.canonic(filename)
-        self.msg(Mmisc.wrapped_lines('Canonic name:', canonic_name,
-                                     self.settings['width']))
+        self.msg(
+            Mmisc.wrapped_lines("Canonic name:", canonic_name, self.settings["width"])
+        )
         for name in (canonic_name, filename):
             if name in sys.modules:
-                for key in [k for k, v in list(sys.modules.items())
-                            if name == v]:
+                for key in [k for k, v in list(sys.modules.items()) if name == v]:
                     self.msg("module: %s", key)
                     pass
                 pass
             pass
         for arg in args[1:]:
             processed_arg = False
-            if arg in ['all', 'size']:
+            if arg in ["all", "size"]:
                 if pyficache.size(canonic_name):
-                    self.msg("File has %d lines." %
-                             pyficache.size(canonic_name))
+                    self.msg("File has %d lines." % pyficache.size(canonic_name))
                     pass
                 processed_arg = True
                 pass
-            if arg in ['all', 'sha1']:
+            if arg in ["all", "sha1"]:
                 self.msg("SHA1 is %s." % pyficache.sha1(canonic_name))
                 processed_arg = True
                 pass
-            if arg in ['all', 'brkpts']:
+            if arg in ["all", "brkpts"]:
                 lines = pyficache.trace_line_numbers(canonic_name)
                 if lines:
                     self.section("Possible breakpoint line numbers:")
-                    fmt_lines = columnize.columnize(list(lines), ljust = False,
-                                                    arrange_vertical = False,
-                                                    lineprefix='  ')
+                    fmt_lines = columnize.columnize(
+                        list(lines),
+                        ljust=False,
+                        arrange_vertical=False,
+                        lineprefix="  ",
+                    )
                     self.msg(fmt_lines)
                     pass
                 processed_arg = True
                 pass
             if not processed_arg:
                 self.errmsg("Don't understand sub-option %s." % arg)
                 pass
             pass
         return
+
     pass
 
-if __name__ == '__main__':
-    from trepan.processor.command import mock, info as Minfo
+
+if __name__ == "__main__":
+    from trepan.processor.command import info as Minfo, mock
+
     d, cp = mock.dbg_setup()
     i = Minfo.InfoCommand(cp)
     sub = InfoFiles(i)
     sub.run([])
     cp.curframe = inspect.currentframe()
-    sub.run(['file.py', 'foo'])
+    sub.run(["file.py", "foo"])
     for width in (200, 80):
-        sub.settings['width'] = width
-        sub.run(['file.py', 'lines'])
+        sub.settings["width"] = width
+        sub.run(["file.py", "lines"])
         print(sub.run([]))
         pass
-    sub.run(['file.py', 'all'])
-    print(sub.complete(''))
+    sub.run(["file.py", "all"])
+    print(sub.complete(""))
     # sub.run(['file.py', 'lines', 'sha1'])
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/frame.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/frame.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2015 Rocky Bernstein <rocky@gnu.org>
+#   Copyright (C) 2015, 2023 Rocky Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -11,123 +11,137 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import inspect
+
 # Our local modules
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 from trepan.lib import complete as Mcomplete
 from trepan.processor import frame as Mframe
 
 
 class InfoFrame(Mbase_subcmd.DebuggerSubcommand):
     """**info frame** [-v] [ *frame-number* | *frame-object* ]
 
-Show the detailed information for *frame-number* or the current frame if
-*frame-number* is not specified. You can also give a frame object instead of
-a frame number
+    Show the detailed information for *frame-number* or the current frame if
+    *frame-number* is not specified. You can also give a frame object instead of
+    a frame number
 
-Specific information includes:
+    Specific information includes:
 
-* the frame number (if not an object)
+    * the frame number (if not an object)
 
-* the source-code line number that this frame is stopped in
+    * the source-code line number that this frame is stopped in
 
-* the last instruction executed; -1 if the program are before the first
-instruction
+    * the last instruction executed; -1 if the program are before the first
+    instruction
 
-* a function that tracing this frame or `None`
+    * a function that tracing this frame or `None`
 
-* Whether the frame is in restricted execution
+    * Whether the frame is in restricted execution
 
-If `-v` is given we show builtin and global names the frame sees.
+    If `-v` is given we show builtin and global names the frame sees.
 
-See also:
----------
+    See also:
+    ---------
 
-`info locals`, `info globals`, `info args`"""
+    `info locals`, `info globals`, `info args`"""
 
     min_abbrev = 2
     max_args = 2
     need_stack = True
-    short_help = '''Show detailed info about the current frame'''
+    short_help = """Show detailed info about the current frame"""
 
     def complete(self, prefix):
         proc_obj = self.proc
         low, high = Mframe.frame_low_high(proc_obj, None)
-        ary = [str(low+i) for i in range(high-low+1)]
+        ary = [str(low + i) for i in range(high - low + 1)]
         # FIXME: add in Thread names
         return Mcomplete.complete_token(ary, prefix)
 
     def run(self, args):
 
         # FIXME: should DRY this with code.py
         proc = self.proc
         frame = proc.curframe
         if not frame:
             self.errmsg("No frame selected.")
             return False
 
         show_lists = False
-        if len(args) >= 1 and args[0] == '-v':
+        if len(args) >= 1 and args[0] == "-v":
             args.pop(0)
             show_lists = True
 
         frame_num = None
         if len(args) == 1:
             try:
                 frame_num = int(args[0])
                 i_stack = len(proc.stack)
-                if frame_num < -i_stack or frame_num > i_stack-1:
-                    self.errmsg(('a frame number number has to be in the range %d to %d.' +
-                                 ' Got: %d (%s).') % (-i_stack, i_stack-1,
-                                                      frame_num, args[0]))
+                if frame_num < -i_stack or frame_num > i_stack - 1:
+                    self.errmsg(
+                        (
+                            "a frame number number has to be in the range %d to %d."
+                            + " Got: %d (%s)."
+                        )
+                        % (-i_stack, i_stack - 1, frame_num, args[0])
+                    )
                     return False
                 frame = proc.stack[frame_num][0]
-            except:
+            except Exception:
                 try:
                     frame = eval(args[0], frame.f_globals, frame.f_locals)
-                except:
-                    self.errmsg('%s is not a evaluable as a frame object or frame number.' %
-                                 args[0])
+                except Exception:
+                    self.errmsg(
+                        "%s is not a evaluable as a frame object or frame number."
+                        % args[0]
+                    )
                     return False
                 if not inspect.isframe(frame):
-                    self.errmsg('%s is not a frame object' % frame)
+                    self.errmsg("%s is not a frame object" % frame)
                 pass
         else:
             frame_num = proc.curindex
 
-        mess = 'Frame %d' % Mframe.frame_num(proc, frame_num) \
-          if frame_num is not None else 'Frame Info'
+        mess = (
+            "Frame %d" % Mframe.frame_num(proc, frame_num)
+            if frame_num is not None and proc.stack is not None
+            else "Frame Info"
+        )
         self.section(mess)
-        if hasattr(frame, 'f_restricted'):
-            self.msg('  restricted execution: %s' % frame.f_restricted)
-        self.msg('  current line number: %d' % frame.f_lineno)
-        self.msg('  last instruction: %d' % frame.f_lasti)
-        self.msg('  code: %s' % frame.f_code)
-        self.msg('  previous frame: %s' % frame.f_back)
-        self.msg('  tracing function: %s' % frame.f_trace)
+        if hasattr(frame, "f_restricted"):
+            self.msg("  restricted execution: %s" % frame.f_restricted)
+        self.msg("  current line number: %d" % frame.f_lineno)
+        self.msg("  last instruction: %d" % frame.f_lasti)
+        self.msg("  code: %s" % frame.f_code)
+        self.msg("  previous frame: %s" % frame.f_back)
+        self.msg("  tracing function: %s" % frame.f_trace)
 
         if show_lists:
-            for name, field in [('Globals', 'f_globals'),
-                                ('Builtins', 'f_builtins'),
-                                ]:
+            for name, field in [
+                ("Globals", "f_globals"),
+                ("Builtins", "f_builtins"),
+            ]:
                 vals = getattr(frame, field).keys()
                 if vals:
                     self.section(name)
                     m = self.columnize_commands(vals)
                     self.msg_nocr(m)
 
         return False
+
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command import mock, info as Minfo
+
     d, cp = mock.dbg_setup()
     cp.setup()
     i = Minfo.InfoCommand(cp)
 
     sub = InfoFrame(i)
     cp.curframe = inspect.currentframe()
     sub.run([])
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/globals.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/globals.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,59 +19,74 @@
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 from trepan.lib import pp as Mpp
 
 
 class InfoGlobals(Mbase_subcmd.DebuggerSubcommand):
     """**info globals** [*var1 ...*]
 
-**info globals** *
+    **info globals** *
 
-With no arguments, show all of the global variables of the current stack
-frame. If a list of names is provide limit display to just those
-variables.
+    With no arguments, show all of the global variables of the current stack
+    frame. If a list of names is provide limit display to just those
+    variables.
 
-If `*` is given, just show the variable names, not the values.
+    If `*` is given, just show the variable names, not the values.
+
+    See also:
+    ---------
+    `info locals`, `info args`, `info frame`"""
 
-See also:
----------
-`info locals`, `info args`, `info frame`"""
     min_abbrev = 2
     need_stack = True
-    short_help = '''Show the debugged programs's global variables'''
+    short_help = """Show the debugged programs's global variables"""
 
     def run(self, args):
         if not self.proc.curframe:
             self.errmsg("No frame selected.")
             return False
         names = list(self.proc.curframe.f_globals.keys())
-        if len(args) > 0 and args[0] == '*' :
+        if len(args) > 0 and args[0] == "*":
             self.section("globals")
             self.msg(self.columnize_commands(names))
         elif len(args) == 0:
             names.sort()
             for name in sorted(names):
                 val = self.proc.getval(name)
-                Mpp.pp(val, self.settings['width'], self.msg_nocr, self.msg,
-                       prefix='%s =' % name)
+                Mpp.pp(
+                    val,
+                    self.settings["width"],
+                    self.msg_nocr,
+                    self.msg,
+                    prefix="%s =" % name,
+                )
                 pass
         else:
             for name in args:
                 if name in names:
                     val = self.proc.getval(name)
-                    Mpp.pp(val, self.settings['width'], self.msg_nocr,
-                           self.msg, prefix='%s =' % name)
+                    Mpp.pp(
+                        val,
+                        self.settings["width"],
+                        self.msg_nocr,
+                        self.msg,
+                        prefix="%s =" % name,
+                    )
                     pass
                 else:
                     self.errmsg("%s is not a global variable" % name)
                     pass
                 pass
         return False
+
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command import mock, info as Minfo
+
     d, cp = mock.dbg_setup()
     i = Minfo.InfoCommand(cp)
     sub = InfoGlobals(i)
     import inspect
+
     cp.curframe = inspect.currentframe()
     sub.run([])
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/line.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/line.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2008-2009, 2013, 2015, 2020 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2008-2009, 2013, 2015, 2020, 2023 Rocky Bernstein
+#   <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import inspect, re
+import inspect
 import os.path as osp
+import re
+
+from pyficache import code_line_info
 
-# Our local modules
-from trepan.processor.command.base_subcmd import DebuggerSubcommand
 from trepan.clifns import search_file
 from trepan.misc import wrapped_lines
 from trepan.processor.cmdbreak import parse_break_cmd
-from pyficache import code_line_info
+
+# Our local modules
+from trepan.processor.command.base_subcmd import DebuggerSubcommand
 
 
 def find_function(funcname, filename):
     cre = re.compile(r"def\s+%s\s*[(]" % re.escape(funcname))
     try:
         fp = open(filename)
     except IOError:
@@ -45,44 +50,44 @@
     fp.close()
     return answer
 
 
 class InfoLine(DebuggerSubcommand):
     """**info line* [*location*]
 
-Show line information for location *location*.
+    Show line information for location *location*.
 
-If no location is given, use the the current stopped line.
+    If no location is given, use the the current stopped line.
 
-Examples
---------
+    Examples
+    --------
 
-    (trepan3k) info line
-    Line 3 of "/tmp/python3-trepan/test/example/multi-line.py"
-        starts at offset 0 of <module> and contains 2 instructions
-    There are multiple line offsets this line number. Other line offsets: 4 of <module>
+        (trepan3k) info line
+        Line 3 of "/tmp/python3-trepan/test/example/multi-line.py"
+            starts at offset 0 of <module> and contains 2 instructions
+        There are multiple line offsets this line number. Other line offsets: 4 of <module>
 
-    (trepan3k) info line 5
-    Line 5 of "/tmp/python3-trepan/test/example/multi-line.py"
-        starts at offset 16 of <module> and contains 7 instructions
+        (trepan3k) info line 5
+        Line 5 of "/tmp/python3-trepan/test/example/multi-line.py"
+            starts at offset 16 of <module> and contains 7 instructions
 
-See also:
----------
-`info program`, `info frame`"""
+    See also:
+    ---------
+    `info program`, `info frame`"""
 
     min_abbrev = 2
     max_args = 4
     need_stack = False
     short_help = "Show line information"
 
     def lineinfo(self, arg):
         (func, filename, lineno, condition, offset) = parse_break_cmd(
             self.proc, ["info args"]
         )
-        if filename != None and lineno != None:
+        if filename is not None and lineno is not None:
             return lineno, filename
         else:
             return None, None
 
     def run(self, args):
         """Current line number in source file"""
         if not self.proc.curframe:
@@ -119,31 +124,33 @@
             self.msg(wrapped_lines(msg1, msg2, self.settings["width"]))
         else:
             self.errmsg(
                 "No line information for line %d of %s"
                 % (line_number, self.core.filename(filename))
             )
         if line_info and len(line_info) > 1:
-            self.msg(wrapped_lines(
-                "There are multiple line offsets for line number.",
-                "Other line offsets: %s"
-                % ", ".join(
-                    ["%s of %s" % (li.offsets[0], li.name) for li in line_info[1:]]),
-                self.settings["width"]
+            self.msg(
+                wrapped_lines(
+                    "There are multiple line offsets for line number.",
+                    "Other line offsets: %s"
+                    % ", ".join(
+                        ["%s of %s" % (li.offsets[0], li.name) for li in line_info[1:]]
+                    ),
+                    self.settings["width"],
                 )
             )
         return False
 
     pass
 
 
 if __name__ == "__main__":
+    from trepan.debugger import Trepan
     from trepan.processor.command import mock
     from trepan.processor.command.info import InfoCommand
-    from trepan.debugger import Trepan
 
     d = Trepan()
     d, cp = mock.dbg_setup(d)
     i = InfoCommand(cp)
     sub = InfoLine(i)
     cp.curframe = inspect.currentframe()
     for width in (80, 200):
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/lines.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/lines.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,54 +22,58 @@
 from trepan.misc import pretty_modfunc_name
 from pyficache import cache_code_lines
 
 
 class InfoOffsets(DebuggerSubcommand):
     """**info lines** [-n *function-or-module*]
 
-Show line - function/offset information
-Use -n *function-or-module* to filter results.
+    Show line - function/offset information
+    Use -n *function-or-module* to filter results.
 
-Examples
---------
+    Examples
+    --------
 
-    (trepan3k) info lines
-    Line - (fn, start offset) table for test/example/gcd.py
-      10: <module> @0         21: check_args() @84     36: gcd() @30
-      11: <module> @4         22: check_args() @106    37: gcd() @50
-      13: <module> @12        23: check_args() @116    38: gcd() @54
-      14: check_args() @0     24: check_args() @122    40: <module> @28
-      16: check_args() @14    26: <module> @20         41: <module> @36
-      17: check_args() @22    30: gcd() @0             43: <module> @42
-      18: check_args() @36    31: gcd() @8             44: <module> @60
-      19: check_args() @38    34: gcd() @18            45: <module> @84
-      20: check_args() @70    35: gcd() @26
-    (trepan3k) info lines -n <module>
-      10: <module> @0    11: <module> @4   13: <module> @12
-      40: <module> @28   26: <module> @20  41: <module> @36
-      43: <module> @42   44: <module> @60  45: <module> @84
-    (trepan3k) info lines -n gcd
-      30: gcd() @0   31: gcd() @8   34: gcd() @18
-      35: gcd() @26  36: gcd() @30  37: gcd() @50
-      38: gcd() @54
-
-See also:
----------
-`info line`, `info offsets`, `info file`, `info program`, and `info frame`"""
+        (trepan3k) info lines
+        Line - (fn, start offset) table for test/example/gcd.py
+          10: <module> @0         21: check_args() @84     36: gcd() @30
+          11: <module> @4         22: check_args() @106    37: gcd() @50
+          13: <module> @12        23: check_args() @116    38: gcd() @54
+          14: check_args() @0     24: check_args() @122    40: <module> @28
+          16: check_args() @14    26: <module> @20         41: <module> @36
+          17: check_args() @22    30: gcd() @0             43: <module> @42
+          18: check_args() @36    31: gcd() @8             44: <module> @60
+          19: check_args() @38    34: gcd() @18            45: <module> @84
+          20: check_args() @70    35: gcd() @26
+        (trepan3k) info lines -n <module>
+          10: <module> @0    11: <module> @4   13: <module> @12
+          40: <module> @28   26: <module> @20  41: <module> @36
+          43: <module> @42   44: <module> @60  45: <module> @84
+        (trepan3k) info lines -n gcd
+          30: gcd() @0   31: gcd() @8   34: gcd() @18
+          35: gcd() @26  36: gcd() @30  37: gcd() @50
+          38: gcd() @54
+
+    See also:
+    ---------
+    `info line`, `info offsets`, `info file`, `info program`, and `info frame`"""
 
     min_abbrev = 5
     max_args = 2
     need_stack = False
     short_help = "Show line offset information for a file or module"
 
     def run(self, args):
         """Current line number in source file"""
         # info line <loc>
         try:
-            opts, args = getopt(args, "hn:", ["help", "name"],)
+            opts, args = getopt(
+                args,
+                "hn:",
+                ["help", "name"],
+            )
         except GetoptError:
             # print help information and exit:
             self.errmsg(
                 str(sys.exc_info()[1])
             )  # will print something like "option -a not recognized"
             return
 
@@ -102,16 +106,18 @@
                 if not name or any(li.name == name for li in line_info):
                     lines.append(
                         "%4d: %s"
                         % (
                             line_number,
                             ", ".join(
                                 [
-                                    "%s @%d" % (pretty_modfunc_name(li.name), li.offsets[0])
-                                    for li in line_info if not name or li.name == name
+                                    "%s @%d"
+                                    % (pretty_modfunc_name(li.name), li.offsets[0])
+                                    for li in line_info
+                                    if not name or li.name == name
                                 ]
                             ),
                         )
                     )
             m = self.columnize_commands(list(sorted(lines)))
             self.msg(m)
         else:
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/locals.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/locals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2008-2009, 2013, 2015, 2018, 2020 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2008-2009, 2013, 2015, 2018, 2020, 2023 Rocky
+#   Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -21,41 +23,40 @@
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 from trepan.lib import pp as Mpp
 from trepan.lib import complete as Mcomplete
 
 # when the "with" statement is used, there
 # can be get variables having names
 # _[1], _[2], etc.
-_with_local_varname = re.compile(r'_\[[0-9+]\]')
+_with_local_varname = re.compile(r"_\[[0-9+]\]")
+
 
 class InfoLocals(Mbase_subcmd.DebuggerSubcommand):
     """**info locals** [-l | --list | | -h --help]
 
-    **info locals** [*var1 ...*]
+        **info locals** [*var1 ...*]
 
-**info locals** *
+    **info locals** *
 
-With no arguments, show all of the local variables of the current stack
-frame. If a list of names is provide limit display to just those
-variables.
+    With no arguments, show all of the local variables of the current stack
+    frame. If a list of names is provide limit display to just those
+    variables.
 
-If `*` is given, just show the variable names, not the values.
+    If `*` is given, just show the variable names, not the values.
 
-See also:
----------
-`info globals`, `info args`, `info frame`
-"""
+    See also:
+    ---------
+    `info globals`, `info args`, `info frame`"""
 
     min_abbrev = 2
     need_stack = True
     short_help = "Show the local variables of current stack frame"
 
     def complete(self, prefix):
-        completions = sorted(['*'] +
-                              self.proc.curframe.f_locals.keys())
+        completions = sorted(["*"] + self.proc.curframe.f_locals.keys())
         return Mcomplete.complete_token(completions, prefix)
 
     def run(self, args):
         if not self.proc.curframe:
             self.errmsg("No frame selected")
             return False
 
@@ -80,67 +81,78 @@
             elif o in ("-l", "--list"):
                 list_only = True
             else:
                 self.errmsg("unhandled option '%s'" % o)
             pass
         pass
 
-
         names = list(self.proc.curframe.f_locals.keys())
 
         if list_only:
             for name in names:
                 self.msg(name)
             return
-        if len(args) > 0 and args[0] == '*' :
+        if len(args) > 0 and args[0] == "*":
             self.section("locals")
             self.msg(self.columnize_commands(names))
         elif len(args) == 0:
             for name in sorted(names):
                 # ALB: a fix for a problem with the new 'with'
                 # statement. It seems to work, but I don't know exactly
                 # why... (the problem was in self.getval called by
                 # info_locals)
                 if _with_local_varname.match(name):
                     val = self.proc.curframe.f_locals[name]
                 else:
                     val = self.proc.getval(name)
                     pass
-                Mpp.pp(val, self.settings['width'], self.msg_nocr, self.msg,
-                       prefix='%s =' % name)
+                Mpp.pp(
+                    val,
+                    self.settings["width"],
+                    self.msg_nocr,
+                    self.msg,
+                    prefix="%s =" % name,
+                )
                 pass
             pass
         else:
             for name in args:
                 # ALB: a fix for a problem with the new 'with'
                 # statement. It seems to work, but I don't know exactly
                 # why... (the problem was in self.getval called by
                 # info_locals)
                 if name in names:
                     if _with_local_varname.match(name):
                         val = self.proc.curframe.f_locals[name]
                     else:
                         val = self.proc.getval(name)
                         pass
-                    Mpp.pp(val, self.settings['width'], self.msg_nocr,
-                           self.msg,
-                           prefix='%s =' % name)
+                    Mpp.pp(
+                        val,
+                        self.settings["width"],
+                        self.msg_nocr,
+                        self.msg,
+                        prefix="%s =" % name,
+                    )
                 else:
                     self.errmsg("%s is not a local variable" % name)
                     pass
         return False
+
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command import mock, info as Minfo
     from trepan import debugger as Mdebugger
+
     d = Mdebugger.Trepan()
     d, cp = mock.dbg_setup(d)
     i = Minfo.InfoCommand(cp)
     sub = InfoLocals(i)
-    l = list(range(30))  # Add a simple array to the local mix printed below.
     import inspect
+
     cp.curframe = inspect.currentframe()
     sub.run([])
-    sub.run(['*'])
-    sub.run(['Minfo'])
+    sub.run(["*"])
+    sub.run(["Minfo"])
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/macro.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/macro.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,62 +20,65 @@
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 from trepan.lib import complete as Mcomplete
 
 
 class InfoMacro(Mbase_subcmd.DebuggerSubcommand):
     """**info macro * ***
 
-**info macro** *macro1* [*macro2* ..]
+    **info macro** *macro1* [*macro2* ..]
 
-In the first form a list of the existing macro names are shown
-in column format.
+    In the first form a list of the existing macro names are shown
+    in column format.
 
-In the second form, all macro names and their definitions are shown.
+    In the second form, all macro names and their definitions are shown.
 
-In the last form the only definitions of the given macro names is shown."""
+    In the last form the only definitions of the given macro names is shown."""
 
     min_abbrev = 1
     need_stack = True
     short_help = "List of defined macros"
 
     def complete(self, prefix):
-        m = sorted(list(self.proc.macros.keys()) + ['*'])
+        m = sorted(list(self.proc.macros.keys()) + ["*"])
         return Mcomplete.complete_token(m, prefix)
 
     def run(self, args):
         if len(args) > 0:
-            if len(args) == 1 and '*' == args[0]:
+            if len(args) == 1 and "*" == args[0]:
                 macro_names = list(self.proc.macros.keys())
             else:
                 macro_names = args
                 pass
 
             for macro_name in sorted(macro_names):
                 if macro_name in self.proc.macros:
                     self.section("%s:" % macro_name)
                     string = self.proc.macros[macro_name][1]
-                    highlight = self.settings['highlight']
-                    if highlight in ['light', 'dark']:
+                    highlight = self.settings["highlight"]
+                    if highlight in ["light", "dark"]:
                         string = highlight_string(string, highlight)
                         pass
                     self.msg("  %s" % string)
                 else:
-                    self.errmsg('%s is not a defined macro' % macro_name)
+                    self.errmsg("%s is not a defined macro" % macro_name)
                     pass
                 pass
         elif 0 == len(list(self.proc.macros.keys())):
-            self.msg('No macros defined.')
+            self.msg("No macros defined.")
         else:
             self.msg(self.columnize_commands(list(self.proc.macros.keys())))
             pass
         return
+
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     # Demo it.
     from trepan.processor.command import mock, info as Minfo
+
     d, cp = mock.dbg_setup()
     i = Minfo.InfoCommand(cp)
     sub = InfoMacro(i)
     sub.run(["u"])
-    print(sub.complete(''))
+    print(sub.complete(""))
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/offsets.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/offsets.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 from trepan.processor.command.base_subcmd import DebuggerSubcommand
 from pyficache import cache_code_lines
 
 
 class InfoOffsets(DebuggerSubcommand):
     """**info offsets** [*function-file-or-module*]
 
-Show line offset information for a function, module, or a file.
+    Show line offset information for a function, module, or a file.
 
-If no location is given, use the the current frame.
+    If no location is given, use the the current frame.
 
-Examples
---------
+    Examples
+    --------
 
-    (trepan3k) info offsets
-    Offset - line number table for offsets.py
-           0:  16    40:  23    72:  94   108:  98   136: 101   164: 104   188: 107
-          16:  19    48:  45    84:  95   114:  99   144: 102   174: 105
-          28:  20    64:  93    96:  96   128: 100   154: 103   184: 106
-
-See also:
----------
-`info line`, `info program`, `info frame`"""
+        (trepan3k) info offsets
+        Offset - line number table for offsets.py
+               0:  16    40:  23    72:  94   108:  98   136: 101   164: 104   188: 107
+              16:  19    48:  45    84:  95   114:  99   144: 102   174: 105
+              28:  20    64:  93    96:  96   128: 100   154: 103   184: 106
+
+    See also:
+    ---------
+    `info line`, `info program`, `info frame`"""
 
     min_abbrev = 2
     max_args = 2
     need_stack = False
     short_help = "Show line offset information for a file or module"
 
     def run(self, args):
@@ -51,41 +51,46 @@
             curframe = self.proc.curframe
             if not curframe:
                 self.errmsg("No line number information available.")
                 return
 
             # No line number. Use current frame line number
             filename = curframe.f_code.co_filename
-            file_info = cache_code_lines(filename, toplevel_only=False, include_offsets=True)
+            file_info = cache_code_lines(
+                filename, toplevel_only=False, include_offsets=True
+            )
             if file_info:
                 self.section("Offset - line number table for %s" % filename)
-                offsets = ["@%4d:%4d" % (offset, line) for offset, line in file_info.linestarts.items()]
+                offsets = [
+                    "@%4d:%4d" % (offset, line)
+                    for offset, line in file_info.linestarts.items()
+                ]
                 m = self.columnize_commands(list(sorted(offsets)))
                 self.msg(m)
             else:
-                self.errmsg(
-                    "haven't recorded info for offset file %s" % filename
-                )
+                self.errmsg("haven't recorded info for offset file %s" % filename)
                 pass
             pass
         else:
             self.errmsg("Passing a filename, function, or module not completed yet...")
         return
+
     pass
 
 
 if __name__ == "__main__":
     from trepan.processor.command import mock
     from trepan.processor.command.info import InfoCommand
     from trepan.debugger import Trepan
 
     d = Trepan()
     d, cp = mock.dbg_setup(d)
     i = InfoCommand(cp)
     sub = InfoOffsets(i)
     import inspect
+
     cp.curframe = inspect.currentframe()
     for width in (80, 200):
         sub.settings["width"] = width
         sub.run([])
         pass
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/pc.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/pc.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,22 +27,21 @@
 # requires a running program whereas where we just use f_lasti.
 # What we have here is more flexible in the presence of exceptions.
 # trepan3k would have to be looked over to see if it too would
 # work.
 class InfoPC(DebuggerSubcommand):
     """**info pc**
 
-List the current program counter or bytecode offset,
-and disassemble the instructions around that.
+    List the current program counter or bytecode offset,
+    and disassemble the instructions around that.
 
-See also:
----------
+    See also:
+    ---------
 
-`info line`, `info program`
-"""
+    `info line`, `info program`"""
 
     min_abbrev = 2  # Need at least info 'pc'
     max_args = 0
     need_stack = True
     short_help = "Show Program Counter or Instruction Offset information"
 
     def run(self, args):
@@ -56,19 +55,19 @@
                 self.msg("PC offset is %d." % offset)
                 offset = max(offset, 0)
                 code = curframe.f_code
                 co_code = code.co_code
                 disassemble_bytes(
                     self.msg,
                     self.msg_nocr,
-                    code = co_code,
-                    lasti = offset,
-                    cur_line = line_no,
-                    start_line = line_no - 1,
-                    end_line = line_no + 1,
+                    code=co_code,
+                    lasti=offset,
+                    cur_line=line_no,
+                    start_line=line_no - 1,
+                    end_line=line_no + 1,
                     varnames=code.co_varnames,
                     names=code.co_names,
                     constants=code.co_consts,
                     cells=code.co_cellvars,
                     freevars=code.co_freevars,
                     linestarts=dict(findlinestarts(code)),
                     end_offset=offset + 10,
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/program.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/program.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,26 +18,26 @@
 from trepan.processor.command.base_subcmd import DebuggerSubcommand
 from trepan.misc import wrapped_lines
 
 
 class InfoProgram(DebuggerSubcommand):
     """**info program**
 
-Execution status of the program. Listed are:
+    Execution status of the program. Listed are:
 
-* Program name
+    * Program name
 
-* Instruction PC
+    * Instruction PC
 
-* Reason the program is stopped.
+    * Reason the program is stopped.
 
-See also:
----------
+    See also:
+    ---------
 
-`info line`, `info args`, `info frame`, `info pc`"""
+    `info line`, `info args`, `info frame`, `info pc`"""
 
     min_abbrev = 2  # Need at least "info pr"
     max_args = 0
     need_stack = True
     short_help = "Execution status of the program"
 
     def run(self, args):
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/return.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/return.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,39 +14,44 @@
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 # Our local modules
 from trepan.processor.command.base_subcmd import DebuggerSubcommand
 from pprint import pformat
 
+
 class InfoReturn(DebuggerSubcommand):
     """return value
 
-Show the value that is to be returned from a function.  This command
-is useful after a 'finish' command or stepping just after a 'return'
-statement."""
-
-    min_abbrev    = 1
-    need_stack    = True
-    short_help    = 'Show function return value'
+    Show the value that is to be returned from a function.  This command
+    is useful after a 'finish' command or stepping just after a 'return'
+    statement."""
+
+    min_abbrev = 1
+    need_stack = True
+    short_help = "Show function return value"
 
     def run(self, args):
         # pdb checks to see if __return__ is the frame's f_locals which doesn't work
         # at least on any Python I am aware of back to 2.4.
         # Testing on the event however does work.
-        if self.proc.event in ['return', 'exception']:
+        if self.proc.event in ["return", "exception"]:
             val = self.proc.event_arg
             formatted_val = pformat(val)
             self.msg("return value (type %s):\n\t%s" % (type(val), formatted_val))
         else:
-            self.errmsg("Must be in a 'return' or 'exception' event "
-                        "rather than a %s event." % self.proc.event)
+            self.errmsg(
+                "Must be in a 'return' or 'exception' event "
+                "rather than a %s event." % self.proc.event
+            )
             pass
         return
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command import mock, info as Minfo
+
     d, cp = mock.dbg_setup()
     i = Minfo.InfoCommand(cp)
     sub = InfoReturn(i)
     print(sub.run([]))
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/signals.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/signals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2015 Rocky Bernstein <rocky@gnu.org>
+#   Copyright (C) 2009, 2015, 2023 Rocky Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -13,54 +13,56 @@
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 # Our local modules
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 from trepan.lib import complete as Mcomplete
-import columnize
 
 
 class InfoSignals(Mbase_subcmd.DebuggerSubcommand):
-    '''**info signals** [*signal-name*]
+    r"""**info signals** [*signal-name*]
 
-**info signals** \*
+    **info signals** *
 
-Show information about how debugger treats signals to the program.
-Here are the boolean actions we can take:
+    Show information about how debugger treats signals to the program.
+    Here are the boolean actions we can take:
 
- * Stop: enter the debugger when the signal is sent to the debugged program
+     * Stop: enter the debugger when the signal is sent to the debugged program
 
- * Print: print that the signal was received
+     * Print: print that the signal was received
 
- * Stack: show a call stack
+     * Stack: show a call stack
 
- * Pass: pass the signal onto the program
+     * Pass: pass the signal onto the program
 
-If *signal-name* is not given, we the above show information for all
-signals. If '*' is given we just give a list of signals.
- '''
+    If *signal-name* is not given, we the above show information for all
+    signals. If '*' is given we just give a list of signals.
+    """
 
     min_abbrev = 3  # info sig
     need_stack = False
-    short_help = 'What debugger does when program gets various signals'
+    short_help = "What debugger does when program gets various signals"
 
     def complete(self, prefix):
-        completions = sorted(['*'] + self.debugger.sigmgr.siglist)
+        completions = sorted(["*"] + self.debugger.sigmgr.siglist)
         return Mcomplete.complete_token(completions, prefix)
 
     def run(self, args):
-        if len(args) > 0 and args[0] == '*' :
+        if len(args) > 0 and args[0] == "*":
             self.msg(self.columnize_commands(self.debugger.sigmgr.siglist))
         else:
-            self.debugger.sigmgr.info_signal(['signal'] + args)
+            self.debugger.sigmgr.info_signal(["signal"] + args)
         return
+
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command import mock, info as Minfo
+
     d, cp = mock.dbg_setup()
     i = Minfo.InfoCommand(cp)
     sub = InfoSignals(i)
     # sub.run([])
     # sub.run(['*'])
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/source.py` & `trepan3k-1.2.9/trepan/processor/command/show_subcmd/confirm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2008-2009, 2013, 2015 Rocky Bernstein <rocky@gnu.org>
+#   Copyright (C) 2009, 2013, 2015 Rocky Bernstein
 #
-#   This program is free software: you can redistribute it and/or modify
-#   it under the terms of the GNU General Public License as published by
-#   the Free Software Foundation, either version 3 of the License, or
-#   (at your option) any later version.
+#  This program is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
 #
-#   This program is distributed in the hope that it will be useful,
-#   but WITHOUT ANY WARRANTY; without even the implied warranty of
-#   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#   GNU General Public License for more details.
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
 #
-#   You should have received a copy of the GNU General Public License
-#   along with this program.  If not, see <http://www.gnu.org/licenses/>.
+#  You should have received a copy of the GNU General Public License
+#  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 # Our local modules
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 
 
-class InfoSource(Mbase_subcmd.DebuggerSubcommand):
-    """Information about the current Python file."""
+class ShowConfirm(Mbase_subcmd.DebuggerShowBoolSubcommand):
+    """**show confirm**
 
-    min_abbrev = 1
-    need_stack = True
-    short_help = "Information about the current Python file"
-
-    def run(self, args):
-        if not self.proc.curframe:
-            self.errmsg("No current source file.")
-            return
-        filename = self.core.canonic_filename(self.proc.curframe)
-        self.msg('Current Python file is %s' % self.core.filename(filename))
-        return False
+    Show confirmation of potentially dangerous operations
+
+    See also:
+    ---------
+
+    `set confirm`"""
+
+    min_abbrev = 3  # Need at least "show con"
+    pass
+
+
+if __name__ == "__main__":
+    from trepan.processor.command.show_subcmd import __demo_helper__ as Mhelper
+
+    Mhelper.demo_run(ShowConfirm)
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/info_subcmd/threads.py` & `trepan3k-1.2.9/trepan/processor/command/info_subcmd/threads.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,73 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2014 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2009, 2014, 2023 Rocky Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import sys, threading
+import sys
+import threading
+
+from trepan.lib import stack as Mstack, thred as Mthread
 
 # Our local modules
 from trepan.processor.command import base_subcmd as Mbase_subcmd
-from trepan.lib import stack as Mstack, thred as Mthread
 
 
 # FIXME turn into yet another subcommand thingy.
 class InfoThread(Mbase_subcmd.DebuggerSubcommand):
     """**info threads** [*thread-name*|*thread-number*] [**terse**|**verbose**]
 
-List all currently-known thread name(s).
+    List all currently-known thread name(s).
+
+    If no thread name is given, we list info for all threads. Unless a
+    terse listing, for each thread we give:
 
-If no thread name is given, we list info for all threads. Unless a
-terse listing, for each thread we give:
+      - the class, thread name, and status as *Class(Thread-n, status)*
 
-  - the class, thread name, and status as *Class(Thread-n, status)*
+      - the top-most call-stack information for that thread.
 
-  - the top-most call-stack information for that thread.
+    Generally the top-most calls into the debugger and dispatcher are
+    omitted unless set dbg_trepan is *True*.
 
-Generally the top-most calls into the debugger and dispatcher are
-omitted unless set dbg_trepan is *True*.
+    If 'verbose' appended to the end of the command, then the entire stack
+    trace is given for each frame.  If 'terse' is appended we just list
+    the thread name and thread id.
 
-If 'verbose' appended to the end of the command, then the entire stack
-trace is given for each frame.  If 'terse' is appended we just list
-the thread name and thread id.
+    To get the full stack trace for a specific thread pass in the thread name."""
 
-To get the full stack trace for a specific thread pass in the thread name.
-"""
     min_abbrev = 2  # Min is "info th"
     max_args = 2
     need_stack = True
     short_help = "List thread info"
 
     def __init__(self, cmd):
         Mbase_subcmd.DebuggerSubcommand.__init__(self, cmd)
         self.name2id = {}
         return
 
     def stack_trace(self, f):
         """A mini stack trace routine for threads."""
         while f:
-            if (not self.core.ignore_filter.is_included(f)
-                or self.settings['dbg_trepan']):
+            if (
+                not self.core.ignore_filter.is_included(f)
+                or self.settings["dbg_trepan"]
+            ):
                 s = Mstack.format_stack_entry(self, (f, f.f_lineno))
-                self.msg(" "*4 + s)
+                self.msg(" " * 4 + s)
                 pass
             f = f.f_back
             pass
         return
 
     def info_thread_terse(self, name2id, arg=None):
         if arg is not None:
@@ -81,23 +86,22 @@
             self.info_thread_line(thread_name, name2id)
             pass
         # self.info_thread_missing()
         return
 
     def info_thread_line(self, thread_name, name2id):
         if thread_name == self.proc.frame_thread_name:
-            prefix = '-> '
+            prefix = "-> "
         elif thread_name == self.proc.thread_name:
-            prefix = '=> '
+            prefix = "=> "
         else:
-            prefix = '   '
+            prefix = "   "
             pass
 
-        self.msg("%s%s: %d" % (prefix, thread_name,
-                               name2id[thread_name]))
+        self.msg("%s%s: %d" % (prefix, thread_name, name2id[thread_name]))
         return
 
     def run(self, args):
         # FIXME: add thread locking here?
 
         self.thread_name = Mthread.current_thread_name()
 
@@ -109,30 +113,29 @@
             if name not in list(self.name2id.keys()):
                 self.name2id[name] = thread_id
                 pass
             pass
 
         all_verbose = False
         if len(args) == 1:
-            if args[0].startswith('verbose'):
+            if args[0].startswith("verbose"):
                 all_verbose = True
-            elif args[0].startswith('terse'):
+            elif args[0].startswith("terse"):
                 self.info_thread_terse(name2id)
                 return
             pass
 
         if len(args) > 0 and not all_verbose:
             thread_name = args[0]
-            if thread_name == '.':
+            if thread_name == ".":
                 thread_name = self.thread_name
             try:
                 thread_id = int(thread_name)
                 if thread_id not in list(threading._active.keys()):
-                    self.errmsg("Don't know about thread number %s" %
-                                thread_name)
+                    self.errmsg("Don't know about thread number %s" % thread_name)
                     self.info_thread_terse(name2id)
                     return
             except ValueError:
                 if thread_name not in list(self.name2id.keys()):
                     self.errmsg("Don't know about thread %s" % thread_name)
                     self.info_thread_terse(name2id)
                     return
@@ -145,62 +148,67 @@
 
         # Show info about *all* threads
         thread_key_list = list(self.name2id.keys())
         thread_key_list.sort()
         for thread_name in thread_key_list:
             thread_id = self.name2id[thread_name]
             frame = sys._current_frames()[thread_id]
-            s = ''
+            s = ""
             # Print location where thread was created and line number
             if thread_id in threading._active:
                 thread = threading._active[thread_id]
                 thread_name = thread.getName()
                 if thread_name == self.proc.frame_thread_name:
-                    prefix = '-> '
-                    if not self.settings['dbg_trepan']:
+                    prefix = "-> "
+                    if not self.settings["dbg_trepan"]:
                         frame = Mthread.find_debugged_frame(frame)
                         pass
                     pass
                 elif thread_name == self.proc.thread_name:
-                    prefix = '=> '
+                    prefix = "=> "
                 else:
-                    prefix='   '
+                    prefix = "   "
                     pass
                 s += "%s%s" % (prefix, str(thread))
                 if all_verbose:
                     s += ": %d" % thread_id
                     pass
             else:
                 s += "    thread id: %d" % thread_id
                 pass
             s += "\n    "
-            s += Mstack.format_stack_entry(self, (frame, frame.f_lineno),
-                                           color=self.settings['highlight'])
-            self.section('-' * 40)
+            s += Mstack.format_stack_entry(
+                self, (frame, frame.f_lineno), color=self.settings["highlight"]
+            )
+            self.section("-" * 40)
             self.msg(s)
             frame = frame.f_back
             if all_verbose and frame:
                 self.stack_trace(frame)
                 pass
         return
+
     pass
 
-if __name__ == '__main__':
-    from trepan.processor.command import mock, info as Minfo
+
+if __name__ == "__main__":
+    from trepan.processor.command import info as Minfo, mock
+
     d, cp = mock.dbg_setup()
     i = Minfo.InfoCommand(cp)
     sub = InfoThread(i)
     import inspect
+
     cp.curframe = inspect.currentframe()
     sub.run([])
-    print('=' * 30)
-    sub.run(['foo'])
-    print('=' * 30)
-    sub.run(['MainThread'])
-    print('=' * 30)
-    sub.run(['terse'])
-    print('=' * 30)
-    sub.run(['verbose'])
-    print('=' * 30)
-    sub.run(['MainThread', 'verbose'])
+    print("=" * 30)
+    sub.run(["foo"])
+    print("=" * 30)
+    sub.run(["MainThread"])
+    print("=" * 30)
+    sub.run(["terse"])
+    print("=" * 30)
+    sub.run(["verbose"])
+    print("=" * 30)
+    sub.run(["MainThread", "verbose"])
     # Try with threading.
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/ipython.py` & `trepan3k-1.2.9/trepan/processor/command/ipython.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 # -*- coding: utf-8 -*-
-#  Copyright (C) 2009-2010, 2013, 2015, 2017, 2020 Rocky Bernstein
+#
+#  Copyright (C) 2009-2010, 2013, 2015, 2017, 2020, 2023 Rocky
+#  Bernstein
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import code, sys
+import code
+import sys
+
+from traitlets.config.loader import Config
 
 # Our local modules
 from trepan.processor.command.base_cmd import DebuggerCommand
 
-from traitlets.config.loader import Config
-
 
 class IPythonCommand(DebuggerCommand):
     """**ipython** [**-d**]
 
-Run IPython as a command subshell.
+    Run IPython as a command subshell.
 
-If *-d* is passed, you can access debugger state via local variable *debugger*.
+    If *-d* is passed, you can access debugger state via local variable *debugger*.
 
-To issue a debugger command use function *dbgr()*. For example:
+    To issue a debugger command use function *dbgr()*. For example:
 
-  dbgr('info program')
+      dbgr('info program')
 
-See also:
----------
+    See also:
+    ---------
 
-`python`, `bpython`
-"""
+    `python`, `bpython`"""
 
     short_help = "Run IPython as a command subshell"
 
     DebuggerCommand.setup(locals(), category="support", max_args=1)
 
     def dbgr(self, string):
         """Invoke a debugger command from inside a IPython shell called
@@ -115,15 +117,15 @@
             module=my_globals,
             exit_msg="IPython exiting to trepan3k...",
         )()
 
         # restore completion and our history if we can do so.
         if hasattr(self.proc.intf[-1], "complete"):
             try:
-                from readline import set_completer, parse_and_bind
+                from readline import parse_and_bind, set_completer
 
                 parse_and_bind("tab: complete")
                 set_completer(self.proc.intf[-1].complete)
             except ImportError:
                 pass
             pass
 
@@ -153,19 +155,14 @@
 
     """
     console = code.InteractiveConsole(my_locals, filename="<trepan>")
     console.runcode = lambda code_obj: runcode(console, code_obj)
     setattr(console, "globals", my_globals)
     if readfunc is not None:
         console.raw_input = readfunc
-    else:
-        try:
-            import readline
-        except ImportError:
-            pass
     console.interact(banner)
     pass
 
 
 # Also monkey-patched from code.py
 # FIXME: get changes into Python.
 def runcode(obj, code_obj):
@@ -180,15 +177,15 @@
     caller should be prepared to deal with it.
 
     """
     try:
         exec(code_obj, obj.locals, obj.globals)
     except SystemExit:
         raise
-    except:
+    except Exception:
         obj.showtraceback()
     else:
         if code.softspace(sys.stdout, 0):
             print()
             pass
         pass
     return
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/jump.py` & `trepan3k-1.2.9/trepan/processor/command/jump.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,88 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2013, 2015, 2020 Rocky Bernstein
+#
+#  Copyright (C) 2009, 2013, 2015, 2020, 2023 Rocky Bernstein
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import inspect, os, sys
+import inspect
+import os
+
+from trepan.processor import cmdproc as Mcmdproc
 
 # Our local modules
 from trepan.processor.command.base_cmd import DebuggerCommand
-from trepan.processor import cmdproc as Mcmdproc
 
 
 class JumpCommand(DebuggerCommand):
     """**jump** *lineno*
 
-Set the next line that will be executed. The line must be within the
-stopped or bottom-most execution frame."""
+    Set the next line that will be executed. The line must be within the
+    stopped or bottom-most execution frame."""
 
-    aliases       = ('j',)
-    category      = 'running'
-    execution_set = ['Running']
-    min_args      = 1
-    max_args      = 1
-    name          = os.path.basename(__file__).split('.')[0]
-    need_stack    = False
-    short_help    = 'Set the next line to be executed'
+    aliases = ("j",)
+    category = "running"
+    execution_set = ["Running"]
+    min_args = 1
+    max_args = 1
+    name = os.path.basename(__file__).split(".")[0]
+    need_stack = False
+    short_help = "Set the next line to be executed"
 
     def run(self, args):
-        if not self.core.is_running(): return False
+        if not self.core.is_running():
+            return False
 
         if self.proc.curindex + 1 != len(self.proc.stack):
             self.errmsg("You can only jump within the bottom frame")
             return False
 
         if self.proc.curframe.f_trace is None:
             self.errmsg("Sigh - operation can't be done here.")
             return False
 
-        lineno = self.proc.get_an_int(args[1],
-                                      ("jump: a line number is required, " +
-                                       "got %s.") % args[1])
-        if lineno is None: return False
+        lineno = self.proc.get_an_int(
+            args[1], ("jump: a line number is required, " + "got %s.") % args[1]
+        )
+        if lineno is None:
+            return False
         try:
             # Set to change position, update our copy of the stack,
             # and display the new position
             print(self.proc.curframe.f_trace)
             self.proc.curframe.f_lineno = lineno
-            self.proc.stack[self.proc.curindex] = \
-                self.proc.stack[self.proc.curindex][0], lineno
+            self.proc.stack[self.proc.curindex] = (
+                self.proc.stack[self.proc.curindex][0],
+                lineno,
+            )
             Mcmdproc.print_location(self.proc)
         except ValueError as e:
-            self.errmsg('jump failed: %s' % e)
+            self.errmsg("jump failed: %s" % e)
         return False
+
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command import mock
+
     d, cp = mock.dbg_setup()
     command = JumpCommand(cp)
-    print('jump when not running: ', command.run(['jump', '1']))
-    command.core.execution_status = 'Running'
+    print("jump when not running: ", command.run(["jump", "1"]))
+    command.core.execution_status = "Running"
     cp.curframe = inspect.currentframe()
     cp.curindex = 0
     cp.stack = Mcmdproc.get_stack(cp.curframe, None, None)
-    command.run(['jump', '1'])
-    cp.curindex = len(cp.stack)-1
-    command.run(['jump', '1'])
+    command.run(["jump", "1"])
+    cp.curindex = len(cp.stack) - 1
+    command.run(["jump", "1"])
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/kill.py` & `trepan3k-1.2.9/trepan/processor/command/kill.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,50 +92,47 @@
                 if interval <= 0:
                     break
 
 
 class KillCommand(DebuggerCommand):
     """**kill** [ *signal-number* ] [unconditional]
 
-Send this process a POSIX signal ('9' for 'SIGKILL' or 'kill -SIGKILL')
+    Send this process a POSIX signal ('9' for 'SIGKILL' or 'kill -SIGKILL')
 
-9 is a non-maskable interrupt that terminates the program. If program
-is threaded it may be expedient to use this command to terminate the program.
+    9 is a non-maskable interrupt that terminates the program. If program
+    is threaded it may be expedient to use this command to terminate the program.
 
-However other signals, such as those that allow for the debugged to
-handle them can be sent.
+    However other signals, such as those that allow for the debugged to
+    handle them can be sent.
 
-Giving a negative number is the same as using its
-positive value.
+    Giving a negative number is the same as using its
+    positive value.
 
-Examples:
---------
+    Examples:
+    --------
 
-    kill                # non-interuptable, nonmaskable kill
-    kill 9              # same as above
-    kill -9             # same as above
-    kill!               # same as above, but no confirmation
-    kill unconditional  # same as above
-    kill 15             # nicer, maskable TERM signal
-    kill! 15            # same as above, but no confirmation
+        kill                # non-interuptable, nonmaskable kill
+        kill 9              # same as above
+        kill -9             # same as above
+        kill!               # same as above, but no confirmation
+        kill unconditional  # same as above
+        kill 15             # nicer, maskable TERM signal
+        kill! 15            # same as above, but no confirmation
 
-See also:
----------
+    See also:
+    ---------
 
-`quit` for less a forceful termination command; `exit` for another way to force termination.
+    `quit` for less a forceful termination command; `exit` for another way to force termination.
 
-`run` and `restart` are ways to restart the debugged program.
-"""
+    `run` and `restart` are ways to restart the debugged program."""
 
     aliases = ("kill!",)
     short_help = 'Send this process a POSIX signal ("9" for "kill -9")'
 
-    DebuggerCommand.setup(
-        locals(), category="running", max_args=1
-    )
+    DebuggerCommand.setup(locals(), category="running", max_args=1)
 
     def complete(self, prefix):
         names = [sig for sig in signal.__dict__.keys() if sig.startswith("SIG")]
         nums = [str(eval("signal." + name)) for name in names]
         lnames = [sig.lower() for sig in names]
         completions = lnames + nums + ["unconditional"]
         return Mcomplete.complete_token(completions, prefix.lower())
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/list.py` & `trepan3k-1.2.9/trepan/processor/command/list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,76 +1,80 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2012-2017, 2020-2021 Rocky Bernstein
+#  Copyright (C) 2009, 2012-2017, 2020-2021, 2023 Rocky Bernstein
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import inspect, linecache, pyficache, sys
+import inspect
+import linecache
 import os.path as osp
+import sys
+
+import pyficache
 
 # Our local modules
 from pygments.console import colorize
 
+from trepan.lib.deparse import deparse_cache
+from trepan.processor.cmdlist import parse_list_cmd
+
 # Our local modules
 from trepan.processor.command.base_cmd import DebuggerCommand
-from trepan.processor.cmdlist import parse_list_cmd
-from trepan.lib.deparse import deparse_cache
 
 
 class ListCommand(DebuggerCommand):
     """**list** [ *range* ]
 
-**list**  **+** | **-** | **.**
+    **list**  **+** | **-** | **.**
 
-List source code. See `help syntax range` for what can go in a list range.
+    List source code. See `help syntax range` for what can go in a list range.
 
-Without arguments, print lines starting from where the last list left off
-since the last entry to the debugger. We start off at the location indicated
-by the current stack.
-
-in addition you can also use:
-
-  - a '.' for the location of the current frame
-  - a '-' for the lines before the last list
-  - a '+' for the lines after the last list
-
-Examples:
---------
-
-    list 5               # List starting from line 5 of current file
-    list 5 ,             # Same as above.
-    list , 5             # list listsize lines before and up to 5
-    list foo.py:5        # List starting from line 5 of file foo.py
-    list foo()           # List starting from function foo
-    list os.path:5       # List starting from line 5 of module os.path
-    list os.path:5, 6    # list lines 5 and 6 of os.path
-    list os.path:5, +1   # Same as above. +1 is an offset
-    list os.path:5, 1    # Same as above, since 1 < 5.
-    list os.path:5, +6   # list lines 5-11
-    list os.path.join()  # List lines centered around the os.join.path function.
-    list .               # List lines centered from where we currently are stopped
-    list -               # List lines previous to those just shown
-    list                 # List continuing from where we last left off
-
-See also:
----------
-
-`set listize` or `show listsize` to see or set the value; `help syntax location`
-for the specification of a location and `help syntax range` for the specification
-of a range.
-"""
+    Without arguments, print lines starting from where the last list left off
+    since the last entry to the debugger. We start off at the location indicated
+    by the current stack.
+
+    in addition you can also use:
+
+      - a '.' for the location of the current frame
+      - a '-' for the lines before the last list
+      - a '+' for the lines after the last list
+
+    Examples:
+    --------
+
+        list 5               # List starting from line 5 of current file
+        list 5 ,             # Same as above.
+        list , 5             # list listsize lines before and up to 5
+        list foo.py:5        # List starting from line 5 of file foo.py
+        list foo()           # List starting from function foo
+        list os.path:5       # List starting from line 5 of module os.path
+        list os.path:5, 6    # list lines 5 and 6 of os.path
+        list os.path:5, +1   # Same as above. +1 is an offset
+        list os.path:5, 1    # Same as above, since 1 < 5.
+        list os.path:5, +6   # list lines 5-11
+        list os.path.join()  # List lines centered around the os.join.path function.
+        list .               # List lines centered from where we currently are stopped
+        list -               # List lines previous to those just shown
+        list                 # List continuing from where we last left off
+
+    See also:
+    ---------
+
+    `set listize` or `show listsize` to see or set the value; `help syntax location`
+    for the specification of a location and `help syntax range` for the specification
+    of a range."""
 
     aliases = ("l",)
     short_help = "List source code"
 
     DebuggerCommand.setup(locals(), category="files", max_args=3)
 
     def run(self, args):
@@ -131,16 +135,24 @@
                     self.msg("[EOF]")
                     break
                 else:
                     line = line.rstrip("\n")
                     s = proc._saferepr(lineno).rjust(3)
                     if len(s) < 5:
                         s += " "
-                    if (canonic_filename, lineno,) in list(bplist.keys()):
-                        bp = bplist[(canonic_filename, lineno,)][0]
+                    if (
+                        canonic_filename,
+                        lineno,
+                    ) in list(bplist.keys()):
+                        bp = bplist[
+                            (
+                                canonic_filename,
+                                lineno,
+                            )
+                        ][0]
                         a_pad = "%02d" % bp.number
                         s += bp.icon_char()
                     else:
                         s += " "
                         a_pad = "  "
                         pass
                     if curframe and lineno == inspect.getlineno(curframe):
@@ -157,23 +169,22 @@
             pass
         except KeyboardInterrupt:
             pass
         return False
 
 
 if __name__ == "__main__":
-
     # FIXME: make sure the below is in a unit test
     def doit(cmd, args):
         proc = cmd.proc
         proc.current_command = " ".join(args)
         cmd.run(args)
 
-    from trepan.processor.command import mock as Mmock
     from trepan.processor.cmdproc import CommandProcessor
+    from trepan.processor.command import mock as Mmock
 
     d = Mmock.MockDebugger()
     cmdproc = CommandProcessor(d.core)
     cmdproc.frame = sys._getframe()
     cmdproc.setup()
     lcmd = ListCommand(cmdproc)
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/macro.py` & `trepan3k-1.2.9/trepan/processor/command/macro.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,68 +19,68 @@
 # Our local modules
 from trepan.processor.command.base_cmd import DebuggerCommand
 
 
 class MacroCommand(DebuggerCommand):
     """**macro** *macro-name* *lambda-object*
 
-Define *macro-name* as a debugger macro. Debugger macros get a list of
-arguments which you supply without parenthesis or commas. See below
-for an example.
+    Define *macro-name* as a debugger macro. Debugger macros get a list of
+    arguments which you supply without parenthesis or commas. See below
+    for an example.
 
-The macro (really a Python lambda) should return either a String or an
-List of Strings. The string in both cases is a debugger command.  Each
-string gets tokenized by a simple split() .  Note that macro
-processing is done right after splitting on `;;`. As a result, if the
-macro returns a string containing `;;` this will not be interpreted as
-separating debugger commands.
+    The macro (really a Python lambda) should return either a String or an
+    List of Strings. The string in both cases is a debugger command.  Each
+    string gets tokenized by a simple split() .  Note that macro
+    processing is done right after splitting on `;;`. As a result, if the
+    macro returns a string containing `;;` this will not be interpreted as
+    separating debugger commands.
 
-If a list of strings is returned, then the first string is
-shifted from the list and executed. The remaining strings are pushed
-onto the command queue. In contrast to the first string, subsequent
-strings can contain other macros. `;;` in those strings will be
-split into separate commands.
+    If a list of strings is returned, then the first string is
+    shifted from the list and executed. The remaining strings are pushed
+    onto the command queue. In contrast to the first string, subsequent
+    strings can contain other macros. `;;` in those strings will be
+    split into separate commands.
 
-Here is an trivial example. The below creates a macro called `l=` which is
-the same thing as `list`:
+    Here is an trivial example. The below creates a macro called `l=` which is
+    the same thing as `list`:
 
-    macro l= lambda: 'list .'
+        macro l= lambda: 'list .'
 
-A simple text to text substitution of one command was all that was
-needed here. But usually you will want to run several commands. So those
-have to be wrapped up into a list.
+    A simple text to text substitution of one command was all that was
+    needed here. But usually you will want to run several commands. So those
+    have to be wrapped up into a list.
 
-The below creates a macro called `fin+` which issues two commands
-`finish` followed by `step`:
+    The below creates a macro called `fin+` which issues two commands
+    `finish` followed by `step`:
 
-    macro fin+ lambda: ['finish','step']
+        macro fin+ lambda: ['finish','step']
 
-If you wanted to parameterize the argument of the `finish` command
-you could do that this way:
+    If you wanted to parameterize the argument of the `finish` command
+    you could do that this way:
 
-    macro fin+ lambda levels: ['finish %s' % levels ,'step']
+        macro fin+ lambda levels: ['finish %s' % levels ,'step']
 
-Invoking with:
+    Invoking with:
 
-     fin+ 3
+         fin+ 3
 
-would expand to: `['finish 3', 'step']`
+    would expand to: `['finish 3', 'step']`
 
-If you were to add another parameter for `step`, the note that the
-invocation might be:
+    If you were to add another parameter for `step`, the note that the
+    invocation might be:
 
-     fin+ 3 2
+         fin+ 3 2
 
-rather than `fin+(3,2)` or `fin+ 3, 2`.
+    rather than `fin+(3,2)` or `fin+ 3, 2`.
 
-See also:
----------
+    See also:
+    ---------
 
- `alias` and `info macro`.
-  """
+     `alias` and `info macro`.
+    """
 
     short_help = "Define a macro"
 
     DebuggerCommand.setup(locals(), category="support", min_args=2)
 
     def run(self, args):
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/mock.py` & `trepan3k-1.2.9/trepan/processor/command/mock.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009-2010, 2013-2015, 2020 Rocky Bernstein
+#   Copyright (C) 2009-2010, 2013-2015, 2020, 2023 Rocky Bernstein
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -12,30 +12,30 @@
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """ Not a command. A stub class used by a command in its 'main' for
 demonstrating how the command works."""
 
-import trepan.lib
-import trepan.inout
-import trepan.interfaces
-import trepan.processor.command
 
-import os, sys
+import sys
+
+# External Egg packages
+import tracefilter
+
 from trepan.lib import breakpoint, default
 
 
 class MockIO(object):
     def readline(self, prompt="", add_to_history=False):
         print(prompt)
         return "quit"
 
     def output(self):
-        print
+        print()
 
     pass
 
 
 class MockUserInterface(object):
     def __init__(self):
         self.io = MockIO()
@@ -85,18 +85,14 @@
     def undefined_cmd(self, cmd):
         self.intf[-1].errmsg('Undefined mock command: "%s' % cmd)
         return
 
     pass
 
 
-# External Egg packages
-import tracefilter
-
-
 class MockDebuggerCore(object):
     def __init__(self, debugger):
         self.debugger = debugger
         self.execution_status = "Pre-execution"
         self.filename_cache = {}
         self.ignore_filter = tracefilter.TraceFilter([])
         self.bpmgr = breakpoint.BreakpointManager()
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/next.py` & `trepan3k-1.2.9/trepan/processor/command/next.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,40 +18,37 @@
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.processor.cmdfns import want_different_line
 
 
 class NextCommand(DebuggerCommand):
     """**next**[**+**|**-**] [*count*]
 
-Execute the current simple statement stopping at the next event but
-ignoring steps into function calls at this level,
+    Execute the current simple statement stopping at the next event but
+    ignoring steps into function calls at this level,
 
-With an integer argument, perform `next` that many times. However if
-an exception occurs at this level, or we *return*, *yield* or the
-thread changes, we stop regardless of count.
-
-A suffix of `+` on the command or an alias to the command forces to
-move to another line, while a suffix of `-` does the opposite and
-disables the requiring a move to a new line. If no suffix is given,
-the debugger setting 'different-line' determines this behavior.
-
-See also:
----------
-
-`step`, `skip`, `jump` (there's no `hop` yet), `continue`, and
-`finish` for other ways to progress execution.
-"""
+    With an integer argument, perform `next` that many times. However if
+    an exception occurs at this level, or we *return*, *yield* or the
+    thread changes, we stop regardless of count.
+
+    A suffix of `+` on the command or an alias to the command forces to
+    move to another line, while a suffix of `-` does the opposite and
+    disables the requiring a move to a new line. If no suffix is given,
+    the debugger setting 'different-line' determines this behavior.
+
+    See also:
+    ---------
+
+    `step`, `skip`, `jump` (there's no `hop` yet), `continue`, and
+    `finish` for other ways to progress execution."""
 
     aliases = ("next+", "next-", "n", "n-", "n+")
     execution_set = ["Running"]
     short_help = "Step over"
 
-    DebuggerCommand.setup(
-        locals(), category="running", need_stack=True, max_args=1
-    )
+    DebuggerCommand.setup(locals(), category="running", need_stack=True, max_args=1)
 
     def run(self, args):
         if len(args) <= 1:
             step_ignore = 0
         else:
             step_ignore = self.proc.get_int(args[1], default=1, cmdname="next")
             if step_ignore is None:
@@ -77,15 +74,18 @@
     for c in (["n", "5"], ["next", "1+2"], ["n", "foo"]):
         d.core.step_ignore = 0
         cmd.continue_running = False
         result = cmd.run(c)
         print("Run result: %s" % result)
         print(
             "step_ignore %d, continue_running: %s"
-            % (d.core.step_ignore, cmd.continue_running,)
+            % (
+                d.core.step_ignore,
+                cmd.continue_running,
+            )
         )
         pass
     for c in (["n"], ["next+"], ["n-"]):
         d.core.step_ignore = 0
         cmd.continue_running = False
         result = cmd.run(c)
         print(cmd.core.different_line)
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/p.py` & `trepan3k-1.2.9/trepan/processor/command/p.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,29 +19,28 @@
 from trepan.lib.printing import printf
 from trepan.processor.complete import complete_identifier
 
 
 class PCommand(DebuggerCommand):
     """**print** *expression*
 
-Print the value of the expression. Variables accessible are those of the
-environment of the selected stack frame, plus globals.
+    Print the value of the expression. Variables accessible are those of the
+    environment of the selected stack frame, plus globals.
 
-The expression may be preceded with */fmt* where *fmt* is one of the
-format letters 'c', 'x', 'o', 'f', or 's' for chr, hex, oct,
-float or str respectively.
+    The expression may be preceded with */fmt* where *fmt* is one of the
+    format letters 'c', 'x', 'o', 'f', or 's' for chr, hex, oct,
+    float or str respectively.
 
-If the length output string large, the first part of the value is
-shown and `...` indicates it has been truncated.
+    If the length output string large, the first part of the value is
+    shown and `...` indicates it has been truncated.
 
-See also:
----------
+    See also:
+    ---------
 
- `pp` and `examine` for commands which do more in the way of formatting.
-"""
+     `pp` and `examine` for commands which do more in the way of formatting."""
 
     aliases = ("print", "pr")
     short_help = "Print value of expression EXP"
 
     complete = complete_identifier
 
     DebuggerCommand.setup(locals(), category="data", need_stack=True, min_args=1)
@@ -56,15 +55,15 @@
         arg = " ".join(args[1:])
         try:
             val = self.proc.eval(arg)
             if fmt:
                 val = printf(val, fmt)
                 pass
             self.msg(self.proc._saferepr(val))
-        except:
+        except Exception:
             pass
 
 
 if __name__ == "__main__":
     import inspect
     from trepan.processor.command import mock
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/pp.py` & `trepan3k-1.2.9/trepan/processor/command/pp.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,25 +19,24 @@
 from trepan.lib.pp import pp
 from trepan.processor.complete import complete_identifier
 
 
 class PrettyPrintCommand(DebuggerCommand):
     """**pp** *expression*
 
-Pretty-print the value of the expression.
+    Pretty-print the value of the expression.
 
-Simple arrays are shown columnized horizontally. Other values are printed
-via *pprint.pformat()*.
+    Simple arrays are shown columnized horizontally. Other values are printed
+    via *pprint.pformat()*.
 
-See also:
----------
+    See also:
+    ---------
 
-`pr` and `examine` for commands which do more in the way of
-formatting.
-"""
+    `pr` and `examine` for commands which do more in the way of
+    formatting."""
 
     short_help = "Pretty print value of expression EXP"
 
     complete = complete_identifier
 
     DebuggerCommand.setup(locals(), category="data", min_args=1)
 
@@ -57,13 +56,13 @@
     d, cp = mock.dbg_setup()
     cp.curframe = inspect.currentframe()
     command = PrettyPrintCommand(cp)
     me = list(range(10))
     command.run(["pp", "me"])
     me = list(range(100))
     command.run(["pp", "me"])
-    import sys
+    import sys  # noqa
 
     command.run(["pp", "sys.modules.keys()"])
     me = "fooled you"
     command.run(["pp", "locals()"])
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/python.py` & `trepan3k-1.2.9/trepan/processor/command/python.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 # -*- coding: utf-8 -*-
-#  Copyright (C) 2009-2010, 2013, 2015, 2017, 2020 Rocky Bernstein
+#
+#  Copyright (C) 2009-2010, 2013, 2015, 2017, 2020, 2023 Rocky
+#  Bernstein
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import code, os.path as osp, sys
+import code
+import sys
+
+from trepan.interfaces.server import ServerInterface
 
 # Our local modules
 from trepan.processor.command.base_cmd import DebuggerCommand
-from trepan.interfaces.server import ServerInterface
 
 
 class PythonCommand(DebuggerCommand):
     """**python** [**-d**]
 
-Run Python as a command subshell. The *sys.ps1* prompt will be set to
-`trepan3 >>> `.
+    Run Python as a command subshell. The *sys.ps1* prompt will be set to
+    `trepan3 >>> `.
 
-If *-d* is passed, you can access debugger state via local variable *debugger*.
+    If *-d* is passed, you can access debugger state via local variable *debugger*.
 
-To issue a debugger command use function *dbgr()*. For example:
+    To issue a debugger command use function *dbgr()*. For example:
 
-  dbgr('info program')
+      dbgr('info program')
 
-See also:
----------
+    See also:
+    ---------
 
-`ipython`, `bpython`
-"""
+    `ipython`, `bpython`"""
 
     aliases = ("py", "shell")
     short_help = "Run Python as a command subshell"
 
     DebuggerCommand.setup(locals(), category="data", max_args=1)
 
     def dbgr(self, string):
@@ -115,15 +118,15 @@
                 pass
         finally:
             sys.excepthook = old_sys_excepthook
 
         # restore completion and our history if we can do so.
         if hasattr(proc.intf[-1], "complete"):
             try:
-                from readline import set_completer, parse_and_bind
+                from readline import parse_and_bind, set_completer
 
                 parse_and_bind("tab: complete")
                 set_completer(proc.intf[-1].complete)
             except ImportError:
                 pass
             pass
 
@@ -157,19 +160,14 @@
         runcode(console, code_obj)
 
     console = code.InteractiveConsole(my_locals, filename="<trepan>")
     console.runcode = console_runcode
     setattr(console, "globals", my_globals)
     if readfunc is not None:
         console.raw_input = readfunc
-    else:
-        try:
-            import readline
-        except ImportError:
-            pass
     console.interact(banner)
     pass
 
 
 # Also monkey-patched from code.py
 # FIXME: get changes into Python.
 def runcode(obj, code_obj):
@@ -184,15 +182,15 @@
     caller should be prepared to deal with it.
 
     """
     try:
         exec(code_obj, obj.locals, obj.globals)
     except SystemExit:
         raise
-    except:
+    except Exception:
         info = sys.exc_info()
         print("%s; %s" % (info[0], info[1]))
     else:
         pass
     return
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/quit.py` & `trepan3k-1.2.9/trepan/processor/command/quit.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,56 +46,53 @@
         ctypes.pythonapi.PyThreadState_SetAsyncExc(target_tid, 0)
         raise SystemError("PyThreadState_SetAsyncExc failed")
 
 
 class QuitCommand(DebuggerCommand):
     """**quit** [**unconditionally**]
 
-Gently terminate the debugged program.
+    Gently terminate the debugged program.
 
-The program being debugged is aborted via a *DebuggerQuit*
-exception.
+    The program being debugged is aborted via a *DebuggerQuit*
+    exception.
 
-When the debugger from the outside (e.g. via a `trepan` command), the
-debugged program is contained inside a try block which handles the
-*DebuggerQuit* exception.  However if you called the debugger was
-started in the middle of a program, there might not be such an
-exception handler; the debugged program still terminates but generally
-with a traceback showing that exception.
+    When the debugger from the outside (e.g. via a `trepan` command), the
+    debugged program is contained inside a try block which handles the
+    *DebuggerQuit* exception.  However if you called the debugger was
+    started in the middle of a program, there might not be such an
+    exception handler; the debugged program still terminates but generally
+    with a traceback showing that exception.
 
-If the debugged program is threaded, we raise an exception in each of
-the threads ending with our own. However this might not quit the
-program.
+    If the debugged program is threaded, we raise an exception in each of
+    the threads ending with our own. However this might not quit the
+    program.
 
-See also:
----------
+    See also:
+    ---------
 
-See `exit` or `kill` for more forceful termination commands.
+    See `exit` or `kill` for more forceful termination commands.
 
-`run` and `restart` are other ways to restart the debugged program.
-"""
+    `run` and `restart` are other ways to restart the debugged program."""
 
     aliases = ("q", "quit!")
     category = "support"
     max_args = 0
     short_help = "Terminate the program - gently"
 
-    DebuggerCommand.setup(
-        locals(), category="support", max_args=0
-    )
+    DebuggerCommand.setup(locals(), category="support", max_args=0)
 
     def nothread_quit(self, arg):
-        """ quit command when there's just one thread. """
+        """quit command when there's just one thread."""
 
         self.debugger.core.stop()
         self.debugger.core.execution_status = "Quit command"
         raise DebuggerQuit
 
     def threaded_quit(self, arg):
-        """ quit command when several threads are involved. """
+        """quit command when several threads are involved."""
         threading_list = threading.enumerate()
         mythread = threading.currentThread()
         for t in threading_list:
             if t != mythread:
                 ctype_async_raise(t, DebuggerQuit)
                 pass
             pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/restart.py` & `trepan3k-1.2.9/trepan/processor/command/restart.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 # -*- coding: utf-8 -*-
-#  Copyright (C) 2009, 2013, 2015, 2020 Rocky Bernstein
+#  Copyright (C) 2009, 2013, 2015, 2020, 2023 Rocky Bernstein
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
-import atexit, os
+import atexit
+import os
+
+from trepan.misc import wrapped_lines
 
 # Our local modules
 from trepan.processor.command.base_cmd import DebuggerCommand
-from trepan.misc import wrapped_lines
 
 
 class RestartCommand(DebuggerCommand):
     """**restart**
 
-Restart debugger and program via an *exec()* call. All state is lost,
-and new copy of the debugger is used.
+    Restart debugger and program via an *exec()* call. All state is lost,
+    and new copy of the debugger is used.
 
-See also:
----------
+    See also:
+    ---------
 
-`run` for another way to restart the debugged program.
+    `run` for another way to restart the debugged program.
 
-See `quit`, `exit` or `kill` for termination commands."""
+    See `quit`, `exit` or `kill` for termination commands."""
 
     short_help = "(Hard) restart of program via execv()"
 
     DebuggerCommand.setup(locals(), category="support", max_args=0)
 
     def run(self, args):
         sys_argv = self.debugger.restart_argv()
@@ -47,15 +49,15 @@
                         "Re exec'ing:", repr(sys_argv), self.settings["width"]
                     )
                 )
                 # Run atexit finalize routines. This seems to be Kosher:
                 # http://mail.python.org/pipermail/python-dev/2009-February/085791.html # NOQA
                 try:
                     atexit._run_exitfuncs()
-                except:
+                except Exception:
                     pass
                 os.execvp(sys_argv[0], sys_argv)
                 pass
             pass
         else:
             self.errmsg("No executable file and command options recorded.")
             pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/run.py` & `trepan3k-1.2.9/trepan/processor/command/run.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,24 +18,23 @@
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.exception import DebuggerRestart
 
 
 class RunCommand(DebuggerCommand):
     """**run**
 
-Soft restart debugger and program via a *DebuggerRestart*
-exception.
+    Soft restart debugger and program via a *DebuggerRestart*
+    exception.
 
-See also:
----------
+    See also:
+    ---------
 
-`restart` for another way to restart the debugged program.
+    `restart` for another way to restart the debugged program.
 
-See `quit`, `exit` or `kill` for termination commands.
-"""
+    See `quit`, `exit` or `kill` for termination commands."""
 
     aliases = ("R",)
     short_help = "(Soft) restart program via a DebuggerRestart exception"
 
     DebuggerCommand.setup(locals(), category="support", max_args=0)
 
     def run(self, args):
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set.py` & `trepan3k-1.2.9/trepan/processor/command/set.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 
 from trepan.processor.command.base_submgr import SubcommandMgr
 
 
 class SetCommand(SubcommandMgr):
     """**set** *set subcommand*
 
-Modifies parts of the debugger environment.
+    Modifies parts of the debugger environment.
 
-You can give unique prefix of the name of a subcommand to get
-information about just that subcommand.
+    You can give unique prefix of the name of a subcommand to get
+    information about just that subcommand.
 
-Type `set` for a list of *set* subcommands and what they do.
-Type `help set *` for just the list of *set* subcommands.
-"""
+    Type `set` for a list of *set* subcommands and what they do.
+    Type `help set *` for just the list of *set* subcommands."""
 
     short_help = "Modify parts of the debugger environment"
 
     SubcommandMgr.setup(locals(), category="data")
 
+
 if __name__ == "__main__":
     from trepan.processor.command import mock
 
     d, cp = mock.dbg_setup()
     command = SetCommand(cp, "set")
     command.run(["set"])
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/__demo_helper__.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/__demo_helper__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-import os, sys
+import os
+import sys
 
 # FIXME: DRY with other demo_helper's
 
+
 def get_name():
     """Get the name caller's caller.
     NB: f_code.co_filenames and thus this code kind of broken for
     zip'ed eggs circa Jan 2009
     """
     caller = sys._getframe(2)
     filename = caller.f_code.co_filename
     filename = os.path.normcase(os.path.basename(filename))
     return os.path.splitext(filename)[0]
 
+
 def demo_setup():
     from trepan.processor.command import mock as Mmock, set as Mset
+
     d, cp = Mmock.dbg_setup()
     mgr = Mset.SetCommand(cp)
     return mgr
 
+
 def demo_run(subcmd, *args):
     mgr = demo_setup()
     sub = subcmd(mgr)
     sub.name = get_name()
     sub.run(*args)
     return sub
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/__init__.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2008-2009, 2015, 2018, 2020 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2008-2009, 2015, 2018, 2020, 2023 Rocky Bernstein
+#   <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
-""" Copyright (C) 2008-2009, 2015, 2018, 2020 Rocky Bernstein <rocky@gnu.org> """
+"""Copyright (C) 2008-2009, 2015, 2018, 2020, 2023
+   Rocky Bernstein <rocky@gnu.org>"""
 
 import glob
 import os.path as osp
 
 # FIXME: Is it really helpful to "privatize" variable names below?
 # The below names are not part of the standard pre-defined names like
 # __name__ or __file__ are.
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/asmfmt.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/asmfmt.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/autoeval.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/different.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2013, 2015 Rocky Bernstein
+#   Copyright (C) 2009, 2013, 2015-2016, 2020 Rocky Bernstein
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
@@ -11,56 +11,45 @@
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 # Our local modules
-from trepan.processor.command import base_subcmd as Mbase_subcmd
+from trepan.processor.command.base_subcmd import DebuggerSetBoolSubcommand
 
 
-class SetAutoEval(Mbase_subcmd.DebuggerSetBoolSubcommand):
-    """**set** **autoeval** [**on**|**off**]
+class SetDifferent(DebuggerSetBoolSubcommand):
+    """**set different** [ **on** | **off** ]
 
-Evaluate unrecognized debugger commands.
+    Set different line location between consecutive debugger stops.
 
-Often inside the debugger, one would like to be able to run arbitrary
-Python commands without having to preface Python expressions with `print` or
-`eval`. Setting *autoeval* on will cause unrecognized debugger
-commands to be *eval*'d as a Python expression.
+    By default, the debugger traces all events possible including line,
+    exceptions, call and return events. Just this alone may mean that for
+    any given source line several consecutive stops at a given line may
+    occur. Independent of this, Python allows one to put several commands
+    in a single source line of code. When a programmer does this, it might
+    be because the programmer thinks of the line as one unit.
+
+    One of the challenges of debugging is getting the granualarity of
+    stepping comfortable. Because of the above, stepping all events can
+    often be too fine-grained and annoying. By setting different on you
+    can set a more coarse-level of stepping which often still is small
+    enough that you won't miss anything important.
+    Note that the `step` and `next` debugger commands have `+` and `-`
+    suffixes if you wan to override this setting on a per-command basis.
+
+    See also:
+    ---------
+    `set trace` to change what events you want to filter.
+    `show trace`"""
 
-Note that if this is set, on error the message shown on type a bad
-debugger command changes from:
-
-  Undefined command: "fdafds". Try "help".
-
-to something more Python-eval-specific such as:
-
-  NameError: name 'fdafds' is not defined
-
-One other thing that trips people up is when setting autoeval is that
-there are some short debugger commands that sometimes one wants to use
-as a variable, such as in an assignment statement. For example:
-
-  s = 5
-
-which produces when *autoeval* is on:
-
-  Command 'step' can take at most 1 argument(s); got 2.
-
-because by default, `s` is an alias for the debugger `step`
-command. It is possible to remove that alias if this causes constant
-problem.
-
-Another possibility is to go into a real Python shell via the `python`
-or `ipython` commands.
-"""
-
-    short_help = "Evaluate unrecognized debugger commands."
-    in_list    = True
-    min_abbrev = len('autoe')
+    in_list = True
+    min_abbrev = len("dif")  # Min is "set dif"
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command.set_subcmd import __demo_helper__ as Mhelper
-    Mhelper.demo_run(SetAutoEval)
+
+    Mhelper.demo_run(SetDifferent)
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/autolist.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/autolist.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,21 +19,20 @@
 from trepan.processor.cmdfns import run_set_bool, run_show_bool
 from trepan.lib.stack import frame2file
 
 
 class SetAutoList(DebuggerSetBoolSubcommand):
     """**set autolist** [ **on** | **off** ]
 
-Run the `list` command every time we enter the debugger.
+    Run the `list` command every time we enter the debugger.
 
-See also:
----------
+    See also:
+    ---------
 
-`show autolist`
-"""
+    `show autolist`"""
 
     in_list = True
     min_abbrev = len("autol")
 
     list_cmd = None
 
     def run(self, args):
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/autopc.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/autopc.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,21 +18,20 @@
 from trepan.processor.command.base_subcmd import DebuggerSetBoolSubcommand
 from trepan.processor.cmdfns import run_set_bool, run_show_bool
 
 
 class SetAutoPC(DebuggerSetBoolSubcommand):
     """**set autopc** [ **on** | **off** ]
 
-Run the `info pc` command every time we enter the debugger.
+    Run the `info pc` command every time we enter the debugger.
 
-See also:
----------
+    See also:
+    ---------
 
-`show autopc`
-"""
+    `show autopc`"""
 
     in_list = True
     min_abbrev = len("autop")
 
     infopc_cmd = None
 
     def run(self, args):
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/autopython.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/autopython.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,43 +18,46 @@
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 from trepan.processor import cmdfns as Mcmdfns, cmdproc as Mcmdproc
 
 
 class SetAutoPython(Mbase_subcmd.DebuggerSetBoolSubcommand):
     """**set** **autopython** [ **on** | **off** ]
 
-Go into a Python shell on debugger entry.
+    Go into a Python shell on debugger entry.
 
-See also:
----------
+    See also:
+    ---------
 
-`python`
-"""
-    in_list    = True
-    min_abbrev = len('autopy')  # Need at least "set autopy"
+    `python`"""
+
+    in_list = True
+    min_abbrev = len("autopy")  # Need at least "set autopy"
 
     python_cmd = None
 
     def run(self, args):
         Mcmdfns.run_set_bool(self, args)
-        if self.settings['autopython']:
+        if self.settings["autopython"]:
             if self.python_cmd is None:
-                self.python_cmd = self.proc.commands['python'].run
+                self.python_cmd = self.proc.commands["python"].run
                 pass
             self.proc.add_preloop_hook(self.run_python, -1)
         else:
             self.proc.remove_preloop_hook(self.run_python)
             pass
         Mcmdfns.run_show_bool(self)
         return
 
     def run_python(self, args):
-        leave_loop = self.python_cmd(['python'])
-        if not leave_loop: Mcmdproc.print_location(self.proc)
+        leave_loop = self.python_cmd(["python"])
+        if not leave_loop:
+            Mcmdproc.print_location(self.proc)
         return leave_loop
 
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command.set_subcmd import __demo_helper__ as Mhelper
+
     Mhelper.demo_run(SetAutoPython)
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/basename.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/basename.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,22 +17,24 @@
 # Our local modules
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 
 
 class SetBasename(Mbase_subcmd.DebuggerSetBoolSubcommand):
     """**set basename** [ **on** | **off** ]
 
-Set basename (short filenames) in debugger output.
+    Set basename (short filenames) in debugger output.
 
-Setting this causes the debugger output to give just the basename for
-filenames. This is useful in debugger testing or possibly showing
-examples where you don't want to hide specific filesystem and
-installation information."""
+    Setting this causes the debugger output to give just the basename for
+    filenames. This is useful in debugger testing or possibly showing
+    examples where you don't want to hide specific filesystem and
+    installation information."""
 
-    in_list    = True
-    min_abbrev = len('ba')
+    in_list = True
+    min_abbrev = len("ba")
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command.set_subcmd import __demo_helper__ as Mhelper
+
     Mhelper.demo_run(SetBasename)
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/cmdtrace.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/cmdtrace.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,21 @@
 # Our local modules
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 from trepan.processor import cmdfns as Mcmdfns
 
 
 class SetCmdtrace(Mbase_subcmd.DebuggerSetBoolSubcommand):
     """Set echoing lines read from debugger command files"""
-    in_list    = True
-    min_abbrev = len('cmdt')    # Need at least "set cmdt"
+
+    in_list = True
+    min_abbrev = len("cmdt")  # Need at least "set cmdt"
     pass
 
     def run(self, args):
         Mcmdfns.run_set_bool(self, args)
         dbg = self.debugger
-        if hasattr(dbg.intf[-1], 'verbose'):
+        if hasattr(dbg.intf[-1], "verbose"):
             dbg.intf[-1].verbose = dbg.settings[self.name]
             pass
         return
+
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/confirm.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/confirm.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,28 +17,29 @@
 # Our local modules
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 
 
 class SetConfirm(Mbase_subcmd.DebuggerSetBoolSubcommand):
     """**set confirm** [ **on* | **off** ]
 
-Set confirmation of potentially dangerous operations.
+    Set confirmation of potentially dangerous operations.
 
-Some operations are a bit disruptive like terminating the program.
-To guard against running this accidentally, by default we ask for
-confirmation. Commands can also be exempted from confirmation by suffixing
-them with an exclamation mark (!).
+    Some operations are a bit disruptive like terminating the program.
+    To guard against running this accidentally, by default we ask for
+    confirmation. Commands can also be exempted from confirmation by suffixing
+    them with an exclamation mark (!).
 
-See Also:
----------
+    See Also:
+    ---------
 
-`show confirm`
-"""
+    `show confirm`"""
 
-    in_list    = True
-    min_abbrev = len('co')
+    in_list = True
+    min_abbrev = len("co")
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command.set_subcmd import __demo_helper__ as Mhelper
+
     Mhelper.demo_run(SetConfirm)
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/dbg_trepan.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/dbg_trepan.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,34 +20,35 @@
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 from trepan.processor import cmdfns as Mcmdfns, cmdproc as Mcmdproc
 
 
 class SetCmdDbgTrepan(Mbase_subcmd.DebuggerSetBoolSubcommand):
     """Set the ability to debug the debugger.
 
-Setting this allows visibility and access to some of the debugger's
-internals. Specifically variable "frame" contains the current frame and
-variable "debugger" contains the top-level debugger object.
-"""
+    Setting this allows visibility and access to some of the debugger's
+    internals. Specifically variable "frame" contains the current frame and
+    variable "debugger" contains the top-level debugger object."""
 
-    in_list    = True
-    min_abbrev = len('dbg')    # Need at least "set dbg"
+    in_list = True
+    min_abbrev = len("dbg")  # Need at least "set dbg"
 
     def run(self, args):
         Mcmdfns.run_set_bool(self, args)
         if self.debugger.settings[self.name]:
             # Put a stack frame in the list of frames so we have
             # something to inspect.
             frame = inspect.currentframe()
             # Also give access to the top-level debugger
-            self.proc.stack, self.proc.curindex = \
-                Mcmdproc.get_stack(frame, None, self.proc)
+            self.proc.stack, self.proc.curindex = Mcmdproc.get_stack(
+                frame, None, self.proc
+            )
             self.proc.curframe = self.proc.stack[self.proc.curindex][0]
             # Remove ignored debugger functions.
             self.save_ignore_filter = self.core.ignore_filter
             self.core.ignore_filter = None
         else:
             self.core.ignore_filter = self.save_ignore_filter
             pass
 
         return
+
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/events.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,34 +20,34 @@
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 
 
 class SetEvents(Mbase_subcmd.DebuggerSubcommand):
 
     """**set events** [*event* ...]
 
-Sets the events that the debugger will stop on. Event names are:
-`c_call`, `c_exception`, `c_return`, `call`, `exception`, `line`,
-or `return`.
+    Sets the events that the debugger will stop on. Event names are:
+    `c_call`, `c_exception`, `c_return`, `call`, `exception`, `line`,
+    or `return`.
 
-`all` can be used as an abbreviation for listing all event names.
+    `all` can be used as an abbreviation for listing all event names.
 
-Changing trace event filters works independently of turning on or off
-tracing-event printing.
+    Changing trace event filters works independently of turning on or off
+    tracing-event printing.
 
-Examples:
----------
+    Examples:
+    ---------
 
-  set events line        # Set trace filter for line events only.
-  set events call return # Trace calls and returns only
-  set events all         # Set trace filter to all events.
+      set events line        # Set trace filter for line events only.
+      set events call return # Trace calls and returns only
+      set events all         # Set trace filter to all events.
 
-See also:
----------
+    See also:
+    ---------
 
-`set trace`, `show trace`, and `show events`. `help step` lists event names.
+    `set trace`, `show trace`, and `show events`. `help step` lists event names.
     """
 
     in_list = True
     min_args = 0
     min_abbrev = len("ev")
     short_help = "Set execution-tracing event set"
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/highlight.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/highlight.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,44 +21,44 @@
 from trepan.lib.complete import complete_token
 from trepan.lib.format import color_tf
 
 
 class SetHighlight(DebuggerSubcommand):
     """**set highlight** [ **reset** ] {**plain** | **light** | **dark** | **off**}
 
-Set whether we use terminal highlighting. Permissible values are:
+    Set whether we use terminal highlighting. Permissible values are:
 
-       plain:  no terminal highlighting
-       off:    same as plain
-       light:  terminal background is light (the default)
-       dark:   terminal background is dark
-
-If the first argument is *reset*, we clear any existing color formatting
-and recolor all source code output.
-
-A related setting is *style* which sets the Pygments style for terminal
-that support, 256 colors. But even here, it is useful to set
-the highlight to tell the debugger for bold and emphasized text what
-values to use.
-
-Examples:
---------
-
-    set highlight off   # no highlight
-    set highlight plain # same as above
-    set highlight       # same as above
-    set highlight dark  # terminal has dark background
-    set highlight light # terminal has light background
-    set highlight reset light # clear source-code cache and
-                              # set for light background
-    set highlight reset # clear source-code cache
-
-See also:
----------
-`show highlight` and `set style`"""
+           plain:  no terminal highlighting
+           off:    same as plain
+           light:  terminal background is light (the default)
+           dark:   terminal background is dark
+
+    If the first argument is *reset*, we clear any existing color formatting
+    and recolor all source code output.
+
+    A related setting is *style* which sets the Pygments style for terminal
+    that support, 256 colors. But even here, it is useful to set
+    the highlight to tell the debugger for bold and emphasized text what
+    values to use.
+
+    Examples:
+    --------
+
+        set highlight off   # no highlight
+        set highlight plain # same as above
+        set highlight       # same as above
+        set highlight dark  # terminal has dark background
+        set highlight light # terminal has light background
+        set highlight reset light # clear source-code cache and
+                                  # set for light background
+        set highlight reset # clear source-code cache
+
+    See also:
+    ---------
+    `show highlight` and `set style`"""
 
     in_list = True
     min_abbrev = len("hi")
     short_help = "Set whether we use terminal highlighting"
 
     highlight_choices = ("reset", "plain", "light", "dark", "off")
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/listsize.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/listsize.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 from trepan.processor.command.base_subcmd import DebuggerSubcommand
 from trepan.processor.cmdfns import run_set_int
 
 
 class SetListSize(DebuggerSubcommand):
     """**set listsize** *number-of-lines*
 
-Set the number lines printed in a *list* command by default
+    Set the number lines printed in a *list* command by default
 
-See also:
----------
+    See also:
+    ---------
 
-`show listsize`"""
+    `show listsize`"""
 
     in_list = True
     min_abbrev = len("lis")  # Need at least "set lis"
 
     def run(self, args):
         run_set_int(
             self,
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/maxstring.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/maxstring.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,21 +18,20 @@
 from trepan.processor.command.base_subcmd import DebuggerSubcommand
 from trepan.processor import cmdfns as Mcmdfns
 
 
 class SetMaxString(DebuggerSubcommand):
     """**set maxstring** *number*
 
-Set the number of characters allowed in showing string values
+    Set the number of characters allowed in showing string values
 
-See also:
----------
+    See also:
+    ---------
 
-`show maxstring`
-"""
+    `show maxstring`"""
 
     in_list = True
     max_args = 1
     min_abbrev = len("str")  # Need at least "set max str"
     min_args = 1
     short_help = "Set maximum characters in showing strings"
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/patsub.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/patsub.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,27 +17,27 @@
 # Our local modules
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 
 
 class SetPatSub(Mbase_subcmd.DebuggerSubcommand):
     """**set patsub** *from-re* *replace-string*
 
-Add a substitution pattern rule replacing *patsub* with
-*replace-string* anywhere it is found in source file names.  If a
-substitution rule was previously set for *from-re*, the old rule is
-replaced by the new one.
-
-In the following example, suppose in a docker container /mnt/project is
-the mount-point for /home/rocky/project. You are running the code
-from the docker container, but debugging this from outside of that.
+    Add a substitution pattern rule replacing *patsub* with
+    *replace-string* anywhere it is found in source file names.  If a
+    substitution rule was previously set for *from-re*, the old rule is
+    replaced by the new one.
+
+    In the following example, suppose in a docker container /mnt/project is
+    the mount-point for /home/rocky/project. You are running the code
+    from the docker container, but debugging this from outside of that.
 
-Example:
---------
+    Example:
+    --------
 
-    set patsub ^/mmt/project /home/rocky/project
+        set patsub ^/mmt/project /home/rocky/project
 
     """
 
     in_list = True
     max_args = 2
     min_abbrev = len("pats")
     min_args = 2
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/skip.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/skip.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,31 +18,33 @@
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 
 
 class SetSkip(Mbase_subcmd.DebuggerSetBoolSubcommand):
     """**set skip** [ **on** | **off** ]
 
 
-Set stopping before *def* or *class* (function or class) statements.
+    Set stopping before *def* or *class* (function or class) statements.
 
-Classes may have many methods and stand-alone programs may have many
-functions. Often there isn't much value to stopping before defining a
-new function or class into Python's symbol table. (More to the point,
-it can be an annoyance.) However if you do want this, for example
-perhaps you want to debug methods is over-writing one another, then
-set this off
+    Classes may have many methods and stand-alone programs may have many
+    functions. Often there isn't much value to stopping before defining a
+    new function or class into Python's symbol table. (More to the point,
+    it can be an annoyance.) However if you do want this, for example
+    perhaps you want to debug methods is over-writing one another, then
+    set this off
 
-See also:
----------
+    See also:
+    ---------
 
-`show skip`"""
+    `show skip`"""
 
-    in_list    = True
-    min_abbrev = len('sk')    # Min 'set sk'
+    in_list = True
+    min_abbrev = len("sk")  # Min 'set sk'
     short_help = "Set stopping before def or class statements"
     # FIXME allow individual setting for class and skip.
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command.set_subcmd import __demo_helper__ as Mhelper
+
     sub = Mhelper.demo_run(SetSkip)
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/style.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/style.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,33 +10,32 @@
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 from trepan.lib import complete as Mcomplete
 
 
 class SetStyle(Mbase_subcmd.DebuggerSubcommand):
     """**set style** [*pygments-style*]
 
-Set the pygments style in to use in formatting text for a 256-color terminal.
-Note: if your terminal doesn't support 256 colors, you may be better off
-using `--highlight=plain` or `--highlight=dark` instead. To turn off styles
-use `set style none`.
+    Set the pygments style in to use in formatting text for a 256-color terminal.
+    Note: if your terminal doesn't support 256 colors, you may be better off
+    using `--highlight=plain` or `--highlight=dark` instead. To turn off styles
+    use `set style none`.
 
-To list the available pygments styles inside the debugger, omit the style name.
+    To list the available pygments styles inside the debugger, omit the style name.
 
-Examples:
----------
+    Examples:
+    ---------
 
-    set style            # give a list of the style names
-    set style colorful   # Pygments 'colorful' style
-    set style none       # Turn off style, still use highlight though
+        set style            # give a list of the style names
+        set style colorful   # Pygments 'colorful' style
+        set style none       # Turn off style, still use highlight though
 
-See also:
---------
+    See also:
+    --------
 
-`show style`, `set highlight`
-"""
+    `show style`, `set highlight`"""
 
     def complete(self, prefix):
         return Mcomplete.complete_token(style_names, prefix)
 
     in_list = True
     min_abbrev = len("sty")
     short_help = "Set the pygments style"
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/substitute.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/substitute.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,30 +19,29 @@
 # Our local modules
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 
 
 class SetSubstitute(Mbase_subcmd.DebuggerSubcommand):
     """**set substitute** *from-name* *to-path*
 
-Add a substitution rule replacing *from-name* into *to-path* in source file names.
-If a substitution rule was previously set for *from-name*, the old rule
-is replaced by the new one.
+    Add a substitution rule replacing *from-name* into *to-path* in source file names.
+    If a substitution rule was previously set for *from-name*, the old rule
+    is replaced by the new one.
 
-Spaces in "filenames" like `<frozen importlib._bootstrap>` messes up our normal shell
-tokenization, so we have added a hack to ignore `<frozen .. >`.
+    Spaces in "filenames" like `<frozen importlib._bootstrap>` messes up our normal shell
+    tokenization, so we have added a hack to ignore `<frozen .. >`.
 
-So, for frozen files like `<frozen importlib._bootstrap>`, `use importlib._bootstrap`
+    So, for frozen files like `<frozen importlib._bootstrap>`, `use importlib._bootstrap`
 
-Examples:
----------
+    Examples:
+    ---------
 
-    set substitute importlib._bootstrap /usr/lib/python3.4/importlib/_bootstrap.py
-    set substitute ./gcd.py /tmp/gcd.py
-
-"""
+        set substitute importlib._bootstrap /usr/lib/python3.4/importlib/_bootstrap.py
+        set substitute ./gcd.py /tmp/gcd.py
+    """
 
     in_list = True
     max_args = 2
     min_args = 2
     min_abbrev = len("sub")
 
     short_help = "Set filename substitution"
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/tempdir.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/tempdir.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,30 +7,29 @@
 # Our local modules
 from trepan.processor.command.base_subcmd import DebuggerSubcommand
 
 
 class SetTempdir(DebuggerSubcommand):
     """**set tempdir** *directory*
 
-Set the temporary directory for temporary decompiled python files.
+    Set the temporary directory for temporary decompiled python files.
 
-This is sometimes useful remote debugging where you might set up a
-common shared location available between the debugged process and
-the front end client.
+    This is sometimes useful remote debugging where you might set up a
+    common shared location available between the debugged process and
+    the front end client.
 
-Examples:
----------
+    Examples:
+    ---------
 
-    set tempdir /code/tmp  # /code is a shared directory
+        set tempdir /code/tmp  # /code is a shared directory
 
-See also:
---------
+    See also:
+    --------
 
-`show tempdir`
-"""
+    `show tempdir`"""
 
     in_list = True
     min_abbrev = len("temp")
     min_args = 1
     max_args = 1
     short_help = "Set a directory for storing decompiled Python"
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/trace.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/trace.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,29 +18,30 @@
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 
 
 class SetTrace(Mbase_subcmd.DebuggerSetBoolSubcommand):
 
     """**set trace** [ **on** | **off** ]
 
-Set event tracing.
+    Set event tracing.
 
-See also:
----------
+    See also:
+    ---------
 
-`set events`, and `show trace`.
-"""
+    `set events`, and `show trace`."""
 
-    in_list    = True
-    min_abbrev = len('trace')  # Must use at least "set trace"
+    in_list = True
+    min_abbrev = len("trace")  # Must use at least "set trace"
     short_help = "Set event tracing"
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command.set_subcmd import __demo_helper__ as Mhelper
+
     sub = Mhelper.demo_run(SetTrace)
     d = sub.proc.debugger
-    for args in (['on'], ['off']):
+    for args in (["on"], ["off"]):
         sub.run(args)
-        print(d.settings['trace'])
+        print(d.settings["trace"])
         pass
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/set_subcmd/width.py` & `trepan3k-1.2.9/trepan/processor/command/set_subcmd/width.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 from trepan.processor.command.base_subcmd import DebuggerSubcommand
 from trepan.processor.cmdfns import run_set_int
 
 
 class SetWidth(DebuggerSubcommand):
     """**set width** *number*
 
-Set the number of characters the debugger thinks are in a line.
+    Set the number of characters the debugger thinks are in a line.
 
-See also:
---------
+    See also:
+    --------
 
-`show width`
-"""
+    `show width`"""
 
     in_list = True
     min_abbrev = len("wid")
     short_help = "Set the width of the terminal"
 
     def run(self, args):
         run_set_int(
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/show.py` & `trepan3k-1.2.9/trepan/processor/command/show.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,21 +16,20 @@
 
 from trepan.processor.command.base_submgr import SubcommandMgr
 
 
 class ShowCommand(SubcommandMgr):
     """**show** *subcommand*
 
-Generic command for showing things about the debugger.  You can
-give unique prefix of the name of a subcommand to get information
-about just that subcommand.
-
-Type `show` for a list of *show* subcommands and what they do.
-Type `help show *` for just a list of *show* subcommands.
-"""
+    Generic command for showing things about the debugger.  You can
+    give unique prefix of the name of a subcommand to get information
+    about just that subcommand.
+
+    Type `show` for a list of *show* subcommands and what they do.
+    Type `help show *` for just a list of *show* subcommands."""
 
     short_help = "Show parts of the debugger environment"
     SubcommandMgr.setup(locals(), category="status")
 
 
 if __name__ == "__main__":
     from trepan.processor.command import mock
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/show_subcmd/__demo_helper__.py` & `trepan3k-1.2.9/trepan/processor/command/show_subcmd/__demo_helper__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-import os, sys
+import os
+import sys
 
 # FIXME: DRY with other demo_helper's
 
+
 def get_name():
     """Get the name caller's caller.
     NB: f_code.co_filenames and thus this code kind of broken for
     zip'ed eggs circa Jan 2009
     """
     caller = sys._getframe(2)
     filename = caller.f_code.co_filename
     filename = os.path.normcase(os.path.basename(filename))
     return os.path.splitext(filename)[0]
 
+
 def demo_setup():
     from trepan.processor.command import mock as Mmock, show as Mshow
+
     d, cp = Mmock.dbg_setup()
     mgr = Mshow.ShowCommand(cp)
     return mgr
 
+
 def demo_run(subcmd):
     mgr = demo_setup()
     sub = subcmd(mgr)
     sub.name = get_name()
     sub.run([])
     return sub
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/show_subcmd/__init__.py` & `trepan3k-1.2.9/trepan/processor/command/show_subcmd/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,25 +8,28 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # """ Copyright (C) 2008-2009, 2015, 2018 Rocky Bernstein <rocky@gnu.org> """
 
-import glob, os
+import glob
+import os
 
 # FIXME: Is it really helpful to "privatize" variable names below?
 # The below names are not part of the standard pre-defined names like
 # __name__ or __file__ are.
 
 # Get the name of our directory.
 __command_dir__ = os.path.dirname(__file__)
 
 # A glob pattern that will get all *.py files but not __init__.py
-__py_files__    = glob.glob(os.path.join(__command_dir__, '[a-z]*.py'))
+__py_files__ = glob.glob(os.path.join(__command_dir__, "[a-z]*.py"))
 
 # Take the basename of the filename and drop off '.py'. That minus the
 # file exclude_file the list of modules that show.py will use to import
 exclude_files = []
-__modules__ = [ os.path.basename(filename[0:-3]) for
-                filename in __py_files__
-                if os.path.basename(filename) not in exclude_files]
+__modules__ = [
+    os.path.basename(filename[0:-3])
+    for filename in __py_files__
+    if os.path.basename(filename) not in exclude_files
+]
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/show_subcmd/aliases.py` & `trepan3k-1.2.9/trepan/processor/command/show_subcmd/aliases.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,34 +17,33 @@
 import columnize
 
 # Our local modules
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 
 
 class ShowAliases(Mbase_subcmd.DebuggerShowIntSubcommand):
-    '''**show aliases** [*alias* ...| *]
+    """**show aliases** [*alias* ...| *]
 
-Show command aliases. If parameters are given a list of all aliases and
-the command they run are printed. Alternatively one can list specific
-alias names for the commands those specific aliases are attached to.
-If instead of an alias `*` appears anywhere as an alias then just a list
-of aliases is printed, not what commands they are attached to.
-
-See also:
----------
-`alias`
-'''
+    Show command aliases. If parameters are given a list of all aliases and
+    the command they run are printed. Alternatively one can list specific
+    alias names for the commands those specific aliases are attached to.
+    If instead of an alias `*` appears anywhere as an alias then just a list
+    of aliases is printed, not what commands they are attached to.
+
+    See also:
+    ---------
+    `alias`"""
 
-    min_abbrev = len('al')
+    min_abbrev = len("al")
     short_help = "Show command aliases"
-    run_cmd    = False
+    run_cmd = False
 
     def _alias_header(self):
-        self.section("%-10s : %s" % ('Alias', 'Command'))
-        self.msg("%-10s : %s" % ('-' * 10, '-' * 11))
+        self.section("%-10s : %s" % ("Alias", "Command"))
+        self.msg("%-10s : %s" % ("-" * 10, "-" * 11))
         return
 
     def _alias_line(self, alias):
         self.msg("%-10s : %s" % (alias, self.proc.aliases[alias]))
         return
 
     def run(self, args):
@@ -52,28 +51,30 @@
         aliases.sort()
         if len(args) == 0:
             self._alias_header()
             for alias in aliases:
                 self._alias_line(alias)
                 pass
             return
-        if '*' in args:
+        if "*" in args:
             self.section("Current aliases:")
-            self.msg(columnize.columnize(aliases, lineprefix='    '))
+            self.msg(columnize.columnize(aliases, lineprefix="    "))
         else:
             self._alias_header()
             for alias in args:
                 if alias in aliases:
                     self._alias_line(alias)
                 else:
                     self.errmsg("%s is not an alias" % alias)
                     pass
                 pass
             return
         return
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command.show_subcmd import __demo_helper__ as Mhelper
+
     sub = Mhelper.demo_run(ShowAliases)
-    sub.run(['*'])
-    sub.run(['s+', "n+"])
+    sub.run(["*"])
+    sub.run(["s+", "n+"])
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/show_subcmd/args.py` & `trepan3k-1.2.9/trepan/processor/command/show_subcmd/args.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,22 +16,27 @@
 
 # Our local modules
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 
 
 class ShowArgs(Mbase_subcmd.DebuggerSubcommand):
     """Show argument list to give debugged program when it is started"""
-    min_abbrev = len('arg')
+
+    min_abbrev = len("arg")
     run_in_help = False
-    short_help = 'Show arguments when program is started'
+    short_help = "Show arguments when program is started"
 
     def run(self, args):
-        self.msg("Argument list to give program being debugged " +
-                 "when it is started is:")
-        self.msg('\t%s.' % ' '.join(self.debugger.program_sys_argv[1:]))
+        self.msg(
+            "Argument list to give program being debugged " + "when it is started is:"
+        )
+        self.msg("\t%s." % " ".join(self.debugger.program_sys_argv[1:]))
         return False
+
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command.show_subcmd import __demo_helper__ as Mhelper
+
     Mhelper.demo_run(ShowArgs)
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/show_subcmd/asmfmt.py` & `trepan3k-1.2.9/trepan/processor/command/show_subcmd/asmfmt.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,39 +17,40 @@
 # Our local modules
 from trepan.processor.command.base_subcmd import DebuggerSubcommand
 
 
 class ShowAsmFmt(DebuggerSubcommand):
     """**show asmfmt**
 
-Show the disassembly format style used in the `disassemble` cmmand.
+    Show the disassembly format style used in the `disassemble` command.
 
-See also:
----------
+    See also:
+    ---------
 
-`set asmfmt`"""
+    `set asmfmt`"""
 
     min_abbrev = len("asmf")
     short_help = "Show assembly format style"
     pass
 
-
     def run(self, args):
         if len(args) != 0:
             self.errmsg("Expecting no args")
             return
 
         style = self.debugger.settings[self.name]
         if style:
             self.msg("Assembly format style is %s" % style)
         else:
             self.msg("Assembly format style not set")
         return
 
     pass
+
+
 if __name__ == "__main__":
     from trepan.processor.command.set_subcmd import __demo_helper__ as Mhelper
 
     sub = Mhelper.demo_run(ShowAsmFmt, [])
     d = sub.proc.debugger
     sub.run(["invalid arg"])
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/show_subcmd/autoeval.py` & `trepan3k-1.2.9/trepan/processor/command/show_subcmd/autoeval.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 # Our local modules
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 
 
 class ShowAutoEval(Mbase_subcmd.DebuggerShowBoolSubcommand):
     """**show autoeval**
 
-Show Python evaluation of unrecognized debugger commands.
+    Show Python evaluation of unrecognized debugger commands.
 
-See also:
----------
+    See also:
+    ---------
 
-`set autoeval`
-"""
-    min_abbrev = len('autoe')
+    `set autoeval`"""
+
+    min_abbrev = len("autoe")
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command.show_subcmd import __demo_helper__ as Mhelper
+
     Mhelper.demo_run(ShowAutoEval)
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/show_subcmd/autolist.py` & `trepan3k-1.2.9/trepan/processor/command/show_subcmd/autolist.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 # Our local modules
 from trepan.processor.command.base_subcmd import DebuggerShowBoolSubcommand
 
 
 class ShowAutoList(DebuggerShowBoolSubcommand):
     """**show autolist**
 
-Show debugger `list` command automatically on entry.
+    Show debugger `list` command automatically on entry.
 
-See also:
----------
+    See also:
+    ---------
 
-`set autolist`"""
+    `set autolist`"""
 
     min_abbrev = len("autol")
     short_help = "Show `list` on debugger entry"
     pass
 
 
 if __name__ == "__main__":
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/show_subcmd/autopc.py` & `trepan3k-1.2.9/trepan/processor/command/show_subcmd/autopc.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/trepan/processor/command/show_subcmd/autopython.py` & `trepan3k-1.2.9/trepan/processor/command/show_subcmd/autopython.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 # Our local modules
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 
 
 class ShowAutoPython(Mbase_subcmd.DebuggerShowBoolSubcommand):
-    '''**show autopython**
+    """**show autopython**
 
-Show whether we go into a python shell when automatically when the
-debugger is entered.
+    Show whether we go into a python shell when automatically when the
+    debugger is entered.
+
+    Change with **set autopython**"""
 
-Change with **set autopython**
-'''
     short_help = "Show automatic Python shell entry"
-    min_abbrev = len('autopy')
+    min_abbrev = len("autopy")
     pass
 
-if __name__ == '__main__':
-    from trepan.processor.command.show_subcmd \
-      import __demo_helper__ as Mhelper
+
+if __name__ == "__main__":
+    from trepan.processor.command.show_subcmd import __demo_helper__ as Mhelper
+
     Mhelper.demo_run(ShowAutoPython)
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/show_subcmd/basename.py` & `trepan3k-1.2.9/trepan/processor/command/show_subcmd/basename.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,22 +15,24 @@
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 # Our local modules
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 
 
 class ShowBasename(Mbase_subcmd.DebuggerShowBoolSubcommand):
-    '''**show basename**
+    """**show basename**
 
-Show whether filenames are reported with just the basename or the
-fully qualified filename.
+    Show whether filenames are reported with just the basename or the
+    fully qualified filename.
+
+    Change with **set basename**"""
 
-Change with **set basename**
-'''
     short_help = "Show the basename portion only of filenames"
-    min_abbrev = len('ba')
+    min_abbrev = len("ba")
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.processor.command.show_subcmd import __demo_helper__ as Mhelper
+
     Mhelper.demo_run(ShowBasename)
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/show_subcmd/confirm.py` & `trepan3k-1.2.9/trepan/processor/command/show_subcmd/substitute.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,54 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2013, 2015 Rocky Bernstein
+#   Copyright (C) 2023 Rocky Bernstein
 #
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
+#   This program is free software: you can redistribute it and/or modify
+#   it under the terms of the GNU General Public License as published by
+#   the Free Software Foundation, either version 3 of the License, or
+#   (at your option) any later version.
 #
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
+#   This program is distributed in the hope that it will be useful,
+#   but WITHOUT ANY WARRANTY; without even the implied warranty of
+#   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#   GNU General Public License for more details.
 #
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <http://www.gnu.org/licenses/>.
+#   You should have received a copy of the GNU General Public License
+#   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 # Our local modules
+from pyficache import file2file_remap
+
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 
 
-class ShowConfirm(Mbase_subcmd.DebuggerShowBoolSubcommand):
-    """**show confirm**
+class ShowSubstitute(Mbase_subcmd.DebuggerSubcommand):
+    """**show substitute** [*from-name1* *from_name2* ... ]
+    If no *from-name* is given, then show all substitute commands
+
+    Examples:
+    ---------
+
+        show substitute importlib._bootstrap /usr/lib/python3.10/importlib/_bootstrap.py
+        show substitute
+    """
+
+    in_list = True
+    min_abbrev = len("sub")
+
+    short_help = "Set filename substitution"
+
+    def run(self, args):
+        if len(args) == 0:
+            args = file2file_remap.keys()
+
+        if len(args) == 0:
+            self.msg("No file remappings in effect.")
+        for from_path in args:
+            self.msg(f"{from_path}:\t{file2file_remap.get(from_path, from_path)}")
 
-Show confirmation of potentially dangerous operations
 
-See also:
----------
+if __name__ == "__main__":
+    from trepan.processor.command.set_subcmd import __demo_helper__ as Mhelper
 
-`set confirm`"""
-    min_abbrev = 3    # Need at least "show con"
-    pass
-
-if __name__ == '__main__':
-    from trepan.processor.command.show_subcmd \
-      import __demo_helper__ as Mhelper
-    Mhelper.demo_run(ShowConfirm)
-    pass
+    sub = Mhelper.demo_run(ShowSubstitute, [])
+    d = sub.proc.debugger
+    sub.run(["show"])
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/show_subcmd/highlight.py` & `trepan3k-1.2.9/trepan/processor/command/show_subcmd/highlight.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,31 +19,36 @@
 # Our local modules
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 
 
 class ShowHighlight(Mbase_subcmd.DebuggerSubcommand):
     """**show highlight**
 
-Show whether we use terminal highlighting.
+    Show whether we use terminal highlighting.
 
-See also:
---------
+    See also:
+    --------
 
-`set highlight`"""
-    short_help = 'Show if we use terminal highlight'
+    `set highlight`"""
+
+    short_help = "Show if we use terminal highlight"
 
     def run(self, args):
-        val = self.settings['highlight']
-        if 'plain' == val:
-            mess = 'output set to not use terminal escape sequences'
-        elif 'light' == val:
-            mess = ('output set for terminal with escape sequences '
-                    'for a light background')
-        elif 'dark' == val:
-            mess = ('output set for terminal with escape sequences '
-                    'for a dark background')
+        val = self.settings["highlight"]
+        if "plain" == val:
+            mess = "output set to not use terminal escape sequences"
+        elif "light" == val:
+            mess = (
+                "output set for terminal with escape sequences "
+                "for a light background"
+            )
+        elif "dark" == val:
+            mess = (
+                "output set for terminal with escape sequences " "for a dark background"
+            )
         else:
-            self.errmsg('Internal error: incorrect highlight setting %s' % val)
+            self.errmsg("Internal error: incorrect highlight setting %s" % val)
             return
         self.msg(mess)
         return
+
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/show_subcmd/listsize.py` & `trepan3k-1.2.9/trepan/processor/command/show_subcmd/listsize.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 # Our local modules
 from trepan.processor.command import base_subcmd as Mbase_subcmd
 
 
 class ShowListSize(Mbase_subcmd.DebuggerShowIntSubcommand):
     """**show maxstring***
 
-Show the number lines printed in a 'list' command by default
+    Show the number lines printed in a 'list' command by default
 
-See also:
---------
+    See also:
+    --------
 
-`set listsize`"""
-    min_abbrev = len('lis')
-    short_help = 'Show number of lines in `list`'
+    `set listsize`"""
+
+    min_abbrev = len("lis")
+    short_help = "Show number of lines in `list`"
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/show_subcmd/style.py` & `trepan3k-1.2.9/trepan/processor/command/show_subcmd/style.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,20 @@
 def complete(self, prefix):
     return complete_token(style_names)
 
 
 class ShowStyle(DebuggerSubcommand):
     """**show style* *pygments-style*
 
-Show the pygments style used in formatting 256-color terminal text.
+    Show the pygments style used in formatting 256-color terminal text.
 
-See also:
----------
+    See also:
+    ---------
 
-`set style`, `show highlight`
-"""
+    `set style`, `show highlight`"""
 
     in_list = True
     min_abbrev = len("sty")
     short_help = "Set the pygments style"
 
     def run(self, args):
         if len(args) != 0:
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/show_subcmd/tempdir.py` & `trepan3k-1.2.9/trepan/processor/command/show_subcmd/tempdir.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 # Our local modules
 from trepan.processor.command.base_subcmd import DebuggerSubcommand
 
 
 class ShowTempdir(DebuggerSubcommand):
     """**show tempdir**
 
-Show the temporary directory usind in decompiled python files.
+    Show the temporary directory using in decompiled python files.
 
-See also:
---------
+    See also:
+    --------
 
-`set tempdir`
-"""
+    `set tempdir`"""
 
     in_list = True
     min_abbrev = len("temp")
     min_args = 0
     max_args = 0
     short_help = "Set a directory for storing decompiled Python"
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/skip.py` & `trepan3k-1.2.9/trepan/processor/command/skip.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,23 +19,22 @@
 from trepan.processor.cmdproc import print_location
 from trepan.lib import bytecode as Mbytecode
 
 
 class SkipCommand(DebuggerCommand):
     """**skip** [*count*]
 
-Set the next line that will be executed. The line must be within the
-stopped or bottom-most execution frame.
+    Set the next line that will be executed. The line must be within the
+    stopped or bottom-most execution frame.
 
-See also:
----------
+    See also:
+    ---------
 
-`next`, `step`, `jump`, `continue`, `return` and
-`finish` for other ways to progress execution.
-"""
+    `next`, `step`, `jump`, `continue`, `return` and
+    `finish` for other ways to progress execution."""
 
     aliases = ("sk",)
     execution_set = ["Running"]
     short_help = "Skip lines to be executed"
 
     DebuggerCommand.setup(locals(), category="running", max_args=1, need_stack=True)
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/source.py` & `trepan3k-1.2.9/trepan/processor/command/source.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,30 +23,28 @@
 from trepan.lib.file import readable
 from trepan.interfaces.script import ScriptInterface
 
 
 class SourceCommand(DebuggerCommand):
     """**source** [**-v**][**-Y**|**-N**][**-c**] *file*
 
-Read debugger commands from a file named *file*.  Optional *-v* switch
-(before the filename) causes each command in *file* to be echoed as it
-is executed.  Option *-Y* sets the default value in any confirmation
-command to be "yes" and *-N* sets the default value to "no".
+    Read debugger commands from a file named *file*.  Optional *-v* switch
+    (before the filename) causes each command in *file* to be echoed as it
+    is executed.  Option *-Y* sets the default value in any confirmation
+    command to be "yes" and *-N* sets the default value to "no".
 
-Note that the command startup file `.trepan3krc` is read automatically
-via a *source* command the debugger is started.
+    Note that the command startup file `.trepan3krc` is read automatically
+    via a *source* command the debugger is started.
 
-An error in any command terminates execution of the command file
-unless option `-c` is given."""
+    An error in any command terminates execution of the command file
+    unless option `-c` is given."""
 
     short_help = "Read and run debugger commands from a file"
 
-    DebuggerCommand.setup(
-        locals(), category="support", max_args=1
-    )
+    DebuggerCommand.setup(locals(), category="support", max_args=1)
 
     def complete(self, prefix):
         # files = Readline::FILENAME_COMPLETION_PROC.call(prefix) || []
         opts = ["-v", "-Y", "-N", "-c"]  # + files
         return complete_token(opts, prefix)
 
     def run(self, args):
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/step.py` & `trepan3k-1.2.9/trepan/processor/command/step.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,53 +19,52 @@
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.processor.cmdfns import want_different_line
 
 
 class StepCommand(DebuggerCommand):
     """**step**[**+**|**-**|**<**|**>**|**!**] [*event*...] [*count*]
 
-Execute the current line, stopping at the next event.
+    Execute the current line, stopping at the next event.
 
-With an integer argument, step that many times.
+    With an integer argument, step that many times.
 
-*event* is list of an event name which is one of: `call`,
-`return`, `line`, `exception` `c-call`, `c-return` or `c-exception`.
-If specified, only those stepping events will be considered. If no
-list of event names is given, then any event triggers a stop when the
-count is 0.
-
-There is however another way to specify a *single* event, by
-suffixing one of the symbols `<`, `>`, or `!` after the command or on
-an alias of that.  A suffix of `+` on a command or an alias forces a
-move to another line, while a suffix of `-` disables this requirement.
-A suffix of `>` will continue until the next call. (`finish` will run
-run until the return for that call.)
-
-If no suffix is given, the debugger setting `different-line`
-determines this behavior.
-
-Examples:
----------
-
-  step        # step 1 event, *any* event
-  step 1      # same as above
-  step 5/5+0  # same as above
-  step line   # step only line events
-  step call   # step only call events
-  step>       # same as above
-  step call line # Step line *and* call events
-
-Related and similar is the `next` command.
-
-See also:
----------
-
-`next`, `skip`, `jump` (there's no `hop` yet), `continue`, `return` and
-`finish` for other ways to progress execution.
-"""
+    *event* is list of an event name which is one of: `call`,
+    `return`, `line`, `exception` `c-call`, `c-return` or `c-exception`.
+    If specified, only those stepping events will be considered. If no
+    list of event names is given, then any event triggers a stop when the
+    count is 0.
+
+    There is however another way to specify a *single* event, by
+    suffixing one of the symbols `<`, `>`, or `!` after the command or on
+    an alias of that.  A suffix of `+` on a command or an alias forces a
+    move to another line, while a suffix of `-` disables this requirement.
+    A suffix of `>` will continue until the next call. (`finish` will run
+    run until the return for that call.)
+
+    If no suffix is given, the debugger setting `different-line`
+    determines this behavior.
+
+    Examples:
+    ---------
+
+      step        # step 1 event, *any* event
+      step 1      # same as above
+      step 5/5+0  # same as above
+      step line   # step only line events
+      step call   # step only call events
+      step>       # same as above
+      step call line # Step line *and* call events
+
+    Related and similar is the `next` command.
+
+    See also:
+    ---------
+
+    `next`, `skip`, `jump` (there's no `hop` yet), `continue`, `return` and
+    `finish` for other ways to progress execution."""
 
     aliases = (
         "step+",
         "step-",
         "step>",
         "step<",
         "step!",
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/tbreak.py` & `trepan3k-1.2.9/trepan/processor/command/tbreak.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,96 +11,97 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 import sys
 
+from trepan.processor.cmdbreak import parse_break_cmd, set_break
+
 # Our local modules
 from trepan.processor.command.base_cmd import DebuggerCommand
-from trepan.processor.cmdbreak import parse_break_cmd, set_break
 from trepan.processor.complete import complete_break_linenumber
 
 
 class TempBreakCommand(DebuggerCommand):
     """**tbreak** [*location*] [**if** *condition*]
 
-Sets a temporary breakpoint, i.e. one that is removed the after
-the first time it is encountered.
+    Sets a temporary breakpoint, i.e. one that is removed the after
+    the first time it is encountered.
 
-See the help for location for what can be specified there.
+    See the help for location for what can be specified there.
 
-Without arguments or an empty *location*, the temporary breakpoint is
-set at the current stopped location.
+    Without arguments or an empty *location*, the temporary breakpoint is
+    set at the current stopped location.
 
-If the word `if` is given after *location*, subsequent arguments given
-a boolean condition which must evaluate to True before the breakpoint
-is honored.
-
-Examples:
----------
-
-   tbreak                # Break where we are current stopped at
-   tbreak if i < j       # Break at current line if i < j
-   tbreak 10             # Break on line 10 of the file we are
-                         # currently stopped at
-   tbreak os.path.join() # Break in function os.path.join
-   tbreak x[i].fn() if x # break in function specified by x[i].fn
-                         # if x is set
-   tbreak os.path:45     # Break on line 45 file holding module os.path
-   tbreak myfile.py:45   # Break on line 45 of myfile.py
-   break '''c:\\foo.bat''':1"  # One way to specify a Windows file name,
-   break '''/My Docs/foo.py''':1"  # One way to specify path with blanks in it
+    If the word `if` is given after *location*, subsequent arguments given
+    a boolean condition which must evaluate to True before the breakpoint
+    is honored.
+
+    Examples:
+    ---------
+
+       tbreak                # Break where we are current stopped at
+       tbreak if i < j       # Break at current line if i < j
+       tbreak 10             # Break on line 10 of the file we are
+                             # currently stopped at
+       tbreak os.path.join() # Break in function os.path.join
+       tbreak x[i].fn() if x # break in function specified by x[i].fn
+                             # if x is set
+       tbreak os.path:45     # Break on line 45 file holding module os.path
+       tbreak myfile.py:45   # Break on line 45 of myfile.py
+       break '''c:\\foo.bat''':1"  # One way to specify a Windows file name,
+       break '''/My Docs/foo.py''':1"  # One way to specify path with blanks in it
 
-See also:
----------
+    See also:
+    ---------
 
-`break`, `condition` and `help syntax location`.
-"""
+    `break`, `condition` and `help syntax location`."""
 
     aliases = ("tb", "tbreak!", "tb!")
-    min_args      = 0
-    short_help    = 'Set temporary breakpoint at specified line or function'
+    min_args = 0
+    short_help = "Set temporary breakpoint at specified line or function"
 
     DebuggerCommand.setup(locals(), category="breakpoints", need_stack=True)
 
     complete = complete_break_linenumber
 
     def run(self, args):
         func, filename, lineno, condition, offset = parse_break_cmd(self.proc, args)
-        if not (func == None and filename == None):
-            set_break(self, func, filename, lineno, condition,
-                      True, args)
+        if not (func is None and filename is None):
+            set_break(self, func, filename, lineno, condition, True, args)
         return
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan.debugger import Trepan
 
     d = Trepan()
     command = TempBreakCommand(d.core.processor)
     command.proc.frame = sys._getframe()
     command.proc.setup()
 
     def doit(args):
         command.proc.current_command = " ".join(args)
         print(parse_break_cmd(command.proc, args))
 
     d = Trepan()
 
     print(doit(["10"]))
-    print(doit([__file__ + ':10']))
+    print(doit([__file__ + ":10"]))
 
     def foo():
-        return 'bar'
-    print(doit(['foo']))
-    print(doit(['os.path']))
-    print(doit(['os.path', '5+1']))
-    print(doit(['os.path.join']))
-    print(doit(['if', 'True']))
-    print(doit(['foo', 'if', 'True']))
-    print(doit(['os.path:10', 'if', 'True']))
-    command.run(['tbreak'])
-    command.run(['tbreak', 'command.run'])
-    command.run(['tbreak', '10'])
-    command.run(['tbreak', __file__ + ':10'])
-    command.run(['tbreak', 'foo'])
+        return "bar"
+
+    print(doit(["foo"]))
+    print(doit(["os.path"]))
+    print(doit(["os.path", "5+1"]))
+    print(doit(["os.path.join"]))
+    print(doit(["if", "True"]))
+    print(doit(["foo", "if", "True"]))
+    print(doit(["os.path:10", "if", "True"]))
+    command.run(["tbreak"])
+    command.run(["tbreak", "command.run"])
+    command.run(["tbreak", "10"])
+    command.run(["tbreak", __file__ + ":10"])
+    command.run(["tbreak", "foo"])
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/unalias.py` & `trepan3k-1.2.9/trepan/processor/command/unalias.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,48 +17,49 @@
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.lib.complete import complete_token
 
 
 class UnaliasCommand(DebuggerCommand):
     """**unalias** *alias-name*
 
-Remove alias *alias-name*
+    Remove alias *alias-name*
 
-See also:
----------
+    See also:
+    ---------
 
-'alias'
-"""
+    'alias'"""
 
-    min_args      = 1
-    short_help    = 'Remove an alias'
+    min_args = 1
+    short_help = "Remove an alias"
+
+    DebuggerCommand.setup(locals(), category="support", max_args=1)
 
-    DebuggerCommand.setup(
-        locals(), category="support", max_args=1
-    )
     def complete(self, prefix):
         return complete_token(self.proc.aliases.keys(), prefix)
 
     # Run command.
     def run(self, args):
         for arg in args[1:]:
             if arg in self.proc.aliases:
-                del(self.proc.aliases[arg])
+                del self.proc.aliases[arg]
                 self.msg("Alias for %s removed." % arg)
             else:
                 self.msg("No alias found for %s" % arg)
                 pass
             pass
         return
+
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     # Demo it.
     from trepan import debugger
-    d            = debugger.Trepan()
-    cp           = d.core.processor
-    command      = UnaliasCommand(cp)
-    command.run(['unalias', 's'])
-    command.run(['unalias', 's'])
-    command.run(['unalias', 'foo', 'n'])
-    print(command.complete(''))
+
+    d = debugger.Trepan()
+    cp = d.core.processor
+    command = UnaliasCommand(cp)
+    command.run(["unalias", "s"])
+    command.run(["unalias", "s"])
+    command.run(["unalias", "foo", "n"])
+    print(command.complete(""))
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/undisplay.py` & `trepan3k-1.2.9/trepan/processor/command/undisplay.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,60 +17,58 @@
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.lib import complete as Mcomplete
 
 
 class UndisplayCommand(DebuggerCommand):
     """**undisplay** *display-number*...
 
-Cancel some expressions to be displayed when program stops.
-Arguments are the code numbers of the expressions to stop displaying.
+    Cancel some expressions to be displayed when program stops.
+    Arguments are the code numbers of the expressions to stop displaying.
 
-No argument cancels all automatic-display expressions and is
-the same as `delete display`.
+    No argument cancels all automatic-display expressions and is
+    the same as `delete display`.
 
-See also:
----------
+    See also:
+    ---------
 
-`info display` to see current list of code numbers.
-"""
+    `info display` to see current list of code numbers."""
 
-    aliases       = ('und',)
-    short_help    = ('Cancel some expressions to be displayed '
-                     'when program stops')
+    aliases = ("und",)
+    short_help = "Cancel some expressions to be displayed " "when program stops"
 
     DebuggerCommand.setup(locals(), category="data", min_args=1)
 
-
     def complete(self, prefix):
-        completions = [str(disp.number) for disp in
-                       self.proc.display_mgr.list]
+        completions = [str(disp.number) for disp in self.proc.display_mgr.list]
         return Mcomplete.complete_token(completions, prefix)
 
     def run(self, args):
 
         if len(args) == 1:
             self.proc.display_mgr.clear()
             return
         for i in args[1:]:
-            i = self.proc.get_an_int(i, '%r must be a display number' % i)
+            i = self.proc.get_an_int(i, "%r must be a display number" % i)
             if i is not None:
                 if not self.proc.display_mgr.delete_index(i):
                     self.errmsg("No display number %d." % i)
                     return
                 pass
             pass
         return False
+
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     from trepan import debugger as Mdebugger
     from trepan.processor import cmdproc as Mcmdproc
     import inspect
-    d            = Mdebugger.Trepan()
-    cp           = d.core.processor
+
+    d = Mdebugger.Trepan()
+    cp = d.core.processor
     command = UndisplayCommand(d.core.processor)
     cp.curframe = inspect.currentframe()
-    cp.stack, cp.curindex = Mcmdproc.get_stack(cp.curframe, None, None,
-                                               cp)
-    command.run(['undisplay', 'z'])
-    command.run(['undisplay', '1', '10'])
+    cp.stack, cp.curindex = Mcmdproc.get_stack(cp.curframe, None, None, cp)
+    command.run(["undisplay", "z"])
+    command.run(["undisplay", "1", "10"])
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/up.py` & `trepan3k-1.2.9/trepan/processor/command/up.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,59 +17,61 @@
 # Our local modules
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.processor.frame import adjust_relative, frame_complete
 
 
 class UpCommand(DebuggerCommand):
 
-    signum        = -1  # This is what distinguishes us from "down"
+    signum = -1  # This is what distinguishes us from "down"
 
     DebuggerCommand.setup(locals(), category="stack", need_stack=True, max_args=1)
 
-    short_help    = 'Move frame in the direction of the caller of ' \
-      'the last-selected frame'
+    short_help = (
+        "Move frame in the direction of the caller of " "the last-selected frame"
+    )
 
     def complete(self, prefix):
         proc_obj = self.proc
         return frame_complete(proc_obj, prefix, self.signum)
 
     def run(self, args):
         """**up** [*count*]
 
-Move the current frame up in the stack trace (to an older frame). 0 is
-the most recent frame. If no count is given, move up 1.
+        Move the current frame up in the stack trace (to an older frame). 0 is
+        the most recent frame. If no count is given, move up 1.
 
-See also:
----------
+        See also:
+        ---------
 
-`down` and `frame`."""
+        `down` and `frame`."""
         adjust_relative(self.proc, self.name, args, self.signum)
         return False
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     from trepan.processor import cmdproc as Mcmdproc
     from trepan import debugger as Mdebugger
-    d            = Mdebugger.Trepan()
-    cp           = d.core.processor
+
+    d = Mdebugger.Trepan()
+    cp = d.core.processor
     command = UpCommand(cp)
-    command.run(['up'])
+    command.run(["up"])
 
     def nest_me(cp, command, i):
         import inspect
+
         if i > 1:
             cp.curframe = inspect.currentframe()
-            cp.stack, cp.curindex = Mcmdproc.get_stack(cp.curframe, None, None,
-                                                       cp)
-            command.run(['up'])
-            print('-' * 10)
-            command.run(['up', '-2'])
-            print('-' * 10)
-            command.run(['up', '-3'])
-            print('-' * 10)
+            cp.stack, cp.curindex = Mcmdproc.get_stack(cp.curframe, None, None, cp)
+            command.run(["up"])
+            print("-" * 10)
+            command.run(["up", "-2"])
+            print("-" * 10)
+            command.run(["up", "-3"])
+            print("-" * 10)
         else:
-            nest_me(cp, command, i+1)
+            nest_me(cp, command, i + 1)
         return
 
     cp.forget()
     nest_me(cp, command, 1)
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/command/whatis.py` & `trepan3k-1.2.9/trepan/processor/command/whatis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2013, 2015, 2020 Rocky Bernstein
+#
+#    Copyright (C) 2009, 2013, 2015, 2020, 2023 Rocky Bernstein
 #
 #    This program is free software; you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation; either version 2 of the License, or
 #    (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
@@ -11,44 +12,45 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program; if not, write to the Free Software
 #    Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 #    02110-1301 USA.
-import inspect, sys
+import inspect
+import sys
 
 # Our local modules
 from trepan.processor.command.base_cmd import DebuggerCommand
 from trepan.processor.complete import complete_id_and_builtins
 
 
 class WhatisCommand(DebuggerCommand):
     """**whatis** *arg*
 
-Prints the information argument which can be a Python expression.
+    Prints the information argument which can be a Python expression.
 
-When possible, we give information about:
+    When possible, we give information about:
 
-* type of argument
+    * type of argument
 
-* doc string for the argument (if a module, class, or function)
+    * doc string for the argument (if a module, class, or function)
 
-* comments around the definition of the argument (module)
+    * comments around the definition of the argument (module)
 
-* the module it was defined in
+    * the module it was defined in
 
-* where the argument was defined
+    * where the argument was defined
 
-We get this most of this information via the *inspect* module.
+    We get this most of this information via the *inspect* module.
 
-See also:
---------
+    See also:
+    --------
 
-the *inspect* module."""
+    the *inspect* module."""
 
     aliases = ()
     min_args = 1
     short_help = "Print data type of expression EXP"
 
     complete = complete_id_and_builtins
 
@@ -60,15 +62,15 @@
         try:
             if not proc.curframe:
                 # ?? Should we have set up a dummy globals
                 # to have persistence?
                 value = eval(arg, None, None)
             else:
                 value = eval(arg, proc.curframe.f_globals, proc.curframe.f_locals)
-        except:
+        except Exception:
             t, v = sys.exc_info()[:2]
             if type(t) == str:
                 exc_type_name = t
             else:
                 exc_type_name = t.__name__
             if exc_type_name == "NameError":
                 self.errmsg("Name Error: %s" % arg)
@@ -109,19 +111,19 @@
         comments = inspect.getcomments(value)
         if comments:
             self.msg("  comments:\n%s" % comments)
         try:
             m = inspect.getmodule(value)
             if m:
                 self.msg("  module:\t%s" % m)
-        except:
+        except Exception:
             try:
                 f = inspect.getfile(value)
                 self.msg("  file: %s" % f)
-            except:
+            except Exception:
                 pass
             pass
         return False
 
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/complete.py` & `trepan3k-1.2.9/trepan/processor/complete.py`

 * *Files identical despite different names*

### Comparing `trepan3k-1.2.8/trepan/processor/frame.py` & `trepan3k-1.2.9/trepan/processor/frame.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,32 +20,37 @@
 from trepan.processor import cmdfns as Mcmdfns
 from trepan.lib import complete as Mcomplete
 
 
 def frame_low_high(proc_obj, direction):
     stack_size = len(proc_obj.stack)  # - hide_level
     if direction is None:
-        return [-stack_size, stack_size-1]
+        return [-stack_size, stack_size - 1]
     else:
         frame_index = proc_obj.curindex
-        low, high = [ frame_index * -direction,
-                      (stack_size - frame_index - 1) * direction ]
-        if direction < 0: low, high = [high, low]
+        low, high = [
+            frame_index * -direction,
+            (stack_size - frame_index - 1) * direction,
+        ]
+        if direction < 0:
+            low, high = [high, low]
         return (low, high)
     return
 
 
 def frame_complete(proc_obj, prefix, direction):
     low, high = frame_low_high(proc_obj, direction)
-    ary = [str(low+i) for i in range(high-low+1)]
+    ary = [str(low + i) for i in range(high - low + 1)]
     return Mcomplete.complete_token(ary, prefix)
 
+
 def frame_num(proc_obj, pos):
     return len(proc_obj.stack) - pos - 1
 
+
 def adjust_frame(proc_obj, name, pos, absolute_pos):
     """Adjust stack frame by pos positions. If absolute_pos then
     pos is an absolute number. Otherwise it is a relative number.
 
     A negative number indexes from the other end."""
     if not proc_obj.curframe:
         proc_obj.errmsg("No stack.")
@@ -69,34 +74,38 @@
     elif pos >= len(proc_obj.stack):
         proc_obj.errmsg("Adjusting would put us beyond the newest frame.")
         return
 
     proc_obj.curindex = pos
     proc_obj.curframe = proc_obj.stack[proc_obj.curindex][0]
     proc_obj.location()
-    proc_obj.list_lineno   = None
-    proc_obj.list_offset   = proc_obj.curframe.f_lasti
-    proc_obj.list_object   = proc_obj.curframe
+    proc_obj.list_lineno = None
+    proc_obj.list_offset = proc_obj.curframe.f_lasti
+    proc_obj.list_object = proc_obj.curframe
     proc_obj.list_filename = proc_obj.curframe.f_code.co_filename
 
     return
 
 
 def adjust_relative(proc_obj, name, args, signum):
     if not proc_obj.stack:
         proc_obj.errmsg("Program has no stack frame set.")
         return False
     if len(args) == 1:
         count = 1
     else:
         count_str = args[1]
         low, high = frame_low_high(proc_obj, signum)
-        count = Mcmdfns.get_an_int( proc_obj.errmsg, count_str,
-                                    ("The '%s' command argument must eval to" +
-                                     " an integer. Got: %s") %
-                                     (name, count_str), low, high )
-        if count is None: return
+        count = Mcmdfns.get_an_int(
+            proc_obj.errmsg,
+            count_str,
+            ("The '%s' command argument must eval to" + " an integer. Got: %s")
+            % (name, count_str),
+            low,
+            high,
+        )
+        if count is None:
+            return
         pass
 
-    adjust_frame(proc_obj, name, pos=signum*count,
-                 absolute_pos=False)
+    adjust_frame(proc_obj, name, pos=signum * count, absolute_pos=False)
     return
```

### Comparing `trepan3k-1.2.8/trepan/processor/location.py` & `trepan3k-1.2.9/trepan/processor/location.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 # -*- coding: utf-8 -*-
 #
-#  Copyright (C) 2017, 2020 Rocky Bernstein
+#  Copyright (C) 2017, 2020, 2023 Rocky Bernstein
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import inspect, pyficache
-from trepan.lib.stack import frame2file
+import inspect
 import os.path as osp
+
+import pyficache
+
+from trepan.lib.stack import frame2file
 from trepan.processor.parse.semantics import Location
 
 INVALID_LOCATION = None
 
 
 def resolve_location(proc, location):
     """Expand fields in Location namedtuple. If:
-       '.':  get fields from stack
-       function/module: get fields from evaluation/introspection
-       location file and line number: use that
+    '.':  get fields from stack
+    function/module: get fields from evaluation/introspection
+    location file and line number: use that
     """
     curframe = proc.curframe
     offset = None
     if location == ".":
         if not curframe:
             proc.errmsg("Don't have a stack to get location from")
             return INVALID_LOCATION
@@ -39,58 +42,58 @@
         offset = curframe.f_lasti
         return Location(filename, lineno, False, None, offset)
 
     assert isinstance(location, Location)
     is_address = location.is_address
     if proc.curframe:
         g = curframe.f_globals
-        l = curframe.f_locals
+        locals_dict = curframe.f_locals
     else:
         g = globals()
-        l = locals()
+        locals_dict = locals()
         pass
     if location.method:
         # Validate arguments that can't be done in parsing
         filename = lineno = None
         msg = "Object %s is not known yet as a function, " % location.method
         try:
-            modfunc = eval(location.method, g, l)
-        except:
+            modfunc = eval(location.method, g, locals_dict)
+        except Exception:
             proc.errmsg(msg)
             return INVALID_LOCATION
 
         try:
             # Check if the converted string is a function or instance
             # method.  We don't want to test on attributes and not use
-            # `inspect.isfunction()` so that we can accomadate
+            # `inspect.isfunction()` so that we can accommodate
             # trepan-xpy() which has it's own type of compatible
             # Function, that would fail an `inspect.isfunction()`
             # test.
             if hasattr(modfunc, "__code__") or hasattr(modfunc, "im_func"):
                 offset = -1
             else:
                 proc.errmsg(msg)
                 return INVALID_LOCATION
-        except:
+        except Exception:
             proc.errmsg(msg)
             return INVALID_LOCATION
         filename = proc.core.canonic(modfunc.__code__.co_filename)
         # FIXME: we may want to check lineno and
         # respect that in the future
         lineno = modfunc.__code__.co_firstlineno
     elif location.path:
         filename = proc.core.canonic(location.path)
         lineno = location.line_number
         modfunc = None
         msg = "%s is not known as a file" % location.path
         if not osp.isfile(filename):
             # See if argument is a module
             try:
-                modfunc = eval(location.path, g, l)
-            except:
+                modfunc = eval(location.path, g, locals_dict)
+            except Exception:
                 msg = (
                     "Don't see '%s' as a existing file or as an module" % location.path
                 )
                 proc.errmsg(msg)
                 return INVALID_LOCATION
             pass
             is_address = location.is_address
@@ -146,52 +149,52 @@
         modfunc = None
         offset = location.offset
     return Location(filename, lineno, is_address, modfunc, offset)
 
 
 def resolve_address_location(proc, location):
     """Expand fields in Location namedtuple. If:
-       '.':  get fields from stack
-       function/module: get fields from evaluation/introspection
-       location file and line number: use that
+    '.':  get fields from stack
+    function/module: get fields from evaluation/introspection
+    location file and line number: use that
     """
     curframe = proc.curframe
     if location == ".":
         filename = frame2file(proc.core, curframe, canonic=False)
         offset = curframe.f_lasti
         is_address = True
         return Location(filename, offset, False, None, offset)
 
     assert isinstance(location, Location)
     is_address = True
     if proc.curframe:
         g = curframe.f_globals
-        l = curframe.f_locals
+        locals_dict = curframe.f_locals
     else:
         g = globals()
-        l = locals()
+        locals_dict = locals()
         pass
     if location.method:
         # Validate arguments that can't be done in parsing
         filename = offset = None
         msg = "Object %s is not known yet as a function, " % location.method
         try:
-            modfunc = eval(location.method, g, l)
-        except:
+            modfunc = eval(location.method, g, locals_dict)
+        except Exception:
             proc.errmsg(msg)
             return INVALID_LOCATION
 
         try:
             # Check if the converted string is a function or instance method
             if inspect.isfunction(modfunc) or hasattr(modfunc, "im_func"):
                 pass
             else:
                 proc.errmsg(msg)
                 return INVALID_LOCATION
-        except:
+        except Exception:
             proc.errmsg(msg)
             return INVALID_LOCATION
         filename = proc.core.canonic(modfunc.func_code.co_filename)
         # FIXME: we may want to check offset and
         # respect that in the future
         offset = 0
     elif location.path:
@@ -199,16 +202,16 @@
         offset = location.line_number
         is_address = location.is_address
         modfunc = None
         msg = "%s is not known as a file" % location.path
         if not osp.isfile(filename):
             # See if argument is a module
             try:
-                modfunc = eval(location.path, g, l)
-            except:
+                modfunc = eval(location.path, g, locals_dict)
+            except Exception:
                 msg = (
                     "Don't see '%s' as a existing file or as an module" % location.path
                 )
                 proc.errmsg(msg)
                 return INVALID_LOCATION
             pass
             is_address = location.is_address
```

### Comparing `trepan3k-1.2.8/trepan/processor/parse/parser.py` & `trepan3k-1.2.9/trepan/processor/parse/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,114 +13,126 @@
 import sys
 from spark_parser.ast import AST
 
 from trepan.processor.parse.scanner import LocationScanner, ScannerError
 
 from spark_parser import GenericASTBuilder
 
-DEFAULT_DEBUG = {'rules': False, 'transition': False, 'reduce': False,
-                 'errorstack': None,
-                 'dups': False, 'local_print': False}
+DEFAULT_DEBUG = {
+    "rules": False,
+    "transition": False,
+    "reduce": False,
+    "errorstack": None,
+    "dups": False,
+    "local_print": False,
+}
+
 
 class LocationError(Exception):
     def __init__(self, text, text_cursor):
         self.text = text
         self.text_cursor = text_cursor
 
     def __str__(self):
         return self.text + "\n" + self.text_cursor
 
+
 class LocationParser(GenericASTBuilder):
     """Location parsing as used in trepan2 and trepan3k
     for list, breakpoint, and assembly commands
     Note: function parse() comes from GenericASTBuilder
     """
 
     def __init__(self, start_nt, text, debug=None):
         super(LocationParser, self).__init__(AST, start_nt, debug=DEFAULT_DEBUG)
         self.debug = debug
-        self.text  = text
+        self.text = text
 
     def error(self, tokens, index):
         token = tokens[index]
-        if self.debug.get('local_print', False):
+        if self.debug.get("local_print", False):
             print(self.text)
-            print(' ' * (token.offset + len(str(token.value))) + '^')
+            print(" " * (token.offset + len(str(token.value))) + "^")
             print("Syntax error at or near token '%s'" % token.value)
-            if 'context' in self.debug and self.debug['context']:
+            if "context" in self.debug and self.debug["context"]:
                 super(LocationParser, self).error(tokens, index)
-        raise LocationError(self.text,
-                         ' ' * (token.offset + len(str(token.value))) + '^')
+        raise LocationError(
+            self.text, " " * (token.offset + len(str(token.value))) + "^"
+        )
 
     def nonterminal(self, nt, args):
-        has_len = hasattr(args, '__len__')
+        has_len = hasattr(args, "__len__")
 
         # collect = ('tokens',)
         # if nt in collect and len(args) > 1:
         #     #
         #     #  Collect iterated thingies together.
         #     #
         #     rv = args[0]
         #     for arg in args[1:]:
         #         rv.append(arg)
 
-        if (has_len and len(args) == 1 and
-            hasattr(args[0], '__len__') and len(args[0]) == 1):
+        if (
+            has_len
+            and len(args) == 1
+            and hasattr(args[0], "__len__")
+            and len(args[0]) == 1
+        ):
             # Remove singleton derivations
             rv = GenericASTBuilder.nonterminal(self, nt, args[0])
-            del args[0] # save memory
+            del args[0]  # save memory
         else:
             rv = GenericASTBuilder.nonterminal(self, nt, args)
         return rv
 
     ##########################################################
     # Expression grammar rules. Grammar rule functions
     # start with the name p_ and are collected automatically
     ##########################################################
 
     def p_bp_location(self, args):
-        '''
+        """
         bp_start    ::= opt_space location_if opt_space
-        '''
+        """
 
     # "disasm" command range which might refer to locations, ranges, and addresses
     def p_asm_range(self, args):
-        '''
+        """
         arange_start  ::= opt_space arange
         arange ::= range
         arange ::= addr_location opt_space COMMA opt_space NUMBER
         arange ::= addr_location opt_space COMMA opt_space OFFSET
         arange ::= addr_location opt_space COMMA opt_space ADDRESS
         arange ::= location opt_space COMMA opt_space ADDRESS
         arange ::= addr_location opt_space COMMA
         arange ::= addr_location
 
         # Unlike ranges, We don't allow ending at an address
         # arange ::= COMMA opt_space addr_location
 
         addr_location ::= location
         addr_location ::= ADDRESS
-        '''
+        """
 
     # "list" command range which may refer to locations
     def p_list_range(self, args):
-        '''
+        """
         range_start  ::= opt_space range
         range ::= location
         range ::= location opt_space COMMA opt_space NUMBER
         range ::= location opt_space COMMA opt_space OFFSET
         range ::= COMMA opt_space location
         range ::= location opt_space COMMA
         range ::= location
         range ::= DIRECTION
-        '''
+        """
 
     # location that is used in breakpoints, list commands, and disassembly
     def p_location(self, args):
-        '''
+        """
         opt_space   ::= SPACE?
 
         location_if ::= location
         location_if ::= location SPACE IF tokens
 
         # Note no space is allowed between FILENAME COLON, and NUMBER
         location    ::= FILENAME COLON NUMBER
@@ -140,18 +152,20 @@
         token       ::= COMMA
         token       ::= DIRECTION
         token       ::= FILENAME
         token       ::= FUNCNAME
         token       ::= NUMBER
         token       ::= OFFSET
         token       ::= SPACE
-        '''
+        """
+
 
-def parse_location(start_symbol, text, out=sys.stdout,
-                      show_tokens=False, parser_debug=DEFAULT_DEBUG):
+def parse_location(
+    start_symbol, text, out=sys.stdout, show_tokens=False, parser_debug=DEFAULT_DEBUG
+):
     assert isinstance(text, str)
     tokens = LocationScanner().tokenize(text)
     if show_tokens:
         for t in tokens:
             print(t)
 
     # For heavy grammar debugging
@@ -160,24 +174,28 @@
     # parser_debug = {'rules': False, 'transition': False, 'reduce': True,
     #                 'errorstack': 'full', 'dups': False}
 
     parser = LocationParser(start_symbol, text, parser_debug)
     # parser.check_grammar(frozenset(('bp_start', 'range_start', 'arange_start')))
     return parser.parse(tokens)
 
+
 def parse_bp_location(*args, **kwargs):
-    return parse_location('bp_start', *args, **kwargs)
+    return parse_location("bp_start", *args, **kwargs)
+
 
 def parse_range(*args, **kwargs):
-    return parse_location('range_start', *args, **kwargs)
+    return parse_location("range_start", *args, **kwargs)
+
 
 def parse_arange(*args, **kwargs):
-    return parse_location('arange_start', *args, **kwargs)
+    return parse_location("arange_start", *args, **kwargs)
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":
 
     def doit(fn, line):
         try:
             ast = fn(line, show_tokens=True)
             print(ast)
         except ScannerError as e:
             print("Scanner error")
@@ -232,22 +250,15 @@
     #         continue
     #     print("=" * 30)
     #     print(line)
     #     print("+" * 30)
     #     doit(parse_range, line)
     #     print(ast)
 
-    lines = (
-    "*0",
-    "*1 ,",
-    "2 , *10",
-    "2, 10",
-    "*3,  10",
-    "sys.exit() , *20"
-    )
+    lines = ("*0", "*1 ,", "2 , *10", "2, 10", "*3,  10", "sys.exit() , *20")
     for line in lines:
         line = line.strip()
         if not line:
             continue
         print("=" * 30)
         print(line)
         print("+" * 30)
```

### Comparing `trepan3k-1.2.8/trepan/processor/parse/scanner.py` & `trepan3k-1.2.9/trepan/processor/parse/scanner.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,35 +4,34 @@
 """
 
 from __future__ import print_function
 import re
 from spark_parser.scanner import GenericScanner
 from trepan.processor.parse.tok import Token
 
+
 class ScannerError(Exception):
     def __init__(self, text, text_cursor):
         self.text = text
         self.text_cursor = text_cursor
 
     def __str__(self):
         return self.text + "\n" + self.text_cursor
 
-class LocationScanner(GenericScanner):
 
+class LocationScanner(GenericScanner):
     def error(self, s):
         """Show text and a caret under that. For example:
-x = 2y + z
-     ^
-"""
+        x = 2y + z
+             ^"""
         # print("Lexical error:")
         # print("%s" % s[:self.pos+10])  # + 10 for trailing context
         # print("%s^" % (" "*(self.pos-1)))
         # for t in self.rv: print(t)
-        raise ScannerError( ("%s" % s),
-                            ("%s^" % (" "*(self.pos-1))) )
+        raise ScannerError(("%s" % s), ("%s^" % (" " * (self.pos - 1))))
 
     def tokenize(self, input):
         self.rv = []
         GenericScanner.tokenize(self, input)
         return self.rv
 
     def add_token(self, name, v):
@@ -46,115 +45,117 @@
     # method names of this class and the docstrings to come
     # up with both the names of the tokens and the regular expressions
     # that make up those tokens
 
     # Recognize white space, but we don't create a token for it.
     # This has the effect of stripping white space between tokens
     def t_whitespace(self, s):
-        r'\s+'
-        self.add_token('SPACE', s)
+        r"\s+"
+        self.add_token("SPACE", s)
         self.pos += len(s)
         pass
 
     def t_file_or_func(self, s):
         r'(?:[^*-+@,\d\'"\t \n:][^\'"\t \n:,]*)|(?:^""".+""")|(?:\'\'\'.+\'\'\')'
         maybe_funcname = True
-        if s == 'if':
-            self.add_token('IF', s)
+        if s == "if":
+            self.add_token("IF", s)
             return
         if s[0] in frozenset(('"', "'")):
             # Pick out text inside of triple-quoted string
-            if ( (s.startswith("'''") and s.endswith("'''") ) or
-                 (s.startswith('"""') and s.endswith('"""') ) ):
+            if (s.startswith("'''") and s.endswith("'''")) or (
+                s.startswith('"""') and s.endswith('"""')
+            ):
                 base = s[3:-3]
             else:
                 # Pick out text inside singly-quote string
                 base = s[1:-1]
             maybe_funcname = False
         else:
             base = s
-        if maybe_funcname and re.match('[a-zA-Z_][a-zA-Z_.0-9]+\(\)', s):
-            self.add_token('FUNCNAME', base)
+        if maybe_funcname and re.match(r"[a-zA-Z_][a-zA-Z_.0-9]+\(\)", s):
+            self.add_token("FUNCNAME", base)
         else:
-            self.add_token('FILENAME', base)
+            self.add_token("FILENAME", base)
         self.pos += len(s)
 
     def t_single_quote_file(self, s):
         r"'[^'].+'"
         # Pick out text inside of singe-quoted string
         base = s[1:-1]
-        self.add_token('FILENAME', base)
+        self.add_token("FILENAME", base)
         self.pos += len(s)
 
     def t_double_quote_file(self, s):
         r'"[^"]+"'
         # Pick out text inside of singe-quoted string
         base = s[1:-1]
-        self.add_token('FILENAME', base)
+        self.add_token("FILENAME", base)
         self.pos += len(s)
 
     def t_colon(self, s):
-        r':'
+        r":"
         # Used to separate a filename from a line number
-        self.add_token('COLON', s)
+        self.add_token("COLON", s)
         self.pos += len(s)
 
     def t_comma(self, s):
-        r','
+        r","
         # Used in "list" to separate first from last
-        self.add_token('COMMA', s)
+        self.add_token("COMMA", s)
         self.pos += len(s)
 
     def t_direction(self, s):
-        r'^[+-]$'
+        r"^[+-]$"
         # Used in the "list" command
-        self.add_token('DIRECTION', s)
+        self.add_token("DIRECTION", s)
         self.pos += len(s)
 
     # Recognize integers
     def t_number(self, s):
-        r'\d+'
+        r"\d+"
         pos = self.pos
-        self.add_token('NUMBER', int(s))
+        self.add_token("NUMBER", int(s))
         self.pos = pos + len(s)
 
     # Recognize list offsets (counts)
     def t_offset(self, s):
-        r'[+]\d+'
+        r"[+]\d+"
         pos = self.pos
-        self.add_token('OFFSET', s)
+        self.add_token("OFFSET", s)
         self.pos = pos + len(s)
 
     # Recognize addresses (bytecode offsets)
     def t_address(self, s):
-        r'[*@]\d+'
+        r"[*@]\d+"
         pos = self.pos
-        self.add_token('ADDRESS', s)
+        self.add_token("ADDRESS", s)
         self.pos = pos + len(s)
 
+
 if __name__ == "__main__":
     for line in (
-            # '/tmp/foo.py:12',
-            # "'''/tmp/foo.py:12'''",
-            "'/tmp/foo.py:12'",
-            "6",
-            "*6",
-            "@6",
-            "8 *6",
-            # "/tmp/foo.py line 12",
-            # "\"\"\"/tmp/foo.py's line 12\"\"\"",
-            # "12",
-            # "../foo.py:5",
-            # "gcd()",
-            # "foo.py line 5 if x > 1",
-            # "5 ,",
-            # "5,",
-            # "5,10",
-            # ",10",
-            ):
+        # '/tmp/foo.py:12',
+        # "'''/tmp/foo.py:12'''",
+        "'/tmp/foo.py:12'",
+        "6",
+        "*6",
+        "@6",
+        "8 *6",
+        # "/tmp/foo.py line 12",
+        # "\"\"\"/tmp/foo.py's line 12\"\"\"",
+        # "12",
+        # "../foo.py:5",
+        # "gcd()",
+        # "foo.py line 5 if x > 1",
+        # "5 ,",
+        # "5,",
+        # "5,10",
+        # ",10",
+    ):
         try:
             tokens = LocationScanner().tokenize(line.strip())
             for t in tokens:
                 print(t)
                 pass
         except ScannerError as e:
             print("Lexical error at or around: ")
```

### Comparing `trepan3k-1.2.8/trepan/processor/parse/semantics.py` & `trepan3k-1.2.9/trepan/processor/parse/semantics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,83 +1,89 @@
 #  Copyright (c) 2017-2018, 2020 by Rocky Bernstein
 
 from trepan.processor.parse.parser import (
-    parse_bp_location, parse_range, parse_arange, parse_location
-    )
+    parse_bp_location,
+    parse_range,
+    parse_arange,
+    parse_location,
+)
 from trepan.processor.parse.parser import LocationError as PLocationError
 from trepan.processor.parse.scanner import ScannerError
-from spark_parser import GenericASTTraversal # , DEFAULT_DEBUG as PARSER_DEFAULT_DEBUG
+from spark_parser import GenericASTTraversal  # , DEFAULT_DEBUG as PARSER_DEFAULT_DEBUG
 
 from collections import namedtuple
+
 Location = namedtuple("Location", "path line_number is_address method offset")
 BPLocation = namedtuple("BPLocation", "location condition")
 ListRange = namedtuple("ListRange", "first last")
 
 
 class LocationError(Exception):
     def __init__(self, errmsg):
         self.errmsg = errmsg
 
     def __str__(self):
         return self.errmsg
 
+
 class RangeError(Exception):
     def __init__(self, errmsg):
         self.errmsg = errmsg
 
     def __str__(self):
         return self.errmsg
 
-class LocationGrok(GenericASTTraversal, object):
 
+class LocationGrok(GenericASTTraversal, object):
     def __init__(self, text):
         GenericASTTraversal.__init__(self, None)
         self.text = text
         self.result = None
         return
 
     def n_addr_location(self, node):
         # addr_location ::= location
         # addr_location ::= ADDRESS
         # addr_location ::= FUNCNAME (via location singleton reduce)
         # addr_location ::= NUMBER (via location singleton reduce)
 
         path, line_number, method = None, None, None
         n0 = node[0]
-        if n0 in ('ADDRESS', 'FUNCNAME', 'NUMBER'):
-            if n0 == 'ADDRESS':
-                assert node[0].value[0] == '*'
+        if n0 in ("ADDRESS", "FUNCNAME", "NUMBER"):
+            if n0 == "ADDRESS":
+                assert node[0].value[0] == "*"
                 line_number = int(node[0].value[1:])
                 self.result = Location(path, line_number, True, method, offset=None)
-            elif n0 == 'NUMBER':
+            elif n0 == "NUMBER":
                 self.result = Location(path, node[0].value, True, method, offset=None)
             else:
-                self.result = Location(path, line_number, False, node[0].value[:-2], offset=None)
+                self.result = Location(
+                    path, line_number, False, node[0].value[:-2], offset=None
+                )
             node.location = self.result
             self.prune()
         elif n0 == "OFFSET":
             print("WOOT")
         else:
             # print(node[0])
-            assert node[0] == 'location'
+            assert node[0] == "location"
             self.preorder(node[0])
             node.location = node[0].location
 
-
     def n_location(self, node):
         path, line_number, method, offset = None, None, None, None
-        if node[0] == 'FILENAME':
+        if node[0] == "FILENAME":
             path = node[0].value
             # If there is a line number, it is the last token of a location
-            if len(node) > 1 and node[-1] == 'NUMBER':
+            if len(node) > 1 and node[-1] == "NUMBER":
                 line_number = node[-1].value
-        elif node[0] == 'FUNCNAME':
+        elif node[0] == "FUNCNAME":
             method = node[0].value[:-2]
             offset = 0
-        elif node[0] == 'NUMBER':
+        elif node[0] == "NUMBER":
             line_number = node[0].value
         else:
             assert True, "n_location: Something's is wrong; node[0] is %s" % node[0]
         self.result = Location(path, line_number, False, method, offset=offset)
         node.location = Location(path, line_number, False, method, offset=offset)
         self.prune()
 
@@ -88,224 +94,252 @@
         self.result = Location(None, None, True, None, offset=int(node.value[1:]))
 
     def n_FUNCNAME(self, node):
         self.result = Location(None, None, False, node.value[:-2], offset=0)
 
     def n_location_if(self, node):
         location = None
-        if node[0] == 'location':
+        if node[0] == "location":
             self.preorder(node[0])
             location = node[0].location
 
         if len(node) == 1:
             return
-        if node[1] == 'IF':
+        if node[1] == "IF":
             if_node = node[1]
-        elif node[2] == 'IF':
+        elif node[2] == "IF":
             if_node = node[2]
-        elif node[3] == 'IF':
+        elif node[3] == "IF":
             if_node = node[3]
         else:
             assert False, 'location_if: Something is wrong; cannot find "if"'
 
-        condition = self.text[if_node.offset+len(if_node.value)+1:]
+        condition = self.text[if_node.offset + len(if_node.value) + 1 :]
 
         # Pick out condition from string and location inside "IF" token
         self.result = BPLocation(location, condition)
         self.prune()
 
     # FIXME: DRY with range
     def n_arange(self, arange_node):
-        if arange_node[0]  == 'range':
+        if arange_node[0] == "range":
             arange_node = arange_node[0]
-        l = len(arange_node)
-        if 1 <= l <= 2:
+        node_len = len(arange_node)
+        if 1 <= node_len <= 2:
             # arange ::= location
             # arange ::= DIRECTION
             # arange ::= FUNCNAME
             # arange ::= NUMBER
             # arange ::= ADDRESS
             last_node = arange_node[-1]
-            if last_node == 'location':
+            if last_node == "location":
                 self.preorder(arange_node[-1])
                 self.result = ListRange(last_node.location, None)
-            elif last_node == 'FUNCNAME':
-                self.result = ListRange(Location(None, None, False, last_node.value[:-2], offset=0),
-                                        None)
-            elif last_node in ('NUMBER', 'OFFSET', 'ADDRESS'):
+            elif last_node == "FUNCNAME":
+                self.result = ListRange(
+                    Location(None, None, False, last_node.value[:-2], offset=0), None
+                )
+            elif last_node in ("NUMBER", "OFFSET", "ADDRESS"):
                 offset = None
-                if last_node == 'ADDRESS':
+                if last_node == "ADDRESS":
                     assert last_node.value[0] in ["*", "@"]
                     is_address = True
                     value = int(last_node.value[1:])
                     offset = value
                 else:
                     is_address = False
                     value = last_node.value
 
-                self.result = ListRange(Location(None, value, is_address, None, offset=offset),
-                                        None)
+                self.result = ListRange(
+                    Location(None, value, is_address, None, offset=offset), None
+                )
             else:
-                assert last_node == 'DIRECTION'
+                assert last_node == "DIRECTION"
                 self.result = ListRange(None, last_node.value)
                 pass
             self.prune()
-        elif l == 3:
+        elif node_len == 3:
             # arange ::= COMMA opt_space location
             # arange ::= location opt_space COMMA
-            if arange_node[0] == 'COMMA':
-                assert arange_node[-1] == 'location'
+            if arange_node[0] == "COMMA":
+                assert arange_node[-1] == "location"
                 self.preorder(arange_node[-1])
                 self.result = ListRange(None, self.result)
                 self.prune()
             else:
-                assert arange_node[-1] == 'COMMA'
-                assert arange_node[0] == 'location'
+                assert arange_node[-1] == "COMMA"
+                assert arange_node[0] == "location"
                 self.preorder(arange_node[0])
                 self.result = ListRange(arange_node[0].location, None)
                 self.prune()
                 pass
-        elif l == 5:
+        elif node_len == 5:
             # arange ::= location opt_space COMMA opt_space {NUMBER | OFFSET | ADDRESS}
-            assert arange_node[2] == 'COMMA'
-            assert arange_node[-1] in ('NUMBER', 'OFFSET', 'ADDRESS')
+            assert arange_node[2] == "COMMA"
+            assert arange_node[-1] in ("NUMBER", "OFFSET", "ADDRESS")
             self.preorder(arange_node[0])
             self.result = ListRange(arange_node[0].location, arange_node[-1].value)
             self.prune()
         else:
             raise RangeError("Something is wrong")
         return
 
     def n_range(self, range_node):
-        l = len(range_node)
-        if 1 <= l <= 2:
+        node_len = len(range_node)
+        if 1 <= node_len <= 2:
             # range ::= location
             # range ::= DIRECTION
             # range ::= FUNCNAME
             # range ::= NUMBER
             # range ::= OFFSET
             last_node = range_node[-1]
-            if last_node == 'location':
+            if last_node == "location":
                 self.preorder(range_node[-1])
                 self.result = ListRange(last_node.location, None)
-            elif last_node == 'FUNCNAME':
-                self.result = ListRange(Location(None, None, False, last_node.value[:-2], offset=None),
-                                        None)
-            elif last_node in ('NUMBER', 'OFFSET'):
-                self.result = ListRange(Location(None, last_node.value, False, None, offset=None),
-                                        None)
+            elif last_node == "FUNCNAME":
+                self.result = ListRange(
+                    Location(None, None, False, last_node.value[:-2], offset=None), None
+                )
+            elif last_node in ("NUMBER", "OFFSET"):
+                self.result = ListRange(
+                    Location(None, last_node.value, False, None, offset=None), None
+                )
             else:
-                assert last_node == 'DIRECTION'
+                assert last_node == "DIRECTION"
                 self.result = ListRange(None, last_node.value)
                 pass
             self.prune()
-        elif l == 3:
+        elif node_len == 3:
             # range ::= COMMA opt_space location
             # range ::= location opt_space COMMA
-            if range_node[0] == 'COMMA':
-                assert range_node[-1] == 'location'
+            if range_node[0] == "COMMA":
+                assert range_node[-1] == "location"
                 self.preorder(range_node[-1])
                 self.result = ListRange(None, self.result)
                 self.prune()
             else:
-                assert range_node[-1] == 'COMMA'
-                assert range_node[0] == 'location'
+                assert range_node[-1] == "COMMA"
+                assert range_node[0] == "location"
                 self.preorder(range_node[0])
                 self.result = ListRange(range_node[0].location, None)
                 self.prune()
                 pass
-        elif l == 5:
+        elif node_len == 5:
             # range ::= location opt_space COMMA opt_space {NUMBER|OFFSET}
-            assert range_node[2] == 'COMMA'
-            assert range_node[-1] in ('NUMBER', 'OFFSET')
+            assert range_node[2] == "COMMA"
+            assert range_node[-1] in ("NUMBER", "OFFSET")
             self.preorder(range_node[0])
             self.result = ListRange(range_node[0].location, range_node[-1].value)
             self.prune()
         else:
             raise RangeError("Something is wrong")
         return
 
     def default(self, node):
-        if node not in frozenset(("""opt_space tokens token bp_start range_start arange_start
-                                  IF FILENAME COLON COMMA SPACE DIRECTION""".split())):
-            assert False, ("Something's wrong: you missed a rule for %s" % node.kind)
+        if node not in frozenset(
+            (
+                """opt_space tokens token bp_start range_start arange_start
+                                  IF FILENAME COLON COMMA SPACE DIRECTION""".split()
+            )
+        ):
+            assert False, "Something's wrong: you missed a rule for %s" % node.kind
 
     def traverse(self, node):
         return self.preorder(node)
 
 
 def build_bp_expr(string, show_tokens=False, show_ast=False, show_grammar=False):
-    parser_debug = {'rules': False, 'transition': False,
-                    'reduce': show_grammar,
-                    'errorstack': None, 'dups': False
-                    # 'context': True, 'dups': True
-                        }
-    parsed = parse_bp_location(string, show_tokens=show_tokens,
-                               parser_debug=parser_debug)
-    assert parsed == 'bp_start'
+    parser_debug = {
+        "rules": False,
+        "transition": False,
+        "reduce": show_grammar,
+        "errorstack": None,
+        "dups": False
+        # 'context': True, 'dups': True
+    }
+    parsed = parse_bp_location(
+        string, show_tokens=show_tokens, parser_debug=parser_debug
+    )
+    assert parsed == "bp_start"
     if show_ast:
         print(parsed)
     walker = LocationGrok(string)
     walker.traverse(parsed)
     bp_expr = walker.result
     if isinstance(bp_expr, Location):
         bp_expr = BPLocation(bp_expr, None)
     location = bp_expr.location
-    assert location.line_number is not None or location.offset is not None or location.method
+    assert (
+        location.line_number is not None
+        or location.offset is not None
+        or location.method
+    )
     return bp_expr
 
+
 def build_range(string, show_tokens=False, show_ast=False, show_grammar=False):
-    parser_debug = {'rules': False, 'transition': False,
-                    'reduce': show_grammar,
-                    'errorstack': None,
-                    'context': False, 'dups': True
-                        }
-    parsed = parse_range(string, show_tokens=show_tokens,
-                               parser_debug=parser_debug)
+    parser_debug = {
+        "rules": False,
+        "transition": False,
+        "reduce": show_grammar,
+        "errorstack": None,
+        "context": False,
+        "dups": True,
+    }
+    parsed = parse_range(string, show_tokens=show_tokens, parser_debug=parser_debug)
     if show_ast:
         print(parsed)
-    assert parsed == 'range_start'
+    assert parsed == "range_start"
     walker = LocationGrok(string)
     walker.traverse(parsed)
     list_range = walker.result
     return list_range
 
+
 def build_location(string, show_tokens=False, show_ast=False, show_grammar=False):
-    parser_debug = {'rules': False, 'transition': False,
-                    'reduce': show_grammar,
-                    'errorstack': None,
-                    'context': False, 'dups': True
-                        }
-    parsed = parse_location("location", string, show_tokens=show_tokens,
-                            parser_debug=parser_debug)
+    parser_debug = {
+        "rules": False,
+        "transition": False,
+        "reduce": show_grammar,
+        "errorstack": None,
+        "context": False,
+        "dups": True,
+    }
+    parsed = parse_location(
+        "location", string, show_tokens=show_tokens, parser_debug=parser_debug
+    )
     if show_ast:
         print(parsed)
-    assert parsed == 'location'
+    assert parsed == "location"
     walker = LocationGrok(string)
     walker.traverse(parsed)
     return walker.result
 
+
 # FIXME: DRY with build_range
 def build_arange(string, show_tokens=False, show_ast=False, show_grammar=False):
-    parser_debug = {'rules': False, 'transition': False,
-                    'reduce': show_grammar,
-                    'errorstack': None,
-                    'context': True, 'dups': True
-                        }
-    parsed = parse_arange(string, show_tokens=show_tokens,
-                          parser_debug=parser_debug)
+    parser_debug = {
+        "rules": False,
+        "transition": False,
+        "reduce": show_grammar,
+        "errorstack": None,
+        "context": True,
+        "dups": True,
+    }
+    parsed = parse_arange(string, show_tokens=show_tokens, parser_debug=parser_debug)
     if show_ast:
         print(parsed)
-    assert parsed == 'arange_start'
+    assert parsed == "arange_start"
     walker = LocationGrok(string)
     walker.traverse(parsed)
     list_range = walker.result
     return list_range
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     # FIXME: make sure the below is in a test
     def doit(fn, line):
         print("=" * 30)
         print(line)
         print("+" * 30)
         try:
             result = fn(line)
```

### Comparing `trepan3k-1.2.8/trepan/processor/parse/tok.py` & `trepan3k-1.2.9/trepan/processor/parse/tok.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 class Token:
     """
     Class representing a token.
     kind: the kind of token, e.g. filename, number, other
     value: specific instance value, e.g. "/tmp/foo.c", or 5
     offset: byte offset from start of parse string
     """
+
     def __init__(self, kind, value=None, offset=None):
         self.offset = offset
         self.kind = kind
         self.value = value
 
     def __eq__(self, o):
-        """ '==', but it's okay if offset is different"""
+        """'==', but it's okay if offset is different"""
         if isinstance(o, Token):
             # Both are tokens: compare kind and value
             # It's okay if offsets are different
-            return (self.kind == o.kind)
+            return self.kind == o.kind
         else:
             return self.kind == o
 
     def __repr__(self):
         return str(self.kind)
 
-    def __repr1__(self, indent, sib_num=''):
+    def __repr1__(self, indent, sib_num=""):
         return self.format(line_prefix=indent, sib_num=sib_num)
 
     def __str__(self):
-        return self.format(line_prefix='')
+        return self.format(line_prefix="")
 
-    def format(self, line_prefix='', sib_num=None):
+    def format(self, line_prefix="", sib_num=None):
         if sib_num:
             sib_num = "%d." % sib_num
         else:
-            sib_num = ''
-        prefix = ('%s%s' % (line_prefix, sib_num))
-        offset_opname = '%5s %-10s' % (self.offset, self.kind)
+            sib_num = ""
+        prefix = "%s%s" % (line_prefix, sib_num)
+        offset_opname = "%5s %-10s" % (self.offset, self.kind)
         if not self.value:
             return "%s%s" % (prefix, offset_opname)
-        return "%s%s %s" % (prefix, offset_opname,  self.value)
+        return "%s%s %s" % (prefix, offset_opname, self.value)
 
     def __hash__(self):
         return hash(self.kind)
 
     def __getitem__(self, i):
         raise IndexError
```

### Comparing `trepan3k-1.2.8/trepan/processor/subcmd.py` & `trepan3k-1.2.9/trepan/processor/subcmd.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2006-2010, 2013-2015 Rocky Bernstein
+#
+#   Copyright (C) 2006-2010, 2013-2015, 2023 Rocky Bernstein
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
@@ -13,43 +14,46 @@
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Handles gdb-like subcommand processing."""
 
 
 class Subcmd:
-    """Gdb-like subcommand handling """
+    """Gdb-like subcommand handling"""
+
     def __init__(self, name, cmd_obj):
-        self.name    = name
+        self.name = name
         self.cmd_obj = cmd_obj
         self.subcmds = {}
         self.cmdlist = []
         return
 
     def lookup(self, subcmd_prefix):
         """Find subcmd in self.subcmds"""
         for subcmd_name in list(self.subcmds.keys()):
-            if subcmd_name.startswith(subcmd_prefix) \
-               and len(subcmd_prefix) >= \
-               self.subcmds[subcmd_name].__class__.min_abbrev:
+            if (
+                subcmd_name.startswith(subcmd_prefix)
+                and len(subcmd_prefix) >= self.subcmds[subcmd_name].__class__.min_abbrev
+            ):
                 return self.subcmds[subcmd_name]
             pass
         return None
 
     def short_help(self, subcmd_cb, subcmd_name, label=False):
         """Show short help for a subcommand."""
         entry = self.lookup(subcmd_name)
         if entry:
             if label:
                 prefix = entry.name
             else:
-                prefix = ''
+                prefix = ""
                 pass
-            if hasattr(entry, 'short_help'):
-                if prefix: prefix += ' -- '
+            if hasattr(entry, "short_help"):
+                if prefix:
+                    prefix += " -- "
                 self.cmd_obj.msg(prefix + entry.short_help)
                 pass
             pass
         else:
             self.undefined_subcmd("help", subcmd_name)
             pass
         return
@@ -66,107 +70,122 @@
         subcmd_name = subcmd_cb.name
         self.subcmds[subcmd_name] = subcmd_cb
 
         # We keep a list of subcommands to assist command completion
         self.cmdlist.append(subcmd_name)
 
     def run(self, subcmd_name, arg):
-        """Run subcmd_name with args using obj for the environent"""
-        entry=self.lookup(subcmd_name)
+        """Run subcmd_name with args using obj for the environment"""
+        entry = self.lookup(subcmd_name)
         if entry:
-            entry['callback'](arg)
+            entry["callback"](arg)
         else:
             self.cmdproc.undefined_cmd(entry.__class__.name, subcmd_name)
             pass
         return
 
     # Note: format of help is compatible with ddd.
     def help(self, *args):
         """help for subcommands."""
 
         print(args)
         subcmd_prefix = args[0]
         if not subcmd_prefix or len(subcmd_prefix) == 0:
             self.msg(self.doc)
-            self.msg("""
+            self.msg(
+                """
 List of %s subcommands:
-""" % (self.name))
+"""
+                % (self.name)
+            )
             for subcmd_name in self.list():
                 self._subcmd_helper(subcmd_name, self, True, True)
             return
 
         entry = self.lookup(subcmd_prefix)
-        if entry and hasattr(entry, 'help'):
+        if entry and hasattr(entry, "help"):
             entry.help(args)
         else:
-            self.cmd_obj.errmsg("Unknown 'help %s' subcommand %s"
-                                % (self.name, subcmd_prefix))
+            self.cmd_obj.errmsg(
+                "Unknown 'help %s' subcommand %s" % (self.name, subcmd_prefix)
+            )
 
     def list(self):
-        l = list(self.subcmds.keys())
-        l.sort()
-        return l
+        sorted_keys = list(self.subcmds.keys())
+        sorted_keys.sort()
+        return sorted_keys
 
     def undefined_subcmd(self, cmd, subcmd):
         """Error message when a subcommand doesn't exist"""
-        self.cmd_obj.errmsg('Undefined "%s" command: "%s". Try "help".' %
-                         (cmd, subcmd,))
+        self.cmd_obj.errmsg(
+            'Undefined "%s" command: "%s". Try "help".'
+            % (
+                cmd,
+                subcmd,
+            )
+        )
         return
+
     pass
 
+
 # When invoked as main program, invoke the debugger on a script
-if __name__ == '__main__':
+if __name__ == "__main__":
 
-    from trepan.processor.command import mock as Mmock
-    from trepan.processor.command import base_cmd as Mbase_cmd
+    from trepan.processor.command import base_cmd as Mbase_cmd, mock as Mmock
 
     class TestCommand(Mbase_cmd.DebuggerCommand):
-        '''Doc string for testing'''
+        """Doc string for testing"""
 
-        category = 'data'
+        category = "data"
         min_args = 0
         max_args = 5
-        name = 'test'
+        name = "test"
 
         def __init__(self):
-            self.name  = 'test'
+            self.name = "test"
             return
 
-        def run(self, args): print('test command run')
+        def run(self, args):
+            print("test command run")
 
     class TestTestingSubcommand:
-        '''Doc string for test testing subcommand'''
+        """Doc string for test testing subcommand"""
 
         def __init__(self):
-            self.name  = 'testing'
+            self.name = "testing"
             return
 
-        short_help = 'This is short help for test testing'
+        short_help = "This is short help for test testing"
         min_abbrev = 4
-        in_list    = True
+        in_list = True
+
+        def run(self, args):
+            print("test testing run")
 
-        def run(self, args): print('test testing run')
         pass
 
     d = Mmock.MockDebugger()
-    testcmd    = TestCommand()
+    testcmd = TestCommand()
     testcmd.debugger = d
-    testcmd.proc     = d.core.processor
-    testcmdMgr = Subcmd('test', testcmd)
+    testcmd.proc = d.core.processor
+    testcmdMgr = Subcmd("test", testcmd)
     testsub = TestTestingSubcommand()
     testcmdMgr.add(testsub)
 
-    for prefix in ['tes', 'test', 'testing', 'testing1']:
+    for prefix in ["tes", "test", "testing", "testing1"]:
         x = testcmdMgr.lookup(prefix)
-        if x: print(x.name)
-        else: print('None')
+        if x:
+            print(x.name)
+        else:
+            print("None")
         pass
 
-    testcmdMgr.short_help(testcmd, 'testing')
-    testcmdMgr.short_help(testcmd, 'test', True)
-    testcmdMgr.short_help(testcmd, 'tes')
+    testcmdMgr.short_help(testcmd, "testing")
+    testcmdMgr.short_help(testcmd, "test", True)
+    testcmdMgr.short_help(testcmd, "tes")
     print(testcmdMgr.list())
     testsub2 = TestTestingSubcommand()
-    testsub2.name = 'foobar'
+    testsub2.name = "foobar"
     testcmdMgr.add(testsub2)
     print(testcmdMgr.list())
     pass
```

### Comparing `trepan3k-1.2.8/trepan/processor/trace.py` & `trepan3k-1.2.9/trepan/processor/trace.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2009, 2013-2014 Rocky Bernstein
+#   Copyright (C) 2009, 2013-2014, 2023 Rocky Bernstein
 #
 #    This program is free software; you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation; either version 2 of the License, or
 #    (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
@@ -14,41 +14,40 @@
 #    You should have received a copy of the GNU General Public License
 #    along with this program; if not, write to the Free Software
 #    Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
 #    02110-1301 USA.
 # 'Helper' function for Processor. Put here so we
 # can use this in a couple of processors.
 
-from tracer import EVENT2SHORT
-
 from trepan import vprocessor as Mprocessor
 
 
 class PrintProcessor(Mprocessor.Processor):
-    """ A processor that just prints out events as we see them. This
+    """A processor that just prints out events as we see them. This
     is suitable for example for line/call tracing. We assume that the
     caller is going to filter out which events it wants printed or
     whether it wants any printed at all.
     """
+
     def __init__(self, debugger, opts=None):
         Mprocessor.Processor.__init__(self, debugger)
         return
 
     def event_processor(self, frame, event, arg):
-        'A simple event processor that prints out events.'
+        "A simple event processor that prints out events."
         out = self.debugger.intf[-1].output
         lineno = frame.f_lineno
         filename = self.core.canonic_filename(frame)
         filename = self.core.filename(filename)
         if not out:
             print("%s - %s:%d" % (event, filename, lineno))
         else:
             out.write("%s - %s:%d" % (event, filename, lineno))
             if arg is not None:
-                out.writeline(', %s ' % repr(arg))
+                out.writeline(", %s " % repr(arg))
             else:
-                out.writeline('')
+                out.writeline("")
                 pass
             pass
         return self.event_processor
 
     pass
```

### Comparing `trepan3k-1.2.8/trepan/vprocessor.py` & `trepan3k-1.2.9/trepan/vprocessor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,80 @@
 # -*- coding: utf-8 -*-
-#   Copyright (C) 2008-2010, 2012-2013, 2015, 2020 Rocky Bernstein <rocky@gnu.org>
+#
+#   Copyright (C) 2008-2010, 2012-2013, 2015, 2020, 2023 Rocky
+#   Bernstein <rocky@gnu.org>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation, either version 3 of the License, or
 #   (at your option) any later version.
 #
 #   This program is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU General Public License for more details.
 #
 #   You should have received a copy of the GNU General Public License
 #   along with this program.  If not, see <http://www.gnu.org/licenses/>.
-NotImplementedMessage = "This method must be overriden in a subclass"
-
 from pygments.console import colorize
 
-__all__ = ['Processor']
+NotImplementedMessage = "This method must be overridden in a subclass"
+
+__all__ = ["Processor"]
 
 
 class Processor(object):
     """A processor is the thing that handles the events that come to
     the debugger.  It has it's own I/O mechanism and a way to handle
     the events.
     """
+
     def __init__(self, core_obj):
         self.core = core_obj
         self.debugger = core_obj.debugger
         return
 
     # Note for errmsg, msg, and msg_nocr we don't want to simply make
     # an assignment of method names like self.msg = self.intf.msg,
     # because we want to allow the interface (intf) to change
     # dynamically. That is, the value of self.debugger may change
-    # in the course of the program and if we made such an method assignemnt
+    # in the course of the program and if we made such an method assignment
     # we wouldn't pick up that change in our self.msg
     def errmsg(self, message, opts={}):
-        """ Convenience short-hand for self.intf[-1].errmsg """
-        if 'plain' != self.debugger.settings['highlight']:
-            message = colorize('standout', message)
+        """Convenience short-hand for self.intf[-1].errmsg"""
+        if "plain" != self.debugger.settings["highlight"]:
+            message = colorize("standout", message)
             pass
-        return(self.intf[-1].errmsg(message))
+        return self.intf[-1].errmsg(message)
 
     def msg(self, msg, opts={}):
-        """ Convenience short-hand for self.debugger.intf[-1].msg """
-        return(self.intf[-1].msg(msg))
+        """Convenience short-hand for self.debugger.intf[-1].msg"""
+        return self.intf[-1].msg(msg)
 
     def msg_nocr(self, msg, opts={}):
-        """ Convenience short-hand for self.debugger.intf[-1].msg_nocr """
-        return(self.intf[-1].msg_nocr(msg))
+        """Convenience short-hand for self.debugger.intf[-1].msg_nocr"""
+        return self.intf[-1].msg_nocr(msg)
 
     def event_processor(self, frame, event, arg):
         raise NotImplementedError(NotImplementedMessage)
 
     def rst_msg(self, text, opts={}):
         """Convert ReStructuredText and run through msg()"""
         from trepan.lib.format import rst_text
-        text = rst_text(text,
-                        'plain' == self.debugger.settings['highlight'],
-                        self.debugger.settings['width'])
+
+        text = rst_text(
+            text,
+            "plain" == self.debugger.settings["highlight"],
+            self.debugger.settings["width"],
+        )
         return self.msg(text)
 
     def section(self, message, opts={}):
-        if 'plain' != self.settings('highlight'):
-            message = colorize('bold', message)
+        if "plain" != self.settings("highlight"):
+            message = colorize("bold", message)
             pass
         return self.msg(message, opts)
 
     def settings(self, setting):
         return self.core.debugger.settings[setting]
+
     pass
```

### Comparing `trepan3k-1.2.8/trepan3k.egg-info/PKG-INFO` & `trepan3k-1.2.9/trepan3k.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,342 +1,344 @@
 Metadata-Version: 2.1
 Name: trepan3k
-Version: 1.2.8
+Version: 1.2.9
 Summary: GDB-like Python Debugger in the Trepan family
 Home-page: http://github.com/rocky/python3-trepan/
 Author: Rocky Bernstein
 Author-email: rocky@gnu.org
 License: GPL3
-Description: |TravisCI| |CircleCI| |Pypi Installs| |license| |Supported Python Versions|
-        
-        |packagestatus|
-        
-        .. contents:: :local:
-        
-        Abstract
-        ========
-        
-        This is a gdb-like debugger for Python. It is a rewrite of *pdb* from
-        the ground up. It is both a high-level debugger as well as a
-        lower-level bytecode debugger. By lower-level debugger, I mean that it
-        understands a lot about byte code and will try to make use of that in
-        its normal higher-level instructions.
-        
-        A command-line interface (CLI) is provided as well as an remote access
-        interface over TCP/IP.
-        
-        See the Tutorial_ for how to use. See ipython-trepan_ for using this
-        in *ipython* or an *ipython notebook*.
-        
-        This package is for Python 3.2 and above. See trepan2_ for the same code
-        modified to work with Python 2.
-        
-        Features
-        ========
-        
-        Since this debugger is similar to other_ trepanning_ debuggers_ and *gdb*
-        in general, knowledge gained by learning this is transferable to those
-        debuggers and vice versa.
-        
-        There's a lot of cool stuff here that's not in the stock
-        Python debugger *pdb*, or in any other Python debugger that I know about.
-        
-        
-        More Exact location information
-        -------------------------------
-        
-        Python reports line information on the granularity of a line. To get
-        more precise information, we can (de)parse into Python the byte code
-        around a bytecode offset such as the place you are stopped at.
-        
-        So far as I know, there is no other debugger that decompile code at runtime.
-        
-        See the deparse_ command for details.
-        
-        We use information in the line number table in byte to understand
-        which lines are breakpointable, and in which module or function the
-        line appears in. Use info_line_ to see this information.
-        
-        In the future we may allow specifiying an offset to indicate which
-        offset to stop at when there are several choices for a given line
-        number.
-        
-        
-        Debugging Python bytecode (no source available)
-        -----------------------------------------------
-        
-        You can pass the debugger the name of Python bytecode and many times,
-        the debugger will merrily proceed.  This debugger tries very hard find
-        the source code. Either by using the current executable search path
-        (e.g. ``PATH``) or for some by looking inside the bytecode for a
-        filename in the main code object (``co_filename``) and applying that
-        with a search path which takes into account directory where the
-        bytecode lives.
-        
-        Failing to find source code this way, and in other situations where
-        source code can't be found, the debugger will decompile the bytecode
-        and use that for showing source test. *This allows us to debug `eval`'d
-        or `exec''d code.*
-        
-        But if you happen to know where the source code is located, you can
-        associate a file source code with the current name listed in the
-        bytecode. See the set_substitute_ command for details here.
-        
-        Source-code Syntax Colorization
-        -------------------------------
-        
-        Terminal source code is colorized via pygments_ . And with that you
-        can set the pygments color style, e.g. "colorful", "paraiso-dark". See
-        set_style_ . Furthermore, we make use of terminal bold and emphasized
-        text in debugger output and help text. Of course, you can also turn
-        this off. You can use your own
-        pygments_style_, provided you have a terminal that supports 256
-        colors. If your terminal supports the basic ANSI color sequences only,
-        we support that too in both dark and light themes.
-        
-        
-        Command Completion
-        ------------------
-        
-        GNU readline command completion is available. Command completion is
-        not just a simple static list, but varies depending on the
-        context. For example, for frame-changing commands which take optional
-        numbers, on the list of *valid numbers* is considered.
-        
-        Terminal Handling
-        -----------------
-        
-        We can adjust debugger output depending on the line width of your
-        terminal. If it changes, or you want to adjust it, see set_width_ .
-        
-        Smart Eval
-        ----------
-        
-        If you want to evaluate the current source line before it is run in
-        the code, use ``eval``. To evaluate text of a common fragment of line,
-        such as the expression part of an *if* statement, you can do that with
-        ``eval?``. See eval_ for more information.
-        
-        Function Breakpoints
-        ---------------------
-        
-        Many Python debuggers only allow setting a breakpoint at a line event
-        and functions are treated like line numbers. But functions and lines
-        are fundamentally different. If I write::
-        
-             def five(): return 5
-        
-        this line means has three different kinds of things. First there is
-        the code in Python that defines function ``five()`` for the first
-        time. Then there is the function itself, and then there is some code
-        inside that function.
-        
-        In this debugger, you can give the name of a *function* by surrounding
-        adding ``()`` at the end::
-        
-            break five()
-        
-        Also ``five`` could be a method of an object that is currently defined when the
-        ``breakpoint`` command is given::
-        
-            self.five()
-        
-        More Stepping Control
-        ---------------------
-        
-        Sometimes you want small steps, and sometimes large stepping.
-        
-        This fundamental issue is handled in a couple ways:
-        
-        Step Granularity
-        ................
-        
-        There are now ``step`` *event* and ``next`` *event* commands with
-        aliases to ``s+``, ``s>`` and so on. The plus-suffixed commands force
-        a different line on a subsequent stop, the dash-suffixed commands
-        don't.  Suffixes ``>``, ``<``, and ``!`` specify ``call``, ``return``
-        and ``exception`` events respectively. And without a suffix you get
-        the default; this is set by the ``set different`` command.
-        
-        Event Filtering and Tracing
-        ...........................
-        
-        By default the debugger stops at every event: ``call``, ``return``,
-        ``line``, ``exception``, ``c-call``, ``c-exception``. If you just want
-        to stop at ``line`` events (which is largely what you happens in
-        *pdb*) you can. If however you just want to stop at calls and returns,
-        that's possible too. Or pick some combination.
-        
-        In conjunction with handling *all* events by default, the event status is shown when stopped. The reason for stopping is also available via ``info program``.
-        
-        Event Tracing of Calls and Returns
-        ----------------------------------
-        
-        I'm not sure why this was not done before. Probably because of the
-        lack of the ability to set and move by different granularities,
-        tracing calls and returns lead to too many uninteresting stops (such
-        as at the same place you just were at). Also, stopping on function
-        definitions probably also added to this tedium.
-        
-        Because we're really handling return events, we can show you the return value. (*pdb* has an "undocumented" *retval* command that doesn't seem to work.)
-        
-        Debugger Macros via Python Lambda expressions
-        ---------------------------------------------
-        
-        There are debugger macros.  In *gdb*, there is a *macro* debugger
-        command to extend debugger commands.
-        
-        However Python has its own rich programming language so it seems silly
-        to recreate the macro language that is in *gdb*. Simpler and more
-        powerful is just to use Python here. A debugger macro here is just a
-        lambda expression which returns a string or a list of strings. Each
-        string returned should be a debugger command.
-        
-        We also have *aliases* for the extremely simple situation where you
-        want to give an alias to an existing debugger command. But beware:
-        some commands, like step_ inspect command suffixes and change their
-        behavior accordingly.
-        
-        We also envision a number of other ways to allow extension of this
-        debugger either through additional modules, or user-supplied debugger
-        command directories.
-        
-        Byte-code Instruction Introspection
-        ------------------------------------
-        
-        We do more in the way of looking at the byte codes to give better information. Through this we can provide:
-        
-        * a *skip* command. It is like the *jump* command, but you don't have
-          to deal with line numbers.
-        * disassembly of code fragments. You can now disassemble relative to
-          the stack frames you are currently stopped at.
-        * Better interpretation of where you are when inside *execfile* or
-          *exec*. (But really though this is probably a Python compiler
-          misfeature.)
-        * Check that breakpoints are set only where they make sense.
-        * A more accurate determination of if you are at a function-defining
-          *def* or *class* statements (because the caller instruction contains
-          ``MAKE_FUNCTION`` or ``BUILD_CLASS``.)
-        
-        Even without "deparsing" mentioned above, the ability to disassemble
-        where the PC is currently located (see `info pc <info_pc>`_), by line
-        number range or byte-offset range lets you tell exactly where you are
-        and code is getting run.
-        
-        Some Debugger Command Arguments can be Variables and Expressions
-        ----------------------------------------------------------------
-        
-        Commands that take integer arguments like *up*, *list*, or
-        *disassemble* allow you to use a Python expression which may include
-        local or global variables that evaluates to an integer. This
-        eliminates the need in *gdb* for special "dollar" debugger
-        variables. (Note however because of *shlex* parsing, expressions can't
-        have embedded blanks.)
-        
-        Out-of-Process Debugging
-        ------------------------
-        
-        You can now debug your program in a different process or even a different computer on a different network!
-        
-        Related, is flexible support for remapping path names from file
-        system, e.g. that inside a docker container or on a remote filesystem
-        with locally-installed files. See subst_ for more information.
-        
-        Egg, Wheel, and Tarballs
-        ------------------------
-        
-        Can be installed via the usual *pip* or *easy_install*. There is a
-        source tarball. `How To Install
-        <https://python3-trepan.readthedocs.io/en/latest/install.html>`_ has
-        full instructions and installing from git and by other means.
-        
-        Modularity
-        ----------
-        
-        The Debugger plays nice with other trace hooks. You can have several debugger objects.
-        
-        Many of the things listed below doesn't directly effect end-users, but
-        it does eventually by way of more robust and featureful code. And
-        keeping developers happy is a good thing.(TM)
-        
-        * Commands and subcommands are individual classes now, not methods in a class. This means they now have properties like the context in which they can be run, minimum abbreviation name or alias names. To add a new command you basically add a file in a directory.
-        * I/O is it's own layer. This simplifies interactive readline behavior from reading commands over a TCP socket.
-        * An interface is it's own layer. Local debugging, remote debugging, running debugger commands from a file (``source``) are different interfaces. This means, for example, that we are able to give better error reporting if a debugger command file has an error.
-        * There is an experimental Python-friendly interface for front-ends
-        * more testable. Much more unit and functional tests. More of *pydb*'s integration test will eventually be added.
-        
-        Documentation
-        -------------
-        
-        Documentation: http://python3-trepan.readthedocs.org
-        
-        See Also
-        --------
-        
-        * trepan2_ : trepan debugger for Python 2
-        * trepanxpy_ : trepan debugger for `x-python <https://pypi.python.org/pypi/x-python>`_, the bytecode interpreter written in Python
-        * pydbgr_  : previous incarnation of the Python 2 debugger
-        * pydb_ : even older incarnation of debugger (for very old Python 2)
-        * Tutorial_: Tutorial for how to use
-        * https://github.com/rocky/trepan-xpy : Python debugger using this code to support `x-python <https://pypi.python.org/pypi/x-python>`_
-        * https://pypi.python.org/pypi/uncompyle6 : Python decompiler
-        * https://pypi.python.org/pypi/decompyle3 : Python 3.7 and 3.8 decompiler
-        * https://pypi.python.org/pypi/xdis : cross-platform disassembler
-        
-        
-        .. _pygments:  http://pygments.org
-        .. _pygments_style:  http://pygments.org/docs/styles/
-        .. _howtoinstall: https://github.com/rocky/python3-trepan/wiki/How-to-Install
-        .. _pydb:  http://bashdb.sf.net/pydb
-        .. _pydbgr: https://pypi.python.org/pypi/pydbgr
-        .. _trepan2: https://pypi.python.org/pypi/trepan2
-        .. _trepan3: https://github.com/rocky/python3-trepan
-        .. _trepanxpy: https://pypi.python.org/pypi/trepanxpy
-        .. _other: https://repology.org/project/zshdb/versions
-        .. _trepanning: https://rubygems.org/gems/trepanning
-        .. _debuggers: https://metacpan.org/pod/Devel::Trepan
-        .. _this: http://bashdb.sourceforge.net/pydb/features.html
-        .. _Tutorial: http://python2-trepan.readthedocs.io/en/latest/entry-exit.html
-        .. |downloads| image:: https://img.shields.io/pypi/dd/trepan3k.svg
-           :target: https://pypi.python.org/pypi/trepan3k/
-        .. |TravisCI| image:: https://api.travis-ci.org/rocky/python3-trepan.svg
-           :target: https://travis-ci.org/rocky/python3-trepan
-        .. |CircleCI| image:: https://circleci.com/gh/rocky/python3-trepan.svg?style=svg
-           :target: https://circleci.com/gh/rocky/python3-trepan
-        .. _ipython-trepan: https://github.com/rocky/ipython-trepan
-        .. |license| image:: https://img.shields.io/pypi/l/trepan.svg
-            :target: https://pypi.python.org/pypi/trepan3k
-            :alt: License
-        .. _deparse:  https://python3-trepan.readthedocs.io/en/latest/commands/data/deparse.html
-        .. _info_line:  https://python3-trepan.readthedocs.io/en/latest/commands/info/line.html
-        .. _set_style:  https://python3-trepan.readthedocs.org/en/latest/commands/set/style.html
-        .. _set_substitute:  https://python3-trepan.readthedocs.org/en/latest/commands/set/substitute.html
-        .. _set_width:  https://python3-trepan.readthedocs.org/en/latest/commands/set/width.html
-        .. _eval: https://python3-trepan.readthedocs.org/en/latest/commands/data/eval.html
-        .. _step: https://python3-trepan.readthedocs.org/en/latest/commands/running/step.html
-        .. _subst: https://python3-trepan.readthedocs.io/en/latest/commands/set/substitute.html
-        .. _install: http://python3-trepan.readthedocs.org/en/latest/install.html
-        .. |Supported Python Versions| image:: https://img.shields.io/pypi/pyversions/trepan3k.svg
-           :target: https://pypi.python.org/pypi/trepan3k/
-        .. |Pypi Installs| image:: https://pepy.tech/badge/trepan3k
-        .. |packagestatus| image:: https://repology.org/badge/vertical-allrepos/python:trepan3k.svg
-        		 :target: https://repology.org/project/python:trepan3k/versions
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5 
-Classifier: Programming Language :: Python :: 3.6 
-Classifier: Programming Language :: Python :: 3.7 
-Classifier: Programming Language :: Python :: 3.8 
-Classifier: Programming Language :: Python :: 3.9 
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/x-rst
+License-File: COPYING
+
+|CircleCI| |Pypi Installs| |license| |Supported Python Versions|
+
+|packagestatus|
+
+.. contents:: :local:
+
+Abstract
+========
+
+This is a gdb-like debugger for Python. It is a rewrite of *pdb* from
+the ground up. It is both a high-level debugger as well as a
+lower-level bytecode debugger. By lower-level debugger, I mean that it
+understands a lot about byte code and will try to make use of that in
+its normal higher-level instructions.
+
+A command-line interface (CLI) is provided as well as an remote access
+interface over TCP/IP.
+
+See the Tutorial_ for how to use. See ipython-trepan_ for using this
+in *ipython* or an *ipython notebook*.
+
+This package is for Python 3.2 and above. See trepan2_ for the same code
+modified to work with Python 2.
+
+Features
+========
+
+Since this debugger is similar to other_ trepanning_ debuggers_ and *gdb*
+in general, knowledge gained by learning this is transferable to those
+debuggers and vice versa.
+
+There's a lot of cool stuff here that's not in the stock
+Python debugger *pdb*, or in any other Python debugger that I know about.
+
+
+More Exact location information
+-------------------------------
+
+Python reports line information on the granularity of a line. To get
+more precise information, we can (de)parse into Python the byte code
+around a bytecode offset such as the place you are stopped at.
+
+So far as I know, there is no other debugger that decompile code at runtime.
+
+See the deparse_ command for details.
+
+We use information in the line number table in byte to understand
+which lines are breakpointable, and in which module or function the
+line appears in. Use info_line_ to see this information.
+
+In the future we may allow specifiying an offset to indicate which
+offset to stop at when there are several choices for a given line
+number.
+
+
+Debugging Python bytecode (no source available)
+-----------------------------------------------
+
+You can pass the debugger the name of Python bytecode and many times,
+the debugger will merrily proceed.  This debugger tries very hard find
+the source code. Either by using the current executable search path
+(e.g. ``PATH``) or for some by looking inside the bytecode for a
+filename in the main code object (``co_filename``) and applying that
+with a search path which takes into account directory where the
+bytecode lives.
+
+Failing to find source code this way, and in other situations where
+source code can't be found, the debugger will decompile the bytecode
+and use that for showing source test. *This allows us to debug `eval`'d
+or `exec''d code.*
+
+But if you happen to know where the source code is located, you can
+associate a file source code with the current name listed in the
+bytecode. See the set_substitute_ command for details here.
+
+Source-code Syntax Colorization
+-------------------------------
+
+Terminal source code is colorized via pygments_ . And with that you
+can set the pygments color style, e.g. "colorful", "paraiso-dark". See
+set_style_ . Furthermore, we make use of terminal bold and emphasized
+text in debugger output and help text. Of course, you can also turn
+this off. You can use your own
+pygments_style_, provided you have a terminal that supports 256
+colors. If your terminal supports the basic ANSI color sequences only,
+we support that too in both dark and light themes.
+
+
+Command Completion
+------------------
+
+GNU readline command completion is available. Command completion is
+not just a simple static list, but varies depending on the
+context. For example, for frame-changing commands which take optional
+numbers, on the list of *valid numbers* is considered.
+
+Terminal Handling
+-----------------
+
+We can adjust debugger output depending on the line width of your
+terminal. If it changes, or you want to adjust it, see set_width_ .
+
+Smart Eval
+----------
+
+If you want to evaluate the current source line before it is run in
+the code, use ``eval``. To evaluate text of a common fragment of line,
+such as the expression part of an *if* statement, you can do that with
+``eval?``. See eval_ for more information.
+
+Function Breakpoints
+---------------------
+
+Many Python debuggers only allow setting a breakpoint at a line event
+and functions are treated like line numbers. But functions and lines
+are fundamentally different. If I write::
+
+     def five(): return 5
+
+this line means has three different kinds of things. First there is
+the code in Python that defines function ``five()`` for the first
+time. Then there is the function itself, and then there is some code
+inside that function.
+
+In this debugger, you can give the name of a *function* by surrounding
+adding ``()`` at the end::
+
+    break five()
+
+Also ``five`` could be a method of an object that is currently defined when the
+``breakpoint`` command is given::
+
+    self.five()
+
+More Stepping Control
+---------------------
+
+Sometimes you want small steps, and sometimes large stepping.
+
+This fundamental issue is handled in a couple ways:
+
+Step Granularity
+................
+
+There are now ``step`` *event* and ``next`` *event* commands with
+aliases to ``s+``, ``s>`` and so on. The plus-suffixed commands force
+a different line on a subsequent stop, the dash-suffixed commands
+don't.  Suffixes ``>``, ``<``, and ``!`` specify ``call``, ``return``
+and ``exception`` events respectively. And without a suffix you get
+the default; this is set by the ``set different`` command.
+
+Event Filtering and Tracing
+...........................
+
+By default the debugger stops at every event: ``call``, ``return``,
+``line``, ``exception``, ``c-call``, ``c-exception``. If you just want
+to stop at ``line`` events (which is largely what you happens in
+*pdb*) you can. If however you just want to stop at calls and returns,
+that's possible too. Or pick some combination.
+
+In conjunction with handling *all* events by default, the event status is shown when stopped. The reason for stopping is also available via ``info program``.
+
+Event Tracing of Calls and Returns
+----------------------------------
+
+I'm not sure why this was not done before. Probably because of the
+lack of the ability to set and move by different granularities,
+tracing calls and returns lead to too many uninteresting stops (such
+as at the same place you just were at). Also, stopping on function
+definitions probably also added to this tedium.
+
+Because we're really handling return events, we can show you the return value. (*pdb* has an "undocumented" *retval* command that doesn't seem to work.)
+
+Debugger Macros via Python Lambda expressions
+---------------------------------------------
+
+There are debugger macros.  In *gdb*, there is a *macro* debugger
+command to extend debugger commands.
+
+However Python has its own rich programming language so it seems silly
+to recreate the macro language that is in *gdb*. Simpler and more
+powerful is just to use Python here. A debugger macro here is just a
+lambda expression which returns a string or a list of strings. Each
+string returned should be a debugger command.
+
+We also have *aliases* for the extremely simple situation where you
+want to give an alias to an existing debugger command. But beware:
+some commands, like step_ inspect command suffixes and change their
+behavior accordingly.
+
+We also envision a number of other ways to allow extension of this
+debugger either through additional modules, or user-supplied debugger
+command directories.
+
+Byte-code Instruction Introspection
+------------------------------------
+
+We do more in the way of looking at the byte codes to give better information. Through this we can provide:
+
+* a *skip* command. It is like the *jump* command, but you don't have
+  to deal with line numbers.
+* disassembly of code fragments. You can now disassemble relative to
+  the stack frames you are currently stopped at.
+* Better interpretation of where you are when inside *execfile* or
+  *exec*. (But really though this is probably a Python compiler
+  misfeature.)
+* Check that breakpoints are set only where they make sense.
+* A more accurate determination of if you are at a function-defining
+  *def* or *class* statements (because the caller instruction contains
+  ``MAKE_FUNCTION`` or ``BUILD_CLASS``.)
+
+Even without "deparsing" mentioned above, the ability to disassemble
+where the PC is currently located (see `info pc <info_pc>`_), by line
+number range or byte-offset range lets you tell exactly where you are
+and code is getting run.
+
+Some Debugger Command Arguments can be Variables and Expressions
+----------------------------------------------------------------
+
+Commands that take integer arguments like *up*, *list*, or
+*disassemble* allow you to use a Python expression which may include
+local or global variables that evaluates to an integer. This
+eliminates the need in *gdb* for special "dollar" debugger
+variables. (Note however because of *shlex* parsing, expressions can't
+have embedded blanks.)
+
+Out-of-Process Debugging
+------------------------
+
+You can now debug your program in a different process or even a different computer on a different network!
+
+Related, is flexible support for remapping path names from file
+system, e.g. that inside a docker container or on a remote filesystem
+with locally-installed files. See subst_ for more information.
+
+Egg, Wheel, and Tarballs
+------------------------
+
+Can be installed via the usual *pip* or *easy_install*. There is a
+source tarball. `How To Install
+<https://python3-trepan.readthedocs.io/en/latest/install.html>`_ has
+full instructions and installing from git and by other means.
+
+Modularity
+----------
+
+The Debugger plays nice with other trace hooks. You can have several debugger objects.
+
+Many of the things listed below doesn't directly effect end-users, but
+it does eventually by way of more robust and featureful code. And
+keeping developers happy is a good thing.(TM)
+
+* Commands and subcommands are individual classes now, not methods in a class. This means they now have properties like the context in which they can be run, minimum abbreviation name or alias names. To add a new command you basically add a file in a directory.
+* I/O is it's own layer. This simplifies interactive readline behavior from reading commands over a TCP socket.
+* An interface is it's own layer. Local debugging, remote debugging, running debugger commands from a file (``source``) are different interfaces. This means, for example, that we are able to give better error reporting if a debugger command file has an error.
+* There is an experimental Python-friendly interface for front-ends
+* more testable. Much more unit and functional tests. More of *pydb*'s integration test will eventually be added.
+
+Documentation
+-------------
+
+Documentation: http://python3-trepan.readthedocs.org
+
+See Also
+--------
+
+* trepan2_ : trepan debugger for Python 2
+* trepanxpy_ : trepan debugger for `x-python <https://pypi.python.org/pypi/x-python>`_, the bytecode interpreter written in Python
+* pydbgr_  : previous incarnation of the Python 2 debugger
+* pydb_ : even older incarnation of debugger (for very old Python 2)
+* Tutorial_: Tutorial for how to use
+* https://github.com/rocky/trepan-xpy : Python debugger using this code to support `x-python <https://pypi.python.org/pypi/x-python>`_
+* https://pypi.python.org/pypi/uncompyle6 : Python decompiler
+* https://pypi.python.org/pypi/decompyle3 : Python 3.7 and 3.8 decompiler
+* https://pypi.python.org/pypi/xdis : cross-platform disassembler
+
+
+.. _pygments:  http://pygments.org
+.. _pygments_style:  http://pygments.org/docs/styles/
+.. _howtoinstall: https://github.com/rocky/python3-trepan/wiki/How-to-Install
+.. _pydb:  http://bashdb.sf.net/pydb
+.. _pydbgr: https://pypi.python.org/pypi/pydbgr
+.. _trepan2: https://pypi.python.org/pypi/trepan2
+.. _trepan3: https://github.com/rocky/python3-trepan
+.. _trepanxpy: https://pypi.python.org/pypi/trepanxpy
+.. _other: https://repology.org/project/zshdb/versions
+.. _trepanning: https://rubygems.org/gems/trepanning
+.. _debuggers: https://metacpan.org/pod/Devel::Trepan
+.. _this: http://bashdb.sourceforge.net/pydb/features.html
+.. _Tutorial: http://python2-trepan.readthedocs.io/en/latest/entry-exit.html
+.. |downloads| image:: https://img.shields.io/pypi/dd/trepan3k.svg
+   :target: https://pypi.python.org/pypi/trepan3k/
+.. |TravisCI| image:: https://api.travis-ci.org/rocky/python3-trepan.svg
+   :target: https://travis-ci.org/rocky/python3-trepan
+.. |CircleCI| image:: https://circleci.com/gh/rocky/python3-trepan.svg?style=svg
+   :target: https://circleci.com/gh/rocky/python3-trepan
+.. _ipython-trepan: https://github.com/rocky/ipython-trepan
+.. |license| image:: https://img.shields.io/pypi/l/trepan.svg
+    :target: https://pypi.python.org/pypi/trepan3k
+    :alt: License
+.. _deparse:  https://python3-trepan.readthedocs.io/en/latest/commands/data/deparse.html
+.. _info_line:  https://python3-trepan.readthedocs.io/en/latest/commands/info/line.html
+.. _set_style:  https://python3-trepan.readthedocs.org/en/latest/commands/set/style.html
+.. _set_substitute:  https://python3-trepan.readthedocs.org/en/latest/commands/set/substitute.html
+.. _set_width:  https://python3-trepan.readthedocs.org/en/latest/commands/set/width.html
+.. _eval: https://python3-trepan.readthedocs.org/en/latest/commands/data/eval.html
+.. _step: https://python3-trepan.readthedocs.org/en/latest/commands/running/step.html
+.. _subst: https://python3-trepan.readthedocs.io/en/latest/commands/set/substitute.html
+.. _install: http://python3-trepan.readthedocs.org/en/latest/install.html
+.. |Supported Python Versions| image:: https://img.shields.io/pypi/pyversions/trepan3k.svg
+   :target: https://pypi.python.org/pypi/trepan3k/
+.. |Pypi Installs| image:: https://pepy.tech/badge/trepan3k
+.. |packagestatus| image:: https://repology.org/badge/vertical-allrepos/python:trepan3k.svg
+		 :target: https://repology.org/project/python:trepan3k/versions
+
```

### Comparing `trepan3k-1.2.8/trepan3k.egg-info/SOURCES.txt` & `trepan3k-1.2.9/trepan3k.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -366,14 +366,15 @@
 trepan/processor/command/show_subcmd/autopython.py
 trepan/processor/command/show_subcmd/basename.py
 trepan/processor/command/show_subcmd/confirm.py
 trepan/processor/command/show_subcmd/dbg_trepan.py
 trepan/processor/command/show_subcmd/highlight.py
 trepan/processor/command/show_subcmd/listsize.py
 trepan/processor/command/show_subcmd/style.py
+trepan/processor/command/show_subcmd/substitute.py
 trepan/processor/command/show_subcmd/tempdir.py
 trepan/processor/parse/__init__.py
 trepan/processor/parse/parser.py
 trepan/processor/parse/scanner.py
 trepan/processor/parse/semantics.py
 trepan/processor/parse/tok.py
 trepan3k.egg-info/PKG-INFO
```

