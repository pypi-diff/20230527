# Comparing `tmp/thztools-1.0.3.tar.gz` & `tmp/thztools-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thztools-1.0.3.tar", last modified: Sat May 27 04:52:56 2023, max compression
+gzip compressed data, was "thztools-1.0.4.tar", last modified: Sat May 27 05:04:30 2023, max compression
```

## Comparing `thztools-1.0.3.tar` & `thztools-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 04:52:56.285281 thztools-1.0.3/
--rw-rw-rw-   0        0        0       26 2023-05-26 04:13:13.000000 thztools-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2856 2023-05-27 04:52:56.281281 thztools-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2434 2023-05-27 04:40:50.000000 thztools-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-27 04:52:56.287281 thztools-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1066 2023-05-27 04:23:43.000000 thztools-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 04:52:55.879258 thztools-1.0.3/thztools/
--rw-rw-rw-   0        0        0        0 2023-05-25 09:22:46.000000 thztools-1.0.3/thztools/__init__.py
--rw-rw-rw-   0        0        0     1496 2023-05-27 04:40:24.000000 thztools-1.0.3/thztools/ip.py
--rw-rw-rw-   0        0        0     6106 2023-05-27 04:21:41.000000 thztools-1.0.3/thztools/jiami.py
-drwxrwxrwx   0        0        0        0 2023-05-27 04:52:56.272280 thztools-1.0.3/thztools.egg-info/
--rw-rw-rw-   0        0        0     2856 2023-05-27 04:52:54.000000 thztools-1.0.3/thztools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-05-27 04:52:55.000000 thztools-1.0.3/thztools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 04:52:54.000000 thztools-1.0.3/thztools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-27 04:52:54.000000 thztools-1.0.3/thztools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-27 04:52:54.000000 thztools-1.0.3/thztools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 05:04:30.916012 thztools-1.0.4/
+-rw-rw-rw-   0        0        0       26 2023-05-26 04:13:13.000000 thztools-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3001 2023-05-27 05:04:30.913011 thztools-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2579 2023-05-27 05:04:03.000000 thztools-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-27 05:04:30.920012 thztools-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2023-05-27 04:59:48.000000 thztools-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 05:04:30.861009 thztools-1.0.4/thztools/
+-rw-rw-rw-   0        0        0        0 2023-05-25 09:22:46.000000 thztools-1.0.4/thztools/__init__.py
+-rw-rw-rw-   0        0        0     2212 2023-05-27 05:03:59.000000 thztools-1.0.4/thztools/ip.py
+-rw-rw-rw-   0        0        0     6106 2023-05-27 04:21:41.000000 thztools-1.0.4/thztools/jiami.py
+drwxrwxrwx   0        0        0        0 2023-05-27 05:04:30.903011 thztools-1.0.4/thztools.egg-info/
+-rw-rw-rw-   0        0        0     3001 2023-05-27 05:04:30.000000 thztools-1.0.4/thztools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-05-27 05:04:30.000000 thztools-1.0.4/thztools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 05:04:30.000000 thztools-1.0.4/thztools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-27 05:04:30.000000 thztools-1.0.4/thztools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-27 05:04:30.000000 thztools-1.0.4/thztools.egg-info/top_level.txt
```

### Comparing `thztools-1.0.3/PKG-INFO` & `thztools-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thztools
-Version: 1.0.3
+Version: 1.0.4
 Summary: 由天狐宗开发的工具，方便开发时使用
 Home-page: https://github.com/tianhuzong/thztools
 Author: Sen
 Author-email: tianhuzong@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,17 @@
 >>Github:https://github.com/tianhuzong
 >>Gitee:https://gitee.com/thzsen
 >>QQ:1485319167
 - - -
 >Tianhuzong开发的工具，方便在开发中使用
 1.0.2加入了加密解密内容：<kbd>RSA</kbd>,<kbd>AES</kbd>，<kbd>凯撒加密</kbd>
 - - -
->1.0.3版本中，引入了与ip地址有关的类<kbd>IP</kbd>
+>1.0.3版本中，修复了维吉尼亚密码的错误，引入了与ip地址有关的类<kbd>IP</kbd>
+- - -
+>1.0.4版本中，新增了检测ip是否为合法的IPv4
 - - -
 ##使用方法：
 - - -
 ####安装模块
 ```bash
 pip install thztools
 ```
@@ -91,13 +93,13 @@
 ```
 
 下面是使用ip模块的类的用法
 
 ```python
 from thztools.ip import *
 ip = IP()
-
+#请注意，输入的ip应为IPv4地址
 #IP地址的基本信息
 infomation = ip.jbxx(ip = '192.0.2.0')
 #ip地理位置
 geo = ip.geo(ip = '8.8.8.8')
 ```
```

### Comparing `thztools-1.0.3/README.md` & `thztools-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 >>Github:https://github.com/tianhuzong
 >>Gitee:https://gitee.com/thzsen
 >>QQ:1485319167
 - - -
 >Tianhuzong开发的工具，方便在开发中使用
 1.0.2加入了加密解密内容：<kbd>RSA</kbd>,<kbd>AES</kbd>，<kbd>凯撒加密</kbd>
 - - -
->1.0.3版本中，引入了与ip地址有关的类<kbd>IP</kbd>
+>1.0.3版本中，修复了维吉尼亚密码的错误，引入了与ip地址有关的类<kbd>IP</kbd>
+- - -
+>1.0.4版本中，新增了检测ip是否为合法的IPv4
 - - -
 ##使用方法：
 - - -
 ####安装模块
 ```bash
 pip install thztools
 ```
@@ -78,13 +80,13 @@
 ```
 
 下面是使用ip模块的类的用法
 
 ```python
 from thztools.ip import *
 ip = IP()
-
+#请注意，输入的ip应为IPv4地址
 #IP地址的基本信息
 infomation = ip.jbxx(ip = '192.0.2.0')
 #ip地理位置
 geo = ip.geo(ip = '8.8.8.8')
 ```
```

### Comparing `thztools-1.0.3/setup.py` & `thztools-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 with open("./README.md",mode='r',encoding='utf-8') as f:
     des = f.read()
 setup(
     name="thztools",      # 包名，用于安装和调用该包
-    version="1.0.3",               # 版本号
+    version="1.0.4",               # 版本号
     author="Sen",
     description="由天狐宗开发的工具，方便开发时使用",
     long_description=des,
     long_description_content_type='text/markdown',
     author_email="tianhuzong@qq.com",
     url="https://github.com/tianhuzong/thztools",
     license="MIT",
```

### Comparing `thztools-1.0.3/thztools/ip.py` & `thztools-1.0.4/thztools/ip.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,50 @@
 from twoip import TwoIP
+import socket
 twoip = TwoIP(key = None)
 class IP:
+    def __is_ipv4(self,ip:str) -> bool:
+            try:
+                # 将地址转换为二进制表示
+                socket.inet_aton(ip)
+                # 如果转换成功，则说明该字符串是合法的 IPv4 地址
+                return True
+            except socket.error:
+                return False
     def jbxx(self , ip : str) -> dict:
         """
         获取一个ip的基本信息
         'ip'：表示查询到的 IP 地址。
         'ip_range_start' 和 'ip_range_end'：分别表示该 IP 地址所处的 IP 范围的起始和结束地址。
         'mask'：表示子网掩码的位数。
         'name_ripe' 和 'name_rus'：分别表示英文和俄文形式的公司名称或组织名称。
         'route'：表示与 IP 地址相关联的路由。
         Args:
             ip : (str) 一个合法的IPv4地址
         Return:
             返回这个ip的基本信息
+        Error:
+            如果填入的ip不是合法的IPv4，则会报错
         """
+        if self.__is_ipv4(ip) == False:
+            raise ValueError(f'{ip}不是合法的IPv4地址')
         re = twoip.provider(ip=ip)
         return re
     def geo(self,ip : str) -> dict:
         """
         返回一个ip地址的地理位置等信息
         'ip'：表示查询到的 IP 地址。
         'country' 和 'country_rus' 和 'country_ua'：分别表示英文、俄文和乌克兰文形式的国家名称。
         'country_code'：表示该 IP 地址所属国家的 ISO 3166-1 alpha-2 代码。
         'region'、'region_rus' 和 'region_ua'：分别表示英文、俄文和乌克兰文形式的区域或州的名称。
         'city'：表示城市名称。
         'zip_code'：表示邮政编码
         'latitude' 和 'longitude'：表示该 IP 地址的纬度和经度。
         'time_zone'：表示该地的时区。
+        Error:
+            如果填入的ip不是合法的IPv4，则会报错
         """
+        if self.__is_ipv4(ip) == False:
+            raise ValueError(f'{ip}不是合法的IPv4地址')
         re = twoip.geo(ip = ip)
         return re
```

### Comparing `thztools-1.0.3/thztools/jiami.py` & `thztools-1.0.4/thztools/jiami.py`

 * *Files identical despite different names*

### Comparing `thztools-1.0.3/thztools.egg-info/PKG-INFO` & `thztools-1.0.4/thztools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thztools
-Version: 1.0.3
+Version: 1.0.4
 Summary: 由天狐宗开发的工具，方便开发时使用
 Home-page: https://github.com/tianhuzong/thztools
 Author: Sen
 Author-email: tianhuzong@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,17 @@
 >>Github:https://github.com/tianhuzong
 >>Gitee:https://gitee.com/thzsen
 >>QQ:1485319167
 - - -
 >Tianhuzong开发的工具，方便在开发中使用
 1.0.2加入了加密解密内容：<kbd>RSA</kbd>,<kbd>AES</kbd>，<kbd>凯撒加密</kbd>
 - - -
->1.0.3版本中，引入了与ip地址有关的类<kbd>IP</kbd>
+>1.0.3版本中，修复了维吉尼亚密码的错误，引入了与ip地址有关的类<kbd>IP</kbd>
+- - -
+>1.0.4版本中，新增了检测ip是否为合法的IPv4
 - - -
 ##使用方法：
 - - -
 ####安装模块
 ```bash
 pip install thztools
 ```
@@ -91,13 +93,13 @@
 ```
 
 下面是使用ip模块的类的用法
 
 ```python
 from thztools.ip import *
 ip = IP()
-
+#请注意，输入的ip应为IPv4地址
 #IP地址的基本信息
 infomation = ip.jbxx(ip = '192.0.2.0')
 #ip地理位置
 geo = ip.geo(ip = '8.8.8.8')
 ```
```

