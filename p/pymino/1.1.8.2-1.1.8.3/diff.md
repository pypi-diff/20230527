# Comparing `tmp/pymino-1.1.8.2.tar.gz` & `tmp/pymino-1.1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.1.8.1\dist\.tmp-sip2wi96\pymino-1.1.8.2.tar", last modified: Sun May 21 23:47:52 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\submitpypi\dist\.tmp-ibrvdd1p\pymino-1.1.8.3.tar", last modified: Sat May 27 20:45:02 2023, max compression
```

## Comparing `pymino-1.1.8.2.tar` & `pymino-1.1.8.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 23:47:52.216487 pymino-1.1.8.2/
--rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.8.2/LICENSE
--rw-rw-rw-   0        0        0     6082 2023-05-21 23:47:52.216983 pymino-1.1.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.8.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-21 23:47:52.171847 pymino-1.1.8.2/pymino/
--rw-rw-rw-   0        0        0      676 2023-05-21 23:46:35.000000 pymino-1.1.8.2/pymino/__init__.py
--rw-rw-rw-   0        0        0    26133 2023-05-17 23:36:26.000000 pymino-1.1.8.2/pymino/bot.py
--rw-rw-rw-   0        0        0    48170 2023-04-13 01:03:38.000000 pymino-1.1.8.2/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-05-21 23:47:52.198631 pymino-1.1.8.2/pymino/ext/
--rw-rw-rw-   0        0        0      372 2023-02-10 13:25:37.000000 pymino-1.1.8.2/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    11206 2023-04-13 00:39:17.000000 pymino-1.1.8.2/pymino/ext/account.py
--rw-rw-rw-   0        0        0   271483 2023-05-18 00:27:35.000000 pymino-1.1.8.2/pymino/ext/community.py
--rw-rw-rw-   0        0        0    45062 2023-05-21 23:47:05.000000 pymino-1.1.8.2/pymino/ext/context.py
--rw-rw-rw-   0        0        0      871 2023-03-04 01:25:46.000000 pymino-1.1.8.2/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-05-21 23:47:52.210039 pymino-1.1.8.2/pymino/ext/entities/
--rw-rw-rw-   0        0        0      198 2023-03-05 23:07:04.000000 pymino-1.1.8.2/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.8.2/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    14506 2023-05-17 03:04:03.000000 pymino-1.1.8.2/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    49421 2023-05-17 03:04:26.000000 pymino-1.1.8.2/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     2653 2023-05-17 23:34:15.000000 pymino-1.1.8.2/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0    44257 2023-05-17 02:59:21.000000 pymino-1.1.8.2/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     6109 2023-02-10 17:39:14.000000 pymino-1.1.8.2/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.8.2/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.8.2/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0     7900 2023-05-17 02:59:28.000000 pymino-1.1.8.2/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-05-21 23:47:52.215494 pymino-1.1.8.2/pymino/ext/utilities/
--rw-rw-rw-   0        0        0       80 2023-03-04 01:08:01.000000 pymino-1.1.8.2/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.8.2/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.8.2/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0    10274 2023-04-02 23:47:45.000000 pymino-1.1.8.2/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-05-21 23:47:52.189702 pymino-1.1.8.2/pymino.egg-info/
--rw-rw-rw-   0        0        0     6082 2023-05-21 23:47:52.000000 pymino-1.1.8.2/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-05-21 23:47:52.000000 pymino-1.1.8.2/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 23:47:52.000000 pymino-1.1.8.2/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-05-21 23:47:52.000000 pymino-1.1.8.2/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-21 23:47:52.000000 pymino-1.1.8.2/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-05-21 23:47:52.223926 pymino-1.1.8.2/setup.cfg
--rw-rw-rw-   0        0        0     1340 2023-05-18 00:06:54.000000 pymino-1.1.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 20:45:02.502750 pymino-1.1.8.3/
+-rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.8.3/LICENSE
+-rw-rw-rw-   0        0        0     6082 2023-05-27 20:45:02.502750 pymino-1.1.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.8.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 20:45:02.458606 pymino-1.1.8.3/pymino/
+-rw-rw-rw-   0        0        0      676 2023-05-27 20:44:15.000000 pymino-1.1.8.3/pymino/__init__.py
+-rw-rw-rw-   0        0        0    26133 2023-05-17 23:36:26.000000 pymino-1.1.8.3/pymino/bot.py
+-rw-rw-rw-   0        0        0    48170 2023-04-13 01:03:38.000000 pymino-1.1.8.3/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-05-27 20:45:02.483407 pymino-1.1.8.3/pymino/ext/
+-rw-rw-rw-   0        0        0      372 2023-02-10 13:25:37.000000 pymino-1.1.8.3/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    11206 2023-04-13 00:39:17.000000 pymino-1.1.8.3/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   271224 2023-05-25 22:50:46.000000 pymino-1.1.8.3/pymino/ext/community.py
+-rw-rw-rw-   0        0        0    44587 2023-05-27 20:44:04.000000 pymino-1.1.8.3/pymino/ext/context.py
+-rw-rw-rw-   0        0        0      871 2023-03-04 01:25:46.000000 pymino-1.1.8.3/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-05-27 20:45:02.495806 pymino-1.1.8.3/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      198 2023-03-05 23:07:04.000000 pymino-1.1.8.3/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.8.3/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    14662 2023-05-27 20:43:58.000000 pymino-1.1.8.3/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    52847 2023-05-27 20:44:10.000000 pymino-1.1.8.3/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     2653 2023-05-17 23:34:15.000000 pymino-1.1.8.3/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0    44257 2023-05-17 02:59:21.000000 pymino-1.1.8.3/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     6185 2023-05-25 23:01:02.000000 pymino-1.1.8.3/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.8.3/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.8.3/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0     7900 2023-05-17 02:59:28.000000 pymino-1.1.8.3/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-05-27 20:45:02.501758 pymino-1.1.8.3/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0       80 2023-03-04 01:08:01.000000 pymino-1.1.8.3/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.8.3/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.8.3/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0    10274 2023-04-02 23:47:45.000000 pymino-1.1.8.3/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-27 20:45:02.475470 pymino-1.1.8.3/pymino.egg-info/
+-rw-rw-rw-   0        0        0     6082 2023-05-27 20:45:02.000000 pymino-1.1.8.3/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-05-27 20:45:02.000000 pymino-1.1.8.3/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 20:45:02.000000 pymino-1.1.8.3/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-05-27 20:45:02.000000 pymino-1.1.8.3/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-27 20:45:02.000000 pymino-1.1.8.3/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-05-27 20:45:02.504734 pymino-1.1.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2023-05-18 00:06:54.000000 pymino-1.1.8.3/setup.py
```

### Comparing `pymino-1.1.8.2/LICENSE` & `pymino-1.1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.2/PKG-INFO` & `pymino-1.1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.8.2
+Version: 1.1.8.3
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.8.2 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.8.3 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.8.2/README.md` & `pymino-1.1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.2/pymino/__init__.py` & `pymino-1.1.8.3/pymino/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.1.8.2'
+__version__ = '1.1.8.3'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .client import Client as Client
 
 from requests import get
 from colorama import Fore, Style
```

### Comparing `pymino-1.1.8.2/pymino/bot.py` & `pymino-1.1.8.3/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.2/pymino/client.py` & `pymino-1.1.8.3/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.2/pymino/ext/account.py` & `pymino-1.1.8.3/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.2/pymino/ext/community.py` & `pymino-1.1.8.3/pymino/ext/community.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,20 +15,15 @@
 from .entities.messages import (
     CMessage, CMessages, PrepareMessage
     )
 from .entities.exceptions import (
     InvalidImage, MissingCommunityId,
     MissingTimers, NoDataProvided, NotLoggedIn
     )
-from .entities.general import (
-    ApiResponse, CBlog, CBlogList, CChatMembers,
-    CComment, CCommentList, CCommunity, CCommunityList,
-    CheckIn, CommunityInvitation, Coupon, FeaturedBlogs,
-    InvitationId, LinkInfo, NotificationList, QuizRankingList
-    )
+from .entities.general import *
 
 F = TypeVar("F", bound=Callable[..., Any])
 
 class Community:
     """
     The `Community` class handles community related actions.
 
@@ -3921,15 +3916,15 @@
         """
         return CBlogList(self.session.handler(
             method = "GET",
             url = f"/x{self.community_id if comId is None else comId}/s/blog?type=user&q={userId}&start={start}&size={size}"
             ))
 
     @community
-    def fetch_user_wikis(self, userId: str, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> ApiResponse: #TODO: Add WikiList
+    def fetch_user_wikis(self, userId: str, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> CWikiList:
         """
         Fetches wikis created by a user based on the specified parameters.
 
         :param userId: The ID of the user to fetch wikis for.
         :type userId: str
         :param start: The index of the first item to fetch. Default is 0.
         :type start: int
@@ -3963,15 +3958,15 @@
 
         >>> response = client.community.fetch_user_wikis(userId="2222-2222-2222-2222", comId=123)
         ... if response.statuscode == 0:
         ...     print(response.json())
         ... else:
         ...     print("Failed to fetch user wikis.")
         """
-        return ApiResponse(self.session.handler(
+        return CWikiList(self.session.handler(
             method = "GET",
             url = f"/x{self.community_id if comId is None else comId}/s/item?type=user-all&start={start}&size={size}&cv=1.2&uid={userId}"
             ))
 
     @community
     def fetch_user_check_ins(self, userId: str, comId: Union[str, int] = None) -> ApiResponse:
         """
```

### Comparing `pymino-1.1.8.2/pymino/ext/context.py` & `pymino-1.1.8.3/pymino/ext/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,18 +183,15 @@
         def on_text_message(ctx: Context):
             ctx.send(content="Hello World!", delete_after=None)
         ```
         """
         message: CMessage = self.__send_message__(
             content=content,
             extensions = {
-            "mentionedArray": [
-            {"uid": self.message.author.userId}
-            ] if isinstance(mentioned, str) else [{"uid": i} for i in mentioned
-            ] if isinstance(mentioned, list) else None
+            "mentionedArray": [{"uid": user} for user in mentioned] if mentioned else None
             })
 
         Thread(target=self._delete, args=(message, delete_after)).start() if delete_after else None
 
         return message
 
     @_run
@@ -216,48 +213,45 @@
             ctx.reply(content = "Hello World!", delete_after = None)
         ```
         """
         message: CMessage = self.__send_message__(
             content=content,
             replyMessageId=self.message.messageId,
             extensions = {
-            "mentionedArray": [
-            {"uid": self.message.author.userId}
-            ] if isinstance(mentioned, str) else [{"uid": i} for i in mentioned
-            ] if isinstance(mentioned, list) else None
+            "mentionedArray": [{"uid": user} for user in mentioned] if mentioned else None
             })
         
         Thread(target=self._delete, args=(message, delete_after)).start() if delete_after else None
         
         return message
 
-    def prepare_mentions(self, mentioned: dict) -> list:
+    def prepare_mentions(self, mentioned: list) -> list:
         """
         `prepare_mentions` - This prepares the mentions for the message.
         
         `**Parameters**``
-        - `mentioned` - `ctx.message.mentioned_dictionary`.
+        - `mentioned` - `ctx.message.mentioned_user_names`.
         
         `**Returns**``
         - `list` - The list of mentions to use as your `message`
 
         `**Example**``
         ```py
         @bot.command("mention")
         def mention(ctx: Context):
-            mentioned_users = ctx.message.mentioned_dictionary
+            mentioned_users = ctx.message.mentioned_user_names
             if not mentioned_users:
                 return ctx.reply("You didn't mention anyone!")
 
             mentioned = ctx.prepare_mentions(mentioned_users)
             return ctx.reply(
                 "Mentioned: " + ", ".join(mentioned), mentioned=list(mentioned_users)
             )
         """
-        return [f"\u200e\u200f@{mentioned[user_id]}\u202c\u202d" for user_id in mentioned]
+        return [f"\u200e\u200f@{username}\u202c\u202d" for username in mentioned]
 
     @_run
     def send_link_snippet(self, image: str, message: str = "[c]", link: str = "ndc://user-me", mentioned: list = None) -> CMessage:
         """
         `send_link_snippet` - This sends a link snippet.
 
         `**Parameters**``
@@ -287,18 +281,15 @@
                 "mediaType": 100,
                 "mediaUploadValue": self.encode_media(
                     self.__handle_media__(media=image, content_type="image/jpg", media_value=False)
                 ),
                 "mediaUploadValueContentType": "image/png",
                 "link": link
                 }],
-            "mentionedArray": [
-            {"uid": self.message.author.userId}
-            ] if isinstance(mentioned, str) else [{"uid": i} for i in mentioned
-            ] if isinstance(mentioned, list) else None
+            "mentionedArray": [{"uid": user} for user in mentioned] if mentioned else None
             })
 
         return message
     
     @_run
     def send_embed(
         self,
@@ -339,18 +330,15 @@
             attachedObject = {
                 "title": title,
                 "content": content,
                 "mediaList": [[100, self.__handle_media__(media=image, media_value=True), None]],
                 "link": link
                 },
             extensions = {
-                "mentionedArray": [
-                {"uid": self.message.author.userId}
-                ] if isinstance(mentioned, str) else [{"uid": i} for i in mentioned
-                ] if isinstance(mentioned, list) else None
+                "mentionedArray": [{"uid": user} for user in mentioned] if mentioned else None
             })
         
         return message
 
     def __handle_media__(self, media: str, content_type: str = "image/jpg", media_value: bool = False) -> str:
         response = None
         
@@ -456,14 +444,15 @@
         @bot.on_text_message()
         def on_text_message(ctx: Context):
             ctx.send_gif(gif="https://i.imgur.com/image.gif")
         ```
         """
         message: CMessage = self.__send_message__(
             mediaType=100,
+            mediaUploadValueContentType="image/gif",
             mediaUploadValue=self.encode_media(
                 self.__handle_media__(
                     media=gif,
                     content_type="image/gif",
                     media_value=False
             )))
```

### Comparing `pymino-1.1.8.2/pymino/ext/dispatcher.py` & `pymino-1.1.8.3/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.2/pymino/ext/entities/enums.py` & `pymino-1.1.8.3/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.2/pymino/ext/entities/exceptions.py` & `pymino-1.1.8.3/pymino/ext/entities/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,18 +256,23 @@
     def __init__(self, response: str):
         super().__init__(response)
 
 class DataNoLongerExists(Exception):
     def __init__(self, response: str):
         super().__init__(response)
 
+class InternalServerError(Exception):
+    def __init__(self, response: str):
+        super().__init__(response)
+
 class APIException(Exception):
     def __init__(self, response: dict):
         self.exception_map = {
             100: UnsupportedService,
+            101: InternalServerError,
             102: FileTooLarge,
             103: InvalidRequest,
             105: InvalidSession,
             106: AccessDenied,
             107: UnexistentData,
             110: ActionNotAllowed,
             111: ServiceUnderMaintenance,
```

### Comparing `pymino-1.1.8.2/pymino/ext/entities/general.py` & `pymino-1.1.8.3/pymino/ext/entities/general.py`

 * *Files 4% similar despite different names*

```diff
@@ -226,80 +226,133 @@
     
     def json(self) -> Union[dict, str]:
         return self.data
 
 class CBlog:
     def __init__(self, data: Union[dict, str]) -> None:
         self.data                   = data
-        self.globalVotesCount       = None
-        self.globalVotedValue       = None
-        self.votedValue             = None
-        self.keywords               = None
-        self.mediaList              = []
-        self.style                  = {}
-        self.totalQuizPlayCount     = None
-        self.title                  = None
-        self.tipInfo                = {}
-        self.contentRating          = None
-        self.content                = None
-        self.needHidden             = None
-        self.guestVotesCount        = None
-        self.type                   = None
-        self.status                 = None
-        self.globalCommentsCount    = None
-        self.modifiedTime           = None
-        self.widgetDisplayInterval  = None
-        self.totalPollVoteCount     = None
-        self.blogId                 = None
-        self.viewCount              = None
-        self.language               = None
-        self.author                 = None
-        self.extensions             = {}
-        self.votesCount             = None
-        self.ndcId                  = None
-        self.createdTime            = None
-        self.endTime                = None
-        self.commentsCount          = None
 
         if isinstance(data, dict):
             self.data:                  dict = data.get("blog", data)
-            self.globalVotesCount:      int = self.data.get("globalVotesCount", self.globalVotesCount)
-            self.globalVotedValue:      int = self.data.get("globalVotedValue", self.globalVotedValue)
-            self.votedValue:            int = self.data.get("votedValue", self.votedValue)
-            self.keywords:              str = self.data.get("keywords", self.keywords)
-            self.mediaList:             list = self.data.get("mediaList", self.mediaList)
-            self.style:                 dict = self.data.get("style", self.style)
-            self.totalQuizPlayCount:    int = self.data.get("totalQuizPlayCount", self.totalQuizPlayCount)
-            self.title:                 str = self.data.get("title", self.title)
-            self.tipInfo:               dict = self.data.get("tipInfo", self.tipInfo)
-            self.contentRating:         int = self.data.get("contentRating", self.contentRating)
-            self.content:               str = self.data.get("content", self.content)
-            self.needHidden:            bool = self.data.get("needHidden", self.needHidden)
-            self.guestVotesCount:       int = self.data.get("guestVotesCount", self.guestVotesCount)
-            self.type:                  int = self.data.get("type", self.type)
-            self.status:                int = self.data.get("status", self.status)
-            self.globalCommentsCount:   int = self.data.get("globalCommentsCount", self.globalCommentsCount)
-            self.modifiedTime:          str = self.data.get("modifiedTime", self.modifiedTime)
-            self.widgetDisplayInterval: str = self.data.get("widgetDisplayInterval", self.widgetDisplayInterval)
-            self.totalPollVoteCount:    int = self.data.get("totalPollVoteCount", self.totalPollVoteCount)
-            self.blogId:                str = self.data.get("blogId", self.blogId)
-            self.viewCount:             int = self.data.get("viewCount", self.viewCount)
-            self.language:              str = self.data.get("language", self.language)
+            self.globalVotesCount:      int = self.data.get("globalVotesCount")
+            self.globalVotedValue:      int = self.data.get("globalVotedValue")
+            self.votedValue:            int = self.data.get("votedValue")
+            self.keywords:              str = self.data.get("keywords")
+            self.mediaList:             list = self.data.get("mediaList")
+            self.style:                 dict = self.data.get("style")
+            self.totalQuizPlayCount:    int = self.data.get("totalQuizPlayCount")
+            self.title:                 str = self.data.get("title")
+            self.tipInfo:               dict = self.data.get("tipInfo")
+            self.contentRating:         int = self.data.get("contentRating")
+            self.content:               str = self.data.get("content")
+            self.needHidden:            bool = self.data.get("needHidden")
+            self.guestVotesCount:       int = self.data.get("guestVotesCount")
+            self.type:                  int = self.data.get("type")
+            self.status:                int = self.data.get("status")
+            self.globalCommentsCount:   int = self.data.get("globalCommentsCount")
+            self.modifiedTime:          str = self.data.get("modifiedTime")
+            self.widgetDisplayInterval: str = self.data.get("widgetDisplayInterval")
+            self.totalPollVoteCount:    int = self.data.get("totalPollVoteCount")
+            self.blogId:                str = self.data.get("blogId")
+            self.viewCount:             int = self.data.get("viewCount")
+            self.language:              str = self.data.get("language")
 
             try:
-                self.author:            Union[UserProfile, None] = UserProfile(data=self.data.get("author", self.author))
+                self.author:            Union[UserProfile, None] = UserProfile(data=self.data.get("author"))
             except Exception:
                 self.author:            Union[UserProfile, None] = None
 
-            self.extensions:            dict = self.data.get("extensions", self.extensions)
-            self.votesCount:            int = self.data.get("votesCount", self.votesCount)
-            self.ndcId:                 int = self.data.get("ndcId", self.ndcId)
-            self.createdTime:           str = self.data.get("createdTime", self.createdTime)
-            self.endTime:               str = self.data.get("endTime", self.endTime)
-            self.commentsCount:         int = self.data.get("commentsCount", self.commentsCount)
+            self.extensions:            dict = self.data.get("extensions")
+            self.votesCount:            int = self.data.get("votesCount")
+            self.ndcId:                 int = self.data.get("ndcId")
+            self.createdTime:           str = self.data.get("createdTime")
+            self.endTime:               str = self.data.get("endTime")
+            self.commentsCount:         int = self.data.get("commentsCount")
+
+    def json(self) -> Union[dict, str]:
+        return self.data
+
+class CWiki:
+    def __init__(self, data: Union[dict, str]) -> None:
+        self.data                   = data
+
+        if isinstance(data, dict):
+            self.data:                  dict = data.get("item", data)
+            self.globalVotesCount:      int = self.data.get("globalVotesCount")
+            self.globalVotedValue:      int = self.data.get("globalVotedValue")
+            self.votedValue:            int = self.data.get("votedValue")
+            self.keywords:              str = self.data.get("keywords")
+            self.mediaList:             list = self.data.get("mediaList")
+            self.style:                 dict = self.data.get("style")
+            self.totalQuizPlayCount:    int = self.data.get("totalQuizPlayCount")
+            self.title:                 str = self.data.get("title")
+            self.tipInfo:               dict = self.data.get("tipInfo")
+            self.contentRating:         int = self.data.get("contentRating")
+            self.content:               str = self.data.get("content")
+            self.needHidden:            bool = self.data.get("needHidden")
+            self.guestVotesCount:       int = self.data.get("guestVotesCount")
+            self.type:                  int = self.data.get("type")
+            self.status:                int = self.data.get("status")
+            self.globalCommentsCount:   int = self.data.get("globalCommentsCount")
+            self.modifiedTime:          str = self.data.get("modifiedTime")
+            self.widgetDisplayInterval: str = self.data.get("widgetDisplayInterval")
+            self.totalPollVoteCount:    int = self.data.get("totalPollVoteCount")
+            self.wikiId:                str = self.data.get("itemId")
+            self.viewCount:             int = self.data.get("viewCount")
+            self.language:              str = self.data.get("language")
+
+            try:
+                self.author:            Union[UserProfile, None] = UserProfile(data=self.data.get("author"))
+            except Exception:
+                self.author:            Union[UserProfile, None] = None
+
+            self.extensions:            dict = self.data.get("extensions")
+            self.votesCount:            int = self.data.get("votesCount")
+            self.ndcId:                 int = self.data.get("ndcId")
+            self.createdTime:           str = self.data.get("createdTime")
+            self.endTime:               str = self.data.get("endTime")
+            self.commentsCount:         int = self.data.get("commentsCount")
+
+    def json(self) -> Union[dict, str]:
+        return self.data
+
+
+class CWikiList:
+    def __init__(self, data: Union[dict, str]):
+        self.data:                   dict = data.get("itemList", data)
+        parser:                      List[CWiki] = [CWiki(x) for x in self.data]
+        self.author:                 UserProfileList = UserProfileList([x.author.json() for x in parser])
+        self.globalVotesCount:       list = [x.globalVotesCount for x in parser]
+        self.globalVotedValue:       list = [x.globalVotedValue for x in parser]
+        self.votedValue:             list = [x.votedValue for x in parser]
+        self.keywords:               list = [x.keywords for x in parser]
+        self.mediaList:              list = [x.mediaList for x in parser]
+        self.style:                  list = [x.style for x in parser]
+        self.totalQuizPlayCount:     list = [x.totalQuizPlayCount for x in parser]
+        self.title:                  list = [x.title for x in parser]
+        self.tipInfo:                list = [x.tipInfo for x in parser]
+        self.contentRating:          list = [x.contentRating for x in parser]
+        self.content:                list = [x.content for x in parser]
+        self.needHidden:             list = [x.needHidden for x in parser]
+        self.guestVotesCount:        list = [x.guestVotesCount for x in parser]
+        self.type:                   list = [x.type for x in parser]
+        self.status:                 list = [x.status for x in parser]
+        self.globalCommentsCount:    list = [x.globalCommentsCount for x in parser]
+        self.modifiedTime:           list = [x.modifiedTime for x in parser]
+        self.widgetDisplayInterval:  list = [x.widgetDisplayInterval for x in parser]
+        self.totalPollVoteCount:     list = [x.totalPollVoteCount for x in parser]
+        self.wikiId:                 list = [x.wikiId for x in parser]
+        self.viewCount:              list = [x.viewCount for x in parser]
+        self.language:               list = [x.language for x in parser]
+        self.extensions:             list = [x.extensions for x in parser]
+        self.votesCount:             list = [x.votesCount for x in parser]
+        self.ndcId:                  list = [x.ndcId for x in parser]
+        self.createdTime:            list = [x.createdTime for x in parser]
+        self.endTime:                list = [x.endTime for x in parser]
+        self.commentsCount:          list = [x.commentsCount for x in parser]
 
     def json(self) -> Union[dict, str]:
         return self.data
 
 class CBlogList:
     def __init__(self, data: Union[dict, str]):
         self.data:                   dict = data.get("blogList", data)
```

### Comparing `pymino-1.1.8.2/pymino/ext/entities/handlers.py` & `pymino-1.1.8.3/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.2/pymino/ext/entities/messages.py` & `pymino-1.1.8.3/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.2/pymino/ext/entities/threads.py` & `pymino-1.1.8.3/pymino/ext/entities/threads.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 
     def __parser__(self, key: str, default=None): return [i.get(key, default) for i in self.data]
 
     def json(self): return self.data
 
 class MemberSummary:
     def __init__(self, data: dict):
-        self.data = data[0] if isinstance(data[0], list) else data
+        try:
+            self.data = data[0] if isinstance(data[0], list) else data
+        except IndexError:
+            self.data = data
             
         self.status:            list = [x.get("status") for x in self.data]
         self.uid:               list = [x.get("uid") for x in self.data]
         self.userId:            list = self.uid
         self.membershipStatus:  list = [x.get("membershipStatus") for x in self.data]
         self.role:              list = [x.get("role") for x in self.data]
         self.nickname:          list = [x.get("nickname") for x in self.data]
```

### Comparing `pymino-1.1.8.2/pymino/ext/entities/userprofile.py` & `pymino-1.1.8.3/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.2/pymino/ext/entities/wsevents.py` & `pymino-1.1.8.3/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.2/pymino/ext/socket.py` & `pymino-1.1.8.3/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.2/pymino/ext/utilities/commands.py` & `pymino-1.1.8.3/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.2/pymino/ext/utilities/generate.py` & `pymino-1.1.8.3/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.2/pymino/ext/utilities/request_handler.py` & `pymino-1.1.8.3/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.2/pymino.egg-info/PKG-INFO` & `pymino-1.1.8.3/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.8.2
+Version: 1.1.8.3
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.8.2 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.8.3 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.8.2/pymino.egg-info/SOURCES.txt` & `pymino-1.1.8.3/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.2/setup.cfg` & `pymino-1.1.8.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e31 2e38 2e32 0d0a 6175  on = 1.1.8.2..au
+00000020: 6f6e 203d 2031 2e31 2e38 2e33 0d0a 6175  on = 1.1.8.3..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.1.8.2/setup.py` & `pymino-1.1.8.3/setup.py`

 * *Files identical despite different names*

