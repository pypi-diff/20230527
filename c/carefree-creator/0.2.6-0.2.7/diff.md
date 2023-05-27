# Comparing `tmp/carefree-creator-0.2.6.tar.gz` & `tmp/carefree-creator-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-creator-0.2.6.tar", last modified: Mon May 22 14:47:54 2023, max compression
+gzip compressed data, was "carefree-creator-0.2.7.tar", last modified: Sat May 27 11:37:26 2023, max compression
```

## Comparing `carefree-creator-0.2.6.tar` & `carefree-creator-0.2.7.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 14:47:54.250428 carefree-creator-0.2.6/
--rw-rw-rw-   0        0        0     1090 2022-10-31 07:20:41.000000 carefree-creator-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      195 2023-04-13 07:31:10.000000 carefree-creator-0.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4419 2023-05-22 14:47:54.250428 carefree-creator-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     4117 2023-05-22 08:04:35.000000 carefree-creator-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 14:47:54.237466 carefree-creator-0.2.6/carefree_creator.egg-info/
--rw-rw-rw-   0        0        0     4419 2023-05-22 14:47:54.000000 carefree-creator-0.2.6/carefree_creator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      962 2023-05-22 14:47:54.000000 carefree-creator-0.2.6/carefree_creator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 14:47:54.000000 carefree-creator-0.2.6/carefree_creator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-22 14:47:54.000000 carefree-creator-0.2.6/carefree_creator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      139 2023-05-22 14:47:54.000000 carefree-creator-0.2.6/carefree_creator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-22 14:47:54.000000 carefree-creator-0.2.6/carefree_creator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-22 14:47:54.244447 carefree-creator-0.2.6/cfcreator/
--rw-rw-rw-   0        0        0       96 2023-04-18 08:30:52.000000 carefree-creator-0.2.6/cfcreator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:47:54.245444 carefree-creator-0.2.6/cfcreator/apis/
--rw-rw-rw-   0        0        0      821 2023-04-13 07:31:10.000000 carefree-creator-0.2.6/cfcreator/apis/config.yml
--rw-rw-rw-   0        0        0     9028 2023-05-22 08:04:35.000000 carefree-creator-0.2.6/cfcreator/apis/interface.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:47:54.247437 carefree-creator-0.2.6/cfcreator/apis/kafka/
--rw-rw-rw-   0        0        0      821 2023-04-18 08:30:52.000000 carefree-creator-0.2.6/cfcreator/apis/kafka/config.yml
--rw-rw-rw-   0        0        0    13714 2023-05-22 14:06:42.000000 carefree-creator-0.2.6/cfcreator/apis/kafka/consumer.py
--rw-rw-rw-   0        0        0    12102 2023-05-22 08:53:07.000000 carefree-creator-0.2.6/cfcreator/apis/kafka/producer.py
--rw-rw-rw-   0        0        0     2984 2023-04-23 02:27:17.000000 carefree-creator-0.2.6/cfcreator/cli.py
--rw-rw-rw-   0        0        0    20510 2023-05-22 08:04:35.000000 carefree-creator-0.2.6/cfcreator/common.py
--rw-rw-rw-   0        0        0    16286 2023-05-22 14:06:42.000000 carefree-creator-0.2.6/cfcreator/control.py
--rw-rw-rw-   0        0        0     2270 2023-05-22 14:06:42.000000 carefree-creator-0.2.6/cfcreator/control_multi.py
--rw-rw-rw-   0        0        0     8444 2023-05-22 14:06:42.000000 carefree-creator-0.2.6/cfcreator/cos.py
--rw-rw-rw-   0        0        0     4566 2023-04-18 08:30:52.000000 carefree-creator-0.2.6/cfcreator/cv.py
--rw-rw-rw-   0        0        0     2408 2023-05-22 14:06:42.000000 carefree-creator-0.2.6/cfcreator/endpoints.py
--rw-rw-rw-   0        0        0    20532 2023-05-22 14:06:32.000000 carefree-creator-0.2.6/cfcreator/img2img.py
--rw-rw-rw-   0        0        0     1657 2023-05-22 08:04:35.000000 carefree-creator-0.2.6/cfcreator/img2txt.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:47:54.248434 carefree-creator-0.2.6/cfcreator/legacy/
--rw-rw-rw-   0        0        0        0 2023-05-22 08:04:35.000000 carefree-creator-0.2.6/cfcreator/legacy/__init__.py
--rw-rw-rw-   0        0        0     2169 2023-05-22 14:06:42.000000 carefree-creator-0.2.6/cfcreator/legacy/common.py
--rw-rw-rw-   0        0        0    13783 2023-05-22 14:06:42.000000 carefree-creator-0.2.6/cfcreator/legacy/control.py
--rw-rw-rw-   0        0        0     3216 2023-05-22 08:04:35.000000 carefree-creator-0.2.6/cfcreator/legacy/control_multi.py
--rw-rw-rw-   0        0        0     3271 2023-05-22 08:53:07.000000 carefree-creator-0.2.6/cfcreator/parameters.py
--rw-rw-rw-   0        0        0     3431 2023-05-22 14:06:42.000000 carefree-creator-0.2.6/cfcreator/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:47:54.250428 carefree-creator-0.2.6/cfcreator/sdks/
--rw-rw-rw-   0        0        0       45 2023-04-18 08:30:52.000000 carefree-creator-0.2.6/cfcreator/sdks/__init__.py
--rw-rw-rw-   0        0        0      659 2023-04-23 02:27:17.000000 carefree-creator-0.2.6/cfcreator/sdks/direct.py
--rw-rw-rw-   0        0        0     2130 2023-04-23 02:27:17.000000 carefree-creator-0.2.6/cfcreator/sdks/kafka.py
--rw-rw-rw-   0        0        0     1103 2023-04-23 02:27:17.000000 carefree-creator-0.2.6/cfcreator/sdks/utils.py
--rw-rw-rw-   0        0        0     7034 2023-05-22 08:04:35.000000 carefree-creator-0.2.6/cfcreator/txt2img.py
--rw-rw-rw-   0        0        0     2371 2023-04-23 02:27:17.000000 carefree-creator-0.2.6/cfcreator/txt2txt.py
--rw-rw-rw-   0        0        0     5715 2023-05-22 11:54:08.000000 carefree-creator-0.2.6/cfcreator/utils.py
--rw-rw-rw-   0        0        0       42 2023-05-22 14:47:54.251424 carefree-creator-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1015 2023-05-22 14:47:31.000000 carefree-creator-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:37:26.850636 carefree-creator-0.2.7/
+-rw-rw-rw-   0        0        0     1090 2022-10-31 07:20:41.000000 carefree-creator-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0      195 2023-04-13 07:31:10.000000 carefree-creator-0.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4419 2023-05-27 11:37:26.850636 carefree-creator-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4117 2023-05-22 08:04:35.000000 carefree-creator-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 11:37:26.830287 carefree-creator-0.2.7/carefree_creator.egg-info/
+-rw-rw-rw-   0        0        0     4419 2023-05-27 11:37:26.000000 carefree-creator-0.2.7/carefree_creator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2023-05-27 11:37:26.000000 carefree-creator-0.2.7/carefree_creator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 11:37:26.000000 carefree-creator-0.2.7/carefree_creator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-27 11:37:26.000000 carefree-creator-0.2.7/carefree_creator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      139 2023-05-27 11:37:26.000000 carefree-creator-0.2.7/carefree_creator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-27 11:37:26.000000 carefree-creator-0.2.7/carefree_creator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 11:37:26.839636 carefree-creator-0.2.7/cfcreator/
+-rw-rw-rw-   0        0        0       96 2023-04-18 08:30:52.000000 carefree-creator-0.2.7/cfcreator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:37:26.843635 carefree-creator-0.2.7/cfcreator/apis/
+-rw-rw-rw-   0        0        0      821 2023-04-13 07:31:10.000000 carefree-creator-0.2.7/cfcreator/apis/config.yml
+-rw-rw-rw-   0        0        0     9028 2023-05-22 08:04:35.000000 carefree-creator-0.2.7/cfcreator/apis/interface.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:37:26.845634 carefree-creator-0.2.7/cfcreator/apis/kafka/
+-rw-rw-rw-   0        0        0      821 2023-04-18 08:30:52.000000 carefree-creator-0.2.7/cfcreator/apis/kafka/config.yml
+-rw-rw-rw-   0        0        0    13714 2023-05-23 09:07:48.000000 carefree-creator-0.2.7/cfcreator/apis/kafka/consumer.py
+-rw-rw-rw-   0        0        0    12102 2023-05-22 08:53:07.000000 carefree-creator-0.2.7/cfcreator/apis/kafka/producer.py
+-rw-rw-rw-   0        0        0     2984 2023-04-23 02:27:17.000000 carefree-creator-0.2.7/cfcreator/cli.py
+-rw-rw-rw-   0        0        0    20510 2023-05-22 08:04:35.000000 carefree-creator-0.2.7/cfcreator/common.py
+-rw-rw-rw-   0        0        0    17555 2023-05-24 13:03:13.000000 carefree-creator-0.2.7/cfcreator/control.py
+-rw-rw-rw-   0        0        0     2295 2023-05-27 11:36:59.000000 carefree-creator-0.2.7/cfcreator/control_multi.py
+-rw-rw-rw-   0        0        0     8444 2023-05-23 09:07:48.000000 carefree-creator-0.2.7/cfcreator/cos.py
+-rw-rw-rw-   0        0        0     4566 2023-04-18 08:30:52.000000 carefree-creator-0.2.7/cfcreator/cv.py
+-rw-rw-rw-   0        0        0     2408 2023-05-23 09:07:48.000000 carefree-creator-0.2.7/cfcreator/endpoints.py
+-rw-rw-rw-   0        0        0    20657 2023-05-24 15:54:47.000000 carefree-creator-0.2.7/cfcreator/img2img.py
+-rw-rw-rw-   0        0        0     1657 2023-05-22 08:04:35.000000 carefree-creator-0.2.7/cfcreator/img2txt.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:37:26.847635 carefree-creator-0.2.7/cfcreator/legacy/
+-rw-rw-rw-   0        0        0        0 2023-05-22 08:04:35.000000 carefree-creator-0.2.7/cfcreator/legacy/__init__.py
+-rw-rw-rw-   0        0        0     2169 2023-05-23 09:07:48.000000 carefree-creator-0.2.7/cfcreator/legacy/common.py
+-rw-rw-rw-   0        0        0    13783 2023-05-23 09:07:48.000000 carefree-creator-0.2.7/cfcreator/legacy/control.py
+-rw-rw-rw-   0        0        0     3216 2023-05-22 08:04:35.000000 carefree-creator-0.2.7/cfcreator/legacy/control_multi.py
+-rw-rw-rw-   0        0        0     3271 2023-05-22 08:53:07.000000 carefree-creator-0.2.7/cfcreator/parameters.py
+-rw-rw-rw-   0        0        0     3431 2023-05-23 09:07:48.000000 carefree-creator-0.2.7/cfcreator/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:37:26.849636 carefree-creator-0.2.7/cfcreator/sdks/
+-rw-rw-rw-   0        0        0       45 2023-04-18 08:30:52.000000 carefree-creator-0.2.7/cfcreator/sdks/__init__.py
+-rw-rw-rw-   0        0        0     3952 2023-05-27 11:36:59.000000 carefree-creator-0.2.7/cfcreator/sdks/apis.py
+-rw-rw-rw-   0        0        0      659 2023-04-23 02:27:17.000000 carefree-creator-0.2.7/cfcreator/sdks/direct.py
+-rw-rw-rw-   0        0        0     2130 2023-04-23 02:27:17.000000 carefree-creator-0.2.7/cfcreator/sdks/kafka.py
+-rw-rw-rw-   0        0        0     1103 2023-04-23 02:27:17.000000 carefree-creator-0.2.7/cfcreator/sdks/utils.py
+-rw-rw-rw-   0        0        0     7034 2023-05-22 08:04:35.000000 carefree-creator-0.2.7/cfcreator/txt2img.py
+-rw-rw-rw-   0        0        0     2371 2023-04-23 02:27:17.000000 carefree-creator-0.2.7/cfcreator/txt2txt.py
+-rw-rw-rw-   0        0        0     5715 2023-05-27 11:36:59.000000 carefree-creator-0.2.7/cfcreator/utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-27 11:37:26.851635 carefree-creator-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2023-05-25 01:26:08.000000 carefree-creator-0.2.7/setup.py
```

### Comparing `carefree-creator-0.2.6/LICENSE` & `carefree-creator-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/PKG-INFO` & `carefree-creator-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-creator
-Version: 0.2.6
+Version: 0.2.7
 Summary: An AI-powered creator for everyone.
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn PyTorch
 Description-Content-Type: text/markdown
 Provides-Extra: kafka
 License-File: LICENSE
```

### Comparing `carefree-creator-0.2.6/README.md` & `carefree-creator-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/carefree_creator.egg-info/PKG-INFO` & `carefree-creator-0.2.7/carefree_creator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-creator
-Version: 0.2.6
+Version: 0.2.7
 Summary: An AI-powered creator for everyone.
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn PyTorch
 Description-Content-Type: text/markdown
 Provides-Extra: kafka
 License-File: LICENSE
```

### Comparing `carefree-creator-0.2.6/carefree_creator.egg-info/SOURCES.txt` & `carefree-creator-0.2.7/carefree_creator.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -29,10 +29,11 @@
 cfcreator/apis/kafka/consumer.py
 cfcreator/apis/kafka/producer.py
 cfcreator/legacy/__init__.py
 cfcreator/legacy/common.py
 cfcreator/legacy/control.py
 cfcreator/legacy/control_multi.py
 cfcreator/sdks/__init__.py
+cfcreator/sdks/apis.py
 cfcreator/sdks/direct.py
 cfcreator/sdks/kafka.py
 cfcreator/sdks/utils.py
```

### Comparing `carefree-creator-0.2.6/cfcreator/apis/config.yml` & `carefree-creator-0.2.7/cfcreator/apis/config.yml`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/apis/interface.py` & `carefree-creator-0.2.7/cfcreator/apis/interface.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/apis/kafka/config.yml` & `carefree-creator-0.2.7/cfcreator/apis/kafka/config.yml`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/apis/kafka/consumer.py` & `carefree-creator-0.2.7/cfcreator/apis/kafka/consumer.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/apis/kafka/producer.py` & `carefree-creator-0.2.7/cfcreator/apis/kafka/producer.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/cli.py` & `carefree-creator-0.2.7/cfcreator/cli.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/common.py` & `carefree-creator-0.2.7/cfcreator/common.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/control.py` & `carefree-creator-0.2.7/cfcreator/control.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pydantic import Field
 from pydantic import BaseModel
 from cftool.cv import to_rgb
 from cftool.cv import to_uint8
 from cftool.cv import np_to_bytes
 from cftool.cv import restrict_wh
 from cftool.cv import get_suitable_size
+from cftool.misc import shallow_copy_dict
 from cfclient.models.core import ImageModel
 from cflearn.api.cv.diffusion import ControlNetHints
 from cflearn.models.cv.diffusion.utils import CONTROL_HINT_KEY
 from cflearn.models.cv.diffusion.utils import CONTROL_HINT_START_KEY
 
 from .utils import api_pool
 from .utils import to_canvas
@@ -79,14 +80,15 @@
 
 
 async def apply_control(
     self: IAlgorithm,
     common: ControlNetModel,
     controls: List[ControlNetBundle],
     normalized_inpainting_mask: Optional[np.ndarray] = None,
+    **kwargs: Any,
 ) -> apply_response:
     api_key = APIs.SD_INPAINTING if common.use_inpainting else APIs.SD
     api = get_sd_from(api_key, common, no_change=True)
     need_change_device = api_pool.need_change_device(api_key)
     api.enable_control()
     # download images
     urls = set()
@@ -200,15 +202,16 @@
             if i_data.guess_mode
             else ([i_data.control_strength] * num_scales)
         )
     api.m.control_scales = all_scales
     if not common.prompt:
         raise ValueError("prompt should be provided in `common`")
     cond = [common.prompt] * common.num_samples
-    kw = handle_diffusion_model(api, common)
+    kw = shallow_copy_dict(kwargs)
+    kw.update(handle_diffusion_model(api, common))
     hint = [(b.type, all_key_values[k][0]) for b, k in zip(controls, all_keys)]
     kw[CONTROL_HINT_KEY] = hint
     kw[CONTROL_HINT_START_KEY] = [b.data.hint_start for b in controls]
     kw["max_wh"] = common.max_wh
     dt = time.time()
     if need_change_device:
         api.to("cuda:0", use_half=True, no_annotator=True)
@@ -272,18 +275,19 @@
     return results, latencies
 
 
 async def run_single_control(
     self: IAlgorithm,
     data: ControlNetModel,
     hint_type: ControlNetHints,
+    **kwargs: Any,
 ) -> Tuple[List[np.ndarray], Dict[str, float]]:
     self.log_endpoint(data)
     bundle = ControlNetBundle(type=hint_type, data=data)
-    return await apply_control(self, data, [bundle])
+    return await apply_control(self, data, [bundle], **kwargs)
 
 
 def register_control(
     algorithm_model_class: Type[ControlNetModel],
     algorithm_endpoint: str,
     hint_type: ControlNetHints,
 ) -> None:
@@ -292,52 +296,54 @@
 
         endpoint = algorithm_endpoint
 
         def initialize(self) -> None:
             register_sd()
             register_sd_inpainting()
 
-        async def run(self, data: algorithm_model_class, *args: Any) -> Response:
-            results, latencies = await run_single_control(self, data, hint_type)
+        async def run(
+            self, data: algorithm_model_class, *args: Any, **kwargs: Any
+        ) -> Response:
+            rs, latencies = await run_single_control(self, data, hint_type, **kwargs)
             t0 = time.time()
-            content = None if data.return_arrays else np_to_bytes(to_canvas(results))
+            content = None if data.return_arrays else np_to_bytes(to_canvas(rs))
             t1 = time.time()
             latencies["to_canvas"] = t1 - t0
             self.log_times(latencies)
             if data.return_arrays:
-                return results
+                return rs
             return Response(content=content, media_type="image/png")
 
     IAlgorithm.auto_register()(_)
+    control_hint2endpoints[hint_type] = algorithm_endpoint
+    control_hint2data_models[hint_type] = algorithm_model_class
 
 
-def register_control_hint(
+def register_hint(
     hint_model_class: Type,
     hint_endpoint: str,
     hint_type: ControlNetHints,
 ) -> None:
-    class _Model(hint_model_class, ReturnArraysModel, ImageModel):
-        pass
-
     class _(IAlgorithm):
-        model_class = _Model
+        model_class = hint_model_class
         model_class.__name__ = hint_model_class.__name__
 
         endpoint = hint_endpoint
 
         def initialize(self) -> None:
             register_sd()
 
-        async def run(self, data: _Model, *args: Any) -> Response:
+        async def run(self, data: hint_model_class, *args: Any) -> Response:
             t0 = time.time()
             image = await self.download_image_with_retry(data.url)
             w, h = image.size
             t1 = time.time()
             m = api_pool.get(APIs.SD)
             t2 = time.time()
+            image = to_contrast_rgb(image)
             hint_image = np.array(image)
             detect_resolution = getattr(data, "detect_resolution", None)
             if detect_resolution is not None:
                 hint_image = resize_image(hint_image, detect_resolution)
             hint = m.get_hint_of(hint_type, hint_image, **data.dict())
             hint = cv2.resize(hint, (w, h), interpolation=cv2.INTER_LINEAR)
             t3 = time.time()
@@ -351,14 +357,16 @@
                 )
             )
             if data.return_arrays:
                 return [hint]
             return Response(content=np_to_bytes(hint), media_type="image/png")
 
     IAlgorithm.auto_register()(_)
+    control_hint2hint_endpoints[hint_type] = hint_endpoint
+    control_hint2hint_data_models[hint_type] = hint_model_class
 
 
 class DetectResolutionModel(BaseModel):
     detect_resolution: int = Field(
         384,
         ge=128,
         le=1024,
@@ -382,14 +390,18 @@
     pass
 
 
 class ControlDepthModel(_DepthModel, ControlStrengthModel, ControlNetModel):
     pass
 
 
+class ControlDepthHintModel(_DepthModel, ReturnArraysModel, ImageModel):
+    pass
+
+
 # ControlNet (canny2image)
 
 
 class _CannyModel(LargeDetectResolutionModel):
     low_threshold: int = Field(
         100,
         ge=1,
@@ -404,25 +416,33 @@
     )
 
 
 class ControlCannyModel(_CannyModel, ControlStrengthModel, ControlNetModel):
     pass
 
 
+class ControlCannyHintModel(_CannyModel, ReturnArraysModel, ImageModel):
+    pass
+
+
 # ControlNet (pose2image)
 
 
 class _PoseModel(LargeDetectResolutionModel):
     pass
 
 
 class ControlPoseModel(_PoseModel, ControlStrengthModel, ControlNetModel):
     pass
 
 
+class ControlPoseHintModel(_PoseModel, ReturnArraysModel, ImageModel):
+    pass
+
+
 # ControlNet (canny2image)
 
 
 class _MLSDModel(LargeDetectResolutionModel):
     value_threshold: float = Field(
         0.1,
         ge=0.01,
@@ -437,34 +457,50 @@
     )
 
 
 class ControlMLSDModel(_MLSDModel, ControlStrengthModel, ControlNetModel):
     pass
 
 
+class ControlMLSDHintModel(_MLSDModel, ReturnArraysModel, ImageModel):
+    pass
+
+
 # register
 
+control_hint2endpoints: Dict[ControlNetHints, str] = {}
+control_hint2hint_endpoints: Dict[ControlNetHints, str] = {}
+control_hint2data_models: Dict[ControlNetHints, Type[BaseModel]] = {}
+control_hint2hint_data_models: Dict[ControlNetHints, Type[BaseModel]] = {}
 register_control(ControlDepthModel, new_control_depth_endpoint, ControlNetHints.DEPTH)
 register_control(ControlCannyModel, new_control_canny_endpoint, ControlNetHints.CANNY)
 register_control(ControlPoseModel, new_control_pose_endpoint, ControlNetHints.POSE)
 register_control(ControlMLSDModel, new_control_mlsd_endpoint, ControlNetHints.MLSD)
-register_control_hint(_DepthModel, control_depth_hint_endpoint, ControlNetHints.DEPTH)
-register_control_hint(_CannyModel, control_canny_hint_endpoint, ControlNetHints.CANNY)
-register_control_hint(_PoseModel, control_pose_hint_endpoint, ControlNetHints.POSE)
-register_control_hint(_MLSDModel, control_mlsd_hint_endpoint, ControlNetHints.MLSD)
+register_hint(ControlDepthHintModel, control_depth_hint_endpoint, ControlNetHints.DEPTH)
+register_hint(ControlCannyHintModel, control_canny_hint_endpoint, ControlNetHints.CANNY)
+register_hint(ControlPoseHintModel, control_pose_hint_endpoint, ControlNetHints.POSE)
+register_hint(ControlMLSDHintModel, control_mlsd_hint_endpoint, ControlNetHints.MLSD)
 
 
 __all__ = [
     "get_bundle_key",
     "new_control_depth_endpoint",
     "new_control_canny_endpoint",
     "new_control_pose_endpoint",
     "new_control_mlsd_endpoint",
     "control_depth_hint_endpoint",
     "control_canny_hint_endpoint",
     "control_pose_hint_endpoint",
     "control_mlsd_hint_endpoint",
     "ControlDepthModel",
+    "ControlDepthHintModel",
     "ControlCannyModel",
+    "ControlCannyHintModel",
     "ControlPoseModel",
+    "ControlPoseHintModel",
     "ControlMLSDModel",
+    "ControlMLSDHintModel",
+    "control_hint2endpoints",
+    "control_hint2hint_endpoints",
+    "control_hint2data_models",
+    "control_hint2hint_data_models",
 ]
```

### Comparing `carefree-creator-0.2.6/cfcreator/control_multi.py` & `carefree-creator-0.2.7/cfcreator/control_multi.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,17 +57,17 @@
 
     endpoint = new_control_multi_endpoint
 
     def initialize(self) -> None:
         register_sd()
         register_sd_inpainting()
 
-    async def run(self, data: ControlMultiModel, *args: Any) -> Response:
+    async def run(self, data: ControlMultiModel, *args: Any, **kwargs: Any) -> Response:
         self.log_endpoint(data)
-        results, latencies = await apply_control(self, data, data.controls)
+        results, latencies = await apply_control(self, data, data.controls, **kwargs)
         t0 = time.time()
         content = None if data.return_arrays else np_to_bytes(to_canvas(results))
         t1 = time.time()
         latencies["to_canvas"] = t1 - t0
         self.log_times(latencies)
         if data.return_arrays:
             return results
```

### Comparing `carefree-creator-0.2.6/cfcreator/cos.py` & `carefree-creator-0.2.7/cfcreator/cos.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/cv.py` & `carefree-creator-0.2.7/cfcreator/cv.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/endpoints.py` & `carefree-creator-0.2.7/cfcreator/endpoints.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/img2img.py` & `carefree-creator-0.2.7/cfcreator/img2img.py`

 * *Files 0% similar despite different names*

```diff
@@ -520,15 +520,15 @@
         "get_model": t1 - t0,
         "inference": t2 - t1,
         "cleanup": time.time() - t2,
     }
     return result, latencies
 
 
-class Img2ImgHarmonizationModel(ImageModel):
+class Img2ImgHarmonizationModel(ReturnArraysModel, ImageModel):
     mask_url: str = Field(
         ...,
         description="The `cdn` / `cos` url of the harmonization mask. (`cos` url is preferred)",
     )
     strength: float = Field(1.0, description="Strength of the harmonization process.")
     harmonization_max_wh: int = Field(
         2048,
@@ -547,34 +547,38 @@
 
     async def run(self, data: Img2ImgHarmonizationModel, *args: Any) -> Response:
         self.log_endpoint(data)
         t0 = time.time()
         image = await self.download_image_with_retry(data.url)
         mask = await self.download_image_with_retry(data.mask_url)
         t1 = time.time()
+        mask_arr = read_image(
+            mask,
+            None,
+            anchor=None,
+            to_mask=True,
+            to_torch_fmt=False,
+        ).image
+        mask_arr[mask_arr > 0.0] = 1.0
         result, latencies = apply_harmonization(
             data.harmonization_max_wh,
             data.strength,
             read_image(
                 image,
                 None,
                 anchor=None,
                 normalize=False,
                 to_torch_fmt=False,
             ).image,
-            read_image(
-                mask,
-                None,
-                anchor=None,
-                to_mask=True,
-                to_torch_fmt=False,
-            ).image,
+            mask_arr,
         )
         latencies["download"] = t1 - t0
         self.log_times(latencies)
+        if data.return_arrays:
+            return [result]
         return Response(content=np_to_bytes(result), media_type="image/png")
 
 
 # salient object detection (isnet)
 
 
 class Img2ImgSODModel(ReturnArraysModel, ImageModel):
```

### Comparing `carefree-creator-0.2.6/cfcreator/img2txt.py` & `carefree-creator-0.2.7/cfcreator/img2txt.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/legacy/common.py` & `carefree-creator-0.2.7/cfcreator/legacy/common.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/legacy/control.py` & `carefree-creator-0.2.7/cfcreator/legacy/control.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/legacy/control_multi.py` & `carefree-creator-0.2.7/cfcreator/legacy/control_multi.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/parameters.py` & `carefree-creator-0.2.7/cfcreator/parameters.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/pipeline.py` & `carefree-creator-0.2.7/cfcreator/pipeline.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/sdks/direct.py` & `carefree-creator-0.2.7/cfcreator/sdks/direct.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/sdks/kafka.py` & `carefree-creator-0.2.7/cfcreator/sdks/kafka.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/sdks/utils.py` & `carefree-creator-0.2.7/cfcreator/sdks/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/txt2img.py` & `carefree-creator-0.2.7/cfcreator/txt2img.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/txt2txt.py` & `carefree-creator-0.2.7/cfcreator/txt2txt.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/cfcreator/utils.py` & `carefree-creator-0.2.7/cfcreator/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.6/setup.py` & `carefree-creator-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.2.6"
+VERSION = "0.2.7"
 PACKAGE_NAME = "carefree-creator"
 
 DESCRIPTION = "An AI-powered creator for everyone."
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
```

