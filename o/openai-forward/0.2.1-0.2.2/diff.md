# Comparing `tmp/openai_forward-0.2.1.tar.gz` & `tmp/openai_forward-0.2.2.tar.gz`

## Comparing `openai_forward-0.2.1.tar` & `openai_forward-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/__init__.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/__main__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/app.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/base.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/config.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/content/__init__.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/content/chat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/content/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/routers/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/routers/openai_v1.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/routers/schemas.py
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 openai_forward-0.2.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.2.1/LICENSE
--rw-r--r--   0        0        0     8223 2020-02-02 00:00:00.000000 openai_forward-0.2.1/README.md
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 openai_forward-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     9557 2020-02-02 00:00:00.000000 openai_forward-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/__init__.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/__main__.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/app.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/base.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/config.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/openai.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/content/__init__.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/content/chat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/content/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/routers/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/routers/openai_v1.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 openai_forward-0.2.2/openai_forward/routers/schemas.py
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 openai_forward-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.2.2/LICENSE
+-rw-r--r--   0        0        0    10855 2020-02-02 00:00:00.000000 openai_forward-0.2.2/README.md
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 openai_forward-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    12250 2020-02-02 00:00:00.000000 openai_forward-0.2.2/PKG-INFO
```

### Comparing `openai_forward-0.2.1/openai_forward/__main__.py` & `openai_forward-0.2.2/openai_forward/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,40 +29,50 @@
         base_url: str, None
         log_chat: str, None
         route_prefix: str, None
         ip_whitelist: str, None
         ip_blacklist: str, None
         """
         if base_url:
-            os.environ['OPENAI_BASE_URL'] = base_url
+            os.environ["OPENAI_BASE_URL"] = base_url
         if api_key:
-            os.environ['OPENAI_API_KEY'] = api_key
+            os.environ["OPENAI_API_KEY"] = api_key
         if forward_key:
-            os.environ['FORWARD_KEY'] = forward_key
+            os.environ["FORWARD_KEY"] = forward_key
         if log_chat:
-            os.environ['LOG_CHAT'] = log_chat
+            os.environ["LOG_CHAT"] = log_chat
         if route_prefix:
-            os.environ['ROUTE_PREFIX'] = route_prefix
+            os.environ["ROUTE_PREFIX"] = route_prefix
         if ip_whitelist:
-            os.environ['IP_WHITELIST'] = ip_whitelist
+            os.environ["IP_WHITELIST"] = ip_whitelist
         if ip_blacklist:
-            os.environ['IP_BLACKLIST'] = ip_blacklist
+            os.environ["IP_BLACKLIST"] = ip_blacklist
 
         ssl_keyfile = os.environ.get("ssl_keyfile", None) or None
         ssl_certfile = os.environ.get("ssl_certfile", None) or None
         uvicorn.run(
             app="openai_forward.app:app",
             host="0.0.0.0",
             port=port,
             workers=workers,
-            app_dir='..',
+            app_dir="..",
             ssl_keyfile=ssl_keyfile,
             ssl_certfile=ssl_certfile,
         )
 
+    @staticmethod
+    def convert(
+        log_path: str = "./Log/chat.log", target_path: str = "./Log/chat.jsonl"
+    ):
+        """Convert log file  to jsonl file"""
+        from openai_forward.tool import convert_chatlog_to_jsonl
+
+        print(f"Convert {log_path} to {target_path}")
+        convert_chatlog_to_jsonl(log_path, target_path)
+
 
 def main():
     fire.Fire(Cli)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `openai_forward-0.2.1/openai_forward/base.py` & `openai_forward-0.2.2/openai_forward/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,116 +3,104 @@
 
 import httpx
 from fastapi import HTTPException, Request, status
 from fastapi.responses import StreamingResponse
 from loguru import logger
 from starlette.background import BackgroundTask
 
-from .config import env2list, print_startup_info, setting_log
+from .config import print_startup_info, setting_log
 from .content.chat import ChatSaver
+from .tool import env2list
 
 
 class OpenaiBase:
     BASE_URL = os.environ.get("OPENAI_BASE_URL", "https://api.openai.com").strip()
     ROUTE_PREFIX = os.environ.get("ROUTE_PREFIX", "").strip()
     _LOG_CHAT = os.environ.get("LOG_CHAT", "False").strip().lower() == "true"
     _openai_api_key_list = env2list("OPENAI_API_KEY", sep=" ")
     _cycle_api_key = cycle(_openai_api_key_list)
-    _FWD_KEYS = env2list("FORWARD_KEY", sep=" ")
-    _use_forward_key = _openai_api_key_list != [] and _FWD_KEYS != []
+    _FWD_KEYS = set(env2list("FORWARD_KEY", sep=" "))
+    _no_auth_mode = _openai_api_key_list != [] and _FWD_KEYS == set()
     IP_WHITELIST = env2list("IP_WHITELIST", sep=" ")
     IP_BLACKLIST = env2list("IP_BLACKLIST", sep=" ")
 
     if ROUTE_PREFIX:
-        if ROUTE_PREFIX.endswith('/'):
+        if ROUTE_PREFIX.endswith("/"):
             ROUTE_PREFIX = ROUTE_PREFIX[:-1]
-        if not ROUTE_PREFIX.startswith('/'):
-            ROUTE_PREFIX = '/' + ROUTE_PREFIX
-    timeout = 30
+        if not ROUTE_PREFIX.startswith("/"):
+            ROUTE_PREFIX = "/" + ROUTE_PREFIX
+    timeout = 60
 
     print_startup_info(
-        BASE_URL, ROUTE_PREFIX, _openai_api_key_list, _FWD_KEYS, _LOG_CHAT
+        BASE_URL, ROUTE_PREFIX, _openai_api_key_list, _no_auth_mode, _LOG_CHAT
     )
     if _LOG_CHAT:
         setting_log(save_file=False)
-        chatsaver = ChatSaver(save_interval=10)
+        chatsaver = ChatSaver()
 
     def validate_request_host(self, ip):
         if self.IP_WHITELIST and ip not in self.IP_WHITELIST:
             raise HTTPException(
                 status_code=status.HTTP_403_FORBIDDEN,
                 detail=f"Forbidden, ip={ip} not in whitelist!",
             )
         if self.IP_BLACKLIST and ip in self.IP_BLACKLIST:
             raise HTTPException(
                 status_code=status.HTTP_403_FORBIDDEN,
                 detail=f"Forbidden, ip={ip} in blacklist!",
             )
 
     @classmethod
-    async def aiter_bytes(cls, r: httpx.Response, route_path: str):
-        bytes_ = b''
+    async def aiter_bytes(cls, r: httpx.Response, route_path: str, uid: str):
+        bytes_ = b""
         async for chunk in r.aiter_bytes():
             bytes_ += chunk
             yield chunk
         try:
             target_info = cls.chatsaver.parse_bytes_to_content(bytes_, route_path)
-            cls.chatsaver.add_chat({target_info['role']: target_info['content']})
+            cls.chatsaver.add_chat(
+                {target_info["role"]: target_info["content"], "uid": uid}
+            )
         except Exception as e:
             logger.debug(f"log chat (not) error:\n{e=}")
 
     @classmethod
     async def _reverse_proxy(cls, request: Request):
         client = httpx.AsyncClient(base_url=cls.BASE_URL, http1=True, http2=False)
         url_path = request.url.path
         url_path = url_path[len(cls.ROUTE_PREFIX) :]
-        url = httpx.URL(path=url_path, query=request.url.query.encode('utf-8'))
+        url = httpx.URL(path=url_path, query=request.url.query.encode("utf-8"))
         headers = dict(request.headers)
-        auth = headers.pop("authorization", None)
-        if auth and str(auth).startswith("Bearer sk-"):
-            tmp_headers = {'Authorization': auth}
-        elif cls._openai_api_key_list:
-            logger.info(f"Use forward key: {cls._use_forward_key}")
-            if cls._use_forward_key:
-                fk_prefix = "Bearer fk-"
-                logger.info(f"current forward key: {auth}")
-                if (
-                    auth
-                    and str(auth).startswith(fk_prefix)
-                    and auth[len("Bearer ") :] in cls._FWD_KEYS
-                ):
-                    auth = "Bearer " + next(cls._cycle_api_key)
-                    tmp_headers = {'Authorization': auth}
-                else:
-                    tmp_headers = {}
-            else:
-                auth = "Bearer " + next(cls._cycle_api_key)
-                tmp_headers = {'Authorization': auth}
-        else:
-            tmp_headers = {}
+        auth = headers.pop("authorization", "")
+        auth_headers_dict = {"Content-Type": "application/json", "Authorization": auth}
+        auth_prefix = "Bearer "
+        if cls._no_auth_mode or auth and auth[len(auth_prefix) :] in cls._FWD_KEYS:
+            auth = auth_prefix + next(cls._cycle_api_key)
+            auth_headers_dict["Authorization"] = auth
 
         log_chat_completions = False
-        if cls._LOG_CHAT and request.method == 'POST':
+        uid = None
+        if cls._LOG_CHAT and request.method == "POST":
             try:
                 chat_info = await cls.chatsaver.parse_payload_to_content(
                     request, route_path=url_path
                 )
                 if chat_info:
                     cls.chatsaver.add_chat(chat_info)
+                    uid = chat_info.get("uid")
                     log_chat_completions = True
             except Exception as e:
                 logger.debug(
                     f"log chat error:\n{request.client.host=} {request.method=}: {e}"
                 )
 
-        tmp_headers.update({"Content-Type": "application/json"})
         req = client.build_request(
             request.method,
             url,
-            headers=tmp_headers,
+            headers=auth_headers_dict,
             content=request.stream(),
             timeout=cls.timeout,
         )
         try:
             r = await client.send(req, stream=True)
         except (httpx.ConnectError, httpx.ConnectTimeout) as e:
             error_info = (
@@ -120,22 +108,23 @@
                 f"Please check if host={request.client.host} can access [{cls.BASE_URL}] successfully?"
             )
             logger.error(error_info)
             raise HTTPException(
                 status_code=status.HTTP_504_GATEWAY_TIMEOUT, detail=error_info
             )
         except Exception as e:
-            error_info = f"{type(e)}: {e}"
-            logger.error(error_info)
+            logger.exception(f"{type(e)}:")
             raise HTTPException(
-                status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=error_info
+                status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=e
             )
 
         aiter_bytes = (
-            cls.aiter_bytes(r, url_path) if log_chat_completions else r.aiter_bytes()
+            cls.aiter_bytes(r, url_path, uid)
+            if log_chat_completions
+            else r.aiter_bytes()
         )
         return StreamingResponse(
             aiter_bytes,
             status_code=r.status_code,
             media_type=r.headers.get("content-type"),
             background=BackgroundTask(r.aclose),
         )
```

### Comparing `openai_forward-0.2.1/openai_forward/config.py` & `openai_forward-0.2.2/openai_forward/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 import logging
 import os
 import sys
 import time
-from typing import Dict, List, Union
 
-import orjson
 from loguru import logger
 from rich import print
 from rich.panel import Panel
 from rich.table import Table
-from sparrow import relp
 
 
-def print_startup_info(base_url, route_prefix, api_key, forward_key, log_chat):
+def print_startup_info(base_url, route_prefix, api_key, no_auth_mode, log_chat):
     try:
         from dotenv import load_dotenv
 
-        load_dotenv('.env')
+        load_dotenv(".env")
     except Exception:
         ...
     route_prefix = route_prefix or "/"
     api_key_info = True if len(api_key) else False
-    forward_key_info = True if len(forward_key) else False
     table = Table(title="", box=None, width=100)
     table.add_column("base-url", justify="left", style="#df412f")
-    table.add_column("route-prefix", justify="center", style="#df412f")
-    table.add_column("openai-api-key", justify="center", style="green")
-    table.add_column("forward-key", justify="center", style="green")
+    table.add_column("route-prefix", justify="center", style="green")
+    table.add_column("api-key-polling-pool", justify="center", style="green")
+    table.add_column(
+        "no-auth-mode", justify="center", style="red" if no_auth_mode else "green"
+    )
     table.add_column("Log-chat", justify="center", style="green")
-    table.add_column("Log-dir", justify="center", style="#f5bb00")
     table.add_row(
         base_url,
         route_prefix,
         str(api_key_info),
-        str(forward_key_info),
+        str(no_auth_mode),
         str(log_chat),
-        "./Log/*.log",
     )
-    print(Panel(table, title="🤗openai-forward is ready to serve!", expand=False))
+    print(Panel(table, title="🤗 openai-forward is ready to serve! ", expand=False))
 
 
 class InterceptHandler(logging.Handler):
     def emit(self, record):
         # Get corresponding Loguru level if it exists
         try:
             level = logger.level(record.levelname).name
@@ -57,85 +53,38 @@
             level, record.getMessage()
         )
 
 
 def setting_log(save_file=False, log_name="openai_forward", multi_process=True):
     # TODO 修复时区配置
     if os.environ.get("TZ") == "Asia/Shanghai":
-        os.environ['TZ'] = "UTC-8"
-        if hasattr(time, 'tzset'):
+        os.environ["TZ"] = "UTC-8"
+        if hasattr(time, "tzset"):
             time.tzset()
 
     logging.root.handlers = [InterceptHandler()]
     for name in logging.root.manager.loggerDict.keys():
         logging.getLogger(name).handlers = []
         logging.getLogger(name).propagate = True
 
     config_handlers = [
         {"sink": sys.stdout, "level": "DEBUG"},
+        {
+            "sink": f"./Log/chat.log",
+            "enqueue": multi_process,
+            "rotation": "20 MB",
+            "filter": lambda record: "chat" in record["extra"],
+            "format": "{message}",
+        },
     ]
     if save_file:
         config_handlers += [
             {
                 "sink": f"./Log/{log_name}.log",
                 "enqueue": multi_process,
                 "rotation": "100 MB",
                 "level": "INFO",
             }
         ]
 
     logger_config = {"handlers": config_handlers}
     logger.configure(**logger_config)
-
-
-def yaml_dump(data, filepath, rel_path=False, mode='w'):
-    abs_path = relp(filepath, parents=1) if rel_path else filepath
-    from yaml import dump
-
-    try:
-        from yaml import CDumper as Dumper
-    except ImportError:
-        from yaml import Dumper
-    with open(abs_path, mode=mode, encoding="utf-8") as fw:
-        fw.write(dump(data, Dumper=Dumper, allow_unicode=True, indent=4))
-
-
-def yaml_load(filepath, rel_path=False, mode='r'):
-    abs_path = relp(filepath, parents=1) if rel_path else filepath
-    from yaml import load
-
-    try:
-        from yaml import CLoader as Loader
-    except ImportError:
-        from yaml import Loader
-    with open(abs_path, mode=mode, encoding="utf-8") as stream:
-        #     stream = stream.read()
-        content = load(stream, Loader=Loader)
-    return content
-
-
-def json_load(filepath: str, rel=False, mode='rb'):
-    abs_path = relp(filepath, parents=1) if rel else filepath
-    with open(abs_path, mode=mode) as f:
-        return orjson.loads(f.read())
-
-
-def json_dump(
-    data: Union[List, Dict], filepath: str, rel=False, indent_2=False, mode='wb'
-):
-    orjson_option = 0
-    if indent_2:
-        orjson_option = orjson.OPT_INDENT_2
-    abs_path = relp(filepath, parents=1) if rel else filepath
-    with open(abs_path, mode=mode) as f:
-        f.write(orjson.dumps(data, option=orjson_option))
-
-
-def str2list(s: str, sep=' '):
-    if s:
-        return [i.strip() for i in s.split(sep) if i.strip()]
-    else:
-        return []
-
-
-def env2list(env_name: str, sep=" "):
-    return str2list(os.environ.get(env_name, "").strip(), sep=sep)
```

### Comparing `openai_forward-0.2.1/openai_forward/routers/openai_v1.py` & `openai_forward-0.2.2/openai_forward/routers/openai_v1.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.1/openai_forward/routers/schemas.py` & `openai_forward-0.2.2/openai_forward/routers/schemas.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.1/.gitignore` & `openai_forward-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.1/LICENSE` & `openai_forward-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.1/README.md` & `openai_forward-0.2.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -31,208 +31,295 @@
         <img alt="pypi downloads" src="https://img.shields.io/pypi/dm/openai_forward">
     </a>
     <a href="https://codecov.io/gh/beidongjiedeguang/openai-forward">
         <img alt="codecov" src="https://codecov.io/gh/beidongjiedeguang/openai-forward/branch/dev/graph/badge.svg">
     </a>
 </p>
 
+<div align="center">
 
+[功能](#功能) |
+[部署指南](#部署指南) |
+[应用](#应用) |
+[配置选项](#配置选项) |
+[聊天日志](#聊天日志)
+
+[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/tejCum?referralCode=U0-kXv)  
+[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/beidongjiedeguang/openai-forward)
+
+</div>
 
 本项目用于解决一些地区无法直接访问OpenAI的问题，将该服务部署在可以正常访问openai
-api的服务器上，通过该服务转发OpenAI的请求。即搭建反向代理服务  
+api的服务器上，通过该服务转发OpenAI的请求。即搭建反向代理服务
 
 ---
 
 由本项目搭建的长期代理地址：
-> https://api.openai-forward.top  
-
+> https://api.openai-forward.com
 
+## 功能
 
-## 目录
-
-- [功能](#功能)
-- [部署指南](#部署指南)
-- [应用](#应用)
-- [配置选项](#配置选项)
-- [聊天日志](#聊天日志)
-- [高级配置](#高级配置)
+**基础功能**
 
-## 功能
-**基础功能**  
 - [x] 支持转发OpenAI所有接口
 - [x] 支持流式响应
 - [x] 支持指定转发路由前缀
 - [x] docker部署
 - [x] pip 安装部署
-- [x] vercel 一键个人免费部署
-  [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fbeidongjiedeguang%2Fopenai-forward&project-name=openai-forward&repository-name=openai-forward&framework=other)
 - [x] cloudflare 部署
+- [x] ~~Vercel一键部署(不建议)~~
+- [x] Railway 一键部署
+- [x] Render 一键部署
+
+**高级功能**
 
-**高级功能**  
 - [x] 实时记录聊天记录(包括流式响应的聊天内容)
 - [x] 允许输入多个openai api key 组成轮询池
-- [x] 自定义 api key (见高级配置)
-- [x] 支持请求IP验证(IP白名单与黑名单)
+- [x] 自定义 转发api key (见[高级配置](#高级配置))
 
 ## 部署指南
 
-提供四种部署方式
-1. [vps + pip 安装部署](deploy.md#pip-推荐) (推荐)
-2. [vps + Docker](deploy.md#docker-推荐) (推荐) 
-    > https://api.openai-forward.top 
-3. [一键Vercel部署](deploy.md#vercel-一键部署) (目前不推荐)
-   > ~~https://vercel.openai-forward.top~~  
-4. [cloudflare部署](deploy.md#cloudflare-部署) (推荐)
-   > https://cloudflare.openai-forward.top
+提供以下几种部署方式
+
+**有海外vps方案**
+
+1. [pip 安装部署](deploy.md#pip-推荐) (推荐)
+2. [Docker部署](deploy.md#docker-推荐) (推荐)
+   > https://api.openai-forward.com
+
+**无vps免费部署方案**
+
+1. [一键Vercel部署](deploy.md#vercel-一键部署) (不推荐)
+   > ~~https://vercel.openai-forward.com~~
+2. [cloudflare部署](deploy.md#cloudflare-部署) (推荐)
+   > https://cloudflare.openai-forward.com
+3. [Railway部署](deploy.md#Railway-一键部署)
+   > https://railway.openai-forward.com
+4. [Render一键部署](deploy.md#render-一键部署) (推荐)
+   > https://render.openai-forward.com
 
 ## 应用
 
 ### [聊天应用](https://chat.beidongjiedeguang.top)
 
 基于开源项目[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)搭建自己的chatgpt服务  
 替换docker启动命令中的 `BASE_URL`为我们自己搭建的代理服务地址
 
+<details markdown="1">
+<summary>Click for more details</summary>  
+
 ```bash 
 docker run -d \
     -p 3000:3000 \
     -e OPENAI_API_KEY="sk-******" \
-    -e BASE_URL="https://api.openai-forward.top" \
+    -e BASE_URL="https://api.openai-forward.com" \
     -e CODE="kunyuan" \
     yidadaa/chatgpt-next-web 
 ``` 
+
 这里部署了一个，供大家轻度使用:  
- https://chat.beidongjiedeguang.top , 访问密码: `kunyuan` 
+https://chat.beidongjiedeguang.top , 访问密码: `kunyuan`
+</details>
 
 ### 在代码中使用
 
+**Python**
+
+```diff
+  import openai
++ openai.api_base = "https://api.openai-forward.com/v1"
+  openai.api_key = "sk-******"
+```
+
+<details markdown="1">
+  <summary>More Examples</summary>
+
 **JS/TS**
 
 ```diff
   import { Configuration } from "openai";
   
   const configuration = new Configuration({
-+ basePath: "https://api.openai-forward.top/v1",
++ basePath: "https://api.openai-forward.com/v1",
   apiKey: "sk-******",
   });
 ```
 
-**Python**
-
-```diff
-  import openai
-+ openai.api_base = "https://api.openai-forward.top/v1"
-  openai.api_key = "sk-******"
-```
-
 **gpt-3.5-turbo**
+
 ```bash
-curl https://api.openai-forward.top/v1/chat/completions \
+curl https://api.openai-forward.com/v1/chat/completions \
   -H "Content-Type: application/json" \
   -H "Authorization: Bearer sk-******" \
   -d '{
     "model": "gpt-3.5-turbo",
     "messages": [{"role": "user", "content": "Hello!"}]
   }'
 ```
 
 **Image Generation (DALL-E)**
+
 ```bash
-curl --location 'https://api.openai-forward.top/v1/images/generations' \
+curl --location 'https://api.openai-forward.com/v1/images/generations' \
 --header 'Authorization: Bearer sk-******' \
 --header 'Content-Type: application/json' \
 --data '{
     "prompt": "A photo of a cat",
     "n": 1,
     "size": "512x512"
 }'
 ```
 
+</details>
 
 ## 配置选项
 
+配置的设置方式支持两种  
+一种为在shell中运行`openai-forward run --port=8000`的命令行方式指定;  
+另一种为读取环境变量的方式指定。
+
+<details markdown="1">
+<summary>Click for more details</summary>  
+
 **`openai-forward run`参数配置项**
 
-| 配置项       | 说明 | 默认值 |
-|-----------| --- | :---: |
-| --port    | 服务端口号 | 8000 |
-| --workers | 工作进程数 | 1 |
+| 配置项 | 说明                |          默认值           |
+|-----------------|-------------------|:----------------------:|
+| --port | 服务端口号             |          8000          |
+| --workers | 工作进程数             |           1            |
+| --base_url | 同 OPENAI_BASE_URL | https://api.openai.com |
+| --api_key | 同 OPENAI_API_KEY  |         `None`         |
+| --forward_key | 同 FORWARD_KEY     |         `None`         |
+| --route_prefix | 同 ROUTE_PREFIX    |          `None`          |
+| --log_chat | 同 LOG_CHAT        |        `False`         |
 
-更多参数 `openai-forward run --help` 查看
+也可通过 `openai-forward run --help` 查看
 
 **环境变量配置项**  
-支持从运行目录下的`.env`文件中读取: 
+支持从运行目录下的`.env`文件中读取
 
-| 环境变量            | 说明                                                              |           默认值            |
-|-----------------|-----------------------------------------------------------------|:------------------------:|
-| OPENAI_API_KEY  | 默认openai api key，支持多个默认api key, 以 `sk-` 开头， 以空格分割      |            无             |
-| FORWARD_KEY     | 允许调用方使用该key代替openai api key，支持多个forward key, 以`fk-` 开头, 以空格分割 |      无             |
-| OPENAI_BASE_URL | 转发base url                                                      | `https://api.openai.com` |
-| LOG_CHAT        | 是否记录聊天内容                                                        |          `true`          |
-| ROUTE_PREFIX    | 路由前缀                                                            |            无             |
-| IP_WHITELIST    | ip白名单, 空格分开                                                     |           无            |
-| IP_BLACKLIST    | ip黑名单, 空格分开                                                     |           无            | 
+| 环境变量            | 说明                                                                                                                                |           默认值            |
+|-----------------|-----------------------------------------------------------------------------------------------------------------------------------|:------------------------:|
+| OPENAI_BASE_URL  | 默认 openai官方 api 地址                                                                                                                |        https://api.openai.com           |
+| OPENAI_API_KEY  | 默认openai api key，支持多个默认api key, 以 `sk-` 开头， 以空格分割                                                                                 |            无             |
+| FORWARD_KEY     | 允许调用方使用该key代替openai api key，支持多个forward key, 以空格分割; 如果设置了OPENAI_API_KEY，而没有设置FORWARD_KEY, 则客户端调用时无需提供密钥, 此时出于安全考虑不建议FORWARD_KEY置空 |            无             |
+| OPENAI_BASE_URL | 转发base url                                                                                                                        | `https://api.openai.com` |
+| ROUTE_PREFIX    | 路由前缀                                                                                                                              |            无             |
+| LOG_CHAT        | 是否记录聊天内容                                                                                                                          |         `false`          |
 
+</details>
 
 ## 高级配置
 
 **设置api_key为自己设置的forward key**  
 需要配置 OPENAI_API_KEY 和 FORWARD_KEY, 例如
+<details markdown="1">
+  <summary>Click for more details</summary>
 
 ```bash
 OPENAI_API_KEY=sk-*******
 FORWARD_KEY=fk-****** # 这里fk-token由我们自己定义
 ```
+
 这里我们配置了FORWARD_KEY为`fk-******`, 那么后面客户端在调用时只需设置OPENAI_API_KEY为我们自定义的`fk-******` 即可。  
-这样的好处是在使用一些需要输入OPENAI_API_KEY的第三方应用时，我们可以使用`fk-******`搭配proxy使用（如下面的例子） 而无需担心OPENAI_API_KEY被泄露。
+这样的好处是在使用一些需要输入OPENAI_API_KEY的第三方应用时，我们可以使用`fk-******`搭配代理服务使用（如下面的例子）
+而无需担心OPENAI_API_KEY被泄露。  
+并且可以对外分发`fk-******`
 
 **用例:**
+
 ```bash
-curl https://api.openai-forward.top/v1/chat/completions \
+curl https://api.openai-forward.com/v1/chat/completions \
   -H "Content-Type: application/json" \
   -H "Authorization: Bearer fk-******" \
   -d '{
     "model": "gpt-3.5-turbo",
     "messages": [{"role": "user", "content": "Hello!"}]
   }'
 ```
+
 **Python**
+
 ```diff
   import openai
-+ openai.api_base = "https://api.openai-forward.top/v1"
++ openai.api_base = "https://api.openai-forward.com/v1"
 - openai.api_key = "sk-******"
 + openai.api_key = "fk-******"
 ```
+
 **Web application**
+
 ```bash 
 docker run -d \
     -p 3000:3000 \
     -e OPENAI_API_KEY="fk-******" \
-    -e BASE_URL="https://api.openai-forward.top" \
+    -e BASE_URL="https://api.openai-forward.com" \
     -e CODE="<your password>" \
     yidadaa/chatgpt-next-web 
 ``` 
 
+</details>
+
 ## 聊天日志
 
-保存路径在当前目录下的`Log/`路径中。  
-聊天日志以 `chat_`开头, 默认每5轮对话写入一次文件    
+默认不记录聊天日志，若要开启需设置环境变量`LOG_CHAT=true`
+<details markdown="1">
+  <summary>Click for more details</summary>
+
+保存路径在当前目录下的`Log/chat.log`路径中。  
 记录格式为
 
 ```text
-{'host': xxx, 'model': xxx, 'message': [{'user': xxx}, {'assistant': xxx}]}
-{'assistant': xxx}
+{'messages': [{'user': 'hi'}], 'model': 'gpt-3.5-turbo', 'host': '', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'}
+{'assistant': 'Hello! How can I assist you today?', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'}
+{'messages': [{'user': 'Hello!'}], 'model': 'gpt-3.5-turbo', 'host': '', 'uid': 'f844d156-e747-4887-aef8-e40d977b5ee7'}
+{'assistant': 'Hi there! How can I assist you today?', 'uid': 'f844d156-e747-4887-aef8-e40d977b5ee7'}
+...
+```
 
-{'host': ...}
-{'assistant': ...}
+转换为`jsonl`格式：
 
+```bash
+openai-forward convert
+```
+
+即可转换为以下格式：
+
+```json lines
+[
+    {
+        "messages": [
+            {
+                "user": "hi!"
+            }
+        ]
+    },
+    {
+        "assistant": "Hello! How can I assist you today?"
+    }
+]
+[
+    {
+        "messages": [
+            {
+                "user": "Hello!"
+            }
+        ]
+    },
+    {
+        "assistant": "Hi there! How can I assist you today?"
+    }
+]
 ...
 ```
 
+</details>
+
 ## Backer and Sponsor
 
 <a href="https://www.jetbrains.com/?from=beidongjiedeguang/openai-forward" target="_blank">
 <img src=".github/images/jetbrains.svg" width="100px" height="100px">
 </a>
 
 ## License
 
-Openai-forward is licensed under the [MIT](https://opensource.org/license/mit/) license.
+OpenAI-Forward is licensed under the [MIT](https://opensource.org/license/mit/) license.
```

#### html2text {}

```diff
@@ -2,83 +2,107 @@
                                     ******
                                 OpenAI Forward
                                      ******
                         OpenAI API æ¥å£è½¬åæå¡
                 The fastest way to deploy openai api forwarding
  [PyPI_version] [License] [Release_(latest_by_date)] [GitHub_repo_size] [docer
                 image_size] [tests] [pypi_downloads] [codecov]
+   [åè½](#åè½) | [é¨ç½²æå](#é¨ç½²æå) | [åºç¨](#åºç¨) |
+  [éç½®éé¡¹](#éç½®éé¡¹) | [èå¤©æ¥å¿](#èå¤©æ¥å¿) [![Deploy on
+    Railway](https://railway.app/button.svg)](https://railway.app/template/
+  tejCum?referralCode=U0-kXv) [![Deploy to Render](https://render.com/images/
+     deploy-to-render-button.svg)](https://render.com/deploy?repo=https://
+                 github.com/beidongjiedeguang/openai-forward)
 æ¬é¡¹ç®ç¨äºè§£å³ä¸äºå°åºæ æ³ç´æ¥è®¿é®OpenAIçé®é¢ï¼å°è¯¥æå¡é¨ç½²å¨å¯ä»¥æ­£å¸¸è®¿é®openai
 apiçæå¡å¨ä¸ï¼éè¿è¯¥æå¡è½¬åOpenAIçè¯·æ±ãå³æ­å»ºååä»£çæå¡
---- ç±æ¬é¡¹ç®æ­å»ºçé¿æä»£çå°åï¼ > https://api.openai-forward.top
-## ç®å½ - [åè½](#åè½) - [é¨ç½²æå](#é¨ç½²æå) - [åºç¨]
-(#åºç¨) - [éç½®éé¡¹](#éç½®éé¡¹) - [èå¤©æ¥å¿](#èå¤©æ¥å¿) -
-[é«çº§éç½®](#é«çº§éç½®) ## åè½ **åºç¡åè½** - [x]
-æ¯æè½¬åOpenAIæææ¥å£ - [x] æ¯ææµå¼ååº - [x]
-æ¯ææå®è½¬åè·¯ç±åç¼ - [x] dockeré¨ç½² - [x] pip å®è£é¨ç½² - [x]
-vercel ä¸é®ä¸ªäººåè´¹é¨ç½² [![Deploy with Vercel](https://vercel.com/
-button)](https://vercel.com/new/clone?repository-
-url=https%3A%2F%2Fgithub.com%2Fbeidongjiedeguang%2Fopenai-forward&project-
-name=openai-forward&repository-name=openai-forward&framework=other) - [x]
-cloudflare é¨ç½² **é«çº§åè½** - [x] å®æ¶è®°å½èå¤©è®°å½
+--- ç±æ¬é¡¹ç®æ­å»ºçé¿æä»£çå°åï¼ > https://api.openai-forward.com
+## åè½ **åºç¡åè½** - [x] æ¯æè½¬åOpenAIæææ¥å£ - [x]
+æ¯ææµå¼ååº - [x] æ¯ææå®è½¬åè·¯ç±åç¼ - [x] dockeré¨ç½² -
+[x] pip å®è£é¨ç½² - [x] cloudflare é¨ç½² - [x] ~~Vercelä¸é®é¨ç½²
+(ä¸å»ºè®®)~~ - [x] Railway ä¸é®é¨ç½² - [x] Render ä¸é®é¨ç½²
+**é«çº§åè½** - [x] å®æ¶è®°å½èå¤©è®°å½
 (åæ¬æµå¼ååºçèå¤©åå®¹) - [x] åè®¸è¾å¥å¤ä¸ªopenai api key
-ç»æè½®è¯¢æ±  - [x] èªå®ä¹ api key (è§é«çº§éç½®) - [x]
-æ¯æè¯·æ±IPéªè¯(IPç½ååä¸é»åå) ## é¨ç½²æå
-æä¾åç§é¨ç½²æ¹å¼ 1. [vps + pip å®è£é¨ç½²](deploy.md#pip-æ¨è)
-(æ¨è) 2. [vps + Docker](deploy.md#docker-æ¨è) (æ¨è) > https://
-api.openai-forward.top 3. [ä¸é®Vercelé¨ç½²](deploy.md#vercel-ä¸é®é¨ç½²)
-(ç®åä¸æ¨è) > ~~https://vercel.openai-forward.top~~ 4. [cloudflareé¨ç½²]
-(deploy.md#cloudflare-é¨ç½²) (æ¨è) > https://cloudflare.openai-forward.top
-## åºç¨ ### [èå¤©åºç¨](https://chat.beidongjiedeguang.top)
+ç»æè½®è¯¢æ±  - [x] èªå®ä¹ è½¬åapi key (è§[é«çº§éç½®]
+(#é«çº§éç½®)) ## é¨ç½²æå æä¾ä»¥ä¸å ç§é¨ç½²æ¹å¼
+**ææµ·å¤vpsæ¹æ¡** 1. [pip å®è£é¨ç½²](deploy.md#pip-æ¨è) (æ¨è) 2.
+[Dockeré¨ç½²](deploy.md#docker-æ¨è) (æ¨è) > https://api.openai-
+forward.com **æ vpsåè´¹é¨ç½²æ¹æ¡** 1. [ä¸é®Vercelé¨ç½²]
+(deploy.md#vercel-ä¸é®é¨ç½²) (ä¸æ¨è) > ~~https://vercel.openai-
+forward.com~~ 2. [cloudflareé¨ç½²](deploy.md#cloudflare-é¨ç½²) (æ¨è) >
+https://cloudflare.openai-forward.com 3. [Railwayé¨ç½²](deploy.md#Railway-
+ä¸é®é¨ç½²) > https://railway.openai-forward.com 4. [Renderä¸é®é¨ç½²]
+(deploy.md#render-ä¸é®é¨ç½²) (æ¨è) > https://render.openai-forward.com ##
+åºç¨ ### [èå¤©åºç¨](https://chat.beidongjiedeguang.top)
 åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-
 Web)æ­å»ºèªå·±çchatgptæå¡ æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
-`BASE_URL`ä¸ºæä»¬èªå·±æ­å»ºçä»£çæå¡å°å ```bash docker run -d \ -
-p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -e BASE_URL="https://api.openai-
-forward.top" \ -e CODE="kunyuan" \ yidadaa/chatgpt-next-web ```
-è¿éé¨ç½²äºä¸ä¸ªï¼ä¾å¤§å®¶è½»åº¦ä½¿ç¨: https://
-chat.beidongjiedeguang.top , è®¿é®å¯ç : `kunyuan` ### å¨ä»£ç ä¸­ä½¿ç¨
-**JS/TS** ```diff import { Configuration } from "openai"; const configuration =
-new Configuration({ + basePath: "https://api.openai-forward.top/v1", apiKey:
-"sk-******", }); ``` **Python** ```diff import openai + openai.api_base =
-"https://api.openai-forward.top/v1" openai.api_key = "sk-******" ``` **gpt-3.5-
-turbo** ```bash curl https://api.openai-forward.top/v1/chat/completions \ -
-H "Content-Type: application/json" \ -H "Authorization: Bearer sk-******" \ -
-d '{ "model": "gpt-3.5-turbo", "messages": [{"role": "user", "content":
-"Hello!"}] }' ``` **Image Generation (DALL-E)** ```bash curl --location 'https:
-//api.openai-forward.top/v1/images/generations' \ --header 'Authorization:
-Bearer sk-******' \ --header 'Content-Type: application/json' \ --data '
-{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ``` ##
-éç½®éé¡¹ **`openai-forward run`åæ°éç½®é¡¹** | éç½®é¡¹ | è¯´æ |
-é»è®¤å¼ | |-----------| --- | :---: | | --port | æå¡ç«¯å£å· | 8000 | | -
--workers | å·¥ä½è¿ç¨æ° | 1 | æ´å¤åæ° `openai-forward run --help`
-æ¥ç **ç¯å¢åééç½®é¡¹**
-æ¯æä»è¿è¡ç®å½ä¸ç`.env`æä»¶ä¸­è¯»å: | ç¯å¢åé | è¯´æ |
+`BASE_URL`ä¸ºæä»¬èªå·±æ­å»ºçä»£çæå¡å°å  Click for more details
+```bash docker run -d \ -p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -
+e BASE_URL="https://api.openai-forward.com" \ -e CODE="kunyuan" \ yidadaa/
+chatgpt-next-web ``` è¿éé¨ç½²äºä¸ä¸ªï¼ä¾å¤§å®¶è½»åº¦ä½¿ç¨: https://
+chat.beidongjiedeguang.top , è®¿é®å¯ç : `kunyuan`  ### å¨ä»£ç ä¸­ä½¿ç¨
+**Python** ```diff import openai + openai.api_base = "https://api.openai-
+forward.com/v1" openai.api_key = "sk-******" ```  More Examples **JS/TS**
+```diff import { Configuration } from "openai"; const configuration = new
+Configuration({ + basePath: "https://api.openai-forward.com/v1", apiKey: "sk-
+******", }); ``` **gpt-3.5-turbo** ```bash curl https://api.openai-forward.com/
+v1/chat/completions \ -H "Content-Type: application/json" \ -H "Authorization:
+Bearer sk-******" \ -d '{ "model": "gpt-3.5-turbo", "messages": [{"role":
+"user", "content": "Hello!"}] }' ``` **Image Generation (DALL-E)** ```bash curl
+--location 'https://api.openai-forward.com/v1/images/generations' \ --header
+'Authorization: Bearer sk-******' \ --header 'Content-Type: application/json' \
+--data '{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ```  ##
+éç½®éé¡¹ éç½®çè®¾ç½®æ¹å¼æ¯æä¸¤ç§
+ä¸ç§ä¸ºå¨shellä¸­è¿è¡`openai-forward run --
+port=8000`çå½ä»¤è¡æ¹å¼æå®;
+å¦ä¸ç§ä¸ºè¯»åç¯å¢åéçæ¹å¼æå®ã  Click for more details
+**`openai-forward run`åæ°éç½®é¡¹** | éç½®é¡¹ | è¯´æ | é»è®¤å¼ | |---
+--------------|-------------------|:----------------------:| | --port |
+æå¡ç«¯å£å· | 8000 | | --workers | å·¥ä½è¿ç¨æ° | 1 | | --base_url | å
+OPENAI_BASE_URL | https://api.openai.com | | --api_key | å OPENAI_API_KEY |
+`None` | | --forward_key | å FORWARD_KEY | `None` | | --route_prefix | å
+ROUTE_PREFIX | `None` | | --log_chat | å LOG_CHAT | `False` | ä¹å¯éè¿
+`openai-forward run --help` æ¥ç **ç¯å¢åééç½®é¡¹**
+æ¯æä»è¿è¡ç®å½ä¸ç`.env`æä»¶ä¸­è¯»å | ç¯å¢åé | è¯´æ |
 é»è®¤å¼ | |-----------------|------------------------------------------------
------------------|:------------------------:| | OPENAI_API_KEY | é»è®¤openai
-api keyï¼æ¯æå¤ä¸ªé»è®¤api key, ä»¥ `sk-` å¼å¤´ï¼ ä»¥ç©ºæ ¼åå² | æ 
-| | FORWARD_KEY | åè®¸è°ç¨æ¹ä½¿ç¨è¯¥keyä»£æ¿openai api
-keyï¼æ¯æå¤ä¸ªforward key, ä»¥`fk-` å¼å¤´, ä»¥ç©ºæ ¼åå² | æ  | |
-OPENAI_BASE_URL | è½¬åbase url | `https://api.openai.com` | | LOG_CHAT |
-æ¯å¦è®°å½èå¤©åå®¹ | `true` | | ROUTE_PREFIX | è·¯ç±åç¼ | æ  | |
-IP_WHITELIST | ipç½åå, ç©ºæ ¼åå¼ | æ  | | IP_BLACKLIST | ipé»åå,
-ç©ºæ ¼åå¼ | æ  | ## é«çº§éç½® **è®¾ç½®api_keyä¸ºèªå·±è®¾ç½®çforward
-key** éè¦éç½® OPENAI_API_KEY å FORWARD_KEY, ä¾å¦ ```bash
-OPENAI_API_KEY=sk-******* FORWARD_KEY=fk-****** # è¿éfk-
-tokenç±æä»¬èªå·±å®ä¹ ``` è¿éæä»¬éç½®äºFORWARD_KEYä¸º`fk-******`,
+-------------------------------------------------------------------------------
+----|:------------------------:| | OPENAI_BASE_URL | é»è®¤ openaiå®æ¹ api
+å°å | https://api.openai.com | | OPENAI_API_KEY | é»è®¤openai api
+keyï¼æ¯æå¤ä¸ªé»è®¤api key, ä»¥ `sk-` å¼å¤´ï¼ ä»¥ç©ºæ ¼åå² | æ  | |
+FORWARD_KEY | åè®¸è°ç¨æ¹ä½¿ç¨è¯¥keyä»£æ¿openai api
+keyï¼æ¯æå¤ä¸ªforward key, ä»¥ç©ºæ ¼åå²;
+å¦æè®¾ç½®äºOPENAI_API_KEYï¼èæ²¡æè®¾ç½®FORWARD_KEY,
+åå®¢æ·ç«¯è°ç¨æ¶æ éæä¾å¯é¥,
+æ­¤æ¶åºäºå®å¨èèä¸å»ºè®®FORWARD_KEYç½®ç©º | æ  | | OPENAI_BASE_URL |
+è½¬åbase url | `https://api.openai.com` | | ROUTE_PREFIX | è·¯ç±åç¼ | æ 
+| | LOG_CHAT | æ¯å¦è®°å½èå¤©åå®¹ | `false` |  ## é«çº§éç½®
+**è®¾ç½®api_keyä¸ºèªå·±è®¾ç½®çforward key** éè¦éç½® OPENAI_API_KEY å
+FORWARD_KEY, ä¾å¦  Click for more details ```bash OPENAI_API_KEY=sk-*******
+FORWARD_KEY=fk-****** # è¿éfk-tokenç±æä»¬èªå·±å®ä¹ ```
+è¿éæä»¬éç½®äºFORWARD_KEYä¸º`fk-******`,
 é£ä¹åé¢å®¢æ·ç«¯å¨è°ç¨æ¶åªéè®¾ç½®OPENAI_API_KEYä¸ºæä»¬èªå®ä¹ç`fk-
 ******` å³å¯ã
 è¿æ ·çå¥½å¤æ¯å¨ä½¿ç¨ä¸äºéè¦è¾å¥OPENAI_API_KEYçç¬¬ä¸æ¹åºç¨æ¶ï¼æä»¬å¯ä»¥ä½¿ç¨`fk-
-******`æ­éproxyä½¿ç¨ï¼å¦ä¸é¢çä¾å­ï¼
-èæ éæå¿OPENAI_API_KEYè¢«æ³é²ã **ç¨ä¾:** ```bash curl https://
-api.openai-forward.top/v1/chat/completions \ -H "Content-Type: application/
-json" \ -H "Authorization: Bearer fk-******" \ -d '{ "model": "gpt-3.5-turbo",
-"messages": [{"role": "user", "content": "Hello!"}] }' ``` **Python** ```diff
-import openai + openai.api_base = "https://api.openai-forward.top/v1" -
-openai.api_key = "sk-******" + openai.api_key = "fk-******" ``` **Web
-application** ```bash docker run -d \ -p 3000:3000 \ -e OPENAI_API_KEY="fk-
-******" \ -e BASE_URL="https://api.openai-forward.top" \ -e CODE="" \ yidadaa/
-chatgpt-next-web ``` ## èå¤©æ¥å¿ ä¿å­è·¯å¾å¨å½åç®å½ä¸ç`Log/
-`è·¯å¾ä¸­ã èå¤©æ¥å¿ä»¥ `chat_`å¼å¤´,
-é»è®¤æ¯5è½®å¯¹è¯åå¥ä¸æ¬¡æä»¶ è®°å½æ ¼å¼ä¸º ```text {'host': xxx,
-'model': xxx, 'message': [{'user': xxx}, {'assistant': xxx}]} {'assistant':
-xxx} {'host': ...} {'assistant': ...} ... ``` ## Backer and Sponsor [.github/
-images/jetbrains.svg] ## License Openai-forward is licensed under the [MIT]
-(https://opensource.org/license/mit/) license.
+******`æ­éä»£çæå¡ä½¿ç¨ï¼å¦ä¸é¢çä¾å­ï¼
+èæ éæå¿OPENAI_API_KEYè¢«æ³é²ã å¹¶ä¸å¯ä»¥å¯¹å¤åå`fk-******`
+**ç¨ä¾:** ```bash curl https://api.openai-forward.com/v1/chat/completions \ -
+H "Content-Type: application/json" \ -H "Authorization: Bearer fk-******" \ -
+d '{ "model": "gpt-3.5-turbo", "messages": [{"role": "user", "content":
+"Hello!"}] }' ``` **Python** ```diff import openai + openai.api_base = "https:/
+/api.openai-forward.com/v1" - openai.api_key = "sk-******" + openai.api_key =
+"fk-******" ``` **Web application** ```bash docker run -d \ -p 3000:3000 \ -
+e OPENAI_API_KEY="fk-******" \ -e BASE_URL="https://api.openai-forward.com" \ -
+e CODE="" \ yidadaa/chatgpt-next-web ```  ## èå¤©æ¥å¿
+é»è®¤ä¸è®°å½èå¤©æ¥å¿ï¼è¥è¦å¼å¯éè®¾ç½®ç¯å¢åé`LOG_CHAT=true`
+Click for more details ä¿å­è·¯å¾å¨å½åç®å½ä¸ç`Log/
+chat.log`è·¯å¾ä¸­ã è®°å½æ ¼å¼ä¸º ```text {'messages': [{'user': 'hi'}],
+'model': 'gpt-3.5-turbo', 'host': '', 'uid': '467a17ec-bf39-4b65-9ebd-
+e722b3bdd5c3'} {'assistant': 'Hello! How can I assist you today?', 'uid':
+'467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'} {'messages': [{'user': 'Hello!'}],
+'model': 'gpt-3.5-turbo', 'host': '', 'uid': 'f844d156-e747-4887-aef8-
+e40d977b5ee7'} {'assistant': 'Hi there! How can I assist you today?', 'uid':
+'f844d156-e747-4887-aef8-e40d977b5ee7'} ... ``` è½¬æ¢ä¸º`jsonl`æ ¼å¼ï¼
+```bash openai-forward convert ``` å³å¯è½¬æ¢ä¸ºä»¥ä¸æ ¼å¼ï¼ ```json lines
+[ { "messages": [ { "user": "hi!" } ] }, { "assistant": "Hello! How can I
+assist you today?" } ] [ { "messages": [ { "user": "Hello!" } ] },
+{ "assistant": "Hi there! How can I assist you today?" } ] ... ```  ## Backer
+and Sponsor [.github/images/jetbrains.svg] ## License OpenAI-Forward is
+licensed under the [MIT](https://opensource.org/license/mit/) license.
```

### Comparing `openai_forward-0.2.1/pyproject.toml` & `openai_forward-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,17 @@
 ]
 bard = [
     "GoogleBard",
 ]
 edge = [
     "EdgeGPT",
 ]
+tool = [
+    "orjsonl"
+]
 
 [project.scripts]
 openai_forward = "openai_forward.__main__:main"
 openai-forward = "openai_forward.__main__:main"
 aifwd = "openai_forward.__main__:main"
 
 [tool.hatch.version]
```

### Comparing `openai_forward-0.2.1/PKG-INFO` & `openai_forward-0.2.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_forward
-Version: 0.2.1
+Version: 0.2.2
 Summary: 🚀 Openai api forward · OpenAI 接口转发服务 · stream forwarding
 Project-URL: Homepage, https://github.com/beidongjiedeguang/openai-forward
 Project-URL: Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-forward
 Project-URL: Issues, https://github.com/beidongjiedeguang/openai-forward/issues
 Project-URL: Source, https://github.com/beidongjiedeguang/openai-forward
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
 License-Expression: MIT
@@ -26,14 +26,16 @@
 Requires-Dist: googlebard; extra == 'bard'
 Provides-Extra: chatgpt
 Requires-Dist: revchatgpt; extra == 'chatgpt'
 Provides-Extra: edge
 Requires-Dist: edgegpt; extra == 'edge'
 Provides-Extra: ssl
 Requires-Dist: certbot; extra == 'ssl'
+Provides-Extra: tool
+Requires-Dist: orjsonl; extra == 'tool'
 Description-Content-Type: text/markdown
 
 **中文** | [**English**](./README_EN.md)
 
 <h1 align="center">
     <br>
     OpenAI Forward
@@ -65,208 +67,295 @@
         <img alt="pypi downloads" src="https://img.shields.io/pypi/dm/openai_forward">
     </a>
     <a href="https://codecov.io/gh/beidongjiedeguang/openai-forward">
         <img alt="codecov" src="https://codecov.io/gh/beidongjiedeguang/openai-forward/branch/dev/graph/badge.svg">
     </a>
 </p>
 
+<div align="center">
 
+[功能](#功能) |
+[部署指南](#部署指南) |
+[应用](#应用) |
+[配置选项](#配置选项) |
+[聊天日志](#聊天日志)
+
+[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/tejCum?referralCode=U0-kXv)  
+[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/beidongjiedeguang/openai-forward)
+
+</div>
 
 本项目用于解决一些地区无法直接访问OpenAI的问题，将该服务部署在可以正常访问openai
-api的服务器上，通过该服务转发OpenAI的请求。即搭建反向代理服务  
+api的服务器上，通过该服务转发OpenAI的请求。即搭建反向代理服务
 
 ---
 
 由本项目搭建的长期代理地址：
-> https://api.openai-forward.top  
-
+> https://api.openai-forward.com
 
+## 功能
 
-## 目录
-
-- [功能](#功能)
-- [部署指南](#部署指南)
-- [应用](#应用)
-- [配置选项](#配置选项)
-- [聊天日志](#聊天日志)
-- [高级配置](#高级配置)
+**基础功能**
 
-## 功能
-**基础功能**  
 - [x] 支持转发OpenAI所有接口
 - [x] 支持流式响应
 - [x] 支持指定转发路由前缀
 - [x] docker部署
 - [x] pip 安装部署
-- [x] vercel 一键个人免费部署
-  [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fbeidongjiedeguang%2Fopenai-forward&project-name=openai-forward&repository-name=openai-forward&framework=other)
 - [x] cloudflare 部署
+- [x] ~~Vercel一键部署(不建议)~~
+- [x] Railway 一键部署
+- [x] Render 一键部署
+
+**高级功能**
 
-**高级功能**  
 - [x] 实时记录聊天记录(包括流式响应的聊天内容)
 - [x] 允许输入多个openai api key 组成轮询池
-- [x] 自定义 api key (见高级配置)
-- [x] 支持请求IP验证(IP白名单与黑名单)
+- [x] 自定义 转发api key (见[高级配置](#高级配置))
 
 ## 部署指南
 
-提供四种部署方式
-1. [vps + pip 安装部署](deploy.md#pip-推荐) (推荐)
-2. [vps + Docker](deploy.md#docker-推荐) (推荐) 
-    > https://api.openai-forward.top 
-3. [一键Vercel部署](deploy.md#vercel-一键部署) (目前不推荐)
-   > ~~https://vercel.openai-forward.top~~  
-4. [cloudflare部署](deploy.md#cloudflare-部署) (推荐)
-   > https://cloudflare.openai-forward.top
+提供以下几种部署方式
+
+**有海外vps方案**
+
+1. [pip 安装部署](deploy.md#pip-推荐) (推荐)
+2. [Docker部署](deploy.md#docker-推荐) (推荐)
+   > https://api.openai-forward.com
+
+**无vps免费部署方案**
+
+1. [一键Vercel部署](deploy.md#vercel-一键部署) (不推荐)
+   > ~~https://vercel.openai-forward.com~~
+2. [cloudflare部署](deploy.md#cloudflare-部署) (推荐)
+   > https://cloudflare.openai-forward.com
+3. [Railway部署](deploy.md#Railway-一键部署)
+   > https://railway.openai-forward.com
+4. [Render一键部署](deploy.md#render-一键部署) (推荐)
+   > https://render.openai-forward.com
 
 ## 应用
 
 ### [聊天应用](https://chat.beidongjiedeguang.top)
 
 基于开源项目[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)搭建自己的chatgpt服务  
 替换docker启动命令中的 `BASE_URL`为我们自己搭建的代理服务地址
 
+<details markdown="1">
+<summary>Click for more details</summary>  
+
 ```bash 
 docker run -d \
     -p 3000:3000 \
     -e OPENAI_API_KEY="sk-******" \
-    -e BASE_URL="https://api.openai-forward.top" \
+    -e BASE_URL="https://api.openai-forward.com" \
     -e CODE="kunyuan" \
     yidadaa/chatgpt-next-web 
 ``` 
+
 这里部署了一个，供大家轻度使用:  
- https://chat.beidongjiedeguang.top , 访问密码: `kunyuan` 
+https://chat.beidongjiedeguang.top , 访问密码: `kunyuan`
+</details>
 
 ### 在代码中使用
 
+**Python**
+
+```diff
+  import openai
++ openai.api_base = "https://api.openai-forward.com/v1"
+  openai.api_key = "sk-******"
+```
+
+<details markdown="1">
+  <summary>More Examples</summary>
+
 **JS/TS**
 
 ```diff
   import { Configuration } from "openai";
   
   const configuration = new Configuration({
-+ basePath: "https://api.openai-forward.top/v1",
++ basePath: "https://api.openai-forward.com/v1",
   apiKey: "sk-******",
   });
 ```
 
-**Python**
-
-```diff
-  import openai
-+ openai.api_base = "https://api.openai-forward.top/v1"
-  openai.api_key = "sk-******"
-```
-
 **gpt-3.5-turbo**
+
 ```bash
-curl https://api.openai-forward.top/v1/chat/completions \
+curl https://api.openai-forward.com/v1/chat/completions \
   -H "Content-Type: application/json" \
   -H "Authorization: Bearer sk-******" \
   -d '{
     "model": "gpt-3.5-turbo",
     "messages": [{"role": "user", "content": "Hello!"}]
   }'
 ```
 
 **Image Generation (DALL-E)**
+
 ```bash
-curl --location 'https://api.openai-forward.top/v1/images/generations' \
+curl --location 'https://api.openai-forward.com/v1/images/generations' \
 --header 'Authorization: Bearer sk-******' \
 --header 'Content-Type: application/json' \
 --data '{
     "prompt": "A photo of a cat",
     "n": 1,
     "size": "512x512"
 }'
 ```
 
+</details>
 
 ## 配置选项
 
+配置的设置方式支持两种  
+一种为在shell中运行`openai-forward run --port=8000`的命令行方式指定;  
+另一种为读取环境变量的方式指定。
+
+<details markdown="1">
+<summary>Click for more details</summary>  
+
 **`openai-forward run`参数配置项**
 
-| 配置项       | 说明 | 默认值 |
-|-----------| --- | :---: |
-| --port    | 服务端口号 | 8000 |
-| --workers | 工作进程数 | 1 |
+| 配置项 | 说明                |          默认值           |
+|-----------------|-------------------|:----------------------:|
+| --port | 服务端口号             |          8000          |
+| --workers | 工作进程数             |           1            |
+| --base_url | 同 OPENAI_BASE_URL | https://api.openai.com |
+| --api_key | 同 OPENAI_API_KEY  |         `None`         |
+| --forward_key | 同 FORWARD_KEY     |         `None`         |
+| --route_prefix | 同 ROUTE_PREFIX    |          `None`          |
+| --log_chat | 同 LOG_CHAT        |        `False`         |
 
-更多参数 `openai-forward run --help` 查看
+也可通过 `openai-forward run --help` 查看
 
 **环境变量配置项**  
-支持从运行目录下的`.env`文件中读取: 
+支持从运行目录下的`.env`文件中读取
 
-| 环境变量            | 说明                                                              |           默认值            |
-|-----------------|-----------------------------------------------------------------|:------------------------:|
-| OPENAI_API_KEY  | 默认openai api key，支持多个默认api key, 以 `sk-` 开头， 以空格分割      |            无             |
-| FORWARD_KEY     | 允许调用方使用该key代替openai api key，支持多个forward key, 以`fk-` 开头, 以空格分割 |      无             |
-| OPENAI_BASE_URL | 转发base url                                                      | `https://api.openai.com` |
-| LOG_CHAT        | 是否记录聊天内容                                                        |          `true`          |
-| ROUTE_PREFIX    | 路由前缀                                                            |            无             |
-| IP_WHITELIST    | ip白名单, 空格分开                                                     |           无            |
-| IP_BLACKLIST    | ip黑名单, 空格分开                                                     |           无            | 
+| 环境变量            | 说明                                                                                                                                |           默认值            |
+|-----------------|-----------------------------------------------------------------------------------------------------------------------------------|:------------------------:|
+| OPENAI_BASE_URL  | 默认 openai官方 api 地址                                                                                                                |        https://api.openai.com           |
+| OPENAI_API_KEY  | 默认openai api key，支持多个默认api key, 以 `sk-` 开头， 以空格分割                                                                                 |            无             |
+| FORWARD_KEY     | 允许调用方使用该key代替openai api key，支持多个forward key, 以空格分割; 如果设置了OPENAI_API_KEY，而没有设置FORWARD_KEY, 则客户端调用时无需提供密钥, 此时出于安全考虑不建议FORWARD_KEY置空 |            无             |
+| OPENAI_BASE_URL | 转发base url                                                                                                                        | `https://api.openai.com` |
+| ROUTE_PREFIX    | 路由前缀                                                                                                                              |            无             |
+| LOG_CHAT        | 是否记录聊天内容                                                                                                                          |         `false`          |
 
+</details>
 
 ## 高级配置
 
 **设置api_key为自己设置的forward key**  
 需要配置 OPENAI_API_KEY 和 FORWARD_KEY, 例如
+<details markdown="1">
+  <summary>Click for more details</summary>
 
 ```bash
 OPENAI_API_KEY=sk-*******
 FORWARD_KEY=fk-****** # 这里fk-token由我们自己定义
 ```
+
 这里我们配置了FORWARD_KEY为`fk-******`, 那么后面客户端在调用时只需设置OPENAI_API_KEY为我们自定义的`fk-******` 即可。  
-这样的好处是在使用一些需要输入OPENAI_API_KEY的第三方应用时，我们可以使用`fk-******`搭配proxy使用（如下面的例子） 而无需担心OPENAI_API_KEY被泄露。
+这样的好处是在使用一些需要输入OPENAI_API_KEY的第三方应用时，我们可以使用`fk-******`搭配代理服务使用（如下面的例子）
+而无需担心OPENAI_API_KEY被泄露。  
+并且可以对外分发`fk-******`
 
 **用例:**
+
 ```bash
-curl https://api.openai-forward.top/v1/chat/completions \
+curl https://api.openai-forward.com/v1/chat/completions \
   -H "Content-Type: application/json" \
   -H "Authorization: Bearer fk-******" \
   -d '{
     "model": "gpt-3.5-turbo",
     "messages": [{"role": "user", "content": "Hello!"}]
   }'
 ```
+
 **Python**
+
 ```diff
   import openai
-+ openai.api_base = "https://api.openai-forward.top/v1"
++ openai.api_base = "https://api.openai-forward.com/v1"
 - openai.api_key = "sk-******"
 + openai.api_key = "fk-******"
 ```
+
 **Web application**
+
 ```bash 
 docker run -d \
     -p 3000:3000 \
     -e OPENAI_API_KEY="fk-******" \
-    -e BASE_URL="https://api.openai-forward.top" \
+    -e BASE_URL="https://api.openai-forward.com" \
     -e CODE="<your password>" \
     yidadaa/chatgpt-next-web 
 ``` 
 
+</details>
+
 ## 聊天日志
 
-保存路径在当前目录下的`Log/`路径中。  
-聊天日志以 `chat_`开头, 默认每5轮对话写入一次文件    
+默认不记录聊天日志，若要开启需设置环境变量`LOG_CHAT=true`
+<details markdown="1">
+  <summary>Click for more details</summary>
+
+保存路径在当前目录下的`Log/chat.log`路径中。  
 记录格式为
 
 ```text
-{'host': xxx, 'model': xxx, 'message': [{'user': xxx}, {'assistant': xxx}]}
-{'assistant': xxx}
+{'messages': [{'user': 'hi'}], 'model': 'gpt-3.5-turbo', 'host': '', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'}
+{'assistant': 'Hello! How can I assist you today?', 'uid': '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'}
+{'messages': [{'user': 'Hello!'}], 'model': 'gpt-3.5-turbo', 'host': '', 'uid': 'f844d156-e747-4887-aef8-e40d977b5ee7'}
+{'assistant': 'Hi there! How can I assist you today?', 'uid': 'f844d156-e747-4887-aef8-e40d977b5ee7'}
+...
+```
 
-{'host': ...}
-{'assistant': ...}
+转换为`jsonl`格式：
 
+```bash
+openai-forward convert
+```
+
+即可转换为以下格式：
+
+```json lines
+[
+    {
+        "messages": [
+            {
+                "user": "hi!"
+            }
+        ]
+    },
+    {
+        "assistant": "Hello! How can I assist you today?"
+    }
+]
+[
+    {
+        "messages": [
+            {
+                "user": "Hello!"
+            }
+        ]
+    },
+    {
+        "assistant": "Hi there! How can I assist you today?"
+    }
+]
 ...
 ```
 
+</details>
+
 ## Backer and Sponsor
 
 <a href="https://www.jetbrains.com/?from=beidongjiedeguang/openai-forward" target="_blank">
 <img src=".github/images/jetbrains.svg" width="100px" height="100px">
 </a>
 
 ## License
 
-Openai-forward is licensed under the [MIT](https://opensource.org/license/mit/) license.
+OpenAI-Forward is licensed under the [MIT](https://opensource.org/license/mit/) license.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openai_forward Version: 0.2.1 Summary: ð Openai
+Metadata-Version: 2.1 Name: openai_forward Version: 0.2.2 Summary: ð Openai
 api forward Â· OpenAI æ¥å£è½¬åæå¡ Â· stream forwarding Project-URL:
 Homepage, https://github.com/beidongjiedeguang/openai-forward Project-URL:
 Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-
 forward Project-URL: Issues, https://github.com/beidongjiedeguang/openai-
 forward/issues Project-URL: Source, https://github.com/beidongjiedeguang/
 openai-forward Author-email: kunyuan
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords: OpenAI API
@@ -11,92 +11,117 @@
 Stable Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.6 Requires-Dist: fastapi Requires-
 Dist: httpx Requires-Dist: loguru Requires-Dist: orjson Requires-Dist: python-
 dotenv Requires-Dist: pytz Requires-Dist: sparrow-python>=0.1.3 Requires-Dist:
 uvicorn Provides-Extra: bard Requires-Dist: googlebard; extra == 'bard'
 Provides-Extra: chatgpt Requires-Dist: revchatgpt; extra == 'chatgpt' Provides-
 Extra: edge Requires-Dist: edgegpt; extra == 'edge' Provides-Extra: ssl
-Requires-Dist: certbot; extra == 'ssl' Description-Content-Type: text/markdown
-**ä¸­æ** | [**English**](./README_EN.md)
+Requires-Dist: certbot; extra == 'ssl' Provides-Extra: tool Requires-Dist:
+orjsonl; extra == 'tool' Description-Content-Type: text/markdown **ä¸­æ** |
+[**English**](./README_EN.md)
                                     ******
                                 OpenAI Forward
                                      ******
                         OpenAI API æ¥å£è½¬åæå¡
                 The fastest way to deploy openai api forwarding
  [PyPI_version] [License] [Release_(latest_by_date)] [GitHub_repo_size] [docer
                 image_size] [tests] [pypi_downloads] [codecov]
+   [åè½](#åè½) | [é¨ç½²æå](#é¨ç½²æå) | [åºç¨](#åºç¨) |
+  [éç½®éé¡¹](#éç½®éé¡¹) | [èå¤©æ¥å¿](#èå¤©æ¥å¿) [![Deploy on
+    Railway](https://railway.app/button.svg)](https://railway.app/template/
+  tejCum?referralCode=U0-kXv) [![Deploy to Render](https://render.com/images/
+     deploy-to-render-button.svg)](https://render.com/deploy?repo=https://
+                 github.com/beidongjiedeguang/openai-forward)
 æ¬é¡¹ç®ç¨äºè§£å³ä¸äºå°åºæ æ³ç´æ¥è®¿é®OpenAIçé®é¢ï¼å°è¯¥æå¡é¨ç½²å¨å¯ä»¥æ­£å¸¸è®¿é®openai
 apiçæå¡å¨ä¸ï¼éè¿è¯¥æå¡è½¬åOpenAIçè¯·æ±ãå³æ­å»ºååä»£çæå¡
---- ç±æ¬é¡¹ç®æ­å»ºçé¿æä»£çå°åï¼ > https://api.openai-forward.top
-## ç®å½ - [åè½](#åè½) - [é¨ç½²æå](#é¨ç½²æå) - [åºç¨]
-(#åºç¨) - [éç½®éé¡¹](#éç½®éé¡¹) - [èå¤©æ¥å¿](#èå¤©æ¥å¿) -
-[é«çº§éç½®](#é«çº§éç½®) ## åè½ **åºç¡åè½** - [x]
-æ¯æè½¬åOpenAIæææ¥å£ - [x] æ¯ææµå¼ååº - [x]
-æ¯ææå®è½¬åè·¯ç±åç¼ - [x] dockeré¨ç½² - [x] pip å®è£é¨ç½² - [x]
-vercel ä¸é®ä¸ªäººåè´¹é¨ç½² [![Deploy with Vercel](https://vercel.com/
-button)](https://vercel.com/new/clone?repository-
-url=https%3A%2F%2Fgithub.com%2Fbeidongjiedeguang%2Fopenai-forward&project-
-name=openai-forward&repository-name=openai-forward&framework=other) - [x]
-cloudflare é¨ç½² **é«çº§åè½** - [x] å®æ¶è®°å½èå¤©è®°å½
+--- ç±æ¬é¡¹ç®æ­å»ºçé¿æä»£çå°åï¼ > https://api.openai-forward.com
+## åè½ **åºç¡åè½** - [x] æ¯æè½¬åOpenAIæææ¥å£ - [x]
+æ¯ææµå¼ååº - [x] æ¯ææå®è½¬åè·¯ç±åç¼ - [x] dockeré¨ç½² -
+[x] pip å®è£é¨ç½² - [x] cloudflare é¨ç½² - [x] ~~Vercelä¸é®é¨ç½²
+(ä¸å»ºè®®)~~ - [x] Railway ä¸é®é¨ç½² - [x] Render ä¸é®é¨ç½²
+**é«çº§åè½** - [x] å®æ¶è®°å½èå¤©è®°å½
 (åæ¬æµå¼ååºçèå¤©åå®¹) - [x] åè®¸è¾å¥å¤ä¸ªopenai api key
-ç»æè½®è¯¢æ±  - [x] èªå®ä¹ api key (è§é«çº§éç½®) - [x]
-æ¯æè¯·æ±IPéªè¯(IPç½ååä¸é»åå) ## é¨ç½²æå
-æä¾åç§é¨ç½²æ¹å¼ 1. [vps + pip å®è£é¨ç½²](deploy.md#pip-æ¨è)
-(æ¨è) 2. [vps + Docker](deploy.md#docker-æ¨è) (æ¨è) > https://
-api.openai-forward.top 3. [ä¸é®Vercelé¨ç½²](deploy.md#vercel-ä¸é®é¨ç½²)
-(ç®åä¸æ¨è) > ~~https://vercel.openai-forward.top~~ 4. [cloudflareé¨ç½²]
-(deploy.md#cloudflare-é¨ç½²) (æ¨è) > https://cloudflare.openai-forward.top
-## åºç¨ ### [èå¤©åºç¨](https://chat.beidongjiedeguang.top)
+ç»æè½®è¯¢æ±  - [x] èªå®ä¹ è½¬åapi key (è§[é«çº§éç½®]
+(#é«çº§éç½®)) ## é¨ç½²æå æä¾ä»¥ä¸å ç§é¨ç½²æ¹å¼
+**ææµ·å¤vpsæ¹æ¡** 1. [pip å®è£é¨ç½²](deploy.md#pip-æ¨è) (æ¨è) 2.
+[Dockeré¨ç½²](deploy.md#docker-æ¨è) (æ¨è) > https://api.openai-
+forward.com **æ vpsåè´¹é¨ç½²æ¹æ¡** 1. [ä¸é®Vercelé¨ç½²]
+(deploy.md#vercel-ä¸é®é¨ç½²) (ä¸æ¨è) > ~~https://vercel.openai-
+forward.com~~ 2. [cloudflareé¨ç½²](deploy.md#cloudflare-é¨ç½²) (æ¨è) >
+https://cloudflare.openai-forward.com 3. [Railwayé¨ç½²](deploy.md#Railway-
+ä¸é®é¨ç½²) > https://railway.openai-forward.com 4. [Renderä¸é®é¨ç½²]
+(deploy.md#render-ä¸é®é¨ç½²) (æ¨è) > https://render.openai-forward.com ##
+åºç¨ ### [èå¤©åºç¨](https://chat.beidongjiedeguang.top)
 åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-
 Web)æ­å»ºèªå·±çchatgptæå¡ æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
-`BASE_URL`ä¸ºæä»¬èªå·±æ­å»ºçä»£çæå¡å°å ```bash docker run -d \ -
-p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -e BASE_URL="https://api.openai-
-forward.top" \ -e CODE="kunyuan" \ yidadaa/chatgpt-next-web ```
-è¿éé¨ç½²äºä¸ä¸ªï¼ä¾å¤§å®¶è½»åº¦ä½¿ç¨: https://
-chat.beidongjiedeguang.top , è®¿é®å¯ç : `kunyuan` ### å¨ä»£ç ä¸­ä½¿ç¨
-**JS/TS** ```diff import { Configuration } from "openai"; const configuration =
-new Configuration({ + basePath: "https://api.openai-forward.top/v1", apiKey:
-"sk-******", }); ``` **Python** ```diff import openai + openai.api_base =
-"https://api.openai-forward.top/v1" openai.api_key = "sk-******" ``` **gpt-3.5-
-turbo** ```bash curl https://api.openai-forward.top/v1/chat/completions \ -
-H "Content-Type: application/json" \ -H "Authorization: Bearer sk-******" \ -
-d '{ "model": "gpt-3.5-turbo", "messages": [{"role": "user", "content":
-"Hello!"}] }' ``` **Image Generation (DALL-E)** ```bash curl --location 'https:
-//api.openai-forward.top/v1/images/generations' \ --header 'Authorization:
-Bearer sk-******' \ --header 'Content-Type: application/json' \ --data '
-{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ``` ##
-éç½®éé¡¹ **`openai-forward run`åæ°éç½®é¡¹** | éç½®é¡¹ | è¯´æ |
-é»è®¤å¼ | |-----------| --- | :---: | | --port | æå¡ç«¯å£å· | 8000 | | -
--workers | å·¥ä½è¿ç¨æ° | 1 | æ´å¤åæ° `openai-forward run --help`
-æ¥ç **ç¯å¢åééç½®é¡¹**
-æ¯æä»è¿è¡ç®å½ä¸ç`.env`æä»¶ä¸­è¯»å: | ç¯å¢åé | è¯´æ |
+`BASE_URL`ä¸ºæä»¬èªå·±æ­å»ºçä»£çæå¡å°å  Click for more details
+```bash docker run -d \ -p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -
+e BASE_URL="https://api.openai-forward.com" \ -e CODE="kunyuan" \ yidadaa/
+chatgpt-next-web ``` è¿éé¨ç½²äºä¸ä¸ªï¼ä¾å¤§å®¶è½»åº¦ä½¿ç¨: https://
+chat.beidongjiedeguang.top , è®¿é®å¯ç : `kunyuan`  ### å¨ä»£ç ä¸­ä½¿ç¨
+**Python** ```diff import openai + openai.api_base = "https://api.openai-
+forward.com/v1" openai.api_key = "sk-******" ```  More Examples **JS/TS**
+```diff import { Configuration } from "openai"; const configuration = new
+Configuration({ + basePath: "https://api.openai-forward.com/v1", apiKey: "sk-
+******", }); ``` **gpt-3.5-turbo** ```bash curl https://api.openai-forward.com/
+v1/chat/completions \ -H "Content-Type: application/json" \ -H "Authorization:
+Bearer sk-******" \ -d '{ "model": "gpt-3.5-turbo", "messages": [{"role":
+"user", "content": "Hello!"}] }' ``` **Image Generation (DALL-E)** ```bash curl
+--location 'https://api.openai-forward.com/v1/images/generations' \ --header
+'Authorization: Bearer sk-******' \ --header 'Content-Type: application/json' \
+--data '{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ```  ##
+éç½®éé¡¹ éç½®çè®¾ç½®æ¹å¼æ¯æä¸¤ç§
+ä¸ç§ä¸ºå¨shellä¸­è¿è¡`openai-forward run --
+port=8000`çå½ä»¤è¡æ¹å¼æå®;
+å¦ä¸ç§ä¸ºè¯»åç¯å¢åéçæ¹å¼æå®ã  Click for more details
+**`openai-forward run`åæ°éç½®é¡¹** | éç½®é¡¹ | è¯´æ | é»è®¤å¼ | |---
+--------------|-------------------|:----------------------:| | --port |
+æå¡ç«¯å£å· | 8000 | | --workers | å·¥ä½è¿ç¨æ° | 1 | | --base_url | å
+OPENAI_BASE_URL | https://api.openai.com | | --api_key | å OPENAI_API_KEY |
+`None` | | --forward_key | å FORWARD_KEY | `None` | | --route_prefix | å
+ROUTE_PREFIX | `None` | | --log_chat | å LOG_CHAT | `False` | ä¹å¯éè¿
+`openai-forward run --help` æ¥ç **ç¯å¢åééç½®é¡¹**
+æ¯æä»è¿è¡ç®å½ä¸ç`.env`æä»¶ä¸­è¯»å | ç¯å¢åé | è¯´æ |
 é»è®¤å¼ | |-----------------|------------------------------------------------
------------------|:------------------------:| | OPENAI_API_KEY | é»è®¤openai
-api keyï¼æ¯æå¤ä¸ªé»è®¤api key, ä»¥ `sk-` å¼å¤´ï¼ ä»¥ç©ºæ ¼åå² | æ 
-| | FORWARD_KEY | åè®¸è°ç¨æ¹ä½¿ç¨è¯¥keyä»£æ¿openai api
-keyï¼æ¯æå¤ä¸ªforward key, ä»¥`fk-` å¼å¤´, ä»¥ç©ºæ ¼åå² | æ  | |
-OPENAI_BASE_URL | è½¬åbase url | `https://api.openai.com` | | LOG_CHAT |
-æ¯å¦è®°å½èå¤©åå®¹ | `true` | | ROUTE_PREFIX | è·¯ç±åç¼ | æ  | |
-IP_WHITELIST | ipç½åå, ç©ºæ ¼åå¼ | æ  | | IP_BLACKLIST | ipé»åå,
-ç©ºæ ¼åå¼ | æ  | ## é«çº§éç½® **è®¾ç½®api_keyä¸ºèªå·±è®¾ç½®çforward
-key** éè¦éç½® OPENAI_API_KEY å FORWARD_KEY, ä¾å¦ ```bash
-OPENAI_API_KEY=sk-******* FORWARD_KEY=fk-****** # è¿éfk-
-tokenç±æä»¬èªå·±å®ä¹ ``` è¿éæä»¬éç½®äºFORWARD_KEYä¸º`fk-******`,
+-------------------------------------------------------------------------------
+----|:------------------------:| | OPENAI_BASE_URL | é»è®¤ openaiå®æ¹ api
+å°å | https://api.openai.com | | OPENAI_API_KEY | é»è®¤openai api
+keyï¼æ¯æå¤ä¸ªé»è®¤api key, ä»¥ `sk-` å¼å¤´ï¼ ä»¥ç©ºæ ¼åå² | æ  | |
+FORWARD_KEY | åè®¸è°ç¨æ¹ä½¿ç¨è¯¥keyä»£æ¿openai api
+keyï¼æ¯æå¤ä¸ªforward key, ä»¥ç©ºæ ¼åå²;
+å¦æè®¾ç½®äºOPENAI_API_KEYï¼èæ²¡æè®¾ç½®FORWARD_KEY,
+åå®¢æ·ç«¯è°ç¨æ¶æ éæä¾å¯é¥,
+æ­¤æ¶åºäºå®å¨èèä¸å»ºè®®FORWARD_KEYç½®ç©º | æ  | | OPENAI_BASE_URL |
+è½¬åbase url | `https://api.openai.com` | | ROUTE_PREFIX | è·¯ç±åç¼ | æ 
+| | LOG_CHAT | æ¯å¦è®°å½èå¤©åå®¹ | `false` |  ## é«çº§éç½®
+**è®¾ç½®api_keyä¸ºèªå·±è®¾ç½®çforward key** éè¦éç½® OPENAI_API_KEY å
+FORWARD_KEY, ä¾å¦  Click for more details ```bash OPENAI_API_KEY=sk-*******
+FORWARD_KEY=fk-****** # è¿éfk-tokenç±æä»¬èªå·±å®ä¹ ```
+è¿éæä»¬éç½®äºFORWARD_KEYä¸º`fk-******`,
 é£ä¹åé¢å®¢æ·ç«¯å¨è°ç¨æ¶åªéè®¾ç½®OPENAI_API_KEYä¸ºæä»¬èªå®ä¹ç`fk-
 ******` å³å¯ã
 è¿æ ·çå¥½å¤æ¯å¨ä½¿ç¨ä¸äºéè¦è¾å¥OPENAI_API_KEYçç¬¬ä¸æ¹åºç¨æ¶ï¼æä»¬å¯ä»¥ä½¿ç¨`fk-
-******`æ­éproxyä½¿ç¨ï¼å¦ä¸é¢çä¾å­ï¼
-èæ éæå¿OPENAI_API_KEYè¢«æ³é²ã **ç¨ä¾:** ```bash curl https://
-api.openai-forward.top/v1/chat/completions \ -H "Content-Type: application/
-json" \ -H "Authorization: Bearer fk-******" \ -d '{ "model": "gpt-3.5-turbo",
-"messages": [{"role": "user", "content": "Hello!"}] }' ``` **Python** ```diff
-import openai + openai.api_base = "https://api.openai-forward.top/v1" -
-openai.api_key = "sk-******" + openai.api_key = "fk-******" ``` **Web
-application** ```bash docker run -d \ -p 3000:3000 \ -e OPENAI_API_KEY="fk-
-******" \ -e BASE_URL="https://api.openai-forward.top" \ -e CODE="" \ yidadaa/
-chatgpt-next-web ``` ## èå¤©æ¥å¿ ä¿å­è·¯å¾å¨å½åç®å½ä¸ç`Log/
-`è·¯å¾ä¸­ã èå¤©æ¥å¿ä»¥ `chat_`å¼å¤´,
-é»è®¤æ¯5è½®å¯¹è¯åå¥ä¸æ¬¡æä»¶ è®°å½æ ¼å¼ä¸º ```text {'host': xxx,
-'model': xxx, 'message': [{'user': xxx}, {'assistant': xxx}]} {'assistant':
-xxx} {'host': ...} {'assistant': ...} ... ``` ## Backer and Sponsor [.github/
-images/jetbrains.svg] ## License Openai-forward is licensed under the [MIT]
-(https://opensource.org/license/mit/) license.
+******`æ­éä»£çæå¡ä½¿ç¨ï¼å¦ä¸é¢çä¾å­ï¼
+èæ éæå¿OPENAI_API_KEYè¢«æ³é²ã å¹¶ä¸å¯ä»¥å¯¹å¤åå`fk-******`
+**ç¨ä¾:** ```bash curl https://api.openai-forward.com/v1/chat/completions \ -
+H "Content-Type: application/json" \ -H "Authorization: Bearer fk-******" \ -
+d '{ "model": "gpt-3.5-turbo", "messages": [{"role": "user", "content":
+"Hello!"}] }' ``` **Python** ```diff import openai + openai.api_base = "https:/
+/api.openai-forward.com/v1" - openai.api_key = "sk-******" + openai.api_key =
+"fk-******" ``` **Web application** ```bash docker run -d \ -p 3000:3000 \ -
+e OPENAI_API_KEY="fk-******" \ -e BASE_URL="https://api.openai-forward.com" \ -
+e CODE="" \ yidadaa/chatgpt-next-web ```  ## èå¤©æ¥å¿
+é»è®¤ä¸è®°å½èå¤©æ¥å¿ï¼è¥è¦å¼å¯éè®¾ç½®ç¯å¢åé`LOG_CHAT=true`
+Click for more details ä¿å­è·¯å¾å¨å½åç®å½ä¸ç`Log/
+chat.log`è·¯å¾ä¸­ã è®°å½æ ¼å¼ä¸º ```text {'messages': [{'user': 'hi'}],
+'model': 'gpt-3.5-turbo', 'host': '', 'uid': '467a17ec-bf39-4b65-9ebd-
+e722b3bdd5c3'} {'assistant': 'Hello! How can I assist you today?', 'uid':
+'467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'} {'messages': [{'user': 'Hello!'}],
+'model': 'gpt-3.5-turbo', 'host': '', 'uid': 'f844d156-e747-4887-aef8-
+e40d977b5ee7'} {'assistant': 'Hi there! How can I assist you today?', 'uid':
+'f844d156-e747-4887-aef8-e40d977b5ee7'} ... ``` è½¬æ¢ä¸º`jsonl`æ ¼å¼ï¼
+```bash openai-forward convert ``` å³å¯è½¬æ¢ä¸ºä»¥ä¸æ ¼å¼ï¼ ```json lines
+[ { "messages": [ { "user": "hi!" } ] }, { "assistant": "Hello! How can I
+assist you today?" } ] [ { "messages": [ { "user": "Hello!" } ] },
+{ "assistant": "Hi there! How can I assist you today?" } ] ... ```  ## Backer
+and Sponsor [.github/images/jetbrains.svg] ## License OpenAI-Forward is
+licensed under the [MIT](https://opensource.org/license/mit/) license.
```

