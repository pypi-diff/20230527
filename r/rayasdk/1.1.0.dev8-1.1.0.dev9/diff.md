# Comparing `tmp/rayasdk-1.1.0.dev8.tar.gz` & `tmp/rayasdk-1.1.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rayasdk-1.1.0.dev8.tar", last modified: Wed May 24 18:48:06 2023, max compression
+gzip compressed data, was "rayasdk-1.1.0.dev9.tar", last modified: Wed May 24 19:09:25 2023, max compression
```

## Comparing `rayasdk-1.1.0.dev8.tar` & `rayasdk-1.1.0.dev9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-24 18:48:06.605626 rayasdk-1.1.0.dev8/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6569 2023-05-24 18:48:06.605626 rayasdk-1.1.0.dev8/PKG-INFO
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6219 2023-05-11 21:39:47.000000 rayasdk-1.1.0.dev8/README.md
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-24 18:48:06.605626 rayasdk-1.1.0.dev8/rayasdk/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      546 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev8/rayasdk/__init__.py
--rwxrwxr-x   0 camilo    (1000) camilo    (1000)     5077 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev8/rayasdk/__main__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     5324 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev8/rayasdk/connect.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     3381 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev8/rayasdk/constants.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-24 18:48:06.605626 rayasdk-1.1.0.dev8/rayasdk/container_handlers/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev8/rayasdk/container_handlers/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     7391 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev8/rayasdk/container_handlers/docker_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2787 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev8/rayasdk/initializer.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1439 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev8/rayasdk/killer.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     4123 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev8/rayasdk/logger.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1235 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev8/rayasdk/messages.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6664 2023-05-23 18:10:01.000000 rayasdk-1.1.0.dev8/rayasdk/runner.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     4354 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev8/rayasdk/scanner.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     5536 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev8/rayasdk/simulator.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2657 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev8/rayasdk/sshKeyGen.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-24 18:48:06.605626 rayasdk-1.1.0.dev8/rayasdk/template/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      244 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev8/rayasdk/template/__main__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      551 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev8/rayasdk/template/app.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      399 2023-04-17 17:27:42.000000 rayasdk-1.1.0.dev8/rayasdk/template/launch.json
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      108 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev8/rayasdk/template/manifest.json
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1775 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev8/rayasdk/utils.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)    11638 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev8/rayasdk/vcs.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-24 18:48:06.605626 rayasdk-1.1.0.dev8/rayasdk.egg-info/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6569 2023-05-24 18:48:06.000000 rayasdk-1.1.0.dev8/rayasdk.egg-info/PKG-INFO
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      683 2023-05-24 18:48:06.000000 rayasdk-1.1.0.dev8/rayasdk.egg-info/SOURCES.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        1 2023-05-24 18:48:06.000000 rayasdk-1.1.0.dev8/rayasdk.egg-info/dependency_links.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       51 2023-05-24 18:48:06.000000 rayasdk-1.1.0.dev8/rayasdk.egg-info/entry_points.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      103 2023-05-24 18:48:06.000000 rayasdk-1.1.0.dev8/rayasdk.egg-info/requires.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        8 2023-05-24 18:48:06.000000 rayasdk-1.1.0.dev8/rayasdk.egg-info/top_level.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       79 2023-05-24 18:48:06.605626 rayasdk-1.1.0.dev8/setup.cfg
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1101 2023-05-24 18:47:19.000000 rayasdk-1.1.0.dev8/setup.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-24 19:09:25.881965 rayasdk-1.1.0.dev9/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6569 2023-05-24 19:09:25.881965 rayasdk-1.1.0.dev9/PKG-INFO
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6219 2023-05-11 21:39:47.000000 rayasdk-1.1.0.dev9/README.md
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-24 19:09:25.877966 rayasdk-1.1.0.dev9/rayasdk/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      546 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev9/rayasdk/__init__.py
+-rwxrwxr-x   0 camilo    (1000) camilo    (1000)     5077 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev9/rayasdk/__main__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     5324 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev9/rayasdk/connect.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     3381 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev9/rayasdk/constants.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-24 19:09:25.881965 rayasdk-1.1.0.dev9/rayasdk/container_handlers/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev9/rayasdk/container_handlers/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     7391 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev9/rayasdk/container_handlers/docker_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2787 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev9/rayasdk/initializer.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1439 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev9/rayasdk/killer.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     4123 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev9/rayasdk/logger.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1235 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev9/rayasdk/messages.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6664 2023-05-23 18:10:01.000000 rayasdk-1.1.0.dev9/rayasdk/runner.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     4354 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev9/rayasdk/scanner.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     5536 2023-05-23 18:09:34.000000 rayasdk-1.1.0.dev9/rayasdk/simulator.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2657 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev9/rayasdk/sshKeyGen.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-24 19:09:25.881965 rayasdk-1.1.0.dev9/rayasdk/template/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      244 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev9/rayasdk/template/__main__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      551 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev9/rayasdk/template/app.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      399 2023-04-17 17:27:42.000000 rayasdk-1.1.0.dev9/rayasdk/template/launch.json
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      108 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev9/rayasdk/template/manifest.json
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1775 2023-05-18 19:48:04.000000 rayasdk-1.1.0.dev9/rayasdk/utils.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)    11619 2023-05-24 19:08:37.000000 rayasdk-1.1.0.dev9/rayasdk/vcs.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-24 19:09:25.881965 rayasdk-1.1.0.dev9/rayasdk.egg-info/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6569 2023-05-24 19:09:25.000000 rayasdk-1.1.0.dev9/rayasdk.egg-info/PKG-INFO
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      683 2023-05-24 19:09:25.000000 rayasdk-1.1.0.dev9/rayasdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        1 2023-05-24 19:09:25.000000 rayasdk-1.1.0.dev9/rayasdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       51 2023-05-24 19:09:25.000000 rayasdk-1.1.0.dev9/rayasdk.egg-info/entry_points.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      103 2023-05-24 19:09:25.000000 rayasdk-1.1.0.dev9/rayasdk.egg-info/requires.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        8 2023-05-24 19:09:25.000000 rayasdk-1.1.0.dev9/rayasdk.egg-info/top_level.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       79 2023-05-24 19:09:25.881965 rayasdk-1.1.0.dev9/setup.cfg
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1101 2023-05-24 19:09:01.000000 rayasdk-1.1.0.dev9/setup.py
```

### Comparing `rayasdk-1.1.0.dev8/PKG-INFO` & `rayasdk-1.1.0.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayasdk
-Version: 1.1.0.dev8
+Version: 1.1.0.dev9
 Summary: Raya SDK - Unlimited Robotics Software Development Kit
 Home-page: UNKNOWN
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: MIT
 Keywords: robotics,unlimited-robotics,gary
 Platform: UNKNOWN
```

### Comparing `rayasdk-1.1.0.dev8/README.md` & `rayasdk-1.1.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev8/rayasdk/__init__.py` & `rayasdk-1.1.0.dev9/rayasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev8/rayasdk/__main__.py` & `rayasdk-1.1.0.dev9/rayasdk/__main__.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev8/rayasdk/connect.py` & `rayasdk-1.1.0.dev9/rayasdk/connect.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev8/rayasdk/constants.py` & `rayasdk-1.1.0.dev9/rayasdk/constants.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev8/rayasdk/container_handlers/docker_handler.py` & `rayasdk-1.1.0.dev9/rayasdk/container_handlers/docker_handler.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev8/rayasdk/initializer.py` & `rayasdk-1.1.0.dev9/rayasdk/initializer.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev8/rayasdk/killer.py` & `rayasdk-1.1.0.dev9/rayasdk/killer.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev8/rayasdk/logger.py` & `rayasdk-1.1.0.dev9/rayasdk/logger.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev8/rayasdk/messages.py` & `rayasdk-1.1.0.dev9/rayasdk/messages.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev8/rayasdk/runner.py` & `rayasdk-1.1.0.dev9/rayasdk/runner.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev8/rayasdk/scanner.py` & `rayasdk-1.1.0.dev9/rayasdk/scanner.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev8/rayasdk/simulator.py` & `rayasdk-1.1.0.dev9/rayasdk/simulator.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev8/rayasdk/sshKeyGen.py` & `rayasdk-1.1.0.dev9/rayasdk/sshKeyGen.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev8/rayasdk/template/app.py` & `rayasdk-1.1.0.dev9/rayasdk/template/app.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev8/rayasdk/utils.py` & `rayasdk-1.1.0.dev9/rayasdk/utils.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev8/rayasdk/vcs.py` & `rayasdk-1.1.0.dev9/rayasdk/vcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,16 +227,16 @@
 
     def patch_updated(self, component=None, show_msg= True):
         '''Function to check if the latest version is a patch'''
         if component:
             local = self.__local_version(component)
             latest = self.__get_latest_version(component)
             same_major = self.__get_major(latest) == self.__get_major(local)
-            same_minor = self.__get_minor(latest) == self.__get_minor(local)
             diff_patch = self.__get_patch(local) < self.__get_patch(latest)
+            same_minor = self.__get_minor(latest) == self.__get_minor(local)
             if same_major and same_minor and diff_patch:
                 if show_msg:
                     log_warning(
                         (f'{component} have an patch update it is going to be'
                         f' updated to version \'{latest}\', '
                         f'current \'{local}\''))
                 return False
@@ -274,15 +274,15 @@
         return False
 
 
     def get_latest_version(self, component):
         return self.__get_latest_version(component=component)
     
     
-    def get_VCS_json(self, type_version: str = 'latest', component: str = None) -> ( list | None ):
+    def get_VCS_json(self, type_version: str = 'latest', component: str = None):
         try:
             response = requests.request("GET", constants.VCS_URL)
             return response.json()
         except requests.exceptions.ConnectionError as e:
             raise e
         except Exception as e:
             log_error(e)
```

### Comparing `rayasdk-1.1.0.dev8/rayasdk.egg-info/PKG-INFO` & `rayasdk-1.1.0.dev9/rayasdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayasdk
-Version: 1.1.0.dev8
+Version: 1.1.0.dev9
 Summary: Raya SDK - Unlimited Robotics Software Development Kit
 Home-page: UNKNOWN
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: MIT
 Keywords: robotics,unlimited-robotics,gary
 Platform: UNKNOWN
```

### Comparing `rayasdk-1.1.0.dev8/rayasdk.egg-info/SOURCES.txt` & `rayasdk-1.1.0.dev9/rayasdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev8/setup.py` & `rayasdk-1.1.0.dev9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from pip_tools import get_last_release_version, get_last_prerelease_version
 
-VERSION = '1.1.0.dev8'
+VERSION = '1.1.0.dev9'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='rayasdk',
     packages=find_packages(),
```

