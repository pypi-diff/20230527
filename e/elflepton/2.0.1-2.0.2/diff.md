# Comparing `tmp/elflepton-2.0.1.tar.gz` & `tmp/elflepton-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elflepton-2.0.1.tar", last modified: Sun Apr  2 01:38:58 2023, max compression
+gzip compressed data, was "elflepton-2.0.2.tar", last modified: Sat May 27 16:30:22 2023, max compression
```

## Comparing `elflepton-2.0.1.tar` & `elflepton-2.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 nikhilh   (1000) nikhilh   (1000)        0 2023-04-02 01:38:58.355702 elflepton-2.0.1/
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     1127 2023-03-30 04:43:43.000000 elflepton-2.0.1/LICENSE
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     6601 2023-04-02 01:38:58.355702 elflepton-2.0.1/PKG-INFO
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     6441 2023-03-30 04:43:43.000000 elflepton-2.0.1/README.md
-drwxrwxr-x   0 nikhilh   (1000) nikhilh   (1000)        0 2023-04-02 01:38:58.347702 elflepton-2.0.1/elflepton.egg-info/
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     6601 2023-04-02 01:38:58.000000 elflepton-2.0.1/elflepton.egg-info/PKG-INFO
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)      552 2023-04-02 01:38:58.000000 elflepton-2.0.1/elflepton.egg-info/SOURCES.txt
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)        1 2023-04-02 01:38:58.000000 elflepton-2.0.1/elflepton.egg-info/dependency_links.txt
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)        7 2023-04-02 01:38:58.000000 elflepton-2.0.1/elflepton.egg-info/top_level.txt
-drwxrwxr-x   0 nikhilh   (1000) nikhilh   (1000)        0 2023-04-02 01:38:58.351702 elflepton-2.0.1/lepton/
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)        0 2023-03-30 04:43:43.000000 elflepton-2.0.1/lepton/__init__.py
-drwxrwxr-x   0 nikhilh   (1000) nikhilh   (1000)        0 2023-04-02 01:38:58.355702 elflepton-2.0.1/lepton/arch/
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)        0 2023-03-30 04:43:43.000000 elflepton-2.0.1/lepton/arch/__init__.py
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)      509 2023-03-30 04:43:43.000000 elflepton-2.0.1/lepton/arch/amd64.py
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)      508 2023-03-30 04:43:43.000000 elflepton-2.0.1/lepton/arch/arm.py
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)      506 2023-03-30 04:43:43.000000 elflepton-2.0.1/lepton/arch/i386.py
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     1084 2023-03-30 04:43:43.000000 elflepton-2.0.1/lepton/arch/mappings.py
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     2412 2023-03-30 04:43:43.000000 elflepton-2.0.1/lepton/arch/mips.py
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)      507 2023-03-30 04:43:43.000000 elflepton-2.0.1/lepton/arch/ppc.py
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)    22272 2023-03-30 04:43:43.000000 elflepton-2.0.1/lepton/elfheader.py
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)    11401 2023-03-30 04:43:43.000000 elflepton-2.0.1/lepton/elfprogramheader.py
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)    27408 2023-03-31 02:01:29.000000 elflepton-2.0.1/lepton/elfsectionheader.py
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     3876 2023-03-30 04:43:43.000000 elflepton-2.0.1/lepton/embeddedelf.py
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     4111 2023-03-30 04:43:43.000000 elflepton-2.0.1/lepton/lepton.py
-drwxrwxr-x   0 nikhilh   (1000) nikhilh   (1000)        0 2023-04-02 01:38:58.355702 elflepton-2.0.1/lepton/utils/
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)        0 2023-03-30 04:43:43.000000 elflepton-2.0.1/lepton/utils/__init__.py
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     2231 2023-03-30 04:43:43.000000 elflepton-2.0.1/lepton/utils/constants.py
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     1026 2023-03-30 04:43:43.000000 elflepton-2.0.1/lepton/utils/exceptions.py
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     2047 2023-03-30 04:43:43.000000 elflepton-2.0.1/lepton/utils/structures.py
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)      103 2023-04-02 01:38:58.359702 elflepton-2.0.1/setup.cfg
--rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)      493 2023-03-31 02:05:20.000000 elflepton-2.0.1/setup.py
+drwxrwxr-x   0 nikhilh   (1000) nikhilh   (1000)        0 2023-05-27 16:30:22.204994 elflepton-2.0.2/
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     1127 2023-03-30 04:43:43.000000 elflepton-2.0.2/LICENSE
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     6601 2023-05-27 16:30:22.204994 elflepton-2.0.2/PKG-INFO
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     6441 2023-03-30 04:43:43.000000 elflepton-2.0.2/README.md
+drwxrwxr-x   0 nikhilh   (1000) nikhilh   (1000)        0 2023-05-27 16:30:22.200994 elflepton-2.0.2/elflepton.egg-info/
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     6601 2023-05-27 16:30:22.000000 elflepton-2.0.2/elflepton.egg-info/PKG-INFO
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)      552 2023-05-27 16:30:22.000000 elflepton-2.0.2/elflepton.egg-info/SOURCES.txt
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)        1 2023-05-27 16:30:22.000000 elflepton-2.0.2/elflepton.egg-info/dependency_links.txt
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)        7 2023-05-27 16:30:22.000000 elflepton-2.0.2/elflepton.egg-info/top_level.txt
+drwxrwxr-x   0 nikhilh   (1000) nikhilh   (1000)        0 2023-05-27 16:30:22.204994 elflepton-2.0.2/lepton/
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)        0 2023-03-30 04:43:43.000000 elflepton-2.0.2/lepton/__init__.py
+drwxrwxr-x   0 nikhilh   (1000) nikhilh   (1000)        0 2023-05-27 16:30:22.204994 elflepton-2.0.2/lepton/arch/
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)        0 2023-03-30 04:43:43.000000 elflepton-2.0.2/lepton/arch/__init__.py
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)      509 2023-03-30 04:43:43.000000 elflepton-2.0.2/lepton/arch/amd64.py
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)      508 2023-03-30 04:43:43.000000 elflepton-2.0.2/lepton/arch/arm.py
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)      506 2023-03-30 04:43:43.000000 elflepton-2.0.2/lepton/arch/i386.py
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     1084 2023-03-30 04:43:43.000000 elflepton-2.0.2/lepton/arch/mappings.py
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     2412 2023-03-30 04:43:43.000000 elflepton-2.0.2/lepton/arch/mips.py
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)      507 2023-03-30 04:43:43.000000 elflepton-2.0.2/lepton/arch/ppc.py
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)    22272 2023-03-30 04:43:43.000000 elflepton-2.0.2/lepton/elfheader.py
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)    11401 2023-03-30 04:43:43.000000 elflepton-2.0.2/lepton/elfprogramheader.py
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)    27433 2023-05-27 16:22:29.000000 elflepton-2.0.2/lepton/elfsectionheader.py
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     3876 2023-03-30 04:43:43.000000 elflepton-2.0.2/lepton/embeddedelf.py
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     4111 2023-05-27 16:28:28.000000 elflepton-2.0.2/lepton/lepton.py
+drwxrwxr-x   0 nikhilh   (1000) nikhilh   (1000)        0 2023-05-27 16:30:22.204994 elflepton-2.0.2/lepton/utils/
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)        0 2023-03-30 04:43:43.000000 elflepton-2.0.2/lepton/utils/__init__.py
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     2231 2023-03-30 04:43:43.000000 elflepton-2.0.2/lepton/utils/constants.py
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     1026 2023-03-30 04:43:43.000000 elflepton-2.0.2/lepton/utils/exceptions.py
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)     2047 2023-03-30 04:43:43.000000 elflepton-2.0.2/lepton/utils/structures.py
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)      103 2023-05-27 16:30:22.204994 elflepton-2.0.2/setup.cfg
+-rw-rw-r--   0 nikhilh   (1000) nikhilh   (1000)      493 2023-05-27 16:29:14.000000 elflepton-2.0.2/setup.py
```

### Comparing `elflepton-2.0.1/LICENSE` & `elflepton-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `elflepton-2.0.1/PKG-INFO` & `elflepton-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elflepton
-Version: 2.0.1
+Version: 2.0.2
 Summary: Parse an ELF binary with corrupted ELF headers.
 Home-page: https://github.com/nikhilh-20/lepton
 Author: Nikhil Ashok Hegde
 Author-email: nikhilhegde20@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `elflepton-2.0.1/README.md` & `elflepton-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `elflepton-2.0.1/elflepton.egg-info/PKG-INFO` & `elflepton-2.0.2/elflepton.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elflepton
-Version: 2.0.1
+Version: 2.0.2
 Summary: Parse an ELF binary with corrupted ELF headers.
 Home-page: https://github.com/nikhilh-20/lepton
 Author: Nikhil Ashok Hegde
 Author-email: nikhilhegde20@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `elflepton-2.0.1/elflepton.egg-info/SOURCES.txt` & `elflepton-2.0.2/elflepton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elflepton-2.0.1/lepton/arch/mappings.py` & `elflepton-2.0.2/lepton/arch/mappings.py`

 * *Files identical despite different names*

### Comparing `elflepton-2.0.1/lepton/arch/mips.py` & `elflepton-2.0.2/lepton/arch/mips.py`

 * *Files identical despite different names*

### Comparing `elflepton-2.0.1/lepton/elfheader.py` & `elflepton-2.0.2/lepton/elfheader.py`

 * *Files identical despite different names*

### Comparing `elflepton-2.0.1/lepton/elfprogramheader.py` & `elflepton-2.0.2/lepton/elfprogramheader.py`

 * *Files identical despite different names*

### Comparing `elflepton-2.0.1/lepton/elfsectionheader.py` & `elflepton-2.0.2/lepton/elfsectionheader.py`

 * *Files 0% similar despite different names*

```diff
@@ -445,26 +445,29 @@
         if new_header:
             shentsize = unpack(f"{self.endian}H", elfheader["e_shentsize"])[0]
             sh_num, sh_off = self.find_section_header_table(data, shentsize,
                                                             ei_class)
             shstrndx = self.find_section_name_string_table(data, sh_num, sh_off,
                                                            shentsize, ei_class)
 
+        if ei_class == 1:
+            elfheader["e_shnum"], elfheader["e_shoff"], elfheader["e_shstrndx"] = \
+                pack(f"{self.endian}H", sh_num), pack(f"{self.endian}I", sh_off), pack(f"{self.endian}H", shstrndx)
+        else:
+            elfheader["e_shnum"], elfheader["e_shoff"], elfheader["e_shstrndx"] = \
+                pack(f"{self.endian}H", sh_num), pack(f"{self.endian}Q", sh_off), pack(f"{self.endian}H", shstrndx)
+
         for shdr_num in range(sh_num):
             if ei_class == 1:
-                elfheader["e_shnum"], elfheader["e_shoff"], elfheader["e_shstrndx"] = \
-                    pack(f"{self.endian}H", sh_num), pack(f"{self.endian}I", sh_off), pack(f"{self.endian}H", shstrndx)
                 try:
                     shdr = self._build_shdr(data, structures.ELF32SECTIONHEADER,
                                             sh_off, shdr_num, shentsize)
                 except error:
                     continue
             else:
-                elfheader["e_shnum"], elfheader["e_shoff"], elfheader["e_shstrndx"] = \
-                    pack(f"{self.endian}H", sh_num), pack(f"{self.endian}Q", sh_off), pack(f"{self.endian}H", shstrndx)
                 try:
                     shdr = self._build_shdr(data, structures.ELF64SECTIONHEADER,
                                             sh_off, shdr_num, shentsize)
                 except error:
                     continue
 
             shdr_table.append(shdr)
```

### Comparing `elflepton-2.0.1/lepton/embeddedelf.py` & `elflepton-2.0.2/lepton/embeddedelf.py`

 * *Files identical despite different names*

### Comparing `elflepton-2.0.1/lepton/lepton.py` & `elflepton-2.0.2/lepton/lepton.py`

 * *Files identical despite different names*

### Comparing `elflepton-2.0.1/lepton/utils/constants.py` & `elflepton-2.0.2/lepton/utils/constants.py`

 * *Files identical despite different names*

### Comparing `elflepton-2.0.1/lepton/utils/exceptions.py` & `elflepton-2.0.2/lepton/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `elflepton-2.0.1/lepton/utils/structures.py` & `elflepton-2.0.2/lepton/utils/structures.py`

 * *Files identical despite different names*

