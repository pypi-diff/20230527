# Comparing `tmp/UnlimitedGPT-0.0.7.tar.gz` & `tmp/UnlimitedGPT-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnlimitedGPT-0.0.7.tar", last modified: Sat May 27 12:30:12 2023, max compression
+gzip compressed data, was "UnlimitedGPT-0.0.8.tar", last modified: Sat May 27 14:00:55 2023, max compression
```

## Comparing `UnlimitedGPT-0.0.7.tar` & `UnlimitedGPT-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 12:30:12.185871 UnlimitedGPT-0.0.7/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4960 2023-05-27 12:30:12.185871 UnlimitedGPT-0.0.7/PKG-INFO
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 12:30:12.181870 UnlimitedGPT-0.0.7/UnlimitedGPT/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    13097 2023-05-27 10:02:18.000000 UnlimitedGPT-0.0.7/UnlimitedGPT/UnlimitedGPT.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      249 2023-05-27 12:22:12.000000 UnlimitedGPT-0.0.7/UnlimitedGPT/__init__.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 12:30:12.181870 UnlimitedGPT-0.0.7/UnlimitedGPT/internal/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1710 2023-05-27 09:21:23.000000 UnlimitedGPT-0.0.7/UnlimitedGPT/internal/chatgpt_data.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      294 2023-05-27 10:01:38.000000 UnlimitedGPT-0.0.7/UnlimitedGPT/internal/driver.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      494 2023-05-27 09:58:48.000000 UnlimitedGPT-0.0.7/UnlimitedGPT/internal/objects.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 12:30:12.181870 UnlimitedGPT-0.0.7/UnlimitedGPT.egg-info/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4960 2023-05-27 12:30:11.000000 UnlimitedGPT-0.0.7/UnlimitedGPT.egg-info/PKG-INFO
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      344 2023-05-27 12:30:12.000000 UnlimitedGPT-0.0.7/UnlimitedGPT.egg-info/SOURCES.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-05-27 12:30:11.000000 UnlimitedGPT-0.0.7/UnlimitedGPT.egg-info/dependency_links.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-05-27 12:30:11.000000 UnlimitedGPT-0.0.7/UnlimitedGPT.egg-info/requires.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-05-27 12:30:11.000000 UnlimitedGPT-0.0.7/UnlimitedGPT.egg-info/top_level.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-05-27 12:30:12.185871 UnlimitedGPT-0.0.7/setup.cfg
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1664 2023-05-27 12:30:07.000000 UnlimitedGPT-0.0.7/setup.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 14:00:55.179473 UnlimitedGPT-0.0.8/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     5126 2023-05-27 14:00:55.179473 UnlimitedGPT-0.0.8/PKG-INFO
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 14:00:55.175473 UnlimitedGPT-0.0.8/UnlimitedGPT/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    13097 2023-05-27 10:02:18.000000 UnlimitedGPT-0.0.8/UnlimitedGPT/UnlimitedGPT.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      249 2023-05-27 12:22:12.000000 UnlimitedGPT-0.0.8/UnlimitedGPT/__init__.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 14:00:55.179473 UnlimitedGPT-0.0.8/UnlimitedGPT/internal/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1710 2023-05-27 09:21:23.000000 UnlimitedGPT-0.0.8/UnlimitedGPT/internal/chatgpt_data.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      294 2023-05-27 10:01:38.000000 UnlimitedGPT-0.0.8/UnlimitedGPT/internal/driver.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      494 2023-05-27 09:58:48.000000 UnlimitedGPT-0.0.8/UnlimitedGPT/internal/objects.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 14:00:55.179473 UnlimitedGPT-0.0.8/UnlimitedGPT.egg-info/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     5126 2023-05-27 14:00:54.000000 UnlimitedGPT-0.0.8/UnlimitedGPT.egg-info/PKG-INFO
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      344 2023-05-27 14:00:54.000000 UnlimitedGPT-0.0.8/UnlimitedGPT.egg-info/SOURCES.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-05-27 14:00:54.000000 UnlimitedGPT-0.0.8/UnlimitedGPT.egg-info/dependency_links.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-05-27 14:00:54.000000 UnlimitedGPT-0.0.8/UnlimitedGPT.egg-info/requires.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-05-27 14:00:54.000000 UnlimitedGPT-0.0.8/UnlimitedGPT.egg-info/top_level.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-05-27 14:00:55.179473 UnlimitedGPT-0.0.8/setup.cfg
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1686 2023-05-27 14:00:49.000000 UnlimitedGPT-0.0.8/setup.py
```

### Comparing `UnlimitedGPT-0.0.7/PKG-INFO` & `UnlimitedGPT-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.0.7
+Version: 0.0.8
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Classifier: Development Status :: 5 - Production/Stable
@@ -124,7 +124,11 @@
 ## Disclaimer
 
 This project is not affiliated with OpenAI in any way. Use at your own risk. I am not responsible for any damage caused by this project. Please read the [OpenAI Terms of Service](https://beta.openai.com/terms) before using this project.
 
 ## License
 
 This project is licensed under the GPLv3 License - see the [LICENSE](LICENSE) file for details.
+
+## Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=Sxvxgee/UnlimitedGPT&type=Date)](https://star-history.com/#Sxvxgee/UnlimitedGPT&Date)
```

### Comparing `UnlimitedGPT-0.0.7/UnlimitedGPT/UnlimitedGPT.py` & `UnlimitedGPT-0.0.8/UnlimitedGPT/UnlimitedGPT.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.0.7/UnlimitedGPT/internal/chatgpt_data.py` & `UnlimitedGPT-0.0.8/UnlimitedGPT/internal/chatgpt_data.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.0.7/UnlimitedGPT.egg-info/PKG-INFO` & `UnlimitedGPT-0.0.8/UnlimitedGPT.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.0.7
+Version: 0.0.8
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Classifier: Development Status :: 5 - Production/Stable
@@ -124,7 +124,11 @@
 ## Disclaimer
 
 This project is not affiliated with OpenAI in any way. Use at your own risk. I am not responsible for any damage caused by this project. Please read the [OpenAI Terms of Service](https://beta.openai.com/terms) before using this project.
 
 ## License
 
 This project is licensed under the GPLv3 License - see the [LICENSE](LICENSE) file for details.
+
+## Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=Sxvxgee/UnlimitedGPT&type=Date)](https://star-history.com/#Sxvxgee/UnlimitedGPT&Date)
```

### Comparing `UnlimitedGPT-0.0.7/setup.py` & `UnlimitedGPT-0.0.8/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+import os
 from setuptools import setup, find_packages
 
+base_path = os.path.abspath(os.path.dirname(__file__))
+
 requirements = []
-with open('/home/sxvxge/Desktop/My Files/Code Projects/Github/UnlimitedGPT/requirements.txt') as f:
+with open(os.path.join(os.path.dirname(base_path), 'requirements.txt')) as f:
     requirements = f.read().splitlines()
 
 readme = ''
-with open('/home/sxvxge/Desktop/My Files/Code Projects/Github/UnlimitedGPT/README.md') as f:
+with open(os.path.join(os.path.dirname(base_path), 'README.md')) as f:
     readme = f.read()
 
 setup(
     name='UnlimitedGPT',
     author='Sxvxge',
     url='https://github.com/Sxvxgee/UnlimitedGPT',
     project_urls={
         'Documentation': 'https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md',
         'Issue tracker': 'https://github.com/Sxvxgee/UnlimitedGPT/issues',
     },
-    version="0.0.7",
+    version="0.0.8",
     packages=['UnlimitedGPT', 'UnlimitedGPT/internal'],
     py_modules=['UnlimitedGPT'],
     license='GPL-3.0 license',
     description='An unofficial Python wrapper for OpenAI\'s ChatGPT API',
     long_description=readme,
     long_description_content_type='text/markdown',
     include_package_data=True,
```

