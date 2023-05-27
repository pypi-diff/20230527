# Comparing `tmp/aoirint_liveinfo-0.1.8.tar.gz` & `tmp/aoirint_liveinfo-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aoirint_liveinfo-0.1.8.tar", last modified: Sun Nov 27 18:46:00 2022, max compression
+gzip compressed data, was "aoirint_liveinfo-0.1.9.tar", last modified: Sun Nov 27 18:55:16 2022, max compression
```

## Comparing `aoirint_liveinfo-0.1.8.tar` & `aoirint_liveinfo-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 18:46:00.268383 aoirint_liveinfo-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (122)     7519 2022-11-27 18:46:00.268383 aoirint_liveinfo-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5648 2022-11-27 18:45:48.000000 aoirint_liveinfo-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 18:46:00.264382 aoirint_liveinfo-0.1.8/aoirint_liveinfo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7519 2022-11-27 18:46:00.000000 aoirint_liveinfo-0.1.8/aoirint_liveinfo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      358 2022-11-27 18:46:00.000000 aoirint_liveinfo-0.1.8/aoirint_liveinfo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-27 18:46:00.000000 aoirint_liveinfo-0.1.8/aoirint_liveinfo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2022-11-27 18:46:00.000000 aoirint_liveinfo-0.1.8/aoirint_liveinfo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2022-11-27 18:46:00.000000 aoirint_liveinfo-0.1.8/aoirint_liveinfo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2022-11-27 18:46:00.000000 aoirint_liveinfo-0.1.8/aoirint_liveinfo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 18:46:00.268383 aoirint_liveinfo-0.1.8/liveinfo/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2022-11-27 18:45:59.000000 aoirint_liveinfo-0.1.8/liveinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2022-11-27 18:45:48.000000 aoirint_liveinfo-0.1.8/liveinfo/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2022-11-27 18:45:48.000000 aoirint_liveinfo-0.1.8/liveinfo/liveinfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     9835 2022-11-27 18:45:48.000000 aoirint_liveinfo-0.1.8/liveinfo/nicolive.py
--rw-r--r--   0 runner    (1001) docker     (122)    20854 2022-11-27 18:45:48.000000 aoirint_liveinfo-0.1.8/liveinfo/ytlive.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-27 18:46:00.268383 aoirint_liveinfo-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1134 2022-11-27 18:45:48.000000 aoirint_liveinfo-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 18:55:16.649827 aoirint_liveinfo-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     8037 2022-11-27 18:55:16.649827 aoirint_liveinfo-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6094 2022-11-27 18:55:07.000000 aoirint_liveinfo-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 18:55:16.649827 aoirint_liveinfo-0.1.9/aoirint_liveinfo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8037 2022-11-27 18:55:16.000000 aoirint_liveinfo-0.1.9/aoirint_liveinfo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      358 2022-11-27 18:55:16.000000 aoirint_liveinfo-0.1.9/aoirint_liveinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-27 18:55:16.000000 aoirint_liveinfo-0.1.9/aoirint_liveinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2022-11-27 18:55:16.000000 aoirint_liveinfo-0.1.9/aoirint_liveinfo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2022-11-27 18:55:16.000000 aoirint_liveinfo-0.1.9/aoirint_liveinfo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2022-11-27 18:55:16.000000 aoirint_liveinfo-0.1.9/aoirint_liveinfo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 18:55:16.649827 aoirint_liveinfo-0.1.9/liveinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2022-11-27 18:55:16.000000 aoirint_liveinfo-0.1.9/liveinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2022-11-27 18:55:07.000000 aoirint_liveinfo-0.1.9/liveinfo/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2022-11-27 18:55:07.000000 aoirint_liveinfo-0.1.9/liveinfo/liveinfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9835 2022-11-27 18:55:07.000000 aoirint_liveinfo-0.1.9/liveinfo/nicolive.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20854 2022-11-27 18:55:07.000000 aoirint_liveinfo-0.1.9/liveinfo/ytlive.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-27 18:55:16.649827 aoirint_liveinfo-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1134 2022-11-27 18:55:07.000000 aoirint_liveinfo-0.1.9/setup.py
```

### Comparing `aoirint_liveinfo-0.1.8/PKG-INFO` & `aoirint_liveinfo-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aoirint_liveinfo
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/aoirint/liveinfopy
 Author: aoirint
 Author-email: aoirint@gmail.com
 License: MIT
 Description: # liveinfopy
         
@@ -89,14 +89,23 @@
         
         引数にはチャンネルID（URL・ハンドル名は使用不可）を渡してください。
         
         ```shell
         liveinfo -s ytlive --ytlive_api_key_file /secrets/ytlive_api_key "UC7OazbQ3Eo9vrkcReXGIZkQ"
         ```
         
+        ハンドル名が設定されたチャンネルでは、チャンネルIDがURLに含まれなくなるため、
+        チャンネルIDを調べるのが難しいことがあります。
+        チャンネル個別ページを開き、開発者ツールで以下のJavaScriptコードを実行すると、簡単にチャンネルIDを確認できます（2022-11-28 現在）。
+        
+        ```shell
+        document.querySelector('meta[itemprop="channelId"]').content
+        ```
+        
+        
         #### 現在の仕様
         
         - 最新5件の動画・生放送・プレミア公開動画から、生放送・プレミア公開動画を抽出
         - 公開設定が「公開」のコンテンツのみを返す（限定公開、非公開は含まれない）
         - `liveBroadcastContent`
           - ライブ配信予約: `upcoming`
           - ライブ配信中: `live`
```

### Comparing `aoirint_liveinfo-0.1.8/README.md` & `aoirint_liveinfo-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,23 @@
 
 引数にはチャンネルID（URL・ハンドル名は使用不可）を渡してください。
 
 ```shell
 liveinfo -s ytlive --ytlive_api_key_file /secrets/ytlive_api_key "UC7OazbQ3Eo9vrkcReXGIZkQ"
 ```
 
+ハンドル名が設定されたチャンネルでは、チャンネルIDがURLに含まれなくなるため、
+チャンネルIDを調べるのが難しいことがあります。
+チャンネル個別ページを開き、開発者ツールで以下のJavaScriptコードを実行すると、簡単にチャンネルIDを確認できます（2022-11-28 現在）。
+
+```shell
+document.querySelector('meta[itemprop="channelId"]').content
+```
+
+
 #### 現在の仕様
 
 - 最新5件の動画・生放送・プレミア公開動画から、生放送・プレミア公開動画を抽出
 - 公開設定が「公開」のコンテンツのみを返す（限定公開、非公開は含まれない）
 - `liveBroadcastContent`
   - ライブ配信予約: `upcoming`
   - ライブ配信中: `live`
```

### Comparing `aoirint_liveinfo-0.1.8/aoirint_liveinfo.egg-info/PKG-INFO` & `aoirint_liveinfo-0.1.9/aoirint_liveinfo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aoirint-liveinfo
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/aoirint/liveinfopy
 Author: aoirint
 Author-email: aoirint@gmail.com
 License: MIT
 Description: # liveinfopy
         
@@ -89,14 +89,23 @@
         
         引数にはチャンネルID（URL・ハンドル名は使用不可）を渡してください。
         
         ```shell
         liveinfo -s ytlive --ytlive_api_key_file /secrets/ytlive_api_key "UC7OazbQ3Eo9vrkcReXGIZkQ"
         ```
         
+        ハンドル名が設定されたチャンネルでは、チャンネルIDがURLに含まれなくなるため、
+        チャンネルIDを調べるのが難しいことがあります。
+        チャンネル個別ページを開き、開発者ツールで以下のJavaScriptコードを実行すると、簡単にチャンネルIDを確認できます（2022-11-28 現在）。
+        
+        ```shell
+        document.querySelector('meta[itemprop="channelId"]').content
+        ```
+        
+        
         #### 現在の仕様
         
         - 最新5件の動画・生放送・プレミア公開動画から、生放送・プレミア公開動画を抽出
         - 公開設定が「公開」のコンテンツのみを返す（限定公開、非公開は含まれない）
         - `liveBroadcastContent`
           - ライブ配信予約: `upcoming`
           - ライブ配信中: `live`
```

### Comparing `aoirint_liveinfo-0.1.8/liveinfo/cli.py` & `aoirint_liveinfo-0.1.9/liveinfo/cli.py`

 * *Files identical despite different names*

### Comparing `aoirint_liveinfo-0.1.8/liveinfo/liveinfo.py` & `aoirint_liveinfo-0.1.9/liveinfo/liveinfo.py`

 * *Files identical despite different names*

### Comparing `aoirint_liveinfo-0.1.8/liveinfo/nicolive.py` & `aoirint_liveinfo-0.1.9/liveinfo/nicolive.py`

 * *Files identical despite different names*

### Comparing `aoirint_liveinfo-0.1.8/liveinfo/ytlive.py` & `aoirint_liveinfo-0.1.9/liveinfo/ytlive.py`

 * *Files identical despite different names*

### Comparing `aoirint_liveinfo-0.1.8/setup.py` & `aoirint_liveinfo-0.1.9/setup.py`

 * *Files identical despite different names*

