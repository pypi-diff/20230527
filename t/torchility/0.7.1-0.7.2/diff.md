# Comparing `tmp/torchility-0.7.1.tar.gz` & `tmp/torchility-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchility-0.7.1.tar", last modified: Sat May 27 12:53:11 2023, max compression
+gzip compressed data, was "torchility-0.7.2.tar", last modified: Sat May 27 15:22:26 2023, max compression
```

## Comparing `torchility-0.7.1.tar` & `torchility-0.7.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 12:53:11.551668 torchility-0.7.1/
--rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.7.1/LICENSE
--rw-r--r--   0 liuchen    (501) staff       (20)     2119 2023-05-27 12:53:11.550838 torchility-0.7.1/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)     1640 2023-05-27 07:50:27.000000 torchility-0.7.1/README.md
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 12:53:11.495028 torchility-0.7.1/examples/
--rw-r--r--   0 liuchen    (501) staff       (20)     1872 2023-05-27 07:45:07.000000 torchility-0.7.1/examples/1-mnist.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1645 2023-05-15 07:55:10.000000 torchility-0.7.1/examples/10-model_analysis.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.7.1/examples/11-graph_node_clasification_DGL.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2073 2023-05-27 07:49:20.000000 torchility-0.7.1/examples/2-metrics_basic.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2064 2023-05-21 03:49:55.000000 torchility-0.7.1/examples/3-metrics_more.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1738 2023-05-19 08:52:25.000000 torchility-0.7.1/examples/4-callbacks.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.7.1/examples/5-lr_find.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1563 2023-05-16 01:20:14.000000 torchility-0.7.1/examples/6-optimizer.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-15 07:37:59.000000 torchility-0.7.1/examples/7-interpreter.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2531 2023-05-19 12:30:31.000000 torchility-0.7.1/examples/8-multi_dataloaders.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1623 2023-05-16 00:41:34.000000 torchility-0.7.1/examples/9-reset_train_dataloader.py
--rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-05-27 12:53:11.551943 torchility-0.7.1/setup.cfg
--rw-r--r--   0 liuchen    (501) staff       (20)     1163 2023-05-27 06:45:49.000000 torchility-0.7.1/setup.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 12:53:11.511824 torchility-0.7.1/torchility/
--rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-05-27 12:29:45.000000 torchility-0.7.1/torchility/__init__.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 12:53:11.531543 torchility-0.7.1/torchility/callbacks/
--rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.7.1/torchility/callbacks/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1656 2023-05-23 02:30:14.000000 torchility-0.7.1/torchility/callbacks/common.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4840 2023-05-05 13:46:18.000000 torchility-0.7.1/torchility/callbacks/interpreters.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.7.1/torchility/callbacks/performances.py
--rw-r--r--   0 liuchen    (501) staff       (20)     9800 2023-05-27 12:50:02.000000 torchility-0.7.1/torchility/callbacks/progress.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1102 2023-05-15 09:10:40.000000 torchility-0.7.1/torchility/datamodule.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.7.1/torchility/hooks.py
--rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.7.1/torchility/losses.py
--rw-r--r--   0 liuchen    (501) staff       (20)     6541 2023-05-18 13:56:01.000000 torchility-0.7.1/torchility/metrics.py
--rw-r--r--   0 liuchen    (501) staff       (20)     5695 2023-05-23 02:30:35.000000 torchility-0.7.1/torchility/tasks.py
--rw-r--r--   0 liuchen    (501) staff       (20)    12469 2023-05-27 12:31:48.000000 torchility-0.7.1/torchility/trainer.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 12:53:11.548222 torchility-0.7.1/torchility/utils/
--rw-r--r--   0 liuchen    (501) staff       (20)       96 2023-05-15 04:51:01.000000 torchility-0.7.1/torchility/utils/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2647 2023-05-21 03:41:57.000000 torchility-0.7.1/torchility/utils/metric_utils.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.7.1/torchility/utils/plots.py
--rw-r--r--   0 liuchen    (501) staff       (20)     6816 2023-05-18 13:11:06.000000 torchility-0.7.1/torchility/utils/utils.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3014 2022-08-04 03:32:03.000000 torchility-0.7.1/torchility/utils/yaml_config.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 12:53:11.515867 torchility-0.7.1/torchility.egg-info/
--rw-r--r--   0 liuchen    (501) staff       (20)     2119 2023-05-27 12:53:11.000000 torchility-0.7.1/torchility.egg-info/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)      979 2023-05-27 12:53:11.000000 torchility-0.7.1/torchility.egg-info/SOURCES.txt
--rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-05-27 12:53:11.000000 torchility-0.7.1/torchility.egg-info/dependency_links.txt
--rw-r--r--   0 liuchen    (501) staff       (20)      112 2023-05-27 12:53:11.000000 torchility-0.7.1/torchility.egg-info/requires.txt
--rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-05-27 12:53:11.000000 torchility-0.7.1/torchility.egg-info/top_level.txt
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 15:22:26.484918 torchility-0.7.2/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.7.2/LICENSE
+-rw-r--r--   0 liuchen    (501) staff       (20)     2119 2023-05-27 15:22:26.483681 torchility-0.7.2/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)     1640 2023-05-27 07:50:27.000000 torchility-0.7.2/README.md
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 15:22:26.434146 torchility-0.7.2/examples/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1872 2023-05-27 07:45:07.000000 torchility-0.7.2/examples/1-mnist.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1645 2023-05-15 07:55:10.000000 torchility-0.7.2/examples/10-model_analysis.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.7.2/examples/11-graph_node_clasification_DGL.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2073 2023-05-27 07:49:20.000000 torchility-0.7.2/examples/2-metrics_basic.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2064 2023-05-21 03:49:55.000000 torchility-0.7.2/examples/3-metrics_more.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1738 2023-05-19 08:52:25.000000 torchility-0.7.2/examples/4-callbacks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.7.2/examples/5-lr_find.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1563 2023-05-16 01:20:14.000000 torchility-0.7.2/examples/6-optimizer.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-15 07:37:59.000000 torchility-0.7.2/examples/7-interpreter.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2531 2023-05-19 12:30:31.000000 torchility-0.7.2/examples/8-multi_dataloaders.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1623 2023-05-16 00:41:34.000000 torchility-0.7.2/examples/9-reset_train_dataloader.py
+-rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-05-27 15:22:26.485550 torchility-0.7.2/setup.cfg
+-rw-r--r--   0 liuchen    (501) staff       (20)     1163 2023-05-27 06:45:49.000000 torchility-0.7.2/setup.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 15:22:26.442169 torchility-0.7.2/torchility/
+-rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-05-27 15:22:03.000000 torchility-0.7.2/torchility/__init__.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 15:22:26.467400 torchility-0.7.2/torchility/callbacks/
+-rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.7.2/torchility/callbacks/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1656 2023-05-23 02:30:14.000000 torchility-0.7.2/torchility/callbacks/common.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4840 2023-05-05 13:46:18.000000 torchility-0.7.2/torchility/callbacks/interpreters.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.7.2/torchility/callbacks/performances.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     9796 2023-05-27 15:05:14.000000 torchility-0.7.2/torchility/callbacks/progress.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1102 2023-05-15 09:10:40.000000 torchility-0.7.2/torchility/datamodule.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.7.2/torchility/hooks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.7.2/torchility/losses.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     6693 2023-05-27 15:21:51.000000 torchility-0.7.2/torchility/metrics.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     5695 2023-05-23 02:30:35.000000 torchility-0.7.2/torchility/tasks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)    12469 2023-05-27 15:21:26.000000 torchility-0.7.2/torchility/trainer.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 15:22:26.479521 torchility-0.7.2/torchility/utils/
+-rw-r--r--   0 liuchen    (501) staff       (20)       96 2023-05-15 04:51:01.000000 torchility-0.7.2/torchility/utils/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2647 2023-05-21 03:41:57.000000 torchility-0.7.2/torchility/utils/metric_utils.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.7.2/torchility/utils/plots.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     6816 2023-05-18 13:11:06.000000 torchility-0.7.2/torchility/utils/utils.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3014 2022-08-04 03:32:03.000000 torchility-0.7.2/torchility/utils/yaml_config.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 15:22:26.450385 torchility-0.7.2/torchility.egg-info/
+-rw-r--r--   0 liuchen    (501) staff       (20)     2119 2023-05-27 15:22:26.000000 torchility-0.7.2/torchility.egg-info/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)      979 2023-05-27 15:22:26.000000 torchility-0.7.2/torchility.egg-info/SOURCES.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-05-27 15:22:26.000000 torchility-0.7.2/torchility.egg-info/dependency_links.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)      112 2023-05-27 15:22:26.000000 torchility-0.7.2/torchility.egg-info/requires.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-05-27 15:22:26.000000 torchility-0.7.2/torchility.egg-info/top_level.txt
```

### Comparing `torchility-0.7.1/LICENSE` & `torchility-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/PKG-INFO` & `torchility-0.7.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.7.1
+Version: 0.7.2
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torchility-0.7.1/README.md` & `torchility-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/examples/1-mnist.py` & `torchility-0.7.2/examples/1-mnist.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/examples/10-model_analysis.py` & `torchility-0.7.2/examples/10-model_analysis.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/examples/11-graph_node_clasification_DGL.py` & `torchility-0.7.2/examples/11-graph_node_clasification_DGL.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/examples/2-metrics_basic.py` & `torchility-0.7.2/examples/2-metrics_basic.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/examples/3-metrics_more.py` & `torchility-0.7.2/examples/3-metrics_more.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/examples/4-callbacks.py` & `torchility-0.7.2/examples/4-callbacks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/examples/5-lr_find.py` & `torchility-0.7.2/examples/5-lr_find.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/examples/6-optimizer.py` & `torchility-0.7.2/examples/6-optimizer.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/examples/7-interpreter.py` & `torchility-0.7.2/examples/7-interpreter.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/examples/8-multi_dataloaders.py` & `torchility-0.7.2/examples/8-multi_dataloaders.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/examples/9-reset_train_dataloader.py` & `torchility-0.7.2/examples/9-reset_train_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/setup.py` & `torchility-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/torchility/callbacks/common.py` & `torchility-0.7.2/torchility/callbacks/common.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/torchility/callbacks/interpreters.py` & `torchility-0.7.2/torchility/callbacks/interpreters.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/torchility/callbacks/performances.py` & `torchility-0.7.2/torchility/callbacks/performances.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/torchility/callbacks/progress.py` & `torchility-0.7.2/torchility/callbacks/progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
 
         self.progress_info = []
         self.curent_epoch = None
         super().__init__()
 
     def on_train_epoch_start(self, trainer, pl_module):
         if self.unit == 'epoch':
-            self.curent_epoch = {'train_epoch': None, 'val_epoch': None}
+            self.curent_epoch = {'train_epoch': {}, 'val_epoch': {}}
         else:
             self.curent_epoch = {'train_epoch': [], 'val_epoch': []}
 
     def on_train_batch_end(self, trainer, pl_module, outputs, batch, batch_idx):
         self.train_batch_id = batch_idx + 1
         if self.unit == 'step':
             self.curent_epoch['train_epoch'].append(outputs)
```

### Comparing `torchility-0.7.1/torchility/datamodule.py` & `torchility-0.7.2/torchility/datamodule.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/torchility/hooks.py` & `torchility-0.7.2/torchility/hooks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/torchility/losses.py` & `torchility-0.7.2/torchility/losses.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/torchility/metrics.py` & `torchility-0.7.2/torchility/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,16 @@
     def reset(self):
         self.pred_batchs = []
         self.target_batchs = []
         self.cumulate_size = 0
         self.cumulate_value = None
 
     def compute(self):
+        if self.cumulate_size == 0 or self.cumulate_value is None:
+            raise Exception("This metric have not updated!") # pylint: disable=W0719
         if self.simple_cumulate:
             if isinstance(self.cumulate_value, dict):
                 return {k: v/self.cumulate_size for k, v in self.cumulate_value.items()}
             else:
                 return self.cumulate_value / self.cumulate_size
         else:
             if len(self.pred_batchs) == 0 and len(self.pred_batchs) == 0:
```

### Comparing `torchility-0.7.1/torchility/tasks.py` & `torchility-0.7.2/torchility/tasks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/torchility/trainer.py` & `torchility-0.7.2/torchility/trainer.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/torchility/utils/metric_utils.py` & `torchility-0.7.2/torchility/utils/metric_utils.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/torchility/utils/plots.py` & `torchility-0.7.2/torchility/utils/plots.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/torchility/utils/utils.py` & `torchility-0.7.2/torchility/utils/utils.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/torchility/utils/yaml_config.py` & `torchility-0.7.2/torchility/utils/yaml_config.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.1/torchility.egg-info/PKG-INFO` & `torchility-0.7.2/torchility.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.7.1
+Version: 0.7.2
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torchility-0.7.1/torchility.egg-info/SOURCES.txt` & `torchility-0.7.2/torchility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

