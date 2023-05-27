# Comparing `tmp/asgihandler-0.4.2.tar.gz` & `tmp/asgihandler-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgihandler-0.4.2.tar", last modified: Tue May 23 17:55:15 2023, max compression
+gzip compressed data, was "asgihandler-0.4.4.tar", last modified: Fri May 26 18:42:15 2023, max compression
```

## Comparing `asgihandler-0.4.2.tar` & `asgihandler-0.4.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 17:55:15.441125 asgihandler-0.4.2/
--rw-rw-rw-   0        0        0     1067 2022-07-16 23:50:52.000000 asgihandler-0.4.2/LICENSE
--rw-rw-rw-   0        0        0       27 2022-07-16 23:50:52.000000 asgihandler-0.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3117 2023-05-23 17:55:15.440125 asgihandler-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     2483 2023-05-02 06:18:39.000000 asgihandler-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 17:55:15.426124 asgihandler-0.4.2/asgihandler/
--rw-rw-rw-   0        0        0       21 2022-07-16 23:50:52.000000 asgihandler-0.4.2/asgihandler/__init__.py
--rw-rw-rw-   0        0        0       68 2022-07-16 23:55:07.000000 asgihandler-0.4.2/asgihandler/__version__.py
--rw-rw-rw-   0        0        0     1287 2022-08-05 19:34:25.000000 asgihandler-0.4.2/asgihandler/core.py
--rw-rw-rw-   0        0        0      424 2023-05-23 17:48:05.000000 asgihandler-0.4.2/asgihandler/userCheck.py
-drwxrwxrwx   0        0        0        0 2023-05-23 17:55:15.439124 asgihandler-0.4.2/asgihandler.egg-info/
--rw-rw-rw-   0        0        0     3117 2023-05-23 17:55:15.000000 asgihandler-0.4.2/asgihandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-05-23 17:55:15.000000 asgihandler-0.4.2/asgihandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 17:55:15.000000 asgihandler-0.4.2/asgihandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 17:55:15.000000 asgihandler-0.4.2/asgihandler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-23 17:55:15.000000 asgihandler-0.4.2/asgihandler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 17:55:15.441125 asgihandler-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     3878 2023-05-23 17:54:45.000000 asgihandler-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:42:15.923061 asgihandler-0.4.4/
+-rw-rw-rw-   0        0        0     1067 2022-07-16 23:50:52.000000 asgihandler-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0       27 2022-07-16 23:50:52.000000 asgihandler-0.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3117 2023-05-26 18:42:15.923061 asgihandler-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2483 2023-05-02 06:18:39.000000 asgihandler-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 18:42:15.906061 asgihandler-0.4.4/asgihandler/
+-rw-rw-rw-   0        0        0       21 2022-07-16 23:50:52.000000 asgihandler-0.4.4/asgihandler/__init__.py
+-rw-rw-rw-   0        0        0       68 2022-07-16 23:55:07.000000 asgihandler-0.4.4/asgihandler/__version__.py
+-rw-rw-rw-   0        0        0      916 2023-05-26 18:41:46.000000 asgihandler-0.4.4/asgihandler/core.py
+-rw-rw-rw-   0        0        0      460 2023-05-26 18:39:50.000000 asgihandler-0.4.4/asgihandler/userCheck.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:42:15.921059 asgihandler-0.4.4/asgihandler.egg-info/
+-rw-rw-rw-   0        0        0     3117 2023-05-26 18:42:15.000000 asgihandler-0.4.4/asgihandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-05-26 18:42:15.000000 asgihandler-0.4.4/asgihandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 18:42:15.000000 asgihandler-0.4.4/asgihandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-26 18:42:15.000000 asgihandler-0.4.4/asgihandler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-26 18:42:15.000000 asgihandler-0.4.4/asgihandler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 18:42:15.924060 asgihandler-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     3878 2023-05-26 18:41:46.000000 asgihandler-0.4.4/setup.py
```

### Comparing `asgihandler-0.4.2/LICENSE` & `asgihandler-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asgihandler-0.4.2/PKG-INFO` & `asgihandler-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgihandler
-Version: 0.4.2
+Version: 0.4.4
 Summary: ASGIHandler
 Home-page: https://github.com/GreaterWMS/GreaterWMS
 Author: Singosgu
 Author-email: singosgu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `asgihandler-0.4.2/README.md` & `asgihandler-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `asgihandler-0.4.2/asgihandler/core.py` & `asgihandler-0.4.4/asgihandler/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 class ASGIHandler:
     def asgi_get_handler(scope):
         query_string = scope.get('headers')
         host = ''
         referer = ''
         operator = ''
         token = ''
-        can_auth = 0
         for i in query_string:
             if i[0].decode() == 'referer':
                 referer = i[1].decode().split('/')[2]
                 continue
             elif i[0].decode() == 'host':
                 host = i[1].decode()
                 continue
@@ -20,19 +19,9 @@
                 operator = i[1].decode()
                 continue
             elif i[0].decode() == 'token':
                 token = i[1].decode()
                 continue
             else:
                 continue
-        if str(referer).startswith('192'):
-            can_auth = 0
-        else:
-            if str(referer).startswith('127'):
-                can_auth = 0
-            else:
-                if str(referer).startswith('localhost'):
-                    can_auth = 0
-                else:
-                    can_auth = 1
-        if can_auth == 1 and operator != '' and token != '':
+        if operator != '' and token != '':
             userCheck.get_auth_check(scope.get('server', ''), host, referer, operator, token)
```

### Comparing `asgihandler-0.4.2/asgihandler.egg-info/PKG-INFO` & `asgihandler-0.4.4/asgihandler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgihandler
-Version: 0.4.2
+Version: 0.4.4
 Summary: ASGIHandler
 Home-page: https://github.com/GreaterWMS/GreaterWMS
 Author: Singosgu
 Author-email: singosgu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `asgihandler-0.4.2/setup.py` & `asgihandler-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'asgihandler'
 DESCRIPTION = 'ASGIHandler'
 URL = 'https://github.com/GreaterWMS/GreaterWMS'
 EMAIL = 'singosgu@gmail.com'
 AUTHOR = 'Singosgu'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.4.2'
+VERSION = '0.4.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
 ]
 
 # What packages are optional?
```

