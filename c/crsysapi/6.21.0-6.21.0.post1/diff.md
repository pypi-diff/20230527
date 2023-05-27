# Comparing `tmp/crsysapi-6.21.0.zip` & `tmp/crsysapi-6.21.0.post1.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 31776 bytes, number of entries: 15
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-24 16:43 crsysapi-6.21.0/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-24 16:43 crsysapi-6.21.0/crsysapi.egg-info/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-24 16:43 crsysapi-6.21.0/test/
--rw-rw-rw-  2.0 fat      247 b- defN 23-May-18 13:36 crsysapi-6.21.0/CHANGELOG.rst
--rw-rw-rw-  2.0 fat    64787 b- defN 23-May-24 16:39 crsysapi-6.21.0/crsysapi.py
--rw-rw-rw-  2.0 fat       66 b- defN 23-May-21 16:41 crsysapi-6.21.0/MANIFEST.in
--rw-rw-rw-  2.0 fat     4031 b- defN 23-May-24 16:43 crsysapi-6.21.0/PKG-INFO
--rw-rw-rw-  2.0 fat     2818 b- defN 23-May-21 16:09 crsysapi-6.21.0/README.rst
--rw-rw-rw-  2.0 fat      113 b- defN 23-May-24 16:43 crsysapi-6.21.0/setup.cfg
--rw-rw-rw-  2.0 fat      555 b- defN 23-May-24 16:43 crsysapi-6.21.0/setup.py
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-24 16:43 crsysapi-6.21.0/crsysapi.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat     4031 b- defN 23-May-24 16:43 crsysapi-6.21.0/crsysapi.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat      217 b- defN 23-May-24 16:43 crsysapi-6.21.0/crsysapi.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-24 16:43 crsysapi-6.21.0/crsysapi.egg-info/top_level.txt
--rw-rw-rw-  2.0 fat    53453 b- defN 23-May-24 16:40 crsysapi-6.21.0/test/test_crsysapi.py
-15 files, 130328 bytes uncompressed, 29658 bytes compressed:  77.2%
+Zip file size: 32526 bytes, number of entries: 15
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-27 17:36 crsysapi-6.21.0.post1/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-27 17:36 crsysapi-6.21.0.post1/crsysapi.egg-info/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-27 17:36 crsysapi-6.21.0.post1/test/
+-rw-rw-rw-  2.0 fat      247 b- defN 23-May-27 15:08 crsysapi-6.21.0.post1/CHANGELOG.rst
+-rw-rw-rw-  2.0 fat    64805 b- defN 23-May-27 17:33 crsysapi-6.21.0.post1/crsysapi.py
+-rw-rw-rw-  2.0 fat       66 b- defN 23-May-21 16:41 crsysapi-6.21.0.post1/MANIFEST.in
+-rw-rw-rw-  2.0 fat     4037 b- defN 23-May-27 17:36 crsysapi-6.21.0.post1/PKG-INFO
+-rw-rw-rw-  2.0 fat     2818 b- defN 23-May-21 16:09 crsysapi-6.21.0.post1/README.rst
+-rw-rw-rw-  2.0 fat      113 b- defN 23-May-27 17:36 crsysapi-6.21.0.post1/setup.cfg
+-rw-rw-rw-  2.0 fat      561 b- defN 23-May-27 17:36 crsysapi-6.21.0.post1/setup.py
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-27 17:36 crsysapi-6.21.0.post1/crsysapi.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat     4037 b- defN 23-May-27 17:36 crsysapi-6.21.0.post1/crsysapi.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat      217 b- defN 23-May-27 17:36 crsysapi-6.21.0.post1/crsysapi.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-27 17:36 crsysapi-6.21.0.post1/crsysapi.egg-info/top_level.txt
+-rw-rw-rw-  2.0 fat    55773 b- defN 23-May-25 22:19 crsysapi-6.21.0.post1/test/test_crsysapi.py
+15 files, 132684 bytes uncompressed, 30228 bytes compressed:  77.2%
```

## zipnote {}

```diff
@@ -1,46 +1,46 @@
-Filename: crsysapi-6.21.0/
+Filename: crsysapi-6.21.0.post1/
 Comment: 
 
-Filename: crsysapi-6.21.0/crsysapi.egg-info/
+Filename: crsysapi-6.21.0.post1/crsysapi.egg-info/
 Comment: 
 
-Filename: crsysapi-6.21.0/test/
+Filename: crsysapi-6.21.0.post1/test/
 Comment: 
 
-Filename: crsysapi-6.21.0/CHANGELOG.rst
+Filename: crsysapi-6.21.0.post1/CHANGELOG.rst
 Comment: 
 
-Filename: crsysapi-6.21.0/crsysapi.py
+Filename: crsysapi-6.21.0.post1/crsysapi.py
 Comment: 
 
-Filename: crsysapi-6.21.0/MANIFEST.in
+Filename: crsysapi-6.21.0.post1/MANIFEST.in
 Comment: 
 
-Filename: crsysapi-6.21.0/PKG-INFO
+Filename: crsysapi-6.21.0.post1/PKG-INFO
 Comment: 
 
-Filename: crsysapi-6.21.0/README.rst
+Filename: crsysapi-6.21.0.post1/README.rst
 Comment: 
 
-Filename: crsysapi-6.21.0/setup.cfg
+Filename: crsysapi-6.21.0.post1/setup.cfg
 Comment: 
 
-Filename: crsysapi-6.21.0/setup.py
+Filename: crsysapi-6.21.0.post1/setup.py
 Comment: 
 
-Filename: crsysapi-6.21.0/crsysapi.egg-info/dependency_links.txt
+Filename: crsysapi-6.21.0.post1/crsysapi.egg-info/dependency_links.txt
 Comment: 
 
-Filename: crsysapi-6.21.0/crsysapi.egg-info/PKG-INFO
+Filename: crsysapi-6.21.0.post1/crsysapi.egg-info/PKG-INFO
 Comment: 
 
-Filename: crsysapi-6.21.0/crsysapi.egg-info/SOURCES.txt
+Filename: crsysapi-6.21.0.post1/crsysapi.egg-info/SOURCES.txt
 Comment: 
 
-Filename: crsysapi-6.21.0/crsysapi.egg-info/top_level.txt
+Filename: crsysapi-6.21.0.post1/crsysapi.egg-info/top_level.txt
 Comment: 
 
-Filename: crsysapi-6.21.0/test/test_crsysapi.py
+Filename: crsysapi-6.21.0.post1/test/test_crsysapi.py
 Comment: 
 
 Zip file comment:
```

## Comparing `crsysapi-6.21.0/crsysapi.py` & `crsysapi-6.21.0.post1/crsysapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! python3
 # -*- coding: utf-8 -*-
 
 # A Python interface to CryptoSys API
 
 # crsysapi.py
-# $Date: 2023-05-17 12:19:00 $
+# $Date: 2023-05-27 09:31:00 $
 # ************************** LICENSE *****************************************
 # Copyright (C) 2023 David Ireland, DI Management Services Pty Limited.
 # <www.di-mgt.com.au> <www.cryptosys.net>
 # This code is provided 'as-is' without any express or implied warranty.
 # Free license is hereby granted to use this code as part of an application
 # provided this license notice is left intact. You are *not* licensed to
 # share any of this code in any form of mass distribution, including, but not
@@ -17,15 +17,15 @@
 
 # Requires `CryptoSys API` to be installed on your system,
 # available from <https://www.cryptosys.net/api.html>.
 
 import platform
 from ctypes import create_string_buffer, c_char_p, c_void_p, c_int, c_wchar_p
 
-__version__ = "6.21.0.0000"
+__version__ = "6.21.0.0001"
 # History:
 # [6.21.0] Updated for changes in CryptoSys API 6.21
 # [6.20.0] First Python interface to CryptoSys API 6.20
 
 
 # OUR EXPORTED CLASSES
 __all__ = (
@@ -759,15 +759,15 @@
         """
         noptions = int(alg)
         if iv is None:
             ivlen = 0
             iv = b''
         else:
             ivlen = len(iv)
-        r = _didll.CIPHER_StreamFile(fileout, filein, bytes(key), len(key), bytes(iv), ivlen, counter, noptions)
+        r = _didll.CIPHER_StreamFile(fileout.encode(), filein.encode(), bytes(key), len(key), bytes(iv), ivlen, counter, noptions)
         if (r != 0): raise Error(-r if r < 0 else r)
         return r
 
 
 class Blowfish:
     """Blowfish cipher algorithm (Schneier, 1993)."""
```

## Comparing `crsysapi-6.21.0/PKG-INFO` & `crsysapi-6.21.0.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: crsysapi
-Version: 6.21.0
+Version: 6.21.0.post1
 Summary: Python interface to CryptoSys API
 Home-page: https://www.cryptosys.net/api.html
 Author: David Ireland
 Author-email: UNKNOWN
 License: See source code modules
 Description: Python for CryptoSys API
         ===================================
@@ -78,15 +78,15 @@
         | <https://www.di-mgt.com.au> <https://www.cryptosys.net>
         | 18 May 2023
         
         
         Revision History
         -----------------
         
-        6.21.0 (2023-05-18)
+        6.21.0 (2023-05-27)
         ^^^^^^^^^^^^^^^^^^^
         
         * Changes to match main core module version 6.21.
         
         
         6.20.0 (2023-04-09)
         ^^^^^^^^^^^^^^^^^^^
```

## Comparing `crsysapi-6.21.0/README.rst` & `crsysapi-6.21.0.post1/README.rst`

 * *Files identical despite different names*

## Comparing `crsysapi-6.21.0/setup.py` & `crsysapi-6.21.0.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 readme = read('README.rst')
 changelog = read('CHANGELOG.rst')
 
 setup(name='crsysapi',
-      version='6.21.0',
+      version='6.21.0.post1',
       description='Python interface to CryptoSys API',
       long_description=readme + '\n\n' + changelog,
       author='David Ireland',
       url='https://www.cryptosys.net/api.html',
       platforms=['Windows'],
       py_modules=['crsysapi'],
       license='See source code modules'
```

## Comparing `crsysapi-6.21.0/crsysapi.egg-info/PKG-INFO` & `crsysapi-6.21.0.post1/crsysapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: crsysapi
-Version: 6.21.0
+Version: 6.21.0.post1
 Summary: Python interface to CryptoSys API
 Home-page: https://www.cryptosys.net/api.html
 Author: David Ireland
 Author-email: UNKNOWN
 License: See source code modules
 Description: Python for CryptoSys API
         ===================================
@@ -78,15 +78,15 @@
         | <https://www.di-mgt.com.au> <https://www.cryptosys.net>
         | 18 May 2023
         
         
         Revision History
         -----------------
         
-        6.21.0 (2023-05-18)
+        6.21.0 (2023-05-27)
         ^^^^^^^^^^^^^^^^^^^
         
         * Changes to match main core module version 6.21.
         
         
         6.20.0 (2023-04-09)
         ^^^^^^^^^^^^^^^^^^^
```

## Comparing `crsysapi-6.21.0/test/test_crsysapi.py` & `crsysapi-6.21.0.post1/test/test_crsysapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! python3
 # -*- coding: utf-8 -*-
 
 """Some tests for ``crsysapi.py`` the Python interface to CryptoSys API"""
 
-# test_crsysapi.py: version 6.20.0
-# $Date: 2023-05-21 04:43:00 $
+# test_crsysapi.py: version 6.21.0
+# $Date: 2023-05-25 14:19:00 $
 
 # ************************** LICENSE *****************************************
 # Copyright (C) 2023 David Ireland, DI Management Services Pty Limited.
 # All rights reserved. <www.di-mgt.com.au> <www.cryptosys.net>
 # The code in this module is licensed under the terms of the MIT license.
 # For a copy, see <http://opensource.org/licenses/MIT>
 # ****************************************************************************
@@ -259,14 +259,30 @@
     print("OK:", okhex)
     assert cthex == okhex, "crsysapi.Cipher.encrypt_hex failed"
     # Decrypt using flags instead of alg string - this time we don't need the IV argument
     p1hex = crsysapi.Cipher.decrypt_hex(cthex, keyhex, None, alg=crsysapi.Cipher.Alg.AES128, mode=crsysapi.Cipher.Mode.CBC, pad=crsysapi.Cipher.Pad.ONEANDZEROES, opts=crsysapi.Cipher.Opts.PREFIXIV)
     print("P':", p1hex)
     assert(p1hex == pthex)
 
+    # Test in ECB mode
+    # SP 800-38A F.1.3 ECB-AES192.Encrypt
+    keyhex = "8e73b0f7da0e6452c810f32b809079e562f8ead2522c6b7b"
+    pthex = "6bc1bee22e409f96e93d7e117393172aae2d8a571e03ac9c9eb76fac45af8e51" \
+            + "30c81c46a35ce411e5fbc1191a0a52eff69f2445df4f9b17ad2b417be66c3710"
+    okhex = "bd334f1d6e45f25ff712a214571fa5cc974104846d0ad3ad7734ecb3ecee4eef" \
+            + "ef7afd2270e2e60adce0ba2face6444e9a4b41ba738d6c72fb16691603c18e0e"
+    print("PT:", pthex)
+    cthex = crsysapi.Cipher.encrypt_hex(pthex, keyhex, algmodepad="Aes192-ECB-Nopad").lower()
+    print("CT:", cthex)
+    print("OK:", okhex)
+    assert cthex == okhex, "crsysapi.Cipher.encrypt_hex failed"
+    p1hex = crsysapi.Cipher.decrypt_hex(cthex, keyhex, alg=crsysapi.Cipher.Alg.AES192, pad=crsysapi.Cipher.Pad.NOPAD).lower()
+    print("P':", p1hex)
+    assert(p1hex == pthex)
+
 
 def test_cipher_file():
     print("\nTEST CIPHER FILE FUNCTIONS...")
     file_pt = "hello.txt"
     write_text_file(file_pt, "hello world\r\n")
     print(file_pt + ":",)
     _print_file_hex(file_pt)
@@ -346,17 +362,17 @@
         ct, key, iv, alg=crsysapi.Cipher.Alg.AES128, mode=crsysapi.Cipher.Mode.CBC)
     print("P1:", crsysapi.Cnv.tohex(p1))
     print("P1:", p1)
 
     # Using defaults (TDEA/ECB)
     key = crsysapi.Rng.bytestring(crsysapi.Cipher.keybytes(crsysapi.Cipher.Alg.TDEA))
     print("KY:", crsysapi.Cnv.tohex(key))
-    ct = crsysapi.Cipher.encrypt_block(pt, key, iv)
+    ct = crsysapi.Cipher.encrypt_block(pt, key)
     print("CT:", crsysapi.Cnv.tohex(ct))
-    p1 = crsysapi.Cipher.decrypt_block(ct, key, iv)
+    p1 = crsysapi.Cipher.decrypt_block(ct, key)
     print("P1:", crsysapi.Cnv.tohex(p1))
     print("P1:", p1)
 
 
 def test_blowfish():
     print("\nTEST BLOWFISH CIPHER...")
     key = crsysapi.Cnv.fromhex("0123456789ABCDEFF0E1D2C3B4A59687")
@@ -619,14 +635,17 @@
     print("data:", datahex)
     h = crsysapi.Mac.hex_from_hex(datahex, keyhex)
     print("HMAC-SHA-1:", h)
     assert(h == "b617318655057264e28bc0b6fb378c8ef146be00")
     h = crsysapi.Mac.hex_from_hex(datahex, keyhex, crsysapi.Mac.Alg.HMAC_SHA256)
     print("HMAC-SHA-256:", h)
     assert(h == "b0344c61d8db38535ca8afceaf0bf12b881dc200c9833da726e9376c2e32cff7")
+    # HMAC hex <-- string
+    h = crsysapi.Mac.hex_from_string("Hi There", crsysapi.Cnv.fromhex(keyhex), crsysapi.Mac.Alg.HMAC_SHA1)
+    print("HMAC-SHA-1:", h)
 
     print("\nTESTING Mac(SHA-3)...")
     print("NIST HMAC_SHA3-256.pdf Sample #1")
     key = crsysapi.Cnv.fromhex('000102030405060708090A0B0C0D0E0F101112131415161718191A1B1C1D1E1F')
     print("key: ", crsysapi.Cnv.tohex(key))
     data = b'Sample message for keylen<blocklen'
     print("data:", data.decode())
@@ -912,14 +931,23 @@
     print("CT =", crsysapi.Cnv.tohex(ct))
     print("OK =", okhex)
     assert (okhex.lower() == crsysapi.Cnv.tohex(ct).lower())
     # Repeat to decrypt
     dt = crsysapi.CipherStream.bytes(ct, key, None, crsysapi.CipherStream.Alg.ARCFOUR)
     print("DT =", crsysapi.Cnv.tohex(dt))
     assert (pt == dt)
+    # Create and encrypt a file
+    ptfile = "arcfour.dat"
+    encfile = "arcfour.enc"
+    write_binary_file(ptfile, crsysapi.Cnv.fromhex("0123456789abcdef"))
+    r = crsysapi.CipherStream.file(encfile, ptfile, key, b'', crsysapi.CipherStream.Alg.ARCFOUR)
+    print("CipherStream.file returns ", r, "(expected 0)")
+    ct = read_binary_file(encfile)
+    print("CT =", crsysapi.Cnv.tohex(ct))
+    print("OK =", okhex)
 
     print("Using Salsa20...")
     # Set 6, vector#  0:
     key = crsysapi.Cnv.fromhex("0053A6F94C9FF24598EB3E91E4378ADD")
     iv = crsysapi.Cnv.fromhex("0D74DB42A91077DE")
     pt = b'\x00' * 64
     okhex = "05E1E7BEB697D999656BF37C1B978806735D0B903A6007BD329927EFBE1B0E2A8137C1AE291493AA83A821755BEE0B06CD14855A67E46703EBF8F3114B584CBA"
@@ -976,14 +1004,25 @@
     wk = crsysapi.Cipher.key_wrap(keydata, kek, crsysapi.Cipher.Alg.AES256)
     print("WK(AES-256) =", crsysapi.Cnv.tohex(wk))
     print("OK          =", "EAFB901F82B98D37F17497063DE3E5EC7246AB57200AE73EDDDDF24AA403DAFA0C5AE151D1746FA4")
     # Reverse
     kd = crsysapi.Cipher.key_unwrap(wk, kek, crsysapi.Cipher.Alg.AES256)
     print("KD'         =", crsysapi.Cnv.tohex(kd))
 
+    keydata = crsysapi.Cnv.fromhex("84E7F2D878F89FCCCD2D5EBAFC56DAF73300F27EF771CD68")
+    kek = crsysapi.Cnv.fromhex("8AD8274E56F467738EDD83D4394E5E29AF7C4089E4F8D9F4")
+    print("KD          =", crsysapi.Cnv.tohex(keydata))
+    print("KEK         =", crsysapi.Cnv.tohex(kek))
+    wk = crsysapi.Cipher.key_wrap(keydata, kek, crsysapi.Cipher.Alg.TDEA)
+    print("WK(3DES)    =", crsysapi.Cnv.tohex(wk))
+    # NOTE: output for Triple DES key wrap is different each time
+    # Reverse
+    kd = crsysapi.Cipher.key_unwrap(wk, kek, crsysapi.Cipher.Alg.TDEA)
+    print("KD'         =", crsysapi.Cnv.tohex(kd))
+
 
 def test_ascon_aead():
     print("\nTEST ASCON AEAD...")
     # Ref: ascon128v12/LWC_AEAD_KAT_128_128.txt, Count = 303
     key = crsysapi.Cnv.fromhex("000102030405060708090A0B0C0D0E0F")
     nonce = crsysapi.Cnv.fromhex("000102030405060708090A0B0C0D0E0F")
     pt = crsysapi.Cnv.fromhex("000102030405060708")
@@ -1080,14 +1119,18 @@
 
 def test_xof_mgf1():
     print("\nTEST XOF MGF1...")
     msg = crsysapi.Cnv.fromhex("012345ff")
     md = crsysapi.Xof.bytes(24, msg, crsysapi.Xof.Alg.MGF1_SHA1)
     print("MD(mgf1_sha1) =", crsysapi.Cnv.tohex(md))
     assert(crsysapi.Cnv.tohex(md) == "242FB2E7A338AE07E580047F82B7ACFF83A41EC5D8FF9BAB")
+    # MGF1-SHA-1 of empty string
+    md = crsysapi.Xof.bytes(24, b'', crsysapi.Xof.Alg.MGF1_SHA1)
+    print("MD(mgf1_sha1) =", crsysapi.Cnv.tohex(md))
+    assert(crsysapi.Cnv.tohex(md) == "9069CA78E7450A285173431B3E52C5C25299E473479E04F3")
     # Example from SPHINCS+ submission October 2020
     msg = crsysapi.Cnv.fromhex("3b5c056af3ebba70d4c805380420585562b32410a778f558ff951252407647e3")
     md = crsysapi.Xof.bytes(34, msg, crsysapi.Xof.Alg.MGF1_SHA256)
     print("MD(mgf1_sha256) =", crsysapi.Cnv.tohex(md))
     assert(crsysapi.Cnv.tohex(md) == "5B7EB772AECF04C74AF07D9D9C1C1F8D3A90DCDA00D5BAB1DC28DAECDC86EB87611E")
     md = crsysapi.Xof.bytes(34, msg, crsysapi.Xof.Alg.MGF1_SHA512)
     print("MD(mgf1_sha512) =", crsysapi.Cnv.tohex(md))
@@ -1195,19 +1238,19 @@
         # test_xof()
         # test_wipe()
         # test_compress()
         # test_blowfish()
         # test_pbe()
         # test_aead()
         # test_cipherstream()
-        test_keywrap()
+        # test_keywrap()
         # test_ascon_aead()
         # test_ascon_hash()
         # test_ascon_xof()
-        # test_xof_mgf1()
+        test_xof_mgf1()
         # test_shortpathname()
 
     reset_start_dir()
     quick_version()
     print("crsysapi.__version__=", crsysapi.__version__)
     print("ALL DONE.")
```

