# Comparing `tmp/logidrivepy-0.1.2.tar.gz` & `tmp/logidrivepy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logidrivepy-0.1.2.tar", last modified: Sat May 27 10:05:13 2023, max compression
+gzip compressed data, was "logidrivepy-0.1.3.tar", last modified: Sat May 27 10:20:39 2023, max compression
```

## Comparing `logidrivepy-0.1.2.tar` & `logidrivepy-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 10:05:13.338046 logidrivepy-0.1.2/
--rw-rw-rw-   0        0        0     1087 2023-05-23 22:21:13.000000 logidrivepy-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     3469 2023-05-27 10:05:13.337045 logidrivepy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2770 2023-05-27 10:03:51.000000 logidrivepy-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 10:05:13.295035 logidrivepy-0.1.2/logidrivepy/
--rw-rw-rw-   0        0        0      196 2023-05-27 04:08:39.000000 logidrivepy-0.1.2/logidrivepy/__init__.py
--rw-rw-rw-   0        0        0     2078 2023-05-27 03:38:07.000000 logidrivepy-0.1.2/logidrivepy/constants.py
--rw-rw-rw-   0        0        0      760 2023-05-27 09:04:30.000000 logidrivepy-0.1.2/logidrivepy/controller.py
--rw-rw-rw-   0        0        0    16701 2023-05-27 08:42:15.000000 logidrivepy-0.1.2/logidrivepy/functions.py
--rw-rw-rw-   0        0        0     1865 2023-05-27 03:39:18.000000 logidrivepy-0.1.2/logidrivepy/structs.py
-drwxrwxrwx   0        0        0        0 2023-05-27 10:05:13.326044 logidrivepy-0.1.2/logidrivepy.egg-info/
--rw-rw-rw-   0        0        0     3469 2023-05-27 10:05:13.000000 logidrivepy-0.1.2/logidrivepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-05-27 10:05:13.000000 logidrivepy-0.1.2/logidrivepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 10:05:13.000000 logidrivepy-0.1.2/logidrivepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-27 10:05:13.000000 logidrivepy-0.1.2/logidrivepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 10:05:13.339046 logidrivepy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      907 2023-05-27 10:04:05.000000 logidrivepy-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 10:05:13.334045 logidrivepy-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2023-05-23 21:56:36.000000 logidrivepy-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0      743 2023-05-27 09:01:48.000000 logidrivepy-0.1.2/tests/run_controller_test.py
--rw-rw-rw-   0        0        0      585 2023-05-27 09:26:43.000000 logidrivepy-0.1.2/tests/spin_wheel_test.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:20:39.069082 logidrivepy-0.1.3/
+-rw-rw-rw-   0        0        0     1087 2023-05-23 22:21:13.000000 logidrivepy-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3469 2023-05-27 10:20:39.068082 logidrivepy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2770 2023-05-27 10:03:51.000000 logidrivepy-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 10:20:39.036074 logidrivepy-0.1.3/logidrivepy/
+-rw-rw-rw-   0        0        0      196 2023-05-27 04:08:39.000000 logidrivepy-0.1.3/logidrivepy/__init__.py
+-rw-rw-rw-   0        0        0     2078 2023-05-27 03:38:07.000000 logidrivepy-0.1.3/logidrivepy/constants.py
+-rw-rw-rw-   0        0        0      760 2023-05-27 09:04:30.000000 logidrivepy-0.1.3/logidrivepy/controller.py
+-rw-rw-rw-   0        0        0    16701 2023-05-27 08:42:15.000000 logidrivepy-0.1.3/logidrivepy/functions.py
+-rw-rw-rw-   0        0        0     1865 2023-05-27 03:39:18.000000 logidrivepy-0.1.3/logidrivepy/structs.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:20:39.058080 logidrivepy-0.1.3/logidrivepy.egg-info/
+-rw-rw-rw-   0        0        0     3469 2023-05-27 10:20:38.000000 logidrivepy-0.1.3/logidrivepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-05-27 10:20:38.000000 logidrivepy-0.1.3/logidrivepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 10:20:38.000000 logidrivepy-0.1.3/logidrivepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-27 10:20:38.000000 logidrivepy-0.1.3/logidrivepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 10:20:39.069082 logidrivepy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      957 2023-05-27 10:19:36.000000 logidrivepy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:20:39.065081 logidrivepy-0.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-23 21:56:36.000000 logidrivepy-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      743 2023-05-27 09:01:48.000000 logidrivepy-0.1.3/tests/run_controller_test.py
+-rw-rw-rw-   0        0        0      585 2023-05-27 09:26:43.000000 logidrivepy-0.1.3/tests/spin_wheel_test.py
```

### Comparing `logidrivepy-0.1.2/LICENSE.txt` & `logidrivepy-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.1.2/PKG-INFO` & `logidrivepy-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logidrivepy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library for interfacing with a Logitech steering wheel.
 Home-page: https://github.com/cengizozel/logidrivepy
 Author: Cengiz Ozel
 Author-email: cozel@cs.rochester.edu
 License: MIT
 Keywords: logitech,g920,driving,wheel,controller
 Platform: UNKNOWN
```

### Comparing `logidrivepy-0.1.2/README.md` & `logidrivepy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.1.2/logidrivepy/constants.py` & `logidrivepy-0.1.3/logidrivepy/constants.py`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.1.2/logidrivepy/controller.py` & `logidrivepy-0.1.3/logidrivepy/controller.py`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.1.2/logidrivepy/functions.py` & `logidrivepy-0.1.3/logidrivepy/functions.py`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.1.2/logidrivepy/structs.py` & `logidrivepy-0.1.3/logidrivepy/structs.py`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.1.2/logidrivepy.egg-info/PKG-INFO` & `logidrivepy-0.1.3/logidrivepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logidrivepy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library for interfacing with a Logitech steering wheel.
 Home-page: https://github.com/cengizozel/logidrivepy
 Author: Cengiz Ozel
 Author-email: cozel@cs.rochester.edu
 License: MIT
 Keywords: logitech,g920,driving,wheel,controller
 Platform: UNKNOWN
```

### Comparing `logidrivepy-0.1.2/setup.py` & `logidrivepy-0.1.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='logidrivepy',
-    version='0.1.2',
+    version='0.1.3',
     description='A Python library for interfacing with a Logitech steering wheel.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/cengizozel/logidrivepy',
     author='Cengiz Ozel',
     author_email='cozel@cs.rochester.edu',
     license='MIT',
     packages=find_packages(),
     include_package_data=True,
+    package_data={'logidrivepy': ['dll/*.dll']},
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
```

### Comparing `logidrivepy-0.1.2/tests/run_controller_test.py` & `logidrivepy-0.1.3/tests/run_controller_test.py`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.1.2/tests/spin_wheel_test.py` & `logidrivepy-0.1.3/tests/spin_wheel_test.py`

 * *Files identical despite different names*

