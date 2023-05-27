# Comparing `tmp/TimePrintOnPYPI-1.5.2.tar.gz` & `tmp/TimePrintOnPYPI-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimePrintOnPYPI-1.5.2.tar", last modified: Fri May 26 15:30:35 2023, max compression
+gzip compressed data, was "TimePrintOnPYPI-1.5.3.tar", last modified: Sat May 27 10:27:25 2023, max compression
```

## Comparing `TimePrintOnPYPI-1.5.2.tar` & `TimePrintOnPYPI-1.5.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 15:30:35.135335 TimePrintOnPYPI-1.5.2/
--rw-rw-rw-   0        0        0     4611 2023-05-26 15:30:35.135335 TimePrintOnPYPI-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     4121 2023-05-26 15:19:49.000000 TimePrintOnPYPI-1.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 15:30:35.114717 TimePrintOnPYPI-1.5.2/TimePrint/
--rw-rw-rw-   0        0        0     1744 2023-05-26 15:30:10.000000 TimePrintOnPYPI-1.5.2/TimePrint/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:30:35.132237 TimePrintOnPYPI-1.5.2/TimePrintOnPYPI.egg-info/
--rw-rw-rw-   0        0        0     4611 2023-05-26 15:30:35.000000 TimePrintOnPYPI-1.5.2/TimePrintOnPYPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-05-26 15:30:35.000000 TimePrintOnPYPI-1.5.2/TimePrintOnPYPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 15:30:35.000000 TimePrintOnPYPI-1.5.2/TimePrintOnPYPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-26 15:30:35.000000 TimePrintOnPYPI-1.5.2/TimePrintOnPYPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 15:30:35.136334 TimePrintOnPYPI-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1013 2023-05-26 15:30:17.000000 TimePrintOnPYPI-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:27:25.659808 TimePrintOnPYPI-1.5.3/
+-rw-rw-rw-   0        0        0     4611 2023-05-27 10:27:25.657798 TimePrintOnPYPI-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4121 2023-05-26 15:19:49.000000 TimePrintOnPYPI-1.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 10:27:25.640535 TimePrintOnPYPI-1.5.3/TimePrint/
+-rw-rw-rw-   0        0        0     1820 2023-05-27 10:27:17.000000 TimePrintOnPYPI-1.5.3/TimePrint/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:27:25.654782 TimePrintOnPYPI-1.5.3/TimePrintOnPYPI.egg-info/
+-rw-rw-rw-   0        0        0     4611 2023-05-27 10:27:25.000000 TimePrintOnPYPI-1.5.3/TimePrintOnPYPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-05-27 10:27:25.000000 TimePrintOnPYPI-1.5.3/TimePrintOnPYPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 10:27:25.000000 TimePrintOnPYPI-1.5.3/TimePrintOnPYPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-27 10:27:25.000000 TimePrintOnPYPI-1.5.3/TimePrintOnPYPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 10:27:25.660803 TimePrintOnPYPI-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2023-05-27 10:25:07.000000 TimePrintOnPYPI-1.5.3/setup.py
```

### Comparing `TimePrintOnPYPI-1.5.2/PKG-INFO` & `TimePrintOnPYPI-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimePrintOnPYPI
-Version: 1.5.2
+Version: 1.5.3
 Summary: A package for printing text with time delay between characters
 Home-page: https://github.com/SForces/TimePrint
 Author: Osman TUNA
 Author-email: osmntn08@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `TimePrintOnPYPI-1.5.2/README.md` & `TimePrintOnPYPI-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `TimePrintOnPYPI-1.5.2/TimePrint/__init__.py` & `TimePrintOnPYPI-1.5.3/TimePrint/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import time
 import sys
-def TP(seconds: int, text: str):
+def TP(seconds: int, text: str) -> str:
     """
     Usage;
 
     TimePrint.TP(seconds,"text")
 
     Example: TimePrint.TP(1,"Hello")
     Writes Hello In 1 Seconds
 
     """
     for character in text:
         sys.stdout.write(character)
         sys.stdout.flush()
         time.sleep(int(seconds)/len(text))
     print("")
-def P(text:str):
+def P(text:str) -> str:
     """
     Usage;
 
     TimePrint.P("text")
 
     For Example: TimePrint.P("Hello") Writes
 
@@ -31,26 +31,29 @@
     
     """
     for character in text:
         sys.stdout.write(character)
         sys.stdout.flush()
         time.sleep(0.001)
     print("")    
-def info():
+def info() -> str:
+    """
+    Just info about package.
+    """
     print("      _______ _____ __  __ ______     _____  _____  _____ _   _ _______  ")
     print("     |__   __|_   _|  \/  |  ____|   |  __ \|  __ \|_   _| \ | |__   __| ")
     print("        | |    | | | \  / | |__      | |__) | |__) | | | |  \| |  | |   ")
     print("        | |    | | | |\/| |  __|     |  ___/|  _  /  | | | . ` |  | |   ")
     print("        | |   _| |_| |  | | |____    | |    | | \ \ _| |_| |\  |  | |   ")
     print("        |_|  |_____|_|  |_|______|   |_|    |_|  \_\_____|_| \_|  |_|   ")
     print("\nAuthor: Osman TUNA")
     print("Author Email: osmntn08@gmail.com")
     print("Project Page: https://github.com/SForces/TimePrint")
-    print("Version: 1.5.2")
-def Timetag(format: str):
+    print("Version: 1.5.3")
+def Timetag(format: str) -> str:
     """
     Example Usages;
 
     "%H:%M" Returns --> 12:56 = (Hours:Minutes)
 
     "%H:%M:%S" Returns --> 12:56:24 = (Hours:Minutes:Seconds)
```

### Comparing `TimePrintOnPYPI-1.5.2/TimePrintOnPYPI.egg-info/PKG-INFO` & `TimePrintOnPYPI-1.5.3/TimePrintOnPYPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimePrintOnPYPI
-Version: 1.5.2
+Version: 1.5.3
 Summary: A package for printing text with time delay between characters
 Home-page: https://github.com/SForces/TimePrint
 Author: Osman TUNA
 Author-email: osmntn08@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `TimePrintOnPYPI-1.5.2/setup.py` & `TimePrintOnPYPI-1.5.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         print("Need Help ? Contact Me From e-mail: osmntn08@gmail.com")
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='TimePrintOnPYPI',
-    version='1.5.2',
+    version='1.5.3',
     description='A package for printing text with time delay between characters',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/SForces/TimePrint',
     author='Osman TUNA',
     author_email='osmntn08@gmail.com',
     license='MIT',
```

