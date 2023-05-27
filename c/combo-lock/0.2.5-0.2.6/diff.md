# Comparing `tmp/combo_lock-0.2.5.tar.gz` & `tmp/combo_lock-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combo_lock-0.2.5.tar", last modified: Tue Mar 21 05:29:58 2023, max compression
+gzip compressed data, was "combo_lock-0.2.6.tar", last modified: Sat May 27 14:30:59 2023, max compression
```

## Comparing `combo_lock-0.2.5.tar` & `combo_lock-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 05:29:58.360096 combo_lock-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-03-21 05:29:47.000000 combo_lock-0.2.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-21 05:29:47.000000 combo_lock-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-21 05:29:58.360096 combo_lock-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-21 05:29:47.000000 combo_lock-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 05:29:58.360096 combo_lock-0.2.5/combo_lock/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-21 05:29:47.000000 combo_lock-0.2.5/combo_lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-03-21 05:29:47.000000 combo_lock-0.2.5/combo_lock/combo_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-21 05:29:47.000000 combo_lock-0.2.5/combo_lock/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 05:29:58.360096 combo_lock-0.2.5/combo_lock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-21 05:29:58.000000 combo_lock-0.2.5/combo_lock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-21 05:29:58.000000 combo_lock-0.2.5/combo_lock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 05:29:58.000000 combo_lock-0.2.5/combo_lock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-21 05:29:58.000000 combo_lock-0.2.5/combo_lock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-21 05:29:58.000000 combo_lock-0.2.5/combo_lock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-21 05:29:47.000000 combo_lock-0.2.5/requirements-old.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-21 05:29:47.000000 combo_lock-0.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 05:29:58.360096 combo_lock-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-03-21 05:29:47.000000 combo_lock-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 14:30:59.789260 combo_lock-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-05-27 14:30:55.000000 combo_lock-0.2.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-27 14:30:55.000000 combo_lock-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-27 14:30:59.789260 combo_lock-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-27 14:30:55.000000 combo_lock-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 14:30:59.785260 combo_lock-0.2.6/combo_lock/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-27 14:30:55.000000 combo_lock-0.2.6/combo_lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-27 14:30:55.000000 combo_lock-0.2.6/combo_lock/combo_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-27 14:30:55.000000 combo_lock-0.2.6/combo_lock/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 14:30:59.789260 combo_lock-0.2.6/combo_lock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-27 14:30:59.000000 combo_lock-0.2.6/combo_lock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-27 14:30:59.000000 combo_lock-0.2.6/combo_lock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 14:30:59.000000 combo_lock-0.2.6/combo_lock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-27 14:30:59.000000 combo_lock-0.2.6/combo_lock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-27 14:30:59.000000 combo_lock-0.2.6/combo_lock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-27 14:30:55.000000 combo_lock-0.2.6/requirements-old.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-27 14:30:55.000000 combo_lock-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 14:30:59.789260 combo_lock-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-27 14:30:55.000000 combo_lock-0.2.6/setup.py
```

### Comparing `combo_lock-0.2.5/LICENSE.md` & `combo_lock-0.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `combo_lock-0.2.5/PKG-INFO` & `combo_lock-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combo_lock
-Version: 0.2.5
+Version: 0.2.6
 Summary: A combined process and thread lock
 Home-page: https://github.com/forslund/combo-lock
 Author: Åke Forslund, JarbasAI
 Author-email: ake.forslund@gmail.com, jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `combo_lock-0.2.5/README.md` & `combo_lock-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `combo_lock-0.2.5/combo_lock/combo_lock.py` & `combo_lock-0.2.6/combo_lock/combo_lock.py`

 * *Files identical despite different names*

### Comparing `combo_lock-0.2.5/combo_lock.egg-info/PKG-INFO` & `combo_lock-0.2.6/combo_lock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combo-lock
-Version: 0.2.5
+Version: 0.2.6
 Summary: A combined process and thread lock
 Home-page: https://github.com/forslund/combo-lock
 Author: Åke Forslund, JarbasAI
 Author-email: ake.forslund@gmail.com, jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `combo_lock-0.2.5/setup.py` & `combo_lock-0.2.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         return load_requirements("requirements.txt")
     else:
         return load_requirements("requirements-old.txt")
 
 
 setup(
     name='combo_lock',
-    version='0.2.5',
+    version='0.2.6',
     packages=['combo_lock'],
     package_data={
       '*': ['*.txt', '*.md']
     },
     include_package_data=True,
     install_requires=required(),
     url='https://github.com/forslund/combo-lock',
```

