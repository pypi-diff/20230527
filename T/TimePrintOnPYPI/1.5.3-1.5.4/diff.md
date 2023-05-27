# Comparing `tmp/TimePrintOnPYPI-1.5.3.tar.gz` & `tmp/TimePrintOnPYPI-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimePrintOnPYPI-1.5.3.tar", last modified: Sat May 27 10:27:25 2023, max compression
+gzip compressed data, was "TimePrintOnPYPI-1.5.4.tar", last modified: Sat May 27 10:28:24 2023, max compression
```

## Comparing `TimePrintOnPYPI-1.5.3.tar` & `TimePrintOnPYPI-1.5.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 10:27:25.659808 TimePrintOnPYPI-1.5.3/
--rw-rw-rw-   0        0        0     4611 2023-05-27 10:27:25.657798 TimePrintOnPYPI-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     4121 2023-05-26 15:19:49.000000 TimePrintOnPYPI-1.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 10:27:25.640535 TimePrintOnPYPI-1.5.3/TimePrint/
--rw-rw-rw-   0        0        0     1820 2023-05-27 10:27:17.000000 TimePrintOnPYPI-1.5.3/TimePrint/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 10:27:25.654782 TimePrintOnPYPI-1.5.3/TimePrintOnPYPI.egg-info/
--rw-rw-rw-   0        0        0     4611 2023-05-27 10:27:25.000000 TimePrintOnPYPI-1.5.3/TimePrintOnPYPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-05-27 10:27:25.000000 TimePrintOnPYPI-1.5.3/TimePrintOnPYPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 10:27:25.000000 TimePrintOnPYPI-1.5.3/TimePrintOnPYPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-27 10:27:25.000000 TimePrintOnPYPI-1.5.3/TimePrintOnPYPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 10:27:25.660803 TimePrintOnPYPI-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1013 2023-05-27 10:25:07.000000 TimePrintOnPYPI-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:28:24.714994 TimePrintOnPYPI-1.5.4/
+-rw-rw-rw-   0        0        0     4611 2023-05-27 10:28:24.713008 TimePrintOnPYPI-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4121 2023-05-27 10:28:11.000000 TimePrintOnPYPI-1.5.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 10:28:24.689337 TimePrintOnPYPI-1.5.4/TimePrint/
+-rw-rw-rw-   0        0        0     1820 2023-05-27 10:28:01.000000 TimePrintOnPYPI-1.5.4/TimePrint/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:28:24.708998 TimePrintOnPYPI-1.5.4/TimePrintOnPYPI.egg-info/
+-rw-rw-rw-   0        0        0     4611 2023-05-27 10:28:24.000000 TimePrintOnPYPI-1.5.4/TimePrintOnPYPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-05-27 10:28:24.000000 TimePrintOnPYPI-1.5.4/TimePrintOnPYPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 10:28:24.000000 TimePrintOnPYPI-1.5.4/TimePrintOnPYPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-27 10:28:24.000000 TimePrintOnPYPI-1.5.4/TimePrintOnPYPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 10:28:24.715990 TimePrintOnPYPI-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2023-05-27 10:28:06.000000 TimePrintOnPYPI-1.5.4/setup.py
```

### Comparing `TimePrintOnPYPI-1.5.3/PKG-INFO` & `TimePrintOnPYPI-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: TimePrintOnPYPI
-Version: 1.5.3
+Version: 1.5.4
 Summary: A package for printing text with time delay between characters
 Home-page: https://github.com/SForces/TimePrint
 Author: Osman TUNA
 Author-email: osmntn08@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# <span style="color: #FF0000;">**TIME PRINT V1.5.1**</span>
+# <span style="color: #FF0000;">**TIME PRINT V1.5.4**</span>
 # <span style="color: yellow;">**ENGLISH**</span><br>
 <span style="color: #FF4500;">This is a python package to use write effect and more in your texts !</span><br>
 # <span style="color: blue;">**FUNCTIONS**</span><br>
 ## <span style="color: #007FFF;">**TP(seconds,"text")**</span>
 <span style="color: #E6A8D7;">You want to write "<span style="color: #87CEEB">**your_text**<span style="color: #E6A8D7;">" in <span style="color: #87CEEB">**5**<span style="color: #E6A8D7;"> seconds? just use;<br>
 <span style="color: #87CEEB">**TP(5,"your_text")**<span style="color: #E6A8D7;"> !<br>
 <span style="color: #0F52BA">Formats: seconds: int,"text":str<br>
```

### Comparing `TimePrintOnPYPI-1.5.3/README.md` & `TimePrintOnPYPI-1.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# <span style="color: #FF0000;">**TIME PRINT V1.5.1**</span>
+# <span style="color: #FF0000;">**TIME PRINT V1.5.4**</span>
 # <span style="color: yellow;">**ENGLISH**</span><br>
 <span style="color: #FF4500;">This is a python package to use write effect and more in your texts !</span><br>
 # <span style="color: blue;">**FUNCTIONS**</span><br>
 ## <span style="color: #007FFF;">**TP(seconds,"text")**</span>
 <span style="color: #E6A8D7;">You want to write "<span style="color: #87CEEB">**your_text**<span style="color: #E6A8D7;">" in <span style="color: #87CEEB">**5**<span style="color: #E6A8D7;"> seconds? just use;<br>
 <span style="color: #87CEEB">**TP(5,"your_text")**<span style="color: #E6A8D7;"> !<br>
 <span style="color: #0F52BA">Formats: seconds: int,"text":str<br>
```

### Comparing `TimePrintOnPYPI-1.5.3/TimePrint/__init__.py` & `TimePrintOnPYPI-1.5.4/TimePrint/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     print("        | |    | | | \  / | |__      | |__) | |__) | | | |  \| |  | |   ")
     print("        | |    | | | |\/| |  __|     |  ___/|  _  /  | | | . ` |  | |   ")
     print("        | |   _| |_| |  | | |____    | |    | | \ \ _| |_| |\  |  | |   ")
     print("        |_|  |_____|_|  |_|______|   |_|    |_|  \_\_____|_| \_|  |_|   ")
     print("\nAuthor: Osman TUNA")
     print("Author Email: osmntn08@gmail.com")
     print("Project Page: https://github.com/SForces/TimePrint")
-    print("Version: 1.5.3")
+    print("Version: 1.5.4")
 def Timetag(format: str) -> str:
     """
     Example Usages;
 
     "%H:%M" Returns --> 12:56 = (Hours:Minutes)
 
     "%H:%M:%S" Returns --> 12:56:24 = (Hours:Minutes:Seconds)
```

### Comparing `TimePrintOnPYPI-1.5.3/TimePrintOnPYPI.egg-info/PKG-INFO` & `TimePrintOnPYPI-1.5.4/TimePrintOnPYPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: TimePrintOnPYPI
-Version: 1.5.3
+Version: 1.5.4
 Summary: A package for printing text with time delay between characters
 Home-page: https://github.com/SForces/TimePrint
 Author: Osman TUNA
 Author-email: osmntn08@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# <span style="color: #FF0000;">**TIME PRINT V1.5.1**</span>
+# <span style="color: #FF0000;">**TIME PRINT V1.5.4**</span>
 # <span style="color: yellow;">**ENGLISH**</span><br>
 <span style="color: #FF4500;">This is a python package to use write effect and more in your texts !</span><br>
 # <span style="color: blue;">**FUNCTIONS**</span><br>
 ## <span style="color: #007FFF;">**TP(seconds,"text")**</span>
 <span style="color: #E6A8D7;">You want to write "<span style="color: #87CEEB">**your_text**<span style="color: #E6A8D7;">" in <span style="color: #87CEEB">**5**<span style="color: #E6A8D7;"> seconds? just use;<br>
 <span style="color: #87CEEB">**TP(5,"your_text")**<span style="color: #E6A8D7;"> !<br>
 <span style="color: #0F52BA">Formats: seconds: int,"text":str<br>
```

### Comparing `TimePrintOnPYPI-1.5.3/setup.py` & `TimePrintOnPYPI-1.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         print("Need Help ? Contact Me From e-mail: osmntn08@gmail.com")
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='TimePrintOnPYPI',
-    version='1.5.3',
+    version='1.5.4',
     description='A package for printing text with time delay between characters',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/SForces/TimePrint',
     author='Osman TUNA',
     author_email='osmntn08@gmail.com',
     license='MIT',
```

