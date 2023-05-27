# Comparing `tmp/Musicreater-0.5.1.tar.gz` & `tmp/Musicreater-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Musicreater-0.5.1.tar", last modified: Mon May  1 04:41:54 2023, max compression
+gzip compressed data, was "Musicreater-1.0.0.tar", last modified: Sat May 27 11:56:56 2023, max compression
```

## Comparing `Musicreater-0.5.1.tar` & `Musicreater-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 04:41:54.062459 Musicreater-0.5.1/
--rw-rw-rw-   0        0        0    13085 2023-02-05 09:39:58.000000 Musicreater-0.5.1/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-05-01 04:41:54.049458 Musicreater-0.5.1/Musicreater/
--rw-rw-rw-   0        0        0      890 2023-05-01 04:41:16.000000 Musicreater-0.5.1/Musicreater/__init__.py
--rw-rw-rw-   0        0        0     3197 2023-04-29 13:59:22.000000 Musicreater-0.5.1/Musicreater/exceptions.py
--rw-rw-rw-   0        0        0     5479 2023-04-29 11:13:55.000000 Musicreater-0.5.1/Musicreater/instConstants.py
--rw-rw-rw-   0        0        0    10696 2023-04-29 11:13:55.000000 Musicreater-0.5.1/Musicreater/magicmain.py
--rw-rw-rw-   0        0        0    79747 2023-05-01 04:41:16.000000 Musicreater-0.5.1/Musicreater/main.py
--rw-rw-rw-   0        0        0    13516 2023-04-30 14:43:50.000000 Musicreater-0.5.1/Musicreater/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:41:54.059455 Musicreater-0.5.1/Musicreater.egg-info/
--rw-rw-rw-   0        0        0     7718 2023-05-01 04:41:53.000000 Musicreater-0.5.1/Musicreater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-05-01 04:41:53.000000 Musicreater-0.5.1/Musicreater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 04:41:53.000000 Musicreater-0.5.1/Musicreater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-01 04:41:53.000000 Musicreater-0.5.1/Musicreater.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 04:41:53.000000 Musicreater-0.5.1/Musicreater.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7718 2023-05-01 04:41:54.061458 Musicreater-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     6649 2023-05-01 04:41:16.000000 Musicreater-0.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 04:41:54.062459 Musicreater-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1597 2023-04-29 13:59:22.000000 Musicreater-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:56:56.378165 Musicreater-1.0.0/
+-rw-rw-rw-   0        0        0    13072 2023-05-27 11:45:04.000000 Musicreater-1.0.0/LICENSE.md
+drwxrwxrwx   0        0        0        0 2023-05-27 11:56:56.234645 Musicreater-1.0.0/Musicreater/
+-rw-rw-rw-   0        0        0      824 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/__init__.py
+-rw-rw-rw-   0        0        0     6525 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/constants.py
+-rw-rw-rw-   0        0        0     2903 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/exceptions.py
+-rw-rw-rw-   0        0        0    12850 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/experiment.py
+-rw-rw-rw-   0        0        0    10301 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/magicmain.py
+-rw-rw-rw-   0        0        0    32861 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/main.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:56:56.316371 Musicreater-1.0.0/Musicreater/plugin/
+-rw-rw-rw-   0        0        0      559 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/__init__.py
+-rw-rw-rw-   0        0        0     2112 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/archive.py
+-rw-rw-rw-   0        0        0     5999 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/bdx.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:56:56.328331 Musicreater-1.0.0/Musicreater/plugin/bdxfile/
+-rw-rw-rw-   0        0        0      513 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/bdxfile/__init__.py
+-rw-rw-rw-   0        0        0     6194 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/bdxfile/main.py
+-rw-rw-rw-   0        0        0      809 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/common.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:56:56.343282 Musicreater-1.0.0/Musicreater/plugin/funcpack/
+-rw-rw-rw-   0        0        0      513 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/funcpack/__init__.py
+-rw-rw-rw-   0        0        0     3896 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/funcpack/main.py
+-rw-rw-rw-   0        0        0     2492 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/main.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:56:56.355241 Musicreater-1.0.0/Musicreater/plugin/mcstructfile/
+-rw-rw-rw-   0        0        0      521 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/mcstructfile/__init__.py
+-rw-rw-rw-   0        0        0     1836 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/mcstructfile/main.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:56:56.368198 Musicreater-1.0.0/Musicreater/plugin/mcstructpack/
+-rw-rw-rw-   0        0        0      513 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/mcstructpack/__init__.py
+-rw-rw-rw-   0        0        0     6242 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/mcstructpack/main.py
+-rw-rw-rw-   0        0        0     7153 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/mcstructure.py
+-rw-rw-rw-   0        0        0     4535 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/subclass.py
+-rw-rw-rw-   0        0        0      848 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:56:56.273517 Musicreater-1.0.0/Musicreater.egg-info/
+-rw-rw-rw-   0        0        0     7816 2023-05-27 11:56:54.000000 Musicreater-1.0.0/Musicreater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      889 2023-05-27 11:56:55.000000 Musicreater-1.0.0/Musicreater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 11:56:55.000000 Musicreater-1.0.0/Musicreater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-27 11:56:55.000000 Musicreater-1.0.0/Musicreater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-27 11:56:55.000000 Musicreater-1.0.0/Musicreater.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7816 2023-05-27 11:56:56.375178 Musicreater-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6747 2023-05-27 11:45:04.000000 Musicreater-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-27 11:56:56.379161 Musicreater-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1597 2023-05-27 11:45:04.000000 Musicreater-1.0.0/setup.py
```

### Comparing `Musicreater-0.5.1/LICENSE.md` & `Musicreater-1.0.0/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 **注意，以下条款或版权声明应当且必须是高于此项目中任何其他声明的**
 
 1. 音·创的全部开发者享有其完整版权，其开发者可以在任一时刻终止以后音·创源代码开放，若经由其开发者授予特殊权利，则授权对象可以将源代码进行特定的被特殊授权的操作
 2. 音·创或（及）其代码允许在 Apache2.0 协议的条款与说明下进行非商业使用
 3. 除部分代码特殊声明外，音·创允许对其或（及）其代码进行商业化使用，但是需要经过音·创主要开发者（诸葛亮与八卦阵、金羿）的一致授权，同时，授权对象在商业化授权的使用过程中必须依照 Apache2.0 协议的条款与说明
-4. 若存在对于音·创包含的部分代码的特殊开源声明，则此部分代码依照其特定的开源方式授权，但若此部分代码经由此部分代码的主要开发者一致特殊授权后商用，则授权对象在商用时依照此部分的开发者所准许的方式（或条款）进行商用，或默认依照 Apache2.0 协议进行商业化使用
+4. 若存在对于音·创包含的部分代码的特殊开源声明，则此部分代码依照其特定的开源方式授权，但若此部分代码经由此部分代码的主要开发者一致特殊授权后商用，则授权对象在商用时依照此部分的开发者所准许的方式（或条款）进行商用
 5. Apache2.0 协议的英文原文副本可见下文
 
 >  The English Translation of the TERMS AND CONDITIONS above is listed below
 >
 >  This translated version is for reference only and has no legal effect.
 >
 >  The version with legal effect is the Chinese version above.
@@ -199,15 +199,15 @@
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
 
-   Copyright 2022 Team-Ryoun 金羿("Eilles Wan") & 诸葛亮与八卦阵("bgArray")
+   Copyright 2022 TriM-Organization 金羿("Eilles Wan") & 诸葛亮与八卦阵("bgArray") & all the developers of Musicreater
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `Musicreater-0.5.1/Musicreater/__init__.py` & `Musicreater-1.0.0/Musicreater/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,21 +4,20 @@
 是一款免费开源的针对《我的世界》的midi音乐转换库
 Musicreater(音·创)
 A free open source library used for convert midi file into formats that is suitable for **Minecraft**.
 
 版权所有 © 2023 音·创 开发者
 Copyright © 2023 all the developers of Musicreater
 
-开源相关声明请见 ../License.md
-Terms & Conditions: ../License.md
+开源相关声明请见 仓库根目录下的 License.md
+Terms & Conditions: License.md in the root directory
 """
 
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
-# 版权所有 金羿("Eilles Wan") & 诸葛亮与八卦阵("bgArray") & 鸣凤鸽子("MingFengPigeon")
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 from .main import *
 
-__version__ = "0.5.1"
+__version__ = "1.0.0"
 __all__ = []
 __author__ = (("金羿", "Eilles Wan"), ("诸葛亮与八卦阵", "bgArray"), ("鸣凤鸽子", "MingFengPigeon"))
```

### Comparing `Musicreater-0.5.1/Musicreater/exceptions.py` & `Musicreater-1.0.0/Musicreater/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # -*- coding: utf-8 -*-
 
+"""
+存放一堆报错类型
+"""
+
+"""
+版权所有 © 2023 音·创 开发者
+Copyright © 2023 all the developers of Musicreater
+
+开源相关声明请见 仓库根目录下的 License.md
+Terms & Conditions: License.md in the root directory
+"""
 
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
-# 版权所有 金羿("Eilles Wan") & 诸葛亮与八卦阵("bgArray") & 鸣凤鸽子("MingFengPigeon")
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 
-"""一个简单的我的世界音频转换库
-音·创 (Musicreater)
-是一款免费开源的针对《我的世界》的midi音乐转换库
-Musicreater(音·创)
-A free open source library used for convert midi file into formats that is suitable for **Minecraft**.
-
-版权所有 © 2023 音·创 开发者
-Copyright © 2023 all the developers of Musicreater
-
-开源相关声明请见 ../License.md
-Terms & Conditions: ../License.md
-"""
 
 
 class MSCTBaseException(Exception):
     """音·创库版本的所有错误均继承于此"""
 
     def __init__(self, *args):
         """音·创库版本的所有错误均继承于此"""
```

### Comparing `Musicreater-0.5.1/Musicreater/magicmain.py` & `Musicreater-1.0.0/Musicreater/magicmain.py`

 * *Files 5% similar despite different names*

```diff
@@ -208,15 +208,15 @@
 
 
 
 # ============================
 
 
 from typing import Union
-from .utils import x,y,z,bottem_side_length_of_smallest_square_bottom_box,form_note_block_in_NBT_struct,form_repeater_in_NBT_struct
+from .plugin import x,y,z,bottem_side_length_of_smallest_square_bottom_box,form_note_block_in_NBT_struct,form_repeater_in_NBT_struct
 
 # 不要用 没写完
 def delay_to_note_blocks(
     baseblock: str = "stone", 
     position_forward: Union(x, y, z) = z,
     max_height: int = 64,
 ):
@@ -239,67 +239,58 @@
 
     log = print
 
     startpos = [0,0,0]
 
 
     # 1拍 x 2.5 rt
-    def placeNoteBlock():
-        for i in notes:
-            error = True
-            try:
-                struct.set_block(
-                    [startpos[0], startpos[1] + 1, startpos[2]],
-                    form_note_block_in_NBT_struct(height2note[i[0]], instrument),
-                )
-                struct.set_block(startpos, Block("universal_minecraft", instuments[i[0]][1]),)
-                error = False
-            except ValueError:
+    for i in notes:
+        error = True
+        try:
+            struct.set_block(
+                [startpos[0], startpos[1] + 1, startpos[2]],
+                form_note_block_in_NBT_struct(height2note[i[0]], instrument),
+            )
+            struct.set_block(startpos, Block("universal_minecraft", instuments[i[0]][1]),)
+            error = False
+        except ValueError:
+            log("无法放置音符：" + str(i) + "于" + str(startpos))
+            struct.set_block(Block("universal_minecraft", baseblock), startpos)
+            struct.set_block(
+                Block("universal_minecraft", baseblock),
+                [startpos[0], startpos[1] + 1, startpos[2]],
+            )
+        finally:
+            if error is True:
                 log("无法放置音符：" + str(i) + "于" + str(startpos))
                 struct.set_block(Block("universal_minecraft", baseblock), startpos)
                 struct.set_block(
                     Block("universal_minecraft", baseblock),
                     [startpos[0], startpos[1] + 1, startpos[2]],
                 )
-            finally:
-                if error is True:
-                    log("无法放置音符：" + str(i) + "于" + str(startpos))
-                    struct.set_block(Block("universal_minecraft", baseblock), startpos)
-                    struct.set_block(
-                        Block("universal_minecraft", baseblock),
-                        [startpos[0], startpos[1] + 1, startpos[2]],
-                    )
-            delay = int(i[1] * speed + 0.5)
-            if delay <= 4:
+        delay = int(i[1] * speed + 0.5)
+        if delay <= 4:
+            startpos[0] += 1
+            struct.set_block(
+                form_repeater_in_NBT_struct(delay, "west"),
+                [startpos[0], startpos[1] + 1, startpos[2]],
+            )
+            struct.set_block(Block("universal_minecraft", baseblock), startpos)
+        else:
+            for j in range(int(delay / 4)):
                 startpos[0] += 1
                 struct.set_block(
-                    form_repeater_in_NBT_struct(delay, "west"),
+                    form_repeater_in_NBT_struct(4, "west"),
                     [startpos[0], startpos[1] + 1, startpos[2]],
                 )
                 struct.set_block(Block("universal_minecraft", baseblock), startpos)
-            else:
-                for j in range(int(delay / 4)):
-                    startpos[0] += 1
-                    struct.set_block(
-                        form_repeater_in_NBT_struct(4, "west"),
-                        [startpos[0], startpos[1] + 1, startpos[2]],
-                    )
-                    struct.set_block(Block("universal_minecraft", baseblock), startpos)
-                if delay % 4 != 0:
-                    startpos[0] += 1
-                    struct.set_block(
-                        form_repeater_in_NBT_struct(delay % 4, "west"),
-                        [startpos[0], startpos[1] + 1, startpos[2]],
-                    )
-                    struct.set_block(Block("universal_minecraft", baseblock), startpos)
-            startpos[0] += posadder[0]
-            startpos[1] += posadder[1]
-            startpos[2] += posadder[2]
-
-    # e = True
-    try:
-        placeNoteBlock()
-        # e = False
-    except:  # ValueError
-        log("无法放置方块了，可能是因为区块未加载叭")
-
+            if delay % 4 != 0:
+                startpos[0] += 1
+                struct.set_block(
+                    form_repeater_in_NBT_struct(delay % 4, "west"),
+                    [startpos[0], startpos[1] + 1, startpos[2]],
+                )
+                struct.set_block(Block("universal_minecraft", baseblock), startpos)
+        startpos[0] += posadder[0]
+        startpos[1] += posadder[1]
+        startpos[2] += posadder[2]
```

### Comparing `Musicreater-0.5.1/Musicreater.egg-info/PKG-INFO` & `Musicreater-1.0.0/Musicreater.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Musicreater
-Version: 0.5.1
+Version: 1.0.0
 Summary: 一款免费开源的 《我的世界》 mid音乐转换库。
 Home-page: https://github.com/TriM-Organization/Musicreater
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,140 +16,135 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-
 <h1 align="center">
     音·创 Musicreater
 </h1>
 
 <p align="center">
     <img width="128" height="128" src="https://gitee.com/TriM-Organization/Musicreater/raw/master/resources/msctIcon.ico">
     </img>
 </p>
 
-<h3 align="center">一款免费开源的 《我的世界》 MIDI音乐转换库。</h3>
+<h3 align="center">一款免费开源的《我的世界》数字音频转换库。</h3>
 
 <p align="center">
     <img src="https://forthebadge.com/images/badges/built-with-love.svg">
     <a href='https://gitee.com/TriM-Organization/Musicreater'>
         <img align="right" src='https://gitee.com/TriM-Organization/Musicreater/widgets/widget_1.svg' alt='Fork me on Gitee'>
         </img>
     </a>
 <p>
 
-
-
-
-
 [![][Bilibili: 金羿ELS]](https://space.bilibili.com/397369002/)
-[![][Bilibili: 诸葛亮与八卦阵]](https://space.bilibili.com/604072474) 
+[![][Bilibili: 诸葛亮与八卦阵]](https://space.bilibili.com/604072474)
 [![CodeStyle: black]](https://github.com/psf/black)
 [![][python]](https://www.python.org/)
 [![][license]](LICENSE)
 [![][release]](../../releases)
 
 [![GiteeStar](https://gitee.com/TriM-Organization/Musicreater/badge/star.svg?theme=gray)](https://gitee.com/TriM-Organization/Musicreater/stargazers)
 [![GiteeFork](https://gitee.com/TriM-Organization/Musicreater/badge/fork.svg?theme=gray)](https://gitee.com/TriM-Organization/Musicreater/members)
 [![GitHub Repo stars](https://img.shields.io/github/stars/TriM-Organization/Musicreater?color=white&logo=GitHub&style=plastic)](https://github.com/TriM-Organization/Musicreater/stargazers)
 [![GitHub Repo Forks](https://img.shields.io/github/forks/TriM-Organization/Musicreater?color=white&logo=GitHub&style=plastic)](https://github.com/TriM-Organization/Musicreater/forks)
 
+简体中文 🇨🇳 | [English🇬🇧](README_EN.md)
 
-简体中文🇨🇳 | [English🇬🇧](README_EN.md)
-
+## 介绍 🚀
 
-## 介绍🚀
-
-音·创 是一个免费开源的针对 **《我的世界》** 的MIDI音乐转换库
+音·创 是一个免费开源的针对 **《我的世界》** 的 MIDI 音乐转换库
 
 欢迎加群：[861684859](https://jq.qq.com/?_wv=1027&k=hpeRxrYr)
 
-## 下载安装
+## 安装 🔳
+
+- 使用 pypi
 
-- 使用pypi
-    ```bash
-    pip install Musicreater
-    ```
+  ```bash
+  pip install Musicreater
+  ```
 
 - 如果出现错误，可以尝试：
-    ```bash
-    pip install -i https://pypi.python.org/simple Musicreater
-    ```
-- （对于开发者来说）升级：
-    ```bash
-    pip install -i https://pypi.python.org/simple Musicreater --upgrade
-    ```
+  ```bash
+  pip install -i https://pypi.python.org/simple Musicreater
+  ```
+
+- 升级：
+
+  ```bash
+  pip install -i https://pypi.python.org/simple Musicreater --upgrade
+  ```
 
 - 克隆仓库并安装
-    ```bash
-    git clone https://gitee.com/TriM-Organization/Musicreater.git
-    cd Musicreater
-    python setup.py install
-    ```
+  ```bash
+  git clone https://gitee.com/TriM-Organization/Musicreater.git
+  cd Musicreater
+  python setup.py install
+  ```
 
-以上命令种 `python`、`pip` 请依照各个环境不同灵活更换，可能为`python3`或`pip3`之类。
+以上命令中 `python`、`pip` 请依照各个环境不同灵活更换，可能为`python3`或`pip3`之类。
 
-## 文档📄
+## 文档 📄
 
 [生成文件的使用](https://github.com/TriM-Organization/Musicreater/blob/master/docs/%E7%94%9F%E6%88%90%E6%96%87%E4%BB%B6%E7%9A%84%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E.md)
 
-[仓库API文档](https://github.com/TriM-Organization/Musicreater/blob/master/docs/%E5%BA%93%E7%9A%84%E7%94%9F%E6%88%90%E4%B8%8E%E5%8A%9F%E8%83%BD%E6%96%87%E6%A1%A3.md)
+[仓库 API 文档](https://github.com/TriM-Organization/Musicreater/blob/master/docs/%E5%BA%93%E7%9A%84%E7%94%9F%E6%88%90%E4%B8%8E%E5%8A%9F%E8%83%BD%E6%96%87%E6%A1%A3.md)
 
-## 作者✒
+## 作者 ✒
 
-金羿 Eilles：我的世界基岩版指令师，个人开发者，B站不知名UP主，江西在校高中生。
+金羿 Eilles：我的世界基岩版指令师，个人开发者，B 站不知名 UP 主，江西在校高中生。
 
 诸葛亮与八卦阵 bgArray：我的世界基岩版玩家，喜欢编程和音乐，深圳初二学生。
 
-## 致谢🙏
+## 致谢 🙏
+
 本致谢列表排名无顺序。
 
-- 感谢 **昀梦**\<QQ1515399885\> 找出指令生成错误bug并指正
-- 感谢由 **Charlie_Ping “查理平”** 带来的BDX文件转换参考，以及MIDI-我的世界对应乐器参考表格
-- 感谢由 **[CMA_2401PT](https://github.com/CMA2401PT)** 为我们的软件开发的一些方面进行指导，同时我们参考了他的BDXworkshop作为BDX结构编辑的参考
-- 感谢由 **[Dislink Sforza](https://github.com/Dislink) “断联·斯福尔扎”**\<QQ1600515314\> 带来的midi音色解析以及转换指令的算法，我们将其改编并应用；同时，感谢他的[网页版转换器](https://dislink.github.io/midi2bdx/)给我们的开发与更新带来巨大的压力和动力，让我们在原本一骑绝尘的摸鱼道路上转向开发，希望他能考上一个理想的大学！
-- 感谢 **Touch “偷吃”**\<QQ1793537164\> 提供的BDX导入测试支持，并对程序的改进提供了丰富的意见；同时也感谢他的不断尝试新的内容，使我们的排错更进一步
-- 感谢 **Mono**\<QQ738893087\> 反馈安装时的问题，辅助我们找到了视窗操作系统下的兼容性问题；感谢其反馈延迟播放器出现的重大问题，让我们得以修改全部延迟播放错误
-- 感谢 **Ammelia “艾米利亚”**\<QQ2838334637\> 敦促我们进行新的功能开发，并为新功能提出了非常优秀的大量建议，以及提供的BDX导入测试支持，为我们的新结构生成算法提供了大量的实际理论支持
-- 感谢 **[神羽](https://gitee.com/snowykami) “[SnowyKami](https://github.com/snowyfirefly)”** 对我们项目的支持与宣传，希望他能考的一所优秀的大学！
-- 感谢 **指令师_苦力怕 playjuice123**\<QQ240667197\>为我们的程序找出错误，并提醒我们修复一个一直存在的大bug。
-- 感谢 **雷霆**\<QQ3555268519\>为我们的程序找出错误，并提醒修复bug。
+- 感谢 **昀梦**\<QQ1515399885\> 找出指令生成错误 bug 并指正
+- 感谢由 **Charlie_Ping “查理平”** 带来的 BDX 文件转换参考，以及 MIDI-我的世界对应乐器 参考表格
+- 感谢由 **[CMA_2401PT](https://github.com/CMA2401PT)** 为我们的软件开发的一些方面进行指导，同时我们参考了他的 BDXworkshop 作为 BDX 结构编辑的参考
+- 感谢由 **[Dislink Sforza](https://github.com/Dislink) “断联·斯福尔扎”**\<QQ1600515314\> 带来的 midi 音色解析以及转换指令的算法，我们将其改编并应用；同时，感谢他的[网页版转换器](https://dislink.github.io/midi2bdx/)给我们的开发与更新带来巨大的压力和动力，让我们在原本一骑绝尘的摸鱼道路上转向开发，希望他能考上一个理想的大学！
+- 感谢 **Touch “偷吃”**\<QQ1793537164\> 提供的 BDX 导入测试支持，并对程序的改进提供了丰富的意见；同时也感谢他的不断尝试新的内容，使我们的排错更进一步
+- 感谢 **Mono**\<QQ738893087\> 反馈安装时的问题，辅助我们找到了视窗操作系统下的兼容性问题；感谢其反馈延迟播放器出现的重大问题，让我们得以修改全部延迟播放错误；尤其感谢他对于我们的软件的大力宣传
+- 感谢 **Ammelia “艾米利亚”**\<QQ2838334637\> 敦促我们进行新的功能开发，并为新功能提出了非常优秀的大量建议，以及提供的 BDX 导入测试支持，为我们的新结构生成算法提供了大量的实际理论支持
+- 感谢 **[神羽](https://gitee.com/snowykami) “[SnowyKami](https://github.com/snowyfirefly)”** 对我们项目的支持与宣传，希望他能考得一所优秀的大学！
+- 感谢 **指令师\_苦力怕 playjuice123**\<QQ240667197\>为我们的程序找出错误，并提醒我们修复一个一直存在的大 bug。
+- 感谢 **雷霆**\<QQ3555268519\>用他那令所有开发者都大为光火的操作方法为我们的程序找出错误，并提醒修复 bug。
 
->	感谢广大群友为此程序提供的测试等支持
+>     感谢广大群友为此程序提供的测试等支持
 >
->	若您对我们有所贡献但您的名字没有显示在此列表中，请联系我们！
+>     若您对我们有所贡献但您的名字没有显示在此列表中，请联系我们！
 
-## 联系📞
+## 联系 📞
 
-若遇到库中的问题，欢迎在[此](https://gitee.com/TriM-Organization/Musicreater/issues/new)提出你的issue。
+若遇到库中的问题，欢迎在[此](https://gitee.com/TriM-Organization/Musicreater/issues/new)提出你的 issue。
 
-如果需要与开发组进行交流，欢迎加入我们的[开发闲聊Q群](https://jq.qq.com/?_wv=1027&k=hpeRxrYr)。
+如果需要与开发组进行交流，欢迎加入我们的[开发闲聊 Q 群](https://jq.qq.com/?_wv=1027&k=hpeRxrYr)。
 
---------------------------------------------
+---
 
-此项目并非一个官方 《我的世界》（*Minecraft*）项目
+此项目并非一个官方 《我的世界》（_Minecraft_）项目
 
 此项目不隶属或关联于 Mojang Studios 或 微软
 
-此项目亦不与 网易 相关
+此项目亦不隶属或关联于 网易
 
 “Minecraft”是 Mojang Synergies AB 的商标，此项目中所有对于“我的世界”、“Minecraft”等相关称呼均为引用性使用
 
-* 上文提及的 网易 公司，指代的是在中国大陆运营《我的世界：中国版》的上海网之易网络科技发展有限公司
+- 上文提及的 网易 公司，指代的是在中国大陆运营《我的世界：中国版》的上海网之易网络科技发展有限公司
 
 NOT AN OFFICIAL MINECRAFT PRODUCT.
 
 NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR MICROSOFT.
 
-
-
-
+NOT APPROVED BY OR ASSOCIATED WITH NETEASE.
 
 [Bilibili: 金羿ELS]: https://img.shields.io/badge/Bilibili-%E5%87%8C%E4%BA%91%E9%87%91%E7%BE%BF-00A1E7?style=for-the-badge
 [Bilibili: 诸葛亮与八卦阵]: https://img.shields.io/badge/Bilibili-%E8%AF%B8%E8%91%9B%E4%BA%AE%E4%B8%8E%E5%85%AB%E5%8D%A6%E9%98%B5-00A1E7?style=for-the-badge
 [CodeStyle: black]: https://img.shields.io/badge/code%20style-black-121110.svg?style=for-the-badge
 [python]: https://img.shields.io/badge/python-3.8-AB70FF?style=for-the-badge
 [release]: https://img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
 [license]: https://img.shields.io/badge/Licence-Apache-228B22?style=for-the-badge
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Musicreater Version: 0.5.1 Summary:
+Metadata-Version: 2.1 Name: Musicreater Version: 1.0.0 Summary:
 ä¸æ¬¾åè´¹å¼æºç ãæçä¸çã midé³ä¹è½¬æ¢åºã Home-page:
 https://github.com/TriM-Organization/Musicreater Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: Chinese (Simplified) Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python Classifier: Programming Language ::
@@ -10,89 +10,93 @@
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Description-Content-Type: text/markdown
 License-File: LICENSE.md
                       ****** é³Â·å Musicreater ******
     [https://gitee.com/TriM-Organization/Musicreater/raw/master/resources/
                                 msctIcon.ico]
-   **** ä¸æ¬¾åè´¹å¼æºç ãæçä¸çã MIDIé³ä¹è½¬æ¢åºã ****
+   **** ä¸æ¬¾åè´¹å¼æºçãæçä¸çãæ°å­é³é¢è½¬æ¢åºã ****
 [https://forthebadge.com/images/badges/built-with-love.svg] [Fork_me_on_Gitee]_
 [![][Bilibili: éç¾¿ELS]](https://space.bilibili.com/397369002/) [![]
 [Bilibili: è¯¸èäº®ä¸å«å¦éµ]](https://space.bilibili.com/604072474) [!
 [CodeStyle: black]](https://github.com/psf/black) [![][python]](https://
 www.python.org/) [![][license]](LICENSE) [![][release]](../../releases) [!
 [GiteeStar](https://gitee.com/TriM-Organization/Musicreater/badge/
 star.svg?theme=gray)](https://gitee.com/TriM-Organization/Musicreater/
 stargazers) [![GiteeFork](https://gitee.com/TriM-Organization/Musicreater/
 badge/fork.svg?theme=gray)](https://gitee.com/TriM-Organization/Musicreater/
 members) [![GitHub Repo stars](https://img.shields.io/github/stars/TriM-
 Organization/Musicreater?color=white&logo=GitHub&style=plastic)](https://
 github.com/TriM-Organization/Musicreater/stargazers) [![GitHub Repo Forks]
 (https://img.shields.io/github/forks/TriM-Organization/
 Musicreater?color=white&logo=GitHub&style=plastic)](https://github.com/TriM-
-Organization/Musicreater/forks) ç®ä½ä¸­æð¨ð³ | [Englishð¬ð§]
-(README_EN.md) ## ä»ç»ð é³Â·å æ¯ä¸ä¸ªåè´¹å¼æºçéå¯¹
-**ãæçä¸çã** çMIDIé³ä¹è½¬æ¢åº æ¬¢è¿å ç¾¤ï¼[861684859](https:
-//jq.qq.com/?_wv=1027&k=hpeRxrYr) ## ä¸è½½å®è£ - ä½¿ç¨pypi ```bash pip
-install Musicreater ``` - å¦æåºç°éè¯¯ï¼å¯ä»¥å°è¯ï¼ ```bash pip
-install -i https://pypi.python.org/simple Musicreater ``` -
-ï¼å¯¹äºå¼åèæ¥è¯´ï¼åçº§ï¼ ```bash pip install -i https://
-pypi.python.org/simple Musicreater --upgrade ``` - åéä»åºå¹¶å®è£
-```bash git clone https://gitee.com/TriM-Organization/Musicreater.git cd
-Musicreater python setup.py install ``` ä»¥ä¸å½ä»¤ç§ `python`ã`pip`
+Organization/Musicreater/forks) ç®ä½ä¸­æ ð¨ð³ | [Englishð¬ð§]
+(README_EN.md) ## ä»ç» ð é³Â·å æ¯ä¸ä¸ªåè´¹å¼æºçéå¯¹
+**ãæçä¸çã** ç MIDI é³ä¹è½¬æ¢åº æ¬¢è¿å ç¾¤ï¼[861684859]
+(https://jq.qq.com/?_wv=1027&k=hpeRxrYr) ## å®è£ ð³ - ä½¿ç¨ pypi ```bash
+pip install Musicreater ``` - å¦æåºç°éè¯¯ï¼å¯ä»¥å°è¯ï¼ ```bash pip
+install -i https://pypi.python.org/simple Musicreater ``` - åçº§ï¼ ```bash
+pip install -i https://pypi.python.org/simple Musicreater --upgrade ``` -
+åéä»åºå¹¶å®è£ ```bash git clone https://gitee.com/TriM-Organization/
+Musicreater.git cd Musicreater python setup.py install ``` ä»¥ä¸å½ä»¤ä¸­
+`python`ã`pip`
 è¯·ä¾ç§åä¸ªç¯å¢ä¸åçµæ´»æ´æ¢ï¼å¯è½ä¸º`python3`æ`pip3`ä¹ç±»ã
-## ææ¡£ð [çææä»¶çä½¿ç¨](https://github.com/TriM-Organization/
+## ææ¡£ ð [çææä»¶çä½¿ç¨](https://github.com/TriM-Organization/
 Musicreater/blob/master/docs/
 %E7%94%9F%E6%88%90%E6%96%87%E4%BB%B6%E7%9A%84%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E.md)
-[ä»åºAPIææ¡£](https://github.com/TriM-Organization/Musicreater/blob/master/
-docs/
+[ä»åº API ææ¡£](https://github.com/TriM-Organization/Musicreater/blob/
+master/docs/
 %E5%BA%93%E7%9A%84%E7%94%9F%E6%88%90%E4%B8%8E%E5%8A%9F%E8%83%BD%E6%96%87%E6%A1%A3.md)
-## ä½èâ éç¾¿
-Eillesï¼æçä¸çåºå²©çæä»¤å¸ï¼ä¸ªäººå¼åèï¼Bç«ä¸ç¥åUPä¸»ï¼æ±è¥¿å¨æ ¡é«ä¸­çã
-è¯¸èäº®ä¸å«å¦éµ
+## ä½è â éç¾¿
+Eillesï¼æçä¸çåºå²©çæä»¤å¸ï¼ä¸ªäººå¼åèï¼B ç«ä¸ç¥å UP
+ä¸»ï¼æ±è¥¿å¨æ ¡é«ä¸­çã è¯¸èäº®ä¸å«å¦éµ
 bgArrayï¼æçä¸çåºå²©çç©å®¶ï¼åæ¬¢ç¼ç¨åé³ä¹ï¼æ·±å³åäºå­¦çã
-## è´è°¢ð æ¬è´è°¢åè¡¨æåæ é¡ºåºã - æè°¢ **ææ¢¦**\>
-æ¾åºæä»¤çæéè¯¯bugå¹¶ææ­£ - æè°¢ç± **Charlie_Ping
-âæ¥çå¹³â** å¸¦æ¥çBDXæä»¶è½¬æ¢åèï¼ä»¥åMIDI-
-æçä¸çå¯¹åºä¹å¨åèè¡¨æ ¼ - æè°¢ç± **[CMA_2401PT](https://
+## è´è°¢ ð æ¬è´è°¢åè¡¨æåæ é¡ºåºã - æè°¢ **ææ¢¦**\>
+æ¾åºæä»¤çæéè¯¯ bug å¹¶ææ­£ - æè°¢ç± **Charlie_Ping
+âæ¥çå¹³â** å¸¦æ¥ç BDX æä»¶è½¬æ¢åèï¼ä»¥å MIDI-
+æçä¸çå¯¹åºä¹å¨ åèè¡¨æ ¼ - æè°¢ç± **[CMA_2401PT](https://
 github.com/CMA2401PT)**
-ä¸ºæä»¬çè½¯ä»¶å¼åçä¸äºæ¹é¢è¿è¡æå¯¼ï¼åæ¶æä»¬åèäºä»çBDXworkshopä½ä¸ºBDXç»æç¼è¾çåè
-- æè°¢ç± **[Dislink Sforza](https://github.com/Dislink)
-âæ­èÂ·æ¯ç¦å°æâ**\>
-å¸¦æ¥çmidié³è²è§£æä»¥åè½¬æ¢æä»¤çç®æ³ï¼æä»¬å°å¶æ¹ç¼å¹¶åºç¨ï¼åæ¶ï¼æè°¢ä»ç
+ä¸ºæä»¬çè½¯ä»¶å¼åçä¸äºæ¹é¢è¿è¡æå¯¼ï¼åæ¶æä»¬åèäºä»ç
+BDXworkshop ä½ä¸º BDX ç»æç¼è¾çåè - æè°¢ç± **[Dislink Sforza]
+(https://github.com/Dislink) âæ­èÂ·æ¯ç¦å°æâ**\> å¸¦æ¥ç midi
+é³è²è§£æä»¥åè½¬æ¢æä»¤çç®æ³ï¼æä»¬å°å¶æ¹ç¼å¹¶åºç¨ï¼åæ¶ï¼æè°¢ä»ç
 [ç½é¡µçè½¬æ¢å¨](https://dislink.github.io/midi2bdx/
 )ç»æä»¬çå¼åä¸æ´æ°å¸¦æ¥å·¨å¤§çåååå¨åï¼è®©æä»¬å¨åæ¬ä¸éªç»å°çæ¸é±¼éè·¯ä¸è½¬åå¼åï¼å¸æä»è½èä¸ä¸ä¸ªçæ³çå¤§å­¦ï¼
-- æè°¢ **Touch âå·åâ**\>
-æä¾çBDXå¯¼å¥æµè¯æ¯æï¼å¹¶å¯¹ç¨åºçæ¹è¿æä¾äºä¸°å¯çæè§ï¼åæ¶ä¹æè°¢ä»çä¸æ­å°è¯æ°çåå®¹ï¼ä½¿æä»¬çæéæ´è¿ä¸æ­¥
+- æè°¢ **Touch âå·åâ**\> æä¾ç BDX
+å¯¼å¥æµè¯æ¯æï¼å¹¶å¯¹ç¨åºçæ¹è¿æä¾äºä¸°å¯çæè§ï¼åæ¶ä¹æè°¢ä»çä¸æ­å°è¯æ°çåå®¹ï¼ä½¿æä»¬çæéæ´è¿ä¸æ­¥
 - æè°¢ **Mono**\>
-åé¦å®è£æ¶çé®é¢ï¼è¾å©æä»¬æ¾å°äºè§çªæä½ç³»ç»ä¸çå¼å®¹æ§é®é¢ï¼æè°¢å¶åé¦å»¶è¿æ­æ¾å¨åºç°çéå¤§é®é¢ï¼è®©æä»¬å¾ä»¥ä¿®æ¹å¨é¨å»¶è¿æ­æ¾éè¯¯
+åé¦å®è£æ¶çé®é¢ï¼è¾å©æä»¬æ¾å°äºè§çªæä½ç³»ç»ä¸çå¼å®¹æ§é®é¢ï¼æè°¢å¶åé¦å»¶è¿æ­æ¾å¨åºç°çéå¤§é®é¢ï¼è®©æä»¬å¾ä»¥ä¿®æ¹å¨é¨å»¶è¿æ­æ¾éè¯¯ï¼å°¤å¶æè°¢ä»å¯¹äºæä»¬çè½¯ä»¶çå¤§åå®£ä¼ 
 - æè°¢ **Ammelia âè¾ç±³å©äºâ**\>
-æ¦ä¿æä»¬è¿è¡æ°çåè½å¼åï¼å¹¶ä¸ºæ°åè½æåºäºéå¸¸ä¼ç§çå¤§éå»ºè®®ï¼ä»¥åæä¾çBDXå¯¼å¥æµè¯æ¯æï¼ä¸ºæä»¬çæ°ç»æçæç®æ³æä¾äºå¤§éçå®éçè®ºæ¯æ
+æ¦ä¿æä»¬è¿è¡æ°çåè½å¼åï¼å¹¶ä¸ºæ°åè½æåºäºéå¸¸ä¼ç§çå¤§éå»ºè®®ï¼ä»¥åæä¾ç
+BDX
+å¯¼å¥æµè¯æ¯æï¼ä¸ºæä»¬çæ°ç»æçæç®æ³æä¾äºå¤§éçå®éçè®ºæ¯æ
 - æè°¢ **[ç¥ç¾½](https://gitee.com/snowykami) â[SnowyKami](https://
 github.com/snowyfirefly)â**
-å¯¹æä»¬é¡¹ç®çæ¯æä¸å®£ä¼ ï¼å¸æä»è½èçä¸æä¼ç§çå¤§å­¦ï¼
-- æè°¢ **æä»¤å¸_è¦åæ
-playjuice123**\>ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéæä»¬ä¿®å¤ä¸ä¸ªä¸ç´å­å¨çå¤§bugã
-- æè°¢ **é·é**\>ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéä¿®å¤bugã >
-æè°¢å¹¿å¤§ç¾¤åä¸ºæ­¤ç¨åºæä¾çæµè¯ç­æ¯æ > >
+å¯¹æä»¬é¡¹ç®çæ¯æä¸å®£ä¼ ï¼å¸æä»è½èå¾ä¸æä¼ç§çå¤§å­¦ï¼
+- æè°¢ **æä»¤å¸\_è¦åæ
+playjuice123**\>ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéæä»¬ä¿®å¤ä¸ä¸ªä¸ç´å­å¨çå¤§
+bugã - æè°¢
+**é·é**\>ç¨ä»é£ä»¤ææå¼åèé½å¤§ä¸ºåç«çæä½æ¹æ³ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéä¿®å¤
+bugã > æè°¢å¹¿å¤§ç¾¤åä¸ºæ­¤ç¨åºæä¾çæµè¯ç­æ¯æ > >
 è¥æ¨å¯¹æä»¬ææè´¡ç®ä½æ¨çåå­æ²¡ææ¾ç¤ºå¨æ­¤åè¡¨ä¸­ï¼è¯·èç³»æä»¬ï¼
-## èç³»ð è¥éå°åºä¸­çé®é¢ï¼æ¬¢è¿å¨[æ­¤](https://gitee.com/TriM-
-Organization/Musicreater/issues/new)æåºä½ çissueã
-å¦æéè¦ä¸å¼åç»è¿è¡äº¤æµï¼æ¬¢è¿å å¥æä»¬ç[å¼åé²èQç¾¤]
-(https://jq.qq.com/?_wv=1027&k=hpeRxrYr)ã -----------------------------------
---------- æ­¤é¡¹ç®å¹¶éä¸ä¸ªå®æ¹ ãæçä¸çãï¼*Minecraft*ï¼é¡¹ç®
-æ­¤é¡¹ç®ä¸é¶å±æå³èäº Mojang Studios æ å¾®è½¯ æ­¤é¡¹ç®äº¦ä¸ä¸
-ç½æ ç¸å³ âMinecraftâæ¯ Mojang Synergies AB
+## èç³» ð è¥éå°åºä¸­çé®é¢ï¼æ¬¢è¿å¨[æ­¤](https://gitee.com/
+TriM-Organization/Musicreater/issues/new)æåºä½ ç issueã
+å¦æéè¦ä¸å¼åç»è¿è¡äº¤æµï¼æ¬¢è¿å å¥æä»¬ç[å¼åé²è Q
+ç¾¤](https://jq.qq.com/?_wv=1027&k=hpeRxrYr)ã --- æ­¤é¡¹ç®å¹¶éä¸ä¸ªå®æ¹
+ãæçä¸çãï¼_Minecraft_ï¼é¡¹ç® æ­¤é¡¹ç®ä¸é¶å±æå³èäº Mojang
+Studios æ å¾®è½¯ æ­¤é¡¹ç®äº¦ä¸é¶å±æå³èäº ç½æ âMinecraftâæ¯
+Mojang Synergies AB
 çåæ ï¼æ­¤é¡¹ç®ä¸­ææå¯¹äºâæçä¸çâãâMinecraftâç­ç¸å³ç§°å¼åä¸ºå¼ç¨æ§ä½¿ç¨
-* ä¸ææåç ç½æ
+- ä¸ææåç ç½æ
 å¬å¸ï¼æä»£çæ¯å¨ä¸­å½å¤§éè¿è¥ãæçä¸çï¼ä¸­å½çãçä¸æµ·ç½ä¹æç½ç»ç§æåå±æéå¬å¸
 NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR
-MICROSOFT. [Bilibili: éç¾¿ELS]: https://img.shields.io/badge/Bilibili-
-%E5%87%8C%E4%BA%91%E9%87%91%E7%BE%BF-00A1E7?style=for-the-badge [Bilibili:
-è¯¸èäº®ä¸å«å¦éµ]: https://img.shields.io/badge/Bilibili-
+MICROSOFT. NOT APPROVED BY OR ASSOCIATED WITH NETEASE. [Bilibili: éç¾¿ELS]:
+https://img.shields.io/badge/Bilibili-%E5%87%8C%E4%BA%91%E9%87%91%E7%BE%BF-
+00A1E7?style=for-the-badge [Bilibili: è¯¸èäº®ä¸å«å¦éµ]: https://
+img.shields.io/badge/Bilibili-
 %E8%AF%B8%E8%91%9B%E4%BA%AE%E4%B8%8E%E5%85%AB%E5%8D%A6%E9%98%B5-
 00A1E7?style=for-the-badge [CodeStyle: black]: https://img.shields.io/badge/
 code%20style-black-121110.svg?style=for-the-badge [python]: https://
 img.shields.io/badge/python-3.8-AB70FF?style=for-the-badge [release]: https://
 img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
 [license]: https://img.shields.io/badge/Licence-Apache-228B22?style=for-the-
 badge
```

### Comparing `Musicreater-0.5.1/PKG-INFO` & `Musicreater-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Musicreater
-Version: 0.5.1
+Version: 1.0.0
 Summary: 一款免费开源的 《我的世界》 mid音乐转换库。
 Home-page: https://github.com/TriM-Organization/Musicreater
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,140 +16,135 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-
 <h1 align="center">
     音·创 Musicreater
 </h1>
 
 <p align="center">
     <img width="128" height="128" src="https://gitee.com/TriM-Organization/Musicreater/raw/master/resources/msctIcon.ico">
     </img>
 </p>
 
-<h3 align="center">一款免费开源的 《我的世界》 MIDI音乐转换库。</h3>
+<h3 align="center">一款免费开源的《我的世界》数字音频转换库。</h3>
 
 <p align="center">
     <img src="https://forthebadge.com/images/badges/built-with-love.svg">
     <a href='https://gitee.com/TriM-Organization/Musicreater'>
         <img align="right" src='https://gitee.com/TriM-Organization/Musicreater/widgets/widget_1.svg' alt='Fork me on Gitee'>
         </img>
     </a>
 <p>
 
-
-
-
-
 [![][Bilibili: 金羿ELS]](https://space.bilibili.com/397369002/)
-[![][Bilibili: 诸葛亮与八卦阵]](https://space.bilibili.com/604072474) 
+[![][Bilibili: 诸葛亮与八卦阵]](https://space.bilibili.com/604072474)
 [![CodeStyle: black]](https://github.com/psf/black)
 [![][python]](https://www.python.org/)
 [![][license]](LICENSE)
 [![][release]](../../releases)
 
 [![GiteeStar](https://gitee.com/TriM-Organization/Musicreater/badge/star.svg?theme=gray)](https://gitee.com/TriM-Organization/Musicreater/stargazers)
 [![GiteeFork](https://gitee.com/TriM-Organization/Musicreater/badge/fork.svg?theme=gray)](https://gitee.com/TriM-Organization/Musicreater/members)
 [![GitHub Repo stars](https://img.shields.io/github/stars/TriM-Organization/Musicreater?color=white&logo=GitHub&style=plastic)](https://github.com/TriM-Organization/Musicreater/stargazers)
 [![GitHub Repo Forks](https://img.shields.io/github/forks/TriM-Organization/Musicreater?color=white&logo=GitHub&style=plastic)](https://github.com/TriM-Organization/Musicreater/forks)
 
+简体中文 🇨🇳 | [English🇬🇧](README_EN.md)
 
-简体中文🇨🇳 | [English🇬🇧](README_EN.md)
-
+## 介绍 🚀
 
-## 介绍🚀
-
-音·创 是一个免费开源的针对 **《我的世界》** 的MIDI音乐转换库
+音·创 是一个免费开源的针对 **《我的世界》** 的 MIDI 音乐转换库
 
 欢迎加群：[861684859](https://jq.qq.com/?_wv=1027&k=hpeRxrYr)
 
-## 下载安装
+## 安装 🔳
+
+- 使用 pypi
 
-- 使用pypi
-    ```bash
-    pip install Musicreater
-    ```
+  ```bash
+  pip install Musicreater
+  ```
 
 - 如果出现错误，可以尝试：
-    ```bash
-    pip install -i https://pypi.python.org/simple Musicreater
-    ```
-- （对于开发者来说）升级：
-    ```bash
-    pip install -i https://pypi.python.org/simple Musicreater --upgrade
-    ```
+  ```bash
+  pip install -i https://pypi.python.org/simple Musicreater
+  ```
+
+- 升级：
+
+  ```bash
+  pip install -i https://pypi.python.org/simple Musicreater --upgrade
+  ```
 
 - 克隆仓库并安装
-    ```bash
-    git clone https://gitee.com/TriM-Organization/Musicreater.git
-    cd Musicreater
-    python setup.py install
-    ```
+  ```bash
+  git clone https://gitee.com/TriM-Organization/Musicreater.git
+  cd Musicreater
+  python setup.py install
+  ```
 
-以上命令种 `python`、`pip` 请依照各个环境不同灵活更换，可能为`python3`或`pip3`之类。
+以上命令中 `python`、`pip` 请依照各个环境不同灵活更换，可能为`python3`或`pip3`之类。
 
-## 文档📄
+## 文档 📄
 
 [生成文件的使用](https://github.com/TriM-Organization/Musicreater/blob/master/docs/%E7%94%9F%E6%88%90%E6%96%87%E4%BB%B6%E7%9A%84%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E.md)
 
-[仓库API文档](https://github.com/TriM-Organization/Musicreater/blob/master/docs/%E5%BA%93%E7%9A%84%E7%94%9F%E6%88%90%E4%B8%8E%E5%8A%9F%E8%83%BD%E6%96%87%E6%A1%A3.md)
+[仓库 API 文档](https://github.com/TriM-Organization/Musicreater/blob/master/docs/%E5%BA%93%E7%9A%84%E7%94%9F%E6%88%90%E4%B8%8E%E5%8A%9F%E8%83%BD%E6%96%87%E6%A1%A3.md)
 
-## 作者✒
+## 作者 ✒
 
-金羿 Eilles：我的世界基岩版指令师，个人开发者，B站不知名UP主，江西在校高中生。
+金羿 Eilles：我的世界基岩版指令师，个人开发者，B 站不知名 UP 主，江西在校高中生。
 
 诸葛亮与八卦阵 bgArray：我的世界基岩版玩家，喜欢编程和音乐，深圳初二学生。
 
-## 致谢🙏
+## 致谢 🙏
+
 本致谢列表排名无顺序。
 
-- 感谢 **昀梦**\<QQ1515399885\> 找出指令生成错误bug并指正
-- 感谢由 **Charlie_Ping “查理平”** 带来的BDX文件转换参考，以及MIDI-我的世界对应乐器参考表格
-- 感谢由 **[CMA_2401PT](https://github.com/CMA2401PT)** 为我们的软件开发的一些方面进行指导，同时我们参考了他的BDXworkshop作为BDX结构编辑的参考
-- 感谢由 **[Dislink Sforza](https://github.com/Dislink) “断联·斯福尔扎”**\<QQ1600515314\> 带来的midi音色解析以及转换指令的算法，我们将其改编并应用；同时，感谢他的[网页版转换器](https://dislink.github.io/midi2bdx/)给我们的开发与更新带来巨大的压力和动力，让我们在原本一骑绝尘的摸鱼道路上转向开发，希望他能考上一个理想的大学！
-- 感谢 **Touch “偷吃”**\<QQ1793537164\> 提供的BDX导入测试支持，并对程序的改进提供了丰富的意见；同时也感谢他的不断尝试新的内容，使我们的排错更进一步
-- 感谢 **Mono**\<QQ738893087\> 反馈安装时的问题，辅助我们找到了视窗操作系统下的兼容性问题；感谢其反馈延迟播放器出现的重大问题，让我们得以修改全部延迟播放错误
-- 感谢 **Ammelia “艾米利亚”**\<QQ2838334637\> 敦促我们进行新的功能开发，并为新功能提出了非常优秀的大量建议，以及提供的BDX导入测试支持，为我们的新结构生成算法提供了大量的实际理论支持
-- 感谢 **[神羽](https://gitee.com/snowykami) “[SnowyKami](https://github.com/snowyfirefly)”** 对我们项目的支持与宣传，希望他能考的一所优秀的大学！
-- 感谢 **指令师_苦力怕 playjuice123**\<QQ240667197\>为我们的程序找出错误，并提醒我们修复一个一直存在的大bug。
-- 感谢 **雷霆**\<QQ3555268519\>为我们的程序找出错误，并提醒修复bug。
+- 感谢 **昀梦**\<QQ1515399885\> 找出指令生成错误 bug 并指正
+- 感谢由 **Charlie_Ping “查理平”** 带来的 BDX 文件转换参考，以及 MIDI-我的世界对应乐器 参考表格
+- 感谢由 **[CMA_2401PT](https://github.com/CMA2401PT)** 为我们的软件开发的一些方面进行指导，同时我们参考了他的 BDXworkshop 作为 BDX 结构编辑的参考
+- 感谢由 **[Dislink Sforza](https://github.com/Dislink) “断联·斯福尔扎”**\<QQ1600515314\> 带来的 midi 音色解析以及转换指令的算法，我们将其改编并应用；同时，感谢他的[网页版转换器](https://dislink.github.io/midi2bdx/)给我们的开发与更新带来巨大的压力和动力，让我们在原本一骑绝尘的摸鱼道路上转向开发，希望他能考上一个理想的大学！
+- 感谢 **Touch “偷吃”**\<QQ1793537164\> 提供的 BDX 导入测试支持，并对程序的改进提供了丰富的意见；同时也感谢他的不断尝试新的内容，使我们的排错更进一步
+- 感谢 **Mono**\<QQ738893087\> 反馈安装时的问题，辅助我们找到了视窗操作系统下的兼容性问题；感谢其反馈延迟播放器出现的重大问题，让我们得以修改全部延迟播放错误；尤其感谢他对于我们的软件的大力宣传
+- 感谢 **Ammelia “艾米利亚”**\<QQ2838334637\> 敦促我们进行新的功能开发，并为新功能提出了非常优秀的大量建议，以及提供的 BDX 导入测试支持，为我们的新结构生成算法提供了大量的实际理论支持
+- 感谢 **[神羽](https://gitee.com/snowykami) “[SnowyKami](https://github.com/snowyfirefly)”** 对我们项目的支持与宣传，希望他能考得一所优秀的大学！
+- 感谢 **指令师\_苦力怕 playjuice123**\<QQ240667197\>为我们的程序找出错误，并提醒我们修复一个一直存在的大 bug。
+- 感谢 **雷霆**\<QQ3555268519\>用他那令所有开发者都大为光火的操作方法为我们的程序找出错误，并提醒修复 bug。
 
->	感谢广大群友为此程序提供的测试等支持
+>     感谢广大群友为此程序提供的测试等支持
 >
->	若您对我们有所贡献但您的名字没有显示在此列表中，请联系我们！
+>     若您对我们有所贡献但您的名字没有显示在此列表中，请联系我们！
 
-## 联系📞
+## 联系 📞
 
-若遇到库中的问题，欢迎在[此](https://gitee.com/TriM-Organization/Musicreater/issues/new)提出你的issue。
+若遇到库中的问题，欢迎在[此](https://gitee.com/TriM-Organization/Musicreater/issues/new)提出你的 issue。
 
-如果需要与开发组进行交流，欢迎加入我们的[开发闲聊Q群](https://jq.qq.com/?_wv=1027&k=hpeRxrYr)。
+如果需要与开发组进行交流，欢迎加入我们的[开发闲聊 Q 群](https://jq.qq.com/?_wv=1027&k=hpeRxrYr)。
 
---------------------------------------------
+---
 
-此项目并非一个官方 《我的世界》（*Minecraft*）项目
+此项目并非一个官方 《我的世界》（_Minecraft_）项目
 
 此项目不隶属或关联于 Mojang Studios 或 微软
 
-此项目亦不与 网易 相关
+此项目亦不隶属或关联于 网易
 
 “Minecraft”是 Mojang Synergies AB 的商标，此项目中所有对于“我的世界”、“Minecraft”等相关称呼均为引用性使用
 
-* 上文提及的 网易 公司，指代的是在中国大陆运营《我的世界：中国版》的上海网之易网络科技发展有限公司
+- 上文提及的 网易 公司，指代的是在中国大陆运营《我的世界：中国版》的上海网之易网络科技发展有限公司
 
 NOT AN OFFICIAL MINECRAFT PRODUCT.
 
 NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR MICROSOFT.
 
-
-
-
+NOT APPROVED BY OR ASSOCIATED WITH NETEASE.
 
 [Bilibili: 金羿ELS]: https://img.shields.io/badge/Bilibili-%E5%87%8C%E4%BA%91%E9%87%91%E7%BE%BF-00A1E7?style=for-the-badge
 [Bilibili: 诸葛亮与八卦阵]: https://img.shields.io/badge/Bilibili-%E8%AF%B8%E8%91%9B%E4%BA%AE%E4%B8%8E%E5%85%AB%E5%8D%A6%E9%98%B5-00A1E7?style=for-the-badge
 [CodeStyle: black]: https://img.shields.io/badge/code%20style-black-121110.svg?style=for-the-badge
 [python]: https://img.shields.io/badge/python-3.8-AB70FF?style=for-the-badge
 [release]: https://img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
 [license]: https://img.shields.io/badge/Licence-Apache-228B22?style=for-the-badge
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Musicreater Version: 0.5.1 Summary:
+Metadata-Version: 2.1 Name: Musicreater Version: 1.0.0 Summary:
 ä¸æ¬¾åè´¹å¼æºç ãæçä¸çã midé³ä¹è½¬æ¢åºã Home-page:
 https://github.com/TriM-Organization/Musicreater Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: Chinese (Simplified) Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python Classifier: Programming Language ::
@@ -10,89 +10,93 @@
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Description-Content-Type: text/markdown
 License-File: LICENSE.md
                       ****** é³Â·å Musicreater ******
     [https://gitee.com/TriM-Organization/Musicreater/raw/master/resources/
                                 msctIcon.ico]
-   **** ä¸æ¬¾åè´¹å¼æºç ãæçä¸çã MIDIé³ä¹è½¬æ¢åºã ****
+   **** ä¸æ¬¾åè´¹å¼æºçãæçä¸çãæ°å­é³é¢è½¬æ¢åºã ****
 [https://forthebadge.com/images/badges/built-with-love.svg] [Fork_me_on_Gitee]_
 [![][Bilibili: éç¾¿ELS]](https://space.bilibili.com/397369002/) [![]
 [Bilibili: è¯¸èäº®ä¸å«å¦éµ]](https://space.bilibili.com/604072474) [!
 [CodeStyle: black]](https://github.com/psf/black) [![][python]](https://
 www.python.org/) [![][license]](LICENSE) [![][release]](../../releases) [!
 [GiteeStar](https://gitee.com/TriM-Organization/Musicreater/badge/
 star.svg?theme=gray)](https://gitee.com/TriM-Organization/Musicreater/
 stargazers) [![GiteeFork](https://gitee.com/TriM-Organization/Musicreater/
 badge/fork.svg?theme=gray)](https://gitee.com/TriM-Organization/Musicreater/
 members) [![GitHub Repo stars](https://img.shields.io/github/stars/TriM-
 Organization/Musicreater?color=white&logo=GitHub&style=plastic)](https://
 github.com/TriM-Organization/Musicreater/stargazers) [![GitHub Repo Forks]
 (https://img.shields.io/github/forks/TriM-Organization/
 Musicreater?color=white&logo=GitHub&style=plastic)](https://github.com/TriM-
-Organization/Musicreater/forks) ç®ä½ä¸­æð¨ð³ | [Englishð¬ð§]
-(README_EN.md) ## ä»ç»ð é³Â·å æ¯ä¸ä¸ªåè´¹å¼æºçéå¯¹
-**ãæçä¸çã** çMIDIé³ä¹è½¬æ¢åº æ¬¢è¿å ç¾¤ï¼[861684859](https:
-//jq.qq.com/?_wv=1027&k=hpeRxrYr) ## ä¸è½½å®è£ - ä½¿ç¨pypi ```bash pip
-install Musicreater ``` - å¦æåºç°éè¯¯ï¼å¯ä»¥å°è¯ï¼ ```bash pip
-install -i https://pypi.python.org/simple Musicreater ``` -
-ï¼å¯¹äºå¼åèæ¥è¯´ï¼åçº§ï¼ ```bash pip install -i https://
-pypi.python.org/simple Musicreater --upgrade ``` - åéä»åºå¹¶å®è£
-```bash git clone https://gitee.com/TriM-Organization/Musicreater.git cd
-Musicreater python setup.py install ``` ä»¥ä¸å½ä»¤ç§ `python`ã`pip`
+Organization/Musicreater/forks) ç®ä½ä¸­æ ð¨ð³ | [Englishð¬ð§]
+(README_EN.md) ## ä»ç» ð é³Â·å æ¯ä¸ä¸ªåè´¹å¼æºçéå¯¹
+**ãæçä¸çã** ç MIDI é³ä¹è½¬æ¢åº æ¬¢è¿å ç¾¤ï¼[861684859]
+(https://jq.qq.com/?_wv=1027&k=hpeRxrYr) ## å®è£ ð³ - ä½¿ç¨ pypi ```bash
+pip install Musicreater ``` - å¦æåºç°éè¯¯ï¼å¯ä»¥å°è¯ï¼ ```bash pip
+install -i https://pypi.python.org/simple Musicreater ``` - åçº§ï¼ ```bash
+pip install -i https://pypi.python.org/simple Musicreater --upgrade ``` -
+åéä»åºå¹¶å®è£ ```bash git clone https://gitee.com/TriM-Organization/
+Musicreater.git cd Musicreater python setup.py install ``` ä»¥ä¸å½ä»¤ä¸­
+`python`ã`pip`
 è¯·ä¾ç§åä¸ªç¯å¢ä¸åçµæ´»æ´æ¢ï¼å¯è½ä¸º`python3`æ`pip3`ä¹ç±»ã
-## ææ¡£ð [çææä»¶çä½¿ç¨](https://github.com/TriM-Organization/
+## ææ¡£ ð [çææä»¶çä½¿ç¨](https://github.com/TriM-Organization/
 Musicreater/blob/master/docs/
 %E7%94%9F%E6%88%90%E6%96%87%E4%BB%B6%E7%9A%84%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E.md)
-[ä»åºAPIææ¡£](https://github.com/TriM-Organization/Musicreater/blob/master/
-docs/
+[ä»åº API ææ¡£](https://github.com/TriM-Organization/Musicreater/blob/
+master/docs/
 %E5%BA%93%E7%9A%84%E7%94%9F%E6%88%90%E4%B8%8E%E5%8A%9F%E8%83%BD%E6%96%87%E6%A1%A3.md)
-## ä½èâ éç¾¿
-Eillesï¼æçä¸çåºå²©çæä»¤å¸ï¼ä¸ªäººå¼åèï¼Bç«ä¸ç¥åUPä¸»ï¼æ±è¥¿å¨æ ¡é«ä¸­çã
-è¯¸èäº®ä¸å«å¦éµ
+## ä½è â éç¾¿
+Eillesï¼æçä¸çåºå²©çæä»¤å¸ï¼ä¸ªäººå¼åèï¼B ç«ä¸ç¥å UP
+ä¸»ï¼æ±è¥¿å¨æ ¡é«ä¸­çã è¯¸èäº®ä¸å«å¦éµ
 bgArrayï¼æçä¸çåºå²©çç©å®¶ï¼åæ¬¢ç¼ç¨åé³ä¹ï¼æ·±å³åäºå­¦çã
-## è´è°¢ð æ¬è´è°¢åè¡¨æåæ é¡ºåºã - æè°¢ **ææ¢¦**\>
-æ¾åºæä»¤çæéè¯¯bugå¹¶ææ­£ - æè°¢ç± **Charlie_Ping
-âæ¥çå¹³â** å¸¦æ¥çBDXæä»¶è½¬æ¢åèï¼ä»¥åMIDI-
-æçä¸çå¯¹åºä¹å¨åèè¡¨æ ¼ - æè°¢ç± **[CMA_2401PT](https://
+## è´è°¢ ð æ¬è´è°¢åè¡¨æåæ é¡ºåºã - æè°¢ **ææ¢¦**\>
+æ¾åºæä»¤çæéè¯¯ bug å¹¶ææ­£ - æè°¢ç± **Charlie_Ping
+âæ¥çå¹³â** å¸¦æ¥ç BDX æä»¶è½¬æ¢åèï¼ä»¥å MIDI-
+æçä¸çå¯¹åºä¹å¨ åèè¡¨æ ¼ - æè°¢ç± **[CMA_2401PT](https://
 github.com/CMA2401PT)**
-ä¸ºæä»¬çè½¯ä»¶å¼åçä¸äºæ¹é¢è¿è¡æå¯¼ï¼åæ¶æä»¬åèäºä»çBDXworkshopä½ä¸ºBDXç»æç¼è¾çåè
-- æè°¢ç± **[Dislink Sforza](https://github.com/Dislink)
-âæ­èÂ·æ¯ç¦å°æâ**\>
-å¸¦æ¥çmidié³è²è§£æä»¥åè½¬æ¢æä»¤çç®æ³ï¼æä»¬å°å¶æ¹ç¼å¹¶åºç¨ï¼åæ¶ï¼æè°¢ä»ç
+ä¸ºæä»¬çè½¯ä»¶å¼åçä¸äºæ¹é¢è¿è¡æå¯¼ï¼åæ¶æä»¬åèäºä»ç
+BDXworkshop ä½ä¸º BDX ç»æç¼è¾çåè - æè°¢ç± **[Dislink Sforza]
+(https://github.com/Dislink) âæ­èÂ·æ¯ç¦å°æâ**\> å¸¦æ¥ç midi
+é³è²è§£æä»¥åè½¬æ¢æä»¤çç®æ³ï¼æä»¬å°å¶æ¹ç¼å¹¶åºç¨ï¼åæ¶ï¼æè°¢ä»ç
 [ç½é¡µçè½¬æ¢å¨](https://dislink.github.io/midi2bdx/
 )ç»æä»¬çå¼åä¸æ´æ°å¸¦æ¥å·¨å¤§çåååå¨åï¼è®©æä»¬å¨åæ¬ä¸éªç»å°çæ¸é±¼éè·¯ä¸è½¬åå¼åï¼å¸æä»è½èä¸ä¸ä¸ªçæ³çå¤§å­¦ï¼
-- æè°¢ **Touch âå·åâ**\>
-æä¾çBDXå¯¼å¥æµè¯æ¯æï¼å¹¶å¯¹ç¨åºçæ¹è¿æä¾äºä¸°å¯çæè§ï¼åæ¶ä¹æè°¢ä»çä¸æ­å°è¯æ°çåå®¹ï¼ä½¿æä»¬çæéæ´è¿ä¸æ­¥
+- æè°¢ **Touch âå·åâ**\> æä¾ç BDX
+å¯¼å¥æµè¯æ¯æï¼å¹¶å¯¹ç¨åºçæ¹è¿æä¾äºä¸°å¯çæè§ï¼åæ¶ä¹æè°¢ä»çä¸æ­å°è¯æ°çåå®¹ï¼ä½¿æä»¬çæéæ´è¿ä¸æ­¥
 - æè°¢ **Mono**\>
-åé¦å®è£æ¶çé®é¢ï¼è¾å©æä»¬æ¾å°äºè§çªæä½ç³»ç»ä¸çå¼å®¹æ§é®é¢ï¼æè°¢å¶åé¦å»¶è¿æ­æ¾å¨åºç°çéå¤§é®é¢ï¼è®©æä»¬å¾ä»¥ä¿®æ¹å¨é¨å»¶è¿æ­æ¾éè¯¯
+åé¦å®è£æ¶çé®é¢ï¼è¾å©æä»¬æ¾å°äºè§çªæä½ç³»ç»ä¸çå¼å®¹æ§é®é¢ï¼æè°¢å¶åé¦å»¶è¿æ­æ¾å¨åºç°çéå¤§é®é¢ï¼è®©æä»¬å¾ä»¥ä¿®æ¹å¨é¨å»¶è¿æ­æ¾éè¯¯ï¼å°¤å¶æè°¢ä»å¯¹äºæä»¬çè½¯ä»¶çå¤§åå®£ä¼ 
 - æè°¢ **Ammelia âè¾ç±³å©äºâ**\>
-æ¦ä¿æä»¬è¿è¡æ°çåè½å¼åï¼å¹¶ä¸ºæ°åè½æåºäºéå¸¸ä¼ç§çå¤§éå»ºè®®ï¼ä»¥åæä¾çBDXå¯¼å¥æµè¯æ¯æï¼ä¸ºæä»¬çæ°ç»æçæç®æ³æä¾äºå¤§éçå®éçè®ºæ¯æ
+æ¦ä¿æä»¬è¿è¡æ°çåè½å¼åï¼å¹¶ä¸ºæ°åè½æåºäºéå¸¸ä¼ç§çå¤§éå»ºè®®ï¼ä»¥åæä¾ç
+BDX
+å¯¼å¥æµè¯æ¯æï¼ä¸ºæä»¬çæ°ç»æçæç®æ³æä¾äºå¤§éçå®éçè®ºæ¯æ
 - æè°¢ **[ç¥ç¾½](https://gitee.com/snowykami) â[SnowyKami](https://
 github.com/snowyfirefly)â**
-å¯¹æä»¬é¡¹ç®çæ¯æä¸å®£ä¼ ï¼å¸æä»è½èçä¸æä¼ç§çå¤§å­¦ï¼
-- æè°¢ **æä»¤å¸_è¦åæ
-playjuice123**\>ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéæä»¬ä¿®å¤ä¸ä¸ªä¸ç´å­å¨çå¤§bugã
-- æè°¢ **é·é**\>ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéä¿®å¤bugã >
-æè°¢å¹¿å¤§ç¾¤åä¸ºæ­¤ç¨åºæä¾çæµè¯ç­æ¯æ > >
+å¯¹æä»¬é¡¹ç®çæ¯æä¸å®£ä¼ ï¼å¸æä»è½èå¾ä¸æä¼ç§çå¤§å­¦ï¼
+- æè°¢ **æä»¤å¸\_è¦åæ
+playjuice123**\>ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéæä»¬ä¿®å¤ä¸ä¸ªä¸ç´å­å¨çå¤§
+bugã - æè°¢
+**é·é**\>ç¨ä»é£ä»¤ææå¼åèé½å¤§ä¸ºåç«çæä½æ¹æ³ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéä¿®å¤
+bugã > æè°¢å¹¿å¤§ç¾¤åä¸ºæ­¤ç¨åºæä¾çæµè¯ç­æ¯æ > >
 è¥æ¨å¯¹æä»¬ææè´¡ç®ä½æ¨çåå­æ²¡ææ¾ç¤ºå¨æ­¤åè¡¨ä¸­ï¼è¯·èç³»æä»¬ï¼
-## èç³»ð è¥éå°åºä¸­çé®é¢ï¼æ¬¢è¿å¨[æ­¤](https://gitee.com/TriM-
-Organization/Musicreater/issues/new)æåºä½ çissueã
-å¦æéè¦ä¸å¼åç»è¿è¡äº¤æµï¼æ¬¢è¿å å¥æä»¬ç[å¼åé²èQç¾¤]
-(https://jq.qq.com/?_wv=1027&k=hpeRxrYr)ã -----------------------------------
---------- æ­¤é¡¹ç®å¹¶éä¸ä¸ªå®æ¹ ãæçä¸çãï¼*Minecraft*ï¼é¡¹ç®
-æ­¤é¡¹ç®ä¸é¶å±æå³èäº Mojang Studios æ å¾®è½¯ æ­¤é¡¹ç®äº¦ä¸ä¸
-ç½æ ç¸å³ âMinecraftâæ¯ Mojang Synergies AB
+## èç³» ð è¥éå°åºä¸­çé®é¢ï¼æ¬¢è¿å¨[æ­¤](https://gitee.com/
+TriM-Organization/Musicreater/issues/new)æåºä½ ç issueã
+å¦æéè¦ä¸å¼åç»è¿è¡äº¤æµï¼æ¬¢è¿å å¥æä»¬ç[å¼åé²è Q
+ç¾¤](https://jq.qq.com/?_wv=1027&k=hpeRxrYr)ã --- æ­¤é¡¹ç®å¹¶éä¸ä¸ªå®æ¹
+ãæçä¸çãï¼_Minecraft_ï¼é¡¹ç® æ­¤é¡¹ç®ä¸é¶å±æå³èäº Mojang
+Studios æ å¾®è½¯ æ­¤é¡¹ç®äº¦ä¸é¶å±æå³èäº ç½æ âMinecraftâæ¯
+Mojang Synergies AB
 çåæ ï¼æ­¤é¡¹ç®ä¸­ææå¯¹äºâæçä¸çâãâMinecraftâç­ç¸å³ç§°å¼åä¸ºå¼ç¨æ§ä½¿ç¨
-* ä¸ææåç ç½æ
+- ä¸ææåç ç½æ
 å¬å¸ï¼æä»£çæ¯å¨ä¸­å½å¤§éè¿è¥ãæçä¸çï¼ä¸­å½çãçä¸æµ·ç½ä¹æç½ç»ç§æåå±æéå¬å¸
 NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR
-MICROSOFT. [Bilibili: éç¾¿ELS]: https://img.shields.io/badge/Bilibili-
-%E5%87%8C%E4%BA%91%E9%87%91%E7%BE%BF-00A1E7?style=for-the-badge [Bilibili:
-è¯¸èäº®ä¸å«å¦éµ]: https://img.shields.io/badge/Bilibili-
+MICROSOFT. NOT APPROVED BY OR ASSOCIATED WITH NETEASE. [Bilibili: éç¾¿ELS]:
+https://img.shields.io/badge/Bilibili-%E5%87%8C%E4%BA%91%E9%87%91%E7%BE%BF-
+00A1E7?style=for-the-badge [Bilibili: è¯¸èäº®ä¸å«å¦éµ]: https://
+img.shields.io/badge/Bilibili-
 %E8%AF%B8%E8%91%9B%E4%BA%AE%E4%B8%8E%E5%85%AB%E5%8D%A6%E9%98%B5-
 00A1E7?style=for-the-badge [CodeStyle: black]: https://img.shields.io/badge/
 code%20style-black-121110.svg?style=for-the-badge [python]: https://
 img.shields.io/badge/python-3.8-AB70FF?style=for-the-badge [release]: https://
 img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
 [license]: https://img.shields.io/badge/Licence-Apache-228B22?style=for-the-
 badge
```

### Comparing `Musicreater-0.5.1/README.md` & `Musicreater-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,133 +1,128 @@
-
 <h1 align="center">
     音·创 Musicreater
 </h1>
 
 <p align="center">
     <img width="128" height="128" src="https://gitee.com/TriM-Organization/Musicreater/raw/master/resources/msctIcon.ico">
     </img>
 </p>
 
-<h3 align="center">一款免费开源的 《我的世界》 MIDI音乐转换库。</h3>
+<h3 align="center">一款免费开源的《我的世界》数字音频转换库。</h3>
 
 <p align="center">
     <img src="https://forthebadge.com/images/badges/built-with-love.svg">
     <a href='https://gitee.com/TriM-Organization/Musicreater'>
         <img align="right" src='https://gitee.com/TriM-Organization/Musicreater/widgets/widget_1.svg' alt='Fork me on Gitee'>
         </img>
     </a>
 <p>
 
-
-
-
-
 [![][Bilibili: 金羿ELS]](https://space.bilibili.com/397369002/)
-[![][Bilibili: 诸葛亮与八卦阵]](https://space.bilibili.com/604072474) 
+[![][Bilibili: 诸葛亮与八卦阵]](https://space.bilibili.com/604072474)
 [![CodeStyle: black]](https://github.com/psf/black)
 [![][python]](https://www.python.org/)
 [![][license]](LICENSE)
 [![][release]](../../releases)
 
 [![GiteeStar](https://gitee.com/TriM-Organization/Musicreater/badge/star.svg?theme=gray)](https://gitee.com/TriM-Organization/Musicreater/stargazers)
 [![GiteeFork](https://gitee.com/TriM-Organization/Musicreater/badge/fork.svg?theme=gray)](https://gitee.com/TriM-Organization/Musicreater/members)
 [![GitHub Repo stars](https://img.shields.io/github/stars/TriM-Organization/Musicreater?color=white&logo=GitHub&style=plastic)](https://github.com/TriM-Organization/Musicreater/stargazers)
 [![GitHub Repo Forks](https://img.shields.io/github/forks/TriM-Organization/Musicreater?color=white&logo=GitHub&style=plastic)](https://github.com/TriM-Organization/Musicreater/forks)
 
+简体中文 🇨🇳 | [English🇬🇧](README_EN.md)
 
-简体中文🇨🇳 | [English🇬🇧](README_EN.md)
-
+## 介绍 🚀
 
-## 介绍🚀
-
-音·创 是一个免费开源的针对 **《我的世界》** 的MIDI音乐转换库
+音·创 是一个免费开源的针对 **《我的世界》** 的 MIDI 音乐转换库
 
 欢迎加群：[861684859](https://jq.qq.com/?_wv=1027&k=hpeRxrYr)
 
-## 下载安装
+## 安装 🔳
+
+- 使用 pypi
 
-- 使用pypi
-    ```bash
-    pip install Musicreater
-    ```
+  ```bash
+  pip install Musicreater
+  ```
 
 - 如果出现错误，可以尝试：
-    ```bash
-    pip install -i https://pypi.python.org/simple Musicreater
-    ```
-- （对于开发者来说）升级：
-    ```bash
-    pip install -i https://pypi.python.org/simple Musicreater --upgrade
-    ```
+  ```bash
+  pip install -i https://pypi.python.org/simple Musicreater
+  ```
+
+- 升级：
+
+  ```bash
+  pip install -i https://pypi.python.org/simple Musicreater --upgrade
+  ```
 
 - 克隆仓库并安装
-    ```bash
-    git clone https://gitee.com/TriM-Organization/Musicreater.git
-    cd Musicreater
-    python setup.py install
-    ```
+  ```bash
+  git clone https://gitee.com/TriM-Organization/Musicreater.git
+  cd Musicreater
+  python setup.py install
+  ```
 
-以上命令种 `python`、`pip` 请依照各个环境不同灵活更换，可能为`python3`或`pip3`之类。
+以上命令中 `python`、`pip` 请依照各个环境不同灵活更换，可能为`python3`或`pip3`之类。
 
-## 文档📄
+## 文档 📄
 
 [生成文件的使用](./docs/%E7%94%9F%E6%88%90%E6%96%87%E4%BB%B6%E7%9A%84%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E.md)
 
-[仓库API文档](./docs/%E5%BA%93%E7%9A%84%E7%94%9F%E6%88%90%E4%B8%8E%E5%8A%9F%E8%83%BD%E6%96%87%E6%A1%A3.md)
+[仓库 API 文档](./docs/%E5%BA%93%E7%9A%84%E7%94%9F%E6%88%90%E4%B8%8E%E5%8A%9F%E8%83%BD%E6%96%87%E6%A1%A3.md)
 
-## 作者✒
+## 作者 ✒
 
-金羿 Eilles：我的世界基岩版指令师，个人开发者，B站不知名UP主，江西在校高中生。
+金羿 Eilles：我的世界基岩版指令师，个人开发者，B 站不知名 UP 主，江西在校高中生。
 
 诸葛亮与八卦阵 bgArray：我的世界基岩版玩家，喜欢编程和音乐，深圳初二学生。
 
-## 致谢🙏
+## 致谢 🙏
+
 本致谢列表排名无顺序。
 
-- 感谢 **昀梦**\<QQ1515399885\> 找出指令生成错误bug并指正
-- 感谢由 **Charlie_Ping “查理平”** 带来的BDX文件转换参考，以及MIDI-我的世界对应乐器参考表格
-- 感谢由 **[CMA_2401PT](https://github.com/CMA2401PT)** 为我们的软件开发的一些方面进行指导，同时我们参考了他的BDXworkshop作为BDX结构编辑的参考
-- 感谢由 **[Dislink Sforza](https://github.com/Dislink) “断联·斯福尔扎”**\<QQ1600515314\> 带来的midi音色解析以及转换指令的算法，我们将其改编并应用；同时，感谢他的[网页版转换器](https://dislink.github.io/midi2bdx/)给我们的开发与更新带来巨大的压力和动力，让我们在原本一骑绝尘的摸鱼道路上转向开发，希望他能考上一个理想的大学！
-- 感谢 **Touch “偷吃”**\<QQ1793537164\> 提供的BDX导入测试支持，并对程序的改进提供了丰富的意见；同时也感谢他的不断尝试新的内容，使我们的排错更进一步
-- 感谢 **Mono**\<QQ738893087\> 反馈安装时的问题，辅助我们找到了视窗操作系统下的兼容性问题；感谢其反馈延迟播放器出现的重大问题，让我们得以修改全部延迟播放错误
-- 感谢 **Ammelia “艾米利亚”**\<QQ2838334637\> 敦促我们进行新的功能开发，并为新功能提出了非常优秀的大量建议，以及提供的BDX导入测试支持，为我们的新结构生成算法提供了大量的实际理论支持
-- 感谢 **[神羽](https://gitee.com/snowykami) “[SnowyKami](https://github.com/snowyfirefly)”** 对我们项目的支持与宣传，希望他能考的一所优秀的大学！
-- 感谢 **指令师_苦力怕 playjuice123**\<QQ240667197\>为我们的程序找出错误，并提醒我们修复一个一直存在的大bug。
-- 感谢 **雷霆**\<QQ3555268519\>为我们的程序找出错误，并提醒修复bug。
+- 感谢 **昀梦**\<QQ1515399885\> 找出指令生成错误 bug 并指正
+- 感谢由 **Charlie_Ping “查理平”** 带来的 BDX 文件转换参考，以及 MIDI-我的世界对应乐器 参考表格
+- 感谢由 **[CMA_2401PT](https://github.com/CMA2401PT)** 为我们的软件开发的一些方面进行指导，同时我们参考了他的 BDXworkshop 作为 BDX 结构编辑的参考
+- 感谢由 **[Dislink Sforza](https://github.com/Dislink) “断联·斯福尔扎”**\<QQ1600515314\> 带来的 midi 音色解析以及转换指令的算法，我们将其改编并应用；同时，感谢他的[网页版转换器](https://dislink.github.io/midi2bdx/)给我们的开发与更新带来巨大的压力和动力，让我们在原本一骑绝尘的摸鱼道路上转向开发，希望他能考上一个理想的大学！
+- 感谢 **Touch “偷吃”**\<QQ1793537164\> 提供的 BDX 导入测试支持，并对程序的改进提供了丰富的意见；同时也感谢他的不断尝试新的内容，使我们的排错更进一步
+- 感谢 **Mono**\<QQ738893087\> 反馈安装时的问题，辅助我们找到了视窗操作系统下的兼容性问题；感谢其反馈延迟播放器出现的重大问题，让我们得以修改全部延迟播放错误；尤其感谢他对于我们的软件的大力宣传
+- 感谢 **Ammelia “艾米利亚”**\<QQ2838334637\> 敦促我们进行新的功能开发，并为新功能提出了非常优秀的大量建议，以及提供的 BDX 导入测试支持，为我们的新结构生成算法提供了大量的实际理论支持
+- 感谢 **[神羽](https://gitee.com/snowykami) “[SnowyKami](https://github.com/snowyfirefly)”** 对我们项目的支持与宣传，希望他能考得一所优秀的大学！
+- 感谢 **指令师\_苦力怕 playjuice123**\<QQ240667197\>为我们的程序找出错误，并提醒我们修复一个一直存在的大 bug。
+- 感谢 **雷霆**\<QQ3555268519\>用他那令所有开发者都大为光火的操作方法为我们的程序找出错误，并提醒修复 bug。
 
->	感谢广大群友为此程序提供的测试等支持
+>     感谢广大群友为此程序提供的测试等支持
 >
->	若您对我们有所贡献但您的名字没有显示在此列表中，请联系我们！
+>     若您对我们有所贡献但您的名字没有显示在此列表中，请联系我们！
 
-## 联系📞
+## 联系 📞
 
-若遇到库中的问题，欢迎在[此](https://gitee.com/TriM-Organization/Musicreater/issues/new)提出你的issue。
+若遇到库中的问题，欢迎在[此](https://gitee.com/TriM-Organization/Musicreater/issues/new)提出你的 issue。
 
-如果需要与开发组进行交流，欢迎加入我们的[开发闲聊Q群](https://jq.qq.com/?_wv=1027&k=hpeRxrYr)。
+如果需要与开发组进行交流，欢迎加入我们的[开发闲聊 Q 群](https://jq.qq.com/?_wv=1027&k=hpeRxrYr)。
 
---------------------------------------------
+---
 
-此项目并非一个官方 《我的世界》（*Minecraft*）项目
+此项目并非一个官方 《我的世界》（_Minecraft_）项目
 
 此项目不隶属或关联于 Mojang Studios 或 微软
 
-此项目亦不与 网易 相关
+此项目亦不隶属或关联于 网易
 
 “Minecraft”是 Mojang Synergies AB 的商标，此项目中所有对于“我的世界”、“Minecraft”等相关称呼均为引用性使用
 
-* 上文提及的 网易 公司，指代的是在中国大陆运营《我的世界：中国版》的上海网之易网络科技发展有限公司
+- 上文提及的 网易 公司，指代的是在中国大陆运营《我的世界：中国版》的上海网之易网络科技发展有限公司
 
 NOT AN OFFICIAL MINECRAFT PRODUCT.
 
 NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR MICROSOFT.
 
-
-
-
+NOT APPROVED BY OR ASSOCIATED WITH NETEASE.
 
 [Bilibili: 金羿ELS]: https://img.shields.io/badge/Bilibili-%E5%87%8C%E4%BA%91%E9%87%91%E7%BE%BF-00A1E7?style=for-the-badge
 [Bilibili: 诸葛亮与八卦阵]: https://img.shields.io/badge/Bilibili-%E8%AF%B8%E8%91%9B%E4%BA%AE%E4%B8%8E%E5%85%AB%E5%8D%A6%E9%98%B5-00A1E7?style=for-the-badge
 [CodeStyle: black]: https://img.shields.io/badge/code%20style-black-121110.svg?style=for-the-badge
 [python]: https://img.shields.io/badge/python-3.8-AB70FF?style=for-the-badge
 [release]: https://img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
 [license]: https://img.shields.io/badge/Licence-Apache-228B22?style=for-the-badge
```

#### html2text {}

```diff
@@ -1,83 +1,87 @@
                       ****** é³Â·å Musicreater ******
     [https://gitee.com/TriM-Organization/Musicreater/raw/master/resources/
                                 msctIcon.ico]
-   **** ä¸æ¬¾åè´¹å¼æºç ãæçä¸çã MIDIé³ä¹è½¬æ¢åºã ****
+   **** ä¸æ¬¾åè´¹å¼æºçãæçä¸çãæ°å­é³é¢è½¬æ¢åºã ****
 [https://forthebadge.com/images/badges/built-with-love.svg] [Fork_me_on_Gitee]_
 [![][Bilibili: éç¾¿ELS]](https://space.bilibili.com/397369002/) [![]
 [Bilibili: è¯¸èäº®ä¸å«å¦éµ]](https://space.bilibili.com/604072474) [!
 [CodeStyle: black]](https://github.com/psf/black) [![][python]](https://
 www.python.org/) [![][license]](LICENSE) [![][release]](../../releases) [!
 [GiteeStar](https://gitee.com/TriM-Organization/Musicreater/badge/
 star.svg?theme=gray)](https://gitee.com/TriM-Organization/Musicreater/
 stargazers) [![GiteeFork](https://gitee.com/TriM-Organization/Musicreater/
 badge/fork.svg?theme=gray)](https://gitee.com/TriM-Organization/Musicreater/
 members) [![GitHub Repo stars](https://img.shields.io/github/stars/TriM-
 Organization/Musicreater?color=white&logo=GitHub&style=plastic)](https://
 github.com/TriM-Organization/Musicreater/stargazers) [![GitHub Repo Forks]
 (https://img.shields.io/github/forks/TriM-Organization/
 Musicreater?color=white&logo=GitHub&style=plastic)](https://github.com/TriM-
-Organization/Musicreater/forks) ç®ä½ä¸­æð¨ð³ | [Englishð¬ð§]
-(README_EN.md) ## ä»ç»ð é³Â·å æ¯ä¸ä¸ªåè´¹å¼æºçéå¯¹
-**ãæçä¸çã** çMIDIé³ä¹è½¬æ¢åº æ¬¢è¿å ç¾¤ï¼[861684859](https:
-//jq.qq.com/?_wv=1027&k=hpeRxrYr) ## ä¸è½½å®è£ - ä½¿ç¨pypi ```bash pip
-install Musicreater ``` - å¦æåºç°éè¯¯ï¼å¯ä»¥å°è¯ï¼ ```bash pip
-install -i https://pypi.python.org/simple Musicreater ``` -
-ï¼å¯¹äºå¼åèæ¥è¯´ï¼åçº§ï¼ ```bash pip install -i https://
-pypi.python.org/simple Musicreater --upgrade ``` - åéä»åºå¹¶å®è£
-```bash git clone https://gitee.com/TriM-Organization/Musicreater.git cd
-Musicreater python setup.py install ``` ä»¥ä¸å½ä»¤ç§ `python`ã`pip`
+Organization/Musicreater/forks) ç®ä½ä¸­æ ð¨ð³ | [Englishð¬ð§]
+(README_EN.md) ## ä»ç» ð é³Â·å æ¯ä¸ä¸ªåè´¹å¼æºçéå¯¹
+**ãæçä¸çã** ç MIDI é³ä¹è½¬æ¢åº æ¬¢è¿å ç¾¤ï¼[861684859]
+(https://jq.qq.com/?_wv=1027&k=hpeRxrYr) ## å®è£ ð³ - ä½¿ç¨ pypi ```bash
+pip install Musicreater ``` - å¦æåºç°éè¯¯ï¼å¯ä»¥å°è¯ï¼ ```bash pip
+install -i https://pypi.python.org/simple Musicreater ``` - åçº§ï¼ ```bash
+pip install -i https://pypi.python.org/simple Musicreater --upgrade ``` -
+åéä»åºå¹¶å®è£ ```bash git clone https://gitee.com/TriM-Organization/
+Musicreater.git cd Musicreater python setup.py install ``` ä»¥ä¸å½ä»¤ä¸­
+`python`ã`pip`
 è¯·ä¾ç§åä¸ªç¯å¢ä¸åçµæ´»æ´æ¢ï¼å¯è½ä¸º`python3`æ`pip3`ä¹ç±»ã
-## ææ¡£ð [çææä»¶çä½¿ç¨](./docs/
+## ææ¡£ ð [çææä»¶çä½¿ç¨](./docs/
 %E7%94%9F%E6%88%90%E6%96%87%E4%BB%B6%E7%9A%84%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E.md)
-[ä»åºAPIææ¡£](./docs/
+[ä»åº API ææ¡£](./docs/
 %E5%BA%93%E7%9A%84%E7%94%9F%E6%88%90%E4%B8%8E%E5%8A%9F%E8%83%BD%E6%96%87%E6%A1%A3.md)
-## ä½èâ éç¾¿
-Eillesï¼æçä¸çåºå²©çæä»¤å¸ï¼ä¸ªäººå¼åèï¼Bç«ä¸ç¥åUPä¸»ï¼æ±è¥¿å¨æ ¡é«ä¸­çã
-è¯¸èäº®ä¸å«å¦éµ
+## ä½è â éç¾¿
+Eillesï¼æçä¸çåºå²©çæä»¤å¸ï¼ä¸ªäººå¼åèï¼B ç«ä¸ç¥å UP
+ä¸»ï¼æ±è¥¿å¨æ ¡é«ä¸­çã è¯¸èäº®ä¸å«å¦éµ
 bgArrayï¼æçä¸çåºå²©çç©å®¶ï¼åæ¬¢ç¼ç¨åé³ä¹ï¼æ·±å³åäºå­¦çã
-## è´è°¢ð æ¬è´è°¢åè¡¨æåæ é¡ºåºã - æè°¢ **ææ¢¦**\>
-æ¾åºæä»¤çæéè¯¯bugå¹¶ææ­£ - æè°¢ç± **Charlie_Ping
-âæ¥çå¹³â** å¸¦æ¥çBDXæä»¶è½¬æ¢åèï¼ä»¥åMIDI-
-æçä¸çå¯¹åºä¹å¨åèè¡¨æ ¼ - æè°¢ç± **[CMA_2401PT](https://
+## è´è°¢ ð æ¬è´è°¢åè¡¨æåæ é¡ºåºã - æè°¢ **ææ¢¦**\>
+æ¾åºæä»¤çæéè¯¯ bug å¹¶ææ­£ - æè°¢ç± **Charlie_Ping
+âæ¥çå¹³â** å¸¦æ¥ç BDX æä»¶è½¬æ¢åèï¼ä»¥å MIDI-
+æçä¸çå¯¹åºä¹å¨ åèè¡¨æ ¼ - æè°¢ç± **[CMA_2401PT](https://
 github.com/CMA2401PT)**
-ä¸ºæä»¬çè½¯ä»¶å¼åçä¸äºæ¹é¢è¿è¡æå¯¼ï¼åæ¶æä»¬åèäºä»çBDXworkshopä½ä¸ºBDXç»æç¼è¾çåè
-- æè°¢ç± **[Dislink Sforza](https://github.com/Dislink)
-âæ­èÂ·æ¯ç¦å°æâ**\>
-å¸¦æ¥çmidié³è²è§£æä»¥åè½¬æ¢æä»¤çç®æ³ï¼æä»¬å°å¶æ¹ç¼å¹¶åºç¨ï¼åæ¶ï¼æè°¢ä»ç
+ä¸ºæä»¬çè½¯ä»¶å¼åçä¸äºæ¹é¢è¿è¡æå¯¼ï¼åæ¶æä»¬åèäºä»ç
+BDXworkshop ä½ä¸º BDX ç»æç¼è¾çåè - æè°¢ç± **[Dislink Sforza]
+(https://github.com/Dislink) âæ­èÂ·æ¯ç¦å°æâ**\> å¸¦æ¥ç midi
+é³è²è§£æä»¥åè½¬æ¢æä»¤çç®æ³ï¼æä»¬å°å¶æ¹ç¼å¹¶åºç¨ï¼åæ¶ï¼æè°¢ä»ç
 [ç½é¡µçè½¬æ¢å¨](https://dislink.github.io/midi2bdx/
 )ç»æä»¬çå¼åä¸æ´æ°å¸¦æ¥å·¨å¤§çåååå¨åï¼è®©æä»¬å¨åæ¬ä¸éªç»å°çæ¸é±¼éè·¯ä¸è½¬åå¼åï¼å¸æä»è½èä¸ä¸ä¸ªçæ³çå¤§å­¦ï¼
-- æè°¢ **Touch âå·åâ**\>
-æä¾çBDXå¯¼å¥æµè¯æ¯æï¼å¹¶å¯¹ç¨åºçæ¹è¿æä¾äºä¸°å¯çæè§ï¼åæ¶ä¹æè°¢ä»çä¸æ­å°è¯æ°çåå®¹ï¼ä½¿æä»¬çæéæ´è¿ä¸æ­¥
+- æè°¢ **Touch âå·åâ**\> æä¾ç BDX
+å¯¼å¥æµè¯æ¯æï¼å¹¶å¯¹ç¨åºçæ¹è¿æä¾äºä¸°å¯çæè§ï¼åæ¶ä¹æè°¢ä»çä¸æ­å°è¯æ°çåå®¹ï¼ä½¿æä»¬çæéæ´è¿ä¸æ­¥
 - æè°¢ **Mono**\>
-åé¦å®è£æ¶çé®é¢ï¼è¾å©æä»¬æ¾å°äºè§çªæä½ç³»ç»ä¸çå¼å®¹æ§é®é¢ï¼æè°¢å¶åé¦å»¶è¿æ­æ¾å¨åºç°çéå¤§é®é¢ï¼è®©æä»¬å¾ä»¥ä¿®æ¹å¨é¨å»¶è¿æ­æ¾éè¯¯
+åé¦å®è£æ¶çé®é¢ï¼è¾å©æä»¬æ¾å°äºè§çªæä½ç³»ç»ä¸çå¼å®¹æ§é®é¢ï¼æè°¢å¶åé¦å»¶è¿æ­æ¾å¨åºç°çéå¤§é®é¢ï¼è®©æä»¬å¾ä»¥ä¿®æ¹å¨é¨å»¶è¿æ­æ¾éè¯¯ï¼å°¤å¶æè°¢ä»å¯¹äºæä»¬çè½¯ä»¶çå¤§åå®£ä¼ 
 - æè°¢ **Ammelia âè¾ç±³å©äºâ**\>
-æ¦ä¿æä»¬è¿è¡æ°çåè½å¼åï¼å¹¶ä¸ºæ°åè½æåºäºéå¸¸ä¼ç§çå¤§éå»ºè®®ï¼ä»¥åæä¾çBDXå¯¼å¥æµè¯æ¯æï¼ä¸ºæä»¬çæ°ç»æçæç®æ³æä¾äºå¤§éçå®éçè®ºæ¯æ
+æ¦ä¿æä»¬è¿è¡æ°çåè½å¼åï¼å¹¶ä¸ºæ°åè½æåºäºéå¸¸ä¼ç§çå¤§éå»ºè®®ï¼ä»¥åæä¾ç
+BDX
+å¯¼å¥æµè¯æ¯æï¼ä¸ºæä»¬çæ°ç»æçæç®æ³æä¾äºå¤§éçå®éçè®ºæ¯æ
 - æè°¢ **[ç¥ç¾½](https://gitee.com/snowykami) â[SnowyKami](https://
 github.com/snowyfirefly)â**
-å¯¹æä»¬é¡¹ç®çæ¯æä¸å®£ä¼ ï¼å¸æä»è½èçä¸æä¼ç§çå¤§å­¦ï¼
-- æè°¢ **æä»¤å¸_è¦åæ
-playjuice123**\>ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéæä»¬ä¿®å¤ä¸ä¸ªä¸ç´å­å¨çå¤§bugã
-- æè°¢ **é·é**\>ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéä¿®å¤bugã >
-æè°¢å¹¿å¤§ç¾¤åä¸ºæ­¤ç¨åºæä¾çæµè¯ç­æ¯æ > >
+å¯¹æä»¬é¡¹ç®çæ¯æä¸å®£ä¼ ï¼å¸æä»è½èå¾ä¸æä¼ç§çå¤§å­¦ï¼
+- æè°¢ **æä»¤å¸\_è¦åæ
+playjuice123**\>ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéæä»¬ä¿®å¤ä¸ä¸ªä¸ç´å­å¨çå¤§
+bugã - æè°¢
+**é·é**\>ç¨ä»é£ä»¤ææå¼åèé½å¤§ä¸ºåç«çæä½æ¹æ³ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéä¿®å¤
+bugã > æè°¢å¹¿å¤§ç¾¤åä¸ºæ­¤ç¨åºæä¾çæµè¯ç­æ¯æ > >
 è¥æ¨å¯¹æä»¬ææè´¡ç®ä½æ¨çåå­æ²¡ææ¾ç¤ºå¨æ­¤åè¡¨ä¸­ï¼è¯·èç³»æä»¬ï¼
-## èç³»ð è¥éå°åºä¸­çé®é¢ï¼æ¬¢è¿å¨[æ­¤](https://gitee.com/TriM-
-Organization/Musicreater/issues/new)æåºä½ çissueã
-å¦æéè¦ä¸å¼åç»è¿è¡äº¤æµï¼æ¬¢è¿å å¥æä»¬ç[å¼åé²èQç¾¤]
-(https://jq.qq.com/?_wv=1027&k=hpeRxrYr)ã -----------------------------------
---------- æ­¤é¡¹ç®å¹¶éä¸ä¸ªå®æ¹ ãæçä¸çãï¼*Minecraft*ï¼é¡¹ç®
-æ­¤é¡¹ç®ä¸é¶å±æå³èäº Mojang Studios æ å¾®è½¯ æ­¤é¡¹ç®äº¦ä¸ä¸
-ç½æ ç¸å³ âMinecraftâæ¯ Mojang Synergies AB
+## èç³» ð è¥éå°åºä¸­çé®é¢ï¼æ¬¢è¿å¨[æ­¤](https://gitee.com/
+TriM-Organization/Musicreater/issues/new)æåºä½ ç issueã
+å¦æéè¦ä¸å¼åç»è¿è¡äº¤æµï¼æ¬¢è¿å å¥æä»¬ç[å¼åé²è Q
+ç¾¤](https://jq.qq.com/?_wv=1027&k=hpeRxrYr)ã --- æ­¤é¡¹ç®å¹¶éä¸ä¸ªå®æ¹
+ãæçä¸çãï¼_Minecraft_ï¼é¡¹ç® æ­¤é¡¹ç®ä¸é¶å±æå³èäº Mojang
+Studios æ å¾®è½¯ æ­¤é¡¹ç®äº¦ä¸é¶å±æå³èäº ç½æ âMinecraftâæ¯
+Mojang Synergies AB
 çåæ ï¼æ­¤é¡¹ç®ä¸­ææå¯¹äºâæçä¸çâãâMinecraftâç­ç¸å³ç§°å¼åä¸ºå¼ç¨æ§ä½¿ç¨
-* ä¸ææåç ç½æ
+- ä¸ææåç ç½æ
 å¬å¸ï¼æä»£çæ¯å¨ä¸­å½å¤§éè¿è¥ãæçä¸çï¼ä¸­å½çãçä¸æµ·ç½ä¹æç½ç»ç§æåå±æéå¬å¸
 NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR
-MICROSOFT. [Bilibili: éç¾¿ELS]: https://img.shields.io/badge/Bilibili-
-%E5%87%8C%E4%BA%91%E9%87%91%E7%BE%BF-00A1E7?style=for-the-badge [Bilibili:
-è¯¸èäº®ä¸å«å¦éµ]: https://img.shields.io/badge/Bilibili-
+MICROSOFT. NOT APPROVED BY OR ASSOCIATED WITH NETEASE. [Bilibili: éç¾¿ELS]:
+https://img.shields.io/badge/Bilibili-%E5%87%8C%E4%BA%91%E9%87%91%E7%BE%BF-
+00A1E7?style=for-the-badge [Bilibili: è¯¸èäº®ä¸å«å¦éµ]: https://
+img.shields.io/badge/Bilibili-
 %E8%AF%B8%E8%91%9B%E4%BA%AE%E4%B8%8E%E5%85%AB%E5%8D%A6%E9%98%B5-
 00A1E7?style=for-the-badge [CodeStyle: black]: https://img.shields.io/badge/
 code%20style-black-121110.svg?style=for-the-badge [python]: https://
 img.shields.io/badge/python-3.8-AB70FF?style=for-the-badge [release]: https://
 img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
 [license]: https://img.shields.io/badge/Licence-Apache-228B22?style=for-the-
 badge
```

### Comparing `Musicreater-0.5.1/setup.py` & `Musicreater-1.0.0/setup.py`

 * *Files identical despite different names*

