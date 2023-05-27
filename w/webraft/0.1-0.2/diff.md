# Comparing `tmp/webraft-0.1.tar.gz` & `tmp/webraft-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\webraft-0.1.tar", last modified: Thu May 11 14:40:45 2023, max compression
+gzip compressed data, was "dist\webraft-0.2.tar", last modified: Sat May 27 20:40:12 2023, max compression
```

## Comparing `webraft-0.1.tar` & `webraft-0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 14:40:45.000000 webraft-0.1/
--rw-rw-rw-   0        0        0     1695 2023-05-11 14:40:45.000000 webraft-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-11 14:40:45.000000 webraft-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1808 2023-05-11 14:40:20.000000 webraft-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 14:40:45.000000 webraft-0.1/webraft/
--rw-rw-rw-   0        0        0        0 2023-04-06 16:55:39.000000 webraft-0.1/webraft/__init__.py
--rw-rw-rw-   0        0        0    11357 2023-05-11 13:12:41.000000 webraft-0.1/webraft/core.py
--rw-rw-rw-   0        0        0      545 2023-04-06 16:55:39.000000 webraft-0.1/webraft/ipinfo.py
-drwxrwxrwx   0        0        0        0 2023-05-11 14:40:45.000000 webraft-0.1/webraft.egg-info/
--rw-rw-rw-   0        0        0     1695 2023-05-11 14:40:44.000000 webraft-0.1/webraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-05-11 14:40:44.000000 webraft-0.1/webraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 14:40:44.000000 webraft-0.1/webraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-05-11 14:40:44.000000 webraft-0.1/webraft.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-11 14:40:44.000000 webraft-0.1/webraft.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 20:40:12.000000 webraft-0.2/
+-rw-rw-rw-   0        0        0     1631 2023-05-27 20:40:12.000000 webraft-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3944 2023-05-15 06:04:47.000000 webraft-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-27 20:40:12.000000 webraft-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1701 2023-05-27 20:39:43.000000 webraft-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 20:40:12.000000 webraft-0.2/webraft/
+-rw-rw-rw-   0        0        0        0 2023-04-06 16:55:39.000000 webraft-0.2/webraft/__init__.py
+-rw-rw-rw-   0        0        0    12080 2023-05-27 20:35:50.000000 webraft-0.2/webraft/core.py
+-rw-rw-rw-   0        0        0      545 2023-04-06 16:55:39.000000 webraft-0.2/webraft/ipinfo.py
+drwxrwxrwx   0        0        0        0 2023-05-27 20:40:12.000000 webraft-0.2/webraft.egg-info/
+-rw-rw-rw-   0        0        0     1631 2023-05-27 20:40:11.000000 webraft-0.2/webraft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-05-27 20:40:11.000000 webraft-0.2/webraft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 20:40:11.000000 webraft-0.2/webraft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-27 20:40:11.000000 webraft-0.2/webraft.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-27 20:40:11.000000 webraft-0.2/webraft.egg-info/top_level.txt
```

### Comparing `webraft-0.1/PKG-INFO` & `webraft-0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: webraft
-Version: 0.1
-Summary: WebRaft is a Python library for creating and reading JSON Web Tokens, extracting user agent information, retrieving IP data, and creating and reading API keys.
+Version: 0.2
+Summary: WebRaft for python web developers
 Home-page: UNKNOWN
 Author: Momin Iqbal (Pakistan Dedov)
 Author-email: <mominiqbal1214@gmail.com>
 License: UNKNOWN
 Description: 
-            # WebRaft
+        # WebRaft
         
-            creating and reading JSON Web Tokens, extracting user agent
-            information, retrieving IP data, and creating and reading API keys
+        WebRaft for python web developers to creating and reading JSON Web Tokens, extracting user agent information (like os,device,browser), retrieving IP data, and creating and reading API keys.
         
-            # How to install webraft
+        # How to install webraft
         
-            ```python
-            pip install webraft
-            ```
-            # Documentation
-            open Github repository for the WebRaft Python library. The link is included in the package's documentation to provide
-            users with access to the source code and additional information about the library.
-            <br>
-            https://github.com/MominIqbal-1234/webraft
+        ```python
+        pip install webraft
+        ```
+        # Documentation
+        open Github repository for the WebRaft Python library. The link is included in the package's documentation to provide
+        users with access to the source code and additional information about the library.
+        <br>
+        Githib : https://github.com/MominIqbal-1234/webraft
+        <br>
+        Documentation : https://webraft.mefiz.com
         
         
-        
-            Check Our Site : https://mefiz.com/about </br>
-            Developed by : Momin Iqbal
+        Check Our Site : https://mefiz.com/about </br>
+        Developed by : Momin Iqbal
         
             
 Keywords: webraft,WebRaftpython,django,jwt,jwt for django,create api key,read api key,create token,read token,user agent django,ip info python,user agent python,jwt flask,jwt bottle,jwt fastapi
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `webraft-0.1/setup.py` & `webraft-0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from setuptools import setup, find_packages
 
 
 
-VERSION = '0.1'
-DESCRIPTION = "WebRaft is a Python library for creating and reading JSON Web Tokens, extracting user agent information, retrieving IP data, and creating and reading API keys."
+VERSION = '0.2'
+DESCRIPTION = "WebRaft for python web developers"
 
 
 # Setting up
 setup(
     name="webraft",
     version=VERSION,
     author="Momin Iqbal (Pakistan Dedov)",
     author_email="<mominiqbal1214@gmail.com>",
     description=DESCRIPTION,
     long_description="""
-    # WebRaft
+# WebRaft
 
-    creating and reading JSON Web Tokens, extracting user agent
-    information, retrieving IP data, and creating and reading API keys
+WebRaft for python web developers to creating and reading JSON Web Tokens, extracting user agent information (like os,device,browser), retrieving IP data, and creating and reading API keys.
 
-    # How to install webraft
+# How to install webraft
 
-    ```python
-    pip install webraft
-    ```
-    # Documentation
-    open Github repository for the WebRaft Python library. The link is included in the package's documentation to provide
-    users with access to the source code and additional information about the library.
-    <br>
-    https://github.com/MominIqbal-1234/webraft
+```python
+pip install webraft
+```
+# Documentation
+open Github repository for the WebRaft Python library. The link is included in the package's documentation to provide
+users with access to the source code and additional information about the library.
+<br>
+Githib : https://github.com/MominIqbal-1234/webraft
+<br>
+Documentation : https://webraft.mefiz.com
 
 
-
-    Check Our Site : https://mefiz.com/about </br>
-    Developed by : Momin Iqbal
+Check Our Site : https://mefiz.com/about </br>
+Developed by : Momin Iqbal
 
     """,
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    install_requires=["django","djangorestframework","PyJWT","fastapi","flask","bottle"],
+    install_requires=["PyJWT",'cryptography'],
     keywords=['webraft','WebRaft''python', 'django', 'jwt', 'jwt for django','create api key','read api key','create token','read token','user agent django','ip info python','user agent python','jwt flask','jwt bottle','jwt fastapi'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `webraft-0.1/webraft/core.py` & `webraft-0.2/webraft/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import datetime
 from cryptography.fernet import Fernet
 from .ipinfo import IPInfo
-from user_agents import parse
+
+import pkg_resources
 import jwt
 try:
+    from user_agents import parse
+except:
+    pass
+try:
     from django.middleware import csrf
     from django_user_agents.utils import get_user_agent
 except:
     pass
 
 
 __name__ = "webraft"
@@ -32,40 +37,49 @@
 ----------------------------------------------------------------------------------------------------------------
 
 Check Our Site : https://mefiz.com
 
 """
 
 
-_framework = [
-
+__framework__ = [
+    
     "django",
     "flask",
     "fastapi",
     "bottle",
 
 ]
 
 
+__algorithm__ = [
+    "HS256",
+    "HS512",
+    "RS256",
+]
+
+
 
 
 class JWTToken:
-    def __init__(self, secret_key=None,expiry_token=None,framework=None):
+    def __init__(self, secret_key=None,expiry_token=None,framework=None,algorithm=None):
         """
         The JWTToken class that creates and reads JSON Web Tokens
         with a specified secret key, expiry date, and framework.
         
         """
+        self.installframework(framework)
         self.validateexpirytoken(expiry_token)
         self.validateframework(framework)
+        self.validatealgorithm(algorithm)
         self.secret_key = secret_key
         self.expiry_token = int(expiry_token)
         self.framework=framework
         self.today = datetime.datetime.now()
-        self.algorithm = "HS512"
+        self.algorithm = algorithm
         
         
     def create(self,request,data:list) -> str:
         """
         This function creates a token using the provided data and request.
         
         :param request: The request object
@@ -107,21 +121,31 @@
         """
        
         return ProcessToken.anonymous(self)
         
     def validateframework(self,framework):
         if framework == None:
             raise ValueError("framework not define")
-        elif framework not in _framework:
-            raise ValueError(f"framework support",_framework)
+        elif framework not in __framework__:
+            raise ValueError(f"framework support",__framework__)
     def validateexpirytoken(self,expiry_token):
         if expiry_token == None:
             raise ValueError("add token expire date")
         elif expiry_token <= 0:
             raise ValueError("0 expiry_token not valid")
+    def validatealgorithm(self,algorithm):
+        if algorithm == None:
+            raise ValueError("algorithm not define")
+        elif algorithm not in __algorithm__:
+            raise ValueError("support algorithm",__algorithm__)
+    def installframework(self,framework):
+        try:
+            pkg_resources.get_distribution(framework)
+        except:
+            raise ModuleNotFoundError(framework)
 
 
 class ProcessToken(JWTToken):
     def _create_token(self,request):
         return Json.encode(self,request)
     
     def get_data(self):
@@ -209,21 +233,22 @@
             return jwt.decode(token, self.secret_key, algorithms=self.algorithm)
         except Exception as e:
             raise ValueError(e)
 
 
 
 
-
 class GenerateKey:
     """
-    The GenerateKey class contains a method to generate a Fernet key.
+    The GenerateKey class contains a method to generate key
     """
     def generate_key():
-        return Fernet.generate_key()
+        key = str(Fernet.generate_key())
+        _key = key.replace("'", "")
+        return _key[1:]
 
 
 
 class MetaData:
     def __init__(self,request,framework=None):
         
         """
@@ -328,21 +353,21 @@
     def encode(self):
         self.dublication()
         self.today = datetime.datetime.now()
         self.data.update({
                 "created_date": str(self.today),
             })
         try:
-            return jwt.encode(self.data, self.api_secret_key, algorithm="HS512")
+            return jwt.encode(self.data, self.api_secret_key, algorithm=self.algorithm)
         except Exception as e:
             raise ValueError(e)
 
     def decode(self):
         try:
-            return jwt.decode(self.apikey, self.api_secret_key, algorithms="HS512")
+            return jwt.decode(self.apikey, self.api_secret_key, algorithms=self.algorithm)
         except Exception as e:
             raise ValueError(e)
 
     def data_list(self):
         if len(self.args) != 0:
             self.dataList = []
             self.values = self.decode()
```

### Comparing `webraft-0.1/webraft/ipinfo.py` & `webraft-0.2/webraft/ipinfo.py`

 * *Files identical despite different names*

### Comparing `webraft-0.1/webraft.egg-info/PKG-INFO` & `webraft-0.2/webraft.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: webraft
-Version: 0.1
-Summary: WebRaft is a Python library for creating and reading JSON Web Tokens, extracting user agent information, retrieving IP data, and creating and reading API keys.
+Version: 0.2
+Summary: WebRaft for python web developers
 Home-page: UNKNOWN
 Author: Momin Iqbal (Pakistan Dedov)
 Author-email: <mominiqbal1214@gmail.com>
 License: UNKNOWN
 Description: 
-            # WebRaft
+        # WebRaft
         
-            creating and reading JSON Web Tokens, extracting user agent
-            information, retrieving IP data, and creating and reading API keys
+        WebRaft for python web developers to creating and reading JSON Web Tokens, extracting user agent information (like os,device,browser), retrieving IP data, and creating and reading API keys.
         
-            # How to install webraft
+        # How to install webraft
         
-            ```python
-            pip install webraft
-            ```
-            # Documentation
-            open Github repository for the WebRaft Python library. The link is included in the package's documentation to provide
-            users with access to the source code and additional information about the library.
-            <br>
-            https://github.com/MominIqbal-1234/webraft
+        ```python
+        pip install webraft
+        ```
+        # Documentation
+        open Github repository for the WebRaft Python library. The link is included in the package's documentation to provide
+        users with access to the source code and additional information about the library.
+        <br>
+        Githib : https://github.com/MominIqbal-1234/webraft
+        <br>
+        Documentation : https://webraft.mefiz.com
         
         
-        
-            Check Our Site : https://mefiz.com/about </br>
-            Developed by : Momin Iqbal
+        Check Our Site : https://mefiz.com/about </br>
+        Developed by : Momin Iqbal
         
             
 Keywords: webraft,WebRaftpython,django,jwt,jwt for django,create api key,read api key,create token,read token,user agent django,ip info python,user agent python,jwt flask,jwt bottle,jwt fastapi
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

