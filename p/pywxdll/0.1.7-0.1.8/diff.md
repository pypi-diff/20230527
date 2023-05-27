# Comparing `tmp/pywxdll-0.1.7.tar.gz` & `tmp/pywxdll-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywxdll-0.1.7.tar", last modified: Thu May 25 10:36:02 2023, max compression
+gzip compressed data, was "dist/pywxdll-0.1.8.tar", last modified: Sat May 27 17:50:30 2023, max compression
```

## Comparing `pywxdll-0.1.7.tar` & `pywxdll-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-25 10:36:02.000000 pywxdll-0.1.7/
--rw-r--r--   0 henryyang   (501) staff       (20)     1067 2023-04-30 06:33:02.000000 pywxdll-0.1.7/LICENSE
--rw-rw-r--   0 henryyang   (501) staff       (20)       26 2023-05-01 18:24:33.000000 pywxdll-0.1.7/MANIFEST.in
--rw-r--r--   0 henryyang   (501) staff       (20)      699 2023-05-25 10:36:02.000000 pywxdll-0.1.7/PKG-INFO
--rw-r--r--   0 henryyang   (501) staff       (20)      577 2023-05-02 16:49:34.000000 pywxdll-0.1.7/README.md
-drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-25 10:36:02.000000 pywxdll-0.1.7/pywxdll/
--rw-r--r--   0 henryyang   (501) staff       (20)       74 2023-05-25 10:32:34.000000 pywxdll-0.1.7/pywxdll/__init__.py
--rw-r--r--   0 henryyang   (501) staff       (20)     6353 2023-05-25 10:33:14.000000 pywxdll-0.1.7/pywxdll/pywxdll.py
--rw-r--r--   0 henryyang   (501) staff       (20)     4028 2023-05-25 10:33:14.000000 pywxdll-0.1.7/pywxdll/pywxdll_json.py
-drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-25 10:36:02.000000 pywxdll-0.1.7/pywxdll.egg-info/
--rw-r--r--   0 henryyang   (501) staff       (20)        1 2023-05-02 16:36:22.000000 pywxdll-0.1.7/pywxdll.egg-info/.gitignore
--rw-r--r--   0 henryyang   (501) staff       (20)      699 2023-05-25 10:36:02.000000 pywxdll-0.1.7/pywxdll.egg-info/PKG-INFO
--rw-r--r--   0 henryyang   (501) staff       (20)      283 2023-05-25 10:36:02.000000 pywxdll-0.1.7/pywxdll.egg-info/SOURCES.txt
--rw-r--r--   0 henryyang   (501) staff       (20)        1 2023-05-25 10:36:02.000000 pywxdll-0.1.7/pywxdll.egg-info/dependency_links.txt
--rw-r--r--   0 henryyang   (501) staff       (20)       26 2023-05-25 10:36:02.000000 pywxdll-0.1.7/pywxdll.egg-info/requires.txt
--rw-r--r--   0 henryyang   (501) staff       (20)        8 2023-05-25 10:36:02.000000 pywxdll-0.1.7/pywxdll.egg-info/top_level.txt
--rw-r--r--   0 henryyang   (501) staff       (20)       38 2023-05-25 10:36:02.000000 pywxdll-0.1.7/setup.cfg
--rw-r--r--   0 henryyang   (501) staff       (20)     3743 2023-05-25 10:32:31.000000 pywxdll-0.1.7/setup.py
+drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-27 17:50:30.000000 pywxdll-0.1.8/
+-rw-r--r--   0 henryyang   (501) staff       (20)     1067 2023-04-30 06:33:02.000000 pywxdll-0.1.8/LICENSE
+-rw-rw-r--   0 henryyang   (501) staff       (20)       26 2023-05-01 18:24:33.000000 pywxdll-0.1.8/MANIFEST.in
+-rw-r--r--   0 henryyang   (501) staff       (20)      699 2023-05-27 17:50:30.000000 pywxdll-0.1.8/PKG-INFO
+-rw-r--r--   0 henryyang   (501) staff       (20)      577 2023-05-02 16:49:34.000000 pywxdll-0.1.8/README.md
+drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-27 17:50:30.000000 pywxdll-0.1.8/pywxdll/
+-rw-r--r--   0 henryyang   (501) staff       (20)       74 2023-05-27 17:48:44.000000 pywxdll-0.1.8/pywxdll/__init__.py
+-rw-r--r--   0 henryyang   (501) staff       (20)     6244 2023-05-27 17:46:40.000000 pywxdll-0.1.8/pywxdll/pywxdll.py
+-rw-r--r--   0 henryyang   (501) staff       (20)     4038 2023-05-27 17:43:06.000000 pywxdll-0.1.8/pywxdll/pywxdll_json.py
+drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-27 17:50:30.000000 pywxdll-0.1.8/pywxdll.egg-info/
+-rw-r--r--   0 henryyang   (501) staff       (20)        1 2023-05-02 16:36:22.000000 pywxdll-0.1.8/pywxdll.egg-info/.gitignore
+-rw-r--r--   0 henryyang   (501) staff       (20)      699 2023-05-27 17:50:30.000000 pywxdll-0.1.8/pywxdll.egg-info/PKG-INFO
+-rw-r--r--   0 henryyang   (501) staff       (20)      283 2023-05-27 17:50:30.000000 pywxdll-0.1.8/pywxdll.egg-info/SOURCES.txt
+-rw-r--r--   0 henryyang   (501) staff       (20)        1 2023-05-27 17:50:30.000000 pywxdll-0.1.8/pywxdll.egg-info/dependency_links.txt
+-rw-r--r--   0 henryyang   (501) staff       (20)       26 2023-05-27 17:50:30.000000 pywxdll-0.1.8/pywxdll.egg-info/requires.txt
+-rw-r--r--   0 henryyang   (501) staff       (20)        8 2023-05-27 17:50:30.000000 pywxdll-0.1.8/pywxdll.egg-info/top_level.txt
+-rw-r--r--   0 henryyang   (501) staff       (20)       38 2023-05-27 17:50:30.000000 pywxdll-0.1.8/setup.cfg
+-rw-r--r--   0 henryyang   (501) staff       (20)     3743 2023-05-27 17:48:48.000000 pywxdll-0.1.8/setup.py
```

### Comparing `pywxdll-0.1.7/LICENSE` & `pywxdll-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pywxdll-0.1.7/PKG-INFO` & `pywxdll-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywxdll
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python package for wechat dll hook
 Home-page: https://github.com/HenryXiaoYang/pywxdll
 Author: HenryXiaoYang
 Author-email: henryyang666@hotmal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pywxdll-0.1.7/README.md` & `pywxdll-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pywxdll-0.1.7/pywxdll/pywxdll.py` & `pywxdll-0.1.8/pywxdll/pywxdll.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,20 +52,20 @@
     def on_open(self, ws):  # For websocket
         pass
 
     def on_message(self, ws, message):  # For websocket
         recieve = json.loads(message)
         r_type = recieve['type']
         if r_type == 5005:
-            print('Heartbeat')
+            pass
         elif r_type == 1 or r_type == 3:
             self.msg_list.append(self.recv_txt_handle(recieve))
 
     def on_error(self, ws, error):  # For websocket
-        print(error)
+        raise error
 
     def on_close(self, ws):  # For websocket
         pass
 
     ######## Recieve ########
 
     # 返回所有收到的信息 不建议使用 Return all the messages recieved  #USE IN CAUTION!
@@ -92,18 +92,17 @@
             'wxid': 'null',
             'content': 'null',
             'nickname': 'null',
             'ext': 'null',
         }
         base_data.update(data)
         url = f'http://{self.ip}:{self.port}/{uri}'
-        try:
-            rsp = requests.post(url, json={'para': base_data})
-        except:
-            print('发送信息失败！信息：', base_data)
+
+        rsp = requests.post(url, json={'para': base_data})
+
         rsp = rsp.json()
         if 'content' in rsp and isinstance(rsp['content'], str):
             try:
                 rsp['content'] = json.loads(rsp['content'])
             except:
                 pass
         return rsp
```

### Comparing `pywxdll-0.1.7/pywxdll/pywxdll_json.py` & `pywxdll-0.1.8/pywxdll/pywxdll_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # 发送txt消息到个人或群 wxid为用户id或群id content为发送内容  Send txt message to a wxid(perosnal or group)
 def json_send_txt_msg(wxid, content: str):
     qs = {
         'id': getid(),
         'type': TXT_MSG,
         'roomid': 'null',
         'wxid': wxid,
-        'content': content,
+        'content': str(content),
         'nickname': 'null',
         'ext': 'null'
     }
     return json.dumps(qs)
 
 
 # 发送图片信息 wxid为用户id或群id path为发送图片的路径（建议用绝对路径） Send picture to wxid(perosnal or group)
@@ -54,15 +54,15 @@
 # 发送@信息 roomid为群id wxid为用户id nickname为@的人昵称 content为发送内容 send @ message
 def json_send_at_msg(roomid, wxid, nickname: str, content: str):
     qs = {
         'id': getid(),
         'type': AT_MSG,
         'roomid': roomid,
         'wxid': wxid,
-        'content': content,
+        'content': str(content),
         'nickname': nickname,
         'ext': 'null'
     }
     s = json.dumps(qs)
     return s
```

### Comparing `pywxdll-0.1.7/pywxdll.egg-info/PKG-INFO` & `pywxdll-0.1.8/pywxdll.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywxdll
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python package for wechat dll hook
 Home-page: https://github.com/HenryXiaoYang/pywxdll
 Author: HenryXiaoYang
 Author-email: henryyang666@hotmal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pywxdll-0.1.7/setup.py` & `pywxdll-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pywxdll'
 DESCRIPTION = 'A Python package for wechat dll hook'
 URL = 'https://github.com/HenryXiaoYang/pywxdll'
 EMAIL = 'henryyang666@hotmal.com'
 AUTHOR = 'HenryXiaoYang'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 
 # What packages are required for this module to be executed?
 REQUIRED = ['websocket-client', 'requests']
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

