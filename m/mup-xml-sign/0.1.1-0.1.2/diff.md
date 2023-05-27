# Comparing `tmp/mup-xml-sign-0.1.1.tar.gz` & `tmp/mup-xml-sign-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mup-xml-sign-0.1.1.tar", last modified: Sat May 27 18:07:10 2023, max compression
+gzip compressed data, was "mup-xml-sign-0.1.2.tar", last modified: Sat May 27 18:13:25 2023, max compression
```

## Comparing `mup-xml-sign-0.1.1.tar` & `mup-xml-sign-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sergei     (501) staff       (20)        0 2023-05-27 18:07:10.108715 mup-xml-sign-0.1.1/
--rw-r--r--   0 sergei     (501) staff       (20)       40 2023-05-27 17:53:56.000000 mup-xml-sign-0.1.1/MANIFEST.in
--rw-r--r--   0 sergei     (501) staff       (20)      273 2023-05-27 18:07:10.108508 mup-xml-sign-0.1.1/PKG-INFO
--rw-r--r--   0 sergei     (501) staff       (20)     1377 2023-05-27 18:00:19.000000 mup-xml-sign-0.1.1/README.md
-drwxr-xr-x   0 sergei     (501) staff       (20)        0 2023-05-27 18:07:10.103824 mup-xml-sign-0.1.1/bin/
--rw-r--r--   0 sergei     (501) staff       (20)       89 2023-05-27 17:40:51.000000 mup-xml-sign-0.1.1/bin/mup-xml-sign
-drwxr-xr-x   0 sergei     (501) staff       (20)        0 2023-05-27 18:07:10.107325 mup-xml-sign-0.1.1/mup_xml_sign/
--rw-r--r--   0 sergei     (501) staff       (20)  1584992 2023-05-27 08:13:40.000000 mup-xml-sign-0.1.1/mup_xml_sign/libnstpkcs11.dylib
--rw-r--r--   0 sergei     (501) staff       (20)     5458 2023-05-27 09:25:36.000000 mup-xml-sign-0.1.1/mup_xml_sign/mup_xml_sign.py
-drwxr-xr-x   0 sergei     (501) staff       (20)        0 2023-05-27 18:07:10.108313 mup-xml-sign-0.1.1/mup_xml_sign.egg-info/
--rw-r--r--   0 sergei     (501) staff       (20)      273 2023-05-27 18:07:10.000000 mup-xml-sign-0.1.1/mup_xml_sign.egg-info/PKG-INFO
--rw-r--r--   0 sergei     (501) staff       (20)      287 2023-05-27 18:07:10.000000 mup-xml-sign-0.1.1/mup_xml_sign.egg-info/SOURCES.txt
--rw-r--r--   0 sergei     (501) staff       (20)        1 2023-05-27 18:07:10.000000 mup-xml-sign-0.1.1/mup_xml_sign.egg-info/dependency_links.txt
--rw-r--r--   0 sergei     (501) staff       (20)       54 2023-05-27 18:07:10.000000 mup-xml-sign-0.1.1/mup_xml_sign.egg-info/requires.txt
--rw-r--r--   0 sergei     (501) staff       (20)       13 2023-05-27 18:07:10.000000 mup-xml-sign-0.1.1/mup_xml_sign.egg-info/top_level.txt
--rw-r--r--   0 sergei     (501) staff       (20)       38 2023-05-27 18:07:10.108775 mup-xml-sign-0.1.1/setup.cfg
--rw-r--r--   0 sergei     (501) staff       (20)      516 2023-05-27 18:06:52.000000 mup-xml-sign-0.1.1/setup.py
+drwxr-xr-x   0 sergei     (501) staff       (20)        0 2023-05-27 18:13:25.603437 mup-xml-sign-0.1.2/
+-rw-r--r--   0 sergei     (501) staff       (20)       40 2023-05-27 17:53:56.000000 mup-xml-sign-0.1.2/MANIFEST.in
+-rw-r--r--   0 sergei     (501) staff       (20)      273 2023-05-27 18:13:25.603201 mup-xml-sign-0.1.2/PKG-INFO
+-rw-r--r--   0 sergei     (501) staff       (20)     1377 2023-05-27 18:00:19.000000 mup-xml-sign-0.1.2/README.md
+drwxr-xr-x   0 sergei     (501) staff       (20)        0 2023-05-27 18:13:25.598835 mup-xml-sign-0.1.2/bin/
+-rw-r--r--   0 sergei     (501) staff       (20)       89 2023-05-27 17:40:51.000000 mup-xml-sign-0.1.2/bin/mup-xml-sign
+drwxr-xr-x   0 sergei     (501) staff       (20)        0 2023-05-27 18:13:25.602010 mup-xml-sign-0.1.2/mup_xml_sign/
+-rw-r--r--   0 sergei     (501) staff       (20)  1584992 2023-05-27 08:13:40.000000 mup-xml-sign-0.1.2/mup_xml_sign/libnstpkcs11.dylib
+-rw-r--r--   0 sergei     (501) staff       (20)     5458 2023-05-27 09:25:36.000000 mup-xml-sign-0.1.2/mup_xml_sign/mup_xml_sign.py
+drwxr-xr-x   0 sergei     (501) staff       (20)        0 2023-05-27 18:13:25.602980 mup-xml-sign-0.1.2/mup_xml_sign.egg-info/
+-rw-r--r--   0 sergei     (501) staff       (20)      273 2023-05-27 18:13:25.000000 mup-xml-sign-0.1.2/mup_xml_sign.egg-info/PKG-INFO
+-rw-r--r--   0 sergei     (501) staff       (20)      287 2023-05-27 18:13:25.000000 mup-xml-sign-0.1.2/mup_xml_sign.egg-info/SOURCES.txt
+-rw-r--r--   0 sergei     (501) staff       (20)        1 2023-05-27 18:13:25.000000 mup-xml-sign-0.1.2/mup_xml_sign.egg-info/dependency_links.txt
+-rw-r--r--   0 sergei     (501) staff       (20)       54 2023-05-27 18:13:25.000000 mup-xml-sign-0.1.2/mup_xml_sign.egg-info/requires.txt
+-rw-r--r--   0 sergei     (501) staff       (20)       13 2023-05-27 18:13:25.000000 mup-xml-sign-0.1.2/mup_xml_sign.egg-info/top_level.txt
+-rw-r--r--   0 sergei     (501) staff       (20)       38 2023-05-27 18:13:25.603501 mup-xml-sign-0.1.2/setup.cfg
+-rw-r--r--   0 sergei     (501) staff       (20)      516 2023-05-27 18:13:16.000000 mup-xml-sign-0.1.2/setup.py
```

### Comparing `mup-xml-sign-0.1.1/README.md` & `mup-xml-sign-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mup-xml-sign-0.1.1/mup_xml_sign/libnstpkcs11.dylib` & `mup-xml-sign-0.1.2/mup_xml_sign/libnstpkcs11.dylib`

 * *Files identical despite different names*

### Comparing `mup-xml-sign-0.1.1/mup_xml_sign/mup_xml_sign.py` & `mup-xml-sign-0.1.2/mup_xml_sign/mup_xml_sign.py`

 * *Files identical despite different names*

### Comparing `mup-xml-sign-0.1.1/setup.py` & `mup-xml-sign-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(name='mup-xml-sign',
-    version='0.1.1',
+    version='0.1.2',
     description='mup-xml-sign',
     url='http://github.com/SergeiPatiakin/mup-xml-sign',
     author='Sergei Patiakin',
     author_email='sergei.patiakin@gmail.com',
     license='Public Domain',
     packages=['mup_xml_sign'],
     scripts=['bin/mup-xml-sign'],
     python_requires='>=3.7',
     install_requires=[
         'cryptography~=40.0.2',
         'lxml~=4.9.2',
         'python-pkcs11~=0.7.0',
     ],
-    install_package_data=True,
+    include_package_data=True,
 )
```

