# Comparing `tmp/sorcerun-0.2.2.tar.gz` & `tmp/sorcerun-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorcerun-0.2.2.tar", last modified: Wed May 10 21:19:48 2023, max compression
+gzip compressed data, was "sorcerun-0.2.3.tar", last modified: Fri May 26 23:48:11 2023, max compression
```

## Comparing `sorcerun-0.2.2.tar` & `sorcerun-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:19:48.158432 sorcerun-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-10 21:19:32.000000 sorcerun-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-10 21:19:48.158432 sorcerun-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-10 21:19:32.000000 sorcerun-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 21:19:48.158432 sorcerun-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-10 21:19:32.000000 sorcerun-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:19:48.158432 sorcerun-0.2.2/sorcerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-10 21:19:48.000000 sorcerun-0.2.2/sorcerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-10 21:19:48.000000 sorcerun-0.2.2/sorcerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 21:19:48.000000 sorcerun-0.2.2/sorcerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 21:19:48.000000 sorcerun-0.2.2/sorcerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-10 21:19:48.000000 sorcerun-0.2.2/sorcerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 21:19:48.000000 sorcerun-0.2.2/sorcerun.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:19:48.158432 sorcerun-0.2.2/sorcerun_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:19:32.000000 sorcerun-0.2.2/sorcerun_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-10 21:19:32.000000 sorcerun-0.2.2/sorcerun_package/auth_mongodb_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-10 21:19:32.000000 sorcerun-0.2.2/sorcerun_package/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 21:19:32.000000 sorcerun-0.2.2/sorcerun_package/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-10 21:19:32.000000 sorcerun-0.2.2/sorcerun_package/mongodb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-10 21:19:32.000000 sorcerun-0.2.2/sorcerun_package/sacred_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:48:11.979192 sorcerun-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-26 23:47:58.000000 sorcerun-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-26 23:48:11.979192 sorcerun-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-26 23:47:58.000000 sorcerun-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 23:48:11.979192 sorcerun-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-26 23:47:58.000000 sorcerun-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:48:11.979192 sorcerun-0.2.3/sorcerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-26 23:48:11.000000 sorcerun-0.2.3/sorcerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-26 23:48:11.000000 sorcerun-0.2.3/sorcerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 23:48:11.000000 sorcerun-0.2.3/sorcerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-26 23:48:11.000000 sorcerun-0.2.3/sorcerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-26 23:48:11.000000 sorcerun-0.2.3/sorcerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 23:48:11.000000 sorcerun-0.2.3/sorcerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:48:11.979192 sorcerun-0.2.3/sorcerun_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 23:47:58.000000 sorcerun-0.2.3/sorcerun_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-26 23:47:58.000000 sorcerun-0.2.3/sorcerun_package/auth_mongodb_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-05-26 23:47:58.000000 sorcerun-0.2.3/sorcerun_package/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-26 23:47:58.000000 sorcerun-0.2.3/sorcerun_package/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-26 23:47:58.000000 sorcerun-0.2.3/sorcerun_package/mongodb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-26 23:47:58.000000 sorcerun-0.2.3/sorcerun_package/sacred_utils.py
```

### Comparing `sorcerun-0.2.2/LICENSE` & `sorcerun-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.2/PKG-INFO` & `sorcerun-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.2.2
+Version: 0.2.3
 License-File: LICENSE
 
 Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.
```

### Comparing `sorcerun-0.2.2/README.md` & `sorcerun-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.2/setup.py` & `sorcerun-0.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sorcerun",
-    version="0.2.2",
+    version="0.2.3",
     packages=find_packages(),
     install_requires=[
         "click",
         # "sacred @ git+https://github.com/rajatvd/sacred.git",
         "sacred==0.8.4",
         "pymongo",
         "pyyaml",
+        "scikit-learn",
     ],
     entry_points="""
         [console_scripts]
         sorcerun=sorcerun_package.cli:sorcerun
     """,
     long_description="Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.",
 )
```

### Comparing `sorcerun-0.2.2/sorcerun.egg-info/PKG-INFO` & `sorcerun-0.2.3/sorcerun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.2.2
+Version: 0.2.3
 License-File: LICENSE
 
 Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.
```

### Comparing `sorcerun-0.2.2/sorcerun_package/auth_mongodb_option.py` & `sorcerun-0.2.3/sorcerun_package/auth_mongodb_option.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.2/sorcerun_package/mongodb_utils.py` & `sorcerun-0.2.3/sorcerun_package/mongodb_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,21 +11,55 @@
 def mongodb_server(conf_path):
     click.echo(f"Starting MongoD server using config at {conf_path}")
     mongodb_process = subprocess.Popen(
         ["mongod", "--config", conf_path],
         stdout=subprocess.DEVNULL,  # Suppress output
     )
 
+    # read from log file using tail and then clean it up using jq
+    with open(conf_path, "r") as conf_file:
+        conf = yaml.load(conf_file.read(), Loader=yaml.Loader)
+        log_path = conf["systemLog"]["path"]
+
+    # Failed attempt at reading important stuff from logs and printing on a line
+
+    # separator = ", "
+    # jq_command = (
+    #     "["
+    #     + separator.join(
+    #         [
+    #             '.t."$date"',
+    #             r".s",
+    #             r".c",
+    #             r".id",
+    #             r".ctx",
+    #             r".msg",
+    #             r".attr.mechanism",
+    #             r".attr.principalName",
+    #             r".attr.remote",
+    #         ]
+    #     )
+    #     + "]"
+    # )
+
+    jq_command = "."
+    taillog_process = subprocess.Popen(
+        f"tail -f {log_path} | jq '{jq_command}'",
+        shell=True,
+    )
     try:
         yield
     finally:
         click.echo(f"Terimnating MongoD server that used config at {conf_path}\n")
         mongodb_process.terminate()
         mongodb_process.wait()
 
+        taillog_process.terminate()
+        taillog_process.wait()
+
 
 def create_mongod_conf(db_path, conf_path, auth=True):
     conf_data = {
         "storage": {
             "dbPath": db_path,
         },
         "net": {
```

### Comparing `sorcerun-0.2.2/sorcerun_package/sacred_utils.py` & `sorcerun-0.2.3/sorcerun_package/sacred_utils.py`

 * *Files identical despite different names*

