# Comparing `tmp/LegacyNeuralNetworks-0.0.2.tar.gz` & `tmp/LegacyNeuralNetworks-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LegacyNeuralNetworks-0.0.2.tar", last modified: Sat May 27 10:23:00 2023, max compression
+gzip compressed data, was "LegacyNeuralNetworks-0.0.3.tar", last modified: Sat May 27 14:41:47 2023, max compression
```

## Comparing `LegacyNeuralNetworks-0.0.2.tar` & `LegacyNeuralNetworks-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 10:23:00.710592 LegacyNeuralNetworks-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-27 10:23:00.700169 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks/
--rw-rw-rw-   0        0        0    31698 2023-05-27 10:22:37.000000 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks/Fill.py
--rw-rw-rw-   0        0        0    19189 2023-05-27 08:44:43.000000 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks/LegacyNeuralNetworks.py
--rw-rw-rw-   0        0        0      101 2023-05-27 08:55:33.000000 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 10:23:00.707581 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks.egg-info/
--rw-rw-rw-   0        0        0      649 2023-05-27 10:23:00.000000 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-05-27 10:23:00.000000 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 10:23:00.000000 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-27 10:23:00.000000 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-27 10:23:00.000000 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      649 2023-05-27 10:23:00.708593 LegacyNeuralNetworks-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      595 2023-05-27 09:13:04.000000 LegacyNeuralNetworks-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-27 10:23:00.710592 LegacyNeuralNetworks-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      859 2023-05-27 10:22:51.000000 LegacyNeuralNetworks-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 14:41:47.673488 LegacyNeuralNetworks-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-05-27 14:41:47.663516 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks/
+-rw-rw-rw-   0        0        0    31698 2023-05-27 10:22:37.000000 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks/Fill.py
+-rw-rw-rw-   0        0        0    19189 2023-05-27 08:44:43.000000 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks/LegacyNeuralNetworks.py
+-rw-rw-rw-   0        0        0      151 2023-05-27 14:39:50.000000 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks/__init__.py
+-rw-rw-rw-   0        0        0    14578 2023-05-27 14:39:19.000000 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks/ann_fill.py
+drwxrwxrwx   0        0        0        0 2023-05-27 14:41:47.669041 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks.egg-info/
+-rw-rw-rw-   0        0        0     1628 2023-05-27 14:41:47.000000 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-05-27 14:41:47.000000 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 14:41:47.000000 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-27 14:41:47.000000 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-27 14:41:47.000000 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1628 2023-05-27 14:41:47.670048 LegacyNeuralNetworks-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      722 2023-05-27 10:52:46.000000 LegacyNeuralNetworks-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-27 14:41:47.673488 LegacyNeuralNetworks-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      907 2023-05-27 14:41:12.000000 LegacyNeuralNetworks-0.0.3/setup.py
```

### Comparing `LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks/Fill.py` & `LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks/Fill.py`

 * *Files identical despite different names*

### Comparing `LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks/LegacyNeuralNetworks.py` & `LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks/LegacyNeuralNetworks.py`

 * *Files identical despite different names*

### Comparing `LegacyNeuralNetworks-0.0.2/setup.py` & `LegacyNeuralNetworks-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Legacy Neural Networks'
  
 # Setting up
 setup(
     name="LegacyNeuralNetworks",
     version=VERSION,
     author="Hrushikesh Kachgunde",
     author_email="<hrushiskachgunde@gmail.com>",
     description=DESCRIPTION,
+    long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=['numpy', 'matplotlib', 'scikit-learn', 'tensorflow'],
     keywords=['python', 'neural networks', 'ann', 'mcculloh-pitt', 'ART neural network'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
```

