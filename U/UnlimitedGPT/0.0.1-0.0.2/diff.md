# Comparing `tmp/UnlimitedGPT-0.0.1.tar.gz` & `tmp/UnlimitedGPT-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnlimitedGPT-0.0.1.tar", last modified: Sat May 27 10:42:55 2023, max compression
+gzip compressed data, was "UnlimitedGPT-0.0.2.tar", last modified: Sat May 27 11:00:42 2023, max compression
```

## Comparing `UnlimitedGPT-0.0.1.tar` & `UnlimitedGPT-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 10:42:55.331952 UnlimitedGPT-0.0.1/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    35149 2023-05-26 09:35:45.000000 UnlimitedGPT-0.0.1/LICENSE
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1160 2023-05-27 10:42:55.327952 UnlimitedGPT-0.0.1/PKG-INFO
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       67 2023-05-26 09:35:45.000000 UnlimitedGPT-0.0.1/README.md
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 10:42:55.327952 UnlimitedGPT-0.0.1/UnlimitedGPT.egg-info/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1160 2023-05-27 10:42:55.000000 UnlimitedGPT-0.0.1/UnlimitedGPT.egg-info/PKG-INFO
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      377 2023-05-27 10:42:55.000000 UnlimitedGPT-0.0.1/UnlimitedGPT.egg-info/SOURCES.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-05-27 10:42:55.000000 UnlimitedGPT-0.0.1/UnlimitedGPT.egg-info/dependency_links.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-05-27 10:42:55.000000 UnlimitedGPT-0.0.1/UnlimitedGPT.egg-info/requires.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       44 2023-05-27 10:42:55.000000 UnlimitedGPT-0.0.1/UnlimitedGPT.egg-info/top_level.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-05-27 10:42:55.331952 UnlimitedGPT-0.0.1/setup.cfg
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1529 2023-05-27 10:40:58.000000 UnlimitedGPT-0.0.1/setup.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 10:42:55.323952 UnlimitedGPT-0.0.1/src/
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 10:42:55.327952 UnlimitedGPT-0.0.1/src/UnlimitedGPT/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    13097 2023-05-27 10:02:18.000000 UnlimitedGPT-0.0.1/src/UnlimitedGPT/ChatGPT.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      244 2023-05-27 10:00:18.000000 UnlimitedGPT-0.0.1/src/UnlimitedGPT/__init__.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 10:42:55.327952 UnlimitedGPT-0.0.1/src/UnlimitedGPT/internal/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1710 2023-05-27 09:21:23.000000 UnlimitedGPT-0.0.1/src/UnlimitedGPT/internal/chatgpt_data.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      294 2023-05-27 10:01:38.000000 UnlimitedGPT-0.0.1/src/UnlimitedGPT/internal/driver.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      494 2023-05-27 09:58:48.000000 UnlimitedGPT-0.0.1/src/UnlimitedGPT/internal/objects.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 11:00:42.111559 UnlimitedGPT-0.0.2/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    35149 2023-05-26 09:35:45.000000 UnlimitedGPT-0.0.2/LICENSE
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4973 2023-05-27 11:00:42.111559 UnlimitedGPT-0.0.2/PKG-INFO
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3880 2023-05-27 10:55:46.000000 UnlimitedGPT-0.0.2/README.md
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 11:00:42.107558 UnlimitedGPT-0.0.2/UnlimitedGPT.egg-info/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4973 2023-05-27 11:00:41.000000 UnlimitedGPT-0.0.2/UnlimitedGPT.egg-info/PKG-INFO
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      377 2023-05-27 11:00:42.000000 UnlimitedGPT-0.0.2/UnlimitedGPT.egg-info/SOURCES.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-05-27 11:00:41.000000 UnlimitedGPT-0.0.2/UnlimitedGPT.egg-info/dependency_links.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-05-27 11:00:41.000000 UnlimitedGPT-0.0.2/UnlimitedGPT.egg-info/requires.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       44 2023-05-27 11:00:41.000000 UnlimitedGPT-0.0.2/UnlimitedGPT.egg-info/top_level.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-05-27 11:00:42.111559 UnlimitedGPT-0.0.2/setup.cfg
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1529 2023-05-27 10:45:53.000000 UnlimitedGPT-0.0.2/setup.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 11:00:42.103558 UnlimitedGPT-0.0.2/src/
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 11:00:42.111559 UnlimitedGPT-0.0.2/src/UnlimitedGPT/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    13097 2023-05-27 10:02:18.000000 UnlimitedGPT-0.0.2/src/UnlimitedGPT/ChatGPT.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      244 2023-05-27 10:00:18.000000 UnlimitedGPT-0.0.2/src/UnlimitedGPT/__init__.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 11:00:42.111559 UnlimitedGPT-0.0.2/src/UnlimitedGPT/internal/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1710 2023-05-27 09:21:23.000000 UnlimitedGPT-0.0.2/src/UnlimitedGPT/internal/chatgpt_data.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      294 2023-05-27 10:01:38.000000 UnlimitedGPT-0.0.2/src/UnlimitedGPT/internal/driver.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      494 2023-05-27 09:58:48.000000 UnlimitedGPT-0.0.2/src/UnlimitedGPT/internal/objects.py
```

### Comparing `UnlimitedGPT-0.0.1/LICENSE` & `UnlimitedGPT-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.0.1/setup.py` & `UnlimitedGPT-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     name='UnlimitedGPT',
     author='Sxvxge',
     url='https://github.com/Sxvxgee/UnlimitedGPT',
     project_urls={
         'Documentation': 'https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md',
         'Issue tracker': 'https://github.com/Sxvxgee/UnlimitedGPT/issues',
     },
-    version="0.0.1",
+    version="0.0.2",
     packages=packages,
     license='GPL-3.0 license',
     description='An unofficial Python wrapper for OpenAI\'s ChatGPT API',
     long_description=readme,
     long_description_content_type='text/markdown',
     include_package_data=True,
     install_requires=requirements,
```

### Comparing `UnlimitedGPT-0.0.1/src/UnlimitedGPT/ChatGPT.py` & `UnlimitedGPT-0.0.2/src/UnlimitedGPT/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.0.1/src/UnlimitedGPT/internal/chatgpt_data.py` & `UnlimitedGPT-0.0.2/src/UnlimitedGPT/internal/chatgpt_data.py`

 * *Files identical despite different names*

