# Comparing `tmp/python-ndn-0.3a1.post3.tar.gz` & `tmp/python-ndn-0.3a1.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-ndn-0.3a1.post3.tar", last modified: Sat May 22 07:43:57 2021, max compression
+gzip compressed data, was "python-ndn-0.3a1.post4.tar", last modified: Mon Jul  5 20:24:33 2021, max compression
```

## Comparing `python-ndn-0.3a1.post3.tar` & `python-ndn-0.3a1.post4.tar`

### file list

```diff
@@ -1,81 +1,97 @@
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-05-22 07:43:57.219822 python-ndn-0.3a1.post3/
--rw-r--r--   0 cs217a     (501) staff       (20)      187 2020-09-25 00:48:59.000000 python-ndn-0.3a1.post3/AUTHORS.rst
--rw-r--r--   0 cs217a     (501) staff       (20)    10175 2019-11-26 04:57:08.000000 python-ndn-0.3a1.post3/COPYING
--rw-r--r--   0 cs217a     (501) staff       (20)     1040 2021-05-22 07:43:57.219344 python-ndn-0.3a1.post3/PKG-INFO
--rw-r--r--   0 cs217a     (501) staff       (20)      988 2021-04-29 18:37:08.000000 python-ndn-0.3a1.post3/README.rst
--rw-r--r--   0 cs217a     (501) staff       (20)       38 2021-05-22 07:43:57.220007 python-ndn-0.3a1.post3/setup.cfg
--rw-r--r--   0 cs217a     (501) staff       (20)     1683 2021-05-21 07:25:14.000000 python-ndn-0.3a1.post3/setup.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-05-22 07:43:57.186423 python-ndn-0.3a1.post3/src/
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-05-22 07:43:57.191127 python-ndn-0.3a1.post3/src/ndn/
--rw-r--r--   0 cs217a     (501) staff       (20)       24 2021-05-22 07:41:53.000000 python-ndn-0.3a1.post3/src/ndn/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)    22612 2021-05-22 07:39:53.000000 python-ndn-0.3a1.post3/src/ndn/app.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-05-22 07:43:57.193986 python-ndn-0.3a1.post3/src/ndn/app_support/
--rw-r--r--   0 cs217a     (501) staff       (20)        0 2019-10-02 17:36:51.000000 python-ndn-0.3a1.post3/src/ndn/app_support/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2430 2021-01-28 09:43:21.000000 python-ndn-0.3a1.post3/src/ndn/app_support/dispatcher.py
--rw-r--r--   0 cs217a     (501) staff       (20)     7122 2020-09-25 17:27:02.000000 python-ndn-0.3a1.post3/src/ndn/app_support/nfd_mgmt.py
--rw-r--r--   0 cs217a     (501) staff       (20)     4493 2020-09-25 17:27:13.000000 python-ndn-0.3a1.post3/src/ndn/app_support/security_v2.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2637 2020-09-25 17:27:17.000000 python-ndn-0.3a1.post3/src/ndn/app_support/segment_fetcher.py
--rw-r--r--   0 cs217a     (501) staff       (20)     3873 2020-09-25 17:29:50.000000 python-ndn-0.3a1.post3/src/ndn/client_conf.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-05-22 07:43:57.194538 python-ndn-0.3a1.post3/src/ndn/contrib/
--rw-r--r--   0 cs217a     (501) staff       (20)        0 2019-10-23 22:58:35.000000 python-ndn-0.3a1.post3/src/ndn/contrib/__init__.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-05-22 07:43:57.196497 python-ndn-0.3a1.post3/src/ndn/contrib/cocoapy/
--rw-r--r--   0 cs217a     (501) staff       (20)     1742 2019-10-10 22:49:52.000000 python-ndn-0.3a1.post3/src/ndn/contrib/cocoapy/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)    13048 2020-11-15 07:42:05.000000 python-ndn-0.3a1.post3/src/ndn/contrib/cocoapy/cocoalibs.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2629 2019-10-10 22:49:52.000000 python-ndn-0.3a1.post3/src/ndn/contrib/cocoapy/cocoatypes.py
--rw-r--r--   0 cs217a     (501) staff       (20)    51363 2020-11-15 07:58:22.000000 python-ndn-0.3a1.post3/src/ndn/contrib/cocoapy/runtime.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-05-22 07:43:57.200276 python-ndn-0.3a1.post3/src/ndn/encoding/
--rw-r--r--   0 cs217a     (501) staff       (20)      415 2019-09-28 20:57:01.000000 python-ndn-0.3a1.post3/src/ndn/encoding/__init__.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-05-22 07:43:57.201920 python-ndn-0.3a1.post3/src/ndn/encoding/name/
--rw-r--r--   0 cs217a     (501) staff       (20)    10641 2020-09-25 17:27:52.000000 python-ndn-0.3a1.post3/src/ndn/encoding/name/Component.py
--rw-r--r--   0 cs217a     (501) staff       (20)     6972 2020-09-25 17:27:57.000000 python-ndn-0.3a1.post3/src/ndn/encoding/name/Name.py
--rw-r--r--   0 cs217a     (501) staff       (20)       32 2019-11-07 04:59:36.000000 python-ndn-0.3a1.post3/src/ndn/encoding/name/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)    19631 2020-09-25 17:28:03.000000 python-ndn-0.3a1.post3/src/ndn/encoding/ndn_format_0_3.py
--rw-r--r--   0 cs217a     (501) staff       (20)     4173 2020-11-16 10:03:22.000000 python-ndn-0.3a1.post3/src/ndn/encoding/ndnlp_v2.py
--rw-r--r--   0 cs217a     (501) staff       (20)     1975 2020-09-25 17:28:10.000000 python-ndn-0.3a1.post3/src/ndn/encoding/signer.py
--rw-r--r--   0 cs217a     (501) staff       (20)    34439 2020-09-25 17:28:14.000000 python-ndn-0.3a1.post3/src/ndn/encoding/tlv_model.py
--rw-r--r--   0 cs217a     (501) staff       (20)     1899 2020-09-25 17:28:19.000000 python-ndn-0.3a1.post3/src/ndn/encoding/tlv_type.py
--rw-r--r--   0 cs217a     (501) staff       (20)     5007 2020-09-25 17:28:23.000000 python-ndn-0.3a1.post3/src/ndn/encoding/tlv_var.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2725 2020-09-25 17:29:53.000000 python-ndn-0.3a1.post3/src/ndn/name_tree.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-05-22 07:43:57.205427 python-ndn-0.3a1.post3/src/ndn/schema/
--rw-r--r--   0 cs217a     (501) staff       (20)        0 2020-09-25 00:48:54.000000 python-ndn-0.3a1.post3/src/ndn/schema/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)     3868 2020-09-25 17:33:09.000000 python-ndn-0.3a1.post3/src/ndn/schema/policy.py
--rw-r--r--   0 cs217a     (501) staff       (20)    25245 2021-04-29 18:34:03.000000 python-ndn-0.3a1.post3/src/ndn/schema/schema_tree.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2509 2020-09-25 17:33:19.000000 python-ndn-0.3a1.post3/src/ndn/schema/simple_cache.py
--rw-r--r--   0 cs217a     (501) staff       (20)     7378 2020-09-25 17:38:42.000000 python-ndn-0.3a1.post3/src/ndn/schema/simple_node.py
--rw-r--r--   0 cs217a     (501) staff       (20)     5780 2020-09-25 17:33:30.000000 python-ndn-0.3a1.post3/src/ndn/schema/simple_trust.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2839 2020-09-25 17:39:08.000000 python-ndn-0.3a1.post3/src/ndn/schema/util.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-05-22 07:43:57.206461 python-ndn-0.3a1.post3/src/ndn/security/
--rw-r--r--   0 cs217a     (501) staff       (20)      231 2019-10-23 22:58:35.000000 python-ndn-0.3a1.post3/src/ndn/security/__init__.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-05-22 07:43:57.208546 python-ndn-0.3a1.post3/src/ndn/security/keychain/
--rw-r--r--   0 cs217a     (501) staff       (20)      244 2019-10-23 22:58:35.000000 python-ndn-0.3a1.post3/src/ndn/security/keychain/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)     1651 2020-09-25 17:28:38.000000 python-ndn-0.3a1.post3/src/ndn/security/keychain/keychain.py
--rw-r--r--   0 cs217a     (501) staff       (20)     1378 2020-09-25 17:28:43.000000 python-ndn-0.3a1.post3/src/ndn/security/keychain/keychain_digest.py
--rw-r--r--   0 cs217a     (501) staff       (20)    17273 2020-09-25 17:28:47.000000 python-ndn-0.3a1.post3/src/ndn/security/keychain/keychain_sqlite3.py
--rw-r--r--   0 cs217a     (501) staff       (20)     4669 2020-09-25 17:29:33.000000 python-ndn-0.3a1.post3/src/ndn/security/osx.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-05-22 07:43:57.211173 python-ndn-0.3a1.post3/src/ndn/security/signer/
--rw-r--r--   0 cs217a     (501) staff       (20)      311 2019-10-25 06:53:37.000000 python-ndn-0.3a1.post3/src/ndn/security/signer/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)     1390 2020-09-25 17:28:54.000000 python-ndn-0.3a1.post3/src/ndn/security/signer/sha256_digest_signer.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2306 2020-09-25 17:29:00.000000 python-ndn-0.3a1.post3/src/ndn/security/signer/sha256_ecdsa_signer.py
--rw-r--r--   0 cs217a     (501) staff       (20)     1704 2020-09-25 17:29:03.000000 python-ndn-0.3a1.post3/src/ndn/security/signer/sha256_hmac_signer.py
--rw-r--r--   0 cs217a     (501) staff       (20)     1892 2020-09-25 17:29:06.000000 python-ndn-0.3a1.post3/src/ndn/security/signer/sha256_rsa_signer.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-05-22 07:43:57.213136 python-ndn-0.3a1.post3/src/ndn/security/tpm/
--rw-r--r--   0 cs217a     (501) staff       (20)       82 2019-10-23 22:58:35.000000 python-ndn-0.3a1.post3/src/ndn/security/tpm/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2376 2020-09-25 17:29:14.000000 python-ndn-0.3a1.post3/src/ndn/security/tpm/tpm.py
--rw-r--r--   0 cs217a     (501) staff       (20)     3760 2020-09-25 17:29:18.000000 python-ndn-0.3a1.post3/src/ndn/security/tpm/tpm_file.py
--rw-r--r--   0 cs217a     (501) staff       (20)     9634 2020-09-25 17:29:21.000000 python-ndn-0.3a1.post3/src/ndn/security/tpm/tpm_osx_keychain.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-05-22 07:43:57.214027 python-ndn-0.3a1.post3/src/ndn/security/validator/
--rw-r--r--   0 cs217a     (501) staff       (20)      170 2019-10-23 22:58:35.000000 python-ndn-0.3a1.post3/src/ndn/security/validator/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2341 2020-09-25 17:29:27.000000 python-ndn-0.3a1.post3/src/ndn/security/validator/digest_validator.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-05-22 07:43:57.215748 python-ndn-0.3a1.post3/src/ndn/transport/
--rw-r--r--   0 cs217a     (501) staff       (20)        0 2019-09-26 07:09:13.000000 python-ndn-0.3a1.post3/src/ndn/transport/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2413 2020-09-25 17:29:38.000000 python-ndn-0.3a1.post3/src/ndn/transport/dummy_face.py
--rw-r--r--   0 cs217a     (501) staff       (20)     3176 2021-05-21 07:25:46.000000 python-ndn-0.3a1.post3/src/ndn/transport/stream_socket.py
--rwxrwxrwx   0 cs217a     (501) staff       (20)     2876 2021-05-21 07:12:46.000000 python-ndn-0.3a1.post3/src/ndn/transport/windows.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2667 2021-03-23 10:53:39.000000 python-ndn-0.3a1.post3/src/ndn/types.py
--rw-r--r--   0 cs217a     (501) staff       (20)     1307 2020-09-25 17:30:01.000000 python-ndn-0.3a1.post3/src/ndn/utils.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-05-22 07:43:57.218561 python-ndn-0.3a1.post3/src/python_ndn.egg-info/
--rw-r--r--   0 cs217a     (501) staff       (20)     1040 2021-05-22 07:43:57.000000 python-ndn-0.3a1.post3/src/python_ndn.egg-info/PKG-INFO
--rw-r--r--   0 cs217a     (501) staff       (20)     1979 2021-05-22 07:43:57.000000 python-ndn-0.3a1.post3/src/python_ndn.egg-info/SOURCES.txt
--rw-r--r--   0 cs217a     (501) staff       (20)        1 2021-05-22 07:43:57.000000 python-ndn-0.3a1.post3/src/python_ndn.egg-info/dependency_links.txt
--rw-r--r--   0 cs217a     (501) staff       (20)      103 2021-05-22 07:43:57.000000 python-ndn-0.3a1.post3/src/python_ndn.egg-info/requires.txt
--rw-r--r--   0 cs217a     (501) staff       (20)        4 2021-05-22 07:43:57.000000 python-ndn-0.3a1.post3/src/python_ndn.egg-info/top_level.txt
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.399994 python-ndn-0.3a1.post4/
+-rw-r--r--   0 cs217a     (501) staff       (20)      187 2020-09-25 00:48:59.000000 python-ndn-0.3a1.post4/AUTHORS.rst
+-rw-r--r--   0 cs217a     (501) staff       (20)    10175 2019-11-26 04:57:08.000000 python-ndn-0.3a1.post4/COPYING
+-rw-r--r--   0 cs217a     (501) staff       (20)     3971 2021-07-05 20:24:33.400154 python-ndn-0.3a1.post4/PKG-INFO
+-rw-r--r--   0 cs217a     (501) staff       (20)      988 2021-04-29 18:37:08.000000 python-ndn-0.3a1.post4/README.rst
+-rw-r--r--   0 cs217a     (501) staff       (20)       96 2021-07-02 04:01:59.000000 python-ndn-0.3a1.post4/pyproject.toml
+-rw-r--r--   0 cs217a     (501) staff       (20)     1431 2021-07-05 20:24:33.401493 python-ndn-0.3a1.post4/setup.cfg
+-rw-r--r--   0 cs217a     (501) staff       (20)       69 2021-07-02 08:34:37.000000 python-ndn-0.3a1.post4/setup.py
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.352630 python-ndn-0.3a1.post4/src/
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.358610 python-ndn-0.3a1.post4/src/ndn/
+-rw-r--r--   0 cs217a     (501) staff       (20)       24 2021-07-02 04:13:19.000000 python-ndn-0.3a1.post4/src/ndn/__init__.py
+-rw-r--r--   0 cs217a     (501) staff       (20)    22914 2021-05-28 09:11:08.000000 python-ndn-0.3a1.post4/src/ndn/app.py
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.361867 python-ndn-0.3a1.post4/src/ndn/app_support/
+-rw-r--r--   0 cs217a     (501) staff       (20)        0 2019-10-02 17:36:51.000000 python-ndn-0.3a1.post4/src/ndn/app_support/__init__.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     2419 2021-07-05 05:00:49.000000 python-ndn-0.3a1.post4/src/ndn/app_support/dispatcher.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     7122 2020-09-25 17:27:02.000000 python-ndn-0.3a1.post4/src/ndn/app_support/nfd_mgmt.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     5095 2021-05-29 09:18:09.000000 python-ndn-0.3a1.post4/src/ndn/app_support/security_v2.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     2637 2020-09-25 17:27:17.000000 python-ndn-0.3a1.post4/src/ndn/app_support/segment_fetcher.py
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.362400 python-ndn-0.3a1.post4/src/ndn/bin/
+-rw-r--r--   0 cs217a     (501) staff       (20)        0 2021-07-05 20:02:19.000000 python-ndn-0.3a1.post4/src/ndn/bin/__init__.py
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.363020 python-ndn-0.3a1.post4/src/ndn/bin/sec/
+-rw-r--r--   0 cs217a     (501) staff       (20)      814 2021-07-05 20:06:43.000000 python-ndn-0.3a1.post4/src/ndn/bin/sec/__init__.py
+-rw-r--r--   0 cs217a     (501) staff       (20)       57 2021-07-05 20:07:14.000000 python-ndn-0.3a1.post4/src/ndn/bin/sec/__main__.py
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.363595 python-ndn-0.3a1.post4/src/ndn/bin/tools/
+-rw-r--r--   0 cs217a     (501) staff       (20)      814 2021-07-05 20:06:51.000000 python-ndn-0.3a1.post4/src/ndn/bin/tools/__init__.py
+-rw-r--r--   0 cs217a     (501) staff       (20)       57 2021-07-05 20:07:49.000000 python-ndn-0.3a1.post4/src/ndn/bin/tools/__main__.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     4021 2021-07-05 05:03:51.000000 python-ndn-0.3a1.post4/src/ndn/client_conf.py
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.363871 python-ndn-0.3a1.post4/src/ndn/contrib/
+-rw-r--r--   0 cs217a     (501) staff       (20)        0 2019-10-23 22:58:35.000000 python-ndn-0.3a1.post4/src/ndn/contrib/__init__.py
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.365626 python-ndn-0.3a1.post4/src/ndn/contrib/cocoapy/
+-rw-r--r--   0 cs217a     (501) staff       (20)     1742 2019-10-10 22:49:52.000000 python-ndn-0.3a1.post4/src/ndn/contrib/cocoapy/__init__.py
+-rw-r--r--   0 cs217a     (501) staff       (20)    13048 2020-11-15 07:42:05.000000 python-ndn-0.3a1.post4/src/ndn/contrib/cocoapy/cocoalibs.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     2629 2019-10-10 22:49:52.000000 python-ndn-0.3a1.post4/src/ndn/contrib/cocoapy/cocoatypes.py
+-rw-r--r--   0 cs217a     (501) staff       (20)    51363 2020-11-15 07:58:22.000000 python-ndn-0.3a1.post4/src/ndn/contrib/cocoapy/runtime.py
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.372592 python-ndn-0.3a1.post4/src/ndn/encoding/
+-rw-r--r--   0 cs217a     (501) staff       (20)      415 2019-09-28 20:57:01.000000 python-ndn-0.3a1.post4/src/ndn/encoding/__init__.py
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.375365 python-ndn-0.3a1.post4/src/ndn/encoding/name/
+-rw-r--r--   0 cs217a     (501) staff       (20)    10641 2020-09-25 17:27:52.000000 python-ndn-0.3a1.post4/src/ndn/encoding/name/Component.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     6972 2020-09-25 17:27:57.000000 python-ndn-0.3a1.post4/src/ndn/encoding/name/Name.py
+-rw-r--r--   0 cs217a     (501) staff       (20)       32 2019-11-07 04:59:36.000000 python-ndn-0.3a1.post4/src/ndn/encoding/name/__init__.py
+-rw-r--r--   0 cs217a     (501) staff       (20)    19631 2020-09-25 17:28:03.000000 python-ndn-0.3a1.post4/src/ndn/encoding/ndn_format_0_3.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     4173 2020-11-16 10:03:22.000000 python-ndn-0.3a1.post4/src/ndn/encoding/ndnlp_v2.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     1975 2020-09-25 17:28:10.000000 python-ndn-0.3a1.post4/src/ndn/encoding/signer.py
+-rw-r--r--   0 cs217a     (501) staff       (20)    34436 2021-07-05 05:00:49.000000 python-ndn-0.3a1.post4/src/ndn/encoding/tlv_model.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     1899 2020-09-25 17:28:19.000000 python-ndn-0.3a1.post4/src/ndn/encoding/tlv_type.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     5007 2020-09-25 17:28:23.000000 python-ndn-0.3a1.post4/src/ndn/encoding/tlv_var.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     2725 2020-09-25 17:29:53.000000 python-ndn-0.3a1.post4/src/ndn/name_tree.py
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.378696 python-ndn-0.3a1.post4/src/ndn/platform/
+-rw-r--r--   0 cs217a     (501) staff       (20)       69 2021-07-01 03:36:59.000000 python-ndn-0.3a1.post4/src/ndn/platform/__init__.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     2100 2021-07-05 05:00:49.000000 python-ndn-0.3a1.post4/src/ndn/platform/general.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     1591 2021-07-05 05:00:49.000000 python-ndn-0.3a1.post4/src/ndn/platform/linux.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     5480 2021-07-05 05:00:49.000000 python-ndn-0.3a1.post4/src/ndn/platform/osx.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     6856 2021-07-05 05:03:42.000000 python-ndn-0.3a1.post4/src/ndn/platform/windows.py
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.384268 python-ndn-0.3a1.post4/src/ndn/schema/
+-rw-r--r--   0 cs217a     (501) staff       (20)        0 2020-09-25 00:48:54.000000 python-ndn-0.3a1.post4/src/ndn/schema/__init__.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     3868 2020-09-25 17:33:09.000000 python-ndn-0.3a1.post4/src/ndn/schema/policy.py
+-rw-r--r--   0 cs217a     (501) staff       (20)    25245 2021-04-29 18:34:03.000000 python-ndn-0.3a1.post4/src/ndn/schema/schema_tree.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     2509 2020-09-25 17:33:19.000000 python-ndn-0.3a1.post4/src/ndn/schema/simple_cache.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     7378 2020-09-25 17:38:42.000000 python-ndn-0.3a1.post4/src/ndn/schema/simple_node.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     5780 2020-09-25 17:33:30.000000 python-ndn-0.3a1.post4/src/ndn/schema/simple_trust.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     2839 2020-09-25 17:39:08.000000 python-ndn-0.3a1.post4/src/ndn/schema/util.py
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.384978 python-ndn-0.3a1.post4/src/ndn/security/
+-rw-r--r--   0 cs217a     (501) staff       (20)      231 2019-10-23 22:58:35.000000 python-ndn-0.3a1.post4/src/ndn/security/__init__.py
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.387479 python-ndn-0.3a1.post4/src/ndn/security/keychain/
+-rw-r--r--   0 cs217a     (501) staff       (20)      244 2019-10-23 22:58:35.000000 python-ndn-0.3a1.post4/src/ndn/security/keychain/__init__.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     1651 2020-09-25 17:28:38.000000 python-ndn-0.3a1.post4/src/ndn/security/keychain/keychain.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     1378 2020-09-25 17:28:43.000000 python-ndn-0.3a1.post4/src/ndn/security/keychain/keychain_digest.py
+-rw-r--r--   0 cs217a     (501) staff       (20)    17273 2020-09-25 17:28:47.000000 python-ndn-0.3a1.post4/src/ndn/security/keychain/keychain_sqlite3.py
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.391054 python-ndn-0.3a1.post4/src/ndn/security/signer/
+-rw-r--r--   0 cs217a     (501) staff       (20)      311 2019-10-25 06:53:37.000000 python-ndn-0.3a1.post4/src/ndn/security/signer/__init__.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     1390 2020-09-25 17:28:54.000000 python-ndn-0.3a1.post4/src/ndn/security/signer/sha256_digest_signer.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     2306 2020-09-25 17:29:00.000000 python-ndn-0.3a1.post4/src/ndn/security/signer/sha256_ecdsa_signer.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     1704 2020-09-25 17:29:03.000000 python-ndn-0.3a1.post4/src/ndn/security/signer/sha256_hmac_signer.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     1892 2020-09-25 17:29:06.000000 python-ndn-0.3a1.post4/src/ndn/security/signer/sha256_rsa_signer.py
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.394426 python-ndn-0.3a1.post4/src/ndn/security/tpm/
+-rw-r--r--   0 cs217a     (501) staff       (20)       82 2019-10-23 22:58:35.000000 python-ndn-0.3a1.post4/src/ndn/security/tpm/__init__.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     2376 2020-09-25 17:29:14.000000 python-ndn-0.3a1.post4/src/ndn/security/tpm/tpm.py
+-rw-r--r--   0 cs217a     (501) staff       (20)    11547 2021-07-05 05:03:42.000000 python-ndn-0.3a1.post4/src/ndn/security/tpm/tpm_cng.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     3760 2020-09-25 17:29:18.000000 python-ndn-0.3a1.post4/src/ndn/security/tpm/tpm_file.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     9692 2021-07-05 05:03:42.000000 python-ndn-0.3a1.post4/src/ndn/security/tpm/tpm_osx_keychain.py
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.396138 python-ndn-0.3a1.post4/src/ndn/security/validator/
+-rw-r--r--   0 cs217a     (501) staff       (20)      394 2021-05-29 08:45:36.000000 python-ndn-0.3a1.post4/src/ndn/security/validator/__init__.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     2341 2020-09-25 17:29:27.000000 python-ndn-0.3a1.post4/src/ndn/security/validator/digest_validator.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     3248 2021-05-29 08:56:19.000000 python-ndn-0.3a1.post4/src/ndn/security/validator/known_key_validator.py
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.397595 python-ndn-0.3a1.post4/src/ndn/transport/
+-rw-r--r--   0 cs217a     (501) staff       (20)        0 2019-09-26 07:09:13.000000 python-ndn-0.3a1.post4/src/ndn/transport/__init__.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     2413 2020-09-25 17:29:38.000000 python-ndn-0.3a1.post4/src/ndn/transport/dummy_face.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     2981 2021-07-05 05:00:49.000000 python-ndn-0.3a1.post4/src/ndn/transport/stream_socket.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     2667 2021-03-23 10:53:39.000000 python-ndn-0.3a1.post4/src/ndn/types.py
+-rw-r--r--   0 cs217a     (501) staff       (20)     1307 2020-09-25 17:30:01.000000 python-ndn-0.3a1.post4/src/ndn/utils.py
+drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.399727 python-ndn-0.3a1.post4/src/python_ndn.egg-info/
+-rw-r--r--   0 cs217a     (501) staff       (20)     3971 2021-07-05 20:24:33.000000 python-ndn-0.3a1.post4/src/python_ndn.egg-info/PKG-INFO
+-rw-r--r--   0 cs217a     (501) staff       (20)     2349 2021-07-05 20:24:33.000000 python-ndn-0.3a1.post4/src/python_ndn.egg-info/SOURCES.txt
+-rw-r--r--   0 cs217a     (501) staff       (20)        1 2021-07-05 20:24:33.000000 python-ndn-0.3a1.post4/src/python_ndn.egg-info/dependency_links.txt
+-rw-r--r--   0 cs217a     (501) staff       (20)       79 2021-07-05 20:24:33.000000 python-ndn-0.3a1.post4/src/python_ndn.egg-info/entry_points.txt
+-rw-r--r--   0 cs217a     (501) staff       (20)      116 2021-07-05 20:24:33.000000 python-ndn-0.3a1.post4/src/python_ndn.egg-info/requires.txt
+-rw-r--r--   0 cs217a     (501) staff       (20)        4 2021-07-05 20:24:33.000000 python-ndn-0.3a1.post4/src/python_ndn.egg-info/top_level.txt
```

### Comparing `python-ndn-0.3a1.post3/COPYING` & `python-ndn-0.3a1.post4/COPYING`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/README.rst` & `python-ndn-0.3a1.post4/README.rst`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/app.py` & `python-ndn-0.3a1.post4/src/ndn/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,18 +208,28 @@
         if 'interest_param' in kwargs:
             interest_param = kwargs['interest_param']
         else:
             if 'nonce' not in kwargs:
                 kwargs['nonce'] = gen_nonce()
             interest_param = InterestParam.from_dict(kwargs)
         interest, final_name = make_interest(name, interest_param, app_param, signer=signer, need_final_name=True)
+        return self.express_raw_interest(final_name, interest_param, interest, validator, need_raw_packet)
+
+    def express_raw_interest(self,
+                             final_name: NonStrictName,
+                             interest_param: InterestParam,
+                             raw_interest: BinaryStr,
+                             validator: Optional[Validator] = None,
+                             need_raw_packet: bool = False
+                             ) -> Coroutine[Any, None, Tuple[FormalName, MetaInfo, Optional[BinaryStr]]]:
+        final_name = Name.normalize(final_name)
         future = aio.get_running_loop().create_future()
         node = self._int_tree.setdefault(final_name, InterestTreeNode())
         node.append_interest(future, interest_param)
-        self.face.send(interest)
+        self.face.send(raw_interest)
         return self._wait_for_data(future, interest_param.lifetime, final_name, node, validator, need_raw_packet)
 
     async def _wait_for_data(self, future: aio.Future, lifetime: int, name: FormalName,
                              node: InterestTreeNode, validator: Validator, need_raw_packet: bool):
         lifetime = 100 if lifetime is None else lifetime
         try:
             name, meta_info, content, sig, raw_packet = await aio.wait_for(future, timeout=lifetime/1000.0)
@@ -382,21 +392,15 @@
         :type need_sig_ptrs: bool
 
         :raises ValueError: the prefix is already registered.
         :raises NetworkError: the face to NFD is down now.
         """
         name = Name.normalize(name)
         if func is not None:
-            node = self._prefix_tree.setdefault(name, PrefixTreeNode())
-            if node.callback:
-                raise ValueError(f'Duplicated registration: {Name.to_str(name)}')
-            node.callback = func
-            node.extra_param = {'raw_packet': need_raw_packet, 'sig_ptrs': need_sig_ptrs}
-            if validator:
-                node.validator = validator
+            self.set_interest_filter(name, func, validator, need_raw_packet, need_sig_ptrs)
 
         # Fix the issue that NFD only allows one packet signed by a specific key for a timestamp number
         async with self._prefix_register_semaphore:
             try:
                 _, _, reply = await self.express_interest(make_command('rib', 'register', name=name), lifetime=1000)
                 ret = parse_response(reply)
                 if ret['status_code'] != 200:
@@ -423,16 +427,16 @@
         try:
             await self.express_interest(make_command('rib', 'unregister', name=name), lifetime=1000)
             return True
         except (InterestNack, InterestTimeout, InterestCanceled, ValidationFailure):
             return False
 
     def set_interest_filter(self, name: NonStrictName, func: Route,
-                                  validator: Optional[Validator] = None, need_raw_packet: bool = False,
-                                  need_sig_ptrs: bool = False):
+                            validator: Optional[Validator] = None, need_raw_packet: bool = False,
+                            need_sig_ptrs: bool = False):
         """
         Set the callback function for an Interest prefix without sending a register command to the forwarder.
 
         .. note::
             All callbacks registered by ``set_interest_filter`` are removed when disconnected from
             the the forwarder, and will not be added back after reconnection.
             This behaviour is the same as ``register``.
```

### Comparing `python-ndn-0.3a1.post3/src/ndn/app_support/dispatcher.py` & `python-ndn-0.3a1.post4/src/ndn/app_support/dispatcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
 from typing import Optional
 from ..encoding import NonStrictName, Name, BinaryStr, InterestParam, FormalName
-from ..types import Validator, Route
+from ..types import Route
 from ..name_tree import NameTrie, PrefixTreeNode
 
 
 class Dispatcher:
     """
     An Interest dispatcher that helps a producer application further dispatches Interests under some route.
     """
```

### Comparing `python-ndn-0.3a1.post3/src/ndn/app_support/nfd_mgmt.py` & `python-ndn-0.3a1.post4/src/ndn/app_support/nfd_mgmt.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/app_support/security_v2.py` & `python-ndn-0.3a1.post4/src/ndn/app_support/security_v2.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
 from typing import Tuple
-from datetime import datetime
+from datetime import datetime, timedelta
 from ..utils import timestamp
 from ..encoding import Component, Name, ModelField, TlvModel, ContentType, BytesField,\
     SignatureInfo, TypeNumber, RepeatedField, IncludeBase, MetaInfo, VarBinaryStr,\
     get_tl_num_size, write_tl_num, parse_and_check_tl, FormalName
 from ..encoding.ndn_format_0_3 import DataPacketValue
 
 
@@ -74,37 +74,51 @@
     certificate_v2 = BytesField(TypeNumber.DATA)
     # We do not use ModelField due to 2 reasons:
     # 1. The encoded length of CertificateV2 is unknown.
     # 2. Generally we already have an encoded certificate when exporting a SafeBag.
     encrypted_key_bag = BytesField(SecurityV2TypeNumber.ENCRYPTED_KEY_BAG)
 
 
-def self_sign(key_name, pub_key, signer) -> Tuple[FormalName, VarBinaryStr]:
+def parse_certificate(wire) -> CertificateV2Value:
+    wire = parse_and_check_tl(wire, TypeNumber.DATA)
+    return CertificateV2Value.parse(wire)
+
+
+def new_cert(key_name, issuer_id_component, pub_key, signer, start_time, end_time) -> Tuple[FormalName, VarBinaryStr]:
     cert_val = CertificateV2Value()
-    cert_name = Name.normalize(key_name) + [SELF_COMPONENT, Component.from_version(timestamp())]
+    cert_name = Name.normalize(key_name) + [issuer_id_component, Component.from_version(timestamp())]
     cert_val.name = cert_name
     cert_val.content = pub_key
     cert_val.meta_info = MetaInfo(content_type=ContentType.KEY, freshness_period=3600000)
     cert_val.signature_info = CertificateV2SignatureInfo()
     cert_val.signature_info.validity_period = ValidityPeriod()
-    cert_val.signature_info.validity_period.not_before = b'19700101T000000'
-    end_time = datetime.utcnow()
-    not_after = (f'{end_time.year+20:04}{end_time.month:02}{end_time.day:02}T'
-                 f'{end_time.hour:02}{end_time.minute:02}{end_time.second:02}').encode()
+    cur_time = start_time
+    not_before = cur_time.strftime('%Y%m%dT%H%M%S').encode()
+    cert_val.signature_info.validity_period.not_before = not_before
+    not_after = end_time.strftime('%Y%m%dT%H%M%S').encode()
     cert_val.signature_info.validity_period.not_after = not_after
 
     markers = {}
     cert_val._signer.set_arg(markers, signer)
     value = cert_val.encode(markers=markers)
     shrink_size = cert_val._shrink_len.get_arg(markers)
     type_len = get_tl_num_size(TypeNumber.DATA)
     size_len = get_tl_num_size(len(value) - shrink_size)
     buf = bytearray(type_len + size_len + len(value) - shrink_size)
     write_tl_num(TypeNumber.DATA, buf)
     write_tl_num(len(value) - shrink_size, buf, type_len)
-    buf[type_len+size_len:] = memoryview(value)[0:len(value)-shrink_size]
+    buf[type_len + size_len:] = memoryview(value)[0:len(value) - shrink_size]
     return cert_name, buf
 
 
-def parse_certificate(wire) -> CertificateV2Value:
-    wire = parse_and_check_tl(wire, TypeNumber.DATA)
-    return CertificateV2Value.parse(wire)
+def self_sign(key_name, pub_key, signer) -> Tuple[FormalName, VarBinaryStr]:
+    end_time = datetime.utcnow()
+    end_time.replace(year=end_time.year + 20)
+    return new_cert(key_name, SELF_COMPONENT, pub_key, signer,
+                    datetime.fromisoformat('1970-01-01T00:00:00'), end_time)
+
+
+def derive_cert(key_name, issuer_id, pub_key, signer, start_time, expire_sec):
+    end_time = start_time + timedelta(seconds=expire_sec)
+    if isinstance(issuer_id, str):
+        issuer_id = Component.from_str(issuer_id)
+    return new_cert(key_name, issuer_id, pub_key, signer, start_time, end_time)
```

### Comparing `python-ndn-0.3a1.post3/src/ndn/app_support/segment_fetcher.py` & `python-ndn-0.3a1.post4/src/ndn/app_support/segment_fetcher.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/client_conf.py` & `python-ndn-0.3a1.post4/src/ndn/client_conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,56 +14,60 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
 import os
 import sys
 from configparser import ConfigParser
+from .platform import Platform
 from .security import TpmFile, Keychain, KeychainSqlite3
 from .transport.stream_socket import Face, UnixFace, TcpFace
 if sys.platform == 'darwin':
     from .security.tpm.tpm_osx_keychain import TpmOsxKeychain
+if sys.platform == 'win32':
+    from .security.tpm.tpm_cng import TpmCng
 
 
 def read_client_conf():
-    def get_path():
-        path = os.path.expanduser('~/.ndn/client.conf')
-        if os.path.exists(path):
-            return path
-        path = '/usr/local/etc/ndn/client.conf'
-        if os.path.exists(path):
-            return path
-        path = '/opt/local/etc/ndn/client.conf'
-        if os.path.exists(path):
-            return path
-        path = '/etc/ndn/client.conf'
-        if os.path.exists(path):
-            return path
+    def get_path() -> str:
+        paths = Platform().client_conf_paths()
+        for p_str in paths:
+            p = os.path.expandvars(p_str)
+            if os.path.exists(p):
+                return p
+        return ''
 
-    def resolve_location(value):
+    def resolve_location(item: str, value: str) -> str:
         nonlocal path
         sp = value.split(':')
         if len(sp) == 1:
             schema = value
             loc = ''
         else:
             schema, loc = sp
         if not loc or not os.path.exists(loc):
             if loc and (path is not None):
                 loc = os.path.join(os.path.dirname(path), loc)
             if not loc or not os.path.exists(loc):
-                loc = '~/.ndn/ndnsec-key-file' if schema == 'tpm-file' else '~/.ndn'
-                loc = os.path.expanduser(loc)
+                if item == 'pib':
+                    paths = Platform().default_pib_paths()
+                else:
+                    paths = Platform().default_tpm_paths()
+                for p_str in paths:
+                    p = os.path.expandvars(p_str)
+                    if os.path.exists(p):
+                        loc = p
+                        break
         return ':'.join((schema, loc))
 
     path = get_path()
     ret = {
-        'transport': 'unix:///run/nfd.sock' if sys.platform == 'linux' else 'unix:///var/run/nfd.sock',
-        'pib': 'pib-sqlite3',
-        'tpm': 'tpm-osxkeychain' if sys.platform == 'darwin' else 'tpm-file'
+        'transport': Platform().default_transport(),
+        'pib': Platform().default_pib_schema(),
+        'tpm': Platform().default_tpm_schema()
     }
     if path:
         parser = ConfigParser()
         text = '[DEFAULT]\n'
         with open(path) as f:
             text += f.read()
         parser.read_string(text)
@@ -74,25 +78,27 @@
                 pass
     for key in ret.keys():
         try:
             ret[key] = os.environ[f'NDN_CLIENT_{key.upper()}']
         except KeyError:
             pass
     for key in ['pib', 'tpm']:
-        ret[key] = resolve_location(ret[key])
+        ret[key] = resolve_location(key, ret[key])
     return ret
 
 
 def default_keychain(pib: str, tpm: str) -> Keychain:
-    pib_schema, pib_loc = pib.split(':')
-    tpm_schema, tpm_loc = tpm.split(':')
+    pib_schema, pib_loc = pib.split(':', 1)
+    tpm_schema, tpm_loc = tpm.split(':', 1)
     if tpm_schema == 'tpm-file':
         tpm = TpmFile(tpm_loc)
     elif tpm_schema == 'tpm-osxkeychain':
         tpm = TpmOsxKeychain()
+    elif tpm_schema == 'tpm-cng':
+        tpm = TpmCng()
     else:
         raise ValueError(f'Unrecognized tpm schema: {tpm}')
     if pib_schema == 'pib-sqlite3':
         pib = KeychainSqlite3(os.path.join(pib_loc, 'pib.db'), tpm)
     else:
         raise ValueError(f'Unrecognized pib schema: {pib}')
     return pib
```

### Comparing `python-ndn-0.3a1.post3/src/ndn/contrib/cocoapy/__init__.py` & `python-ndn-0.3a1.post4/src/ndn/contrib/cocoapy/__init__.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/contrib/cocoapy/cocoalibs.py` & `python-ndn-0.3a1.post4/src/ndn/contrib/cocoapy/cocoalibs.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/contrib/cocoapy/cocoatypes.py` & `python-ndn-0.3a1.post4/src/ndn/contrib/cocoapy/cocoatypes.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/contrib/cocoapy/runtime.py` & `python-ndn-0.3a1.post4/src/ndn/contrib/cocoapy/runtime.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/encoding/name/Component.py` & `python-ndn-0.3a1.post4/src/ndn/encoding/name/Component.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/encoding/name/Name.py` & `python-ndn-0.3a1.post4/src/ndn/encoding/name/Name.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/encoding/ndn_format_0_3.py` & `python-ndn-0.3a1.post4/src/ndn/encoding/ndn_format_0_3.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/encoding/ndnlp_v2.py` & `python-ndn-0.3a1.post4/src/ndn/encoding/ndnlp_v2.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/encoding/signer.py` & `python-ndn-0.3a1.post4/src/ndn/encoding/signer.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/encoding/tlv_model.py` & `python-ndn-0.3a1.post4/src/ndn/encoding/tlv_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -679,15 +679,15 @@
         :return: the encoded Length.
         """
         if markers is None:
             markers = {}
         ret = 0
         for field in self._encoded_fields:
             ret += field.encoded_length(field.get_value(self), markers)
-        markers[f'##encoded_length'] = ret
+        markers['##encoded_length'] = ret
         return ret
 
     def encode(self,
                wire: VarBinaryStr = None,
                offset: int = 0,
                markers: Optional[dict] = None) -> VarBinaryStr:
         r"""
@@ -702,16 +702,16 @@
         :raises ValueError: some field is assigned with improper value.
         :raises TypeError: some field is assigned with value of wrong type.
         :raises IndexError: wire does not have enough length.
         :raises struct.error: a negative number is assigned to any non-negative integer field.
         """
         if markers is None:
             markers = {}
-        if f'##encoded_length' in markers:
-            length = markers[f'##encoded_length']
+        if '##encoded_length' in markers:
+            length = markers['##encoded_length']
         else:
             length = self.encoded_length(markers)
         if wire is None:
             wire = bytearray(length)
         wire_view = memoryview(wire)
         for field in self._encoded_fields:
             offset += field.encode_into(field.get_value(self), markers, wire_view, offset)
```

### Comparing `python-ndn-0.3a1.post3/src/ndn/encoding/tlv_type.py` & `python-ndn-0.3a1.post4/src/ndn/encoding/tlv_type.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/encoding/tlv_var.py` & `python-ndn-0.3a1.post4/src/ndn/encoding/tlv_var.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/name_tree.py` & `python-ndn-0.3a1.post4/src/ndn/name_tree.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/schema/policy.py` & `python-ndn-0.3a1.post4/src/ndn/schema/policy.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/schema/schema_tree.py` & `python-ndn-0.3a1.post4/src/ndn/schema/schema_tree.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/schema/simple_cache.py` & `python-ndn-0.3a1.post4/src/ndn/schema/simple_cache.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/schema/simple_node.py` & `python-ndn-0.3a1.post4/src/ndn/schema/simple_node.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/schema/simple_trust.py` & `python-ndn-0.3a1.post4/src/ndn/schema/simple_trust.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/schema/util.py` & `python-ndn-0.3a1.post4/src/ndn/schema/util.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/security/keychain/keychain.py` & `python-ndn-0.3a1.post4/src/ndn/security/keychain/keychain.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/security/keychain/keychain_digest.py` & `python-ndn-0.3a1.post4/src/ndn/security/keychain/keychain_digest.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/security/keychain/keychain_sqlite3.py` & `python-ndn-0.3a1.post4/src/ndn/security/keychain/keychain_sqlite3.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/security/osx.py` & `python-ndn-0.3a1.post4/src/ndn/platform/osx.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -----------------------------------------------------------------------------
-# Copyright (C) 2019-2020 The python-ndn authors
+# Copyright (C) 2019-2021 The python-ndn authors
 #
 # This file is part of python-ndn.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -11,16 +11,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
+import os
 import sys
+import asyncio as aio
 from ctypes import cdll, c_void_p, c_ubyte, POINTER, c_int32, c_ulong, c_uint16
+from .general import Platform
 if sys.platform == 'darwin':
     from ..contrib.cocoapy import cf, CFIndex, CFRange, CFAllocatorRef
 
 
 class OsxSec(object):
     __instance = None
 
@@ -104,7 +107,33 @@
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         for v in self._dict.values():
             if v:
                 cf.CFRelease(v)
         return False
+
+
+class Darwin(Platform):
+    def client_conf_paths(self):
+        return [os.path.expanduser('~/.ndn/client.conf'),
+                '/usr/local/etc/ndn/client.conf',
+                '/opt/local/etc/ndn/client.conf',
+                '/etc/ndn/client.conf']
+
+    def default_transport(self):
+        return 'unix:///var/run/nfd.sock'
+
+    def default_pib_schema(self):
+        return 'pib-sqlite3'
+
+    def default_pib_paths(self):
+        return [os.path.expanduser(r'~/.ndn')]
+
+    def default_tpm_schema(self):
+        return 'tpm-osxkeychain'
+
+    def default_tpm_paths(self):
+        return [os.path.expanduser(r'~/.ndn/ndnsec-key-file')]
+
+    async def open_unix_connection(self, path=None):
+        return await aio.open_unix_connection(path)
```

### Comparing `python-ndn-0.3a1.post3/src/ndn/security/signer/sha256_digest_signer.py` & `python-ndn-0.3a1.post4/src/ndn/security/signer/sha256_digest_signer.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/security/signer/sha256_ecdsa_signer.py` & `python-ndn-0.3a1.post4/src/ndn/security/signer/sha256_ecdsa_signer.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/security/signer/sha256_hmac_signer.py` & `python-ndn-0.3a1.post4/src/ndn/security/signer/sha256_hmac_signer.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/security/signer/sha256_rsa_signer.py` & `python-ndn-0.3a1.post4/src/ndn/security/signer/sha256_rsa_signer.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/security/tpm/tpm.py` & `python-ndn-0.3a1.post4/src/ndn/security/tpm/tpm.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/security/tpm/tpm_file.py` & `python-ndn-0.3a1.post4/src/ndn/security/tpm/tpm_file.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/security/tpm/tpm_osx_keychain.py` & `python-ndn-0.3a1.post4/src/ndn/security/tpm/tpm_osx_keychain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -----------------------------------------------------------------------------
-# Copyright (C) 2019-2020 The python-ndn authors
+# Copyright (C) 2019-2021 The python-ndn authors
 #
 # This file is part of python-ndn.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -21,15 +21,15 @@
 from ctypes import c_void_p, pointer, c_int
 from Cryptodome.Hash import SHA256
 from Cryptodome.PublicKey import RSA, ECC
 from ...encoding import Signer, NonStrictName, Name, SignatureType, KeyLocator, BinaryStr, FormalName
 from .tpm import Tpm
 if sys.platform == 'darwin':
     from ...contrib.cocoapy import cf, CFSTR, ObjCInstance, cfstring_to_string, cfnumber_to_number, kCFNumberIntType
-    from ..osx import OsxSec, ReleaseGuard
+    from ...platform.osx import OsxSec, ReleaseGuard
 
 
 class OsxSigner(Signer):
     def __init__(self, key_name: NonStrictName, key_bits, key_type, key_ref):
         self.key_ref = key_ref
         self.key_name = key_name
         if key_type == cfstring_to_string(OsxSec().kSecAttrKeyTypeRSA):
@@ -78,14 +78,15 @@
 
 
 class TpmOsxKeychain(Tpm):
     @staticmethod
     def _get_key(key_name: NonStrictName):
         sec = OsxSec()
         with ReleaseGuard() as g:
+            # TODO: what about name convension?
             logging.debug('Get OSX Key %s' % Name.to_str(key_name))
             g.key_label = CFSTR(Name.to_str(key_name))
             g.query = ObjCInstance(cf.CFDictionaryCreateMutable(None, 6, cf.kCFTypeDictionaryKeyCallBacks, None))
             cf.CFDictionaryAddValue(g.query, sec.kSecClass, sec.kSecClassKey)
             cf.CFDictionaryAddValue(g.query, sec.kSecAttrLabel, g.key_label)
             cf.CFDictionaryAddValue(g.query, sec.kSecAttrKeyClass, sec.kSecAttrKeyClassPrivate)
             cf.CFDictionaryAddValue(g.query, sec.kSecReturnAttributes, sec.kCFBooleanTrue)
```

### Comparing `python-ndn-0.3a1.post3/src/ndn/security/validator/digest_validator.py` & `python-ndn-0.3a1.post4/src/ndn/security/validator/digest_validator.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/transport/dummy_face.py` & `python-ndn-0.3a1.post4/src/ndn/transport/dummy_face.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/transport/stream_socket.py` & `python-ndn-0.3a1.post4/src/ndn/transport/stream_socket.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
 import io
 import abc
-import sys
 import asyncio as aio
 from typing import Optional, Callable, Coroutine, Any
 from ..encoding.tlv_var import read_tl_num_from_stream
-if sys.platform.startswith('win32'):
-    from .windows import open_unix_connection
+from ..platform import Platform
 
 
 class Face(metaclass=abc.ABCMeta):
     running: bool = False
     callback: Callable[[int, bytes], Coroutine[Any, None, None]] = None
 
     def __init__(self):
@@ -80,18 +78,15 @@
 
     def __init__(self, path: str = ''):
         super().__init__()
         if path:
             self.path = path
 
     async def open(self):
-        if sys.platform.startswith('win32'):
-            self.reader, self.writer = await open_unix_connection(self.path)
-        else:
-            self.reader, self.writer = await aio.open_unix_connection(self.path)
+        self.reader, self.writer = await Platform().open_unix_connection(self.path)
         self.running = True
 
 
 class TcpFace(StreamFace):
     host: str = '127.0.0.1'
     port: int = 6363
```

### Comparing `python-ndn-0.3a1.post3/src/ndn/types.py` & `python-ndn-0.3a1.post4/src/ndn/types.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/ndn/utils.py` & `python-ndn-0.3a1.post4/src/ndn/utils.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post3/src/python_ndn.egg-info/SOURCES.txt` & `python-ndn-0.3a1.post4/src/python_ndn.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 AUTHORS.rst
 COPYING
 README.rst
+pyproject.toml
+setup.cfg
 setup.py
 src/ndn/__init__.py
 src/ndn/app.py
 src/ndn/client_conf.py
 src/ndn/name_tree.py
 src/ndn/types.py
 src/ndn/utils.py
 src/ndn/app_support/__init__.py
 src/ndn/app_support/dispatcher.py
 src/ndn/app_support/nfd_mgmt.py
 src/ndn/app_support/security_v2.py
 src/ndn/app_support/segment_fetcher.py
+src/ndn/bin/__init__.py
+src/ndn/bin/sec/__init__.py
+src/ndn/bin/sec/__main__.py
+src/ndn/bin/tools/__init__.py
+src/ndn/bin/tools/__main__.py
 src/ndn/contrib/__init__.py
 src/ndn/contrib/cocoapy/__init__.py
 src/ndn/contrib/cocoapy/cocoalibs.py
 src/ndn/contrib/cocoapy/cocoatypes.py
 src/ndn/contrib/cocoapy/runtime.py
 src/ndn/encoding/__init__.py
 src/ndn/encoding/ndn_format_0_3.py
@@ -24,40 +31,46 @@
 src/ndn/encoding/signer.py
 src/ndn/encoding/tlv_model.py
 src/ndn/encoding/tlv_type.py
 src/ndn/encoding/tlv_var.py
 src/ndn/encoding/name/Component.py
 src/ndn/encoding/name/Name.py
 src/ndn/encoding/name/__init__.py
+src/ndn/platform/__init__.py
+src/ndn/platform/general.py
+src/ndn/platform/linux.py
+src/ndn/platform/osx.py
+src/ndn/platform/windows.py
 src/ndn/schema/__init__.py
 src/ndn/schema/policy.py
 src/ndn/schema/schema_tree.py
 src/ndn/schema/simple_cache.py
 src/ndn/schema/simple_node.py
 src/ndn/schema/simple_trust.py
 src/ndn/schema/util.py
 src/ndn/security/__init__.py
-src/ndn/security/osx.py
 src/ndn/security/keychain/__init__.py
 src/ndn/security/keychain/keychain.py
 src/ndn/security/keychain/keychain_digest.py
 src/ndn/security/keychain/keychain_sqlite3.py
 src/ndn/security/signer/__init__.py
 src/ndn/security/signer/sha256_digest_signer.py
 src/ndn/security/signer/sha256_ecdsa_signer.py
 src/ndn/security/signer/sha256_hmac_signer.py
 src/ndn/security/signer/sha256_rsa_signer.py
 src/ndn/security/tpm/__init__.py
 src/ndn/security/tpm/tpm.py
+src/ndn/security/tpm/tpm_cng.py
 src/ndn/security/tpm/tpm_file.py
 src/ndn/security/tpm/tpm_osx_keychain.py
 src/ndn/security/validator/__init__.py
 src/ndn/security/validator/digest_validator.py
+src/ndn/security/validator/known_key_validator.py
 src/ndn/transport/__init__.py
 src/ndn/transport/dummy_face.py
 src/ndn/transport/stream_socket.py
-src/ndn/transport/windows.py
 src/python_ndn.egg-info/PKG-INFO
 src/python_ndn.egg-info/SOURCES.txt
 src/python_ndn.egg-info/dependency_links.txt
+src/python_ndn.egg-info/entry_points.txt
 src/python_ndn.egg-info/requires.txt
 src/python_ndn.egg-info/top_level.txt
```

