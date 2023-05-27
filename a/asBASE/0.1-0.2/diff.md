# Comparing `tmp/asBASE-0.1.tar.gz` & `tmp/asBASE-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asBASE-0.1.tar", last modified: Sat May 27 00:11:22 2023, max compression
+gzip compressed data, was "asBASE-0.2.tar", last modified: Sat May 27 12:28:13 2023, max compression
```

## Comparing `asBASE-0.1.tar` & `asBASE-0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-27 00:11:22.910300 asBASE-0.1/
--rw-rw----   0 root         (0) everybody  (9997)       20 2023-05-26 23:55:19.000000 asBASE-0.1/LICENSE.txt
--rw-rw----   0 root         (0) everybody  (9997)      320 2023-05-27 00:11:22.894300 asBASE-0.1/PKG-INFO
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-27 00:11:22.774300 asBASE-0.1/asBASE/
--rw-rw----   0 root         (0) everybody  (9997)     2621 2023-05-26 23:57:13.000000 asBASE-0.1/asBASE/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-27 00:11:22.874300 asBASE-0.1/asBASE.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      320 2023-05-27 00:11:22.000000 asBASE-0.1/asBASE.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      159 2023-05-27 00:11:22.000000 asBASE-0.1/asBASE.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-27 00:11:22.000000 asBASE-0.1/asBASE.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        7 2023-05-27 00:11:22.000000 asBASE-0.1/asBASE.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-27 00:11:22.914300 asBASE-0.1/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      361 2023-05-27 00:09:45.000000 asBASE-0.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-27 12:28:13.090643 asBASE-0.2/
+-rw-rw----   0 root         (0) everybody  (9997)       20 2023-05-26 23:55:19.000000 asBASE-0.2/LICENSE.txt
+-rw-rw----   0 root         (0) everybody  (9997)      320 2023-05-27 12:28:13.066643 asBASE-0.2/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      818 2023-05-27 00:54:02.000000 asBASE-0.2/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-27 12:28:12.926643 asBASE-0.2/asBASE/
+-rw-rw----   0 root         (0) everybody  (9997)     2175 2023-05-27 12:27:19.000000 asBASE-0.2/asBASE/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-27 12:28:13.042643 asBASE-0.2/asBASE.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      320 2023-05-27 12:28:12.000000 asBASE-0.2/asBASE.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      169 2023-05-27 12:28:12.000000 asBASE-0.2/asBASE.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-27 12:28:12.000000 asBASE-0.2/asBASE.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        7 2023-05-27 12:28:12.000000 asBASE-0.2/asBASE.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-27 12:28:13.090643 asBASE-0.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      361 2023-05-27 12:28:01.000000 asBASE-0.2/setup.py
```

