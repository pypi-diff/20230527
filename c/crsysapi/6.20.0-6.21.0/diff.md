# Comparing `tmp/crsysapi-6.20.0.zip` & `tmp/crsysapi-6.21.0.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 27191 bytes, number of entries: 15
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-09 18:33 crsysapi-6.20.0/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-09 18:33 crsysapi-6.20.0/crsysapi.egg-info/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-09 18:33 crsysapi-6.20.0/test/
--rw-rw-rw-  2.0 fat      154 b- defN 23-Apr-09 18:19 crsysapi-6.20.0/CHANGELOG.rst
--rw-rw-rw-  2.0 fat    59723 b- defN 23-Apr-09 16:37 crsysapi-6.20.0/crsysapi.py
--rw-rw-rw-  2.0 fat       67 b- defN 23-Apr-09 17:05 crsysapi-6.20.0/MANIFEST.in
--rw-rw-rw-  2.0 fat     3408 b- defN 23-Apr-09 18:33 crsysapi-6.20.0/PKG-INFO
--rw-rw-rw-  2.0 fat     2390 b- defN 23-Apr-09 18:32 crsysapi-6.20.0/README.rst
--rw-rw-rw-  2.0 fat      113 b- defN 23-Apr-09 18:33 crsysapi-6.20.0/setup.cfg
--rw-rw-rw-  2.0 fat      547 b- defN 23-Apr-09 17:06 crsysapi-6.20.0/setup.py
--rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-09 18:33 crsysapi-6.20.0/crsysapi.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat     3408 b- defN 23-Apr-09 18:33 crsysapi-6.20.0/crsysapi.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat      217 b- defN 23-Apr-09 18:33 crsysapi-6.20.0/crsysapi.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-09 18:33 crsysapi-6.20.0/crsysapi.egg-info/top_level.txt
--rw-rw-rw-  2.0 fat    41705 b- defN 23-Apr-09 16:37 crsysapi-6.20.0/test/test_crsysapi.py
-15 files, 111742 bytes uncompressed, 25073 bytes compressed:  77.6%
+Zip file size: 31776 bytes, number of entries: 15
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-24 16:43 crsysapi-6.21.0/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-24 16:43 crsysapi-6.21.0/crsysapi.egg-info/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-24 16:43 crsysapi-6.21.0/test/
+-rw-rw-rw-  2.0 fat      247 b- defN 23-May-18 13:36 crsysapi-6.21.0/CHANGELOG.rst
+-rw-rw-rw-  2.0 fat    64787 b- defN 23-May-24 16:39 crsysapi-6.21.0/crsysapi.py
+-rw-rw-rw-  2.0 fat       66 b- defN 23-May-21 16:41 crsysapi-6.21.0/MANIFEST.in
+-rw-rw-rw-  2.0 fat     4031 b- defN 23-May-24 16:43 crsysapi-6.21.0/PKG-INFO
+-rw-rw-rw-  2.0 fat     2818 b- defN 23-May-21 16:09 crsysapi-6.21.0/README.rst
+-rw-rw-rw-  2.0 fat      113 b- defN 23-May-24 16:43 crsysapi-6.21.0/setup.cfg
+-rw-rw-rw-  2.0 fat      555 b- defN 23-May-24 16:43 crsysapi-6.21.0/setup.py
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-24 16:43 crsysapi-6.21.0/crsysapi.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat     4031 b- defN 23-May-24 16:43 crsysapi-6.21.0/crsysapi.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat      217 b- defN 23-May-24 16:43 crsysapi-6.21.0/crsysapi.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-24 16:43 crsysapi-6.21.0/crsysapi.egg-info/top_level.txt
+-rw-rw-rw-  2.0 fat    53453 b- defN 23-May-24 16:40 crsysapi-6.21.0/test/test_crsysapi.py
+15 files, 130328 bytes uncompressed, 29658 bytes compressed:  77.2%
```

## zipnote {}

```diff
@@ -1,46 +1,46 @@
-Filename: crsysapi-6.20.0/
+Filename: crsysapi-6.21.0/
 Comment: 
 
-Filename: crsysapi-6.20.0/crsysapi.egg-info/
+Filename: crsysapi-6.21.0/crsysapi.egg-info/
 Comment: 
 
-Filename: crsysapi-6.20.0/test/
+Filename: crsysapi-6.21.0/test/
 Comment: 
 
-Filename: crsysapi-6.20.0/CHANGELOG.rst
+Filename: crsysapi-6.21.0/CHANGELOG.rst
 Comment: 
 
-Filename: crsysapi-6.20.0/crsysapi.py
+Filename: crsysapi-6.21.0/crsysapi.py
 Comment: 
 
-Filename: crsysapi-6.20.0/MANIFEST.in
+Filename: crsysapi-6.21.0/MANIFEST.in
 Comment: 
 
-Filename: crsysapi-6.20.0/PKG-INFO
+Filename: crsysapi-6.21.0/PKG-INFO
 Comment: 
 
-Filename: crsysapi-6.20.0/README.rst
+Filename: crsysapi-6.21.0/README.rst
 Comment: 
 
-Filename: crsysapi-6.20.0/setup.cfg
+Filename: crsysapi-6.21.0/setup.cfg
 Comment: 
 
-Filename: crsysapi-6.20.0/setup.py
+Filename: crsysapi-6.21.0/setup.py
 Comment: 
 
-Filename: crsysapi-6.20.0/crsysapi.egg-info/dependency_links.txt
+Filename: crsysapi-6.21.0/crsysapi.egg-info/dependency_links.txt
 Comment: 
 
-Filename: crsysapi-6.20.0/crsysapi.egg-info/PKG-INFO
+Filename: crsysapi-6.21.0/crsysapi.egg-info/PKG-INFO
 Comment: 
 
-Filename: crsysapi-6.20.0/crsysapi.egg-info/SOURCES.txt
+Filename: crsysapi-6.21.0/crsysapi.egg-info/SOURCES.txt
 Comment: 
 
-Filename: crsysapi-6.20.0/crsysapi.egg-info/top_level.txt
+Filename: crsysapi-6.21.0/crsysapi.egg-info/top_level.txt
 Comment: 
 
-Filename: crsysapi-6.20.0/test/test_crsysapi.py
+Filename: crsysapi-6.21.0/test/test_crsysapi.py
 Comment: 
 
 Zip file comment:
```

## Comparing `crsysapi-6.20.0/crsysapi.py` & `crsysapi-6.21.0/crsysapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 #! python3
 # -*- coding: utf-8 -*-
 
-"""A Python interface to CryptoSys API <https://www.cryptosys.net/>."""
+# A Python interface to CryptoSys API
 
 # crsysapi.py
-# $Date: 2023-04-09 08:37:00 $
+# $Date: 2023-05-17 12:19:00 $
 # ************************** LICENSE *****************************************
 # Copyright (C) 2023 David Ireland, DI Management Services Pty Limited.
 # <www.di-mgt.com.au> <www.cryptosys.net>
 # This code is provided 'as-is' without any express or implied warranty.
 # Free license is hereby granted to use this code as part of an application
 # provided this license notice is left intact. You are *not* licensed to
 # share any of this code in any form of mass distribution, including, but not
 # limited to, reposting on other websites or in any source code repository.
 # ****************************************************************************
 
 # Requires `CryptoSys API` to be installed on your system,
-# available from <https://www.cryptosys.net/>.
+# available from <https://www.cryptosys.net/api.html>.
 
 import platform
 from ctypes import create_string_buffer, c_char_p, c_void_p, c_int, c_wchar_p
 
-__version__ = "6.20.0.0000"
+__version__ = "6.21.0.0000"
 # History:
+# [6.21.0] Updated for changes in CryptoSys API 6.21
 # [6.20.0] First Python interface to CryptoSys API 6.20
 
 
 # OUR EXPORTED CLASSES
 __all__ = (
     'Error',
-    'Gen', 'Aead', 'Cipher', 'CipherStream', 'Cnv', 'Crc', 'Compr',
+    'Gen', 'Aead', 'Blowfish', 'Cipher', 'CipherStream', 'Cnv', 'Crc', 'Compr',
     'Hash', 'Mac', 'Pbe', 'Prf', 'Rng', 'Wipe', 'Xof',
 )
 
 # Our global DLL/solibrary object for CryptoSys API
 if platform.system() == 'Windows':
     from ctypes import windll
     _didll = windll.diCryptoSys
@@ -99,20 +100,27 @@
         """Return full path name of the current process's DLL module."""
         nchars = _didll.API_ModuleName(None, 0, 0)
         buf = create_string_buffer(nchars + 1)
         nchars = _didll.API_ModuleName(buf, nchars, 0)
         return buf.value.decode()
 
     @staticmethod
+    def module_info():
+        """Get additional information about the core DLL module."""
+        nchars = _didll.API_ModuleInfo(None, 0, 0)
+        buf = create_string_buffer(nchars + 1)
+        nchars = _didll.API_ModuleInfo(buf, nchars, 0)
+        return buf.value.decode()
+
+    @staticmethod
     def core_platform():
         """Return the platform the core DLL was compiled for ('Win32' or 'X64')."""
-        _GEN_MODULE = 0x40
         nchars = 5
         buf = create_string_buffer(nchars + 1)
-        nchars = _didll.API_ModuleName(buf, nchars, _GEN_MODULE)
+        nchars = _didll.API_Platform(buf, nchars)
         return buf.value.decode()[:nchars]
 
     @staticmethod
     def licence_type():
         """Return licence type: "D"=Developer "T"=Trial."""
         n = _didll.API_LicenceType(0)
         return chr(n)
@@ -142,14 +150,16 @@
     """Authenticated encryption with Additional Data (AEAD) functions."""
 
     class AeadAlg:
         """AEAD algorithm options."""
         AES_128_GCM = 1  #: AEAD_AES_128_GCM authenticated encryption algorithm (RFC 5116)
         AES_256_GCM = 2  #: AEAD_AES_256_GCM authenticated encryption algorithm (RFC 5116)
         CHACHA20_POLY1305 = 29  #: AEAD_CHACHA20_POLY1305 authenticated encryption algorithm (RFC 7539)
+        AEAD_ASCON_128 = 0x1a  #: ASCON-128 authentication scheme (provisional)
+        AEAD_ASCON_128A = 0x1b  #: ASCON-128A authentication scheme (provisional)
 
     class Opts:
         """Advanced options."""
         DEFAULT = 0  #: Use default options
         PREFIXIV = 0x1000  #: Prepend the IV before the ciphertext in the output
 
     @staticmethod
@@ -209,19 +219,17 @@
             ivlen = len(iv)
         if aad is None:
             aadlen = 0
             aad = b''
         else:
             aadlen = len(aad)
         n = _didll.AEAD_DecryptWithTag(None, 0, bytes(input), len(input), bytes(key), len(key), bytes(iv), ivlen, bytes(aad), aadlen, noptions)
-        print(f"AEAD_DecryptWithTag returns {n}")
         if (n < 0): raise Error(-n)
         buf = create_string_buffer(n)
         n = _didll.AEAD_DecryptWithTag(buf, n, bytes(input), len(input), bytes(key), len(key), bytes(iv), ivlen, bytes(aad), aadlen, noptions)
-        print(f"AEAD_DecryptWithTag returns {n}")
         return bytes(buf.raw)
 
 
 class Cipher:
     """Generic block cipher functions."""
     # CONSTANTS
     class Alg:
@@ -552,14 +560,57 @@
         else:
             ivlen = len(iv)
         n = _didll.CIPHER_FileDecrypt(fileout.encode(), filein.encode(), bytes(key), len(key), bytes(iv), ivlen, algmodepad.encode(), noptions)
         if (n != 0): raise Error(-n)
         return n
 
     @staticmethod
+    def key_wrap(data, kek, alg):
+        """
+        Wrap (encrypt) key material with a key-encryption key.
+
+        Args:
+            data (bytes): Input key material to be encrypted
+            kek (bytes): Key encryption key
+            alg (Cipher.Alg): Cipher algorithm
+
+        Returns:
+            bytes: Wrapped key in byte array.
+        """
+        noptions = alg
+        n = _didll.CIPHER_KeyWrap(None, 0, bytes(data), len(data), bytes(kek), len(kek), noptions)
+        if (n < 0): raise Error(-n)
+        buf = create_string_buffer(n)
+        n = _didll.CIPHER_KeyWrap(buf, n, bytes(data), len(data), bytes(kek), len(kek), noptions)
+        if (n < 0): raise Error(-n)
+        return bytearray(buf.raw)
+
+    @staticmethod
+    def key_unwrap(data, kek, alg):
+        """
+        Unwrap (decrypt) key material with a key-encryption key.
+
+        Args:
+            data (bytes): Wrapped key
+            kek (bytes): Key encryption key
+            alg (Cipher.Alg): Cipher algorithm
+
+        Returns:
+            bytes: Unwrapped key material in byte array.
+        """
+        noptions = alg
+        n = _didll.CIPHER_KeyUnwrap(None, 0, bytes(data), len(data), bytes(kek), len(kek), noptions)
+        if (n < 0): raise Error(-n)
+        buf = create_string_buffer(n)
+        n = _didll.CIPHER_KeyUnwrap(buf, n, bytes(data), len(data), bytes(kek), len(kek), noptions)
+        if (n < 0): raise Error(-n)
+        return bytearray(buf.raw)
+
+
+    @staticmethod
     def pad(data, alg, pad=Pad.PKCS5):
         # HINT: Repeat signature as first line of docstring to get "pad=Pad.PKCS5" not "pad=131072"
         # http://www.sphinx-doc.org/en/stable/ext/autodoc.html#confval-autodoc_docstring_signature
         """pad(data, alg, pad=Pad.PKCS5)
         Pad byte array to correct length for ECB and CBC encryption.
 
         Args:
@@ -665,15 +716,15 @@
             iv (bytes): Initialization Vector (IV, nonce) or None for Arcfour.
             alg (CipherStream.Alg): Stream cipher algorithm.
             counter (int): Counter value for ChaCha20 only, otherwise ignored.
 
         Returns:
             bytes: Ciphertext in a byte array.
 
-        Remarks:
+        Note:
             - **Arcfour:** any length key; no IV.
             - **Salsa20:** key must be exactly 16 or 32 bytes and IV exactly 8 bytes long.
             - **ChaCha20:** key must be exactly 16 or 32 bytes and IV exactly 8, 12, or 16 bytes long. Counter is ignored if IV is 16 bytes.
         """
         noptions = int(alg)
         if iv is None:
             ivlen = 0
@@ -697,15 +748,15 @@
             iv (bytes): Initialization Vector (IV, nonce) or None for Arcfour.
             alg (CipherStream.Alg): Stream cipher algorithm.
             counter (int): Counter value for ChaCha20 only, otherwise ignored.
 
         Returns:
             int: 0 if successful.
 
-        Remarks:
+        Note:
             - **Arcfour:** any length key; no IV.
             - **Salsa20:** key must be exactly 16 or 32 bytes and IV exactly 8 bytes long.
             - **ChaCha20:** key must be exactly 16 or 32 bytes and IV exactly 8, 12, or 16 bytes long. Counter is ignored if IV is 16 bytes.
         """
         noptions = int(alg)
         if iv is None:
             ivlen = 0
@@ -714,28 +765,28 @@
             ivlen = len(iv)
         r = _didll.CIPHER_StreamFile(fileout, filein, bytes(key), len(key), bytes(iv), ivlen, counter, noptions)
         if (r != 0): raise Error(-r if r < 0 else r)
         return r
 
 
 class Blowfish:
-    """Blowfish cipher algorithm."""
+    """Blowfish cipher algorithm (Schneier, 1993)."""
 
     # Local constants
     __ENCRYPT = 1
     __DECRYPT = 0
 
     @staticmethod
     def encrypt_block(data, key, modestr="ECB", iv=None):
         """Encrypt a block of data. Must be an exact multiple of 8 bytes.
 
         Args:
             data (bytes): Input data to be encrypted
             key (bytes): Key of length between 1 and 56 bytes (448 bits)
-            modestr (str): Cipher mode {"[ECB]"|"CBC"|"CFB"|'OFB'|"CTR'}
+            modestr (str): Cipher mode {"[ECB]"|"CBC"|"CFB"|"OFB"|"CTR"}
             iv (bytes): Initialization Vector (IV) of exactly 8 bytes or ``None`` for ECB mode
 
         Returns:
             bytes: Ciphertext in byte array or empty array on error.
             Output is always the same length as the input.
         """
         if iv is None:
@@ -750,15 +801,15 @@
     @staticmethod
     def decrypt_block(data, key, modestr="ECB", iv=None):
         """Decrypt a block of data. Must be an exact multiple of 8 bytes.
 
         Args:
             data (bytes): Input data to be decrypted
             key (bytes): Key of length between 1 and 56 bytes (448 bits)
-            modestr (str): Cipher mode {"[ECB]"|"CBC"|"CFB"|'OFB'|"CTR'}
+            modestr (str): Cipher mode {"[ECB]"|"CBC"|"CFB"|"OFB"|"CTR"}
             iv (bytes): Initialization Vector (IV) of exactly 8 bytes or ``None`` for ECB mode
 
         Returns:
             bytes: Plaintext in byte array or empty array on error.
             Output is always the same length as the input.
         """
         if iv is None:
@@ -853,25 +904,51 @@
 
         Args:
             s (str): Base64-encoded data
 
         Returns:
             bytes: Binary data in byte array.
 
-        Remarks:
+        Note:
             Whitespace characters are ignored,
             but other non-base64 characters will cause an error.
         """
         n = _didll.CNV_BytesFromB64Str(None, 0, s.encode())
         if (n < 0): raise Error(-n)
         if (n == 0): return bytes("")
         buf = create_string_buffer(n)
         n = _didll.CNV_BytesFromB64Str(buf, n, s.encode())
         return bytes(buf.raw)[:n]
 
+    @staticmethod
+    def shortpathname(pathName):
+        """Retrieve the Windows short path form of the specified path.
+
+        Args:
+            pathName (str): Path name.
+
+        Returns:
+            str: Windows short path name of file or empty string if file does not exist.
+
+        Note:
+            Windows only. The file path must exist. The short path name is guaranteed to be ASCII and
+            can be used as a filename argument in any function in this Toolkit.
+
+        Example:
+            >>> Cnv.shortpathname("work/你好.txt")
+            'work/FC0F~1.TXT'
+        """
+
+        n = _didll.CNV_ShortPathName(None, 0, pathName)
+        if (n < 0): raise Error(-n)
+        if (n == 0): return str("")
+        buf = create_string_buffer(n)
+        n = _didll.CNV_ShortPathName(buf, n, pathName)
+        return (buf.raw.decode())[:n]
+
 
 class Crc:
     """CRC-32 computations."""
 
     @staticmethod
     def bytes(data):
         """Computes the CRC-32 checksum of an array of bytes."""
@@ -894,40 +971,42 @@
         SHA256 = 3  #: SHA-256
         SHA384 = 4  #: SHA-384
         SHA512 = 5  #: SHA-512
         SHA3_224 = 0xA  #: SHA-3-224
         SHA3_256 = 0xB  #: SHA-3-256
         SHA3_384 = 0xC  #: SHA-3-384
         SHA3_512 = 0xD  #: SHA-3-512
-        MD5    = 1  #: MD5 (as per RFC 1321)
+        MD5 = 1  #: MD5
         RMD160 = 7  #: RIPEMD-160
+        ASCON_HASH = 0xAF  #: ASCON-HASH
+        ASCON_HASHA = 0xBF #: ASCON-HASHA
 
         def __or__(self, other):
             return self | other
 
-    # @staticmethod
-    # def length(alg):
-    #     """length(alg)
-    #     Return length of message digest output in bytes.
-    #
-    #     Args:
-    #         alg (Hash.Alg): Hash algorithm.
-    #
-    #     Returns:
-    #         int: Length of the hash function output in bytes.
-    #
-    #     Examples:
-    #         >>> Hash.length(Hash.Alg.SHA256)
-    #         32
-    #         >>> Hash.length(Hash.Alg.SHA512)
-    #         64
-    #     """
-    #     n = _didll.HASH_Length(alg)
-    #     if (n < 0): raise Error(-n)
-    #     return n
+    @staticmethod
+    def length(alg):
+        """length(alg)
+        Return length of message digest output in bytes.
+
+        Args:
+            alg (Hash.Alg): Hash algorithm.
+
+        Returns:
+            int: Length of the hash function output in bytes.
+
+        Examples:
+            >>> Hash.length(Hash.Alg.SHA256)
+            32
+            >>> Hash.length(Hash.Alg.SHA512)
+            64
+        """
+        n = _didll.HASH_Length(alg)
+        if (n < 0): raise Error(-n)
+        return n
 
     @staticmethod
     def data(data, alg=Alg.SHA1):
         """data(data, alg=Alg.SHA1)
         Compute message digest as a byte array from bytes data.
 
         Args:
@@ -946,15 +1025,15 @@
     @staticmethod
     def file(filename, alg=Alg.SHA1):
         """file(filename, alg=Alg.SHA1)
         Compute message digest as a byte array from data in a file.
 
         Args:
             filename (str): Name of file containing message data
-            alg (Hash.Alg): Hash algorithm to be used
+            alg (Hash.Alg): Hash algorithm to be used (ASCON is not supported in file mode)
 
         Returns:
             bytes: Message digest in byte array.
         """
         n = _didll.HASH_File(None, 0, filename.encode(), alg)
         if (n < 0): raise Error(-n)
         buf = create_string_buffer(n)
@@ -998,25 +1077,27 @@
             str: Message digest in hex-encoded format.
 
         Examples:
             >>> Hash.hex_from_string('abc', Hash.Alg.SHA256)
             'ba7816bf8f01cfea414140de5dae2223b00361a396177a9cb410ff61f20015ad'
             >>> Hash.hex_from_string('Olá mundo')  # UTF-8
             'f6c2fc0dd7f1131d8cb5ac7420d77a4c28ac1aa0'
+            >>> Hash.hex_from_string("", Hash.Alg.ASCON_HASHA)
+            'aecd027026d0675f9de7a8ad8ccf512db64b1edcf0b20c388a0c7cc617aaa2c4'
         """
         return Hash.hex_from_data(s.encode(), alg)
 
     @staticmethod
     def hex_from_file(filename, alg=Alg.SHA1):
         """hex_from_file(filename, alg=Alg.SHA1)
         Compute message digest in hexadecimal format from data in a file.
 
         Args:
             filename (str): Name of file containing message data
-            alg (Hash.Alg): Hash algorithm to be used
+            alg (Hash.Alg): Hash algorithm to be used (ASCON is not supported in file mode)
 
         Returns:
             str: Message digest in hex-encoded format
         """
         nc = _didll.HASH_HexFromFile(None, 0, filename.encode(), alg)
         if (nc < 0): raise Error(-nc)
         buf = create_string_buffer(nc + 1)
@@ -1041,14 +1122,44 @@
         """
         nc = _didll.HASH_HexFromHex(None, 0, datahex.encode(), alg)
         if (nc < 0): raise Error(-nc)
         buf = create_string_buffer(nc + 1)
         _didll.HASH_HexFromHex(buf, nc, datahex.encode(), alg)
         return buf.value.decode()
 
+    @staticmethod
+    def hex_from_bits(data, databitlen, alg=Alg.SHA1):
+        """hex_from_bits(data, databitlen, alg=Alg.SHA1)
+        Compute message digest in hexadecimal format from bit-oriented data.
+
+        Args:
+            data (bytes): Message data in byte array.
+            databitlen (int): Length of message data in bits.
+            alg (Hash.Alg): Hash algorithm to be used (only the SHA family is supported).
+
+        Returns:
+            string: Message digest in hex-encoded format.
+
+        Note:
+            Pass a bitstring as an array of bytes in `data` in big-endian order with the most-significant bit first.
+            The bitstring will be truncated to the number of bits specified in `databitlen`.
+            The number of bytes in `data` must be at least `ceil(databitlen / 8)`.
+
+        Examples:
+            >>> Hash.hex_from_bits(Cnv.fromhex("5180"), 9, Hash.Alg.SHA1)  # 0101 0001 1
+            '0f582fa68b71ecdf1dcfc4946019cf5a18225bd2'
+            >>> Hash.hex_from_bits(Cnv.fromhex("2590A0"), 22, Hash.Alg.SHA3_256)  # 1001 0110 0100 0010 1000 00
+            'd5863d4b1ff41551c92a9e08c52177e32376c9bd100c611c607db840096eb22f'
+        """
+        nc = _didll.HASH_HexFromBits(None, 0, bytes(data), databitlen, alg)
+        if (nc < 0): raise Error(-nc)
+        buf = create_string_buffer(nc + 1)
+        _didll.HASH_HexFromBits(buf, nc, bytes(data), databitlen, alg)
+        return buf.value.decode()
+
 
 class Mac:
     """Message authentication code (MAC) functions."""
 
     # CONSTANTS
     class Alg:
         """MAC algorithms."""
@@ -1241,15 +1352,15 @@
     class Alg:
         """Key derivation function algorithms."""
         ZLIB = 0x0  #: zlib algorithm (default)
         ZSTD = 0x1  #: Zstandard algorithm
 
     @staticmethod
     def compress(data, alg=Alg.ZLIB):
-        """Compress data using zlib compression.
+        """Compress data using compression algorithm.
 
         Args:
              data (bytes): Data to be compressed.
              alg (Compr.Alg): Compression algorithm.
 
         Returns:
              bytes: Compressed data.
@@ -1260,15 +1371,15 @@
         if (n == 0): return bytes("")
         buf = create_string_buffer(n)
         n = _didll.COMPR_Compress(buf, n, bytes(data), len(data), opts)
         return bytes(buf.raw)[:n]
 
     @staticmethod
     def uncompress(data, alg=Alg.ZLIB):
-        """Uncompress data using zlib compression.
+        """Uncompress data using compression algorithm.
 
         Args:
              data (bytes): Compressed data to be uncompressed.
              alg (Compr.Alg): Compression algorithm.
 
         Returns:
              bytes: Uncompressed data.
@@ -1417,74 +1528,87 @@
     class Alg:
         """Extendable-output function (XOF) algorithm."""
         SHAKE128 = 0x203  #: SHAKE128 as per FIPS PUB 202
         SHAKE256 = 0x204  #: SHAKE256 as per FIPS PUB 202
         MGF1_SHA1 = 0x210    #: MGF1-SHA-1 as per PKCS#1
         MGF1_SHA256 = 0x213  #: MGF1-SHA-256
         MGF1_SHA512 = 0x215  #: MGF1-SHA-512
+        ASCON_XOF = 0x20A  #: ASCON-XOF
+        ASCON_XOFA = 0x20B  #: ASCON-XOFA
 
     @staticmethod
     def bytes(numbytes, msg, xofalg):
         """Generate bytes using an extendable-output function (XOF).
 
         Args:
             numbytes (int): Required number of output bytes.
             msg (bytes): Input message data.
-            xofalg (Xof.Alg): PRF algorithm
+            xofalg (Xof.Alg): XOF algorithm
 
         Returns:
             bytes: Output data.
 
         """
         # NB numbytes is arbitrary, returns numbytes on success
         if (numbytes <= 0 or numbytes > _INTMAX): raise Error('numbytes out of range')
         buf = create_string_buffer(numbytes)
         opts = xofalg
         n = _didll.XOF_Bytes(buf, numbytes, bytes(msg), len(msg), opts)
         if (n < 0): raise Error(-n if n < 0 else n)
         return bytes(buf.raw)
 
 
+class _NotUsed:
+    """Dummy for parsing."""
+    pass
+
+
 # PROTOTYPES (derived from diCryptoSys.h)
 # If wrong argument type is passed, these will raise an `ArgumentError` exception
 #     ArgumentError: argument 1: <type 'exceptions.TypeError'>: wrong type
 _didll.API_Version.argtypes = []
 _didll.API_LicenceType.argtypes = [c_int]
 _didll.API_ErrorCode.argtypes = []
 _didll.API_ErrorLookup.argtypes = [c_char_p, c_int, c_int]
 _didll.API_CompileTime.argtypes = [c_char_p, c_int]
 _didll.API_ModuleName.argtypes = [c_char_p, c_int, c_int]
+_didll.API_ModuleInfo.argtypes = [c_char_p, c_int, c_int]
+_didll.API_Platform.argtypes = [c_char_p, c_int]
 _didll.API_PowerUpTests.argtypes = [c_int]
 _didll.AEAD_EncryptWithTag.argtypes = [c_char_p, c_int, c_char_p, c_int, c_char_p, c_int, c_char_p, c_int, c_char_p, c_int, c_int]
 _didll.AEAD_DecryptWithTag.argtypes = [c_char_p, c_int, c_char_p, c_int, c_char_p, c_int, c_char_p, c_int, c_char_p, c_int, c_int]
 _didll.CIPHER_EncryptBytes.argtypes = [c_char_p, c_int, c_char_p, c_int, c_char_p, c_int, c_char_p, c_int, c_char_p, c_int]
 _didll.CIPHER_DecryptBytes.argtypes = [c_char_p, c_int, c_char_p, c_int, c_char_p, c_int, c_char_p, c_int, c_char_p, c_int]
 _didll.CIPHER_EncryptHex.argtypes = [c_char_p, c_int, c_char_p, c_char_p, c_char_p, c_char_p, c_int]
 _didll.CIPHER_DecryptHex.argtypes = [c_char_p, c_int, c_char_p, c_char_p, c_char_p, c_char_p, c_int]
 _didll.CIPHER_FileEncrypt.argtypes = [c_char_p, c_char_p, c_char_p, c_int, c_char_p, c_int, c_char_p, c_int]
 _didll.CIPHER_FileDecrypt.argtypes = [c_char_p, c_char_p, c_char_p, c_int, c_char_p, c_int, c_char_p, c_int]
+_didll.CIPHER_KeyWrap.argtypes = [c_char_p, c_int, c_char_p, c_int, c_char_p, c_int, c_int]
+_didll.CIPHER_KeyUnwrap.argtypes = [c_char_p, c_int, c_char_p, c_int, c_char_p, c_int, c_int]
 _didll.PAD_BytesBlock.argtypes = [c_char_p, c_int, c_char_p, c_int, c_int, c_int]
 _didll.PAD_HexBlock.argtypes = [c_char_p, c_int, c_char_p, c_int, c_int]
 _didll.PAD_UnpadBytes.argtypes = [c_char_p, c_int, c_char_p, c_int, c_int, c_int]
 _didll.PAD_UnpadHex.argtypes = [c_char_p, c_int, c_char_p, c_int, c_int]
 _didll.CIPHER_StreamBytes.argtypes = [c_char_p, c_char_p, c_int, c_char_p, c_int, c_char_p, c_int, c_int, c_int]
 _didll.CIPHER_StreamFile.argtypes = [c_char_p, c_char_p, c_char_p, c_int, c_char_p, c_int, c_int, c_int]
 _didll.BLF_BytesMode.argtypes = [c_char_p, c_char_p, c_int, c_char_p, c_int, c_int, c_char_p, c_char_p]
 _didll.BLF_BytesMode.argtypes = [c_char_p, c_char_p, c_int, c_char_p, c_int, c_int, c_char_p, c_char_p]
 _didll.CNV_HexStrFromBytes.argtypes = [c_char_p, c_int, c_char_p, c_int]
 _didll.CNV_BytesFromHexStr.argtypes = [c_char_p, c_int, c_char_p]
 _didll.CNV_B64StrFromBytes.argtypes = [c_char_p, c_int, c_char_p, c_int]
 _didll.CNV_BytesFromB64Str.argtypes = [c_char_p, c_int, c_char_p]
+_didll.CNV_ShortPathName.argtypes = [c_char_p, c_int, c_wchar_p]
 _didll.CRC_Bytes.argtypes = [c_char_p, c_int, c_int]
 _didll.CRC_File.argtypes = [c_char_p, c_int]
 _didll.HASH_Bytes.argtypes = [c_char_p, c_int, c_void_p, c_int, c_int]
 _didll.HASH_File.argtypes = [c_char_p, c_int, c_char_p, c_int]
 _didll.HASH_HexFromBytes.argtypes = [c_char_p, c_int, c_void_p, c_int, c_int]
 _didll.HASH_HexFromFile.argtypes = [c_char_p, c_int, c_char_p, c_int]
 _didll.HASH_HexFromHex.argtypes = [c_char_p, c_int, c_char_p, c_int]
+_didll.HASH_HexFromBits.argtypes = [c_char_p, c_int, c_char_p, c_int, c_int]
 _didll.MAC_Bytes.argtypes = [c_char_p, c_int, c_void_p, c_int, c_void_p, c_int, c_int]
 _didll.MAC_HexFromBytes.argtypes = [c_char_p, c_int, c_void_p, c_int, c_void_p, c_int, c_int]
 _didll.MAC_HexFromHex.argtypes = [c_char_p, c_int, c_char_p, c_char_p, c_int]
 _didll.RNG_KeyBytes.argtypes = [c_char_p, c_int, c_char_p, c_int]
 _didll.RNG_Number.argtypes = [c_int, c_int]
 _didll.RNG_Initialize.argtypes = [c_char_p, c_int]
 _didll.RNG_UpdateSeedFile.argtypes = [c_char_p, c_int]
```

## Comparing `crsysapi-6.20.0/PKG-INFO` & `crsysapi-6.21.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,71 @@
-Metadata-Version: 1.0
-Name: crsysapi
-Version: 6.20.0
-Summary: Python interface to CryptoSys API
-Home-page: https://www.cryptosys.net/
-Author: David Ireland
-Author-email: UNKNOWN
-License: See source code modules
-Description: A Python interface to CryptoSys API
-        ===================================
-        
-        This is a Python interface to the **CryptoSys API** library. 
-        
-        
-        Requires: Python 3.
-        CryptoSys API v6.20 or above must be installed.
-        This is available from
-        
-            https://www.cryptosys.net/.
-        
-        
-        To use in Python's REPL
-        -----------------------
-        
-        Using wild import for simplicity.
-        
-        .. code-block:: python
-        
-            >>> from crsysapi import *  # @UnusedWildImport
-            >>> Gen.version() # "hello world!" for CryptoSys API
-            62000
-            >>> Hash.hex_from_data(b'abc') # compute SHA-1 hash in hex of 'abc' as bytes
-            'a9993e364706816aba3e25717850c26c9cd0d89d'
-            >>> Hash.hex_from_string('abc', Hash.Alg.SHA256)   # same but over a string and using SHA-256
-            'ba7816bf8f01cfea414140de5dae2223b00361a396177a9cb410ff61f20015ad'
-            >>> h = Hash.data(b'abc')   # h is a byte array (bytes->bytes)
-            >>> print(Cnv.tohex(h))     # display the byte array in hex
-            A9993E364706816ABA3E25717850C26C9CD0D89D
-        
-        The proper way using the ``crsysapi`` prefix.
-        
-        .. code-block:: python
-        
-            >>> import crsysapi
-            >>> crsysapi.Gen.version() # Underlying core CryptoSys API dll
-            62000
-            >>> crsysapi.__version__  # crsysapi.py module version
-            6.20.0.0000
-            >>> crsysapi.Hash.hex_from_data(b'abc') # compute SHA-1 hash in hex of 'abc' as bytes
-            'a9993e364706816aba3e25717850c26c9cd0d89d'
-            >>> crsysapi.Hash.hex_from_string('abc', crsysapi.Hash.Alg.SHA256)   # same but over a string and using SHA-256
-            'ba7816bf8f01cfea414140de5dae2223b00361a396177a9cb410ff61f20015ad'
-            >>> h = crsysapi.Hash.data(b'abc')   # h is a byte array (bytes->bytes)
-            >>> print(crsysapi.Cnv.tohex(h))     # display the byte array in hex
-            A9993E364706816ABA3E25717850C26C9CD0D89D
-        
-        Note that ``crsysapi.Gen.version()`` gives the version number of the underlying core CryptoSys API DLL, and ``crsysapi.__version__`` gives the version of the Python crsysapi modulw. 
-        
-        Examples
-        --------
-        
-        See the test file ``test/test_crsysapi.py`` for examples of all classes and methods. This creates any required test files automatically.
-        
-        Contact
-        -------
-        
-        For more information or to make suggestions, please contact us at
-        https://www.cryptosys.net/contact/
-        
-        | David Ireland
-        | DI Management Services Pty Ltd
-        | Australia
-        | <https://www.di-mgt.com.au> <https://www.cryptosys.net>
-        | 9 April 2023
-        
-        
-        Revision History
-        -----------------
-        
-        6.20.0 (2023-04-09)
-        ^^^^^^^^^^^^^^^^^^^
-        
-        * First release of crsysapi.py, the Python interface to CryptoSys API v6.20.
-        
-Platform: Windows
+Python for CryptoSys API
+===================================
+
+This is a Python interface to the **CryptoSys API** library <https://www.cryptosys.net/api.html>. 
+
+CryptoSys API is a library to carry out "symmetrical" encryption using block ciphers like AES and Triple DES; 
+stream ciphers ArcFour, Salsa and ChaCha20; Authenticated Encryption with Additional Data (AEAD);
+message authentication algorithms HMAC, CMAC and KMAC; 
+hash functions SHA-1, SHA-2 and SHA-3; the PBKDF2 and SCRYPT key derivation functions; and more. 
+
+Requires: Python 3.
+CryptoSys API v6.21 or above must be installed on your system.
+This is available from
+
+    https://www.cryptosys.net/api.html.
+
+
+To use in Python's REPL
+-----------------------
+
+Using wild import for simplicity.
+
+.. code-block:: python
+
+    >>> from crsysapi import *  # @UnusedWildImport
+    >>> Gen.version() # "hello world!" for CryptoSys API
+    62000
+    >>> Hash.hex_from_data(b'abc') # compute SHA-1 hash in hex of 'abc' as bytes
+    'a9993e364706816aba3e25717850c26c9cd0d89d'
+    >>> Hash.hex_from_string('abc', Hash.Alg.SHA256)   # same but over a string and using SHA-256
+    'ba7816bf8f01cfea414140de5dae2223b00361a396177a9cb410ff61f20015ad'
+    >>> h = Hash.data(b'abc')   # h is a byte array (bytes->bytes)
+    >>> print(Cnv.tohex(h))     # display the byte array in hex
+    A9993E364706816ABA3E25717850C26C9CD0D89D
+
+The stricter way using the ``crsysapi`` prefix.
+
+.. code-block:: python
+
+    >>> import crsysapi
+    >>> crsysapi.Gen.version() # Underlying core CryptoSys API dll
+    62000
+    >>> crsysapi.__version__  # crsysapi.py module version
+    6.20.0.0000
+    >>> crsysapi.Hash.hex_from_data(b'abc') # compute SHA-1 hash in hex of 'abc' as bytes
+    'a9993e364706816aba3e25717850c26c9cd0d89d'
+    >>> crsysapi.Hash.hex_from_string('abc', crsysapi.Hash.Alg.SHA256)   # same but over a string and using SHA-256
+    'ba7816bf8f01cfea414140de5dae2223b00361a396177a9cb410ff61f20015ad'
+    >>> h = crsysapi.Hash.data(b'abc')   # h is a byte array (bytes->bytes)
+    >>> print(crsysapi.Cnv.tohex(h))     # display the byte array in hex
+    A9993E364706816ABA3E25717850C26C9CD0D89D
+
+Note that ``crsysapi.Gen.version()`` gives the version number of the underlying core (native) CryptoSys API DLL, 
+and ``crsysapi.__version__`` gives the version of the Python crsysapi module. 
+
+Examples
+--------
+
+See the test file ``test/test_crsysapi.py`` for examples of all classes and methods. This creates any required test files automatically.
+
+Contact
+-------
+
+For more information or to make suggestions, please contact us at
+https://www.cryptosys.net/contact/
+
+| David Ireland
+| DI Management Services Pty Ltd
+| Australia
+| <https://www.di-mgt.com.au> <https://www.cryptosys.net>
+| 18 May 2023
```

## Comparing `crsysapi-6.20.0/setup.py` & `crsysapi-6.21.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 readme = read('README.rst')
 changelog = read('CHANGELOG.rst')
 
 setup(name='crsysapi',
-      version='6.20.0',
+      version='6.21.0',
       description='Python interface to CryptoSys API',
       long_description=readme + '\n\n' + changelog,
       author='David Ireland',
-      url='https://www.cryptosys.net/',
+      url='https://www.cryptosys.net/api.html',
       platforms=['Windows'],
       py_modules=['crsysapi'],
       license='See source code modules'
       )
```

## Comparing `crsysapi-6.20.0/crsysapi.egg-info/PKG-INFO` & `crsysapi-6.21.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 1.0
 Name: crsysapi
-Version: 6.20.0
+Version: 6.21.0
 Summary: Python interface to CryptoSys API
-Home-page: https://www.cryptosys.net/
+Home-page: https://www.cryptosys.net/api.html
 Author: David Ireland
 Author-email: UNKNOWN
 License: See source code modules
-Description: A Python interface to CryptoSys API
+Description: Python for CryptoSys API
         ===================================
         
-        This is a Python interface to the **CryptoSys API** library. 
+        This is a Python interface to the **CryptoSys API** library <https://www.cryptosys.net/api.html>. 
         
+        CryptoSys API is a library to carry out "symmetrical" encryption using block ciphers like AES and Triple DES; 
+        stream ciphers ArcFour, Salsa and ChaCha20; Authenticated Encryption with Additional Data (AEAD);
+        message authentication algorithms HMAC, CMAC and KMAC; 
+        hash functions SHA-1, SHA-2 and SHA-3; the PBKDF2 and SCRYPT key derivation functions; and more. 
         
         Requires: Python 3.
-        CryptoSys API v6.20 or above must be installed.
+        CryptoSys API v6.21 or above must be installed on your system.
         This is available from
         
-            https://www.cryptosys.net/.
+            https://www.cryptosys.net/api.html.
         
         
         To use in Python's REPL
         -----------------------
         
         Using wild import for simplicity.
         
@@ -33,15 +37,15 @@
             'a9993e364706816aba3e25717850c26c9cd0d89d'
             >>> Hash.hex_from_string('abc', Hash.Alg.SHA256)   # same but over a string and using SHA-256
             'ba7816bf8f01cfea414140de5dae2223b00361a396177a9cb410ff61f20015ad'
             >>> h = Hash.data(b'abc')   # h is a byte array (bytes->bytes)
             >>> print(Cnv.tohex(h))     # display the byte array in hex
             A9993E364706816ABA3E25717850C26C9CD0D89D
         
-        The proper way using the ``crsysapi`` prefix.
+        The stricter way using the ``crsysapi`` prefix.
         
         .. code-block:: python
         
             >>> import crsysapi
             >>> crsysapi.Gen.version() # Underlying core CryptoSys API dll
             62000
             >>> crsysapi.__version__  # crsysapi.py module version
@@ -50,15 +54,16 @@
             'a9993e364706816aba3e25717850c26c9cd0d89d'
             >>> crsysapi.Hash.hex_from_string('abc', crsysapi.Hash.Alg.SHA256)   # same but over a string and using SHA-256
             'ba7816bf8f01cfea414140de5dae2223b00361a396177a9cb410ff61f20015ad'
             >>> h = crsysapi.Hash.data(b'abc')   # h is a byte array (bytes->bytes)
             >>> print(crsysapi.Cnv.tohex(h))     # display the byte array in hex
             A9993E364706816ABA3E25717850C26C9CD0D89D
         
-        Note that ``crsysapi.Gen.version()`` gives the version number of the underlying core CryptoSys API DLL, and ``crsysapi.__version__`` gives the version of the Python crsysapi modulw. 
+        Note that ``crsysapi.Gen.version()`` gives the version number of the underlying core (native) CryptoSys API DLL, 
+        and ``crsysapi.__version__`` gives the version of the Python crsysapi module. 
         
         Examples
         --------
         
         See the test file ``test/test_crsysapi.py`` for examples of all classes and methods. This creates any required test files automatically.
         
         Contact
@@ -67,19 +72,25 @@
         For more information or to make suggestions, please contact us at
         https://www.cryptosys.net/contact/
         
         | David Ireland
         | DI Management Services Pty Ltd
         | Australia
         | <https://www.di-mgt.com.au> <https://www.cryptosys.net>
-        | 9 April 2023
+        | 18 May 2023
         
         
         Revision History
         -----------------
         
+        6.21.0 (2023-05-18)
+        ^^^^^^^^^^^^^^^^^^^
+        
+        * Changes to match main core module version 6.21.
+        
+        
         6.20.0 (2023-04-09)
         ^^^^^^^^^^^^^^^^^^^
         
         * First release of crsysapi.py, the Python interface to CryptoSys API v6.20.
         
 Platform: Windows
```

## Comparing `crsysapi-6.20.0/test/test_crsysapi.py` & `crsysapi-6.21.0/test/test_crsysapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! python3
 # -*- coding: utf-8 -*-
 
 """Some tests for ``crsysapi.py`` the Python interface to CryptoSys API"""
 
 # test_crsysapi.py: version 6.20.0
-# $Date: 2023-04-09 08:37:00 $
+# $Date: 2023-05-21 04:43:00 $
 
 # ************************** LICENSE *****************************************
 # Copyright (C) 2023 David Ireland, DI Management Services Pty Limited.
 # All rights reserved. <www.di-mgt.com.au> <www.cryptosys.net>
 # The code in this module is licensed under the terms of the MIT license.
 # For a copy, see <http://opensource.org/licenses/MIT>
 # ****************************************************************************
@@ -16,35 +16,81 @@
 import crsysapi
 import os
 import sys
 import pytest
 import shutil
 from glob import iglob
 
-_MIN_API_VERSION = 62000
-do_all = True
+_MIN_API_VERSION = 62100
 
 print("crsysapi version =", crsysapi.__version__)
 # Show some info about the core native DLL
 print("API core version =", crsysapi.Gen.version())
 print("module_name =", crsysapi.Gen.module_name())
 print("compile_time =", crsysapi.Gen.compile_time())
 print("platform =", crsysapi.Gen.core_platform())
 print("licence_type =", crsysapi.Gen.licence_type())
-# print("module_info =", crsysapi.Gen.module_info())
+print("module_info =", crsysapi.Gen.module_info())
 # Show some system values
 print("sys.getdefaultencoding()=", sys.getdefaultencoding())
 print("sys.getfilesystemencoding()=", sys.getfilesystemencoding())
 print("sys.platform()=", sys.platform)
 print("cwd =", os.getcwd())
 
 if crsysapi.Gen.version() < _MIN_API_VERSION:
     raise Exception('Require API version ' +
                     str(_MIN_API_VERSION) + ' or greater')
 
+# GLOBAL VARS
+# Remember CWD where we started
+start_dir = os.getcwd()
+# We use a subdir `work` for our temp files
+work_dir = os.path.join(start_dir, "work")
+
+
+def setup_work_dir():
+    if not os.path.isdir(work_dir):
+        os.mkdir(work_dir)
+    # Set CWD here
+    os.chdir(work_dir)
+    print("Working in directory:", os.getcwd())
+
+
+def reset_start_dir():
+    if not os.path.isdir(start_dir):
+        return
+    if (work_dir == start_dir):
+        return
+    os.chdir(start_dir)
+    print("")
+    # print("CWD:", os.getcwd())
+
+
+# JIGGERY_POKERY FOR py.test
+@pytest.fixture(scope="module", autouse=True)
+def divider_module(request):
+    print("\n   --- module %s() start ---" % request.module.__name__)
+    setup_work_dir()
+
+    def fin():
+        print("\n   --- module %s() done ---" % request.module.__name__)
+        reset_start_dir()
+    request.addfinalizer(fin)
+
+
+@pytest.fixture(scope="function", autouse=True)
+def divider_function(request):
+    print("\n   --- function %s() start ---" % request.function.__name__)
+    os.chdir(work_dir)
+
+    def fin():
+        print("\n   --- function %s() done ---" % request.function.__name__)
+        os.chdir(start_dir)
+    request.addfinalizer(fin)
+
 
 # FILE-RELATED UTILITIES
 def read_binary_file(fname):
     with open(fname, "rb") as f:
         return bytearray(f.read())
 
 
@@ -80,14 +126,15 @@
     s = read_text_file(fname)
     ndash = (24 if len(s) > 24 else len(s))
     print("FILE:", fname)
     print("-" * ndash)
     print(s)
     print("-" * ndash)
 
+
 #############
 # THE TESTS #
 #############
 
 
 def test_error_lookup():
     print("\nLOOKUP SOME ERROR CODES...")
@@ -444,15 +491,15 @@
     print('crsysapi.Rng.update_seedfile() returns', n, ". Contents of seed file:")
     sd = read_binary_file(seedfile)
     print(crsysapi.Cnv.tohex(sd))
     assert(len(sd) == crsysapi.Rng.SEED_BYTES)
 
 
 def test_hash():
-    print("\nTESTING Hash...")
+    print("\nTESTING HASH...")
     # write a file containing the 3 bytes 'abc'
     write_text_file('abc.txt', 'abc')
     _dump_file('abc.txt')
     abc_hex = crsysapi.Cnv.tohex(b'abc')
     print("'abc' in hex:", abc_hex)
 
     # Use default SHA-1 algorithm
@@ -496,20 +543,35 @@
     print("crsysapi.Hash.file('abc.txt'):", crsysapi.Cnv.tohex(b))
     assert(b == crsysapi.Cnv.fromhex('ec01498288516fc926459f58e2c6ad8df9b473cb0fc08c2596da7cf0e49be4b298d88cea927ac7f539f1edf228376d25'))
     h = crsysapi.Hash.hex_from_file('abc.txt', crsysapi.Hash.Alg.SHA3_512)
     print("crsysapi.Hash.hex_from_file('abc.txt'):", h)
     assert(crsysapi.Cnv.fromhex(h) == crsysapi.Cnv.fromhex('b751850b1a57168a5693cd924b6b096e08f621827444f70d884f5d0240d2712e10e116e9192af3c91a7ec57647e3934057340b4cf408d5a56592f8274eec53f0'))
 
 
-# def test_hash_length():
-#     print("\nTEST HASH LENGTH...")
-#     print("Hash.length(SHA-1) =", crsysapi.Hash.length(crsysapi.Hash.Alg.SHA1))
-#     print("Hash.length(SHA-256) =", crsysapi.Hash.length(crsysapi.Hash.Alg.SHA256))
-#     print("Hash.length(SHA-512) =", crsysapi.Hash.length(crsysapi.Hash.Alg.SHA512))
-#     print("Hash.length(RMD160) =", crsysapi.Hash.length(crsysapi.Hash.Alg.RMD160))
+def test_hash_bits():
+    print("\nTESTING HASH BITS...")
+    h = crsysapi.Hash.hex_from_bits(crsysapi.Cnv.fromhex("5180"), 9, crsysapi.Hash.Alg.SHA1)
+    print("Input bits (9) = 0101 0001 1")
+    print("hex_from_bits(SHA-1) =", h)
+    assert(crsysapi.Cnv.fromhex(h) == crsysapi.Cnv.fromhex('0f582fa68b71ecdf1dcfc4946019cf5a18225bd2'))
+    # Ref: SHAVS-SHA3 CAVS 19.0 "SHA3-256 ShortMsg"
+    h = crsysapi.Hash.hex_from_bits(crsysapi.Cnv.fromhex("2590A0"), 22, crsysapi.Hash.Alg.SHA3_256)
+    print("Input bits (22) = 1001 0110 0100 0010 1000 00")
+    print("hex_from_bits(SHA-3-256) =", h)
+    assert(crsysapi.Cnv.fromhex(h) == crsysapi.Cnv.fromhex('d5863d4b1ff41551c92a9e08c52177e32376c9bd100c611c607db840096eb22f'))
+
+
+def test_hash_length():
+    print("\nTEST HASH LENGTH...")
+    print("Hash.length(SHA-1) =", crsysapi.Hash.length(crsysapi.Hash.Alg.SHA1))
+    print("Hash.length(SHA-256) =", crsysapi.Hash.length(crsysapi.Hash.Alg.SHA256))
+    print("Hash.length(SHA-384) =", crsysapi.Hash.length(crsysapi.Hash.Alg.SHA384))
+    print("Hash.length(SHA-512) =", crsysapi.Hash.length(crsysapi.Hash.Alg.SHA512))
+    print("Hash.length(RMD160) =", crsysapi.Hash.length(crsysapi.Hash.Alg.RMD160))
+    print("Hash.length(ASCON-HASH) =", crsysapi.Hash.length(crsysapi.Hash.Alg.ASCON_HASH))
 
 
 def test_mac():
     print("\nTESTING MAC...")
     print("Test case 4 from RFC 2202 and RFC 4231")
     key = crsysapi.Cnv.fromhex('0102030405060708090a0b0c0d0e0f10111213141516171819')
     print("key: ", crsysapi.Cnv.tohex(key))
@@ -890,78 +952,265 @@
     assert (okhex.lower() == crsysapi.Cnv.tohex(ct).lower())
     # Repeat to decrypt
     dt = crsysapi.CipherStream.bytes(ct, key, iv, crsysapi.CipherStream.Alg.CHACHA20, counter=1)
     print("DT =", crsysapi.Cnv.tohex(dt))
     assert (pt == dt)
 
 
+def test_keywrap():
+    print("\nTESTING CipherKeyWrap...")
+    keydata = crsysapi.Cnv.fromhex("00112233 44556677 8899aabb ccddeeff")
+    kek = crsysapi.Cnv.fromhex("c17a44e8 e28d7d64 81d1ddd5 0a3b8914")
+    print("KD          =", crsysapi.Cnv.tohex(keydata))
+    print("KEK         =", crsysapi.Cnv.tohex(kek))
+    wk = crsysapi.Cipher.key_wrap(keydata, kek, crsysapi.Cipher.Alg.AES128)
+    print("WK(AES-128) =", crsysapi.Cnv.tohex(wk))
+    print("OK          =", "503D75C73630A7B02ECF51B9B29B907749310B77B0B2E054")
+    # Reverse
+    kd = crsysapi.Cipher.key_unwrap(wk, kek, crsysapi.Cipher.Alg.AES128)
+    print("KD'         =", crsysapi.Cnv.tohex(kd))
+
+    keydata = crsysapi.Cnv.fromhex("8cbedec4 8d063e1b a46be8e3 69a9c398 d8e30ee5 42bc347c 4f30e928 ddd7db49")
+    kek = crsysapi.Cnv.fromhex("9e84ee99 e6a84b50 c76cd414 a2d2ec05 8af41bfe 4bf3715b f894c8da 1cd445f6")
+    print("KD          =", crsysapi.Cnv.tohex(keydata))
+    print("KEK         =", crsysapi.Cnv.tohex(kek))
+    wk = crsysapi.Cipher.key_wrap(keydata, kek, crsysapi.Cipher.Alg.AES256)
+    print("WK(AES-256) =", crsysapi.Cnv.tohex(wk))
+    print("OK          =", "EAFB901F82B98D37F17497063DE3E5EC7246AB57200AE73EDDDDF24AA403DAFA0C5AE151D1746FA4")
+    # Reverse
+    kd = crsysapi.Cipher.key_unwrap(wk, kek, crsysapi.Cipher.Alg.AES256)
+    print("KD'         =", crsysapi.Cnv.tohex(kd))
+
+
+def test_ascon_aead():
+    print("\nTEST ASCON AEAD...")
+    # Ref: ascon128v12/LWC_AEAD_KAT_128_128.txt, Count = 303
+    key = crsysapi.Cnv.fromhex("000102030405060708090A0B0C0D0E0F")
+    nonce = crsysapi.Cnv.fromhex("000102030405060708090A0B0C0D0E0F")
+    pt = crsysapi.Cnv.fromhex("000102030405060708")
+    ad = crsysapi.Cnv.fromhex("0001020304")
+    print("K =", crsysapi.Cnv.tohex(key))
+    print("N =", crsysapi.Cnv.tohex(nonce))
+    print("P =", crsysapi.Cnv.tohex(pt))
+    print("A =", crsysapi.Cnv.tohex(ad))
+
+    ct = crsysapi.Aead.encrypt_with_tag(pt, key, nonce, crsysapi.Aead.AeadAlg.AEAD_ASCON_128, aad=ad)
+    print("C =", crsysapi.Cnv.tohex(ct))
+    assert(crsysapi.Cnv.tohex(ct) == "0E6A8B0CA517F53D3D375623AC11C852FF0A98098CCB7429F2")
+    # Check decrypted text
+    dt = crsysapi.Aead.decrypt_with_tag(ct, key, nonce, crsysapi.Aead.AeadAlg.AEAD_ASCON_128, aad=ad)
+    print("D =", crsysapi.Cnv.tohex(dt))
+    assert(crsysapi.Cnv.tohex(dt) == crsysapi.Cnv.tohex(pt))
+    # Same but prepending iv (nonce) to ciphertext
+    ct = crsysapi.Aead.encrypt_with_tag(pt, key, nonce, crsysapi.Aead.AeadAlg.AEAD_ASCON_128, aad=ad, opts=crsysapi.Aead.Opts.PREFIXIV)
+    print("C =", crsysapi.Cnv.tohex(ct))
+    dt = crsysapi.Aead.decrypt_with_tag(ct, key, nonce, crsysapi.Aead.AeadAlg.AEAD_ASCON_128, aad=ad, opts=crsysapi.Aead.Opts.PREFIXIV)
+    print("D =", crsysapi.Cnv.tohex(dt))
+    assert(crsysapi.Cnv.tohex(dt) == crsysapi.Cnv.tohex(pt))
+
+    # Use ASCON-128A with no AAD on empty string
+    # Ref: ascon128av12/LWC_AEAD_KAT_128_128.txt, Count = 1
+    pt = crsysapi.Cnv.fromhex("")  # Empty string
+    print("P =", crsysapi.Cnv.tohex(pt))
+    ct = crsysapi.Aead.encrypt_with_tag(pt, key, nonce, crsysapi.Aead.AeadAlg.AEAD_ASCON_128A)
+    print("C =", crsysapi.Cnv.tohex(ct))
+    assert(crsysapi.Cnv.tohex(ct) == "7A834E6F09210957067B10FD831F0078")
+    dt = crsysapi.Aead.decrypt_with_tag(ct, key, nonce, crsysapi.Aead.AeadAlg.AEAD_ASCON_128A)
+    print("D =", crsysapi.Cnv.tohex(dt))
+    assert(crsysapi.Cnv.tohex(dt) == crsysapi.Cnv.tohex(pt))
+
+
+def test_ascon_hash():
+    print("\nTEST ASCON HASH...")
+    # Ref: asconhashv12/LWC_HASH_KAT_256.txt; Count = 513
+    msg = crsysapi.Cnv.fromhex("""000102030405060708090A0B0C0D0E0F101112131415161718191A1B1C1D1E1F2021222324252627
+28292A2B2C2D2E2F303132333435363738393A3B3C3D3E3F404142434445464748494A4B4C4D4E4F
+505152535455565758595A5B5C5D5E5F606162636465666768696A6B6C6D6E6F7071727374757677
+78797A7B7C7D7E7F808182838485868788898A8B8C8D8E8F909192939495969798999A9B9C9D9E9F
+A0A1A2A3A4A5A6A7A8A9AAABACADAEAFB0B1B2B3B4B5B6B7B8B9BABBBCBDBEBFC0C1C2C3C4C5C6C7
+C8C9CACBCCCDCECFD0D1D2D3D4D5D6D7D8D9DADBDCDDDEDFE0E1E2E3E4E5E6E7E8E9EAEBECEDEEEF
+F0F1F2F3F4F5F6F7F8F9FAFBFCFDFEFF000102030405060708090A0B0C0D0E0F1011121314151617
+18191A1B1C1D1E1F202122232425262728292A2B2C2D2E2F303132333435363738393A3B3C3D3E3F
+404142434445464748494A4B4C4D4E4F505152535455565758595A5B5C5D5E5F6061626364656667
+68696A6B6C6D6E6F707172737475767778797A7B7C7D7E7F808182838485868788898A8B8C8D8E8F
+909192939495969798999A9B9C9D9E9FA0A1A2A3A4A5A6A7A8A9AAABACADAEAFB0B1B2B3B4B5B6B7
+B8B9BABBBCBDBEBFC0C1C2C3C4C5C6C7C8C9CACBCCCDCECFD0D1D2D3D4D5D6D7D8D9DADBDCDDDEDF
+E0E1E2E3E4E5E6E7E8E9EAEBECEDEEEFF0F1F2F3F4F5F6F7F8F9FAFBFCFDFEFF""")
+    digest = crsysapi.Hash.data(msg, crsysapi.Hash.Alg.ASCON_HASH)
+    print("MD =", crsysapi.Cnv.tohex(digest))
+    assert(crsysapi.Cnv.tohex(digest) == "7039284FA1CB4C798250B1A62E2378718040E10F206527BFCEB2FF3887884484")
+    # Ref: asconhashav12/LWC_HASH_KAT_256.txt; Count = 1
+    # ASCON-HASHA of empty string
+    digesthex = crsysapi.Hash.hex_from_string("", crsysapi.Hash.Alg.ASCON_HASHA).upper()
+    print("MD =", digesthex)
+    assert(digesthex == "AECD027026D0675F9DE7A8AD8CCF512DB64B1EDCF0B20C388A0C7CC617AAA2C4")
+    # Compute digest of file - ah! cannot use ASCON for files
+    print("<<EXPECTING AN ERROR HERE...")
+    print("Cannot hash file using ASCON:")
+    try:
+        write_binary_file("ascon_data.dat", msg);
+        digest = crsysapi.Hash.file("ascon_data.dat", crsysapi.Hash.Alg.ASCON_HASH)
+        print("MD =", crsysapi.Cnv.tohex(digest))
+    except Exception as e:
+        print("\t", e)
+    print(">>")
+
+
+def test_ascon_xof():
+    print("\nTEST ASCON XOF...")
+    # Ref: asconxofv12/LWC_HASH_KAT_256.txt, Count = 17
+    msg = crsysapi.Cnv.fromhex("000102030405060708090A0B0C0D0E0F")
+    md = crsysapi.Xof.bytes(32, msg, crsysapi.Xof.Alg.ASCON_XOF)
+    print("MD =", crsysapi.Cnv.tohex(md))
+    assert(crsysapi.Cnv.tohex(md) == "C861A89CFB1335F278C96CF7FFC9753C290CBE1A4E186D2923B496BB4EA5E519")
+    # Repeat but ask for more or fewer bytes in output
+    md = crsysapi.Xof.bytes(20, msg, crsysapi.Xof.Alg.ASCON_XOF)
+    print("MD =", crsysapi.Cnv.tohex(md))
+    md = crsysapi.Xof.bytes(40, msg, crsysapi.Xof.Alg.ASCON_XOF)
+    print("MD =", crsysapi.Cnv.tohex(md))
+    # ASCON-XOFA of empty string
+    # Ref: asconxofav12/LWC_HASH_KAT_256.txt, Count = 1
+    md = crsysapi.Xof.bytes(32, b"", crsysapi.Xof.Alg.ASCON_XOFA)
+    print("MD =", crsysapi.Cnv.tohex(md))
+    assert(crsysapi.Cnv.tohex(md) == "7C10DFFD6BB03BE262D72FBE1B0F530013C6C4EADAABDE278D6F29D579E3908D")
+    md = crsysapi.Xof.bytes(20, b"", crsysapi.Xof.Alg.ASCON_XOFA)
+    print("MD =", crsysapi.Cnv.tohex(md))
+    md = crsysapi.Xof.bytes(40, b"", crsysapi.Xof.Alg.ASCON_XOFA)
+    print("MD =", crsysapi.Cnv.tohex(md))
+
+
+def test_xof_mgf1():
+    print("\nTEST XOF MGF1...")
+    msg = crsysapi.Cnv.fromhex("012345ff")
+    md = crsysapi.Xof.bytes(24, msg, crsysapi.Xof.Alg.MGF1_SHA1)
+    print("MD(mgf1_sha1) =", crsysapi.Cnv.tohex(md))
+    assert(crsysapi.Cnv.tohex(md) == "242FB2E7A338AE07E580047F82B7ACFF83A41EC5D8FF9BAB")
+    # Example from SPHINCS+ submission October 2020
+    msg = crsysapi.Cnv.fromhex("3b5c056af3ebba70d4c805380420585562b32410a778f558ff951252407647e3")
+    md = crsysapi.Xof.bytes(34, msg, crsysapi.Xof.Alg.MGF1_SHA256)
+    print("MD(mgf1_sha256) =", crsysapi.Cnv.tohex(md))
+    assert(crsysapi.Cnv.tohex(md) == "5B7EB772AECF04C74AF07D9D9C1C1F8D3A90DCDA00D5BAB1DC28DAECDC86EB87611E")
+    md = crsysapi.Xof.bytes(34, msg, crsysapi.Xof.Alg.MGF1_SHA512)
+    print("MD(mgf1_sha512) =", crsysapi.Cnv.tohex(md))
+
+
+def test_shortpathname():
+    print("\nTEST SHORTNAMEPATH...")
+    fname = "你好.txt"
+    write_text_file(fname, "你好")
+    print("filename =", fname)
+    shortname = crsysapi.Cnv.shortpathname(fname)
+    print("shortname=", shortname)
+    # Create an empty file with Unicode name for encrypted output
+    file_ct = "你好加密.enc"
+    write_text_file(file_ct, "")
+    key = crsysapi.Cnv.fromhex("fedcba9876543210fedcba9876543210")
+    iv = crsysapi.Rng.bytestring(crsysapi.Cipher.blockbytes(crsysapi.Cipher.Alg.AES128))
+    # Get shortname for output file
+    shortname_ct = crsysapi.Cnv.shortpathname(file_ct)
+    print("shortname_ct=", shortname_ct)
+    # Carry out file encryption using shortpath names
+    n = crsysapi.Cipher.file_encrypt(shortname_ct, shortname, key, iv, "aes128-ctr", opts=crsysapi.Cipher.Opts.PREFIXIV)
+    assert(n == 0)
+    # Note we can use the Unicode name with pure Python functions,
+    # but we must use the shortpathname when calling cryptosyspki functions.
+    print(file_ct + ":",)
+    _print_file_hex(file_ct)
+
+    file_chk = "nihao.aes128.chk.txt"
+    # Use shortpathname for filein argument
+    n = crsysapi.Cipher.file_decrypt(file_chk, shortname_ct, key, None, "aes128-ctr", opts=crsysapi.Cipher.Opts.PREFIXIV)
+    assert(n == 0)
+    print(file_chk + ":",)
+    _print_file(file_chk)
+    # check files are equal
+    assert(read_binary_file(fname) == read_binary_file(file_chk))
+
+
 def quick_version():
     print("\nDETAILS OF CORE DLL...")
     print("DLL Version=" + str(crsysapi.Gen.version())
           + " [" + crsysapi.Gen.core_platform() + "] Lic="
           + crsysapi.Gen.licence_type()
           + " Compiled=["
           + crsysapi.Gen.compile_time() + "]")
+    print("[" + crsysapi.Gen.module_info() + "]")
     print("[" + crsysapi.Gen.module_name() + "]")
 
 
 def main():
-    # TODO:
-    # for arg in sys.argv:
-    #     global delete_tmp_dir
-    #     if (arg == 'nodelete'):
-    #         delete_tmp_dir = False
-    #     elif (arg == 'some'):
-    #         do_all = False
-    # setup_temp_dir()
+    # Act on any arguments in command line
+    do_all = True
+    for arg in sys.argv:
+        if (arg == 'some'):
+            do_all = False
+    setup_work_dir()
 
     # DO THE TESTS - EITHER SOME OR ALL
     if (do_all):
+        print("DOING ALL TESTS...")
         test_error_lookup()
         test_cnv()
         test_cipher()
         test_cipher_hex()
         test_cipher_file()
         test_cipher_block()
         test_cipher_pad()
         test_crc()
         test_rng()
         test_hash()
+        test_hash_bits()
+        test_hash_length()
         test_mac()
         test_prf()
         test_xof()
         test_wipe()
         test_compress()
         test_blowfish()
         test_pbe()
         test_aead()
         test_cipherstream()
+        test_keywrap()
+        test_ascon_aead()
+        test_ascon_hash()
+        test_ascon_xof()
+        test_xof_mgf1()
+        test_shortpathname()
 
     else:   # just do some tests: comment out as necessary
+        print("DOING SOME TESTS...")
         # test_error_lookup()
         # test_cnv()
         # test_cipher()
         # test_cipher_hex()
         # test_cipher_block()
         # test_cipher_file()
-        test_cipher_pad()
+        # test_cipher_pad()
         # test_crc()
         # test_rng()
         # test_hash()
+        # test_hash_length()
+        # test_hash_bits()
         # test_mac()
         # test_prf()
         # test_xof()
         # test_wipe()
         # test_compress()
         # test_blowfish()
         # test_pbe()
         # test_aead()
         # test_cipherstream()
+        test_keywrap()
+        # test_ascon_aead()
+        # test_ascon_hash()
+        # test_ascon_xof()
+        # test_xof_mgf1()
+        # test_shortpathname()
 
-        # ## reset_start_dir()
+    reset_start_dir()
     quick_version()
     print("crsysapi.__version__=", crsysapi.__version__)
     print("ALL DONE.")
 
 
 if __name__ == "__main__":
     main()
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

