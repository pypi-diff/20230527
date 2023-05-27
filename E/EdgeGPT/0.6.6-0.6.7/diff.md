# Comparing `tmp/EdgeGPT-0.6.6.tar.gz` & `tmp/EdgeGPT-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.6.6.tar", last modified: Sat May 27 06:46:26 2023, max compression
+gzip compressed data, was "EdgeGPT-0.6.7.tar", last modified: Sat May 27 10:12:42 2023, max compression
```

## Comparing `EdgeGPT-0.6.6.tar` & `EdgeGPT-0.6.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:46:26.876631 EdgeGPT-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-27 06:45:44.000000 EdgeGPT-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-27 06:46:26.876631 EdgeGPT-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-05-27 06:46:26.000000 EdgeGPT-0.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 06:46:26.876631 EdgeGPT-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-27 06:45:44.000000 EdgeGPT-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:46:26.876631 EdgeGPT-0.6.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:46:26.876631 EdgeGPT-0.6.6/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-27 06:46:26.000000 EdgeGPT-0.6.6/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-27 06:46:26.000000 EdgeGPT-0.6.6/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 06:46:26.000000 EdgeGPT-0.6.6/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-27 06:46:26.000000 EdgeGPT-0.6.6/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-27 06:46:26.000000 EdgeGPT-0.6.6/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-27 06:46:26.000000 EdgeGPT-0.6.6/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    39038 2023-05-27 06:45:44.000000 EdgeGPT-0.6.6/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-27 06:45:44.000000 EdgeGPT-0.6.6/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:12:42.877380 EdgeGPT-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-27 10:11:01.000000 EdgeGPT-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-27 10:12:42.877380 EdgeGPT-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-05-27 10:12:42.000000 EdgeGPT-0.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 10:12:42.877380 EdgeGPT-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-27 10:11:01.000000 EdgeGPT-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:12:42.877380 EdgeGPT-0.6.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:12:42.877380 EdgeGPT-0.6.7/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-27 10:12:42.000000 EdgeGPT-0.6.7/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-27 10:12:42.000000 EdgeGPT-0.6.7/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 10:12:42.000000 EdgeGPT-0.6.7/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-27 10:12:42.000000 EdgeGPT-0.6.7/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-27 10:12:42.000000 EdgeGPT-0.6.7/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-27 10:12:42.000000 EdgeGPT-0.6.7/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    39053 2023-05-27 10:11:01.000000 EdgeGPT-0.6.7/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-27 10:11:01.000000 EdgeGPT-0.6.7/src/ImageGen.py
```

### Comparing `EdgeGPT-0.6.6/LICENSE` & `EdgeGPT-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.6.6/PKG-INFO` & `EdgeGPT-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.6.6
+Version: 0.6.7
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.6.6 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.6.7 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.6.6/README.md` & `EdgeGPT-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.6.6/setup.py` & `EdgeGPT-0.6.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.6.6",
+    version="0.6.7",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.6.6/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.6.7/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.6.6
+Version: 0.6.7
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.6.6 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.6.7 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.6.6/src/EdgeGPT.py` & `EdgeGPT-0.6.7/src/EdgeGPT.py`

 * *Files 0% similar despite different names*

```diff
@@ -758,15 +758,15 @@
         cookies = json.loads(open(args.cookie_file, encoding="utf-8").read())
     bot = await Chatbot.create(proxy=args.proxy, cookies=cookies)
     session = _create_session()
     completer = _create_completer(["!help", "!exit", "!reset"])
     initial_prompt = args.prompt
 
     # Log chat history
-    def p_hist():
+    def p_hist(*args, **kwargs):
         pass
     if args.history_file:
         f = open(args.history_file, 'a+')
         p_hist = _create_history_logger(f)
 
     while True:
         print("\nYou:")
```

