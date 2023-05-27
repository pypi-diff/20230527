# Comparing `tmp/pyslit-1.0.0.tar.gz` & `tmp/pyslit-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslit-1.0.0.tar", last modified: Fri May 26 19:07:24 2023, max compression
+gzip compressed data, was "pyslit-2.0.5.tar", last modified: Sat May 27 11:58:28 2023, max compression
```

## Comparing `pyslit-1.0.0.tar` & `pyslit-2.0.5.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 19:07:23.993620 pyslit-1.0.0/
--rw-rw-rw-   0        0        0     1082 2023-05-26 04:35:22.000000 pyslit-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4061 2023-05-26 19:07:23.991427 pyslit-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3656 2023-05-26 19:06:02.000000 pyslit-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 19:07:23.945083 pyslit-1.0.0/pyslit/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:07:23.989426 pyslit-1.0.0/pyslit/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:07:23.987056 pyslit-1.0.0/pyslit/src/pyslit.egg-info/
--rw-rw-rw-   0        0        0     4061 2023-05-26 19:07:23.000000 pyslit-1.0.0/pyslit/src/pyslit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-05-26 19:07:23.000000 pyslit-1.0.0/pyslit/src/pyslit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 19:07:23.000000 pyslit-1.0.0/pyslit/src/pyslit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-26 19:07:23.000000 pyslit-1.0.0/pyslit/src/pyslit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10398 2023-05-26 18:44:27.000000 pyslit-1.0.0/pyslit/src/pyslit.py
--rw-rw-rw-   0        0        0       42 2023-05-26 19:07:23.993620 pyslit-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1263 2023-05-26 19:00:55.000000 pyslit-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:58:28.014863 pyslit-2.0.5/
+-rw-rw-rw-   0        0        0     1082 2023-05-26 04:35:22.000000 pyslit-2.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       34 2023-05-27 11:57:20.000000 pyslit-2.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     5597 2023-05-27 11:58:28.012856 pyslit-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5054 2023-05-27 11:55:13.000000 pyslit-2.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 11:58:27.847616 pyslit-2.0.5/pyslit/
+drwxrwxrwx   0        0        0        0 2023-05-27 11:58:28.008663 pyslit-2.0.5/pyslit/src/
+-rw-rw-rw-   0        0        0     8622 2023-05-27 11:52:33.000000 pyslit-2.0.5/pyslit/src/Music_player.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:58:27.927584 pyslit-2.0.5/pyslit/src/pyslit.egg-info/
+-rw-rw-rw-   0        0        0     5597 2023-05-27 11:58:27.000000 pyslit-2.0.5/pyslit/src/pyslit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-05-27 11:58:27.000000 pyslit-2.0.5/pyslit/src/pyslit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 11:58:27.000000 pyslit-2.0.5/pyslit/src/pyslit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-05-27 11:58:27.000000 pyslit-2.0.5/pyslit/src/pyslit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-27 11:58:27.000000 pyslit-2.0.5/pyslit/src/pyslit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13307 2023-05-27 10:03:28.000000 pyslit-2.0.5/pyslit/src/pyslit.py
+-rw-rw-rw-   0        0        0       42 2023-05-27 11:58:28.014863 pyslit-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1715 2023-05-27 11:53:18.000000 pyslit-2.0.5/setup.py
```

### Comparing `pyslit-1.0.0/LICENSE.txt` & `pyslit-2.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyslit-1.0.0/setup.py` & `pyslit-2.0.5/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyslit",                     # This is the name of the package
-    version="1.0.0",                        # The initial release version
+    version="2.0.5",                        # The initial release version
     author="Ashraq",                     # Full name of the author
     author_email='ashraqmohideen@gmail.com',
-    description="All in one perfect module for data types",
+    description="Text to speech, Speech recognizer, Music player, Play video on youtube, Google and Wikipedia search, Control the system, News, Datetime, All in one perfect module for data types",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
-    python_requires='>=3.6',                # Minimum version requirement of the package
+    setup_requires=['setuptools_scm'],
+    include_package_data = True,
+    python_requires='>=3.10',                # Minimum version requirement of the package
     py_modules=["pyslit"],             # Name of the python package
     package_dir={'':'pyslit/src'},     # Directory of the source code of the package
-    install_requires=[]                     # Install other dependencies if any
+    package_data={'':['Music_player.py']},
+    install_requires=[                     # Install other dependencies if any
+        'pyttsx3',
+        'pygame',
+        'pyaudio',
+        'SpeechRecognition',
+        'pywhatkit',
+        'wikipedia',
+        'requests',
+        'datetime',
+        'bs4'
+    ]
 )
```

