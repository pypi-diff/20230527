# Comparing `tmp/exorad-2.1.86.tar.gz` & `tmp/exorad-2.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/lorenzo/Dropbox/git/ExoRad2-public/dist/tmpwa0dv52c/exorad-2.1.86.tar", last modified: Mon Aug  2 10:02:20 2021, max compression
+gzip compressed data, was "dist/exorad-2.1.94.tar", last modified: Mon Nov 15 09:34:22 2021, max compression
```

## Comparing `exorad-2.1.86.tar` & `exorad-2.1.94.tar`

### file list

```diff
@@ -1,67 +1,154 @@
-drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-08-02 10:02:20.543486 exorad-2.1.86/
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     6318 2021-07-02 09:04:42.000000 exorad-2.1.86/LICENSE
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     3336 2021-08-02 10:02:20.543486 exorad-2.1.86/PKG-INFO
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     2401 2021-07-02 09:49:02.000000 exorad-2.1.86/README.md
-drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-08-02 10:02:20.531486 exorad-2.1.86/exorad/
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1054 2021-07-02 07:50:20.000000 exorad-2.1.86/exorad/__init__.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)       23 2021-08-02 09:50:16.000000 exorad-2.1.86/exorad/__version__.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     4653 2021-07-02 07:42:29.000000 exorad-2.1.86/exorad/exorad.py
-drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-08-02 10:02:20.535486 exorad-2.1.86/exorad/log/
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     3419 2021-07-02 08:35:49.000000 exorad-2.1.86/exorad/log/__init__.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     4299 2021-07-02 08:35:49.000000 exorad-2.1.86/exorad/log/logger.py
-drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-08-02 10:02:20.535486 exorad-2.1.86/exorad/models/
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)        0 2020-05-14 09:43:29.000000 exorad-2.1.86/exorad/models/__init__.py
-drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-08-02 10:02:20.535486 exorad-2.1.86/exorad/models/foregrounds/
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)        0 2020-08-24 13:21:00.000000 exorad-2.1.86/exorad/models/foregrounds/__init__.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1505 2020-09-28 10:52:30.000000 exorad-2.1.86/exorad/models/foregrounds/skyForegrounds.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     3539 2021-03-05 16:02:02.000000 exorad-2.1.86/exorad/models/foregrounds/zodiacalForeground.py
-drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-08-02 10:02:20.535486 exorad-2.1.86/exorad/models/instruments/
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      109 2020-10-13 13:06:11.000000 exorad-2.1.86/exorad/models/instruments/__init__.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    12856 2021-01-28 10:47:06.000000 exorad-2.1.86/exorad/models/instruments/instrument.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     5140 2020-12-10 14:52:04.000000 exorad-2.1.86/exorad/models/instruments/photometer.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    12986 2021-08-02 09:35:20.000000 exorad-2.1.86/exorad/models/instruments/spectrometer.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     5800 2021-01-25 10:50:24.000000 exorad-2.1.86/exorad/models/noise.py
-drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-08-02 10:02:20.539486 exorad-2.1.86/exorad/models/optics/
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)        0 2020-08-24 13:20:36.000000 exorad-2.1.86/exorad/models/optics/__init__.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     6593 2021-01-28 10:47:06.000000 exorad-2.1.86/exorad/models/optics/opticalElement.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     9615 2020-12-10 14:52:04.000000 exorad-2.1.86/exorad/models/optics/opticalPath.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     7495 2021-01-04 16:08:21.000000 exorad-2.1.86/exorad/models/signal.py
--rwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)     6682 2021-06-08 10:52:02.000000 exorad-2.1.86/exorad/models/source.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1407 2020-12-22 07:37:54.000000 exorad-2.1.86/exorad/models/target.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    10100 2021-02-16 14:29:43.000000 exorad-2.1.86/exorad/models/targetlist.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      449 2021-01-28 10:47:33.000000 exorad-2.1.86/exorad/models/utils.py
-drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-08-02 10:02:20.539486 exorad-2.1.86/exorad/output/
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)        0 2020-07-03 12:22:23.000000 exorad-2.1.86/exorad/output/__init__.py
-drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-08-02 10:02:20.539486 exorad-2.1.86/exorad/output/hdf5/
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)       52 2020-07-10 16:38:03.000000 exorad-2.1.86/exorad/output/hdf5/__init__.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     8480 2021-07-02 08:35:49.000000 exorad-2.1.86/exorad/output/hdf5/hdf5.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     4127 2021-03-16 08:56:26.000000 exorad-2.1.86/exorad/output/hdf5/util.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     3880 2021-07-02 08:35:49.000000 exorad-2.1.86/exorad/output/output.py
-drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-08-02 10:02:20.539486 exorad-2.1.86/exorad/tasks/
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      565 2020-08-24 14:18:59.000000 exorad-2.1.86/exorad/tasks/__init__.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     5096 2020-12-10 14:52:04.000000 exorad-2.1.86/exorad/tasks/foregroundHandler.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    10586 2021-06-25 11:01:54.000000 exorad-2.1.86/exorad/tasks/instrumentHandler.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     6699 2021-07-24 11:25:28.000000 exorad-2.1.86/exorad/tasks/loadOptions.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     5364 2021-06-16 09:30:54.000000 exorad-2.1.86/exorad/tasks/loadSource.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     4522 2020-12-19 13:48:38.000000 exorad-2.1.86/exorad/tasks/noiseHandler.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     2535 2020-12-10 14:52:04.000000 exorad-2.1.86/exorad/tasks/propagateLight.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    10268 2021-07-02 07:41:49.000000 exorad-2.1.86/exorad/tasks/targetHandler.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1794 2021-05-21 14:14:29.000000 exorad-2.1.86/exorad/tasks/task.py
-drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-08-02 10:02:20.543486 exorad-2.1.86/exorad/utils/
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)        0 2020-07-07 13:24:35.000000 exorad-2.1.86/exorad/utils/__init__.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1224 2020-08-04 09:50:41.000000 exorad-2.1.86/exorad/utils/ascii_art.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     3652 2021-07-27 15:13:16.000000 exorad-2.1.86/exorad/utils/diffuse_light_propagation.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     8349 2021-08-02 09:35:20.000000 exorad-2.1.86/exorad/utils/exolib.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1390 2020-08-08 08:47:18.000000 exorad-2.1.86/exorad/utils/mpi.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    13753 2021-01-28 12:27:04.000000 exorad-2.1.86/exorad/utils/plotter.py
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     3534 2020-12-10 14:53:11.000000 exorad-2.1.86/exorad/utils/util.py
-drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-08-02 10:02:20.535486 exorad-2.1.86/exorad.egg-info/
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     3336 2021-08-02 10:02:20.000000 exorad-2.1.86/exorad.egg-info/PKG-INFO
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1484 2021-08-02 10:02:20.000000 exorad-2.1.86/exorad.egg-info/SOURCES.txt
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)        1 2021-08-02 10:02:20.000000 exorad-2.1.86/exorad.egg-info/dependency_links.txt
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)       94 2021-08-02 10:02:20.000000 exorad-2.1.86/exorad.egg-info/entry_points.txt
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)        1 2021-02-11 10:14:45.000000 exorad-2.1.86/exorad.egg-info/not-zip-safe
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)       83 2021-08-02 10:02:20.000000 exorad-2.1.86/exorad.egg-info/requires.txt
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)        7 2021-08-02 10:02:20.000000 exorad-2.1.86/exorad.egg-info/top_level.txt
--rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)       38 2021-08-02 10:02:20.543486 exorad-2.1.86/setup.cfg
--rwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)     2391 2021-07-02 08:01:51.000000 exorad-2.1.86/setup.py
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.410367 exorad-2.1.94/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     4740 2020-08-08 08:37:16.000000 exorad-2.1.94/.gitignore
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      583 2020-08-27 13:03:14.000000 exorad-2.1.94/.readthedocs.yaml
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     8090 2021-11-15 09:25:38.000000 exorad-2.1.94/CHANGELOG.md
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     6318 2021-07-02 09:04:42.000000 exorad-2.1.94/LICENSE
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     3336 2021-11-15 09:34:22.410367 exorad-2.1.94/PKG-INFO
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     2401 2021-07-02 09:49:02.000000 exorad-2.1.94/README.md
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.254365 exorad-2.1.94/docs/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      638 2020-05-13 14:08:50.000000 exorad-2.1.94/docs/Makefile
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      799 2020-05-13 14:08:50.000000 exorad-2.1.94/docs/make.bat
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.254365 exorad-2.1.94/docs/source/
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.254365 exorad-2.1.94/docs/source/_static/
+-rw-r--r--   0 lorenzo   (1001) lorenzo   (1001)    15086 2020-11-24 11:20:59.000000 exorad-2.1.94/docs/source/_static/favicon.ico
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)   146217 2020-11-24 11:18:22.000000 exorad-2.1.94/docs/source/_static/logo.png
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.262365 exorad-2.1.94/docs/source/api/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      576 2020-08-24 13:24:51.000000 exorad-2.1.94/docs/source/api/exorad.models.foregrounds.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      488 2020-08-20 14:39:42.000000 exorad-2.1.94/docs/source/api/exorad.models.instruments.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      488 2020-08-24 14:03:27.000000 exorad-2.1.94/docs/source/api/exorad.models.noise.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      652 2020-08-24 13:26:23.000000 exorad-2.1.94/docs/source/api/exorad.models.optics.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      882 2020-08-24 13:51:43.000000 exorad-2.1.94/docs/source/api/exorad.models.signal.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      337 2020-08-24 13:58:45.000000 exorad-2.1.94/docs/source/api/exorad.models.source.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      159 2020-08-25 10:36:57.000000 exorad-2.1.94/docs/source/api/exorad.output.hdf5.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      556 2020-08-24 14:09:03.000000 exorad-2.1.94/docs/source/api/exorad.tasks.foregroundHandler.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1009 2020-08-25 13:09:40.000000 exorad-2.1.94/docs/source/api/exorad.tasks.instrumentHandler.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      222 2020-08-24 14:11:47.000000 exorad-2.1.94/docs/source/api/exorad.tasks.loadOptions.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      219 2020-08-24 14:11:47.000000 exorad-2.1.94/docs/source/api/exorad.tasks.loadSource.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      392 2020-08-25 13:09:32.000000 exorad-2.1.94/docs/source/api/exorad.tasks.noiseHandler.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      431 2020-08-25 13:09:24.000000 exorad-2.1.94/docs/source/api/exorad.tasks.propagateLight.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1010 2020-08-24 14:17:36.000000 exorad-2.1.94/docs/source/api/exorad.tasks.targetHandler.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      192 2020-08-24 14:20:31.000000 exorad-2.1.94/docs/source/api/exorad.tasks.task.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      462 2020-08-25 14:45:25.000000 exorad-2.1.94/docs/source/api/exorad.utils.exolib.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      204 2020-08-24 14:21:22.000000 exorad-2.1.94/docs/source/api/exorad.utils.plotter.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      646 2021-02-16 14:33:16.000000 exorad-2.1.94/docs/source/api/index.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     4486 2021-01-26 15:22:36.000000 exorad-2.1.94/docs/source/conf.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1758 2021-07-02 08:28:39.000000 exorad-2.1.94/docs/source/index.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1165 2021-06-22 14:03:58.000000 exorad-2.1.94/docs/source/requirements.txt
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.262365 exorad-2.1.94/docs/source/user/
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.270365 exorad-2.1.94/docs/source/user/_static/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    48827 2020-08-20 13:14:19.000000 exorad-2.1.94/docs/source/user/_static/ExoRad-scheme.png
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    40125 2020-08-24 13:09:02.000000 exorad-2.1.94/docs/source/user/_static/efficiency.png
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    90005 2020-08-24 13:09:03.000000 exorad-2.1.94/docs/source/user/_static/myTest.png
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    14212 2020-08-25 09:47:19.000000 exorad-2.1.94/docs/source/user/_static/output_channels.png
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    15336 2020-08-25 09:47:05.000000 exorad-2.1.94/docs/source/user/_static/output_main.png
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    16238 2020-08-25 09:47:13.000000 exorad-2.1.94/docs/source/user/_static/output_payload.png
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    24590 2020-08-25 09:47:44.000000 exorad-2.1.94/docs/source/user/_static/output_spec.png
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)   101361 2020-08-25 09:47:58.000000 exorad-2.1.94/docs/source/user/_static/output_spec_table.png
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    23003 2020-08-26 07:35:41.000000 exorad-2.1.94/docs/source/user/_static/output_target.png
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    18571 2020-08-26 07:35:54.000000 exorad-2.1.94/docs/source/user/_static/output_target_table.png
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    15870 2020-08-26 07:35:33.000000 exorad-2.1.94/docs/source/user/_static/output_targets.png
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      525 2020-08-25 14:53:19.000000 exorad-2.1.94/docs/source/user/index.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     2598 2020-08-25 15:11:39.000000 exorad-2.1.94/docs/source/user/inputs.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1279 2020-12-26 16:42:48.000000 exorad-2.1.94/docs/source/user/installation.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      526 2020-08-25 13:08:59.000000 exorad-2.1.94/docs/source/user/introduction.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     4196 2020-08-26 08:08:10.000000 exorad-2.1.94/docs/source/user/light_and_noise.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     2838 2021-08-02 09:59:28.000000 exorad-2.1.94/docs/source/user/outputs.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     5665 2020-08-25 14:13:17.000000 exorad-2.1.94/docs/source/user/prepare_optics.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     6237 2021-02-16 14:24:00.000000 exorad-2.1.94/docs/source/user/prepare_payload.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     5383 2021-02-16 16:28:39.000000 exorad-2.1.94/docs/source/user/prepare_target.rst
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     4938 2021-02-16 14:25:38.000000 exorad-2.1.94/docs/source/user/quickstart_guide.rst
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.382366 exorad-2.1.94/examples/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     3800 2020-07-08 09:40:21.000000 exorad-2.1.94/examples/QE.csv
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    18316 2020-07-02 10:48:31.000000 exorad-2.1.94/examples/Spec-wl_sol.csv
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001) 22299529 2020-04-09 14:00:57.000000 exorad-2.1.94/examples/customsed.csv
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)   345709 2020-08-24 13:03:16.000000 exorad-2.1.94/examples/modtran_38km_sun_180az_55zd_los_45zd.csv
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    11256 2021-02-16 16:13:02.000000 exorad-2.1.94/examples/payload_example.xml
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)   323075 2020-12-22 11:25:26.000000 exorad-2.1.94/examples/quickstart.ipynb
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)   264406 2020-12-22 11:25:33.000000 exorad-2.1.94/examples/quickstart.pdf
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      124 2020-12-03 13:03:03.000000 exorad-2.1.94/examples/test_target.csv
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.382366 exorad-2.1.94/exorad/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1128 2021-08-02 14:14:41.000000 exorad-2.1.94/exorad/__init__.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)       23 2021-11-15 09:25:38.000000 exorad-2.1.94/exorad/__version__.py
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.382366 exorad-2.1.94/exorad/data/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)  1565888 2021-02-16 15:45:57.000000 exorad-2.1.94/exorad/data/Zodi_map.hdf5
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     4761 2021-11-03 09:13:57.000000 exorad-2.1.94/exorad/exorad.py
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.390366 exorad-2.1.94/exorad/log/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     3419 2021-07-02 08:35:49.000000 exorad-2.1.94/exorad/log/__init__.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     4299 2021-07-02 08:35:49.000000 exorad-2.1.94/exorad/log/logger.py
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.390366 exorad-2.1.94/exorad/models/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)        0 2020-05-14 09:43:29.000000 exorad-2.1.94/exorad/models/__init__.py
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.390366 exorad-2.1.94/exorad/models/foregrounds/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)        0 2020-08-24 13:21:00.000000 exorad-2.1.94/exorad/models/foregrounds/__init__.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1505 2020-09-28 10:52:30.000000 exorad-2.1.94/exorad/models/foregrounds/skyForegrounds.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     3539 2021-03-05 16:02:02.000000 exorad-2.1.94/exorad/models/foregrounds/zodiacalForeground.py
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.394366 exorad-2.1.94/exorad/models/instruments/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      109 2020-10-13 13:06:11.000000 exorad-2.1.94/exorad/models/instruments/__init__.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    12856 2021-01-28 10:47:06.000000 exorad-2.1.94/exorad/models/instruments/instrument.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     5388 2021-11-03 09:23:28.000000 exorad-2.1.94/exorad/models/instruments/photometer.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    12986 2021-08-02 09:35:20.000000 exorad-2.1.94/exorad/models/instruments/spectrometer.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     5800 2021-01-25 10:50:24.000000 exorad-2.1.94/exorad/models/noise.py
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.394366 exorad-2.1.94/exorad/models/optics/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)        0 2020-08-24 13:20:36.000000 exorad-2.1.94/exorad/models/optics/__init__.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     6593 2021-01-28 10:47:06.000000 exorad-2.1.94/exorad/models/optics/opticalElement.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     9615 2021-09-07 13:36:29.000000 exorad-2.1.94/exorad/models/optics/opticalPath.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     7495 2021-01-04 16:08:21.000000 exorad-2.1.94/exorad/models/signal.py
+-rwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)     9301 2021-11-12 11:19:47.000000 exorad-2.1.94/exorad/models/source.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1407 2020-12-22 07:37:54.000000 exorad-2.1.94/exorad/models/target.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    10100 2021-02-16 14:29:43.000000 exorad-2.1.94/exorad/models/targetlist.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      449 2021-01-28 10:47:33.000000 exorad-2.1.94/exorad/models/utils.py
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.394366 exorad-2.1.94/exorad/output/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)        0 2020-07-03 12:22:23.000000 exorad-2.1.94/exorad/output/__init__.py
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.394366 exorad-2.1.94/exorad/output/hdf5/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)       52 2020-07-10 16:38:03.000000 exorad-2.1.94/exorad/output/hdf5/__init__.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     8480 2021-07-02 08:35:49.000000 exorad-2.1.94/exorad/output/hdf5/hdf5.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     4127 2021-03-16 08:56:26.000000 exorad-2.1.94/exorad/output/hdf5/util.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     3880 2021-07-02 08:35:49.000000 exorad-2.1.94/exorad/output/output.py
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.398366 exorad-2.1.94/exorad/tasks/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      565 2020-08-24 14:18:59.000000 exorad-2.1.94/exorad/tasks/__init__.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     5096 2020-12-10 14:52:04.000000 exorad-2.1.94/exorad/tasks/foregroundHandler.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    11605 2021-11-03 09:10:46.000000 exorad-2.1.94/exorad/tasks/instrumentHandler.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     6820 2021-09-16 14:32:23.000000 exorad-2.1.94/exorad/tasks/loadOptions.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     6054 2021-09-22 15:50:28.000000 exorad-2.1.94/exorad/tasks/loadSource.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     4522 2020-12-19 13:48:38.000000 exorad-2.1.94/exorad/tasks/noiseHandler.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     2535 2020-12-10 14:52:04.000000 exorad-2.1.94/exorad/tasks/propagateLight.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    10174 2021-09-30 13:14:48.000000 exorad-2.1.94/exorad/tasks/targetHandler.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1794 2021-05-21 14:14:29.000000 exorad-2.1.94/exorad/tasks/task.py
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.398366 exorad-2.1.94/exorad/utils/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)        0 2020-07-07 13:24:35.000000 exorad-2.1.94/exorad/utils/__init__.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1224 2020-08-04 09:50:41.000000 exorad-2.1.94/exorad/utils/ascii_art.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     3652 2021-07-27 15:13:16.000000 exorad-2.1.94/exorad/utils/diffuse_light_propagation.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     8390 2021-10-10 15:03:24.000000 exorad-2.1.94/exorad/utils/exolib.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1390 2020-08-08 08:47:18.000000 exorad-2.1.94/exorad/utils/mpi.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    13753 2021-01-28 12:27:04.000000 exorad-2.1.94/exorad/utils/plotter.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     3534 2020-12-10 14:53:11.000000 exorad-2.1.94/exorad/utils/util.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     2568 2021-08-02 15:27:46.000000 exorad-2.1.94/exorad/utils/version_control.py
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.382366 exorad-2.1.94/exorad.egg-info/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     3336 2021-11-15 09:34:21.000000 exorad-2.1.94/exorad.egg-info/PKG-INFO
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     3979 2021-11-15 09:34:22.000000 exorad-2.1.94/exorad.egg-info/SOURCES.txt
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)        1 2021-11-15 09:34:21.000000 exorad-2.1.94/exorad.egg-info/dependency_links.txt
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)       94 2021-11-15 09:34:21.000000 exorad-2.1.94/exorad.egg-info/entry_points.txt
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)        1 2021-02-11 10:14:45.000000 exorad-2.1.94/exorad.egg-info/not-zip-safe
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)       83 2021-11-15 09:34:22.000000 exorad-2.1.94/exorad.egg-info/requires.txt
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)        7 2021-11-15 09:34:22.000000 exorad-2.1.94/exorad.egg-info/top_level.txt
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)       38 2021-11-15 09:34:22.410367 exorad-2.1.94/setup.cfg
+-rwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)     2391 2021-07-02 08:01:51.000000 exorad-2.1.94/setup.py
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.406366 exorad-2.1.94/tests/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)       17 2021-06-16 12:40:55.000000 exorad-2.1.94/tests/conf.py
+drwxrwxr-x   0 lorenzo   (1001) lorenzo   (1001)        0 2021-11-15 09:34:22.410367 exorad-2.1.94/tests/test_data/
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     7925 2021-06-16 12:40:55.000000 exorad-2.1.94/tests/test_data/payload_example_missing_data_file.xml
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    11287 2021-11-15 09:29:52.000000 exorad-2.1.94/tests/test_data/payload_test.xml
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      144 2021-06-16 12:40:55.000000 exorad-2.1.94/tests/test_data/test_target.csv
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     2603 2021-06-16 12:40:55.000000 exorad-2.1.94/tests/test_foreground.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)      570 2021-08-02 14:32:39.000000 exorad-2.1.94/tests/test_git.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     4233 2021-06-16 13:56:45.000000 exorad-2.1.94/tests/test_instrument.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1245 2021-06-16 12:40:55.000000 exorad-2.1.94/tests/test_logger.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1819 2021-06-16 12:40:55.000000 exorad-2.1.94/tests/test_noise.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)    11437 2021-07-27 15:14:43.000000 exorad-2.1.94/tests/test_optical.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     3336 2021-06-16 13:55:51.000000 exorad-2.1.94/tests/test_options.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     2936 2021-06-16 12:40:55.000000 exorad-2.1.94/tests/test_pipeline.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     2261 2021-06-16 12:40:55.000000 exorad-2.1.94/tests/test_plotter.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     2196 2021-06-16 12:40:55.000000 exorad-2.1.94/tests/test_propagation.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     2741 2021-06-16 12:40:55.000000 exorad-2.1.94/tests/test_signal.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     4582 2021-11-03 14:38:50.000000 exorad-2.1.94/tests/test_star.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     4221 2021-06-16 14:11:55.000000 exorad-2.1.94/tests/test_target.py
+-rw-rw-r--   0 lorenzo   (1001) lorenzo   (1001)     1060 2020-07-03 08:51:06.000000 exorad-2.1.94/tests/test_task.py
```

### Comparing `exorad-2.1.86/LICENSE` & `exorad-2.1.94/LICENSE`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/PKG-INFO` & `exorad-2.1.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exorad
-Version: 2.1.86
+Version: 2.1.94
 Summary: The generic point source radiometric model
 Home-page: https://github.com/ExObsSim/ExoRad2-public
 Author: Lorenzo V. Mugnai, Enzo Pascale
 Author-email: lorenzo.mugnai@uniroma1.it
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `exorad-2.1.86/README.md` & `exorad-2.1.94/README.md`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/__init__.py` & `exorad-2.1.94/exorad/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,7 +31,11 @@
 __author__ = "Lorenzo V. Mugnai, Enzo Pascale"
 __email__ = "lorenzo.mugnai@uniroma1.it"
 
 __license__ = "BSD-3-Clause"
 __copyright__ = '2020-{:d}, {}'.format(date.today().year, __author__)
 
 from exorad.exorad import standard_pipeline
+
+
+from exorad.utils.version_control import VersionControl
+VersionControl()
```

### Comparing `exorad-2.1.86/exorad/exorad.py` & `exorad-2.1.94/exorad/exorad.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,24 +30,28 @@
     else:
         plotter.save_fig(os.path.join(output_dir, 'efficiency.png'), efficiency=True)
         logger.info('efficiency plot saved in output directory')
     plt.close()
 
 
 def standard_pipeline(options, target_list, output=None, plot=False, full_contrib=False,
-                      n_thread=1, debug=False, log=False):
+                      n_thread=1, debug=False, log=False, replace=True):
     from exorad.utils.ascii_art import ascii_art
     logger.info(ascii_art)
     logger.info('code version {}'.format(version))
 
     if debug: setLogLevel(logging.DEBUG)
     if isinstance(log, str): addLogFile(fname=log)
     elif log: addLogFile()
 
     if output is not None:
+        if replace:
+            if os.path.exists(output):
+                os.remove(output)
+
         out_dir = pathlib.Path(output).parent.absolute()
         if not os.path.exists(out_dir):
             os.makedirs(out_dir)
             logger.info('output directory created')
         logger.info('output directory set as {}'.format(out_dir))
         try:
             shutil.copy(options, out_dir)
```

### Comparing `exorad-2.1.86/exorad/log/__init__.py` & `exorad-2.1.94/exorad/log/__init__.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/log/logger.py` & `exorad-2.1.94/exorad/log/logger.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/models/foregrounds/skyForegrounds.py` & `exorad-2.1.94/exorad/models/foregrounds/skyForegrounds.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/models/foregrounds/zodiacalForeground.py` & `exorad-2.1.94/exorad/models/foregrounds/zodiacalForeground.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/models/instruments/instrument.py` & `exorad-2.1.94/exorad/models/instruments/instrument.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/models/instruments/photometer.py` & `exorad-2.1.94/exorad/models/instruments/photometer.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,25 +31,30 @@
         self._wavelength_table()
         # self.table['TR'], transmission_data = self._get_transmission()
         # self._add_data_to_built('transmission_data', transmission_data.to_dict())
 
         self.table['QE'], qe_data = self._get_qe()
         self._add_data_to_built('qe_data', qe_data.to_dict())
 
+        psfFilename = None
+        psf_format = None
+
         if 'PSF' in self.description.keys():
             self.debug('PSF found')
             psfFilename = self.description['PSF']['value']
-        else:
-            psfFilename = None
+            if 'format' in self.description['PSF'].keys():
+                psf_format = self.description['PSF']['format']['value']
 
         prf, pixel_rf, extent = binnedPSF(self.description['Fnum_x']['value'],
                                           self.description['Fnum_y']['value'],
                                           self.table['Wavelength'],
-                                          self.description['detector']['delta_pix']['value'],
-                                          filename=psfFilename)
+                                          self.description['detector'][
+                                              'delta_pix']['value'],
+                                          filename=psfFilename,
+                                          format=psf_format)
         self._add_data_to_built('PRF', prf)
         self._add_data_to_built('pixelRF', pixel_rf)
         self._add_data_to_built('extent', extent)
 
         window_size_px = self.description['aperture']['radius']['value'] ** 2 * \
                          self.description['Fnum_x']['value'] * self.table['Wavelength'] * \
                          self.description['Fnum_y']['value'] * self.table['Wavelength'] / \
```

### Comparing `exorad-2.1.86/exorad/models/instruments/spectrometer.py` & `exorad-2.1.94/exorad/models/instruments/spectrometer.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/models/noise.py` & `exorad-2.1.94/exorad/models/noise.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/models/optics/opticalElement.py` & `exorad-2.1.94/exorad/models/optics/opticalElement.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/models/optics/opticalPath.py` & `exorad-2.1.94/exorad/models/optics/opticalPath.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/models/signal.py` & `exorad-2.1.94/exorad/models/signal.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/models/target.py` & `exorad-2.1.94/exorad/models/target.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/models/targetlist.py` & `exorad-2.1.94/exorad/models/targetlist.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/output/hdf5/hdf5.py` & `exorad-2.1.94/exorad/output/hdf5/hdf5.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/output/hdf5/util.py` & `exorad-2.1.94/exorad/output/hdf5/util.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/output/output.py` & `exorad-2.1.94/exorad/output/output.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/tasks/__init__.py` & `exorad-2.1.94/exorad/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/tasks/foregroundHandler.py` & `exorad-2.1.94/exorad/tasks/foregroundHandler.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/tasks/instrumentHandler.py` & `exorad-2.1.94/exorad/tasks/instrumentHandler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from collections import OrderedDict
+
 from astropy.io.misc.hdf5 import read_table_hdf5
 
 from exorad.models.instruments import Photometer, Spectrometer
 from exorad.output.hdf5 import load
 from .task import Task
 
 instruments = {'photometer': Photometer,
@@ -106,22 +108,39 @@
         if self.get_task_param('write'):
             inst = self.get_task_param('output').create_group('payload')
             inst.store_dictionary(self.get_task_param('payload'),
                                   group_name='payload description')
             ch = inst.create_group('channels')
 
         buildInstrument = BuildInstrument()
-        for det in self.get_task_param('payload')['channel'].keys():
+        if isinstance(self.get_task_param('payload')['channel'], OrderedDict):
+            for det in self.get_task_param('payload')['channel'].keys():
+                channel_type = \
+                    self.get_task_param('payload')['channel'][det][
+                        'channelClass'][
+                        'value'].lower()
+                channels[det] = buildInstrument(type=channel_type, name=det,
+                                                description=
+                                                self.get_task_param('payload')[
+                                                    'channel'][det],
+                                                payload=self.get_task_param(
+                                                    'payload'),
+                                                write=False,
+                                                output=None)
+                if self.get_task_param('write'):
+                    channels[det].write(ch)
+        else:
             channel_type = \
-                self.get_task_param('payload')['channel'][det]['channelClass'][
+                self.get_task_param('payload')['channel']['channelClass'][
                     'value'].lower()
+            det = self.get_task_param('payload')['channel']['value']
             channels[det] = buildInstrument(type=channel_type, name=det,
                                             description=
                                             self.get_task_param('payload')[
-                                                'channel'][det],
+                                                'channel'],
                                             payload=self.get_task_param(
                                                 'payload'),
                                             write=False,
                                             output=None)
             if self.get_task_param('write'):
                 channels[det].write(ch)
         self.debug('channels : {}'.format(channels))
```

### Comparing `exorad-2.1.86/exorad/tasks/loadOptions.py` & `exorad-2.1.94/exorad/tasks/loadOptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,18 @@
                 datatype_attr = root_dict['datatype']
                 datatype = datatype_attr['value']
             except:
                 datatype = 'ecsv'
 
             attrValue = root_dict['datafile']
             datafile = attrValue
-            datafile = datafile['value'].replace('__ConfigPath__', self.configPath)
+            if '__ConfigPath__' in datafile['value']:
+                datafile = datafile['value'].replace('__ConfigPath__', self.configPath)
+            else:
+                datafile = datafile['value']
             try:
                 data = self.__read_datatable__(datafile, datatype)
                 root_dict['data'] = data
             except IOError:
                 self.error("Cannot read input file")
                 raise IOError
```

### Comparing `exorad-2.1.86/exorad/tasks/loadSource.py` & `exorad-2.1.94/exorad/tasks/loadSource.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import os
+
 import numpy as np
 from astropy import units as u
 
 from exorad.models.source import Star, CustomSed
 from exorad.tasks.task import Task
-import os
+
 
 class LoadSource(Task):
     """
     Updates target with its source and return the source Sed
 
     Parameters
     ----------
@@ -85,24 +87,38 @@
                 except KeyError:
                     if os.environ.get('PHOENIX_PATH', None) is not None:
                         star_sed_path = os.environ.get('PHOENIX_PATH', None)
                     else:
                         raise IOError('No phoenix path specificed')
 
                 if not os.path.exists(star_sed_path):
-                    raise IOError('Phoenix path does not exist: {}'.format(star_sed_path))
-                    
-                star = Star(star_sed_path,
-                            target.star.D,
-                            target.star.Teff,
-                            target.star.calc_logg(target.star.M, target.star.R),
-                            0.0,
-                            target.star.R,
-                            use_planck_spectrum=False)
-                self.debug('stellar sed used {}'.format(star.filename))
+                    raise IOError('Phoenix path does not exist: {}'.format(
+                        star_sed_path))
+
+                try:
+                    star = Star(star_sed_path,
+                                target.star.D,
+                                target.star.Teff,
+                                target.star.calc_logg(target.star.M,
+                                                      target.star.R),
+                                0.0,
+                                target.star.R,
+                                use_planck_spectrum=False)
+                    self.debug('stellar sed used {}'.format(star.filename))
+                except ValueError:
+                    self.warning(
+                        'stellar temperature out sed boundaries: Planck star used instead')
+                    star = Star('.',
+                                target.star.D,
+                                target.star.Teff,
+                                target.star.calc_logg(target.star.M,
+                                                      target.star.R),
+                                0.0,
+                                target.star.R,
+                                use_planck_spectrum=True)
             else:
                 star = Star('.',
                             target.star.D,
                             target.star.Teff,
                             target.star.calc_logg(target.star.M, target.star.R),
                             0.0,
                             target.star.R,
```

### Comparing `exorad-2.1.86/exorad/tasks/noiseHandler.py` & `exorad-2.1.94/exorad/tasks/noiseHandler.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/tasks/propagateLight.py` & `exorad-2.1.94/exorad/tasks/propagateLight.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/tasks/targetHandler.py` & `exorad-2.1.94/exorad/tasks/targetHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from copy import deepcopy
+
 from exorad.__version__ import __version__
 from exorad.log import disableLogging, enableLogging
-from ..models.targetlist import XLXSTargetList, CSVTargetList, QTableTargetList
 from .task import Task
+from ..models.targetlist import XLXSTargetList, CSVTargetList, QTableTargetList
 
 
 class LoadTargetList(Task):
     """
     Loads target list from file
 
     Parameters
@@ -268,32 +269,31 @@
         self.addTaskParam('wl_range', 'wavelength range to investigate. (wl_min, wl_max)')
         self.addTaskParam('plot', 'allow to save plots')
         self.addTaskParam('out_dir', 'indicate the directory where to save plots')
         self.addTaskParam('n_thread', 'number of threads', 1)
         self.addTaskParam('debug', 'debug mode', False)
 
     def execute(self):
-        from exorad.utils.util import chunks
-        import multiprocessing as mp
-        try:
-            mp.set_start_method('fork')
-        except RuntimeError:
-            pass
-
         targets = self.get_task_param('targets')
         n_thread = self.get_task_param('n_thread')
 
-        manager = mp.Manager()
-        outputDict = manager.dict()
-        for tt in chunks(targets, n_thread):
-            job = [mp.Process(target=self.pipeline_to_dict, args=(target, outputDict)) for target in tt]
-            for j in job:
-                j.start()
-            for j in job:
-                j.join()
+        if n_thread > 1:
+
+            from joblib import Parallel, delayed
+
+            outputDict = {}
+            Parallel(n_jobs=n_thread, require='sharedmem')(
+                delayed(self.pipeline_to_dict)(target, outputDict) for target
+                in targets)
+
+        else:
+            outputDict = {}
+            for target in targets:
+                self.pipeline_to_dict(target, outputDict)
+
         self.set_output(outputDict)
 
     def pipeline_to_dict(self,  target, outputDict):
         from . import ObserveTarget
         from exorad.utils.plotter import Plotter
         import matplotlib.pyplot as plt
         import matplotlib
```

### Comparing `exorad-2.1.86/exorad/tasks/task.py` & `exorad-2.1.94/exorad/tasks/task.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/utils/ascii_art.py` & `exorad-2.1.94/exorad/utils/ascii_art.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/utils/diffuse_light_propagation.py` & `exorad-2.1.94/exorad/utils/diffuse_light_propagation.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/utils/exolib.py` & `exorad-2.1.94/exorad/utils/exolib.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     k_x, k_y = 0.12487792968758*u.micron/u.micron, 0.1248779296875*u.micron/u.micron #hack to make it dimensionless in astropy units
     xmin = -hdr['NAXIS2']/2.*delta_pix
     xmax = hdr['NAXIS2']/2.*delta_pix
     ymin = -hdr['NAXIS1']/2.*delta_pix
     ymax = hdr['NAXIS1']/2.*delta_pix
     extent = (xmin, xmax, ymin, ymax)
     return k_x, k_y, extent
-    
+
 def binnedPSF(F_x, F_y, wl, delta_pix, filename=None, format=None, PSFtype='AIRY'):
     if filename:
         if filename[-5:] == '.fits':
             with fits.open(os.path.expanduser(filename)) as hdu:
                 ima = hdu[0].data
                 hdr = hdu[0].header
                 # define a kernel representing the detector pixel response
@@ -179,28 +179,30 @@
                 ima = hdu[0].data
                 hdr = hdu[0].header
                 if format == 'Twinkle':
                     k_x, k_y, extent=load_twinkle_psf(delta_pix, hdr)
                 else:
                     k_x, k_y, extent=load_standard_psf(F_x, F_y, wl, delta_pix, hdr)
     else:
-        x = np.linspace(-3.0, 3.0, 256)
+        x = np.linspace(-4.0, 4.0, 256)
         xx, yy = np.meshgrid(x, x)
         r = np.pi * np.sqrt(xx ** 2 + yy ** 2) + 1.0e-10
 
         ima = (2.0 * j1(r) / r) ** 2
         ima *= 0.25 * np.pi * (x[1] - x[0]) ** 2
         # print ima.sum()
         k_x = delta_pix / (F_x * wl * (x[1] - x[0]))
         k_y = delta_pix / (F_y * wl * (x[1] - x[0]))
         # print k_y, k_x
         extent = (-(ima.shape[1] // 2) * F_x * wl * (x[1] - x[0]),
                   (ima.shape[1] // 2) * F_x * wl * (x[1] - x[0]),
                   -(ima.shape[0] // 2) * F_y * wl * (x[1] - x[0]),
                   (ima.shape[0] // 2) * F_y * wl * (x[1] - x[0]))
+        # normalise
+        ima /= ima.sum()
 
     fk_x, ik_x = np.modf(k_x)
     fk_y, ik_y = np.modf(k_y)
 
     kernel = np.ones((int(ik_y) + 2, int(ik_x) + 2)) * fk_x.unit
     kernel[:, 0] *= 0.5 * fk_x
     kernel[:, -1] *= 0.5 * fk_x
```

### Comparing `exorad-2.1.86/exorad/utils/mpi.py` & `exorad-2.1.94/exorad/utils/mpi.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/utils/plotter.py` & `exorad-2.1.94/exorad/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad/utils/util.py` & `exorad-2.1.94/exorad/utils/util.py`

 * *Files identical despite different names*

### Comparing `exorad-2.1.86/exorad.egg-info/PKG-INFO` & `exorad-2.1.94/exorad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exorad
-Version: 2.1.86
+Version: 2.1.94
 Summary: The generic point source radiometric model
 Home-page: https://github.com/ExObsSim/ExoRad2-public
 Author: Lorenzo V. Mugnai, Enzo Pascale
 Author-email: lorenzo.mugnai@uniroma1.it
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `exorad-2.1.86/setup.py` & `exorad-2.1.94/setup.py`

 * *Files identical despite different names*

