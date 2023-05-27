# Comparing `tmp/OpenAIAuth-1.0.1.tar.gz` & `tmp/OpenAIAuth-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenAIAuth-1.0.1.tar", last modified: Sat May 27 02:10:56 2023, max compression
+gzip compressed data, was "OpenAIAuth-1.0.2.tar", last modified: Sat May 27 02:21:47 2023, max compression
```

## Comparing `OpenAIAuth-1.0.1.tar` & `OpenAIAuth-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:10:56.641596 OpenAIAuth-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-27 02:10:31.000000 OpenAIAuth-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-27 02:10:56.641596 OpenAIAuth-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-27 02:10:31.000000 OpenAIAuth-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 02:10:56.641596 OpenAIAuth-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-27 02:10:31.000000 OpenAIAuth-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:10:56.641596 OpenAIAuth-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:10:56.641596 OpenAIAuth-1.0.1/src/OpenAIAuth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-27 02:10:56.000000 OpenAIAuth-1.0.1/src/OpenAIAuth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-27 02:10:56.000000 OpenAIAuth-1.0.1/src/OpenAIAuth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 02:10:56.000000 OpenAIAuth-1.0.1/src/OpenAIAuth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-27 02:10:56.000000 OpenAIAuth-1.0.1/src/OpenAIAuth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-27 02:10:56.000000 OpenAIAuth-1.0.1/src/OpenAIAuth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-05-27 02:10:31.000000 OpenAIAuth-1.0.1/src/OpenAIAuth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:21:47.687727 OpenAIAuth-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-27 02:21:22.000000 OpenAIAuth-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-27 02:21:47.687727 OpenAIAuth-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-27 02:21:22.000000 OpenAIAuth-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 02:21:47.687727 OpenAIAuth-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-27 02:21:22.000000 OpenAIAuth-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:21:47.687727 OpenAIAuth-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:21:47.687727 OpenAIAuth-1.0.2/src/OpenAIAuth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-27 02:21:47.000000 OpenAIAuth-1.0.2/src/OpenAIAuth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-27 02:21:47.000000 OpenAIAuth-1.0.2/src/OpenAIAuth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 02:21:47.000000 OpenAIAuth-1.0.2/src/OpenAIAuth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-27 02:21:47.000000 OpenAIAuth-1.0.2/src/OpenAIAuth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-27 02:21:47.000000 OpenAIAuth-1.0.2/src/OpenAIAuth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-05-27 02:21:22.000000 OpenAIAuth-1.0.2/src/OpenAIAuth.py
```

### Comparing `OpenAIAuth-1.0.1/LICENSE` & `OpenAIAuth-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenAIAuth-1.0.1/PKG-INFO` & `OpenAIAuth-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenAIAuth
-Version: 1.0.1
+Version: 1.0.2
 Summary: OpenAI Authentication Reverse Engineered
 Home-page: https://github.com/acheong08/OpenAIAuth
 Author: pengzhile
 Author-email: acheong@student.dalat.org
 License: MIT
 Project-URL: Bug Report, https://github.com/acheong08/OpenAIAuth/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OpenAIAuth-1.0.1/README.md` & `OpenAIAuth-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `OpenAIAuth-1.0.1/setup.py` & `OpenAIAuth-1.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="OpenAIAuth",
-    version="1.0.1",
+    version="1.0.2",
     license="MIT",
     author="pengzhile",
     author_email="acheong@student.dalat.org",
     description="OpenAI Authentication Reverse Engineered",
     packages=find_packages("src"),
     package_dir={"": "src"},
     py_modules=["OpenAIAuth"],
```

### Comparing `OpenAIAuth-1.0.1/src/OpenAIAuth.egg-info/PKG-INFO` & `OpenAIAuth-1.0.2/src/OpenAIAuth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenAIAuth
-Version: 1.0.1
+Version: 1.0.2
 Summary: OpenAI Authentication Reverse Engineered
 Home-page: https://github.com/acheong08/OpenAIAuth
 Author: pengzhile
 Author-email: acheong@student.dalat.org
 License: MIT
 Project-URL: Bug Report, https://github.com/acheong08/OpenAIAuth/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OpenAIAuth-1.0.1/src/OpenAIAuth.py` & `OpenAIAuth-1.0.2/src/OpenAIAuth.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,34 +38,33 @@
         }
         self.access_token = None
         self.expires = None
         self.user_agent = (
             "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) "
             "Chrome/109.0.0.0 Safari/537.36"
         )
-        self.api_prefix = getenv("CHATGPT_API_PREFIX", "https://ai.fakeopen.com")
 
     @staticmethod
     def __check_email(email: str):
         regex = r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b"
         return re.fullmatch(regex, email)
 
-    def auth(self, login_local=True) -> str:
+    def auth(self) -> str:
         if (
             self.use_cache
             and self.access_token
             and self.expires
             and self.expires > dt.now()
         ):
             return self.access_token
 
         if not self.__check_email(self.email) or not self.password:
             raise Exception("invalid email or password.")
 
-        return self.__part_two() if login_local else self.get_access_token_proxy()
+        return self.__part_two()
 
     def __part_two(self) -> str:
         code_challenge = "w6n3Ix420Xhhu-Q5-mOOEyuPZmAsJHUbBpO8Ub7xBCY"
         code_verifier = "yGrXROHx_VazA0uovsxKfE263LMFcrSrdm4SlC-rob8"
 
         url = (
             "https://auth0.openai.com/authorize?client_id=pdlLIX2Y72MIl2rhLhTE9VV9bN905kBh&audience=https%3A%2F"
@@ -243,37 +242,7 @@
                 dt.utcnow()
                 + datetime.timedelta(seconds=json["expires_in"])
                 - datetime.timedelta(minutes=5)
             )
             return self.access_token
         else:
             raise Exception(resp.text)
-
-    def get_access_token_proxy(self) -> str:
-        url = "{}/api/auth/login".format(self.api_prefix)
-        headers = {
-            "User-Agent": self.user_agent,
-        }
-        data = {
-            "username": self.email,
-            "password": self.password,
-        }
-        resp = self.session.post(
-            url=url,
-            headers=headers,
-            data=data,
-            allow_redirects=False,
-            **self.req_kwargs
-        )
-
-        if resp.status_code == 200:
-            json = resp.json()
-            if "accessToken" not in json:
-                raise Exception("Get access token failed.")
-
-            self.access_token = json["accessToken"]
-            self.expires = dt.strptime(
-                json["expires"], "%Y-%m-%dT%H:%M:%S.%fZ"
-            ) - datetime.timedelta(minutes=5)
-            return self.access_token
-        else:
-            raise Exception("Error get access token.")
```

