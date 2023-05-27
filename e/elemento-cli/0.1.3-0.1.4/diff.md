# Comparing `tmp/elemento-cli-0.1.3.tar.gz` & `tmp/elemento-cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elemento-cli-0.1.3.tar", last modified: Wed May 17 12:25:44 2023, max compression
+gzip compressed data, was "elemento-cli-0.1.4.tar", last modified: Sat May 27 12:25:16 2023, max compression
```

## Comparing `elemento-cli-0.1.3.tar` & `elemento-cli-0.1.4.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.408244 elemento-cli-0.1.3/
--rw-r--r--   0 filippovalle   (501) staff       (20)     3532 2023-05-17 12:25:44.407985 elemento-cli-0.1.3/PKG-INFO
--rw-r--r--   0 filippovalle   (501) staff       (20)     3286 2023-04-24 10:43:54.000000 elemento-cli-0.1.3/README.md
--rw-r--r--   0 filippovalle   (501) staff       (20)     2772 2023-04-18 10:37:58.000000 elemento-cli-0.1.3/betterprinttable.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.396889 elemento-cli-0.1.3/common/
--rw-r--r--   0 filippovalle   (501) staff       (20)      558 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/README.md
--rw-r--r--   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/__init__.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.397139 elemento-cli-0.1.3/common/lib/
--rw-r--r--   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/__init__.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.397243 elemento-cli-0.1.3/common/lib/components/
--rw-r--r--   0 filippovalle   (501) staff       (20)       94 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/__init__.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.399080 elemento-cli-0.1.3/common/lib/components/cpu/
--rw-r--r--   0 filippovalle   (501) staff       (20)      174 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      127 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/common.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1824 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/cpudescriptor.py
--rw-r--r--   0 filippovalle   (501) staff       (20)    88145 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/cpuinfo.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      647 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/cpumatcher.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1443 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/cpurequirements.py
--rw-r--r--   0 filippovalle   (501) staff       (20)    12275 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/cpustatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.400287 elemento-cli-0.1.3/common/lib/components/cpu/tests/
--rwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/tests/__init__.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     5890 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/tests/test_coresstatus.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     7412 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/tests/test_corestatus.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)      959 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/tests/test_cpudescriptor.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     2694 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/tests/test_cpumatcher.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     2105 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/cpu/tests/test_cpustatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.401055 elemento-cli-0.1.3/common/lib/components/memory/
--rw-r--r--   0 filippovalle   (501) staff       (20)      134 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/memory/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      788 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/memory/memdescriptor.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      456 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/memory/memmatcher.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      615 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/memory/memrequirements.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     2405 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/memory/memstatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.401688 elemento-cli-0.1.3/common/lib/components/misc/
--rw-r--r--   0 filippovalle   (501) staff       (20)       65 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/misc/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      461 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/misc/miscmatcher.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      609 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/misc/miscrequirements.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1525 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/misc/miscstatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.402427 elemento-cli-0.1.3/common/lib/components/net/
--rw-r--r--   0 filippovalle   (501) staff       (20)       88 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/net/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      449 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/net/netmatcher.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     2016 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/net/netrequirements.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1909 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/net/netspeed.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     7668 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/net/netstatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.403039 elemento-cli-0.1.3/common/lib/components/pcidev/
--rw-r--r--   0 filippovalle   (501) staff       (20)       68 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      456 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/pcimatcher.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      940 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/pcirequirements.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     7024 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/pcistatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.404096 elemento-cli-0.1.3/common/lib/components/pcidev/tests/
--rwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/tests/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1037 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pciaddress.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)      747 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pcidevice.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      785 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pcimatcher.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)      682 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pcirequirements.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)      793 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pciscanner.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     2481 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pcistatus.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.404747 elemento-cli-0.1.3/common/lib/system/
--rw-r--r--   0 filippovalle   (501) staff       (20)      108 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/system/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      565 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/system/systemmatcher.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1416 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/system/systemrequirements.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     6528 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/lib/system/systemstatus.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      106 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/requirements.txt
--rwxr-xr-x   0 filippovalle   (501) staff       (20)      167 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/common/run_tests.sh
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.405660 elemento-cli-0.1.3/ecd/
--rw-r--r--   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/ecd/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      677 2022-11-25 10:13:55.000000 elemento-cli-0.1.3/ecd/networking.json
--rw-r--r--   0 filippovalle   (501) staff       (20)      222 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/ecd/networking.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     1104 2022-11-25 10:13:32.000000 elemento-cli-0.1.3/ecd/restkeys.json
--rw-r--r--   0 filippovalle   (501) staff       (20)      222 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/ecd/restkeys.py
--rw-r--r--   0 filippovalle   (501) staff       (20)      148 2022-11-10 10:08:31.000000 elemento-cli-0.1.3/ecd/test.py
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     5790 2023-04-18 10:37:58.000000 elemento-cli-0.1.3/elemento
--rwxr-xr-x   0 filippovalle   (501) staff       (20)     5790 2023-04-18 10:37:58.000000 elemento-cli-0.1.3/elemento.py
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.406243 elemento-cli-0.1.3/elemento_cli.egg-info/
--rw-r--r--   0 filippovalle   (501) staff       (20)     3532 2023-05-17 12:25:44.000000 elemento-cli-0.1.3/elemento_cli.egg-info/PKG-INFO
--rw-r--r--   0 filippovalle   (501) staff       (20)     2472 2023-05-17 12:25:44.000000 elemento-cli-0.1.3/elemento_cli.egg-info/SOURCES.txt
--rw-r--r--   0 filippovalle   (501) staff       (20)        1 2023-05-17 12:25:44.000000 elemento-cli-0.1.3/elemento_cli.egg-info/dependency_links.txt
--rw-r--r--   0 filippovalle   (501) staff       (20)       84 2023-05-17 12:25:44.000000 elemento-cli-0.1.3/elemento_cli.egg-info/requires.txt
--rw-r--r--   0 filippovalle   (501) staff       (20)       20 2023-05-17 12:25:44.000000 elemento-cli-0.1.3/elemento_cli.egg-info/top_level.txt
-drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-17 12:25:44.407644 elemento-cli-0.1.3/handlers/
--rw-r--r--   0 filippovalle   (501) staff       (20)     2168 2023-03-17 11:00:12.000000 elemento-cli-0.1.3/handlers/__init__.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     6781 2023-03-17 11:00:12.000000 elemento-cli-0.1.3/handlers/account.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     3261 2023-03-17 11:00:12.000000 elemento-cli-0.1.3/handlers/iso.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     6871 2023-03-17 11:00:12.000000 elemento-cli-0.1.3/handlers/login.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     6950 2023-03-17 11:00:12.000000 elemento-cli-0.1.3/handlers/network.py
--rw-r--r--   0 filippovalle   (501) staff       (20)    13109 2023-04-18 10:37:58.000000 elemento-cli-0.1.3/handlers/vm.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     9321 2023-04-13 08:13:05.000000 elemento-cli-0.1.3/handlers/volumes.py
--rw-r--r--   0 filippovalle   (501) staff       (20)     3880 2023-04-18 10:37:58.000000 elemento-cli-0.1.3/headers.py
--rw-r--r--   0 filippovalle   (501) staff       (20)       38 2023-05-17 12:25:44.408287 elemento-cli-0.1.3/setup.cfg
--rw-r--r--   0 filippovalle   (501) staff       (20)     2972 2023-05-17 12:25:37.000000 elemento-cli-0.1.3/setup.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-27 12:25:16.070168 elemento-cli-0.1.4/
+-rw-r--r--   0 filippovalle   (501) staff       (20)     4893 2023-05-27 12:25:16.069837 elemento-cli-0.1.4/PKG-INFO
+-rw-r--r--   0 filippovalle   (501) staff       (20)     4648 2023-05-27 12:24:38.000000 elemento-cli-0.1.4/README.md
+-rw-r--r--   0 filippovalle   (501) staff       (20)     2772 2023-04-18 10:37:58.000000 elemento-cli-0.1.4/betterprinttable.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-27 12:25:16.058903 elemento-cli-0.1.4/common/
+-rw-r--r--   0 filippovalle   (501) staff       (20)      558 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/README.md
+-rw-r--r--   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/__init__.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-27 12:25:16.059094 elemento-cli-0.1.4/common/lib/
+-rw-r--r--   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/__init__.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-27 12:25:16.059214 elemento-cli-0.1.4/common/lib/components/
+-rw-r--r--   0 filippovalle   (501) staff       (20)       94 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/__init__.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-27 12:25:16.060723 elemento-cli-0.1.4/common/lib/components/cpu/
+-rw-r--r--   0 filippovalle   (501) staff       (20)      174 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/cpu/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      127 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/cpu/common.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1824 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/cpu/cpudescriptor.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)    88145 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/cpu/cpuinfo.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      647 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/cpu/cpumatcher.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1443 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/cpu/cpurequirements.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)    12275 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/cpu/cpustatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-27 12:25:16.062116 elemento-cli-0.1.4/common/lib/components/cpu/tests/
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/cpu/tests/__init__.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     5890 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/cpu/tests/test_coresstatus.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     7412 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/cpu/tests/test_corestatus.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)      959 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/cpu/tests/test_cpudescriptor.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     2694 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/cpu/tests/test_cpumatcher.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     2105 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/cpu/tests/test_cpustatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-27 12:25:16.062951 elemento-cli-0.1.4/common/lib/components/memory/
+-rw-r--r--   0 filippovalle   (501) staff       (20)      134 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/memory/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      788 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/memory/memdescriptor.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      456 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/memory/memmatcher.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      615 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/memory/memrequirements.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     2405 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/memory/memstatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-27 12:25:16.063573 elemento-cli-0.1.4/common/lib/components/misc/
+-rw-r--r--   0 filippovalle   (501) staff       (20)       65 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/misc/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      461 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/misc/miscmatcher.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      609 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/misc/miscrequirements.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1525 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/misc/miscstatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-27 12:25:16.064378 elemento-cli-0.1.4/common/lib/components/net/
+-rw-r--r--   0 filippovalle   (501) staff       (20)       88 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/net/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      449 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/net/netmatcher.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     2016 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/net/netrequirements.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1909 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/net/netspeed.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     7668 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/net/netstatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-27 12:25:16.065019 elemento-cli-0.1.4/common/lib/components/pcidev/
+-rw-r--r--   0 filippovalle   (501) staff       (20)       68 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/pcidev/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      456 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/pcidev/pcimatcher.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      940 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/pcidev/pcirequirements.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     7024 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/pcidev/pcistatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-27 12:25:16.066095 elemento-cli-0.1.4/common/lib/components/pcidev/tests/
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/pcidev/tests/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1037 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/pcidev/tests/test_pciaddress.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)      747 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/pcidev/tests/test_pcidevice.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      785 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/pcidev/tests/test_pcimatcher.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)      682 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/pcidev/tests/test_pcirequirements.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)      793 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/pcidev/tests/test_pciscanner.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     2481 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/components/pcidev/tests/test_pcistatus.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-27 12:25:16.066709 elemento-cli-0.1.4/common/lib/system/
+-rw-r--r--   0 filippovalle   (501) staff       (20)      108 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/system/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      565 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/system/systemmatcher.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1416 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/system/systemrequirements.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     6528 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/lib/system/systemstatus.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      106 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/requirements.txt
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)      167 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/common/run_tests.sh
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-27 12:25:16.067578 elemento-cli-0.1.4/ecd/
+-rw-r--r--   0 filippovalle   (501) staff       (20)        0 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/ecd/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      677 2022-11-25 10:13:55.000000 elemento-cli-0.1.4/ecd/networking.json
+-rw-r--r--   0 filippovalle   (501) staff       (20)      222 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/ecd/networking.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     1104 2022-11-25 10:13:32.000000 elemento-cli-0.1.4/ecd/restkeys.json
+-rw-r--r--   0 filippovalle   (501) staff       (20)      222 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/ecd/restkeys.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)      148 2022-11-10 10:08:31.000000 elemento-cli-0.1.4/ecd/test.py
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     5790 2023-04-18 10:37:58.000000 elemento-cli-0.1.4/elemento
+-rwxr-xr-x   0 filippovalle   (501) staff       (20)     5790 2023-04-18 10:37:58.000000 elemento-cli-0.1.4/elemento.py
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-27 12:25:16.068340 elemento-cli-0.1.4/elemento_cli.egg-info/
+-rw-r--r--   0 filippovalle   (501) staff       (20)     4893 2023-05-27 12:25:16.000000 elemento-cli-0.1.4/elemento_cli.egg-info/PKG-INFO
+-rw-r--r--   0 filippovalle   (501) staff       (20)     2472 2023-05-27 12:25:16.000000 elemento-cli-0.1.4/elemento_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 filippovalle   (501) staff       (20)        1 2023-05-27 12:25:16.000000 elemento-cli-0.1.4/elemento_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 filippovalle   (501) staff       (20)       84 2023-05-27 12:25:16.000000 elemento-cli-0.1.4/elemento_cli.egg-info/requires.txt
+-rw-r--r--   0 filippovalle   (501) staff       (20)       20 2023-05-27 12:25:16.000000 elemento-cli-0.1.4/elemento_cli.egg-info/top_level.txt
+drwxr-xr-x   0 filippovalle   (501) staff       (20)        0 2023-05-27 12:25:16.069618 elemento-cli-0.1.4/handlers/
+-rw-r--r--   0 filippovalle   (501) staff       (20)     2168 2023-03-17 11:00:12.000000 elemento-cli-0.1.4/handlers/__init__.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     6781 2023-03-17 11:00:12.000000 elemento-cli-0.1.4/handlers/account.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     3261 2023-03-17 11:00:12.000000 elemento-cli-0.1.4/handlers/iso.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     6871 2023-03-17 11:00:12.000000 elemento-cli-0.1.4/handlers/login.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     6950 2023-03-17 11:00:12.000000 elemento-cli-0.1.4/handlers/network.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)    13109 2023-04-18 10:37:58.000000 elemento-cli-0.1.4/handlers/vm.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     9321 2023-04-13 08:13:05.000000 elemento-cli-0.1.4/handlers/volumes.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)     3880 2023-04-18 10:37:58.000000 elemento-cli-0.1.4/headers.py
+-rw-r--r--   0 filippovalle   (501) staff       (20)       38 2023-05-27 12:25:16.070219 elemento-cli-0.1.4/setup.cfg
+-rw-r--r--   0 filippovalle   (501) staff       (20)     2972 2023-05-27 12:25:13.000000 elemento-cli-0.1.4/setup.py
```

### Comparing `elemento-cli-0.1.3/betterprinttable.py` & `elemento-cli-0.1.4/betterprinttable.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/README.md` & `elemento-cli-0.1.4/common/README.md`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/cpu/cpudescriptor.py` & `elemento-cli-0.1.4/common/lib/components/cpu/cpudescriptor.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/cpu/cpuinfo.py` & `elemento-cli-0.1.4/common/lib/components/cpu/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/cpu/cpumatcher.py` & `elemento-cli-0.1.4/common/lib/components/cpu/cpumatcher.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/cpu/cpurequirements.py` & `elemento-cli-0.1.4/common/lib/components/cpu/cpurequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/cpu/cpustatus.py` & `elemento-cli-0.1.4/common/lib/components/cpu/cpustatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/cpu/tests/test_coresstatus.py` & `elemento-cli-0.1.4/common/lib/components/cpu/tests/test_coresstatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/cpu/tests/test_corestatus.py` & `elemento-cli-0.1.4/common/lib/components/cpu/tests/test_corestatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/cpu/tests/test_cpudescriptor.py` & `elemento-cli-0.1.4/common/lib/components/cpu/tests/test_cpudescriptor.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/cpu/tests/test_cpumatcher.py` & `elemento-cli-0.1.4/common/lib/components/cpu/tests/test_cpumatcher.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/cpu/tests/test_cpustatus.py` & `elemento-cli-0.1.4/common/lib/components/cpu/tests/test_cpustatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/memory/memdescriptor.py` & `elemento-cli-0.1.4/common/lib/components/memory/memdescriptor.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/memory/memrequirements.py` & `elemento-cli-0.1.4/common/lib/components/memory/memrequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/memory/memstatus.py` & `elemento-cli-0.1.4/common/lib/components/memory/memstatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/misc/miscrequirements.py` & `elemento-cli-0.1.4/common/lib/components/misc/miscrequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/misc/miscstatus.py` & `elemento-cli-0.1.4/common/lib/components/misc/miscstatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/net/netrequirements.py` & `elemento-cli-0.1.4/common/lib/components/net/netrequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/net/netspeed.py` & `elemento-cli-0.1.4/common/lib/components/net/netspeed.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/net/netstatus.py` & `elemento-cli-0.1.4/common/lib/components/net/netstatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/pcidev/pcirequirements.py` & `elemento-cli-0.1.4/common/lib/components/pcidev/pcirequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/pcidev/pcistatus.py` & `elemento-cli-0.1.4/common/lib/components/pcidev/pcistatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pciaddress.py` & `elemento-cli-0.1.4/common/lib/components/pcidev/tests/test_pciaddress.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pcidevice.py` & `elemento-cli-0.1.4/common/lib/components/pcidev/tests/test_pcidevice.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pcimatcher.py` & `elemento-cli-0.1.4/common/lib/components/pcidev/tests/test_pcimatcher.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pcirequirements.py` & `elemento-cli-0.1.4/common/lib/components/pcidev/tests/test_pcirequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pciscanner.py` & `elemento-cli-0.1.4/common/lib/components/pcidev/tests/test_pciscanner.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/components/pcidev/tests/test_pcistatus.py` & `elemento-cli-0.1.4/common/lib/components/pcidev/tests/test_pcistatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/system/systemmatcher.py` & `elemento-cli-0.1.4/common/lib/system/systemmatcher.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/system/systemrequirements.py` & `elemento-cli-0.1.4/common/lib/system/systemrequirements.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/common/lib/system/systemstatus.py` & `elemento-cli-0.1.4/common/lib/system/systemstatus.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/ecd/networking.json` & `elemento-cli-0.1.4/ecd/networking.json`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/ecd/restkeys.json` & `elemento-cli-0.1.4/ecd/restkeys.json`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/elemento` & `elemento-cli-0.1.4/elemento`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/elemento.py` & `elemento-cli-0.1.4/elemento.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/elemento_cli.egg-info/SOURCES.txt` & `elemento-cli-0.1.4/elemento_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/handlers/__init__.py` & `elemento-cli-0.1.4/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/handlers/account.py` & `elemento-cli-0.1.4/handlers/account.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/handlers/iso.py` & `elemento-cli-0.1.4/handlers/iso.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/handlers/login.py` & `elemento-cli-0.1.4/handlers/login.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/handlers/network.py` & `elemento-cli-0.1.4/handlers/network.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/handlers/vm.py` & `elemento-cli-0.1.4/handlers/vm.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/handlers/volumes.py` & `elemento-cli-0.1.4/handlers/volumes.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/headers.py` & `elemento-cli-0.1.4/headers.py`

 * *Files identical despite different names*

### Comparing `elemento-cli-0.1.3/setup.py` & `elemento-cli-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="elemento-cli",
-    version="0.1.3",
+    version="0.1.4",
     author="Elemento",
     author_email="hello@elemento.cloud",
     description="CLI for Elemento",
     license="GPL",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://elemento.cloud",
```

