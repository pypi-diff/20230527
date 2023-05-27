# Comparing `tmp/bilix-0.9.4.tar.gz` & `tmp/bilix-1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bilix-0.9.4.tar", last modified: Tue Oct 25 08:15:59 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `bilix-0.9.4.tar` & `bilix-1.0a0.tar`

### file list

```diff
@@ -1,49 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 08:15:59.353625 bilix-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-10-25 08:15:49.000000 bilix-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-25 08:15:49.000000 bilix-0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11061 2022-10-25 08:15:59.353625 bilix-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10391 2022-10-25 08:15:49.000000 bilix-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 08:15:59.353625 bilix-0.9.4/bilix/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8600 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 08:15:59.353625 bilix-0.9.4/bilix/api/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9128 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/api/bilibili.py
--rw-r--r--   0 runner    (1001) docker     (121)     2663 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/api/cctv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2463 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/api/douyin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1572 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/api/jable.py
--rw-r--r--   0 runner    (1001) docker     (121)     3654 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/api/yhdmp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1432 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/api/yinghuacd.py
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/assign.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 08:15:59.353625 bilix-0.9.4/bilix/dm/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/dm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17064 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/dm/reply_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1685 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/dm/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3179 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/dm/view_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 08:15:59.353625 bilix-0.9.4/bilix/download/
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3235 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/download/base_downloader.py
--rw-r--r--   0 runner    (1001) docker     (121)     6774 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/download/base_downloader_m3u8.py
--rw-r--r--   0 runner    (1001) docker     (121)     5603 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/download/base_downloader_part.py
--rw-r--r--   0 runner    (1001) docker     (121)    25301 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/download/downloader_bilibili.py
--rw-r--r--   0 runner    (1001) docker     (121)     2509 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/download/downloader_cctv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/download/downloader_douyin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/download/downloader_jable.py
--rw-r--r--   0 runner    (1001) docker     (121)     3082 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/download/downloader_yhdmp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2928 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/download/downloader_yinghuacd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 08:15:59.353625 bilix-0.9.4/bilix/js/
--rw-r--r--   0 runner    (1001) docker     (121)    23731 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/js/yhdmp.js
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/log.py
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/process.py
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/subtitle.py
--rw-r--r--   0 runner    (1001) docker     (121)     2688 2022-10-25 08:15:49.000000 bilix-0.9.4/bilix/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 08:15:59.353625 bilix-0.9.4/bilix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11061 2022-10-25 08:15:59.000000 bilix-0.9.4/bilix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-10-25 08:15:59.000000 bilix-0.9.4/bilix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 08:15:59.000000 bilix-0.9.4/bilix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-25 08:15:59.000000 bilix-0.9.4/bilix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-10-25 08:15:59.000000 bilix-0.9.4/bilix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-10-25 08:15:59.000000 bilix-0.9.4/bilix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-25 08:15:59.353625 bilix-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-10-25 08:15:49.000000 bilix-0.9.4/setup.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/__main__.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/_process.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/exception.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/ffmpeg.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/log.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/utils.py
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/cli/assign.py
+-rw-r--r--   0        0        0     9958 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/cli/core.py
+-rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/cli/handler.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/cli/main.py
+-rw-r--r--   0        0        0    10400 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/download/base_downloader.py
+-rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/download/base_downloader_m3u8.py
+-rw-r--r--   0        0        0    10165 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/download/base_downloader_part.py
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/download/utils.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/progress/abc.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/progress/cli_progress.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/progress/ws_progress.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/bilibili/__init__.py
+-rw-r--r--   0        0        0    16421 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/bilibili/api.py
+-rw-r--r--   0        0        0     4670 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/bilibili/api_test.py
+-rw-r--r--   0        0        0    27218 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/bilibili/downloader.py
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/bilibili/downloader_test.py
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/bilibili/informer.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/bilibili/informer_test.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/cctv/__init__.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/cctv/api.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/cctv/api_test.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/cctv/downloader.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/douyin/__init__.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/douyin/api.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/douyin/api_test.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/douyin/downloader.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/douyin/downloader_test.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/hanime1/__init__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/hanime1/api.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/hanime1/api_test.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/hanime1/downloader.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/jable/__init__.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/jable/api.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/jable/api_test.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/jable/downloader.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/tiktok/__init__.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/tiktok/api.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/tiktok/api_test.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/tiktok/downloader.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/tiktok/downloader_test.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/yhdmp/__init__.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/yhdmp/api.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/yhdmp/api_test.py
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/yhdmp/downloader.py
+-rw-r--r--   0        0        0    23731 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/yhdmp/yhdmp.js
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/yinghuacd/__init__.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/yinghuacd/api.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/yinghuacd/api_test.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/yinghuacd/downloader.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 bilix-1.0a0/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 bilix-1.0a0/LICENSE
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 bilix-1.0a0/README.md
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 bilix-1.0a0/pyproject.toml
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 bilix-1.0a0/PKG-INFO
```

### Comparing `bilix-0.9.4/LICENSE` & `bilix-1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `bilix-0.9.4/bilix/api/cctv.py` & `bilix-1.0a0/bilix/sites/cctv/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 import asyncio
 import re
 import json
 from typing import Sequence, Tuple
 
 import httpx
 import m3u8
-from bilix.log import logger
-from bilix.utils import legal_title, req_retry
 
-_dft_headers = {'user-agent': 'PostmanRuntime/7.29.0'}
+from bilix.download.utils import req_retry, raise_api_error
+from bilix.utils import legal_title
 
+dft_client_settings = {
+    'headers': {'user-agent': 'PostmanRuntime/7.29.0'},
+    'http2': True
+}
 
+
+@raise_api_error
 async def get_id(client: httpx.AsyncClient, url: str) -> Tuple[str, str, str]:
     res_web = await req_retry(client, url)
     pid = re.findall(r'guid ?= ?"(\w+)"', res_web.text)[0]
     vide = re.findall(r'/(VIDE\w+)\.', url)[0]
     try:
         vida = re.findall(r'videotvCodes ?= ?"(\w+)"', res_web.text)[0]
     except IndexError:
         vida = None
     return pid, vide, vida
 
 
+@raise_api_error
 async def get_media_info(client: httpx.AsyncClient, pid: str) -> Tuple[str, Sequence[str]]:
     """
 
     :param pid:
     :param client:
     :return: title and m3u8 urls sorted by quality
     """
@@ -39,14 +45,15 @@
     if m3u8_info.base_uri is None:
         m3u8_info.base_uri = re.match(r'(https?://[^/]*)/', m3u8_main_url).groups()[0]
     m3u8_urls = list(sorted((i.absolute_uri for i in m3u8_info.playlists), reverse=True,
                             key=lambda s: int(re.findall(r'/(\d+).m3u8', s)[0])))
     return title, m3u8_urls
 
 
+@raise_api_error
 async def get_series_info(client: httpx.AsyncClient, vide: str, vida: str) -> Tuple[str, Sequence[str]]:
     """
 
     :param vide:
     :param vida:
     :param client:
     :return: title and list of guid(pid)
@@ -58,23 +65,7 @@
     )
     meta_data = json.loads(res_meta.text)
     list_data = json.loads(res_list.text)
     # extract
     title = legal_title(meta_data['data']['title'])
     pids = [i['guid'] for i in list_data['data']['list']]
     return title, pids
-
-
-if __name__ == '__main__':
-    async def main():
-        _dft_client = httpx.AsyncClient(headers=_dft_headers, http2=True)
-
-        return await asyncio.gather(
-            get_id(
-                _dft_client,
-                "https://tv.cctv.com/2012/05/02/VIDE1355968282695723.shtml?spm=C55853485115.P6UrzpiudtDc.0.0"
-            ))
-
-
-    logger.setLevel("DEBUG")
-    result = asyncio.run(main())
-    print(result)
```

### Comparing `bilix-0.9.4/bilix/api/douyin.py` & `bilix-1.0a0/bilix/sites/douyin/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,35 +5,39 @@
 
 Modified by
 @Author: https://github.com/HFrost0/
 """
 import asyncio
 import re
 import json
-from typing import Sequence
+from typing import List
 import httpx
-from dataclasses import dataclass
-from bilix.utils import req_retry, legal_title
+from pydantic import BaseModel
+from bilix.utils import legal_title
+from bilix.download.utils import req_retry, raise_api_error
 
-_dft_headers = {'user-agent': 'Mozilla/5.0 (Linux; Android 8.0; Pixel 2 Build/OPD3.170816.012)'
+dft_client_settings = {
+    'headers': {'user-agent': 'Mozilla/5.0 (Linux; Android 8.0; Pixel 2 Build/OPD3.170816.012)'
                               ' AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.88 Mobile'
-                              ' Safari/537.36 Edg/87.0.664.66'}
+                              ' Safari/537.36 Edg/87.0.664.66'},
+    'http2': True
+}
 
 
-@dataclass
-class VideoInfo:
+class VideoInfo(BaseModel):
     title: str
     author_name: str
-    wm_urls: Sequence[str]
-    nwm_urls: Sequence[str]
+    wm_urls: List[str]
+    nwm_urls: List[str]
     cover: str
     dynamic_cover: str
     origin_cover: str
 
 
+@raise_api_error
 async def get_video_info(client: httpx.AsyncClient, url: str) -> VideoInfo:
     if short_url := re.findall(r'https://v.douyin.com/\w+/', url):
         res = await req_retry(client, short_url[0], follow_redirects=True)
         url = str(res.url)
     if key := re.search(r'/video/(\d+)', url):
         key = key.groups()[0]
     else:
@@ -58,13 +62,13 @@
     video_info = VideoInfo(title=title, author_name=author_name, wm_urls=wm_urls, nwm_urls=nwm_urls, cover=cover,
                            dynamic_cover=dynamic_cover, origin_cover=origin_cover)
     return video_info
 
 
 if __name__ == '__main__':
     async def main():
-        _dft_client = httpx.AsyncClient(headers=_dft_headers, http2=True)
-        data = await get_video_info(_dft_client, 'https://www.douyin.com/video/7132430286415252773')
+        client = httpx.AsyncClient(**dft_client_settings)
+        data = await get_video_info(client, 'https://www.douyin.com/video/7132430286415252773')
         print(data)
 
 
     asyncio.run(main())
```

### Comparing `bilix-0.9.4/bilix/api/jable.py` & `bilix-1.0a0/bilix/sites/hanime1/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,40 @@
-import asyncio
-import re
-from dataclasses import dataclass
+from pydantic import BaseModel
 import httpx
+from bilix.utils import legal_title
+from bilix.download.utils import req_retry, raise_api_error
 from bs4 import BeautifulSoup
-from bilix.log import logger
-from bilix.utils import legal_title, req_retry
 
-BASE_URL = "https://jable.tv"
-_dft_headers = {'user-agent': 'PostmanRuntime/7.29.0', "Referer": BASE_URL}
+BASE_URL = "https://hanime1.me"
+dft_client_settings = {
+    'headers': {'user-agent': 'Mozilla/5.0 (Linux; Android 8.0; Pixel 2 Build/OPD3.170816.012)'
+                              ' AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.88 Mobile'
+                              ' Safari/537.36 Edg/87.0.664.66',
+                "Referer": BASE_URL},
+    'http2': False
+}
 
 
-@dataclass
-class VideoInfo:
+class VideoInfo(BaseModel):
     url: str
     avid: str
     title: str
-    model_name: str
-    m3u8_url: str
+    video_url: str
     img_url: str
 
 
+@raise_api_error
 async def get_video_info(client: httpx.AsyncClient, url_or_avid: str) -> VideoInfo:
     if url_or_avid.startswith('http'):
         url = url_or_avid
-        avid = url.split('/')[-2]
+        avid = url.split('=')[-1]
     else:
-        url = f'{BASE_URL}/videos/{url_or_avid}/'
+        url = f'{BASE_URL}/watch?v={url_or_avid}'
         avid = url_or_avid
-    avid = avid.upper()
-    res = await req_retry(client, url)  # proxies default global in httpx
+    res = await req_retry(client, url)
     soup = BeautifulSoup(res.text, "html.parser")
     title = soup.find('meta', property="og:title")['content']
     title = legal_title(title)
-    model_name = soup.find("span", class_="placeholder rounded-circle")['title']
     img_url = soup.find('meta', property="og:image")['content']
-    m3u8_url = re.findall(r'http.*m3u8', res.text)[0]
-    video_info = VideoInfo(url=url, avid=avid, title=title, img_url=img_url, m3u8_url=m3u8_url, model_name=model_name)
+    video_url = soup.find('input', {'id': 'video-sd'})['value']
+    video_info = VideoInfo(url=url, avid=avid, title=title, img_url=img_url, video_url=video_url)
     return video_info
-
-
-if __name__ == '__main__':
-    async def main():
-        _dft_client = httpx.AsyncClient(headers=_dft_headers, http2=True)
-        return await asyncio.gather(
-            get_video_info(_dft_client, "MIAA-650"),
-        )
-
-
-    logger.setLevel("DEBUG")
-    result = asyncio.run(main())
-    print(result)
```

### Comparing `bilix-0.9.4/bilix/api/yhdmp.py` & `bilix-1.0a0/bilix/sites/yhdmp/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,72 @@
 import asyncio
 import json
-import os
 import random
 import re
-from dataclasses import dataclass
-from typing import Union, Sequence
+from pathlib import Path
+from pydantic import BaseModel
+from typing import Union, List
 import httpx
 import execjs
 from bs4 import BeautifulSoup
-from bilix.log import logger
-import bilix.utils
 from bilix.utils import legal_title
+from bilix.download.utils import req_retry as rr, raise_api_error
 
 BASE_URL = "https://www.yhdmp.cc"
-_dft_headers = {'user-agent': 'PostmanRuntime/7.29.0', "Referer": BASE_URL}
+dft_client_settings = {
+    'headers': {'user-agent': 'PostmanRuntime/7.29.0', "Referer": BASE_URL},
+    'http2': False
+}
+_js = None
 
-with open(f'{os.path.dirname(bilix.__file__)}/js/yhdmp.js', 'r') as f:
-    js = execjs.compile(f.read())
+
+def _get_js():
+    global _js
+    if _js is None:
+        with open(Path(__file__).parent / 'yhdmp.js', 'r') as f:
+            _js = execjs.compile(f.read())
+    return _js
 
 
 def _get_t2_k2(t1: str, k1: str) -> dict:
-    new_cookies = js.call("get_t2_k2", t1, k1)
+    new_cookies = _get_js().call("get_t2_k2", t1, k1)
     return new_cookies
 
 
 def _decode(data: str) -> str:
-    return js.call('__getplay_rev_data', data)
+    return _get_js().call('__getplay_rev_data', data)
 
 
-async def req_retry(client: httpx.AsyncClient, url_or_urls: Union[str, Sequence[str]],
+async def req_retry(client: httpx.AsyncClient, url_or_urls: Union[str, List[str]],
                     method: str = 'GET',
                     follow_redirects: bool = False,
                     **kwargs):
     if 't1' in client.cookies and 'k1' in client.cookies:
         new_cookies = _get_t2_k2(client.cookies['t1'], client.cookies['k1'])
         if 't2' in client.cookies:
             client.cookies.delete('t2')
         if 'k2' in client.cookies:
             client.cookies.delete('k2')
         client.cookies.update(new_cookies)
 
-    res = await bilix.utils.req_retry(client, url_or_urls, method, follow_redirects, **kwargs)
+    res = await rr(client, url_or_urls, method, follow_redirects, **kwargs)
     return res
 
 
-@dataclass
-class VideoInfo:
+class VideoInfo(BaseModel):
     aid: Union[str, int]
     play_idx: int
     ep_idx: int
     title: str
     sub_title: str
-    play_info: Sequence[Union[Sequence[str], Sequence]]  # may be empty
+    play_info: List[Union[List[str], List]]  # may be empty
     m3u8_url: str
 
 
+@raise_api_error
 async def get_video_info(client: httpx.AsyncClient, url: str) -> VideoInfo:
     aid, play_idx, ep_idx = url.split('/')[-1].split('.')[0].split('-')
     play_idx, ep_idx = int(play_idx), int(ep_idx)
     # request
     res_web = req_retry(client, url)
     m3u8_url = get_m3u8_url(url=url, client=client)
     if 't1' in client.cookies and 'k1' in client.cookies:
@@ -74,32 +82,18 @@
     for div in divs:
         play_info.append([[legal_title(a["title"]), f"{BASE_URL}/{a['href']}"] for a in div.find_all("a")])
     video_info = VideoInfo(aid=aid, play_idx=play_idx, ep_idx=ep_idx, title=title, sub_title=sub_title,
                            play_info=play_info, m3u8_url=m3u8_url)
     return video_info
 
 
+@raise_api_error
 async def get_m3u8_url(client: httpx.AsyncClient, url):
     aid, play_idx, ep_idx = url.split('/')[-1].split('.')[0].split('-')
     params = {"aid": aid, "playindex": play_idx, "epindex": ep_idx, "r": random.random()}
     res_play = await req_retry(client, f"{BASE_URL}/_getplay", params=params)
     if res_play.text.startswith("err"):  # maybe first time
         res_play = await req_retry(client, f"{BASE_URL}/_getplay", params=params)
     data = json.loads(res_play.text)
     purl, vurl = _decode(data['purl']), _decode(data['vurl'])
     m3u8_url = purl.split("url=")[-1] + vurl
     return m3u8_url
-
-
-async def main():
-    _dft_client = httpx.AsyncClient(headers=_dft_headers, http2=True)
-
-    return await asyncio.gather(
-        get_video_info(_dft_client, "https://www.yhdmp.cc/vp/22224-1-0.html"),
-        get_m3u8_url(_dft_client, "https://www.yhdmp.cc/vp/18261-2-0.html"),
-    )
-
-
-if __name__ == '__main__':
-    logger.setLevel("DEBUG")
-    result = asyncio.run(main())
-    print(result)
```

### Comparing `bilix-0.9.4/bilix/download/downloader_bilibili.py` & `bilix-1.0a0/bilix/sites/bilibili/downloader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,522 +1,548 @@
 import asyncio
-from typing import Union, Sequence, Tuple
+import functools
+import logging
+import re
+from enum import Enum
+from pathlib import Path
+from typing import Union, Tuple, List, Annotated
 import aiofiles
 import httpx
 from datetime import datetime, timedelta
-import os
-from itertools import groupby
-from anyio import run_process
-import bilix.api.bilibili as api
-from bilix.assign import Handler
+from . import api
 from bilix.download.base_downloader_part import BaseDownloaderPart
-from bilix.subtitle import json2srt
-from bilix.dm import dm2ass_factory
-from bilix.utils import legal_title, req_retry, cors_slice
-from bilix.log import logger
-
-__all__ = ['DownloaderBilibili']
-
-
-def choose_quality(dash, support_formats, quality: Union[str, int]) -> Tuple[dict, Sequence]:
-    # 1. absolute choice with quality name like 4k 1080p '1080p 60帧'
-    if isinstance(quality, str):
-        for f_info in support_formats:
-            if quality.upper() in f_info['new_description'].upper():
-                q_id = f_info['quality']
-                for video_info in dash['video']:
-                    if video_info['id'] == q_id:
-                        video_urls = (video_info['base_url'], *(video_info['backup_url']
-                                                                if video_info['backup_url'] else ()))
-                        logger.debug(f"quality <{f_info['new_description']}> has been chosen")
-                        return video_info, video_urls
-        raise ValueError(f'No valid quality for {quality}')
-    # 2. relative choice
-    else:
-        video_info, video_urls = None, None
-        for q, (q_id, it) in enumerate(groupby(dash['video'], key=lambda x: x['id'])):
-            video_info = next(it)  # use the first codec
-            video_urls = (video_info['base_url'], *(video_info['backup_url']
-                                                    if video_info['backup_url'] else ()))
-            if q == quality:
-                break
-        logger.debug(f'Relative quality {quality} has been chosen')
-        return video_info, video_urls
+from bilix._process import SingletonPPE
+from bilix.utils import legal_title, cors_slice, valid_sess_data, t2s, json2srt
+from bilix.download.utils import req_retry, path_check, parse_speed_str, str2path, parse_time_range
+from bilix.exception import APIUnsupportedError, APIResourceError, APIError
+from bilix.progress.abc import Progress
+from bilix import ffmpeg
+from danmakuC.bilibili import proto2ass
+
+
+def _dm2ass_factory(width: int, height: int):
+    async def dm2ass(protobuf_bytes: bytes) -> bytes:
+        loop = asyncio.get_event_loop()
+        f = functools.partial(proto2ass, protobuf_bytes, width, height, font_size=width / 40, )
+        content = await loop.run_in_executor(SingletonPPE(), f)
+        return content.encode('utf-8')
+
+    return dm2ass
 
 
 class DownloaderBilibili(BaseDownloaderPart):
-    def __init__(self, videos_dir='videos', sess_data='', video_concurrency=3, part_concurrency=10):
-        """
+    cookie_domain = "bilibili.com"  # for load cookies quickly
+    pattern = re.compile(r"^https?://([A-Za-z0-9-]+\.)*(bilibili\.com|b23\.tv)")
 
-        :param videos_dir: 下载到哪个目录，默认当前目录下的为videos中，如果路径不存在将自动创建
-        :param sess_data: 有条件的用户填写大会员凭证，填写后可下载大会员资源
-        :param video_concurrency: 限制最大同时下载的视频数量
-        :param part_concurrency: 每个媒体的分段并发数
-        """
-        cookies = {'SESSDATA': sess_data}
-        headers = {'user-agent': 'PostmanRuntime/7.29.0', 'referer': 'https://www.bilibili.com'}
-        client = httpx.AsyncClient(headers=headers, cookies=cookies, http2=True)
-        super(DownloaderBilibili, self).__init__(client, videos_dir, part_concurrency)
-        self.v_sema = asyncio.Semaphore(video_concurrency)
+    def __init__(
+            self,
+            *,
+            client: httpx.AsyncClient = None,
+            browser: str = None,
+            speed_limit: Annotated[float, parse_speed_str] = None,
+            stream_retry: int = 5,
+            progress: Progress = None,
+            logger: logging.Logger = None,
+            part_concurrency: int = 10,
+            # unique params
+            sess_data: str = None,
+            video_concurrency: Union[int, asyncio.Semaphore] = 3,
+            hierarchy: bool = True,
+    ):
+        """
+
+        :param client:
+        :param browser:
+        :param speed_limit:
+        :param stream_retry:
+        :param progress:
+        :param logger:
+        :param sess_data: bilibili SESSDATA cookie
+        :param part_concurrency:
+        :param video_concurrency: 视频并发数
+        :param hierarchy: 是否使用层级目录，如果为否，将所有文件下载到同一目录下
+        """
+        client = client or httpx.AsyncClient(**api.dft_client_settings)
+        super(DownloaderBilibili, self).__init__(
+            client=client,
+            browser=browser,
+            speed_limit=speed_limit,
+            stream_retry=stream_retry,
+            progress=progress,
+            logger=logger,
+            part_concurrency=part_concurrency,
+        )
+        client.cookies.set('SESSDATA', valid_sess_data(sess_data))
         self._cate_meta = None
-
-    async def get_collect_or_list(self, url, quality=0, image=False, subtitle=False, dm=False, only_audio=False,
-                                  hierarchy: Union[bool, str] = True):
-        """
-        下载合集或视频列表
-
-        :param url: 合集或视频列表详情页url
-        :param quality:
-        :param image:
-        :param subtitle:
-        :param dm:
-        :param only_audio:
-        :param hierarchy: 是否使用层次目录保存文件
-        :return:
-        """
-        if 'seriesdetail' in url:
-            await self.get_list(url, quality, image, subtitle, dm, only_audio, hierarchy)
-        elif 'collectiondetail' in url:
-            await self.get_collect(url, quality, image, subtitle, dm, only_audio, hierarchy)
-        else:
-            raise Exception(f'未知的详情页 {url}')
-
-    async def get_list(self, url, quality=0, image=False, subtitle=False, dm=False, only_audio=False,
-                       hierarchy: Union[bool, str] = True):
-        """
-        下载视频列表
-
-        :param url: 列表详情页url
-        :param quality:
-        :param image:
-        :param subtitle:
-        :param dm:
-        :param only_audio:
-        :param hierarchy:
+        self.v_sema = asyncio.Semaphore(video_concurrency)
+        self.api_sema = asyncio.Semaphore(video_concurrency)
+        self.hierarchy = hierarchy
+        self.title_overflow = 50
+
+    @classmethod
+    def parse_url(cls, url: str):
+        if re.match(r'https://space\.bilibili\.com/\d+/favlist\?fid=\d+', url):
+            return cls.get_favour
+        elif re.match(r'https://space\.bilibili\.com/\d+/channel/seriesdetail\?sid=\d+', url):
+            return cls.get_collect_or_list
+        elif re.match(r'https://space\.bilibili\.com/\d+/channel/collectiondetail\?sid=\d+', url):
+            return cls.get_collect_or_list
+        elif re.match(r'https://space\.bilibili\.com/\d+', url):  # up space url
+            return cls.get_up
+        elif re.search(r'(www\.bilibili\.com)|(b23\.tv)', url):
+            return cls.get_video
+        raise ValueError(f'{url} no match for bilibili')
+
+    async def auto(self, key: str, **method_options: dict):
+        """
+        自动选择下载方法
+        :cli short: a
+        :param key:
+        :param method_options:
         :return:
         """
-        list_name, up_name, bvids = await api.get_list_info(self.client, url)
-        if hierarchy:
-            name = legal_title(f"【视频列表】{up_name}-{list_name}")
-            hierarchy = self._make_hierarchy_dir(hierarchy, name)
-        await asyncio.gather(
-            *[self.get_series(f"https://www.bilibili.com/video/{i}", quality=quality,
-                              image=image, subtitle=subtitle, dm=dm, only_audio=only_audio, hierarchy=hierarchy)
-              for i in bvids])
+        method = self.parse_url(key)
+        return await method(self, key, **method_options)
 
-    async def get_collect(self, url, quality=0, image=False, subtitle=False, dm=False, only_audio=False,
-                          hierarchy: Union[bool, str] = True):
+    async def get_collect_or_list(self, url, path: Annotated[Path, str2path] = Path('.'),
+                                  quality: Union[str, int] = 0, image=False, subtitle=False, dm=False, only_audio=False,
+                                  codec: str = ''):
         """
-        下载合集
-
-        :param url: 合集详情页url
+        下载合集或视频列表
+        :cli short: col
+        :param url: 合集或视频列表详情页url
+        :param path: 保存路径
         :param quality: 画面质量，0为可以观看的最高画质，越大质量越低，超过范围时自动选择最低画质，或者直接使用字符串指定'1080p'等名称
         :param image: 是否下载封面
         :param subtitle: 是否下载字幕
         :param dm: 是否下载弹幕
-        :param only_audio: 是否仅下载音频
-        :param hierarchy:
+        :param only_audio: 是否只下载音频
+        :param codec:
         :return:
         """
-        col_name, up_name, bvids = await api.get_collect_info(self.client, url)
-        if hierarchy:
-            name = legal_title(f"【合集】{up_name}-{col_name}")
-            hierarchy = self._make_hierarchy_dir(hierarchy, name)
+        if 'series' in url:
+            list_name, up_name, bvids = await api.get_list_info(self.client, url)
+            name = legal_title(f"【视频列表】{up_name}", list_name)
+        elif 'collection' in url:
+            col_name, up_name, bvids = await api.get_collect_info(self.client, url)
+            name = legal_title(f"【合集】{up_name}", col_name)
+        else:
+            raise ValueError(f'{url} invalid for get_collect_or_list')
+        if self.hierarchy:
+            path /= name
+            path.mkdir(parents=True, exist_ok=True)
         await asyncio.gather(
-            *[self.get_series(f"https://www.bilibili.com/video/{i}", quality=quality,
-                              image=image, subtitle=subtitle, dm=dm, only_audio=only_audio, hierarchy=hierarchy)
+            *[self.get_series(f"https://www.bilibili.com/video/{i}", path=path, quality=quality, codec=codec,
+                              image=image, subtitle=subtitle, dm=dm, only_audio=only_audio)
               for i in bvids])
 
-    async def get_favour(self, url_or_fid, num=20, keyword='', quality=0, series=True, image=False, subtitle=False,
-                         dm=False, only_audio=False, hierarchy: Union[bool, str] = True):
+    async def get_favour(self, url_or_fid, path: Annotated[Path, str2path] = Path('.'),
+                         num=20, keyword='', quality: Union[str, int] = 0, series=True, image=False, subtitle=False,
+                         dm=False, only_audio=False, codec: str = ''):
         """
         下载收藏夹内的视频
-
+        :cli short: fav
         :param url_or_fid: 收藏夹url或收藏夹id
+        :param path: 保存路径
         :param num: 下载数量
         :param keyword: 搜索关键词
         :param quality: 画面质量，0为可以观看的最高画质，越大质量越低，超过范围时自动选择最低画质，或者直接使用字符串指定'1080p'等名称
         :param series: 每个视频是否下载所有p，False时仅下载系列中的第一个视频
         :param image: 是否下载封面
         :param subtitle: 是否下载字幕
         :param dm: 是否下载弹幕
         :param only_audio: 是否仅下载音频
-        :param hierarchy:
+        :param codec: 视频编码
         :return:
         """
         fav_name, up_name, total_size, bvids = await api.get_favour_page_info(self.client, url_or_fid, keyword=keyword)
-        if hierarchy:
+        if self.hierarchy:
             name = legal_title(f"【收藏夹】{up_name}-{fav_name}")
-            hierarchy = self._make_hierarchy_dir(hierarchy, name)
+            path /= name
+            path.mkdir(parents=True, exist_ok=True)
         total = min(total_size, num)
         ps = 20
         page_nums = total // ps + min(1, total % ps)
         cors = []
         for i in range(page_nums):
             if i + 1 == page_nums:
                 num = total - (page_nums - 1) * ps
             else:
                 num = ps
-            cors.append(self._get_favor_by_page(url_or_fid, i + 1, num, keyword, quality, series,
-                                                image, subtitle, dm, only_audio, hierarchy=hierarchy))
+            cors.append(self._get_favor_by_page(
+                url_or_fid, path, i + 1, num, keyword, quality, series, image, subtitle, dm, only_audio, codec=codec))
         await asyncio.gather(*cors)
 
-    async def _get_favor_by_page(self, url_or_fid, pn=1, num=20, keyword='', quality=0, series=True,
-                                 image=False, subtitle=False, dm=False, only_audio=False, hierarchy=True):
+    async def _get_favor_by_page(self, url_or_fid, path: Path, pn=1, num=20, keyword='', quality: Union[str, int] = 0,
+                                 series=True, image=False, subtitle=False, dm=False, only_audio=False, codec=''):
         ps = 20
         num = min(ps, num)
         _, _, _, bvids = await api.get_favour_page_info(self.client, url_or_fid, pn, ps, keyword)
         cors = []
         for i in bvids[:num]:
             func = self.get_series if series else self.get_video
             # noinspection PyArgumentList
-            cors.append(func(f'https://www.bilibili.com/video/{i}', quality=quality,
-                             image=image, subtitle=subtitle, dm=dm, only_audio=only_audio, hierarchy=hierarchy))
+            cors.append(func(f'https://www.bilibili.com/video/{i}', path=path, quality=quality, codec=codec,
+                             image=image, subtitle=subtitle, dm=dm, only_audio=only_audio))
         await asyncio.gather(*cors)
 
     @property
     async def cate_meta(self):
         if not self._cate_meta:
             self._cate_meta = asyncio.ensure_future(api.get_cate_meta(self.client))
             self._cate_meta = await self._cate_meta
         elif asyncio.isfuture(self._cate_meta):
             await self._cate_meta
         return self._cate_meta
 
-    async def get_cate_videos(self, cate_name: str, num=10, order='click', keyword='', days=7, quality=0, series=True,
-                              image=False, subtitle=False, dm=False, only_audio=False,
-                              hierarchy: Union[bool, str] = True):
+    class CateOrder(Enum):
+        click = 'click'
+        scores = 'scores'
+        stow = 'stow'
+        coin = 'coin'
+        dm = 'dm'
+
+    async def get_cate(self, cate_name: str, path: Annotated[Path, str2path] = Path('.'),
+                       num=10,
+                       order: CateOrder = CateOrder.click,
+                       keyword='', days=7, quality: Union[str, int] = 0,
+                       series=True, image=False, subtitle=False, dm=False, only_audio=False, codec='', ):
         """
         下载分区视频
-
+        :cli short: cate
         :param cate_name: 分区名称
+        :param path: 保存路径
         :param num: 下载数量
         :param order: 何种排序，click播放数，scores评论数，stow收藏数，coin硬币数，dm弹幕数
         :param keyword: 搜索关键词
         :param days: 过去days天中的结果
         :param quality: 画面质量，0为可以观看的最高画质，越大质量越低，超过范围时自动选择最低画质，或者直接使用字符串指定'1080p'等名称
         :param series: 每个视频是否下载所有p，False时仅下载系列中的第一个视频
         :param image: 是否下载封面
         :param subtitle: 是否下载字幕
         :param dm: 是否下载弹幕
         :param only_audio: 是否仅下载音频
-        :param hierarchy:
+        :param codec: 视频编码
         :return:
         """
         cate_meta = await self.cate_meta
         if cate_name not in cate_meta:
-            logger.error(f'未找到分区 {cate_name}')
-            return
+            return self.logger.error(f'未找到分区 {cate_name}')
         if 'subChannelId' not in cate_meta[cate_name]:
             sub_names = [i['name'] for i in cate_meta[cate_name]['sub']]
-            logger.error(f'{cate_name} 是主分区，仅支持子分区，试试 {sub_names}')
-            return
-        if hierarchy:
-            hierarchy = self._make_hierarchy_dir(hierarchy, legal_title(f"【分区】{cate_name}"))
+            return self.logger.error(f'{cate_name} 是主分区，仅支持子分区，试试 {sub_names}')
+        if self.hierarchy:
+            path /= legal_title(f"【分区】{cate_name}")
+            path.mkdir(parents=True, exist_ok=True)
         cate_id = cate_meta[cate_name]['tid']
         time_to = datetime.now()
         time_from = time_to - timedelta(days=days)
         time_from, time_to = time_from.strftime('%Y%m%d'), time_to.strftime('%Y%m%d')
         pagesize = 30
         page = 1
         cors = []
         while num > 0:
-            cors.append(
-                self._get_cate_videos_by_page(cate_id, time_from, time_to, page, min(pagesize, num), order, keyword,
-                                              quality, series, image=image, subtitle=subtitle, dm=dm,
-                                              only_audio=only_audio, hierarchy=hierarchy))
+            cors.append(self._get_cate_by_page(
+                cate_id, path, time_from, time_to, page, min(pagesize, num), order, keyword, quality,
+                series, image=image, subtitle=subtitle, dm=dm, only_audio=only_audio, codec=codec))
             num -= pagesize
             page += 1
         await asyncio.gather(*cors)
 
-    async def _get_cate_videos_by_page(self, cate_id, time_from, time_to, pn=1, num=30, order='click', keyword='',
-                                       quality=0, series=True, image=False, subtitle=False, dm=False,
-                                       only_audio=False, hierarchy=True):
+    async def _get_cate_by_page(self, cate_id, path: Path,
+                                time_from, time_to, pn=1, num=30, order: CateOrder = CateOrder.click, keyword='',
+                                quality: Union[str, int] = 0,
+                                series=True, image=False, subtitle=False, dm=False, only_audio=False, codec=''):
         bvids = await api.get_cate_page_info(self.client, cate_id, time_from, time_to, pn, 30, order, keyword)
         bvids = bvids[:num]
         func = self.get_series if series else self.get_video
         # noinspection PyArgumentList
-        cors = [func(f"https://www.bilibili.com/video/{i}", quality=quality,
-                     image=image, subtitle=subtitle, dm=dm, only_audio=only_audio, hierarchy=hierarchy)
+        cors = [func(f"https://www.bilibili.com/video/{i}", path=path, quality=quality, codec=codec,
+                     image=image, subtitle=subtitle, dm=dm, only_audio=only_audio)
                 for i in bvids]
         await asyncio.gather(*cors)
 
-    async def get_up_videos(self, url_or_mid: str, num=10, order='pubdate', keyword='', quality: Union[int, str] = 0,
-                            series=True, image=False, subtitle=False, dm=False, only_audio=False,
-                            hierarchy: Union[bool, str] = True):
+    class UpOrder(Enum):
+        pubdate = 'pubdate'
+        click = 'click'
+        stow = 'stow'
+
+    async def get_up(self, url_or_mid: str, path: Annotated[Path, str2path] = Path('.'),
+                     num=10, order: UpOrder = UpOrder.pubdate, keyword='', quality: Union[str, int] = 0,
+                     series=True, image=False, subtitle=False, dm=False, only_audio=False, codec='', ):
         """
-
+        下载up主视频
+        :cli short: up
         :param url_or_mid: b站用户空间页面url 或b站用户id，在空间页面的url中可以找到
+        :param path: 保存路径
         :param num: 下载总数
         :param order: 何种排序，b站支持：最新发布pubdate，最多播放click，最多收藏stow
         :param keyword: 过滤关键词
         :param quality: 画面质量，0为可以观看的最高画质，越大质量越低，超过范围时自动选择最低画质，或者直接使用字符串指定'1080p'等名称
         :param series: 每个视频是否下载所有p，False时仅下载系列中的第一个视频
         :param image: 是否下载封面
         :param subtitle: 是否下载字幕
         :param dm: 是否下载弹幕
         :param only_audio: 是否仅下载音频
-        :param hierarchy:
+        :param codec: 视频编码
         :return:
         """
         ps = 30
         up_name, total_size, bv_ids = await api.get_up_info(self.client, url_or_mid, 1, ps, order, keyword)
-        if hierarchy:
-            hierarchy = self._make_hierarchy_dir(hierarchy, legal_title(f"【up】{up_name}"))
+        if self.hierarchy:
+            path /= legal_title(f"【up】{up_name}")
+            path.mkdir(parents=True, exist_ok=True)
         num = min(total_size, num)
         page_nums = num // ps + min(1, num % ps)
         cors = []
         for i in range(page_nums):
             if i + 1 == page_nums:
                 p_num = num - (page_nums - 1) * ps
             else:
                 p_num = ps
-            cors.append(self._get_up_videos_by_page(url_or_mid, i + 1, p_num, order, keyword, quality, series,
-                                                    image=image, subtitle=subtitle, dm=dm, only_audio=only_audio,
-                                                    hierarchy=hierarchy))
+            cors.append(self._get_up_by_page(
+                url_or_mid, path, i + 1, p_num, order, keyword, quality, series, image=image,
+                subtitle=subtitle, dm=dm, only_audio=only_audio, codec=codec))
         await asyncio.gather(*cors)
 
-    async def _get_up_videos_by_page(self, url_or_mid, pn=1, num=30, order='pubdate', keyword='', quality=0,
-                                     series=True, image=False, subtitle=False, dm=False, only_audio=False,
-                                     hierarchy=None):
+    async def _get_up_by_page(self, url_or_mid, path: Path,
+                              pn=1, num=30, order=UpOrder.pubdate, keyword='', quality: Union[str, int] = 0,
+                              series=True, image=False, subtitle=False, dm=False, only_audio=False, codec='', ):
         ps = 30
         num = min(ps, num)
         _, _, bvids = await api.get_up_info(self.client, url_or_mid, pn, ps, order, keyword)
         bvids = bvids[:num]
         func = self.get_series if series else self.get_video
         # noinspection PyArgumentList
         await asyncio.gather(
-            *[func(f'https://www.bilibili.com/video/{bv}', quality=quality,
-                   image=image, subtitle=subtitle, dm=dm, only_audio=only_audio, hierarchy=hierarchy) for bv in bvids])
+            *[func(f'https://www.bilibili.com/video/{bv}', path=path, quality=quality, codec=codec,
+                   image=image, subtitle=subtitle, dm=dm, only_audio=only_audio) for bv in bvids])
 
-    async def get_series(self, url: str, quality: Union[str, int] = 0, image=False, subtitle=False,
-                         dm=False, only_audio=False, p_range: Sequence[int] = None,
-                         hierarchy: Union[bool, str] = True):
+    async def get_series(self, url: str, path: Annotated[Path, str2path] = Path('.'),
+                         quality: Union[str, int] = 0, image: bool = False, subtitle=False,
+                         dm=False, only_audio=False, p_range: Tuple[int, int] = None, codec: str = ''):
         """
         下载某个系列（包括up发布的多p投稿，动画，电视剧，电影等）的所有视频。只有一个视频的情况下仍然可用该方法
-
+        :cli short: s
         :param url: 系列中任意一个视频的url
+        :param path: 保存路径
         :param quality: 画面质量，0为可以观看的最高画质，越大质量越低，超过范围时自动选择最低画质，或者直接使用字符串指定'1080p'等名称
         :param image: 是否下载封面
         :param subtitle: 是否下载字幕
         :param dm: 是否下载弹幕
         :param only_audio: 是否仅下载音频
         :param p_range: 下载集数范围，例如(1, 3)：P1至P3
-        :param hierarchy:
+        :param codec: 视频编码
         :return:
         """
         try:
-            video_info = await api.get_video_info(self.client, url)
-        except AttributeError as e:
-            logger.warning(f'{e} {url}')
-            return
-        title = video_info.title
-        pages = video_info.pages
-        p = video_info.p
-        if hierarchy and len(pages) > 1:
-            hierarchy = self._make_hierarchy_dir(hierarchy, title)
-        else:
-            hierarchy = hierarchy if type(hierarchy) is str else ''  # incase hierarchy is False
-        cors = [self.get_video(p_url, quality, add_name,
-                               image=image,
-                               subtitle=subtitle, dm=dm, only_audio=only_audio, hierarchy=hierarchy,
-                               extra=video_info if idx == p else None)
-                for idx, (add_name, p_url) in enumerate(pages)]
+            async with self.api_sema:
+                video_info = await api.get_video_info(self.client, url)
+        except (APIResourceError, APIUnsupportedError) as e:
+            return self.logger.warning(e)
+        if self.hierarchy and len(video_info.pages) > 1:
+            path /= video_info.title
+            path.mkdir(parents=True, exist_ok=True)
+        cors = [self.get_video(p.p_url, path=path,
+                               quality=quality, image=image, subtitle=subtitle, dm=dm,
+                               only_audio=only_audio, codec=codec,
+                               video_info=video_info if idx == video_info.p else None)
+                for idx, p in enumerate(video_info.pages)]
         if p_range:
             cors = cors_slice(cors, p_range)
         await asyncio.gather(*cors)
 
-    async def get_video(self, url: str, quality: Union[str, int] = 0, add_name='', image=False, subtitle=False,
-                        dm=False, only_audio=False, hierarchy: str = '', extra=None):
+    async def get_video(self, url: str, path: Annotated[Path, str2path] = Path('.'),
+                        quality: Union[str, int] = 0, image=False, subtitle=False, dm=False, only_audio=False,
+                        codec: str = '', time_range: Annotated[Tuple[int, int], parse_time_range] = None,
+                        video_info: api.VideoInfo = None):
         """
         下载单个视频
-
+        :cli short: v
         :param url: 视频的url
+        :param path: 保存路径
         :param quality: 画面质量，0为可以观看的最高画质，越大质量越低，超过范围时自动选择最低画质，或者直接使用字符串指定'1080p'等名称
-        :param add_name: 给文件的额外添加名，用户请直接保持默认
         :param image: 是否下载封面
         :param subtitle: 是否下载字幕
         :param dm: 是否下载弹幕
         :param only_audio: 是否仅下载音频
-        :param hierarchy:
-        :param extra: 额外数据，提供时不用再次请求页面
+        :param codec: 视频编码（可通过codec获取）
+        :param time_range: 切片的时间范围，例如(10, 20)：从第10秒到第20秒，或字符串如'00:00:10-00:00:20' (hour:minute:second)
+        :param video_info: 额外数据，提供时不用再次请求页面
         :return:
         """
         async with self.v_sema:
-            if not extra:
+            if not video_info:
                 try:
-                    extra = await api.get_video_info(self.client, url)
-                except AttributeError as e:
-                    logger.warning(f'{url} {e}')
-                    return
-            title = extra.h1_title
-            title = legal_title(title, add_name)
-            extra.title = title  # update extra title
-            dash = extra.dash
-            img_url = extra.img_url
-            formats = extra.support_formats
-            if not dash:
-                logger.warning(f'{extra.title} 需要大会员或该地区不支持')
-                return
-            # choose video quality
-            try:
-                video_info, video_urls = choose_quality(dash, formats, quality)
-            except ValueError:
-                logger.warning(f"{extra.title} 清晰度<{quality}>不可用，请检查输入是否正确或是否需要大会员")
-                return
-            # for audio, choose the highest quality
-            audio_info = dash['audio'][0]
-            audio_urls = (audio_info['base_url'], *(audio_info['backup_url'] if audio_info['backup_url'] else ()))
-
-            file_dir = f'{self.videos_dir}/{hierarchy}' if hierarchy else self.videos_dir
-            task_id = self.progress.add_task(
-                total=1, description=title if len(title) < 33 else f'{title[:15]}...{title[-15:]}', visible=False)
-            cors = []
-            # add cor according to params
-            if not only_audio:
-                if os.path.exists(f'{file_dir}/{title}.mp4'):
-                    logger.info(f'[green]已存在[/green] {title}.mp4')
+                    video_info = await api.get_video_info(self.client, url)
+                except (APIResourceError, APIUnsupportedError) as e:
+                    return self.logger.warning(e)
+            p_name = legal_title(video_info.pages[video_info.p].p_name)
+            task_name = legal_title(video_info.h1_title, p_name)
+            # if title is too long, use p_name as base_name
+            base_name = p_name if len(video_info.h1_title) > self.title_overflow and self.hierarchy and p_name else \
+                task_name
+            media_name = base_name if not time_range else legal_title(base_name, *map(t2s, time_range))
+            media_cors = []
+            task_id = await self.progress.add_task(total=None, description=task_name)
+            if video_info.dash:
+                try:  # choose video quality
+                    video, audio = video_info.dash.choose_quality(quality, codec)
+                except KeyError:
+                    self.logger.warning(
+                        f"{task_name} 清晰度<{quality}> 编码<{codec}>不可用，请检查输入是否正确或是否需要大会员")
                 else:
-                    cors.append(self.get_media(video_urls, f'{title}-video', task_id, hierarchy))
-                    cors.append(self.get_media(audio_urls, f'{title}-audio', task_id, hierarchy))
+                    tmp: List[Tuple[api.Media, Path]] = []
+                    # 1. only video
+                    if not audio and not only_audio:
+                        tmp.append((video, path / f'{media_name}.mp4'))
+                    # 2. video and audio
+                    elif audio and not only_audio:
+                        exists, media_path = path_check(path / f'{media_name}.mp4')
+                        if exists:
+                            self.logger.info(f'[green]已存在[/green] {media_path.name}')
+                        else:
+                            tmp.append((video, path / f'{media_name}-v'))
+                            tmp.append((audio, path / f'{media_name}-a'))
+                            # task need to be merged
+                            await self.progress.update(task_id=task_id, upper=ffmpeg.combine)
+                    # 3. only audio
+                    elif audio and only_audio:
+                        tmp.append((audio, path / f'{media_name}{audio.suffix}'))
+                    else:
+                        self.logger.warning(f"No audio for {task_name}")
+                    # convert to coroutines
+                    if not time_range:
+                        media_cors.extend(self.get_file(t[0].urls, path=t[1], task_id=task_id) for t in tmp)
+                    else:
+                        if len(tmp) > 0:
+                            fut = asyncio.Future()  # to fix key frame
+                            v = tmp[0]
+                            media_cors.append(self.get_media_clip(
+                                v[0].urls, v[1], time_range, init_range=v[0].segment_base['initialization'],
+                                seg_range=v[0].segment_base['index_range'], set_s=fut, task_id=task_id))
+                        if len(tmp) > 1:  # with audio
+                            a = tmp[1]
+                            media_cors.append(self.get_media_clip(
+                                a[0].urls, a[1], time_range, init_range=a[0].segment_base['initialization'],
+                                seg_range=a[0].segment_base['index_range'], get_s=fut, task_id=task_id))
+
+            elif video_info.other:
+                self.logger.warning(
+                    f"{task_name} 未解析到dash资源，转入durl mp4/flv下载（不需要会员的电影/番剧预览，不支持dash的视频）")
+                media_name = base_name
+                if len(video_info.other) == 1:
+                    m = video_info.other[0]
+                    media_cors.append(
+                        self.get_file(m.urls, path=path / f'{media_name}.{m.suffix}', task_id=task_id))
+                else:
+                    exist, media_path = path_check(path / f'{media_name}.mp4')
+                    if exist:
+                        self.logger.info(f'[green]已存在[/green] {media_path.name}')
+                    else:
+                        p_sema = asyncio.Semaphore(self.part_concurrency)
+
+                        async def _get_file(media: api.Media, p: Path) -> Path:
+                            async with p_sema:
+                                return await self.get_file(media.urls, path=p, task_id=task_id)
+
+                        for i, m in enumerate(video_info.other):
+                            f = f'{media_name}-{i}.{m.suffix}'
+                            media_cors.append(_get_file(m, path / f))
+                        await self.progress.update(task_id=task_id, upper=ffmpeg.concat)
             else:
-                cors.append(self.get_media(audio_urls, f'{title}.mp3', task_id, hierarchy))
+                self.logger.warning(f'{task_name} 需要大会员或该地区不支持')
             # additional task
+            add_cors = []
             if image or subtitle or dm:
-                extra_hierarchy = self._make_hierarchy_dir(hierarchy if hierarchy else True, 'extra')
+                extra_path = path / "extra" if self.hierarchy else path
+                extra_path.mkdir(exist_ok=True)
                 if image:
-                    cors.append(self._get_static(img_url, title, hierarchy=extra_hierarchy))
+                    add_cors.append(self.get_static(video_info.img_url, path=extra_path / base_name))
                 if subtitle:
-                    cors.append(self.get_subtitle(url, extra=extra, hierarchy=extra_hierarchy))
+                    add_cors.append(self.get_subtitle(url, path=extra_path, video_info=video_info))
                 if dm:
-                    w, h = video_info['width'], video_info['height']
-                    cors.append(
-                        self.get_dm(url, convert_func=dm2ass_factory(w, h), hierarchy=extra_hierarchy, extra=extra))
-            await asyncio.gather(*cors)
-
-        if not only_audio and not os.path.exists(f'{file_dir}/{title}.mp4'):
-            await run_process(
-                ['ffmpeg', '-i', f'{file_dir}/{title}-video', '-i', f'{file_dir}/{title}-audio',
-                 '-codec', 'copy', f'{file_dir}/{title}.mp4', '-loglevel', 'quiet'])
-            os.remove(f'{file_dir}/{title}-video')
-            os.remove(f'{file_dir}/{title}-audio')
-        # make progress invisible
-        if self.progress.tasks[task_id].visible:
-            self.progress.update(task_id, advance=1, visible=False)
-            logger.info(f'[cyan]已完成[/cyan] {title}{".mp3" if only_audio else ".mp4"}')
+                    try:
+                        width, height = video.width, video.height
+                    except UnboundLocalError:
+                        width, height = 1920, 1080
+                    add_cors.append(self.get_dm(
+                        url, path=extra_path, convert_func=_dm2ass_factory(width, height), video_info=video_info))
+            path_lst, _ = await asyncio.gather(asyncio.gather(*media_cors), asyncio.gather(*add_cors))
+
+        if upper := self.progress.tasks[task_id].fields.get('upper', None):
+            await upper(path_lst, media_path)
+            self.logger.info(f'[cyan]已完成[/cyan] {media_path.name}')
+        await self.progress.update(task_id, visible=False)
 
-    async def get_dm(self, url, update=False, convert_func=None,
-                     hierarchy: str = '', extra=None):
+    async def get_dm(self, url: str, path: Annotated[Path, str2path] = Path('.'),
+                     update: bool = False, convert_func=_dm2ass_factory(1920, 1080), video_info: api.VideoInfo = None):
         """
-
+        下载视频的弹幕
+        :cli short: dm
         :param url: 视频url
+        :param path: 保存路径
         :param update: 是否更新覆盖之前下载的弹幕文件
-        :param convert_func:
-        :param hierarchy:
-        :param extra: 额外数据，提供则不再访问前端
+        :param convert_func: function used to convert original danmaku bytes
+        :param video_info: 额外数据，提供则不再访问前端
         :return:
         """
-        if not extra:
-            extra = await api.get_video_info(self.client, url)
-        title = extra.title
-        aid, cid = extra.aid, extra.cid
-
-        file_dir = f'{self.videos_dir}/{hierarchy}' if hierarchy else self.videos_dir
-        file_type = '.' + ('bin' if not convert_func else convert_func.__name__.split('2')[-1])
-        file_name = f"{title}-弹幕{file_type}"
-        file_path = f'{file_dir}/{file_name}'
-        if not update and os.path.exists(file_path):
-            logger.info(f"[green]已存在[/green] {file_name}")
+        if not video_info:
+            video_info = await api.get_video_info(self.client, url)
+        aid, cid = video_info.aid, video_info.cid
+        file_type = '.' + ('pb' if not convert_func else convert_func.__name__.split('2')[-1])
+        p_name = video_info.pages[video_info.p].p_name
+        # to avoid file name too long bug
+        if len(video_info.h1_title) > self.title_overflow and self.hierarchy and p_name:
+            file_name = legal_title(p_name, "弹幕") + file_type
+        else:
+            file_name = legal_title(video_info.h1_title, p_name, "弹幕") + file_type
+        file_path = path / file_name
+        exist, file_path = path_check(file_path)
+        if not update and exist:
+            self.logger.info(f"[green]已存在[/green] {file_name}")
             return file_path
-        dm_urls = await api.get_dm_info(self.client, aid, cid)
+        dm_urls = await api.get_dm_urls(self.client, aid, cid)
         cors = [req_retry(self.client, dm_url) for dm_url in dm_urls]
         results = await asyncio.gather(*cors)
         content = b''.join(res.content for res in results)
         content = convert_func(content) if convert_func else content
         if asyncio.iscoroutine(content):
             content = await content
         async with aiofiles.open(file_path, 'wb') as f:
             await f.write(content)
-        logger.info(f"[cyan]已完成[/cyan] {file_name}")
+        self.logger.info(f"[cyan]已完成[/cyan] {file_name}")
         return file_path
 
-    async def get_subtitle(self, url, convert=True, hierarchy: str = '', extra=None):
+    async def get_subtitle(self, url: str, path: Annotated[Path, str2path] = Path('.'),
+                           convert_func=json2srt, video_info: api.VideoInfo = None):
         """
-        获取某个视频的字幕文件
-
+        下载视频的字幕文件
+        :cli short: sub
         :param url: 视频url
-        :param convert: 是否转换成srt
-        :param hierarchy:
-        :param extra: 额外数据，提供则不再访问前端
+        :param path: 字幕文件保存路径
+        :param convert_func: function used to convert original subtitle text
+        :param video_info: 额外数据，提供则不再访问前端
         :return:
         """
-        if not extra:
-            extra = await api.get_video_info(self.client, url)
-        bvid = extra.bvid
-        p, cid = extra.p, extra.cid
-        title = extra.title
-        add_name = extra.pages[p][0]
-        title = legal_title(title, add_name)
+        if not video_info:
+            video_info = await api.get_video_info(self.client, url)
+        p, cid = video_info.p, video_info.cid
+        p_name = video_info.pages[p].p_name
         try:
-            subtitles = await api.get_subtitle_info(self.client, bvid, cid)
-        except AttributeError as e:
-            logger.warning(f'{url} {e}')
-            return
+            subtitles = await api.get_subtitle_info(self.client, video_info.bvid, cid)
+        except APIError as e:
+            return self.logger.warning(e)
         cors = []
+
         for sub_url, sub_name in subtitles:
-            file_name = f"{title}-{sub_name}"
-            cors.append(self._get_static(sub_url, file_name, convert_func=json2srt if convert else None,
-                                         hierarchy=hierarchy))
+            if len(video_info.h1_title) > self.title_overflow and self.hierarchy and p_name:
+                file_name = legal_title(p_name, sub_name)
+            else:
+                file_name = legal_title(video_info.h1_title, p_name, sub_name)
+            cors.append(self.get_static(sub_url, path / file_name, convert_func=convert_func))
         paths = await asyncio.gather(*cors)
         return paths
 
-
-@Handler(name='bilibili')
-def handle(
-        method: str,
-        key: str,
-        videos_dir: str,
-        video_concurrency: int,
-        part_concurrency: int,
-        cookie: str,
-        quality: Union[str, int],
-        days: int,
-        num: int,
-        order: str,
-        keyword: str,
-        no_series: bool,
-        hierarchy: bool,
-        image: bool,
-        subtitle: bool,
-        dm: bool,
-        only_audio: bool,
-        p_range,
-):
-    d = DownloaderBilibili(videos_dir=videos_dir,
-                           video_concurrency=video_concurrency,
-                           part_concurrency=part_concurrency,
-                           sess_data=cookie)
-    if method == 'get_series' or method == 's':
-        cor = d.get_series(key, quality=quality, image=image, subtitle=subtitle, dm=dm, only_audio=only_audio,
-                           p_range=p_range, hierarchy=hierarchy)
-    elif method == 'get_video' or method == 'v':
-        cor = d.get_video(key, quality=quality,
-                          image=image, subtitle=subtitle, dm=dm, only_audio=only_audio)
-    elif method == 'get_up' or method == 'up':
-        cor = d.get_up_videos(
-            key, quality=quality, num=num, order=order, keyword=keyword, series=no_series,
-            image=image, subtitle=subtitle, dm=dm, only_audio=only_audio, hierarchy=hierarchy
-        )
-    elif method == 'get_cate' or method == 'cate':
-        cor = d.get_cate_videos(
-            key, quality=quality, num=num, order=order, keyword=keyword, days=days, series=no_series,
-            image=image, subtitle=subtitle, dm=dm, only_audio=only_audio, hierarchy=hierarchy)
-    elif method == 'get_favour' or method == 'fav':
-        cor = d.get_favour(key, quality=quality, num=num, keyword=keyword, series=no_series,
-                           image=image, subtitle=subtitle, dm=dm, only_audio=only_audio, hierarchy=hierarchy)
-    elif method == 'get_collect' or method == 'col':
-        cor = d.get_collect_or_list(key, quality=quality,
-                                    image=image, subtitle=subtitle, dm=dm, only_audio=only_audio,
-                                    hierarchy=hierarchy)
-    else:
-        raise ValueError(f'For {d.__class__.__name__} "{method}" is not available')
-    return d, cor
+    @classmethod
+    def decide_handle(cls, method_name: str, keys: Tuple[str, ...]):
+        return method_name in {'cate', 'get_cate'} or super().decide_handle(method_name, keys)
```

### Comparing `bilix-0.9.4/bilix/download/downloader_jable.py` & `bilix-1.0a0/bilix/sites/yinghuacd/downloader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,90 @@
 import asyncio
-import re
-
+from pathlib import Path
 import httpx
-import bilix.api.jable as api
-from bilix.assign import Handler
+import re
+from m3u8 import Segment
+from typing import Union, Tuple, Annotated
+from . import api
+from bilix.utils import legal_title, cors_slice
 from bilix.download.base_downloader_m3u8 import BaseDownloaderM3u8
+from bilix.exception import APIError
+from bilix.download.utils import parse_speed_str, str2path
 
 
-class DownloaderJable(BaseDownloaderM3u8):
-    def __init__(self, videos_dir: str = "videos", video_concurrency: int = 3, part_concurrency: int = 10):
-        client = httpx.AsyncClient(
-            headers={'user-agent': 'PostmanRuntime/7.29.0', "referer": "https://jable.tv"}, http2=False)
-        super(DownloaderJable, self).__init__(client, videos_dir, video_concurrency, part_concurrency)
-
-    async def get_video(self, url: str, image=True, hierarchy=True):
-        video_info = await api.get_video_info(self.client, url)
-        if hierarchy:
-            hierarchy = self._make_hierarchy_dir(hierarchy, f"{video_info.avid} {video_info.model_name}")
-        cors = [self.get_m3u8_video(m3u8_url=video_info.m3u8_url, name=video_info.title,
-                                    hierarchy=hierarchy if hierarchy else '')]
-        if image:
-            cors.append(self._get_static(video_info.img_url, name=video_info.title,
-                                         hierarchy=hierarchy if hierarchy else ''))
+class DownloaderYinghuacd(BaseDownloaderM3u8):
+    def __init__(
+            self,
+            *,
+            stream_client: httpx.AsyncClient = None,
+            api_client: httpx.AsyncClient = None,
+            browser: str = None,
+            speed_limit: Annotated[float, parse_speed_str] = None,
+            stream_retry: int = 5,
+            progress=None,
+            logger=None,
+            part_concurrency: int = 10,
+            video_concurrency: Union[int, asyncio.Semaphore] = 3,
+            hierarchy: bool = True,
+    ):
+        stream_client = stream_client or httpx.AsyncClient()
+        super(DownloaderYinghuacd, self).__init__(
+            client=stream_client,
+            browser=browser,
+            speed_limit=speed_limit,
+            stream_retry=stream_retry,
+            progress=progress,
+            logger=logger,
+            part_concurrency=part_concurrency,
+            video_concurrency=video_concurrency,
+        )
+        self.api_client = api_client or httpx.AsyncClient(**api.dft_client_settings)
+        self.hierarchy = hierarchy
+
+    def _after_seg(self, seg: Segment, content: bytearray) -> bytearray:
+        # in case .png
+        if re.fullmatch(r'.*\.png', seg.absolute_uri):
+            _, _, content = content.partition(b'\x47\x40')
+        return content
+
+    async def get_series(self, url: str, path: Annotated[Path, str2path] = Path("."),
+                         p_range: Tuple[int, int] = None):
+        """
+        :cli short: s
+        :param url:
+        :param path:
+        :param p_range:
+        :return:
+        """
+        video_info = await api.get_video_info(self.api_client, url)
+        if self.hierarchy:
+            path /= video_info.title
+            path.mkdir(parents=True, exist_ok=True)
+        cors = [self.get_video(u, path=path, video_info=video_info if u == url else None)
+                for _, u in video_info.play_info]
+        if p_range:
+            cors = cors_slice(cors, p_range)
         await asyncio.gather(*cors)
 
-
-@Handler('jable')
-def handle(
-        method: str,
-        key: str,
-        videos_dir: str,
-        video_concurrency: int,
-        part_concurrency: int,
-        cookie: str,
-        quality: int,
-        days: int,
-        num: int,
-        order: str,
-        keyword: str,
-        no_series: bool,
-        hierarchy: bool,
-        image: bool,
-        subtitle: bool,
-        dm: bool,
-        only_audio: bool,
-        p_range,
-):
-    if 'jable' in key or re.match(r"[A-Za-z]+-\d+", key):
-        d = DownloaderJable(videos_dir=videos_dir, video_concurrency=video_concurrency,
-                            part_concurrency=part_concurrency)
-        if method == 'get_video' or method == 'v':
-            cor = d.get_video(key, image=image, hierarchy=hierarchy)
-            return d, cor
-        raise ValueError(f'For {d.__class__.__name__} "{method}" is not available')
+    async def get_video(self, url: str, path: Annotated[Path, str2path] = Path('.'),
+                        time_range: Tuple[int, int] = None, video_info=None):
+        """
+        :cli short: v
+        :param url:
+        :param path:
+        :param time_range:
+        :param video_info:
+        :return:
+        """
+        if video_info is None:
+            try:
+                video_info = await api.get_video_info(self.api_client, url)
+            except APIError as e:
+                return self.logger.error(e)
+        else:
+            video_info = video_info
+        name = legal_title(video_info.title, video_info.sub_title)
+        await self.get_m3u8_video(m3u8_url=video_info.m3u8_url, path=path / f'{name}.mp4', time_range=time_range)
+
+    @classmethod
+    def decide_handle(cls, method: str, keys: Tuple[str, ...]):
+        return 'yinghuacd.' in keys[0]
```

### Comparing `bilix-0.9.4/bilix/download/downloader_yinghuacd.py` & `bilix-1.0a0/bilix/sites/cctv/downloader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,78 @@
 import asyncio
+import re
+import logging
+from pathlib import Path
+from typing import Union, Tuple, Annotated
 import httpx
-from typing import Sequence
-
-import bilix.api.yinghuacd as api
-from bilix.assign import Handler
-from bilix.log import logger
-from bilix.utils import legal_title, cors_slice
 from bilix.download.base_downloader_m3u8 import BaseDownloaderM3u8
-
-
-class DownloaderYinghuacd(BaseDownloaderM3u8):
-    def __init__(self, videos_dir: str = "videos", video_concurrency: int = 3, part_concurrency: int = 10):
-        client = httpx.AsyncClient(
-            headers={'user-agent': 'PostmanRuntime/7.29.0', "Referer": "http://www.yinghuacd.com"}, http2=False)
-        super(DownloaderYinghuacd, self).__init__(client, videos_dir, video_concurrency, part_concurrency)
-
-    async def get_series(self, url: str, p_range: Sequence[int] = None, hierarchy=True):
-        video_info = await api.get_video_info(self.client, url)
-        if hierarchy:
-            hierarchy = self._make_hierarchy_dir(hierarchy, video_info.title)
-        cors = [self.get_video(u, hierarchy=hierarchy if hierarchy else '', extra=video_info if u == url else None)
-                for _, u in video_info.play_info]
-        if p_range:
-            cors = cors_slice(cors, p_range)
-        await asyncio.gather(*cors)
-
-    async def get_video(self, url: str, hierarchy: str = '', extra=None):
-        if extra is None:
-            try:
-                video_info = await api.get_video_info(self.client, url)
-            except Exception as e:
-                logger.error(f"{url} 解析失败 {e}")
-                return
+from bilix.download.utils import parse_speed_str, str2path, parse_time_range
+from bilix.progress.abc import Progress
+from . import api
+
+
+class DownloaderCctv(BaseDownloaderM3u8):
+    pattern = re.compile(r'https?://(?:tv\.cctv\.com|tv\.cctv\.cn)/?[?/](?:pid=)?(\d+)(?:&vid=(\d+))?(?:&v=(\d+))?')
+
+    def __init__(
+            self,
+            *,
+            client: httpx.AsyncClient = None,
+            browser: str = None,
+            speed_limit: Annotated[float, parse_speed_str] = None,
+            stream_retry: int = 5,
+            progress: Progress = None,
+            logger: logging.Logger = None,
+            part_concurrency: int = 10,
+            video_concurrency: Union[int, asyncio.Semaphore] = 3,
+            # unique params
+            hierarchy: bool = True,
+    ):
+        client = client or httpx.AsyncClient(**api.dft_client_settings)
+        super(DownloaderCctv, self).__init__(
+            client=client,
+            browser=browser,
+            speed_limit=speed_limit,
+            stream_retry=stream_retry,
+            progress=progress,
+            logger=logger,
+            part_concurrency=part_concurrency,
+            video_concurrency=video_concurrency,
+        )
+        self.hierarchy = hierarchy
+
+    async def get_series(self, url: str, path: Annotated[Path, str2path] = Path('.'), quality: int = 0):
+        """
+        :cli short: s
+        :param url:
+        :param path:
+        :param quality: 画面质量，越大画面质量越低，超过可选范围时自动选择最低画质
+        :return:
+        """
+        pid, vide, vida = await api.get_id(self.client, url)
+        if vida is None:  # 单个视频
+            await self.get_video(pid, quality=quality)
+        else:  # 剧集
+            title, pids = await api.get_series_info(self.client, vide, vida)
+            if self.hierarchy:
+                path /= title
+                path.mkdir(parents=True, exist_ok=True)
+            await asyncio.gather(*[self.get_video(pid, path, quality) for pid in pids])
+
+    async def get_video(self, url_or_pid: str, path: Annotated[Path, str2path] = Path('.'),
+                        quality: int = 0, time_range: Annotated[Tuple[int, int], parse_time_range] = None):
+        """
+        :cli short: v
+        :param url_or_pid:
+        :param path:
+        :param quality: 画面质量，越大画面质量越低，超过可选范围时自动选择最低画质
+        :param time_range: 切片的时间范围，例如(10, 20)：从第10秒到第20秒，或字符串如'00:00:10-00:00:20' (hour:minute:second)
+        :return:
+        """
+        if url_or_pid.startswith('http'):
+            pid, _, _ = await api.get_id(self.client, url_or_pid)
         else:
-            video_info = extra
-        name = legal_title(video_info.title, video_info.sub_title)
-        await self.get_m3u8_video(m3u8_url=video_info.m3u8_url, name=name, hierarchy=hierarchy)
-
-
-@Handler(name='樱花动漫')
-def handle(
-        method: str,
-        key: str,
-        videos_dir: str,
-        video_concurrency: int,
-        part_concurrency: int,
-        cookie: str,
-        quality: int,
-        days: int,
-        num: int,
-        order: str,
-        keyword: str,
-        no_series: bool,
-        hierarchy: bool,
-        image: bool,
-        subtitle: bool,
-        dm: bool,
-        only_audio: bool,
-        p_range,
-):
-    if 'yinghuacd' in key:
-        d = DownloaderYinghuacd(videos_dir=videos_dir, video_concurrency=video_concurrency,
-                                part_concurrency=part_concurrency)
-        if method == 'get_series' or method == 's':
-            cor = d.get_series(key, p_range=p_range, hierarchy=hierarchy)
-            return d, cor
-        elif method == 'get_video' or method == 'v':
-            cor = d.get_video(key)
-            return d, cor
-        raise ValueError(f'For {d.__class__.__name__} "{method}" is not available')
-
-
-if __name__ == '__main__':
-    async def main():
-        async with DownloaderYinghuacd() as d:
-            await d.get_series("http://www.yinghuacd.com/v/5606-7.html")
-
-
-    logger.setLevel('DEBUG')
-    asyncio.run(main())
+            pid = url_or_pid
+        title, m3u8_urls = await api.get_media_info(self.client, pid)
+        m3u8_url = m3u8_urls[min(quality, len(m3u8_urls) - 1)]
+        file_path = await self.get_m3u8_video(m3u8_url, path / f"{title}.mp4", time_range=time_range)
+        return file_path
```

### Comparing `bilix-0.9.4/bilix/js/yhdmp.js` & `bilix-1.0a0/bilix/sites/yhdmp/yhdmp.js`

 * *Files identical despite different names*

### Comparing `bilix-0.9.4/bilix/process.py` & `bilix-1.0a0/bilix/_process.py`

 * *Files identical despite different names*

### Comparing `bilix-0.9.4/bilix/utils.py` & `bilix-1.0a0/bilix/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,80 +1,119 @@
-import asyncio
+"""
+some useful functions
+"""
 import html
-import os
+import json
 import re
-import random
-from typing import Union, Sequence, Coroutine
-import aiofiles
-import httpx
-
+import time
+from functools import wraps
+from urllib.parse import quote_plus
+from typing import Union, Sequence, Coroutine, List, Tuple, Optional
 from bilix.log import logger
 
 
 def cors_slice(cors: Sequence[Coroutine], p_range: Sequence[int]):
     h, t = p_range[0] - 1, p_range[1]
     assert 0 <= h <= t
     [cor.close() for idx, cor in enumerate(cors) if idx < h or idx >= t]  # avoid runtime warning
     cors = cors[h:t]
     return cors
 
 
-async def req_retry(client: httpx.AsyncClient, url_or_urls: Union[str, Sequence[str]], method='GET',
-                    follow_redirects=False, repeat_time=3, **kwargs) -> httpx.Response:
-    """Client request with multiple backup urls and retry"""
-    pre_exc = Exception("超过重复次数")  # predefine to avoid warning
-    for _ in range(repeat_time):
-        url = url_or_urls if type(url_or_urls) is str else random.choice(url_or_urls)
-        try:
-            res = await client.request(method, url, follow_redirects=follow_redirects, **kwargs)
-            res.raise_for_status()
-        except (httpx.ReadTimeout, httpx.ConnectTimeout, httpx.ConnectError) as e:
-            logger.warning(f'{method} {e.__class__.__name__} url: {url}')
-            pre_exc = e
-            await asyncio.sleep(0.1)
-        except httpx.HTTPStatusError as e:
-            logger.warning(f'{method} {e.response.status_code} {url}')
-            pre_exc = e
-            await asyncio.sleep(0.5)
-        except Exception as e:
-            logger.warning(f'{method} {e.__class__.__name__} 未知异常 url: {url}')
-            pre_exc = e
-            await asyncio.sleep(0.5)
-        else:
-            return res
-    logger.error(f"超过重复次数 {url_or_urls}")
-    raise pre_exc
-
-
-async def merge_files(file_list: Sequence[str], new_name: str):
-    first_file = file_list[0]
-    async with aiofiles.open(first_file, 'ab') as f:
-        for idx in range(1, len(file_list)):
-            async with aiofiles.open(file_list[idx], 'rb') as fa:
-                await f.write(await fa.read())
-            os.remove(file_list[idx])
-    os.rename(first_file, new_name)
-
-
-def legal_title(title, add_name=''):
+def legal_title(*parts: str, join_str: str = '-'):
     """
+    join several string parts to os illegal file/dir name (no illegal character and not too long).
+    auto skip empty.
 
-    :param title: 主标题
-    :param add_name: 分P名
+    :param parts:
+    :param join_str: the string to join each part
     :return:
     """
-    title, add_name = _replace(title), _replace(add_name)
-    title = _truncate(title)  # avoid OSError caused by title too long
-    return f'{title}-{add_name}' if add_name else title
+    return join_str.join(filter(lambda x: len(x) > 0, map(replace_illegal, parts)))
 
 
-def _replace(s: str):
+def replace_illegal(s: str):
+    """strip, unescape html and replace os illegal character in s"""
     s = s.strip()
     s = html.unescape(s)  # handel & "...
-    s = re.sub(r"[/\\:*?\"<>|\n]", '', s)  # replace illegal filename character
+    s = re.sub(r"[/\\:*?\"<>|\n\t]", '', s)  # replace illegal filename character
     return s
 
 
-def _truncate(s: str, target=150):
-    while len(s.encode('utf8')) > target - 3:
-        s = s[:-1]
-    return s
+def convert_size(total_bytes: int) -> str:
+    unit, suffix = pick_unit_and_suffix(
+        total_bytes, ["bytes", "kB", "MB", "GB", "TB", "PB", "EB", "ZB", "YB"], 1000
+    )
+    return f"{total_bytes / unit:,.2f}{suffix}"
+
+
+def pick_unit_and_suffix(size: int, suffixes: List[str], base: int) -> Tuple[int, str]:
+    """Borrowed from rich.filesize. Pick a suffix and base for the given size."""
+    for i, suffix in enumerate(suffixes):
+        unit = base ** i
+        if size < unit * base:
+            break
+    else:
+        raise ValueError('Invalid input')
+    return unit, suffix
+
+
+def valid_sess_data(sess_data: Optional[str]) -> str:
+    """check and encode sess_data"""
+    # url-encoding sess_data if it's not encoded
+    # https://github.com/HFrost0/bilix/pull/114https://github.com/HFrost0/bilix/pull/114
+    if sess_data and not re.search(r'(%[0-9A-Fa-f]{2})|(\+)', sess_data):
+        sess_data = quote_plus(sess_data)
+        logger.debug(f"sess_data encoded: {sess_data}")
+    return sess_data
+
+
+def t2s(t: int) -> str:
+    return str(t)
+
+
+def s2t(s: str) -> int:
+    """
+    :param s: hour:minute:second or xx(s) format input
+    :return:
+    """
+    if ':' not in s:
+        return int(s)
+    h, m, s = map(int, s.split(':'))
+    return h * 60 * 60 + m * 60 + s
+
+
+def json2srt(data: Union[bytes, str, dict]):
+    b = False
+    if type(data) is bytes:
+        data = data.decode('utf-8')
+        b = True
+    if type(data) is str:
+        data = json.loads(data)
+
+    def t2str(t):
+        ms = int(round(t % 1, 3) * 1000)
+        s = int(t)
+        m = s // 60
+        h = m // 60
+        m, s = m % 60, s % 60
+        t_str = f'{h:0>2}:{m:0>2}:{s:0>2},{ms:0>3}'
+        return t_str
+
+    res = ''
+    for idx, i in enumerate(data['body']):
+        from_time, to_time = t2str(i['from']), t2str(i['to'])
+        content = i['content']
+        res += f"{idx + 1}\n{from_time} --> {to_time}\n{content}\n\n"
+    return res.encode('utf-8') if b else res
+
+
+def timer(func):
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        start = time.monotonic_ns()
+        res = func(*args, **kwargs)
+        logger.debug(
+            f"{func.__name__} cost {time.monotonic_ns() - start} ns with args: {args}, kwargs: {kwargs} result: {res}")
+        return res
+
+    return wrapper
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

