# Comparing `tmp/gs_engine-0.22.0a20230526-py2.py3-none-macosx_11_0_x86_64.whl.zip` & `tmp/gs_engine-0.22.0a20230527-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11906 bytes, number of entries: 9
--rw-r--r--  2.0 unx      694 b- defN 23-May-26 19:10 graphscope_runtime/__init__.py
--rw-r--r--  2.0 unx     1573 b- defN 23-May-26 19:10 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      398 b- defN 23-May-26 19:10 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      504 b- defN 23-May-26 19:10 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx      204 b- defN 23-May-26 19:10 graphscope.runtime/conf/log4rs.yml
--rw-rw-r--  2.0 unx      840 b- defN 23-May-26 21:09 gs_engine-0.22.0a20230526.dist-info/RECORD
--rw-r--r--  2.0 unx      140 b- defN 23-May-26 20:58 gs_engine-0.22.0a20230526.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-May-26 20:58 gs_engine-0.22.0a20230526.dist-info/top_level.txt
--rw-r--r--  2.0 unx    21664 b- defN 23-May-26 20:58 gs_engine-0.22.0a20230526.dist-info/METADATA
-9 files, 26036 bytes uncompressed, 10444 bytes compressed:  59.9%
+Zip file size: 11885 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      398 b- defN 23-May-27 19:02 graphscope.runtime/conf/executor.vineyard.properties
+-rw-r--r--  2.0 unx      504 b- defN 23-May-27 19:02 graphscope.runtime/conf/frontend.vineyard.properties
+-rw-r--r--  2.0 unx     1573 b- defN 23-May-27 19:02 graphscope.runtime/conf/log4j2.xml
+-rw-r--r--  2.0 unx      204 b- defN 23-May-27 19:02 graphscope.runtime/conf/log4rs.yml
+-rw-r--r--  2.0 unx      694 b- defN 23-May-27 19:02 graphscope_runtime/__init__.py
+-rw-r--r--  2.0 unx    21664 b- defN 23-May-27 20:34 gs_engine-0.22.0a20230527.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-27 20:34 gs_engine-0.22.0a20230527.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-May-27 20:34 gs_engine-0.22.0a20230527.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      831 b- defN 23-May-27 20:34 gs_engine-0.22.0a20230527.dist-info/RECORD
+9 files, 25997 bytes uncompressed, 10423 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
-Filename: graphscope_runtime/__init__.py
+Filename: graphscope.runtime/conf/executor.vineyard.properties
 Comment: 
 
-Filename: graphscope.runtime/conf/log4j2.xml
+Filename: graphscope.runtime/conf/frontend.vineyard.properties
 Comment: 
 
-Filename: graphscope.runtime/conf/executor.vineyard.properties
+Filename: graphscope.runtime/conf/log4j2.xml
 Comment: 
 
-Filename: graphscope.runtime/conf/frontend.vineyard.properties
+Filename: graphscope.runtime/conf/log4rs.yml
 Comment: 
 
-Filename: graphscope.runtime/conf/log4rs.yml
+Filename: graphscope_runtime/__init__.py
 Comment: 
 
-Filename: gs_engine-0.22.0a20230526.dist-info/RECORD
+Filename: gs_engine-0.22.0a20230527.dist-info/METADATA
 Comment: 
 
-Filename: gs_engine-0.22.0a20230526.dist-info/WHEEL
+Filename: gs_engine-0.22.0a20230527.dist-info/WHEEL
 Comment: 
 
-Filename: gs_engine-0.22.0a20230526.dist-info/top_level.txt
+Filename: gs_engine-0.22.0a20230527.dist-info/top_level.txt
 Comment: 
 
-Filename: gs_engine-0.22.0a20230526.dist-info/METADATA
+Filename: gs_engine-0.22.0a20230527.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gs_engine-0.22.0a20230526.dist-info/RECORD` & `gs_engine-0.22.0a20230527.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-graphscope_runtime/__init__.py,sha256=w_Me0NHI5zy8GitMCD7mzOi0Qz7ZfeE2zUI5wGfZIyM,694
-graphscope.runtime/conf/log4j2.xml,sha256=JiMUDFQ779aE33kOkah4-VlGQqMVW1_xlzWVZsvhHWQ,1573
-graphscope.runtime/conf/executor.vineyard.properties,sha256=FX6Og8G2x4VrMvdtT-XGjTsDGkY0iTWrLlNUg2aFX6o,398
-graphscope.runtime/conf/frontend.vineyard.properties,sha256=eIDnFSXj53FD5KWKOg_keg6pA-OrNUg9BsQP-gxslHU,504
-graphscope.runtime/conf/log4rs.yml,sha256=jFXF2AwsTarQhUr2vH4qD9-TJGdY2vVbvBtGYm-fotM,204
-gs_engine-0.22.0a20230526.dist-info/RECORD,,
-gs_engine-0.22.0a20230526.dist-info/WHEEL,sha256=fw_hGi-Yx84a3ggAIzpSq5odRE77o5K1cXAmZvJuyLk,140
-gs_engine-0.22.0a20230526.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
-gs_engine-0.22.0a20230526.dist-info/METADATA,sha256=Ls7_B2i07MtFoQ6HMXDI7ALLqnaY5fyDMWcNrxhEmy4,21664
+graphscope.runtime/conf/executor.vineyard.properties,sha256=FX6Og8G2x4VrMvdtT-XGjTsDGkY0iTWrLlNUg2aFX6o,398
+graphscope.runtime/conf/frontend.vineyard.properties,sha256=eIDnFSXj53FD5KWKOg_keg6pA-OrNUg9BsQP-gxslHU,504
+graphscope.runtime/conf/log4j2.xml,sha256=JiMUDFQ779aE33kOkah4-VlGQqMVW1_xlzWVZsvhHWQ,1573
+graphscope.runtime/conf/log4rs.yml,sha256=jFXF2AwsTarQhUr2vH4qD9-TJGdY2vVbvBtGYm-fotM,204
+graphscope_runtime/__init__.py,sha256=w_Me0NHI5zy8GitMCD7mzOi0Qz7ZfeE2zUI5wGfZIyM,694
+gs_engine-0.22.0a20230527.dist-info/METADATA,sha256=fnOFTAHBOQaivyl-AUPJk2IFSEED_5iahwKtThK2ItU,21664
+gs_engine-0.22.0a20230527.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+gs_engine-0.22.0a20230527.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
+gs_engine-0.22.0a20230527.dist-info/RECORD,,
```

## Comparing `gs_engine-0.22.0a20230526.dist-info/METADATA` & `gs_engine-0.22.0a20230527.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-engine
-Version: 0.22.0a20230526
+Version: 0.22.0a20230527
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

