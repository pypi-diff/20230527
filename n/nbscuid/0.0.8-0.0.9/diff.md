# Comparing `tmp/nbscuid-0.0.8.tar.gz` & `tmp/nbscuid-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbscuid-0.0.8.tar", last modified: Thu May 25 22:57:55 2023, max compression
+gzip compressed data, was "nbscuid-0.0.9.tar", last modified: Fri May 26 22:17:12 2023, max compression
```

## Comparing `nbscuid-0.0.8.tar` & `nbscuid-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-25 22:57:55.711661 nbscuid-0.0.8/
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      332 2023-05-03 23:21:30.000000 nbscuid-0.0.8/.gitignore
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      715 2023-05-04 22:27:17.000000 nbscuid-0.0.8/.readthedocs.yml
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     1073 2023-02-24 23:26:03.000000 nbscuid-0.0.8/LICENSE
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     3205 2023-05-25 22:57:55.710971 nbscuid-0.0.8/PKG-INFO
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     1495 2023-05-18 15:54:26.000000 nbscuid-0.0.8/README.md
-drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-25 22:57:55.585642 nbscuid-0.0.8/docs/
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      638 2023-05-03 20:38:18.000000 nbscuid-0.0.8/docs/Makefile
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      804 2023-05-03 20:38:18.000000 nbscuid-0.0.8/docs/make.bat
--rw-r--r--   0 eromashkova (38594) ncar      (1000)       32 2023-05-04 22:11:40.000000 nbscuid-0.0.8/docs/requirements.txt
-drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-25 22:57:55.590756 nbscuid-0.0.8/docs/source/
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     1915 2023-05-04 15:24:38.000000 nbscuid-0.0.8/docs/source/conf.py
--rw-r--r--   0 eromashkova (38594) ncar      (1000)       35 2023-05-17 16:40:58.000000 nbscuid-0.0.8/docs/source/gettingstarted.md
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      497 2023-05-17 15:13:04.000000 nbscuid-0.0.8/docs/source/index.rst
--rw-r--r--   0 eromashkova (38594) ncar      (1000)       58 2023-05-03 20:44:35.000000 nbscuid-0.0.8/docs/source/modules.rst
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      795 2023-05-03 20:44:35.000000 nbscuid-0.0.8/docs/source/nbscuid.rst
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     1320 2023-05-25 22:52:39.000000 nbscuid-0.0.8/docs/source/tutorialsetup.md
-drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-25 22:57:55.598086 nbscuid-0.0.8/nbscuid/
--rw-r--r--   0 eromashkova (38594) ncar      (1000)        0 2023-02-24 23:33:45.000000 nbscuid-0.0.8/nbscuid/__init__.py
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     1671 2023-05-16 17:45:54.000000 nbscuid-0.0.8/nbscuid/_jupyter-book-config-defaults.yml
--rwxr-xr-x   0 eromashkova (38594) ncar      (1000)     1053 2023-04-24 23:15:21.000000 nbscuid-0.0.8/nbscuid/build.py
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     7640 2023-02-24 23:27:28.000000 nbscuid-0.0.8/nbscuid/cache.py
--rw-r--r--   0 eromashkova (38594) ncar      (1000)        0 2023-05-04 07:46:51.000000 nbscuid-0.0.8/nbscuid/quickstart.py
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     1048 2023-03-08 00:11:40.000000 nbscuid-0.0.8/nbscuid/read.py
--rwxr-xr-x   0 eromashkova (38594) ncar      (1000)     8247 2023-05-25 20:08:44.000000 nbscuid-0.0.8/nbscuid/run.py
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     9642 2023-05-25 22:23:26.000000 nbscuid-0.0.8/nbscuid/util.py
-drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-25 22:57:55.603561 nbscuid-0.0.8/nbscuid.egg-info/
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     3205 2023-05-25 22:57:55.599283 nbscuid-0.0.8/nbscuid.egg-info/PKG-INFO
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      612 2023-05-25 22:57:55.600060 nbscuid-0.0.8/nbscuid.egg-info/SOURCES.txt
--rw-r--r--   0 eromashkova (38594) ncar      (1000)        1 2023-05-25 22:57:55.601259 nbscuid-0.0.8/nbscuid.egg-info/dependency_links.txt
--rw-r--r--   0 eromashkova (38594) ncar      (1000)       84 2023-05-25 22:57:55.602151 nbscuid-0.0.8/nbscuid.egg-info/entry_points.txt
--rw-r--r--   0 eromashkova (38594) ncar      (1000)       94 2023-05-25 22:57:55.602830 nbscuid-0.0.8/nbscuid.egg-info/requires.txt
--rw-r--r--   0 eromashkova (38594) ncar      (1000)        8 2023-05-25 22:57:55.603658 nbscuid-0.0.8/nbscuid.egg-info/top_level.txt
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      939 2023-05-25 22:56:29.000000 nbscuid-0.0.8/pyproject.toml
--rw-r--r--   0 eromashkova (38594) ncar      (1000)       38 2023-05-25 22:57:55.711800 nbscuid-0.0.8/setup.cfg
+drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-26 22:17:12.204862 nbscuid-0.0.9/
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      332 2023-05-26 07:45:42.000000 nbscuid-0.0.9/.gitignore
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      715 2023-05-26 07:45:42.000000 nbscuid-0.0.9/.readthedocs.yml
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     1073 2023-05-26 07:45:42.000000 nbscuid-0.0.9/LICENSE
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     3285 2023-05-26 22:17:12.204510 nbscuid-0.0.9/PKG-INFO
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     1575 2023-05-26 22:11:19.000000 nbscuid-0.0.9/README.md
+drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-26 22:17:12.190527 nbscuid-0.0.9/docs/
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      638 2023-05-26 07:45:42.000000 nbscuid-0.0.9/docs/Makefile
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      804 2023-05-26 07:45:42.000000 nbscuid-0.0.9/docs/make.bat
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)       32 2023-05-26 07:45:42.000000 nbscuid-0.0.9/docs/requirements.txt
+drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-26 22:17:12.195631 nbscuid-0.0.9/docs/source/
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     1946 2023-05-26 22:11:19.000000 nbscuid-0.0.9/docs/source/conf.py
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)       35 2023-05-26 07:45:42.000000 nbscuid-0.0.9/docs/source/gettingstarted.md
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      497 2023-05-26 07:45:42.000000 nbscuid-0.0.9/docs/source/index.rst
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)       58 2023-05-26 07:45:42.000000 nbscuid-0.0.9/docs/source/modules.rst
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      795 2023-05-26 07:45:42.000000 nbscuid-0.0.9/docs/source/nbscuid.rst
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)   109740 2023-05-26 22:11:19.000000 nbscuid-0.0.9/docs/source/nbscuid_logo.png
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     1320 2023-05-26 07:45:42.000000 nbscuid-0.0.9/docs/source/tutorialsetup.md
+drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-26 22:17:12.200587 nbscuid-0.0.9/nbscuid/
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)        0 2023-05-26 07:45:42.000000 nbscuid-0.0.9/nbscuid/__init__.py
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     1671 2023-05-26 07:45:42.000000 nbscuid-0.0.9/nbscuid/_jupyter-book-config-defaults.yml
+-rwxr-xr-x   0 eromashkova (38594) ncar      (1000)     1038 2023-05-26 22:11:19.000000 nbscuid-0.0.9/nbscuid/build.py
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     7640 2023-05-26 07:45:42.000000 nbscuid-0.0.9/nbscuid/cache.py
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)        0 2023-05-26 07:45:42.000000 nbscuid-0.0.9/nbscuid/quickstart.py
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     1048 2023-05-26 07:45:42.000000 nbscuid-0.0.9/nbscuid/read.py
+-rwxr-xr-x   0 eromashkova (38594) ncar      (1000)     8397 2023-05-26 22:11:19.000000 nbscuid-0.0.9/nbscuid/run.py
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     9661 2023-05-26 22:11:19.000000 nbscuid-0.0.9/nbscuid/util.py
+drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-26 22:17:12.203822 nbscuid-0.0.9/nbscuid.egg-info/
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     3285 2023-05-26 22:17:12.201285 nbscuid-0.0.9/nbscuid.egg-info/PKG-INFO
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      641 2023-05-26 22:17:12.201971 nbscuid-0.0.9/nbscuid.egg-info/SOURCES.txt
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)        1 2023-05-26 22:17:12.202406 nbscuid-0.0.9/nbscuid.egg-info/dependency_links.txt
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)       84 2023-05-26 22:17:12.202970 nbscuid-0.0.9/nbscuid.egg-info/entry_points.txt
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)       94 2023-05-26 22:17:12.203490 nbscuid-0.0.9/nbscuid.egg-info/requires.txt
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)        8 2023-05-26 22:17:12.203936 nbscuid-0.0.9/nbscuid.egg-info/top_level.txt
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      939 2023-05-26 22:11:19.000000 nbscuid-0.0.9/pyproject.toml
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)       38 2023-05-26 22:17:12.204993 nbscuid-0.0.9/setup.cfg
```

### Comparing `nbscuid-0.0.8/.readthedocs.yml` & `nbscuid-0.0.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.8/LICENSE` & `nbscuid-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.8/PKG-INFO` & `nbscuid-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbscuid
-Version: 0.0.8
+Version: 0.0.9
 Summary: Notebook-Based, Super CUstomizable Infrastructure for Diagnostics
 Author-email: Elena Romashkova <eromashkova@ucar.edu>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -27,17 +27,19 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nbscuid 🦑
-
 ### Notebook-Based, Super CUstomizable Infrastructure for Diagnostics
 
+<img title="logo" alt="logo" src="docs/source/nbscuid_logo.png" width = 400px>
+
+
 This is a package to enable running notebook-based diagnostic workflows. Based on my-cesm-experiment by matt-long: https://github.com/matt-long/my-cesm-experiment. 
 
 See some examples of workflows at https://github.com/rmshkv/nbscuid-examples. For a basic tutorial, follow https://nbscuid.readthedocs.io/en/latest/tutorialsetup.html.
 
 ## Capabilities
 
 - Integration with data catalogs
```

### Comparing `nbscuid-0.0.8/README.md` & `nbscuid-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # nbscuid 🦑
-
 ### Notebook-Based, Super CUstomizable Infrastructure for Diagnostics
 
+<img title="logo" alt="logo" src="docs/source/nbscuid_logo.png" width = 400px>
+
+
 This is a package to enable running notebook-based diagnostic workflows. Based on my-cesm-experiment by matt-long: https://github.com/matt-long/my-cesm-experiment. 
 
 See some examples of workflows at https://github.com/rmshkv/nbscuid-examples. For a basic tutorial, follow https://nbscuid.readthedocs.io/en/latest/tutorialsetup.html.
 
 ## Capabilities
 
 - Integration with data catalogs
```

### Comparing `nbscuid-0.0.8/docs/Makefile` & `nbscuid-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.8/docs/make.bat` & `nbscuid-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.8/docs/source/conf.py` & `nbscuid-0.0.9/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,9 +48,10 @@
 #
 html_theme = "furo"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
+html_logo = 'nbscuid_logo.png'
 
 autoclass_content = 'both'
```

### Comparing `nbscuid-0.0.8/docs/source/nbscuid.rst` & `nbscuid-0.0.9/docs/source/nbscuid.rst`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.8/docs/source/tutorialsetup.md` & `nbscuid-0.0.9/docs/source/tutorialsetup.md`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.8/nbscuid/_jupyter-book-config-defaults.yml` & `nbscuid-0.0.9/nbscuid/_jupyter-book-config-defaults.yml`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.8/nbscuid/build.py` & `nbscuid-0.0.9/nbscuid/build.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 def build():
     
     config_path = str(sys.argv[1])
     
     with open(config_path, "r") as fid:
         control = yaml.safe_load(fid)
     
-    casename = control["data_sources"]["casename"]
+    sname = control["data_sources"]["sname"]
     run_dir = control["data_sources"]["run_dir"]
 
-    subprocess.run(["jupyter-book", "clean" , f"{run_dir}/computed_notebooks/{casename}"])
-    subprocess.run(["jupyter-book",  "build" , f"{run_dir}/computed_notebooks/{casename}",  "--all"])
+    subprocess.run(["jupyter-book", "clean" , f"{run_dir}/computed_notebooks/{sname}"])
+    subprocess.run(["jupyter-book",  "build" , f"{run_dir}/computed_notebooks/{sname}",  "--all"])
                    
 #     if 'publish_location' in control:
         
 #         user = os.environ.get('USER')
 #         remote_mach = control["publish_location"]["remote_mach"]
 #         remote_dir = control["publish_location"]["remote_dir"]
 # this seems more complicated than expected...people have mentioned paramiko library?
         # subprocess.run(["mkdir", "-p", remote_dir])
-        # subprocess.run(["scp", "-r", f"{run_dir}/computed_notebooks/{casename}/_build/html/*", f"{user}@{remote_mach}:{remote_dir}"])
+        # subprocess.run(["scp", "-r", f"{run_dir}/computed_notebooks/{sname}/_build/html/*", f"{user}@{remote_mach}:{remote_dir}"])
         
     return None
```

### Comparing `nbscuid-0.0.8/nbscuid/cache.py` & `nbscuid-0.0.9/nbscuid/cache.py`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.8/nbscuid/read.py` & `nbscuid-0.0.9/nbscuid/read.py`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.8/nbscuid/run.py` & `nbscuid-0.0.9/nbscuid/run.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 def run():
     
     # Get control structure
     config_path = str(sys.argv[1])
     control = nbscuid.util.get_control_dict(config_path)    
     nbscuid.util.setup_book(config_path)
         
-    if control['use_cluster']:    
+    if control['computation_config']['use_cluster']:    
         # Cluster management 
         # Notebooks are configured to connect to this cluster    
-        cluster = nbscuid.util.get_Cluster(account=control['account'])
+        cluster = nbscuid.util.get_Cluster(account=control['computation_config']['account'])
         cluster.scale(4) # Should this be user modifiable?
     else:
         cluster = None
     
     # Grab paths
     
     ### This code seems repetitive, is there a better way to do this?
     run_dir = os.path.expanduser(control['data_sources']['run_dir'])
-    output_dir = run_dir + "/computed_notebooks/" + control['data_sources']['casename']
+    output_dir = run_dir + "/computed_notebooks/" + control['data_sources']['sname']
     cache_metadata_path = run_dir + "/cache_metadata_path"
     cache_data_path = run_dir + "/cache_data_path"
     temp_data_path = run_dir + "/temp_data" 
     nb_path_root = os.path.expanduser(control['data_sources']['nb_path_root'])
 
     # Access catalog if it exists
 
@@ -92,15 +92,15 @@
         if key in regular_nbs:
             regular_nbs.pop(key)
             
             
     #####################################################################
     # Pausing to wait for workers to avoid timeout error
         
-    if control['use_cluster']:
+    if control['computation_config']['use_cluster']:
         
         dask.config.set({'distributed.comm.timeouts.connect': '90s'})
 
         client = Client(cluster.scheduler_address)
 
         nworkers = 1
 
@@ -125,15 +125,15 @@
 
     ### To do: figure out how to organize the caching code better, keeping the whole block for now
     
     for nb, info in precompute_nbs.items():
     
         parameter_groups = info['parameter_groups']
         
-        use_cluster = control['use_cluster'] and info['use_cluster']
+        use_cluster = control['computation_config']['use_cluster'] and info['use_cluster']
 
         ### passing in subset kwargs if they're provided
         if 'subset' in info:
             subset_kwargs = info['subset']
         else:
             subset_kwargs = {}
 
@@ -204,28 +204,28 @@
                 # this can only properly handle one save per notebook (FIX LATER)
                 precompute_nbs[nb]["asset_path"] = asset_path
     
     # Calculating regular notebooks
     
     for nb, info in regular_nbs.items():
         
-        use_cluster = control['use_cluster'] and info['use_cluster']
+        use_cluster = control['computation_config']['use_cluster']and info['use_cluster']
         
         nbscuid.util.run_notebook(nb, info, use_cluster, cat_path, nb_path_root, output_dir, global_params, cluster=cluster)
     
     # Calculating notebooks with dependencies
     
     for nb, info in dependent_nbs.items():
         
-        use_cluster = control['use_cluster'] and info['use_cluster']
+        use_cluster = control['computation_config']['use_cluster'] and info['use_cluster']
     
         ### getting necessary asset:
         dependent_asset_path = precompute_nbs[info['dependency']]["asset_path"]
         
         nbscuid.util.run_notebook(nb, info, use_cluster, cat_path, nb_path_root, output_dir, global_params, dependent_asset_path=dependent_asset_path, cluster=cluster)
     
-    if control['use_cluster']:
+    if control['computation_config']['use_cluster']:
         # Closing cluster
         cluster.close()
     
     return None
```

### Comparing `nbscuid-0.0.8/nbscuid/util.py` & `nbscuid-0.0.9/nbscuid/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 pm.engines.papermill_engines._engines["md_jinja"] = md_jinja_engine
 
 
 def get_control_dict(config_path):
     with open(config_path, "r") as fid:
         control = yaml.safe_load(fid)
 
-    default_kernel_name = control.pop("default_kernel_name", None)
+    default_kernel_name = control["computation_config"].pop("default_kernel_name", None)
 
     if default_kernel_name is not None:
         for d in control["compute_notebooks"].values():
             if "kernel_name" not in d:
                 d["kernel_name"] = default_kernel_name
     else:
         for nb, d in control["compute_notebooks"].items():
@@ -143,15 +143,15 @@
 
     # ensure directory
     run_dir = os.path.expanduser(control['data_sources']["run_dir"])
     output_root = run_dir + "/computed_notebooks"
     
     os.makedirs(output_root, exist_ok=True)
     
-    output_dir = f'{output_root}/{control["data_sources"]["casename"]}'
+    output_dir = f'{output_root}/{control["data_sources"]["sname"]}'
     
     os.makedirs(output_dir, exist_ok=True)
     
     # create cache and temp catalog directories
     cache_metadata_path = run_dir + "/cache_metadata_path"
     cache_data_path = run_dir + "/cache_data_path"
     temp_data_path = run_dir + "/temp_data"
```

### Comparing `nbscuid-0.0.8/nbscuid.egg-info/PKG-INFO` & `nbscuid-0.0.9/nbscuid.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbscuid
-Version: 0.0.8
+Version: 0.0.9
 Summary: Notebook-Based, Super CUstomizable Infrastructure for Diagnostics
 Author-email: Elena Romashkova <eromashkova@ucar.edu>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -27,17 +27,19 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nbscuid 🦑
-
 ### Notebook-Based, Super CUstomizable Infrastructure for Diagnostics
 
+<img title="logo" alt="logo" src="docs/source/nbscuid_logo.png" width = 400px>
+
+
 This is a package to enable running notebook-based diagnostic workflows. Based on my-cesm-experiment by matt-long: https://github.com/matt-long/my-cesm-experiment. 
 
 See some examples of workflows at https://github.com/rmshkv/nbscuid-examples. For a basic tutorial, follow https://nbscuid.readthedocs.io/en/latest/tutorialsetup.html.
 
 ## Capabilities
 
 - Integration with data catalogs
```

### Comparing `nbscuid-0.0.8/nbscuid.egg-info/SOURCES.txt` & `nbscuid-0.0.9/nbscuid.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 docs/make.bat
 docs/requirements.txt
 docs/source/conf.py
 docs/source/gettingstarted.md
 docs/source/index.rst
 docs/source/modules.rst
 docs/source/nbscuid.rst
+docs/source/nbscuid_logo.png
 docs/source/tutorialsetup.md
 nbscuid/__init__.py
 nbscuid/_jupyter-book-config-defaults.yml
 nbscuid/build.py
 nbscuid/cache.py
 nbscuid/quickstart.py
 nbscuid/read.py
```

### Comparing `nbscuid-0.0.8/pyproject.toml` & `nbscuid-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools]
 packages = ["nbscuid"]
 
 
 [project]
 name = "nbscuid"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Elena Romashkova", email="eromashkova@ucar.edu" },
 ]
 description = "Notebook-Based, Super CUstomizable Infrastructure for Diagnostics"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
```

