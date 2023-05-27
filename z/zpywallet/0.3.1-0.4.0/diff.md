# Comparing `tmp/zpywallet-0.3.1.tar.gz` & `tmp/zpywallet-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpywallet-0.3.1.tar", last modified: Mon May 15 10:19:31 2023, max compression
+gzip compressed data, was "zpywallet-0.4.0.tar", last modified: Sat May 27 13:47:56 2023, max compression
```

## Comparing `zpywallet-0.3.1.tar` & `zpywallet-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:19:31.172811 zpywallet-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-15 10:19:18.000000 zpywallet-0.3.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-15 10:19:18.000000 zpywallet-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 10:19:18.000000 zpywallet-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-15 10:19:31.172811 zpywallet-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-15 10:19:18.000000 zpywallet-0.3.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-15 10:19:31.172811 zpywallet-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-15 10:19:18.000000 zpywallet-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:19:31.168811 zpywallet-0.3.1/zpywallet/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:19:31.172811 zpywallet-0.3.1/zpywallet/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28188 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/utils/bip32.py
--rw-r--r--   0 runner    (1001) docker     (123)    31084 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/utils/ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    63187 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/utils/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/utils/ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-05-15 10:19:18.000000 zpywallet-0.3.1/zpywallet/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:19:31.168811 zpywallet-0.3.1/zpywallet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-15 10:19:31.000000 zpywallet-0.3.1/zpywallet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-15 10:19:31.000000 zpywallet-0.3.1/zpywallet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:19:31.000000 zpywallet-0.3.1/zpywallet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 10:19:31.000000 zpywallet-0.3.1/zpywallet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 10:19:31.000000 zpywallet-0.3.1/zpywallet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 13:47:55.993326 zpywallet-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-27 13:47:44.000000 zpywallet-0.4.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-27 13:47:44.000000 zpywallet-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 13:47:44.000000 zpywallet-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-05-27 13:47:55.993326 zpywallet-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-27 13:47:44.000000 zpywallet-0.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-27 13:47:55.993326 zpywallet-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-27 13:47:44.000000 zpywallet-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 13:47:55.993326 zpywallet-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-27 13:47:44.000000 zpywallet-0.4.0/tests/test_base58.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-05-27 13:47:44.000000 zpywallet-0.4.0/tests/test_bech32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-27 13:47:44.000000 zpywallet-0.4.0/tests/test_keccak.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6002 2023-05-27 13:47:44.000000 zpywallet-0.4.0/tests/test_mnemonic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-05-27 13:47:44.000000 zpywallet-0.4.0/tests/test_zpywallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 13:47:55.993326 zpywallet-0.4.0/zpywallet/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-27 13:47:44.000000 zpywallet-0.4.0/zpywallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 13:47:44.000000 zpywallet-0.4.0/zpywallet/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 13:47:55.993326 zpywallet-0.4.0/zpywallet/mnemonic/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-27 13:47:44.000000 zpywallet-0.4.0/zpywallet/mnemonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-05-27 13:47:44.000000 zpywallet-0.4.0/zpywallet/mnemonic/mnemonic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-05-27 13:47:44.000000 zpywallet-0.4.0/zpywallet/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 13:47:55.993326 zpywallet-0.4.0/zpywallet/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-27 13:47:44.000000 zpywallet-0.4.0/zpywallet/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-27 13:47:44.000000 zpywallet-0.4.0/zpywallet/utils/base58.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-05-27 13:47:44.000000 zpywallet-0.4.0/zpywallet/utils/bech32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33279 2023-05-27 13:47:44.000000 zpywallet-0.4.0/zpywallet/utils/bip32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-05-27 13:47:44.000000 zpywallet-0.4.0/zpywallet/utils/keccak.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-05-27 13:47:44.000000 zpywallet-0.4.0/zpywallet/utils/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-05-27 13:47:44.000000 zpywallet-0.4.0/zpywallet/utils/ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-27 13:47:44.000000 zpywallet-0.4.0/zpywallet/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-27 13:47:44.000000 zpywallet-0.4.0/zpywallet/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 13:47:55.993326 zpywallet-0.4.0/zpywallet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-05-27 13:47:55.000000 zpywallet-0.4.0/zpywallet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-27 13:47:55.000000 zpywallet-0.4.0/zpywallet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 13:47:55.000000 zpywallet-0.4.0/zpywallet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 13:47:55.000000 zpywallet-0.4.0/zpywallet.egg-info/top_level.txt
```

### Comparing `zpywallet-0.3.1/LICENSE` & `zpywallet-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zpywallet-0.3.1/PKG-INFO` & `zpywallet-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 Metadata-Version: 2.1
 Name: zpywallet
-Version: 0.3.1
-Summary: Simple BIP32 (HD) wallet creation for BTC, BTX, RVN, MXT, BTG, BCH, LTC, DASH, USDT, QTUM and DOGE
+Version: 0.4.0
+Summary: Simple BIP32 (HD) wallet creation for BTC, BCH, LTC, DASH, USDT (Omni) and DOGE
 Home-page: https://github.com/ZenulAbidin/pywallet
 Author: Ali Sherief
 Author-email: ali@notatether.com
 License: MIT License
-Keywords: bitcoin,wallet,litecoin,hd-wallet,dogecoin,dashcoin,bitcore,qtum,ravencoin,martexcoin,address,crypto,python
+Keywords: bitcoin,wallet,litecoin,hd-wallet,dogecoin,dashcoin,tether,address,crypto,python
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 License-File: AUTHORS
 
@@ -36,24 +31,28 @@
     :target: https://pypi.python.org/pypi/zpywallet
     :alt: PyPi version
 
 .. image:: https://img.shields.io/pypi/status/zpywallet.svg?maxAge=60
     :target: https://pypi.python.org/pypi/zpywallet
     :alt: PyPi status
 
-\
+.. image:: https://codecov.io/gh/ZenulAbidin/zpywallet/branch/master/graph/badge.svg?token=G2tC6LpTNm
+    :target: https://codecov.io/gh/ZenulAbidin/zpywallet
+    :alt: Code coverage
 
-**Simple BIP32 (HD) wallet creation for: BTC, BTX, RVN, MXT, BTG, BCH, ETH, LTC, DASH, DOGE**
+**Simple BIP32 (HD) wallet creation for: BTC, BCH, ETH, LTC, DASH, USDT (Omni), DOGE**
 
 BIP32 (or HD for "hierarchical deterministic") wallets allow you to create
 child wallets which can only generate public keys and don't expose a
 private key to an insecure server.
 
-This library simplify the process of creating new wallets for the
-BTC, BTX, RVN, MXT, BTG, BCH, ETH, LTC, DASH and DOGE cryptocurrencies.
+This library simplifies the process of creating new wallets for the
+BTC, BCH, ETH, LTC, DASH, USDT (Omni) and DOGE cryptocurrencies.
+In addition, it can also create Bitcoin Bech32 addresses for all supported
+witness versions.
 
 This is a fork of `PyWallet <https://github.com/ranaroussi/pywallet>` with support for more coins, and some bugfixes.
 
 Enjoy!
 
 --------------
 
@@ -187,14 +186,21 @@
     {
       "address": "1KpS2wC5J8bDsGShXDHD7qdGvnic1h27Db",
       "path": "m/0/394997119"
     }
 
 -----
 
+CONTRIBUTING
+============
+
+Bugfixes and enhancements are welcome. Please read CONTRIBUTING.md for contributing instructions.
+
+At the moment, I'm not accepting pull requests for new coins unless they are big and historic coins such as Tether (ERC20), BNB and XMR.
+
 IMPORTANT
 =========
 
 I **highly** recommend that you familiarize yourself with the Blockchain technology and
 be aware of security issues.
 Reading `Mastering Bitcoin <https://github.com/bitcoinbook/bitcoinbook>`_ and going over
 Steven Buss's security notes on the `Bitmerchant repository <https://github.com/sbuss/bitmerchant>`_
```

### Comparing `zpywallet-0.3.1/README.rst` & `zpywallet-0.4.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,28 @@
     :target: https://pypi.python.org/pypi/zpywallet
     :alt: PyPi version
 
 .. image:: https://img.shields.io/pypi/status/zpywallet.svg?maxAge=60
     :target: https://pypi.python.org/pypi/zpywallet
     :alt: PyPi status
 
-\
+.. image:: https://codecov.io/gh/ZenulAbidin/zpywallet/branch/master/graph/badge.svg?token=G2tC6LpTNm
+    :target: https://codecov.io/gh/ZenulAbidin/zpywallet
+    :alt: Code coverage
 
-**Simple BIP32 (HD) wallet creation for: BTC, BTX, RVN, MXT, BTG, BCH, ETH, LTC, DASH, DOGE**
+**Simple BIP32 (HD) wallet creation for: BTC, BCH, ETH, LTC, DASH, USDT (Omni), DOGE**
 
 BIP32 (or HD for "hierarchical deterministic") wallets allow you to create
 child wallets which can only generate public keys and don't expose a
 private key to an insecure server.
 
-This library simplify the process of creating new wallets for the
-BTC, BTX, RVN, MXT, BTG, BCH, ETH, LTC, DASH and DOGE cryptocurrencies.
+This library simplifies the process of creating new wallets for the
+BTC, BCH, ETH, LTC, DASH, USDT (Omni) and DOGE cryptocurrencies.
+In addition, it can also create Bitcoin Bech32 addresses for all supported
+witness versions.
 
 This is a fork of `PyWallet <https://github.com/ranaroussi/pywallet>` with support for more coins, and some bugfixes.
 
 Enjoy!
 
 --------------
 
@@ -161,14 +165,21 @@
     {
       "address": "1KpS2wC5J8bDsGShXDHD7qdGvnic1h27Db",
       "path": "m/0/394997119"
     }
 
 -----
 
+CONTRIBUTING
+============
+
+Bugfixes and enhancements are welcome. Please read CONTRIBUTING.md for contributing instructions.
+
+At the moment, I'm not accepting pull requests for new coins unless they are big and historic coins such as Tether (ERC20), BNB and XMR.
+
 IMPORTANT
 =========
 
 I **highly** recommend that you familiarize yourself with the Blockchain technology and
 be aware of security issues.
 Reading `Mastering Bitcoin <https://github.com/bitcoinbook/bitcoinbook>`_ and going over
 Steven Buss's security notes on the `Bitmerchant repository <https://github.com/sbuss/bitmerchant>`_
```

### Comparing `zpywallet-0.3.1/setup.py` & `zpywallet-0.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,43 +24,30 @@
                 version_file=version_file))
 
 version = load_version()
 
 setup(
     name='zpywallet',
     version=version,
-    description="Simple BIP32 (HD) wallet creation for BTC, BTX, RVN, MXT, BTG, BCH, LTC, DASH, USDT, QTUM and DOGE",
+    description="Simple BIP32 (HD) wallet creation for BTC, BCH, LTC, DASH, USDT (Omni) and DOGE",
     long_description=long_description,
     url='https://github.com/ZenulAbidin/pywallet',
     author='Ali Sherief',
     author_email='ali@notatether.com',
     license='MIT License',
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Development Status :: 4 - Beta",
 
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
 
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     platforms = ['any'],
-    keywords='bitcoin, wallet, litecoin, hd-wallet, dogecoin, dashcoin, bitcore, qtum, ravencoin, martexcoin, address, crypto, python',
+    keywords='bitcoin, wallet, litecoin, hd-wallet, dogecoin, dashcoin, tether, address, crypto, python',
     packages = find_packages(exclude=['contrib', 'docs', 'tests', 'demo', 'demos', 'examples']),
-    package_data={'': ['AUTHORS', 'LICENSE']},
-    install_requires=[
-        'base58>=0.2.2',
-        'ecdsa>=0.11',
-        'six>=1.8.0',
-        'pycryptodome>=3.6.6',
-        'mnemonic>=0.18',
-        'cachetools>=1.1.1'
-    ]
+    package_data={'': ['AUTHORS', 'LICENSE']}
 )
```

### Comparing `zpywallet-0.3.1/zpywallet/utils/bip32.py` & `zpywallet-0.4.0/zpywallet/utils/bip32.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,28 @@
-from binascii import hexlify
-from binascii import unhexlify
-from hashlib import sha256
-from hashlib import sha512
+"""
+Module for generating Heirarchical Deterministic (HD) keys for supported networks.
+"""
+from binascii import hexlify, unhexlify
+from hashlib import sha256, sha512
 import hmac
-from mnemonic.mnemonic import Mnemonic
-
-import base58
 from os import urandom
-from ecdsa import SECP256k1
-from ecdsa.ecdsa import Public_key as _ECDSA_Public_key
-from ecdsa.ellipticcurve import INFINITY
-import six
 import time
-from cachetools.func import lru_cache
+
+import coincurve
+import six
+
+from .base58 import b58encode_check, b58decode_check
+from ..mnemonic.mnemonic import Mnemonic
+from .keys import incompatible_network_exception_factory, PrivateKey, PublicKey, Point, secp256k1
+from .keys import InvalidKeyDataException
+from .utils import ensure_bytes, ensure_str, hash160, is_hex_string, long_or_int, long_to_hex
 
 # import all the networks
 from ..network import *
 
-from .keys import incompatible_network_exception_factory
-from .keys import PrivateKey
-from .keys import PublicKey
-from .keys import PublicPair
-from .utils import chr_py2
-from .utils import ensure_bytes
-from .utils import ensure_str
-from .utils import hash160
-from .utils import is_hex_string
-from .utils import long_or_int
-from .utils import long_to_hex
-
 
 
 class Wallet(object):
     """A BIP32 wallet is made up of Wallet nodes.
 
     A Private node contains both a public and private key, while a public
     node contains only a public key.
@@ -41,15 +31,15 @@
 
     When creating a NEW wallet you MUST back up the private key. If
     you don't then any coins sent to your address will be LOST FOREVER.
 
     You need to save the private key somewhere. It is OK to just write
     it down on a piece of paper! Don't share this key with anyone!
 
-    >>> my_wallet = Wallet.from_master_secret(
+    >>> my_wallet = Wallet.from_mnemonic(
     ...     key='correct horse battery staple')
     >>> private = my_wallet.serialize(private=True)
     >>> private  # doctest: +ELLIPSIS
     u'xprv9s21ZrQH143K2mDJW8vDeFwbyDbFv868mM2Zr87rJSTj8q16Unkaq1pryiV...'
 
     If you want to use this wallet on your website to accept bitcoin or
     altcoin payments, you should first create a primary child.
@@ -63,106 +53,124 @@
                  depth=0,
                  parent_fingerprint=0,
                  child_number=0,
                  private_exponent=None,
                  private_key=None,
                  public_pair=None,
                  public_key=None,
-                 network="BTC"):
+                 mnemonic=None,
+                 network="btc"):
         """Construct a new BIP32 compliant wallet.
 
         You probably don't want to use this init methd. Instead use one
-        of the 'from_master_secret' or 'deserialize' cosntructors.
+        of the class methods for creating a wallet.
+
+        In particular, the mnemonic is not used to generate the wallet in
+        this constructor and its only purpose here is for storage. The Wallet
+        object deals with master private keys for creating things, which are generated
+        in the class methods.
         """
 
         if (not (private_exponent or private_key) and
                 not (public_pair or public_key)):
             raise InsufficientKeyDataError(
                 "You must supply one of private_exponent or public_pair")
 
-        network = Wallet.get_network(network)
+        self.mnemonic = mnemonic
         self.private_key = None
         self.public_key = None
         if private_key:
             self.private_key = private_key
         elif private_exponent:
-            self.private_key = PrivateKey(private_exponent)
+            self.private_key = PrivateKey.from_int(private_exponent)
 
         if public_key:
             self.public_key = public_key
         elif public_pair:
-            self.public_key = PublicKey(public_pair.x, public_pair.y)
+            self.public_key = PublicKey.from_point(public_pair)
         else:
             self.public_key = self.private_key.public_key
 
         if (self.private_key and self.private_key.public_key !=
                 self.public_key):
             raise KeyMismatchError(
                 "Provided private and public values do not match")
 
-        def h(val, hex_len):
+        def hex_check_length(val, hex_len):
             if isinstance(val, six.integer_types):
                 return long_to_hex(val, hex_len)
             elif (isinstance(val, six.string_types) or
                     isinstance(val, six.binary_type)) and is_hex_string(val):
                 val = ensure_bytes(val)
                 if len(val) != hex_len:
                     raise ValueError("Invalid parameter length")
                 return val
             else:
                 raise ValueError("Invalid parameter type")
 
-        def l(val):
+        def hex_long_or_int(val):
             if isinstance(val, six.integer_types):
                 return long_or_int(val)
             elif (isinstance(val, six.string_types) or
                     isinstance(val, six.binary_type)):
                 val = ensure_bytes(val)
                 if not is_hex_string(val):
                     val = hexlify(val)
                 return long_or_int(val, 16)
             else:
                 raise ValueError("parameter must be an int or long")
 
-        self.network = Wallet.get_network(network)
-        self.depth = l(depth)
+        if isinstance(network, six.string_types):
+            self.network = Wallet.get_network(network)
+        else:
+            self.network = network
+        self.depth = hex_long_or_int(depth)
         if (isinstance(parent_fingerprint, six.string_types) or
                 isinstance(parent_fingerprint, six.binary_type)):
             val = ensure_bytes(parent_fingerprint)
             if val.startswith(b"0x"):
                 parent_fingerprint = val[2:]
-        self.parent_fingerprint = b"0x" + h(parent_fingerprint, 8)
-        self.child_number = l(child_number)
-        self.chain_code = h(chain_code, 64)
+        self.parent_fingerprint = b"0x" + hex_check_length(parent_fingerprint, 8)
+        self.child_number = hex_long_or_int(child_number)
+        self.chain_code = hex_check_length(chain_code, 64)
 
     def get_private_key_hex(self):
         """
         Get the hex-encoded (I guess SEC1?) representation of the private key.
 
         DO NOT share this private key with anyone.
         """
-        return ensure_bytes(self.private_key.get_key())
+        return ensure_bytes(self.private_key.to_hex())
 
     def get_public_key_hex(self, compressed=True):
         """Get the sec1 representation of the public key."""
-        return hexlify(ensure_bytes(self.public_key.get_key(compressed)))
+        return ensure_bytes(self.public_key.to_hex(compressed))
 
     @property
     def identifier(self):
         """Get the identifier for this node.
 
         Extended keys can be identified by the Hash160 (RIPEMD160 after SHA256)
         of the public key's `key`. This corresponds exactly to the data used in
         traditional Bitcoin addresses. It is not advised to represent this data
         in base58 format though, as it may be interpreted as an address that
         way (and wallet software is not required to accept payment to the chain
         key itself).
         """
         key = self.get_public_key_hex()
         return ensure_bytes(hexlify(hash160(unhexlify(key))))
+    
+    @property
+    def mnemonic_phrase(self):
+        """Returns the mnemonic phrase for this wallet, if specified.
+        
+        WARNING: Never share your mnemonic phrase with anyone. They can
+        use it to steal your assets.
+        """
+        return self.mnemonic
 
     @property
     def fingerprint(self):
         """The first 32 bits of the identifier are called the fingerprint."""
         # 32 bits == 4 Bytes == 8 hex characters
         return b'0x' + self.identifier[:8]
 
@@ -171,16 +179,15 @@
 
         This is a convenience wrapper around `get_child` that helps you do
         the right thing. This method always creates a public, non-prime
         address that can be generated from a BIP32 public key on an
         insecure server."""
         max_id = 0x80000000
         if user_id < 0 or user_id > max_id:
-            raise ValueError(
-                "Invalid UserID. Must be between 0 and %s" % max_id)
+            raise ValueError(f"Invalid UserID. Must be between 0 and {max_id}")
         return self.get_child(user_id, is_prime=False, as_private=False)
 
     def get_child_for_path(self, path):
         """Get a child for a given path.
 
         Rather than repeated calls to get_child, children can be found
         by a derivation path. Paths look like:
@@ -205,15 +212,15 @@
             M/0/1
             m/0/1.pub
             M/0/1.pub
         """
         path = ensure_str(path)
 
         if not path:
-            raise InvalidPathError("%s is not a valid path" % path)
+            raise InvalidPathError(f"{path} is not a valid path")
 
         # Figure out public/private derivation
         as_private = True
         if path.startswith("M"):
             as_private = False
         if path.endswith(".pub"):
             as_private = False
@@ -229,22 +236,31 @@
                 continue
             is_prime = None  # Let primeness be figured out by the child number
             if part[-1] in "'p":
                 is_prime = True
                 part = part.replace("'", "").replace("p", "")
             try:
                 child_number = long_or_int(part)
-            except ValueError:
-                raise InvalidPathError("%s is not a valid path" % path)
+            except ValueError as exc:
+                raise InvalidPathError(f"{path} is not a valid path") from exc
             child = child.get_child(child_number, is_prime)
         if not as_private:
             return child.public_copy()
         return child
 
-    @lru_cache(maxsize=1024)
+    def legacy_child(self):
+        """Equivalent to get_child(44, is_prime=True)
+        """
+        return self.get_child(44, is_prime=True)
+
+    def segwit_child(self):
+        """Equivalent to get_child(84, is_prime=True)
+        """
+        return self.get_child(84, is_prime=True)
+
     def get_child(self, child_number, is_prime=None, as_private=True):
         """Derive a child key.
 
         :param child_number: The number of the child key to compute
         :type child_number: int
         :param is_prime: If True, the child is calculated via private
             derivation. If False, then public derivation is used. If None,
@@ -265,38 +281,36 @@
 
         NOTE: negative numbered children are provided as a convenience
         because nobody wants to remember the above numbers. Negative numbers
         are considered 'prime children', which is described in the BIP32 spec
         as a leading 1 in a 32 bit unsigned int.
 
         This derivation is fully described at
-        https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki#child-key-derivation-functions  # nopep8
+        https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki#child-key-derivation-functions
         """
         boundary = 0x80000000
 
         # Note: If this boundary check gets removed, then children above
         # the boundary should use private (prime) derivation.
         if abs(child_number) >= boundary:
-            raise ValueError("Invalid child number %s" % child_number)
+            raise ValueError(f"Invalid child number {child_number}")
 
         # If is_prime isn't set, then we can infer it from the child_number
         if is_prime is None:
             # Prime children are either < 0 or > 0x80000000
             if child_number < 0:
                 child_number = abs(child_number)
                 is_prime = True
             else:
                 is_prime = False
         else:
             # Otherwise is_prime is set so the child_number should be between
             # 0 and 0x80000000
             if child_number < 0 or child_number >= boundary:
-                raise ValueError(
-                    "Invalid child number. Must be between 0 and %s" %
-                    boundary)
+                raise ValueError(f"Invalid child number. Must be between 0 and {boundary}")
 
         if not self.private_key and is_prime:
             raise ValueError(
                 "Cannot compute a prime child without a private key")
 
         if is_prime:
             # Even though we take child_number as an int < boundary, the
@@ -309,67 +323,62 @@
             data = b'00' + ensure_bytes(self.private_key.to_hex())
         else:
             data = self.get_public_key_hex()
         data += child_number_hex
 
         # Compute a 64 Byte I that is the HMAC-SHA512, using self.chain_code
         # as the seed, and data as the message.
-        I = hmac.new(
+        ichild = hmac.new(
             unhexlify(ensure_bytes(self.chain_code)),
             msg=unhexlify(ensure_bytes(data)),
             digestmod=sha512).digest()
         # Split I into its 32 Byte components.
-        I_L, I_R = I[:32], I[32:]
+        ichild_left, ichild_right = ichild[:32], ichild[32:]
 
-        if long_or_int(hexlify(I_L), 16) >= SECP256k1.order:
+        if long_or_int(hexlify(ichild_left), 16) >= secp256k1.N:
             raise InvalidPrivateKeyError("The derived key is too large.")
 
-        c_i = hexlify(I_R)
+        c_i = hexlify(ichild_right)
         private_exponent = None
-        public_pair = None
+        point = None
         if self.private_key:
             # Use private information for derivation
             # I_L is added to the current key's secret exponent (mod n), where
             # n is the order of the ECDSA curve in use.
             private_exponent = (
-                (long_or_int(hexlify(I_L), 16) +
+                (long_or_int(hexlify(ichild_left), 16) +
                  long_or_int(ensure_bytes(self.private_key.to_hex()), 16))
-                % SECP256k1.order)
+                % secp256k1.N)
             # I_R is the child's chain code
         else:
             # Only use public information for this derivation
-            g = SECP256k1.generator
-            I_L_long = long_or_int(hexlify(I_L), 16)
-            point = (_ECDSA_Public_key(g, g * I_L_long).point +
-                     self.public_key.to_point())
+            gen = coincurve.PublicKey.from_point(secp256k1.Gx, secp256k1.Gy)
+            point = Point(*gen.multiply(ichild_left).add(self.public_key.to_bytes()).point())
             # I_R is the child's chain code
-            public_pair = PublicPair(point.x(), point.y())
 
         child = self.__class__(
             chain_code=c_i,
             depth=self.depth + 1,  # we have to go deeper...
             parent_fingerprint=self.fingerprint,
             child_number=child_number_hex,
             private_exponent=private_exponent,
-            public_pair=public_pair,
+            public_pair=point,
             network=self.network)
-        if child.public_key.point.infinity:
-            raise InfinityPointException("The point at infinity is invalid.")
         if not as_private:
             return child.public_copy()
         return child
 
     def public_copy(self):
         """Clone this wallet and strip it of its private information."""
         return self.__class__(
             chain_code=self.chain_code,
             depth=self.depth,
             parent_fingerprint=self.parent_fingerprint,
             child_number=self.child_number,
-            public_pair=self.public_key.to_public_pair(),
+            public_pair=self.public_key.to_point(),
             network=self.network)
 
     def crack_private_key(self, child_private_key):
         """Crack the parent private key given a child private key.
 
         BIP32 has a vulnerability/feature that allows you to recover the
         master private key if you're given a master public key and any of its
@@ -383,37 +392,37 @@
         >>> master_public_key = w_pub.serialize_b58(private=False)
         >>> # Now you put master_public_key on your website
         >>> # and give somebody a private key
         >>> public_master = Wallet.deserialize(master_public_key)
         >>> cracked_private_master = public_master.crack_private_key(child)
         >>> assert w == cracked_private_master  # :(
 
-        Implementation details from http://bitcoinmagazine.com/8396/deterministic-wallets-advantages-flaw/  # nopep8
+        Implementation details from:
+          http://bitcoinmagazine.com/8396/deterministic-wallets-advantages-flaw/
         """
         if self.private_key:
             raise AssertionError("You already know the private key")
         if child_private_key.parent_fingerprint != self.fingerprint:
             raise ValueError("This is not a valid child")
         if child_private_key.child_number >= 0x80000000:
             raise ValueError(
                 "Cannot crack private keys from private derivation")
 
         # Duplicate the public child derivation
         child_number_hex = long_to_hex(child_private_key.child_number, 8)
         data = self.get_public_key_hex() + child_number_hex
-        I = hmac.new(
+        ichild = hmac.new(
             unhexlify(self.chain_code),
             msg=unhexlify(data),
             digestmod=sha512).digest()
-        I_L, I_R = I[:32], I[32:]
+        ichild_left, _ = ichild[:32], ichild[32:]
         # Public derivation is the same as private derivation plus some offset
         # knowing the child's private key allows us to find this offset just
         # by subtracting the child's private key from the parent I_L data
-        privkey = PrivateKey(long_or_int(hexlify(I_L), 16),
-                             network=self.network)
+        privkey = PrivateKey.from_bytes(ichild_left)
         parent_private_key = child_private_key.private_key - privkey
         return self.__class__(
             chain_code=self.chain_code,
             depth=self.depth,
             parent_fingerprint=self.parent_fingerprint,
             child_number=self.child_number,
             private_key=parent_private_key,
@@ -432,17 +441,21 @@
 
         See the spec in `deserialize` for more details.
         """
         if private and not self.private_key:
             raise ValueError("Cannot serialize a public key as private")
 
         if private:
+            if not self.network.EXT_SECRET_KEY:
+                raise ValueError("Network does not support private key serialization")
             network_version = long_to_hex(
                 self.network.EXT_SECRET_KEY, 8)
         else:
+            if not self.network.EXT_PUBLIC_KEY:
+                raise ValueError("Network does not support public key serialization")
             network_version = long_to_hex(
                 self.network.EXT_PUBLIC_KEY, 8)
         depth = long_to_hex(self.depth, 2)
         parent_fingerprint = self.parent_fingerprint[2:]  # strip leading 0x
         child_number = long_to_hex(self.child_number, 8)
         chain_code = self.chain_code
         ret = (network_version + depth + parent_fingerprint + child_number +
@@ -453,35 +466,40 @@
         else:
             ret += self.get_public_key_hex(compressed=True)
         return ensure_bytes(ret.lower())
 
     def serialize_b58(self, private=True):
         """Encode the serialized node in base58."""
         return ensure_str(
-            base58.b58encode_check(unhexlify(self.serialize(private))))
+            b58encode_check(unhexlify(self.serialize(private))))
 
-    def to_address(self):
+    def address(self, compressed=True, witness_version=0):
         """Create a public address from this Wallet.
 
         Public addresses can accept payments.
 
         https://en.bitcoin.it/wiki/Technical_background_of_Bitcoin_addresses
-        """
-        key = unhexlify(self.get_public_key_hex())
-        # First get the hash160 of the key
-        hash160_bytes = hash160(key)
-        # Prepend the network address byte
-        network_hash160_bytes = \
-            chr_py2(self.network.PUBKEY_ADDRESS) + hash160_bytes
-        # Return a base58 encoded address with a checksum
-        return ensure_str(base58.b58encode_check(network_hash160_bytes))
+
+
+        Args:
+            compressed (bool): Whether or not the compressed key should
+               be used.
+            witness_version (int): Used only when creating Bech32 addresses.
+                Allowed values are 0 (segwit) and 1 (Taproot).
+
+        Returns:
+            str: An encoded address
+        """
+        key = PublicKey.from_bytes(unhexlify(self.get_public_key_hex()), network=self.network)
+        return ensure_str(key.address(compressed=compressed,
+                                      witness_version=witness_version))
 
     @classmethod
-    def deserialize(cls, key, network="BTC"):
-        """Load the ExtendedBip32Key from a hex key.
+    def deserialize(cls, key, network="btc"):
+        """Load an extended BIP32 private key from a hex string.
 
         The key consists of
 
             * 4 byte version bytes (network key)
             * 1 byte depth:
                 - 0x00 for master nodes,
                 - 0x01 for level-1 descendants, ....
@@ -504,101 +522,176 @@
         else:
             key = ensure_bytes(key)
             if len(key) in [78 * 2, (78 + 32) * 2]:
                 # we have a hexlified non-base58 key, continue!
                 key = unhexlify(key)
             elif len(key) == 111:
                 # We have a base58 encoded string
-                key = base58.b58decode_check(key)
+                key = b58decode_check(key)
         # Now that we double checkd the values, convert back to bytes because
         # they're easier to slice
         version, depth, parent_fingerprint, child, chain_code, key_data = (
             key[:4], key[4], key[5:9], key[9:13], key[13:45], key[45:])
 
+        if long_or_int(depth) == 0 and long_or_int(hexlify(parent_fingerprint), 16) != 0:
+            raise InvalidKeyDataException("Zero depth with non-zero parent fingerprint")
+        if long_or_int(depth) == 0 and long_or_int(hexlify(child)) != 0:
+            raise InvalidKeyDataException("Zero depth with non-zero index")
         version_long = long_or_int(hexlify(version), 16)
         exponent = None
         pubkey = None
         point_type = key_data[0]
         if not isinstance(point_type, six.integer_types):
             point_type = ord(point_type)
         if point_type == 0:
             # Private key
             if version_long != network.EXT_SECRET_KEY:
                 raise incompatible_network_exception_factory(
-                    network.NAME, network.EXT_SECRET_KEY,
+                    network.NAME, unhexlify(f"{network.EXT_SECRET_KEY:x}".zfill(8)),
                     version)
             exponent = key_data[1:]
+            iexponent = long_or_int(hexlify(exponent), 16)
+            if iexponent < 1 or iexponent >= secp256k1.N:
+                raise InvalidKeyDataException("Private key is out of range")
         elif point_type in [2, 3, 4]:
             # Compressed public coordinates
             if version_long != network.EXT_PUBLIC_KEY:
                 raise incompatible_network_exception_factory(
-                    network.NAME, network.EXT_PUBLIC_KEY,
+                    network.NAME, unhexlify(f"{network.EXT_PUBLIC_KEY:x}".zfill(8)),
                     version)
-            pubkey = PublicKey.from_hex_key(key_data, network=network)
+            pubkey = PublicKey.from_bytes(key_data)
             # Even though this was generated from a compressed pubkey, we
             # want to store it as an uncompressed pubkey
             pubkey.compressed = False
         else:
-            raise ValueError("Invalid key_data prefix, got %s" % point_type)
+            raise ValueError(f"Invalid key_data prefix, got {point_type}")
 
-        def l(byte_seq):
+        def bytes_long_or_int(byte_seq):
             if byte_seq is None:
                 return byte_seq
             elif isinstance(byte_seq, six.integer_types):
                 return byte_seq
             return long_or_int(hexlify(byte_seq), 16)
 
-        return cls(depth=l(depth),
-                   parent_fingerprint=l(parent_fingerprint),
-                   child_number=l(child),
-                   chain_code=l(chain_code),
-                   private_exponent=l(exponent),
+        return cls(depth=bytes_long_or_int(depth),
+                   parent_fingerprint=bytes_long_or_int(parent_fingerprint),
+                   child_number=bytes_long_or_int(child),
+                   chain_code=bytes_long_or_int(chain_code),
+                   private_exponent=bytes_long_or_int(exponent),
                    public_key=pubkey,
                    network=network)
 
     @classmethod
-    def from_master_secret(cls, mnemonic, network="BTC"):
+    def from_mnemonic(cls, mnemonic, passphrase='', network="BTC"):
         """Generate a new PrivateKey from a secret key.
 
-        :param mnemonic: The key to use to generate this wallet. It may be a long
-            string. Do not use a phrase from a book or song, as that will
-            be guessed and is not secure. My advice is to not supply this
-            argument and let me generate a new random key for you.
+        :param mnemonic: The key to use to generate this wallet.
+        :param passphrase: An optional passphrase for this mnemonic.
+        :param network: The network to use. Defaults to Bitcoin mainnet.
+        
 
-        See https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki#Serialization_format  # nopep8
+        See https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki#Serialization_format
         """
         network = Wallet.get_network(network)
-        m = Mnemonic(language='english')
-        seed = ensure_bytes(m.to_seed(mnemonic))
-        
+        mne = Mnemonic(language='english')
+        seed = ensure_bytes(mne.to_seed(mnemonic, passphrase))
+
         # Given a seed S of at least 128 bits, but 256 is advised
         # Calculate I = HMAC-SHA512(key="Bitcoin seed", msg=S)
         I = hmac.new(b"Bitcoin seed", msg=seed, digestmod=sha512).digest()
         # Split I into two 32-byte sequences, IL and IR.
-        I_L, I_R = I[:32], I[32:]
+        Il, Ir = I[:32], I[32:]
         # Use IL as master secret key, and IR as master chain code.
-        return cls(private_exponent=long_or_int(hexlify(I_L), 16),
-                   chain_code=hexlify(I_R),
+        return cls(private_exponent=long_or_int(hexlify(Il), 16),
+                   chain_code=hexlify(Ir), mnemonic=mnemonic,
                    network=network)
 
     @classmethod
-    def from_master_secret_slow(cls, password, network=BitcoinMainNet):
+    def from_brainwallet(cls, password, network=BitcoinMainNet):
         """
         Generate a new key from a password using 50,000 rounds of HMAC-SHA256.
 
         This should generate the same result as bip32.org.
 
         WARNING: The security of this method has not been evaluated.
+
+        Args:
+            :param password (str):  The value to hash for generating the wallet.
+            It may be a long string. Do not use a phrase from a book or song,
+            as that will be guessed and is not secure.
+            :param network: The network to use. Defaults to Bitcoin mainnet.
+        
+        Returns:
+            Wallet: A Wallet object.
         """
+        network = Wallet.get_network(network)
         # Make sure the password string is bytes
         key = ensure_bytes(password)
         data = unhexlify(b"0" * 64)  # 256-bit 0
-        for i in range(50000):
+        for _ in range(50000):
             data = hmac.new(key, msg=data, digestmod=sha256).digest()
-        return cls.from_master_secret(data, network)
+
+        I = hmac.new(b"Bitcoin seed", msg=data, digestmod=sha512).digest()
+        # Split I into two 32-byte sequences, IL and IR.
+        Il, Ir = I[:32], I[32:]
+        # Use IL as master secret key, and IR as master chain code.
+        return cls(private_exponent=long_or_int(hexlify(Il), 16),
+                   chain_code=hexlify(Ir),
+                   network=network)
+
+    @classmethod
+    def from_master_seed(cls, seed, network="BTC"):
+        """Generate a new PrivateKey from a seed (byte string).
+
+        :param seed: The byte sequence to use to generate this wallet. The seed length
+            should be at least 128 bits, no longer than 256 bits, and be divisible by 32.
+        :param network: The network to use. Defaults to Bitcoin mainnet.
+        
+
+        See https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki#Serialization_format
+        """
+        network = Wallet.get_network(network)
+
+        # Given a seed S of at least 128 bits, but 256 is advised
+        # Calculate I = HMAC-SHA512(key="Bitcoin seed", msg=S)
+        I = hmac.new(b"Bitcoin seed", msg=seed, digestmod=sha512).digest()
+        # Split I into two 32-byte sequences, IL and IR.
+        Il, Ir = I[:32], I[32:]
+        # Use IL as master secret key, and IR as master chain code.
+        return cls(private_exponent=long_or_int(hexlify(Il), 16),
+                   chain_code=hexlify(Ir),
+                   network=network)
+    
+    @classmethod
+    def from_random(cls, passphrase='', strength=128, network=BitcoinMainNet):
+        """ Generates a master key from system entropy.
+
+        Args:
+            :param strength (int): Amount of entropy desired, in bits.
+                This should be a multiple of 32 between 128 and 256.
+                It directly affects the length of the mnemonic exported
+                (each additional 32 bits adds an extra three words at the end).
+            passphrase (str): An optional passphrase for the generated
+               mnemonic string.
+            :param network: The network to use for things like defining key
+                key paths and supported address formats. Defaults to Bitcoin mainnet.
+
+        Returns:
+            Wallet: The wallet object created.
+        """
+        if strength % 32 != 0:
+            raise ValueError("strength must be a multiple of 32")
+        if strength < 128 or strength > 256:
+            raise ValueError("strength should be >= 128 and <= 256")
+        entropy = urandom(strength // 8)
+        mne = Mnemonic(language='english')
+        mnemonic = mne.to_mnemonic(entropy)
+        return cls.from_mnemonic(
+            mnemonic, passphrase, network=network)
+
 
     def __eq__(self, other):
         attrs = [
             'chain_code',
             'depth',
             'parent_fingerprint',
             'child_number',
@@ -611,62 +704,68 @@
 
     def __ne__(self, other):
         return not self == other
 
     __hash__ = object.__hash__
 
     @classmethod
-    def get_network(self, network):
-        # returns a network class object
+    def get_network(cls, network):
+        """
+        Returns the appropriate network class object based on the provided network string.
 
+        Args:
+            network (str): A string indicating the name or code of the network
+
+        Returns:
+            A class object representing the requested network, or the fallback string if no match
+            found.
+
+        Raises:
+            ValueError: If no match is found from the predefined networks
+        """
         response = None
-        if network == "bitcoin_testnet" or network == "BTCTEST":
+        network = network.lower()
+        if network == "bitcoin_testnet" or network == "btctest":
             response = BitcoinTestNet
-        elif network == "bitcoin" or network == "BTC":
+        elif network == "bitcoin" or network == "btc":
             response = BitcoinMainNet
-        elif network == "dogecoin" or network == "DOGE":
+        elif network == "dogecoin" or network == "doge":
             response = DogecoinMainNet
-        elif network == "dogecoin_testnet" or network == "DOGETEST":
+        elif network == "dogecoin-btc" or network == "dogebtc":
+            response = DogecoinBTCMainNet
+        elif network == "dogecoin-testnet" or network == "dogetest":
             response = DogecoinTestNet
-        elif network == "litecoin" or network == "LTC":
+        elif network == "litecoin" or network == "ltc":
             response = LitecoinMainNet
-        elif network == "litecoin_testnet" or network == "LTCTEST":
+        elif network == "litecoin-btc" or network == "ltcbtc":
+            response = LitecoinBTCMainNet
+        elif network == "litecoin-testnet" or network == "ltctest":
             response = LitecoinTestNet
-        elif network == "bitcoin_cash" or network == "BCH":
+        elif network == "bitcoin-cash" or network == "bch":
             response = BitcoinCashMainNet
-        elif network == "bitcoin_gold" or network == "BTG":
-            response = BitcoinGoldMainNet
-        elif network == "dash" or network == "DASH":
+        elif network == "dash":
             response = DashMainNet
-        elif network == 'dash_testnet' or network == 'DASHTEST':
+        elif network == "dash-inverted":
+            response = DashInvertedMainNet
+        elif network == "dash-btc" or network == "dashbtc":
+            response = DashBTCMainNet
+        elif network == 'dash_testnet' or network == 'dashtest':
             response = DashTestNet
-        elif network == "martex" or network == "MXT":
-            response = MarteXMainNet
-        elif network == 'martex_testnet' or network == 'MXTTEST':
-            response = MarteXTestNet
-        elif network == 'omni' or network == 'OMNI':
+        elif network == 'dash_testnet_inverted':
+            response = DashInvertedTestNet
+        elif network == 'omni':
             response = OmniMainNet
-        elif network == 'omni_testnet' or network == 'OMNI_TESTNET':
+        elif network == 'omni_testnet' or network == 'omnitest':
             response = OmniTestNet
-        elif network == 'feathercoin' or network == 'FTC':
-            response = FeathercoinMainNet
-        elif network == "qtum" or network == "QTUM":
-            response = QtumMainNet
-        elif network == 'qtum_testnet' or network == 'QTUMTEST':
-            response = QtumTestNet
-        elif network == 'raven' or network == 'RVN':
-            response = RavenMainNet
-        elif network == 'raven_testnet' or network == 'RVNTEST':
-            response = RavenTestNet
-        elif network == 'bitcore' or network == 'BTX':
-            response = BitcoreMainNet
-        elif network == 'bitcore_testnet' or network == 'BTX_TESTNET':
-            response = BitcoreTestNet
+        elif network == 'ethereum' or network == 'eth':
+            response = EthereumMainNet
+        elif network == 'blockcypher_testnet' or network == 'bcytest':
+            response = BlockCypherTestNet
         else:
-            response = network
+            raise ValueError("Network is not defined")
         return response
 
     @classmethod
     def new_random_wallet(cls, user_entropy=None, network=BitcoinMainNet):
         """
         Generate a new wallet using a randomly generated 512 bit seed.
 
@@ -684,32 +783,44 @@
         """
         seed = str(urandom(64))  # 512/8
         # weak extra protection inspired by pybitcointools implementation:
         seed += str(int(time.time()*10**6))
         if user_entropy:
             user_entropy = str(user_entropy)  # allow for int/long
             seed += user_entropy
-        return cls.from_master_secret(seed, network=network)
+        return cls.from_mnemonic(seed, network=network)
 
 
 class InvalidPathError(Exception):
-    pass
+    """
+    Raised when the provided derivation path is invalid.
+    """
 
 
 class InsufficientKeyDataError(ValueError):
-    pass
+    """
+    Exception raised when there is insufficient key data for a specific operation.
+    """
 
 
 class InvalidPrivateKeyError(ValueError):
-    pass
+    """
+    Raised when a private key is out of range.
+    """
 
 
 class InvalidPublicKeyError(ValueError):
-    pass
+    """
+    Raised when a public key is outside of the curve.
+    """
 
 
 class KeyMismatchError(ValueError):
-    pass
+    """
+    Raised when the public key and private key don't match
+    """
 
 
 class InfinityPointException(Exception):
-    pass
+    """
+    Raised when the point at infinity is encountered.
+    """
```

### Comparing `zpywallet-0.3.1/zpywallet/utils/ripemd160.py` & `zpywallet-0.4.0/zpywallet/utils/ripemd160.py`

 * *Files identical despite different names*

### Comparing `zpywallet-0.3.1/zpywallet/utils/utils.py` & `zpywallet-0.4.0/zpywallet/utils/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from functools import wraps
-import hashlib
 from hashlib import sha256
 import re
 
 import six
 
+from .ripemd160 import ripemd160
+
 if six.PY3:
     long = int
 
 
 def ensure_bytes(data):
     if not isinstance(data, six.binary_type):
         return data.encode('utf-8')
@@ -28,16 +28,15 @@
     if six.PY3:
         return bytes([num])
     return chr(num)
 
 
 def hash160(data):
     """Return ripemd160(sha256(data))"""
-    rh = hashlib.new('ripemd160', sha256(data).digest())
-    return rh.digest()
+    return ripemd160(sha256(data).digest())
 
 
 def is_hex_string(string):
     """Check if the string is only composed of hex characters."""
     pattern = re.compile(r'[A-Fa-f0-9]+')
     if isinstance(string, six.binary_type):
         string = str(string)
```

### Comparing `zpywallet-0.3.1/zpywallet.egg-info/PKG-INFO` & `zpywallet-0.4.0/zpywallet.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 Metadata-Version: 2.1
 Name: zpywallet
-Version: 0.3.1
-Summary: Simple BIP32 (HD) wallet creation for BTC, BTX, RVN, MXT, BTG, BCH, LTC, DASH, USDT, QTUM and DOGE
+Version: 0.4.0
+Summary: Simple BIP32 (HD) wallet creation for BTC, BCH, LTC, DASH, USDT (Omni) and DOGE
 Home-page: https://github.com/ZenulAbidin/pywallet
 Author: Ali Sherief
 Author-email: ali@notatether.com
 License: MIT License
-Keywords: bitcoin,wallet,litecoin,hd-wallet,dogecoin,dashcoin,bitcore,qtum,ravencoin,martexcoin,address,crypto,python
+Keywords: bitcoin,wallet,litecoin,hd-wallet,dogecoin,dashcoin,tether,address,crypto,python
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 License-File: AUTHORS
 
@@ -36,24 +31,28 @@
     :target: https://pypi.python.org/pypi/zpywallet
     :alt: PyPi version
 
 .. image:: https://img.shields.io/pypi/status/zpywallet.svg?maxAge=60
     :target: https://pypi.python.org/pypi/zpywallet
     :alt: PyPi status
 
-\
+.. image:: https://codecov.io/gh/ZenulAbidin/zpywallet/branch/master/graph/badge.svg?token=G2tC6LpTNm
+    :target: https://codecov.io/gh/ZenulAbidin/zpywallet
+    :alt: Code coverage
 
-**Simple BIP32 (HD) wallet creation for: BTC, BTX, RVN, MXT, BTG, BCH, ETH, LTC, DASH, DOGE**
+**Simple BIP32 (HD) wallet creation for: BTC, BCH, ETH, LTC, DASH, USDT (Omni), DOGE**
 
 BIP32 (or HD for "hierarchical deterministic") wallets allow you to create
 child wallets which can only generate public keys and don't expose a
 private key to an insecure server.
 
-This library simplify the process of creating new wallets for the
-BTC, BTX, RVN, MXT, BTG, BCH, ETH, LTC, DASH and DOGE cryptocurrencies.
+This library simplifies the process of creating new wallets for the
+BTC, BCH, ETH, LTC, DASH, USDT (Omni) and DOGE cryptocurrencies.
+In addition, it can also create Bitcoin Bech32 addresses for all supported
+witness versions.
 
 This is a fork of `PyWallet <https://github.com/ranaroussi/pywallet>` with support for more coins, and some bugfixes.
 
 Enjoy!
 
 --------------
 
@@ -187,14 +186,21 @@
     {
       "address": "1KpS2wC5J8bDsGShXDHD7qdGvnic1h27Db",
       "path": "m/0/394997119"
     }
 
 -----
 
+CONTRIBUTING
+============
+
+Bugfixes and enhancements are welcome. Please read CONTRIBUTING.md for contributing instructions.
+
+At the moment, I'm not accepting pull requests for new coins unless they are big and historic coins such as Tether (ERC20), BNB and XMR.
+
 IMPORTANT
 =========
 
 I **highly** recommend that you familiarize yourself with the Blockchain technology and
 be aware of security issues.
 Reading `Mastering Bitcoin <https://github.com/bitcoinbook/bitcoinbook>`_ and going over
 Steven Buss's security notes on the `Bitmerchant repository <https://github.com/sbuss/bitmerchant>`_
```

