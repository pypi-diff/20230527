# Comparing `tmp/discord-oauth2.py-1.2.0.tar.gz` & `tmp/discord-oauth2.py-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-oauth2.py-1.2.0.tar", last modified: Tue May 23 13:21:14 2023, max compression
+gzip compressed data, was "discord-oauth2.py-1.2.1.tar", last modified: Sat May 27 09:00:53 2023, max compression
```

## Comparing `discord-oauth2.py-1.2.0.tar` & `discord-oauth2.py-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:21:14.158206 discord-oauth2.py-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 13:21:03.000000 discord-oauth2.py-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-23 13:21:14.158206 discord-oauth2.py-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-23 13:21:03.000000 discord-oauth2.py-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:21:14.158206 discord-oauth2.py-1.2.0/discord_oauth2.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-23 13:21:14.000000 discord-oauth2.py-1.2.0/discord_oauth2.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-23 13:21:14.000000 discord-oauth2.py-1.2.0/discord_oauth2.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:21:14.000000 discord-oauth2.py-1.2.0/discord_oauth2.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 13:21:14.000000 discord-oauth2.py-1.2.0/discord_oauth2.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 13:21:14.000000 discord-oauth2.py-1.2.0/discord_oauth2.py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:21:14.158206 discord-oauth2.py-1.2.0/discordoauth2/
--rw-r--r--   0 runner    (1001) docker     (123)    17451 2023-05-23 13:21:03.000000 discord-oauth2.py-1.2.0/discordoauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:21:14.158206 discord-oauth2.py-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-23 13:21:03.000000 discord-oauth2.py-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:00:53.140377 discord-oauth2.py-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-27 09:00:42.000000 discord-oauth2.py-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-27 09:00:53.140377 discord-oauth2.py-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-27 09:00:42.000000 discord-oauth2.py-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:00:53.140377 discord-oauth2.py-1.2.1/discord_oauth2.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-27 09:00:53.000000 discord-oauth2.py-1.2.1/discord_oauth2.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-27 09:00:53.000000 discord-oauth2.py-1.2.1/discord_oauth2.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 09:00:53.000000 discord-oauth2.py-1.2.1/discord_oauth2.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-27 09:00:53.000000 discord-oauth2.py-1.2.1/discord_oauth2.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-27 09:00:53.000000 discord-oauth2.py-1.2.1/discord_oauth2.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:00:53.140377 discord-oauth2.py-1.2.1/discordoauth2/
+-rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-05-27 09:00:42.000000 discord-oauth2.py-1.2.1/discordoauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 09:00:53.140377 discord-oauth2.py-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-27 09:00:42.000000 discord-oauth2.py-1.2.1/setup.py
```

### Comparing `discord-oauth2.py-1.2.0/LICENSE` & `discord-oauth2.py-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-oauth2.py-1.2.0/PKG-INFO` & `discord-oauth2.py-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-oauth2.py
-Version: 1.2.0
+Version: 1.2.1
 Summary: Use Discord's OAuth2 effortlessly! Turns the auth code to a access token and the access token into scope infomation. 
 Home-page: https://github.com/TreeBen77/discordoauth2
 Author: TreeBen77
 License: MIT
 Keywords: flask,oauth2,discord,discord-api
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `discord-oauth2.py-1.2.0/README.md` & `discord-oauth2.py-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `discord-oauth2.py-1.2.0/discord_oauth2.py.egg-info/PKG-INFO` & `discord-oauth2.py-1.2.1/discord_oauth2.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-oauth2.py
-Version: 1.2.0
+Version: 1.2.1
 Summary: Use Discord's OAuth2 effortlessly! Turns the auth code to a access token and the access token into scope infomation. 
 Home-page: https://github.com/TreeBen77/discordoauth2
 Author: TreeBen77
 License: MIT
 Keywords: flask,oauth2,discord,discord-api
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `discord-oauth2.py-1.2.0/discordoauth2/__init__.py` & `discord-oauth2.py-1.2.1/discordoauth2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,29 +252,31 @@
         if response.ok:
             return
         elif response.status_code == 401: raise exceptions.Forbidden(f"this AccessToken does not have the nessasary scope.")
         elif response.status_code == 429: raise exceptions.RateLimited(f"You are being Rate Limited. Retry after: {response.json()['retry_after']}", retry_after=response.json()['retry_after'])
         else:
             raise exceptions.HTTPException(f"Unexpected HTTP {response.status_code}")
     
-    def generate_uri(self, scope: Union[str, list[str]], state: Optional[str]=None, response_type: Literal["code", "token"]="code", guild_id=None, disable_guild_select=None, permissions=None) -> str:
+    def generate_uri(self, scope: Union[str, list[str]], state: Optional[str]=None, skip_prompt: Optional[bool]=False, response_type: Optional[Literal["code", "token"]]="code", guild_id: Optional[Union[int, str]]=None, disable_guild_select: Optional[bool]=None, permissions: Optional[Union[int, str]]=None) -> str:
         """Creates an authorization uri with client information prefilled.
         
         scope: a string, or list of strings for the scope
         state: optional state parameter. Optional but recommended.
+        skip_prompt: doesn't require the end user to reauthorize if they've already authorized you app before. Defaults to `False`.
         response_type: either code, or token. token means the server can't access it, but the client can use it without converting.
         guild_id: the guild ID to add a bot/webhook.
         disable_guild_select: wether to allow the authorizing user to change the selected guild
         permissions: the permission bitwise integer for the bot being added.
         """
         params = {
             "client_id": self.id,
             "scope": " ".join(scope) if type(scope) == list else scope,
             "state": state,
             "redirect_uri": self.redirect_url,
+            "prompt": "none" if skip_prompt else None,
             "response_type": response_type,
             "guild_id": guild_id,
             "disable_guild_select": disable_guild_select,
             "permissions": permissions
         }
         return f"https://discord.com/oauth2/authorize?{parse.urlencode({key: value for key, value in params.items() if value is not None})}"
```

### Comparing `discord-oauth2.py-1.2.0/setup.py` & `discord-oauth2.py-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setup(
     name='discord-oauth2.py',
     description='Use Discord\'s OAuth2 effortlessly! Turns the auth code to a access token and the access token into scope infomation. ',
-    version="1.2.0",
+    version="1.2.1",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     python_requires='>=3.8',
     author="TreeBen77",
     packages=[
         'discordoauth2'
```

