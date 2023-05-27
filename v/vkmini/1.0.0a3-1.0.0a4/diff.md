# Comparing `tmp/vkmini-1.0.0a3.tar.gz` & `tmp/vkmini-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vkmini-1.0.0a3.tar", last modified: Mon Mar 20 15:15:27 2023, max compression
+gzip compressed data, was "vkmini-1.0.0a4.tar", last modified: Sat May 27 11:17:51 2023, max compression
```

## Comparing `vkmini-1.0.0a3.tar` & `vkmini-1.0.0a4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 15:15:27.248396 vkmini-1.0.0a3/
--rw-rw-rw-   0        0        0     1071 2022-08-06 09:07:09.000000 vkmini-1.0.0a3/LICENSE
--rw-rw-rw-   0        0        0       93 2022-10-14 19:41:47.000000 vkmini-1.0.0a3/MANIFEST.in
--rw-rw-rw-   0        0        0     1421 2023-03-20 15:15:27.247396 vkmini-1.0.0a3/PKG-INFO
--rw-rw-rw-   0        0        0      908 2023-03-20 14:05:33.000000 vkmini-1.0.0a3/README.md
--rw-rw-rw-   0        0        0       42 2023-03-20 15:15:27.248396 vkmini-1.0.0a3/setup.cfg
--rw-rw-rw-   0        0        0      787 2023-03-20 15:14:44.000000 vkmini-1.0.0a3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-20 15:15:27.190396 vkmini-1.0.0a3/vkmini/
--rw-rw-rw-   0        0        0      552 2023-03-16 13:01:20.000000 vkmini-1.0.0a3/vkmini/__init__.py
--rw-rw-rw-   0        0        0     6141 2023-03-16 13:06:54.000000 vkmini-1.0.0a3/vkmini/api.py
--rw-rw-rw-   0        0        0     4904 2023-03-13 13:00:15.000000 vkmini-1.0.0a3/vkmini/api.pyi
--rw-rw-rw-   0        0        0    30719 2022-10-07 18:08:49.000000 vkmini-1.0.0a3/vkmini/exceptions.py
--rw-rw-rw-   0        0        0     6104 2023-03-16 13:06:27.000000 vkmini-1.0.0a3/vkmini/group_longpoll.py
--rw-rw-rw-   0        0        0     5992 2023-03-20 14:00:07.000000 vkmini-1.0.0a3/vkmini/keyboard.py
--rw-rw-rw-   0        0        0     1353 2023-03-20 14:00:24.000000 vkmini-1.0.0a3/vkmini/method_groups.py
--rw-rw-rw-   0        0        0        0 2022-09-24 06:11:52.000000 vkmini-1.0.0a3/vkmini/py.typed
--rw-rw-rw-   0        0        0     3218 2023-03-20 14:00:49.000000 vkmini-1.0.0a3/vkmini/request.py
-drwxrwxrwx   0        0        0        0 2023-03-20 15:15:27.239396 vkmini-1.0.0a3/vkmini/types/
--rw-rw-rw-   0        0        0      420 2022-11-29 16:24:13.000000 vkmini-1.0.0a3/vkmini/types/__init__.pyi
--rw-rw-rw-   0        0        0   146645 2022-12-02 23:27:24.000000 vkmini-1.0.0a3/vkmini/types/methods.pyi
--rw-rw-rw-   0        0        0   165436 2023-03-14 05:47:08.000000 vkmini-1.0.0a3/vkmini/types/objects.pyi
--rw-rw-rw-   0        0        0    50978 2022-11-29 16:26:34.000000 vkmini-1.0.0a3/vkmini/types/responses.pyi
--rw-rw-rw-   0        0        0     3037 2023-03-16 13:02:53.000000 vkmini-1.0.0a3/vkmini/user_longpoll.py
--rw-rw-rw-   0        0        0     2735 2023-03-15 03:39:52.000000 vkmini-1.0.0a3/vkmini/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-20 15:15:27.223397 vkmini-1.0.0a3/vkmini.egg-info/
--rw-rw-rw-   0        0        0     1421 2023-03-20 15:15:26.000000 vkmini-1.0.0a3/vkmini.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-03-20 15:15:26.000000 vkmini-1.0.0a3/vkmini.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 15:15:26.000000 vkmini-1.0.0a3/vkmini.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-03-20 15:15:26.000000 vkmini-1.0.0a3/vkmini.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-20 15:15:26.000000 vkmini-1.0.0a3/vkmini.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 11:17:51.574771 vkmini-1.0.0a4/
+-rw-rw-rw-   0        0        0     1071 2022-08-06 09:07:09.000000 vkmini-1.0.0a4/LICENSE
+-rw-rw-rw-   0        0        0       93 2022-10-14 19:41:47.000000 vkmini-1.0.0a4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1421 2023-05-27 11:17:51.574771 vkmini-1.0.0a4/PKG-INFO
+-rw-rw-rw-   0        0        0      908 2023-03-20 14:05:33.000000 vkmini-1.0.0a4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-27 11:17:51.574771 vkmini-1.0.0a4/setup.cfg
+-rw-rw-rw-   0        0        0      787 2023-05-27 11:17:33.000000 vkmini-1.0.0a4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:17:51.563513 vkmini-1.0.0a4/vkmini/
+-rw-rw-rw-   0        0        0      552 2023-03-16 13:01:20.000000 vkmini-1.0.0a4/vkmini/__init__.py
+-rw-rw-rw-   0        0        0     6141 2023-03-16 13:06:54.000000 vkmini-1.0.0a4/vkmini/api.py
+-rw-rw-rw-   0        0        0     4904 2023-03-13 13:00:15.000000 vkmini-1.0.0a4/vkmini/api.pyi
+-rw-rw-rw-   0        0        0    30719 2022-10-07 18:08:49.000000 vkmini-1.0.0a4/vkmini/exceptions.py
+-rw-rw-rw-   0        0        0     6169 2023-05-21 10:30:32.000000 vkmini-1.0.0a4/vkmini/group_longpoll.py
+-rw-rw-rw-   0        0        0     5992 2023-03-20 14:00:07.000000 vkmini-1.0.0a4/vkmini/keyboard.py
+-rw-rw-rw-   0        0        0     1353 2023-03-20 14:00:24.000000 vkmini-1.0.0a4/vkmini/method_groups.py
+-rw-rw-rw-   0        0        0        0 2022-09-24 06:11:52.000000 vkmini-1.0.0a4/vkmini/py.typed
+-rw-rw-rw-   0        0        0     3218 2023-03-20 14:00:49.000000 vkmini-1.0.0a4/vkmini/request.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:17:51.573771 vkmini-1.0.0a4/vkmini/types/
+-rw-rw-rw-   0        0        0      420 2022-11-29 16:24:13.000000 vkmini-1.0.0a4/vkmini/types/__init__.pyi
+-rw-rw-rw-   0        0        0   146645 2022-12-02 23:27:24.000000 vkmini-1.0.0a4/vkmini/types/methods.pyi
+-rw-rw-rw-   0        0        0   165436 2023-03-14 05:47:08.000000 vkmini-1.0.0a4/vkmini/types/objects.pyi
+-rw-rw-rw-   0        0        0    50978 2022-11-29 16:26:34.000000 vkmini-1.0.0a4/vkmini/types/responses.pyi
+-rw-rw-rw-   0        0        0     3171 2023-05-27 11:11:21.000000 vkmini-1.0.0a4/vkmini/user_longpoll.py
+-rw-rw-rw-   0        0        0     2735 2023-03-15 03:39:52.000000 vkmini-1.0.0a4/vkmini/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:17:51.567770 vkmini-1.0.0a4/vkmini.egg-info/
+-rw-rw-rw-   0        0        0     1421 2023-05-27 11:17:51.000000 vkmini-1.0.0a4/vkmini.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2023-05-27 11:17:51.000000 vkmini-1.0.0a4/vkmini.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 11:17:51.000000 vkmini-1.0.0a4/vkmini.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-27 11:17:51.000000 vkmini-1.0.0a4/vkmini.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-27 11:17:51.000000 vkmini-1.0.0a4/vkmini.egg-info/top_level.txt
```

### Comparing `vkmini-1.0.0a3/LICENSE` & `vkmini-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `vkmini-1.0.0a3/PKG-INFO` & `vkmini-1.0.0a4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vkmini
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: VK API wrapper
 Home-page: https://github.com/elchinchel/vkmini
 Author: Elchin Sarkarov
 Author-email: elchin751@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vkmini-1.0.0a3/README.md` & `vkmini-1.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `vkmini-1.0.0a3/setup.py` & `vkmini-1.0.0a4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="vkmini",
-    version="1.0.0a3",
+    version="1.0.0a4",
     author="Elchin Sarkarov",
     author_email="elchin751@gmail.com",
     description="VK API wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/elchinchel/vkmini",
     packages=setuptools.find_packages(),
```

### Comparing `vkmini-1.0.0a3/vkmini/__init__.py` & `vkmini-1.0.0a4/vkmini/__init__.py`

 * *Files identical despite different names*

### Comparing `vkmini-1.0.0a3/vkmini/api.py` & `vkmini-1.0.0a4/vkmini/api.py`

 * *Files identical despite different names*

### Comparing `vkmini-1.0.0a3/vkmini/api.pyi` & `vkmini-1.0.0a4/vkmini/api.pyi`

 * *Files identical despite different names*

### Comparing `vkmini-1.0.0a3/vkmini/exceptions.py` & `vkmini-1.0.0a4/vkmini/exceptions.py`

 * *Files identical despite different names*

### Comparing `vkmini-1.0.0a3/vkmini/group_longpoll.py` & `vkmini-1.0.0a4/vkmini/group_longpoll.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,32 +31,35 @@
     async def _set_longpoll_data(self, *, new_ts: bool) -> None:
         data = await self._lp_data_getter()
         self.server = data['server']
         self.key = data['key']
         if new_ts:
             self.ts = data['ts']
 
+    async def _handle_fail(self, data):
+        if data['failed'] == 1:
+            self.ts = data['ts']
+        elif data['failed'] == 2:
+            await self._set_longpoll_data(new_ts=False)
+        else:
+            await self._set_longpoll_data(new_ts=True)
+        return []
+
     async def check(
             self,
             url_builder: 'Callable[[LongPoller], str]',
             session: Optional[ClientSession]
     ):
         if self.server is None:
             await self._set_longpoll_data(new_ts=(not hasattr(self, 'ts')))
 
         data = await request.get(url_builder(self), session)
 
         if 'failed' in data:
-            if data['failed'] == 1:
-                self.ts = data['ts']
-            elif data['failed'] == 2:
-                await self._set_longpoll_data(new_ts=False)
-            else:
-                await self._set_longpoll_data(new_ts=True)
-            return []
+            return await self._handle_fail(data)
         else:
             self.ts = data['ts']
             return data['updates']
 
 
 class BaseLP(ABC):
     _session: Optional[ClientSession]
```

### Comparing `vkmini-1.0.0a3/vkmini/keyboard.py` & `vkmini-1.0.0a4/vkmini/keyboard.py`

 * *Files identical despite different names*

### Comparing `vkmini-1.0.0a3/vkmini/method_groups.py` & `vkmini-1.0.0a4/vkmini/method_groups.py`

 * *Files identical despite different names*

### Comparing `vkmini-1.0.0a3/vkmini/request.py` & `vkmini-1.0.0a4/vkmini/request.py`

 * *Files identical despite different names*

### Comparing `vkmini-1.0.0a3/vkmini/types/methods.pyi` & `vkmini-1.0.0a4/vkmini/types/methods.pyi`

 * *Files identical despite different names*

### Comparing `vkmini-1.0.0a3/vkmini/types/objects.pyi` & `vkmini-1.0.0a4/vkmini/types/objects.pyi`

 * *Files identical despite different names*

### Comparing `vkmini-1.0.0a3/vkmini/types/responses.pyi` & `vkmini-1.0.0a4/vkmini/types/responses.pyi`

 * *Files identical despite different names*

### Comparing `vkmini-1.0.0a3/vkmini/user_longpoll.py` & `vkmini-1.0.0a4/vkmini/user_longpoll.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,35 @@
-from typing import Optional, List, Any
+from typing import Optional, TypeVar, Generic, List, Any
 
 from aiohttp.client import ClientSession
 
 from vkmini.api import VkApi
 from vkmini.utils import AbstractLogger
 from vkmini.request import check_longpoll_session
 from vkmini.group_longpoll import LongPoller, BaseLP
 
 
-class UserLP(BaseLP):
+PollerT = TypeVar('PollerT', bound=LongPoller)
+
+
+class UserLP(BaseLP, Generic[PollerT]):
     """
     Реализует получение событий через User Long Poll API
 
     Официальная документация:
     https://dev.vk.com/api/user-long-poll/getting-started
 
     Неофициальная документация:
     https://github.com/danyadev/longpoll-doc
     """
     mode: int
     wait: int
 
     _vk: VkApi
-    _poller: Optional[LongPoller]
+    _poller: Optional[PollerT]
 
     def __init__(
             self,
             vk: VkApi,
             wait: int = 25,
             mode: int = 2,
             logger: Optional[AbstractLogger] = None,
@@ -62,17 +65,17 @@
         """
         Выполняет однократный запрос к API и возвращает
         список событий из поля 'updates'
         (https://dev.vk.com/api/user-long-poll/getting-started#Формат%20ответа)
         """
         if self._poller is None:
             check_longpoll_session(self._session)
-            self._poller = LongPoller(self._get_longpoll_data)
+            self.set_poller(LongPoller(self._get_longpoll_data))
 
-        return await self._poller.check(self._get_url, self._session)
+        return await self._poller.check(self._get_url, self._session)  # pyright: ignore[reportOptionalMemberAccess]
 
     def _get_url(self, poller: LongPoller):
         return (f"https://{poller.server}?act=a_check&key={poller.key}"
                 f"&ts={poller.ts}&wait={self.wait}&mode={self.mode}&version=10")
 
     async def _get_longpoll_data(self):
         return await self._vk.messages.getLongPollServer(
```

### Comparing `vkmini-1.0.0a3/vkmini/utils.py` & `vkmini-1.0.0a4/vkmini/utils.py`

 * *Files identical despite different names*

### Comparing `vkmini-1.0.0a3/vkmini.egg-info/PKG-INFO` & `vkmini-1.0.0a4/vkmini.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vkmini
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: VK API wrapper
 Home-page: https://github.com/elchinchel/vkmini
 Author: Elchin Sarkarov
 Author-email: elchin751@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

