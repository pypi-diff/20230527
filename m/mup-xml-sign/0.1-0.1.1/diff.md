# Comparing `tmp/mup-xml-sign-0.1.tar.gz` & `tmp/mup-xml-sign-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mup-xml-sign-0.1.tar", last modified: Sat May 27 17:55:21 2023, max compression
+gzip compressed data, was "mup-xml-sign-0.1.1.tar", last modified: Sat May 27 18:07:10 2023, max compression
```

## Comparing `mup-xml-sign-0.1.tar` & `mup-xml-sign-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sergei     (501) staff       (20)        0 2023-05-27 17:55:21.373175 mup-xml-sign-0.1/
--rw-r--r--   0 sergei     (501) staff       (20)       40 2023-05-27 17:53:56.000000 mup-xml-sign-0.1/MANIFEST.in
--rw-r--r--   0 sergei     (501) staff       (20)      271 2023-05-27 17:55:21.372976 mup-xml-sign-0.1/PKG-INFO
--rw-r--r--   0 sergei     (501) staff       (20)     1280 2023-05-27 17:47:03.000000 mup-xml-sign-0.1/README.md
-drwxr-xr-x   0 sergei     (501) staff       (20)        0 2023-05-27 17:55:21.367531 mup-xml-sign-0.1/bin/
--rw-r--r--   0 sergei     (501) staff       (20)       89 2023-05-27 17:40:51.000000 mup-xml-sign-0.1/bin/mup-xml-sign
-drwxr-xr-x   0 sergei     (501) staff       (20)        0 2023-05-27 17:55:21.372002 mup-xml-sign-0.1/mup_xml_sign/
--rw-r--r--   0 sergei     (501) staff       (20)  1584992 2023-05-27 08:13:40.000000 mup-xml-sign-0.1/mup_xml_sign/libnstpkcs11.dylib
--rw-r--r--   0 sergei     (501) staff       (20)     5458 2023-05-27 09:25:36.000000 mup-xml-sign-0.1/mup_xml_sign/mup_xml_sign.py
-drwxr-xr-x   0 sergei     (501) staff       (20)        0 2023-05-27 17:55:21.372787 mup-xml-sign-0.1/mup_xml_sign.egg-info/
--rw-r--r--   0 sergei     (501) staff       (20)      271 2023-05-27 17:55:21.000000 mup-xml-sign-0.1/mup_xml_sign.egg-info/PKG-INFO
--rw-r--r--   0 sergei     (501) staff       (20)      287 2023-05-27 17:55:21.000000 mup-xml-sign-0.1/mup_xml_sign.egg-info/SOURCES.txt
--rw-r--r--   0 sergei     (501) staff       (20)        1 2023-05-27 17:55:21.000000 mup-xml-sign-0.1/mup_xml_sign.egg-info/dependency_links.txt
--rw-r--r--   0 sergei     (501) staff       (20)       54 2023-05-27 17:55:21.000000 mup-xml-sign-0.1/mup_xml_sign.egg-info/requires.txt
--rw-r--r--   0 sergei     (501) staff       (20)       13 2023-05-27 17:55:21.000000 mup-xml-sign-0.1/mup_xml_sign.egg-info/top_level.txt
--rw-r--r--   0 sergei     (501) staff       (20)       38 2023-05-27 17:55:21.373221 mup-xml-sign-0.1/setup.cfg
--rw-r--r--   0 sergei     (501) staff       (20)      482 2023-05-27 17:44:57.000000 mup-xml-sign-0.1/setup.py
+drwxr-xr-x   0 sergei     (501) staff       (20)        0 2023-05-27 18:07:10.108715 mup-xml-sign-0.1.1/
+-rw-r--r--   0 sergei     (501) staff       (20)       40 2023-05-27 17:53:56.000000 mup-xml-sign-0.1.1/MANIFEST.in
+-rw-r--r--   0 sergei     (501) staff       (20)      273 2023-05-27 18:07:10.108508 mup-xml-sign-0.1.1/PKG-INFO
+-rw-r--r--   0 sergei     (501) staff       (20)     1377 2023-05-27 18:00:19.000000 mup-xml-sign-0.1.1/README.md
+drwxr-xr-x   0 sergei     (501) staff       (20)        0 2023-05-27 18:07:10.103824 mup-xml-sign-0.1.1/bin/
+-rw-r--r--   0 sergei     (501) staff       (20)       89 2023-05-27 17:40:51.000000 mup-xml-sign-0.1.1/bin/mup-xml-sign
+drwxr-xr-x   0 sergei     (501) staff       (20)        0 2023-05-27 18:07:10.107325 mup-xml-sign-0.1.1/mup_xml_sign/
+-rw-r--r--   0 sergei     (501) staff       (20)  1584992 2023-05-27 08:13:40.000000 mup-xml-sign-0.1.1/mup_xml_sign/libnstpkcs11.dylib
+-rw-r--r--   0 sergei     (501) staff       (20)     5458 2023-05-27 09:25:36.000000 mup-xml-sign-0.1.1/mup_xml_sign/mup_xml_sign.py
+drwxr-xr-x   0 sergei     (501) staff       (20)        0 2023-05-27 18:07:10.108313 mup-xml-sign-0.1.1/mup_xml_sign.egg-info/
+-rw-r--r--   0 sergei     (501) staff       (20)      273 2023-05-27 18:07:10.000000 mup-xml-sign-0.1.1/mup_xml_sign.egg-info/PKG-INFO
+-rw-r--r--   0 sergei     (501) staff       (20)      287 2023-05-27 18:07:10.000000 mup-xml-sign-0.1.1/mup_xml_sign.egg-info/SOURCES.txt
+-rw-r--r--   0 sergei     (501) staff       (20)        1 2023-05-27 18:07:10.000000 mup-xml-sign-0.1.1/mup_xml_sign.egg-info/dependency_links.txt
+-rw-r--r--   0 sergei     (501) staff       (20)       54 2023-05-27 18:07:10.000000 mup-xml-sign-0.1.1/mup_xml_sign.egg-info/requires.txt
+-rw-r--r--   0 sergei     (501) staff       (20)       13 2023-05-27 18:07:10.000000 mup-xml-sign-0.1.1/mup_xml_sign.egg-info/top_level.txt
+-rw-r--r--   0 sergei     (501) staff       (20)       38 2023-05-27 18:07:10.108775 mup-xml-sign-0.1.1/setup.cfg
+-rw-r--r--   0 sergei     (501) staff       (20)      516 2023-05-27 18:06:52.000000 mup-xml-sign-0.1.1/setup.py
```

### Comparing `mup-xml-sign-0.1/README.md` & `mup-xml-sign-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 # Installation
 
 This tool must be run with x86 Python in order to be compatible with x86 PKCS11 libraries.
 - Find an Intel-only Python installer on https://www.python.org/downloads/
 - Install it. Note the installation location such as `/Library/Frameworks/Python.framework/Versions/3.9`
 - Use the newly installed pip instance to install mup-xml-sign: `/Library/Frameworks/Python.framework/Versions/3.9/bin/pip3 install mup-xml-sign`
-
+- The tools is now installed at `/Library/Frameworks/Python.framework/Versions/3.9/bin/mup-xml-sign`
 # Usage
 
 - Locate the path of your unsigned XML file, such as `/path/to/unsigned.xml`
 - Choose a path for your signed XML file, such as `/path/to/signed.xml`
 - Insert MUP-issued smart card into card reader
 - Run the tool:
 
 ```
-/Library/Frameworks/Python.framework/Versions/3.9/bin/python3 sign.py -i /path/to/unsigned.xml -o /path/to/signed.xml
+/Library/Frameworks/Python.framework/Versions/3.9/bin/mup-xml-sign -i /path/to/unsigned.xml -o /path/to/signed.xml
 ```
 
 - If you have multiple card readers, you will be prompted to choose one interactively
 - If you have multiple certificates, you will be prompted to choose one interactively
 - You will be prompted for your PIN interactively
 - The signed XML will be written to `/path/to/signed.xml`
```

### Comparing `mup-xml-sign-0.1/mup_xml_sign/libnstpkcs11.dylib` & `mup-xml-sign-0.1.1/mup_xml_sign/libnstpkcs11.dylib`

 * *Files identical despite different names*

### Comparing `mup-xml-sign-0.1/mup_xml_sign/mup_xml_sign.py` & `mup-xml-sign-0.1.1/mup_xml_sign/mup_xml_sign.py`

 * *Files identical despite different names*

