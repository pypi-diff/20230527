# Comparing `tmp/CUQIpy-CIL-0.3.0.post0.dev2.tar.gz` & `tmp/CUQIpy-CIL-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CUQIpy-CIL-0.3.0.post0.dev2.tar", last modified: Mon May  1 06:34:22 2023, max compression
+gzip compressed data, was "CUQIpy-CIL-0.4.0.tar", last modified: Sat May 27 08:29:36 2023, max compression
```

## Comparing `CUQIpy-CIL-0.3.0.post0.dev2.tar` & `CUQIpy-CIL-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:34:22.542355 CUQIpy-CIL-0.3.0.post0.dev2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:34:22.542355 CUQIpy-CIL-0.3.0.post0.dev2/CUQIpy_CIL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-01 06:34:22.000000 CUQIpy-CIL-0.3.0.post0.dev2/CUQIpy_CIL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-01 06:34:22.000000 CUQIpy-CIL-0.3.0.post0.dev2/CUQIpy_CIL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 06:34:22.000000 CUQIpy-CIL-0.3.0.post0.dev2/CUQIpy_CIL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-01 06:34:22.000000 CUQIpy-CIL-0.3.0.post0.dev2/CUQIpy_CIL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 06:34:22.000000 CUQIpy-CIL-0.3.0.post0.dev2/CUQIpy_CIL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-01 06:34:22.542355 CUQIpy-CIL-0.3.0.post0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:34:22.542355 CUQIpy-CIL-0.3.0.post0.dev2/cuqipy_cil/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/cuqipy_cil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-01 06:34:22.542355 CUQIpy-CIL-0.3.0.post0.dev2/cuqipy_cil/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/cuqipy_cil/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/cuqipy_cil/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/cuqipy_cil/testproblem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 06:34:22.542355 CUQIpy-CIL-0.3.0.post0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:34:22.542355 CUQIpy-CIL-0.3.0.post0.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-01 06:34:01.000000 CUQIpy-CIL-0.3.0.post0.dev2/tests/test_testproblem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:29:36.712808 CUQIpy-CIL-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:29:36.712808 CUQIpy-CIL-0.4.0/CUQIpy_CIL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14792 2023-05-27 08:29:36.000000 CUQIpy-CIL-0.4.0/CUQIpy_CIL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-27 08:29:36.000000 CUQIpy-CIL-0.4.0/CUQIpy_CIL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 08:29:36.000000 CUQIpy-CIL-0.4.0/CUQIpy_CIL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 08:29:36.000000 CUQIpy-CIL-0.4.0/CUQIpy_CIL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-27 08:29:36.000000 CUQIpy-CIL-0.4.0/CUQIpy_CIL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-27 08:29:25.000000 CUQIpy-CIL-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14792 2023-05-27 08:29:36.712808 CUQIpy-CIL-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-27 08:29:25.000000 CUQIpy-CIL-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:29:36.712808 CUQIpy-CIL-0.4.0/cuqipy_cil/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-27 08:29:25.000000 CUQIpy-CIL-0.4.0/cuqipy_cil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-27 08:29:36.716807 CUQIpy-CIL-0.4.0/cuqipy_cil/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-27 08:29:25.000000 CUQIpy-CIL-0.4.0/cuqipy_cil/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-05-27 08:29:25.000000 CUQIpy-CIL-0.4.0/cuqipy_cil/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-05-27 08:29:25.000000 CUQIpy-CIL-0.4.0/cuqipy_cil/testproblem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-27 08:29:25.000000 CUQIpy-CIL-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-27 08:29:25.000000 CUQIpy-CIL-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 08:29:36.712808 CUQIpy-CIL-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-27 08:29:25.000000 CUQIpy-CIL-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:29:36.712808 CUQIpy-CIL-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-27 08:29:25.000000 CUQIpy-CIL-0.4.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-27 08:29:25.000000 CUQIpy-CIL-0.4.0/tests/test_testproblem.py
```

### Comparing `CUQIpy-CIL-0.3.0.post0.dev2/CUQIpy_CIL.egg-info/PKG-INFO` & `CUQIpy-CIL-0.4.0/CUQIpy_CIL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy-CIL
-Version: 0.3.0.post0.dev2
+Version: 0.4.0
 Summary: CUQIpy plugin for CIL
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `CUQIpy-CIL-0.3.0.post0.dev2/LICENSE` & `CUQIpy-CIL-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CUQIpy-CIL-0.3.0.post0.dev2/PKG-INFO` & `CUQIpy-CIL-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy-CIL
-Version: 0.3.0.post0.dev2
+Version: 0.4.0
 Summary: CUQIpy plugin for CIL
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `CUQIpy-CIL-0.3.0.post0.dev2/README.md` & `CUQIpy-CIL-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `CUQIpy-CIL-0.3.0.post0.dev2/cuqipy_cil/config.py` & `CUQIpy-CIL-0.4.0/cuqipy_cil/config.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-CIL-0.3.0.post0.dev2/cuqipy_cil/model.py` & `CUQIpy-CIL-0.4.0/cuqipy_cil/model.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-CIL-0.3.0.post0.dev2/cuqipy_cil/testproblem.py` & `CUQIpy-CIL-0.4.0/cuqipy_cil/testproblem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-CIL-0.3.0.post0.dev2/pyproject.toml` & `CUQIpy-CIL-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CUQIpy-CIL-0.3.0.post0.dev2/tests/test_model.py` & `CUQIpy-CIL-0.4.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-CIL-0.3.0.post0.dev2/tests/test_testproblem.py` & `CUQIpy-CIL-0.4.0/tests/test_testproblem.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         im_size=(256, 256),
         det_count=256,
         angles=np.linspace(0, np.pi, 180),
         phantom="shepp-logan",
     )
 
     # Cauchy difference prior
-    TP.prior = cuqi.distribution.Cauchy_diff(
+    TP.prior = cuqi.distribution.CMRF(
         location=np.zeros(TP.model.domain_dim),
         scale=0.01,
         physical_dim=2,
     )
 
     # Sample posterior with automatic sampler choice
     samples = TP.sample_posterior(20)
```

