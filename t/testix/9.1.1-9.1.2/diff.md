# Comparing `tmp/testix-9.1.1-py3-none-any.whl.zip` & `tmp/testix-9.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 13828 bytes, number of entries: 30
+Zip file size: 13836 bytes, number of entries: 30
 -rw-r--r--  2.0 unx      107 b- defN 80-Jan-01 00:00 testix/DSL.py
 -rw-r--r--  2.0 unx      115 b- defN 80-Jan-01 00:00 testix/__init__.py
 -rw-r--r--  2.0 unx     1325 b- defN 80-Jan-01 00:00 testix/argumentexpectations.py
 -rw-r--r--  2.0 unx      496 b- defN 80-Jan-01 00:00 testix/call_character.py
 -rw-r--r--  2.0 unx     1224 b- defN 80-Jan-01 00:00 testix/call_formatter.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 testix/call_modifiers/__init__.py
 -rw-r--r--  2.0 unx      842 b- defN 80-Jan-01 00:00 testix/call_modifiers/asynchronous.py
@@ -16,17 +16,17 @@
 -rw-r--r--  2.0 unx      803 b- defN 80-Jan-01 00:00 testix/failhooks.py
 -rw-r--r--  2.0 unx     1924 b- defN 80-Jan-01 00:00 testix/fake.py
 -rw-r--r--  2.0 unx       82 b- defN 80-Jan-01 00:00 testix/fake_privacy_violator.py
 -rw-r--r--  2.0 unx      156 b- defN 80-Jan-01 00:00 testix/fakefile.py
 -rw-r--r--  2.0 unx       43 b- defN 80-Jan-01 00:00 testix/fakeobject.py
 -rw-r--r--  2.0 unx      196 b- defN 80-Jan-01 00:00 testix/frequentlyused.py
 -rw-r--r--  2.0 unx      239 b- defN 80-Jan-01 00:00 testix/hook.py
--rw-r--r--  2.0 unx      858 b- defN 80-Jan-01 00:00 testix/patch_module.py
+-rw-r--r--  2.0 unx      898 b- defN 80-Jan-01 00:00 testix/patch_module.py
 -rw-r--r--  2.0 unx      436 b- defN 80-Jan-01 00:00 testix/saveargument.py
 -rw-r--r--  2.0 unx     5453 b- defN 80-Jan-01 00:00 testix/scenario.py
 -rw-r--r--  2.0 unx     1214 b- defN 80-Jan-01 00:00 testix/scenario_mocks.py
 -rw-r--r--  2.0 unx      213 b- defN 80-Jan-01 00:00 testix/testixexception.py
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 testix-9.1.1.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 testix-9.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx      926 b- defN 16-Jan-01 00:00 testix-9.1.1.dist-info/METADATA
-?rw-r--r--  2.0 unx     2391 b- defN 16-Jan-01 00:00 testix-9.1.1.dist-info/RECORD
-30 files, 28120 bytes uncompressed, 10000 bytes compressed:  64.4%
+-rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 testix-9.1.2.dist-info/LICENSE
+?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 testix-9.1.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx      926 b- defN 16-Jan-01 00:00 testix-9.1.2.dist-info/METADATA
+?rw-r--r--  2.0 unx     2391 b- defN 16-Jan-01 00:00 testix-9.1.2.dist-info/RECORD
+30 files, 28160 bytes uncompressed, 10008 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -72,20 +72,20 @@
 
 Filename: testix/scenario_mocks.py
 Comment: 
 
 Filename: testix/testixexception.py
 Comment: 
 
-Filename: testix-9.1.1.dist-info/LICENSE
+Filename: testix-9.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: testix-9.1.1.dist-info/WHEEL
+Filename: testix-9.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: testix-9.1.1.dist-info/METADATA
+Filename: testix-9.1.2.dist-info/METADATA
 Comment: 
 
-Filename: testix-9.1.1.dist-info/RECORD
+Filename: testix-9.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## testix/patch_module.py

```diff
@@ -17,15 +17,16 @@
         setattr( module, attribute, mock )
         self.__stack.append( ( module, attribute, original ) )
         return mock
 
     def undo(self):
         for module, attribute, original in reversed(self.__stack):
             if original is _SENTINEL:
-                continue
-            setattr(module, attribute, original)
+                delattr(module, attribute)
+            else:
+                setattr(module, attribute, original)
 
 @pytest.fixture
 def patch_module():
     patcher = Patcher()
     yield patcher
     patcher.undo()
```

## Comparing `testix-9.1.1.dist-info/LICENSE` & `testix-9.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `testix-9.1.1.dist-info/METADATA` & `testix-9.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testix
-Version: 9.1.1
+Version: 9.1.2
 Summary: Mocking framework Python with *exact* Scenarios
 License: MIT
 Author: Yoav Kleinberger
 Author-email: haarcuba@gmail.com
 Requires-Python: >=3.5
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `testix-9.1.1.dist-info/RECORD` & `testix-9.1.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 testix/failhooks.py,sha256=ntDxPaf95u_5IzrYxpgb3zCBPcxAFnD3ogmY8ZBIdHU,803
 testix/fake.py,sha256=XaN5DjtADr72KAxiaIpCGNue5mK2FvA0A4EpbHHaEXc,1924
 testix/fake_privacy_violator.py,sha256=mXBLTL0PojU97ue9H015x6DW1CtjQpuMSpDnZVno8KA,82
 testix/fakefile.py,sha256=TwKhn4Cgu1UyNmkouM5giz5KuCb_COVuhjNPxrai8FI,156
 testix/fakeobject.py,sha256=W9yVQzQK6OxEe6iDCZl2Roe-bqz7GErJlLMgqGEjbf4,43
 testix/frequentlyused.py,sha256=KcMRE2TpDTkvInVFg44VgjurpuRpsGPXfA-0Kj-59pM,196
 testix/hook.py,sha256=QzLYR_IV8iEI_SPLuKPKGmAz7Yao1-0GRtQEbOsY8dE,239
-testix/patch_module.py,sha256=xAWRLwz4HFsshnjpDZUAybhm2bqJuoSPPjOgq1Jr_VY,858
+testix/patch_module.py,sha256=tvZgbNrgHXPeePKTPXXqNSYOrVAiKFUituI2ozRNLck,898
 testix/saveargument.py,sha256=hTcuCI1gxUqKKGSAFx_M_h69AEAh09Qg-QOzKgruClM,436
 testix/scenario.py,sha256=Wq1TKeytX5xvtr4oEwoZCIHj5gR9HlCBdYYkOV5LhIE,5453
 testix/scenario_mocks.py,sha256=f0BTKMZgZ7TyTPHbZ12Ziphr7AqJRt2tGDAlE17XSr8,1214
 testix/testixexception.py,sha256=Y4sWiocfYgyHSeNjNSPMT5Bj31c3y_b3xu4_bPfa7w8,213
-testix-9.1.1.dist-info/LICENSE,sha256=h3436G9qk2b7_ym-riBpViR0B5_xLefrQ2i8tBMbNxQ,1073
-testix-9.1.1.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
-testix-9.1.1.dist-info/METADATA,sha256=aX6vyN9MmbBsZ9DjsEb9CnScMiCPk2yU6UjEDR3nz4c,926
-testix-9.1.1.dist-info/RECORD,,
+testix-9.1.2.dist-info/LICENSE,sha256=h3436G9qk2b7_ym-riBpViR0B5_xLefrQ2i8tBMbNxQ,1073
+testix-9.1.2.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
+testix-9.1.2.dist-info/METADATA,sha256=pvw2J2s0uXvY2srR0ON2g0pzbd2VCMQWYyO6tsRAgeg,926
+testix-9.1.2.dist-info/RECORD,,
```

