# Comparing `tmp/ofscraper-2.0.1.tar.gz` & `tmp/ofscraper-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-2.0.1.tar", max compression
+gzip compressed data, was "ofscraper-2.1.tar", max compression
```

## Comparing `ofscraper-2.0.1.tar` & `ofscraper-2.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0     1067 2023-05-25 21:03:02.597295 ofscraper-2.0.1/LICENSE
--rw-r--r--   0        0        0     5192 2023-05-25 21:03:02.601295 ofscraper-2.0.1/README.md
--rw-r--r--   0        0        0      607 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/__init__.py
--rw-r--r--   0        0        0      999 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/__version__.py
--rw-r--r--   0        0        0        1 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     1986 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/highlights.py
--rw-r--r--   0        0        0      838 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/init.py
--rw-r--r--   0        0        0     2243 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/me.py
--rw-r--r--   0        0        0     5671 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/messages.py
--rw-r--r--   0        0        0     1884 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/paid.py
--rw-r--r--   0        0        0     9037 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/posts.py
--rw-r--r--   0        0        0     2841 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/profile.py
--rw-r--r--   0        0        0     1867 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     8069 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/api/timeline.py
--rw-r--r--   0        0        0     4999 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/db/__init__.py
--rw-r--r--   0        0        0     6759 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3199 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     4053 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/interaction/like.py
--rw-r--r--   0        0        0     5477 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/prompts/prompt_functions.py
--rw-r--r--   0        0        0      359 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0    20976 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/prompts/prompts.py
--rwxr-xr-x   0        0        0    23572 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/scraper.py
--rw-r--r--   0        0        0        1 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     4320 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/args.py
--rw-r--r--   0        0        0     8996 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/auth.py
--rw-r--r--   0        0        0    10859 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/config.py
--rw-r--r--   0        0        0      257 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/console.py
--rw-r--r--   0        0        0      993 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    17889 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2938 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     2381 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     4408 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/logger.py
--rw-r--r--   0        0        0     5220 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     3008 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      779 2023-05-25 21:03:03.557340 ofscraper-2.0.1/ofscraper/utils/separate.py
--rw-r--r--   0        0        0     1528 2023-05-25 21:03:36.441192 ofscraper-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     6595 1970-01-01 00:00:00.000000 ofscraper-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-27 02:37:19.645984 ofscraper-2.1/LICENSE
+-rw-r--r--   0        0        0     5192 2023-05-27 02:37:19.645984 ofscraper-2.1/README.md
+-rw-r--r--   0        0        0      607 2023-05-27 02:37:20.529999 ofscraper-2.1/ofscraper/__init__.py
+-rw-r--r--   0        0        0      999 2023-05-27 02:37:20.529999 ofscraper-2.1/ofscraper/__version__.py
+-rw-r--r--   0        0        0        1 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     1986 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0      979 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/init.py
+-rw-r--r--   0        0        0     2264 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/me.py
+-rw-r--r--   0        0        0     5599 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     1884 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     9037 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/posts.py
+-rw-r--r--   0        0        0     2841 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     1867 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     7882 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0     5033 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0     6759 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3199 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     4028 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0     5477 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/prompts/prompt_functions.py
+-rw-r--r--   0        0        0      359 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    20976 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/prompts/prompts.py
+-rwxr-xr-x   0        0        0    25673 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/scraper.py
+-rw-r--r--   0        0        0        1 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     4373 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     8996 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0    10857 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      257 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      993 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    18388 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2865 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     2381 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     5105 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0     5220 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     3060 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      779 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      674 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0     1509 2023-05-27 02:37:53.298575 ofscraper-2.1/pyproject.toml
+-rw-r--r--   0        0        0     6554 1970-01-01 00:00:00.000000 ofscraper-2.1/PKG-INFO
```

### Comparing `ofscraper-2.0.1/LICENSE` & `ofscraper-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/README.md` & `ofscraper-2.1/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/ofscraper/__init__.py` & `ofscraper-2.1/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/ofscraper/__version__.py` & `ofscraper-2.1/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/ofscraper/api/highlights.py` & `ofscraper-2.1/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/ofscraper/api/me.py` & `ofscraper-2.1/ofscraper/api/me.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import logging
 import httpx
 from rich.console import Console
 from tenacity import retry,stop_after_attempt,wait_random
 import ofscraper.constants as constants
 import ofscraper.utils.auth as auth
 import ofscraper.utils.encoding as encoding
+import ofscraper.utils.stdout as stdout
 from ofscraper.utils.logger import updateSenstiveDict
 log=logging.getLogger(__package__)
 console=Console()
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=2, max=6),reraise=True,after=lambda retry_state:print(f"Attempting to login attempt:{retry_state.attempt_number}/5")) 
 def scrape_user(headers):
     with httpx.Client(http2=True, headers=headers) as c:
@@ -40,15 +41,15 @@
     name = encoding.encode_utf_16(profile['name'])
     username = profile['username']
 
     return (name, username)
 
 
 def print_user(name, username):
-    if log.level<=constants.SUPPRESS_LOG_LEVEL:
+    with stdout.lowstdout():
         console.print(f'Welcome, {name} | {username}')
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
 def parse_subscriber_count(headers):
     with httpx.Client(http2=True, headers=headers) as c:
         url = constants.subscribeCountEP
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
```

### Comparing `ofscraper-2.0.1/ofscraper/api/messages.py` & `ofscraper-2.1/ofscraper/api/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     global sem
     sem = asyncio.Semaphore(8)
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue"),),TextColumn("Getting Messages...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
-    with Live(progress_group, refresh_per_second=10,console=console.shared_console): 
+    with Live(progress_group, refresh_per_second=constants.refreshScreen,console=console.shared_console): 
 
         oldmessages=cache.get(f"messages_{model_id}",default=[]) 
         oldmsgset=set(map(lambda x:x.get("id"),oldmessages))
         log.debug(f"[bold]Messages Cache[/bold] {len(oldmessages)} found")
         oldmessages=list(filter(lambda x:x.get("createdAt")!=None,oldmessages))
         postedAtArray=list(map(lambda x:x["id"],sorted(oldmessages,key=lambda x:arrow.get(x["createdAt"]).float_timestamp,reverse=True)))
         global tasks
@@ -68,15 +68,15 @@
             tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress,recursive=True)))
     
     
         
         
         responseArray=[]
         page_count=0 
-        page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=False if logging.getLogger("ofscraper").handlers[1].level>=constants.SUPPRESS_LOG_LEVEL else True)
+        page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
 
 
         while len(tasks)!=0:
                     for coro in asyncio.as_completed(tasks):
                         result=await coro or []
                         page_count=page_count+1
                         overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
```

### Comparing `ofscraper-2.0.1/ofscraper/api/paid.py` & `ofscraper-2.1/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/ofscraper/api/posts.py` & `ofscraper-2.1/ofscraper/api/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/ofscraper/api/profile.py` & `ofscraper-2.1/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/ofscraper/api/subscriptions.py` & `ofscraper-2.1/ofscraper/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/ofscraper/api/timeline.py` & `ofscraper-2.1/ofscraper/api/timeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         ep = constants.timelineNextEP
         url = ep.format(model_id, timestamp)
     else:
         ep=constants.timelineEP
         url=ep.format(model_id)
     log.debug(url)
     async with sem:
-        task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Timestamp -> {arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}",visible=False if logging.getLogger("ofscraper").handlers[1].level>=constants.SUPPRESS_LOG_LEVEL else True)
+        task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Timestamp -> {arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}",visible=True)
 
         async with httpx.AsyncClient(http2=True, headers=headers) as c:
             auth.add_cookies(c)
             c.headers.update(auth.create_sign(url, headers))
             r = await c.get(url , timeout=None)
             if not r.is_error:
                 progress.remove_task(task)
@@ -96,15 +96,15 @@
     global sem
     sem = asyncio.Semaphore(8)
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting timeline media...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
-    with Live(progress_group, refresh_per_second=10,console=console.shared_console): 
+    with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
 
         oldtimeline=cache.get(f"timeline_{model_id}",default=[]) 
         oldtimeset=set(map(lambda x:x.get("id"),oldtimeline))
         log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
         oldtimeline=list(filter(lambda x:x.get("postedAtPrecise")!=None,oldtimeline))
         postedAtArray=sorted(list(map(lambda x:float(x["postedAtPrecise"]),oldtimeline)))
         global tasks
@@ -125,15 +125,15 @@
         else:
             tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,recursive=True)))
 
         responseArray=[]
     
     
         page_count=0 
-        page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=False if logging.getLogger("ofscraper").handlers[1].level>=constants.SUPPRESS_LOG_LEVEL else True)
+        page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
         while len(tasks)!=0:
             for coro in asyncio.as_completed(tasks):
                 result=await coro or []
                 page_count=page_count+1
                 overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
                 responseArray.extend(result)
             time.sleep(2)
```

### Comparing `ofscraper-2.0.1/ofscraper/constants.py` & `ofscraper-2.1/ofscraper/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,8 +104,10 @@
             "highlights":"stories",
             "profile":"profile",
             "pinned":"posts"
         }
 NUM_TRIES=5
 RESPONSE_EXPIRY=5000000
 LICENCE_URL="https://onlyfans.com/api2/v2/users/media/{}/drm/{}/{}?type=widevine"
-logname="ofscraper"
+logname="ofscraper"
+PATH_STR_MAX=200
+refreshScreen=20
```

### Comparing `ofscraper-2.0.1/ofscraper/db/operations.py` & `ofscraper-2.1/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/ofscraper/db/queries.py` & `ofscraper-2.1/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/ofscraper/interaction/like.py` & `ofscraper-2.1/ofscraper/interaction/like.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import random
 import time
 import logging
 from typing import Union
 import asyncio
 import httpx
 
-from halo import Halo
 log=logging.getLogger(__package__)
 
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     MofNCompleteColumn,
     BarColumn,
@@ -107,8 +106,8 @@
             if 'error' in json and 'message' in json['error']:
                 message = json['error']['message']
             status = f'STATUS CODE {param.status_code}: '
         else:
             message = str(param)
     except:
         pass
-    log.warning(f'{status}{message}, post at {url}')
+    log.info(f'{status}{message}, post at {url}')
```

### Comparing `ofscraper-2.0.1/ofscraper/prompts/prompt_functions.py` & `ofscraper-2.1/ofscraper/prompts/prompt_functions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/ofscraper/prompts/prompts.py` & `ofscraper-2.1/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/ofscraper/scraper.py` & `ofscraper-2.1/ofscraper/scraper.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import asyncio
+import time
 import os
 import sys
 import platform
 import time
 import traceback
 import schedule
 import threading
@@ -21,16 +22,22 @@
 import textwrap
 from contextlib import contextmanager
 import timeit
 from itertools import chain
 import re
 from rich.console import Console
 import webbrowser
-from halo import Halo
 import arrow
+from rich.progress import (
+    Progress,
+    TextColumn,
+    SpinnerColumn
+)
+from rich.style import Style
+
 import ofscraper.prompts.prompts as prompts
 import ofscraper.api.messages as messages
 import ofscraper.db.operations as operations
 import ofscraper.api.posts as posts_
 import ofscraper.utils.args as args_
 import ofscraper.utils.paths as paths
 import ofscraper.utils.exit as exit
@@ -44,126 +51,139 @@
 import ofscraper.utils.auth as auth
 import ofscraper.utils.profiles as profiles
 import ofscraper.api.init as init
 import ofscraper.utils.download as download
 import ofscraper.interaction.like as like
 import ofscraper.utils.logger as logger
 import ofscraper.utils.args as args_
-import ofscraper.constants as constants
 import ofscraper.utils.filters as filters
+import ofscraper.utils.stdout as stdout
+import ofscraper.utils.console as console
 
-
-
-console=Console()
 log=logger.init_logger(logging.getLogger(__package__))
 args=args_.getargs()
 log.debug(args)
-f = open(os.devnull, 'w')
-
 def process_messages(headers, model_id,username):
-    messages_ =asyncio.run(messages.get_messages(headers,  model_id)) 
-    messages_=list(map(lambda x:posts_.Post(x,model_id,username),messages_))
-    log.debug(f"[bold]Messages Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),messages_))}")
-    log.debug("Removing locked messages media")
-    for message in messages_:
-     operations.write_messages_table(message)
-    output=[]
-    [ output.extend(message.media) for message in messages_]
-    return list(filter(lambda x:isinstance(x,posts_.Media),output))
+    with stdout.lowstdout():
+        with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
+
+            messages_ =asyncio.run(messages.get_messages(headers,  model_id)) 
+            messages_=list(map(lambda x:posts_.Post(x,model_id,username),messages_))
+            log.debug(f"[bold]Messages Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),messages_))}")
+            log.debug("Removing locked messages media")
+            for message in messages_:
+                operations.write_messages_table(message)
+            output=[]
+            [ output.extend(message.media) for message in messages_]
+            return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
-@Halo(stream=sys.stdout if logging.getLogger("ofscraper").handlers[1].level<constants.SUPPRESS_LOG_LEVEL else f,text='Getting Paid Content...')
 def process_paid_post(model_id,username):
-    paid_content=paid.scrape_paid(username)
-    paid_content=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="paid"),paid_content))
-    log.debug(f"[bold]Paid Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),paid_content))}")
-    log.debug("Removing locked paid media")
-    for post in paid_content:
-        operations.write_post_table(post,model_id,username)
-    output=[]
-    [output.extend(post.media) for post in paid_content]
-    return list(filter(lambda x:isinstance(x,posts_.Media),output))
+    with stdout.lowstdout():
+        with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
+            task1=progress.add_task("Getting Paid Media....")
+            paid_content=paid.scrape_paid(username)
+            paid_content=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="paid"),paid_content))
+            log.debug(f"[bold]Paid Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),paid_content))}")
+            log.debug("Removing locked paid media")
+            for post in paid_content:
+                operations.write_post_table(post,model_id,username)
+            output=[]
+            [output.extend(post.media) for post in paid_content]
+            progress.remove_task(task1)
+            return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
          
 
-@Halo(stream=sys.stdout  if logging.getLogger("ofscraper").handlers[1].level<constants.SUPPRESS_LOG_LEVEL else f,text='Getting highlights and stories...\n')
 def process_highlights(headers, model_id,username):
-    highlights_, stories = highlights.scrape_highlights(headers, model_id)
-    highlights_, stories=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="highlights"),highlights_)),\
-    list(map(lambda x:posts_.Post(x,model_id,username,responsetype="stories"),stories))
-    log.debug(f"[bold]Combined Story and Highlight Media count[/bold] {sum(map(lambda x:len(x.allmedia), highlights_))+sum(map(lambda x:len(x.allmedia), stories))}")
-    for post in highlights_:
-        operations.write_stories_table(post,model_id,username)
-    for post in stories:
-        operations.write_stories_table(post,model_id,username)   
-    output=[]
-    output2=[]
-    [ output.extend(highlight.media) for highlight in highlights_]
-    [ output2.extend(stories.media) for stories in stories]
-    return list(filter(lambda x:isinstance(x,posts_.Media),output)),list(filter(lambda x:isinstance(x,posts_.Media),output2))
+    with stdout.lowstdout():
+        with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
+            task1=progress.add_task("Highlights and Stories....")
+            highlights_, stories = highlights.scrape_highlights(headers, model_id)
+            highlights_, stories=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="highlights"),highlights_)),\
+            list(map(lambda x:posts_.Post(x,model_id,username,responsetype="stories"),stories))
+            log.debug(f"[bold]Combined Story and Highlight Media count[/bold] {sum(map(lambda x:len(x.allmedia), highlights_))+sum(map(lambda x:len(x.allmedia), stories))}")
+            for post in highlights_:
+                operations.write_stories_table(post,model_id,username)
+            for post in stories:
+                operations.write_stories_table(post,model_id,username)   
+            output=[]
+            output2=[]
+            [ output.extend(highlight.media) for highlight in highlights_]
+            [ output2.extend(stories.media) for stories in stories]
+            progress.remove_task(task1)
+            return list(filter(lambda x:isinstance(x,posts_.Media),output)),list(filter(lambda x:isinstance(x,posts_.Media),output2))
 
-     
+            
 
 
 
 
 
 
-# @Halo(stream=sys.stdout if logging.getLogger("ofscraper").handlers[1].level<constants.SUPPRESS_LOG_LEVEL else f,text='Getting timeline media...')
 def process_timeline_posts(headers, model_id,username):
-    timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id))
-    timeline_posts  =list(map(lambda x:posts_.Post(x,model_id,username,"timeline"), timeline_posts ))
-    log.debug(f"[bold]Timeline Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),timeline_posts))}")
-    log.debug("Removing locked timeline media")
-    for post in timeline_posts:
-        operations.write_post_table(post,model_id,username)
-    output=[]
-    [output.extend(post.media) for post in  timeline_posts ]
-    return list(filter(lambda x:isinstance(x,posts_.Media),output))
+    with stdout.lowstdout():
+        with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
+            timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id))
+            timeline_posts  =list(map(lambda x:posts_.Post(x,model_id,username,"timeline"), timeline_posts ))
+            log.debug(f"[bold]Timeline Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),timeline_posts))}")
+            log.debug("Removing locked timeline media")
+            for post in timeline_posts:
+                operations.write_post_table(post,model_id,username)
+            output=[]
+            [output.extend(post.media) for post in  timeline_posts ]
+            return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
-@Halo(stream=sys.stdout if logging.getLogger("ofscraper").handlers[1].level<constants.SUPPRESS_LOG_LEVEL else f,text='Getting archived media...')
 def process_archived_posts(headers, model_id,username):
-    archived_posts = timeline.get_archive_post(headers, model_id)
-    archived_posts =list(map(lambda x:posts_.Post(x,model_id,username),archived_posts ))
-    log.debug(f"[bold]Archived Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),archived_posts))}")
-    log.debug("Removing locked archived media")
-
-    for post in archived_posts:
-        operations.write_post_table(post,model_id,username)
-    output=[]
-    [ output.extend(post.media) for post in archived_posts ]
-    return list(filter(lambda x:isinstance(x,posts_.Media),output))
+    with stdout.lowstdout():
+        with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
+            task1=progress.add_task("Getting Archived Media....")
+            archived_posts = timeline.get_archive_post(headers, model_id)
+            archived_posts =list(map(lambda x:posts_.Post(x,model_id,username),archived_posts ))
+            log.debug(f"[bold]Archived Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),archived_posts))}")
+            log.debug("Removing locked archived media")
+
+            for post in archived_posts:
+                operations.write_post_table(post,model_id,username)
+            output=[]
+            [ output.extend(post.media) for post in archived_posts ]
+            progress.remove_task(task1)
+            return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
 
 
 
-@Halo(stream=sys.stdout if logging.getLogger("ofscraper").handlers[1].level<constants.SUPPRESS_LOG_LEVEL else f,text='Getting pinned media...')
 def process_pinned_posts(headers, model_id,username):
-    pinned_posts = timeline.get_pinned_post(headers, model_id,username)
-    pinned_posts =list(map(lambda x:posts_.Post(x,model_id,username,"pinned"),pinned_posts ))
-    log.debug(f"[bold]Pinned Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),pinned_posts))}")
-    log.debug("Removing locked pinned media")
-    for post in  pinned_posts:
-        operations.write_post_table(post,model_id,username)
-    output=[]
-    [ output.extend(post.media) for post in pinned_posts ]
-    return list(filter(lambda x:isinstance(x,posts_.Media),output))
+    with stdout.lowstdout():
+        with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
+            task1=progress.add_task("Getting Pinned Media....")
+            pinned_posts = timeline.get_pinned_post(headers, model_id,username)
+            pinned_posts =list(map(lambda x:posts_.Post(x,model_id,username,"pinned"),pinned_posts ))
+            log.debug(f"[bold]Pinned Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),pinned_posts))}")
+            log.debug("Removing locked pinned media")
+            for post in  pinned_posts:
+                operations.write_post_table(post,model_id,username)
+            output=[]
+            [ output.extend(post.media) for post in pinned_posts ]
+            progress.remove_task(task1)
+            return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
 def process_profile(headers, username) -> list:
-    user_profile = profile.scrape_profile(headers, username)
-    urls, info = profile.parse_profile(user_profile)
-    profile.print_profile_info(info)       
-    output=[]
-    for ele in enumerate(urls):
-        count=ele[0]
-        data=ele[1]
-        output.append(posts_.Media({"url":data["url"],"type":data["mediatype"]},count,posts_.Post(data,info[2],username,responsetype="profile")))
-    avatars=list(filter(lambda x:x.filename=='avatar',output))
-    if len(avatars)>0:
-        log.warning(f"Avatar : {avatars[0].url}")
-    return output
+    with stdout.lowstdout():
+        user_profile = profile.scrape_profile(headers, username)
+        urls, info = profile.parse_profile(user_profile)
+        profile.print_profile_info(info)       
+        output=[]
+        for ele in enumerate(urls):
+            count=ele[0]
+            data=ele[1]
+            output.append(posts_.Media({"url":data["url"],"type":data["mediatype"]},count,posts_.Post(data,info[2],username,responsetype="profile")))
+        avatars=list(filter(lambda x:x.filename=='avatar',output))
+        if len(avatars)>0:
+            log.warning(f"Avatar : {avatars[0].url}")
+        return output
 
 
 
 def process_areas(headers, ele, model_id) -> list:
     args.posts = list(map(lambda x:x.capitalize(),(args.posts or prompts.areas_prompt())
 ))
     timeline_posts_dicts  = []
@@ -224,24 +244,27 @@
   
 def get_model_inputsplit(commaString):
     def hyphenRange(hyphenString):
         x = [int(x) for x in hyphenString.split('-')]
         return range(x[0], x[-1]+1)
     return chain(*[hyphenRange(r) for r in list(filter(lambda x:x.isdigit(),re.split(',| ',commaString)))])
 
-@Halo(stream=sys.stdout if logging.getLogger("ofscraper").handlers[1].level<constants.SUPPRESS_LOG_LEVEL else f,text='Getting your subscriptions (this may take awhile)...') 
 def get_models(headers, subscribe_count) -> list:
     """
     Get user's subscriptions in form of a list.
     """
-    list_subscriptions = asyncio.run(
-        subscriptions.get_subscriptions(headers, subscribe_count))
-    parsed_subscriptions = subscriptions.parse_subscriptions(
-        list_subscriptions)
-    return parsed_subscriptions
+    with stdout.lowstdout():
+        with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
+            task1=progress.add_task('Getting your subscriptions (this may take awhile)...')
+            list_subscriptions = asyncio.run(
+                subscriptions.get_subscriptions(headers, subscribe_count))
+            parsed_subscriptions = subscriptions.parse_subscriptions(
+                list_subscriptions)
+            progress.remove_task(task1)
+            return parsed_subscriptions
 
 #check if auth is valid
 def process_me(headers):
     my_profile = me.scrape_user(headers)
     name, username = me.parse_user(my_profile)
     subscribe_count=me.parse_subscriber_count(headers)
     me.print_user(name, username)
@@ -383,35 +406,37 @@
         
 
 def process_like():
     with scrape_context_manager():
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
         userdata=getselected_usernames()
-        for ele in list(filter(lambda x: x["active"],userdata)):
-                model_id = profile.get_id(headers, ele["name"])
-                posts = like.get_posts(headers, model_id)
-                unfavorited_posts = like.filter_for_unfavorited(posts)  
-                unfavorited_posts=filters.timeline_array_filter(unfavorited_posts)             
-                post_ids = like.get_post_ids(unfavorited_posts)
-                like.like(headers, model_id, ele["name"], post_ids)
+        with stdout.lowstdout():
+            for ele in list(filter(lambda x: x["active"],userdata)):
+                    model_id = profile.get_id(headers, ele["name"])
+                    posts = like.get_posts(headers, model_id)
+                    unfavorited_posts = like.filter_for_unfavorited(posts)  
+                    unfavorited_posts=filters.timeline_array_filter(unfavorited_posts)             
+                    post_ids = like.get_post_ids(unfavorited_posts)
+                    like.like(headers, model_id, ele["name"], post_ids)
 
 def process_unlike():
     with scrape_context_manager(): 
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
         init.print_sign_status(headers)
         userdata=getselected_usernames()
-        for ele in list(filter(lambda x: x["active"],userdata)):
-                model_id = profile.get_id(headers, ele["name"])
-                posts = like.get_posts(headers, model_id)
-                favorited_posts = like.filter_for_favorited(posts)
-                favorited_posts=filters.timeline_array_filter(favorited_posts) 
-                post_ids = like.get_post_ids(favorited_posts)
-                like.unlike(headers, model_id, ele["name"], post_ids)
+        with stdout.lowstdout():
+            for ele in list(filter(lambda x: x["active"],userdata)):
+                    model_id = profile.get_id(headers, ele["name"])
+                    posts = like.get_posts(headers, model_id)
+                    favorited_posts = like.filter_for_favorited(posts)
+                    favorited_posts=filters.timeline_array_filter(favorited_posts) 
+                    post_ids = like.get_post_ids(favorited_posts)
+                    like.unlike(headers, model_id, ele["name"], post_ids)
 #Adds a function to the job queue
 def set_schedule(*functs):
     [schedule.every(args.daemon).minutes.do(jobqueue.put,funct) for funct in functs]
     while True:
         schedule.run_pending()
         time.sleep(30)
 
@@ -455,19 +480,19 @@
             auth.make_auth(auth=auth.read_auth())
             continue
         break
         
 
 def check_config():
     while not  paths.mp4decryptchecker(config.get_mp4decrypt(config.read_config())):
-        console.print("You need to select path for mp4decrypt\n\n")
+        console.shared_console.print("You need to select path for mp4decrypt\n\n")
         log.debug(f"[bold]current mp4decrypt path[/bold] {config.get_mp4decrypt(config.read_config())}")
         config.update_mp4decrypt()
     while not  paths.ffmpegchecker(config.get_ffmpeg(config.read_config())):
-        console.print("You need to select path for ffmpeg\n\n")
+        console.shared_console.print("You need to select path for ffmpeg\n\n")
         log.debug(f"[bold]current ffmpeg path[/bold] {config.get_ffmpeg(config.read_config())}")
         config.update_ffmpeg()
     log.debug(f"[bold]final mp4decrypt path[/bold] {config.get_mp4decrypt(config.read_config())}")
     log.debug(f"[bold]final ffmpeg path[/bold] {config.get_ffmpeg(config.read_config())}")
 
 
 def getselected_usernames():
@@ -566,44 +591,59 @@
         end=timeit.default_timer()
         log.error(f"""
 ===========================
 [bold]Script Finished[/bold]
 Run Time:  [bold]{str(arrow.get(end)-arrow.get(start)).split(".")[0]}[/bold]
 ===========================
 """)
-        None   
+def print_start():
+    with stdout.lowstdout():
+        console.shared_console.print(
+            f"[bold green]Welcome to OF-Scraper Version {args.version}[/bold green]"
+        )                
 def main():
-    
-# Python program for creating a
-# context manager using @contextmanager
-# decorator
  
-    with exit.DelayedKeyboardInterrupt(paths.cleanup,False):
         try:
-            scrapper()        
-        except Exception as E:
-            log.traceback(E)
-            log.traceback(traceback.format_exc())
-        quit()
-def scrapper():
-    import time
+            print_start()
+            scrapper()
+            paths.cleanup()
+            logger.discord_cleanup()
+        except KeyboardInterrupt as E:
+            try:
+                with exit.DelayedKeyboardInterrupt():
+                    paths.cleanup()
+                    logger.discord_cleanup()
+                    sys.exit(0)
+            except KeyboardInterrupt:
+                    sys.exit(0)
 
 
+        except Exception as E:
+            try:
+                with exit.DelayedKeyboardInterrupt():
+                    paths.cleanup()
+                    logger.discord_cleanup()
+                    log.traceback(E)
+                    log.traceback(traceback.format_exc())
+                    sys.exit(0)
+            except KeyboardInterrupt:
+                sys.exit(0)
+def scrapper():
     if platform.system == 'Windows':
         os.system('color')
     # try:
     #     webbrowser.open(donateEP)
     # except:
     #     pass
     global selectedusers
     selectedusers=None
     functs=[]
     if len(args.posts)==0 and not args.action:
         if args.daemon:
-                    log.warning("You need to pass at least one scraping method\n--action\n--posts\n--purchase\nAre all valid options. Skipping and going to menu")
+                    log.error("You need to pass at least one scraping method\n--action\n--posts\n--purchase\nAre all valid options. Skipping and going to menu")
         process_prompts()
         return
     check_auth()
     check_config()
     if len(args.posts)>0: 
         functs.append(process_post)      
     elif args.action=="like":
```

### Comparing `ofscraper-2.0.1/ofscraper/utils/args.py` & `ofscraper-2.1/ofscraper/utils/args.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,34 +15,34 @@
     elif input==None:
         input=sys.argv[1:]
 
     parser = argparse.ArgumentParser()
 
     parser = argparse.ArgumentParser(add_help=False)   
     general=parser.add_argument_group("General",description="General Args")  
-    general.add_argument('-v', '--version', action='version', version=__version__ )
+    general.add_argument('-v', '--version', action='version', version=__version__ ,default=__version__)
     general.add_argument('-h', '--help', action='help')
 
                                     
     general.add_argument(
         '-u', '--username', help="select which username to process (name,name2)\nSet to ALL for all users",type=lambda x: list(filter( lambda y:y!="",x.split(",")))
     )
     general.add_argument(
         '-d', '--daemon', help='run script in the background\nSet value to minimum minutes between script runs\nOverdue runs will run as soon as previous run finishes', type=int,default=None
     )
 
     general.add_argument(
-        '-l', '--log', help = 'set log file level', type=str.upper,default="OFF",choices=["OFF","LOW","NORMAL","DEBUG"]
+        '-l', '--log', help = 'set log file level', type=str.upper,default="OFF",choices=["OFF","STATS","LOW","NORMAL","DEBUG"]
     ),
     general.add_argument(
-        '-dc', '--discord', help = 'set discord log level', type=str.upper,default="OFF",choices=["OFF","LOW","NORMAL","DEBUG"]
+        '-dc', '--discord', help = 'set discord log level', type=str.upper,default="OFF",choices=["OFF","STATS","LOW","NORMAL","DEBUG"]
     )
 
     general.add_argument(
-        '-p', '--output', help = 'set output log level', type=str.upper,default="NORMAL",choices=["PROMPT","LOW","NORMAL","DEBUG"]
+        '-p', '--output', help = 'set output log level', type=str.upper,default="NORMAL",choices=["PROMPT","STATS","LOW","NORMAL","DEBUG"]
     )
     post=parser.add_argument_group("Post",description="What type of post to scrape")                                      
 
     post.add_argument("-e","--dupe",action="store_true",default=False,help="Bypass the dupe check and redownload all files")
     post.add_argument(
         '-o', '--posts', help = 'Download content from a model',default=[],required=False,type = posttype_helper,action='extend'
     )
@@ -58,23 +58,23 @@
     filters.add_argument(
         '-r', '--renewal', help = 'Filter by whether renewal is on or off for account',default=None,required=False,type = str.lower,choices=["active","disabled"]
     )
     filters.add_argument(
         '-ss', '--sub-status', help = 'Filter by whether or not your subscription has expired or not',default=None,required=False,type = str.lower,choices=["active","expired"]
     )
     filters.add_argument(
-        '-be', '--before', help = 'Process post at or before the given date general synax is Month/Day/Year\nWorks for like,unlike, and scraping posts',type=arrow.get)
+        '-be', '--before', help = 'Process post at or before the given date general synax is Month/Day/Year\nWorks for like,unlike, and downloading posts',type=arrow.get)
  
     filters.add_argument(
-        '-af', '--after', help = 'Process post at or after the given date Month/Day/Year\nnWorks for like,unlike, and scraping posts',type=arrow.get)
+        '-af', '--after', help = 'Process post at or after the given date Month/Day/Year\nnWorks for like,unlike, and downloading posts',type=arrow.get)
     
     
     advanced=parser.add_argument_group("Advanced",description="Advanced Args")  
     advanced.add_argument(
-        '-uf', '--users-first', help = 'Scrape all users first rather then one at a time. This only effects scraping posts',default=False,required=False,action="store_true"
+        '-uf', '--users-first', help = 'Scrape all users first rather then one at a time. This only effects downloading posts',default=False,required=False,action="store_true"
     )
 
     args=parser.parse_args(input)
     #deduplicate posts
     args.posts=list(set(args.posts or []))
     return args
```

### Comparing `ofscraper-2.0.1/ofscraper/utils/auth.py` & `ofscraper-2.1/ofscraper/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/ofscraper/utils/config.py` & `ofscraper-2.1/ofscraper/utils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     config['config'].update({field: value})
 
     with open(p, 'w') as f:
         f.write(json.dumps(config, indent=4))
 
 
 def auto_update_config(path, config: dict) -> dict:
-    log.warning("Auto updating config...")
+    log.error("Auto updating config...")
     new_config = get_current_config_schema(config)
 
     with open(path / constants.configFile, 'w') as f:
         f.write(json.dumps(new_config, indent=4))
 
     return new_config
```

### Comparing `ofscraper-2.0.1/ofscraper/utils/dates.py` & `ofscraper-2.1/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/ofscraper/utils/download.py` & `ofscraper-2.1/ofscraper/utils/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,21 @@
 from rich.progress import (
     Progress,
     TimeElapsedColumn,
     TotalFileSizeColumn,
     TransferSpeedColumn,
     TextColumn,
     TaskProgressColumn,
-    BarColumn
+    BarColumn,
+    TimeRemainingColumn
 )
 from rich.live import Live
 from rich.panel import Panel
 from rich.console import Group
+from rich.table import Column
 import arrow
 from bs4 import BeautifulSoup
 try:
     from win32_setctime import setctime  # pylint: disable=import-error
 except ModuleNotFoundError:
     pass
 from tenacity import retry,stop_after_attempt,wait_random,retry_if_result
@@ -48,122 +50,126 @@
 import ofscraper.db.operations as operations
 import ofscraper.utils.paths as paths
 import ofscraper.utils.auth as auth
 import ofscraper.constants as constants
 import ofscraper.utils.dates as dates
 import ofscraper.utils.logger as logger
 import ofscraper.utils.console as console
+import ofscraper.utils.stdout as stdout
 from diskcache import Cache
 
 cache = Cache(paths.getcachepath())
 attempt = contextvars.ContextVar("attempt")
 log=logging.getLogger(__package__)
 
 
 async def process_dicts(username, model_id, medialist,forced=False):
-    overall_progress=Progress(  TextColumn("{task.description}"),
-    BarColumn(),TaskProgressColumn(),TimeElapsedColumn())
-    job_progress=Progress(*Progress.get_default_columns(),TransferSpeedColumn(),TotalFileSizeColumn())
-    progress_group = Group(
-    overall_progress
-    , Panel(Group(job_progress)))
-    with Live(progress_group, refresh_per_second=10,console=console.shared_console):    
-            if not forced:
-                media_ids = set(operations.get_media_ids(model_id,username))
-                medialist = seperate.separate_by_id(medialist, media_ids)
-                log.info(f"Skipping previously downloaded\nMedia left for download {len(medialist)}")
-            else:
-                log.info("forcing all downloads")
-            file_size_limit = config_.get_filesize()
-            global sem
-            sem = asyncio.Semaphore(8)
-        
-            aws=[]
-            photo_count = 0
-            video_count = 0
-            audio_count=0
-            skipped = 0
-            total_bytes_downloaded = 0
-            data = 0
-            desc = 'Progress: ({p_count} photos, {v_count} videos, {a_count} audios,  {skipped} skipped || {sumcount}/{mediacount}||{data})'    
-        
+    with stdout.lowstdout():
+        overall_progress=Progress(  TextColumn("{task.description}"),
+        BarColumn(),TaskProgressColumn(),TimeElapsedColumn())
+        job_progress=Progress(TextColumn("{task.description}",table_column=Column(ratio=2)),BarColumn(),
+        TaskProgressColumn(),TimeRemainingColumn(),TransferSpeedColumn(),TotalFileSizeColumn())
+        progress_group = Group(
+        overall_progress
+        , Panel(Group(job_progress,fit=True)))
+        with Live(progress_group, refresh_per_second=constants.refreshScreen,console=console.shared_console):    
+                if not forced:
+                    media_ids = set(operations.get_media_ids(model_id,username))
+                    medialist = seperate.separate_by_id(medialist, media_ids)
+                    log.info(f"Skipping previously downloaded\nMedia left for download {len(medialist)}")
+                else:
+                    log.info("forcing all downloads")
+                file_size_limit = config_.get_filesize()
+                global sem
+                sem = asyncio.Semaphore(8)
             
-
+                aws=[]
+                photo_count = 0
+                video_count = 0
+                audio_count=0
+                skipped = 0
+                total_bytes_downloaded = 0
+                data = 0
+                desc = 'Progress: ({p_count} photos, {v_count} videos, {a_count} audios,  {skipped} skipped || {sumcount}/{mediacount}||{data})'    
             
-            for ele in medialist:
-                with paths.set_directory(paths.getmediadir(ele,username,model_id)):
-                    aws.append(asyncio.create_task(download(ele,pathlib.Path(".").absolute() ,model_id, username,file_size_limit,job_progress)))
-            task1 = overall_progress.add_task(desc.format(p_count=photo_count, v_count=video_count,a_count=audio_count, skipped=skipped,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped,data=data), total=len(aws),visible=False if logging.getLogger("ofscraper").handlers[1].level>=constants.SUPPRESS_LOG_LEVEL else True)
-            for coro in asyncio.as_completed(aws):
-                    try:
-                        media_type, num_bytes_downloaded = await coro
-                    except Exception as e:
-                        log.traceback(e)
-                        log.traceback(traceback.format_exc())
-                        media_type = "skipped"
-                        num_bytes_downloaded = 0
-
-                    total_bytes_downloaded += num_bytes_downloaded
-                    data = convert_num_bytes(total_bytes_downloaded)
-                    if media_type == 'images':
-                        photo_count += 1 
-
-                    elif media_type == 'videos':
-                        video_count += 1
-                    elif media_type == 'audios':
-                        audio_count += 1
-                    elif media_type == 'skipped':
-                        skipped += 1
-                    overall_progress.update(task1,description=desc.format(
-                                p_count=photo_count, v_count=video_count, a_count=audio_count,skipped=skipped, data=data,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped), refresh=True, advance=1)
-    overall_progress.remove_task(task1)
-    log.warning(f'[bold]{username}[/bold] ({photo_count} photos, {video_count} videos, {audio_count} audios,  {skipped} skipped)' )
+                
+
+                
+                for ele in medialist:
+                    with paths.set_directory(paths.getmediadir(ele,username,model_id)):
+                        aws.append(asyncio.create_task(download(ele,pathlib.Path(".").absolute() ,model_id, username,file_size_limit,job_progress)))
+                task1 = overall_progress.add_task(desc.format(p_count=photo_count, v_count=video_count,a_count=audio_count, skipped=skipped,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped,data=data), total=len(aws),visible=True)
+                # progress_group.renderables[1].height=max(15,console.shared_console.size[1]-2)
+                for coro in asyncio.as_completed(aws):
+                        try:
+                            media_type, num_bytes_downloaded = await coro
+                        except Exception as e:
+                            log.traceback(e)
+                            log.traceback(traceback.format_exc())
+                            media_type = "skipped"
+                            num_bytes_downloaded = 0
+
+                        total_bytes_downloaded += num_bytes_downloaded
+                        data = convert_num_bytes(total_bytes_downloaded)
+                        if media_type == 'images':
+                            photo_count += 1 
+
+                        elif media_type == 'videos':
+                            video_count += 1
+                        elif media_type == 'audios':
+                            audio_count += 1
+                        elif media_type == 'skipped':
+                            skipped += 1
+                        overall_progress.update(task1,description=desc.format(
+                                    p_count=photo_count, v_count=video_count, a_count=audio_count,skipped=skipped, data=data,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped), refresh=True, advance=1)
+        overall_progress.remove_task(task1)
+    log.error(f'[bold]{username}[/bold] ({photo_count} photos, {video_count} videos, {audio_count} audios,  {skipped} skipped)' )
 def retry_required(value):
     return value == ('skipped', 1)
 
 @retry(retry=retry_if_result(retry_required),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=20, max=40),reraise=True) 
 async def download(ele,path,model_id,username,file_size_limit,progress):
     attempt.set(attempt.get(0) + 1)
     
     try:
         if ele.url:
-           log.debug(f"Media:{ele.id} Post:{ele.postid} Downloading with normal downloader")
            return await main_download_helper(ele,path,file_size_limit,username,model_id,progress)
         elif ele.mpd:  
-            log.debug(f"Media:{ele.id} Post:{ele.postid} Downloading with protected media downloader")      
             return await alt_download_helper(ele,path,file_size_limit,username,model_id,progress)
         else:
             return "skipped",1
     except Exception as e:
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] exception {e}")   
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] exception {traceback.format_exc()}")   
         return 'skipped', 1
 async def main_download_helper(ele,path,file_size_limit,username,model_id,progress):
     url=ele.url
-    log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename} with {url}")
     path_to_file=None
     async with sem:
+            log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename} with {url}")
+            log.debug(f"Media:{ele.id} Post:{ele.postid} Downloading with normal downloader")
+
             async with httpx.AsyncClient(http2=True, follow_redirects=True, timeout=None) as c: 
                 auth.add_cookies(c)        
                 async with c.stream('GET',url) as r:
                     if not r.is_error:
                         rheaders=r.headers
                         total = int(rheaders['Content-Length'])
                         if file_size_limit>0 and total > int(file_size_limit): 
                                 return 'skipped', 1       
                         content_type = rheaders.get("content-type").split('/')[-1]
                         filename=createfilename(ele,username,model_id,content_type)
                         path_to_file = paths.trunicate(pathlib.Path(path,f"{filename}"))                 
                         pathstr=str(path_to_file)
                         temp=paths.trunicate(f"{path_to_file}.part")
                         pathlib.Path(temp).unlink(missing_ok=True)
-                        task1 = progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES} {(pathstr[:50] + '....') if len(pathstr) > 50 else pathstr}", total=total,visible=False)
+                        task1 = progress.add_task(f"{(pathstr[:constants.PATH_STR_MAX] + '....') if len(pathstr) > constants.PATH_STR_MAX else pathstr}\n", total=total,visible=True)
                         with open(temp, 'wb') as f:                           
                             num_bytes_downloaded = r.num_bytes_downloaded
-                            progress.update(task1,visible=False if logging.getLogger("ofscraper").handlers[1].level>=constants.SUPPRESS_LOG_LEVEL else True)
+                            progress.update(task1,visible=True )
                             async for chunk in r.aiter_bytes(chunk_size=1024):
                                 f.write(chunk)
                                 progress.update(task1, advance=r.num_bytes_downloaded - num_bytes_downloaded)
                                 num_bytes_downloaded = r.num_bytes_downloaded
                             progress.remove_task(task1) 
         
                     else:
@@ -185,64 +191,66 @@
             log.debug(f"Media:{ele.id} Post:{ele.postid} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
 
         if ele.id:
             operations.write_media_table(ele,path_to_file,model_id,username)
         return ele.mediatype,total
 
 async def alt_download_helper(ele,path,file_size_limit,username,model_id,progress):
-    video = None
-    audio = None
-    base_url=re.sub("[0-9a-z]*\.mpd$","",ele.mpd,re.IGNORECASE)
-    mpd=ele.parse_mpd
-    path_to_file = paths.trunicate(pathlib.Path(path,f'{createfilename(ele,username,model_id,"mp4")}')) 
-
-    for period in mpd.periods:
-        for adapt_set in filter(lambda x:x.mime_type=="video/mp4",period.adaptation_sets):             
-            kId=None
-            for prot in adapt_set.content_protections:
-                if prot.value==None:
-                    kId = prot.pssh[0].pssh 
-                    break
-            maxquality=max(map(lambda x:x.height,adapt_set.representations))
-            for repr in adapt_set.representations:
-                if repr.height==maxquality:
-                    video={"name":repr.base_urls[0].base_url_value,"pssh":kId,"type":"video"}
-                    break
-        for adapt_set in filter(lambda x:x.mime_type=="audio/mp4",period.adaptation_sets):             
-            kId=None
-            for prot in adapt_set.content_protections:
-                if prot.value==None:
-                    kId = prot.pssh[0].pssh 
-                    logger.updateSenstiveDict(kId,"pssh_code")
+    async with sem:
+        log.debug(f"Media:{ele.id} Post:{ele.postid} Downloading with protected media downloader")      
+        log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename} with {ele.mpd}")
+        video = None
+        audio = None
+        base_url=re.sub("[0-9a-z]*\.mpd$","",ele.mpd,re.IGNORECASE)
+        mpd=ele.parse_mpd
+        path_to_file = paths.trunicate(pathlib.Path(path,f'{createfilename(ele,username,model_id,"mp4")}')) 
+
+        for period in mpd.periods:
+            for adapt_set in filter(lambda x:x.mime_type=="video/mp4",period.adaptation_sets):             
+                kId=None
+                for prot in adapt_set.content_protections:
+                    if prot.value==None:
+                        kId = prot.pssh[0].pssh 
+                        break
+                maxquality=max(map(lambda x:x.height,adapt_set.representations))
+                for repr in adapt_set.representations:
+                    if repr.height==maxquality:
+                        video={"name":repr.base_urls[0].base_url_value,"pssh":kId,"type":"video"}
+                        break
+            for adapt_set in filter(lambda x:x.mime_type=="audio/mp4",period.adaptation_sets):             
+                kId=None
+                for prot in adapt_set.content_protections:
+                    if prot.value==None:
+                        kId = prot.pssh[0].pssh 
+                        logger.updateSenstiveDict(kId,"pssh_code")
+                        break
+                for repr in adapt_set.representations:
+                    audio={"name":repr.base_urls[0].base_url_value,"pssh":kId,"type":"audio"}
                     break
-            for repr in adapt_set.representations:
-                audio={"name":repr.base_urls[0].base_url_value,"pssh":kId,"type":"audio"}
-                break
-        for item in [audio,video]:
-            url=f"{base_url}{item['name']}"
-            log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {item['name']} with {url}")
-            async with sem:
+            for item in [audio,video]:
+                url=f"{base_url}{item['name']}"
+                log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {item['name']} with {url}")
                 params={"Policy":ele.policy,"Key-Pair-Id":ele.keypair,"Signature":ele.signature}   
                 async with httpx.AsyncClient(http2=True, headers = auth.make_headers(auth.read_auth()), follow_redirects=True, timeout=None,params=params) as c: 
                     auth.add_cookies(c) 
                     async with c.stream('GET',url) as r:
                         if not r.is_error:
                             rheaders=r.headers
                             total = int(rheaders['Content-Length'])
                             item["total"]=total
                             if file_size_limit>0 and total > int(file_size_limit): 
                                     return 'skipped', 1       
                             temp= paths.trunicate(pathlib.Path(path,f"{item['name']}.part"))
                             temp.unlink(missing_ok=True)
                             item["path"]=temp
                             pathstr=str(temp)
-                            task1 = progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES} {(pathstr[:50] + '....') if len(pathstr) > 50 else pathstr}", total=total,visible=False)
+                            task1 = progress.add_task(f"{(pathstr[:constants.PATH_STR_MAX] + '....') if len(pathstr) > constants.PATH_STR_MAX else pathstr}\n", total=total,visible=True)
                             with open(temp, 'wb') as f:                           
                                 num_bytes_downloaded = r.num_bytes_downloaded
-                                progress.update(task1,visible=False if logging.getLogger("ofscraper").handlers[1].level>=constants.SUPPRESS_LOG_LEVEL else True)
+                                progress.update(task1,visible=True )
                                 async for chunk in r.aiter_bytes(chunk_size=1024):
                                     f.write(chunk)
                                     progress.update(task1, advance=r.num_bytes_downloaded - num_bytes_downloaded)
                                     num_bytes_downloaded = r.num_bytes_downloaded
                                 progress.remove_task(task1) 
                         else:
                             r.raise_for_status()
```

### Comparing `ofscraper-2.0.1/ofscraper/utils/encoding.py` & `ofscraper-2.1/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/ofscraper/utils/exit.py` & `ofscraper-2.1/ofscraper/utils/exit.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 SIGNAL_TRANSLATION_MAP = {
     signal.SIGINT: 'SIGINT',
     signal.SIGTERM: 'SIGTERM',
 }
 
 
 class DelayedKeyboardInterrupt:
-    def __init__(self, endprogram,propagate_to_forked_processes=None):
+    def __init__(self,propagate_to_forked_processes=None):
         """
         Constructs a context manager that suppresses SIGINT & SIGTERM signal handlers
         for a block of code.
 
         The signal handlers are called on exit from the block.
 
         Inspired by: https://stackoverflow.com/a/21919644
@@ -34,27 +34,25 @@
         If None, signals received in forked processes are ignored (default).
         """
         self._pid = os.getpid()
         self._propagate_to_forked_processes = propagate_to_forked_processes
         self._sig = None
         self._frame = None
         self._old_signal_handler_map = None
-        self.endprogram=endprogram
 
     def __enter__(self):
         self._old_signal_handler_map = {
             sig: signal.signal(sig, self._handler)
             for sig, _ in SIGNAL_TRANSLATION_MAP.items()
         }
 
     def __exit__(self, exc_type, exc_val, exc_tb):
 
         for sig, handler in self._old_signal_handler_map.items():
             signal.signal(sig, handler)
-        self.endprogram()
         if self._sig is None:
             return
         self._old_signal_handler_map[self._sig](self._sig, self._frame)
 
     def _handler(self, sig, frame):
         self._sig = sig
         self._frame = frame
```

### Comparing `ofscraper-2.0.1/ofscraper/utils/filters.py` & `ofscraper-2.1/ofscraper/utils/filters.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/ofscraper/utils/logger.py` & `ofscraper-2.1/ofscraper/utils/logger.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import logging
 import re
 import httpx
 import logging
+import threading
+import time
+import queue
 from rich.logging import RichHandler
 import ofscraper.utils.paths as paths
 import ofscraper.utils.config as config_
 import ofscraper.utils.args as args
 import ofscraper.utils.console as console
 
 senstiveDict={}
+discord_queue=queue.Queue()
+
 
 class DebugOnly(logging.Filter):
     def filter(self, record):
         if record.levelname=="DEBUG" or record.levelname=="TRACEBACK":
             return True
         return False
 class NoDebug(logging.Filter):
@@ -27,18 +32,36 @@
         log_entry = self.format(record)
         url=config_.get_discord(config_.read_config())
         log_entry=f"{log_entry}\n\n"
         if url==None or url=="":
             return
         #convert markup
         log_entry=re.sub("\[bold\]|\[/bold\]","**",log_entry)
-        httpx.post(url, headers={"Content-type": "application/json"},json={"content":log_entry})
+        discord_queue.put((url,log_entry))
 
+def discord_messenger():
+    with httpx.Client() as c:
+        while True:
+            url,entry=discord_queue.get()   
+            if url=="exit":
+                return 
+            c.post(url, headers={"Content-type": "application/json"},json={"content":entry})
+def discord_cleanup():
+    logging.getLogger("ofscraper").info("Pushing Discord Queue")
+    with httpx.Client() as c:
+        while True:
+            if discord_queue.empty:
+                discord_queue.put(("exit",None))
+                break
+            time.sleep(.5)
+             
 
 
+worker_thread = threading.Thread(target=discord_messenger)
+worker_thread.start()
 class SensitiveFormatter(logging.Formatter):
     """Formatter that removes sensitive information in logs."""
     @staticmethod
     def _filter(s):
         s=re.sub("&Policy=[^&\"]+", "&Policy={hidden}", s)
         s=re.sub("&Signature=[^&\"]+", "&Signature={hidden}", s)
         s=re.sub("&Key-Pair-Id=[^&\"]+", "&Key-Pair-Id={hidden}", s)
@@ -78,21 +101,23 @@
 def updateSenstiveDict(word,replacement):
      global senstiveDict
      senstiveDict[word]=replacement
 
 
 def getLevel(input):
     """
-    ERROR 50
+    CRITICAL 50
+    ERROR 40
     WARNING 30
     INFO 20
     DEBUG 10
     """
     return {"OFF":100,
-            "PROMPT":"ERROR",
+            "PROMPT":"CRITICAL",
+            "STATS":"ERROR",
             "LOW":"WARNING",
             "NORMAL":"INFO",
             "DEBUG":"DEBUG"}.get(input,100)
 
 def init_logger(log):
     log.setLevel(1)
     addtrackback()
```

### Comparing `ofscraper-2.0.1/ofscraper/utils/paths.py` & `ofscraper-2.1/ofscraper/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/ofscraper/utils/profiles.py` & `ofscraper-2.1/ofscraper/utils/profiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 import pathlib
 import shutil
 from rich.console import Console
 from rich import print
 import ofscraper.utils.config as config_
 import ofscraper.prompts.prompts as prompts
 import ofscraper.constants as constants
-
+import logging
+log=logging.getLogger(__package__)
 console=Console()
 
 
 def get_profile_path():
     config_path = pathlib.Path.home() / constants.configPath
     return config_path
 
@@ -93,8 +94,8 @@
     return config[constants.mainProfile]
 
 
 def print_current_profile():
     get_profiles()
 
     current_profile = get_current_profile()
-    print('Using profile: [cyan]{}[/cyan]'.format(current_profile))
+    log.info('Using profile: [cyan]{}[/cyan]'.format(current_profile))
```

### Comparing `ofscraper-2.0.1/ofscraper/utils/separate.py` & `ofscraper-2.1/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.0.1/pyproject.toml` & `ofscraper-2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "2.0.1"
+version = "2.1"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 packages = [{include = "ofscraper"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
@@ -14,15 +14,14 @@
 schedule = "^1.1.0"
 browser-cookie3 = "^0.17.1"
 requests = "^2.28.2"
 bs4 = "^0.0.1"
 rich = "^13.3.2"
 tenacity = "^8.2.2"
 arrow = "^1.2.3"
-halo = "^0.0.31"
 win32-setctime = "^1.1.0"
 pathvalidate = "^2.5.2"
 xxhash = "^3.2.0"
 mpegdash = "^0.3.1"
 diskcache = "^5.6.1"
 ffmpeg-python = "^0.2.0"
 dunamai = "^1.17.0"
```

### Comparing `ofscraper-2.0.1/PKG-INFO` & `ofscraper-2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 2.0.1
+Version: 2.1
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -13,15 +13,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: browser-cookie3 (>=0.17.1,<0.18.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: diskcache (>=5.6.1,<6.0.0)
 Requires-Dist: dunamai (>=1.17.0,<2.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
-Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: httpx[http2] (>=0.23.3,<0.24.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Requires-Dist: mpegdash (>=0.3.1,<0.4.0)
 Requires-Dist: pathvalidate (>=2.5.2,<3.0.0)
 Requires-Dist: poetry-dynamic-versioning (>=0.22.0,<0.23.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
```

