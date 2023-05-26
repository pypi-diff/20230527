# Comparing `tmp/bfg9000-0.7.0.tar.gz` & `tmp/bfg9000-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfg9000-0.7.0.tar", last modified: Sun May 21 01:43:10 2023, max compression
+gzip compressed data, was "bfg9000-0.7.1.tar", last modified: Fri May 26 23:26:54 2023, max compression
```

## Comparing `bfg9000-0.7.0.tar` & `bfg9000-0.7.1.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.962722 bfg9000-0.7.0/
--rw-rw-r--   0 jim       (1000) jim       (1000)    14313 2023-05-21 01:42:08.000000 bfg9000-0.7.0/CHANGES.md
--rw-rw-r--   0 jim       (1000) jim       (1000)     1486 2023-01-03 04:51:05.000000 bfg9000-0.7.0/LICENSE
--rw-rw-r--   0 jim       (1000) jim       (1000)       19 2020-11-10 03:37:38.000000 bfg9000-0.7.0/MANIFEST.in
--rw-rw-r--   0 jim       (1000) jim       (1000)     4659 2023-05-21 01:43:10.962722 bfg9000-0.7.0/PKG-INFO
--rw-rw-r--   0 jim       (1000) jim       (1000)     3313 2023-03-25 21:38:18.000000 bfg9000-0.7.0/README.md
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.926722 bfg9000-0.7.0/bfg9000/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)       18 2023-05-21 01:41:50.000000 bfg9000-0.7.0/bfg9000/app_version.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.934722 bfg9000-0.7.0/bfg9000/arguments/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/arguments/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     4385 2021-09-26 20:58:29.000000 bfg9000-0.7.0/bfg9000/arguments/parser.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     6794 2021-08-04 20:26:41.000000 bfg9000-0.7.0/bfg9000/arguments/windows.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.934722 bfg9000-0.7.0/bfg9000/backends/
--rw-rw-r--   0 jim       (1000) jim       (1000)      517 2023-04-02 06:27:55.000000 bfg9000-0.7.0/bfg9000/backends/__init__.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.934722 bfg9000-0.7.0/bfg9000/backends/compdb/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2021-06-27 05:36:00.000000 bfg9000-0.7.0/bfg9000/backends/compdb/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2702 2021-06-14 02:40:53.000000 bfg9000-0.7.0/bfg9000/backends/compdb/writer.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.934722 bfg9000-0.7.0/bfg9000/backends/make/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/backends/make/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    14282 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/backends/make/syntax.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     3229 2020-12-31 22:29:46.000000 bfg9000-0.7.0/bfg9000/backends/make/writer.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.938722 bfg9000-0.7.0/bfg9000/backends/msbuild/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/backends/msbuild/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     5970 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/backends/msbuild/solution.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    14204 2022-03-02 21:04:35.000000 bfg9000-0.7.0/bfg9000/backends/msbuild/syntax.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1589 2021-12-31 21:55:46.000000 bfg9000-0.7.0/bfg9000/backends/msbuild/writer.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.938722 bfg9000-0.7.0/bfg9000/backends/ninja/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/backends/ninja/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    11419 2020-11-10 03:37:38.000000 bfg9000-0.7.0/bfg9000/backends/ninja/syntax.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2822 2020-12-31 22:29:46.000000 bfg9000-0.7.0/bfg9000/backends/ninja/writer.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     4005 2021-12-31 21:55:46.000000 bfg9000-0.7.0/bfg9000/build.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2568 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/build_inputs.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.946722 bfg9000-0.7.0/bfg9000/builtins/
--rw-rw-r--   0 jim       (1000) jim       (1000)      270 2020-11-19 04:05:52.000000 bfg9000-0.7.0/bfg9000/builtins/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1220 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/builtins/alias.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     6615 2020-08-05 21:45:09.000000 bfg9000-0.7.0/bfg9000/builtins/builtin.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      929 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/builtins/clean.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     7218 2021-06-14 02:40:53.000000 bfg9000-0.7.0/bfg9000/builtins/command.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    17356 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/builtins/compile.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     7283 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/builtins/copy_file.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1097 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/builtins/core.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2203 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/builtins/default.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1713 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/builtins/dist.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     5421 2021-07-12 04:00:01.000000 bfg9000-0.7.0/bfg9000/builtins/file_types.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     5986 2020-12-02 05:42:02.000000 bfg9000-0.7.0/bfg9000/builtins/find.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     7361 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/builtins/install.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    25468 2021-11-23 05:28:03.000000 bfg9000-0.7.0/bfg9000/builtins/link.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      277 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/builtins/opts.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2733 2021-09-27 18:18:11.000000 bfg9000-0.7.0/bfg9000/builtins/packages.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      993 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/builtins/path.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    18909 2022-09-04 21:45:52.000000 bfg9000-0.7.0/bfg9000/builtins/pkg_config.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      988 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/builtins/project.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2313 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/builtins/regenerate.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     4222 2021-11-23 05:28:03.000000 bfg9000-0.7.0/bfg9000/builtins/tests.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     3619 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/builtins/toolchain.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      306 2021-09-26 04:02:06.000000 bfg9000-0.7.0/bfg9000/builtins/user_arguments.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      791 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/builtins/version.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     3891 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/depfixer.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    16828 2023-01-14 04:23:13.000000 bfg9000-0.7.0/bfg9000/driver.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2524 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/e1m1.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    12905 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/environment.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      318 2020-12-02 05:42:02.000000 bfg9000-0.7.0/bfg9000/exceptions.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     9854 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/file_types.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     6999 2020-12-02 05:42:02.000000 bfg9000-0.7.0/bfg9000/glob.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     5778 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/iterutils.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2203 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/jvmoutput.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     4685 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/languages.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     7120 2021-12-31 21:55:46.000000 bfg9000-0.7.0/bfg9000/log.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2228 2020-11-21 00:01:55.000000 bfg9000-0.7.0/bfg9000/objutils.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     7750 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/options.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2420 2021-08-04 20:26:41.000000 bfg9000-0.7.0/bfg9000/packages.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2624 2021-12-31 21:55:46.000000 bfg9000-0.7.0/bfg9000/path.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.950722 bfg9000-0.7.0/bfg9000/platforms/
--rw-rw-r--   0 jim       (1000) jim       (1000)       75 2021-12-31 21:55:46.000000 bfg9000-0.7.0/bfg9000/platforms/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     9111 2022-09-04 21:45:52.000000 bfg9000-0.7.0/bfg9000/platforms/basepath.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     4512 2023-04-02 06:27:55.000000 bfg9000-0.7.0/bfg9000/platforms/core.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      648 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/platforms/cygwin.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      334 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/platforms/host.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2779 2022-09-03 05:36:28.000000 bfg9000-0.7.0/bfg9000/platforms/posix.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      340 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/platforms/target.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2039 2022-09-03 05:36:35.000000 bfg9000-0.7.0/bfg9000/platforms/windows.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1623 2021-11-23 05:28:03.000000 bfg9000-0.7.0/bfg9000/rccdep.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     6917 2020-11-10 03:37:38.000000 bfg9000-0.7.0/bfg9000/safe_str.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.950722 bfg9000-0.7.0/bfg9000/shell/
--rw-rw-r--   0 jim       (1000) jim       (1000)     3124 2021-12-31 21:55:46.000000 bfg9000-0.7.0/bfg9000/shell/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      615 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/shell/list.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     3835 2022-10-31 03:40:08.000000 bfg9000-0.7.0/bfg9000/shell/posix.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2475 2022-09-04 21:45:52.000000 bfg9000-0.7.0/bfg9000/shell/syntax.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     4838 2022-10-31 03:40:08.000000 bfg9000-0.7.0/bfg9000/shell/windows.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.958722 bfg9000-0.7.0/bfg9000/tools/
--rw-rw-r--   0 jim       (1000) jim       (1000)     1339 2020-11-19 04:05:52.000000 bfg9000-0.7.0/bfg9000/tools/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2685 2020-11-21 00:01:55.000000 bfg9000-0.7.0/bfg9000/tools/ar.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     4635 2021-01-02 22:53:27.000000 bfg9000-0.7.0/bfg9000/tools/c_family.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.962722 bfg9000-0.7.0/bfg9000/tools/cc/
--rw-rw-r--   0 jim       (1000) jim       (1000)     8222 2022-01-22 05:33:55.000000 bfg9000-0.7.0/bfg9000/tools/cc/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     5370 2021-09-27 18:18:11.000000 bfg9000-0.7.0/bfg9000/tools/cc/compiler.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      219 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/tools/cc/flags.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    16904 2021-07-12 05:24:44.000000 bfg9000-0.7.0/bfg9000/tools/cc/linker.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2571 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/tools/cc/rc.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     6537 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/tools/common.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1879 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/tools/copy_file.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1452 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/tools/doppel.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      530 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/tools/fortran.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1651 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/tools/install_name_tool.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1829 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/tools/internal.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      822 2021-12-31 21:55:46.000000 bfg9000-0.7.0/bfg9000/tools/java.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    12771 2021-09-27 18:18:11.000000 bfg9000-0.7.0/bfg9000/tools/jvm.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1614 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/tools/ld.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     3594 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/tools/lex.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      406 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/tools/mkdir_p.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     4739 2023-02-18 23:42:47.000000 bfg9000-0.7.0/bfg9000/tools/mopack.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.962722 bfg9000-0.7.0/bfg9000/tools/msvc/
--rw-rw-r--   0 jim       (1000) jim       (1000)     5468 2021-12-31 21:55:46.000000 bfg9000-0.7.0/bfg9000/tools/msvc/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     7289 2020-11-19 04:05:52.000000 bfg9000-0.7.0/bfg9000/tools/msvc/compiler.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     8683 2021-08-04 20:26:41.000000 bfg9000-0.7.0/bfg9000/tools/msvc/linker.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     3125 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/tools/msvc/rc.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2282 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/tools/patchelf.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    10396 2021-12-31 21:55:46.000000 bfg9000-0.7.0/bfg9000/tools/pkg_config.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     7250 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/tools/qt.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1848 2020-12-28 02:52:54.000000 bfg9000-0.7.0/bfg9000/tools/rc.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      455 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/tools/rm.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1408 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/tools/scripts.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      807 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/tools/setenv.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     4065 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/tools/yacc.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2800 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/versioning.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.930722 bfg9000-0.7.0/bfg9000.egg-info/
--rw-rw-r--   0 jim       (1000) jim       (1000)     4659 2023-05-21 01:43:10.000000 bfg9000-0.7.0/bfg9000.egg-info/PKG-INFO
--rw-rw-r--   0 jim       (1000) jim       (1000)     3025 2023-05-21 01:43:10.000000 bfg9000-0.7.0/bfg9000.egg-info/SOURCES.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)        1 2023-05-21 01:43:10.000000 bfg9000-0.7.0/bfg9000.egg-info/dependency_links.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)     1152 2023-05-21 01:43:10.000000 bfg9000-0.7.0/bfg9000.egg-info/entry_points.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)      321 2023-05-21 01:43:10.000000 bfg9000-0.7.0/bfg9000.egg-info/requires.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)        8 2023-05-21 01:43:10.000000 bfg9000-0.7.0/bfg9000.egg-info/top_level.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)      487 2023-05-21 01:43:10.962722 bfg9000-0.7.0/setup.cfg
--rw-rw-r--   0 jim       (1000) jim       (1000)     6838 2023-05-16 03:14:43.000000 bfg9000-0.7.0/setup.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-26 23:26:54.357266 bfg9000-0.7.1/
+-rw-rw-r--   0 jim       (1000) jim       (1000)    14550 2023-05-26 23:26:40.000000 bfg9000-0.7.1/CHANGES.md
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1486 2023-01-03 04:51:05.000000 bfg9000-0.7.1/LICENSE
+-rw-rw-r--   0 jim       (1000) jim       (1000)       19 2020-11-10 03:37:38.000000 bfg9000-0.7.1/MANIFEST.in
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4659 2023-05-26 23:26:54.357266 bfg9000-0.7.1/PKG-INFO
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3313 2023-03-25 21:38:18.000000 bfg9000-0.7.1/README.md
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-26 23:26:54.333266 bfg9000-0.7.1/bfg9000/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.7.1/bfg9000/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)       18 2023-05-26 23:26:40.000000 bfg9000-0.7.1/bfg9000/app_version.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-26 23:26:54.333266 bfg9000-0.7.1/bfg9000/arguments/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.7.1/bfg9000/arguments/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4385 2021-09-26 20:58:29.000000 bfg9000-0.7.1/bfg9000/arguments/parser.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     6794 2021-08-04 20:26:41.000000 bfg9000-0.7.1/bfg9000/arguments/windows.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-26 23:26:54.333266 bfg9000-0.7.1/bfg9000/backends/
+-rw-rw-r--   0 jim       (1000) jim       (1000)      517 2023-04-02 06:27:55.000000 bfg9000-0.7.1/bfg9000/backends/__init__.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-26 23:26:54.337266 bfg9000-0.7.1/bfg9000/backends/compdb/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2021-06-27 05:36:00.000000 bfg9000-0.7.1/bfg9000/backends/compdb/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2702 2021-06-14 02:40:53.000000 bfg9000-0.7.1/bfg9000/backends/compdb/writer.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-26 23:26:54.337266 bfg9000-0.7.1/bfg9000/backends/make/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.7.1/bfg9000/backends/make/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    14282 2020-09-07 06:23:31.000000 bfg9000-0.7.1/bfg9000/backends/make/syntax.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3229 2020-12-31 22:29:46.000000 bfg9000-0.7.1/bfg9000/backends/make/writer.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-26 23:26:54.337266 bfg9000-0.7.1/bfg9000/backends/msbuild/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.7.1/bfg9000/backends/msbuild/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     5970 2020-09-07 06:23:31.000000 bfg9000-0.7.1/bfg9000/backends/msbuild/solution.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    14204 2022-03-02 21:04:35.000000 bfg9000-0.7.1/bfg9000/backends/msbuild/syntax.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1589 2021-12-31 21:55:46.000000 bfg9000-0.7.1/bfg9000/backends/msbuild/writer.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-26 23:26:54.337266 bfg9000-0.7.1/bfg9000/backends/ninja/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.7.1/bfg9000/backends/ninja/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    11419 2020-11-10 03:37:38.000000 bfg9000-0.7.1/bfg9000/backends/ninja/syntax.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2822 2020-12-31 22:29:46.000000 bfg9000-0.7.1/bfg9000/backends/ninja/writer.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4005 2021-12-31 21:55:46.000000 bfg9000-0.7.1/bfg9000/build.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2568 2020-09-07 06:23:31.000000 bfg9000-0.7.1/bfg9000/build_inputs.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-26 23:26:54.345265 bfg9000-0.7.1/bfg9000/builtins/
+-rw-rw-r--   0 jim       (1000) jim       (1000)      270 2020-11-19 04:05:52.000000 bfg9000-0.7.1/bfg9000/builtins/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1220 2020-08-05 21:44:42.000000 bfg9000-0.7.1/bfg9000/builtins/alias.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     6615 2020-08-05 21:45:09.000000 bfg9000-0.7.1/bfg9000/builtins/builtin.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      929 2021-02-17 02:23:34.000000 bfg9000-0.7.1/bfg9000/builtins/clean.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     7218 2021-06-14 02:40:53.000000 bfg9000-0.7.1/bfg9000/builtins/command.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    17356 2021-07-12 23:57:44.000000 bfg9000-0.7.1/bfg9000/builtins/compile.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     7283 2021-07-12 23:57:44.000000 bfg9000-0.7.1/bfg9000/builtins/copy_file.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1097 2020-08-05 21:44:42.000000 bfg9000-0.7.1/bfg9000/builtins/core.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2203 2020-09-07 06:23:31.000000 bfg9000-0.7.1/bfg9000/builtins/default.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1713 2021-02-17 02:23:34.000000 bfg9000-0.7.1/bfg9000/builtins/dist.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     5421 2021-07-12 04:00:01.000000 bfg9000-0.7.1/bfg9000/builtins/file_types.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     5986 2020-12-02 05:42:02.000000 bfg9000-0.7.1/bfg9000/builtins/find.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     7361 2021-07-12 23:57:44.000000 bfg9000-0.7.1/bfg9000/builtins/install.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    25468 2021-11-23 05:28:03.000000 bfg9000-0.7.1/bfg9000/builtins/link.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      277 2020-08-05 21:44:42.000000 bfg9000-0.7.1/bfg9000/builtins/opts.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2733 2023-05-21 01:45:47.000000 bfg9000-0.7.1/bfg9000/builtins/packages.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      993 2020-09-07 06:23:31.000000 bfg9000-0.7.1/bfg9000/builtins/path.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    18909 2022-09-04 21:45:52.000000 bfg9000-0.7.1/bfg9000/builtins/pkg_config.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      988 2020-09-07 06:23:31.000000 bfg9000-0.7.1/bfg9000/builtins/project.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2313 2021-02-17 02:23:34.000000 bfg9000-0.7.1/bfg9000/builtins/regenerate.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4222 2021-11-23 05:28:03.000000 bfg9000-0.7.1/bfg9000/builtins/tests.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3619 2020-09-07 06:23:31.000000 bfg9000-0.7.1/bfg9000/builtins/toolchain.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      306 2021-09-26 04:02:06.000000 bfg9000-0.7.1/bfg9000/builtins/user_arguments.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      791 2020-09-07 06:23:31.000000 bfg9000-0.7.1/bfg9000/builtins/version.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3891 2020-08-05 21:44:42.000000 bfg9000-0.7.1/bfg9000/depfixer.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    16828 2023-01-14 04:23:13.000000 bfg9000-0.7.1/bfg9000/driver.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2524 2020-08-05 21:44:42.000000 bfg9000-0.7.1/bfg9000/e1m1.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    12905 2021-07-12 23:57:44.000000 bfg9000-0.7.1/bfg9000/environment.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      318 2020-12-02 05:42:02.000000 bfg9000-0.7.1/bfg9000/exceptions.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     9854 2021-07-12 23:57:44.000000 bfg9000-0.7.1/bfg9000/file_types.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     6999 2020-12-02 05:42:02.000000 bfg9000-0.7.1/bfg9000/glob.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     5778 2021-02-17 02:23:34.000000 bfg9000-0.7.1/bfg9000/iterutils.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2203 2021-02-17 02:23:34.000000 bfg9000-0.7.1/bfg9000/jvmoutput.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4685 2020-09-07 06:23:31.000000 bfg9000-0.7.1/bfg9000/languages.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     7120 2021-12-31 21:55:46.000000 bfg9000-0.7.1/bfg9000/log.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2228 2023-05-25 23:24:46.000000 bfg9000-0.7.1/bfg9000/objutils.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     7750 2021-02-17 02:23:34.000000 bfg9000-0.7.1/bfg9000/options.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2420 2021-08-04 20:26:41.000000 bfg9000-0.7.1/bfg9000/packages.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2624 2021-12-31 21:55:46.000000 bfg9000-0.7.1/bfg9000/path.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-26 23:26:54.345265 bfg9000-0.7.1/bfg9000/platforms/
+-rw-rw-r--   0 jim       (1000) jim       (1000)       75 2021-12-31 21:55:46.000000 bfg9000-0.7.1/bfg9000/platforms/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     9111 2022-09-04 21:45:52.000000 bfg9000-0.7.1/bfg9000/platforms/basepath.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4512 2023-04-02 06:27:55.000000 bfg9000-0.7.1/bfg9000/platforms/core.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      648 2020-09-07 06:23:31.000000 bfg9000-0.7.1/bfg9000/platforms/cygwin.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      334 2020-08-05 21:44:42.000000 bfg9000-0.7.1/bfg9000/platforms/host.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2779 2022-09-03 05:36:28.000000 bfg9000-0.7.1/bfg9000/platforms/posix.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      340 2021-02-17 02:23:34.000000 bfg9000-0.7.1/bfg9000/platforms/target.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2039 2022-09-03 05:36:35.000000 bfg9000-0.7.1/bfg9000/platforms/windows.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1623 2021-11-23 05:28:03.000000 bfg9000-0.7.1/bfg9000/rccdep.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     6917 2020-11-10 03:37:38.000000 bfg9000-0.7.1/bfg9000/safe_str.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-26 23:26:54.349265 bfg9000-0.7.1/bfg9000/shell/
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3124 2021-12-31 21:55:46.000000 bfg9000-0.7.1/bfg9000/shell/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      615 2020-08-05 21:44:42.000000 bfg9000-0.7.1/bfg9000/shell/list.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3835 2022-10-31 03:40:08.000000 bfg9000-0.7.1/bfg9000/shell/posix.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2475 2022-09-04 21:45:52.000000 bfg9000-0.7.1/bfg9000/shell/syntax.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4838 2022-10-31 03:40:08.000000 bfg9000-0.7.1/bfg9000/shell/windows.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-26 23:26:54.353266 bfg9000-0.7.1/bfg9000/tools/
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1339 2020-11-19 04:05:52.000000 bfg9000-0.7.1/bfg9000/tools/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2685 2020-11-21 00:01:55.000000 bfg9000-0.7.1/bfg9000/tools/ar.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4635 2021-01-02 22:53:27.000000 bfg9000-0.7.1/bfg9000/tools/c_family.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-26 23:26:54.353266 bfg9000-0.7.1/bfg9000/tools/cc/
+-rw-rw-r--   0 jim       (1000) jim       (1000)     8222 2022-01-22 05:33:55.000000 bfg9000-0.7.1/bfg9000/tools/cc/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     6645 2023-05-26 02:47:05.000000 bfg9000-0.7.1/bfg9000/tools/cc/compiler.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      219 2020-09-07 06:23:31.000000 bfg9000-0.7.1/bfg9000/tools/cc/flags.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    16983 2023-05-26 02:47:05.000000 bfg9000-0.7.1/bfg9000/tools/cc/linker.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2571 2021-07-12 23:57:44.000000 bfg9000-0.7.1/bfg9000/tools/cc/rc.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     6537 2021-07-12 23:57:44.000000 bfg9000-0.7.1/bfg9000/tools/common.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1879 2021-07-12 23:57:44.000000 bfg9000-0.7.1/bfg9000/tools/copy_file.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1452 2021-02-17 02:23:34.000000 bfg9000-0.7.1/bfg9000/tools/doppel.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      530 2020-09-07 06:23:31.000000 bfg9000-0.7.1/bfg9000/tools/fortran.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1651 2020-09-07 06:23:31.000000 bfg9000-0.7.1/bfg9000/tools/install_name_tool.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1829 2021-02-17 02:23:34.000000 bfg9000-0.7.1/bfg9000/tools/internal.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      822 2021-12-31 21:55:46.000000 bfg9000-0.7.1/bfg9000/tools/java.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    12771 2021-09-27 18:18:11.000000 bfg9000-0.7.1/bfg9000/tools/jvm.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1614 2021-07-12 23:57:44.000000 bfg9000-0.7.1/bfg9000/tools/ld.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3594 2021-07-12 23:57:44.000000 bfg9000-0.7.1/bfg9000/tools/lex.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      406 2020-08-05 21:44:42.000000 bfg9000-0.7.1/bfg9000/tools/mkdir_p.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4739 2023-02-18 23:42:47.000000 bfg9000-0.7.1/bfg9000/tools/mopack.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-26 23:26:54.357266 bfg9000-0.7.1/bfg9000/tools/msvc/
+-rw-rw-r--   0 jim       (1000) jim       (1000)     5468 2021-12-31 21:55:46.000000 bfg9000-0.7.1/bfg9000/tools/msvc/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     7289 2020-11-19 04:05:52.000000 bfg9000-0.7.1/bfg9000/tools/msvc/compiler.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     8683 2021-08-04 20:26:41.000000 bfg9000-0.7.1/bfg9000/tools/msvc/linker.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3125 2021-07-12 23:57:44.000000 bfg9000-0.7.1/bfg9000/tools/msvc/rc.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2282 2020-09-07 06:23:31.000000 bfg9000-0.7.1/bfg9000/tools/patchelf.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    10605 2023-05-25 02:45:14.000000 bfg9000-0.7.1/bfg9000/tools/pkg_config.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     7250 2021-07-12 23:57:44.000000 bfg9000-0.7.1/bfg9000/tools/qt.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1848 2020-12-28 02:52:54.000000 bfg9000-0.7.1/bfg9000/tools/rc.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      455 2020-08-05 21:44:42.000000 bfg9000-0.7.1/bfg9000/tools/rm.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1408 2020-08-05 21:44:42.000000 bfg9000-0.7.1/bfg9000/tools/scripts.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      807 2020-08-05 21:44:42.000000 bfg9000-0.7.1/bfg9000/tools/setenv.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4065 2021-07-12 23:57:44.000000 bfg9000-0.7.1/bfg9000/tools/yacc.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2800 2021-02-17 02:23:34.000000 bfg9000-0.7.1/bfg9000/versioning.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-26 23:26:54.333266 bfg9000-0.7.1/bfg9000.egg-info/
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4659 2023-05-26 23:26:53.000000 bfg9000-0.7.1/bfg9000.egg-info/PKG-INFO
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3025 2023-05-26 23:26:53.000000 bfg9000-0.7.1/bfg9000.egg-info/SOURCES.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)        1 2023-05-26 23:26:53.000000 bfg9000-0.7.1/bfg9000.egg-info/dependency_links.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1152 2023-05-26 23:26:53.000000 bfg9000-0.7.1/bfg9000.egg-info/entry_points.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)      321 2023-05-26 23:26:53.000000 bfg9000-0.7.1/bfg9000.egg-info/requires.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)        8 2023-05-26 23:26:53.000000 bfg9000-0.7.1/bfg9000.egg-info/top_level.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)      487 2023-05-26 23:26:54.357266 bfg9000-0.7.1/setup.cfg
+-rw-rw-r--   0 jim       (1000) jim       (1000)     6838 2023-05-16 03:14:43.000000 bfg9000-0.7.1/setup.py
```

### Comparing `bfg9000-0.7.0/CHANGES.md` & `bfg9000-0.7.1/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Changes
 
+## v0.7.1 (2023-05-26)
+
+### Bug fixes
+- When using the `PKG_CONFIG_PATH` specified by mopack, add it to any existing
+  `PKG_CONFIG_PATH` from the environment
+- Don't explicitly include default `#include` paths on CC-like compilers
+
+---
+
 ## v0.7.0 (2023-05-20)
 
 ### New features
 - Add support for resolving external package dependencies via [mopack][mopack]
 - Add `bfg9000 run` command to allow executing other commands using the
   environment variables for a given build
 - Add support for installing man pages
```

### Comparing `bfg9000-0.7.0/LICENSE` & `bfg9000-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/PKG-INFO` & `bfg9000-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfg9000
-Version: 0.7.0
+Version: 0.7.1
 Summary: A cross-platform build file generator
 Home-page: https://jimporter.github.io/bfg9000/
 Author: Jim Porter
 Author-email: itsjimporter@gmail.com
 License: BSD-3-Clause
 Description: # bfg9000 - build file generator
         **bfg9000** is a cross-platform *build configuration system* with an emphasis on
```

### Comparing `bfg9000-0.7.0/README.md` & `bfg9000-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/arguments/parser.py` & `bfg9000-0.7.1/bfg9000/arguments/parser.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/arguments/windows.py` & `bfg9000-0.7.1/bfg9000/arguments/windows.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/backends/__init__.py` & `bfg9000-0.7.1/bfg9000/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/backends/compdb/writer.py` & `bfg9000-0.7.1/bfg9000/backends/compdb/writer.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/backends/make/syntax.py` & `bfg9000-0.7.1/bfg9000/backends/make/syntax.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/backends/make/writer.py` & `bfg9000-0.7.1/bfg9000/backends/make/writer.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/backends/msbuild/solution.py` & `bfg9000-0.7.1/bfg9000/backends/msbuild/solution.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/backends/msbuild/syntax.py` & `bfg9000-0.7.1/bfg9000/backends/msbuild/syntax.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/backends/msbuild/writer.py` & `bfg9000-0.7.1/bfg9000/backends/msbuild/writer.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/backends/ninja/syntax.py` & `bfg9000-0.7.1/bfg9000/backends/ninja/syntax.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/backends/ninja/writer.py` & `bfg9000-0.7.1/bfg9000/backends/ninja/writer.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/build.py` & `bfg9000-0.7.1/bfg9000/build.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/build_inputs.py` & `bfg9000-0.7.1/bfg9000/build_inputs.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/alias.py` & `bfg9000-0.7.1/bfg9000/builtins/alias.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/builtin.py` & `bfg9000-0.7.1/bfg9000/builtins/builtin.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/clean.py` & `bfg9000-0.7.1/bfg9000/builtins/clean.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/command.py` & `bfg9000-0.7.1/bfg9000/builtins/command.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/compile.py` & `bfg9000-0.7.1/bfg9000/builtins/compile.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/copy_file.py` & `bfg9000-0.7.1/bfg9000/builtins/copy_file.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/core.py` & `bfg9000-0.7.1/bfg9000/builtins/core.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/default.py` & `bfg9000-0.7.1/bfg9000/builtins/default.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/dist.py` & `bfg9000-0.7.1/bfg9000/builtins/dist.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/file_types.py` & `bfg9000-0.7.1/bfg9000/builtins/file_types.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/find.py` & `bfg9000-0.7.1/bfg9000/builtins/find.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/install.py` & `bfg9000-0.7.1/bfg9000/builtins/install.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/link.py` & `bfg9000-0.7.1/bfg9000/builtins/link.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/packages.py` & `bfg9000-0.7.1/bfg9000/builtins/packages.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/path.py` & `bfg9000-0.7.1/bfg9000/builtins/path.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/pkg_config.py` & `bfg9000-0.7.1/bfg9000/builtins/pkg_config.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/project.py` & `bfg9000-0.7.1/bfg9000/builtins/project.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/regenerate.py` & `bfg9000-0.7.1/bfg9000/builtins/regenerate.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/tests.py` & `bfg9000-0.7.1/bfg9000/builtins/tests.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/toolchain.py` & `bfg9000-0.7.1/bfg9000/builtins/toolchain.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/builtins/version.py` & `bfg9000-0.7.1/bfg9000/builtins/version.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/depfixer.py` & `bfg9000-0.7.1/bfg9000/depfixer.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/driver.py` & `bfg9000-0.7.1/bfg9000/driver.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/e1m1.py` & `bfg9000-0.7.1/bfg9000/e1m1.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/environment.py` & `bfg9000-0.7.1/bfg9000/environment.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/file_types.py` & `bfg9000-0.7.1/bfg9000/file_types.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/glob.py` & `bfg9000-0.7.1/bfg9000/glob.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/iterutils.py` & `bfg9000-0.7.1/bfg9000/iterutils.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/jvmoutput.py` & `bfg9000-0.7.1/bfg9000/jvmoutput.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/languages.py` & `bfg9000-0.7.1/bfg9000/languages.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/log.py` & `bfg9000-0.7.1/bfg9000/log.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/objutils.py` & `bfg9000-0.7.1/bfg9000/objutils.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/options.py` & `bfg9000-0.7.1/bfg9000/options.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/packages.py` & `bfg9000-0.7.1/bfg9000/packages.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/path.py` & `bfg9000-0.7.1/bfg9000/path.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/platforms/basepath.py` & `bfg9000-0.7.1/bfg9000/platforms/basepath.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/platforms/core.py` & `bfg9000-0.7.1/bfg9000/platforms/core.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/platforms/cygwin.py` & `bfg9000-0.7.1/bfg9000/platforms/cygwin.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/platforms/posix.py` & `bfg9000-0.7.1/bfg9000/platforms/posix.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/platforms/windows.py` & `bfg9000-0.7.1/bfg9000/platforms/windows.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/rccdep.py` & `bfg9000-0.7.1/bfg9000/rccdep.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/safe_str.py` & `bfg9000-0.7.1/bfg9000/safe_str.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/shell/__init__.py` & `bfg9000-0.7.1/bfg9000/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/shell/list.py` & `bfg9000-0.7.1/bfg9000/shell/list.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/shell/posix.py` & `bfg9000-0.7.1/bfg9000/shell/posix.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/shell/syntax.py` & `bfg9000-0.7.1/bfg9000/shell/syntax.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/shell/windows.py` & `bfg9000-0.7.1/bfg9000/shell/windows.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/__init__.py` & `bfg9000-0.7.1/bfg9000/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/ar.py` & `bfg9000-0.7.1/bfg9000/tools/ar.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/c_family.py` & `bfg9000-0.7.1/bfg9000/tools/c_family.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/cc/__init__.py` & `bfg9000-0.7.1/bfg9000/tools/cc/__init__.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/cc/compiler.py` & `bfg9000-0.7.1/bfg9000/tools/cc/compiler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from itertools import chain
 
-from ... import options as opts, safe_str
+from ... import options as opts, safe_str, shell
 from .flags import optimize_flags
 from ..common import BuildCommand
 from ...file_types import ObjectFile, PrecompiledHeader
-from ...iterutils import iterate
-from ...path import Path
+from ...iterutils import default_sentinel, iterate
+from ...objutils import memoize_method
+from ...path import abspath, Path
 from ...versioning import SpecifierSet
 
 
 class CcBaseCompiler(BuildCommand):
     @property
     def deps_flavor(self):
         return None if self.lang in ('f77', 'f95') else 'gcc'
@@ -18,16 +19,45 @@
     def needs_libs(self):
         return False
 
     @property
     def needs_package_options(self):
         return True
 
+    @memoize_method
+    def _search_dirs(self, cpath=default_sentinel, strict=False):
+        try:
+            extra_env = ({'CPATH': cpath or ''}
+                         if cpath is not default_sentinel else None)
+            output = self.env.execute(
+                (self.command + self._always_flags + self.global_flags +
+                 ['-E', '-Wp,-v', '/dev/null']),
+                extra_env=extra_env, stdout=shell.Mode.pipe,
+                stderr=shell.Mode.stdout
+            )
+
+            found = False
+            dirs = []
+            for i in output.splitlines():  # pragma: no branch
+                if i == '#include <...> search starts here:':
+                    found = True
+                elif i == 'End of search list.':
+                    break
+                elif i[0] != ' ':
+                    found = False
+                elif found:
+                    dirs.append(abspath(i[1:]))
+            return dirs
+        except (OSError, shell.CalledProcessError):
+            if strict:
+                raise
+            return self.env.variables.getpaths('CPATH')
+
     def search_dirs(self, strict=False):
-        return self.env.variables.getpaths('CPATH')
+        return self._search_dirs(strict=strict)
 
     def _call(self, cmd, input, output, deps=None, flags=None):
         result = list(chain(
             cmd, self._always_flags, iterate(flags), ['-c', input]
         ))
         if deps:
             result.extend(['-MMD', '-MF', deps])
@@ -45,20 +75,22 @@
                 flags.append('-fcolor-diagnostics')
             elif (self.brand == 'gcc' and self.version and
                   self.version in SpecifierSet('>=4.9')):
                 flags.append('-fdiagnostics-color')
         return flags
 
     def _include_dir(self, directory, allow_system):
-        is_default = directory.path in self.env.host_platform.include_dirs
-
-        # Don't include default directories as system dirs (e.g. /usr/include).
-        # Doing so would break GCC 6 when #including stdlib.h:
-        # <https://gcc.gnu.org/bugzilla/show_bug.cgi?id=70129>.
-        if allow_system and directory.system and not is_default:
+        default_dirs = self._search_dirs(None)
+        if directory.path in default_dirs:
+            # Don't include default directories (e.g. /usr/include). Including
+            # them as system dirs would break GCC 6 when #including stdlib.h:
+            # <https://gcc.gnu.org/bugzilla/show_bug.cgi?id=70129>. Including
+            # them as regular directories isn't right either.
+            return []
+        elif allow_system and directory.system:
             return ['-isystem', directory.path]
         else:
             return ['-I' + directory.path]
 
     def flags(self, options, global_options=None, output=None, mode='normal'):
         pkgconf_mode = mode == 'pkg-config'
         flags = []
```

### Comparing `bfg9000-0.7.0/bfg9000/tools/cc/linker.py` & `bfg9000-0.7.1/bfg9000/tools/cc/linker.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .. import install_name_tool, patchelf
 from ... import options as opts, safe_str, shell
 from .flags import optimize_flags
 from ..common import BuildCommand, library_macro
 from ...builtins.copy_file import CopyFile
 from ...file_types import *
 from ...iterutils import first, iterate, listify, recursive_walk, uniques
+from ...objutils import memoize_method
 from ...path import abspath, Path
 from ...versioning import SpecifierSet
 from ...packages import Framework
 
 
 class CcLinker(BuildCommand):
     __known_langs = {'java', 'c', 'c++', 'objc', 'objc++', 'f77', 'f95'}
@@ -67,26 +68,28 @@
     def _has_link_macros(self):
         # We only need to define LIBFOO_EXPORTS/LIBFOO_STATIC macros on
         # platforms that have different import/export rules for libraries. We
         # approximate this by checking if the platform uses import libraries,
         # and only define the macros if it does.
         return self.env.target_platform.has_import_library
 
+    @memoize_method
     def sysroot(self, strict=False):
         try:
             # XXX: clang doesn't support -print-sysroot.
             return self.env.execute(
                 self.command + self.global_flags + ['-print-sysroot'],
                 stdout=shell.Mode.pipe, stderr=shell.Mode.devnull
             ).rstrip()
         except (OSError, shell.CalledProcessError):
             if strict:
                 raise
             return '' if self.env.target_platform.family == 'windows' else '/'
 
+    @memoize_method
     def search_dirs(self, strict=False):
         try:
             output = self.env.execute(
                 self.command + self.global_flags + ['-print-search-dirs'],
                 stdout=shell.Mode.pipe, stderr=shell.Mode.devnull
             )
             m = re.search(r'^libraries: =(.*)', output, re.MULTILINE)
```

### Comparing `bfg9000-0.7.0/bfg9000/tools/cc/rc.py` & `bfg9000-0.7.1/bfg9000/tools/cc/rc.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/common.py` & `bfg9000-0.7.1/bfg9000/tools/common.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/copy_file.py` & `bfg9000-0.7.1/bfg9000/tools/copy_file.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/doppel.py` & `bfg9000-0.7.1/bfg9000/tools/doppel.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/fortran.py` & `bfg9000-0.7.1/bfg9000/tools/fortran.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/install_name_tool.py` & `bfg9000-0.7.1/bfg9000/tools/install_name_tool.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/internal.py` & `bfg9000-0.7.1/bfg9000/tools/internal.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/java.py` & `bfg9000-0.7.1/bfg9000/tools/java.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/jvm.py` & `bfg9000-0.7.1/bfg9000/tools/jvm.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/ld.py` & `bfg9000-0.7.1/bfg9000/tools/ld.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/lex.py` & `bfg9000-0.7.1/bfg9000/tools/lex.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/mopack.py` & `bfg9000-0.7.1/bfg9000/tools/mopack.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/msvc/__init__.py` & `bfg9000-0.7.1/bfg9000/tools/msvc/__init__.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/msvc/compiler.py` & `bfg9000-0.7.1/bfg9000/tools/msvc/compiler.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/msvc/linker.py` & `bfg9000-0.7.1/bfg9000/tools/msvc/linker.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/msvc/rc.py` & `bfg9000-0.7.1/bfg9000/tools/msvc/rc.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/patchelf.py` & `bfg9000-0.7.1/bfg9000/tools/patchelf.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/pkg_config.py` & `bfg9000-0.7.1/bfg9000/tools/pkg_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,24 +100,30 @@
 
         result = super().run(names, type, *args, extra_env=extra_env,
                              **kwargs).strip()
         if self._options[type][1]:
             return self._options[type][1](result)
         return result
 
+    def search_path(self, extra=[]):
+        path = self.env.variables.get('PKG_CONFIG_PATH')
+        if path:
+            return shell.join_paths(extra + [path])
+        return shell.join_paths(extra)
+
 
 class PkgConfigPackage(Package):
     def __init__(self, pkg_config, name, submodules=None,
                  specifier=SpecifierSet(), pcnames=None, *, format,
                  kind=PackageKind.any, system=True, deps=None,
                  search_path=None):
         super().__init__(name, submodules, format=format, deps=deps)
 
         self._pkg_config = pkg_config
-        self._env = ({'PKG_CONFIG_PATH': shell.join_paths(search_path)}
+        self._env = ({'PKG_CONFIG_PATH': pkg_config.search_path(search_path)}
                      if search_path else {})
         self.pcnames = pcnames if pcnames is not None else [name]
 
         try:
             version = self._call(self.pcnames[0], 'version')
             version = Version(version) if version else None
         except subprocess.CalledProcessError:
```

### Comparing `bfg9000-0.7.0/bfg9000/tools/qt.py` & `bfg9000-0.7.1/bfg9000/tools/qt.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/rc.py` & `bfg9000-0.7.1/bfg9000/tools/rc.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/scripts.py` & `bfg9000-0.7.1/bfg9000/tools/scripts.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/setenv.py` & `bfg9000-0.7.1/bfg9000/tools/setenv.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/tools/yacc.py` & `bfg9000-0.7.1/bfg9000/tools/yacc.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000/versioning.py` & `bfg9000-0.7.1/bfg9000/versioning.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000.egg-info/PKG-INFO` & `bfg9000-0.7.1/bfg9000.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfg9000
-Version: 0.7.0
+Version: 0.7.1
 Summary: A cross-platform build file generator
 Home-page: https://jimporter.github.io/bfg9000/
 Author: Jim Porter
 Author-email: itsjimporter@gmail.com
 License: BSD-3-Clause
 Description: # bfg9000 - build file generator
         **bfg9000** is a cross-platform *build configuration system* with an emphasis on
```

### Comparing `bfg9000-0.7.0/bfg9000.egg-info/SOURCES.txt` & `bfg9000-0.7.1/bfg9000.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/bfg9000.egg-info/entry_points.txt` & `bfg9000-0.7.1/bfg9000.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `bfg9000-0.7.0/setup.py` & `bfg9000-0.7.1/setup.py`

 * *Files identical despite different names*

