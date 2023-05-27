# Comparing `tmp/ossapi-3.1.9.tar.gz` & `tmp/ossapi-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ossapi-3.1.9.tar", last modified: Sun Apr  9 00:25:59 2023, max compression
+gzip compressed data, was "ossapi-3.2.0.tar", last modified: Sat May 27 00:17:15 2023, max compression
```

## Comparing `ossapi-3.1.9.tar` & `ossapi-3.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-09 00:25:59.765352 ossapi-3.1.9/
--rw-r--r--   0 tybug      (501) staff       (20)    34523 2023-01-30 05:20:33.000000 ossapi-3.1.9/LICENSE
--rw-r--r--   0 tybug      (501) staff       (20)    10020 2023-04-09 00:25:59.765113 ossapi-3.1.9/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)     9513 2023-03-28 20:31:37.000000 ossapi-3.1.9/README.md
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-09 00:25:59.761620 ossapi-3.1.9/ossapi/
--rw-r--r--   0 tybug      (501) staff       (20)     3864 2023-03-09 02:19:38.000000 ossapi-3.1.9/ossapi/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)      925 2023-03-31 23:04:14.000000 ossapi-3.1.9/ossapi/encoder.py
--rw-r--r--   0 tybug      (501) staff       (20)    16948 2023-04-06 05:02:02.000000 ossapi-3.1.9/ossapi/enums.py
--rw-r--r--   0 tybug      (501) staff       (20)    11982 2023-01-31 22:30:17.000000 ossapi-3.1.9/ossapi/mod.py
--rw-r--r--   0 tybug      (501) staff       (20)    36025 2023-03-09 05:37:37.000000 ossapi-3.1.9/ossapi/models.py
--rw-r--r--   0 tybug      (501) staff       (20)    14955 2023-02-01 05:09:38.000000 ossapi-3.1.9/ossapi/ossapi.py
--rw-r--r--   0 tybug      (501) staff       (20)    84207 2023-04-09 00:25:54.000000 ossapi-3.1.9/ossapi/ossapiv2.py
--rw-r--r--   0 tybug      (501) staff       (20)    89585 2023-04-09 00:25:54.000000 ossapi-3.1.9/ossapi/ossapiv2_async.py
--rw-r--r--   0 tybug      (501) staff       (20)     2639 2023-03-08 17:51:25.000000 ossapi-3.1.9/ossapi/replay.py
--rw-r--r--   0 tybug      (501) staff       (20)     8707 2023-01-30 00:39:41.000000 ossapi-3.1.9/ossapi/utils.py
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-09 00:25:59.762825 ossapi-3.1.9/ossapi.egg-info/
--rw-r--r--   0 tybug      (501) staff       (20)    10020 2023-04-09 00:25:59.000000 ossapi-3.1.9/ossapi.egg-info/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)      460 2023-04-09 00:25:59.000000 ossapi-3.1.9/ossapi.egg-info/SOURCES.txt
--rw-r--r--   0 tybug      (501) staff       (20)        1 2023-04-09 00:25:59.000000 ossapi-3.1.9/ossapi.egg-info/dependency_links.txt
--rw-r--r--   0 tybug      (501) staff       (20)       71 2023-04-09 00:25:59.000000 ossapi-3.1.9/ossapi.egg-info/requires.txt
--rw-r--r--   0 tybug      (501) staff       (20)        7 2023-04-09 00:25:59.000000 ossapi-3.1.9/ossapi.egg-info/top_level.txt
--rw-r--r--   0 tybug      (501) staff       (20)      644 2023-04-09 00:25:40.000000 ossapi-3.1.9/pyproject.toml
--rw-r--r--   0 tybug      (501) staff       (20)       38 2023-04-09 00:25:59.765426 ossapi-3.1.9/setup.cfg
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-09 00:25:59.764727 ossapi-3.1.9/tests/
--rw-r--r--   0 tybug      (501) staff       (20)     3082 2023-04-09 00:25:54.000000 ossapi-3.1.9/tests/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)      523 2023-01-28 21:17:50.000000 ossapi-3.1.9/tests/test_cursor.py
--rw-r--r--   0 tybug      (501) staff       (20)     9694 2023-03-09 05:36:41.000000 ossapi-3.1.9/tests/test_endpoints.py
--rw-r--r--   0 tybug      (501) staff       (20)     4040 2023-04-09 00:25:54.000000 ossapi-3.1.9/tests/test_models.py
--rw-r--r--   0 tybug      (501) staff       (20)     1137 2023-01-28 21:17:50.000000 ossapi-3.1.9/tests/test_v1.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-05-27 00:17:15.039376 ossapi-3.2.0/
+-rw-r--r--   0 tybug      (501) staff       (20)    34523 2023-01-30 05:20:33.000000 ossapi-3.2.0/LICENSE
+-rw-r--r--   0 tybug      (501) staff       (20)    10020 2023-05-27 00:17:15.039150 ossapi-3.2.0/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)     9513 2023-05-27 00:03:28.000000 ossapi-3.2.0/README.md
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-05-27 00:17:15.037145 ossapi-3.2.0/ossapi/
+-rw-r--r--   0 tybug      (501) staff       (20)     3882 2023-05-27 00:03:28.000000 ossapi-3.2.0/ossapi/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)      925 2023-04-18 20:48:24.000000 ossapi-3.2.0/ossapi/encoder.py
+-rw-r--r--   0 tybug      (501) staff       (20)    16948 2023-04-18 20:48:22.000000 ossapi-3.2.0/ossapi/enums.py
+-rw-r--r--   0 tybug      (501) staff       (20)    11982 2023-04-18 20:48:16.000000 ossapi-3.2.0/ossapi/mod.py
+-rw-r--r--   0 tybug      (501) staff       (20)    36025 2023-05-27 00:03:28.000000 ossapi-3.2.0/ossapi/models.py
+-rw-r--r--   0 tybug      (501) staff       (20)    14955 2023-04-29 22:39:56.000000 ossapi-3.2.0/ossapi/ossapi.py
+-rw-r--r--   0 tybug      (501) staff       (20)    87037 2023-05-27 00:14:44.000000 ossapi-3.2.0/ossapi/ossapiv2.py
+-rw-r--r--   0 tybug      (501) staff       (20)    89789 2023-05-27 00:03:28.000000 ossapi-3.2.0/ossapi/ossapiv2_async.py
+-rw-r--r--   0 tybug      (501) staff       (20)     2639 2023-04-18 20:48:42.000000 ossapi-3.2.0/ossapi/replay.py
+-rw-r--r--   0 tybug      (501) staff       (20)     8707 2023-04-29 20:32:03.000000 ossapi-3.2.0/ossapi/utils.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-05-27 00:17:15.037961 ossapi-3.2.0/ossapi.egg-info/
+-rw-r--r--   0 tybug      (501) staff       (20)    10020 2023-05-27 00:17:15.000000 ossapi-3.2.0/ossapi.egg-info/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)      460 2023-05-27 00:17:15.000000 ossapi-3.2.0/ossapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        1 2023-05-27 00:17:15.000000 ossapi-3.2.0/ossapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tybug      (501) staff       (20)       71 2023-05-27 00:17:15.000000 ossapi-3.2.0/ossapi.egg-info/requires.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        7 2023-05-27 00:17:15.000000 ossapi-3.2.0/ossapi.egg-info/top_level.txt
+-rw-r--r--   0 tybug      (501) staff       (20)      644 2023-05-27 00:14:54.000000 ossapi-3.2.0/pyproject.toml
+-rw-r--r--   0 tybug      (501) staff       (20)       38 2023-05-27 00:17:15.039418 ossapi-3.2.0/setup.cfg
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-05-27 00:17:15.038892 ossapi-3.2.0/tests/
+-rw-r--r--   0 tybug      (501) staff       (20)     3080 2023-05-27 00:03:28.000000 ossapi-3.2.0/tests/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)      523 2023-01-28 21:17:50.000000 ossapi-3.2.0/tests/test_cursor.py
+-rw-r--r--   0 tybug      (501) staff       (20)    10591 2023-05-27 00:03:28.000000 ossapi-3.2.0/tests/test_endpoints.py
+-rw-r--r--   0 tybug      (501) staff       (20)     4040 2023-04-29 20:32:03.000000 ossapi-3.2.0/tests/test_models.py
+-rw-r--r--   0 tybug      (501) staff       (20)     1137 2023-01-28 21:17:50.000000 ossapi-3.2.0/tests/test_v1.py
```

### Comparing `ossapi-3.1.9/LICENSE` & `ossapi-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.9/PKG-INFO` & `ossapi-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossapi
-Version: 3.1.9
+Version: 3.2.0
 Summary: Complete python wrapper for osu! api v2 and v1.
 Author-email: Liam DeVoe <orionldevoe@gmail.com>
 Project-URL: Homepage, https://github.com/circleguard/ossapi
 Keywords: osu!,wrapper,api,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `ossapi-3.1.9/README.md` & `ossapi-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.9/ossapi/__init__.py` & `ossapi-3.2.0/ossapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # we need to explicitly set a handler for the logging module to be happy
 handler = logging.StreamHandler()
 logging.getLogger("ossapi").addHandler(handler)
 from importlib import metadata
 
 from ossapi.ossapi import (OssapiV1, ReplayUnavailableException,
     InvalidKeyException, APIException)
-from ossapi.ossapiv2 import Ossapi, Grant, Scope
+from ossapi.ossapiv2 import Ossapi, Grant, Scope, Domain
 from ossapi.models import (Beatmap, BeatmapCompact, BeatmapUserScore,
     ForumTopicAndPosts, Search, CommentBundle, Cursor, Score,
     BeatmapsetSearchResult, ModdingHistoryEventsBundle, User, Rankings,
     BeatmapScores, KudosuHistory, Beatmapset, BeatmapPlaycount, Spotlight,
     Spotlights, WikiPage, _Event, Event, BeatmapsetDiscussionPosts, Build,
     ChangelogListing, MultiplayerScores,
     BeatmapsetDiscussionVotes, CreatePMResponse, BeatmapsetDiscussions,
@@ -38,15 +38,15 @@
 __version__ = metadata.version(__package__)
 
 __all__ = [
     # OssapiV1
     "OssapiV1", "ReplayUnavailableException", "InvalidKeyException",
     "APIException",
     # OssapiV2 core
-    "Ossapi", "OssapiAsync", "Grant", "Scope",
+    "Ossapi", "OssapiAsync", "Grant", "Scope", "Domain",
     # OssapiV2 models
     "Beatmap", "BeatmapCompact", "BeatmapUserScore", "ForumTopicAndPosts",
     "Search", "CommentBundle", "Cursor", "Score", "BeatmapsetSearchResult",
     "ModdingHistoryEventsBundle", "User", "Rankings", "BeatmapScores",
     "KudosuHistory", "Beatmapset", "BeatmapPlaycount", "Spotlight",
     "Spotlights", "WikiPage", "_Event", "Event", "BeatmapsetDiscussionPosts",
     "Build", "ChangelogListing", "MultiplayerScores",
```

### Comparing `ossapi-3.1.9/ossapi/encoder.py` & `ossapi-3.2.0/ossapi/encoder.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.9/ossapi/enums.py` & `ossapi-3.2.0/ossapi/enums.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.9/ossapi/mod.py` & `ossapi-3.2.0/ossapi/mod.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.9/ossapi/models.py` & `ossapi-3.2.0/ossapi/models.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.9/ossapi/ossapi.py` & `ossapi-3.2.0/ossapi/ossapi.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.9/ossapi/ossapiv2.py` & `ossapi-3.2.0/ossapi/ossapiv2.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,14 +226,27 @@
     CHAT_WRITE = "chat.write"
     DELEGATE = "delegate"
     FORUM_WRITE = "forum.write"
     FRIENDS_READ = "friends.read"
     IDENTIFY = "identify"
     PUBLIC = "public"
 
+class Domain(Enum):
+    """
+    Different possible api domains. These correspond to different deployments of
+    the osu server: osu.ppy.sh, lazer.ppy.sh, and dev.ppy.sh respectively.
+
+    The default domain, and the one the vast majority of users want, is
+    :data:`Domain.OSU <ossapi.ossapiv2.Domain.OSU>`, and corresponds to the
+    main website. To retrieve information from the lazer website or the dev
+    website, use the corresponding domain.
+    """
+    OSU = "osu"
+    LAZER = "lazer"
+    DEV = "dev"
 
 class Ossapi:
     """
     A wrapper around osu! api v2. The main entry point for ossapi.
 
     Parameters
     ----------
@@ -292,47 +305,67 @@
         :class:`~ossapi.ossapiv2.Ossapi` after manually authenticating with the
         osu! api.
     refresh_token: str
         Refresh token from the osu! api. Allows instantiating
         :class:`~ossapi.ossapiv2.Ossapi` after manually authenticating with the
         osu! api. Optional if using :data:`Grant.CLIENT_CREDENTIALS
         <ossapi.ossapiv2.Grant.CLIENT_CREDENTIALS>`.
+    domain: Domain or str
+        The domain to retrieve information from. This defaults to
+        :data:`Domain.OSU <ossapi.ossapiv2.Domain.OSU>`, which corresponds to
+        osu.ppy.sh, the main website.
+        |br|
+        To retrieve information from lazer.ppy.sh - for instance, the
+        leaderboards on lazer, or a user's best score on lazer - specify
+        :data:`Domain.LAZER <ossapi.ossapiv2.Domain.LAZER>`. To retureve
+        information from dev.ppy.sh, specify
+        :data:`Domain.DEV <ossapi.ossapiv2.Domain.DEV>`.
+        |br|
+        See :doc:`Domains <domains>` for more about domains.
     """
-    TOKEN_URL = "https://osu.ppy.sh/oauth/token"
-    AUTH_CODE_URL = "https://osu.ppy.sh/oauth/authorize"
-    BASE_URL = "https://osu.ppy.sh/api/v2"
+    TOKEN_URL = "https://{domain}.ppy.sh/oauth/token"
+    AUTH_CODE_URL = "https://{domain}.ppy.sh/oauth/authorize"
+    BASE_URL = "https://{domain}.ppy.sh/api/v2"
 
     def __init__(self,
         client_id: int,
         client_secret: str,
         redirect_uri: Optional[str] = None,
         scopes: List[Union[str, Scope]] = [Scope.PUBLIC],
         *,
         grant: Optional[Union[Grant, str]] = None,
         strict: bool = False,
         token_directory: Optional[str] = None,
         token_key: Optional[str] = None,
         access_token: Optional[str] = None,
-        refresh_token: Optional[str] = None
+        refresh_token: Optional[str] = None,
+        domain: Union[str, Domain] = Domain.OSU
     ):
         if not grant:
             grant = (Grant.AUTHORIZATION_CODE if redirect_uri else
                 Grant.CLIENT_CREDENTIALS)
         grant = Grant(grant)
 
+        domain = Domain(domain)
+
+        self.token_url = self.TOKEN_URL.format(domain=domain.value)
+        self.auth_code_url = self.AUTH_CODE_URL.format(domain=domain.value)
+        self.base_url = self.BASE_URL.format(domain=domain.value)
+
         self.grant = grant
         self.client_id = client_id
         self.client_secret = client_secret
         self.redirect_uri = redirect_uri
         self.scopes = [Scope(scope) for scope in scopes]
         self.strict = strict
+        self.domain = domain
 
         self.log = logging.getLogger(__name__)
         self.token_key = token_key or self.gen_token_key(self.grant,
-            self.client_id, self.client_secret, self.scopes)
+            self.client_id, self.client_secret, self.scopes, self.domain.value)
 
         # support saving tokens when being run from pyinstaller
         if hasattr(sys, '_MEIPASS') and not token_directory:
             token_directory = sys._MEIPASS # pylint: disable=no-member
 
         self.token_directory = (
             Path(token_directory) if token_directory else Path(__file__).parent
@@ -359,32 +392,46 @@
                 "refresh_token": refresh_token
             }
             token = OAuth2Token(params)
 
         self.session = self.authenticate(token=token)
 
     @staticmethod
-    def gen_token_key(grant, client_id, client_secret, scopes):
+    def gen_token_key(grant, client_id, client_secret, scopes,
+        domain=Domain.OSU
+    ):
         """
         The unique key / hash for the given set of parameters. This is intended
         to provide a way to allow multiple OssapiV2's to live at the same time,
         by eg saving their tokens to different files based on their key.
 
         This function is also deterministic, to eg allow tokens to be reused if
         OssapiV2 is instantiated twice with the same parameters. This avoids the
         need to reauthenticate unless absolutely necessary.
         """
         grant = Grant(grant)
         scopes = [Scope(scope) for scope in scopes]
+        domain = Domain(domain)
+
         m = hashlib.sha256()
         m.update(grant.value.encode("utf-8"))
         m.update(str(client_id).encode("utf-8"))
         m.update(client_secret.encode("utf-8"))
+
         for scope in scopes:
             m.update(scope.value.encode("utf-8"))
+
+        # for backwards compatability, only hash the domain when it's
+        # non-default. This ensures keys from before and after domains were
+        # introduced coincide.
+        # This intentionally treats Domain.OSU and Domain.LAZER as the same key,
+        # as those domains share account and oauth credentials.
+        if domain is Domain.DEV:
+            m.update(domain.value.encode("utf-8"))
+
         return m.hexdigest()
 
     @staticmethod
     def remove_token(key, token_directory=None):
         """
         Removes the token file associated with the given key. If
         ``token_directory`` is passed, looks there for the token file instead of
@@ -416,15 +463,15 @@
             if self.grant is Grant.AUTHORIZATION_CODE:
                 auto_refresh_kwargs = {
                     "client_id": self.client_id,
                     "client_secret": self.client_secret
                 }
                 return OAuth2Session(self.client_id, token=token,
                     redirect_uri=self.redirect_uri,
-                    auto_refresh_url=self.TOKEN_URL,
+                    auto_refresh_url=self.token_url,
                     auto_refresh_kwargs=auto_refresh_kwargs,
                     token_updater=self._save_token,
                     scope=[scope.value for scope in self.scopes])
 
         if self.grant is Grant.CLIENT_CREDENTIALS:
             return self._new_client_grant(self.client_id, self.client_secret)
 
@@ -434,15 +481,15 @@
     def _new_client_grant(self, client_id, client_secret):
         """
         Authenticates with the api from scratch on the client grant.
         """
         self.log.info("initializing client credentials grant")
         client = BackendApplicationClient(client_id=client_id, scope=["public"])
         session = OAuth2Session(client=client)
-        token = session.fetch_token(token_url=self.TOKEN_URL,
+        token = session.fetch_token(token_url=self.token_url,
             client_id=client_id, client_secret=client_secret)
 
         self._save_token(token)
         return session
 
     def _new_authorization_grant(self, client_id, client_secret, redirect_uri,
         scopes):
@@ -452,21 +499,21 @@
         self.log.info("initializing authorization code")
 
         auto_refresh_kwargs = {
             "client_id": client_id,
             "client_secret": client_secret
         }
         session = OAuth2Session(client_id, redirect_uri=redirect_uri,
-            auto_refresh_url=self.TOKEN_URL,
+            auto_refresh_url=self.token_url,
             auto_refresh_kwargs=auto_refresh_kwargs,
             token_updater=self._save_token,
             scope=[scope.value for scope in scopes])
 
         authorization_url, _state = (
-            session.authorization_url(self.AUTH_CODE_URL)
+            session.authorization_url(self.auth_code_url)
         )
         webbrowser.open(authorization_url)
 
         # open up a temporary socket so we can receive the GET request to the
         # callback url
         port = int(redirect_uri.rsplit(":", 1)[1].split("/")[0])
         serversocket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
@@ -483,15 +530,15 @@
             may now close this tab safely.
             </body></html>
         """)
         connection.close()
         serversocket.close()
 
         code = data.split("code=")[1].split("&state=")[0]
-        token = session.fetch_token(self.TOKEN_URL, client_id=client_id,
+        token = session.fetch_token(self.token_url, client_id=client_id,
             client_secret=client_secret, code=code)
         self._save_token(token)
 
         return session
 
     def _save_token(self, token):
         """
@@ -502,29 +549,29 @@
             pickle.dump(token, f)
 
     def _request(self, type_, method, url, params={}, data={}):
         params = self._format_params(params)
         # also format data for post requests
         data = self._format_params(data)
         try:
-            r = self.session.request(method, f"{self.BASE_URL}{url}",
+            r = self.session.request(method, f"{self.base_url}{url}",
                 params=params, data=data)
         except TokenExpiredError:
             # provide "auto refreshing" for client credentials grant. The client
             # grant doesn't actually provide a refresh token, so we can't hook
             # onto OAuth2Session's auto_refresh functionality like we do for the
             # authorization code grant. But we can do something effectively
             # equivalent: whenever we make a request with an expired client
             # grant token, just request a new one.
             if self.grant is not Grant.CLIENT_CREDENTIALS:
                 raise
             self.session = self._new_client_grant(self.client_id,
                 self.client_secret)
             # redo the request now that we have a valid token
-            r = self.session.request(method, f"{self.BASE_URL}{url}",
+            r = self.session.request(method, f"{self.base_url}{url}",
                 params=params, data=data)
 
         self.log.info(f"made {method} request to {r.request.url}, data {data}")
         json_ = r.json()
         self.log.debug(f"received json: \n{json.dumps(json_, indent=4)}")
         self._check_response(json_, r.url)
 
@@ -534,14 +581,21 @@
         # TODO this should just be `if "error" in json`, but for some reason
         # `self.search_beatmaps` always returns an error in the response...
         # open an issue on osu-web?
         if len(json_) == 1 and "error" in json_:
             raise ValueError(f"api returned an error of `{json_['error']}` for "
                 f"a request to {unquote(url)}")
 
+        # Shouldn't happen in normal usage. Might occur if a client gets revoked
+        # and we still have a local token.pickel saved for it. But I haven't
+        # tested.
+        if json_ == {"authentication": "basic"}:
+            raise ValueError(f"Invalid authentication. json: {json_}, url: "
+                f"{url}")
+
     def _get(self, type_, url, params={}):
         return self._request(type_, "GET", url, params=params)
 
     def _post(self, type_, url, data={}):
         return self._request(type_, "POST", url, data=data)
 
     def _put(self, type_, url, data={}):
@@ -899,36 +953,40 @@
 
     @request(Scope.PUBLIC, category="beatmaps")
     def beatmap_scores(self,
         beatmap_id: BeatmapIdT,
         *,
         mode: Optional[GameModeT] = None,
         mods: Optional[ModT] = None,
-        type: Optional[RankingTypeT] = None
+        type: Optional[RankingTypeT] = None,
+        limit: Optional[int] = None
     ) -> BeatmapScores:
         """
         Get the top scores of a beatmap.
 
         Parameters
         ----------
         beatmap_id
             The beatmap to get scores of.
         mode
             The mode to get scores of.
         mods
             Get the top scores set with exactly these mods, if passed.
         type
             How to order the scores. Defaults to ordering by score.
+        limit
+            How many results to return. Defaults to 50. Must be between 1 and
+            100.
 
         Notes
         -----
         Implements the `Get Beatmap Scores
         <https://osu.ppy.sh/docs/index.html#get-beatmap-scores>`__ endpoint.
         """
-        params = {"mode": mode, "mods": mods, "type": type}
+        params = {"mode": mode, "mods": mods, "type": type, "limit": limit}
         return self._get(BeatmapScores, f"/beatmaps/{beatmap_id}/scores",
             params)
 
     @request(Scope.PUBLIC, category="beatmaps")
     def beatmap(self,
         beatmap_id: Optional[BeatmapIdT] = None,
         *,
@@ -1884,15 +1942,15 @@
         you unable to make any more api calls until you re-authenticate.
 
         Notes
         -----
         Implements the `Revoke Current Token
         <https://osu.ppy.sh/docs/index.html#revoke-current-token>`__ endpoint.
         """
-        self.session.delete(f"{self.BASE_URL}/oauth/tokens/current")
+        self.session.delete(f"{self.base_url}/oauth/tokens/current")
         self.remove_token(self.token_key, self.token_directory)
 
 
     # /rankings
     # ---------
 
     @request(Scope.PUBLIC, category="rankings")
@@ -2080,21 +2138,28 @@
 
         Notes
         -----
         Implements the `Download Score
         <https://osu.ppy.sh/docs/index.html#scoresmodescoredownload>`__
         endpoint.
         """
-        url = f"{self.BASE_URL}/scores/{mode.value}/{score_id}/download"
+        if self.domain is Domain.LAZER:
+            raise ValueError("Downloading scores using the lazer domain is not "
+                "currently supported, as lazer itself does not currently "
+                "support replay downloads. This may change in the future. To "
+                "download replays, use the osu domain (ie, a normal Ossapi "
+                "instance.)")
+
+        url = f"{self.base_url}/scores/{mode.value}/{score_id}/download"
         r = self.session.get(url)
 
         # if the response above succeeded, it will return a raw string
         # instead of json. If it didn't succeed, it will return json with an
         # error.
-        # So always try parsing as json to check if there's an error. If parsin
+        # So always try parsing as json to check if there's an error. If parsing
         # fails, just assume the request succeeded and move on.
         try:
             json_ = r.json()
             self._check_response(json_, url)
         except json.JSONDecodeError:
             pass
```

### Comparing `ossapi-3.1.9/ossapi/ossapiv2_async.py` & `ossapi-3.2.0/ossapi/ossapiv2_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -994,36 +994,40 @@
 
     @request(Scope.PUBLIC, category="beatmaps")
     async def beatmap_scores(self,
         beatmap_id: BeatmapIdT,
         *,
         mode: Optional[GameModeT] = None,
         mods: Optional[ModT] = None,
-        type: Optional[RankingTypeT] = None
+        type: Optional[RankingTypeT] = None,
+        limit: Optional[int] = None
     ) -> BeatmapScores:
         """
         Get the top scores of a beatmap.
 
         Parameters
         ----------
         beatmap_id
             The beatmap to get scores of.
         mode
             The mode to get scores of.
         mods
             Get the top scores set with exactly these mods, if passed.
         type
             How to order the scores. Defaults to ordering by score.
+        limit
+            How many results to return. Defaults to 50. Must be between 1 and
+            100.
 
         Notes
         -----
         Implements the `Get Beatmap Scores
         <https://osu.ppy.sh/docs/index.html#get-beatmap-scores>`__ endpoint.
         """
-        params = {"mode": mode, "mods": mods, "type": type}
+        params = {"mode": mode, "mods": mods, "type": type, "limit": limit}
         return await self._get(BeatmapScores, f"/beatmaps/{beatmap_id}/scores",
             params)
 
     @request(Scope.PUBLIC, category="beatmaps")
     async def beatmap(self,
         beatmap_id: Optional[BeatmapIdT] = None,
         *,
@@ -2193,14 +2197,15 @@
         # error.
         # So always try parsing as json to check if there's an error. If parsing
         # fails, just assume the request succeeded and move on.
         # TODO we probably want to be checking headers here instead.
         # Should be x-osu-replay for valid response.
         try:
             json_ = await r.json()
+            await aiohttp_session.close()
             self._check_response(json_, url)
         except ContentTypeError:
             pass
 
         content = await r.read()
         await aiohttp_session.close()
```

### Comparing `ossapi-3.1.9/ossapi/replay.py` & `ossapi-3.2.0/ossapi/replay.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.9/ossapi/utils.py` & `ossapi-3.2.0/ossapi/utils.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.9/ossapi.egg-info/PKG-INFO` & `ossapi-3.2.0/ossapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossapi
-Version: 3.1.9
+Version: 3.2.0
 Summary: Complete python wrapper for osu! api v2 and v1.
 Author-email: Liam DeVoe <orionldevoe@gmail.com>
 Project-URL: Homepage, https://github.com/circleguard/ossapi
 Keywords: osu!,wrapper,api,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `ossapi-3.1.9/pyproject.toml` & `ossapi-3.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ossapi"
-version = "3.1.9"
+version = "3.2.0"
 description = "Complete python wrapper for osu! api v2 and v1."
 readme = "README.md"
 keywords = ["osu!", "wrapper", "api", "python"]
 authors = [
   {name = "Liam DeVoe", email = "orionldevoe@gmail.com" }
 ]
 classifiers = [
```

### Comparing `ossapi-3.1.9/tests/__init__.py` & `ossapi-3.2.0/tests/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 import os
 from unittest import TestCase
 
-from ossapi import Ossapi, OssapiV1, Grant, Scope
+from ossapi import Ossapi, OssapiV1, Grant, Scope, Domain
 
 
 # technically all scopes except Scope.DELEGATE, since I don't own a bot account
 ALL_SCOPES = [Scope.CHAT_WRITE, Scope.FORUM_WRITE, Scope.FRIENDS_READ,
     Scope.IDENTIFY, Scope.PUBLIC]
 UNIT_TEST_MESSAGE = ("unit test from ossapi "
     "(https://github.com/circleguard/ossapi/), please ignore")
 
 headless = os.environ.get("OSSAPI_TEST_HEADLESS", False)
 
 
-class DevOssapi(Ossapi):
-    TOKEN_URL = "https://dev.ppy.sh/oauth/token"
-    AUTH_CODE_URL = "https://dev.ppy.sh/oauth/authorize"
-    BASE_URL = "https://dev.ppy.sh/api/v2"
-
 def get_env(name):
     val = os.environ.get(name)
     if val is None:
         val = input(f"Enter a value for {name}: ")
     return val
 
 def setup_api_v1():
@@ -29,23 +24,25 @@
     return OssapiV1(key)
 
 def setup_api_v2():
     client_id = int(get_env("OSU_API_CLIENT_ID"))
     client_secret = get_env("OSU_API_CLIENT_SECRET")
     api_v2 = Ossapi(client_id, client_secret, strict=True,
         grant=Grant.CLIENT_CREDENTIALS)
+    api_v2_lazer = Ossapi(client_id, client_secret, strict=True,
+        grant=Grant.CLIENT_CREDENTIALS, domain=Domain.LAZER)
 
     if headless:
         api_v2_full = None
     else:
         redirect_uri = get_env("OSU_API_REDIRECT_URI")
         api_v2_full = Ossapi(client_id, client_secret, redirect_uri,
             strict=True, grant=Grant.AUTHORIZATION_CODE, scopes=ALL_SCOPES)
 
-    return (api_v2, api_v2_full)
+    return (api_v2, api_v2_full, api_v2_lazer)
 
 def setup_api_v2_dev():
     if headless:
         return None
 
     run_dev = os.environ.get("OSSAPI_TEST_RUN_DEV")
     # set OSSAPI_TEST_RUN_DEV to 0 to always skip dev tests.
@@ -63,19 +60,19 @@
         if use_dev.lower().strip() == "n":
             return None
 
     client_id = int(get_env("OSU_API_CLIENT_ID_DEV"))
     client_secret = get_env("OSU_API_CLIENT_SECRET_DEV")
 
     redirect_uri = get_env("OSU_API_REDIRECT_URI_DEV")
-    return DevOssapi(client_id, client_secret, redirect_uri, strict=True,
-        grant=Grant.AUTHORIZATION_CODE, scopes=ALL_SCOPES)
+    return Ossapi(client_id, client_secret, redirect_uri, strict=True,
+        grant=Grant.AUTHORIZATION_CODE, scopes=ALL_SCOPES, domain="dev")
 
 api_v1 = setup_api_v1()
-api_v2, api_v2_full = setup_api_v2()
+api_v2, api_v2_full, api_v2_lazer = setup_api_v2()
 api_v2_dev = setup_api_v2_dev()
 
 
 class TestCaseAuthorizationCode(TestCase):
     def setUp(self):
         if not api_v2_full:
             self.skipTest("Running in headless mode because "
```

### Comparing `ossapi-3.1.9/tests/test_cursor.py` & `ossapi-3.2.0/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.9/tests/test_endpoints.py` & `ossapi-3.2.0/tests/test_endpoints.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from ossapi import (RankingType, BeatmapsetEventType, AccessDeniedError,
     InsufficientScopeError, Mod, GameMode, ForumPoll, RoomSearchType)
 
 from tests import (
     TestCaseAuthorizationCode, TestCaseDevServer, UNIT_TEST_MESSAGE,
     api_v2 as api,
     api_v2_full as api_full,
+    api_v2_lazer as api_lazer,
     api_v2_dev as api_dev
 )
 
 
 class TestBeatmapsetDiscussionPosts(TestCase):
     def test_deserialize(self):
         api.beatmapset_discussion_posts()
@@ -211,14 +212,15 @@
         # https://osu.ppy.sh/community/matches/97947404, tournament match
         api.match(97947404)
 
 class TestComments(TestCase):
     def test_deserialize(self):
         api.comments()
 
+
 # ======================
 # api_full test cases
 # ======================
 
 class TestCreateNewPM(TestCaseAuthorizationCode):
     def test_deserialize(self):
         # test_account https://osu.ppy.sh/users/14212521
@@ -242,14 +244,38 @@
         api_full.rooms()
         # not really sure what OWNED means here, owned by the resource owner?
         # but when I test it against myself I don't think it returns my hosted
         # rooms...
         api_full.rooms(RoomSearchType.OWNED)
 
 
+# ====================
+# api_lazer test cases
+# ====================
+class TestLazerUser(TestCase):
+    def test_lazer_different_from_osu(self):
+        # make sure the lazer domain returns something different than the osu
+        # domain. ie, we're actually hitting a different db.
+
+        statistics = api.user("tybug2").statistics
+        pp_osu = statistics.pp
+        pp_exp_osu = statistics.pp_exp
+
+        statistics = api_lazer.user("tybug2").statistics
+        pp_lazer = statistics.pp
+        pp_exp_lazer = statistics.pp_exp
+
+        # pp_exp is 0 in lazer
+        self.assertEqual(pp_exp_lazer, 0)
+        # not necessarily an invariant, but happens to be true for my account
+        self.assertNotEqual(pp_osu, pp_lazer)
+        # this is the real invariant relating pp_exp and pp on the two domains.
+        self.assertEqual(pp_lazer, pp_exp_osu)
+
+
 # =====================
 # api_dev test cases
 # =====================
 
 class TestForum(TestCaseDevServer):
     def test_forum(self):
         # test creating both a topic and posting a reply in that topic.
```

### Comparing `ossapi-3.1.9/tests/test_models.py` & `ossapi-3.2.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.9/tests/test_v1.py` & `ossapi-3.2.0/tests/test_v1.py`

 * *Files identical despite different names*

