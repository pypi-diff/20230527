# Comparing `tmp/attacus-0.1.0-cp310-cp310-win_amd64.whl.zip` & `tmp/attacus-0.1.1-cp310-cp310-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,15 @@
-Zip file size: 898135 bytes, number of entries: 11
+Zip file size: 899932 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat       23 b- defN 23-May-26 10:35 attacus/__about__.py
--rw-rw-rw-  2.0 fat      161 b- defN 23-May-26 10:35 attacus/__init__.py
+-rw-rw-rw-  2.0 fat      165 b- defN 23-May-27 06:52 attacus/__init__.py
 -rw-rw-rw-  2.0 fat      189 b- defN 23-May-26 08:44 attacus/app.py
--rw-rw-rw-  2.0 fat  2273280 b- defN 23-May-26 10:49 attacus/attacus.pyd
+-rw-rw-rw-  2.0 fat     2395 b- defN 23-May-27 06:55 attacus/artifacts.py
+-rw-rw-rw-  2.0 fat  2275328 b- defN 23-May-27 08:20 attacus/attacus.pyd
 -rw-rw-rw-  2.0 fat     1650 b- defN 23-May-26 09:47 attacus/ensure.py
--rw-rw-rw-  2.0 fat      323 b- defN 23-May-25 13:01 attacus/flutter_view.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-26 10:50 attacus-0.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     5047 b- defN 23-May-26 10:50 attacus-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-May-26 10:50 attacus-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-26 10:50 attacus-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      838 b- defN 23-May-26 10:50 attacus-0.1.0.dist-info/RECORD
-11 files, 2282712 bytes uncompressed, 896735 bytes compressed:  60.7%
+-rw-rw-rw-  2.0 fat      365 b- defN 23-May-27 08:25 attacus/flutter_config.py
+-rw-rw-rw-  2.0 fat      355 b- defN 23-May-27 08:23 attacus/flutter_view.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-27 08:52 attacus-0.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     5082 b- defN 23-May-27 08:52 attacus-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-May-27 08:52 attacus-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-27 08:52 attacus-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      996 b- defN 23-May-27 08:52 attacus-0.1.1.dist-info/RECORD
+13 files, 2287749 bytes uncompressed, 898290 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -3,32 +3,38 @@
 
 Filename: attacus/__init__.py
 Comment: 
 
 Filename: attacus/app.py
 Comment: 
 
+Filename: attacus/artifacts.py
+Comment: 
+
 Filename: attacus/attacus.pyd
 Comment: 
 
 Filename: attacus/ensure.py
 Comment: 
 
+Filename: attacus/flutter_config.py
+Comment: 
+
 Filename: attacus/flutter_view.py
 Comment: 
 
-Filename: attacus-0.1.0.dist-info/LICENSE
+Filename: attacus-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: attacus-0.1.0.dist-info/METADATA
+Filename: attacus-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: attacus-0.1.0.dist-info/WHEEL
+Filename: attacus-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: attacus-0.1.0.dist-info/top_level.txt
+Filename: attacus-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: attacus-0.1.0.dist-info/RECORD
+Filename: attacus-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## attacus/__init__.py

```diff
@@ -1,8 +1,7 @@
-from .ensure import ensure
-ensure()
+from .artifacts import ensure ; ensure()
 from .attacus import *
 
 from .app import App
 from .flutter_view import FlutterView
 
 __all__ = ["App", "FlutterView"]
```

## attacus/flutter_view.py

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from importlib import resources
 
+from loguru import logger
+
 #from .attacus import *
 from . import attacus as core
+from .flutter_config import FlutterConfig
 
 class FlutterView(core.FlutterView):
-    def __init__(self, app :core.App) -> None:
-        super().__init__(app)
-        self.icu_data_path = str(resources.path('attacus', 'icudtl.dat'))
-        
-
+    def __init__(self, app :core.App, config: FlutterConfig = FlutterConfig()) -> None:
+        super().__init__(app, config)
```

## Comparing `attacus-0.1.0.dist-info/LICENSE` & `attacus-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `attacus-0.1.0.dist-info/METADATA` & `attacus-0.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attacus
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Flutter Extension
 Author-email: Kurtis Fields <kurtisfields@gmail.com>
 License: MIT License        
         Copyright (c) 2023 Kurtis Fields        
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -33,14 +33,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru (==0.7.0)
 Requires-Dist: platformdirs (==3.5.1)
+Requires-Dist: requests (==2.31.0)
 Provides-Extra: dev
 Requires-Dist: black (~=22.12.0) ; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest (~=7.2.1) ; extra == 'test'
 
 # Attacus :butterfly: :snake:
```

## Comparing `attacus-0.1.0.dist-info/RECORD` & `attacus-0.1.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 attacus/__about__.py,sha256=ryAfvAaW7VM8g1gnCrFCPrXmcbbm99Xw44aLkwGZzaI,23
-attacus/__init__.py,sha256=-rNerZJis5PyeoFqUU-CiMh4OsH6bOxLwl87pM0DkFo,161
+attacus/__init__.py,sha256=aJCUEMMOC7CoN0HXU20S5egMwzY1teojhDwcDsSWfCU,165
 attacus/app.py,sha256=qdfUm8sRao1JsrGJplAVsa5xVeqco2LRQO0PzbBuFHU,189
-attacus/attacus.pyd,sha256=_Lp3U_oAnlVct7iz7L0h49N2F5fCenjZhSgM_CgFGhI,2273280
+attacus/artifacts.py,sha256=EuYkYmytD5ol7KPYiUUoWS5nN7iQv-Zjm8HUzJ0bnkQ,2395
+attacus/attacus.pyd,sha256=Nh2i7mj56vWCv9SA68CNMhTG47XenHGqYxT2zNbuvtc,2275328
 attacus/ensure.py,sha256=ZvRjcirqcu6us-WqDGTWqY314_j31xsb4K-5_P3c0iM,1650
-attacus/flutter_view.py,sha256=fDuq0vVfngbCsWalxoKoo__BfPxooz8LjRrAQwGbuGU,323
-attacus-0.1.0.dist-info/LICENSE,sha256=_66BWzWzllOL6nPR0Jn9JDr5IFHvfOCeTUBcY-IAOR8,1091
-attacus-0.1.0.dist-info/METADATA,sha256=yltSgtpvKfW2vbV6jSUN85xbA_0PV3i_DPD_0f975k4,5047
-attacus-0.1.0.dist-info/WHEEL,sha256=W26pYN7HLsBT1jrDSL9udgf_mdNKJmYmL23sIP-FcgM,102
-attacus-0.1.0.dist-info/top_level.txt,sha256=MzO2IQ9x5yLfi1noaf99pmzxRu3h7OczbuZKytaFjUI,8
-attacus-0.1.0.dist-info/RECORD,,
+attacus/flutter_config.py,sha256=0ERLbiaKTHwliVQAxdoNRY_-YnzeAjlhPU4cxIc-wQs,365
+attacus/flutter_view.py,sha256=lFA-0N8qlBcyogR_aHvVUETf_F6YBIboYSW5b8UXBQU,355
+attacus-0.1.1.dist-info/LICENSE,sha256=_66BWzWzllOL6nPR0Jn9JDr5IFHvfOCeTUBcY-IAOR8,1091
+attacus-0.1.1.dist-info/METADATA,sha256=23E1qx_hWE3_tYbohIbsWhA2X6jUt3fruAgl8b_Vc6M,5082
+attacus-0.1.1.dist-info/WHEEL,sha256=W26pYN7HLsBT1jrDSL9udgf_mdNKJmYmL23sIP-FcgM,102
+attacus-0.1.1.dist-info/top_level.txt,sha256=MzO2IQ9x5yLfi1noaf99pmzxRu3h7OczbuZKytaFjUI,8
+attacus-0.1.1.dist-info/RECORD,,
```

