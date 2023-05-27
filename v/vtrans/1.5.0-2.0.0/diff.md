# Comparing `tmp/vtrans-1.5.0.tar.gz` & `tmp/vtrans-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtrans-1.5.0.tar", last modified: Sat May 27 10:47:51 2023, max compression
+gzip compressed data, was "vtrans-2.0.0.tar", last modified: Sat May 27 11:09:48 2023, max compression
```

## Comparing `vtrans-1.5.0.tar` & `vtrans-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 10:47:51.626632 vtrans-1.5.0/
--rw-rw-rw-   0        0        0       82 2023-05-27 10:46:49.000000 vtrans-1.5.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-05-27 08:21:58.000000 vtrans-1.5.0/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-05-27 08:18:00.000000 vtrans-1.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1786 2023-05-27 10:47:51.622634 vtrans-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      899 2023-05-27 09:44:39.000000 vtrans-1.5.0/README.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 10:47:51.628643 vtrans-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1120 2023-05-27 10:45:52.000000 vtrans-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 10:47:51.508459 vtrans-1.5.0/vtrans/
--rw-rw-rw-   0        0        0     9157 2023-05-27 10:46:01.000000 vtrans-1.5.0/vtrans/__init__.py
--rw-rw-rw-   0        0        0       58 2023-05-27 07:48:30.000000 vtrans-1.5.0/vtrans/config.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 10:47:51.607605 vtrans-1.5.0/vtrans.egg-info/
--rw-rw-rw-   0        0        0     1786 2023-05-27 10:47:50.000000 vtrans-1.5.0/vtrans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-05-27 10:47:51.000000 vtrans-1.5.0/vtrans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 10:47:50.000000 vtrans-1.5.0/vtrans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-27 10:47:50.000000 vtrans-1.5.0/vtrans.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-27 10:47:50.000000 vtrans-1.5.0/vtrans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 11:09:48.445428 vtrans-2.0.0/
+-rw-rw-rw-   0        0        0       82 2023-05-27 11:05:51.000000 vtrans-2.0.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-05-27 08:21:58.000000 vtrans-2.0.0/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-05-27 08:18:00.000000 vtrans-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1786 2023-05-27 11:09:48.443421 vtrans-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      899 2023-05-27 09:44:39.000000 vtrans-2.0.0/README.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 11:09:48.447432 vtrans-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1120 2023-05-27 11:06:06.000000 vtrans-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:09:48.363307 vtrans-2.0.0/vtrans/
+-rw-rw-rw-   0        0        0     9512 2023-05-27 11:09:14.000000 vtrans-2.0.0/vtrans/__init__.py
+-rw-rw-rw-   0        0        0       58 2023-05-27 07:48:30.000000 vtrans-2.0.0/vtrans/config.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 11:09:48.435412 vtrans-2.0.0/vtrans.egg-info/
+-rw-rw-rw-   0        0        0     1786 2023-05-27 11:09:47.000000 vtrans-2.0.0/vtrans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-05-27 11:09:48.000000 vtrans-2.0.0/vtrans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 11:09:47.000000 vtrans-2.0.0/vtrans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-27 11:09:47.000000 vtrans-2.0.0/vtrans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-27 11:09:47.000000 vtrans-2.0.0/vtrans.egg-info/top_level.txt
```

### Comparing `vtrans-1.5.0/LICENCE.txt` & `vtrans-2.0.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `vtrans-1.5.0/PKG-INFO` & `vtrans-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtrans
-Version: 1.5.0
+Version: 2.0.0
 Summary: This is a self-updating translator powered by Google Translate for free and unlimited usage.
 Home-page: https://github.com/megalosVigneswaran/vtrans/tree/main/vtrans
 Author: S.Vigneswaran
 Author-email: t896242@gmail.com
 License: MIT
 Keywords: translator,googletranslate,self-updating,googletrans
 Classifier: Development Status :: 5 - Production/Stable
@@ -40,11 +40,11 @@
 So it have more langauges.
 
 If google update their langauges in google translate it update it self.
 
 Change log
 ==========
 
-1.5.0(27/05/2023)
+2.0.0(27/05/2023)
 -------------------
 
 -First Release
```

### Comparing `vtrans-1.5.0/README.txt` & `vtrans-2.0.0/README.txt`

 * *Files identical despite different names*

### Comparing `vtrans-1.5.0/setup.py` & `vtrans-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 8',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='vtrans',
-  version='1.5.0',
+  version='2.0.0',
   description='This is a self-updating translator powered by Google Translate for free and unlimited usage.',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='https://github.com/megalosVigneswaran/vtrans/tree/main/vtrans',  
   author='S.Vigneswaran',
   author_email='t896242@gmail.com',
   license='MIT',
   classifiers=classifiers,
```

### Comparing `vtrans-1.5.0/vtrans/__init__.py` & `vtrans-2.0.0/vtrans/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     
     IT CHECK UPDATING IN EVERY IMPORT OF THIS LIBRARY IT MAKE IT LITTLE BIT SLOWER,
     
     BUT YOU CAN DISABLE AUTOUPDATE CHECKING BY THIS CODE '''vtrans.config(auto_updating = False)'''."""
 
 __Author__ = "S.Vigneswaran"
 
-__Version__ = 1.5
-
+__Version__ = 2.0
 
+import os
 
 """ This function is helps to set optional settings of this translator 
        
     it helps to disable the autoupdating"""
 def config(auto_updating='True'):
     #Convert auto_updating value to string
     auto_updating = str(auto_updating)
@@ -204,14 +204,24 @@
 
     print("Update finished. Now you can use extra languages.")
 
 def ready(data):
     if data['print'] == 'True':
         print("ready to translate")
 
+confile_path = get_sitePackages_path()
+confile_path = confile_path + "vtrans\\config.txt"
+if os.path.isfile(confile_path):
+    file_vai = "ok"
+else:
+    print("setup config file")
+    pattern = {'print':'True','autoupdate':'True','original_lang':'107'}
+    with open(confile_path,'w') as new_file:
+        new_file.write(str(pattern))
+
 data =check_con() #get confile data
 
 if data['autoupdate'] == 'True': #if the autoupdate value id 'true'
     update_chacker() #check the update
 
 from googletrans import Translator #import Translator 
 from googletrans import LANGCODES, LANGUAGES #import LANGCODE and LANGAUGES
```

### Comparing `vtrans-1.5.0/vtrans.egg-info/PKG-INFO` & `vtrans-2.0.0/vtrans.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtrans
-Version: 1.5.0
+Version: 2.0.0
 Summary: This is a self-updating translator powered by Google Translate for free and unlimited usage.
 Home-page: https://github.com/megalosVigneswaran/vtrans/tree/main/vtrans
 Author: S.Vigneswaran
 Author-email: t896242@gmail.com
 License: MIT
 Keywords: translator,googletranslate,self-updating,googletrans
 Classifier: Development Status :: 5 - Production/Stable
@@ -40,11 +40,11 @@
 So it have more langauges.
 
 If google update their langauges in google translate it update it self.
 
 Change log
 ==========
 
-1.5.0(27/05/2023)
+2.0.0(27/05/2023)
 -------------------
 
 -First Release
```

