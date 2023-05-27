# Comparing `tmp/pymonntorch-0.1.0.tar.gz` & `tmp/pymonntorch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonntorch-0.1.0.tar", last modified: Tue May 16 07:15:40 2023, max compression
+gzip compressed data, was "pymonntorch-0.1.1.tar", last modified: Sat May 27 06:20:10 2023, max compression
```

## Comparing `pymonntorch-0.1.0.tar` & `pymonntorch-0.1.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-16 07:15:40.092893 pymonntorch-0.1.0/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      232 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/AUTHORS.rst
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     3592 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       90 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/HISTORY.rst
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     1117 2023-05-16 06:37:35.000000 pymonntorch-0.1.0/LICENSE
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      262 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/MANIFEST.in
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     4273 2023-05-16 07:15:40.092949 pymonntorch-0.1.0/PKG-INFO
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     3539 2023-05-16 07:14:45.000000 pymonntorch-0.1.0/README.rst
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-16 07:15:40.087821 pymonntorch-0.1.0/docs/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      612 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/docs/Makefile
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-16 07:15:40.088127 pymonntorch-0.1.0/docs/_images/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)    42525 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/docs/_images/spike.png
--rw-r--r--   0 atenamohammadi   (501) staff       (20)   138598 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/docs/_images/voltage.png
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       28 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/docs/authors.rst
--rwxr-xr-x   0 atenamohammadi   (501) staff       (20)     5043 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/docs/conf.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       33 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/docs/contributing.rst
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     1001 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/docs/documentation.rst
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       28 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/docs/history.rst
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      317 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/docs/index.rst
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     1160 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/docs/installation.rst
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      809 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/docs/make.bat
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       27 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/docs/readme.rst
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     5802 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/docs/tutorial.rst
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-16 07:15:40.088697 pymonntorch-0.1.0/pymonntorch/
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-16 07:15:40.089747 pymonntorch-0.1.0/pymonntorch/NetworkBehavior/
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-16 07:15:40.090106 pymonntorch-0.1.0/pymonntorch/NetworkBehavior/Basics/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     5791 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/NetworkBehavior/Basics/BasicHomeostasis.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      964 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/NetworkBehavior/Basics/Normalization.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/NetworkBehavior/Basics/__init__.py
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-16 07:15:40.090763 pymonntorch-0.1.0/pymonntorch/NetworkBehavior/EulerEquationModules/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     1426 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/NetworkBehavior/EulerEquationModules/Equation.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      865 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/NetworkBehavior/EulerEquationModules/EulerClock.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     1082 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/NetworkBehavior/EulerEquationModules/Helper.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     1695 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/NetworkBehavior/EulerEquationModules/VariableInitializer.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/NetworkBehavior/EulerEquationModules/__init__.py
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-16 07:15:40.090990 pymonntorch-0.1.0/pymonntorch/NetworkBehavior/Recorder/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     7754 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/NetworkBehavior/Recorder/Recorder.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/NetworkBehavior/Recorder/__init__.py
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-16 07:15:40.091222 pymonntorch-0.1.0/pymonntorch/NetworkBehavior/Structure/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)    11408 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/NetworkBehavior/Structure/Structure.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/NetworkBehavior/Structure/__init__.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/NetworkBehavior/__init__.py
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-16 07:15:40.092461 pymonntorch-0.1.0/pymonntorch/NetworkCore/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     8262 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/NetworkCore/AnalysisModule.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)    10630 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/NetworkCore/Base.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     7368 2023-05-16 06:37:35.000000 pymonntorch-0.1.0/pymonntorch/NetworkCore/Behavior.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)    13106 2023-05-13 12:28:56.000000 pymonntorch-0.1.0/pymonntorch/NetworkCore/Network.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)    15236 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/NetworkCore/NeuronGroup.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)    12723 2023-05-13 12:28:56.000000 pymonntorch-0.1.0/pymonntorch/NetworkCore/SynapseGroup.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     4194 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/NetworkCore/TaggableObject.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/NetworkCore/__init__.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      967 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/__init__.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      411 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/cli.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       19 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/pymonntorch.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      459 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/pymonntorch/utils.py
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-16 07:15:40.089619 pymonntorch-0.1.0/pymonntorch.egg-info/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     4273 2023-05-16 07:15:40.000000 pymonntorch-0.1.0/pymonntorch.egg-info/PKG-INFO
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     1721 2023-05-16 07:15:40.000000 pymonntorch-0.1.0/pymonntorch.egg-info/SOURCES.txt
--rw-r--r--   0 atenamohammadi   (501) staff       (20)        1 2023-05-16 07:15:40.000000 pymonntorch-0.1.0/pymonntorch.egg-info/dependency_links.txt
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       53 2023-05-16 07:15:40.000000 pymonntorch-0.1.0/pymonntorch.egg-info/entry_points.txt
--rw-r--r--   0 atenamohammadi   (501) staff       (20)        1 2023-05-09 14:25:31.000000 pymonntorch-0.1.0/pymonntorch.egg-info/not-zip-safe
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       28 2023-05-16 07:15:40.000000 pymonntorch-0.1.0/pymonntorch.egg-info/requires.txt
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       12 2023-05-16 07:15:40.000000 pymonntorch-0.1.0/pymonntorch.egg-info/top_level.txt
--rw-r--r--   0 atenamohammadi   (501) staff       (20)      428 2023-05-16 07:15:40.093177 pymonntorch-0.1.0/setup.cfg
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     1465 2023-05-16 07:09:00.000000 pymonntorch-0.1.0/setup.py
-drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-16 07:15:40.092760 pymonntorch-0.1.0/tests/
--rw-r--r--   0 atenamohammadi   (501) staff       (20)       41 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/tests/__init__.py
--rw-r--r--   0 atenamohammadi   (501) staff       (20)     4169 2023-05-09 07:39:39.000000 pymonntorch-0.1.0/tests/test_pymonntorch.py
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.383475 pymonntorch-0.1.1/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      232 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/AUTHORS.rst
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     3592 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      261 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/HISTORY.rst
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     1118 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/LICENSE
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      262 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/MANIFEST.in
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     4550 2023-05-27 06:20:10.383550 pymonntorch-0.1.1/PKG-INFO
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     3544 2023-05-27 06:18:55.000000 pymonntorch-0.1.1/README.rst
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.376985 pymonntorch-0.1.1/docs/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      612 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/Makefile
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.377490 pymonntorch-0.1.1/docs/_images/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)    42525 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/_images/spike.png
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)   138598 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/_images/voltage.png
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       28 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/authors.rst
+-rwxr-xr-x   0 atenamohammadi   (501) staff       (20)     5024 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/docs/conf.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       33 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/contributing.rst
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     1001 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/documentation.rst
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       28 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/history.rst
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      317 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/index.rst
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     1130 2023-05-19 06:09:06.000000 pymonntorch-0.1.1/docs/installation.rst
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      809 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/make.bat
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       27 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/docs/readme.rst
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     5803 2023-05-19 06:09:57.000000 pymonntorch-0.1.1/docs/tutorial.rst
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.378321 pymonntorch-0.1.1/pymonntorch/
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.379595 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.380166 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Basics/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     5791 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Basics/BasicHomeostasis.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      964 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Basics/Normalization.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Basics/__init__.py
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.381013 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     1426 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/Equation.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      865 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/EulerClock.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     1082 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/Helper.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     1695 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/VariableInitializer.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/__init__.py
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.381339 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Recorder/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     7793 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Recorder/Recorder.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Recorder/__init__.py
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.381654 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Structure/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)    11399 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Structure/Structure.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Structure/__init__.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkBehavior/__init__.py
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.382955 pymonntorch-0.1.1/pymonntorch/NetworkCore/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     8262 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkCore/AnalysisModule.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)    10859 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/pymonntorch/NetworkCore/Base.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     7436 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/pymonntorch/NetworkCore/Behavior.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)    14360 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/pymonntorch/NetworkCore/Network.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)    14984 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/pymonntorch/NetworkCore/NeuronGroup.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)    12458 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/pymonntorch/NetworkCore/SynapseGroup.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     4194 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkCore/TaggableObject.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)        0 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/NetworkCore/__init__.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      967 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/pymonntorch/__init__.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      411 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/cli.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       19 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/pymonntorch.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      459 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/pymonntorch/utils.py
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.379446 pymonntorch-0.1.1/pymonntorch.egg-info/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     4550 2023-05-27 06:20:10.000000 pymonntorch-0.1.1/pymonntorch.egg-info/PKG-INFO
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     1721 2023-05-27 06:20:10.000000 pymonntorch-0.1.1/pymonntorch.egg-info/SOURCES.txt
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)        1 2023-05-27 06:20:10.000000 pymonntorch-0.1.1/pymonntorch.egg-info/dependency_links.txt
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       53 2023-05-27 06:20:10.000000 pymonntorch-0.1.1/pymonntorch.egg-info/entry_points.txt
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)        1 2023-05-09 14:25:31.000000 pymonntorch-0.1.1/pymonntorch.egg-info/not-zip-safe
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       28 2023-05-27 06:20:10.000000 pymonntorch-0.1.1/pymonntorch.egg-info/requires.txt
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       12 2023-05-27 06:20:10.000000 pymonntorch-0.1.1/pymonntorch.egg-info/top_level.txt
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)      428 2023-05-27 06:20:10.383815 pymonntorch-0.1.1/setup.cfg
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     1476 2023-05-27 06:00:43.000000 pymonntorch-0.1.1/setup.py
+drwxr-xr-x   0 atenamohammadi   (501) staff       (20)        0 2023-05-27 06:20:10.383245 pymonntorch-0.1.1/tests/
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)       41 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/tests/__init__.py
+-rw-r--r--   0 atenamohammadi   (501) staff       (20)     4169 2023-05-09 07:39:39.000000 pymonntorch-0.1.1/tests/test_pymonntorch.py
```

### Comparing `pymonntorch-0.1.0/CONTRIBUTING.rst` & `pymonntorch-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.0/LICENSE` & `pymonntorch-0.1.1/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023, Computational Neuroscience Laboratory (CNRL) & Maius Vieth
+Copyright (c) 2023, Computational Neuroscience Laboratory (CNRL) & Marius Vieth
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pymonntorch-0.1.0/PKG-INFO` & `pymonntorch-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: pymonntorch
-Version: 0.1.0
+Version: 0.1.1
 Summary: PymoNNtorch is a Pytorch version of PymoNNto
 Home-page: https://github.com/cnrl/PymoNNtorch
 Author: Computational Neuroscience Research Laboratory
 Author-email: ashenatena@gmail.com
 License: MIT license
 Keywords: pymonntorch
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ===========
 PymoNNtorch
 ===========
 
 
 .. image:: https://img.shields.io/pypi/v/pymonntorch.svg
         :target: https://pypi.python.org/pypi/pymonntorch
 
-.. image:: https://img.shields.io/travis/cnrl/pymonntorch.svg
-        :target: https://travis-ci.com/cnrl/pymonntorch
+.. .. image:: https://img.shields.io/travis/cnrl/pymonntorch.svg
+..         :target: https://travis-ci.com/cnrl/pymonntorch
 
 .. image:: https://readthedocs.org/projects/pymonntorch/badge/?version=latest
         :target: https://pymonntorch.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
 
@@ -124,16 +126,23 @@
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 It changes the codebase of `PymoNNto <https://github.com/trieschlab/PymoNNto>`_ to use ``torch`` rather than ``numpy`` and ``tensorflow numpy``.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
-
 =======
 History
 =======
 
+0.1.1 (2023-05-26)
+------------------
+
+* Every NetworkObject can have a recorder behavior.
+* Netowrk settings accept "index" entry.
+* Bug fixes and general improvement.
+
+
 0.1.0 (2023-03-17)
 ------------------
 
 * Repository made public.
```

### Comparing `pymonntorch-0.1.0/README.rst` & `pymonntorch-0.1.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 PymoNNtorch
 ===========
 
 
 .. image:: https://img.shields.io/pypi/v/pymonntorch.svg
         :target: https://pypi.python.org/pypi/pymonntorch
 
-.. image:: https://img.shields.io/travis/cnrl/pymonntorch.svg
-        :target: https://travis-ci.com/cnrl/pymonntorch
+.. .. image:: https://img.shields.io/travis/cnrl/pymonntorch.svg
+..         :target: https://travis-ci.com/cnrl/pymonntorch
 
 .. image:: https://readthedocs.org/projects/pymonntorch/badge/?version=latest
         :target: https://pymonntorch.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
 
@@ -103,8 +103,8 @@
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 It changes the codebase of `PymoNNto <https://github.com/trieschlab/PymoNNto>`_ to use ``torch`` rather than ``numpy`` and ``tensorflow numpy``.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `pymonntorch-0.1.0/docs/Makefile` & `pymonntorch-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.0/docs/_images/spike.png` & `pymonntorch-0.1.1/docs/_images/spike.png`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.0/docs/_images/voltage.png` & `pymonntorch-0.1.1/docs/_images/voltage.png`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.0/docs/conf.py` & `pymonntorch-0.1.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto, manual, or own class]).
 latex_documents = [
     (master_doc, 'pymonntorch.tex',
      'PymoNNtorch Documentation',
-     'Ashena Gorgan Mohammadi', 'manual'),
+     'CNRL', 'manual'),
 ]
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
```

### Comparing `pymonntorch-0.1.0/docs/documentation.rst` & `pymonntorch-0.1.1/docs/documentation.rst`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.0/docs/installation.rst` & `pymonntorch-0.1.1/docs/installation.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 .. highlight:: shell
 
 ============
 Installation
 ============
 
 
-.. Stable release
-.. --------------
+Stable release
+--------------
 
-.. To install PymoNNtorch, run this command in your terminal:
+To install PymoNNtorch, run this command in your terminal:
 
-.. .. code-block:: console
+.. code-block:: console
 
-..     $ pip install pymonntorch
+    $ pip install pymonntorch
 
-.. This is the preferred method to install PymoNNtorch, as it will always install the most recent stable release.
+This is the preferred method to install PymoNNtorch, as it will always install the most recent stable release.
 
-.. If you don't have `pip`_ installed, this `Python installation guide`_ can guide
-.. you through the process.
+If you don't have `pip`_ installed, this `Python installation guide`_ can guide
+you through the process.
 
-.. .. _pip: https://pip.pypa.io
-.. .. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
+.. _pip: https://pip.pypa.io
+.. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
 
 
 From sources
 ------------
 
 The sources for PymoNNtorch can be downloaded from the `Github repo`_.
```

### Comparing `pymonntorch-0.1.0/docs/make.bat` & `pymonntorch-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.0/docs/tutorial.rst` & `pymonntorch-0.1.1/docs/tutorial.rst`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     net = Network()
     ng = NeuronGroup(net=net, size=1000, behavior={})
     syn = SynapseGroup(net=net, src=ng, dst=ng, tag='GLUTAMATE')
 
 So far, ``ng`` has been added to network ``net`` and synaptic connection has been defined to connect ``ng`` to itself, i.e. both afferent and efferent synapses of ``ng`` are ``syn``. By default, each network and its components are created on CPU and the data type of any tensor inside the objects is set to ``torch.float32``. Pass an argument ``settings`` to the ``Network`` to change these default setups. ``settings`` is a dictionary with keys ``device`` and ``def_dtype`` which indicate the device and data type of everything within the network, respectively.
 
-To have a functioning network, we can write ``Behavior``(s) for different network objects to define dynamics and attributes for them. To do so, we can proceed as follows: ::
+To have a functioning network, we can write ``Behavior`` (s) for different network objects to define dynamics and attributes for them. To do so, we can proceed as follows: ::
 
     class BasicBehavior(Behavior):  # Any user-defined behavior should inherit pymonntorch.NetworkCore.Behavior
         # This behavior is defining dynamics for NeuronGroups
         def initialize(self, neurons):  # override this method to define and initialize attributes. This is called upon calling Network's initialize method.
 
             super().initialize(neurons)  # Always remember to call the super method to ensure all objects and tensors are located on the same device.
```

### Comparing `pymonntorch-0.1.0/pymonntorch/NetworkBehavior/Basics/BasicHomeostasis.py` & `pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Basics/BasicHomeostasis.py`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.0/pymonntorch/NetworkBehavior/Basics/Normalization.py` & `pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Basics/Normalization.py`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.0/pymonntorch/NetworkBehavior/EulerEquationModules/Equation.py` & `pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/Equation.py`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.0/pymonntorch/NetworkBehavior/EulerEquationModules/EulerClock.py` & `pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/EulerClock.py`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.0/pymonntorch/NetworkBehavior/EulerEquationModules/Helper.py` & `pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/Helper.py`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.0/pymonntorch/NetworkBehavior/EulerEquationModules/VariableInitializer.py` & `pymonntorch-0.1.1/pymonntorch/NetworkBehavior/EulerEquationModules/VariableInitializer.py`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.0/pymonntorch/NetworkBehavior/Recorder/Recorder.py` & `pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Recorder/Recorder.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,37 +19,38 @@
     return Recorder(variables=[variable])
 
 
 class Recorder(Behavior):
     """This is the base class to record variables of a network object.
     
     Args:
-        variables (list of str): List of variable names to record.
+        variables (list of str): List of variable names to record. A variable should be of tensor type.
         gap_width (int): The intervals of time to record variables. The default is 0.
         tag (str): A tag name for the `Recorder` object. The default is None.
         max_length (int): The history buffer size. If `None`, the variables are recorded \
             for the whole simulation time. The default is None.
         auto_annotate (bool): This parameter specifies whether the variable names include the \
             network object prefix (neurons/synapse/n/s) or not. The default is True.
     """
+
     initialize_last = True
     visualization_module_outputs = []
 
     def initialize(self, object):
         super().initialize(object)
 
-        variables = self.parameter('variables', [])
+        variables = self.parameter("variables", [])
         if variables == []:
-            variables = self.parameter('arg_0', [])
+            variables = self.parameter("arg_0", [])
         if isinstance(variables, str):
             variables = [variables]
 
-        self.gap_width = self.parameter('gap_width', 0)
-        self.max_length = self.parameter('max_length', None)
-        self.auto_annotate = self.parameter('auto_annotate', True)
+        self.gap_width = self.parameter("gap_width", 0)
+        self.max_length = self.parameter("max_length", None)
+        self.auto_annotate = self.parameter("auto_annotate", True)
         self.counter = 0
         self.new_data_available = False
         self.variables = {}
         self.compiled = {}
 
         self.add_variables(variables)
         self.reset()
@@ -197,14 +198,15 @@
         gap_width (int): The intervals of time to record variables. The default is 0.
         tag (str): A tag name for the `Recorder` object. The default is None.
         max_length (int): The history buffer size. If `None`, the variables are recorded \
             for the whole simulation time. The default is None.
         auto_annotate (bool): This parameter specifies whether the variable names include the \
             network object prefix (neurons/synapse/n/s) or not. The default is True.
     """
+
     def find_objects(self, key):
         result = []
         if key in self.variables:
             result.append(self.variables[key])
 
         if type(key) is str and key[-2:] == ".t" and key[:-2] in self.variables:
             result.append(self.variables[key[:-2]][:, 0])
```

### Comparing `pymonntorch-0.1.0/pymonntorch/NetworkBehavior/Structure/Structure.py` & `pymonntorch-0.1.1/pymonntorch/NetworkBehavior/Structure/Structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,33 +87,34 @@
 
     return NeuronDimension(width=width, height=height, depth=depth)
 
 
 class NeuronDimension(Behavior):
     """
     The Behavior that defines structure for a `NeuronGroup`.
-    It overrides the `size` variable of the `NeuronGroup` and adds `x`, `y`, and `z` vectors, 
-    as well as `width`, `height` and `depth` variables. The Behaviour is special, because its 
-    `initialize` function is executed when the `NeuronGroup` is created rather than 
-    when network.initialize() is called. The neurons are arranged in a 3-dimensional grid 
-    with size=width * height * depth. Because is overrides the `size` variable, it does not 
-    have to be added in the behaviour dictionary directly, but also indirectly 
-    ( `NeuronGroup(size=NeuronDimension(),...)` ). In this case it will be added to 
+    It overrides the `size` variable of the `NeuronGroup` and adds `x`, `y`, and `z` vectors,
+    as well as `width`, `height` and `depth` variables. The Behaviour is special, because its
+    `initialize` function is executed when the `NeuronGroup` is created rather than
+    when network.initialize() is called. The neurons are arranged in a 3-dimensional grid
+    with size=width * height * depth. Because is overrides the `size` variable, it does not
+    have to be added in the behaviour dictionary directly, but also indirectly
+    ( `NeuronGroup(size=NeuronDimension(),...)` ). In this case it will be added to
     position 0 in the dictionary.
 
     Args:
         width (int): Width of the `NeuronGroup`. The default is 1.
         height (int): Height of the `NeuronGroup`. The default is 1.
         depth (int): Depth of the `NeuronGroup`. The default is 1.
     """
+
     initialize_on_init = True
 
     def set_position(self, width, height, depth):
         """Set the coordinate of neurons by setting vectors `x`, `y`, and `z`.
-        
+
         Args:
             width (int): Width of the neurons.
             height (int): Height of the neurons.
             depth (int): Depth of the neurons.
         """
         self.neurons.x = (
             torch.arange(
@@ -148,17 +149,17 @@
                 (width * height),
                 rounding_mode="floor",
             )
             % depth
         )
 
     def get_area_mask(self, xmin=0, xmax=-1, ymin=0, ymax=-1, zmin=0, zmax=-1):
-        """Returns a mask tensor with the same shape as the NeuronGroup 
+        """Returns a mask tensor with the same shape as the NeuronGroup
         with the given start and end points.
-        
+
         Args:
             xmin (int): Start point in x axis. The default is 0.
             xmax (int): End point in x axis. The default is -1.
             ymin (int): Start point in y axis. The default is 0.
             ymax (int): End point in y axis. The default is -1.
             zmin (int): Start point in z axis. The default is 0.
             zmax (int): End point in z axis. The default is -1.
@@ -181,15 +182,15 @@
             device=self.neurons.device,
         )
         result[zmin:zmax, ymin:ymax, xmin:xmax] = True
         return result.flatten()
 
     def apply_pattern_transformation_function(self, transform_mat, hup, wup, depth):
         """Apply a transformation matrix on the neurons.
-        
+
         Args:
             transform_mat (torch.tensor): The transformation matrix.
             hup (int): The height upperbound.
             wup (int): The width upperbound.
             depth (int): The depth.
         """
         big_x_mat = torch.stack(
@@ -206,15 +207,15 @@
         )
 
         self.neurons.x = big_x_mat[transform_mat]
         self.neurons.y = big_y_mat[transform_mat]
 
     def move(self, x=0, y=0, z=0):
         """Move the neurons in the 3D space.
-        
+
         Args:
             x (int or float): The displacement in x axis.
             y (int or float): The displacement in y axis.
             z (int or float): The displacement in z axis.
 
         Returns:
             NeuronDimension: The modified `NeuronDimension`.
@@ -222,15 +223,15 @@
         self.neurons.x += x
         self.neurons.y += y
         self.neurons.z += z
         return self
 
     def scale(self, x=1, y=1, z=1):
         """Scale the neuron grid in the 3D space.
-        
+
         Args:
             x (int or float): The stretch in x axis.
             y (int or float): The stretch in y axis.
             z (int or float): The stretch in z axis.
 
         Returns:
             NeuronDimension: The modified `NeuronDimension`.
@@ -238,15 +239,15 @@
         self.neurons.x *= x
         self.neurons.y *= y
         self.neurons.z *= z
         return self
 
     def noise(self, x_noise=1, y_noise=1, z_noise=1):
         """Apply random noise to neuron coordinates.
-        
+
         Args:
             x (int or float): The noise bounds in x axis.
             y (int or float): The noise bounds in y axis.
             z (int or float): The noise bounds in z axis.
 
         Returns:
             NeuronDimension: The modified `NeuronDimension`.
@@ -260,15 +261,15 @@
         self.neurons.z += torch.randint(
             -z_noise, z_noise, self.neurons.size, device=self.neurons.device
         )
         return self
 
     def rotate(self, axis, angle):
         """Rotate the `NeuronGroup` in space.
-        
+
         Args:
             axis (int): The axis along which the rotation is made.
             angle (float): The angle to rotate in radians.
 
         Returns:
             NeuronDimension: The modified `NeuronDimension`.
         """
@@ -276,15 +277,15 @@
         self.neurons.x, self.neurons.y, self.neurons.z = torch.matmul(
             rotation, torch.stack([self.neurons.x, self.neurons.y, self.neurons.z])
         )
         return self
 
     def stretch_to_equal_size(self, target_neurons):
         """Stretch to `NeuronGroup` to match a target `NeuronGroup` dimensions.
-        
+
         Args:
             target_neurons (NeuronGroup): The target `NeuronGroup`.
         """
         if hasattr(target_neurons, "width") and self.neurons.width > 0:
             x_stretch = target_neurons.width / self.neurons.width
             self.neurons.x *= x_stretch
         if hasattr(target_neurons, "height") and self.neurons.height > 0:
@@ -317,13 +318,14 @@
         neurons.shape = self
         neurons.width = self.width
         neurons.height = self.height
         neurons.depth = self.depth
 
         neurons.size = self.width * self.height * self.depth
 
-        self.set_position(self.width, self.height, self.depth)
+        if neurons.network.index_neurons:
+            self.set_position(self.width, self.height, self.depth)
 
-        if self.parameter("centered", True, neurons):
-            self.move(
-                -(self.width - 1) / 2, -(self.height - 1) / 2, -(self.depth - 1) / 2
-            )
+            if self.parameter("centered", True, neurons):
+                self.move(
+                    -(self.width - 1) / 2, -(self.height - 1) / 2, -(self.depth - 1) / 2
+                )
```

### Comparing `pymonntorch-0.1.0/pymonntorch/NetworkCore/AnalysisModule.py` & `pymonntorch-0.1.1/pymonntorch/NetworkCore/AnalysisModule.py`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.0/pymonntorch/NetworkCore/Base.py` & `pymonntorch-0.1.1/pymonntorch/NetworkCore/Base.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,26 +40,28 @@
 
         for k in sorted(list(self.behavior.keys())):
             if self.behavior[k].initialize_on_init:
                 self.behavior[k].initialize(self)
 
         self.analysis_modules = []
 
+        self.recording = True
+
     def add_behavior(self, key, behavior, initialize=True):
         """Add a single behavior to the network object.
 
         Args:
             key (str): Key to be used to access behavior.
             behavior (Behavior): Behavior to be added.
             initialize (bool): If true, behavior will be initialized. The default is True.
 
         Returns:
             Behavior: The behavior.
         """
-        if not key in self.behavior:
+        if key not in self.behavior:
             self.behavior[key] = behavior
             self.network._add_behavior_to_sorted_execution_list(
                 key, self, self.behavior[key]
             )
             self.network.clear_tag_cache()
             if initialize:
                 behavior.initialize(self)
@@ -284,18 +286,26 @@
             .reshape(size, *dim)
             .to(self.device)
         )
 
     @property
     def iteration(self):
         """int: iteration number or time step."""
-        return self._iteration
+        return self.network._iteration
 
     @iteration.setter
     def iteration(self, iteration):
         if iteration >= 0 and type(iteration) is int:
-            self._iteration = iteration
+            self.network._iteration = iteration
         else:
             print(
                 "WARNING: Attempting to set an invalid value for iteration!\n Setting iteration to zero..."
             )
-            self._iteration = 0
+            self.network._iteration = 0
+
+    @property
+    def def_dtype(self):
+        return self.network._def_dtype
+
+    @def_dtype.setter
+    def def_dtype(self, dtype):
+        self.network._def_dtype = dtype
```

### Comparing `pymonntorch-0.1.0/pymonntorch/NetworkCore/Behavior.py` & `pymonntorch-0.1.1/pymonntorch/NetworkCore/Behavior.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         """Forward pass of the behavior. This method is called by the `Network` class per simulation iteration.
 
         Args:
             object (TaggableObject): Object possessing the behavior.
         """
         pass
 
-    def __str__(self):
+    def __repr__(self):
         result = self.__class__.__name__ + "("
         for k in self.init_kwargs:
             result += str(k) + "=" + str(self.init_kwargs[k]) + ","
         result += ")"
         return result
 
     def evaluate_diversity_string(self, ds, object):
@@ -109,26 +109,27 @@
         for key in self.init_kwargs:
             setattr(object, key, self.parameter(key, None, object=object))
             print("init", key)
 
     def check_unused_attrs(self):
         """Checks whether all attributes have been used in the `initialize` method."""
         for key in self.init_kwargs:
-            if not key in self.used_attr_keys:
+            if key not in self.used_attr_keys:
                 print(
                     'Warning: "'
                     + key
                     + '" not used in initialize of '
                     + str(self)
                     + ' behavior! Make sure that "'
                     + key
                     + '" is spelled correctly and parameter('
                     + key
-                    + ",...) is called in initialize. Valid attributes are:"
-                    + str(self.used_attr_keys)
+                    + ",...) is called in initialize. Valid attributes are: "
+                    + ", ".join([f'"{param}"' for param in list(self.used_attr_keys)])
+                    + "."
                 )
 
     def parameter(
         self,
         key,
         default,
         object=None,
@@ -145,15 +146,15 @@
             do_not_diversify (bool): Whether to diversify the attribute. The default is False.
             search_other_behaviors (bool): Whether to search for the attribute in other behaviors of the object. The default is False.
             required (bool): Whether the attribute is required. The default is False.
 
         Returns:
             any: The value of the attribute.
         """
-        if required and not key in self.init_kwargs:
+        if required and key not in self.init_kwargs:
             print(
                 "Warning:",
                 key,
                 "has to be specified for the behavior to run properly.",
                 self,
             )
```

### Comparing `pymonntorch-0.1.0/pymonntorch/NetworkCore/Network.py` & `pymonntorch-0.1.1/pymonntorch/NetworkCore/Network.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,38 +2,45 @@
 
 import torch
 
 from pymonntorch.NetworkCore.Base import *
 from pymonntorch.NetworkCore.Behavior import Behavior
 from pymonntorch.NetworkCore.SynapseGroup import *
 
-SxD = 0
-DxS = 1
+SxD = False
+DxS = True
 
 
 class Network(NetworkObject):
     """This is the class to construct a neural network.
 
     This is the placeholder of all neural network components to be simulated.
     All objects will receive an instance of this class.
 
     Attributes:
         NeuronGroups (list): List of all NeuronGroups in the network.
         SynapseGroups (list): List of all SynapseGroups in the network.
         behavior (list or dict): List of all network-specific behaviors.
-        settings (dict): Dictionary of network-wide settings, e.g. `def_dtype`, `synapse_mode` and `device`.
+        def_dtype (type): Floating point precision of tensors. Defaults to `torch.float32`; can be changed via setttings with "dtype" key.
+        device (string): The device to allocate tensors' memory on. Defaults to `'cpu'`; can be changed via setttings with "device" key.
+        transposed_synapse_matrix_mode (bool): If `True`, in the matrix created by synapse, each row corresponds to a neuron from the source neuron group. Defaults to `False`; can be changed via settings with the "synapse_mode" key, which can have `DxS` and `SxD` as possible values.
+        index_neurons (bool): If True, the `id` attribute for neuron groups refers to neuron indices. Defaults to `True`; can be changed via setttings with "index" key.
     """
 
     def __init__(self, tag=None, behavior=None, settings=None):
         """Initialize the network.
 
         Args:
             tag (str): Tag to add to the network. It can also be a comma-separated string of multiple tags.
             behavior (list or dict): List or dictionary of behaviors. If a dictionary is used, the keys must be integers.
-            device (str): Device on which the network is located. The default is "cpu".
+            settings (dict): Dictionary of network-wide settings, e.g. `dtype`, `synapse_mode`, `device` and `index`.
+                             `dtype`: Floating point precision of tensors. Defaults to `torch.float32`.
+                             `synapse_mode`: If `SxD`, rows of matrix created by a synapse referes to the source neuron group and columns referes to the Destination neurpn group. Possible values `DxS` and `SxD`.
+                             `device`: The device to allocate tensors' data on. Defaults to `'cpu'`.
+                             `index`: If True, create an indexing tensor as `id` attribute for each neuron group.
         """
         settings = settings if settings is not None else {}
         self.apply_settings(settings)
 
         self.NeuronGroups = []
         self.SynapseGroups = []
 
@@ -43,15 +50,16 @@
             []
         )  # stores (key, beh_parent, behavior) triplets
 
         super().__init__(tag, self, behavior, device=self.device)
 
     def apply_settings(self, settings):
         self.device = settings.setdefault("device", "cpu")
-        self.def_dtype = settings.setdefault("dtype", torch.float32)
+        self._def_dtype = settings.setdefault("dtype", torch.float32)
+        self.index_neurons = settings.setdefault("index", True)
         self.transposed_synapse_matrix_mode = (
             settings.setdefault("synapse_mode", DxS) != DxS
         )
 
     def set_behaviors(self, tag, enabled):
         """Set behaviors of specific tag to be enabled or disabled.
 
@@ -97,15 +105,15 @@
         for obj in self.all_objects():
             for key in obj.behavior:
                 if (keys is None or key in keys) and hasattr(
                     obj.behavior[key], "clear_recorder"
                 ):
                     obj.behavior[key].clear_recorder()
 
-    def __str__(self):
+    def __repr__(self):
         neuron_count = torch.sum(torch.tensor([ng.size for ng in self.NeuronGroups]))
         synapse_count = torch.sum(
             torch.tensor([sg.src.size * sg.dst.size for sg in self.SynapseGroups])
         )
 
         basic_info = (
             "(Neurons: "
```

### Comparing `pymonntorch-0.1.0/pymonntorch/NetworkCore/NeuronGroup.py` & `pymonntorch-0.1.1/pymonntorch/NetworkCore/NeuronGroup.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,18 +57,16 @@
             setattr(net, self.tags[0], self)
 
         self.afferent_synapses = {}  # set by Network
         self.efferent_synapses = {}
 
         self.mask = True
 
-        self.learning = True
-        self.recording = True
-
-        self.id = torch.arange(self.size, device=self.device)
+        if net.index_neurons:
+            self.id = torch.arange(self.size, device=self.device)
 
     def synapses(self, mode, tag="All"):
         """Get synapses connected to the NeuronGroup.
 
         Args:
             mode (str or bool): Whether to return efferent or afferent synapses connected to the NeuronGroup.
                                 Values indicating afferent: ` "afferent", "dendrite", "pre", "preSynaptic", 0, False `
@@ -79,22 +77,14 @@
             List[SynapseGroup]: The list containing SynapseGroups
         """
         if mode in ["afferent", "dendrite", "pre", "preSynaptic", 0]:
             return self.afferent_synapses[tag]
         if mode in ["efferent", "axon", "post", "postSynaptic", 1]:
             return self.efferent_synapses[tag]
 
-    @property
-    def def_dtype(self):
-        self.network.def_dtype
-
-    @property
-    def iteration(self):
-        return self.network.iteration
-
     def require_synapses(self, name, afferent=True, efferent=True, warning=True):
         """Require the existence of synapses.
 
         Args:
             name (str): The name of the synapse.
             afferent (bool): Whether to require afferent synapses.
             efferent (bool): Whether to require efferent synapses.
@@ -163,15 +153,15 @@
         """
         source_num = 0
         for syn in self.afferent_synapses[Synapse_ID]:
             _, s = syn.matrix_dim()
             source_num += s
         return self.size, source_num
 
-    def __str__(self):
+    def __repr__(self):
         result = "NeuronGroup" + str(self.tags) + "(" + str(self.size) + "){"
         for k in sorted(list(self.behavior.keys())):
             result += str(k) + ":" + str(self.behavior[k])
         return result + "}"
 
     def subGroup(self, mask=None):
         """Get a NeuronSubGroup object from the population.
@@ -363,18 +353,14 @@
             var (torch.Tensor): The variable.
 
         Returns:
             torch.Tensor: The masked variable.
         """
         return var
 
-    @property
-    def def_dtype(self):
-        return self.network.def_dtype
-
 
 class NeuronSubGroup:
     def __init__(self, BaseNeuronGroup, mask):
         self.cache = {}
         self.key_id_cache = {}
         self.BaseNeuronGroup = BaseNeuronGroup
         self.mask = mask
```

### Comparing `pymonntorch-0.1.0/pymonntorch/NetworkCore/SynapseGroup.py` & `pymonntorch-0.1.1/pymonntorch/NetworkCore/SynapseGroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,14 @@
         if len(src.tags) > 0 and len(dst.tags) > 0:
             self.add_tag(src.tags[0] + " => " + dst.tags[0])
 
         if net is not None:
             net.SynapseGroups.append(self)
             setattr(net, self.tags[0], self)
 
-        self.recording = True
-
         self.src = src
         self.dst = dst
         self.enabled = True
         self.group_weighting = 1
 
         for ng in self.network.NeuronGroups:
             for tag in self.tags + ["All"]:
@@ -90,22 +88,14 @@
 
         Returns:
             SynapseGroup: The synapse group itself.
         """
         setattr(self, key, value)
         return self
 
-    @property
-    def def_dtype(self):
-        return self.network.def_dtype
-
-    @property
-    def iteration(self):
-        return self.network.iteration
-
     def matrix_dim(self):
         """Returns the dimension of the synapse matrix.
 
         For a synapse group between a source population of size n and a destination population of size m, the synapse matrix has the dimension m x n.
 
         Returns:
             tuple: The dimension of the synapse matrix.
@@ -326,11 +316,7 @@
             if key == "behavior":
                 for k in self.behavior:
                     result.behavior[k] = copy.copy(self.behavior[k])
             elif key not in ["src", "dst", "enabled", "_mat_eval_dict"]:
                 setattr(result, key, copy.copy(sgd[key]))
 
         return result
-
-    @property
-    def def_dtype(self):
-        return self.network.def_dtype
```

### Comparing `pymonntorch-0.1.0/pymonntorch/NetworkCore/TaggableObject.py` & `pymonntorch-0.1.1/pymonntorch/NetworkCore/TaggableObject.py`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.0/pymonntorch/__init__.py` & `pymonntorch-0.1.1/pymonntorch/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for PymoNNtorch."""
 
 __author__ = """Computational Neuroscience Research Laboratory"""
-__email__ = 'ashenatena@gmail.com'
-__version__ = '0.1.0'
+__email__ = "ashenatena@gmail.com"
+__version__ = "0.1.1"
 
 from pymonntorch.NetworkCore.Network import *
 from pymonntorch.NetworkCore.Behavior import *
 from pymonntorch.NetworkCore.NeuronGroup import *
 from pymonntorch.NetworkCore.SynapseGroup import *
 from pymonntorch.NetworkCore.AnalysisModule import *
```

### Comparing `pymonntorch-0.1.0/pymonntorch.egg-info/PKG-INFO` & `pymonntorch-0.1.1/pymonntorch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: pymonntorch
-Version: 0.1.0
+Version: 0.1.1
 Summary: PymoNNtorch is a Pytorch version of PymoNNto
 Home-page: https://github.com/cnrl/PymoNNtorch
 Author: Computational Neuroscience Research Laboratory
 Author-email: ashenatena@gmail.com
 License: MIT license
 Keywords: pymonntorch
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ===========
 PymoNNtorch
 ===========
 
 
 .. image:: https://img.shields.io/pypi/v/pymonntorch.svg
         :target: https://pypi.python.org/pypi/pymonntorch
 
-.. image:: https://img.shields.io/travis/cnrl/pymonntorch.svg
-        :target: https://travis-ci.com/cnrl/pymonntorch
+.. .. image:: https://img.shields.io/travis/cnrl/pymonntorch.svg
+..         :target: https://travis-ci.com/cnrl/pymonntorch
 
 .. image:: https://readthedocs.org/projects/pymonntorch/badge/?version=latest
         :target: https://pymonntorch.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
 
@@ -124,16 +126,23 @@
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 It changes the codebase of `PymoNNto <https://github.com/trieschlab/PymoNNto>`_ to use ``torch`` rather than ``numpy`` and ``tensorflow numpy``.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
-
 =======
 History
 =======
 
+0.1.1 (2023-05-26)
+------------------
+
+* Every NetworkObject can have a recorder behavior.
+* Netowrk settings accept "index" entry.
+* Bug fixes and general improvement.
+
+
 0.1.0 (2023-03-17)
 ------------------
 
 * Repository made public.
```

### Comparing `pymonntorch-0.1.0/pymonntorch.egg-info/SOURCES.txt` & `pymonntorch-0.1.1/pymonntorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymonntorch-0.1.0/tests/test_pymonntorch.py` & `pymonntorch-0.1.1/tests/test_pymonntorch.py`

 * *Files identical despite different names*

