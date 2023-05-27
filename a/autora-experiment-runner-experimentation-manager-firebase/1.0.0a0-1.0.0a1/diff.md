# Comparing `tmp/autora-experiment-runner-experimentation-manager-firebase-1.0.0a0.tar.gz` & `tmp/autora-experiment-runner-experimentation-manager-firebase-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experiment-runner-experimentation-manager-firebase-1.0.0a0.tar", last modified: Mon May  8 18:40:34 2023, max compression
+gzip compressed data, was "autora-experiment-runner-experimentation-manager-firebase-1.0.0a1.tar", last modified: Sat May 27 17:00:54 2023, max compression
```

## Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a0.tar` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:40:34.548984 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:40:34.536984 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:40:34.540984 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-08 18:40:20.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-08 18:40:20.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-08 18:40:20.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-08 18:40:34.548984 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-08 18:40:20.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:40:34.540984 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-08 18:40:20.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:40:34.544984 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-08 18:40:20.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-08 18:40:20.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/docs/quick-start.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:40:34.544984 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-08 18:40:20.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-08 18:40:20.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-08 18:40:20.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 18:40:34.548984 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:40:34.536984 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:40:34.536984 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:40:34.536984 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:40:34.536984 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/src/autora/experiment_runner/experimentation_manager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:40:34.544984 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/src/autora/experiment_runner/experimentation_manager/firebase/
--rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-05-08 18:40:20.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/src/autora/experiment_runner/experimentation_manager/firebase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:40:34.544984 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-08 18:40:34.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-08 18:40:34.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:40:34.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-08 18:40:34.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 18:40:34.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:40:34.548984 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-08 18:40:20.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:40:20.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 18:40:20.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/tests/test_experimentation_manager_firebase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 17:00:54.597297 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 17:00:54.593297 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 17:00:54.593297 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-27 17:00:42.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-27 17:00:42.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-27 17:00:42.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-27 17:00:54.597297 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-27 17:00:42.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 17:00:54.593297 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-27 17:00:42.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/docs/SweetPea.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-27 17:00:42.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 17:00:54.593297 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-27 17:00:42.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-27 17:00:42.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 17:00:54.593297 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-27 17:00:42.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-27 17:00:42.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-27 17:00:42.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 17:00:54.597297 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 17:00:54.593297 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 17:00:54.593297 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 17:00:54.593297 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 17:00:54.593297 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/src/autora/experiment_runner/experimentation_manager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 17:00:54.593297 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/src/autora/experiment_runner/experimentation_manager/firebase/
+-rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-05-27 17:00:42.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/src/autora/experiment_runner/experimentation_manager/firebase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 17:00:54.593297 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-27 17:00:54.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-27 17:00:54.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 17:00:54.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 17:00:54.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 17:00:54.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 17:00:54.597297 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-27 17:00:42.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 17:00:42.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 17:00:42.000000 autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/tests/test_experimentation_manager_firebase.py
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/.github/workflows/python-publish.yml` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/.gitignore` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/.pre-commit-config.yaml` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/PKG-INFO` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-experimentation-manager-firebase
-Version: 1.0.0a0
+Version: 1.0.0a1
 Summary: AutoRA Experimentation Manager Firebase provides functionality to manage communication of conditions and observation between AutoRA and an experiment on Firebase.
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experiment-runner-experimentation-manager-firebase
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
-# Firebase Experimentation Manager
+# AutoRA Firebase Experimentation Manager
 
 Firebase Experimentation Manager provides functionality to manage communication of conditions and observation between AutoRA and an experiment on Firebase.
 
 # Quickstart Guide
 
 You will need:
 `python` >=3.8,<4: [https://www.python.org/downloads/](https://www.python.org/downloads/)
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/README.md` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Firebase Experimentation Manager
+# AutoRA Firebase Experimentation Manager
 
 Firebase Experimentation Manager provides functionality to manage communication of conditions and observation between AutoRA and an experiment on Firebase.
 
 # Quickstart Guide
 
 You will need:
 `python` >=3.8,<4: [https://www.python.org/downloads/](https://www.python.org/downloads/)
@@ -19,8 +19,8 @@
 ```shell
 python -c "from autora.experiment_runner.experimentation_manager.firebase import send_conditions"
 ```
 
 
 ## Dependencies
 
-autora-core, firebase_admin
+autora-core, firebase_admin
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/mkdocs/base.yml` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/pyproject.toml` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.8,<4"
 
 # ADD NEW DEPENDENCIES HERE
 dependencies = [
     "autora-core",
-    "firebase_admin",
+    "firebase-admin",
 ]
 
 [project.optional-dependencies]
 dev = [
     "autora-core[dev]"
 ]
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-experimentation-manager-firebase
-Version: 1.0.0a0
+Version: 1.0.0a1
 Summary: AutoRA Experimentation Manager Firebase provides functionality to manage communication of conditions and observation between AutoRA and an experiment on Firebase.
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experiment-runner-experimentation-manager-firebase
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
-# Firebase Experimentation Manager
+# AutoRA Firebase Experimentation Manager
 
 Firebase Experimentation Manager provides functionality to manage communication of conditions and observation between AutoRA and an experiment on Firebase.
 
 # Quickstart Guide
 
 You will need:
 `python` >=3.8,<4: [https://www.python.org/downloads/](https://www.python.org/downloads/)
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 .gitignore
 .pre-commit-config.yaml
 README.md
 mkdocs.yml
 pyproject.toml
 .github/workflows/python-publish.yml
+docs/SweetPea.ipynb
 docs/index.md
-docs/quick-start.md
+docs/quickstart.md
 docs/javascripts/mathjax.js
 mkdocs/base.yml
 src/autora/experiment_runner/experimentation_manager/firebase/__init__.py
 src/autora_experiment_runner_experimentation_manager_firebase.egg-info/PKG-INFO
 src/autora_experiment_runner_experimentation_manager_firebase.egg-info/SOURCES.txt
 src/autora_experiment_runner_experimentation_manager_firebase.egg-info/dependency_links.txt
 src/autora_experiment_runner_experimentation_manager_firebase.egg-info/requires.txt
```

### Comparing `autora-experiment-runner-experimentation-manager-firebase-1.0.0a0/tests/README.md` & `autora-experiment-runner-experimentation-manager-firebase-1.0.0a1/tests/README.md`

 * *Files identical despite different names*

