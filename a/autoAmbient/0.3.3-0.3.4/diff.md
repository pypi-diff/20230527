# Comparing `tmp/autoAmbient-0.3.3.tar.gz` & `tmp/autoAmbient-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoAmbient-0.3.3.tar", last modified: Wed May 24 00:53:43 2023, max compression
+gzip compressed data, was "autoAmbient-0.3.4.tar", last modified: Sat May 27 21:54:42 2023, max compression
```

## Comparing `autoAmbient-0.3.3.tar` & `autoAmbient-0.3.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-24 00:53:43.865197 autoAmbient-0.3.3/
--rw-rw-r--   0 luis      (1000) luis      (1000)      348 2023-05-24 00:53:43.865197 autoAmbient-0.3.3/PKG-INFO
--rw-rw-r--   0 luis      (1000) luis      (1000)        0 2023-05-24 00:51:08.000000 autoAmbient-0.3.3/README.md
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-24 00:53:43.865197 autoAmbient-0.3.3/ambient/
--rw-rw-r--   0 luis      (1000) luis      (1000)       73 2023-04-17 21:37:09.000000 autoAmbient-0.3.3/ambient/__init__.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      897 2023-04-25 14:38:15.000000 autoAmbient-0.3.3/ambient/createAutoAmbient.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      785 2023-04-25 15:08:35.000000 autoAmbient-0.3.3/ambient/createTagsFile.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      721 2023-04-11 15:44:13.000000 autoAmbient-0.3.3/ambient/getFile.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-24 00:53:43.865197 autoAmbient-0.3.3/ambient/models/
--rw-rw-r--   0 luis      (1000) luis      (1000)      165 2023-04-25 14:32:48.000000 autoAmbient-0.3.3/ambient/models/blocksModel.py
--rw-rw-r--   0 luis      (1000) luis      (1000)       47 2023-04-17 21:10:55.000000 autoAmbient-0.3.3/ambient/models/mainModel.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      476 2023-04-25 14:56:13.000000 autoAmbient-0.3.3/ambient/models/runModel.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-24 00:53:43.865197 autoAmbient-0.3.3/ambient/tolls/
--rw-rw-r--   0 luis      (1000) luis      (1000)     1892 2023-05-07 20:31:23.000000 autoAmbient-0.3.3/ambient/tolls/clicks.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     4826 2023-04-17 22:02:18.000000 autoAmbient-0.3.3/ambient/tolls/gui.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      822 2023-05-07 20:31:23.000000 autoAmbient-0.3.3/ambient/tolls/utils.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-24 00:53:43.865197 autoAmbient-0.3.3/autoAmbient.egg-info/
--rw-rw-r--   0 luis      (1000) luis      (1000)      348 2023-05-24 00:53:43.000000 autoAmbient-0.3.3/autoAmbient.egg-info/PKG-INFO
--rw-rw-r--   0 luis      (1000) luis      (1000)      502 2023-05-24 00:53:43.000000 autoAmbient-0.3.3/autoAmbient.egg-info/SOURCES.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        1 2023-05-24 00:53:43.000000 autoAmbient-0.3.3/autoAmbient.egg-info/dependency_links.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)      142 2023-05-24 00:53:43.000000 autoAmbient-0.3.3/autoAmbient.egg-info/entry_points.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)       52 2023-05-24 00:53:43.000000 autoAmbient-0.3.3/autoAmbient.egg-info/requires.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        8 2023-05-24 00:53:43.000000 autoAmbient-0.3.3/autoAmbient.egg-info/top_level.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        0 2023-04-11 14:47:07.000000 autoAmbient-0.3.3/pyproject.toml
--rw-rw-r--   0 luis      (1000) luis      (1000)      149 2023-05-24 00:53:43.869197 autoAmbient-0.3.3/setup.cfg
--rw-rw-r--   0 luis      (1000) luis      (1000)      868 2023-05-24 00:52:24.000000 autoAmbient-0.3.3/setup.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-27 21:54:42.218104 autoAmbient-0.3.4/
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1087 2023-04-11 13:55:02.000000 autoAmbient-0.3.4/LICENSE
+-rw-rw-r--   0 luis      (1000) luis      (1000)     3209 2023-05-27 21:54:42.218104 autoAmbient-0.3.4/PKG-INFO
+-rw-rw-r--   0 luis      (1000) luis      (1000)     2324 2023-05-24 02:01:26.000000 autoAmbient-0.3.4/README.md
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-27 21:54:42.214104 autoAmbient-0.3.4/ambient/
+-rw-rw-r--   0 luis      (1000) luis      (1000)       73 2023-04-17 21:37:09.000000 autoAmbient-0.3.4/ambient/__init__.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      897 2023-04-25 14:38:15.000000 autoAmbient-0.3.4/ambient/createAutoAmbient.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      785 2023-04-25 15:08:35.000000 autoAmbient-0.3.4/ambient/createTagsFile.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      721 2023-04-11 15:44:13.000000 autoAmbient-0.3.4/ambient/getFile.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-27 21:54:42.214104 autoAmbient-0.3.4/ambient/models/
+-rw-rw-r--   0 luis      (1000) luis      (1000)      165 2023-04-25 14:32:48.000000 autoAmbient-0.3.4/ambient/models/blocksModel.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)       47 2023-04-17 21:10:55.000000 autoAmbient-0.3.4/ambient/models/mainModel.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      476 2023-04-25 14:56:13.000000 autoAmbient-0.3.4/ambient/models/runModel.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-27 21:54:42.214104 autoAmbient-0.3.4/ambient/tolls/
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1892 2023-05-07 20:31:23.000000 autoAmbient-0.3.4/ambient/tolls/clicks.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     4826 2023-04-17 22:02:18.000000 autoAmbient-0.3.4/ambient/tolls/gui.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      822 2023-05-07 20:31:23.000000 autoAmbient-0.3.4/ambient/tolls/utils.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-27 21:54:42.218104 autoAmbient-0.3.4/autoAmbient.egg-info/
+-rw-rw-r--   0 luis      (1000) luis      (1000)     3209 2023-05-27 21:54:42.000000 autoAmbient-0.3.4/autoAmbient.egg-info/PKG-INFO
+-rw-rw-r--   0 luis      (1000) luis      (1000)      510 2023-05-27 21:54:42.000000 autoAmbient-0.3.4/autoAmbient.egg-info/SOURCES.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        1 2023-05-27 21:54:42.000000 autoAmbient-0.3.4/autoAmbient.egg-info/dependency_links.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)      142 2023-05-27 21:54:42.000000 autoAmbient-0.3.4/autoAmbient.egg-info/entry_points.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)       94 2023-05-27 21:54:42.000000 autoAmbient-0.3.4/autoAmbient.egg-info/requires.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        8 2023-05-27 21:54:42.000000 autoAmbient-0.3.4/autoAmbient.egg-info/top_level.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        0 2023-04-11 14:47:07.000000 autoAmbient-0.3.4/pyproject.toml
+-rw-rw-r--   0 luis      (1000) luis      (1000)      149 2023-05-27 21:54:42.218104 autoAmbient-0.3.4/setup.cfg
+-rw-rw-r--   0 luis      (1000) luis      (1000)      921 2023-05-27 21:53:12.000000 autoAmbient-0.3.4/setup.py
```

### Comparing `autoAmbient-0.3.3/ambient/createAutoAmbient.py` & `autoAmbient-0.3.4/ambient/createAutoAmbient.py`

 * *Files identical despite different names*

### Comparing `autoAmbient-0.3.3/ambient/createTagsFile.py` & `autoAmbient-0.3.4/ambient/createTagsFile.py`

 * *Files identical despite different names*

### Comparing `autoAmbient-0.3.3/ambient/getFile.py` & `autoAmbient-0.3.4/ambient/getFile.py`

 * *Files identical despite different names*

### Comparing `autoAmbient-0.3.3/ambient/tolls/clicks.py` & `autoAmbient-0.3.4/ambient/tolls/clicks.py`

 * *Files identical despite different names*

### Comparing `autoAmbient-0.3.3/ambient/tolls/gui.py` & `autoAmbient-0.3.4/ambient/tolls/gui.py`

 * *Files identical despite different names*

### Comparing `autoAmbient-0.3.3/ambient/tolls/utils.py` & `autoAmbient-0.3.4/ambient/tolls/utils.py`

 * *Files identical despite different names*

### Comparing `autoAmbient-0.3.3/setup.py` & `autoAmbient-0.3.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="autoAmbient",
-    version="0.3.3",
+    version="0.3.4",
     author="Luis Arthur Rodrigues da Silva",
     author_email="luisarthurlards03@gmail.com",
     packages=["ambient", "ambient.tolls", "ambient.models"],
-
     url="https://github.com/luisArthurRodriguesDaSilva/automations-enviroment",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    python_requires='>=3.8',
+    python_requires=">=3.8",
     entry_points={
         "console_scripts": [
             "getFile=ambient.getFile:main",
             "createTagsFile=ambient.createTagsFile:main",
             "createAmbient=ambient.createAutoAmbient:main",
         ],
     },
     install_requires=[
         "PySimpleGUI==4.20.0",
-        "botcity==1.8.1",
-        "requests>=2.25.1"
+        "botcity-framework-core>=0.3.0",
+        "botcity-maestro-sdk>=0.1.5",
+        "requests>=2.25.1",
     ],
-    license='MIT',
+    license="MIT",
 )
```

