# Comparing `tmp/torchility-0.6.9.tar.gz` & `tmp/torchility-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchility-0.6.9.tar", last modified: Mon May 15 12:12:54 2023, max compression
+gzip compressed data, was "torchility-0.7.0.tar", last modified: Sat May 27 07:51:04 2023, max compression
```

## Comparing `torchility-0.6.9.tar` & `torchility-0.7.0.tar`

### file list

```diff
@@ -1,39 +1,44 @@
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 12:12:54.015920 torchility-0.6.9/
--rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.6.9/LICENSE
--rw-r--r--   0 liuchen    (501) staff       (20)     2074 2023-05-15 12:12:54.014770 torchility-0.6.9/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)     1595 2023-03-20 06:35:45.000000 torchility-0.6.9/README.md
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 12:12:53.988128 torchility-0.6.9/examples/
--rw-r--r--   0 liuchen    (501) staff       (20)     1728 2023-05-13 05:23:14.000000 torchility-0.6.9/examples/1-mnist.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2663 2023-03-28 13:54:47.000000 torchility-0.6.9/examples/2-mnist_callbacks.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-15 07:37:59.000000 torchility-0.6.9/examples/3-mnist_interpreter.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1645 2023-05-15 07:55:10.000000 torchility-0.6.9/examples/4-mnist_model_analysis.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.6.9/examples/5-mnist_lr_find.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.6.9/examples/6-graph_node_clasification_DGL.py
--rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-05-15 12:12:54.016115 torchility-0.6.9/setup.cfg
--rw-r--r--   0 liuchen    (501) staff       (20)     1117 2023-05-05 12:13:44.000000 torchility-0.6.9/setup.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 12:12:53.992376 torchility-0.6.9/torchility/
--rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-05-15 12:09:07.000000 torchility-0.6.9/torchility/__init__.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 12:12:54.006213 torchility-0.6.9/torchility/callbacks/
--rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.6.9/torchility/callbacks/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1205 2023-05-15 08:23:01.000000 torchility-0.6.9/torchility/callbacks/common.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4840 2023-05-05 13:46:18.000000 torchility-0.6.9/torchility/callbacks/interpreters.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.6.9/torchility/callbacks/performances.py
--rw-r--r--   0 liuchen    (501) staff       (20)     9598 2023-05-15 12:11:12.000000 torchility-0.6.9/torchility/callbacks/progress.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1102 2023-05-15 09:10:40.000000 torchility-0.6.9/torchility/datamodule.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.6.9/torchility/hooks.py
--rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.6.9/torchility/losses.py
--rw-r--r--   0 liuchen    (501) staff       (20)     5023 2023-05-15 07:26:34.000000 torchility-0.6.9/torchility/metrics.py
--rw-r--r--   0 liuchen    (501) staff       (20)     6694 2023-05-15 08:53:50.000000 torchility-0.6.9/torchility/tasks.py
--rw-r--r--   0 liuchen    (501) staff       (20)    10682 2023-05-15 11:48:35.000000 torchility-0.6.9/torchility/trainer.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 12:12:54.013665 torchility-0.6.9/torchility/utils/
--rw-r--r--   0 liuchen    (501) staff       (20)       96 2023-05-15 04:51:01.000000 torchility-0.6.9/torchility/utils/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2525 2023-05-15 09:18:12.000000 torchility-0.6.9/torchility/utils/metric_utils.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.6.9/torchility/utils/plots.py
--rw-r--r--   0 liuchen    (501) staff       (20)     6050 2023-05-05 01:14:22.000000 torchility-0.6.9/torchility/utils/utils.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3014 2022-08-04 03:32:03.000000 torchility-0.6.9/torchility/utils/yaml_config.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 12:12:53.999542 torchility-0.6.9/torchility.egg-info/
--rw-r--r--   0 liuchen    (501) staff       (20)     2074 2023-05-15 12:12:53.000000 torchility-0.6.9/torchility.egg-info/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)      853 2023-05-15 12:12:53.000000 torchility-0.6.9/torchility.egg-info/SOURCES.txt
--rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-05-15 12:12:53.000000 torchility-0.6.9/torchility.egg-info/dependency_links.txt
--rw-r--r--   0 liuchen    (501) staff       (20)       83 2023-05-15 12:12:53.000000 torchility-0.6.9/torchility.egg-info/requires.txt
--rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-05-15 12:12:53.000000 torchility-0.6.9/torchility.egg-info/top_level.txt
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 07:51:04.494789 torchility-0.7.0/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.7.0/LICENSE
+-rw-r--r--   0 liuchen    (501) staff       (20)     2119 2023-05-27 07:51:04.494413 torchility-0.7.0/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)     1640 2023-05-27 07:50:27.000000 torchility-0.7.0/README.md
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 07:51:04.479923 torchility-0.7.0/examples/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1872 2023-05-27 07:45:07.000000 torchility-0.7.0/examples/1-mnist.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1645 2023-05-15 07:55:10.000000 torchility-0.7.0/examples/10-model_analysis.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.7.0/examples/11-graph_node_clasification_DGL.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2073 2023-05-27 07:49:20.000000 torchility-0.7.0/examples/2-metrics_basic.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2064 2023-05-21 03:49:55.000000 torchility-0.7.0/examples/3-metrics_more.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1738 2023-05-19 08:52:25.000000 torchility-0.7.0/examples/4-callbacks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.7.0/examples/5-lr_find.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1563 2023-05-16 01:20:14.000000 torchility-0.7.0/examples/6-optimizer.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-15 07:37:59.000000 torchility-0.7.0/examples/7-interpreter.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2531 2023-05-19 12:30:31.000000 torchility-0.7.0/examples/8-multi_dataloaders.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1623 2023-05-16 00:41:34.000000 torchility-0.7.0/examples/9-reset_train_dataloader.py
+-rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-05-27 07:51:04.494950 torchility-0.7.0/setup.cfg
+-rw-r--r--   0 liuchen    (501) staff       (20)     1163 2023-05-27 06:45:49.000000 torchility-0.7.0/setup.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 07:51:04.486096 torchility-0.7.0/torchility/
+-rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-05-27 07:49:35.000000 torchility-0.7.0/torchility/__init__.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 07:51:04.491602 torchility-0.7.0/torchility/callbacks/
+-rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.7.0/torchility/callbacks/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1656 2023-05-23 02:30:14.000000 torchility-0.7.0/torchility/callbacks/common.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4840 2023-05-05 13:46:18.000000 torchility-0.7.0/torchility/callbacks/interpreters.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.7.0/torchility/callbacks/performances.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     9598 2023-05-15 12:11:12.000000 torchility-0.7.0/torchility/callbacks/progress.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1102 2023-05-15 09:10:40.000000 torchility-0.7.0/torchility/datamodule.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.7.0/torchility/hooks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.7.0/torchility/losses.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     6541 2023-05-18 13:56:01.000000 torchility-0.7.0/torchility/metrics.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     5695 2023-05-23 02:30:35.000000 torchility-0.7.0/torchility/tasks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)    12469 2023-05-27 07:48:28.000000 torchility-0.7.0/torchility/trainer.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 07:51:04.493859 torchility-0.7.0/torchility/utils/
+-rw-r--r--   0 liuchen    (501) staff       (20)       96 2023-05-15 04:51:01.000000 torchility-0.7.0/torchility/utils/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2647 2023-05-21 03:41:57.000000 torchility-0.7.0/torchility/utils/metric_utils.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.7.0/torchility/utils/plots.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     6816 2023-05-18 13:11:06.000000 torchility-0.7.0/torchility/utils/utils.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3014 2022-08-04 03:32:03.000000 torchility-0.7.0/torchility/utils/yaml_config.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-27 07:51:04.489230 torchility-0.7.0/torchility.egg-info/
+-rw-r--r--   0 liuchen    (501) staff       (20)     2119 2023-05-27 07:51:04.000000 torchility-0.7.0/torchility.egg-info/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)      979 2023-05-27 07:51:04.000000 torchility-0.7.0/torchility.egg-info/SOURCES.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-05-27 07:51:04.000000 torchility-0.7.0/torchility.egg-info/dependency_links.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)      112 2023-05-27 07:51:04.000000 torchility-0.7.0/torchility.egg-info/requires.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-05-27 07:51:04.000000 torchility-0.7.0/torchility.egg-info/top_level.txt
```

### Comparing `torchility-0.6.9/LICENSE` & `torchility-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchility-0.6.9/PKG-INFO` & `torchility-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.6.9
+Version: 0.7.0
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -20,17 +20,19 @@
 A tool for training pytorch deep learning model more simply which is based on Pytorch-lightning.
 
 ## Install
 
 - `pip install torchility`
 ### Dependency
 - pytorch>=2.0
-- pytorch-lightning>=2.0
-- torchmetrics>=0.11
+- pytorch-lightning>=2.0,<2.1
+- torchmetrics>=0.11,<0.12
 - matplotlib>=3.3
+- pyyaml>=5.4
+- tensorboardX>=2.6
 
 ## Usage
 
 - MNIST
 
 ```python
 from torchility import Trainer
```

### Comparing `torchility-0.6.9/README.md` & `torchility-0.7.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 A tool for training pytorch deep learning model more simply which is based on Pytorch-lightning.
 
 ## Install
 
 - `pip install torchility`
 ### Dependency
 - pytorch>=2.0
-- pytorch-lightning>=2.0
-- torchmetrics>=0.11
+- pytorch-lightning>=2.0,<2.1
+- torchmetrics>=0.11,<0.12
 - matplotlib>=3.3
+- pyyaml>=5.4
+- tensorboardX>=2.6
 
 ## Usage
 
 - MNIST
 
 ```python
 from torchility import Trainer
```

### Comparing `torchility-0.6.9/examples/1-mnist.py` & `torchility-0.7.0/examples/1-mnist.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,18 +33,20 @@
 
 
 # 3. --- 优化器
 opt = torch.optim.Adam(model.parameters(), lr=2e-4)
 
 
 # 4. --- 训练
-trainer = Trainer(model, F.cross_entropy, opt, epochs=2, logger=False)            # 训练器
-trainer.fit(train_dl, val_dl)                                       # 训练、验证
-trainer.test(test_dl)                                               # 测试
-trainer.predict(test_dl, has_label=True)
+trainer = Trainer(model, F.cross_entropy, opt, epochs=2, logger=False)  # 训练器
+trainer.fit(train_dl, val_dl)                                           # 训练、验证
+# trainer.test(test_dl)                                                 # 测试
+trainer.test(test_dl, do_loss=False)                                    # 测试过程中不计算损失
+trainer.predict(test_dl, has_label=True)                                # 预测
+
 
 """ 使用GPU
 # 默认情况下自动选择可用的GPU，如下两种形式相同
 trainer = Trainer()
 trainer = Trainer(accelerator="auto", devices="auto", strategy="auto") 
 
 # 使用一个GPU
```

### Comparing `torchility-0.6.9/examples/2-mnist_callbacks.py` & `torchility-0.7.0/examples/7-interpreter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from pytorch_lightning.callbacks import ModelCheckpoint, EarlyStopping
-from torchility import Trainer
-from torch.utils.data import DataLoader, random_split
-from torchvision import transforms
-from torchvision.datasets import MNIST
-from torch.nn import functional as F
-from torchmetrics import Accuracy, F1Score
-from torch import nn
 import torch
+from torch import nn
+from torch.nn import functional as F
+from torchvision.datasets import MNIST
+from torchvision import transforms
+from torch.utils.data import DataLoader, random_split
+from torchility import Trainer
+from torchility.callbacks import ClassifierInterpreter
+import matplotlib.pyplot as plt
 import warnings
-
 warnings.simplefilter("ignore")
 
+
 # 1. --- 数据
 data_dir = './datasets'
-transform = transforms.Compose([transforms.ToTensor(), transforms.Normalize((0.1307,), (0.3081,))])
+transform = transforms.Compose([transforms.ToTensor()])
 mnist_full = MNIST(data_dir, train=True, transform=transform, download=True)
 train_ds, val_ds = random_split(mnist_full, [55000, 5000])
 test_ds = MNIST(data_dir, train=False, transform=transform, download=True)
 train_dl = DataLoader(train_ds, batch_size=32)
 val_dl = DataLoader(val_ds, batch_size=32)
 test_dl = DataLoader(test_ds, batch_size=32)
 
@@ -34,39 +34,39 @@
     nn.Dropout(0.1),
     nn.Linear(64, 10)
 )
 
 
 # 3. --- 优化器
 opt = torch.optim.Adam(model.parameters(), lr=2e-4)
-scheduler = torch.optim.lr_scheduler.StepLR(opt, 8, gamma=0.1, last_epoch=-1)
 
 
 # 4. --- 训练
-acc = 'acc', Accuracy(task='multiclass', num_classes=10)
-acc1 = 'acc1', Accuracy(task='multiclass', average='macro', num_classes=10)
-f1 = 'f1', F1Score(task='multiclass', average='macro', num_classes=10)
-
-def acc2(preds, targets):
-    preds = preds.argmax(1)
-    return (preds == targets).float().mean()
-
-def acc3(preds, targets):
-    """一个函数计算多个指标"""
-    preds = preds.argmax(1)
-    return {'a':(preds == targets).float().mean(), 'b':(preds == targets).float().mean()}
-
-# 早停callback
-early_stop_cbk = EarlyStopping(monitor='val_loss', min_delta=0.00, patience=3, verbose=False, mode='min')
-model_cbk = ModelCheckpoint(save_top_k=1, monitor='val_loss', mode='min')
-
-# 训练器，使用新的进度条，以及其他callbacks
-trainer = Trainer(model, F.cross_entropy, [opt, scheduler], epochs=10,
-                  metrics=[acc, acc1, acc2, acc3],
-                  callbacks=[
-                                model_cbk,
-                                early_stop_cbk,     # 早停
-                            ])
-progress = trainer.fit(train_dl, val_dl)            # 训练、验证
-trainer.test(test_dl, metrics=[f1, acc2, acc3], do_loss=False)  # 测试：metrics用于指定测试专用的指标，do_loss用于指定是否计算测试损失
 
-print(progress)  # 训练过程，包括训练和验证中的损失和其他指标
+# 要计算每个样本的指标，因此不能reduction（即求和、平均等操作）
+metric = nn.CrossEntropyLoss(reduction='none')
+
+interpreter = ClassifierInterpreter(metric=metric, k=15, class_num=10, stage='test')          # 针对分类模型测试数据的解释器
+trainer = Trainer(model, F.cross_entropy, opt,                           # 训练器
+                  epochs=5, callbacks=[interpreter])
+trainer.fit(train_dl, val_dl)                                            # 训练、验证
+trainer.test(test_dl)                                                    # 测试
+
+
+# 5. --- 解释
+
+# 返回测试集中损失最大的k个样本的信息
+tops = trainer.interpreter.top_samples()
+
+# 绘制损失最大的k个样本
+plt.figure(figsize=[10, 6])
+for i, sample in enumerate(tops):
+    loss, pred, target, x = sample
+    plt.subplot(3, 5, i+1)
+    plt.imshow(sample[3][0])
+    plt.title(f'{sample[0]:.3},  {target}->{pred.argmax()}')
+    plt.xticks([])
+    plt.yticks([])
+
+# 绘制混淆矩阵
+trainer.interpreter.plot_confusion()
+plt.show()
```

### Comparing `torchility-0.6.9/examples/3-mnist_interpreter.py` & `torchility-0.7.0/examples/4-callbacks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-import torch
-from torch import nn
-from torch.nn import functional as F
-from torchvision.datasets import MNIST
-from torchvision import transforms
-from torch.utils.data import DataLoader, random_split
+from pytorch_lightning.callbacks import ModelCheckpoint, EarlyStopping
 from torchility import Trainer
-from torchility.callbacks import ClassifierInterpreter
-import matplotlib.pyplot as plt
+from torch.utils.data import DataLoader, random_split
+from torchvision import transforms
+from torchvision.datasets import MNIST
+from torch.nn import functional as F
+from torch import nn
+import torch
 import warnings
-warnings.simplefilter("ignore")
 
+warnings.simplefilter("ignore")
 
 # 1. --- 数据
 data_dir = './datasets'
-transform = transforms.Compose([transforms.ToTensor()])
+transform = transforms.Compose([transforms.ToTensor(), transforms.Normalize((0.1307,), (0.3081,))])
 mnist_full = MNIST(data_dir, train=True, transform=transform, download=True)
 train_ds, val_ds = random_split(mnist_full, [55000, 5000])
 test_ds = MNIST(data_dir, train=False, transform=transform, download=True)
 train_dl = DataLoader(train_ds, batch_size=32)
 val_dl = DataLoader(val_ds, batch_size=32)
 test_dl = DataLoader(test_ds, batch_size=32)
 
@@ -38,35 +37,21 @@
 
 # 3. --- 优化器
 opt = torch.optim.Adam(model.parameters(), lr=2e-4)
 
 
 # 4. --- 训练
 
-# 要计算每个样本的指标，因此不能reduction（即求和、平均等操作）
-metric = nn.CrossEntropyLoss(reduction='none')
+# 早停callback
+early_stop_cbk = EarlyStopping(monitor='val_loss', min_delta=0.00, patience=3, verbose=False, mode='min')
+# 模型checkpoint callback
+model_cbk = ModelCheckpoint(save_top_k=1, monitor='val_loss', mode='min')
+
+# 训练器，使用新的进度条，以及其他callbacks
+trainer = Trainer(model, F.cross_entropy, opt, epochs=2,
+                  callbacks=[
+                                model_cbk,
+                                early_stop_cbk
+                            ])
+trainer.fit(train_dl, val_dl)
 
-interpreter = ClassifierInterpreter(metric=metric, k=15, class_num=10, stage='test')          # 针对分类模型测试数据的解释器
-trainer = Trainer(model, F.cross_entropy, opt,                           # 训练器
-                  epochs=5, callbacks=[interpreter])
-trainer.fit(train_dl, val_dl)                                            # 训练、验证
-trainer.test(test_dl)                                                    # 测试
-
-
-# 5. --- 解释
-
-# 返回测试集中损失最大的k个样本的信息
-tops = trainer.interpreter.top_samples()
-
-# 绘制损失最大的k个样本
-plt.figure(figsize=[10, 6])
-for i, sample in enumerate(tops):
-    loss, pred, target, x = sample
-    plt.subplot(3, 5, i+1)
-    plt.imshow(sample[3][0])
-    plt.title(f'{sample[0]:.3},  {target}->{pred.argmax()}')
-    plt.xticks([])
-    plt.yticks([])
-
-# 绘制混淆矩阵
-trainer.interpreter.plot_confusion()
-plt.show()
+trainer.test(test_dl)
```

### Comparing `torchility-0.6.9/examples/4-mnist_model_analysis.py` & `torchility-0.7.0/examples/10-model_analysis.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.9/examples/5-mnist_lr_find.py` & `torchility-0.7.0/examples/5-lr_find.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.9/examples/6-graph_node_clasification_DGL.py` & `torchility-0.7.0/examples/11-graph_node_clasification_DGL.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.9/setup.py` & `torchility-0.7.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,11 +19,11 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     keywords='',
     packages=setuptools.find_packages(exclude=['__pycache__', '__pycache__/*']),
     py_modules=[],  # any single-file Python modules that aren’t part of a package
-    install_requires=['torch>=2.0', 'pytorch-lightning==2.0', 'torchmetrics==0.11.4', 'matplotlib>=3.3','pyyaml>=5.4'],
-    # install_requires=['torch>=2.0', 'pytorch-lightning>=2.0,<2.1', 'torchmetrics>=0.11.4', 'matplotlib>=3.3','pyyaml>=5.4'],
+    # install_requires=['torch>=2.0', 'pytorch-lightning==2.0', 'torchmetrics==0.11.4', 'matplotlib>=3.3','pyyaml>=5.4', 'tensorboard>2.9'],
+    install_requires=['torch>=2.0', 'pytorch-lightning>=2.0,<2.1', 'torchmetrics>=0.11.4,<0.12', 'matplotlib>=3.3','pyyaml>=5.4', 'tensorboardX>=2.6'],
     python_requires='>=3.8'
 )
```

### Comparing `torchility-0.6.9/torchility/callbacks/interpreters.py` & `torchility-0.7.0/torchility/callbacks/interpreters.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.9/torchility/callbacks/performances.py` & `torchility-0.7.0/torchility/callbacks/performances.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.9/torchility/callbacks/progress.py` & `torchility-0.7.0/torchility/callbacks/progress.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.9/torchility/datamodule.py` & `torchility-0.7.0/torchility/datamodule.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.9/torchility/hooks.py` & `torchility-0.7.0/torchility/hooks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.9/torchility/losses.py` & `torchility-0.7.0/torchility/losses.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.9/torchility/tasks.py` & `torchility-0.7.0/torchility/tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from pytorch_lightning import LightningModule
 from torchmetrics import Metric
-from .utils import detach_clone
+from .utils import detach_clone, get_batch_size
 from torch.optim.lr_scheduler import LRScheduler
 from torch.optim import Optimizer
 from typing import Any
+from .callbacks.common import dict_metric_name
 
 
 class GeneralTaskModule(LightningModule):
     def __init__(self, model, loss, optimizer, metrics=None, **kwargs):
         super().__init__(**kwargs)
         self.model = model
         self.loss_fn = loss
         self.opt = optimizer
         self.metrics = metrics
         self.messages = dict()          # 存放训练、验证、测试过程中的各种消息数据
-        self.do_test_loss = True
         self.pred_dataloader_has_label = True
         self.current_dl_idx = 0
 
     def forward(self, *batch_data):                         # 前向计算
         return self.model(*batch_data)
 
     def on_train_start(self):
@@ -34,53 +34,58 @@
 
     def training_step(self, batch, batch_nb):               # 训练步
         loss, preds, targets, batch_size = self.do_forward(batch)
         self.log('train_loss', loss, prog_bar=True, on_step=True, on_epoch=True, batch_size=batch_size)
 
         preds, targets = detach_clone(preds), detach_clone(targets)
         if self.metrics:
-            metric_values = self.do_metric(preds, targets, 'train', batch_size, 0)
+            metric_values = self.do_metric(preds, targets, 'train', 0)
         self.messages['train_batch'] = (batch_nb, preds, targets)  # (batch_idx, preds, tagets)
         metric_values['loss'] = loss
         return metric_values
 
     def validation_step(self, batch, batch_nb, dataloader_idx=0):             # 验证步
-        loss, preds, targets, batch_size = self.do_forward(batch)
-        self.log('val_loss', loss, prog_bar=True, on_step=True, on_epoch=True, batch_size=batch_size)
+        do_loss = self.do_val_loss
+        if isinstance(do_loss, (list, tuple)):
+            do_loss = dataloader_idx in do_loss
+        loss, preds, targets, batch_size = self.do_forward(batch, do_loss)
 
         metric_values = {}
-        if self.multi_val_dataloaders:
-            metric_values[f'loss/{dataloader_idx}'] = loss
-        else:
-            metric_values['loss'] = loss
+        if loss is not None:
+            self.log('val_loss', loss, prog_bar=True, on_step=True, on_epoch=True, batch_size=batch_size)
+            if self.multi_val_dataloaders:
+                metric_values[f'loss/{dataloader_idx}'] = loss
+            else:
+                metric_values['loss'] = loss
 
         preds, targets = detach_clone(preds), detach_clone(targets)
         if self.metrics:
             dl_idx = dataloader_idx if self.multi_val_dataloaders else -1
-            metric_values.update(self.do_metric(preds, targets, 'val', batch_size, dl_idx))
+            metric_values.update(self.do_metric(preds, targets, 'val', dl_idx))
         self.messages['val_batch'] = (batch_nb, preds, targets)  # (batch_idx, preds, tagets)
 
         return metric_values
 
     def test_step(self, batch, batch_nb, dataloader_idx=0):                   # 测试步
-        loss, preds, targets, batch_size = self.do_forward(batch, self.do_test_loss)
-        if loss is not None:
-            self.log('test_loss', loss, prog_bar=True, on_step=True, on_epoch=True, batch_size=batch_size)
+        do_loss = self.do_test_loss
+        if isinstance(do_loss, (list, tuple)):
+            do_loss = dataloader_idx in do_loss
+        loss, preds, targets, _ = self.do_forward(batch, do_loss)
 
         metric_values = {}
         if loss is not None:
             if self.multi_test_dataloaders:
                 metric_values[f'loss/{dataloader_idx}'] = loss
             else:
                 metric_values['loss'] = loss
 
         preds, targets = detach_clone(preds), detach_clone(targets)
         if self.metrics:
             dl_idx = dataloader_idx if self.multi_test_dataloaders else -1
-            metric_values.update(self.do_metric(preds, targets, 'test', batch_size, dl_idx))
+            metric_values.update(self.do_metric(preds, targets, 'test', dl_idx))
         self.messages['test_batch'] = (batch_nb, preds, targets)  # (batch_idx, preds, tagets)
 
         return metric_values
 
     def predict_step(self, batch: Any, batch_idx: int, dataloader_idx: int = 0) -> Any:
         _, preds, _, _ = self.do_forward(batch, False, self.pred_dataloader_has_label)
         return preds
@@ -104,47 +109,23 @@
             if not isinstance(input_feat, (list, tuple)):
                 input_feat = [input_feat]
         preds = self(*input_feat)
         if do_loss:
             loss = self.loss_fn(preds, targets)
         else:
             loss = None
-        batch_size = self._batch_size(input_feat)
+        batch_size = get_batch_size(input_feat)
         return loss, preds, targets, batch_size
 
-    def do_metric(self, preds, targets, stage, batch_size, dl_idx):  # 指标计算
+    def do_metric(self, preds, targets, stage, dl_idx):  # 指标计算
         metrics = self.metrics[stage]
         metric_values = {}
         for metric in metrics:
             if (metric.dl_idx >=0 and metric.dl_idx != dl_idx) or (stage not in metric.stages):
                 continue
             value = metric(preds, targets)
             if isinstance(value, dict):  # 一个函数中计算多个指标，返回一个字典
-                value_dict = {f"{stage}_{metric.name}{k}_step":v for k, v in value.items()}
                 for k, v in value.items():
-                    metric_values[f"{metric.name}{k}"] = v.item()
-                self.log_dict(value_dict, prog_bar=metric.on_bar, on_step=metric.on_step, on_epoch=False, batch_size=batch_size)
+                    metric_values[dict_metric_name(metric.name, k)] = v
             else:
-                metric_values[f"{metric.name}"] = value.item()
-                self.log(f"{stage}_{metric.name}_step", value, prog_bar=metric.on_bar, on_step=metric.on_step, on_epoch=False, batch_size=batch_size)
+                metric_values[f"{metric.name}"] = value
         return metric_values
-
-    def _batch_size(self, inputs):
-        """检测batch size以用于输出日志"""
-        if isinstance(inputs, (tuple, list)):
-            data = inputs[0]
-        else:
-            data = inputs
-        if hasattr(data, 'shape'):
-            return data.shape[0]
-        elif hasattr(data, '__len__'):
-            return len(data)
-        else:
-            data_type = f'{type(data).__module__}.{type(data).__name__}'
-            if data_type == 'dgl.heterograph.DGLHeteroGraph':
-                return data.batch_size
-            elif data_type == 'torch_geometric.data.batch.DataBatch':
-                return data.num_graphs
-            elif data_type == 'torch_geometric.data.data.Data':
-                return 1
-            else:
-                return None
```

### Comparing `torchility-0.6.9/torchility/trainer.py` & `torchility-0.7.0/torchility/trainer.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     def __init__(self, model:torch.nn.Module=None,  # pytorch Module
         loss:Callable=None,                         # loss function
         optimizer:torch.optim.Optimizer=None,       # pytorch optimizer
         epochs:int=None,                            # max epochs
         metrics:Union[Callable, Metric]=(),         # instance of torchmetrics.Metric or other callable instance
         task_module: LightningModule=None,          # task_model
         default_bar=False,                          # 是否使用默认进度条
-        reset_dl:int=0,                             # 每隔多个少epoch重置一次训练DataLoader，与reload_dataloaders_every_n_epochs相似
+        reset_dl:int=0,                             # 每隔多少个epoch重置一次训练DataLoader，与reload_dataloaders_every_n_epochs相似
+        val_frac=1,                                 # 每隔多少个epoch验证一次，与check_val_every_n_epoch相同
         task_kwargs:dict=None,                      # parameters dict of the task_module
         **pltrainer_kwargs                          # keyword arguments of pytorch_lightning Trainer
         ):
         self.init_params = default_args(PLTrainer)
         self.progress = None
         self.best_model = None   # 训练中最好的torch模型
 
@@ -54,14 +55,16 @@
         #   *************************************
         #   *    Trainer Parameters    --- LIC  *
         #   *************************************
         if epochs is not None:  # for easy use
             self.init_params['max_epochs'] = epochs
         if pltrainer_kwargs.get('log_every_n_steps', None) is None: # log each step
             pltrainer_kwargs['log_every_n_steps'] = 1
+        if pltrainer_kwargs.get('check_val_every_n_epoch', None) is None:  # val freq
+            pltrainer_kwargs['check_val_every_n_epoch'] = val_frac
         self.init_params.update(pltrainer_kwargs)     # get default arguments
         self.init_params['num_sanity_val_steps'] = 0  # how many validation steps to execute before running
 
         # === set callbacks
         cbks = [ResetMetrics()]
         if self.init_params['callbacks'] is not None:
             cbks.extend(self.init_params['callbacks'])
@@ -81,51 +84,79 @@
             self.init_params['logger'] = TensorBoardLogger(log_dir, name=None, log_graph=True, default_hp_metric=False)
 
         # === reset dataloader
         self.reset_dl = reset_dl
         if reset_dl > 0:
             self.init_params['reload_dataloaders_every_n_epochs'] = reset_dl
 
+        self.val_epoch_metric_values = {}
+        self.train_epoch_metric_values = {}
+        self.test_epoch_metric_values = {}
+
         super().__init__(**self.init_params)
 
     def _prepare_metrics(self, metrics, just_for_test=False):
         metrics_ready = {'train': [], 'val':[], 'test':[]}
         for m in metrics:
             m = set_metric_attr(m)
             if just_for_test:
                 metrics_ready['test'].append(m)
             else:
                 for stage in m.stages:
                     metrics_ready[stage].append(m.clone())
         del metrics
         return metrics_ready if not just_for_test else metrics_ready['test']
 
-    def fit(self, train_dl, val_dls=None, ckpt_path=None):
+    def fit(self, train_dl, val_dls=None, ckpt_path=None, do_val_loss=True):
+        """
+        Args:
+            train_dl: 用于训练的dataloader
+            val_dls:  用于验证的一个dataloader或多个dataloader列表
+            ckpt_path: checkpoints保存路径
+            do_val_loss: True表示在验证时计算损失；
+                         False表示验证时不计算损失；
+                         int 表示在使用多个验证dataloader时，在哪个dataloader上计算损失
+                         [int, ...]整数列表，表示在在哪些dataloader上计算损失
+        """
+        if isinstance(do_val_loss, (list, tuple)):
+            assert isinstance(val_dls, (list, tuple)), 'do_val_loss 的取值为val_dls中dataloader对应的id'
+            assert len(do_val_loss) < len(val_dls), 'do_val_loss 的取值为val_dls中dataloader对应的id'
+        elif do_val_loss.__class__ is int:
+            do_val_loss = [do_val_loss]
+        self.task_module.do_val_loss = do_val_loss
+
         self.task_module.multi_val_dataloaders = False  # 是否使用多个验证dataloader
         if isinstance(val_dls, (list, tuple)) and len(val_dls) > 1:
             self.task_module.multi_val_dataloaders = True
 
         dm = GeneralDataModule(train_dl=train_dl, val_dls=val_dls, reset=self.reset_dl)
         self.datamodule = dm
         super().fit(self.task_module, datamodule=dm, ckpt_path=ckpt_path)
         return self.progress
 
     def test(self, test_dls, ckpt_path='best', verbose=True, metrics=None, do_loss=True):  # pylint: disable=arguments-renamed
         """
         Args:
             metrics: 一旦提供了test的metrics，则会将trainer中用于test的metrics覆盖，也就是说可以指定仅用于test的metrics
-            do_loss: 在测试时是否计算损失函数，当测试任务和训练任务数据不一致无法计算损失函数时，可设do_loss=False
+            do_loss: True表示在测试时计算损失；
+                     False表示测试时不计算损失；
+                     [int, ...]整数列表示在使用多个测试dataloader时，在哪些dataloader上计算损失
         """
         print('-' * 35)
+        if isinstance(do_loss, (list, tuple)):
+            assert isinstance(test_dls, (list, tuple)), 'do_loss 的取值为test_dls中dataloader对应的id'
+            assert len(do_loss) < len(test_dls), 'do_loss 的取值为test_dls中dataloader对应的id'
+        elif do_loss.__class__ is int:
+            do_loss = [do_loss]
+        self.task_module.do_test_loss = do_loss
 
         self.task_module.multi_test_dataloaders = False          # 是否使用多个测试dataloader
         if isinstance(test_dls, (list, tuple)) and len(test_dls) > 1:
             self.task_module.multi_test_dataloaders = True
 
-        self.task_module.do_test_loss = do_loss
         if metrics is not None:  # 如果提供了仅用于test的metrics
             test_metrics = self._prepare_metrics(metrics, just_for_test=True)
             self.task_module.metrics['test'] = test_metrics
 
         dm = GeneralDataModule(test_dls=test_dls)
         super().test(self.task_module, datamodule=dm, ckpt_path=ckpt_path, verbose=False)
```

### Comparing `torchility-0.6.9/torchility/utils/metric_utils.py` & `torchility-0.7.0/torchility/utils/metric_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 from ..metrics import MetricBase
 from torchmetrics import Metric
 
 
-def set_metric_attr(metric, name=None, stages=None, dl_idx:int=None, on_step:bool=None, on_epoch:bool=None, on_bar:bool=None):
+def set_metric_attr(metric, name=None, stages=None, dl_idx:int=None, simple_cumulate=None, log:bool=None, on_bar:bool=None):
     """
     Args:
-        metric: 指标
-        name: 指标名
-        stages: 在哪些阶段运行，取值为 'train', 'val', 'test' 或者它们组成的列表，默认值 ['train', 'val', 'test']
-        dl_idx: 验证或测试阶段使用多个dataloader时，指标运行在哪个dataloader之上，默认值 -1 表示所有的dataloader
-        on_step: 是否将每个batch的指标值记入日志，默认值 True
-        on_epoch: 是否将每个epoch的指标值记入日志，默认值 False
-        on_bar: 指标是否在pytorch_lightning内置的进度条上显示，默认值 True
+        metric:   指标
+        name:     指标名
+        stages:   在哪些阶段运行，取值为 'train', 'val', 'test' 或者它们组成的列表，默认值 ['train', 'val', 'test']
+        dl_idx:   验证或测试阶段使用多个dataloader时，指标运行在哪个dataloader之上，默认值 -1 表示所有的dataloader
+        simple_cumulate: MetricBase子类是否采用简单累积方式计算Epoch指标（利用batch_size累积指标值，效率高但不适用于基于混淆矩阵的指标），默认为False
+        log:      是否将计算结果记入日志，默认值 True
+        on_bar:   指标是否在pytorch_lightning内置的进度条上显示，默认值 True
     """
     # 默认属性取值
-    attr = {'name': None, 'stages': ['train', 'val', 'test'], 'dl_idx': -1,
-            'on_step': True, 'on_epoch': False, 'on_bar': True}
+    attr = {'name': None, 'stages': ['train', 'val', 'test'], 'dl_idx': -1, 'simple_cumulate': False, 'log': True, 'on_bar': True}
 
     if isinstance(metric, (tuple, list)):
         assert len(metric) == 2, "'`metric` should be a tuple of (metric_name, metric_callable) or (metric_callable, metric_name)"
         if callable(metric[0]):      # (metric_callable, dataloader_idx)
             metric, name_ = metric
         elif callable(metric[1]):    # (metric_name, metric_callable)
             name_, metric = metric
         attr['name'] = name_
     else:
         for k, v in attr.items():
             attr[k] = getattr(metric, k, v)
 
-    # 如果没有提供name
+    # 如果指标没有提供name
     if attr['name'] is None:
         attr['name'] = metric.__name__ if hasattr(metric, '__name__') else type(metric).__name__
 
     if not isinstance(metric, (Metric, MetricBase)):  # 如果指标是一个函数（或其他可调用对象）
         metric = MetricBase(metric)
 
     if name is not None:
@@ -44,18 +43,18 @@
         else:
             assert stages in ['train', 'val', 'test']
             stages = [stages]
         attr['stages'] = stages
     if dl_idx is not None:
         attr['dl_idx'] = dl_idx
         attr['name'] = f"{attr['name']}/{dl_idx}"
-    if on_step is not None:
-        attr['on_step'] = on_step
-    if on_epoch is not None:
-        attr['on_epoch'] = on_epoch
+    if simple_cumulate is not None:
+        attr['simple_cumulate'] = simple_cumulate
+    if log is not None:
+        attr['log'] = log
     if on_bar is not None:
         attr['on_bar'] = on_bar
 
     # 设置指标属性
     for k, v in attr.items():
         setattr(metric, k, v)
```

### Comparing `torchility-0.6.9/torchility/utils/plots.py` & `torchility-0.7.0/torchility/utils/plots.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.9/torchility/utils/utils.py` & `torchility-0.7.0/torchility/utils/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,23 +47,49 @@
         else:
             break
 
 
 def detach_clone(tensors):
     if isinstance(tensors, torch.Tensor):
         return tensors.detach().clone()
-    else:
+    elif isinstance(tensors, (list, tuple)):
         return [detach_clone(t) for t in tensors]
+    else:
+        return tensors
+
 
 def concat(tensor_lst, dim=0):
     if isinstance(tensor_lst[0], (list, tuple)):
         return [torch.concat(ts, dim) for ts in zip(*tensor_lst)]
     else:
         return torch.concat(tensor_lst, dim)
 
+
+def get_batch_size(inputs):
+    """检测batch size"""
+    if isinstance(inputs, (tuple, list)):
+        data = inputs[0]
+    else:
+        data = inputs
+    if hasattr(data, 'shape'):
+        return data.shape[0]
+    elif hasattr(data, '__len__'):
+        return len(data)
+    else:
+        data_type = f'{type(data).__module__}.{type(data).__name__}'
+        if data_type == 'dgl.heterograph.DGLHeteroGraph':
+            return data.batch_size
+        elif data_type == 'torch_geometric.data.batch.DataBatch':
+            return data.num_graphs
+        elif data_type == 'torch_geometric.data.data.Data':
+            return 1
+        else:
+            raise ValueError('Unknown batch size!')
+
+
 class TensorTuple(tuple):
     """
     list of tensors
     """
     @property
     def device(self):
         if len(self) > 0:
@@ -94,14 +120,15 @@
         return TensorTuple(t.long() for t in self)
 
     def int(self):
         return TensorTuple(t.int() for t in self)
 
 TensorList = TensorTuple
 
+
 def rename(newname):
     def decorator(f):
         f.__name__ = newname
         return f
     return decorator
 
 
@@ -161,15 +188,14 @@
     plt.xlabel('Prediction')
     plt.grid(False)
     # plt.tight_layout()
     fig.subplots_adjust(bottom=0.15)
     return fig
 
 
-
 def unpack(data, num=None):
     """
     unpack data to given number of variables.
     Example:
         Code:
             data = [1, 2]
             x, y, z = unpack(data, 3)
```

### Comparing `torchility-0.6.9/torchility/utils/yaml_config.py` & `torchility-0.7.0/torchility/utils/yaml_config.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.9/torchility.egg-info/PKG-INFO` & `torchility-0.7.0/torchility.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.6.9
+Version: 0.7.0
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -20,17 +20,19 @@
 A tool for training pytorch deep learning model more simply which is based on Pytorch-lightning.
 
 ## Install
 
 - `pip install torchility`
 ### Dependency
 - pytorch>=2.0
-- pytorch-lightning>=2.0
-- torchmetrics>=0.11
+- pytorch-lightning>=2.0,<2.1
+- torchmetrics>=0.11,<0.12
 - matplotlib>=3.3
+- pyyaml>=5.4
+- tensorboardX>=2.6
 
 ## Usage
 
 - MNIST
 
 ```python
 from torchility import Trainer
```

### Comparing `torchility-0.6.9/torchility.egg-info/SOURCES.txt` & `torchility-0.7.0/torchility.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 LICENSE
 README.md
 setup.py
 examples/1-mnist.py
-examples/2-mnist_callbacks.py
-examples/3-mnist_interpreter.py
-examples/4-mnist_model_analysis.py
-examples/5-mnist_lr_find.py
-examples/6-graph_node_clasification_DGL.py
+examples/10-model_analysis.py
+examples/11-graph_node_clasification_DGL.py
+examples/2-metrics_basic.py
+examples/3-metrics_more.py
+examples/4-callbacks.py
+examples/5-lr_find.py
+examples/6-optimizer.py
+examples/7-interpreter.py
+examples/8-multi_dataloaders.py
+examples/9-reset_train_dataloader.py
 torchility/__init__.py
 torchility/datamodule.py
 torchility/hooks.py
 torchility/losses.py
 torchility/metrics.py
 torchility/tasks.py
 torchility/trainer.py
```

