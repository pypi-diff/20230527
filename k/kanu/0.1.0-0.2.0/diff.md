# Comparing `tmp/kanu-0.1.0.tar.gz` & `tmp/kanu-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanu-0.1.0.tar", last modified: Wed May 24 04:40:35 2023, max compression
+gzip compressed data, was "kanu-0.2.0.tar", last modified: Fri May 26 22:21:10 2023, max compression
```

## Comparing `kanu-0.1.0.tar` & `kanu-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-05-24 04:40:35.618043 kanu-0.1.0/
--rw-r--r--   0 sbslee     (501) staff       (20)     1080 2023-05-24 04:06:50.000000 kanu-0.1.0/LICENSE
--rw-r--r--   0 sbslee     (501) staff       (20)      292 2023-05-24 04:40:35.617903 kanu-0.1.0/PKG-INFO
--rw-r--r--   0 sbslee     (501) staff       (20)        6 2023-05-24 04:06:50.000000 kanu-0.1.0/README.md
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-05-24 04:40:35.617759 kanu-0.1.0/kanu.egg-info/
--rw-r--r--   0 sbslee     (501) staff       (20)      292 2023-05-24 04:40:35.000000 kanu-0.1.0/kanu.egg-info/PKG-INFO
--rw-r--r--   0 sbslee     (501) staff       (20)      196 2023-05-24 04:40:35.000000 kanu-0.1.0/kanu.egg-info/SOURCES.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        1 2023-05-24 04:40:35.000000 kanu-0.1.0/kanu.egg-info/dependency_links.txt
--rw-r--r--   0 sbslee     (501) staff       (20)       44 2023-05-24 04:40:35.000000 kanu-0.1.0/kanu.egg-info/entry_points.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        7 2023-05-24 04:40:35.000000 kanu-0.1.0/kanu.egg-info/requires.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        1 2023-05-24 04:40:35.000000 kanu-0.1.0/kanu.egg-info/top_level.txt
--rw-r--r--   0 sbslee     (501) staff       (20)       38 2023-05-24 04:40:35.618081 kanu-0.1.0/setup.cfg
--rw-r--r--   0 sbslee     (501) staff       (20)      546 2023-05-24 04:33:43.000000 kanu-0.1.0/setup.py
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-05-26 22:21:10.800472 kanu-0.2.0/
+-rw-r--r--   0 sbslee     (501) staff       (20)     1080 2023-05-26 22:20:47.000000 kanu-0.2.0/LICENSE
+-rw-r--r--   0 sbslee     (501) staff       (20)      346 2023-05-26 22:21:10.800325 kanu-0.2.0/PKG-INFO
+-rw-r--r--   0 sbslee     (501) staff       (20)      382 2023-05-26 22:20:47.000000 kanu-0.2.0/README.md
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-05-26 22:21:10.799536 kanu-0.2.0/kanu/
+-rw-r--r--   0 sbslee     (501) staff       (20)        0 2023-05-26 22:20:47.000000 kanu-0.2.0/kanu/__init__.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     3639 2023-05-26 22:20:47.000000 kanu-0.2.0/kanu/__main__.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     2582 2023-05-26 22:20:47.000000 kanu-0.2.0/kanu/chatgpt.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     6218 2023-05-26 22:20:47.000000 kanu-0.2.0/kanu/docgpt.py
+-rw-r--r--   0 sbslee     (501) staff       (20)       21 2023-05-26 22:20:47.000000 kanu-0.2.0/kanu/version.py
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-05-26 22:21:10.800147 kanu-0.2.0/kanu.egg-info/
+-rw-r--r--   0 sbslee     (501) staff       (20)      346 2023-05-26 22:21:10.000000 kanu-0.2.0/kanu.egg-info/PKG-INFO
+-rw-r--r--   0 sbslee     (501) staff       (20)      250 2023-05-26 22:21:10.000000 kanu-0.2.0/kanu.egg-info/SOURCES.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)        1 2023-05-26 22:21:10.000000 kanu-0.2.0/kanu.egg-info/dependency_links.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)       44 2023-05-26 22:21:10.000000 kanu-0.2.0/kanu.egg-info/entry_points.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)        5 2023-05-26 22:21:10.000000 kanu-0.2.0/kanu.egg-info/top_level.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)       38 2023-05-26 22:21:10.800511 kanu-0.2.0/setup.cfg
+-rw-r--r--   0 sbslee     (501) staff       (20)      567 2023-05-26 22:20:47.000000 kanu-0.2.0/setup.py
```

### Comparing `kanu-0.1.0/LICENSE` & `kanu-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kanu-0.1.0/setup.py` & `kanu-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 exec(open("kanu/version.py").read())
 
 setup(
     name="kanu",
     version=__version__,
     author='Seung-been "Steven" Lee',
     author_email="sbstevenlee@gmail.com",
-    description="KANU",
+    description="A minimalistic Python-based GUI for various chatbots",
     url="https://github.com/sbslee/kanu",
     packages=find_packages(),
-    install_requires=["openai"],
     license="MIT",
     entry_points={"console_scripts": ["kanu=kanu.__main__:main"]},
-    long_description="This is a detailed description of the package.",
+    long_description="A minimalistic Python-based GUI for various chatbots",
     long_description_content_type="text/plain"
 )
```

