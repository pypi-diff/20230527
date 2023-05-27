# Comparing `tmp/scatterd-1.3.2.tar.gz` & `tmp/scatterd-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatterd-1.3.2.tar", last modified: Sat May 27 12:42:29 2023, max compression
+gzip compressed data, was "scatterd-1.3.3.tar", last modified: Sat May 27 16:48:51 2023, max compression
```

## Comparing `scatterd-1.3.2.tar` & `scatterd-1.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 12:42:29.570647 scatterd-1.3.2/
--rw-rw-rw-   0        0        0     1121 2021-11-13 12:45:24.000000 scatterd-1.3.2/LICENSE
--rw-rw-rw-   0        0        0      115 2021-11-13 12:45:24.000000 scatterd-1.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4994 2023-05-27 12:42:29.571648 scatterd-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     4451 2022-12-19 19:17:15.000000 scatterd-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 12:42:29.553455 scatterd-1.3.2/scatterd/
--rw-rw-rw-   0        0        0     1817 2023-05-27 12:40:09.000000 scatterd-1.3.2/scatterd/__init__.py
--rw-rw-rw-   0        0        0     7267 2023-05-27 12:38:44.000000 scatterd-1.3.2/scatterd/examples.py
--rw-rw-rw-   0        0        0    21943 2023-05-27 12:27:07.000000 scatterd-1.3.2/scatterd/scatterd.py
-drwxrwxrwx   0        0        0        0 2023-05-27 12:42:29.569649 scatterd-1.3.2/scatterd.egg-info/
--rw-rw-rw-   0        0        0     4994 2023-05-27 12:42:29.000000 scatterd-1.3.2/scatterd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-27 12:42:29.000000 scatterd-1.3.2/scatterd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 12:42:29.000000 scatterd-1.3.2/scatterd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-27 12:42:29.000000 scatterd-1.3.2/scatterd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-27 12:42:29.000000 scatterd-1.3.2/scatterd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      259 2023-05-27 12:42:29.584609 scatterd-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1419 2023-04-21 11:44:02.000000 scatterd-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 16:48:51.666620 scatterd-1.3.3/
+-rw-rw-rw-   0        0        0     1121 2021-11-13 12:45:24.000000 scatterd-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0      115 2021-11-13 12:45:24.000000 scatterd-1.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4994 2023-05-27 16:48:51.666620 scatterd-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4451 2022-12-19 19:17:15.000000 scatterd-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 16:48:51.647751 scatterd-1.3.3/scatterd/
+-rw-rw-rw-   0        0        0     1790 2023-05-27 16:48:36.000000 scatterd-1.3.3/scatterd/__init__.py
+-rw-rw-rw-   0        0        0     7314 2023-05-27 16:47:07.000000 scatterd-1.3.3/scatterd/examples.py
+-rw-rw-rw-   0        0        0    21943 2023-05-27 12:27:07.000000 scatterd-1.3.3/scatterd/scatterd.py
+drwxrwxrwx   0        0        0        0 2023-05-27 16:48:51.664586 scatterd-1.3.3/scatterd.egg-info/
+-rw-rw-rw-   0        0        0     4994 2023-05-27 16:48:51.000000 scatterd-1.3.3/scatterd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-27 16:48:51.000000 scatterd-1.3.3/scatterd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 16:48:51.000000 scatterd-1.3.3/scatterd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-27 16:48:51.000000 scatterd-1.3.3/scatterd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-27 16:48:51.000000 scatterd-1.3.3/scatterd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      259 2023-05-27 16:48:51.669650 scatterd-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1419 2023-05-27 12:43:17.000000 scatterd-1.3.3/setup.py
```

### Comparing `scatterd-1.3.2/LICENSE` & `scatterd-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scatterd-1.3.2/PKG-INFO` & `scatterd-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scatterd
-Version: 1.3.2
+Version: 1.3.3
 Summary: scatterd is an easy and fast way of creating scatter plots.
 Home-page: https://erdogant.github.io/scatterd
-Download-URL: https://github.com/erdogant/scatterd/archive/1.3.2.tar.gz
+Download-URL: https://github.com/erdogant/scatterd/archive/1.3.3.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: scatterd Version: 1.3.2 Summary: scatterd is an
+Metadata-Version: 2.1 Name: scatterd Version: 1.3.3 Summary: scatterd is an
 easy and fast way of creating scatter plots. Home-page: https://
 erdogant.github.io/scatterd Download-URL: https://github.com/erdogant/scatterd/
-archive/1.3.2.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
+archive/1.3.3.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE # scatterd [![Python](https://img.shields.io/pypi/pyversions/scatterd)]
 (https://img.shields.io/pypi/pyversions/scatterd) [![Pypi](https://
 img.shields.io/pypi/v/scatterd)](https://pypi.org/project/scatterd/) [![Docs]
 (https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
```

### Comparing `scatterd-1.3.2/README.md` & `scatterd-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `scatterd-1.3.2/scatterd/__init__.py` & `scatterd-1.3.3/scatterd/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from scatterd.scatterd import scatterd,import_example, set_colors, _preprocessing, gradient_on_density_color
+from scatterd.scatterd import scatterd,import_example, set_colors, _preprocessing
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.3.2'
+__version__ = '1.3.3'
 
 # module level doc-string
 __doc__ = """
 scatterd
 =====================================================================
 
 Scatterd is an easy and fast way of creating beautiful scatter plots.
```

### Comparing `scatterd-1.3.2/scatterd/examples.py` & `scatterd-1.3.3/scatterd/examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from scatterd import scatterd, import_example
 import numpy as np
 
+# %%
+from scatterd import scatterd
+
+# %%
+
 df = import_example()
 fig, ax = scatterd(df['tsneX'],
                    df['tsneY'],
                    labels=df['labx'],
                    )
 
 # %%
```

### Comparing `scatterd-1.3.2/scatterd/scatterd.py` & `scatterd-1.3.3/scatterd/scatterd.py`

 * *Files identical despite different names*

### Comparing `scatterd-1.3.2/scatterd.egg-info/PKG-INFO` & `scatterd-1.3.3/scatterd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scatterd
-Version: 1.3.2
+Version: 1.3.3
 Summary: scatterd is an easy and fast way of creating scatter plots.
 Home-page: https://erdogant.github.io/scatterd
-Download-URL: https://github.com/erdogant/scatterd/archive/1.3.2.tar.gz
+Download-URL: https://github.com/erdogant/scatterd/archive/1.3.3.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: scatterd Version: 1.3.2 Summary: scatterd is an
+Metadata-Version: 2.1 Name: scatterd Version: 1.3.3 Summary: scatterd is an
 easy and fast way of creating scatter plots. Home-page: https://
 erdogant.github.io/scatterd Download-URL: https://github.com/erdogant/scatterd/
-archive/1.3.2.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
+archive/1.3.3.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE # scatterd [![Python](https://img.shields.io/pypi/pyversions/scatterd)]
 (https://img.shields.io/pypi/pyversions/scatterd) [![Pypi](https://
 img.shields.io/pypi/v/scatterd)](https://pypi.org/project/scatterd/) [![Docs]
 (https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
```

### Comparing `scatterd-1.3.2/setup.py` & `scatterd-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE))
 
 #--------  Create setup file    
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-     install_requires=['matplotlib','numpy','colourmap>=1.1.11','seaborn','requests'],
+     install_requires=['matplotlib','numpy','colourmap>=1.1.12','seaborn','requests'],
      python_requires='>=3',
      name='scatterd',
      version=new_version,
      author="Erdogan Taskesen",
      author_email="erdogant@gmail.com",
      description="scatterd is an easy and fast way of creating scatter plots.",
      long_description=long_description,
```

