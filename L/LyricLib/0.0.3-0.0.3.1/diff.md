# Comparing `tmp/LyricLib-0.0.3.tar.gz` & `tmp/LyricLib-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LyricLib-0.0.3.tar", last modified: Sun May  7 03:04:30 2023, max compression
+gzip compressed data, was "LyricLib-0.0.3.1.tar", last modified: Sat May 27 11:55:59 2023, max compression
```

## Comparing `LyricLib-0.0.3.tar` & `LyricLib-0.0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 03:04:30.431396 LyricLib-0.0.3/
--rw-rw-rw-   0        0        0    12937 2023-05-01 02:54:44.000000 LyricLib-0.0.3/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-05-07 03:04:30.416446 LyricLib-0.0.3/LyricLib/
--rw-rw-rw-   0        0        0     1261 2023-05-01 02:54:44.000000 LyricLib-0.0.3/LyricLib/LICENSE(lrc-parser).md
--rw-rw-rw-   0        0        0      619 2023-05-07 03:03:51.000000 LyricLib-0.0.3/LyricLib/__init__.py
--rw-rw-rw-   0        0        0     1241 2023-05-01 02:54:44.000000 LyricLib-0.0.3/LyricLib/constants.py
--rw-rw-rw-   0        0        0     1053 2023-05-01 02:54:44.000000 LyricLib-0.0.3/LyricLib/exceptions.py
--rw-rw-rw-   0        0        0     7715 2023-05-01 03:40:42.000000 LyricLib-0.0.3/LyricLib/main.py
--rw-rw-rw-   0        0        0    11166 2023-05-07 03:03:51.000000 LyricLib-0.0.3/LyricLib/subclass.py
-drwxrwxrwx   0        0        0        0 2023-05-07 03:04:30.425415 LyricLib-0.0.3/LyricLib.egg-info/
--rw-rw-rw-   0        0        0     2745 2023-05-07 03:04:30.000000 LyricLib-0.0.3/LyricLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      404 2023-05-07 03:04:30.000000 LyricLib-0.0.3/LyricLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 03:04:30.000000 LyricLib-0.0.3/LyricLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-07 03:04:30.000000 LyricLib-0.0.3/LyricLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       41 2023-05-07 03:03:51.000000 LyricLib-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2745 2023-05-07 03:04:30.430400 LyricLib-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1795 2023-05-01 02:56:30.000000 LyricLib-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 03:04:30.427410 LyricLib-0.0.3/docs/
--rw-rw-rw-   0        0        0     6577 2023-05-01 02:54:44.000000 LyricLib-0.0.3/docs/Lrc文件格式.md
--rw-rw-rw-   0        0        0      470 2023-05-07 03:03:51.000000 LyricLib-0.0.3/docs/开发日志.TXT
--rw-rw-rw-   0        0        0       42 2023-05-07 03:04:30.431396 LyricLib-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1354 2023-05-07 03:03:51.000000 LyricLib-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:55:59.032659 LyricLib-0.0.3.1/
+-rw-rw-rw-   0        0        0    12940 2023-05-27 11:50:34.000000 LyricLib-0.0.3.1/LICENSE.md
+drwxrwxrwx   0        0        0        0 2023-05-27 11:55:59.018706 LyricLib-0.0.3.1/LyricLib/
+-rw-rw-rw-   0        0        0     1261 2023-05-01 02:54:44.000000 LyricLib-0.0.3.1/LyricLib/LICENSE(lrc-parser).md
+-rw-rw-rw-   0        0        0      631 2023-05-27 11:50:34.000000 LyricLib-0.0.3.1/LyricLib/__init__.py
+-rw-rw-rw-   0        0        0     1241 2023-05-01 02:54:44.000000 LyricLib-0.0.3.1/LyricLib/constants.py
+-rw-rw-rw-   0        0        0     1053 2023-05-01 02:54:44.000000 LyricLib-0.0.3.1/LyricLib/exceptions.py
+-rw-rw-rw-   0        0        0     7737 2023-05-27 11:50:34.000000 LyricLib-0.0.3.1/LyricLib/main.py
+-rw-rw-rw-   0        0        0    11222 2023-05-27 11:50:34.000000 LyricLib-0.0.3.1/LyricLib/subclass.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:55:59.026677 LyricLib-0.0.3.1/LyricLib.egg-info/
+-rw-rw-rw-   0        0        0     2753 2023-05-27 11:55:58.000000 LyricLib-0.0.3.1/LyricLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2023-05-27 11:55:58.000000 LyricLib-0.0.3.1/LyricLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 11:55:58.000000 LyricLib-0.0.3.1/LyricLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-27 11:55:58.000000 LyricLib-0.0.3.1/LyricLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       41 2023-05-07 03:03:51.000000 LyricLib-0.0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2753 2023-05-27 11:55:59.031668 LyricLib-0.0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1801 2023-05-27 11:50:34.000000 LyricLib-0.0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 11:55:59.029667 LyricLib-0.0.3.1/docs/
+-rw-rw-rw-   0        0        0     6577 2023-05-01 02:54:44.000000 LyricLib-0.0.3.1/docs/Lrc文件格式.md
+-rw-rw-rw-   0        0        0      533 2023-05-27 11:50:34.000000 LyricLib-0.0.3.1/docs/开发日志.TXT
+-rw-rw-rw-   0        0        0       42 2023-05-27 11:55:59.032659 LyricLib-0.0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1354 2023-05-07 03:03:51.000000 LyricLib-0.0.3.1/setup.py
```

### Comparing `LyricLib-0.0.3/LICENSE.md` & `LyricLib-0.0.3.1/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 **注意，以下条款或版权声明应当且必须是高于此仓库中任何其他声明的**
 
 1. 此项目项目的全部开发者享有其完整版权，其开发者可以在任一时刻终止以后的源代码开放，若经由其开发者授予特殊权利，则授权对象可以将源代码进行特定的被特殊授权的操作
 2. 此项目或（及）其代码允许在 Apache2.0 协议的条款与说明下进行非商业使用
 3. 除部分代码特殊声明外，此项目允许对其或（及）其代码进行商业化使用，但是需要经过项目的主要开发者一致授权，同时，授权对象在商业化授权的使用过程中必须依照 Apache2.0 协议的条款与说明
 4. 若存在对于此项目中包含的部分代码的特殊开源声明，则此部分代码依照其特定的开源方式授权，但若此部分代码经由此部分代码的主要开发者一致特殊授权后商用，则授权对象在商用时依照此部分的开发者所准许的方式（或条款）进行商用
-5. Apache2.0 协议的英文原文副本可见下文
+5. Apache2.0 协议的英文原文副本可见下方
 
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
 
 
-   Copyright 2022-2023 thecasttim and all the developers of Lyric
+   Copyright 2022-2023 thecasttim and all the developers of LyricLib
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `LyricLib-0.0.3/LyricLib/LICENSE(lrc-parser).md` & `LyricLib-0.0.3.1/LyricLib/LICENSE(lrc-parser).md`

 * *Files identical despite different names*

### Comparing `LyricLib-0.0.3/LyricLib/__init__.py` & `LyricLib-0.0.3.1/LyricLib/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 """
 简单的歌词处理库
 A library for parsing, reading & editing LyricLib
 
-版权所有© 全体 LyricLib 作者 及 thecasttim
+版权所有© 2022-2023 全体 LyricLib 作者 及 thecasttim
 Copyright 2022-2023 thecasttim and all the developers of LyricLib
 
 开源相关声明请见 ../License.md
 Terms & Conditions: ../License.md
 """
 
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 版权所有 Lyric全体开发者
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 from .main import *
 
-__version__ = "0.0.3"
+__version__ = "0.0.3.1"
 __all__ = []
 __author__ = (("金羿", "Eilles Wan"), ("thecasttim", "thecasttim"))
```

### Comparing `LyricLib-0.0.3/LyricLib/constants.py` & `LyricLib-0.0.3.1/LyricLib/constants.py`

 * *Files identical despite different names*

### Comparing `LyricLib-0.0.3/LyricLib/exceptions.py` & `LyricLib-0.0.3.1/LyricLib/exceptions.py`

 * *Files identical despite different names*

### Comparing `LyricLib-0.0.3/LyricLib/main.py` & `LyricLib-0.0.3.1/LyricLib/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
     AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
     SOFTWARE.
 
 继承协议：
-版权所有© 全体 LyricLib 作者 及 thecasttim
+版权所有© 2022-2023 全体 LyricLib 作者 及 thecasttim
 Copyright 2022-2023 thecasttim and all the developers of LyricLib
 
 开源相关声明请见 ../License.md
 Terms & Conditions: ../License.md
 """
 
 import codecs
@@ -202,25 +202,25 @@
         pattern = LRC_ENHANCE_TIME_PATTERN_N
         timestamps = [time[1:-1] for time in re.findall(pattern, segment)]
         parts = re.split(pattern, segment)
         return timestamps, parts
 
     @property
     def get_ids(self):
-        # 获取 ID 标签列表
+        """获取 ID 标签列表"""
         return self.meta_info
 
     @property
     def get_lyrics(self):
-        # 获取歌词列表
+        """获取歌词列表"""
         return self.lyrics
 
     @property
     def get_unknowns(self):
-        # 获取未知标签字段列表
+        """获取未知标签字段列表"""
         return self.extra_info
 
     def to_lrc(self, fdist: TextIO, time_format_style=STABLE_LRC_TIME_FORMAT_STYLE):
         """
         保存为LRC文件
         """
         for id, value in self.meta_info.lrc_id_dict().items():
```

### Comparing `LyricLib-0.0.3/LyricLib/subclass.py` & `LyricLib-0.0.3.1/LyricLib/subclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,23 +61,23 @@
         time_tag_str: str
             Lrc歌词文件的字符串时间标签
         """
 
         try:
             # print(time_tag_str)
             return cls(
-                *cls.parse_time_tag(time_tag_str.replace("[", "").replace("]", ""))
+                *cls.parse_lrc_time_tag(time_tag_str.replace("[", "").replace("]", ""))
             )
         except TimeTooPreciseError:
             raise LrcDestroyedError("时间标签出现错误: {}".format(time_tag_str), time_tag_str)
 
     @staticmethod
-    def parse_time_tag(time_tag_str):
+    def parse_lrc_time_tag(time_tag_str):
         """
-        将字符串格式的时间戳解析为 时、分、秒、毫秒
+        将LRC文件的字符串格式的时间戳解析为 时、分、秒、毫秒
 
         Parameters
         ----------
         time_tag_str: int
             时间戳字符串
 
         Returns
@@ -246,25 +246,25 @@
     def __init__(self, sentence: str, extension: Dict[TimeStamp, str] = {}):
         """建立一句歌词"""
         self.whole_context = sentence
         self.word_extension = extension
 
     @classmethod
     def from_lrc_str_dict(cls, sentence: str, **extension):
-        """从lrc时间标签字符串而组成的字典中获取附加信息"""
+        """从LRC时间标签字符串而组成的字典中获取附加信息"""
         word_extension = {}
         for time_str, word in extension.items():
             word_extension[TimeStamp.from_lrc_time_tag(time_tag_str=time_str)] = word
         return cls(sentence, word_extension)
 
     @classmethod
     def from_lrc_str_list(
         cls, sentence: str, time_str_list: List[str], word_list: List[str]
     ):
-        """从lrc时间列表和单词列表中获取附加信息"""
+        """从LRC时间列表和单词列表中获取附加信息"""
         time_list_length = len(time_str_list)
         word_list_length = len(word_list)
         if time_list_length != word_list_length:
             raise WordTagError(
                 word_list_length < time_list_length, time_str_list, word_list
             )
         word_extension = {}
@@ -358,14 +358,15 @@
             "Recorder": self.Recorder,
             "Editor": self.Editor,
             "Version": self.Version,
             "Offset": self.Offset,
         }
 
     def set_meta(self, meta_name: str, meta_value: str):
+        """设置单个元信息"""
         if meta_name == "Singer":
             self.Singer = meta_value
         elif meta_name == "Album":
             self.Album = meta_value
         elif meta_name == "Title":
             self.Title = meta_value
         elif meta_name == "LyricAuthor":
```

### Comparing `LyricLib-0.0.3/LyricLib.egg-info/PKG-INFO` & `LyricLib-0.0.3.1/LyricLib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LyricLib
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: 歌词的处理库
 Home-page: https://github.com/TriM-Organization/Lyric
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-<h1 align="center">歌词 Lyric</h1>
+<h1 align="center">歌词 LyricLib</h1>
 
 <h3 align="center">歌词的处理库</h3>
 
 <p align="center">
 <img src="https://forthebadge.com/images/badges/built-with-love.svg">
 <p>
 
@@ -37,19 +37,19 @@
 
 
 简体中文🇨🇳 | [English🇬🇧](README_EN.md)
 
 
 ## 介绍🚀
 
-Lyric是一个简单的歌词处理库
+LyricLib是一个简单的歌词处理库
 
 欢迎加群：[861684859](https://jq.qq.com/?_wv=1027&k=hpeRxrYr)
 
-## 使用📖
+## 文档📖
 
 暂无
 
 ## 致谢🙏
 
 非常感谢 [thecasttim](https://gitee.com/thecasttim) 的 [LrcParser](https://gitee.com/thecasttim/lrc-parser) 项目，为此项目提供了非常大的参考。可以说，本项目就是基于它进行了进一步的修改而开发的。
```

### Comparing `LyricLib-0.0.3/PKG-INFO` & `LyricLib-0.0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LyricLib
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: 歌词的处理库
 Home-page: https://github.com/TriM-Organization/Lyric
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-<h1 align="center">歌词 Lyric</h1>
+<h1 align="center">歌词 LyricLib</h1>
 
 <h3 align="center">歌词的处理库</h3>
 
 <p align="center">
 <img src="https://forthebadge.com/images/badges/built-with-love.svg">
 <p>
 
@@ -37,19 +37,19 @@
 
 
 简体中文🇨🇳 | [English🇬🇧](README_EN.md)
 
 
 ## 介绍🚀
 
-Lyric是一个简单的歌词处理库
+LyricLib是一个简单的歌词处理库
 
 欢迎加群：[861684859](https://jq.qq.com/?_wv=1027&k=hpeRxrYr)
 
-## 使用📖
+## 文档📖
 
 暂无
 
 ## 致谢🙏
 
 非常感谢 [thecasttim](https://gitee.com/thecasttim) 的 [LrcParser](https://gitee.com/thecasttim/lrc-parser) 项目，为此项目提供了非常大的参考。可以说，本项目就是基于它进行了进一步的修改而开发的。
```

### Comparing `LyricLib-0.0.3/README.md` & `LyricLib-0.0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<h1 align="center">歌词 Lyric</h1>
+<h1 align="center">歌词 LyricLib</h1>
 
 <h3 align="center">歌词的处理库</h3>
 
 <p align="center">
 <img src="https://forthebadge.com/images/badges/built-with-love.svg">
 <p>
 
@@ -15,19 +15,19 @@
 
 
 简体中文🇨🇳 | [English🇬🇧](README_EN.md)
 
 
 ## 介绍🚀
 
-Lyric是一个简单的歌词处理库
+LyricLib是一个简单的歌词处理库
 
 欢迎加群：[861684859](https://jq.qq.com/?_wv=1027&k=hpeRxrYr)
 
-## 使用📖
+## 文档📖
 
 暂无
 
 ## 致谢🙏
 
 非常感谢 [thecasttim](https://gitee.com/thecasttim) 的 [LrcParser](https://gitee.com/thecasttim/lrc-parser) 项目，为此项目提供了非常大的参考。可以说，本项目就是基于它进行了进一步的修改而开发的。
```

### Comparing `LyricLib-0.0.3/docs/Lrc文件格式.md` & `LyricLib-0.0.3.1/docs/Lrc文件格式.md`

 * *Files identical despite different names*

### Comparing `LyricLib-0.0.3/setup.py` & `LyricLib-0.0.3.1/setup.py`

 * *Files identical despite different names*

