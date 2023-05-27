# Comparing `tmp/python-mbedtls-2.6.1.tar.gz` & `tmp/python-mbedtls-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-mbedtls-2.6.1.tar", last modified: Wed Feb 15 21:12:45 2023, max compression
+gzip compressed data, was "python-mbedtls-2.7.0.tar", last modified: Sat May 27 19:44:02 2023, max compression
```

## Comparing `python-mbedtls-2.6.1.tar` & `python-mbedtls-2.7.0.tar`

### file list

```diff
@@ -1,123 +1,131 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 21:12:45.867013 python-mbedtls-2.6.1/
--rw-rw-rw-   0        0        0     2310 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    13542 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/ChangeLog
--rw-rw-rw-   0        0        0     1112 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/LICENSE.txt
--rw-rw-rw-   0        0        0      458 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0    14078 2023-02-15 21:12:45.867013 python-mbedtls-2.6.1/PKG-INFO
--rw-rw-rw-   0        0        0    13185 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-15 21:12:45.804573 python-mbedtls-2.6.1/docs/
-drwxrwxrwx   0        0        0        0 2023-02-15 21:12:45.820138 python-mbedtls-2.6.1/docs/source/
--rw-rw-rw-   0        0        0     2082 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/docs/source/apicipher.rst
--rw-rw-rw-   0        0        0      299 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/docs/source/apimd.rst
--rw-rw-rw-   0        0        0       93 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/docs/source/apimpi.rst
--rw-rw-rw-   0        0        0      125 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/docs/source/apipk.rst
--rw-rw-rw-   0        0        0       97 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/docs/source/apisecrets.rst
--rw-rw-rw-   0        0        0       93 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/docs/source/apitls.rst
--rw-rw-rw-   0        0        0       96 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/docs/source/apix509.rst
--rw-rw-rw-   0        0        0      520 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/docs/source/index.rst
-drwxrwxrwx   0        0        0        0 2023-02-15 21:12:45.820138 python-mbedtls-2.6.1/programs/
--rw-rw-rw-   0        0        0     5770 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/programs/client.py
--rw-rw-rw-   0        0        0     6024 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/programs/server.py
--rw-rw-rw-   0        0        0     2229 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-02-15 21:12:45.820138 python-mbedtls-2.6.1/requirements/
--rw-rw-rw-   0        0        0       99 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/requirements/build.in
--rw-rw-rw-   0        0        0      525 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/requirements/build.txt
--rw-rw-rw-   0        0        0       26 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/requirements/docs.in
--rw-rw-rw-   0        0        0      745 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/requirements/docs.txt
--rw-rw-rw-   0        0        0      182 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/requirements/tests.in
--rw-rw-rw-   0        0        0     1005 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/requirements/tests.txt
--rw-rw-rw-   0        0        0       25 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/requirements/typing.in
--rw-rw-rw-   0        0        0      273 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/requirements/typing.txt
--rw-rw-rw-   0        0        0      210 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-02-15 21:12:45.835764 python-mbedtls-2.6.1/scripts/
--rw-rw-rw-   0        0        0      700 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/scripts/build-wheel.sh
--rw-rw-rw-   0        0        0      167 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/scripts/check-future-annotations.sh
--rw-rw-rw-   0        0        0      151 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/scripts/check-license-header.sh
--rw-rw-rw-   0        0        0      169 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/scripts/deploy.sh
--rw-rw-rw-   0        0        0      503 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/scripts/download-mbedtls.sh
--rw-rw-rw-   0        0        0      483 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/scripts/install-mbedtls.sh
--rw-rw-rw-   0        0        0     1038 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/scripts/install-pymbedtls.sh
--rw-rw-rw-   0        0        0      256 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/scripts/run-tests.sh
--rw-rw-rw-   0        0        0      732 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/scripts/start-devpi.sh
--rw-rw-rw-   0        0        0       45 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/scripts/stop-devpi.sh
--rw-rw-rw-   0        0        0      277 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/scripts/update-reqs.sh
--rw-rw-rw-   0        0        0       42 2023-02-15 21:12:45.867013 python-mbedtls-2.6.1/setup.cfg
--rw-rw-rw-   0        0        0     6131 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-15 21:12:45.804573 python-mbedtls-2.6.1/src/
-drwxrwxrwx   0        0        0        0 2023-02-15 21:12:45.851389 python-mbedtls-2.6.1/src/mbedtls/
--rw-rw-rw-   0        0        0      819 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/__init__.py
--rw-rw-rw-   0        0        0     2137 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/_md.pxd
--rw-rw-rw-   0        0        0     1209 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/_md.pyi
--rw-rw-rw-   0        0        0     8152 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/_md.pyx
--rw-rw-rw-   0        0        0      233 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/_platform.pxd
--rw-rw-rw-   0        0        0      151 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/_platform.pyi
--rw-rw-rw-   0        0        0      262 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/_platform.pyx
--rw-rw-rw-   0        0        0     2894 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/_random.pxd
--rw-rw-rw-   0        0        0      925 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/_random.pyi
--rw-rw-rw-   0        0        0     4892 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/_random.pyx
--rw-rw-rw-   0        0        0      922 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/_ringbuf.pxd
--rw-rw-rw-   0        0        0     5607 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/_ringbuf.pyx
--rw-rw-rw-   0        0        0    15478 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/_tls.pxd
--rw-rw-rw-   0        0        0     4212 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/_tls.pyi
--rw-rw-rw-   0        0        0    41710 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/_tls.pyx
--rw-rw-rw-   0        0        0    15109 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/_tlsi.py
-drwxrwxrwx   0        0        0        0 2023-02-15 21:12:45.851389 python-mbedtls-2.6.1/src/mbedtls/cipher/
--rw-rw-rw-   0        0        0     2810 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/cipher/AES.py
--rw-rw-rw-   0        0        0     1494 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/cipher/ARC4.py
--rw-rw-rw-   0        0        0     2095 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/cipher/ARIA.py
--rw-rw-rw-   0        0        0     1747 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/cipher/Blowfish.py
--rw-rw-rw-   0        0        0     2317 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/cipher/CHACHA20.py
--rw-rw-rw-   0        0        0     1838 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/cipher/Camellia.py
--rw-rw-rw-   0        0        0     1635 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/cipher/DES.py
--rw-rw-rw-   0        0        0     1725 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/cipher/DES3.py
--rw-rw-rw-   0        0        0     1718 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/cipher/DES3dbl.py
--rw-rw-rw-   0        0        0     2474 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/cipher/__init__.py
--rw-rw-rw-   0        0        0     5241 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/cipher/_cipher.pxd
--rw-rw-rw-   0        0        0     1651 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/cipher/_cipher.pyi
--rw-rw-rw-   0        0        0     9518 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/cipher/_cipher.pyx
--rw-rw-rw-   0        0        0      231 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/exceptions.pxd
--rw-rw-rw-   0        0        0      329 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/exceptions.pyi
--rw-rw-rw-   0        0        0     1494 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/exceptions.pyx
--rw-rw-rw-   0        0        0     2734 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/hashlib.py
--rw-rw-rw-   0        0        0      909 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/hkdf.pxd
--rw-rw-rw-   0        0        0      586 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/hkdf.pyi
--rw-rw-rw-   0        0        0     5118 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/hkdf.pyx
--rw-rw-rw-   0        0        0     2987 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/hmac.py
--rw-rw-rw-   0        0        0     3286 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/mpi.pxd
--rw-rw-rw-   0        0        0     3625 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/mpi.pyi
--rw-rw-rw-   0        0        0    11411 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/mpi.pyx
--rw-rw-rw-   0        0        0    14254 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/pk.pxd
--rw-rw-rw-   0        0        0     8158 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/pk.pyi
--rw-rw-rw-   0        0        0    36413 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/pk.pyx
--rw-rw-rw-   0        0        0        0 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/py.typed
--rw-rw-rw-   0        0        0     1723 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/secrets.py
--rw-rw-rw-   0        0        0    15190 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/tls.py
--rw-rw-rw-   0        0        0      383 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/version.pxd
--rw-rw-rw-   0        0        0      457 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/version.pyi
--rw-rw-rw-   0        0        0     1665 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/version.pyx
--rw-rw-rw-   0        0        0     9874 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/x509.pxd
--rw-rw-rw-   0        0        0     5740 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/x509.pyi
--rw-rw-rw-   0        0        0    32201 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/src/mbedtls/x509.pyx
-drwxrwxrwx   0        0        0        0 2023-02-15 21:12:45.851389 python-mbedtls-2.6.1/src/python_mbedtls.egg-info/
--rw-rw-rw-   0        0        0    14078 2023-02-15 21:12:45.000000 python-mbedtls-2.6.1/src/python_mbedtls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2581 2023-02-15 21:12:45.000000 python-mbedtls-2.6.1/src/python_mbedtls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 21:12:45.000000 python-mbedtls-2.6.1/src/python_mbedtls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-02-15 21:12:45.000000 python-mbedtls-2.6.1/src/python_mbedtls.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-15 21:12:45.000000 python-mbedtls-2.6.1/src/python_mbedtls.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-15 21:12:45.867013 python-mbedtls-2.6.1/tests/
--rw-rw-rw-   0        0        0     1928 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/tests/conftest.py
--rw-rw-rw-   0        0        0     1375 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/tests/test_assertion_rewriting.py
--rw-rw-rw-   0        0        0    13296 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/tests/test_cipher.py
--rw-rw-rw-   0        0        0      673 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/tests/test_error.py
--rw-rw-rw-   0        0        0    11093 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/tests/test_hkdf.py
--rw-rw-rw-   0        0        0     6915 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/tests/test_md.py
--rw-rw-rw-   0        0        0     7640 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/tests/test_mpi.py
--rw-rw-rw-   0        0        0    19072 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/tests/test_pk.py
--rw-rw-rw-   0        0        0      317 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/tests/test_platform.py
--rw-rw-rw-   0        0        0     4128 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/tests/test_random.py
--rw-rw-rw-   0        0        0      715 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/tests/test_readme.py
--rw-rw-rw-   0        0        0     8157 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/tests/test_ringbuf.py
--rw-rw-rw-   0        0        0     1637 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/tests/test_secrets.py
--rw-rw-rw-   0        0        0    37533 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/tests/test_tls.py
--rw-rw-rw-   0        0        0      879 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/tests/test_version.py
--rw-rw-rw-   0        0        0    10384 2023-02-15 21:12:14.000000 python-mbedtls-2.6.1/tests/test_x509.py
+drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.977504 python-mbedtls-2.7.0/
+-rw-rw-rw-   0        0        0     2310 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    13721 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/ChangeLog
+-rw-rw-rw-   0        0        0     1112 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      458 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    14078 2023-05-27 19:44:02.977504 python-mbedtls-2.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13185 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.915009 python-mbedtls-2.7.0/docs/
+drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.915009 python-mbedtls-2.7.0/docs/source/
+-rw-rw-rw-   0        0        0     2082 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/docs/source/apicipher.rst
+-rw-rw-rw-   0        0        0      299 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/docs/source/apimd.rst
+-rw-rw-rw-   0        0        0       93 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/docs/source/apimpi.rst
+-rw-rw-rw-   0        0        0      125 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/docs/source/apipk.rst
+-rw-rw-rw-   0        0        0       97 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/docs/source/apisecrets.rst
+-rw-rw-rw-   0        0        0       93 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/docs/source/apitls.rst
+-rw-rw-rw-   0        0        0       96 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/docs/source/apix509.rst
+-rw-rw-rw-   0        0        0      520 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/docs/source/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.930631 python-mbedtls-2.7.0/programs/
+-rw-rw-rw-   0        0        0     5770 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/programs/client.py
+-rw-rw-rw-   0        0        0     6024 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/programs/server.py
+-rw-rw-rw-   0        0        0     2221 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.930631 python-mbedtls-2.7.0/requirements/
+-rw-rw-rw-   0        0        0       99 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/requirements/build.in
+-rw-rw-rw-   0        0        0      525 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/requirements/build.txt
+-rw-rw-rw-   0        0        0       26 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/requirements/docs.in
+-rw-rw-rw-   0        0        0      767 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/requirements/docs.txt
+-rw-rw-rw-   0        0        0      182 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/requirements/tests.in
+-rw-rw-rw-   0        0        0      992 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/requirements/tests.txt
+-rw-rw-rw-   0        0        0       25 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/requirements/typing.in
+-rw-rw-rw-   0        0        0      273 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/requirements/typing.txt
+-rw-rw-rw-   0        0        0      209 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.930631 python-mbedtls-2.7.0/scripts/
+-rw-rw-rw-   0        0        0      700 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/build-wheel.sh
+-rw-rw-rw-   0        0        0      167 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/check-future-annotations.sh
+-rw-rw-rw-   0        0        0      151 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/check-license-header.sh
+-rw-rw-rw-   0        0        0      169 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/deploy.sh
+-rw-rw-rw-   0        0        0      503 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/download-mbedtls.sh
+-rw-rw-rw-   0        0        0      483 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/install-mbedtls.sh
+-rw-rw-rw-   0        0        0     1038 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/install-pymbedtls.sh
+-rw-rw-rw-   0        0        0      256 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/run-tests.sh
+-rw-rw-rw-   0        0        0      732 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/start-devpi.sh
+-rw-rw-rw-   0        0        0       45 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/stop-devpi.sh
+-rw-rw-rw-   0        0        0      277 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/update-reqs.sh
+-rw-rw-rw-   0        0        0       42 2023-05-27 19:44:02.977504 python-mbedtls-2.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     6131 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.915009 python-mbedtls-2.7.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.961879 python-mbedtls-2.7.0/src/mbedtls/
+-rw-rw-rw-   0        0        0      819 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/__init__.py
+-rw-rw-rw-   0        0        0      495 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_asn1.pxd
+-rw-rw-rw-   0        0        0      168 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_debug.pxd
+-rw-rw-rw-   0        0        0     1617 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_dhm.pxd
+-rw-rw-rw-   0        0        0     2287 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_ecdh.pxd
+-rw-rw-rw-   0        0        0     1036 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_ecdsa.pxd
+-rw-rw-rw-   0        0        0     4499 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_ecp.pxd
+-rw-rw-rw-   0        0        0     2092 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_md.pxd
+-rw-rw-rw-   0        0        0     1209 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_md.pyi
+-rw-rw-rw-   0        0        0     8152 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_md.pyx
+-rw-rw-rw-   0        0        0      183 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_platform.pxd
+-rw-rw-rw-   0        0        0      151 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_platform.pyi
+-rw-rw-rw-   0        0        0      262 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_platform.pyx
+-rw-rw-rw-   0        0        0     2844 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_random.pxd
+-rw-rw-rw-   0        0        0      925 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_random.pyi
+-rw-rw-rw-   0        0        0     4892 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_random.pyx
+-rw-rw-rw-   0        0        0      922 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_ringbuf.pxd
+-rw-rw-rw-   0        0        0     5607 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_ringbuf.pyx
+-rw-rw-rw-   0        0        0     1260 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_rsa.pxd
+-rw-rw-rw-   0        0        0      825 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_timing.pxd
+-rw-rw-rw-   0        0        0    14971 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_tls.pxd
+-rw-rw-rw-   0        0        0     4259 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_tls.pyi
+-rw-rw-rw-   0        0        0    43292 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_tls.pyx
+-rw-rw-rw-   0        0        0    17041 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_tlsi.py
+drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.961879 python-mbedtls-2.7.0/src/mbedtls/cipher/
+-rw-rw-rw-   0        0        0     2810 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/AES.py
+-rw-rw-rw-   0        0        0     1494 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/ARC4.py
+-rw-rw-rw-   0        0        0     2095 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/ARIA.py
+-rw-rw-rw-   0        0        0     1747 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/Blowfish.py
+-rw-rw-rw-   0        0        0     2317 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/CHACHA20.py
+-rw-rw-rw-   0        0        0     1838 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/Camellia.py
+-rw-rw-rw-   0        0        0     1635 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/DES.py
+-rw-rw-rw-   0        0        0     1725 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/DES3.py
+-rw-rw-rw-   0        0        0     1718 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/DES3dbl.py
+-rw-rw-rw-   0        0        0     2474 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/__init__.py
+-rw-rw-rw-   0        0        0     5241 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/_cipher.pxd
+-rw-rw-rw-   0        0        0     1651 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/_cipher.pyi
+-rw-rw-rw-   0        0        0     9518 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/_cipher.pyx
+-rw-rw-rw-   0        0        0      183 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/exceptions.pxd
+-rw-rw-rw-   0        0        0      329 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/exceptions.pyi
+-rw-rw-rw-   0        0        0     1494 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/exceptions.pyx
+-rw-rw-rw-   0        0        0     2734 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/hashlib.py
+-rw-rw-rw-   0        0        0      862 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/hkdf.pxd
+-rw-rw-rw-   0        0        0      586 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/hkdf.pyi
+-rw-rw-rw-   0        0        0     5118 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/hkdf.pyx
+-rw-rw-rw-   0        0        0     2987 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/hmac.py
+-rw-rw-rw-   0        0        0     3238 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/mpi.pxd
+-rw-rw-rw-   0        0        0     3625 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/mpi.pyi
+-rw-rw-rw-   0        0        0    11411 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/mpi.pyx
+-rw-rw-rw-   0        0        0     4408 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/pk.pxd
+-rw-rw-rw-   0        0        0     8158 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/pk.pyi
+-rw-rw-rw-   0        0        0    36634 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/pk.pyx
+-rw-rw-rw-   0        0        0        0 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/py.typed
+-rw-rw-rw-   0        0        0     1723 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/secrets.py
+-rw-rw-rw-   0        0        0    15543 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/tls.py
+-rw-rw-rw-   0        0        0      333 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/version.pxd
+-rw-rw-rw-   0        0        0      457 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/version.pyi
+-rw-rw-rw-   0        0        0     1665 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/version.pyx
+-rw-rw-rw-   0        0        0     9497 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/x509.pxd
+-rw-rw-rw-   0        0        0     5740 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/x509.pyi
+-rw-rw-rw-   0        0        0    32201 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/x509.pyx
+drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.961879 python-mbedtls-2.7.0/src/python_mbedtls.egg-info/
+-rw-rw-rw-   0        0        0    14078 2023-05-27 19:44:02.000000 python-mbedtls-2.7.0/src/python_mbedtls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2758 2023-05-27 19:44:02.000000 python-mbedtls-2.7.0/src/python_mbedtls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 19:44:02.000000 python-mbedtls-2.7.0/src/python_mbedtls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-27 19:44:02.000000 python-mbedtls-2.7.0/src/python_mbedtls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-27 19:44:02.000000 python-mbedtls-2.7.0/src/python_mbedtls.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.977504 python-mbedtls-2.7.0/tests/
+-rw-rw-rw-   0        0        0     1928 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/conftest.py
+-rw-rw-rw-   0        0        0     1375 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_assertion_rewriting.py
+-rw-rw-rw-   0        0        0    13296 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_cipher.py
+-rw-rw-rw-   0        0        0      673 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_error.py
+-rw-rw-rw-   0        0        0    11093 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_hkdf.py
+-rw-rw-rw-   0        0        0     6915 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_md.py
+-rw-rw-rw-   0        0        0     7640 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_mpi.py
+-rw-rw-rw-   0        0        0    19072 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_pk.py
+-rw-rw-rw-   0        0        0      317 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_platform.py
+-rw-rw-rw-   0        0        0     4128 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_random.py
+-rw-rw-rw-   0        0        0      715 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_readme.py
+-rw-rw-rw-   0        0        0     8157 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_ringbuf.py
+-rw-rw-rw-   0        0        0     1637 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_secrets.py
+-rw-rw-rw-   0        0        0    38946 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_tls.py
+-rw-rw-rw-   0        0        0      879 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_version.py
+-rw-rw-rw-   0        0        0    10426 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_x509.py
```

### Comparing `python-mbedtls-2.6.1/CONTRIBUTING.md` & `python-mbedtls-2.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/ChangeLog` & `python-mbedtls-2.7.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+[2.7.0] - 2023-05-27
+
+* ci: Update wheels to mbedtls 2.28.3.
+* tls: Add `setmtu`, for the maximum transport unit, and an
+optional `max_fragmentation_length` configuration.
+
 [2.6.1] - 2023-02-15
 
 * cipher: Fix encryption and decryption of 0-length strings.
 
 [2.6.0] - 2023-01-15
 
 * ci: Update wheels to mbedtls 2.28.2.
```

### Comparing `python-mbedtls-2.6.1/LICENSE.txt` & `python-mbedtls-2.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/PKG-INFO` & `python-mbedtls-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: python-mbedtls
-Version: 2.6.1
+Version: 2.7.0
 Summary: hash, hmac, RSA, ECC, X.509, TLS, DTLS, handshakes, and secrets with an mbed TLS back end
 Home-page: https://github.com/Synss/python-mbedtls
-Download-URL: https://github.com/Synss/python-mbedtls/tarball/2.6.1
+Download-URL: https://github.com/Synss/python-mbedtls/tarball/2.7.0
 Author: Mathias Laurin
 Author-email: Mathias.Laurin@github.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -83,15 +83,15 @@
 
 https://synss.github.io/python-mbedtls/
 
 
 Installation
 ============
 
-The bindings are tested with mbedTLS 2.28.2 for Python 3.7,
+The bindings are tested with mbedTLS 2.28.3 for Python 3.7,
 3.8, 3.9, 3.10, and 3.11 on Linux, macOS, and Windows.
 
 `manylinux`_ wheels are available for 64-bit Linux systems.  Install
 with ``pip install python-mbedtls``.
 
 .. _manylinux: https://www.python.org/dev/peps/pep-0513/
 
@@ -105,16 +105,16 @@
 Check which version of mbed TLS is being used by python-mbedtls
 ---------------------------------------------------------------
 
 The *mbedtls.version* module shows the run-time version
 information to mbed TLS.
 
 >>> from mbedtls import version
->>> _ = version.version  # "mbed TLS 2.28.2"
->>> _ = version.version_info  # (2, 28, 2)
+>>> _ = version.version  # "mbed TLS 2.28.3"
+>>> _ = version.version_info  # (2, 28, 3)
 
 
 Message digest
 --------------
 
 The *mbedtls.hashlib* module supports MD2, MD4, MD5, SHA-1, SHA-2
 (in 224, 256, 384, and 512-bits), and RIPEMD-160 secure hashes
```

### Comparing `python-mbedtls-2.6.1/README.rst` & `python-mbedtls-2.7.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 https://synss.github.io/python-mbedtls/
 
 
 Installation
 ============
 
-The bindings are tested with mbedTLS 2.28.2 for Python 3.7,
+The bindings are tested with mbedTLS 2.28.3 for Python 3.7,
 3.8, 3.9, 3.10, and 3.11 on Linux, macOS, and Windows.
 
 `manylinux`_ wheels are available for 64-bit Linux systems.  Install
 with ``pip install python-mbedtls``.
 
 .. _manylinux: https://www.python.org/dev/peps/pep-0513/
 
@@ -84,16 +84,16 @@
 Check which version of mbed TLS is being used by python-mbedtls
 ---------------------------------------------------------------
 
 The *mbedtls.version* module shows the run-time version
 information to mbed TLS.
 
 >>> from mbedtls import version
->>> _ = version.version  # "mbed TLS 2.28.2"
->>> _ = version.version_info  # (2, 28, 2)
+>>> _ = version.version  # "mbed TLS 2.28.3"
+>>> _ = version.version_info  # (2, 28, 3)
 
 
 Message digest
 --------------
 
 The *mbedtls.hashlib* module supports MD2, MD4, MD5, SHA-1, SHA-2
 (in 224, 256, 384, and 512-bits), and RIPEMD-160 secure hashes
```

### Comparing `python-mbedtls-2.6.1/docs/source/apicipher.rst` & `python-mbedtls-2.7.0/docs/source/apicipher.rst`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/docs/source/index.rst` & `python-mbedtls-2.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/programs/client.py` & `python-mbedtls-2.7.0/programs/client.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/programs/server.py` & `python-mbedtls-2.7.0/programs/server.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/pyproject.toml` & `python-mbedtls-2.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -88,8 +88,8 @@
 ignore-docstrings = "yes"
 min-similarity-lines = "8"
 
 [tool.pytest.ini_options]
 markers = "e2e: end-to-end tests"
 
 [tool.ruff]
-ignore = ["E701", "E704"]
+ignore = ["E701"]
```

### Comparing `python-mbedtls-2.6.1/requirements/build.txt` & `python-mbedtls-2.7.0/requirements/build.txt`

 * *Files 24% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
 #    pip-compile --no-annotate --resolver=backtracking requirements/build.in
 #
 build==0.10.0
 click==8.1.3
-cython==0.29.33
+cython==0.29.35
 delocate==0.10.4 ; sys_platform == "darwin"
-importlib-metadata==6.0.0
-packaging==23.0
-pip-tools==6.12.1
+importlib-metadata==6.6.0
+packaging==23.1
+pip-tools==6.13.0
 pyproject-hooks==1.0.0
 tomli==2.0.1
-typing-extensions==4.4.0
-wheel==0.38.4
-zipp==3.11.0
+typing-extensions==4.6.2
+wheel==0.40.0
+zipp==3.15.0
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `python-mbedtls-2.6.1/requirements/docs.txt` & `python-mbedtls-2.7.0/requirements/docs.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 #
 # This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
 #    pip-compile --no-annotate --resolver=backtracking requirements/docs.in
 #
 alabaster==0.7.13
-babel==2.11.0
-certifi==2022.12.7
-charset-normalizer==3.0.1
-docutils==0.17.1
+babel==2.12.1
+certifi==2023.5.7
+charset-normalizer==3.1.0
+docutils==0.18.1
 idna==3.4
 imagesize==1.4.1
-importlib-metadata==6.0.0
+importlib-metadata==6.6.0
 jinja2==3.1.2
-markupsafe==2.1.1
-packaging==23.0
-pygments==2.14.0
-pytz==2022.7.1
-requests==2.28.2
+markupsafe==2.1.2
+packaging==23.1
+pygments==2.15.1
+pytz==2023.3
+requests==2.31.0
 snowballstemmer==2.2.0
 sphinx==5.3.0
-sphinx-rtd-theme==1.1.1
+sphinx-rtd-theme==1.2.1
 sphinxcontrib-applehelp==1.0.2
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-jquery==4.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-typing-extensions==4.4.0
-urllib3==1.26.14
-zipp==3.11.0
+typing-extensions==4.6.2
+urllib3==2.0.2
+zipp==3.15.0
```

### Comparing `python-mbedtls-2.6.1/requirements/tests.txt` & `python-mbedtls-2.7.0/requirements/tests.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 #
 # This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
 #    pip-compile --no-annotate --resolver=backtracking requirements/tests.in
 #
-astroid==2.13.2
-attrs==22.2.0
-bleach==5.0.1
+astroid==2.15.5
+bleach==6.0.0
 cfgv==3.3.1
-coverage[toml]==7.0.5
-cython==0.29.33
+coverage[toml]==7.2.6
+cython==0.29.35
 dill==0.3.6
 distlib==0.3.6
-docutils==0.19
-exceptiongroup==1.1.0
-filelock==3.9.0
-identify==2.5.13
-importlib-metadata==6.0.0
+docutils==0.20.1
+exceptiongroup==1.1.1
+filelock==3.12.0
+identify==2.5.24
+importlib-metadata==6.6.0
 iniconfig==2.0.0
-isort==5.11.4
+isort==5.11.5
 lazy-object-proxy==1.9.0
 mccabe==0.7.0
-nodeenv==1.7.0
-packaging==23.0
-platformdirs==2.6.2
+nodeenv==1.8.0
+packaging==23.1
+platformdirs==3.5.1
 pluggy==1.0.0
 pre-commit==2.21.0
-pygments==2.14.0
-pylint==2.15.10
+pygments==2.15.1
+pylint==2.17.4
 pylint-per-file-ignores==1.0.0
-pytest==7.2.1
-pytest-cov==4.0.0
+pytest==7.3.1
+pytest-cov==4.1.0
 pytest-repeat==0.9.1
 pytest-timeout==2.1.0
 pyyaml==6.0
 readme-renderer==37.3
 six==1.16.0
 tomli==2.0.1
-tomlkit==0.11.6
+tomlkit==0.11.8
 typed-ast==1.5.4
-typing-extensions==4.4.0
-virtualenv==20.17.1
+typing-extensions==4.6.2
+virtualenv==20.23.0
 webencodings==0.5.1
-wrapt==1.14.1
-zipp==3.11.0
+wrapt==1.15.0
+zipp==3.15.0
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `python-mbedtls-2.6.1/scripts/build-wheel.sh` & `python-mbedtls-2.7.0/scripts/build-wheel.sh`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/scripts/install-pymbedtls.sh` & `python-mbedtls-2.7.0/scripts/install-pymbedtls.sh`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/scripts/start-devpi.sh` & `python-mbedtls-2.7.0/scripts/start-devpi.sh`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/setup.py` & `python-mbedtls-2.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             match = pattern.match(line)
             if match:
                 return match.group(1)
         raise RuntimeError()
 
 
 VERSION = _get_version()
-MBEDTLS_VERSION = "2.28.2"
+MBEDTLS_VERSION = "2.28.3"
 DOWNLOAD_URL = f"https://github.com/Synss/python-mbedtls/tarball/{VERSION}"
 
 
 __mbedtls_version_info__ = tuple(map(int, MBEDTLS_VERSION.split(".")))
 __mbedtls_url__ = "https://tls.mbed.org"
```

### Comparing `python-mbedtls-2.6.1/src/mbedtls/__init__.py` & `python-mbedtls-2.7.0/src/mbedtls/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import mbedtls.hmac as hmac
 import mbedtls.pk as pk
 import mbedtls.secrets as secrets
 import mbedtls.tls as tls
 import mbedtls.version as version
 import mbedtls.x509 as x509
 
-__version__ = "2.6.1"
+__version__ = "2.7.0"
 
 __all__ = (
     "cipher",
     "exceptions",
     "hashlib",
     "hkdf",
     "hmac",
```

### Comparing `python-mbedtls-2.6.1/src/mbedtls/_md.pxd` & `python-mbedtls-2.7.0/src/mbedtls/_md.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2015, Elaborated Networks GmbH
 # Copyright (c) 2018, Mathias Laurin
 
-"""Declarations from `mbedtls/md.h`."""
-
-
 cdef extern from "mbedtls/md.h" nogil:
     ctypedef struct mbedtls_md_info_t:
         pass
 
     ctypedef enum mbedtls_md_type_t:
         pass
```

### Comparing `python-mbedtls-2.6.1/src/mbedtls/_md.pyi` & `python-mbedtls-2.7.0/src/mbedtls/_md.pyi`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/_md.pyx` & `python-mbedtls-2.7.0/src/mbedtls/_md.pyx`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/_random.pxd` & `python-mbedtls-2.7.0/src/mbedtls/_random.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2016, Elaborated Networks GmbH
 # Copyright (c) 2019, Mathias Laurin
 
-"""Declarations for `mbedtls/ctr_drbg.h`."""
-
-
 cdef extern from "mbedtls/entropy.h" nogil:
     ctypedef struct mbedtls_entropy_context:
         pass
 
     void mbedtls_entropy_init(mbedtls_entropy_context *ctx)
     void mbedtls_entropy_free(mbedtls_entropy_context *ctx)
     # int mbedtls_entropy_add_source(
```

### Comparing `python-mbedtls-2.6.1/src/mbedtls/_random.pyi` & `python-mbedtls-2.7.0/src/mbedtls/_random.pyi`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/_random.pyx` & `python-mbedtls-2.7.0/src/mbedtls/_random.pyx`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/_ringbuf.pxd` & `python-mbedtls-2.7.0/src/mbedtls/_ringbuf.pxd`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/_ringbuf.pyx` & `python-mbedtls-2.7.0/src/mbedtls/_ringbuf.pyx`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/_tls.pxd` & `python-mbedtls-2.7.0/src/mbedtls/_tls.pxd`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2018, Mathias Laurin
 
-"""Declarations from `mbedtls/ssl.h`."""
-
+from libc.stdint cimport uint16_t
 
+cimport mbedtls._ecdh as _ecdh
 cimport mbedtls._ringbuf as _rb
+cimport mbedtls._timing as _timing
 cimport mbedtls.pk as _pk
 cimport mbedtls.x509 as _x509
 
 cdef:
     enum:
         MBEDTLS_SSL_TRANSPORT_STREAM = 0
         MBEDTLS_SSL_TRANSPORT_DATAGRAM = 1
@@ -65,54 +66,24 @@
         MBEDTLS_ERR_SSL_CLIENT_RECONNECT = -0x6780
         MBEDTLS_ERR_SSL_PEER_CLOSE_NOTIFY = -0x7880
         MBEDTLS_ERR_SSL_BUFFER_TOO_SMALL = -0x6a00
         MBEDTLS_ERR_SSL_HELLO_VERIFY_REQUIRED = -0x6a80
         MBEDTLS_ERR_SSL_BAD_INPUT_DATA = -0x7100
 
 
-cdef extern from "mbedtls/debug.h" nogil:
-    void mbedtls_debug_set_threshold(int threshold)
-
-
-cdef extern from "mbedtls/timing.h" nogil:
-    # This provides callbacks for DTLS with blocking IO.
-
-    ctypedef struct mbedtls_timing_hr_time:
-        pass
-
-    ctypedef struct mbedtls_timing_delay_context:
-        mbedtls_timing_hr_time timer
-        int int_ms
-        int fin_ms
-
-    # extern volatile int mbedtls_timing_alarmed
-
-    # unsigned long mbedtls_timing_hardclock()
-    # unsigned long mbedtls_timing_get_timer(
-    #     mbedtls_timing_hr_time *,
-    #     int reset,
-    # )
-    # void mbedtls_set_alarm(int seconds)
-
-    # mbedtls_ssl_set_timer_t callback
-    void mbedtls_timing_set_delay(void *data, int int_ms, int fin_ms)
-    # mbedtls_ssl_get_timer_t callback
-    int mbedtls_timing_get_delay(void *data)
-
-
 cdef extern from "mbedtls/ssl_internal.h" nogil:
     ctypedef struct mbedtls_ssl_transform:
         pass
 
     ctypedef struct mbedtls_ssl_handshake_params:
         int sig_alg
         int verify_sig_alg
         # Diffie-Hellman key exchange:
         # mbedtls_dhm_context dhm_ctx
-        _pk.mbedtls_ecdh_context ecdh_ctx
+        _ecdh.mbedtls_ecdh_context ecdh_ctx
         # EC-J-Pake (not very much used anymore)
         # mbedtls_ecjpake_context ecjpake_ctx
         mbedtls_ssl_key_cert *key_cert
 
     ctypedef struct mbedtls_ssl_key_cert:
         _x509.mbedtls_x509_crt *cert
         _pk.mbedtls_pk_context *key
@@ -310,15 +281,20 @@
         mbedtls_ssl_config *conf,
         int major,
         int minor)
     # mbedtls_ssl_conf_fallback
     # mbedtls_ssl_conf_encrypt_then_mac
     # mbedtls_ssl_conf_extended_master_secret
     # mbedtls_ssl_conf_arc4_support
-    # mbedtls_ssl_conf_max_frag_len
+
+    int mbedtls_ssl_conf_max_frag_len(
+        mbedtls_ssl_config *conf,
+        unsigned char mgl_code,
+    )
+
     # mbedtls_ssl_conf_truncated_hmac
     # mbedtls_ssl_conf_cbc_record_splitting
     # mbedtls_ssl_conf_session_tickets
     void mbedtls_ssl_conf_renegotiation(
         mbedtls_ssl_config *conf,
         int renegotiation)
     # mbedtls_ssl_conf_legacy_renegotiation
@@ -335,14 +311,19 @@
     void mbedtls_ssl_set_bio(
         mbedtls_ssl_context *ssl,
         void *p_bio,
         mbedtls_ssl_send_p f_send,
         mbedtls_ssl_recv_p f_recv,
         mbedtls_ssl_recv_timeout_p f_recv_timeout)
 
+    void mbedtls_ssl_set_mtu(
+        mbedtls_ssl_context *ssl,
+        uint16_t mtu,
+    )
+
     void mbedtls_ssl_set_timer_cb(
         # DTLS
         mbedtls_ssl_context *ssl,
         void *p_timer,
         mbedtls_ssl_set_timer_t f_set_timer,
         mbedtls_ssl_get_timer_t f_get_timer)
     int mbedtls_ssl_set_client_transport_id(
@@ -430,22 +411,24 @@
 cdef class MbedTLSConfiguration:
     cdef mbedtls_ssl_config _ctx
     cdef _chain
     cdef int *_ciphers
     cdef const char **_protos
     cdef _PSKSToreProxy _store
     cdef _DTLSCookie _cookie
+    cdef object _max_fragmentation_length
     # cdef'd because we aim at a non-writable structure.
     cdef _set_validate_certificates(self, validate)
     cdef _set_certificate_chain(self, chain)
     cdef _set_ciphers(self, ciphers)
     cdef _set_inner_protocols(self, protocols)
     cdef _set_lowest_supported_version(self, version)
     cdef _set_highest_supported_version(self, version)
     cdef _set_trust_store(self, object store)
+    cdef _set_max_fragmentation_length(self, object mfl)
     cdef _set_anti_replay(self, mode)
     cdef _set_handshake_timeout(self, minimum, maximum)
     cdef _set_cookie(self, _DTLSCookie cookie)
     cdef _set_sni_callback(self, callback)
     cdef _set_pre_shared_key(self, psk)
     cdef _set_pre_shared_key_store(self, psk_store)
 
@@ -466,8 +449,8 @@
 cdef class MbedTLSBuffer:
     cdef _BaseContext _context
     cdef mbedtls_ssl_context _ctx
     cdef _rb.RingBuffer _c_output_buffer
     cdef _rb.RingBuffer _c_input_buffer
     cdef _C_Buffers _c_buffers
     # DTLS only:
-    cdef mbedtls_timing_delay_context _timer
+    cdef _timing.mbedtls_timing_delay_context _timer
```

### Comparing `python-mbedtls-2.6.1/src/mbedtls/_tls.pyi` & `python-mbedtls-2.7.0/src/mbedtls/_tls.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     SERVER_FINISHED: int
     FLUSH_BUFFERS: int
     HANDSHAKE_WRAPUP: int
     HANDSHAKE_OVER: int
     SERVER_NEW_SESSION_TICKET: int
     SERVER_HELLO_VERIFY_REQUEST_SENT: int
 
+
 class TLSError(Exception): ...
 class WantWriteError(TLSError): ...
 class WantReadError(TLSError): ...
 class RaggedEOF(TLSError): ...
 class HelloVerifyRequest(TLSError): ...
 
 class TrustStore(abc.Sequence[Certificate]):
@@ -106,14 +107,15 @@
     def _output_buffer(self) -> bytes: ...
     @property
     def context(self) -> _BaseContext: ...
     @property
     def _server_hostname(self) -> str: ...
     def shutdown(self) -> None: ...
     def setcookieparam(self, info: bytes) -> None: ...
+    def setmtu(self, mtu: int) -> None: ...
     def read(self, amt: int) -> bytes: ...
     def readinto(self, buffer: bytes, amt: int) -> int: ...
     def write(self, buffer: bytes) -> int: ...
     def receive_from_network(self, data: bytes) -> None: ...
     def peek_outgoing(self, amt: int) -> bytes: ...
     def consume_outgoing(self, amt: int) -> None: ...
     @overload
```

### Comparing `python-mbedtls-2.6.1/src/mbedtls/_tls.pyx` & `python-mbedtls-2.7.0/src/mbedtls/_tls.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2018, Mathias Laurin
 
 cimport libc.stdio as c_stdio
 from libc.stdlib cimport free, malloc
 
+cimport mbedtls._debug as _debug
 cimport mbedtls._random as _rnd
+cimport mbedtls._timing as _timing
 cimport mbedtls._tls as _tls
 cimport mbedtls.pk as _pk
 cimport mbedtls.x509 as _x509
 
 import enum
 from collections import abc
 from functools import partial
@@ -21,14 +23,15 @@
 import mbedtls._random as _rnd
 import mbedtls._ringbuf as _rb
 import mbedtls.exceptions as _exc
 import mbedtls.pk as _pk
 from mbedtls._tlsi import (
     DTLSConfiguration,
     DTLSVersion,
+    MaxFragmentLength,
     NextProtocol,
     TLSConfiguration,
     TLSVersion,
 )
 
 
 cdef _rnd.Random __rng = _rnd.default_rng()
@@ -66,53 +69,53 @@
 
 # Python 2.7: `register()` can be used as a decorator from 3.3.
 abc.Mapping.register(_PSKSToreProxy)
 
 
 @cython.boundscheck(False)
 cdef void _my_debug(void *ctx, int level,
-                    const char *file, int line, const char *str) nogil:
+                    const char *file, int line, const char *str) noexcept nogil:
     c_stdio.fprintf(<c_stdio.FILE *> ctx, "%s:%04d: %s", file, line, str)
     c_stdio.fflush(<c_stdio.FILE *> ctx)
 
 
 def _enable_debug_output(_BaseContext context):
     _tls.mbedtls_ssl_conf_dbg(&context._conf._ctx, _my_debug, c_stdio.stdout)
 
 
 @cython.boundscheck(False)
-cdef int buffer_write(void *ctx, const unsigned char *buf, size_t len) nogil:
+cdef int buffer_write(void *ctx, const unsigned char *buf, size_t len) noexcept nogil:
     """"Write buffer to output buffer."""
     c_buf = <_tls._C_Buffers *> ctx
     if len == 0:
         return _tls.MBEDTLS_ERR_SSL_BAD_INPUT_DATA
     if _rb.c_len(c_buf.out_ctx) == _rb.c_capacity(c_buf.out_ctx):
         return _tls.MBEDTLS_ERR_SSL_WANT_READ
     cdef size_t writelen = min(
         len, _rb.c_capacity(c_buf.out_ctx) - _rb.c_len(c_buf.out_ctx)
     )
     return _rb.c_write(c_buf.out_ctx, buf, writelen)
 
 
 @cython.boundscheck(False)
-cdef int buffer_read(void *ctx, unsigned char *buf, const size_t len) nogil:
+cdef int buffer_read(void *ctx, unsigned char *buf, const size_t len) noexcept nogil:
     """Read from input buffer."""
     c_buf = <_tls._C_Buffers *> ctx
     if _rb.c_len(c_buf.in_ctx) == 0:
         return _tls.MBEDTLS_ERR_SSL_WANT_READ
     return _rb.c_readinto(c_buf.in_ctx, buf, len)
 
 
 @cython.boundscheck(False)
 cdef int _psk_cb(
     void *parameter,
     _tls.mbedtls_ssl_context *ctx,
     const unsigned char *c_identity,
     size_t c_identity_len
-) nogil:
+) noexcept nogil:
     """Wrapper for the PSK callback."""
     # If a valid PSK identity is found, call `mbedtls_ssl_set_hs_psk()` and
     # return 0. Otherwise, return 1.
     with gil:
         store = <_tls._PSKSToreProxy> parameter
         identity = c_identity[:c_identity_len]
         try:
@@ -121,15 +124,15 @@
             return 0
         except Exception:
             return 1
 
 
 def _set_debug_level(int level):
     """Set debug level for logging."""
-    _tls.mbedtls_debug_set_threshold(level)
+    _debug.mbedtls_debug_set_threshold(level)
 
 
 def __get_ciphersuite_name(ciphersuite_id):
     """Return a string containing the ciphersuite name.
 
     Args:
         ciphersuite_id: The ID of the ciphersuite.
@@ -387,36 +390,39 @@
         validate_certificates,
         certificate_chain,
         ciphers,
         inner_protocols,
         lowest_supported_version,
         highest_supported_version,
         trust_store,
+        max_fragmentation_length,
         anti_replay,
         # badmac_limit
         handshake_timeout_min,
         handshake_timeout_max,
         sni_callback,
         pre_shared_key,
         pre_shared_key_store,
         _transport,
     ):
         assert isinstance(_transport, Transport)
+        self._max_fragmentation_length = max_fragmentation_length
         _exc.check_error(_tls.mbedtls_ssl_config_defaults(
             &self._ctx,
             endpoint=0,  # server / client is not known here...
             transport=_transport.value,
             preset=_tls.MBEDTLS_SSL_PRESET_DEFAULT))
         self._set_validate_certificates(validate_certificates)
         self._set_certificate_chain(certificate_chain)
         self._set_ciphers(ciphers)
         self._set_inner_protocols(inner_protocols)
         self._set_lowest_supported_version(lowest_supported_version)
         self._set_highest_supported_version(highest_supported_version)
         self._set_trust_store(trust_store)
+        self._set_max_fragmentation_length(max_fragmentation_length)
         self._set_anti_replay(anti_replay)
         self._set_handshake_timeout(
             handshake_timeout_min, handshake_timeout_max
         )
         self._set_sni_callback(sni_callback)
         self._set_pre_shared_key(pre_shared_key)
         self._set_pre_shared_key_store(pre_shared_key_store)
@@ -465,14 +471,15 @@
                 self.validate_certificates,
                 self.certificate_chain,
                 self.ciphers,
                 self.inner_protocols,
                 self.lowest_supported_version,
                 self.highest_supported_version,
                 self.trust_store,
+                self.max_fragmentation_length,
                 self.anti_replay,
                 self.handshake_timeout_min,
                 self.handshake_timeout_max,
                 self.sni_callback,
                 self.pre_shared_key,
                 self.pre_shared_key_store,
                 self._transport,
@@ -708,14 +715,33 @@
 
         cdef _x509.mbedtls_x509_crt *c_ctx = self._ctx.ca_chain
         while c_ctx is not NULL:
             store.add(_x509.CRT.from_DER(c_ctx.raw.p[0:c_ctx.raw.len]))
             c_ctx = c_ctx.next
         return store
 
+    cdef _set_max_fragmentation_length(self, mfl):
+        if mfl is None:
+            return
+
+        if not isinstance(mfl, MaxFragmentLength):
+            raise TypeError(mfl)
+
+        try:
+            _exc.check_error(
+                _tls.mbedtls_ssl_conf_max_frag_len(&self._ctx, mfl.value)
+            )
+        except _exc.TLSError as exc:
+            raise ValueError(mfl) from exc
+
+    @property
+    def max_fragmentation_length(self):
+        # No accessor in backend.
+        return self._max_fragmentation_length
+
     cdef _set_anti_replay(self, anti_replay):
         """Set anti replay."""
         if anti_replay is None:
             return
         if self._transport is Transport.STREAM:
             # not available with TLS
             raise ValueError(anti_replay)
@@ -882,14 +908,15 @@
                 lowest_supported_version=(
                     configuration.lowest_supported_version
                 ),
                 highest_supported_version=(
                     configuration.highest_supported_version
                 ),
                 trust_store=configuration.trust_store,
+                max_fragmentation_length=configuration.max_fragmentation_length,
                 anti_replay=None,
                 handshake_timeout_min=None,
                 handshake_timeout_max=None,
                 sni_callback=configuration.sni_callback,
                 pre_shared_key=configuration.pre_shared_key,
                 pre_shared_key_store=configuration.pre_shared_key_store,
                 _transport=Transport.STREAM,
@@ -903,14 +930,15 @@
                 lowest_supported_version=(
                     configuration.lowest_supported_version
                 ),
                 highest_supported_version=(
                     configuration.highest_supported_version
                 ),
                 trust_store=configuration.trust_store,
+                max_fragmentation_length=configuration.max_fragmentation_length,
                 anti_replay=configuration.anti_replay,
                 handshake_timeout_min=configuration.handshake_timeout_min,
                 handshake_timeout_max=configuration.handshake_timeout_max,
                 sni_callback=configuration.sni_callback,
                 pre_shared_key=configuration.pre_shared_key,
                 pre_shared_key_store=configuration.pre_shared_key_store,
                 _transport=Transport.DATAGRAM,
@@ -941,27 +969,29 @@
                 validate_certificates=self._conf.validate_certificates,
                 certificate_chain=self._conf.certificate_chain,
                 ciphers=self._conf.ciphers,
                 inner_protocols=self._conf.inner_protocols,
                 lowest_supported_version=self._conf.lowest_supported_version,
                 highest_supported_version=self._conf.highest_supported_version,
                 trust_store=self._conf.trust_store,
+                max_fragmentation_length=self._conf.max_fragmentation_length,
                 sni_callback=self._conf.sni_callback,
                 pre_shared_key=self._conf.pre_shared_key,
                 pre_shared_key_store=self._conf.pre_shared_key_store,
             )
         assert self._conf._transport is Transport.DATAGRAM
         return DTLSConfiguration(
             validate_certificates=self._conf.validate_certificates,
             certificate_chain=self._conf.certificate_chain,
             ciphers=self._conf.ciphers,
             inner_protocols=self._conf.inner_protocols,
             lowest_supported_version=self._conf.lowest_supported_version,
             highest_supported_version=self._conf.highest_supported_version,
             trust_store=self._conf.trust_store,
+            max_fragmentation_length=self._conf.max_fragmentation_length,
             anti_replay=self._conf.anti_replay,
             handshake_timeout_min=self._conf.handshake_timeout_min,
             handshake_timeout_max=self._conf.handshake_timeout_max,
             sni_callback=self._conf.sni_callback,
             pre_shared_key=self._conf.pre_shared_key,
             pre_shared_key_store=self._conf.pre_shared_key_store,
         )
@@ -999,16 +1029,16 @@
 
     def __cinit__(self):
         """Initialize an `ssl_context`."""
         _tls.mbedtls_ssl_init(&self._ctx)
         _tls.mbedtls_ssl_set_timer_cb(
             &self._ctx,
             &self._timer,
-            _tls.mbedtls_timing_set_delay,
-            _tls.mbedtls_timing_get_delay)
+            _timing.mbedtls_timing_set_delay,
+            _timing.mbedtls_timing_get_delay)
 
     def __dealloc__(self):
         """Free and clear the internal structures of ctx."""
         _tls.mbedtls_ssl_free(&self._ctx)
 
     def __getstate__(self):
         cdef size_t olen = 0
@@ -1096,14 +1126,28 @@
             info = b"\0"
         _tls.mbedtls_ssl_set_client_transport_id(
             &self._ctx,
             &info[0],
             info.size,
         )
 
+    def setmtu(self, mtu):
+        """Set Maxiumum Transport Unit (MTU) for DTLS.
+
+        Set to zero to unset.
+
+        Raises:
+            OverflowError: If value cannot be converted to UInt16.
+
+        """
+        # DTLS
+        if not isinstance(mtu, int):
+            raise TypeError(mtu)
+        _tls.mbedtls_ssl_set_mtu(&self._ctx, mtu)
+
     def _reset(self):
         _exc.check_error(_tls.mbedtls_ssl_session_reset(&self._ctx))
 
     def shutdown(self):
         # No error handling:  The connection may be closed already.
         _tls.mbedtls_ssl_close_notify(&self._ctx)
         self._reset()
```

### Comparing `python-mbedtls-2.6.1/src/mbedtls/_tlsi.py` & `python-mbedtls-2.7.0/src/mbedtls/_tlsi.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,22 @@
     WEBRTC: bytes = b"webrtc"
     C_WEBRTC: bytes = b"c-webrtc"
     FTP: bytes = b"ftp"
     STUN: bytes = b"stun.nat-discovery"
     TURN: bytes = b"stun.turn"
 
 
+class MaxFragmentLength(enum.Enum):
+    NONE = 0
+    MFL_512K = 1
+    MFL_1024K = 2
+    MFL_2048K = 3
+    MFL_4096K = 4
+
+
 class TLSVersion(enum.Enum):
     # PEP 543
     MINIMUM_SUPPORTED = enum.auto()
     SSLv2 = enum.auto()
     SSLv3 = enum.auto()
     TLSv1 = enum.auto()
     TLSv1_1 = enum.auto()
@@ -178,14 +186,15 @@
     validate_certificates: bool = True
     certificate_chain: Optional[_CertificateChain] = None
     ciphers: Optional[_Ciphers] = None
     inner_protocols: Optional[_InnerProtocols] = None
     lowest_supported_version: TLSVersion = TLSVersion.TLSv1
     highest_supported_version: TLSVersion = TLSVersion.MAXIMUM_SUPPORTED
     trust_store: Optional[TrustStore] = None
+    max_fragmentation_length: Optional[MaxFragmentLength] = None
     sni_callback: Optional[ServerNameCallback] = None
     pre_shared_key: Optional[Tuple[str, bytes]] = None
     pre_shared_key_store: Mapping[str, bytes] = field(default_factory=dict)
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, TLSConfiguration):
             return NotImplemented
@@ -229,14 +238,16 @@
                     in {
                         TLSVersion.MINIMUM_SUPPORTED,
                         TLSVersion.MAXIMUM_SUPPORTED,
                     }
                 ),
                 self.trust_store == other.trust_store
                 or (not self.trust_store and not other.trust_store),
+                self.max_fragmentation_length
+                == other.max_fragmentation_length,
                 self.sni_callback == other.sni_callback,
                 self.pre_shared_key == other.pre_shared_key,
                 self.pre_shared_key_store == other.pre_shared_key_store,
             )
         )
 
     def update(
@@ -244,46 +255,67 @@
         validate_certificates: _Wrap[bool] = _DEFAULT_VALUE,
         certificate_chain: _Wrap[_CertificateChain] = _DEFAULT_VALUE,
         ciphers: _Wrap[_Ciphers] = _DEFAULT_VALUE,
         inner_protocols: _Wrap[_InnerProtocols] = _DEFAULT_VALUE,
         lowest_supported_version: _Wrap[TLSVersion] = _DEFAULT_VALUE,
         highest_supported_version: _Wrap[TLSVersion] = _DEFAULT_VALUE,
         trust_store: _Wrap[TrustStore] = _DEFAULT_VALUE,
+        max_fragmentation_length: _Wrap[MaxFragmentLength] = _DEFAULT_VALUE,
         sni_callback: _Wrap[Optional[ServerNameCallback]] = _DEFAULT_VALUE,
         pre_shared_key: _Wrap[Tuple[str, bytes]] = _DEFAULT_VALUE,
         pre_shared_key_store: _Wrap[Mapping[str, bytes]] = _DEFAULT_VALUE,
     ) -> TLSConfiguration:
         """
         Create a new ``TLSConfiguration``, overriding some of the settings
         on the original configuration with the new settings.
         """
         return self.__class__(
-            _unwrap(validate_certificates, self.validate_certificates),
-            _unwrap(certificate_chain, self.certificate_chain),
-            _unwrap(ciphers, self.ciphers),
-            _unwrap(inner_protocols, self.inner_protocols),
-            _unwrap(lowest_supported_version, self.lowest_supported_version),
-            _unwrap(highest_supported_version, self.highest_supported_version),
-            _unwrap(trust_store, self.trust_store),
-            _unwrap(sni_callback, self.sni_callback),
-            _unwrap(pre_shared_key, self.pre_shared_key),
-            _unwrap(pre_shared_key_store, self.pre_shared_key_store),
+            validate_certificates=_unwrap(
+                validate_certificates,
+                self.validate_certificates,
+            ),
+            certificate_chain=_unwrap(
+                certificate_chain,
+                self.certificate_chain,
+            ),
+            ciphers=_unwrap(ciphers, self.ciphers),
+            inner_protocols=_unwrap(inner_protocols, self.inner_protocols),
+            lowest_supported_version=_unwrap(
+                lowest_supported_version,
+                self.lowest_supported_version,
+            ),
+            highest_supported_version=_unwrap(
+                highest_supported_version,
+                self.highest_supported_version,
+            ),
+            trust_store=_unwrap(trust_store, self.trust_store),
+            max_fragmentation_length=_unwrap(
+                max_fragmentation_length,
+                self.max_fragmentation_length,
+            ),
+            sni_callback=_unwrap(sni_callback, self.sni_callback),
+            pre_shared_key=_unwrap(pre_shared_key, self.pre_shared_key),
+            pre_shared_key_store=_unwrap(
+                pre_shared_key_store,
+                self.pre_shared_key_store,
+            ),
         )
 
 
 @dataclass(frozen=True)
 class DTLSConfiguration:
     # pylint: disable=too-many-instance-attributes, too-many-arguments
     validate_certificates: bool = True
     certificate_chain: Optional[_CertificateChain] = None
     ciphers: Optional[_Ciphers] = None
     inner_protocols: Optional[_InnerProtocols] = None
     lowest_supported_version: DTLSVersion = DTLSVersion.DTLSv1_0
     highest_supported_version: DTLSVersion = DTLSVersion.MAXIMUM_SUPPORTED
     trust_store: Optional[TrustStore] = None
+    max_fragmentation_length: Optional[MaxFragmentLength] = None
     anti_replay: bool = True
     handshake_timeout_min: float = 1.0
     handshake_timeout_max: float = 60.0
     sni_callback: Optional[ServerNameCallback] = None
     pre_shared_key: Optional[Tuple[str, bytes]] = None
     pre_shared_key_store: Mapping[str, bytes] = field(default_factory=dict)
 
@@ -331,14 +363,16 @@
                         DTLSVersion.MINIMUM_SUPPORTED,
                         DTLSVersion.MAXIMUM_SUPPORTED,
                     }
                 ),
                 self.trust_store == other.trust_store
                 or (not self.trust_store and not other.trust_store)
                 or (not self.trust_store and not other.trust_store),
+                self.max_fragmentation_length
+                == other.max_fragmentation_length,
                 self.anti_replay == other.anti_replay,
                 self.handshake_timeout_min == other.handshake_timeout_min,
                 self.handshake_timeout_max == other.handshake_timeout_max,
                 self.sni_callback == other.sni_callback,
                 self.pre_shared_key == other.pre_shared_key,
                 self.pre_shared_key_store == other.pre_shared_key_store,
             )
@@ -349,33 +383,59 @@
         validate_certificates: _Wrap[bool] = _DEFAULT_VALUE,
         certificate_chain: _Wrap[_CertificateChain] = _DEFAULT_VALUE,
         ciphers: _Wrap[_Ciphers] = _DEFAULT_VALUE,
         inner_protocols: _Wrap[_InnerProtocols] = _DEFAULT_VALUE,
         lowest_supported_version: _Wrap[DTLSVersion] = _DEFAULT_VALUE,
         highest_supported_version: _Wrap[DTLSVersion] = _DEFAULT_VALUE,
         trust_store: _Wrap[TrustStore] = _DEFAULT_VALUE,
+        max_fragmentation_length: _Wrap[MaxFragmentLength] = _DEFAULT_VALUE,
         anti_replay: _Wrap[bool] = _DEFAULT_VALUE,
         handshake_timeout_min: _Wrap[float] = _DEFAULT_VALUE,
         handshake_timeout_max: _Wrap[float] = _DEFAULT_VALUE,
         sni_callback: _Wrap[ServerNameCallback] = _DEFAULT_VALUE,
         pre_shared_key: _Wrap[Tuple[str, bytes]] = _DEFAULT_VALUE,
         pre_shared_key_store: _Wrap[Mapping[str, bytes]] = _DEFAULT_VALUE,
     ) -> DTLSConfiguration:
         """
         Create a new ``TLSConfiguration``, overriding some of the settings
         on the original configuration with the new settings.
         """
         return self.__class__(
-            _unwrap(validate_certificates, self.validate_certificates),
-            _unwrap(certificate_chain, self.certificate_chain),
-            _unwrap(ciphers, self.ciphers),
-            _unwrap(inner_protocols, self.inner_protocols),
-            _unwrap(lowest_supported_version, self.lowest_supported_version),
-            _unwrap(highest_supported_version, self.highest_supported_version),
-            _unwrap(trust_store, self.trust_store),
-            _unwrap(anti_replay, self.anti_replay),
-            _unwrap(handshake_timeout_min, self.handshake_timeout_min),
-            _unwrap(handshake_timeout_max, self.handshake_timeout_max),
-            _unwrap(sni_callback, self.sni_callback),
-            _unwrap(pre_shared_key, self.pre_shared_key),
-            _unwrap(pre_shared_key_store, self.pre_shared_key_store),
+            validate_certificates=_unwrap(
+                validate_certificates,
+                self.validate_certificates,
+            ),
+            certificate_chain=_unwrap(
+                certificate_chain,
+                self.certificate_chain,
+            ),
+            ciphers=_unwrap(ciphers, self.ciphers),
+            inner_protocols=_unwrap(inner_protocols, self.inner_protocols),
+            lowest_supported_version=_unwrap(
+                lowest_supported_version,
+                self.lowest_supported_version,
+            ),
+            highest_supported_version=_unwrap(
+                highest_supported_version,
+                self.highest_supported_version,
+            ),
+            trust_store=_unwrap(trust_store, self.trust_store),
+            max_fragmentation_length=_unwrap(
+                max_fragmentation_length,
+                self.max_fragmentation_length,
+            ),
+            anti_replay=_unwrap(anti_replay, self.anti_replay),
+            handshake_timeout_min=_unwrap(
+                handshake_timeout_min,
+                self.handshake_timeout_min,
+            ),
+            handshake_timeout_max=_unwrap(
+                handshake_timeout_max,
+                self.handshake_timeout_max,
+            ),
+            sni_callback=_unwrap(sni_callback, self.sni_callback),
+            pre_shared_key=_unwrap(pre_shared_key, self.pre_shared_key),
+            pre_shared_key_store=_unwrap(
+                pre_shared_key_store,
+                self.pre_shared_key_store,
+            ),
         )
```

### Comparing `python-mbedtls-2.6.1/src/mbedtls/cipher/AES.py` & `python-mbedtls-2.7.0/src/mbedtls/cipher/AES.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/cipher/ARC4.py` & `python-mbedtls-2.7.0/src/mbedtls/cipher/ARC4.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/cipher/ARIA.py` & `python-mbedtls-2.7.0/src/mbedtls/cipher/ARIA.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/cipher/Blowfish.py` & `python-mbedtls-2.7.0/src/mbedtls/cipher/Blowfish.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/cipher/CHACHA20.py` & `python-mbedtls-2.7.0/src/mbedtls/cipher/CHACHA20.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/cipher/Camellia.py` & `python-mbedtls-2.7.0/src/mbedtls/cipher/Camellia.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/cipher/DES.py` & `python-mbedtls-2.7.0/src/mbedtls/cipher/DES.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/cipher/DES3.py` & `python-mbedtls-2.7.0/src/mbedtls/cipher/DES3.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/cipher/DES3dbl.py` & `python-mbedtls-2.7.0/src/mbedtls/cipher/DES3dbl.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/cipher/__init__.py` & `python-mbedtls-2.7.0/src/mbedtls/cipher/__init__.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/cipher/_cipher.pxd` & `python-mbedtls-2.7.0/src/mbedtls/cipher/_cipher.pxd`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/cipher/_cipher.pyi` & `python-mbedtls-2.7.0/src/mbedtls/cipher/_cipher.pyi`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/cipher/_cipher.pyx` & `python-mbedtls-2.7.0/src/mbedtls/cipher/_cipher.pyx`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/exceptions.pyx` & `python-mbedtls-2.7.0/src/mbedtls/exceptions.pyx`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/hashlib.py` & `python-mbedtls-2.7.0/src/mbedtls/hashlib.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/hkdf.pxd` & `python-mbedtls-2.7.0/src/mbedtls/hkdf.pxd`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2019, Mathias Laurin
 
-"""Declarations from `mbedtls/hkdf.h`."""
-
-
 cimport mbedtls._md as _md
 
 
 cdef extern from "mbedtls/hkdf.h" nogil:
     int mbedtls_hkdf(
         const _md.mbedtls_md_info_t *md,
         const unsigned char *salt, size_t salt_len,
```

### Comparing `python-mbedtls-2.6.1/src/mbedtls/hkdf.pyi` & `python-mbedtls-2.7.0/src/mbedtls/hkdf.pyi`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/hkdf.pyx` & `python-mbedtls-2.7.0/src/mbedtls/hkdf.pyx`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/hmac.py` & `python-mbedtls-2.7.0/src/mbedtls/hmac.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/mpi.pxd` & `python-mbedtls-2.7.0/src/mbedtls/mpi.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2018, Mathias Laurin
 
-"""Declaration from `mbedtls/bignum.h`."""
-
-
 cdef extern from "mbedtls/bignum.h" nogil:
     int MBEDTLS_MPI_MAX_SIZE
 
     # Multi-precision integer library
     # -------------------------------
     ctypedef struct mbedtls_mpi:
         pass
```

### Comparing `python-mbedtls-2.6.1/src/mbedtls/mpi.pyi` & `python-mbedtls-2.7.0/src/mbedtls/mpi.pyi`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/mpi.pyx` & `python-mbedtls-2.7.0/src/mbedtls/mpi.pyx`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/pk.pyi` & `python-mbedtls-2.7.0/src/mbedtls/pk.pyi`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/pk.pyx` & `python-mbedtls-2.7.0/src/mbedtls/pk.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 
 """
 
 
 from libc.stdlib cimport free, malloc
 from libc.string cimport memset
 
+cimport mbedtls._dhm as _dhm
+cimport mbedtls._ecdh as _ecdh
+cimport mbedtls._ecp as _ecp
 cimport mbedtls._random as _rnd
+cimport mbedtls._rsa as _rsa
 cimport mbedtls.mpi as _mpi
 cimport mbedtls.pk as _pk
 
 import enum
 import re
 from collections import namedtuple
 from functools import partial
@@ -82,16 +86,16 @@
 
 
 # The following calculations come from mbedtls/library/pkwrite.c.
 RSA_PUB_DER_MAX_BYTES = 38 + 2 * _mpi.MBEDTLS_MPI_MAX_SIZE
 MPI_MAX_SIZE_2 = _mpi.MBEDTLS_MPI_MAX_SIZE // 2 + _mpi.MBEDTLS_MPI_MAX_SIZE % 2
 RSA_PRV_DER_MAX_BYTES = 47 + 3 * _mpi.MBEDTLS_MPI_MAX_SIZE + 5 * MPI_MAX_SIZE_2
 
-ECP_PUB_DER_MAX_BYTES = 30 + 2 * _pk.MBEDTLS_ECP_MAX_BYTES
-ECP_PRV_DER_MAX_BYTES = 29 + 3 * _pk.MBEDTLS_ECP_MAX_BYTES
+ECP_PUB_DER_MAX_BYTES = 30 + 2 * _ecp.MBEDTLS_ECP_MAX_BYTES
+ECP_PRV_DER_MAX_BYTES = 29 + 3 * _ecp.MBEDTLS_ECP_MAX_BYTES
 
 PUB_DER_MAX_BYTES = max(RSA_PUB_DER_MAX_BYTES, ECP_PUB_DER_MAX_BYTES)
 PRV_DER_MAX_BYTES = max(RSA_PRV_DER_MAX_BYTES, ECP_PRV_DER_MAX_BYTES)
 
 del RSA_PUB_DER_MAX_BYTES, MPI_MAX_SIZE_2, RSA_PRV_DER_MAX_BYTES
 del ECP_PUB_DER_MAX_BYTES, ECP_PRV_DER_MAX_BYTES
 
@@ -107,24 +111,24 @@
 
 cpdef get_supported_ciphers():
     return CIPHER_NAME
 
 
 def get_supported_curves():
     """Return the list of supported curves in order of preference."""
-    cdef const mbedtls_ecp_curve_info* info = _pk.mbedtls_ecp_curve_list()
+    cdef const _ecp.mbedtls_ecp_curve_info* info = _ecp.mbedtls_ecp_curve_list()
     names, idx = [], 0
     while info[idx].name != NULL:
         names.append(Curve(bytes(info[idx].name)))
         idx += 1
     return names
 
 
 cdef curve_name_to_grp_id(curve):
-    cdef const mbedtls_ecp_curve_info* info = _pk.mbedtls_ecp_curve_list()
+    cdef const _ecp.mbedtls_ecp_curve_info* info = _ecp.mbedtls_ecp_curve_list()
     idx = 0
     while info[idx].name != NULL:
         if info[idx].name == curve:
             return info[idx].grp_id
         idx += 1
     raise LookupError(curve.decode("ascii") + " not found")
 
@@ -545,34 +549,34 @@
     def __init__(self,
                  const unsigned char[:] key=None,
                  const unsigned char[:] password=None):
         super().__init__(b"RSA", key, password)
 
     def _has_private(self):
         """Return `True` if the key contains a valid private half."""
-        return _pk.mbedtls_rsa_check_privkey(
+        return _rsa.mbedtls_rsa_check_privkey(
             _pk.mbedtls_pk_rsa(self._ctx)
         ) == 0
 
     def _has_public(self):
         """Return `True` if the key contains a valid public half."""
-        return _pk.mbedtls_rsa_check_pubkey(_pk.mbedtls_pk_rsa(self._ctx)) == 0
+        return _rsa.mbedtls_rsa_check_pubkey(_pk.mbedtls_pk_rsa(self._ctx)) == 0
 
     def generate(self, unsigned int key_size=2048, int exponent=65537):
         """Generate an RSA keypair.
 
         Arguments:
             key_size (unsigned int): size in bits.
             exponent (int): public RSA exponent.
 
         Return:
             (bytes): The private key in DER format.
 
         """
-        _exc.check_error(_pk.mbedtls_rsa_gen_key(
+        _exc.check_error(_rsa.mbedtls_rsa_gen_key(
             _pk.mbedtls_pk_rsa(self._ctx), &_rnd.mbedtls_ctr_drbg_random,
             &__rng._ctx, key_size, exponent))
         return self.export_key("DER")
 
 
 cdef class ECPoint:
 
@@ -583,19 +587,19 @@
         cdef _mpi.MPI _z = _mpi.MPI(z)
         _mpi.mbedtls_mpi_copy(&self._ctx.X, &_x._ctx)
         _mpi.mbedtls_mpi_copy(&self._ctx.Y, &_y._ctx)
         _mpi.mbedtls_mpi_copy(&self._ctx.Z, &_z._ctx)
 
     def __cinit__(self):
         """Initialize the context."""
-        _pk.mbedtls_ecp_point_init(&self._ctx)
+        _ecp.mbedtls_ecp_point_init(&self._ctx)
 
     def __dealloc__(self):
         """Free and clear the context."""
-        _pk.mbedtls_ecp_point_free(&self._ctx)
+        _ecp.mbedtls_ecp_point_free(&self._ctx)
 
     def __reduce__(self):
         return type(self), (self.x, self.y, self.z)
 
     @property
     def x(self):
         """Return the X coordinate."""
@@ -628,25 +632,25 @@
     def __repr__(self):
         return "%s(%r, %r, %r)" % (
             type(self).__name__, self.x, self.y, self.z
         )
 
     def __eq__(self, other):
         if other == 0:
-            return _pk.mbedtls_ecp_is_zero(&self._ctx) == 1
+            return _ecp.mbedtls_ecp_is_zero(&self._ctx) == 1
         elif type(other) is type(self):
             c_other = <ECPoint> other
-            return _pk.mbedtls_ecp_point_cmp(&self._ctx, &c_other._ctx) == 0
+            return _ecp.mbedtls_ecp_point_cmp(&self._ctx, &c_other._ctx) == 0
         return NotImplemented
 
     def __hash__(self):
         return hash((self.x, self.y, self.z))
 
     def __bool__(self):
-        return _pk.mbedtls_ecp_is_zero(&self._ctx) == 0
+        return _ecp.mbedtls_ecp_is_zero(&self._ctx) == 0
 
 
 cdef class ECC(CipherBase):
 
     """Elliptic-curve cryptosystems.
 
     Args:
@@ -667,21 +671,21 @@
 
     @property
     def curve(self):
         return self._curve
 
     def _has_private(self):
         """Return `True` if the key contains a valid private half."""
-        cdef const mbedtls_ecp_keypair* ecp = _pk.mbedtls_pk_ec(self._ctx)
+        cdef const _ecp.mbedtls_ecp_keypair* ecp = _pk.mbedtls_pk_ec(self._ctx)
         return _mpi.mbedtls_mpi_cmp_mpi(&ecp.d, &_mpi.MPI()._ctx) != 0
 
     def _has_public(self):
         """Return `True` if the key contains a valid public half."""
-        cdef mbedtls_ecp_keypair* ecp = _pk.mbedtls_pk_ec(self._ctx)
-        return not _pk.mbedtls_ecp_is_zero(&ecp.Q)
+        cdef _ecp.mbedtls_ecp_keypair* ecp = _pk.mbedtls_pk_ec(self._ctx)
+        return not _ecp.mbedtls_ecp_is_zero(&ecp.Q)
 
     def sign(self,
              const unsigned char[:] message not None,
              digestmod=None):
         if self._curve in (Curve.CURVE25519, Curve.CURVE448):
             raise ValueError("ECDSA does not support Curve25519 or Curve448.")
         return super().sign(message, digestmod)
@@ -692,15 +696,15 @@
         Return:
             (bytes): The private key in DER format.
 
         """
         grp_id = curve_name_to_grp_id(self.curve)
         if grp_id is None:
             raise ValueError(self.curve)
-        _exc.check_error(_pk.mbedtls_ecp_gen_key(
+        _exc.check_error(_ecp.mbedtls_ecp_gen_key(
             grp_id, _pk.mbedtls_pk_ec(self._ctx),
             &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
         format = (
             "NUM"
             if self.curve in (Curve.CURVE25519, Curve.CURVE448)
             else "DER"
         )
@@ -733,15 +737,15 @@
             raise ValueError(
                 "Curve25519 and Curve448 only support export as NUM"
             )
         return super().export_key(format)
 
     def _public_to_point(self):
         point = ECPoint(0, 0, 0)
-        _pk.mbedtls_ecp_copy(&point._ctx, &_pk.mbedtls_pk_ec(self._ctx).Q)
+        _ecp.mbedtls_ecp_copy(&point._ctx, &_pk.mbedtls_pk_ec(self._ctx).Q)
         return point
 
     def export_public_key(self, format="DER"):
         """Return the public key.
 
         If no key is present, return a falsy value.
 
@@ -775,19 +779,19 @@
         _exc.check_error(_mpi.mbedtls_mpi_copy(
             &self._ctx.P, &_mpi.MPI(modulus)._ctx))
         _exc.check_error(_mpi.mbedtls_mpi_copy(
             &self._ctx.G, &_mpi.MPI(generator)._ctx))
 
     def __cinit__(self):
         """Initialize the context."""
-        _pk.mbedtls_dhm_init(&self._ctx)
+        _dhm.mbedtls_dhm_init(&self._ctx)
 
     def __dealloc__(self):
         """Free and clear the context."""
-        _pk.mbedtls_dhm_free(&self._ctx)
+        _dhm.mbedtls_dhm_free(&self._ctx)
 
     def __getstate__(self):
         raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
 
     @property
     def key_size(self):
         """Return the size of the key, in bytes."""
@@ -825,15 +829,15 @@
         cdef _mpi.MPI mpi
         cdef unsigned char* output = <unsigned char*>malloc(
             _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
         cdef size_t olen = 0
         if not output:
             raise MemoryError()
         try:
-            _exc.check_error(mbedtls_dhm_calc_secret(
+            _exc.check_error(_dhm.mbedtls_dhm_calc_secret(
                 &self._ctx, &output[0], _mpi.MBEDTLS_MPI_MAX_SIZE, &olen,
                 &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
             mpi = _mpi.MPI()
             _mpi.mbedtls_mpi_read_binary(&mpi._ctx, &output[0], olen)
             return mpi
         finally:
             free(output)
@@ -852,27 +856,27 @@
         """
         cdef unsigned char* output = <unsigned char*>malloc(
             _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
         cdef size_t olen = 0
         if not output:
             raise MemoryError()
         try:
-            _exc.check_error(_pk.mbedtls_dhm_make_params(
+            _exc.check_error(_dhm.mbedtls_dhm_make_params(
                 &self._ctx, self.key_size, &output[0], &olen,
                 &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
             assert olen != 0
             return output[:olen]
         finally:
             free(output)
 
     def import_CKE(self, const unsigned char[:] buffer not None):
         """Read the ClientKeyExchange payload."""
         if buffer.size == 0:
             buffer = b"\0"
-        _exc.check_error(_pk.mbedtls_dhm_read_public(
+        _exc.check_error(_dhm.mbedtls_dhm_read_public(
             &self._ctx, &buffer[0], buffer.size))
 
 
 cdef class DHClient(DHBase):
 
     """The client side of the DH key exchange."""
 
@@ -885,15 +889,15 @@
         """
         cdef _mpi.MPI mpi
         cdef unsigned char* output = <unsigned char*>malloc(
             _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
         if not output:
             raise MemoryError()
         try:
-            _exc.check_error(_pk.mbedtls_dhm_make_public(
+            _exc.check_error(_dhm.mbedtls_dhm_make_public(
                 &self._ctx, self.key_size, &output[0], self.key_size,
                 &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
             mpi = _mpi.from_mpi_p(&self._ctx.GX)
             return mpi.to_bytes(
                 _mpi.mbedtls_mpi_size(&mpi._ctx), "big")
         finally:
             free(output)
@@ -902,15 +906,15 @@
         """Read the ServerKeyExchange payload."""
         if buffer.size == 0:
             raise ValueError("SKE is empty")
         # Const away cast is safe because the pointer is used as
         # a read-only index in `dhm_read_bignum()`.
         cdef unsigned char* first = <unsigned char*> &buffer[0]
         cdef const unsigned char* end = &buffer[-1] + 1
-        _exc.check_error(_pk.mbedtls_dhm_read_params(&self._ctx, &first, end))
+        _exc.check_error(_dhm.mbedtls_dhm_read_params(&self._ctx, &first, end))
 
 
 cdef class ECDHBase:
 
     """Base class to ECDH(E) key exchange: client and server.
 
     Args:
@@ -922,50 +926,50 @@
 
     """
     def __init__(self, curve=None):
         super().__init__()
         if curve is None:
             curve = get_supported_curves()[0]
         self.curve = Curve(curve)
-        _exc.check_error(mbedtls_ecp_group_load(
+        _exc.check_error(_ecp.mbedtls_ecp_group_load(
             &self._ctx.grp, curve_name_to_grp_id(self.curve)))
 
     def __cinit__(self):
         """Initialize the context."""
-        _pk.mbedtls_ecdh_init(&self._ctx)
+        _ecdh.mbedtls_ecdh_init(&self._ctx)
 
     def __dealloc__(self):
         """Free and clear the context."""
-        _pk.mbedtls_ecdh_free(&self._ctx)
+        _ecdh.mbedtls_ecdh_free(&self._ctx)
 
     def __getstate__(self):
         raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
 
     def _has_private(self):
         """Return `True` if the key contains a valid private half."""
         return _mpi.mbedtls_mpi_cmp_mpi(&self._ctx.d, &_mpi.MPI()._ctx) != 0
 
     def _has_public(self):
         """Return `True` if the key contains a valid public half."""
-        return not _pk.mbedtls_ecp_is_zero(&self._ctx.Q)
+        return not _ecp.mbedtls_ecp_is_zero(&self._ctx.Q)
 
     def _has_peers_public(self):
         """Return `True` if the peer's key is present."""
-        return not _pk.mbedtls_ecp_is_zero(&self._ctx.Qp)
+        return not _ecp.mbedtls_ecp_is_zero(&self._ctx.Qp)
 
     @property
     def public_key(self):
         """The public key (ECPoint)"""
         ecp = ECPoint(0, 0, 0)
-        _exc.check_error(_pk.mbedtls_ecp_copy(&ecp._ctx, &self._ctx.Q))
+        _exc.check_error(_ecp.mbedtls_ecp_copy(&ecp._ctx, &self._ctx.Q))
         return ecp
 
     @public_key.setter
     def public_key(self, ECPoint ecp):
-        _exc.check_error(_pk.mbedtls_ecp_copy(&self._ctx.Q, &ecp._ctx))
+        _exc.check_error(_ecp.mbedtls_ecp_copy(&self._ctx.Q, &ecp._ctx))
 
     @property
     def private_key(self):
         """The private key (int)"""
         return _mpi.from_mpi_p(&self._ctx.d)
 
     @private_key.setter
@@ -973,20 +977,20 @@
         cdef _mpi.MPI c_priv = _mpi.MPI(priv)
         _mpi.mbedtls_mpi_copy(&self._ctx.d, &c_priv._ctx)
 
     @property
     def peers_public_key(self):
         """Peer's public key (ECPoint)"""
         ecp = ECPoint(0, 0, 0)
-        _exc.check_error(_pk.mbedtls_ecp_copy(&ecp._ctx, &self._ctx.Qp))
+        _exc.check_error(_ecp.mbedtls_ecp_copy(&ecp._ctx, &self._ctx.Qp))
         return ecp
 
     @peers_public_key.setter
     def peers_public_key(self, ECPoint ecp):
-        _exc.check_error(_pk.mbedtls_ecp_copy(&self._ctx.Qp, &ecp._ctx))
+        _exc.check_error(_ecp.mbedtls_ecp_copy(&self._ctx.Qp, &ecp._ctx))
 
     @property
     def shared_secret(self):
         """The shared secret (int).
 
         The shared secret is 0 if the TLS handshake is not finished.
 
@@ -1001,111 +1005,111 @@
         cdef _mpi.MPI mpi = _mpi.MPI()
         cdef unsigned char* output = <unsigned char*>malloc(
             _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
         cdef size_t olen = 0
         if not output:
             raise MemoryError()
         try:
-            _exc.check_error(mbedtls_ecdh_calc_secret(
+            _exc.check_error(_ecdh.mbedtls_ecdh_calc_secret(
                 &self._ctx, &olen, &output[0], _mpi.MBEDTLS_MPI_MAX_SIZE,
                 &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
             assert olen != 0
-            curve_type = _pk.mbedtls_ecp_get_type(&self._ctx.grp)
-            if curve_type == _pk.MBEDTLS_ECP_TYPE_MONTGOMERY:
+            curve_type = _ecp.mbedtls_ecp_get_type(&self._ctx.grp)
+            if curve_type == _ecp.MBEDTLS_ECP_TYPE_MONTGOMERY:
                 _mpi.mbedtls_mpi_read_binary_le(&mpi._ctx, &output[0], olen)
             else:
                 _mpi.mbedtls_mpi_read_binary(&mpi._ctx, &output[0], olen)
             return mpi
         finally:
             free(output)
 
     def generate_public_key(self):
         """Generate public key from a private key."""
-        _exc.check_error(_pk.mbedtls_ecp_mul(
+        _exc.check_error(_ecp.mbedtls_ecp_mul(
             &self._ctx.grp, &self._ctx.Q, &self._ctx.d, &self._ctx.grp.G,
             &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
 
 
 cdef class ECDHServer(ECDHBase):
 
     """The server side of the ECDH key exchange."""
 
     def __init__(self, ecc: ECC):
         super().__init__(ecc.curve)
         if ecc.export_key():
-            _exc.check_error(_pk.mbedtls_ecdh_get_params(
-                &self._ctx, _pk.mbedtls_pk_ec(ecc._ctx), MBEDTLS_ECDH_OURS))
+            _exc.check_error(_ecdh.mbedtls_ecdh_get_params(
+                &self._ctx, _pk.mbedtls_pk_ec(ecc._ctx), _ecdh.MBEDTLS_ECDH_OURS))
 
     def generate(self):
         """Generate a public key.
 
         Return:
             bytes: A TLS ServerKeyExchange payload.
 
         """
         cdef unsigned char* output = <unsigned char*>malloc(
             _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
         cdef size_t olen = 0
         if not output:
             raise MemoryError()
         try:
-            _exc.check_error(_pk.mbedtls_ecdh_make_params(
+            _exc.check_error(_ecdh.mbedtls_ecdh_make_params(
                 &self._ctx, &olen, &output[0], _mpi.MBEDTLS_MPI_MAX_SIZE,
                 &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
             assert olen != 0
             return output[:olen]
         finally:
             free(output)
 
     def import_CKE(self, const unsigned char[:] buffer not None):
         """Read the ClientKeyExchange payload."""
         if buffer.size == 0:
             buffer = b"\0"
-        _exc.check_error(_pk.mbedtls_ecdh_read_public(
+        _exc.check_error(_ecdh.mbedtls_ecdh_read_public(
             &self._ctx, &buffer[0], buffer.size))
 
 
 cdef class ECDHClient(ECDHBase):
 
     """The client side of the ephemeral ECDH key exchange."""
 
     def __init__(self, ecc: ECC):
         super().__init__(ecc.curve)
         if ecc.export_key():
-            _exc.check_error(_pk.mbedtls_ecdh_get_params(
-                &self._ctx, _pk.mbedtls_pk_ec(ecc._ctx), MBEDTLS_ECDH_THEIRS))
+            _exc.check_error(_ecdh.mbedtls_ecdh_get_params(
+                &self._ctx, _pk.mbedtls_pk_ec(ecc._ctx), _ecdh.MBEDTLS_ECDH_THEIRS))
 
     def generate(self):
         """Generate a public key.
 
         Return:
             bytes: A TLS ClientKeyExchange payload.
 
         """
         cdef unsigned char* output = <unsigned char*>malloc(
             _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
         cdef size_t olen = 0
         if not output:
             raise MemoryError()
         try:
-            _exc.check_error(_pk.mbedtls_ecdh_make_public(
+            _exc.check_error(_ecdh.mbedtls_ecdh_make_public(
                 &self._ctx, &olen, &output[0], _mpi.MBEDTLS_MPI_MAX_SIZE,
                 &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
             assert olen != 0
             return output[:olen]
         finally:
             free(output)
 
     def import_SKE(self, const unsigned char[:] buffer not None):
         """Read the ServerKeyExchange payload."""
         if buffer.size == 0:
             buffer = b"\0"
         cdef const unsigned char* first = &buffer[0]
         cdef const unsigned char* end = &buffer[-1] + 1
-        _exc.check_error(_pk.mbedtls_ecdh_read_params(
+        _exc.check_error(_ecdh.mbedtls_ecdh_read_params(
             &self._ctx, &first, end))
 
 
 cdef class ECDHNaive(ECDHBase):
 
     """Naive ECDH key exchange."""
 
@@ -1120,25 +1124,25 @@
     def generate(self):
         """Generate a public key.
 
         Return:
             ECPoint: public key.
 
         """
-        _exc.check_error(_pk.mbedtls_ecdh_gen_public(
+        _exc.check_error(_ecdh.mbedtls_ecdh_gen_public(
             &self._ctx.grp, &self._ctx.d, &self._ctx.Q,
             &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
         return self.public_key
 
     def import_peer_public(self, pubkey):
         self.import_peers_public(pubkey.x)
 
     def import_peers_public(self, _pk.ECPoint pubkey):
         """Read peer public key."""
-        _exc.check_error(_pk.mbedtls_ecp_copy(&self._ctx.Qp, &pubkey._ctx))
+        _exc.check_error(_ecp.mbedtls_ecp_copy(&self._ctx.Qp, &pubkey._ctx))
 
     def generate_secret(self):
         """Generate the shared secret."""
-        _exc.check_error(_pk.mbedtls_ecdh_compute_shared(
+        _exc.check_error(_ecdh.mbedtls_ecdh_compute_shared(
             &self._ctx.grp, &self._ctx.z, &self._ctx.Qp, &self._ctx.d,
             &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
         return _mpi.from_mpi_p(&self._ctx.z)
```

### Comparing `python-mbedtls-2.6.1/src/mbedtls/secrets.py` & `python-mbedtls-2.7.0/src/mbedtls/secrets.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/tls.py` & `python-mbedtls-2.7.0/src/mbedtls/tls.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     _BaseContext,
     _tls_from_version,
     _tls_to_version,
     ciphers_available,
 )
 from ._tlsi import DTLSConfiguration as DTLSConfiguration
 from ._tlsi import DTLSVersion as DTLSVersion
+from ._tlsi import MaxFragmentLength as MaxFragmentLength
 from ._tlsi import NextProtocol as NextProtocol
 from ._tlsi import PrivateKey as PrivateKey
 from ._tlsi import ServerNameCallback as ServerNameCallback
 from ._tlsi import TLSConfiguration as TLSConfiguration
 from ._tlsi import TLSVersion as TLSVersion
 
 if sys.version_info < (3, 8):
@@ -46,14 +47,15 @@
 
 
 __all__ = (
     "ClientContext",
     "DTLSConfiguration",
     "DTLSVersion",
     "HelloVerifyRequest",
+    "MaxFragmentLength",
     "NextProtocol",
     "PrivateKey",
     "Purpose",
     "RaggedEOF",
     "ServerContext",
     "ServerNameCallback",
     "TLSConfiguration",
@@ -274,14 +276,25 @@
         return str(self._socket)
 
     @property
     def _handshake_state(self) -> HandshakeStep:
         # pylint: disable=protected-access
         return self._buffer._handshake_state
 
+    def setmtu(self, mtu: int) -> None:
+        """Set Maxiumum Transport Unit (MTU) for DTLS.
+
+        Set to zero to unset.
+
+        Raises:
+            OverflowError: If value cannot be converted to UInt16.
+
+        """
+        self._buffer.setmtu(mtu)
+
     def accept(self) -> Tuple[TLSWrappedSocket, _Address]:
         if self.type == _pysocket.SOCK_STREAM:
             conn, address = self._socket.accept()
         else:
             _, address = self._socket.recvfrom(1024, _pysocket.MSG_PEEK)
             # Use this socket to communicate with the client and bind
             # another one for the next connection.  This procedure is
```

### Comparing `python-mbedtls-2.6.1/src/mbedtls/version.pyx` & `python-mbedtls-2.7.0/src/mbedtls/version.pyx`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/x509.pxd` & `python-mbedtls-2.7.0/src/mbedtls/x509.pxd`

 * *Files 7% similar despite different names*

```diff
@@ -6,38 +6,24 @@
  - CSR: Certificate signing request parsing and writing.
  - CRL: Certificate revocation list parsing.
  - CRT: Certificate parsing and writing.
 
 """
 
 
+cimport mbedtls._asn1 as _asn1
 cimport mbedtls._md as _md
 cimport mbedtls.mpi as _mpi
 cimport mbedtls.pk as _pk
 
 
-cdef extern from "mbedtls/asn1.h" nogil:
-    cdef struct mbedtls_asn1_buf:
-        int tag
-        size_t len
-        unsigned char *p
-    cdef struct mbedtls_asn1_sequence:
-        mbedtls_asn1_buf buf
-        mbedtls_asn1_sequence *next
-    cdef struct mbedtls_asn1_named_data:
-        mbedtls_asn1_buf oid
-        mbedtls_asn1_buf val
-        mbedtls_asn1_named_data *next
-        unsigned char next_merged
-
-
 cdef extern from "mbedtls/x509.h" nogil:
-    ctypedef mbedtls_asn1_buf mbedtls_x509_buf
-    ctypedef mbedtls_asn1_named_data mbedtls_x509_name
-    ctypedef mbedtls_asn1_sequence mbedtls_x509_sequence
+    ctypedef _asn1.mbedtls_asn1_buf mbedtls_x509_buf
+    ctypedef _asn1.mbedtls_asn1_named_data mbedtls_x509_name
+    ctypedef _asn1.mbedtls_asn1_sequence mbedtls_x509_sequence
     int mbedtls_x509_dn_gets(
         char *buf, size_t size, const mbedtls_x509_name *dn)
     cdef struct mbedtls_x509_time:
         int year, mon, day
         int hour, min, sec
```

### Comparing `python-mbedtls-2.6.1/src/mbedtls/x509.pyi` & `python-mbedtls-2.7.0/src/mbedtls/x509.pyi`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/mbedtls/x509.pyx` & `python-mbedtls-2.7.0/src/mbedtls/x509.pyx`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/src/python_mbedtls.egg-info/PKG-INFO` & `python-mbedtls-2.7.0/src/python_mbedtls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: python-mbedtls
-Version: 2.6.1
+Version: 2.7.0
 Summary: hash, hmac, RSA, ECC, X.509, TLS, DTLS, handshakes, and secrets with an mbed TLS back end
 Home-page: https://github.com/Synss/python-mbedtls
-Download-URL: https://github.com/Synss/python-mbedtls/tarball/2.6.1
+Download-URL: https://github.com/Synss/python-mbedtls/tarball/2.7.0
 Author: Mathias Laurin
 Author-email: Mathias.Laurin@github.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -83,15 +83,15 @@
 
 https://synss.github.io/python-mbedtls/
 
 
 Installation
 ============
 
-The bindings are tested with mbedTLS 2.28.2 for Python 3.7,
+The bindings are tested with mbedTLS 2.28.3 for Python 3.7,
 3.8, 3.9, 3.10, and 3.11 on Linux, macOS, and Windows.
 
 `manylinux`_ wheels are available for 64-bit Linux systems.  Install
 with ``pip install python-mbedtls``.
 
 .. _manylinux: https://www.python.org/dev/peps/pep-0513/
 
@@ -105,16 +105,16 @@
 Check which version of mbed TLS is being used by python-mbedtls
 ---------------------------------------------------------------
 
 The *mbedtls.version* module shows the run-time version
 information to mbed TLS.
 
 >>> from mbedtls import version
->>> _ = version.version  # "mbed TLS 2.28.2"
->>> _ = version.version_info  # (2, 28, 2)
+>>> _ = version.version  # "mbed TLS 2.28.3"
+>>> _ = version.version_info  # (2, 28, 3)
 
 
 Message digest
 --------------
 
 The *mbedtls.hashlib* module supports MD2, MD4, MD5, SHA-1, SHA-2
 (in 224, 256, 384, and 512-bits), and RIPEMD-160 secure hashes
```

### Comparing `python-mbedtls-2.6.1/src/python_mbedtls.egg-info/SOURCES.txt` & `python-mbedtls-2.7.0/src/python_mbedtls.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -32,25 +32,33 @@
 scripts/install-mbedtls.sh
 scripts/install-pymbedtls.sh
 scripts/run-tests.sh
 scripts/start-devpi.sh
 scripts/stop-devpi.sh
 scripts/update-reqs.sh
 src/mbedtls/__init__.py
+src/mbedtls/_asn1.pxd
+src/mbedtls/_debug.pxd
+src/mbedtls/_dhm.pxd
+src/mbedtls/_ecdh.pxd
+src/mbedtls/_ecdsa.pxd
+src/mbedtls/_ecp.pxd
 src/mbedtls/_md.pxd
 src/mbedtls/_md.pyi
 src/mbedtls/_md.pyx
 src/mbedtls/_platform.pxd
 src/mbedtls/_platform.pyi
 src/mbedtls/_platform.pyx
 src/mbedtls/_random.pxd
 src/mbedtls/_random.pyi
 src/mbedtls/_random.pyx
 src/mbedtls/_ringbuf.pxd
 src/mbedtls/_ringbuf.pyx
+src/mbedtls/_rsa.pxd
+src/mbedtls/_timing.pxd
 src/mbedtls/_tls.pxd
 src/mbedtls/_tls.pyi
 src/mbedtls/_tls.pyx
 src/mbedtls/_tlsi.py
 src/mbedtls/exceptions.pxd
 src/mbedtls/exceptions.pyi
 src/mbedtls/exceptions.pyx
```

### Comparing `python-mbedtls-2.6.1/tests/conftest.py` & `python-mbedtls-2.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/tests/test_assertion_rewriting.py` & `python-mbedtls-2.7.0/tests/test_assertion_rewriting.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/tests/test_cipher.py` & `python-mbedtls-2.7.0/tests/test_cipher.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/tests/test_error.py` & `python-mbedtls-2.7.0/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/tests/test_hkdf.py` & `python-mbedtls-2.7.0/tests/test_hkdf.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/tests/test_md.py` & `python-mbedtls-2.7.0/tests/test_md.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/tests/test_mpi.py` & `python-mbedtls-2.7.0/tests/test_mpi.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/tests/test_pk.py` & `python-mbedtls-2.7.0/tests/test_pk.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/tests/test_random.py` & `python-mbedtls-2.7.0/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/tests/test_readme.py` & `python-mbedtls-2.7.0/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/tests/test_ringbuf.py` & `python-mbedtls-2.7.0/tests/test_ringbuf.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/tests/test_secrets.py` & `python-mbedtls-2.7.0/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/tests/test_tls.py` & `python-mbedtls-2.7.0/tests/test_tls.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from mbedtls.pk import ECC, RSA
 from mbedtls.tls import (
     ClientContext,
     DTLSConfiguration,
     DTLSVersion,
     HandshakeStep,
     HelloVerifyRequest,
+    MaxFragmentLength,
     NextProtocol,
     Purpose,
     ServerContext,
     TLSConfiguration,
     TLSRecordHeader,
     TLSSession,
     TLSVersion,
@@ -436,14 +437,22 @@
         self,
         conf: Union[TLSConfiguration, DTLSConfiguration],
         trust_store: TrustStore,
     ) -> None:
         assert trust_store
         assert_conf_invariant(conf, trust_store=trust_store)
 
+    @pytest.mark.parametrize("mfl", MaxFragmentLength)
+    def test_max_fragmentation_length(
+        self,
+        conf: Union[TLSConfiguration, DTLSConfiguration],
+        mfl: MaxFragmentLength,
+    ) -> None:
+        assert_conf_invariant(conf, max_fragmentation_length=mfl)
+
     def test_set_sni_callback(
         self,
         conf: Union[TLSConfiguration, DTLSConfiguration],
     ) -> None:
         assert conf.sni_callback is None
 
     @pytest.mark.parametrize("psk", [None, ("client", b"the secret key")])
@@ -814,14 +823,41 @@
         )
         make_full_handshake(client=client, server=server)
 
         secret = b"a very secret message"
         assert do_send(secret, src=client, dst=server) == secret
         assert do_send(secret, src=server, dst=client) == secret
 
+    @pytest.mark.parametrize("mtu_cli", [0, 128, 380, 500, (1 << 16) - 1])
+    @pytest.mark.parametrize("mtu_srv", [0, 128, 380, 500, (1 << 16) - 1])
+    def test_psk_set_mtu(self, mtu_cli: int, mtu_srv: int) -> None:
+        psk = ("cli", b"secret")
+        server = ServerContext(
+            DTLSConfiguration(
+                pre_shared_key_store=dict((psk,)),
+                validate_certificates=False,
+            )
+        ).wrap_buffers()
+        server.setmtu(mtu_srv)
+        client = ClientContext(
+            DTLSConfiguration(
+                pre_shared_key=psk,
+                validate_certificates=False,
+            ),
+        ).wrap_buffers("hostname")
+        client.setmtu(mtu_cli)
+        make_hello_verify_request(
+            client=client, server=server, cookie="🍪🍪🍪".encode()
+        )
+        make_full_handshake(client=client, server=server)
+
+        secret = b"a very secret message"
+        assert do_send(secret, src=client, dst=server) == secret
+        assert do_send(secret, src=server, dst=client) == secret
+
     def test_resume_from_pickle(self) -> None:
         psk = ("cli", b"secret")
         server = ServerContext(
             DTLSConfiguration(
                 pre_shared_key_store=dict((psk,)),
                 validate_certificates=False,
             )
@@ -1020,18 +1056,18 @@
             str(rootpath / "programs" / "server.py"),
             "--port",
             f"{port}",
             "--dtls",
             "--psk-store",
             "cli=secret",
         ]
-        proc = subprocess.Popen(args, text=True, encoding="utf8")
-        yield proc
-        proc.kill()
-        proc.wait(1.0)
+        with subprocess.Popen(args, text=True, encoding="utf8") as proc:
+            yield proc
+            proc.kill()
+            proc.wait(1.0)
 
     @pytest.mark.repeat(3)
     @pytest.mark.usefixtures("server")
     @pytest.mark.timeout(30)
     def test_client(self, rootpath: Path, port: int) -> None:
         secret = "a very secret message"
         args = [
```

### Comparing `python-mbedtls-2.6.1/tests/test_version.py` & `python-mbedtls-2.7.0/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.6.1/tests/test_x509.py` & `python-mbedtls-2.7.0/tests/test_x509.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import datetime as dt
 import pickle
 import sys
+from pathlib import Path
 from typing import Any, Callable, Optional, Tuple, Union
 
 import certifi
 import pytest
 
 from mbedtls import hashlib
 from mbedtls.pk import ECC, RSA
@@ -168,17 +169,19 @@
 
     def test_hash(self, cert: Union[CSR, CRT, CRL]) -> None:
         assert isinstance(hash(cert), int)
 
     def test_from_buffer(self, cert: Union[CSR, CRT, CRL]) -> None:
         assert type(cert).from_buffer(cert.to_DER()) == cert
 
-    def test_from_file(self, cert: Union[CSR, CRT, CRL], tmpdir: Any) -> None:
-        path = tmpdir.join("key.der")
-        path.write_binary(cert.to_DER())
+    def test_from_file(
+        self, cert: Union[CSR, CRT, CRL], tmp_path: Path
+    ) -> None:
+        path = tmp_path / "key.der"
+        path.write_bytes(cert.to_DER())
         assert type(cert).from_file(path) == cert
 
     def test_from_DER(self, cert: Union[CSR, CRT, CRL]) -> None:
         assert type(cert).from_DER(cert.to_DER()) == cert
 
     def test_eq_DER(self, cert: Union[CSR, CRT, CRL]) -> None:
         assert cert == cert.to_DER()
```

