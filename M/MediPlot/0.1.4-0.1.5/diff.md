# Comparing `tmp/MediPlot-0.1.4.tar.gz` & `tmp/MediPlot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MediPlot-0.1.4.tar", last modified: Mon Dec  7 20:22:48 2020, max compression
+gzip compressed data, was "MediPlot-0.1.5.tar", last modified: Sat May 27 08:37:38 2023, max compression
```

## Comparing `MediPlot-0.1.4.tar` & `MediPlot-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxrwx   0        0        0        0 2020-12-07 20:22:48.753288 MediPlot-0.1.4/
-drwxrwxrwx   0        0        0        0 2020-12-07 20:22:48.752291 MediPlot-0.1.4/MediPlot/
--rw-rw-rw-   0        0        0     7041 2020-12-07 20:21:15.767724 MediPlot-0.1.4/MediPlot/BodyMap.py
--rw-rw-rw-   0        0        0       40 2020-12-07 08:39:39.274704 MediPlot-0.1.4/MediPlot/__init__.py
--rw-rw-rw-   0        0        0      673 2020-12-07 20:22:48.753288 MediPlot-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       39 2020-07-03 16:22:33.000000 MediPlot-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      817 2020-12-07 20:22:15.501695 MediPlot-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:37:38.963677 MediPlot-0.1.5/
+-rw-rw-rw-   0        0        0     1100 2023-05-27 08:26:45.000000 MediPlot-0.1.5/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 08:37:38.946764 MediPlot-0.1.5/MediPlot/
+-rw-rw-rw-   0        0        0     6971 2023-05-27 08:30:42.000000 MediPlot-0.1.5/MediPlot/BodyMap.py
+-rw-rw-rw-   0        0        0      206 2023-05-27 08:30:57.000000 MediPlot-0.1.5/MediPlot/Test.py
+-rw-rw-rw-   0        0        0       40 2023-05-27 08:26:45.000000 MediPlot-0.1.5/MediPlot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:37:38.963181 MediPlot-0.1.5/MediPlot.egg-info/
+-rw-rw-rw-   0        0        0      701 2023-05-27 08:37:38.000000 MediPlot-0.1.5/MediPlot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-05-27 08:37:38.000000 MediPlot-0.1.5/MediPlot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 08:37:38.000000 MediPlot-0.1.5/MediPlot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-27 08:37:38.000000 MediPlot-0.1.5/MediPlot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-27 08:37:38.000000 MediPlot-0.1.5/MediPlot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      701 2023-05-27 08:37:38.963677 MediPlot-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-05-27 08:37:38.967671 MediPlot-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      827 2023-05-27 08:36:08.000000 MediPlot-0.1.5/setup.py
```

### Comparing `MediPlot-0.1.4/MediPlot/BodyMap.py` & `MediPlot-0.1.5/MediPlot/BodyMap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from matplotlib import cm
 
 class BodyMap:
     def __init__(self):
-        im_link = 'https://raw.githubusercontent.com/MuteJester/MediPlot/master/MediPlot/Body_Sil.png'
+        im_link = 'Body_Sil.png'
         self.body_sil = plt.imread(im_link)
         self.bmap = {'head': self.set_head, 'legs': self.set_legs, 'les': self.set_right_leg,
                      'left leg': self.set_left_leg, 'right leg': self.set_right_leg, 'right arm': self.set_right_arm,
                      'left arm': self.set_left_arm, 'torso': self.set_torso, 'arms': self.set_arms,
                      'waist': self.set_waist,
                      'neck': self.set_neck, 'left hand': self.set_left_hand, 'right hand': self.set_right_hand,
                      'left foot': self.set_left_foot, 'right foot': self.set_right_foot,
```

### Comparing `MediPlot-0.1.4/PKG-INFO` & `MediPlot-0.1.5/MediPlot.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: MediPlot
-Version: 0.1.4
+Version: 0.1.5
 Summary: A matplotlib based library for anatomical plots
 Home-page: https://github.com/MuteJester/MediPlot
+Download-URL: https://github.com/MuteJester/MediPlot/archive/refs/tags/v_0.1.5.tar.gz
 Author: Thomas Konstantinovsky
 Author-email: thomaskon90@gmail.com
 License: MIT
-Download-URL: https://github.com/MuteJester/MediPlot/archive/v_0.1.4.tar.gz
-Description: UNKNOWN
 Keywords: datascience,data visualization,matplotlib
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE.txt
+
+UNKNOWN
+
```

### Comparing `MediPlot-0.1.4/setup.py` & `MediPlot-0.1.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'MediPlot',
   packages = ['MediPlot'],
-  version = '0.1.4',
+  version = '0.1.5',
   license='MIT',
   description = 'A matplotlib based library for anatomical plots',
   author = 'Thomas Konstantinovsky',
   author_email = 'thomaskon90@gmail.com',
   url = 'https://github.com/MuteJester/MediPlot',
-  download_url = 'https://github.com/MuteJester/MediPlot/archive/v_0.1.4.tar.gz',
+  download_url = 'https://github.com/MuteJester/MediPlot/archive/refs/tags/v_0.1.5.tar.gz',
   keywords = ['datascience', 'data visualization', 'matplotlib'],
   install_requires=[
           'matplotlib',
           'numpy',
 
       ],
   classifiers=[
```

