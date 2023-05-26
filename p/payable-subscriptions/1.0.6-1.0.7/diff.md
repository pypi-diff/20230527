# Comparing `tmp/payable-subscriptions-1.0.6.zip` & `tmp/payable-subscriptions-1.0.7.zip`

## zipinfo {}

```diff
@@ -1,41 +1,42 @@
-Zip file size: 37211 bytes, number of entries: 39
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-10 15:51 payable-subscriptions-1.0.6/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-10 15:51 payable-subscriptions-1.0.6/payable_subscriptions.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-10 15:51 payable-subscriptions-1.0.6/sandbox/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-10 15:51 payable-subscriptions-1.0.6/payablesubs/
--rw-r--r--  2.0 unx     3340 b- defN 23-Feb-10 15:51 payable-subscriptions-1.0.6/PKG-INFO
--rw-r--r--  2.0 unx    35149 b- defN 22-Dec-11 13:43 payable-subscriptions-1.0.6/LICENSE
--rw-r--r--  2.0 unx     2633 b- defN 23-Feb-10 15:49 payable-subscriptions-1.0.6/README.md
--rw-r--r--  2.0 unx     1248 b- defN 23-Feb-10 15:51 payable-subscriptions-1.0.6/setup.py
--rw-r--r--  2.0 unx       38 b- defN 23-Feb-10 15:51 payable-subscriptions-1.0.6/setup.cfg
--rw-r--r--  2.0 unx     3340 b- defN 23-Feb-10 15:51 payable-subscriptions-1.0.6/payable_subscriptions.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      900 b- defN 23-Feb-10 15:51 payable-subscriptions-1.0.6/payable_subscriptions.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       67 b- defN 23-Feb-10 15:51 payable-subscriptions-1.0.6/payable_subscriptions.egg-info/requires.txt
--rw-r--r--  2.0 unx       20 b- defN 23-Feb-10 15:51 payable-subscriptions-1.0.6/payable_subscriptions.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Feb-10 15:51 payable-subscriptions-1.0.6/payable_subscriptions.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx      383 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.6/sandbox/asgi.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.6/sandbox/__init__.py
--rw-r--r--  2.0 unx     3914 b- defN 23-Feb-10 11:33 payable-subscriptions-1.0.6/sandbox/settings.py
--rwxr-xr-x  2.0 unx      655 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.6/sandbox/manage.py
--rw-r--r--  2.0 unx      186 b- defN 22-Dec-28 21:40 payable-subscriptions-1.0.6/sandbox/urls.py
--rw-r--r--  2.0 unx      383 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.6/sandbox/wsgi.py
--rwxr-xr-x  2.0 unx     4421 b- defN 23-Jan-30 06:30 payable-subscriptions-1.0.6/sandbox/init_db.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-10 15:51 payable-subscriptions-1.0.6/payablesubs/clients/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-10 15:51 payable-subscriptions-1.0.6/payablesubs/migrations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-10 15:51 payable-subscriptions-1.0.6/payablesubs/management/
--rw-r--r--  2.0 unx     2806 b- defN 23-Jan-06 15:56 payable-subscriptions-1.0.6/payablesubs/models.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-23 11:11 payable-subscriptions-1.0.6/payablesubs/__init__.py
--rw-r--r--  2.0 unx      273 b- defN 23-Jan-02 15:41 payable-subscriptions-1.0.6/payablesubs/apps.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-30 12:05 payable-subscriptions-1.0.6/payablesubs/clients/__init__.py
--rw-r--r--  2.0 unx     4681 b- defN 23-Feb-10 14:42 payable-subscriptions-1.0.6/payablesubs/clients/google.py
--rw-r--r--  2.0 unx      589 b- defN 23-Feb-10 11:30 payable-subscriptions-1.0.6/payablesubs/clients/venmo.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.6/payablesubs/migrations/__init__.py
--rw-r--r--  2.0 unx     2005 b- defN 23-Jan-06 15:56 payable-subscriptions-1.0.6/payablesubs/migrations/0003_payment_delete_venmotransaction.py
--rw-r--r--  2.0 unx     1156 b- defN 23-Jan-02 20:39 payable-subscriptions-1.0.6/payablesubs/migrations/0002_venmotransaction.py
--rw-r--r--  2.0 unx     3238 b- defN 23-Jan-02 20:39 payable-subscriptions-1.0.6/payablesubs/migrations/0001_initial.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-10 15:51 payable-subscriptions-1.0.6/payablesubs/management/commands/
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.6/payablesubs/management/__init__.py
--rw-r--r--  2.0 unx     3715 b- defN 23-Feb-10 14:47 payable-subscriptions-1.0.6/payablesubs/management/commands/add_subscription.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.6/payablesubs/management/commands/__init__.py
--rw-r--r--  2.0 unx     8848 b- defN 23-Feb-10 11:59 payable-subscriptions-1.0.6/payablesubs/management/commands/_payable_manager.py
-39 files, 83989 bytes uncompressed, 29965 bytes compressed:  64.3%
+Zip file size: 38463 bytes, number of entries: 40
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 15:51 payable-subscriptions-1.0.7/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 15:51 payable-subscriptions-1.0.7/payable_subscriptions.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 15:51 payable-subscriptions-1.0.7/sandbox/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 15:51 payable-subscriptions-1.0.7/payablesubs/
+-rw-r--r--  2.0 unx     3404 b- defN 23-May-26 15:51 payable-subscriptions-1.0.7/PKG-INFO
+-rw-r--r--  2.0 unx    35149 b- defN 22-Dec-11 13:43 payable-subscriptions-1.0.7/LICENSE
+-rw-r--r--  2.0 unx     2697 b- defN 23-Feb-10 16:56 payable-subscriptions-1.0.7/README.md
+-rw-r--r--  2.0 unx     1371 b- defN 23-May-26 15:48 payable-subscriptions-1.0.7/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 23-May-26 15:51 payable-subscriptions-1.0.7/setup.cfg
+-rw-r--r--  2.0 unx     3404 b- defN 23-May-26 15:51 payable-subscriptions-1.0.7/payable_subscriptions.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx      955 b- defN 23-May-26 15:51 payable-subscriptions-1.0.7/payable_subscriptions.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      156 b- defN 23-May-26 15:51 payable-subscriptions-1.0.7/payable_subscriptions.egg-info/requires.txt
+-rw-r--r--  2.0 unx       20 b- defN 23-May-26 15:51 payable-subscriptions-1.0.7/payable_subscriptions.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-26 15:51 payable-subscriptions-1.0.7/payable_subscriptions.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx      383 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.7/sandbox/asgi.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.7/sandbox/__init__.py
+-rw-r--r--  2.0 unx     4072 b- defN 23-Feb-28 15:35 payable-subscriptions-1.0.7/sandbox/settings.py
+-rwxr-xr-x  2.0 unx      655 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.7/sandbox/manage.py
+-rw-r--r--  2.0 unx      186 b- defN 22-Dec-28 21:40 payable-subscriptions-1.0.7/sandbox/urls.py
+-rw-r--r--  2.0 unx      383 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.7/sandbox/wsgi.py
+-rwxr-xr-x  2.0 unx     4421 b- defN 23-Jan-30 06:30 payable-subscriptions-1.0.7/sandbox/init_db.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 15:51 payable-subscriptions-1.0.7/payablesubs/clients/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 15:51 payable-subscriptions-1.0.7/payablesubs/migrations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 15:51 payable-subscriptions-1.0.7/payablesubs/management/
+-rw-r--r--  2.0 unx     2806 b- defN 23-Jan-06 15:56 payable-subscriptions-1.0.7/payablesubs/models.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Dec-23 11:11 payable-subscriptions-1.0.7/payablesubs/__init__.py
+-rw-r--r--  2.0 unx      273 b- defN 23-Jan-02 15:41 payable-subscriptions-1.0.7/payablesubs/apps.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-10 16:56 payable-subscriptions-1.0.7/payablesubs/clients/__init__.py
+-rw-r--r--  2.0 unx     4681 b- defN 23-Feb-10 16:56 payable-subscriptions-1.0.7/payablesubs/clients/google.py
+-rw-r--r--  2.0 unx      589 b- defN 23-Feb-10 16:56 payable-subscriptions-1.0.7/payablesubs/clients/venmo.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.7/payablesubs/migrations/__init__.py
+-rw-r--r--  2.0 unx     2005 b- defN 23-Jan-06 15:56 payable-subscriptions-1.0.7/payablesubs/migrations/0003_payment_delete_venmotransaction.py
+-rw-r--r--  2.0 unx     1156 b- defN 23-Jan-02 20:39 payable-subscriptions-1.0.7/payablesubs/migrations/0002_venmotransaction.py
+-rw-r--r--  2.0 unx     3238 b- defN 23-Jan-02 20:39 payable-subscriptions-1.0.7/payablesubs/migrations/0001_initial.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 15:51 payable-subscriptions-1.0.7/payablesubs/management/commands/
+-rw-r--r--  2.0 unx        0 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.7/payablesubs/management/__init__.py
+-rw-r--r--  2.0 unx     3715 b- defN 23-Feb-10 16:56 payable-subscriptions-1.0.7/payablesubs/management/commands/add_subscription.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.7/payablesubs/management/commands/__init__.py
+-rw-r--r--  2.0 unx     8887 b- defN 23-Mar-07 08:44 payable-subscriptions-1.0.7/payablesubs/management/commands/_payable_manager.py
+-rw-r--r--  2.0 unx     1972 b- defN 23-May-26 15:22 payable-subscriptions-1.0.7/payablesubs/management/commands/print_subscriptions.py
+40 files, 86617 bytes uncompressed, 30977 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -1,118 +1,121 @@
-Filename: payable-subscriptions-1.0.6/
+Filename: payable-subscriptions-1.0.7/
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payable_subscriptions.egg-info/
+Filename: payable-subscriptions-1.0.7/payable_subscriptions.egg-info/
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/sandbox/
+Filename: payable-subscriptions-1.0.7/sandbox/
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/
+Filename: payable-subscriptions-1.0.7/payablesubs/
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/PKG-INFO
+Filename: payable-subscriptions-1.0.7/PKG-INFO
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/LICENSE
+Filename: payable-subscriptions-1.0.7/LICENSE
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/README.md
+Filename: payable-subscriptions-1.0.7/README.md
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/setup.py
+Filename: payable-subscriptions-1.0.7/setup.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/setup.cfg
+Filename: payable-subscriptions-1.0.7/setup.cfg
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payable_subscriptions.egg-info/PKG-INFO
+Filename: payable-subscriptions-1.0.7/payable_subscriptions.egg-info/PKG-INFO
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payable_subscriptions.egg-info/SOURCES.txt
+Filename: payable-subscriptions-1.0.7/payable_subscriptions.egg-info/SOURCES.txt
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payable_subscriptions.egg-info/requires.txt
+Filename: payable-subscriptions-1.0.7/payable_subscriptions.egg-info/requires.txt
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payable_subscriptions.egg-info/top_level.txt
+Filename: payable-subscriptions-1.0.7/payable_subscriptions.egg-info/top_level.txt
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payable_subscriptions.egg-info/dependency_links.txt
+Filename: payable-subscriptions-1.0.7/payable_subscriptions.egg-info/dependency_links.txt
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/sandbox/asgi.py
+Filename: payable-subscriptions-1.0.7/sandbox/asgi.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/sandbox/__init__.py
+Filename: payable-subscriptions-1.0.7/sandbox/__init__.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/sandbox/settings.py
+Filename: payable-subscriptions-1.0.7/sandbox/settings.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/sandbox/manage.py
+Filename: payable-subscriptions-1.0.7/sandbox/manage.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/sandbox/urls.py
+Filename: payable-subscriptions-1.0.7/sandbox/urls.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/sandbox/wsgi.py
+Filename: payable-subscriptions-1.0.7/sandbox/wsgi.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/sandbox/init_db.py
+Filename: payable-subscriptions-1.0.7/sandbox/init_db.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/clients/
+Filename: payable-subscriptions-1.0.7/payablesubs/clients/
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/migrations/
+Filename: payable-subscriptions-1.0.7/payablesubs/migrations/
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/management/
+Filename: payable-subscriptions-1.0.7/payablesubs/management/
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/models.py
+Filename: payable-subscriptions-1.0.7/payablesubs/models.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/__init__.py
+Filename: payable-subscriptions-1.0.7/payablesubs/__init__.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/apps.py
+Filename: payable-subscriptions-1.0.7/payablesubs/apps.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/clients/__init__.py
+Filename: payable-subscriptions-1.0.7/payablesubs/clients/__init__.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/clients/google.py
+Filename: payable-subscriptions-1.0.7/payablesubs/clients/google.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/clients/venmo.py
+Filename: payable-subscriptions-1.0.7/payablesubs/clients/venmo.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/migrations/__init__.py
+Filename: payable-subscriptions-1.0.7/payablesubs/migrations/__init__.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/migrations/0003_payment_delete_venmotransaction.py
+Filename: payable-subscriptions-1.0.7/payablesubs/migrations/0003_payment_delete_venmotransaction.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/migrations/0002_venmotransaction.py
+Filename: payable-subscriptions-1.0.7/payablesubs/migrations/0002_venmotransaction.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/migrations/0001_initial.py
+Filename: payable-subscriptions-1.0.7/payablesubs/migrations/0001_initial.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/management/commands/
+Filename: payable-subscriptions-1.0.7/payablesubs/management/commands/
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/management/__init__.py
+Filename: payable-subscriptions-1.0.7/payablesubs/management/__init__.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/management/commands/add_subscription.py
+Filename: payable-subscriptions-1.0.7/payablesubs/management/commands/add_subscription.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/management/commands/__init__.py
+Filename: payable-subscriptions-1.0.7/payablesubs/management/commands/__init__.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.6/payablesubs/management/commands/_payable_manager.py
+Filename: payable-subscriptions-1.0.7/payablesubs/management/commands/_payable_manager.py
+Comment: 
+
+Filename: payable-subscriptions-1.0.7/payablesubs/management/commands/print_subscriptions.py
 Comment: 
 
 Zip file comment:
```

## Comparing `payable-subscriptions-1.0.6/PKG-INFO` & `payable-subscriptions-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payable-subscriptions
-Version: 1.0.6
+Version: 1.0.7
 Summary: Integrates out-of-the-box payment processing for django-flexible-subscriptions
 Home-page: https://github.com/curtis628/payable-subscriptions
 Author: Tyler Curtis
 Author-email: tjcurt@gmail.com
 Project-URL: Source code, https://github.com/curtis628/payable-subscriptions
 Project-URL: Issues, https://github.com/curtis628/payable-subscriptions/issues
 Classifier: Framework :: Django :: 4.1
@@ -15,14 +15,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # payable-subscriptions
 
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Code Style](https://img.shields.io/badge/code%20style-isort-blue.svg)](https://github.com/timothycrosley/isort)
+[PyPI Project](https://pypi.org/project/payable-subscriptions/)
 
 --------------
 This builds upon the subscription and recurrent billing from [django-flexible-subscriptions](https://github.com/studybuffalo/django-flexible-subscriptions)
 with supported payment vendors, such as Venmo.
 
 * Integrates out-of-the-box payment processing for [django-flexible-subscriptions](https://github.com/studybuffalo/django-flexible-subscriptions).
   * NOTE: Currently, only Venmo is supported.
```

## Comparing `payable-subscriptions-1.0.6/LICENSE` & `payable-subscriptions-1.0.7/LICENSE`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.6/README.md` & `payable-subscriptions-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # payable-subscriptions
 
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Code Style](https://img.shields.io/badge/code%20style-isort-blue.svg)](https://github.com/timothycrosley/isort)
+[PyPI Project](https://pypi.org/project/payable-subscriptions/)
 
 --------------
 This builds upon the subscription and recurrent billing from [django-flexible-subscriptions](https://github.com/studybuffalo/django-flexible-subscriptions)
 with supported payment vendors, such as Venmo.
 
 * Integrates out-of-the-box payment processing for [django-flexible-subscriptions](https://github.com/studybuffalo/django-flexible-subscriptions).
   * NOTE: Currently, only Venmo is supported.
```

## Comparing `payable-subscriptions-1.0.6/setup.py` & `payable-subscriptions-1.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="payable-subscriptions",
-    version="1.0.6",
+    version="1.0.7",
     url='https://github.com/curtis628/payable-subscriptions',
     author='Tyler Curtis',
     author_email="tjcurt@gmail.com",
     description="Integrates out-of-the-box payment processing for django-flexible-subscriptions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['tests*']),
@@ -19,15 +19,18 @@
         'Source code': 'https://github.com/curtis628/payable-subscriptions',
         'Issues': 'https://github.com/curtis628/payable-subscriptions/issues',
     },
     python_requires='>=3.7',
     install_requires=[
         'django>=4.0',
         'django-flexible-subscriptions>=0.15.1',
-        'venmo-api>=0.3.1'
+        'venmo-api>=0.3.1',
+        'google-api-python-client>=2.74.0',
+        'google-auth-httplib2>=0.1.0',
+        'google-auth-oauthlib>=0.8.0',
     ],
     tests_require=[
         'pytest>=6.0.0',
     ],
     # See http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         'Framework :: Django :: 4.1',
```

## Comparing `payable-subscriptions-1.0.6/payable_subscriptions.egg-info/PKG-INFO` & `payable-subscriptions-1.0.7/payable_subscriptions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payable-subscriptions
-Version: 1.0.6
+Version: 1.0.7
 Summary: Integrates out-of-the-box payment processing for django-flexible-subscriptions
 Home-page: https://github.com/curtis628/payable-subscriptions
 Author: Tyler Curtis
 Author-email: tjcurt@gmail.com
 Project-URL: Source code, https://github.com/curtis628/payable-subscriptions
 Project-URL: Issues, https://github.com/curtis628/payable-subscriptions/issues
 Classifier: Framework :: Django :: 4.1
@@ -15,14 +15,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # payable-subscriptions
 
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Code Style](https://img.shields.io/badge/code%20style-isort-blue.svg)](https://github.com/timothycrosley/isort)
+[PyPI Project](https://pypi.org/project/payable-subscriptions/)
 
 --------------
 This builds upon the subscription and recurrent billing from [django-flexible-subscriptions](https://github.com/studybuffalo/django-flexible-subscriptions)
 with supported payment vendors, such as Venmo.
 
 * Integrates out-of-the-box payment processing for [django-flexible-subscriptions](https://github.com/studybuffalo/django-flexible-subscriptions).
   * NOTE: Currently, only Venmo is supported.
```

## Comparing `payable-subscriptions-1.0.6/payable_subscriptions.egg-info/SOURCES.txt` & `payable-subscriptions-1.0.7/payable_subscriptions.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 payablesubs/clients/__init__.py
 payablesubs/clients/google.py
 payablesubs/clients/venmo.py
 payablesubs/management/__init__.py
 payablesubs/management/commands/__init__.py
 payablesubs/management/commands/_payable_manager.py
 payablesubs/management/commands/add_subscription.py
+payablesubs/management/commands/print_subscriptions.py
 payablesubs/migrations/0001_initial.py
 payablesubs/migrations/0002_venmotransaction.py
 payablesubs/migrations/0003_payment_delete_venmotransaction.py
 payablesubs/migrations/__init__.py
 sandbox/__init__.py
 sandbox/asgi.py
 sandbox/init_db.py
```

## Comparing `payable-subscriptions-1.0.6/sandbox/settings.py` & `payable-subscriptions-1.0.7/sandbox/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Django settings file to get basic Django instance running."""
 
 from pathlib import Path
 import os
+import sys
 
 # Build paths inside the project like this: BASE_DIR / 'subdir'.
 BASE_DIR = Path(__file__).resolve().parent
 
-DFS_MANAGER_CLASS = 'payablesubs.management.commands.payable_manager.PayableManager'
+DFS_MANAGER_CLASS = 'payablesubs.management.commands._payable_manager.PayableManager'
 
 # Quick-start development settings - unsuitable for production
 # See https://docs.djangoproject.com/en/4.1/howto/deployment/checklist/
 
 # SECURITY WARNING: keep the secret key used in production secret!
 SECRET_KEY = 'django-insecure-*!5vx+@1a%35cad9vzv9w5@1g$_i(8nd_97(^&%hr=h@&-()b+'
 
@@ -132,8 +133,13 @@
         "console": {
             "level": "DEBUG",
             "class": "logging.StreamHandler",
             "formatter": "standard",
         }
     },
     "loggers": {"payablesubs": {"handlers": ["console"], "level": "DEBUG"}},
-}
+}
+
+print(
+    f"Running payablesubs in sandbox-mode.\n{BASE_DIR=}\n{PAYABLESUBS_BILLING_ENABLED=}\n{PAYABLESUBS_DRY_RUN=}",
+    file=sys.stderr,
+)
```

## Comparing `payable-subscriptions-1.0.6/sandbox/manage.py` & `payable-subscriptions-1.0.7/sandbox/manage.py`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.6/sandbox/init_db.py` & `payable-subscriptions-1.0.7/sandbox/init_db.py`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.6/payablesubs/models.py` & `payable-subscriptions-1.0.7/payablesubs/models.py`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.6/payablesubs/clients/google.py` & `payable-subscriptions-1.0.7/payablesubs/clients/google.py`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.6/payablesubs/clients/venmo.py` & `payable-subscriptions-1.0.7/payablesubs/clients/venmo.py`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.6/payablesubs/migrations/0003_payment_delete_venmotransaction.py` & `payable-subscriptions-1.0.7/payablesubs/migrations/0003_payment_delete_venmotransaction.py`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.6/payablesubs/migrations/0002_venmotransaction.py` & `payable-subscriptions-1.0.7/payablesubs/migrations/0002_venmotransaction.py`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.6/payablesubs/migrations/0001_initial.py` & `payable-subscriptions-1.0.7/payablesubs/migrations/0001_initial.py`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.6/payablesubs/management/commands/add_subscription.py` & `payable-subscriptions-1.0.7/payablesubs/management/commands/add_subscription.py`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.6/payablesubs/management/commands/_payable_manager.py` & `payable-subscriptions-1.0.7/payablesubs/management/commands/_payable_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,16 @@
             self.venmo_txns = [
                 t
                 for t in txns
                 if (t.payment_type == "pay" and t.target.username == venmo_profile.username)
                 or (t.payment_type == "charge" and t.actor.username == venmo_profile.username)
             ]
             txn_strs = [f"{_txn_tostring(t)}" for t in self.venmo_txns]
-            logger.debug(f"{len(self.venmo_txns)} / {len(txns)} from VENMO are payments to us.\n" "\n".join(txn_strs))
+            big_txn_str = "\n".join(txn_strs)
+            logger.debug(f"{len(self.venmo_txns)} / {len(txns)} from VENMO are payments to us.\n{big_txn_str}")
 
         last_payment = Payment.objects.filter(user=sub.user).order_by("-date_transaction").first()
         search_begin_date = last_payment.date_transaction if last_payment else sub.date_billing_start
 
         venmo_acct = VenmoAccount.objects.filter(user=sub.user).first()
         if not venmo_acct:
             logger.warning(f"There's no Venmo account details for {sub.user}!")
```

