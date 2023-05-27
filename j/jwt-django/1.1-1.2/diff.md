# Comparing `tmp/jwt_django-1.1.tar.gz` & `tmp/jwt_django-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jwt_django-1.1.tar", last modified: Thu Feb 23 18:29:02 2023, max compression
+gzip compressed data, was "jwt_django-1.2.tar", last modified: Sat May 27 21:05:03 2023, max compression
```

## Comparing `jwt_django-1.1.tar` & `jwt_django-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-23 18:29:02.000000 jwt_django-1.1/
--rw-rw-rw-   0        0        0     3026 2023-02-23 18:29:02.000000 jwt_django-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2345 2023-02-18 19:35:31.000000 jwt_django-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-23 18:29:02.000000 jwt_django-1.1/jwt_django/
--rw-rw-rw-   0        0        0        0 2023-02-08 08:33:44.000000 jwt_django-1.1/jwt_django/__init__.py
--rw-rw-rw-   0        0        0     5178 2023-02-23 17:28:36.000000 jwt_django-1.1/jwt_django/core.py
--rw-rw-rw-   0        0        0    24576 2023-02-16 17:12:29.000000 jwt_django-1.1/jwt_django/ktoken.cp37-win32.pyd
-drwxrwxrwx   0        0        0        0 2023-02-23 18:29:02.000000 jwt_django-1.1/jwt_django.egg-info/
--rw-rw-rw-   0        0        0     3026 2023-02-23 18:29:01.000000 jwt_django-1.1/jwt_django.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-02-23 18:29:02.000000 jwt_django-1.1/jwt_django.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-23 18:29:01.000000 jwt_django-1.1/jwt_django.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-02-23 18:29:01.000000 jwt_django-1.1/jwt_django.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-02-23 18:29:01.000000 jwt_django-1.1/jwt_django.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-23 18:29:02.000000 jwt_django-1.1/setup.cfg
--rw-rw-rw-   0        0        0     3399 2023-02-23 18:28:43.000000 jwt_django-1.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 21:05:03.186958 jwt_django-1.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      948 2023-05-27 21:05:03.186958 jwt_django-1.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      348 2023-05-27 20:59:22.000000 jwt_django-1.2/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 21:05:03.186958 jwt_django-1.2/jwt_django/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-27 20:59:50.000000 jwt_django-1.2/jwt_django/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4988 2023-05-27 20:59:22.000000 jwt_django-1.2/jwt_django/core.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24576 2023-05-27 20:59:22.000000 jwt_django-1.2/jwt_django/ktoken.cp37-win32.pyd
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 21:05:03.186958 jwt_django-1.2/jwt_django.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      948 2023-05-27 21:05:03.000000 jwt_django-1.2/jwt_django.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      262 2023-05-27 21:05:03.000000 jwt_django-1.2/jwt_django.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-27 21:05:03.000000 jwt_django-1.2/jwt_django.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       33 2023-05-27 21:05:03.000000 jwt_django-1.2/jwt_django.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       11 2023-05-27 21:05:03.000000 jwt_django-1.2/jwt_django.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-27 21:05:03.186958 jwt_django-1.2/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1307 2023-05-27 21:04:09.000000 jwt_django-1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jwt_django-1.1/jwt_django/core.py` & `jwt_django-1.2/jwt_django/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,179 +1,179 @@
-import jwt
-import datetime
-from .ktoken import name
-from cryptography.fernet import Fernet
-
-
-__name__ = "jwt_django"
-__verion__ = "1.0"
-
-"""
-
-
-This project developed by Momin Iqbal
-Support : mefiz.com
-================================================================================================================
-jwt_django:
-
-jwt_django is very useful package for django developers to create, read, authenticate jwt token.
-jwt_django provide end-to-end control jwt token
-
-----------------------------------------------------------------------------------------------------------------
-
-Check Our Site : https://mefiz.com
-
-
-"""
-
-
-class JWTToken:
-    def __init__(
-        self, secret_key=None,
-        expiry_token=None
-    ):
-
-        self.secret_key = secret_key
-        self.expiry_token = int(expiry_token)
-        self.today = datetime.datetime.now()
-
-        if self.expiry_token <= 0:
-            raise ValueError("0 expiry_token token not valid")
-
-    def createToken(self, data):
-        self.data = data
-        """
-        return Token
-        """
-        return ProcessToken.cToken(self)
-
-    def tokenInfo(self, request, *userinfo):
-        self.request = request
-        self.userinfo = userinfo
-        """
-        return token info
-        """
-        if self.is_authenticated() == False:
-            return {"invaild-token": "token expire"}
-        try:
-            return ProcessToken.uInfo(self)
-        except KeyError as e:
-            raise KeyError(f"invalid key {e}")
-
-    def authuser(self, request, *args):
-        self.request = request
-        self.args = args
-
-        """
-        return username and user_id
-        """
-        if self.is_authenticated() == False:
-            return {"invaild-token": "token expire"}
-        try:
-            return ProcessToken.auser(self)
-        except KeyError as e:
-            raise KeyError(f"invalid key {e}")
-
-    def is_authenticated(self):
-        """
-        return Boolean
-        """
-        return ProcessToken.CheckUser(self)
-
-    def isAuthenticated(self, request):
-        self.request = request
-        """
-        return Boolean
-        """
-        return ProcessToken.CheckUser(self)
-
-    def passToken(self, token):
-        self.authDataList = []
-        self.authTokenInfo = PToken.decode(self, token)
-        for i in self.args:
-            self.authDataList.append(self.authTokenInfo.get(i))
-        return self.authDataList
-
-    def passTokenUserInfo(self, token):
-        self.userInfoDataList = []
-        self.userInfo = PToken.decode(self, token)
-        for i in self.userinfo:
-            self.userInfoDataList.append(self.userInfo.get(i))
-        return self.userInfoDataList
-
-
-class ProcessToken(JWTToken):
-    def cToken(self):
-        return PToken.encode(self)
-
-    def uInfo(self):
-        try:
-            return self.passTokenUserInfo(
-                self.request.headers["cache-control"])
-        except ValueError:
-            raise ValueError("cache-control header not exist")
-
-    def auser(self):
-        try:
-            return self.passToken(self.request.headers["authorization"])
-        except ValueError:
-            raise ValueError("authorization header not exist")
-
-    def expiryInfo(self):
-        try:
-            return PToken.decode(self, self.request.headers["authorization"])
-        except ValueError:
-            raise ValueError("authorization header not exist")
-
-    def compareDate(self):
-
-        self.date = ProcessToken.expiryInfo(self)
-        self.expirydate = self.date.get("expiry_date")
-        self.todaydate = str(self.today)[2:]
-
-        self.expirydate = str(self.expirydate)[:8]
-        self.todaydate = str(self.todaydate)[:8]
-
-        self._expirydate = datetime.datetime.strptime(
-            f"{self.expirydate}", "%y-%m-%d")
-        self._todaydate = datetime.datetime.strptime(
-            f"{self.todaydate}", "%y-%m-%d")
-        if self._expirydate > self._todaydate:
-            return True
-        elif self._expirydate < self._todaydate:
-            return False
-        else:
-            return True
-
-    def CheckUser(self):
-        return ProcessToken.compareDate(self)
-
-
-class PToken:
-    def encode(self):
-        PToken.expiry(self)
-        self.expire_date = self.today + \
-            datetime.timedelta(days=self.expiry_token)
-        self.data.update({
-            "expiry_date": str(self.expire_date)[2:],
-        })
-        return jwt.encode(self.data, self.secret_key, algorithm=name.name())
-
-    def decode(self, token):
-        try:
-            return jwt.decode(token, self.secret_key, algorithms=name.name())
-        except Exception as e:
-            print(e)
-
-    def expiry(self):
-        self.check = list(self.data)
-        self.value = [(i) for i in self.check if "expiry_date" == i]
-
-        if self.value == []:
-            return True
-        if self.value[0] == "expiry_date":
-            raise ValueError("expiry_date already exist")
-
-
-class GenerateKey:
-    def generate_key():
-        return Fernet.generate_key()
+import jwt
+import datetime
+from .ktoken import name
+from cryptography.fernet import Fernet
+
+
+
+__name__ = "jwt_django"
+__verion__ = "1.0"
+
+"""
+
+
+This project developed by Momin Iqbal 
+Support : mefiz.com
+================================================================================================================
+jwt_django: 
+
+jwt_django is very useful package for django developers to create, read, authenticate jwt token.
+jwt_django provide end-to-end control jwt token
+
+----------------------------------------------------------------------------------------------------------------
+
+Check Our Site : https://mefiz.com
+
+
+"""
+
+
+class JWTToken:
+    def __init__(
+        self,secret_key=None,
+        expiry_token=None
+        ):
+
+        self.secret_key = secret_key
+        self.expiry_token = int(expiry_token)
+        self.today = datetime.datetime.now()
+
+        if self.expiry_token <= 0:
+            raise ValueError("0 expiry_token token not valid")
+
+    def createToken(self,data):
+        self.data = data
+        """
+        return Token
+        """
+        return ProcessToken.cToken(self)
+       
+
+    def tokenInfo(self,request,*userinfo):
+        self.request = request
+        self.userinfo = userinfo
+        """
+        return token info
+        """
+        if self.is_authenticated() == False:
+            return {"invaild-token":"token expire"}
+        try:
+                return ProcessToken.uInfo(self)
+        except KeyError as e:
+            raise KeyError(f"invalid key {e}")
+
+
+    def authuser(self,request,*args):
+        self.request = request
+        self.args = args
+     
+        """
+        return username and user_id
+        """
+        if self.is_authenticated() == False:
+            return {"invaild-token":"token expire"}
+        try:
+            return ProcessToken.auser(self)
+        except KeyError as e:
+            raise KeyError(f"invalid key {e}")
+
+    def is_authenticated(self):
+        """
+        return Boolean
+        """
+        return ProcessToken.CheckUser(self)
+
+    def isAuthenticated(self,request):
+        self.request = request
+        """
+        return Boolean
+        """
+        return ProcessToken.CheckUser(self)
+
+    def passToken(self,token):
+        self.authDataList = []
+        self.authTokenInfo = PToken.decode(self,token)
+        for i in self.args:
+            self.authDataList.append(self.authTokenInfo.get(i))
+        return self.authDataList
+
+    def passTokenUserInfo(self,token):
+        self.userInfoDataList = []
+        self.userInfo = PToken.decode(self,token)
+        for i in self.userinfo:
+            self.userInfoDataList.append(self.userInfo.get(i))
+        return self.userInfoDataList
+
+
+
+class ProcessToken(JWTToken):
+    def cToken(self):
+        return PToken.encode(self)
+
+    def uInfo(self):
+        try:
+            return self.passTokenUserInfo(self.request.headers["cache-control"]) 
+        except ValueError:
+            raise ValueError("cache-control header not exist")
+            
+    def auser(self):
+        try:
+            return self.passToken(self.request.headers["authorization"]) 
+        except ValueError:
+            raise ValueError("authorization header not exist")
+
+
+    def expiryInfo(self):
+        try:
+            return PToken.decode(self,self.request.headers["authorization"])
+        except ValueError:
+            raise ValueError("authorization header not exist")
+
+    def compareDate(self):
+        
+        self.date = ProcessToken.expiryInfo(self)
+        self.expirydate = self.date.get("expiry_date")
+        self.todaydate = str(self.today)[2:]
+ 
+        self.expirydate = str(self.expirydate)[:8]
+        self.todaydate = str(self.todaydate)[:8]
+
+        self._expirydate = datetime.datetime.strptime(f"{self.expirydate}", "%y-%m-%d")
+        self._todaydate = datetime.datetime.strptime(f"{self.todaydate}", "%y-%m-%d")
+        if self._expirydate > self._todaydate:
+            return True
+        elif self._expirydate < self._todaydate:
+            return False
+        else:
+            return True
+        
+
+    def CheckUser(self):
+        return ProcessToken.compareDate(self)
+
+class PToken:
+    def encode(self):
+        PToken.expiry(self)
+        self.expire_date = self.today + datetime.timedelta(days=self.expiry_token)
+        self.data.update({
+            "expiry_date":str(self.expire_date)[2:],
+        })
+        return jwt.encode(self.data,self.secret_key,algorithm=name.name()) 
+
+    def decode(self,token):
+        try:
+            return jwt.decode(token,self.secret_key,algorithms=name.name())
+        except Exception as e:
+            print(e)
+    def expiry(self):
+        self.check = list(self.data)
+        self.value = [(i) for i in self.check if "expiry_date" == i]
+        
+        if self.value == []:
+            return True
+        if self.value[0] == "expiry_date":
+            raise ValueError("expiry_date already exist")
+
+
+class GenerateKey:
+    def generate_key():
+        return Fernet.generate_key()
```

