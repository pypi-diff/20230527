# Comparing `tmp/thztools-1.0.2.tar.gz` & `tmp/thztools-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thztools-1.0.2.tar", last modified: Fri May 26 04:15:10 2023, max compression
+gzip compressed data, was "thztools-1.0.3.tar", last modified: Sat May 27 04:52:56 2023, max compression
```

## Comparing `thztools-1.0.2.tar` & `thztools-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 04:15:10.686888 thztools-1.0.2/
--rw-rw-rw-   0        0        0       26 2023-05-26 04:13:13.000000 thztools-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2524 2023-05-26 04:15:10.682888 thztools-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2102 2023-05-26 04:13:16.000000 thztools-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-26 04:15:10.687888 thztools-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1051 2023-05-26 04:13:11.000000 thztools-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 04:15:10.653886 thztools-1.0.2/thztools/
--rw-rw-rw-   0        0        0        0 2023-05-25 09:22:46.000000 thztools-1.0.2/thztools/__init__.py
--rw-rw-rw-   0        0        0     6096 2023-05-26 04:13:14.000000 thztools-1.0.2/thztools/jiami.py
-drwxrwxrwx   0        0        0        0 2023-05-26 04:15:10.677888 thztools-1.0.2/thztools.egg-info/
--rw-rw-rw-   0        0        0     2524 2023-05-26 04:15:10.000000 thztools-1.0.2/thztools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-05-26 04:15:10.000000 thztools-1.0.2/thztools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 04:15:10.000000 thztools-1.0.2/thztools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-26 04:15:10.000000 thztools-1.0.2/thztools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-26 04:15:10.000000 thztools-1.0.2/thztools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 04:52:56.285281 thztools-1.0.3/
+-rw-rw-rw-   0        0        0       26 2023-05-26 04:13:13.000000 thztools-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2856 2023-05-27 04:52:56.281281 thztools-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2434 2023-05-27 04:40:50.000000 thztools-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-27 04:52:56.287281 thztools-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2023-05-27 04:23:43.000000 thztools-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 04:52:55.879258 thztools-1.0.3/thztools/
+-rw-rw-rw-   0        0        0        0 2023-05-25 09:22:46.000000 thztools-1.0.3/thztools/__init__.py
+-rw-rw-rw-   0        0        0     1496 2023-05-27 04:40:24.000000 thztools-1.0.3/thztools/ip.py
+-rw-rw-rw-   0        0        0     6106 2023-05-27 04:21:41.000000 thztools-1.0.3/thztools/jiami.py
+drwxrwxrwx   0        0        0        0 2023-05-27 04:52:56.272280 thztools-1.0.3/thztools.egg-info/
+-rw-rw-rw-   0        0        0     2856 2023-05-27 04:52:54.000000 thztools-1.0.3/thztools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-05-27 04:52:55.000000 thztools-1.0.3/thztools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 04:52:54.000000 thztools-1.0.3/thztools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-27 04:52:54.000000 thztools-1.0.3/thztools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-27 04:52:54.000000 thztools-1.0.3/thztools.egg-info/top_level.txt
```

### Comparing `thztools-1.0.2/PKG-INFO` & `thztools-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thztools
-Version: 1.0.2
+Version: 1.0.3
 Summary: 由天狐宗开发的工具，方便开发时使用
 Home-page: https://github.com/tianhuzong/thztools
 Author: Sen
 Author-email: tianhuzong@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,22 +15,28 @@
 >author:Sen
 >>e-mail:tianhuzong@qq.com 
 >>Github:https://github.com/tianhuzong
 >>Gitee:https://gitee.com/thzsen
 >>QQ:1485319167
 - - -
 >Tianhuzong开发的工具，方便在开发中使用
-目前版本加入了加密解密内容：<kbd>RSA</kbd>,<kbd>AES</kbd>，<kbd>凯撒加密</kbd>
+1.0.2加入了加密解密内容：<kbd>RSA</kbd>,<kbd>AES</kbd>，<kbd>凯撒加密</kbd>
+- - -
+>1.0.3版本中，引入了与ip地址有关的类<kbd>IP</kbd>
 - - -
 ##使用方法：
+- - -
 ####安装模块
 ```bash
 pip install thztools
 ```
 安装完模块之后接下来就是引用了
+
+下面是引用jiami模块的类的用法
+
 ```python
 from  thztools.jiami import *
 #-----RSA-----
 rsa = RSA()
 #生成密钥对
 (gongyao,siyao) = rsa.newkeys(1024)#返回生成的密钥对
 #加密
@@ -79,7 +85,19 @@
 miwen = wjny.jiami("这是被加密的文字",'thisisakey')
 #返回密文
 
 #解密
 mingwen = wjny.jiemi("这是被解密的文字",'thisisakey')
 #返回明文
 ```
+
+下面是使用ip模块的类的用法
+
+```python
+from thztools.ip import *
+ip = IP()
+
+#IP地址的基本信息
+infomation = ip.jbxx(ip = '192.0.2.0')
+#ip地理位置
+geo = ip.geo(ip = '8.8.8.8')
+```
```

### Comparing `thztools-1.0.2/README.md` & `thztools-1.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 >author:Sen
 >>e-mail:tianhuzong@qq.com 
 >>Github:https://github.com/tianhuzong
 >>Gitee:https://gitee.com/thzsen
 >>QQ:1485319167
 - - -
 >Tianhuzong开发的工具，方便在开发中使用
-目前版本加入了加密解密内容：<kbd>RSA</kbd>,<kbd>AES</kbd>，<kbd>凯撒加密</kbd>
+1.0.2加入了加密解密内容：<kbd>RSA</kbd>,<kbd>AES</kbd>，<kbd>凯撒加密</kbd>
+- - -
+>1.0.3版本中，引入了与ip地址有关的类<kbd>IP</kbd>
 - - -
 ##使用方法：
+- - -
 ####安装模块
 ```bash
 pip install thztools
 ```
 安装完模块之后接下来就是引用了
+
+下面是引用jiami模块的类的用法
+
 ```python
 from  thztools.jiami import *
 #-----RSA-----
 rsa = RSA()
 #生成密钥对
 (gongyao,siyao) = rsa.newkeys(1024)#返回生成的密钥对
 #加密
@@ -65,8 +71,20 @@
 #加密
 miwen = wjny.jiami("这是被加密的文字",'thisisakey')
 #返回密文
 
 #解密
 mingwen = wjny.jiemi("这是被解密的文字",'thisisakey')
 #返回明文
+```
+
+下面是使用ip模块的类的用法
+
+```python
+from thztools.ip import *
+ip = IP()
+
+#IP地址的基本信息
+infomation = ip.jbxx(ip = '192.0.2.0')
+#ip地理位置
+geo = ip.geo(ip = '8.8.8.8')
 ```
```

### Comparing `thztools-1.0.2/setup.py` & `thztools-1.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup
 with open("./README.md",mode='r',encoding='utf-8') as f:
     des = f.read()
 setup(
     name="thztools",      # 包名，用于安装和调用该包
-    version="1.0.2",               # 版本号
+    version="1.0.3",               # 版本号
     author="Sen",
     description="由天狐宗开发的工具，方便开发时使用",
     long_description=des,
     long_description_content_type='text/markdown',
     author_email="tianhuzong@qq.com",
     url="https://github.com/tianhuzong/thztools",
     license="MIT",
     packages=["thztools"],     # 需要打包的包，可以是单个或多个包
     package_data={"thztools": ["*.py"]},  # 包需要包含的数据文件（可选）
     install_requires=[           # 安装依赖，可以是单个或多个依赖项
         "rsa",
         "Crypto",
+        "2ip"
     ],
     classifiers=[                # 分类标签（可选），使用 PyPI 标准分类
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
 )
```

### Comparing `thztools-1.0.2/thztools/jiami.py` & `thztools-1.0.3/thztools/jiami.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         try:
             # 解密密文
             plaintext = cipher.decrypt_and_verify(ciphertext, tag)
             return plaintext.decode('utf-8')
         except:
             return None
 class Weijiniya:
-    def jiami(plaintext, key):
+    def jiami(self,plaintext, key):
         """
         使用维吉尼亚密码加密明文字符串
 
         参数:
             plaintext (str): 明文字符串
             key (str): 加密秘钥，只能包含小写字母
 
@@ -153,15 +153,15 @@
                 ciphertext += shifted_char
                 key_index += 1
             else:
                 # 非字母字符直接加入密文字符串中
                 ciphertext += c
         return ciphertext
 
-    def jiemi(ciphertext, key):
+    def jiemi(self,ciphertext, key):
         """
         使用维吉尼亚密码解密密文字符串
 
         参数:
             ciphertext (str): 密文字符串
             key (str): 解密秘钥，只能包含小写字母
```

### Comparing `thztools-1.0.2/thztools.egg-info/PKG-INFO` & `thztools-1.0.3/thztools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thztools
-Version: 1.0.2
+Version: 1.0.3
 Summary: 由天狐宗开发的工具，方便开发时使用
 Home-page: https://github.com/tianhuzong/thztools
 Author: Sen
 Author-email: tianhuzong@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,22 +15,28 @@
 >author:Sen
 >>e-mail:tianhuzong@qq.com 
 >>Github:https://github.com/tianhuzong
 >>Gitee:https://gitee.com/thzsen
 >>QQ:1485319167
 - - -
 >Tianhuzong开发的工具，方便在开发中使用
-目前版本加入了加密解密内容：<kbd>RSA</kbd>,<kbd>AES</kbd>，<kbd>凯撒加密</kbd>
+1.0.2加入了加密解密内容：<kbd>RSA</kbd>,<kbd>AES</kbd>，<kbd>凯撒加密</kbd>
+- - -
+>1.0.3版本中，引入了与ip地址有关的类<kbd>IP</kbd>
 - - -
 ##使用方法：
+- - -
 ####安装模块
 ```bash
 pip install thztools
 ```
 安装完模块之后接下来就是引用了
+
+下面是引用jiami模块的类的用法
+
 ```python
 from  thztools.jiami import *
 #-----RSA-----
 rsa = RSA()
 #生成密钥对
 (gongyao,siyao) = rsa.newkeys(1024)#返回生成的密钥对
 #加密
@@ -79,7 +85,19 @@
 miwen = wjny.jiami("这是被加密的文字",'thisisakey')
 #返回密文
 
 #解密
 mingwen = wjny.jiemi("这是被解密的文字",'thisisakey')
 #返回明文
 ```
+
+下面是使用ip模块的类的用法
+
+```python
+from thztools.ip import *
+ip = IP()
+
+#IP地址的基本信息
+infomation = ip.jbxx(ip = '192.0.2.0')
+#ip地理位置
+geo = ip.geo(ip = '8.8.8.8')
+```
```

