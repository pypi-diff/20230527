# Comparing `tmp/yao-0.0.4.tar.gz` & `tmp/yao-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yao-0.0.4.tar", last modified: Thu May  4 08:17:21 2023, max compression
+gzip compressed data, was "yao-0.0.5.tar", last modified: Sat May 27 09:16:22 2023, max compression
```

## Comparing `yao-0.0.4.tar` & `yao-0.0.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.041536 yao-0.0.4/
--rw-r--r--   0 ke         (501) wheel        (0)      433 2023-05-04 08:17:21.041359 yao-0.0.4/PKG-INFO
--rw-r--r--   0 ke         (501) wheel        (0)       38 2023-05-04 08:17:21.041583 yao-0.0.4/setup.cfg
--rw-r--r--   0 ke         (501) wheel        (0)      971 2023-05-04 08:10:53.000000 yao-0.0.4/setup.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.035617 yao-0.0.4/yao/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.4/yao/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)    19246 2023-04-18 07:31:04.000000 yao-0.0.4/yao/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     2211 2023-04-18 07:31:04.000000 yao-0.0.4/yao/db.py
--rw-r--r--   0 ke         (501) wheel        (0)     8279 2023-05-04 06:26:02.000000 yao-0.0.4/yao/depends.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.036791 yao-0.0.4/yao/function/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/__init__.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.037446 yao-0.0.4/yao/function/annex/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/annex/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      187 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/annex/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)    11202 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/annex/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1411 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/annex/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.038024 yao-0.0.4/yao/function/appointment/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/appointment/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)     1202 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/appointment/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4419 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/appointment/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1054 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/appointment/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.038590 yao-0.0.4/yao/function/company/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/company/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      192 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/company/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4071 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/company/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1249 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/company/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.039163 yao-0.0.4/yao/function/department/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/department/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      189 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/department/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4451 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/department/main.py
--rw-r--r--   0 ke         (501) wheel        (0)      992 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/department/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.039924 yao-0.0.4/yao/function/log/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/log/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      169 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/log/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     3314 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/log/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1394 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/log/schema.py
--rw-r--r--   0 ke         (501) wheel        (0)      665 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     7973 2023-04-21 10:39:40.000000 yao-0.0.4/yao/function/model.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.040589 yao-0.0.4/yao/function/permission/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/permission/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      199 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/permission/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     8271 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/permission/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     2045 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/permission/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.041151 yao-0.0.4/yao/function/user/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/user/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)     1364 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/user/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)    11188 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/user/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     3083 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/user/schema.py
--rw-r--r--   0 ke         (501) wheel        (0)     6842 2023-04-18 07:31:04.000000 yao-0.0.4/yao/helpers.py
--rw-r--r--   0 ke         (501) wheel        (0)    11459 2023-04-18 07:31:04.000000 yao-0.0.4/yao/method.py
--rw-r--r--   0 ke         (501) wheel        (0)     1868 2023-04-26 09:42:16.000000 yao-0.0.4/yao/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.036312 yao-0.0.4/yao.egg-info/
--rw-r--r--   0 ke         (501) wheel        (0)      433 2023-05-04 08:17:21.000000 yao-0.0.4/yao.egg-info/PKG-INFO
--rw-r--r--   0 ke         (501) wheel        (0)     1164 2023-05-04 08:17:21.000000 yao-0.0.4/yao.egg-info/SOURCES.txt
--rw-r--r--   0 ke         (501) wheel        (0)        1 2023-05-04 08:17:21.000000 yao-0.0.4/yao.egg-info/dependency_links.txt
--rw-r--r--   0 ke         (501) wheel        (0)      166 2023-05-04 08:17:21.000000 yao-0.0.4/yao.egg-info/requires.txt
--rw-r--r--   0 ke         (501) wheel        (0)        4 2023-05-04 08:17:21.000000 yao-0.0.4/yao.egg-info/top_level.txt
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.079466 yao-0.0.5/
+-rw-r--r--   0 ke         (501) wheel        (0)      433 2023-05-27 09:16:22.079286 yao-0.0.5/PKG-INFO
+-rw-r--r--   0 ke         (501) wheel        (0)       38 2023-05-27 09:16:22.079511 yao-0.0.5/setup.cfg
+-rw-r--r--   0 ke         (501) wheel        (0)      971 2023-05-27 09:06:21.000000 yao-0.0.5/setup.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.073092 yao-0.0.5/yao/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.5/yao/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)    19302 2023-05-06 07:07:58.000000 yao-0.0.5/yao/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2211 2023-05-04 09:42:20.000000 yao-0.0.5/yao/db.py
+-rw-r--r--   0 ke         (501) wheel        (0)     8279 2023-05-04 09:42:20.000000 yao-0.0.5/yao/depends.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.074530 yao-0.0.5/yao/function/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/__init__.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.075098 yao-0.0.5/yao/function/annex/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/annex/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      187 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/annex/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11202 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/annex/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1411 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/annex/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.075644 yao-0.0.5/yao/function/appointment/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/appointment/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1202 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/appointment/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4419 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/appointment/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1054 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/appointment/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.076218 yao-0.0.5/yao/function/company/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/company/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      192 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/company/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4071 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/company/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1249 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/company/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.076724 yao-0.0.5/yao/function/department/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/department/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      189 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/department/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4451 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/department/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)      992 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/department/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.077265 yao-0.0.5/yao/function/log/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/log/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      169 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/log/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     3314 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/log/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1394 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/log/schema.py
+-rw-r--r--   0 ke         (501) wheel        (0)      665 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     7973 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/model.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.078173 yao-0.0.5/yao/function/permission/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/permission/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      199 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/permission/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     8271 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/permission/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2045 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/permission/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.078749 yao-0.0.5/yao/function/user/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/user/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1364 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/user/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11188 2023-05-27 08:54:40.000000 yao-0.0.5/yao/function/user/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     3083 2023-05-04 09:42:20.000000 yao-0.0.5/yao/function/user/schema.py
+-rw-r--r--   0 ke         (501) wheel        (0)     6842 2023-05-04 09:42:20.000000 yao-0.0.5/yao/helpers.py
+-rw-r--r--   0 ke         (501) wheel        (0)    12051 2023-05-08 03:05:36.000000 yao-0.0.5/yao/method.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2062 2023-05-12 09:17:23.000000 yao-0.0.5/yao/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-27 09:16:22.074075 yao-0.0.5/yao.egg-info/
+-rw-r--r--   0 ke         (501) wheel        (0)      433 2023-05-27 09:16:22.000000 yao-0.0.5/yao.egg-info/PKG-INFO
+-rw-r--r--   0 ke         (501) wheel        (0)     1164 2023-05-27 09:16:22.000000 yao-0.0.5/yao.egg-info/SOURCES.txt
+-rw-r--r--   0 ke         (501) wheel        (0)        1 2023-05-27 09:16:22.000000 yao-0.0.5/yao.egg-info/dependency_links.txt
+-rw-r--r--   0 ke         (501) wheel        (0)      166 2023-05-27 09:16:22.000000 yao-0.0.5/yao.egg-info/requires.txt
+-rw-r--r--   0 ke         (501) wheel        (0)        4 2023-05-27 09:16:22.000000 yao-0.0.5/yao.egg-info/top_level.txt
```

### Comparing `yao-0.0.4/setup.py` & `yao-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="yao",
-    version="0.0.4",
+    version="0.0.5",
     description="Dev",
     python_requires=">=3.9",
     author="Lsshu",
     author_email="admin@lsshu.cn",
     url="https://github.com/lsshu/yao",
     packages=find_packages(),
     long_description=long_description,
```

### Comparing `yao-0.0.4/yao/crud.py` & `yao-0.0.5/yao/crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,35 +411,36 @@
         response = [session.delete(u) for u in self.query.all()] if event else self.query.delete()
 
         commit and session.commit()
         close and session.close()
         return response
 
     def update_or_store_model(self, session, where=None, item: BaseModel = None, data: dict = None, commit: bool = True, refresh: bool = True, close: bool = False,
-                              exclude_unset: bool = True, update_event: bool = False, **kwargs):
+                              exclude_unset: bool = True, event: bool = False, update_event: bool = False, **kwargs):
         """
         更新或者创建
         :param session:
         :param where:
         :param item:
         :param data:
         :param commit:
         :param refresh:
         :param close:
         :param exclude_unset:
+        :param event:
         :param update_event:
         :param kwargs:
         :return:
         """
         instance = self.first(session=session, where=where, **kwargs)
         if instance:
             return self.update(session=session, item=item, data=data, pk=getattr(instance, self.model_pk), exclude_unset=exclude_unset, commit=commit, refresh=refresh, close=close,
                                event=update_event, **kwargs)
         else:
-            return self.store(session=session, item=item, data=data, commit=commit, refresh=refresh, close=close, **kwargs)
+            return self.store(session=session, item=item, data=data, commit=commit, refresh=refresh, close=close, event=event, **kwargs)
 
     def find_or_store_model(self, session, where=None, item: BaseModel = None, data: dict = None, commit: bool = True, refresh: bool = True, close: bool = False, **kwargs):
         """
         查找或者创建
         :param session:
         :param where:
         :param item:
```

### Comparing `yao-0.0.4/yao/db.py` & `yao-0.0.5/yao/db.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/depends.py` & `yao-0.0.5/yao/depends.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/function/annex/main.py` & `yao-0.0.5/yao/function/annex/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/function/annex/schema.py` & `yao-0.0.5/yao/function/annex/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/function/appointment/crud.py` & `yao-0.0.5/yao/function/appointment/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/function/appointment/main.py` & `yao-0.0.5/yao/function/appointment/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/function/appointment/schema.py` & `yao-0.0.5/yao/function/appointment/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/function/company/main.py` & `yao-0.0.5/yao/function/company/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/function/company/schema.py` & `yao-0.0.5/yao/function/company/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/function/department/main.py` & `yao-0.0.5/yao/function/department/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/function/department/schema.py` & `yao-0.0.5/yao/function/department/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/function/log/main.py` & `yao-0.0.5/yao/function/log/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/function/log/schema.py` & `yao-0.0.5/yao/function/log/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/function/main.py` & `yao-0.0.5/yao/function/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/function/model.py` & `yao-0.0.5/yao/function/model.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/function/permission/main.py` & `yao-0.0.5/yao/function/permission/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/function/permission/schema.py` & `yao-0.0.5/yao/function/permission/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/function/user/crud.py` & `yao-0.0.5/yao/function/user/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/function/user/main.py` & `yao-0.0.5/yao/function/user/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/function/user/schema.py` & `yao-0.0.5/yao/function/user/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/helpers.py` & `yao-0.0.5/yao/helpers.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.4/yao/method.py` & `yao-0.0.5/yao/method.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import hashlib
 import os
 import random
 import re
 import socket
 import uuid
 import zipfile
+import datetime
 
 
 def hashids_encode(ids: str, **kwargs):
     """
     hashids 加密
     :param ids:
     :param kwargs:
@@ -443,7 +444,24 @@
     :param content:
     :param str_dict:
     :return:
     """
     for item, value in str_dict.items():
         content = re.sub(item, value, content)
     return content
+
+
+def get_date_of_last_month(form="%Y-%m-%d"):
+    """
+    获取上月开始结束日期
+    :param form 返回值显示格式
+    :return: str，date tuple
+    """
+    today = datetime.date.today()
+    year = today.year
+    month = today.month
+    if month == 1:
+        begin_of_last_month = datetime.date(year - 1, 12, 1).strftime(form)
+    else:
+        begin_of_last_month = datetime.date(year, month - 1, 1).strftime(form)
+    end_of_last_month = (datetime.date(year, month, 1) + datetime.timedelta(-1)).strftime(form)
+    return begin_of_last_month, end_of_last_month
```

### Comparing `yao-0.0.4/yao/schema.py` & `yao-0.0.5/yao/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,27 +40,32 @@
 
 
 class SchemaPrefix(BaseModel):
     owns: Optional[str] = None
 
     @validator('owns')
     def p_owns(cls, name: str):
-        return name.split("@", 1)[1] if name else None
+        return name.split("@", 1)[1] if name and len(name.split("@", 1)) == 2 else name
 
 
 class SchemaPrefixNames(SchemaPrefix):
     name: Optional[str] = None
 
     @validator('name')
     def p_name(cls, name: str):
-        return name.split("@", 1)[1] if name else None
+        return name.split("@", 1)[1] if name and len(name.split("@", 1)) == 2 else name
 
 
 class SchemaParamsApi(SchemaPrefixNames):
     uuid: Optional[str] = None
 
     class Config:
         orm_mode = True
 
 
 class ModelUUIDS(BaseModel):
     uuids: List[str] = None
+
+
+class SchemasPrefixOwns(BaseModel):
+    prefix: Optional[str] = None  # 公司前缀
+    owns: Optional[str] = None  # 拥有
```

### Comparing `yao-0.0.4/yao.egg-info/SOURCES.txt` & `yao-0.0.5/yao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

