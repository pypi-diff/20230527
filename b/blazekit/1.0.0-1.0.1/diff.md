# Comparing `tmp/blazekit-1.0.0.tar.gz` & `tmp/blazekit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/blazekit-1.0.0.tar", last modified: Sat May 27 20:56:17 2023, max compression
+gzip compressed data, was "dist/blazekit-1.0.1.tar", last modified: Sat May 27 21:02:33 2023, max compression
```

## Comparing `blazekit-1.0.0.tar` & `blazekit-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rishabhjain   (501) staff       (20)        0 2023-05-27 20:56:17.000000 blazekit-1.0.0/
--rw-r--r--   0 rishabhjain   (501) staff       (20)      352 2023-05-27 20:56:17.000000 blazekit-1.0.0/PKG-INFO
--rw-r--r--   0 rishabhjain   (501) staff       (20)       10 2023-05-18 22:08:52.000000 blazekit-1.0.0/README.md
-drwxr-xr-x   0 rishabhjain   (501) staff       (20)        0 2023-05-27 20:56:17.000000 blazekit-1.0.0/blazekit/
--rw-r--r--   0 rishabhjain   (501) staff       (20)        0 2023-05-18 22:01:59.000000 blazekit-1.0.0/blazekit/__init__.py
--rw-r--r--   0 rishabhjain   (501) staff       (20)    10966 2023-05-22 16:22:29.000000 blazekit-1.0.0/blazekit/__main__.py
-drwxr-xr-x   0 rishabhjain   (501) staff       (20)        0 2023-05-27 20:56:17.000000 blazekit-1.0.0/blazekit.egg-info/
--rw-r--r--   0 rishabhjain   (501) staff       (20)      352 2023-05-27 20:56:16.000000 blazekit-1.0.0/blazekit.egg-info/PKG-INFO
--rw-r--r--   0 rishabhjain   (501) staff       (20)      219 2023-05-27 20:56:17.000000 blazekit-1.0.0/blazekit.egg-info/SOURCES.txt
--rw-r--r--   0 rishabhjain   (501) staff       (20)        1 2023-05-27 20:56:16.000000 blazekit-1.0.0/blazekit.egg-info/dependency_links.txt
--rw-r--r--   0 rishabhjain   (501) staff       (20)     2979 2023-05-27 20:56:17.000000 blazekit-1.0.0/blazekit.egg-info/requires.txt
--rw-r--r--   0 rishabhjain   (501) staff       (20)        9 2023-05-27 20:56:17.000000 blazekit-1.0.0/blazekit.egg-info/top_level.txt
--rw-r--r--   0 rishabhjain   (501) staff       (20)       38 2023-05-27 20:56:17.000000 blazekit-1.0.0/setup.cfg
--rw-r--r--   0 rishabhjain   (501) staff       (20)      726 2023-05-27 20:56:01.000000 blazekit-1.0.0/setup.py
+drwxr-xr-x   0 rishabhjain   (501) staff       (20)        0 2023-05-27 21:02:33.000000 blazekit-1.0.1/
+-rw-r--r--   0 rishabhjain   (501) staff       (20)     1636 2023-05-27 21:02:33.000000 blazekit-1.0.1/PKG-INFO
+-rw-r--r--   0 rishabhjain   (501) staff       (20)     1294 2023-05-27 20:59:23.000000 blazekit-1.0.1/README.md
+drwxr-xr-x   0 rishabhjain   (501) staff       (20)        0 2023-05-27 21:02:33.000000 blazekit-1.0.1/blazekit/
+-rw-r--r--   0 rishabhjain   (501) staff       (20)        0 2023-05-18 22:01:59.000000 blazekit-1.0.1/blazekit/__init__.py
+-rw-r--r--   0 rishabhjain   (501) staff       (20)    10966 2023-05-22 16:22:29.000000 blazekit-1.0.1/blazekit/__main__.py
+drwxr-xr-x   0 rishabhjain   (501) staff       (20)        0 2023-05-27 21:02:33.000000 blazekit-1.0.1/blazekit.egg-info/
+-rw-r--r--   0 rishabhjain   (501) staff       (20)     1636 2023-05-27 21:02:32.000000 blazekit-1.0.1/blazekit.egg-info/PKG-INFO
+-rw-r--r--   0 rishabhjain   (501) staff       (20)      219 2023-05-27 21:02:33.000000 blazekit-1.0.1/blazekit.egg-info/SOURCES.txt
+-rw-r--r--   0 rishabhjain   (501) staff       (20)        1 2023-05-27 21:02:32.000000 blazekit-1.0.1/blazekit.egg-info/dependency_links.txt
+-rw-r--r--   0 rishabhjain   (501) staff       (20)     3179 2023-05-27 21:02:32.000000 blazekit-1.0.1/blazekit.egg-info/requires.txt
+-rw-r--r--   0 rishabhjain   (501) staff       (20)        9 2023-05-27 21:02:33.000000 blazekit-1.0.1/blazekit.egg-info/top_level.txt
+-rw-r--r--   0 rishabhjain   (501) staff       (20)       38 2023-05-27 21:02:33.000000 blazekit-1.0.1/setup.cfg
+-rw-r--r--   0 rishabhjain   (501) staff       (20)      726 2023-05-27 21:02:06.000000 blazekit-1.0.1/setup.py
```

### Comparing `blazekit-1.0.0/blazekit/__main__.py` & `blazekit-1.0.1/blazekit/__main__.py`

 * *Files identical despite different names*

### Comparing `blazekit-1.0.0/blazekit.egg-info/requires.txt` & `blazekit-1.0.1/blazekit.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 crashtest==0.3.1
 cryptography==36.0.2
 cycler==0.11.0
 Cython==0.29.28
 debugpy==1.6.0
 decorator==5.1.1
 defusedxml==0.7.1
+docutils==0.20.1
 entrypoints==0.4
 ephem==4.1.3
 et-xmlfile==1.1.0
 executing==0.8.3
 flatbuffers==2.0
 fonttools==4.31.2
 frozenlist==1.3.0
@@ -49,41 +50,46 @@
 hijri-converter==2.2.3
 holidays==0.13
 hpack==3.0.0
 http3==0.6.7
 httpstan==4.7.2
 hyperframe==5.2.0
 idna==2.10
-importlib-metadata==4.11.3
+importlib-metadata==6.6.0
 ipykernel==6.9.2
 ipython==8.1.1
 ipython-genutils==0.2.0
 ipywidgets==7.7.0
 itsdangerous==2.1.2
+jaraco.classes==3.2.3
 jedi==0.18.1
 Jinja2==3.1.1
 jsonschema==4.4.0
 jupyter==1.0.0
 jupyter-client==7.1.2
 jupyter-console==6.4.3
 jupyter-core==4.9.2
 jupyterlab-pygments==0.1.2
 jupyterlab-widgets==1.1.0
 keras==2.8.0
 Keras-Preprocessing==1.1.2
+keyring==23.13.1
 kiwisolver==1.4.0
 korean-lunar-calendar==0.2.1
 libclang==13.0.0
 LunarCalendar==0.0.9
 Markdown==3.3.6
+markdown-it-py==2.2.0
 MarkupSafe==2.1.1
 marshmallow==3.15.0
 matplotlib==3.5.1
 matplotlib-inline==0.1.3
+mdurl==0.1.2
 mistune==0.8.4
+more-itertools==9.1.0
 multidict==6.0.2
 nb-pdf-template==4.0.0
 nbclient==0.5.13
 nbconvert==6.4.4
 nbformat==5.2.0
 nest-asyncio==1.5.4
 notebook==6.4.10
@@ -98,27 +104,28 @@
 parso==0.8.3
 pastel==0.2.1
 patsy==0.5.2
 pexpect==4.8.0
 pickleshare==0.7.5
 Pillow==9.0.1
 pip-autoremove==0.10.0
+pkginfo==1.9.6
 prometheus-client==0.13.1
 prompt-toolkit==3.0.28
 prophet==1.0.1
 protobuf==3.20.1
 psutil==5.9.0
 ptyprocess==0.7.0
 pure-eval==0.2.2
 pyarrow==9.0.0
 pyasn1==0.4.8
 pyasn1-modules==0.2.8
 pycparser==2.21
 pyee==8.2.2
-Pygments==2.11.2
+Pygments==2.15.1
 PyJWT==2.3.0
 pylance==0.1.1
 pylev==1.4.0
 PyMeeus==0.5.11
 pyparsing==3.0.7
 PyPDF2==1.26.0
 pyppeteer==1.0.2
@@ -126,17 +133,20 @@
 pysimdjson==3.2.0
 pystan==2.19.1.1
 python-dateutil==2.8.2
 pytz==2021.3
 pyzmq==22.3.0
 qtconsole==5.2.2
 QtPy==2.0.1
+readme-renderer==37.3
 requests==2.27.1
 requests-oauthlib==1.3.1
+requests-toolbelt==1.0.0
 rfc3986==1.5.0
+rich==13.3.5
 rsa==4.8
 scipy==1.8.0
 Send2Trash==1.8.0
 setuptools-git==1.2
 six==1.16.0
 soupsieve==2.3.1
 stack-data==0.2.0
@@ -149,14 +159,15 @@
 termcolor==1.1.0
 terminado==0.13.3
 testpath==0.6.0
 tf-estimator-nightly==2.8.0.dev2021122109
 tornado==6.1
 tqdm==4.63.1
 traitlets==5.1.1
+twine==4.0.2
 typing_extensions==4.2.0
 ujson==5.2.0
 uritemplate==4.1.1
 urllib3==1.26.9
 wcwidth==0.2.5
 webargs==8.1.0
 webencodings==0.5.1
```

### Comparing `blazekit-1.0.0/setup.py` & `blazekit-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt") as f:
     INSTALL_LIBRARIES = f.read().splitlines()
 
 
 setup(
     name="blazekit",
-    version="1.0.0",
+    version="1.0.1",
     author="Rishabh Jain",
     author_email="rishabhking05@gmail.com",
     description="UI to interact with Kubernetes Clusters",
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=INSTALL_LIBRARIES,
```

