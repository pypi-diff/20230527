# Comparing `tmp/autora-experiment-runner-experimentation-manager-firebase-1.0.0a3.tar.gz` & `tmp/autora-experiment-runner-experimentation-manager-firebase-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experiment-runner-experimentation-manager-firebase-1.0.0a3.tar", last modified: Sat May 27 19:36:03 2023, max compression
+gzip compressed data, was "autora-experiment-runner-experimentation-manager-firebase-1.0.0a4.tar", last modified: Sat May 27 19:37:48 2023, max compression
```

## Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a3.tar` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:36:03.314418 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:36:03.306419 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:36:03.310418 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-27 19:35:51.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-27 19:35:51.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-27 19:35:51.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-27 19:36:03.314418 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-27 19:35:51.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:36:03.310418 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-27 19:35:51.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/docs/SweetPea.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-27 19:35:51.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:36:03.310418 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-27 19:35:51.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-27 19:35:51.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:36:03.310418 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-27 19:35:51.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-27 19:35:51.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-27 19:35:51.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 19:36:03.314418 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:36:03.310418 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:36:03.310418 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:36:03.310418 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:36:03.310418 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/src/autora/experiment_runner/experimentation_manager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:36:03.310418 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/src/autora/experiment_runner/experimentation_manager/firebase/
--rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-05-27 19:35:51.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/src/autora/experiment_runner/experimentation_manager/firebase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:36:03.310418 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-27 19:36:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-27 19:36:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 19:36:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-27 19:36:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 19:36:03.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:36:03.314418 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-27 19:35:51.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 19:35:51.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 19:35:51.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/tests/test_experimentation_manager_firebase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.689347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/docs/SweetPea.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora/experiment_runner/experimentation_manager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora/experiment_runner/experimentation_manager/firebase/
+-rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora/experiment_runner/experimentation_manager/firebase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-27 19:37:48.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-27 19:37:48.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 19:37:48.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-27 19:37:48.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 19:37:48.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:48.693347 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 19:37:36.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/tests/test_experimentation_manager_firebase.py
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/.github/workflows/python-publish.yml` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/.gitignore` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/.pre-commit-config.yaml` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/PKG-INFO` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-experimentation-manager-firebase
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: AutoRA Experimentation Manager Firebase provides functionality to manage communication of conditions and observation between AutoRA and an experiment on Firebase.
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experiment-runner-experimentation-manager-firebase
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/README.md` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/docs/SweetPea.ipynb` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/docs/SweetPea.ipynb`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/mkdocs/base.yml` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/pyproject.toml` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/src/autora/experiment_runner/experimentation_manager/firebase/__init__.py` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora/experiment_runner/experimentation_manager/firebase/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-experimentation-manager-firebase
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: AutoRA Experimentation Manager Firebase provides functionality to manage communication of conditions and observation between AutoRA and an experiment on Firebase.
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experiment-runner-experimentation-manager-firebase
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a3/tests/README.md` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a4/tests/README.md`

 * *Files identical despite different names*

