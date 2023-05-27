# Comparing `tmp/asociita-0.1.6.1.tar.gz` & `tmp/asociita-0.1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asociita-0.1.6.1.tar", max compression
+gzip compressed data, was "asociita-0.1.6.2.tar", max compression
```

## Comparing `asociita-0.1.6.1.tar` & `asociita-0.1.6.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0        0 2023-04-07 16:31:28.755226 asociita-0.1.6.1/asociita/__init__.py
--rw-r--r--   0        0        0     3959 2023-05-20 16:17:12.712011 asociita-0.1.6.1/asociita/components/archiver/archive_manager.py
--rw-r--r--   0        0        0     4768 2023-05-18 12:35:56.518494 asociita-0.1.6.1/asociita/components/evaluator/evaluation_manager.py
--rw-r--r--   0        0        0    13585 2023-05-04 12:29:03.864051 asociita-0.1.6.1/asociita/components/evaluator/mr_evaluator.py
--rw-r--r--   0        0        0    10175 2023-05-03 13:58:58.211507 asociita-0.1.6.1/asociita/components/evaluator/or_evaluator.py
--rw-r--r--   0        0        0     4497 2023-04-17 14:01:29.838168 asociita-0.1.6.1/asociita/components/nodes/federated_node.py
--rw-r--r--   0        0        0     7400 2023-05-20 16:22:57.462290 asociita-0.1.6.1/asociita/components/orchestrator/evaluator_orchestrator.py
--rw-r--r--   0        0        0     6202 2023-05-20 16:45:47.898655 asociita-0.1.6.1/asociita/components/orchestrator/fedopt_orchestrator.py
--rw-r--r--   0        0        0    10709 2023-05-22 10:06:44.372395 asociita-0.1.6.1/asociita/components/orchestrator/generic_orchestrator.py
--rw-r--r--   0        0        0     2190 2023-05-22 09:43:29.422557 asociita-0.1.6.1/asociita/datasets/fetch_data.py
--rw-r--r--   0        0        0     2699 2023-05-22 14:23:05.141330 asociita-0.1.6.1/asociita/datasets/load_cifar.py
--rw-r--r--   0        0        0     2654 2023-05-22 14:12:53.922859 asociita-0.1.6.1/asociita/datasets/load_mnist.py
--rw-r--r--   0        0        0     6874 2023-05-22 14:12:25.240855 asociita-0.1.6.1/asociita/datasets/shard_splits.py
--rw-r--r--   0        0        0     4661 2023-05-22 14:08:01.227174 asociita-0.1.6.1/asociita/datasets/shard_transformation.py
--rw-r--r--   0        0        0      329 2023-05-19 09:42:13.494113 asociita-0.1.6.1/asociita/exceptions/settingexception.py
--rw-r--r--   0        0        0      701 2023-05-20 18:16:28.662467 asociita-0.1.6.1/asociita/models/pytorch/cifar10.py
--rw-r--r--   0        0        0    15398 2023-05-22 14:25:35.473812 asociita-0.1.6.1/asociita/models/pytorch/federated_model.py
--rw-r--r--   0        0        0      966 2023-05-12 12:18:20.228520 asociita-0.1.6.1/asociita/models/pytorch/mnist.py
--rw-r--r--   0        0        0     6068 2023-04-26 13:48:40.502010 asociita-0.1.6.1/asociita/utils/computations.py
--rw-r--r--   0        0        0      633 2023-05-12 12:12:31.672198 asociita-0.1.6.1/asociita/utils/custom_transformations.py
--rw-r--r--   0        0        0     4756 2023-05-17 12:51:14.070551 asociita-0.1.6.1/asociita/utils/handlers.py
--rw-r--r--   0        0        0      585 2023-05-22 14:29:57.943413 asociita-0.1.6.1/asociita/utils/helpers.py
--rw-r--r--   0        0        0     1843 2023-04-14 15:47:01.523825 asociita-0.1.6.1/asociita/utils/loggers.py
--rw-r--r--   0        0        0     3776 2023-04-24 11:46:41.291752 asociita-0.1.6.1/asociita/utils/optimizers.py
--rw-r--r--   0        0        0     4176 2023-04-19 13:27:23.001147 asociita-0.1.6.1/asociita/utils/orchestrations.py
--rw-r--r--   0        0        0     1059 2023-05-03 14:04:40.497199 asociita-0.1.6.1/asociita/utils/showcase.py
--rw-r--r--   0        0        0     1084 2023-04-07 16:30:34.501923 asociita-0.1.6.1/LICENSE
--rw-r--r--   0        0        0      671 2023-05-25 15:17:07.989704 asociita-0.1.6.1/pyproject.toml
--rw-r--r--   0        0        0     2862 2023-04-18 20:10:20.511705 asociita-0.1.6.1/README.md
--rw-r--r--   0        0        0     3998 1970-01-01 00:00:00.000000 asociita-0.1.6.1/setup.py
--rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 asociita-0.1.6.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-07 16:31:28.755226 asociita-0.1.6.2/asociita/__init__.py
+-rw-r--r--   0        0        0     3959 2023-05-20 16:17:12.712011 asociita-0.1.6.2/asociita/components/archiver/archive_manager.py
+-rw-r--r--   0        0        0     4768 2023-05-18 12:35:56.518494 asociita-0.1.6.2/asociita/components/evaluator/evaluation_manager.py
+-rw-r--r--   0        0        0    13585 2023-05-04 12:29:03.864051 asociita-0.1.6.2/asociita/components/evaluator/mr_evaluator.py
+-rw-r--r--   0        0        0    10175 2023-05-03 13:58:58.211507 asociita-0.1.6.2/asociita/components/evaluator/or_evaluator.py
+-rw-r--r--   0        0        0     4497 2023-04-17 14:01:29.838168 asociita-0.1.6.2/asociita/components/nodes/federated_node.py
+-rw-r--r--   0        0        0     7400 2023-05-20 16:22:57.462290 asociita-0.1.6.2/asociita/components/orchestrator/evaluator_orchestrator.py
+-rw-r--r--   0        0        0     6202 2023-05-20 16:45:47.898655 asociita-0.1.6.2/asociita/components/orchestrator/fedopt_orchestrator.py
+-rw-r--r--   0        0        0    10709 2023-05-22 10:06:44.372395 asociita-0.1.6.2/asociita/components/orchestrator/generic_orchestrator.py
+-rw-r--r--   0        0        0     2190 2023-05-22 09:43:29.422557 asociita-0.1.6.2/asociita/datasets/fetch_data.py
+-rw-r--r--   0        0        0     2699 2023-05-22 14:23:05.141330 asociita-0.1.6.2/asociita/datasets/load_cifar.py
+-rw-r--r--   0        0        0     2654 2023-05-22 14:12:53.922859 asociita-0.1.6.2/asociita/datasets/load_mnist.py
+-rw-r--r--   0        0        0     6874 2023-05-22 14:12:25.240855 asociita-0.1.6.2/asociita/datasets/shard_splits.py
+-rw-r--r--   0        0        0     4661 2023-05-22 14:08:01.227174 asociita-0.1.6.2/asociita/datasets/shard_transformation.py
+-rw-r--r--   0        0        0      329 2023-05-19 09:42:13.494113 asociita-0.1.6.2/asociita/exceptions/settingexception.py
+-rw-r--r--   0        0        0      701 2023-05-20 18:16:28.662467 asociita-0.1.6.2/asociita/models/pytorch/cifar10.py
+-rw-r--r--   0        0        0    15508 2023-05-27 09:30:21.352445 asociita-0.1.6.2/asociita/models/pytorch/federated_model.py
+-rw-r--r--   0        0        0      966 2023-05-12 12:18:20.228520 asociita-0.1.6.2/asociita/models/pytorch/mnist.py
+-rw-r--r--   0        0        0     6068 2023-04-26 13:48:40.502010 asociita-0.1.6.2/asociita/utils/computations.py
+-rw-r--r--   0        0        0      633 2023-05-12 12:12:31.672198 asociita-0.1.6.2/asociita/utils/custom_transformations.py
+-rw-r--r--   0        0        0     4756 2023-05-17 12:51:14.070551 asociita-0.1.6.2/asociita/utils/handlers.py
+-rw-r--r--   0        0        0      585 2023-05-22 14:29:57.943413 asociita-0.1.6.2/asociita/utils/helpers.py
+-rw-r--r--   0        0        0     1843 2023-04-14 15:47:01.523825 asociita-0.1.6.2/asociita/utils/loggers.py
+-rw-r--r--   0        0        0     3776 2023-04-24 11:46:41.291752 asociita-0.1.6.2/asociita/utils/optimizers.py
+-rw-r--r--   0        0        0     4176 2023-04-19 13:27:23.001147 asociita-0.1.6.2/asociita/utils/orchestrations.py
+-rw-r--r--   0        0        0     1059 2023-05-03 14:04:40.497199 asociita-0.1.6.2/asociita/utils/showcase.py
+-rw-r--r--   0        0        0     1084 2023-04-07 16:30:34.501923 asociita-0.1.6.2/LICENSE
+-rw-r--r--   0        0        0      671 2023-05-27 09:30:33.141138 asociita-0.1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     2862 2023-04-18 20:10:20.511705 asociita-0.1.6.2/README.md
+-rw-r--r--   0        0        0     3998 1970-01-01 00:00:00.000000 asociita-0.1.6.2/setup.py
+-rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 asociita-0.1.6.2/PKG-INFO
```

### Comparing `asociita-0.1.6.1/asociita/components/archiver/archive_manager.py` & `asociita-0.1.6.2/asociita/components/archiver/archive_manager.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/components/evaluator/evaluation_manager.py` & `asociita-0.1.6.2/asociita/components/evaluator/evaluation_manager.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/components/evaluator/mr_evaluator.py` & `asociita-0.1.6.2/asociita/components/evaluator/mr_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/components/evaluator/or_evaluator.py` & `asociita-0.1.6.2/asociita/components/evaluator/or_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/components/nodes/federated_node.py` & `asociita-0.1.6.2/asociita/components/nodes/federated_node.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/components/orchestrator/evaluator_orchestrator.py` & `asociita-0.1.6.2/asociita/components/orchestrator/evaluator_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/components/orchestrator/fedopt_orchestrator.py` & `asociita-0.1.6.2/asociita/components/orchestrator/fedopt_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/components/orchestrator/generic_orchestrator.py` & `asociita-0.1.6.2/asociita/components/orchestrator/generic_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/datasets/fetch_data.py` & `asociita-0.1.6.2/asociita/datasets/fetch_data.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/datasets/load_cifar.py` & `asociita-0.1.6.2/asociita/datasets/load_cifar.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/datasets/load_mnist.py` & `asociita-0.1.6.2/asociita/datasets/load_mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/datasets/shard_splits.py` & `asociita-0.1.6.2/asociita/datasets/shard_splits.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/datasets/shard_transformation.py` & `asociita-0.1.6.2/asociita/datasets/shard_transformation.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/models/pytorch/cifar10.py` & `asociita-0.1.6.2/asociita/models/pytorch/cifar10.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/models/pytorch/federated_model.py` & `asociita-0.1.6.2/asociita/models/pytorch/federated_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,16 @@
             self.trainloader, self.testloader = self.prepare_data(local_dataset)
         # If only a test dataset was provided.
         elif len(local_dataset) == 1:
             self.testloader = self.prepare_data(local_dataset, only_test=True)
         else:
             raise "The provided dataset object seem to be wrong. Please provide list[train_set, test_set] or list[test_set]"
 
+        device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+        model_logger.info()
 
         # List containing all the parameters to update
         params_to_update = []
         for _, param in self.net.named_parameters():
             if param.requires_grad is True:
                 params_to_update.append(param)
```

### Comparing `asociita-0.1.6.1/asociita/models/pytorch/mnist.py` & `asociita-0.1.6.2/asociita/models/pytorch/mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/utils/computations.py` & `asociita-0.1.6.2/asociita/utils/computations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/utils/custom_transformations.py` & `asociita-0.1.6.2/asociita/utils/custom_transformations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/utils/handlers.py` & `asociita-0.1.6.2/asociita/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/utils/helpers.py` & `asociita-0.1.6.2/asociita/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/utils/loggers.py` & `asociita-0.1.6.2/asociita/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/utils/optimizers.py` & `asociita-0.1.6.2/asociita/utils/optimizers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/utils/orchestrations.py` & `asociita-0.1.6.2/asociita/utils/orchestrations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/asociita/utils/showcase.py` & `asociita-0.1.6.2/asociita/utils/showcase.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/LICENSE` & `asociita-0.1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/pyproject.toml` & `asociita-0.1.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asociita"
-version = "0.1.6.1"
+version = "0.1.6.2"
 description = "An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting."
 authors = ["Maciej Zuziak <maciejkrzysztof.zuziak@isti.cnr.it>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Scolpe/Asociita"
 repository = "https://github.com/Scolpe/Asociita"
```

### Comparing `asociita-0.1.6.1/README.md` & `asociita-0.1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.1/setup.py` & `asociita-0.1.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'numpy>=1.24.1,<2.0.0',
  'scikit-learn>=1.2.0,<2.0.0',
  'torch>=1.13.1,<2.0.0',
  'torchvision>=0.14.1,<0.15.0']
 
 setup_kwargs = {
     'name': 'asociita',
-    'version': '0.1.6.1',
+    'version': '0.1.6.2',
     'description': "An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting.",
     'long_description': '### Setting Configuration\n\nIn order to run the simulation, the `Orchestrator` instance must receive a `settings` object that contains all the necessary parameters. It is possible to store those parameters in a `JSON` format and load them as the Python dictionary by using `asociita.utils.helper.load_from_json` function. Below is an exemplary settings object embedded as a `json` file. All the elements are necessary unless stated otherwise.\n\n```\n{\n    "orchestrator":{\n        "iterations": int,\n        "number_of_nodes": int,\n        "local_warm_start": bool,\n        "sample_size": int,\n        "evaluation": "none" | "full"\n        "save_metrics": bool,\n\t"save_models": bool,\n\t"save_path": str\n\t"nodes": [0,\n\t1,\n\t2]\n    },\n    "nodes":{\n    "local_epochs": int,\n    "model_settings": {\n        "optimizer": "RMS",\n        "batch_size": int,\n        "learning_rate": float}\n        }\n}\n```\n\nThe `settings` contains two dictionaries: `orchestrator` and `nodes`.\n\n`orchestrator` contains all the settings necessary details of the training:\n\n* `iterations` is the number of rounds to be performed. Example: `iterations:12`\n* `number_of_nodes` is the number of nodes that will be included in the training. Example: `number_of_nodes: 10`\n* `local_warm_start` allows to distribute various pre-trained weights to different local clients. Not implemeneted yet. Example: `local_warm_start: false`.\n* `sample_size` is the size of the sample that will be taken each round. Example: `sample_size : 4.`\n* `evaluation` allows to control the evaluation procedure across the clients.  Currently, only `none` or `full` are supported. Setting the evaluation to full will perform a full evaluation of every client included in the training. Example: `evaluation: full`\n* `save_metrics` allows to control whether the metrics should be saved in a csv file. Example: `save_metrics: true.`\n* `save_models` allows to control whether the models should be saved. Not implemeneted yet. Example: `save_metrics: false`.\n* `save_path` is the system path that will be used when saving the model. It is possible to define a saving_path in a method call.\n* `nodes` is the list containing the ids of all the nodes participating in the training. Length of `nodes` must be equal `number_of_nodes`.\n\n`nodes` contains all the necessary configuration for nodes.\n\n* `"local_epochs":` the number of local epochs to be performed on the local nodes.\n* `"model_settings"` is a dictionary containing all the parameters for training the model.\n  * `optimizer` is an optimizer that will be used during the training. Example: `optimizer: "RMS"`\n  * `batch_size` is the batch size that will be used during the training. Example: `batch_size: 32`\n  * `learning_rate` is the learning rate that will be used during the training. Example: `learning_rate: 0.001`\n',
     'author': 'Maciej Zuziak',
     'author_email': 'maciejkrzysztof.zuziak@isti.cnr.it',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Scolpe/Asociita',
```

### Comparing `asociita-0.1.6.1/PKG-INFO` & `asociita-0.1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asociita
-Version: 0.1.6.1
+Version: 0.1.6.2
 Summary: An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting.
 Home-page: https://github.com/Scolpe/Asociita
 License: MIT
 Author: Maciej Zuziak
 Author-email: maciejkrzysztof.zuziak@isti.cnr.it
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

