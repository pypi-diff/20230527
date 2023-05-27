# Comparing `tmp/lavviebotaio-0.0.1.2.tar.gz` & `tmp/lavviebotaio-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavviebotaio-0.0.1.2.tar", last modified: Sun Sep  4 18:28:02 2022, max compression
+gzip compressed data, was "lavviebotaio-0.0.1.3.tar", last modified: Sat May 27 19:31:24 2023, max compression
```

## Comparing `lavviebotaio-0.0.1.2.tar` & `lavviebotaio-0.0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2022-09-04 18:28:02.533317 lavviebotaio-0.0.1.2/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2022-09-04 18:25:34.000000 lavviebotaio-0.0.1.2/LICENSE
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     3233 2022-09-04 18:28:02.533524 lavviebotaio-0.0.1.2/PKG-INFO
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     2078 2022-09-04 18:25:34.000000 lavviebotaio-0.0.1.2/README.md
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2022-09-04 18:28:02.531229 lavviebotaio-0.0.1.2/lavviebot/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1268 2022-09-04 18:25:34.000000 lavviebotaio-0.0.1.2/lavviebot/__init__.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     4045 2022-09-04 18:25:34.000000 lavviebotaio-0.0.1.2/lavviebot/constants.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      455 2022-09-04 18:25:34.000000 lavviebotaio-0.0.1.2/lavviebot/exceptions.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)    22132 2022-09-04 18:25:34.000000 lavviebotaio-0.0.1.2/lavviebot/lavviebot_client.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1042 2022-09-04 18:25:34.000000 lavviebotaio-0.0.1.2/lavviebot/model.py
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2022-09-04 18:28:02.532958 lavviebotaio-0.0.1.2/lavviebotaio.egg-info/
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     3233 2022-09-04 18:28:02.000000 lavviebotaio-0.0.1.2/lavviebotaio.egg-info/PKG-INFO
--rw-r--r--   0 robertdrinovac   (501) staff       (20)      333 2022-09-04 18:28:02.000000 lavviebotaio-0.0.1.2/lavviebotaio.egg-info/SOURCES.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2022-09-04 18:28:02.000000 lavviebotaio-0.0.1.2/lavviebotaio.egg-info/dependency_links.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       15 2022-09-04 18:28:02.000000 lavviebotaio-0.0.1.2/lavviebotaio.egg-info/requires.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       10 2022-09-04 18:28:02.000000 lavviebotaio-0.0.1.2/lavviebotaio.egg-info/top_level.txt
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)       38 2022-09-04 18:28:02.534091 lavviebotaio-0.0.1.2/setup.cfg
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1000 2022-09-04 18:25:34.000000 lavviebotaio-0.0.1.2/setup.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-05-27 19:31:24.458603 lavviebotaio-0.0.1.3/
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2023-05-27 19:29:33.000000 lavviebotaio-0.0.1.3/LICENSE
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     3233 2023-05-27 19:31:24.458845 lavviebotaio-0.0.1.3/PKG-INFO
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     2078 2023-05-27 19:29:33.000000 lavviebotaio-0.0.1.3/README.md
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-05-27 19:31:24.455412 lavviebotaio-0.0.1.3/lavviebot/
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1298 2023-05-27 19:29:33.000000 lavviebotaio-0.0.1.3/lavviebot/__init__.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     4286 2023-05-27 19:29:33.000000 lavviebotaio-0.0.1.3/lavviebot/constants.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      455 2023-05-27 19:29:33.000000 lavviebotaio-0.0.1.3/lavviebot/exceptions.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)    24526 2023-05-27 19:29:33.000000 lavviebotaio-0.0.1.3/lavviebot/lavviebot_client.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1088 2023-05-27 19:29:33.000000 lavviebotaio-0.0.1.3/lavviebot/model.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-05-27 19:31:24.458025 lavviebotaio-0.0.1.3/lavviebotaio.egg-info/
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     3233 2023-05-27 19:31:24.000000 lavviebotaio-0.0.1.3/lavviebotaio.egg-info/PKG-INFO
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)      333 2023-05-27 19:31:24.000000 lavviebotaio-0.0.1.3/lavviebotaio.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-05-27 19:31:24.000000 lavviebotaio-0.0.1.3/lavviebotaio.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       15 2023-05-27 19:31:24.000000 lavviebotaio-0.0.1.3/lavviebotaio.egg-info/requires.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       10 2023-05-27 19:31:24.000000 lavviebotaio-0.0.1.3/lavviebotaio.egg-info/top_level.txt
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)       38 2023-05-27 19:31:24.459527 lavviebotaio-0.0.1.3/setup.cfg
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1000 2023-05-27 19:29:33.000000 lavviebotaio-0.0.1.3/setup.py
```

### Comparing `lavviebotaio-0.0.1.2/LICENSE` & `lavviebotaio-0.0.1.3/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 RobertD502
+Copyright (c) 2023 RobertD502
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `lavviebotaio-0.0.1.2/PKG-INFO` & `lavviebotaio-0.0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavviebotaio
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: Asynchronous Python library for the PurrSong API utilized by LavvieBot S litter boxes
 Home-page: https://github.com/RobertD502/lavviebotaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/lavviebotaio/issues
 Project-URL: Source, https://github.com/RobertD502/lavviebotaio/
```

### Comparing `lavviebotaio-0.0.1.2/README.md` & `lavviebotaio-0.0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lavviebotaio-0.0.1.2/lavviebot/__init__.py` & `lavviebotaio-0.0.1.3/lavviebot/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from lavviebot import exceptions
 from lavviebot import lavviebot_client
 from lavviebot import model
 
 from lavviebot.constants import (ACCEPT, ACCEPT_ENCODING, ACCEPT_LANGUAGE,
                                  APP_VERSION, BASE_URL, CAT_STATUS, CONNECTION,
                                  CONTENT_TYPE, COOKIE_QUERY, DISCOVER_CATS,
-                                 DISCOVER_LB, LANGUAGE, LB_CAT_LOG, LB_STATUS,
+                                 DISCOVER_LB, LANGUAGE, LB_CAT_LOG, LB_ERROR_LOG, LB_STATUS,
                                  TIMEOUT, TIME_ZONE, TOKEN_QUERY,
                                  UNKNOWN_STATUS, USER_AGENT,)
 from lavviebot.exceptions import (LavviebotAuthError, LavviebotError,)
 from lavviebot.lavviebot_client import (LavviebotClient,)
 from lavviebot.model import (Cat, LavviebotData, LitterBox,)
 
 __all__ = ['ACCEPT', 'ACCEPT_ENCODING', 'ACCEPT_LANGUAGE', 'APP_VERSION',
            'BASE_URL', 'CAT_STATUS', 'CONNECTION', 'CONTENT_TYPE',
            'COOKIE_QUERY', 'Cat', 'DISCOVER_CATS', 'DISCOVER_LB', 'LANGUAGE',
-           'LB_CAT_LOG', 'LB_STATUS', 'LavviebotAuthError', 'LavviebotClient',
+           'LB_CAT_LOG', 'LB_ERROR_LOG', 'LB_STATUS', 'LavviebotAuthError', 'LavviebotClient',
            'LavviebotData', 'LavviebotError', 'LitterBox', 'TIMEOUT',
            'TIME_ZONE', 'TOKEN_QUERY', 'UNKNOWN_STATUS', 'USER_AGENT',
            'constants', 'exceptions', 'lavviebot_client', 'model']
```

### Comparing `lavviebotaio-0.0.1.2/lavviebot/constants.py` & `lavviebotaio-0.0.1.3/lavviebot/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,8 +59,10 @@
                  "{timezone graphType period today avg30days avgTerm graphData __typename}"
 
 """ Query to get most recent status for individual cat """
 CAT_STATUS = "query GetPoopData($data: GetPoopGraphDataArgs!) " \
              "{getPoopData(data: $data) {...GraphData __typename}} fragment GraphData on PoopGraphDataResponse" \
              "{timezone graphType period today avg30days avgTerm graphData __typename}"
 
-
+""" Query to get the error log for a litter boc """
+LB_ERROR_LOG = "query GetIotErrorLog($data: GetIotErrorLogArgs!) " \
+               "{getIotErrorLog(data: $data) {errorLogs {id status creationTime __typename} cursor hasMore __typename}}"
```

### Comparing `lavviebotaio-0.0.1.2/lavviebot/lavviebot_client.py` & `lavviebotaio-0.0.1.3/lavviebot/lavviebot_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Python API for Lavviebot S Litter Box"""
 from __future__ import annotations
 
-from typing import Any
+from typing import Any, Tuple
 
-from datetime import datetime
+from datetime import date, datetime
 from zoneinfo import ZoneInfo
 
 import asyncio
 
 from http.cookies import SimpleCookie
 
 from aiohttp import ClientResponse, ClientSession
 
 from .exceptions import LavviebotAuthError, LavviebotError
 from .model import Cat, LavviebotData, LitterBox
 from .constants import (ACCEPT, ACCEPT_ENCODING, ACCEPT_LANGUAGE,
                         APP_VERSION, BASE_URL, CAT_STATUS, CONNECTION,
                         CONTENT_TYPE, COOKIE_QUERY, DISCOVER_CATS,
-                        DISCOVER_LB, LANGUAGE, LB_CAT_LOG, LB_STATUS,
+                        DISCOVER_LB, LANGUAGE, LB_CAT_LOG, LB_ERROR_LOG, LB_STATUS,
                         TIMEOUT, TIME_ZONE, TOKEN_QUERY, UNKNOWN_STATUS, USER_AGENT,)
 
 
 class LavviebotClient:
     """Lavviebot Client"""
 
     def __init__(
@@ -230,14 +230,27 @@
                 last_cat_used_name: str = state[1]['data']['getLavviebotPoopRecord']['catUsageHistory'][00].get(
                     'nickname')
 
             last_used_duration: int = state[1]['data']['getLavviebotPoopRecord']['catUsageHistory'][00].get('duration')
             last_used: datetime = datetime.fromtimestamp(
                 int(state[1]['data']['getLavviebotPoopRecord']['catUsageHistory'][00].get('creationTime')) / 1000,
                 tz=ZoneInfo('Asia/Seoul')).astimezone()
+            # Get the oldest usage record for today in order to determine number of times litter box was used today
+            today_date: date = date.today()
+            today_usage_list: list = []
+            for usage_record in state[1]['data']['getLavviebotPoopRecord']['catUsageHistory']:
+                epoch_to_date = datetime.fromtimestamp(int(usage_record['creationTime']) / 1000).date()
+                if epoch_to_date == today_date:
+                    today_usage_list.append(usage_record)
+                else:
+                    break
+            times_used_today: int = len(today_usage_list)
+
+            # Litter box error log
+            error_log: list = state[2]['data']['getIotErrorLog']['errorLogs']
 
             litter_box_data[device_id] = LitterBox(
                 device_id=device_id,
                 device_name=device_name,
                 iot_code_tail=iot_code_tail,
                 latest_firmware=latest_firmware,
                 router_ssid=router_ssid,
@@ -252,14 +265,16 @@
                 litter_bottom_amount_pnds=litter_bottom_amount_pnds,
                 humidity=humidity,
                 temperature_c=temperature_c,
                 last_seen=last_seen,
                 last_cat_used_name=last_cat_used_name,
                 last_used_duration=last_used_duration,
                 last_used=last_used,
+                times_used_today=times_used_today,
+                error_log=error_log,
             )
 
         """ Get all cats """
 
         cats = []
         cat_data: dict[int, Cat] = {}
         if self.has_cat:
@@ -323,23 +338,25 @@
                     duration=duration,
                     poop_count=poop_count,
                 )
 
         return LavviebotData(litterboxes=litter_box_data, cats=cat_data)
 
 
-    async def async_fetch_all_endpoints(self, device_id: int) -> tuple[Any, Any]:
+    async def async_fetch_all_endpoints(self, device_id: int) -> tuple[
+        BaseException | Any, BaseException | Any, BaseException | Any]:
         """
         Parallel request are made to all endpoints for each litter box.
         returns a list containing latest status, and cat usage log
         """
 
         results = await asyncio.gather(*[
             self.async_get_litter_box_status(device_id),
-            self.async_get_litter_box_cat_log(device_id)
+            self.async_get_litter_box_cat_log(device_id),
+            self.async_get_litter_box_error_log(device_id),
         ],
                                        )
         return results
 
 
     async def async_get_litter_box_status(self, device_id: int) -> ClientResponse:
         """ Get most recent status available for litter box """
@@ -408,15 +425,51 @@
                 await self.login()
                 return await self.async_get_litter_box_cat_log(device_id)
             else:
                 raise LavviebotError(message)
         else:
             return response
 
-    async def async_get_unknown_status(self, cat_id: int) -> ClientResponse:
+    async def async_get_litter_box_error_log(self, device_id: int) -> ClientResponse:
+        """ Get error log that is associated with the litter box """
+
+        if self.cookie is None or self.token is None:
+            await self.login()
+        headers = {
+            'Accept': ACCEPT,
+            'Cookie': self.cookie,
+            'Accept-Encoding': ACCEPT_ENCODING,
+            'Accept-Language': ACCEPT_LANGUAGE,
+            'Authorization': self.token,
+            'Connection': CONNECTION,
+            'Content-Type': CONTENT_TYPE,
+            'User-Agent': USER_AGENT
+        }
+        lbel_payload = {
+            "operationName": "GetIotErrorLog",
+            "variables": {
+                "data": {
+                    "iotId": device_id
+                }
+            },
+            "query": LB_ERROR_LOG
+        }
+        response = await self._post(headers, lbel_payload)
+        if 'errors' in response:
+            message = response['errors'][0]['message']
+            if message == "Please login again.":
+                await self.login()
+                return await self.async_get_litter_box_error_log(device_id)
+            else:
+                raise LavviebotError(message)
+        else:
+            return response
+
+    async def async_get_unknown_status(self, cat_id: int) -> tuple[
+        SimpleCookie | ClientResponse, SimpleCookie | ClientResponse, SimpleCookie | ClientResponse]:
         """ Get most recent status for Unknown cat if present """
 
         if self.cookie is None or self.token is None:
             await self.login()
         headers = {
             'Accept': ACCEPT,
             'Cookie': self.cookie,
@@ -472,15 +525,16 @@
                 await self.login()
                 return await self.async_get_unknown_status(cat_id)
             else:
                 raise LavviebotError(message)
         else:
             return poop_response, duration_response, weight_response
 
-    async def async_get_cat_status(self, cat_id: int) -> ClientResponse:
+    async def async_get_cat_status(self, cat_id: int) -> tuple[
+        SimpleCookie | ClientResponse, SimpleCookie | ClientResponse, SimpleCookie | ClientResponse]:
         """ Get most recent status for single cat """
 
         if self.cookie is None or self.token is None:
             await self.login()
         headers = {
             'Accept': ACCEPT,
             'Cookie': self.cookie,
```

### Comparing `lavviebotaio-0.0.1.2/lavviebot/model.py` & `lavviebotaio-0.0.1.3/lavviebot/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     litter_bottom_amount_pnds: float
     humidity: int
     temperature_c: int
     last_seen: datetime
     last_cat_used_name: str
     last_used_duration: int
     last_used: datetime
+    times_used_today: int
+    error_log: list
 
 @dataclass
 class Cat:
     """ Dataclass for Lavviebot cat. """
 
     cat_id: int
     cat_name: str
```

### Comparing `lavviebotaio-0.0.1.2/lavviebotaio.egg-info/PKG-INFO` & `lavviebotaio-0.0.1.3/lavviebotaio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavviebotaio
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: Asynchronous Python library for the PurrSong API utilized by LavvieBot S litter boxes
 Home-page: https://github.com/RobertD502/lavviebotaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/lavviebotaio/issues
 Project-URL: Source, https://github.com/RobertD502/lavviebotaio/
```

### Comparing `lavviebotaio-0.0.1.2/setup.py` & `lavviebotaio-0.0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lavviebotaio",
-    version="0.0.1.2",
+    version="0.0.1.3",
     author="Robert Drinovac",
     author_email="unlisted@gmail.com",
     description="Asynchronous Python library for the PurrSong API utilized by LavvieBot S litter boxes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/RobertD502/lavviebotaio',
     keywords='lavviebot, lavviebot s, purrsong, litter box',
```

