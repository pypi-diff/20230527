# Comparing `tmp/nonebot_plugin_access_control-0.4.1.tar.gz` & `tmp/nonebot_plugin_access_control-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_access_control-0.4.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_access_control-0.4.2.tar", max compression
```

## Comparing `nonebot_plugin_access_control-0.4.1.tar` & `nonebot_plugin_access_control-0.4.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1085 2022-07-09 13:18:24.594000 nonebot_plugin_access_control-0.4.1/LICENSE
--rw-r--r--   0        0        0      989 2023-03-29 08:10:57.793884 nonebot_plugin_access_control-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    18074 2023-03-11 14:39:35.351798 nonebot_plugin_access_control-0.4.1/README.MD
--rw-r--r--   0        0        0      940 2023-02-20 02:17:19.253347 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/__init__.py
--rw-r--r--   0        0        0     2046 2023-02-14 08:42:38.604899 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/access_control.py
--rw-r--r--   0        0        0      579 2023-02-14 06:33:57.256438 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/config.py
--rw-r--r--   0        0        0      248 2023-02-14 09:17:25.623083 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/errors.py
--rw-r--r--   0        0        0     2363 2023-02-14 08:19:30.714606 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/event_bus.py
--rw-r--r--   0        0        0    10443 2023-03-13 03:19:06.942840 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/matchers/__init__.py
--rw-r--r--   0        0        0     1005 2023-02-13 06:25:49.446680 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/matchers/handle_error.py
--rw-r--r--   0        0        0     3263 2023-02-14 08:59:49.704358 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/matchers/parser.py
--rw-r--r--   0        0        0     3693 2023-03-13 03:28:05.306313 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py
--rw-r--r--   0        0        0      172 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/models/__init__.py
--rw-r--r--   0        0        0      461 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/models/permission.py
--rw-r--r--   0        0        0     1754 2023-03-13 03:19:06.945840 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/models/rate_limit.py
--rw-r--r--   0        0        0      119 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/plugin_data.py
--rw-r--r--   0        0        0      159 2023-02-13 07:58:33.466319 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/__init__.py
--rw-r--r--   0        0        0     6559 2023-03-11 14:39:35.433802 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/base.py
--rw-r--r--   0        0        0        0 2023-02-13 08:30:50.046295 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/impl/__init__.py
--rw-r--r--   0        0        0     8257 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/impl/permission.py
--rw-r--r--   0        0        0    11109 2023-03-29 08:10:11.301176 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/impl/rate_limit.py
--rw-r--r--   0        0        0       31 2023-02-13 07:07:23.516417 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/interface/__init__.py
--rw-r--r--   0        0        0     1968 2023-02-14 08:42:38.593900 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/interface/base.py
--rw-r--r--   0        0        0     1630 2023-02-14 07:23:00.750461 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/interface/permission.py
--rw-r--r--   0        0        0     1645 2023-02-14 09:36:52.491018 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/interface/rate_limit.py
--rw-r--r--   0        0        0      680 2023-02-13 08:40:31.774931 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/interface/service.py
--rw-r--r--   0        0        0      334 2023-02-13 07:59:53.174308 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/interface/subservice_owner.py
--rw-r--r--   0        0        0      882 2023-02-14 07:23:39.399678 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/methods.py
--rw-r--r--   0        0        0     2392 2023-02-14 07:30:48.027513 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/nonebot.py
--rw-r--r--   0        0        0       36 2023-02-14 06:34:31.631671 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/permission/__init__.py
--rw-r--r--   0        0        0      224 2023-02-14 07:59:38.644831 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/permission/permission.py
--rw-r--r--   0        0        0      907 2023-02-13 07:53:46.438693 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/plugin.py
--rw-r--r--   0        0        0       68 2023-02-14 06:24:06.140463 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/rate_limit/__init__.py
--rw-r--r--   0        0        0      318 2023-02-14 09:29:28.023174 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/rate_limit/rule.py
--rw-r--r--   0        0        0      175 2023-02-14 09:34:25.555714 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/rate_limit/token.py
--rw-r--r--   0        0        0      840 2023-02-13 07:54:44.558096 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/subservice.py
--rw-r--r--   0        0        0     1645 2023-02-14 06:59:06.539473 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/subservice_owner.py
--rw-r--r--   0        0        0       26 2023-02-20 02:15:08.129834 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/subject/__init__.py
--rw-r--r--   0        0        0      501 2023-03-11 14:39:35.434800 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/subject/extractor/__init__.py
--rw-r--r--   0        0        0      681 2023-02-20 02:03:55.940528 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/subject/extractor/base.py
--rw-r--r--   0        0        0     1443 2023-02-20 02:14:18.251076 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/subject/extractor/union.py
--rw-r--r--   0        0        0        0 2022-12-10 06:08:59.849075 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/utils/__init__.py
--rw-r--r--   0        0        0      531 2023-03-13 03:19:06.948840 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/utils/session.py
--rw-r--r--   0        0        0      425 2023-02-20 04:34:52.815055 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/utils/superuser.py
--rw-r--r--   0        0        0     1015 2022-12-10 06:23:22.420137 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/utils/tree.py
--rw-r--r--   0        0        0      234 2023-02-20 02:14:18.267077 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control_kaiheila/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 01:49:13.238000 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control_kaiheila/subject/__init__.py
--rw-r--r--   0        0        0     1398 2023-03-11 14:39:35.402797 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control_kaiheila/subject/extractor/__init__.py
--rw-r--r--   0        0        0      324 2023-02-20 02:14:18.246077 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control_onebot/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 01:49:13.238036 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control_onebot/subject/__init__.py
--rw-r--r--   0        0        0       88 2023-02-20 02:08:23.170135 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control_onebot/subject/extractor/__init__.py
--rw-r--r--   0        0        0     1936 2023-03-11 14:39:35.464798 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control_onebot/subject/extractor/v11.py
--rw-r--r--   0        0        0     2350 2023-03-11 14:39:35.403797 nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control_onebot/subject/extractor/v12.py
--rw-r--r--   0        0        0    18493 1970-01-01 00:00:00.000000 nonebot_plugin_access_control-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-07-09 13:18:24.594000 nonebot_plugin_access_control-0.4.2/LICENSE
+-rw-r--r--   0        0        0      989 2023-05-27 05:12:28.758404 nonebot_plugin_access_control-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    18871 2023-05-27 05:36:59.303416 nonebot_plugin_access_control-0.4.2/README.MD
+-rw-r--r--   0        0        0      979 2023-05-27 05:06:59.270663 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/__init__.py
+-rw-r--r--   0        0        0     2046 2023-02-14 08:42:38.604899 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/access_control.py
+-rw-r--r--   0        0        0      579 2023-02-14 06:33:57.256438 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/config.py
+-rw-r--r--   0        0        0      248 2023-02-14 09:17:25.623083 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/errors.py
+-rw-r--r--   0        0        0     2363 2023-02-14 08:19:30.714606 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/event_bus.py
+-rw-r--r--   0        0        0    10443 2023-03-13 03:19:06.942840 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/matchers/__init__.py
+-rw-r--r--   0        0        0     1005 2023-02-13 06:25:49.446680 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/matchers/handle_error.py
+-rw-r--r--   0        0        0     3263 2023-02-14 08:59:49.704358 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/matchers/parser.py
+-rw-r--r--   0        0        0     3693 2023-03-13 03:28:05.306313 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py
+-rw-r--r--   0        0        0      172 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/models/__init__.py
+-rw-r--r--   0        0        0      461 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/models/permission.py
+-rw-r--r--   0        0        0     1754 2023-03-13 03:19:06.945840 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/models/rate_limit.py
+-rw-r--r--   0        0        0      119 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/plugin_data.py
+-rw-r--r--   0        0        0      159 2023-02-13 07:58:33.466319 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/__init__.py
+-rw-r--r--   0        0        0     6791 2023-05-27 05:06:59.271662 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/base.py
+-rw-r--r--   0        0        0        0 2023-02-13 08:30:50.046295 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/impl/__init__.py
+-rw-r--r--   0        0        0     8257 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/impl/permission.py
+-rw-r--r--   0        0        0    11920 2023-05-27 05:28:53.341561 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/impl/rate_limit.py
+-rw-r--r--   0        0        0       31 2023-02-13 07:07:23.516417 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/__init__.py
+-rw-r--r--   0        0        0     1968 2023-02-14 08:42:38.593900 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/base.py
+-rw-r--r--   0        0        0     1630 2023-02-14 07:23:00.750461 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/permission.py
+-rw-r--r--   0        0        0     1948 2023-05-27 05:06:59.272662 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/rate_limit.py
+-rw-r--r--   0        0        0      680 2023-02-13 08:40:31.774931 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/service.py
+-rw-r--r--   0        0        0      334 2023-02-13 07:59:53.174308 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/subservice_owner.py
+-rw-r--r--   0        0        0      882 2023-02-14 07:23:39.399678 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/methods.py
+-rw-r--r--   0        0        0     2392 2023-02-14 07:30:48.027513 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/nonebot.py
+-rw-r--r--   0        0        0       36 2023-02-14 06:34:31.631671 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/permission/__init__.py
+-rw-r--r--   0        0        0      224 2023-02-14 07:59:38.644831 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/permission/permission.py
+-rw-r--r--   0        0        0      907 2023-02-13 07:53:46.438693 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/plugin.py
+-rw-r--r--   0        0        0       74 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/rate_limit/__init__.py
+-rw-r--r--   0        0        0      318 2023-02-14 09:29:28.023174 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/rate_limit/rule.py
+-rw-r--r--   0        0        0      181 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/rate_limit/token.py
+-rw-r--r--   0        0        0      840 2023-02-13 07:54:44.558096 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/subservice.py
+-rw-r--r--   0        0        0     1645 2023-02-14 06:59:06.539473 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/subservice_owner.py
+-rw-r--r--   0        0        0       26 2023-02-20 02:15:08.129834 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/subject/__init__.py
+-rw-r--r--   0        0        0      501 2023-03-11 14:39:35.434800 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/subject/extractor/__init__.py
+-rw-r--r--   0        0        0      681 2023-02-20 02:03:55.940528 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/subject/extractor/base.py
+-rw-r--r--   0        0        0     1443 2023-02-20 02:14:18.251076 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/subject/extractor/union.py
+-rw-r--r--   0        0        0        0 2022-12-10 06:08:59.849075 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/utils/__init__.py
+-rw-r--r--   0        0        0      531 2023-03-13 03:19:06.948840 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/utils/session.py
+-rw-r--r--   0        0        0      425 2023-02-20 04:34:52.815055 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/utils/superuser.py
+-rw-r--r--   0        0        0     1015 2022-12-10 06:23:22.420137 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/utils/tree.py
+-rw-r--r--   0        0        0      234 2023-02-20 02:14:18.267077 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_kaiheila/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-20 01:49:13.238000 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_kaiheila/subject/__init__.py
+-rw-r--r--   0        0        0     1398 2023-03-11 14:39:35.402797 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_kaiheila/subject/extractor/__init__.py
+-rw-r--r--   0        0        0      324 2023-02-20 02:14:18.246077 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_onebot/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-20 01:49:13.238036 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_onebot/subject/__init__.py
+-rw-r--r--   0        0        0       88 2023-02-20 02:08:23.170135 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_onebot/subject/extractor/__init__.py
+-rw-r--r--   0        0        0     1936 2023-03-11 14:39:35.464798 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_onebot/subject/extractor/v11.py
+-rw-r--r--   0        0        0     2350 2023-03-11 14:39:35.403797 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_onebot/subject/extractor/v12.py
+-rw-r--r--   0        0        0    19263 1970-01-01 00:00:00.000000 nonebot_plugin_access_control-0.4.2/PKG-INFO
```

### Comparing `nonebot_plugin_access_control-0.4.1/LICENSE` & `nonebot_plugin_access_control-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/pyproject.toml` & `nonebot_plugin_access_control-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-access-control"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 license = "MIT"
 readme = "README.MD"
 repository = "https://github.com/ssttkkl/nonebot-plugin-access-control"
 packages = [
     { include = "nonebot_plugin_access_control", from = "src" },
```

### Comparing `nonebot_plugin_access_control-0.4.1/README.MD` & `nonebot_plugin_access_control-0.4.2/README.MD`

 * *Files 2% similar despite different names*

```diff
@@ -299,14 +299,41 @@
 对于非Matcher的功能入口（如APScheduler的定时任务等），需要开发者手动进行鉴权。
 
 - 方法一：调用`service.check(Bot, Event)`方法，传入Bot及Event实例，返回bool值表示该用户是否具有权限
 - 方法二：调用`service.check_by_subject(*str)`方法，传入主体字符串，返回bool值表示该用户是否具有权限
 
 APScheduler示例：[src/nonebot_plugin_ac_demo/apscheduler_demo.py](src/nonebot_plugin_ac_demo/apscheduler_demo.py)
 
+对于一些功能，如果希望在执行失败时不消耗限流次数，则需要开发者手动进行鉴权与限流。
+
+```python
+d_matcher = on_command('d')
+d_service = plugin_service.create_subservice('d')
+
+
+@d_matcher.handle()
+async def _(bot: Bot, event: Event, matcher: Matcher):
+    if not await d_service.check(bot, event, acquire_rate_limit_token=False):
+        # 没有权限
+        await matcher.finish()
+        
+    token = await d_service.acquire_token_for_rate_limit(bot, event)
+    if token is None:
+        # 已达到限流次数上线
+        await matcher.finish()
+    
+    ok = do_your_logic()
+    
+    if not ok:
+        # 功能执行失败时，收回限流消耗的次数
+        await token.retire()
+    
+    await matcher.send("c")
+```
+
 6. 事件订阅
 
 通过`service.on_set_permission`、`service.on_remove_permission`、`service.on_change_permission`方法可以订阅事件，具体如下表：
 
 | 装饰器                                 | 事件类型                                  | 事件接收函数的参数                   |
 |-------------------------------------|---------------------------------------|-----------------------------|
 | `service.on_set_permission`         | 服务设置主体权限                              | service：服务<br>permission：权限 |
```

#### html2text {}

```diff
@@ -132,15 +132,24 @@
 nonebot_plugin_ac_demo.c ``` 5. æå¨é´æ
 å¯¹äºéMatcherçåè½å¥å£ï¼å¦APSchedulerçå®æ¶ä»»å¡ç­ï¼ï¼éè¦å¼åèæå¨è¿è¡é´æã
 - æ¹æ³ä¸ï¼è°ç¨`service.check(Bot,
 Event)`æ¹æ³ï¼ä¼ å¥BotåEventå®ä¾ï¼è¿åboolå¼è¡¨ç¤ºè¯¥ç¨æ·æ¯å¦å·ææé
 - æ¹æ³äºï¼è°ç¨`service.check_by_subject
 (*str)`æ¹æ³ï¼ä¼ å¥ä¸»ä½å­ç¬¦ä¸²ï¼è¿åboolå¼è¡¨ç¤ºè¯¥ç¨æ·æ¯å¦å·ææé
 APSchedulerç¤ºä¾ï¼[src/nonebot_plugin_ac_demo/apscheduler_demo.py](src/
-nonebot_plugin_ac_demo/apscheduler_demo.py) 6. äºä»¶è®¢é
+nonebot_plugin_ac_demo/apscheduler_demo.py)
+å¯¹äºä¸äºåè½ï¼å¦æå¸æå¨æ§è¡å¤±è´¥æ¶ä¸æ¶èéæµæ¬¡æ°ï¼åéè¦å¼åèæå¨è¿è¡é´æä¸éæµã
+```python d_matcher = on_command('d') d_service =
+plugin_service.create_subservice('d') @d_matcher.handle() async def _(bot: Bot,
+event: Event, matcher: Matcher): if not await d_service.check(bot, event,
+acquire_rate_limit_token=False): # æ²¡ææé await matcher.finish() token =
+await d_service.acquire_token_for_rate_limit(bot, event) if token is None: #
+å·²è¾¾å°éæµæ¬¡æ°ä¸çº¿ await matcher.finish() ok = do_your_logic() if not
+ok: # åè½æ§è¡å¤±è´¥æ¶ï¼æ¶åéæµæ¶èçæ¬¡æ° await token.retire()
+await matcher.send("c") ``` 6. äºä»¶è®¢é
 éè¿`service.on_set_permission`ã`service.on_remove_permission`ã`service.on_change_permission`æ¹æ³å¯ä»¥è®¢éäºä»¶ï¼å·ä½å¦ä¸è¡¨ï¼
 | è£é¥°å¨ | äºä»¶ç±»å | äºä»¶æ¥æ¶å½æ°çåæ° | |-------------------
 ------------------|---------------------------------------|--------------------
 ---------| | `service.on_set_permission` | æå¡è®¾ç½®ä¸»ä½æé |
 serviceï¼æå¡
 permissionï¼æé | | `service.on_remove_permission` |
 æå¡å é¤ä¸»ä½æé | serviceï¼æå¡
```

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/__init__.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from nonebot import require
 
 require("nonebot_plugin_datastore")
+require("nonebot_plugin_apscheduler")
 
 from . import access_control
 from . import config
 from . import errors
 from . import event_bus
 from . import matchers
 from . import models
```

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/access_control.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/access_control.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/config.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/event_bus.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/event_bus.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/matchers/__init__.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/matchers/handle_error.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/matchers/handle_error.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/matchers/parser.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/matchers/parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/models/rate_limit.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/models/rate_limit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/base.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from nonebot import Bot
 from nonebot.internal.adapter import Event
 from nonebot.internal.matcher import Matcher
 
 from .impl.permission import ServicePermissionImpl
 from .impl.rate_limit import ServiceRateLimitImpl
 from .interface import IService
+from .interface.rate_limit import IRateLimitToken
 from .permission import Permission
 from .rate_limit import RateLimitRule
 from ..errors import AccessControlError, PermissionDeniedError, RateLimitedError
 from ..event_bus import T_Listener
 from ..subject import extract_subjects
 
 T_ParentService = TypeVar('T_ParentService', bound=Optional["Service"], covariant=True)
@@ -73,18 +74,17 @@
                 return False
 
         allow = await self.check_permission(*subjects)
         if not allow:
             raise PermissionDeniedError()
 
         if acquire_rate_limit_token:
-            user_id = subjects[0]
-            allow = await self.acquire_token_for_rate_limit(*subjects, user=user_id)
+            token = await self.acquire_token_for_rate_limit_by_subjects(*subjects)
 
-            if not allow:
+            if token is None:
                 raise RateLimitedError()
 
     def on_set_permission(self, func: Optional[T_Listener] = None):
         return self._permission_impl.on_set_permission(func)
 
     def on_change_permission(self, func: Optional[T_Listener] = None):
         return self._permission_impl.on_change_permission(func)
@@ -140,13 +140,16 @@
                                   limit: int, overwrite: bool = False) -> RateLimitRule:
         return await self._rate_limit_impl.add_rate_limit_rule(subject, time_span, limit, overwrite)
 
     @classmethod
     async def remove_rate_limit_rule(cls, rule_id: str) -> bool:
         return await ServiceRateLimitImpl.remove_rate_limit_rule(rule_id)
 
-    async def acquire_token_for_rate_limit(self, *subject: str, user: str) -> bool:
-        return await self._rate_limit_impl.acquire_token_for_rate_limit(*subject, user=user)
+    async def acquire_token_for_rate_limit(self, bot: Bot, event: Event) -> Optional[IRateLimitToken]:
+        return await self._rate_limit_impl.acquire_token_for_rate_limit(bot, event)
+
+    async def acquire_token_for_rate_limit_by_subjects(self, *subject: str) -> Optional[IRateLimitToken]:
+        return await self._rate_limit_impl.acquire_token_for_rate_limit_by_subjects(*subject)
 
     @classmethod
     async def clear_rate_limit_tokens(cls):
         return await ServiceRateLimitImpl.clear_rate_limit_tokens()
```

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/impl/permission.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/impl/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/impl/rate_limit.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/impl/rate_limit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 from datetime import datetime, timedelta
-from typing import AsyncGenerator, TypeVar, Generic
+from typing import AsyncGenerator, TypeVar, Generic, Collection
 from typing import Optional
 
-from nonebot import require, logger
+from apscheduler.triggers.interval import IntervalTrigger
+from nonebot import logger, Bot
+from nonebot.internal.adapter import Event
+from nonebot_plugin_apscheduler import scheduler
 from nonebot_plugin_datastore.db import get_engine
 from sqlalchemy import delete, select
 from sqlalchemy import func
 from sqlalchemy.ext.asyncio import AsyncSession
 
 from ..interface import IService
-from ..interface.rate_limit import IServiceRateLimit
-from ..rate_limit import RateLimitRule, RateLimitToken
+from ..interface.rate_limit import IServiceRateLimit, IRateLimitToken
+from ..rate_limit import RateLimitRule, RateLimitSingleToken
 from ...errors import AccessControlValueError
 from ...event_bus import T_Listener, EventType, on_event, fire_event
 from ...models import RateLimitTokenOrm, RateLimitRuleOrm
+from ...subject import extract_subjects
 from ...utils.session import use_session_or_create
 
 T_Service = TypeVar("T_Service", bound=IService)
 
 
+class RateLimitTokenImpl(IRateLimitToken):
+    def __init__(self, tokens: Collection[RateLimitSingleToken], service: "ServiceRateLimitImpl"):
+        self.tokens = tokens
+        self.service = service
+
+    async def retire(self):
+        async with AsyncSession(get_engine()) as sess:
+            for t in self.tokens:
+                await self.service._retire_token(t, session=sess)
+
+
 class ServiceRateLimitImpl(Generic[T_Service], IServiceRateLimit):
     def __init__(self, service: T_Service):
         self.service = service
 
     def on_add_rate_limit_rule(self, func: Optional[T_Listener] = None):
         return on_event(EventType.service_add_rate_limit_rule,
                         lambda service: service == self.service,
@@ -161,15 +176,15 @@
                                  orm.overwrite)
             await cls._fire_service_remove_rate_limit_rule(rule)
 
             return True
 
     @staticmethod
     async def _acquire_token(rule: RateLimitRule, user: str,
-                             *, session: Optional[AsyncSession] = None) -> Optional[RateLimitToken]:
+                             *, session: Optional[AsyncSession] = None) -> Optional[RateLimitSingleToken]:
         now = datetime.utcnow()
 
         async with use_session_or_create(session) as sess:
             stmt = select(func.count()).where(
                 RateLimitTokenOrm.rule_id == rule.id,
                 RateLimitTokenOrm.user == user,
                 RateLimitTokenOrm.acquire_time >= now - rule.time_span
@@ -181,73 +196,76 @@
 
             x = RateLimitTokenOrm(rule_id=rule.id, user=user)
             sess.add(x)
             await sess.commit()
 
             await sess.refresh(x)
 
-            return RateLimitToken(x.id, x.rule_id, x.user, x.acquire_time)
+            logger.trace(f"[rate limit] token acquired for rule {x.rule_id} by user {x.user} "
+                         f"(service: {rule.service})")
+
+            return RateLimitSingleToken(x.id, x.rule_id, x.user, x.acquire_time)
 
     @staticmethod
-    async def _retire_token(token: RateLimitToken, *, session: Optional[AsyncSession] = None):
+    async def _retire_token(token: RateLimitSingleToken, *, session: Optional[AsyncSession] = None):
         async with use_session_or_create(session) as sess:
             stmt = delete(RateLimitTokenOrm).where(RateLimitTokenOrm.id == token.id)
             await sess.execute(stmt)
             await sess.commit()
 
-    async def acquire_token_for_rate_limit(self, *subject: str, user: str,
-                                           session: Optional[AsyncSession] = None) -> bool:
+            logger.trace(f"[rate limit] token retired for rule {token.rule_id} by user {token.user}")
+
+    async def acquire_token_for_rate_limit(self, bot: Bot, event: Event) -> Optional[RateLimitTokenImpl]:
+        return await self.acquire_token_for_rate_limit_by_subjects(*extract_subjects(bot, event))
+
+    async def acquire_token_for_rate_limit_by_subjects(self, *subject: str,
+                                                       session: Optional[AsyncSession] = None) \
+            -> Optional[RateLimitTokenImpl]:
+        assert len(subject) > 0, "require at least one subject"
+        user = subject[0]
+
         async with use_session_or_create(session) as sess:
             tokens = []
 
             # 先获取所有rule，再对每个rule获取token
             rules = [x async for x in self.get_rate_limit_rules_by_subject(*subject, session=sess)]
             for rule in rules:
                 token = await self._acquire_token(rule, user, session=sess)
                 if token is not None:
-                    logger.trace(f"[rate limit] token acquired for rule {rule.id} "
-                                 f"(service: {rule.service}, subject: {rule.subject})")
                     tokens.append(token)
                 else:
                     logger.debug(f"[rate limit] limit reached for rule {rule.id} "
                                  f"(service: {rule.service}, subject: {rule.subject})")
                     for t in tokens:
                         await self._retire_token(t, session=sess)
-                        logger.trace(f"[rate limit] token retired for rule {rule.id} "
-                                     f"(service: {rule.service}, subject: {rule.subject})")
-                    return False
+                    return None
 
                 if rule.overwrite:
                     break
 
-            # 未设置rule
-            return True
+            return RateLimitTokenImpl(tokens, self)
 
     @classmethod
     async def clear_rate_limit_tokens(cls, *, session: Optional[AsyncSession] = None):
         async with use_session_or_create(session) as sess:
             stmt = delete(RateLimitTokenOrm)
             result = await sess.execute(stmt)
             await sess.commit()
             logger.debug(f"deleted {result.rowcount} rate limit token(s)")
 
 
-require('nonebot_plugin_apscheduler')
-from nonebot_plugin_apscheduler import scheduler
-
-
-@scheduler.scheduled_job("cron", minute="*/10", id="delete_outdated_tokens")
+@scheduler.scheduled_job(IntervalTrigger(minutes=10), id="delete_outdated_tokens")
 async def _delete_outdated_tokens():
     async with AsyncSession(get_engine()) as session:
         now = datetime.utcnow()
         stmts = []
         async for rule in await session.stream_scalars(select(RateLimitRuleOrm)):
             stmt = (delete(RateLimitTokenOrm)
                     .where(RateLimitTokenOrm.rule_id == rule.id,
-                           RateLimitTokenOrm.acquire_time < now + timedelta(seconds=rule.time_span))
+                           RateLimitTokenOrm.acquire_time < now - timedelta(seconds=rule.time_span))
                     .execution_options(synchronize_session=False))
             stmts.append(stmt)
 
         rowcount = 0
         for stmt in stmts:
             result = await session.execute(stmt)
             rowcount += result.rowcount
```

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/interface/base.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/interface/permission.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/interface/rate_limit.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/rate_limit.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 from abc import ABC, abstractmethod
 from datetime import timedelta
 from typing import AsyncGenerator, Optional
 
+from nonebot import Bot
+from nonebot.internal.adapter import Event
+
 from ..rate_limit import RateLimitRule
 from ...event_bus import T_Listener
 
 
+class IRateLimitToken:
+    async def retire(self):
+        ...
+
+
 class IServiceRateLimit(ABC):
     @abstractmethod
     def on_add_rate_limit_rule(self, func: Optional[T_Listener] = None):
         raise NotImplementedError()
 
     @abstractmethod
     def on_remove_rate_limit_rule(self, func: Optional[T_Listener] = None):
@@ -40,14 +48,18 @@
         ...
 
     @classmethod
     async def remove_rate_limit_rule(cls, rule_id: str) -> bool:
         ...
 
     @abstractmethod
-    async def acquire_token_for_rate_limit(self, *subject: str, user: str) -> bool:
+    async def acquire_token_for_rate_limit(self, bot: Bot, event: Event) -> Optional[IRateLimitToken]:
+        ...
+
+    @abstractmethod
+    async def acquire_token_for_rate_limit_by_subjects(self, *subject: str) -> Optional[IRateLimitToken]:
         ...
 
     @classmethod
     @abstractmethod
     async def clear_rate_limit_tokens(cls):
         ...
```

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/interface/service.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/methods.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/methods.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/nonebot.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/nonebot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/plugin.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/plugin.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/subservice.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/subservice.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/service/subservice_owner.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/subservice_owner.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/subject/extractor/base.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/subject/extractor/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/subject/extractor/union.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/subject/extractor/union.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/utils/session.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/utils/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control/utils/tree.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/utils/tree.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control_kaiheila/subject/extractor/__init__.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_kaiheila/subject/extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control_onebot/subject/extractor/v11.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_onebot/subject/extractor/v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/src/nonebot_plugin_access_control_onebot/subject/extractor/v12.py` & `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_onebot/subject/extractor/v12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.1/PKG-INFO` & `nonebot_plugin_access_control-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-access-control
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Home-page: https://github.com/ssttkkl/nonebot-plugin-access-control
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -320,14 +320,41 @@
 对于非Matcher的功能入口（如APScheduler的定时任务等），需要开发者手动进行鉴权。
 
 - 方法一：调用`service.check(Bot, Event)`方法，传入Bot及Event实例，返回bool值表示该用户是否具有权限
 - 方法二：调用`service.check_by_subject(*str)`方法，传入主体字符串，返回bool值表示该用户是否具有权限
 
 APScheduler示例：[src/nonebot_plugin_ac_demo/apscheduler_demo.py](src/nonebot_plugin_ac_demo/apscheduler_demo.py)
 
+对于一些功能，如果希望在执行失败时不消耗限流次数，则需要开发者手动进行鉴权与限流。
+
+```python
+d_matcher = on_command('d')
+d_service = plugin_service.create_subservice('d')
+
+
+@d_matcher.handle()
+async def _(bot: Bot, event: Event, matcher: Matcher):
+    if not await d_service.check(bot, event, acquire_rate_limit_token=False):
+        # 没有权限
+        await matcher.finish()
+        
+    token = await d_service.acquire_token_for_rate_limit(bot, event)
+    if token is None:
+        # 已达到限流次数上线
+        await matcher.finish()
+    
+    ok = do_your_logic()
+    
+    if not ok:
+        # 功能执行失败时，收回限流消耗的次数
+        await token.retire()
+    
+    await matcher.send("c")
+```
+
 6. 事件订阅
 
 通过`service.on_set_permission`、`service.on_remove_permission`、`service.on_change_permission`方法可以订阅事件，具体如下表：
 
 | 装饰器                                 | 事件类型                                  | 事件接收函数的参数                   |
 |-------------------------------------|---------------------------------------|-----------------------------|
 | `service.on_set_permission`         | 服务设置主体权限                              | service：服务<br>permission：权限 |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-access-control Version: 0.4.1
+Metadata-Version: 2.1 Name: nonebot-plugin-access-control Version: 0.4.2
 Summary: Home-page: https://github.com/ssttkkl/nonebot-plugin-access-control
 License: MIT Author: ssttkkl Author-email: huang.wen.long@hotmail.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot-
 plugin-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot-plugin-datastore
@@ -143,15 +143,24 @@
 nonebot_plugin_ac_demo.c ``` 5. æå¨é´æ
 å¯¹äºéMatcherçåè½å¥å£ï¼å¦APSchedulerçå®æ¶ä»»å¡ç­ï¼ï¼éè¦å¼åèæå¨è¿è¡é´æã
 - æ¹æ³ä¸ï¼è°ç¨`service.check(Bot,
 Event)`æ¹æ³ï¼ä¼ å¥BotåEventå®ä¾ï¼è¿åboolå¼è¡¨ç¤ºè¯¥ç¨æ·æ¯å¦å·ææé
 - æ¹æ³äºï¼è°ç¨`service.check_by_subject
 (*str)`æ¹æ³ï¼ä¼ å¥ä¸»ä½å­ç¬¦ä¸²ï¼è¿åboolå¼è¡¨ç¤ºè¯¥ç¨æ·æ¯å¦å·ææé
 APSchedulerç¤ºä¾ï¼[src/nonebot_plugin_ac_demo/apscheduler_demo.py](src/
-nonebot_plugin_ac_demo/apscheduler_demo.py) 6. äºä»¶è®¢é
+nonebot_plugin_ac_demo/apscheduler_demo.py)
+å¯¹äºä¸äºåè½ï¼å¦æå¸æå¨æ§è¡å¤±è´¥æ¶ä¸æ¶èéæµæ¬¡æ°ï¼åéè¦å¼åèæå¨è¿è¡é´æä¸éæµã
+```python d_matcher = on_command('d') d_service =
+plugin_service.create_subservice('d') @d_matcher.handle() async def _(bot: Bot,
+event: Event, matcher: Matcher): if not await d_service.check(bot, event,
+acquire_rate_limit_token=False): # æ²¡ææé await matcher.finish() token =
+await d_service.acquire_token_for_rate_limit(bot, event) if token is None: #
+å·²è¾¾å°éæµæ¬¡æ°ä¸çº¿ await matcher.finish() ok = do_your_logic() if not
+ok: # åè½æ§è¡å¤±è´¥æ¶ï¼æ¶åéæµæ¶èçæ¬¡æ° await token.retire()
+await matcher.send("c") ``` 6. äºä»¶è®¢é
 éè¿`service.on_set_permission`ã`service.on_remove_permission`ã`service.on_change_permission`æ¹æ³å¯ä»¥è®¢éäºä»¶ï¼å·ä½å¦ä¸è¡¨ï¼
 | è£é¥°å¨ | äºä»¶ç±»å | äºä»¶æ¥æ¶å½æ°çåæ° | |-------------------
 ------------------|---------------------------------------|--------------------
 ---------| | `service.on_set_permission` | æå¡è®¾ç½®ä¸»ä½æé |
 serviceï¼æå¡
 permissionï¼æé | | `service.on_remove_permission` |
 æå¡å é¤ä¸»ä½æé | serviceï¼æå¡
```

