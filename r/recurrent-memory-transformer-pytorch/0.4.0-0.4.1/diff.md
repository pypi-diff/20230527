# Comparing `tmp/recurrent-memory-transformer-pytorch-0.4.0.tar.gz` & `tmp/recurrent-memory-transformer-pytorch-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurrent-memory-transformer-pytorch-0.4.0.tar", last modified: Thu May 25 22:35:36 2023, max compression
+gzip compressed data, was "recurrent-memory-transformer-pytorch-0.4.1.tar", last modified: Sat May 27 01:18:31 2023, max compression
```

## Comparing `recurrent-memory-transformer-pytorch-0.4.0.tar` & `recurrent-memory-transformer-pytorch-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:35:36.486204 recurrent-memory-transformer-pytorch-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-25 22:35:24.000000 recurrent-memory-transformer-pytorch-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-25 22:35:36.486204 recurrent-memory-transformer-pytorch-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-05-25 22:35:24.000000 recurrent-memory-transformer-pytorch-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:35:36.486204 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-25 22:35:24.000000 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-25 22:35:24.000000 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-05-25 22:35:24.000000 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:35:36.486204 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-25 22:35:36.000000 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-25 22:35:36.000000 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 22:35:36.000000 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 22:35:36.000000 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 22:35:36.000000 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 22:35:36.486204 recurrent-memory-transformer-pytorch-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-25 22:35:24.000000 recurrent-memory-transformer-pytorch-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:31.592264 recurrent-memory-transformer-pytorch-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-27 01:18:18.000000 recurrent-memory-transformer-pytorch-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-27 01:18:31.592264 recurrent-memory-transformer-pytorch-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-05-27 01:18:18.000000 recurrent-memory-transformer-pytorch-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:31.592264 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-27 01:18:18.000000 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-27 01:18:18.000000 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-05-27 01:18:18.000000 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:31.592264 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-27 01:18:31.000000 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-27 01:18:31.000000 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 01:18:31.000000 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-27 01:18:31.000000 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-27 01:18:31.000000 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 01:18:31.592264 recurrent-memory-transformer-pytorch-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-27 01:18:18.000000 recurrent-memory-transformer-pytorch-0.4.1/setup.py
```

### Comparing `recurrent-memory-transformer-pytorch-0.4.0/LICENSE` & `recurrent-memory-transformer-pytorch-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.4.0/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.4.0
+Version: 0.4.1
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.4.0/README.md` & `recurrent-memory-transformer-pytorch-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch/attend.py` & `recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py` & `recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -206,21 +206,25 @@
         rotary_pos_emb = False,
         token_shift = True,
         use_xl_memories = True,
         xl_mem_len = None,
         enhanced_xl_recurrence = False,     # add simple method for enhancing receptive field of xl memories, from ernie-doc paper
         emb_gradient_frac = 0.1,            # trick from cogview paper that leads to a bit more stability
         memory_not_causal = True,           # flash attention behaves a bit more optimally if causal mask is not explicitly passed in - but if the memories perform better without a causal mask, it is necessary to have this turned on
+        resi_dual_scale = 1.,               # in the case of overflows in fp16 on the prenorm branch, set this to a value less than 1.
     ):
         super().__init__()
         self.causal = causal
         self.seq_len = seq_len
 
         self.emb_gradient_frac = emb_gradient_frac
 
+        assert 0 < resi_dual_scale <= 1., 'resiDual scale must be between 0 and 1'
+        self.resi_dual_scale = resi_dual_scale
+
         assert num_memory_tokens > 0
 
         self.token_emb = nn.Embedding(num_tokens, dim)
 
         # positions
 
         assert any([abs_pos_emb, rotary_pos_emb, token_shift])
@@ -380,29 +384,29 @@
         new_xl_memories = []
 
         if has_xl_memories and self.enhanced_xl_recurrence and len(xl_memories) > 1:  # simply shift all the xl memories down by one, so lower layer gets access to representations from layer above
             xl_memories = [*xl_memories[1:], xl_memories[0]]
 
         # attention and feedforward
 
-        residual = x
+        residual = x * self.resi_dual_scale
 
         for attn, attn_post_norm, ff, ff_post_norm in self.layers:
             attn_out, xl_memories = attn(shift_fn(x), mask = mask, xl_memories = next(xl_memories_iter, None), rotary_emb = rotary_emb)
             new_xl_memories.append(xl_memories)
 
             x = attn_post_norm(x + attn_out)
 
-            residual = residual + attn_out
+            residual = residual + attn_out * self.resi_dual_scale
 
             ff_out = ff(shift_fn(x))
 
             x = ff_post_norm(x + ff_out)
 
-            residual = residual + ff_out
+            residual = residual + ff_out * self.resi_dual_scale
 
         # whether to return xl memories
 
         next_xl_memories = None
 
         if self.use_xl_memories:
             next_xl_memories = list(map(lambda t: torch.detach(t[..., -self.xl_mem_len:, :]), new_xl_memories))
```

### Comparing `recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.4.0
+Version: 0.4.1
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.4.0/setup.py` & `recurrent-memory-transformer-pytorch-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'recurrent-memory-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.4.0',
+  version = '0.4.1',
   license='MIT',
   description = 'Recurrent Memory Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/recurrent-memory-transformer-pytorch',
   keywords = [
```

