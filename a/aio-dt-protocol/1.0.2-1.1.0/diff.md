# Comparing `tmp/aio_dt_protocol-1.0.2.tar.gz` & `tmp/aio_dt_protocol-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_dt_protocol-1.0.2.tar", last modified: Wed May 24 17:15:45 2023, max compression
+gzip compressed data, was "aio_dt_protocol-1.1.0.tar", last modified: Sat May 27 18:48:58 2023, max compression
```

## Comparing `aio_dt_protocol-1.0.2.tar` & `aio_dt_protocol-1.1.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.876737 aio_dt_protocol-1.0.2/
--rw-rw-rw-   0        0        0     1526 2023-04-05 18:37:56.000000 aio_dt_protocol-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     6547 2023-05-24 17:15:45.876737 aio_dt_protocol-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5803 2023-05-24 17:10:31.000000 aio_dt_protocol-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.803764 aio_dt_protocol-1.0.2/aio_dt_protocol/
--rw-rw-rw-   0        0        0      369 2023-05-24 17:13:28.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/__init__.py
--rw-rw-rw-   0        0        0    10780 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/actions.py
--rw-rw-rw-   0        0        0    56871 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/browser.py
--rw-rw-rw-   0        0        0    22851 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/connection.py
--rw-rw-rw-   0        0        0    25804 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/data.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.809762 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/
--rw-rw-rw-   0        0        0        0 2021-06-02 19:57:07.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.812762 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/background_service/
--rw-rw-rw-   0        0        0      107 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/background_service/__init__.py
--rw-rw-rw-   0        0        0     3279 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/background_service/background_service.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/background_service/types.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.816759 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/browser/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/browser/__init__.py
--rw-rw-rw-   0        0        0    13585 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/browser/browser.py
--rw-rw-rw-   0        0        0     1346 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/browser/types.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.819759 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/css/
--rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/css/__init__.py
--rw-rw-rw-   0        0        0     6353 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/css/css.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/css/types.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.823757 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/device_orientation/
--rw-rw-rw-   0        0        0       51 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/device_orientation/__init__.py
--rw-rw-rw-   0        0        0     1455 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/device_orientation/device_orientation.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/device_orientation/types.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.828756 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/dom/
--rw-rw-rw-   0        0        0       80 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/dom/__init__.py
--rw-rw-rw-   0        0        0    16508 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/dom/dom.py
--rw-rw-rw-   0        0        0    35568 2023-05-24 16:56:17.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/dom/dom_element.py
--rw-rw-rw-   0        0        0      798 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/dom/types.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.831754 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/emulation/
--rw-rw-rw-   0        0        0       73 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/emulation/__init__.py
--rw-rw-rw-   0        0        0    24489 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/emulation/emulation.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/emulation/types.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.834753 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/fetch/
--rw-rw-rw-   0        0        0       57 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/fetch/__init__.py
--rw-rw-rw-   0        0        0    17264 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/fetch/fetch.py
--rw-rw-rw-   0        0        0     5210 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/fetch/types.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.838751 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/input/
--rw-rw-rw-   0        0        0       26 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/input/__init__.py
--rw-rw-rw-   0        0        0    23645 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/input/input.py
--rw-rw-rw-   0        0        0     2778 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/input/types.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.841750 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/log/
--rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/log/__init__.py
--rw-rw-rw-   0        0        0     1701 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/log/log.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/log/types.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.844749 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/network/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/network/__init__.py
--rw-rw-rw-   0        0        0    18941 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/network/network.py
--rw-rw-rw-   0        0        0     3522 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/network/types.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.847748 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/overlay/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/overlay/__init__.py
--rw-rw-rw-   0        0        0     1731 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/overlay/overlay.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/overlay/types.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.851748 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/page/
--rw-rw-rw-   0        0        0       53 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/page/__init__.py
--rw-rw-rw-   0        0        0    33682 2023-05-24 16:56:23.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/page/page.py
--rw-rw-rw-   0        0        0     3104 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/page/types.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.854746 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/runtime/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/runtime/__init__.py
--rw-rw-rw-   0        0        0    23769 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/runtime/runtime.py
--rw-rw-rw-   0        0        0     7629 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/runtime/types.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.857745 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/system_info/
--rw-rw-rw-   0        0        0       37 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/system_info/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/system_info/system_info.py
--rw-rw-rw-   0        0        0      784 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/system_info/types.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.861744 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/target/
--rw-rw-rw-   0        0        0       61 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/target/__init__.py
--rw-rw-rw-   0        0        0    17276 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/target/target.py
--rw-rw-rw-   0        0        0      408 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/domains/target/types.py
--rw-rw-rw-   0        0        0     3409 2023-05-19 09:15:55.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/exceptions.py
--rw-rw-rw-   0        0        0     7275 2023-05-24 16:56:21.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/extend_connection.py
--rw-rw-rw-   0        0        0     5156 2023-05-19 08:54:16.000000 aio_dt_protocol-1.0.2/aio_dt_protocol/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:15:45.808762 aio_dt_protocol-1.0.2/aio_dt_protocol.egg-info/
--rw-rw-rw-   0        0        0     6547 2023-05-24 17:15:45.000000 aio_dt_protocol-1.0.2/aio_dt_protocol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2504 2023-05-24 17:15:45.000000 aio_dt_protocol-1.0.2/aio_dt_protocol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 17:15:45.000000 aio_dt_protocol-1.0.2/aio_dt_protocol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-24 17:15:45.000000 aio_dt_protocol-1.0.2/aio_dt_protocol.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-24 17:15:45.000000 aio_dt_protocol-1.0.2/aio_dt_protocol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-04-06 10:50:43.000000 aio_dt_protocol-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 17:15:45.877737 aio_dt_protocol-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1503 2023-04-06 10:09:07.000000 aio_dt_protocol-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.681686 aio_dt_protocol-1.1.0/
+-rw-rw-rw-   0        0        0     1526 2023-04-05 18:37:56.000000 aio_dt_protocol-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     7959 2023-05-27 18:48:58.681686 aio_dt_protocol-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7215 2023-05-27 15:28:49.000000 aio_dt_protocol-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.317815 aio_dt_protocol-1.1.0/aio_dt_protocol/
+-rw-rw-rw-   0        0        0      503 2023-05-27 17:32:49.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/__init__.py
+-rw-rw-rw-   0        0        0    10780 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/actions.py
+-rw-rw-rw-   0        0        0    56559 2023-05-27 18:33:35.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/browser.py
+-rw-rw-rw-   0        0        0    16843 2023-05-27 14:24:00.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/connection.py
+-rw-rw-rw-   0        0        0    25804 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/data.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.324813 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/
+-rw-rw-rw-   0        0        0        0 2021-06-02 19:57:07.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.327812 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/background_service/
+-rw-rw-rw-   0        0        0      107 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/background_service/__init__.py
+-rw-rw-rw-   0        0        0     3279 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/background_service/background_service.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/background_service/types.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.343807 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/browser/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/browser/__init__.py
+-rw-rw-rw-   0        0        0    13585 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/browser/browser.py
+-rw-rw-rw-   0        0        0     1346 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/browser/types.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.393790 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/css/
+-rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/css/__init__.py
+-rw-rw-rw-   0        0        0     6353 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/css/css.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/css/types.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.396787 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/device_orientation/
+-rw-rw-rw-   0        0        0       51 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/device_orientation/__init__.py
+-rw-rw-rw-   0        0        0     1455 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/device_orientation/device_orientation.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/device_orientation/types.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.432775 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/dom/
+-rw-rw-rw-   0        0        0       80 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/dom/__init__.py
+-rw-rw-rw-   0        0        0    16508 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/dom/dom.py
+-rw-rw-rw-   0        0        0    35568 2023-05-24 16:56:17.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/dom/dom_element.py
+-rw-rw-rw-   0        0        0      798 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/dom/types.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.457767 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/emulation/
+-rw-rw-rw-   0        0        0       73 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/emulation/__init__.py
+-rw-rw-rw-   0        0        0    24489 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/emulation/emulation.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/emulation/types.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.478758 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/fetch/
+-rw-rw-rw-   0        0        0       57 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/fetch/__init__.py
+-rw-rw-rw-   0        0        0    17264 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/fetch/fetch.py
+-rw-rw-rw-   0        0        0     5210 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/fetch/types.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.519743 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/input/
+-rw-rw-rw-   0        0        0       26 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/input/__init__.py
+-rw-rw-rw-   0        0        0    23645 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/input/input.py
+-rw-rw-rw-   0        0        0     2778 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/input/types.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.549733 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/log/
+-rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/log/__init__.py
+-rw-rw-rw-   0        0        0     1701 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/log/log.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/log/types.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.571725 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/network/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/network/__init__.py
+-rw-rw-rw-   0        0        0    18941 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/network/network.py
+-rw-rw-rw-   0        0        0     3522 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/network/types.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.604713 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/overlay/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/overlay/__init__.py
+-rw-rw-rw-   0        0        0     1731 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/overlay/overlay.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/overlay/types.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.626705 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/page/
+-rw-rw-rw-   0        0        0       53 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/page/__init__.py
+-rw-rw-rw-   0        0        0    33682 2023-05-24 16:56:23.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/page/page.py
+-rw-rw-rw-   0        0        0     3104 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/page/types.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.640700 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/runtime/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/runtime/__init__.py
+-rw-rw-rw-   0        0        0    33744 2023-05-27 18:14:28.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/runtime/runtime.py
+-rw-rw-rw-   0        0        0     8104 2023-05-26 16:33:22.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/runtime/types.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.655695 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/system_info/
+-rw-rw-rw-   0        0        0       37 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/system_info/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/system_info/system_info.py
+-rw-rw-rw-   0        0        0      784 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/system_info/types.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.680687 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/target/
+-rw-rw-rw-   0        0        0       61 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/target/__init__.py
+-rw-rw-rw-   0        0        0    17276 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/target/target.py
+-rw-rw-rw-   0        0        0      408 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/domains/target/types.py
+-rw-rw-rw-   0        0        0     3753 2023-05-26 18:01:07.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/exceptions.py
+-rw-rw-rw-   0        0        0     8527 2023-05-27 18:13:13.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/extend_connection.py
+-rw-rw-rw-   0        0        0     5683 2023-05-27 18:33:35.000000 aio_dt_protocol-1.1.0/aio_dt_protocol/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-27 18:48:58.323813 aio_dt_protocol-1.1.0/aio_dt_protocol.egg-info/
+-rw-rw-rw-   0        0        0     7959 2023-05-27 18:48:58.000000 aio_dt_protocol-1.1.0/aio_dt_protocol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2504 2023-05-27 18:48:58.000000 aio_dt_protocol-1.1.0/aio_dt_protocol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 18:48:58.000000 aio_dt_protocol-1.1.0/aio_dt_protocol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-27 18:48:58.000000 aio_dt_protocol-1.1.0/aio_dt_protocol.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-27 18:48:58.000000 aio_dt_protocol-1.1.0/aio_dt_protocol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-04-06 10:50:43.000000 aio_dt_protocol-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 18:48:58.682686 aio_dt_protocol-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1503 2023-04-06 10:09:07.000000 aio_dt_protocol-1.1.0/setup.py
```

### Comparing `aio_dt_protocol-1.0.2/LICENSE` & `aio_dt_protocol-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/PKG-INFO` & `aio_dt_protocol-1.1.0/aio_dt_protocol.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aio_dt_protocol
-Version: 1.0.2
+Name: aio-dt-protocol
+Version: 1.1.0
 Summary: Asynchronous wrapper over Chromium browser debugger protocol.
 Home-page: https://github.com/PieceOfGood/aio_dt_protocol
 Author: PieceOfGood
 Author-email: 78sanchezz@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
@@ -23,68 +23,80 @@
 ```shell
 pip install aio-dt-protocol
 ```
 
 Имеет одну зависимость:
 https://github.com/aaugustin/websockets
 
-И так как всё общение через протокол основано на формате JSON, по желанию можно установить ujson:
+И так как всё общение через протокол основано на формате JSON, по желанию можно установить в окружение ujson:
 https://github.com/ultrajson/ultrajson
 
 ### Примеры:
 
 ```python
 import asyncio
 from aio_dt_protocol import Browser
+from aio_dt_protocol import BrowserName
 from aio_dt_protocol import find_instances
 from aio_dt_protocol.data import KeyEvents
 
 DEBUG_PORT: int = 9222
-BROWSER_NAME: str = "chrome"
+BROWSER_NAME: str = BrowserName.CHROME
+PROFILE_NAME: str = BROWSER_NAME.capitalize() + "_Profile"
 
 
 async def main() -> None:
     # ? Если на указанном порту есть запущенный браузер, происходит подключение.
     if browser_instances := find_instances(DEBUG_PORT, BROWSER_NAME):
-        browser = Browser(debug_port=DEBUG_PORT, browser_pid=browser_instances[DEBUG_PORT])
+        browser = Browser(
+            debug_port=DEBUG_PORT,
+            browser_pid=browser_instances[DEBUG_PORT])
         msg = f"[- CONNECT TO EXIST BROWSER ON {DEBUG_PORT} PORT -]"
 
     # ? Иначе, запуск нового браузера.
     else:
         browser = Browser(
-            debug_port=DEBUG_PORT, browser_exe=BROWSER_NAME
+            debug_port=DEBUG_PORT, browser_exe=BROWSER_NAME,
+            profile_path=PROFILE_NAME
         )
         msg = f"[- LAUNCH NEW BROWSER ON {DEBUG_PORT} PORT -]"
     print(msg)
 
     # ? Будет печатать в консоль всё, что приходит по соединению со страницей.
     # ? Полезно при разработке.
     # async def action_printer(data: dict) -> None:
     #     print(data)
-    # conn = await browser.getPage(callback=action_printer)
-    conn = await browser.getPage()
+    # conn = await browser.waitFirstTab(callback=action_printer)
+    conn = await browser.waitFirstTab()
 
     print("[- GO TO GOOGLE ... -]")
     await conn.Page.navigate("https://www.google.com", )
     print("[- EMULATE INPUT TEXT ... -]")
 
     input_node = await conn.DOM.querySelector("[type=search]")
+    
+    # ? Эмуляция клика в поисковую строку
     await input_node.click()
     await asyncio.sleep(1)
+    
+    # ? Вставка текста
     await conn.Input.insertText("github PieceOfGood")
     await asyncio.sleep(1)
 
+    # ? Эмуляция нажатия клавиши Enter
     await conn.extend.action.sendKeyEvent(KeyEvents.enter)
     await asyncio.sleep(1)
-
+    
+    # ? Нажатие Enter можно заменить кликом по кнопке
+    # ? используя протокол
     # submit_button_selector = "div:not([jsname])>center>[type=submit]:not([jsaction])"
     # submit_button = await conn.DOM.querySelector(submit_button_selector)
     # await submit_button.click()
 
-    # ? Или выполнить клик используя JS
+    # ? Или выполнить клик используя JavaScript
     # click_code = f"""\
     # document.querySelector("{submit_button_selector}").click();
     # """
     # await conn.extend.injectJS(click_code)
 
     print("[- WAIT FOR CLOSE PAGE ... -]")
     # ? Пока соединение существует, цикл выполняется.
@@ -95,75 +107,92 @@
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
 На страницу можно легко зарегистрировать слушателей, которые будут вызываться на стороне клиентского(Python) кода. Для этого необходимо выполнить в браузере JavaScript, передав в `console.info()` JSON-строку из JavaScript-объекта с двумя обязательными полями `func_name` - имя вызываемой python-функции и `args` - список аргументов, которые будут ей переданы. Например:
 
 ```python
-    html = """
+    html = """\
     <html lang="ru">
     <head>
         <meta charset="utf-8" />
         <title>Test application</title>
     </head>
     <body>
         <button id="knopka">Push me</button>
     </body>
     <script>
         const btn = document.querySelector('#knopka');
         btn.addEventListener('click', () => {
-            console.info(JSON.stringify({
-                 func_name: "test_func",
-                 args: [1, "test"]
-            }))
+            py_call("test_func", 1, "test")
         });
     </script>
     </html>"""
-
-
-# ? number и text будут переданы из браузера, а bind_arg указан при регистрации
-async def test_func(number: int, text: str, bind_arg: dict) -> None:
-    print(f"[- test_func -] Called with args:\n\tnumber: {number}\n\ttext: {text}\n\tbing_arg: {bind_arg}")
-
-
-await conn.addListener(
-    test_func,  # ! слушатель
-    {"name": "test", "value": True}  # ! bind_arg
-)
-
-# ? Если ожидается внушительный функционал прикрутить к странице, то это можно
-# ? сделать за один раз.
-# await conn.addListeners(
-#     (test_func, [ {"name": "test", "value": True} ]),
-#     # (any_awaitable1, [1, 2, 3])
-#     # (any_awaitable2, [])
-# )
-
-await conn.Page.navigate(html)
+    
+    # ? Добавляем на страницу `py_call()`
+    await conn.extend.pyCallAddOnload()
+    
+    # ? number и text будут переданы из браузера, а bind_arg указан при регистрации
+    async def test_func(number: int, text: str, bind_arg: dict) -> None:
+        print(f"[- test_func -] Called with args:\n\tnumber: {number}"
+              f"\n\ttext: {text}\n\tbing_arg: {bind_arg}")
+    
+    
+    await conn.bindFunction(
+        test_func,  # ! слушатель
+        {"name": "test", "value": True}  # ! bind_arg
+    )
+    
+    # ? Если ожидается внушительный функционал прикрутить к странице, то это можно
+    # ? сделать за один раз.
+    # await conn.addListeners(
+    #     (test_func, [ {"name": "test", "value": True} ]),
+    #     # (any_awaitable1, [1, 2, 3])
+    #     # (any_awaitable2, [])
+    # )
+    
+    await conn.Page.navigate(html)
 ```
 ### Headless
-Чтобы запустить браузер в `безголовом` режиме, нужно передать аргументу принимающему путь к папке профиля пустую строку.
+Чтобы запустить браузер в безголовом(`headless`) режиме, передайте пустую строку аргументу(`profile_path`) принимающему путь к папке профиля.
 
 ```python
 import asyncio
-from aio_dt_protocol import Browser
+from aio_dt_protocol import Browser, BrowserName, find_instances
 from aio_dt_protocol.utils import save_img_as, async_util_call
 
+DEBUG_PORT: int = 9222
+BROWSER_NAME: str = BrowserName.CHROME
+
 
 async def main() -> None:
-    print("[- HEADLESS RUN -]")
-    browser = Browser(profile_path="")
+    # ? Если на указанном порту есть запущенный браузер, происходит подключение.
+    if browser_instances := find_instances(DEBUG_PORT, BROWSER_NAME):
+        browser = Browser(
+            debug_port=DEBUG_PORT,
+            browser_pid=browser_instances[DEBUG_PORT])
+        msg = f"[- HEADLESS CONNECT TO EXIST BROWSER ON {DEBUG_PORT} PORT -]"
+
+    # ? Иначе, запуск нового браузера.
+    else:
+        browser = Browser(
+            debug_port=DEBUG_PORT, browser_exe=BROWSER_NAME,
+            profile_path=""
+        )
+        msg = f"[- HEADLESS LAUNCH NEW BROWSER ON {DEBUG_PORT} PORT -]"
+    print(msg)
+    
     print("[- WAITING PAGE -]")
     conn = await browser.waitFirstTab()
     print("[- GO TO GOOGLE -]")
     await conn.Page.navigate("https://www.google.com")
 
     print("[- MAKE SCREENSHOT -]")
     await async_util_call(
-        save_img_as, "google.png", await conn.Page.makeScreenshot()
+        save_img_as, "google.png", await conn.extend.makeScreenshot()
     )
 
     print("[- CLOSE BROWSER -]")
     await conn.Browser.close()
     print("[- DONE -]")
```

### Comparing `aio_dt_protocol-1.0.2/README.md` & `aio_dt_protocol-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -4,68 +4,80 @@
 ```shell
 pip install aio-dt-protocol
 ```
 
 Имеет одну зависимость:
 https://github.com/aaugustin/websockets
 
-И так как всё общение через протокол основано на формате JSON, по желанию можно установить ujson:
+И так как всё общение через протокол основано на формате JSON, по желанию можно установить в окружение ujson:
 https://github.com/ultrajson/ultrajson
 
 ### Примеры:
 
 ```python
 import asyncio
 from aio_dt_protocol import Browser
+from aio_dt_protocol import BrowserName
 from aio_dt_protocol import find_instances
 from aio_dt_protocol.data import KeyEvents
 
 DEBUG_PORT: int = 9222
-BROWSER_NAME: str = "chrome"
+BROWSER_NAME: str = BrowserName.CHROME
+PROFILE_NAME: str = BROWSER_NAME.capitalize() + "_Profile"
 
 
 async def main() -> None:
     # ? Если на указанном порту есть запущенный браузер, происходит подключение.
     if browser_instances := find_instances(DEBUG_PORT, BROWSER_NAME):
-        browser = Browser(debug_port=DEBUG_PORT, browser_pid=browser_instances[DEBUG_PORT])
+        browser = Browser(
+            debug_port=DEBUG_PORT,
+            browser_pid=browser_instances[DEBUG_PORT])
         msg = f"[- CONNECT TO EXIST BROWSER ON {DEBUG_PORT} PORT -]"
 
     # ? Иначе, запуск нового браузера.
     else:
         browser = Browser(
-            debug_port=DEBUG_PORT, browser_exe=BROWSER_NAME
+            debug_port=DEBUG_PORT, browser_exe=BROWSER_NAME,
+            profile_path=PROFILE_NAME
         )
         msg = f"[- LAUNCH NEW BROWSER ON {DEBUG_PORT} PORT -]"
     print(msg)
 
     # ? Будет печатать в консоль всё, что приходит по соединению со страницей.
     # ? Полезно при разработке.
     # async def action_printer(data: dict) -> None:
     #     print(data)
-    # conn = await browser.getPage(callback=action_printer)
-    conn = await browser.getPage()
+    # conn = await browser.waitFirstTab(callback=action_printer)
+    conn = await browser.waitFirstTab()
 
     print("[- GO TO GOOGLE ... -]")
     await conn.Page.navigate("https://www.google.com", )
     print("[- EMULATE INPUT TEXT ... -]")
 
     input_node = await conn.DOM.querySelector("[type=search]")
+    
+    # ? Эмуляция клика в поисковую строку
     await input_node.click()
     await asyncio.sleep(1)
+    
+    # ? Вставка текста
     await conn.Input.insertText("github PieceOfGood")
     await asyncio.sleep(1)
 
+    # ? Эмуляция нажатия клавиши Enter
     await conn.extend.action.sendKeyEvent(KeyEvents.enter)
     await asyncio.sleep(1)
-
+    
+    # ? Нажатие Enter можно заменить кликом по кнопке
+    # ? используя протокол
     # submit_button_selector = "div:not([jsname])>center>[type=submit]:not([jsaction])"
     # submit_button = await conn.DOM.querySelector(submit_button_selector)
     # await submit_button.click()
 
-    # ? Или выполнить клик используя JS
+    # ? Или выполнить клик используя JavaScript
     # click_code = f"""\
     # document.querySelector("{submit_button_selector}").click();
     # """
     # await conn.extend.injectJS(click_code)
 
     print("[- WAIT FOR CLOSE PAGE ... -]")
     # ? Пока соединение существует, цикл выполняется.
@@ -76,75 +88,92 @@
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
 На страницу можно легко зарегистрировать слушателей, которые будут вызываться на стороне клиентского(Python) кода. Для этого необходимо выполнить в браузере JavaScript, передав в `console.info()` JSON-строку из JavaScript-объекта с двумя обязательными полями `func_name` - имя вызываемой python-функции и `args` - список аргументов, которые будут ей переданы. Например:
 
 ```python
-    html = """
+    html = """\
     <html lang="ru">
     <head>
         <meta charset="utf-8" />
         <title>Test application</title>
     </head>
     <body>
         <button id="knopka">Push me</button>
     </body>
     <script>
         const btn = document.querySelector('#knopka');
         btn.addEventListener('click', () => {
-            console.info(JSON.stringify({
-                 func_name: "test_func",
-                 args: [1, "test"]
-            }))
+            py_call("test_func", 1, "test")
         });
     </script>
     </html>"""
-
-
-# ? number и text будут переданы из браузера, а bind_arg указан при регистрации
-async def test_func(number: int, text: str, bind_arg: dict) -> None:
-    print(f"[- test_func -] Called with args:\n\tnumber: {number}\n\ttext: {text}\n\tbing_arg: {bind_arg}")
-
-
-await conn.addListener(
-    test_func,  # ! слушатель
-    {"name": "test", "value": True}  # ! bind_arg
-)
-
-# ? Если ожидается внушительный функционал прикрутить к странице, то это можно
-# ? сделать за один раз.
-# await conn.addListeners(
-#     (test_func, [ {"name": "test", "value": True} ]),
-#     # (any_awaitable1, [1, 2, 3])
-#     # (any_awaitable2, [])
-# )
-
-await conn.Page.navigate(html)
+    
+    # ? Добавляем на страницу `py_call()`
+    await conn.extend.pyCallAddOnload()
+    
+    # ? number и text будут переданы из браузера, а bind_arg указан при регистрации
+    async def test_func(number: int, text: str, bind_arg: dict) -> None:
+        print(f"[- test_func -] Called with args:\n\tnumber: {number}"
+              f"\n\ttext: {text}\n\tbing_arg: {bind_arg}")
+    
+    
+    await conn.bindFunction(
+        test_func,  # ! слушатель
+        {"name": "test", "value": True}  # ! bind_arg
+    )
+    
+    # ? Если ожидается внушительный функционал прикрутить к странице, то это можно
+    # ? сделать за один раз.
+    # await conn.addListeners(
+    #     (test_func, [ {"name": "test", "value": True} ]),
+    #     # (any_awaitable1, [1, 2, 3])
+    #     # (any_awaitable2, [])
+    # )
+    
+    await conn.Page.navigate(html)
 ```
 ### Headless
-Чтобы запустить браузер в `безголовом` режиме, нужно передать аргументу принимающему путь к папке профиля пустую строку.
+Чтобы запустить браузер в безголовом(`headless`) режиме, передайте пустую строку аргументу(`profile_path`) принимающему путь к папке профиля.
 
 ```python
 import asyncio
-from aio_dt_protocol import Browser
+from aio_dt_protocol import Browser, BrowserName, find_instances
 from aio_dt_protocol.utils import save_img_as, async_util_call
 
+DEBUG_PORT: int = 9222
+BROWSER_NAME: str = BrowserName.CHROME
+
 
 async def main() -> None:
-    print("[- HEADLESS RUN -]")
-    browser = Browser(profile_path="")
+    # ? Если на указанном порту есть запущенный браузер, происходит подключение.
+    if browser_instances := find_instances(DEBUG_PORT, BROWSER_NAME):
+        browser = Browser(
+            debug_port=DEBUG_PORT,
+            browser_pid=browser_instances[DEBUG_PORT])
+        msg = f"[- HEADLESS CONNECT TO EXIST BROWSER ON {DEBUG_PORT} PORT -]"
+
+    # ? Иначе, запуск нового браузера.
+    else:
+        browser = Browser(
+            debug_port=DEBUG_PORT, browser_exe=BROWSER_NAME,
+            profile_path=""
+        )
+        msg = f"[- HEADLESS LAUNCH NEW BROWSER ON {DEBUG_PORT} PORT -]"
+    print(msg)
+    
     print("[- WAITING PAGE -]")
     conn = await browser.waitFirstTab()
     print("[- GO TO GOOGLE -]")
     await conn.Page.navigate("https://www.google.com")
 
     print("[- MAKE SCREENSHOT -]")
     await async_util_call(
-        save_img_as, "google.png", await conn.Page.makeScreenshot()
+        save_img_as, "google.png", await conn.extend.makeScreenshot()
     )
 
     print("[- CLOSE BROWSER -]")
     await conn.Browser.close()
     print("[- DONE -]")
```

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/actions.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/actions.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/browser.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/browser.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,21 @@
     HAS_UJSON = False
     import json
 import warnings
 import re, os, sys, signal, subprocess
 from urllib.parse import quote
 from os.path import expanduser
 from inspect import iscoroutinefunction
-from typing import List, Dict, Union, Optional, Tuple
+from typing import List, Dict, Union, Optional, Tuple, Literal
 from collections.abc import Sequence
 from enum import Enum
 from .connection import Connection
 from .data import TargetConnectionInfo, TargetConnectionType, CommonCallback
 from .exceptions import FlagArgumentContainError, NoTargetWithGivenIdFound
-from .utils import get_request, registry_read_key, log, async_util_call
+from .utils import get_request, find_browser_executable_path, log, async_util_call
 
 
 class Browser:
 
     def __init__(
             self,
             profile_path: str = "testProfile",
@@ -52,56 +52,53 @@
                                     несуществующий путь, он будет создан.
 
                                         [-!!!-] ВАЖНО [-!!!-] - для запуска в режиме "headless",
                                         в "profile_path" нужно передать пустую строку.
 
         :param dev_tool_profiles:   Если 'profile_path' указан как имя папки, а не путь,
                                     профиль с указанным именем будет создан/получен в домашней
-                                    дирректории пользователя, из каталога 'DevTools_Profiles',
+                                    директории пользователя, из каталога 'DevTools_Profiles',
                                     если значение установлено в True. (Linux, Windows)
 
         :param url:             Адрес, которым будет инициирован старт браузера.
                                     Со значением по умолчанию, будет открыта пустая страница.
 
-        :param flags:           Список аргументов командной строки. Например:
-                                    [ "--no-first-run", "--no-default-browser-check", "--browser-test",
-                                    "--window-position=400,100", "--window-size=800,600", ... ]
+        :param flags:           Экземпляр `FlagBuilder()` напичканный `CMDFlags()`.
                                     https://peter.sh/experiments/chromium-command-line-switches/
 
-        :param browser_path:    Путь до исполняемого файла браузера. Если не указан, в реестре
-                                    будет произведён поиск установленного браузера Chrome.
+        :param browser_path:    Путь до исполняемого файла браузера. Имеет приоритет над
+                                    аргументом `browser_exe`.
 
         :param debug_port:      Используется порт по умолчанию 9222.
 
-        :param browser_pid:     ProcessID браузера. Используется методом KillChrome(). Если
+        :param browser_pid:     ProcessID браузера. Используется методом kill(). Если
                                     передано значение большее нуля, считается, что производится
-                                    подключение к уже существующему инстансу браузера. Подробнее
-                                    в описании статического метода FindInstances().
+                                    подключение к уже существующему экземпляру браузера. Чтобы
+                                    найти запущенный браузер в режиме отладки, воспользуйтесь
+                                    `find_instances()`.
 
         :param app:             Запускает браузер в окне без пользовательского интерфейса,
                                     вроде адресной строки, кнопок навигации и прочих атрибутов.
-                                    Распространяется только на первый инстанс страниц браузера,
-                                    что означает, что все следующие инстансы будут открываться
-                                    в интерфейсе страниц браузера, в отдельном от первого окне.
+                                    Распространяется только на первую страницу браузера. Прочие
+                                    страницы будут открываться в обычном виде и в отдельном
+                                    от первого окне.
 
         :param browser_exe:     Имя исполняемого файла браузера, который будет автоматизирован.
                                     Например: chrome, brave. Если 'browser_path' окажется пустым,
-                                    путь до исполняемого файла будет найден в реестре.
+                                    будет произведена попытка найти его в системе по этому имени.
 
         :param proxy_port:      Если установлено, браузер будет запущен с флагом 'proxy' и
                                     все его запросы будут перенаправляться на этот порт, на
                                     локальном хосте.
 
         :param verbose:         Печатать некие подробности процесса?
 
         :param position:        Кортеж с иксом и игреком, в которых откроется окно браузера.
-                                    Не имеет смысла для Headless.
 
         :param sizes:           Кортеж с длиной и шириной в которые будет установлено окно браузера.
-                                    Не имеет смысла для Headless.
 
         :param prevent_restore: Предотвращать восстановление предыдущей сессии после крашей.
         """
         if sys.platform not in ("win32", "linux"): raise OSError(f"Platform '{sys.platform}' — not supported")
         self.dev_tool_profiles = dev_tool_profiles if profile_path else False
 
         if verbose and not HAS_UJSON:
@@ -146,32 +143,32 @@
             self.browser_name = "chrome"
             browser_exe = "chrome" if sys.platform == "win32" else "google-chrome"
         elif browser_exe == "brave":
             self.browser_name = "brave"
             browser_exe = "brave" if sys.platform == "win32" else "brave-browser"
         elif browser_exe == "chromium":
             self.browser_name = "chrome"
-            browser_exe = "chrome" if sys.platform == "win32" else "chromium-browser"
+            browser_exe = "chromium" if sys.platform == "win32" else "chromium-browser"
         elif "edge" in browser_exe:
             self.browser_name = "edge"
-            browser_exe = "msedge" if sys.platform == "win32" else "msedge" # !?
+            browser_exe = "msedge" if sys.platform == "win32" else "microsoft-edge"
 
         # ? Константы URL соответствующих вкладок
         self.NEW_TAB:       str = self.browser_name + "://newtab/"          # дефолтная вкладка
         self.SETTINGS:      str = self.browser_name + "://settings/"        # настройки
         self.BRAVE_REWARDS: str = self.browser_name + "://rewards/"         # вознаграждения (brave only)
         self.HISTORY:       str = self.browser_name + "://history/"         # история переходов
         self.BOOKMARKS:     str = self.browser_name + "://bookmarks/"       # закладки
         self.DOWNLOADS:     str = self.browser_name + "://downloads/"       # загрузки
         self.WALLET:        str = self.browser_name + "://wallet/"          # кошельки (brave only)
         self.EXTENSIONS:    str = self.browser_name + "://extensions/"      # расширения
         self.FLAGS:         str = self.browser_name + "://flags/"           # экспериментальные технологии
 
         if sys.platform == "win32":
-            browser_path = browser_path if browser_path else registry_read_key(browser_exe)
+            browser_path = browser_path if browser_path else find_browser_executable_path(browser_exe)
         else:   #  ! sys.platform == "linux"
             browser_path = browser_path if browser_path else os.popen("which " + browser_exe).read().strip()
 
         if not os.path.exists(browser_path) or not os.path.isfile(browser_path):
             raise FileNotFoundError(f"Переданный 'browser_path' => '{browser_path}' — не существует, или содержит ошибку")
         self.browser_path = browser_path
 
@@ -212,18 +209,18 @@
                     # или передать "как есть", раз это строка содержащая url
                     if type(url) is str and "http" == url[:4] or self.browser_name == url[:b_name_len] else
                         # иначе декодировать и установить её как Base64
                         "data:text/html;Base64," + url.decode()
         )
 
         self.is_headless_mode = False
-        self.browser_pid = browser_pid if browser_pid > 0 else self._RunBrowser(_url_, flags, position, sizes)
+        self.browser_pid = browser_pid if browser_pid > 0 else self._run_browser(_url_, flags, position, sizes)
 
-    def _RunBrowser(self, url: str, flags: "FlagBuilder", position: Optional[Tuple[int, int]] = None,
-                    sizes: Optional[Tuple[int, int]] = None) -> int:
+    def _run_browser(self, url: str, flags: "FlagBuilder", position: Optional[Tuple[int, int]] = None,
+                     sizes: Optional[Tuple[int, int]] = None) -> int:
         """
         Запускает браузер с переданными флагами.
         :param url:             Адрес. Если передан, будет загружен в первой вкладке.
         :param flags:           Флаги
         :return:                ProcessID запущенного браузера
         """
         flag_box = FlagBuilder()
@@ -268,41 +265,41 @@
             if self.verbose:
                 log(f"Run browser {self.browser_name!r} on port: {self.debug_port}")
 
         if flags is not None:
             flag_box += flags
 
         run_args += flag_box.flags()
-        return subprocess.Popen(run_args).pid
+
+        pipe = subprocess.PIPE if not self.verbose else None
+        return subprocess.Popen(run_args, stdout=pipe, stderr=pipe).pid
 
     def kill(self) -> None:
         """  Убивает процесс браузера. """
         try:
             os.kill(self.browser_pid, signal.SIGTERM)
         except PermissionError:
             pass
 
-    async def getTargetConnectionInfoList(self) -> List[TargetConnectionInfo]:
-        return [TargetConnectionInfo(**i) for i in await self.getPageList()]
-
-    async def getTargetConnectionInfo(
-            self, key: str = "type",
-            connection_type: Union[str, TargetConnectionType] = "page") -> TargetConnectionInfo:
-        v = connection_type if type(connection_type) is str else connection_type.value
-        for page_data in await self.getPageList():
-            data = page_data[key]
-            if v in data: return TargetConnectionInfo(**page_data)
-        raise ValueError(f"No have value {v} for key {key} in active target list")
+    async def getAllTargetsConnectionInfo(self) -> List[TargetConnectionInfo]:
+        """ Возвращает список описаний соединений со всеми
+        существующими типами соединений.
+        """
+        return [TargetConnectionInfo(**i) for i in await self.getConnectionList()]
 
     async def getConnectionsByType(
-            self, connection_type: Union[str, TargetConnectionType]) -> List[TargetConnectionInfo]:
-        t = connection_type if type(connection_type) is str else connection_type.value
-        return [ti for ti in await self.getTargetConnectionInfoList() if ti.type == t]
+            self, conn_type: Union[str, TargetConnectionType]) -> List[TargetConnectionInfo]:
+        """ Возвращает список описаний соединений, удовлетворяющих
+        запрошенному типу соединения.
+        :param conn_type:     Тип соединения. Например: "page"
+        """
+        t = conn_type if type(conn_type) is str else conn_type.value
+        return [ti for ti in await self.getAllTargetsConnectionInfo() if ti.type == t]
 
-    async def getPageList(self) -> List[dict]:
+    async def getConnectionList(self) -> List[dict]:
         """
         Запрашивает у браузера список всех его дочерних процессов,
         включая табы(вкладки/страницы), воркеры, расширения, сервисы и прочее.
 
         :return: [ {
                     "description": "",
                     "devtoolsFrontendUrl": "/devtools/inspector.html?ws=localhost:9222/devtools/page/DAB7FB6187B554E10B0BD18821265734",
@@ -315,46 +312,45 @@
         """
         result = await async_util_call(
             get_request, f"http://127.0.0.1:{self.debug_port}/json/list")
 
         if self.verbose: log("GetPageList() => " + result)
         return json.loads(result)
 
-    async def getPageBy(
+    async def getConnectionBy(
             self, key: Union[str, int],
             value: Union[str, int],
-            match_mode: str = "exact",
+            match_mode: Literal["exact", "contains", "startswith"] = "exact",
             index: int = 0,
-            callback: CommonCallback = None
-    ) -> Optional[Connection]:
+            callback: CommonCallback = None) -> Optional[Connection]:
         """
-        Организует выбор нужного инстанса из процессов браузера по следующим критериям:
+        Организует выбор нужного соединения из процессов браузера по следующим критериям:
         :param key:                 По ключу из словаря. Список ключей смотри
                                         в возвращаемых значениях GetPageList()
         :param value:               Значение ключа, которому должен соответствовать выбор
         :param match_mode:          Значение ключа:
                                         "exact"      - полностью совпадает с value,
                                         "contains"   - содержит value,
                                         "startswith" - начинается с value
-        :param index:               Поскольку открытых страниц с одинаковым ключём может
+        :param index:               Поскольку открытых страниц с одинаковым ключом может
                                         быть несколько, предоставляется возможность выбрать
                                         по индексу. По умолчанию = 0
         :param callback:            Корутина, которой будет передаваться контекст абсолютно
                                         всех событий страницы в виде словаря. Если передан,
                                         включает уведомления домена "Runtime" для общения
                                         со страницей.
 
         :return:        <Connection>
         """
 
         if callback is not None and not iscoroutinefunction(callback):
             raise TypeError("Argument 'callback' must be a coroutine")
 
         counter = 0; v = value.lower()
-        for page_data in await self.getPageList():
+        for page_data in await self.getConnectionList():
             data = page_data[key]
             if ((match_mode == "exact" and data == v)
                 or (match_mode == "contains" and data.find(v) > -1 )
                     or (match_mode == "startswith" and data.find(v) == 0)):
                 if counter == index:
                     conn = Connection(
                         page_data["webSocketDebuggerUrl"],
@@ -367,219 +363,220 @@
                     )
 
                     await conn.activate()
                     return conn
                 counter += 1
         return None
 
-    async def getPage(
-            self,
-            index: int = 0, page_type: str = "page",
-            callback: CommonCallback = None
-    ) -> "Connection":
+    async def getConnection(
+            self, index: int = 0,
+            conn_type: str = "page",
+            callback: CommonCallback = None) -> Connection:
         """
         Получает страницу браузера по индексу. По умолчанию, первую.
         :param index:       - Желаемый индекс страницы начиная с нуля.
-        :param page_type:   - Тип "page" | 'background_page' | 'service_worker' | ???
+        :param conn_type:   - Тип "page" | 'background_page' | 'service_worker' | ???
         :param callback:    - Корутина, которой будет передаваться контекст абсолютно
                                 всех событий страницы в виде словаря.
         :return:        <Connection>
         """
-        return await self.getPageBy("type", page_type, "exact", index, callback)
+        return await self.getConnectionBy("type", conn_type, "exact", index, callback)
 
-    async def getPageByID(
+    async def getConnectionByID(
             self, conn_id: str,
-            callback: CommonCallback = None
-    ) -> "Connection":
+            callback: CommonCallback = None) -> Connection:
         """
         Получает страницу браузера по уникальному идентификатору.
-        :param conn_id:     - Желаемый идентификатор страницы. Метод GetPageList()
-                                возвращает список доступных инстансов и словарь
-                                каждого из них содержит 'id'. Так же создание инстансов
-                                страниц через домен 'Target' возвращает 'targetId',
-                                который используется с этой же целью.
+        :param conn_id:     - Желаемый идентификатор страницы. Он же 'targetId'.
         :param callback:    - Корутина, которой будет передаваться контекст абсолютно
                                 всех событий страницы в виде словаря.
         :return:        <Connection>
         """
-        return await self.getPageBy("id", conn_id, "exact", 0, callback)
+        return await self.getConnectionBy("id", conn_id, "exact", 0, callback)
 
-    async def getPageByTitle(
+    async def getConnectionByTitle(
             self, value: str,
-            match_mode: str = "startswith",
+            match_mode: Literal["exact", "contains", "startswith"] = "startswith",
             index: int = 0,
-            callback: CommonCallback = None
-    ) -> "Connection":
+            callback: CommonCallback = None) -> Connection:
         """
         Получает страницу браузера по заголовку. По умолчанию, первую.
         :param value:       - Текст, который будет сопоставляться при поиске.
         :param match_mode:  - Тип сопоставления(по умолчанию 'startswith').
                                 Может быть только:
                                     * exact      - полное соответствие заголовка и value
                                     * contains   - заголовок содержит value
                                     * startswith - заголовок начинается с value
         :param index:       - Желаемый индекс страницы начиная с нуля.
         :param callback:    - Корутина, которой будет передаваться контекст абсолютно
                                 всех событий страницы в виде словаря.
         :return:        <Connection>
         """
-        return await self.getPageBy("title", value, match_mode, index, callback)
+        return await self.getConnectionBy("title", value, match_mode, index, callback)
 
-    async def getPageByURL(
+    async def getConnectionByURL(
             self, value: str,
-            match_mode: str = "startswith",
+            match_mode: Literal["exact", "contains", "startswith"] = "startswith",
             index: int = 0,
-            callback: CommonCallback = None
-    ) -> "Connection":
+            callback: CommonCallback = None) -> Connection:
         """
         Получает страницу браузера по её URL. По умолчанию, первую.
         :param value:       - Текст, который будет сопоставляться при поиске.
         :param match_mode:  - Тип сопоставления(по умолчанию 'startswith').
                                 Может быть только:
                                     * exact      - полное соответствие URL и value
                                     * contains   - URL содержит value
                                     * startswith - URL начинается с value
         :param index:       - Желаемый индекс страницы начиная с нуля.
         :param callback:    - Корутина, которой будет передаваться контекст абсолютно
                                 всех событий страницы в виде словаря.
         :return:        <Connection>
         """
-        return await self.getPageBy("url", value, match_mode, index, callback)
+        return await self.getConnectionBy("url", value, match_mode, index, callback)
 
-    async def createPage(
+    async def createTab(
             self, url: str = "about:blank",
             newWindow: bool = False,
             background: bool = False,
             wait_for_create: bool = True,
-            callback: CommonCallback = None
-    ) -> Optional[Connection]:
+            callback: CommonCallback = None) -> Optional[Connection]:
         """
         Создаёт новую вкладку в браузере.
         :param url:                     - (optional) Адрес будет открыт при создании.
         :param newWindow:               - (optional) Если 'True' — страница будет открыта в новом окне.
         :param background:              - (optional) Если 'True' — страница будет открыта в фоне.
         :return:                    * <Connection>
         """
-        while not (tmp := await self.getPage(callback=callback)):
+        while not (tmp := await self.getConnection(callback=callback)):
             await asyncio.sleep(.5)
         page_id = await tmp.Target.createTarget(url, newWindow=newWindow, background=background)
         if wait_for_create:
-            while not (page := await self.getPageByID(page_id)):
+            while not (page := await self.getConnectionByID(page_id)):
                 await asyncio.sleep(.5)
         else:
-            page = await self.getPageByID(page_id)
+            page = await self.getConnectionByID(page_id)
         return page
     
-    async def showInspector(self, conn: Connection, new_window: bool = True,
-                            callback: CommonCallback = None) -> Optional[Connection]:
+    async def showInspector(
+            self, conn: Connection,
+            new_window: bool = True,
+            callback: CommonCallback = None) -> Optional[Connection]:
         """
         Открывает новую вкладку с дебаггером для инспектируемой страницы.
         :param conn:            - Инспектируемая страница. Может принадлежать любому браузеру.
         :param new_window:      - Создать target в отдельном окне?
         :return:        <Connection>
         """
-        return await self.createPage(
+        return await self.createTab(
             "http://127.0.0.1:" + str(self.debug_port) + conn.frontend_url, new_window, callback=callback
         )
 
-    async def createPopupWindow(self, conn: Connection, url: str = "about:blank",
-                                callback: CommonCallback = None) -> Optional[Connection]:
-        """
-        Создаёт всплывающее окно с минимумом интерфейса браузера".
+    async def createPopupWindow(
+            self, conn: Connection,
+            url: str = "about:blank",
+            callback: CommonCallback = None) -> Optional[Connection]:
+        """ Создаёт всплывающее окно с минимумом интерфейса браузера".
         :param url:             - Адрес, ресурс которого будет загружен
         :param conn:            - Родительская страница, инициатор
         :return:        Connection or None
         """
-        await conn.extend.injectJS(f'window.open("{url}", "blank_window_name", "popup,noopener,noreferrer");')
-        return await self.getPageByOpener(conn, callback=callback)
-
-    async def getPageByOpener(self, conn: Connection, callback: CommonCallback = None) -> Optional[Connection]:
-        """
-        Возвращает последний созданный инстанс страницы, открытие которого инициировано с конкретной страницы.
-            Например, при использовании JavaScript "window.open()".
+        await conn.extend.injectJS(
+            f'window.open("{url}", "blank_window_name", "popup,noopener,noreferrer");')
+        return await self.getConnectionByOpener(conn, callback=callback)
+
+    async def getConnectionByOpener(
+            self, conn: Connection,
+            callback: CommonCallback = None) -> Optional[Connection]:
+        """ Возвращает последнее созданное соединение со страницей, открытие которого
+        инициировано с конкретной страницы. Например, при использовании JavaScript
+        "window.open()".
         :param conn:            - Родительская страница, инициатор
         :return:        Connection or None
         """
         for target_info in await conn.Target.getTargets():
             if target_info.openerId == conn.conn_id:
-                return await self.getPageByID(target_info.targetId, callback=callback)
+                return await self.getConnectionByID(target_info.targetId, callback=callback)
         return None
 
-    async def getPagesByOpener(self, conn: Connection, callback: CommonCallback = None) -> List[Connection]:
-        """
-        Возвращает список всех инстансов страниц, открытие которых инициировано с конкретной страницы.
-            Например, при использовании JavaScript "window.open()".
+    async def getConnectionsByOpener(
+            self, conn: Connection,
+            callback: CommonCallback = None) -> List[Connection]:
+        """ Возвращает список всех соединений, открытие которых инициировано с конкретной
+        страницы. Например, при использовании JavaScript "window.open()".
         :param conn:            - Родительская страница, инициатор открытых окон
         :return:        List[Connection]
         """
-        pages = []
+        connections = []
         for target_info in await conn.Target.getTargets():
             if target_info.openerId == conn.conn_id:
-                pages.append(await self.getPageByID(target_info.targetId, callback=callback))
-        return pages
-
-    async def waitFirstTab(self, timeout: float = 20.0, callback: CommonCallback = None) -> Connection:
-        """
-        Вызывает исключение 'asyncio.exceptions.TimeoutError' по истечении таймаута, или возвращает инстанс.
+                connections.append(await self.getConnectionByID(
+                    target_info.targetId, callback=callback))
+        return connections
+
+    async def waitFirstTab(
+            self, timeout: float = 20.0,
+            callback: CommonCallback = None) -> Connection:
+        """ Дожидается получения соединения или вызывает исключение
+        'asyncio.exceptions.TimeoutError' по истечении таймаута.
         """
         return await asyncio.wait_for(self.getFirstTab(callback), timeout)
 
     async def getFirstTab(self, callback: CommonCallback = None) -> Connection:
         """
         Безусловно дожидается соединения со страницей.
         """
         while True:
             try:
-                while (conn := await self.getPage(callback=callback)) is None:
+                while (conn := await self.getConnection(callback=callback)) is None:
                     await asyncio.sleep(.5)
                 return conn
             except URLError: await asyncio.sleep(1)
 
     async def close(self) -> None:
         """ Корректно закрывает браузер если остались ещё его инстансы """
-        if conn := await self.getPage():
+        if conn := await self.getConnection():
             await conn.Browser.close()
 
-    async def closeAllPagesExcept(self, *except_list: Connection) -> None:
-        """ Закрывает все страницы браузера, кроме переданных """
-        for conn in await self.getTargetConnectionInfoList():
-            if conn.type == "page":
+    async def closeAllTabsExcept(self, *except_list: Connection) -> None:
+        """ Закрывает все страницы браузера, кроме переданных. """
+        for conn_info in await self.getAllTargetsConnectionInfo():
+            if conn_info.type == "page":
                 condition = False
                 for conn in except_list:
-                    condition |= conn.conn_id == conn._id
+                    condition |= conn.conn_id == conn_info.id
                 if not condition:
                     i = 4
                     try:
-                        while (tab := await self.getPageByID(conn._id)) is None and i:
+                        while (tab := await self.getConnectionByID(conn_info.id)) is None and i:
                             await asyncio.sleep(.5)
                             i -= 1
                         if tab: await tab.Target.close()
                     except NoTargetWithGivenIdFound:
                         pass
 
     async def getFramesFor(self, conn: Connection) -> List[Connection]:
-        """ Возвращает список iFrame для указанного инстанса """
-        result = []
-        for data in await self.getPageList():
-            if data["type"] == "iframe" and data["parentId"] == conn.conn_id:
-                result.append(await self.getPageByID(data["id"]))
-        return result
+        """ Возвращает список iFrame для указанного соединения. """
+        return [
+            await self.getConnectionByID(data["id"])
+            for data in await self.getConnectionList()
+            if data["type"] == "iframe" and data["parentId"] == conn.conn_id
+        ]
 
     def __eq__(self, other: "Browser") -> bool:
         return self.debug_port == other.debug_port
 
     def __hash__(self) -> int:
         return hash(self.debug_port)
 
 
 class FlagBuilder:
     """ Обеспечивает последовательность неповторяющихся флагов
     для запуска браузера.
     """
-    def __init__(self):
+    def __init__(self) -> None:
         self._flags: Dict[str, Tuple[str]] = {}
 
     def add(self, flag: "CMDFlag", *args: Union[str, int, float]) -> None:
         """ Принимает один флаг и его аргументы. """
         f: str = flag.value
         if f[-1] == "=":
             if not args:
@@ -604,21 +601,24 @@
     def custom(self, flag: str) -> None:
         """ Принимает строку в качестве флага.
         object.custom("--mute-audio")
         """
         self._flags[flag] = tuple()
 
     def flags(self) -> List[str]:
-        result: List[str] = []
-        for cmd_flag, args in self._flags.items():
-            result.append(cmd_flag + ",".join(args))
-        return result
+        """ Возвращает форматированный список флагов
+        для запуска процесса браузера.
+        """
+        return [
+            cmd_flag + ",".join(args)
+            for cmd_flag, args in self._flags.items()
+        ]
 
     def __str__(self) -> str:
-        return str(self.flags())
+        return "[\n" + ",\n\t".join(self.flags()) + "\n]"
 
     def __add__(self, other: "FlagBuilder") -> "FlagBuilder":
         if not isinstance(other, FlagBuilder):
             raise TypeError(f"Ожидаемый тип: {self.__class__.__name__}; "
                             f"полученный тип: {other.__class__.__name__}")
 
         flags = {}
```

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/connection.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/connection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 try:
     import ujson as json
 except ModuleNotFoundError:
     import json
 import asyncio
 from websockets.client import WebSocketClientProtocol, connect
+from websockets.exceptions import ConnectionClosedError
+from inspect import iscoroutinefunction
+from typing import Callable, Optional, Union, Tuple, Dict, Any, Iterable, Coroutine
 
-from .exceptions import EvaluateError, get_cdtp_error, highlight_eval_error, PromiseEvaluateError, \
-    highlight_promise_error
+from .exceptions import get_cdtp_error
 from .utils import log
 
-from websockets.exceptions import ConnectionClosedError
-from inspect import iscoroutinefunction
-from typing import Callable, Awaitable, Optional, Union, Tuple, List, Dict
 from .data import DomainEvent, Sender, Receiver, CommonCallback
 from .extend_connection import Extend
 
 from .domains.background_service import BackgroundService
 from .domains.browser import Browser
 from .domains.css import CSS
 from .domains.device_orientation import DeviceOrientation
@@ -27,25 +26,27 @@
 from .domains.network import Network
 from .domains.overlay import Overlay
 from .domains.page import Page
 from .domains.runtime import Runtime
 from .domains.system_info import SystemInfo
 from .domains.target import Target
 
+CoroTypeNone = Coroutine[None, None, None]
+
 
 class Connection:
     """ Если инстанс страницы более не нужен, например, при перезаписи в него нового
     инстанса, перед этим [-!-] ОБЯЗАТЕЛЬНО [-!-] - вызовите у него метод
     Detach(), или закройте вкладку/страницу браузера, с которой он связан,
     тогда это будет выполнено автоматом. Иначе в цикле событий останутся
     задачи связанные с поддержанием соединения, которое более не востребовано.
     """
     __slots__ = (
-        "ws_url", "frontend_url", "callback", "_id", "extend",
-        "responses", "ws_session", "receiver", "on_detach_listener", "listeners", "listeners_for_event",
+        "ws_url", "frontend_url", "callback", "_id", "extend", "_bindings",
+        "responses", "_ws_session", "_receiver_loop", "_on_detach_listener", "_listeners_for_event",
         "on_close_event", "context_manager", "_connected", "_conn_id", "_verbose",
         "_browser_name", "_is_headless_mode",
 
         "BackgroundService", "Browser", "CSS", "DeviceOrientation", "DOM", "Emulation", "Fetch", "Input",
         "Log", "Network", "Overlay", "Page", "Runtime", "SystemInfo", "Target",
     )
 
@@ -67,29 +68,32 @@
                                         приходящие по WebSocket в виде словарей
         :param is_headless_mode:    "Headless" включён?
         :param verbose:             Печатать некие подробности процесса?
         :param browser_name:        Имя браузера
         """
 
         self.ws_url = ws_url
-        self._conn_id = conn_id
         self.frontend_url = frontend_url
         self.callback = callback
         self._is_headless_mode = is_headless_mode
-
+        self._conn_id = conn_id
         self._verbose = verbose
         self._browser_name = browser_name
-
         self._id = 0
         self._connected = False
-        self.ws_session: Optional[WebSocketClientProtocol] = None
-        self.receiver: Optional[asyncio.Task] = None
-        self.on_detach_listener: List[Callable[[any], Awaitable[None]], list, dict] = []
-        self.listeners = {}
-        self.listeners_for_event = {}
+        self._ws_session: Optional[WebSocketClientProtocol] = None
+        self._receiver_loop: Optional[asyncio.Task] = None
+        self._on_detach_listener: Tuple[Callable[[any], CoroTypeNone], list, dict] = tuple()
+        self._bindings: Dict[str, Tuple[Callable[[any], CoroTypeNone], Tuple[Any, ...]]] = {}
+        self._listeners_for_event: Dict[
+            str, Dict[
+                Callable[[dict, tuple], CoroTypeNone],
+                Tuple[Any, ...]
+            ]
+        ] = {}
         self.on_close_event = asyncio.Event()
         self.responses: Dict[int, Optional[Sender[dict]]] = {}
 
         self.extend = Extend(self)
 
         self.BackgroundService = BackgroundService(self)
         self.Browser = Browser(self)
@@ -164,305 +168,198 @@
         self.responses[_id] = sender
 
         await self._send(json.dumps(data))
 
         response = await receiver.recv()
         if "error" in response:
 
-            if ex := get_cdtp_error(response['error']['message']):
+            if ex := get_cdtp_error((e := response['error'])['message']):
                 raise ex(f"domain_and_method = '{domain_and_method}' | params = '{str(params)}'")
 
             raise Exception(
-                "Browser detect error:\n" +
-                f"error code -> '{response['error']['code']}';\n" +
-                f"error message -> '{response['error']['message']}'\n"+
-                f"domain_and_method = '{domain_and_method}' | params = '{str(params)}'"
+                "\x1b[36mBrowser detect error:\n" +
+                f"\x1b[37mError code: '\x1b[91m{e['code']}\n" +
+                f"\x1b[37mError message: '\x1b[91m{e['message']}\n" +
+                f"\x1b[37mdomain_and_method: '\x1b[91m{domain_and_method}\n" +
+                f"\x1b[37mparams: '\x1b[91m{params}\x1b[0m\n"
             )
 
         return response["result"]
 
-    async def eval(
-        self, expression: str,
-        objectGroup:            str = "console",
-        includeCommandLineAPI: bool = True,
-        silent:                bool = False,
-        returnByValue:         bool = False,
-        userGesture:           bool = True,
-        awaitPromise:          bool = False
-    ) -> dict:
-        response = await self.call(
-            "Runtime.evaluate", {
-                "expression": expression,
-                "objectGroup": objectGroup,
-                "includeCommandLineAPI": includeCommandLineAPI,
-                "silent": silent,
-                "returnByValue": returnByValue,
-                "userGesture": userGesture,
-                "awaitPromise": awaitPromise
-            }
-        )
-        if "exceptionDetails" in response:
-            raise EvaluateError(
-                highlight_eval_error(response["result"]["description"], expression)
-            )
-        return response["result"]
-
     async def _send(self, data: str) -> None:
         if self.connected:
-            await self.ws_session.send(data)
+            await self._ws_session.send(data)
 
     async def _recv(self) -> None:
         while self.connected:
             try:
-                data_msg: dict = json.loads(await self.ws_session.recv())
+                data_msg: dict = json.loads(await self._ws_session.recv())
             # ! Браузер разорвал соединение
             except ConnectionClosedError as e:
                 if self.verbose: log(f"ConnectionClosedError {e!r}")
                 await self.detach()
                 return
 
-            if ("method" in data_msg and data_msg["method"] == "Inspector.detached"
-                    and data_msg["params"]["reason"] == "target_closed"):
-                self.on_close_event.set()
-                await self.detach()
-                return
-
             # Ожидающие ответов вызовы API получают ответ по id входящих сообщений.
             if sender := self.responses.pop(data_msg.get("id"), None):
                 await sender.send(data_msg)
 
+            if ((method := data_msg.get("method")) == "Inspector.detached"
+                    and data_msg["params"]["reason"] == "target_closed"):
+                await self.detach()
+                self.on_close_event.set()
+                return
+
             # Если коллбэк функция была определена, она будет получать все
             #   уведомления из инстанса страницы.
             if self.callback is not None:
                 asyncio.create_task(self.callback(data_msg))
 
-            # Достаточно вызвать в контексте страницы следующее:
-            # console.info(JSON.stringify({
-            #     func_name: "test_func",
-            #     args: [1, "test"]
-            # }))
-            # и если среди зарегистрированных слушателей есть с именем "test_func",
-            #   то он немедленно получит распакованный список args[ ... ], вместе
-            #   с переданными ему аргументами, если таковые имеются.
-            if (method := data_msg.get("method")) == "Runtime.consoleAPICalled":
-                # ? Был вызван домен "info"
-                if data_msg["params"].get("type") == "info":
-
-                    str_value = data_msg["params"]["args"][0].get("value")
-                    try:
-                        value: dict = json.loads(str_value)
-                    except ValueError as e:
-                        if self.verbose:
-                            log(f"ValueError {e!r}")
-                            log(f"Msg from browser {str_value!r}")
-                        raise
-
-                    # ? Есть ожидающие слушатели
-                    if self.listeners:
-
-                        # ? Если есть ожидающая корутина
-                        if listener := self.listeners.get( value.get("func_name") ):
-                            asyncio.create_task(
-                                listener["function"](                               # корутина
-                                    *(value["args"] if "args" in value else []),    # её список аргументов вызова
-                                    *listener["args"]                               # список bind-агрументов
-                                )
-                            )
-
-            # По этой же схеме будут вызваны все слушатели для обработки
-            #   определённого метода, вызванного в контексте страницы,
-            #   если для этого метода они зарегистрированы.
-            if (    # =============================================================
-                    self.listeners_for_event
-                            and
-                    method in self.listeners_for_event
-            ):      # =============================================================
-                # Получаем словарь слушателей, в котором ключи — слушатели,
-                #   значения — их аргументы.
-                listeners: dict = self.listeners_for_event[ method ]
-                p = data_msg.get("params")
-                for listener, args in listeners.items():
+            # ? Был вызов из контекста страницы
+            if method == "Runtime.bindingCalled":
+                name: str = data_msg["params"]["name"]
+                payload: str = data_msg["params"]["payload"]
+
+                # ? Есть вызываемый объект с таким именем
+                if handle := self._bindings.get(name):
+                    function, args = handle
                     asyncio.create_task(
-                        listener(                                           # корутина
-                            p if p is not None else {},                     # её "params" — всегда передаётся
-                            *args                                           # список bind-агрументов
+                        function(
+                            *json.loads(payload),
+                            *args
+                        )
+                    )
+
+            if listeners := self._listeners_for_event.get(method):
+                p = data_msg.get("params") or {}
+                for listener, largs in listeners.items():
+                    asyncio.create_task(
+                        listener(       # корутина
+                            p,          # её "params" — всегда передаётся
+                            *largs      # список bind-агрументов
                         )
                     )
 
-    async def evalPromise(self, script: str) -> dict:
-        """ Выполняет асинхронный код на странице и возвращает результат.
-        !!! ВАЖНО !!! Выполняемый код не может возвращать какие-либо JS
-        типы, поэтому должен возвращать JSON-сериализованный набор данных.
-        """
-        result = await self.eval(script)
-        args = dict(
-            promiseObjectId=result["objectId"],
-            returnByValue=False,
-            generatePreview=False
-        )
-        response = await self.Runtime.awaitPromise(**args)
-        if "exceptionDetails" in response:
-            raise PromiseEvaluateError(
-                highlight_promise_error(response["result"]["description"]) +
-                "\n" + json.dumps(response["exceptionDetails"])
-            )
-        return json.loads(response["result"]["value"])
+
 
     async def waitForClose(self) -> None:
         """ Дожидается, пока не будет потеряно соединение со страницей. """
         await self.on_close_event.wait()
 
     async def activate(self) -> None:
-        self.ws_session = await connect(self.ws_url, ping_interval=None)
+        self._ws_session = await connect(self.ws_url, ping_interval=None)
         self._connected = True
-        self.receiver = asyncio.create_task(self._recv())
-        if self.callback is not None:
-            await self.Runtime.enable()
+        self._receiver_loop = asyncio.create_task(self._recv())
+        await self.Runtime.enable()
 
     async def detach(self) -> None:
-        """
-        Отключается от инстанса страницы. Вызывается автоматически при закрытии браузера,
-            или инстанса текущей страницы. Принудительный вызов не закрывает страницу,
-            а лишь разрывает с ней соединение.
+        """  Отключается от страницы. Вызывается автоматически при закрытии браузера,
+        или текущей страницы. Принудительный вызов не закрывает страницу,
+        а лишь разрывает с ней соединение.
         """
         if not self.connected:
             return
 
-        self.receiver.cancel()
+        self._receiver_loop.cancel()
         if self.verbose: log(f"[ DETACH ] {self.conn_id}")
         self._connected = False
 
-        if self.on_detach_listener:
-            function, args, kvargs = self.on_detach_listener
+        if self._on_detach_listener:
+            function, args, kvargs = self._on_detach_listener
             await function(*args, **kvargs)
 
-    def removeOnDetach(self) -> None:
-        self.on_detach_listener = []
+    def clearOnDetach(self) -> None:
+        self._on_detach_listener = tuple()
 
-    def setOnDetach(self, function: Callable[[any], Awaitable[None]], *args, **kvargs) -> bool:
-        """
-        Регистрирует асинхронный коллбэк, который будет вызван с соответствующими аргументами
-            при разрыве соединения со страницей.
+    def setOnDetach(self, function: Callable[[any], CoroTypeNone], *args, **kvargs) -> bool:
+        """  Регистрирует асинхронный коллбэк, который будет вызван с соответствующими аргументами
+        при разрыве соединения со страницей.
         """
         if not iscoroutinefunction(function):
             raise TypeError("OnDetach-listener must be a async callable object!")
         if not self.connected:
             return False
-        self.on_detach_listener = [function, args, kvargs]
+        self._on_detach_listener = function, args, kvargs
         return True
 
-    async def addListener(self, listener: Callable[[any], Awaitable[None]], *args: any) -> None:
+    async def bindFunction(self, function: Callable[[any], CoroTypeNone], *args: Any) -> None:
+        """ Регистрирует имя в глобальном контексте страницы. Это имя затем используется
+        в вызове функции, принимающей ровно один, строковый аргумент, который передаётся
+        в тело события `Runtime.bindingCalled`.
         """
-        Добавляет 'слушателя', который будет ожидать свой вызов по имени функции.
-            Вызов слушателей из контекста страницы осуществляется за счёт
-            JSON-сериализованного объекта, отправленного сообщением в консоль,
-            через домен 'info'. Объект должен содержать два обязательных свойства:
-                funcName — имя вызываемого слушателя
-                args:    — массив аргументов
-
-            Например, вызов javascript-кода:
-                console.info(JSON.stringify({
-                    funcName: "test_func",
-                    args: [1, "test"]
-                }))
-            Вызовет следующего Python-слушателя:
-                async def test_func(id, text, action):
-                    print(id, text, action)
-            Зарегистрированного следующим образом:
-                await page.AddListener(test_func, "test-action")
-
-            !!! ВНИМАНИЕ !!! В качестве слушателя может выступать ТОЛЬКО асинхронная
-                функция, или метод.
-
-        :param listener:        Асинхронная функция.
-        :param args:            (optional) любое кол-во аргументов, которые будут переданы
-                                    в функцию последними.
-        :return:        None
-        """
-        if not iscoroutinefunction(listener):
+        if not iscoroutinefunction(function):
             raise TypeError("Listener must be a async callable object!")
-        if listener.__name__ not in self.listeners:
-            self.listeners[ listener.__name__ ] = {"function": listener, "args": args}
-            if not self.Runtime.enabled:
-                await self.Runtime.enable()
-
-    async def addListeners(
-            self, *list_of_tuple_listeners_and_args: Tuple[Callable[[any], Awaitable[None]], list]) -> None:
-        """
-        Делает то же самое, что и AddListener(), но может зарегистрировать сразу несколько слушателей.
-            Принимает список кортежей с двумя элементами, вида (async_func_or_method, list_args), где:
-                async_func_or_method    - асинхронная фукция или метод
-                list_args               - список её аргументов(может быть пустым)
-        """
-        for action in list_of_tuple_listeners_and_args:
-            listener, args = action
-            if not iscoroutinefunction(listener):
-                raise TypeError("Listener must be a async callable object!")
-            if listener.__name__ not in self.listeners:
-                self.listeners[listener.__name__] = {"function": listener, "args": args}
-                if not self.Runtime.enabled:
-                    await self.Runtime.enable()
 
-    def removeListener(self, listener: Callable[[any], Awaitable[None]]) -> None:
-        """
-        Удаляет слушателя.
-        :param listener:        Колбэк-функция.
-        :return:        None
-        """
-        if not iscoroutinefunction(listener):
-            raise TypeError("Listener must be a async callable object!")
-        if listener.__name__ in self.listeners:
-            del self.listeners[ listener.__name__ ]
+        self._bindings[function.__name__] = function, args
+        await self.Runtime.addBinding(function.__name__)
+
+    async def bindFunctions(
+            self, *handlers_n_args: Tuple[Callable[[any], CoroTypeNone], Iterable]) -> None:
+        """ Выполняет множественную регистрацию.
+        :param handlers_n_args:     Список двухэлементных последовательностей,
+        в которых:
+            - первый элемент: awaitable-объект
+            - второй элемент: последовательность аргументов любой длины, которая
+                будет передана первому элементу в последнюю очередь.
+        """
+        for function, args in handlers_n_args:
+            await self.bindFunction(function, *args)
+
+    async def unbindFunctions(self, *functions: Union[Callable[[any], CoroTypeNone], str]) -> None:
+        """ Прекращает генерацию событий `Runtime.bindingCalled` для указанных имён.
+        :param functions:  Список функций, или их имён.
+        """
+        for function in functions:
+            name = function if type(function) is str else function.__name__
+            self._bindings.pop(name)
+            await self.Runtime.removeBinding(name)
 
     async def addListenerForEvent(
-        self, event: Union[str, DomainEvent], listener: Callable[[any], Awaitable[None]], *args) -> None:
-        """
-        Регистирует слушателя, который будет вызываться при вызове определённых событий
-            в браузере. Список таких событий можно посмотреть в разделе "Events" почти
-            у каждого домена по адресу: https://chromedevtools.github.io/devtools-protocol/
-            Например: 'DOM.attributeModified'
-        !Внимание! Каждый такой слушатель должен иметь один обязательный 'data'-аргумент,
-            в который будут передаваться параметры случившегося события в виде словаря(dict).
+        self, event: Union[str, DomainEvent], listener: Callable[[dict, tuple], CoroTypeNone], *args) -> None:
+        """ Регистрирует слушателя, который будет вызываться при генерации определённых событий
+        в браузере. Список таких событий можно посмотреть в разделе "Events" почти
+        у каждого домена по адресу: https://chromedevtools.github.io/devtools-protocol/
+        Например: 'DOM.attributeModified'
+            !Внимание! Каждый такой слушатель должен иметь один обязательный 'data'-аргумент,
+        в который будут передаваться параметры случившегося события в виде словаря(dict).
 
         :param event:           Имя события, для которого регистируется слушатель. Например:
                                     'DOM.attributeModified'.
         :param listener:        Колбэк-функция.
         :param args:            (optional) любое кол-во агрументов, которые будут переданы
                                     в функцию последними.
         :return:        None
         """
-        e = event if type(event) is str else event.value
         if not iscoroutinefunction(listener):
             raise TypeError("Listener must be a async callable object!")
-        if e not in self.listeners_for_event:
-            self.listeners_for_event[ e ]: dict = {}
-        self.listeners_for_event[ e ][listener] = args
-        if not self.Runtime.enabled:
-            await self.Runtime.enable()
+
+        e: str = event if type(event) is str else event.value
+        if e not in self._listeners_for_event:
+            self._listeners_for_event[e]: dict = {}
+        self._listeners_for_event[e][listener] = args
 
     def removeListenerForEvent(
-            self, event: Union[str, DomainEvent], listener: Callable[[any], Awaitable[None]]) -> None:
-        """
-        Удаляет регистрацию слушателя для указанного события.
+            self, event: Union[str, DomainEvent], listener: Callable[[dict, tuple], CoroTypeNone]) -> None:
+        """  Удаляет регистрацию слушателя для указанного события.
         :param event:           Имя метода, для которого была регистрация.
         :param listener:        Колбэк-функция, которую нужно удалить.
         :return:        None
         """
         e = event if type(event) is str else event.value
         if not iscoroutinefunction(listener):
             raise TypeError("Listener must be a async callable object!")
-        if m := self.listeners_for_event.get( e ):
+        if m := self._listeners_for_event.get(e):
             if listener in m: m.pop(listener)
 
 
     def removeListenersForEvent(self, event: Union[str, DomainEvent]) -> None:
         """
         Удаляет регистрацию метода и слушателей вместе с ним для указанного события.
         :param event:          Имя метода, для которого была регистрация.
         :return:        None
         """
         e = event if type(event) is str else event.value
-        if e in self.listeners_for_event:
-            self.listeners_for_event.pop(e)
+        if e in self._listeners_for_event:
+            self._listeners_for_event.pop(e)
 
     def __del__(self) -> None:
         if self.verbose: log(f"[ DELETED ] {self.conn_id}")
```

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/data.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/data.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/background_service/background_service.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/background_service/background_service.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/browser/browser.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/browser/browser.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/browser/types.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/browser/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/css/css.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/css/css.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/device_orientation/device_orientation.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/device_orientation/device_orientation.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/dom/dom.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/dom/dom.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/dom/dom_element.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/dom/dom_element.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/dom/types.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/dom/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/emulation/emulation.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/emulation/emulation.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/fetch/fetch.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/fetch/fetch.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/fetch/types.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/fetch/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/input/input.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/input/input.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/input/types.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/input/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/log/log.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/log/log.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/network/network.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/network/network.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/network/types.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/network/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/overlay/overlay.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/overlay/overlay.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/page/page.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/page/page.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/page/types.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/page/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/runtime/runtime.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/runtime/runtime.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,28 @@
 try:
     import ujson as json
 except ModuleNotFoundError:
     import json
 
-from typing import Optional, List
-from .types import PropertyDescriptor, ContextManager, ContextDescription, Script
+from typing import Optional, List, Dict, Union
+from .types import (
+    PropertyDescriptor,
+    ContextManager,
+    ContextDescription,
+    Script,
+    SerializationOptions,
+    RemoteObject,
+)
 from ...data import DomainEvent
-from ...exceptions import PromiseEvaluateError, highlight_promise_error
+from ...exceptions import (
+    PromiseEvaluateError,
+    highlight_promise_error,
+    EvaluateError,
+    highlight_eval_error
+)
 
 
 class Runtime:
     """
     #   https://chromedevtools.github.io/devtools-protocol/tot/Runtime
     """
     __slots__ = ("_connection", "enabled", "context_manager")
@@ -65,52 +77,142 @@
         result = []
         for p in response["result"]:
             if (subtype := p["value"].get("type")) and subtype == "function":
                 continue
             result.append(PropertyDescriptor(**p))
         return result
 
+    async def evaluate(
+            self, expression: str,
+            objectGroup: Optional[str] = None,
+            includeCommandLineAPI: Optional[bool] = None,
+            silent: Optional[bool] = None,
+            contextId: Optional[int] = None,
+            returnByValue: Optional[bool] = None,
+            generatePreview: Optional[bool] = None,
+            userGesture: Optional[bool] = None,
+            awaitPromise: Optional[bool] = None,
+            throwOnSideEffect: Optional[bool] = None,
+            timeout: Optional[float] = None,
+            disableBreaks: Optional[bool] = None,
+            replMode: Optional[bool] = None,
+            allowUnsafeEvalBlockedByCSP: Optional[bool] = None,
+            uniqueContextId: Optional[str] = None,
+            serializationOptions: Optional[SerializationOptions] = None,
+    ) -> RemoteObject:
+        """ Выполняет JavaScript-выражение в глобальном контексте.
+        https://chromedevtools.github.io/devtools-protocol/tot/Runtime/#method-evaluate
+        :param expression:  JavaScript-выражение.
+        :param objectGroup: Символическое имя группы, которое можно использовать
+            для освобождения нескольких объектов.
+        :param includeCommandLineAPI:   Определяет, должен ли быть доступен API
+            командной строки во время выполнения выражения.
+        :param silent:  В автоматическом режиме исключения, возникающие во время
+            выполнения выражения, не сообщаются и не приостанавливают выполнение.
+            Переопределяет setPauseOnException состояние.
+        :param contextId:   Указывает, в каком контексте выполнения выполнять выражение.
+            Если параметр опущен, оценка будет выполняться в контексте проверяемой
+            страницы. Это взаимоисключающее свойство uniqueContextId, которое предлагает
+            альтернативный способ определения контекста выполнения, более надежный в
+            многопроцессорной среде.
+        :param returnByValue:   Ожидается ли, что результат будет объектом JSON, который
+            должен быть отправлен по значению.
+        :param generatePreview: Должен ли быть создан предварительный просмотр для результата.
+        :param userGesture: Следует ли рассматривать выполнение как инициированное
+            пользователем в пользовательском интерфейсе.
+        :param awaitPromise:    Должно ли выполнение выражения ожидать результирующего
+            значения и возвращаться после завершения промиса.
+        :param throwOnSideEffect:   Выбрасывать ли исключение, если во время выполнения
+            выражения нельзя исключить побочный эффект. Это подразумевает использование
+             disableBreaks аргумента.
+        :param timeout: Прервать выполнение по истечении времени ожидания (количество миллисекунд).
+        :param disableBreaks:   Отключите точки останова во время выполнения выражения.
+        :param replMode:    Установка этого флага в значение true разрешает повторное
+            объявление переменных используя 'let', а так же вызов awaitable инструкций
+            в top-level контекста. Обратите внимание, что переменные let могут быть
+            повторно объявлены только в том случае, если они сами происходят из replMode.
+        :param allowUnsafeEvalBlockedByCSP: Политика безопасности содержимого (CSP)
+            для target может блокировать «unsafe-eval», который включает eval(),
+            Function(), setTimeout() и setInterval() при вызове с аргументами, которые
+            нельзя вызывать. Этот флаг обходит CSP для этой оценки и разрешает
+            небезопасную оценку. По умолчанию true.
+        :param uniqueContextId: Альтернативный способ указать контекст выполнения
+            для выполнения выражения. По сравнению с contextId, который может повторно
+            использоваться в процессах, он гарантированно уникален для системы, поэтому
+            его можно использовать для предотвращения случайного вычисления выражения
+            в контексте, отличном от предполагаемого (например, в результате навигации
+            через границы процесса). Это взаимоисключающее значение с contextId.
+        :param serializationOptions:    Указывает сериализацию результата. Если указано,
+            переопределяет generatePreview, returnByValue.
+        :return:
+        """
+        args = {"expression": expression}
+        if objectGroup is not None: args.update(objectGroup=objectGroup)
+        if includeCommandLineAPI is not None:
+            args.update(includeCommandLineAPI=includeCommandLineAPI)
+        if silent is not None: args.update(silent=silent)
+        if contextId is not None: args.update(contextId=contextId)
+        if returnByValue is not None: args.update(returnByValue=returnByValue)
+        if generatePreview is not None: args.update(generatePreview=generatePreview)
+        if userGesture is not None: args.update(userGesture=userGesture)
+        if awaitPromise is not None: args.update(awaitPromise=awaitPromise)
+        if throwOnSideEffect is not None: args.update(throwOnSideEffect=throwOnSideEffect)
+        if timeout is not None: args.update(timeout=timeout)
+        if disableBreaks is not None: args.update(disableBreaks=disableBreaks)
+        if replMode is not None: args.update(replMode=replMode)
+        if allowUnsafeEvalBlockedByCSP is not None:
+            args.update(allowUnsafeEvalBlockedByCSP=allowUnsafeEvalBlockedByCSP)
+        if uniqueContextId is not None: args.update(uniqueContextId=uniqueContextId)
+        if serializationOptions is not None:
+            args.update(serializationOptions=serializationOptions.as_dict())
+
+        response = await self._connection.call("Runtime.evaluate", args)
+        if "exceptionDetails" in response:
+            raise EvaluateError(
+                highlight_eval_error(response["result"]["description"], expression)
+            )
+
+        return RemoteObject(**response["result"])
 
     async def awaitPromise(
             self, promiseObjectId: str, returnByValue: bool = False, generatePreview: bool = False
-    ) -> dict:
-        """
-        Добавляет обработчик к промису с переданным идентификатором.
+    ) -> RemoteObject:
+        """ Дожидается выполнения промиса с указанным promiseObjectId.
         https://chromedevtools.github.io/devtools-protocol/tot/Runtime#method-awaitPromise
         :param promiseObjectId:     Идентификатор промиса.
         :param returnByValue:       (optional) Ожидается ли результат в виде объекта JSON,
                                         который должен быть отправлен по значению.
         :param generatePreview:     (optional) Должен ли предварительный просмотр
                                         генерироваться для результата.
-        :return:                    {
-                                        "result": dict(https://chromedevtools.github.io/devtools-protocol/tot/Runtime#type-RemoteObject)
-                                        "exceptionDetails": dict(https://chromedevtools.github.io/devtools-protocol/tot/Runtime#type-ExceptionDetails)
-                                    }
+        :return:
         """
         args = {"promiseObjectId": promiseObjectId, "returnByValue": returnByValue, "generatePreview": generatePreview}
         response = await self._connection.call("Runtime.awaitPromise", args)
         if "exceptionDetails" in response:
             raise PromiseEvaluateError(
                 highlight_promise_error(response["result"]["description"]) +
                 "\n" + json.dumps(response["exceptionDetails"])
             )
-        return response["result"]
+        return RemoteObject(**response["result"])
 
     async def callFunctionOn(
             self, functionDeclaration: str,
             objectId: Optional[str] = None,
             arguments: Optional[list] = None,
             silent: Optional[bool] = None,
             returnByValue: Optional[bool] = None,
             generatePreview: Optional[bool] = None,
             userGesture: Optional[bool] = None,
             awaitPromise: Optional[bool] = None,
             executionContextId: Optional[int] = None,
-            objectGroup: Optional[str] = None
-    ) -> dict:
+            objectGroup: Optional[str] = None,
+            throwOnSideEffect: Optional[bool] = None,
+            uniqueContextId: Optional[str] = None,
+            serializationOptions: Optional[SerializationOptions] = None
+    ) -> RemoteObject:
         """
         Вызывает функцию с заданным объявлением для данного объекта. Группа объектов результата
             наследуется от целевого объекта.
         https://chromedevtools.github.io/devtools-protocol/tot/Runtime#method-callFunctionOn
         :param functionDeclaration:     Объявление функции для вызова.
         :param objectId:                (optional) Идентификатор объекта для вызова функции.
                                             Должен быть указан либо objectId, либо executeContextId.
@@ -131,15 +233,25 @@
         :param executionContextId:      (optional) Определяет контекст выполнения, в котором будет
                                             использоваться глобальный объект для вызова функции.
                                             Должен быть указан либо executeContextId, либо objectId.
         :param objectGroup:             (optional) Символическое имя группы, которое можно
                                             использовать для освобождения нескольких объектов. Если
                                             objectGroup не указан, а objectId равен, objectGroup
                                             будет унаследован от объекта.
-        :return:                        { ... } - https://chromedevtools.github.io/devtools-protocol/tot/Runtime/#type-RemoteObject
+        :param throwOnSideEffect:   Выбрасывать ли исключение, если во время выполнения функции
+            нельзя исключить побочный эффект.
+        :param uniqueContextId: Альтернативный способ указать контекст выполнения
+            для выполнения выражения. По сравнению с contextId, который может повторно
+            использоваться в процессах, он гарантированно уникален для системы, поэтому
+            его можно использовать для предотвращения случайного вычисления выражения
+            в контексте, отличном от предполагаемого (например, в результате навигации
+            через границы процесса). Это взаимоисключающее значение с contextId.
+        :param serializationOptions:    Указывает сериализацию результата. Если указано,
+            переопределяет generatePreview, returnByValue.
+        :return:
         """
         args = {"functionDeclaration": functionDeclaration}
         if objectId is not None:
             args.update({"objectId": objectId})
         if arguments is not None:
             args.update({"arguments": arguments})
         if silent is not None:
@@ -152,18 +264,26 @@
             args.update({"userGesture": userGesture})
         if awaitPromise is not None:
             args.update({"awaitPromise": awaitPromise})
         if executionContextId is not None:
             args.update({"executionContextId": executionContextId})
         if objectGroup is not None:
             args.update({"objectGroup": objectGroup})
+        if throwOnSideEffect is not None:
+            args.update(throwOnSideEffect=throwOnSideEffect)
+        if uniqueContextId is not None:
+            args.update(uniqueContextId=uniqueContextId)
+        if serializationOptions is not None:
+            args.update(serializationOptions=serializationOptions.as_dict())
         response = await self._connection.call("Runtime.callFunctionOn", args)
         if "exceptionDetails" in response:
-            raise Exception(response["result"]["description"] + "\n" + json.dumps(response["exceptionDetails"]))
-        return response["result"]
+            raise EvaluateError(
+                highlight_eval_error(response["result"]["description"], functionDeclaration)
+            )
+        return RemoteObject(**response["result"])
 
     async def enable(self, watch_for_execution_contexts: bool = False) -> None:
         """
         Включает создание отчетов о создании контекстов выполнения с помощью события executeContextCreated.
             При включении, событие будет отправлено немедленно для каждого существующего контекста выполнения.
 
         Позволяет так же организовать обратную связь со страницей, посылая из её контекста, данные, в консоль.
@@ -218,79 +338,83 @@
             self._connection.removeListenerForEvent(
                 RuntimeEvent.executionContextsCleared, self.context_manager.on_clear)
             self._connection.removeListenerForEvent(
                 RuntimeEvent.executionContextDestroyed, self.context_manager.on_destroy)
             self.context_manager.is_watch = False
 
     async def discardConsoleEntries(self) -> None:
-        """
-        Отбрасывает собранные исключения и вызовы API консоли.
+        """ Отбрасывает собранные исключения и вызовы API консоли.
         https://chromedevtools.github.io/devtools-protocol/tot/Runtime#method-discardConsoleEntries
         :return:
         """
         await self._connection.call("Runtime.discardConsoleEntries")
 
     async def releaseObjectGroup(self, objectGroup: str) -> None:
-        """
-        Освобождает все удаленные объекты, принадлежащие данной группе.
+        """ Освобождает все удаленные объекты, принадлежащие данной группе.
         https://chromedevtools.github.io/devtools-protocol/tot/Runtime#method-releaseObjectGroup
         :param objectGroup:             Символическое имя группы.
         :return:
         """
-        await self._connection.call("Runtime.releaseObjectGroup", {"objectGroup": objectGroup})
+        await self._connection.call("Runtime.releaseObjectGroup", dict(objectGroup=objectGroup))
+
+    async def releaseObject(self, objectId: str) -> None:
+        """  Освобождает удаленный объект, с указанным objectId.
+        https://chromedevtools.github.io/devtools-protocol/tot/Runtime#method-releaseObject
+        :param objectId:             Символическое имя группы.
+        :return:
+        """
+        await self._connection.call("Runtime.releaseObject", dict(objectId=objectId))
 
     async def compileScript(
             self, expression: str,
             sourceURL: str = "",
             persistScript: bool = True,
             executionContextId: Optional[int] = None
     ) -> str:
-        """
-        Компилирует выражение.
+        """ Компилирует выражение.
         https://chromedevtools.github.io/devtools-protocol/tot/Runtime#method-compileScript
         :param expression:              Выражение для компиляции.
         :param sourceURL:               Исходный URL для скрипта.
         :param persistScript:           Указывает, следует ли сохранить скомпилированный скрипт.
         :param executionContextId:      (optional) Указывает, в каком контексте выполнения выполнять сценарий.
                                             Если параметр не указан, выражение будет выполняться в контексте
                                             проверяемой страницы.
-        :return:                        {
-                                            "scriptId": str()
-                                            "exceptionDetails": dict(https://chromedevtools.github.io/devtools-protocol/tot/Runtime#type-ExceptionDetails)
-                                        }
+        :return:
         """
-        args = {"expression": expression, "sourceURL": sourceURL, "persistScript": persistScript}
+        args: Dict[str, Union[int, str, bool]] = dict(
+            expression=expression, sourceURL=sourceURL, persistScript=persistScript)
         if executionContextId is not None:
-            args.update({"executionContextId": executionContextId})
+            args.update(executionContextId=executionContextId)
 
         response = await self._connection.call("Runtime.compileScript", args)
         if "exceptionDetails" in response:
-            raise Exception(response["exceptionDetails"]["text"] + "\n" + json.dumps(response["exceptionDetails"]))
+            raise EvaluateError(
+                highlight_eval_error(response["result"]["description"], expression)
+            )
         return response["scriptId"]
 
     async def buildScript(self, expression: str, context: Optional[ContextDescription] = None) -> Script:
         return Script(self._connection, expression, context)
 
     async def runIfWaitingForDebugger(self) -> None:
-        """
-        Сообщает инспектируемой странице, что можно запуститься, если она ожидает этого после
-            Target.setAutoAttach.
+        """ Сообщает инспектируемой странице, что можно запуститься, если она ожидает этого после
+        Target.setAutoAttach.
         """
         await self._connection.call("Runtime.runIfWaitingForDebugger")
 
     async def runScript(
             self, scriptId: str,
             executionContextId: Optional[int] = None,
             objectGroup: str = "console",
             silent: bool = False,
             includeCommandLineAPI: bool = True,
             returnByValue: bool = False,
             generatePreview: bool = False,
             awaitPromise: bool = True
-    ) -> dict:
+    ) -> RemoteObject:
         """
         Запускает скрипт с заданным идентификатором в заданном контексте.
         https://chromedevtools.github.io/devtools-protocol/tot/Runtime#method-runScript
         :param scriptId:                ID сценария для запуска.
         :param executionContextId:      (optional) Указывает, в каком контексте выполнения выполнять сценарий.
                                             Если параметр не указан, выражение будет выполняться в контексте
                                             проверяемой страницы.
@@ -317,37 +441,45 @@
             "generatePreview": generatePreview, "awaitPromise": awaitPromise
         }
         if executionContextId is not None:
             args.update({"executionContextId": executionContextId})
 
         response = await self._connection.call("Runtime.runScript", args)
         if "exceptionDetails" in response:
-            raise Exception(response["result"]["description"] + "\n" + json.dumps(response["exceptionDetails"]))
-        return response["result"]
+            raise EvaluateError(
+                highlight_eval_error(response["result"]["description"], "scriptId: " + scriptId)
+            )
+        return RemoteObject(**response["result"])
 
-    async def addBinding(self, name: str, executionContextName: Optional[int] = None) -> None:
-        """
-        (EXPERIMENTAL)
-        Если executeContextId пуст, добавляет привязку с заданным именем к глобальным объектам всех
-            проверенных контекстов, включая созданные позже, привязки переживают перезагрузки. Если
-            указан executeContextId, добавляет привязку только к глобальному объекту данного
-            контекста выполнения. Функция привязки принимает ровно один аргумент, этот аргумент
-            должен быть строкой, в случае любого другого ввода функция выдает исключение. Каждый
-            вызов функции привязки создает уведомление Runtime.bindingCalled.
+    async def addBinding(self, name: str, executionContextName: Optional[str] = None) -> None:
+        """ Делает доступным переданное имя в качестве имени функции, доступной глобально. Вызов
+        такой функции принимает ровно один аргумент типа `string`, иначе возбуждается исключение
+        с текстом `Invalid arguments: should be exactly one string.`. Каждый вызов функции по
+        этому имени создает уведомление Runtime.bindingCalled, в теле которого, поле `payload`
+        будет содержать строку, переданную в качестве аргумента вызванной функции.
         https://chromedevtools.github.io/devtools-protocol/tot/Runtime#method-addBinding
-        :param name:                    Имя привязки.
-        :param executionContextName:      (optional) Идентификатор контекста исполнения.
+        :param name:                    Имя вызываемой функции.
+        :param executionContextName:    (optional) Имя контекста исполнения.
         :return:
         """
         args = {"name": name}
         if executionContextName is not None:
             args.update({"executionContextName": executionContextName})
 
         await self._connection.call("Runtime.addBinding", args)
 
+    async def removeBinding(self, name: str) -> None:
+        """ Удаляет привязку по имени. Функцию всё ещё можно будет вызвать, но событие
+        'Runtime.bindingCalled' возбуждаться  не будет.
+        https://chromedevtools.github.io/devtools-protocol/tot/Runtime#method-removeBinding
+        :param name:                    Имя вызываемой функции.
+        :return:
+        """
+        await self._connection.call("Runtime.removeBinding", dict(name=name))
+
 
 class RuntimeEvent(DomainEvent):
     consoleAPICalled = "Runtime.consoleAPICalled"
     exceptionRevoked = "Runtime.exceptionRevoked"
     exceptionThrown = "Runtime.exceptionThrown"
     executionContextCreated = "Runtime.executionContextCreated"
     executionContextDestroyed = "Runtime.executionContextDestroyed"
```

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/runtime/types.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/runtime/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,28 @@
 from dataclasses import dataclass, field
-from typing import Literal, Optional, List, Union
+from typing import Literal, Optional, List, Union, Dict
+
+
+@dataclass
+class BindingCalledData:
+    name: str
+    payload: str
+    executionContextId: int
+
+
+@dataclass
+class SerializationOptions:
+    serialization: Literal["deep", "json", "idOnly"]
+    maxDepth: Optional[int] = None
+
+    def as_dict(self) -> Dict[str, Union[str, int]]:
+        result = {"serialization": self.serialization}
+        if self.maxDepth is not None:
+            result.update({"maxDepth": self.maxDepth})
+        return result
 
 
 @dataclass
 class PropertyPreview:
     name: str
     type: Literal["object", "function", "undefined", "string", "number", "boolean", "symbol", "accessor", "bigint"]
     valuePreview: Optional['ObjectPreview']
@@ -82,16 +101,16 @@
 @dataclass
 class RemoteObject:
     """
     Зеркальный объект, ссылающийся на исходный объект JavaScript.
     # https://chromedevtools.github.io/devtools-protocol/tot/Runtime/#type-RemoteObject
     """
     type: Literal["object", "function", "undefined", "string", "number", "boolean", "symbol", "bigint"]
-    preview: Optional['ObjectPreview']
-    customPreview: Optional['CustomPreview']
+    preview: Optional["ObjectPreview"]
+    customPreview: Optional["CustomPreview"]
     subtype: Optional[Literal[
         "array", "null", "node", "regexp", "date", "map", "set", "weakmap", "weakset", "iterator", "generator",
         "error", "proxy", "promise", "typedarray", "arraybuffer", "dataview", "webassemblymemory", "wasmvalue"]] = None
     className: Optional[str] = None
     value: Optional[any] = None
     unserializableValue: Optional[str] = None   # ? Примитивное значение, которое не может быть преобразовано в строку
                                                 # ?     JSON, не имеет value, но получает это свойство.
```

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/system_info/system_info.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/system_info/system_info.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/system_info/types.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/system_info/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/domains/target/target.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/domains/target/target.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/exceptions.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 
 class NoTargetWithGivenIdFound(MyBaseException): pass
 
 class NoScriptWithGivenId(MyBaseException): pass
 
 class UniqueContextIdNotFound(MyBaseException): pass
 
+class InvalidRemoteObjectId(MyBaseException): pass
+
 class AnotherLocaleOverrideIsAlreadyInEffect(MyBaseException): pass     # ! при установке той же локали
 
 class FontFamiliesCanOnlyBeSetOnce(MyBaseException): pass               # ! при установке тех же шрифтов
 
 class GetRequestBodyBeforeRequestReceived(MyBaseException): pass        # ! получение тела до получения ответа
 
 
@@ -51,14 +53,15 @@
     "Position out of bounds": PositionOutOfBounds,
     "Could not find node with given id": CouldNotFindNodeWithGivenID,
     "Could not compute content quads": CouldNotComputeContentQuads,
     "No dialog is showing": NoDialogIsShowing,
     "No target with given id found": NoTargetWithGivenIdFound,
     "No script with given id": NoScriptWithGivenId,
     "uniqueContextId not found": UniqueContextIdNotFound,
+    "Invalid remote object id": InvalidRemoteObjectId,
     "Another locale override is already in effect": AnotherLocaleOverrideIsAlreadyInEffect,
     "Font families can only be set once": FontFamiliesCanOnlyBeSetOnce,
     "Can only get response body on requests captured after headers received": GetRequestBodyBeforeRequestReceived,
 }
 
 
 def get_cdtp_error(error_text: str) -> Optional[Type[MyBaseException]]:
@@ -67,14 +70,21 @@
             return ex
     return None
     
 
 def highlight_eval_error(error_text: str, expression: str) -> str:
     """ Подсвечивает место в JS-коде ставшее причиной исключения.
     """
+    if "SyntaxError" in error_text:
+        return "\n".join([
+            "\nIn your code:"
+            f"\x1b[37m{expression}\x1b[0m\n"
+            f"\x1b[36mSyntaxError: \x1b[91m\x1b[4m{error_text[13:]}\x1b[0m",
+        ])
+
     line, pos = tuple(map(int, error_text.split(":")[-2:]))
     lines = expression.split("\n")
     l = lines[line - 1]
     word = re.match(r"\w+\b", l[pos - 1:]).group(0)
     l = "".join([l[:pos - 1], f"\x1b[91m\x1b[4m{word}\x1b[0m", l[len(word) + pos - 1:]])
     return "\n".join([
         error_text,
```

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/extend_connection.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/extend_connection.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,53 +9,48 @@
 import base64, re
 from typing import Optional
 
 from .exceptions import EvaluateError, JavaScriptError, NullProperty
 
 
 class Extend:
-    """
-    Расширение для 'Page'. Включает сборку наиболее востребованных методов для работы
-        с API 'ChromeDevTools Protocol', а так же дополняет некоторыми полезными методами.
+    """ Расширение для 'Page' некоторыми полезными методами.
     """
     __slots__ = ("_connection", "action")
 
     def __init__(self, conn) -> None:
 
         from .connection import Connection
 
         self._connection: Connection = conn
         self.action = Actions(conn)             # Совершает действия на странице. Клики;
                                                 # движения мыши; события клавиш
-
-    # region [ |>*<|=== Domains ===|>*<| ] Other [ |>*<|=== Domains ===|>*<| ]
-    #
-
-    async def pyExecAddOnload(self) -> None:
+    async def pyCallAddOnload(self) -> None:
         """ Включает автоматически добавляющийся JavaScript, вызывающий слушателей
-        клиента, добавленных на страницу с помощью await <Page>.AddListener(...) и
-        await <Page>.AddListeners(...).
-
-        Например, `test_func()` объявленная и добавленная следующим образом:
+        клиента, добавленных на страницу с помощью await <Connection>.bindFunction(...)
+        и await <Connection>.bindFunctions(...).
 
+        Например, `test_func()` объявленная следующим образом:
         async def test_func(number: int, text: str, bind_arg: dict) -> None:
             print("[- test_func -] Called with args:\n\tnumber: "
                   f"{number}\n\ttext: {text}\n\tbind_arg: {bind_arg}")
 
-        await page.AddListener(
+        И добавленная  следующим образом:
+        await conn.bindFunction(
             test_func,                          # ! слушатель
             {"name": "test", "value": True}     # ! bind_arg
         )
 
         Может быть вызвана со страницы браузера, так:
-        py_exec("test_func", 1, "testtt");
+        py_call("test_func", 1, "testtt");
         """
-        py_exec_js = """function py_exec(funcName, ...args) {
-            console.info(JSON.stringify({ func_name: funcName, args: args })); }"""
-        await self._connection.Page.addScriptOnLoad(py_exec_js)
+        py_call_js = """\
+        function py_call(funcName,...args){eval(funcName+"(`"+JSON.stringify(args)+"`)");}"""
+        await self._connection.Page.addScriptOnLoad(py_call_js)
+        await self.injectJS(py_call_js)
 
     async def getViewportRect(self) -> ViewportRect:
         """
         Возвращает список с длиной и шириной вьюпорта браузера.
         """
         code = "(()=>{return JSON.stringify([window.innerWidth,window.innerHeight]);})();"
         data = json.loads(await self.injectJS(code))
@@ -96,55 +91,91 @@
         :param fromSurface:     boolean => Capture the screenshot from the surface, rather than the view.
                                     Defaults to true.
         :return:                bytes
         """
         shot = await self._connection.Page.captureScreenshot(format_, quality, clip, fromSurface)
         return base64.b64decode(shot.encode("utf-8"))
 
-    async def selectInputContentBy(self, css: str) -> None:
-        await self.injectJS(f"let _i_ = document.querySelector('{css}'); _i_.focus(); _i_.select();")
+    async def selectOption(self, css: str) -> None:
+        """ Создаёт фокус и делает выбранным опцию тега <select>
+        при помощи JavaScript.
+        """
+        await self.injectJS(f"let _i_ = document.querySelector(`{css}`); _i_.focus(); _i_.select();")
 
     async def scrollIntoViewJS(self, selector: str) -> None:
+        """ Выполняет плавную прокрутку страницы до выбранного селектора. """
         await self.injectJS(
-            "document.querySelector(\"" +
+            "document.querySelector(`" +
             selector +
-            "\").scrollIntoView({'behavior':'smooth', 'block': 'center'});"
+            "`).scrollIntoView({'behavior':'smooth', 'block': 'center'});"
+        )
+
+    async def evalPromise(self, expression: str) -> dict:
+        """ Выполняет асинхронный код на странице и дожидается
+        получения результата.
+        """
+        result = await self._connection.Runtime.evaluate(
+            expression=expression,
+            objectGroup="console",
+            includeCommandLineAPI=True,
+            silent=False,
+            returnByValue=False,
+            userGesture=True,
+            awaitPromise=False
         )
 
-    async def injectJS(self, code: str) -> any:
+        response = await self._connection.Runtime.awaitPromise(
+            promiseObjectId=result.objectId,
+            returnByValue=False,
+            generatePreview=False
+        )
+
+        return json.loads(response.value)
+
+    async def injectJS(self, expression: str) -> any:
         """ Выполняет JavaScript-выражение во фрейме верхнего уровня. """
         try:
-            result = await self._connection.eval(code)
+            response = await self._connection.Runtime.evaluate(
+                expression=expression,
+                objectGroup="console",
+                includeCommandLineAPI=True,
+                silent=False,
+                returnByValue=False,
+                userGesture=True,
+                awaitPromise=False
+            )
         except EvaluateError as error:
             error = str(error)
             if "of null" in error:
                 if match := re.match(r"[\w\s:]+['|\"]([^'\"]+)", error):
                     prop = match.group(1)
                 else:
                     prop = "unmatched error: " + error
-                raise NullProperty(f"InjectJS() Exception with injected code:\n'{code}'\nNull property:\n{prop}")
+                raise NullProperty("InjectJS() Exception with injected code:"
+                                   f"\n'{expression}'\nNull property:\n{prop}")
 
-            raise JavaScriptError(f"JavaScriptError: InjectJS() Exception with injected code:\n'{code}'\nDescription:\n{error}")
+            raise JavaScriptError("JavaScriptError: InjectJS() Exception with "
+                                  f"injected code:\n'{expression}'\nDescription:\n{error}")
 
-        return result.get('value')
+        return response.value
 
     async def getGeoInfo(self) -> GeoInfo:
-        """
-        Возвращает информацию о Вашем местоположении, вычисленному по IP.
+        """ Возвращает информацию о местоположении точки выхода браузера в сеть,
+        вычисленному по IP.
         """
         async_fn_js = """\
         async function get_geo_info() {
             const resp = await fetch('https://time.gologin.com/');
             return await resp.text();
         } get_geo_info();
         """
 
         promise = """fetch('https://time.gologin.com/').then(res => res.text())"""
 
-        result: dict = await self._connection.evalPromise(promise)
+        result: dict = await self._connection.extend.evalPromise(promise)
         result.update(
             geo=dict(
                 latitude=float(result["ll"][0]),
                 longitude=float(result["ll"][1]),
                 accuracy=float(result["accuracy"])
             ),
             languages=result["languages"].split(","),
@@ -153,10 +184,7 @@
         )
         del result["ll"]
         del result["accuracy"]
         del result["stateProv"]
         if pt is not None:
             del result["proxyType"]
         return GeoInfo(**result)
-
-
-    # endregion
```

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol/utils.py` & `aio_dt_protocol-1.1.0/aio_dt_protocol/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 import asyncio
 import subprocess
-import sys, re
+import re
+import sys
 import urllib.request
-from typing import Optional, Dict
-
-if sys.platform == "win32":
-    import winreg
+from typing import Optional, Dict, Callable
 
 
 def get_request(url: str) -> str:
     with urllib.request.urlopen(url) as response:
         return response.read().decode('utf-8')
 
 
-def registry_read_key(exe="chrome") -> str:
-    """ Возвращает путь до EXE.
-    """
+def find_browser_executable_path(exe="chrome") -> str:
+    """ Возвращает путь до EXE. """
+    if not sys.platform == "win32":
+        raise OSError("registry_read_key() is only available on Windows")
+
+    if exe == "chromium":
+        import os
+        from pathlib import Path
+
+        app_data = Path(os.getenv('APPDATA')).parent
+        browser_path = app_data / "Local/Chromium/Application/chrome.exe"
+        if not browser_path.exists():
+            return ""
+        return browser_path.as_posix()
+
+    import winreg
+
     reg_path = f"HKEY_LOCAL_MACHINE\\SOFTWARE\\Microsoft\\Windows\\CurrentVersion\\App Paths\\{exe}.exe"
     key, path = re.findall(r"(^[^\\/]+)[\\/](.*)", reg_path)[0]
     connect_to = eval(f"winreg.{key}")
     try: h_key = winreg.OpenKey( winreg.ConnectRegistry(None, connect_to), path )
     except FileNotFoundError: return ""
     result = winreg.QueryValue(h_key, None)
     winreg.CloseKey(h_key)
@@ -34,71 +46,74 @@
     """ Сохраняет по пути 'path' набор байт 'data', которые можно прислать
     из метода страницы MakeScreenshot()
     """
     with open(path, "wb") as f:
         f.write(data)
 
 
-async def async_util_call(function: callable, *args) -> any:
+async def async_util_call(function: Callable, *args) -> any:
     """ Позволяет выполнять неблокирующий вызов блокирующих функций. Например:
     await async_util_call(
         save_img_as, "ScreenShot.png", await page_instance.MakeScreenshot()
     )
     """
     return await asyncio.get_running_loop().run_in_executor(
         None, function, *args
     )
 
 
 def find_instances(for_port: Optional[int] = None, browser: str = "chrome") -> Dict[int, int]:
-    """
-    Используется для обнаружения уже запущенных инстансов браузера в режиме отладки.
-    Более быстрая альтернатива для win32 систем FindInstances() есть в aio_dt_utils.Utils,
-        но она требует установленный пакет pywin32 для использования COM.
+    """ !!! ВНИМАНИЕ !!! На Windows 11 может быть отключен компонент WMI("Windows Management
+    Instrumentation"), его нужно либо включить в разделе “Программы и компоненты” панели
+    управления, либо установить из официальных источников.
+
+    Используется для обнаружения уже запущенных браузеров в режиме отладки.
     Например:
-            if browser_instances := Browser.FindInstances():
+            if browser_instances := find_instances():
                 port, pid = [(k, v) for k, v in browser_instances.items()][0]
                 browser_instance = Browser(debug_port=port, chrome_pid=pid)
             else:
                 browser_instance = Browser()
 
             # Или для конкретного, известного порта:
-            if browser_instances := Browser.FindInstances(port):
+            if browser_instances := find_instances(port):
                 pid = browser_instances[port]
                 browser_instance = Browser(debug_port=port, chrome_pid=pid)
             else:
                 browser_instance = Browser()
     :param for_port:    - порт, для которого осуществляется поиск.
     :param browser:     - браузер, для которого запрашивается поиск.
     :return:            - словарь, ключами которого являются используемые порты запущенных
                             браузеров, а значениями, их ProcessID, или пустой словарь,
                             если ничего не найдено.
                             { 9222: 16017, 9223: 2001, ... }
     """
     result = {}
     if sys.platform == "win32":
-        if "chrome" in browser: browser = "chrome.exe"
+        if "chrom" in browser: browser = "chrome.exe"
         elif "brave" in browser: browser = "brave.exe"
         elif "edge" in browser: browser = "msedge.exe"
-        else: ValueError("Not support browser: " + browser)
+        # else: ValueError("Not support browser: " + browser)
         cmd = f"WMIC PROCESS WHERE NAME='{browser}' GET Commandline,Processid"
         for line in subprocess.Popen(cmd, stdout=subprocess.PIPE).stdout:
             if b"--type=renderer" not in line and b"--remote-debugging-port=" in line:
                 port, pid = re.findall(r"--remote-debugging-port=(\d+).*?(\d+)\s*$", line.decode())[0]
                 port, pid = int(port), int(pid)
                 if for_port == port: return {port: pid}
                 result[port] = pid
+
     elif sys.platform == "linux":
-        if "chrome" in browser: browser = "google-chrome"
+        if "chrom" in browser: browser = "chrome"
         elif "brave" in browser: browser = "brave"
-        elif "edge" in browser: browser = "edge"
-        else: ValueError("Not support browser: " + browser)
+        elif "edge" in browser: browser = "msedge"
+        # else: ValueError("Not support browser: " + browser)
         try: itr = map(int, subprocess.check_output(["pidof", browser]).split())
         except subprocess.CalledProcessError: itr = []
         for pid in itr:
             with open("/proc/" + str(pid) + "/cmdline") as f: cmd_line =  f.read()[:-1]
             if "--type=renderer" not in cmd_line and "--remote-debugging-port=" in cmd_line:
                 port = int(re.findall(r"--remote-debugging-port=(\d+)", cmd_line)[0])
                 if for_port == port: return {port: pid}
                 result[port] = pid
-    else: raise OSError(f"Platform '{sys.platform}' — not supported")
+    else:
+        raise OSError(f"Platform '{sys.platform}' — not supported")
     return {} if for_port else result
```

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol.egg-info/PKG-INFO` & `aio_dt_protocol-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aio-dt-protocol
-Version: 1.0.2
+Name: aio_dt_protocol
+Version: 1.1.0
 Summary: Asynchronous wrapper over Chromium browser debugger protocol.
 Home-page: https://github.com/PieceOfGood/aio_dt_protocol
 Author: PieceOfGood
 Author-email: 78sanchezz@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
@@ -23,68 +23,80 @@
 ```shell
 pip install aio-dt-protocol
 ```
 
 Имеет одну зависимость:
 https://github.com/aaugustin/websockets
 
-И так как всё общение через протокол основано на формате JSON, по желанию можно установить ujson:
+И так как всё общение через протокол основано на формате JSON, по желанию можно установить в окружение ujson:
 https://github.com/ultrajson/ultrajson
 
 ### Примеры:
 
 ```python
 import asyncio
 from aio_dt_protocol import Browser
+from aio_dt_protocol import BrowserName
 from aio_dt_protocol import find_instances
 from aio_dt_protocol.data import KeyEvents
 
 DEBUG_PORT: int = 9222
-BROWSER_NAME: str = "chrome"
+BROWSER_NAME: str = BrowserName.CHROME
+PROFILE_NAME: str = BROWSER_NAME.capitalize() + "_Profile"
 
 
 async def main() -> None:
     # ? Если на указанном порту есть запущенный браузер, происходит подключение.
     if browser_instances := find_instances(DEBUG_PORT, BROWSER_NAME):
-        browser = Browser(debug_port=DEBUG_PORT, browser_pid=browser_instances[DEBUG_PORT])
+        browser = Browser(
+            debug_port=DEBUG_PORT,
+            browser_pid=browser_instances[DEBUG_PORT])
         msg = f"[- CONNECT TO EXIST BROWSER ON {DEBUG_PORT} PORT -]"
 
     # ? Иначе, запуск нового браузера.
     else:
         browser = Browser(
-            debug_port=DEBUG_PORT, browser_exe=BROWSER_NAME
+            debug_port=DEBUG_PORT, browser_exe=BROWSER_NAME,
+            profile_path=PROFILE_NAME
         )
         msg = f"[- LAUNCH NEW BROWSER ON {DEBUG_PORT} PORT -]"
     print(msg)
 
     # ? Будет печатать в консоль всё, что приходит по соединению со страницей.
     # ? Полезно при разработке.
     # async def action_printer(data: dict) -> None:
     #     print(data)
-    # conn = await browser.getPage(callback=action_printer)
-    conn = await browser.getPage()
+    # conn = await browser.waitFirstTab(callback=action_printer)
+    conn = await browser.waitFirstTab()
 
     print("[- GO TO GOOGLE ... -]")
     await conn.Page.navigate("https://www.google.com", )
     print("[- EMULATE INPUT TEXT ... -]")
 
     input_node = await conn.DOM.querySelector("[type=search]")
+    
+    # ? Эмуляция клика в поисковую строку
     await input_node.click()
     await asyncio.sleep(1)
+    
+    # ? Вставка текста
     await conn.Input.insertText("github PieceOfGood")
     await asyncio.sleep(1)
 
+    # ? Эмуляция нажатия клавиши Enter
     await conn.extend.action.sendKeyEvent(KeyEvents.enter)
     await asyncio.sleep(1)
-
+    
+    # ? Нажатие Enter можно заменить кликом по кнопке
+    # ? используя протокол
     # submit_button_selector = "div:not([jsname])>center>[type=submit]:not([jsaction])"
     # submit_button = await conn.DOM.querySelector(submit_button_selector)
     # await submit_button.click()
 
-    # ? Или выполнить клик используя JS
+    # ? Или выполнить клик используя JavaScript
     # click_code = f"""\
     # document.querySelector("{submit_button_selector}").click();
     # """
     # await conn.extend.injectJS(click_code)
 
     print("[- WAIT FOR CLOSE PAGE ... -]")
     # ? Пока соединение существует, цикл выполняется.
@@ -95,75 +107,92 @@
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
 На страницу можно легко зарегистрировать слушателей, которые будут вызываться на стороне клиентского(Python) кода. Для этого необходимо выполнить в браузере JavaScript, передав в `console.info()` JSON-строку из JavaScript-объекта с двумя обязательными полями `func_name` - имя вызываемой python-функции и `args` - список аргументов, которые будут ей переданы. Например:
 
 ```python
-    html = """
+    html = """\
     <html lang="ru">
     <head>
         <meta charset="utf-8" />
         <title>Test application</title>
     </head>
     <body>
         <button id="knopka">Push me</button>
     </body>
     <script>
         const btn = document.querySelector('#knopka');
         btn.addEventListener('click', () => {
-            console.info(JSON.stringify({
-                 func_name: "test_func",
-                 args: [1, "test"]
-            }))
+            py_call("test_func", 1, "test")
         });
     </script>
     </html>"""
-
-
-# ? number и text будут переданы из браузера, а bind_arg указан при регистрации
-async def test_func(number: int, text: str, bind_arg: dict) -> None:
-    print(f"[- test_func -] Called with args:\n\tnumber: {number}\n\ttext: {text}\n\tbing_arg: {bind_arg}")
-
-
-await conn.addListener(
-    test_func,  # ! слушатель
-    {"name": "test", "value": True}  # ! bind_arg
-)
-
-# ? Если ожидается внушительный функционал прикрутить к странице, то это можно
-# ? сделать за один раз.
-# await conn.addListeners(
-#     (test_func, [ {"name": "test", "value": True} ]),
-#     # (any_awaitable1, [1, 2, 3])
-#     # (any_awaitable2, [])
-# )
-
-await conn.Page.navigate(html)
+    
+    # ? Добавляем на страницу `py_call()`
+    await conn.extend.pyCallAddOnload()
+    
+    # ? number и text будут переданы из браузера, а bind_arg указан при регистрации
+    async def test_func(number: int, text: str, bind_arg: dict) -> None:
+        print(f"[- test_func -] Called with args:\n\tnumber: {number}"
+              f"\n\ttext: {text}\n\tbing_arg: {bind_arg}")
+    
+    
+    await conn.bindFunction(
+        test_func,  # ! слушатель
+        {"name": "test", "value": True}  # ! bind_arg
+    )
+    
+    # ? Если ожидается внушительный функционал прикрутить к странице, то это можно
+    # ? сделать за один раз.
+    # await conn.addListeners(
+    #     (test_func, [ {"name": "test", "value": True} ]),
+    #     # (any_awaitable1, [1, 2, 3])
+    #     # (any_awaitable2, [])
+    # )
+    
+    await conn.Page.navigate(html)
 ```
 ### Headless
-Чтобы запустить браузер в `безголовом` режиме, нужно передать аргументу принимающему путь к папке профиля пустую строку.
+Чтобы запустить браузер в безголовом(`headless`) режиме, передайте пустую строку аргументу(`profile_path`) принимающему путь к папке профиля.
 
 ```python
 import asyncio
-from aio_dt_protocol import Browser
+from aio_dt_protocol import Browser, BrowserName, find_instances
 from aio_dt_protocol.utils import save_img_as, async_util_call
 
+DEBUG_PORT: int = 9222
+BROWSER_NAME: str = BrowserName.CHROME
+
 
 async def main() -> None:
-    print("[- HEADLESS RUN -]")
-    browser = Browser(profile_path="")
+    # ? Если на указанном порту есть запущенный браузер, происходит подключение.
+    if browser_instances := find_instances(DEBUG_PORT, BROWSER_NAME):
+        browser = Browser(
+            debug_port=DEBUG_PORT,
+            browser_pid=browser_instances[DEBUG_PORT])
+        msg = f"[- HEADLESS CONNECT TO EXIST BROWSER ON {DEBUG_PORT} PORT -]"
+
+    # ? Иначе, запуск нового браузера.
+    else:
+        browser = Browser(
+            debug_port=DEBUG_PORT, browser_exe=BROWSER_NAME,
+            profile_path=""
+        )
+        msg = f"[- HEADLESS LAUNCH NEW BROWSER ON {DEBUG_PORT} PORT -]"
+    print(msg)
+    
     print("[- WAITING PAGE -]")
     conn = await browser.waitFirstTab()
     print("[- GO TO GOOGLE -]")
     await conn.Page.navigate("https://www.google.com")
 
     print("[- MAKE SCREENSHOT -]")
     await async_util_call(
-        save_img_as, "google.png", await conn.Page.makeScreenshot()
+        save_img_as, "google.png", await conn.extend.makeScreenshot()
     )
 
     print("[- CLOSE BROWSER -]")
     await conn.Browser.close()
     print("[- DONE -]")
```

### Comparing `aio_dt_protocol-1.0.2/aio_dt_protocol.egg-info/SOURCES.txt` & `aio_dt_protocol-1.1.0/aio_dt_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.0.2/setup.py` & `aio_dt_protocol-1.1.0/setup.py`

 * *Files identical despite different names*

