# Comparing `tmp/rsp_jupyter_extensions-0.8.1.tar.gz` & `tmp/rsp_jupyter_extensions-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsp_jupyter_extensions-0.8.1.tar", last modified: Fri May 26 21:50:27 2023, max compression
+gzip compressed data, was "rsp_jupyter_extensions-0.8.3.tar", last modified: Fri May 26 22:44:57 2023, max compression
```

## Comparing `rsp_jupyter_extensions-0.8.1.tar` & `rsp_jupyter_extensions-0.8.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.580650 rsp_jupyter_extensions-0.8.1/
--rw-r--r--   0 adam       (501) staff       (20)     1068 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)      480 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)     3949 2023-05-26 21:50:27.579962 rsp_jupyter_extensions-0.8.1/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     3072 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/README.md
--rw-r--r--   0 adam       (501) staff       (20)     1146 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/RELEASE.md
--rw-r--r--   0 adam       (501) staff       (20)      205 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/install.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.546509 rsp_jupyter_extensions-0.8.1/jupyter-config/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.556019 rsp_jupyter_extensions-0.8.1/jupyter-config/nb-config/
--rw-r--r--   0 adam       (501) staff       (20)       99 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/jupyter-config/nb-config/rsp_jupyter_extensions.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.556699 rsp_jupyter_extensions-0.8.1/jupyter-config/server-config/
--rw-r--r--   0 adam       (501) staff       (20)       97 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/jupyter-config/server-config/rsp_jupyter_extensions.json
--rw-r--r--   0 adam       (501) staff       (20)     3052 2023-05-26 21:43:44.000000 rsp_jupyter_extensions-0.8.1/package.json
--rw-r--r--   0 adam       (501) staff       (20)      915 2023-05-26 21:43:44.000000 rsp_jupyter_extensions-0.8.1/pyproject.toml
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.561416 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/
--rw-r--r--   0 adam       (501) staff       (20)      699 2021-09-15 20:02:14.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     2218 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/environment.py
--rw-r--r--   0 adam       (501) staff       (20)     2311 2022-09-06 19:43:05.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/execution.py
--rw-r--r--   0 adam       (501) staff       (20)      916 2022-09-06 19:43:05.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/handlers.py
--rw-r--r--   0 adam       (501) staff       (20)     1573 2021-09-15 20:02:14.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/hub.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.566196 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/
--rw-r--r--   0 adam       (501) staff       (20)     3194 2023-05-26 21:35:52.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/package.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.570609 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/static/
--rw-r--r--   0 adam       (501) staff       (20)     6154 2023-05-26 21:35:52.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/static/360.fc403a4ceb567571372e.js
--rw-r--r--   0 adam       (501) staff       (20)     3377 2023-05-26 21:35:52.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/static/747.b57adabf32495ac79fb2.js
--rw-r--r--   0 adam       (501) staff       (20)     6866 2023-05-26 21:35:52.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/static/remoteEntry.ba7b3ca42c9aa9705c93.js
--rw-r--r--   0 adam       (501) staff       (20)      165 2023-05-26 21:35:51.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/static/style.js
--rw-r--r--   0 adam       (501) staff       (20)     2452 2023-05-26 21:35:52.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/static/third-party-licenses.json
--rw-r--r--   0 adam       (501) staff       (20)     3298 2022-09-06 19:43:05.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/query.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.571323 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/templates/
--rw-r--r--   0 adam       (501) staff       (20)     2735 2022-09-16 20:51:36.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/templates/portal_query.ipynb.template
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.565625 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)     3949 2023-05-26 21:50:27.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     1306 2023-05-26 21:50:27.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-05-26 21:50:27.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2021-09-22 18:31:11.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions.egg-info/not-zip-safe
--rw-r--r--   0 adam       (501) staff       (20)       41 2023-05-26 21:50:27.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)       23 2023-05-26 21:50:27.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)       38 2023-05-26 21:50:27.580813 rsp_jupyter_extensions-0.8.1/setup.cfg
--rw-r--r--   0 adam       (501) staff       (20)     3120 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.1/setup.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.576768 rsp_jupyter_extensions-0.8.1/src/
--rw-r--r--   0 adam       (501) staff       (20)     1577 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.1/src/DisplayLabVersion.tsx
--rw-r--r--   0 adam       (501) staff       (20)     4015 2023-05-26 19:05:55.000000 rsp_jupyter_extensions-0.8.1/src/displayversion.ts
--rw-r--r--   0 adam       (501) staff       (20)     1420 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.1/src/index.ts
--rw-r--r--   0 adam       (501) staff       (20)     5503 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.1/src/query.ts
--rw-r--r--   0 adam       (501) staff       (20)     4737 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.1/src/savequit.ts
--rw-r--r--   0 adam       (501) staff       (20)      304 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.1/src/tokens.ts
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.578913 rsp_jupyter_extensions-0.8.1/style/
--rw-r--r--   0 adam       (501) staff       (20)        0 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/style/base.css
--rw-r--r--   0 adam       (501) staff       (20)       25 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/style/index.css
--rw-r--r--   0 adam       (501) staff       (20)       21 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/style/index.js
--rw-r--r--   0 adam       (501) staff       (20)      580 2023-05-26 19:05:55.000000 rsp_jupyter_extensions-0.8.1/tsconfig.json
--rw-r--r--   0 adam       (501) staff       (20)   203643 2023-05-26 21:35:08.000000 rsp_jupyter_extensions-0.8.1/yarn.lock
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.054662 rsp_jupyter_extensions-0.8.3/
+-rw-r--r--   0 adam       (501) staff       (20)     1068 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)      480 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)     3949 2023-05-26 22:44:57.054331 rsp_jupyter_extensions-0.8.3/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     3072 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/README.md
+-rw-r--r--   0 adam       (501) staff       (20)     1146 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/RELEASE.md
+-rw-r--r--   0 adam       (501) staff       (20)      205 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/install.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.029961 rsp_jupyter_extensions-0.8.3/jupyter-config/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.037867 rsp_jupyter_extensions-0.8.3/jupyter-config/nb-config/
+-rw-r--r--   0 adam       (501) staff       (20)       99 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/jupyter-config/nb-config/rsp_jupyter_extensions.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.038308 rsp_jupyter_extensions-0.8.3/jupyter-config/server-config/
+-rw-r--r--   0 adam       (501) staff       (20)       97 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/jupyter-config/server-config/rsp_jupyter_extensions.json
+-rw-r--r--   0 adam       (501) staff       (20)     3052 2023-05-26 22:31:06.000000 rsp_jupyter_extensions-0.8.3/package.json
+-rw-r--r--   0 adam       (501) staff       (20)      915 2023-05-26 21:43:44.000000 rsp_jupyter_extensions-0.8.3/pyproject.toml
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.041835 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/
+-rw-r--r--   0 adam       (501) staff       (20)      699 2021-09-15 20:02:14.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     2218 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/environment.py
+-rw-r--r--   0 adam       (501) staff       (20)     2311 2022-09-06 19:43:05.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/execution.py
+-rw-r--r--   0 adam       (501) staff       (20)      916 2022-09-06 19:43:05.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/handlers.py
+-rw-r--r--   0 adam       (501) staff       (20)     1573 2021-09-15 20:02:14.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/hub.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.044893 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/
+-rw-r--r--   0 adam       (501) staff       (20)     3194 2023-05-26 21:53:39.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/package.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.048391 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/
+-rw-r--r--   0 adam       (501) staff       (20)     6154 2023-05-26 21:53:39.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/360.fc403a4ceb567571372e.js
+-rw-r--r--   0 adam       (501) staff       (20)     3377 2023-05-26 21:53:39.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/747.b57adabf32495ac79fb2.js
+-rw-r--r--   0 adam       (501) staff       (20)     6866 2023-05-26 21:53:39.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/remoteEntry.ba7b3ca42c9aa9705c93.js
+-rw-r--r--   0 adam       (501) staff       (20)      165 2023-05-26 21:53:38.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/style.js
+-rw-r--r--   0 adam       (501) staff       (20)     2452 2023-05-26 21:53:39.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/third-party-licenses.json
+-rw-r--r--   0 adam       (501) staff       (20)     3298 2022-09-06 19:43:05.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/query.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.048897 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/templates/
+-rw-r--r--   0 adam       (501) staff       (20)     2735 2022-09-16 20:51:36.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/templates/portal_query.ipynb.template
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.044528 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)     3949 2023-05-26 22:44:56.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     1306 2023-05-26 22:44:56.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-05-26 22:44:56.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2021-09-22 18:31:11.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions.egg-info/not-zip-safe
+-rw-r--r--   0 adam       (501) staff       (20)       41 2023-05-26 22:44:56.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)       23 2023-05-26 22:44:56.000000 rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)       38 2023-05-26 22:44:57.054752 rsp_jupyter_extensions-0.8.3/setup.cfg
+-rw-r--r--   0 adam       (501) staff       (20)     3120 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.3/setup.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.052634 rsp_jupyter_extensions-0.8.3/src/
+-rw-r--r--   0 adam       (501) staff       (20)     1577 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.3/src/DisplayLabVersion.tsx
+-rw-r--r--   0 adam       (501) staff       (20)     4015 2023-05-26 19:05:55.000000 rsp_jupyter_extensions-0.8.3/src/displayversion.ts
+-rw-r--r--   0 adam       (501) staff       (20)     1420 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.3/src/index.ts
+-rw-r--r--   0 adam       (501) staff       (20)     5503 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.3/src/query.ts
+-rw-r--r--   0 adam       (501) staff       (20)     4737 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.3/src/savequit.ts
+-rw-r--r--   0 adam       (501) staff       (20)      304 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.3/src/tokens.ts
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 22:44:57.053831 rsp_jupyter_extensions-0.8.3/style/
+-rw-r--r--   0 adam       (501) staff       (20)        0 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/style/base.css
+-rw-r--r--   0 adam       (501) staff       (20)       25 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/style/index.css
+-rw-r--r--   0 adam       (501) staff       (20)       21 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.3/style/index.js
+-rw-r--r--   0 adam       (501) staff       (20)      580 2023-05-26 19:05:55.000000 rsp_jupyter_extensions-0.8.3/tsconfig.json
+-rw-r--r--   0 adam       (501) staff       (20)   203643 2023-05-26 21:35:08.000000 rsp_jupyter_extensions-0.8.3/yarn.lock
```

### Comparing `rsp_jupyter_extensions-0.8.1/LICENSE` & `rsp_jupyter_extensions-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/PKG-INFO` & `rsp_jupyter_extensions-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsp_jupyter_extensions
-Version: 0.8.1
+Version: 0.8.3
 Summary: Jupyter Extensions for the RSP
 Home-page: https://github.com/lsst-sqre/rsp-jupyter-extensions
 Author: Adam Thornton
 Author-email: athornton@lsst.org
 License: MIT
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `rsp_jupyter_extensions-0.8.1/README.md` & `rsp_jupyter_extensions-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/RELEASE.md` & `rsp_jupyter_extensions-0.8.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/package.json` & `rsp_jupyter_extensions-0.8.3/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.8.3'"}*

```diff
@@ -97,9 +97,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.8.1"
+    "version": "0.8.3"
 }
```

### Comparing `rsp_jupyter_extensions-0.8.1/pyproject.toml` & `rsp_jupyter_extensions-0.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/__init__.py` & `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/environment.py` & `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/environment.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/execution.py` & `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/execution.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/handlers.py` & `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/handlers.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/hub.py` & `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/hub.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/package.json` & `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/package.json`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/static/360.fc403a4ceb567571372e.js` & `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/360.fc403a4ceb567571372e.js`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/static/747.b57adabf32495ac79fb2.js` & `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/747.b57adabf32495ac79fb2.js`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/static/remoteEntry.ba7b3ca42c9aa9705c93.js` & `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/remoteEntry.ba7b3ca42c9aa9705c93.js`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/static/third-party-licenses.json` & `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/query.py` & `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/query.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/templates/portal_query.ipynb.template` & `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions/templates/portal_query.ipynb.template`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions.egg-info/PKG-INFO` & `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsp-jupyter-extensions
-Version: 0.8.1
+Version: 0.8.3
 Summary: Jupyter Extensions for the RSP
 Home-page: https://github.com/lsst-sqre/rsp-jupyter-extensions
 Author: Adam Thornton
 Author-email: athornton@lsst.org
 License: MIT
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions.egg-info/SOURCES.txt` & `rsp_jupyter_extensions-0.8.3/rsp_jupyter_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/setup.py` & `rsp_jupyter_extensions-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/src/DisplayLabVersion.tsx` & `rsp_jupyter_extensions-0.8.3/src/DisplayLabVersion.tsx`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/src/displayversion.ts` & `rsp_jupyter_extensions-0.8.3/src/displayversion.ts`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/src/index.ts` & `rsp_jupyter_extensions-0.8.3/src/index.ts`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/src/query.ts` & `rsp_jupyter_extensions-0.8.3/src/query.ts`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/src/savequit.ts` & `rsp_jupyter_extensions-0.8.3/src/savequit.ts`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/tsconfig.json` & `rsp_jupyter_extensions-0.8.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.1/yarn.lock` & `rsp_jupyter_extensions-0.8.3/yarn.lock`

 * *Files identical despite different names*

