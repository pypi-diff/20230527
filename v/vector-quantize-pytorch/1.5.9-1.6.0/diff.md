# Comparing `tmp/vector_quantize_pytorch-1.5.9.tar.gz` & `tmp/vector_quantize_pytorch-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.5.9.tar", last modified: Wed May 24 16:45:35 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.6.0.tar", last modified: Sat May 27 16:22:23 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.5.9.tar` & `vector_quantize_pytorch-1.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:45:35.015181 vector_quantize_pytorch-1.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-24 16:45:21.000000 vector_quantize_pytorch-1.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-24 16:45:35.015181 vector_quantize_pytorch-1.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-05-24 16:45:21.000000 vector_quantize_pytorch-1.5.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:45:35.015181 vector_quantize_pytorch-1.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-24 16:45:21.000000 vector_quantize_pytorch-1.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:45:35.011181 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-24 16:45:21.000000 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-24 16:45:21.000000 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-24 16:45:21.000000 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    25918 2023-05-24 16:45:21.000000 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:45:35.015181 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-24 16:45:34.000000 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-24 16:45:34.000000 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:45:34.000000 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 16:45:34.000000 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-24 16:45:34.000000 vector_quantize_pytorch-1.5.9/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:22:23.797050 vector_quantize_pytorch-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-27 16:22:10.000000 vector_quantize_pytorch-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-27 16:22:23.797050 vector_quantize_pytorch-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-05-27 16:22:10.000000 vector_quantize_pytorch-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 16:22:23.797050 vector_quantize_pytorch-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-27 16:22:10.000000 vector_quantize_pytorch-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:22:23.797050 vector_quantize_pytorch-1.6.0/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-27 16:22:10.000000 vector_quantize_pytorch-1.6.0/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-27 16:22:10.000000 vector_quantize_pytorch-1.6.0/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-27 16:22:10.000000 vector_quantize_pytorch-1.6.0/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30022 2023-05-27 16:22:10.000000 vector_quantize_pytorch-1.6.0/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:22:23.797050 vector_quantize_pytorch-1.6.0/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-27 16:22:23.000000 vector_quantize_pytorch-1.6.0/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-27 16:22:23.000000 vector_quantize_pytorch-1.6.0/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 16:22:23.000000 vector_quantize_pytorch-1.6.0/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-27 16:22:23.000000 vector_quantize_pytorch-1.6.0/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-27 16:22:23.000000 vector_quantize_pytorch-1.6.0/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.5.9/LICENSE` & `vector_quantize_pytorch-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.9/PKG-INFO` & `vector_quantize_pytorch-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.5.9
+Version: 1.6.0
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.5.9/README.md` & `vector_quantize_pytorch-1.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -303,15 +303,15 @@
 
 ```
 
 ## Todo
 
 - [x] allow for multi-headed codebooks
 - [x] support masking
-
+- [ ] make sure affine param works in a distributed setting (batch mean and variance must be synced with dist reduce or whatever)
 
 ## Citations
 
 ```bibtex
 @misc{oord2018neural,
     title   = {Neural Discrete Representation Learning},
     author  = {Aaron van den Oord and Oriol Vinyals and Koray Kavukcuoglu},
@@ -412,7 +412,17 @@
     title   = {Bridging Discrete and Backpropagation: Straight-Through and Beyond},
     author  = {Liyuan Liu and Chengyu Dong and Xiaodong Liu and Bin Yu and Jianfeng Gao},
     journal = {ArXiv},
     year    = {2023},
     volume  = {abs/2304.08612}
 }
 ```
+
+```bibtex
+@inproceedings{huh2023improvedvqste,
+    title   = {Straightening Out the Straight-Through Estimator: Overcoming Optimization Challenges in Vector Quantized Networks},
+    author  = {Huh, Minyoung and Cheung, Brian and Agrawal, Pulkit and Isola, Phillip},
+    booktitle = {International Conference on Machine Learning},
+    year    = {2023},
+    organization = {PMLR}
+}
+```
```

#### html2text {}

```diff
@@ -133,40 +133,42 @@
 ( dim = 256, codebook_size = 1024, accept_image_fmap = True, sync_codebook =
 True # this needs to be set to True ) ).cuda(rank) ddp_mp_model = DDP(net,
 device_ids = [rank]) img_fmap = torch.randn(1, 256, 32, 32).cuda(rank)
 quantized, indices, loss = ddp_mp_model(img_fmap) cleanup() if __name__ ==
 '__main__': world_size = torch.cuda.device_count() assert world_size >= 2,
 f"requires at least 2 GPUs to run, but got {n_gpus}" mp.spawn(start, args=
 (world_size,), nprocs=world_size, join=True) ``` ## Todo - [x] allow for multi-
-headed codebooks - [x] support masking ## Citations ```bibtex @misc
-{oord2018neural, title = {Neural Discrete Representation Learning}, author =
-{Aaron van den Oord and Oriol Vinyals and Koray Kavukcuoglu}, year = {2018},
-eprint = {1711.00937}, archivePrefix = {arXiv}, primaryClass = {cs.LG} } ```
-```bibtex @misc{zeghidour2021soundstream, title = {SoundStream: An End-to-End
-Neural Audio Codec}, author = {Neil Zeghidour and Alejandro Luebs and Ahmed
-Omran and Jan Skoglund and Marco Tagliasacchi}, year = {2021}, eprint =
-{2107.03312}, archivePrefix = {arXiv}, primaryClass = {cs.SD} } ``` ```bibtex
-@inproceedings{anonymous2022vectorquantized, title = {Vector-quantized Image
-Modeling with Improved {VQGAN}}, author = {Anonymous}, booktitle = {Submitted
-to The Tenth International Conference on Learning Representations }, year =
-{2022}, url = {https://openreview.net/forum?id=pfNyExj7z2}, note = {under
-review} } ``` ```bibtex @misc{shin2021translationequivariant, title =
-{Translation-equivariant Image Quantizer for Bi-directional Image-Text
-Generation}, author = {Woncheol Shin and Gyubok Lee and Jiyoung Lee and
-Joonseok Lee and Edward Choi}, year = {2021}, eprint = {2112.00384},
-archivePrefix = {arXiv}, primaryClass = {cs.CV} } ``` ```bibtex @unknown
-{unknown, author = {Lee, Doyup and Kim, Chiheon and Kim, Saehoon and Cho, Minsu
-and Han, Wook-Shin}, year = {2022}, month = {03}, title = {Autoregressive Image
-Generation using Residual Quantization} } ``` ```bibtex @article
-{Defossez2022HighFN, title = {High Fidelity Neural Audio Compression}, author =
-{Alexandre D'efossez and Jade Copet and Gabriel Synnaeve and Yossi Adi},
-journal = {ArXiv}, year = {2022}, volume = {abs/2210.13438} } ``` ```bibtex
-@inproceedings{Chiu2022SelfsupervisedLW, title = {Self-supervised Learning with
-Random-projection Quantizer for Speech Recognition}, author = {Chung-Cheng Chiu
-and James Qin and Yu Zhang and Jiahui Yu and Yonghui Wu}, booktitle =
+headed codebooks - [x] support masking - [ ] make sure affine param works in a
+distributed setting (batch mean and variance must be synced with dist reduce or
+whatever) ## Citations ```bibtex @misc{oord2018neural, title = {Neural Discrete
+Representation Learning}, author = {Aaron van den Oord and Oriol Vinyals and
+Koray Kavukcuoglu}, year = {2018}, eprint = {1711.00937}, archivePrefix =
+{arXiv}, primaryClass = {cs.LG} } ``` ```bibtex @misc{zeghidour2021soundstream,
+title = {SoundStream: An End-to-End Neural Audio Codec}, author = {Neil
+Zeghidour and Alejandro Luebs and Ahmed Omran and Jan Skoglund and Marco
+Tagliasacchi}, year = {2021}, eprint = {2107.03312}, archivePrefix = {arXiv},
+primaryClass = {cs.SD} } ``` ```bibtex @inproceedings
+{anonymous2022vectorquantized, title = {Vector-quantized Image Modeling with
+Improved {VQGAN}}, author = {Anonymous}, booktitle = {Submitted to The Tenth
+International Conference on Learning Representations }, year = {2022}, url =
+{https://openreview.net/forum?id=pfNyExj7z2}, note = {under review} } ```
+```bibtex @misc{shin2021translationequivariant, title = {Translation-
+equivariant Image Quantizer for Bi-directional Image-Text Generation}, author =
+{Woncheol Shin and Gyubok Lee and Jiyoung Lee and Joonseok Lee and Edward
+Choi}, year = {2021}, eprint = {2112.00384}, archivePrefix = {arXiv},
+primaryClass = {cs.CV} } ``` ```bibtex @unknown{unknown, author = {Lee, Doyup
+and Kim, Chiheon and Kim, Saehoon and Cho, Minsu and Han, Wook-Shin}, year =
+{2022}, month = {03}, title = {Autoregressive Image Generation using Residual
+Quantization} } ``` ```bibtex @article{Defossez2022HighFN, title = {High
+Fidelity Neural Audio Compression}, author = {Alexandre D'efossez and Jade
+Copet and Gabriel Synnaeve and Yossi Adi}, journal = {ArXiv}, year = {2022},
+volume = {abs/2210.13438} } ``` ```bibtex @inproceedings
+{Chiu2022SelfsupervisedLW, title = {Self-supervised Learning with Random-
+projection Quantizer for Speech Recognition}, author = {Chung-Cheng Chiu and
+James Qin and Yu Zhang and Jiahui Yu and Yonghui Wu}, booktitle =
 {International Conference on Machine Learning}, year = {2022} } ``` ```bibtex
 @inproceedings{Zhang2023GoogleUS, title = {Google USM: Scaling Automatic Speech
 Recognition Beyond 100 Languages}, author = {Yu Zhang and Wei Han and James Qin
 and Yongqiang Wang and Ankur Bapna and Zhehuai Chen and Nanxin Chen and Bo Li
 and Vera Axelrod and Gary Wang and Zhong Meng and Ke Hu and Andrew Rosenberg
 and Rohit Prabhavalkar and Daniel S. Park and Parisa Haghani and Jason Riesa
 and Ginger Perng and Hagen Soltau and Trevor Strohman and Bhuvana Ramabhadran
@@ -179,8 +181,12 @@
 {2023} } ``` ```bibtex @inproceedings{Yang2023HiFiCodecGV, title = {HiFi-Codec:
 Group-residual Vector quantization for High Fidelity Audio Codec}, author =
 {Dongchao Yang and Songxiang Liu and Rongjie Huang and Jinchuan Tian and Chao
 Weng and Yuexian Zou}, year = {2023} } ``` ```bibtex @article
 {Liu2023BridgingDA, title = {Bridging Discrete and Backpropagation: Straight-
 Through and Beyond}, author = {Liyuan Liu and Chengyu Dong and Xiaodong Liu and
 Bin Yu and Jianfeng Gao}, journal = {ArXiv}, year = {2023}, volume = {abs/
-2304.08612} } ```
+2304.08612} } ``` ```bibtex @inproceedings{huh2023improvedvqste, title =
+{Straightening Out the Straight-Through Estimator: Overcoming Optimization
+Challenges in Vector Quantized Networks}, author = {Huh, Minyoung and Cheung,
+Brian and Agrawal, Pulkit and Isola, Phillip}, booktitle = {International
+Conference on Machine Learning}, year = {2023}, organization = {PMLR} } ```
```

### Comparing `vector_quantize_pytorch-1.5.9/setup.py` & `vector_quantize_pytorch-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.5.9',
+  version = '1.6.0',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.5.9/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.6.0/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.9/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.6.0/vector_quantize_pytorch/residual_vq.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         assert heads == 1, 'residual vq is not compatible with multi-headed codes'
 
         self.num_quantizers = num_quantizers
 
         self.accept_image_fmap = accept_image_fmap
         self.layers = nn.ModuleList([VectorQuantize(accept_image_fmap = accept_image_fmap, **kwargs) for _ in range(num_quantizers)])
 
-        self.quantize_dropout = quantize_dropout
+        self.quantize_dropout = quantize_dropout and num_quantizers > 1
 
         assert quantize_dropout_cutoff_index >= 0
 
         self.quantize_dropout_cutoff_index = quantize_dropout_cutoff_index
         self.quantize_dropout_multiple_of = quantize_dropout_multiple_of  # encodec paper proposes structured dropout, believe this was set to 4
 
         if not shared_codebook:
@@ -105,15 +105,16 @@
 
         return all_codes
 
     def forward(
         self,
         x,
         indices = None,
-        return_all_codes = False
+        return_all_codes = False,
+        sample_codebook_temp = None
     ):
         num_quant, quant_dropout_multiple_of, return_loss, device = self.num_quantizers, self.quantize_dropout_multiple_of, exists(indices), x.device
 
         assert not (self.accept_image_fmap and exists(indices))
 
         quantized_out = 0.
         residual = x
@@ -149,15 +150,15 @@
                 all_losses.append(null_loss)
                 continue
 
             layer_indices = None
             if return_loss:
                 layer_indices = indices[..., quantizer_index]
 
-            quantized, *rest = layer(residual, indices = layer_indices)
+            quantized, *rest = layer(residual, indices = layer_indices, sample_codebook_temp = sample_codebook_temp)
 
             residual = residual - quantized.detach()
             quantized_out = quantized_out + quantized
 
             if return_loss:
                 ce_loss = rest[0]
                 ce_losses.append(ce_loss)
@@ -224,29 +225,33 @@
         codes = tuple(rvq.get_codes_from_indices(chunk_indices) for rvq, chunk_indices in zip(self.rvqs, indices))
         return torch.stack(codes)
 
     def forward(
         self,
         x,
         indices = None,
-        return_all_codes = False
+        return_all_codes = False,
+        sample_codebook_temp = None
     ):
         shape = x.shape
         split_dim = 1 if self.accept_image_fmap else -1
         assert shape[split_dim] == self.dim
 
         # split the feature dimension into groups
 
         x = x.chunk(self.groups, dim = split_dim)
 
         indices = default(indices, tuple())
         return_ce_loss = len(indices) > 0
         assert len(indices) == 0 or len(indices) == self.groups
 
-        forward_kwargs = dict(return_all_codes = return_all_codes)
+        forward_kwargs = dict(
+            return_all_codes = return_all_codes,
+            sample_codebook_temp = sample_codebook_temp
+        )
 
         # invoke residual vq on each group
 
         out = tuple(rvq(chunk, indices = chunk_indices, **forward_kwargs) for rvq, chunk, chunk_indices in zip_longest(self.rvqs, x, indices))
         out = tuple(zip(*out))
 
         # if returning cross entropy loss to rvq codebooks
```

### Comparing `vector_quantize_pytorch-1.5.9/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.6.0/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import torch
 from torch import nn, einsum
 import torch.nn.functional as F
 import torch.distributed as distributed
 from torch.cuda.amp import autocast
 
-from einops import rearrange, repeat, pack, unpack
+from einops import rearrange, repeat, reduce, pack, unpack
 from contextlib import contextmanager
 
 def exists(val):
     return val is not None
 
 def default(val, d):
     return val if exists(val) else d
@@ -44,43 +44,48 @@
 
 def gumbel_sample(
     logits,
     temperature = 1.,
     stochastic = False,
     straight_through = False,
     reinmax = False,
-    dim = -1
+    dim = -1,
+    training = True
 ):
     dtype, size = logits.dtype, logits.shape[dim]
 
-    if stochastic:
-        logits = logits + gumbel_noise(logits)
+    if training and stochastic and temperature > 0:
+        sampling_logits = (logits / temperature) + gumbel_noise(logits)
+    else:
+        sampling_logits = logits
 
-    ind = logits.argmax(dim = dim)
+    ind = sampling_logits.argmax(dim = dim)
     one_hot = F.one_hot(ind, size).type(dtype)
 
     assert not (reinmax and not straight_through), 'reinmax can only be turned on if using straight through gumbel softmax'
 
-    if not straight_through:
-        return ind, one_hot
+    if not straight_through or temperature <= 0. or not training:
+        return ind, one_hot, None
 
     # use reinmax for better second-order accuracy - https://arxiv.org/abs/2304.08612
     # algorithm 2
 
     if reinmax:
         π0 = logits.softmax(dim = dim)
         π1 = (one_hot + (logits / temperature).softmax(dim = dim)) / 2
-        π1 = ((π1.log() - logits).detach() + logits).softmax(dim = 1)
+        π1 = ((log(π1) - logits).detach() + logits).softmax(dim = 1)
         π2 = 2 * π1 - 0.5 * π0
         one_hot = π2 - π2.detach() + one_hot
     else:
         π1 = (logits / temperature).softmax(dim = dim)
         one_hot = one_hot + π1 - π1.detach()
 
-    return ind, one_hot
+    st_mult = one_hot.gather(-1, rearrange(ind, '... -> ... 1')) # multiplier for straight-through
+
+    return ind, one_hot, st_mult
 
 def laplace_smoothing(x, n_categories, eps = 1e-5, dim = -1):
     denom = x.sum(dim = dim, keepdim = True)
     return (x + eps) / (denom + n_categories * eps)
 
 def sample_vectors(samples, num):
     num_samples, device = samples.shape[0], samples.device
@@ -228,35 +233,41 @@
         sync_kmeans = True,
         decay = 0.8,
         eps = 1e-5,
         threshold_ema_dead_code = 2,
         reset_cluster_size = None,
         use_ddp = False,
         learnable_codebook = False,
-        sample_codebook_temp = 0,
-        straight_through = False,
-        gumbel_sample = gumbel_sample
+        gumbel_sample = gumbel_sample,
+        sample_codebook_temp = 1.,
+        ema_update = True,
+        affine_param = False,
+        affine_param_batch_decay = 0.99,
+        affine_param_codebook_decay = 0.9
     ):
         super().__init__()
         self.transform_input = identity
 
         self.decay = decay
+        self.ema_update = ema_update
+
         init_fn = uniform_init if not kmeans_init else torch.zeros
         embed = init_fn(num_codebooks, codebook_size, dim)
 
         self.codebook_size = codebook_size
         self.num_codebooks = num_codebooks
 
         self.kmeans_iters = kmeans_iters
         self.eps = eps
         self.threshold_ema_dead_code = threshold_ema_dead_code
         self.reset_cluster_size = default(reset_cluster_size, threshold_ema_dead_code)
 
         assert callable(gumbel_sample)
         self.gumbel_sample = gumbel_sample
+        self.sample_codebook_temp = sample_codebook_temp
 
         assert not (use_ddp and num_codebooks > 1 and kmeans_init), 'kmeans init is not compatible with multiple codebooks in distributed environment for now'
 
         self.sample_fn = sample_vectors_distributed if use_ddp and sync_kmeans else batched_sample_vectors
         self.kmeans_all_reduce_fn = distributed.all_reduce if use_ddp and sync_kmeans else noop
         self.all_reduce_fn = distributed.all_reduce if use_ddp else noop
 
@@ -266,14 +277,30 @@
 
         self.learnable_codebook = learnable_codebook
         if learnable_codebook:
             self.embed = nn.Parameter(embed)
         else:
             self.register_buffer('embed', embed)
 
+        # affine related params
+
+        self.affine_param = affine_param
+
+        if not affine_param:
+            return
+
+        self.affine_param_batch_decay = affine_param_batch_decay
+        self.affine_param_codebook_decay = affine_param_codebook_decay
+
+        self.register_buffer('batch_mean', None)
+        self.register_buffer('batch_variance', None)
+
+        self.register_buffer('codebook_mean', None)
+        self.register_buffer('codebook_variance', None)
+
     @torch.jit.ignore
     def init_embed_(self, data):
         if self.initted:
             return
 
         embed, cluster_size = kmeans(
             data,
@@ -284,14 +311,37 @@
         )
 
         self.embed.data.copy_(embed)
         self.embed_avg.data.copy_(embed.clone())
         self.cluster_size.data.copy_(cluster_size)
         self.initted.data.copy_(torch.Tensor([True]))
 
+    @torch.jit.ignore
+    def update_with_decay(self, buffer_name, new_value, decay):
+        old_value = getattr(self, buffer_name)
+
+        if not exists(old_value):
+            self.register_buffer(buffer_name, new_value)
+            return
+
+        value = old_value * decay + new_value * (1 - decay)
+        self.register_buffer(buffer_name, value)
+
+    @torch.jit.ignore
+    def update_affine(self, data, embed):
+        assert self.affine_param
+
+        var_fn = partial(torch.var, unbiased = False)
+
+        self.update_with_decay('batch_mean', reduce(data, '... d -> d', 'mean'), self.affine_param_batch_decay)
+        self.update_with_decay('batch_variance', reduce(data, '... d -> d', var_fn), self.affine_param_batch_decay)
+
+        self.update_with_decay('codebook_mean', reduce(embed, '... d -> d', 'mean'), self.affine_param_codebook_decay)
+        self.update_with_decay('codebook_variance', reduce(embed, '... d -> d', var_fn), self.affine_param_codebook_decay)
+
     def replace(self, batch_samples, batch_mask):
         for ind, (samples, mask) in enumerate(zip(batch_samples.unbind(dim = 0), batch_mask.unbind(dim = 0))):
             if not torch.any(mask):
                 continue
 
             sampled = self.sample_fn(rearrange(samples, '... -> 1 ...'), mask.sum().item())
             sampled = rearrange(sampled, '1 ... -> ...')
@@ -310,37 +360,59 @@
         if not torch.any(expired_codes):
             return
 
         batch_samples = rearrange(batch_samples, 'h ... d -> h (...) d')
         self.replace(batch_samples, batch_mask = expired_codes)
 
     @autocast(enabled = False)
-    def forward(self, x):
+    def forward(
+        self,
+        x,
+        sample_codebook_temp = None
+    ):
         needs_codebook_dim = x.ndim < 4
+        sample_codebook_temp = default(sample_codebook_temp, self.sample_codebook_temp)
 
         x = x.float()
 
         if needs_codebook_dim:
             x = rearrange(x, '... -> 1 ...')
 
         dtype = x.dtype
         flatten, ps = pack_one(x, 'h * d')
 
         self.init_embed_(flatten)
 
+        if self.affine_param:
+            self.update_affine(flatten, self.embed)
+
         embed = self.embed if not self.learnable_codebook else self.embed.detach()
 
+        if self.affine_param:
+            codebook_std = self.codebook_variance.clamp(min = 1e-5).sqrt()
+            batch_std = self.batch_variance.clamp(min = 1e-5).sqrt()
+            embed = (embed - self.codebook_mean) * (batch_std / codebook_std) + self.batch_mean
+
         dist = -torch.cdist(flatten, embed, p = 2)
 
-        embed_ind, embed_onehot = self.gumbel_sample(dist, dim = -1)
+        embed_ind, embed_onehot, straight_through_mult = self.gumbel_sample(dist, dim = -1, temperature = sample_codebook_temp, training = self.training)
+
         embed_ind = unpack_one(embed_ind, ps, 'h *')
 
         quantize = batched_embedding(embed_ind, self.embed)
 
-        if self.training:
+        if exists(straight_through_mult):
+            mult = unpack_one(straight_through_mult, ps, 'h * d')
+            quantize = quantize * mult
+
+        if self.training and self.ema_update:
+
+            if self.affine_param:
+                flatten = (flatten - self.batch_mean) * (codebook_std / batch_std) + self.codebook_mean
+
             cluster_size = embed_onehot.sum(dim = 1)
 
             self.all_reduce_fn(cluster_size)
             self.cluster_size.data.lerp_(cluster_size, 1 - self.decay)
 
             embed_sum = einsum('h n d, h n c -> h c d', flatten, embed_onehot)
             self.all_reduce_fn(embed_sum.contiguous())
@@ -370,19 +442,22 @@
         sync_kmeans = True,
         decay = 0.8,
         eps = 1e-5,
         threshold_ema_dead_code = 2,
         reset_cluster_size = None,
         use_ddp = False,
         learnable_codebook = False,
-        gumbel_sample = gumbel_sample
+        gumbel_sample = gumbel_sample,
+        sample_codebook_temp = 1.,
+        ema_update = True
     ):
         super().__init__()
         self.transform_input = l2norm
 
+        self.ema_update = ema_update
         self.decay = decay
 
         if not kmeans_init:
             embed = l2norm(uniform_init(num_codebooks, codebook_size, dim))
         else:
             embed = torch.zeros(num_codebooks, codebook_size, dim)
 
@@ -392,14 +467,15 @@
         self.kmeans_iters = kmeans_iters
         self.eps = eps
         self.threshold_ema_dead_code = threshold_ema_dead_code
         self.reset_cluster_size = default(reset_cluster_size, threshold_ema_dead_code)
 
         assert callable(gumbel_sample)
         self.gumbel_sample = gumbel_sample
+        self.sample_codebook_temp = sample_codebook_temp
 
         self.sample_fn = sample_vectors_distributed if use_ddp and sync_kmeans else batched_sample_vectors
         self.kmeans_all_reduce_fn = distributed.all_reduce if use_ddp and sync_kmeans else noop
         self.all_reduce_fn = distributed.all_reduce if use_ddp else noop
 
         self.register_buffer('initted', torch.Tensor([not kmeans_init]))
         self.register_buffer('cluster_size', torch.zeros(num_codebooks, codebook_size))
@@ -453,16 +529,21 @@
         if not torch.any(expired_codes):
             return
 
         batch_samples = rearrange(batch_samples, 'h ... d -> h (...) d')
         self.replace(batch_samples, batch_mask = expired_codes)
 
     @autocast(enabled = False)
-    def forward(self, x):
+    def forward(
+        self,
+        x,
+        sample_codebook_temp = None
+    ):
         needs_codebook_dim = x.ndim < 4
+        sample_codebook_temp = default(sample_codebook_temp, self.sample_codebook_temp)
 
         x = x.float()
 
         if needs_codebook_dim:
             x = rearrange(x, '... -> 1 ...')
 
         dtype = x.dtype
@@ -470,20 +551,25 @@
         flatten, ps = pack_one(x, 'h * d')
 
         self.init_embed_(flatten)
 
         embed = self.embed if not self.learnable_codebook else self.embed.detach()
 
         dist = einsum('h n d, h c d -> h n c', flatten, embed)
-        embed_ind, embed_onehot = self.gumbel_sample(dist, dim = -1)
+
+        embed_ind, embed_onehot, straight_through_mult = self.gumbel_sample(dist, dim = -1, temperature = sample_codebook_temp, training = self.training)
         embed_ind = unpack_one(embed_ind, ps, 'h *')
 
         quantize = batched_embedding(embed_ind, self.embed)
 
-        if self.training:
+        if exists(straight_through_mult):
+            mult = unpack_one(straight_through_mult, ps, 'h * d')
+            quantize = quantize * mult
+
+        if self.training and self.ema_update:
             bins = embed_onehot.sum(dim = 1)
             self.all_reduce_fn(bins)
 
             self.cluster_size.data.lerp_(bins, 1 - self.decay)
 
             embed_sum = einsum('h n d, h n c -> h c d', flatten, embed_onehot)
             self.all_reduce_fn(embed_sum)
@@ -524,18 +610,23 @@
         accept_image_fmap = False,
         commitment_weight = 1.,
         commitment_use_cross_entropy_loss = False,
         orthogonal_reg_weight = 0.,
         orthogonal_reg_active_codes_only = False,
         orthogonal_reg_max_codes = None,
         stochastic_sample_codes = False,
-        sample_codebook_temp = 0.,
+        sample_codebook_temp = 1.,
         straight_through = False,
         reinmax = False,  # using reinmax for improved straight-through, assuming straight through helps at all
         sync_codebook = False,
+        ema_update = True,
+        learnable_codebook = False,
+        affine_param = False,
+        affine_param_batch_decay = 0.99,
+        affine_param_codebook_decay = 0.9
     ):
         super().__init__()
         self.dim = dim
         self.heads = heads
         self.separate_codebook_per_head = separate_codebook_per_head
 
         codebook_dim = default(codebook_dim, dim)
@@ -555,34 +646,46 @@
         self.orthogonal_reg_max_codes = orthogonal_reg_max_codes
 
         codebook_class = EuclideanCodebook if not use_cosine_sim else CosineSimCodebook
 
         gumbel_sample_fn = partial(
             gumbel_sample,
             stochastic = stochastic_sample_codes,
-            temperature = sample_codebook_temp,
             reinmax = reinmax,
             straight_through = straight_through
         )
 
-        self._codebook = codebook_class(
+        codebook_kwargs = dict(
             dim = codebook_dim,
             num_codebooks = heads if separate_codebook_per_head else 1,
             codebook_size = codebook_size,
             kmeans_init = kmeans_init,
             kmeans_iters = kmeans_iters,
             sync_kmeans = sync_kmeans,
             decay = decay,
             eps = eps,
             threshold_ema_dead_code = threshold_ema_dead_code,
             use_ddp = sync_codebook,
-            learnable_codebook = has_codebook_orthogonal_loss,
-            gumbel_sample = gumbel_sample_fn
+            learnable_codebook = has_codebook_orthogonal_loss or learnable_codebook,
+            sample_codebook_temp = sample_codebook_temp,
+            gumbel_sample = gumbel_sample_fn,
+            ema_update = ema_update
         )
 
+        if affine_param:
+            assert not use_cosine_sim
+            codebook_kwargs = dict(
+                **codebook_kwargs,
+                affine_param = True,
+                affine_param_batch_decay = affine_param_batch_decay,
+                affine_param_codebook_decay = affine_param_codebook_decay
+            )
+
+        self._codebook = codebook_class(**codebook_kwargs)
+
         self.codebook_size = codebook_size
 
         self.accept_image_fmap = accept_image_fmap
         self.channel_last = channel_last
 
     @property
     def codebook(self):
@@ -611,15 +714,16 @@
         codes = unpack_one(codes, ps, 'b * d')
         return codes
 
     def forward(
         self,
         x,
         indices = None,
-        mask = None
+        mask = None,
+        sample_codebook_temp = None
     ):
         only_one = x.ndim == 2
 
         if only_one:
             x = rearrange(x, 'b d -> b 1 d')
 
         shape, device, heads, is_multiheaded, codebook_size, return_loss = x.shape, x.device, self.heads, self.heads > 1, self.codebook_size, exists(indices)
@@ -635,27 +739,27 @@
         if need_transpose:
             x = rearrange(x, 'b d n -> b n d')
 
         # project input
 
         x = self.project_in(x)
 
-        # l2norm for cosine sim, otherwise identity
-
-        x = self._codebook.transform_input(x)
-
         # handle multi-headed separate codebooks
 
         if is_multiheaded:
             ein_rhs_eq = 'h b n d' if self.separate_codebook_per_head else '1 (b h) n d'
             x = rearrange(x, f'b n (h d) -> {ein_rhs_eq}', h = heads)
 
+        # l2norm for cosine sim, otherwise identity
+
+        x = self._codebook.transform_input(x)
+
         # quantize
 
-        quantize, embed_ind, distances = self._codebook(x)
+        quantize, embed_ind, distances = self._codebook(x, sample_codebook_temp = sample_codebook_temp)
 
         if self.training:
             quantize = x + (quantize - x).detach()
 
         # function for calculating cross entropy loss to distance matrix
         # used for (1) naturalspeech2 training residual vq latents to be close to the correct codes and (2) cross-entropy based commitment loss
```

### Comparing `vector_quantize_pytorch-1.5.9/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.6.0/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.5.9
+Version: 1.6.0
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

