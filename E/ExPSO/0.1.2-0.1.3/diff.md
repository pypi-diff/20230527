# Comparing `tmp/ExPSO-0.1.2.tar.gz` & `tmp/ExPSO-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExPSO-0.1.2.tar", last modified: Sat May 27 08:31:50 2023, max compression
+gzip compressed data, was "ExPSO-0.1.3.tar", last modified: Sat May 27 08:58:01 2023, max compression
```

## Comparing `ExPSO-0.1.2.tar` & `ExPSO-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 08:31:50.475324 ExPSO-0.1.2/
--rw-rw-rw-   0        0        0    35560 2023-05-07 11:50:19.000000 ExPSO-0.1.2/LICENSE
--rw-rw-rw-   0        0        0    16972 2023-05-27 08:31:50.471318 ExPSO-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    16109 2023-05-27 08:27:33.000000 ExPSO-0.1.2/README.md
--rw-rw-rw-   0        0        0     1041 2023-05-27 08:27:20.000000 ExPSO-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 08:31:50.479328 ExPSO-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 08:31:50.338223 ExPSO-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 08:31:50.373248 ExPSO-0.1.2/src/ExPSO/
--rw-rw-rw-   0        0        0     9942 2023-05-27 07:08:41.000000 ExPSO-0.1.2/src/ExPSO/ExPSOClass.py
--rw-rw-rw-   0        0        0      124 2023-05-07 10:18:51.000000 ExPSO-0.1.2/src/ExPSO/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:31:50.459310 ExPSO-0.1.2/src/ExPSO.egg-info/
--rw-rw-rw-   0        0        0    16972 2023-05-27 08:31:50.000000 ExPSO-0.1.2/src/ExPSO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-05-27 08:31:50.000000 ExPSO-0.1.2/src/ExPSO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 08:31:50.000000 ExPSO-0.1.2/src/ExPSO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-27 08:31:50.000000 ExPSO-0.1.2/src/ExPSO.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 08:58:01.656737 ExPSO-0.1.3/
+-rw-rw-rw-   0        0        0    35560 2023-05-07 11:50:19.000000 ExPSO-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0    16938 2023-05-27 08:58:01.655736 ExPSO-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    16075 2023-05-27 08:54:09.000000 ExPSO-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1041 2023-05-27 08:55:16.000000 ExPSO-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 08:58:01.657723 ExPSO-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 08:58:01.629697 ExPSO-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 08:58:01.641706 ExPSO-0.1.3/src/ExPSO/
+-rw-rw-rw-   0        0        0     9942 2023-05-27 07:08:41.000000 ExPSO-0.1.3/src/ExPSO/ExPSOClass.py
+-rw-rw-rw-   0        0        0      124 2023-05-07 10:18:51.000000 ExPSO-0.1.3/src/ExPSO/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:58:01.653716 ExPSO-0.1.3/src/ExPSO.egg-info/
+-rw-rw-rw-   0        0        0    16938 2023-05-27 08:58:01.000000 ExPSO-0.1.3/src/ExPSO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-05-27 08:58:01.000000 ExPSO-0.1.3/src/ExPSO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 08:58:01.000000 ExPSO-0.1.3/src/ExPSO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-27 08:58:01.000000 ExPSO-0.1.3/src/ExPSO.egg-info/top_level.txt
```

### Comparing `ExPSO-0.1.2/LICENSE` & `ExPSO-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ExPSO-0.1.2/PKG-INFO` & `ExPSO-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ExPSO
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Exponential Particle Swarm Optimization (ExPSO) is a Python library that implements an extended variant of the Particle Swarm Optimization (PSO) algorithm. 
 Author-email: Insaf Kraidia <insaf.kraidia@univ-constantine2.dz>, Khelil Kassoul <khelil.kassoul@etu.unige.ch>, Samir Brahim Belhaouari <sbelhaouari@hbku.edu.qa>, Naoufel Cheikhrouhou <naoufel.cheikhrouhou@hesge.ch>, Nicolas Zufferey <nicolas.zufferey.1@ulaval.ca>
 Project-URL: Homepage, https://github.com/insafkraidia/ExPSO.git
 Project-URL: Bug Tracker, https://github.com/insafkraidia/ExPSO.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Exponential Particle Swarm Optimization for Global Optimization (ExPSO)
 
-<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/06.png?raw=true"> </p>
+<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/master/src/06.png?raw=true"> </p>
 
 The ExPSO package is a Python library that includes an algorithm designed to optimize machine and deep learning parameters/hyperparameters. The algorithm divides the swarm population into three subpopulations and utilizes a search strategy based on an exponential function, allowing particles to make large leaps in the search space. It also adapts the control of the velocity range of each particle to balance the exploration and exploitation search phases. The leaping strategy is integrated into the velocity equation, and a new linearly decreasing cognitive parameter is included in the proposed method, along with a dynamic inertia weight strategy. The algorithm is designed to make large jumps at the beginning of the search and then small jumps for further improvements in specific regions of the solution search space. To obtain further information, we recommend referring to the journal paper available at [Exponential Particle Swarm Optimization for Global Optimization (ExPSO)](https://ieeexplore.ieee.org/document/9837898/).
 
 ## Table of content
 
 | Section                                | Description                                                                              |
 | -------------------------------------- | ---------------------------------------------------------------------------------------- |
```

### Comparing `ExPSO-0.1.2/README.md` & `ExPSO-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Exponential Particle Swarm Optimization for Global Optimization (ExPSO)
 
-<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/06.png?raw=true"> </p>
+<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/master/src/06.png?raw=true"> </p>
 
 The ExPSO package is a Python library that includes an algorithm designed to optimize machine and deep learning parameters/hyperparameters. The algorithm divides the swarm population into three subpopulations and utilizes a search strategy based on an exponential function, allowing particles to make large leaps in the search space. It also adapts the control of the velocity range of each particle to balance the exploration and exploitation search phases. The leaping strategy is integrated into the velocity equation, and a new linearly decreasing cognitive parameter is included in the proposed method, along with a dynamic inertia weight strategy. The algorithm is designed to make large jumps at the beginning of the search and then small jumps for further improvements in specific regions of the solution search space. To obtain further information, we recommend referring to the journal paper available at [Exponential Particle Swarm Optimization for Global Optimization (ExPSO)](https://ieeexplore.ieee.org/document/9837898/).
 
 ## Table of content
 
 | Section                                | Description                                                                              |
 | -------------------------------------- | ---------------------------------------------------------------------------------------- |
```

### Comparing `ExPSO-0.1.2/pyproject.toml` & `ExPSO-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   "scikit-learn"
 ]
 
 
 
 [project]
 name = "ExPSO"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Insaf Kraidia", email="insaf.kraidia@univ-constantine2.dz" },
   { name="Khelil Kassoul", email="khelil.kassoul@etu.unige.ch" },
   { name="Samir Brahim Belhaouari", email="sbelhaouari@hbku.edu.qa" },
   { name="Naoufel Cheikhrouhou",email="naoufel.cheikhrouhou@hesge.ch"},
   { name="Nicolas Zufferey",email="nicolas.zufferey.1@ulaval.ca"}
```

### Comparing `ExPSO-0.1.2/src/ExPSO/ExPSOClass.py` & `ExPSO-0.1.3/src/ExPSO/ExPSOClass.py`

 * *Files identical despite different names*

### Comparing `ExPSO-0.1.2/src/ExPSO.egg-info/PKG-INFO` & `ExPSO-0.1.3/src/ExPSO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ExPSO
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Exponential Particle Swarm Optimization (ExPSO) is a Python library that implements an extended variant of the Particle Swarm Optimization (PSO) algorithm. 
 Author-email: Insaf Kraidia <insaf.kraidia@univ-constantine2.dz>, Khelil Kassoul <khelil.kassoul@etu.unige.ch>, Samir Brahim Belhaouari <sbelhaouari@hbku.edu.qa>, Naoufel Cheikhrouhou <naoufel.cheikhrouhou@hesge.ch>, Nicolas Zufferey <nicolas.zufferey.1@ulaval.ca>
 Project-URL: Homepage, https://github.com/insafkraidia/ExPSO.git
 Project-URL: Bug Tracker, https://github.com/insafkraidia/ExPSO.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Exponential Particle Swarm Optimization for Global Optimization (ExPSO)
 
-<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/06.png?raw=true"> </p>
+<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/master/src/06.png?raw=true"> </p>
 
 The ExPSO package is a Python library that includes an algorithm designed to optimize machine and deep learning parameters/hyperparameters. The algorithm divides the swarm population into three subpopulations and utilizes a search strategy based on an exponential function, allowing particles to make large leaps in the search space. It also adapts the control of the velocity range of each particle to balance the exploration and exploitation search phases. The leaping strategy is integrated into the velocity equation, and a new linearly decreasing cognitive parameter is included in the proposed method, along with a dynamic inertia weight strategy. The algorithm is designed to make large jumps at the beginning of the search and then small jumps for further improvements in specific regions of the solution search space. To obtain further information, we recommend referring to the journal paper available at [Exponential Particle Swarm Optimization for Global Optimization (ExPSO)](https://ieeexplore.ieee.org/document/9837898/).
 
 ## Table of content
 
 | Section                                | Description                                                                              |
 | -------------------------------------- | ---------------------------------------------------------------------------------------- |
```

