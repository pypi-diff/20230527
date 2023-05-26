# Comparing `tmp/ditty-0.2.3.tar.gz` & `tmp/ditty-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ditty-0.2.3.tar", last modified: Thu May 25 03:32:43 2023, max compression
+gzip compressed data, was "ditty-0.3.0.tar", last modified: Fri May 26 21:59:47 2023, max compression
```

## Comparing `ditty-0.2.3.tar` & `ditty-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-25 03:32:43.948102 ditty-0.2.3/
--rw-rw-r--   0 crow      (1000) crow      (1000)    11357 2023-05-20 22:13:26.000000 ditty-0.2.3/LICENSE
--rw-rw-r--   0 crow      (1000) crow      (1000)     3170 2023-05-25 03:32:43.948102 ditty-0.2.3/PKG-INFO
--rw-rw-r--   0 crow      (1000) crow      (1000)     2872 2023-05-23 04:03:46.000000 ditty-0.2.3/README.md
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-25 03:32:43.948102 ditty-0.2.3/lib/
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-25 03:32:43.948102 ditty-0.2.3/lib/ditty/
--rw-rw-r--   0 crow      (1000) crow      (1000)        0 2023-05-21 15:10:10.000000 ditty-0.2.3/lib/ditty/__init__.py
--rw-rw-r--   0 crow      (1000) crow      (1000)     5164 2023-05-23 17:35:55.000000 ditty-0.2.3/lib/ditty/data.py
--rw-rw-r--   0 crow      (1000) crow      (1000)     5670 2023-05-25 02:45:06.000000 ditty-0.2.3/lib/ditty/pipeline.py
--rw-rw-r--   0 crow      (1000) crow      (1000)     6168 2023-05-25 00:24:18.000000 ditty-0.2.3/lib/ditty/trainer.py
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-25 03:32:43.948102 ditty-0.2.3/lib/ditty.egg-info/
--rw-rw-r--   0 crow      (1000) crow      (1000)     3170 2023-05-25 03:32:43.000000 ditty-0.2.3/lib/ditty.egg-info/PKG-INFO
--rw-rw-r--   0 crow      (1000) crow      (1000)      283 2023-05-25 03:32:43.000000 ditty-0.2.3/lib/ditty.egg-info/SOURCES.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)        1 2023-05-25 03:32:43.000000 ditty-0.2.3/lib/ditty.egg-info/dependency_links.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)       56 2023-05-25 03:32:43.000000 ditty-0.2.3/lib/ditty.egg-info/requires.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)        6 2023-05-25 03:32:43.000000 ditty-0.2.3/lib/ditty.egg-info/top_level.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)      103 2023-05-25 03:32:43.948102 ditty-0.2.3/setup.cfg
--rw-rw-r--   0 crow      (1000) crow      (1000)      639 2023-05-25 03:32:10.000000 ditty-0.2.3/setup.py
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-26 21:59:47.635318 ditty-0.3.0/
+-rw-rw-r--   0 crow      (1000) crow      (1000)    11357 2023-05-20 22:13:26.000000 ditty-0.3.0/LICENSE
+-rw-rw-r--   0 crow      (1000) crow      (1000)     3170 2023-05-26 21:59:47.635318 ditty-0.3.0/PKG-INFO
+-rw-rw-r--   0 crow      (1000) crow      (1000)     2872 2023-05-23 04:03:46.000000 ditty-0.3.0/README.md
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-26 21:59:47.635318 ditty-0.3.0/lib/
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-26 21:59:47.635318 ditty-0.3.0/lib/ditty/
+-rw-rw-r--   0 crow      (1000) crow      (1000)        0 2023-05-21 15:10:10.000000 ditty-0.3.0/lib/ditty/__init__.py
+-rw-rw-r--   0 crow      (1000) crow      (1000)     5251 2023-05-26 05:12:23.000000 ditty-0.3.0/lib/ditty/data.py
+-rw-rw-r--   0 crow      (1000) crow      (1000)     7238 2023-05-26 06:50:37.000000 ditty-0.3.0/lib/ditty/pipeline.py
+-rw-rw-r--   0 crow      (1000) crow      (1000)     6597 2023-05-26 21:56:46.000000 ditty-0.3.0/lib/ditty/trainer.py
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-26 21:59:47.635318 ditty-0.3.0/lib/ditty.egg-info/
+-rw-rw-r--   0 crow      (1000) crow      (1000)     3170 2023-05-26 21:59:47.000000 ditty-0.3.0/lib/ditty.egg-info/PKG-INFO
+-rw-rw-r--   0 crow      (1000) crow      (1000)      283 2023-05-26 21:59:47.000000 ditty-0.3.0/lib/ditty.egg-info/SOURCES.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)        1 2023-05-26 21:59:47.000000 ditty-0.3.0/lib/ditty.egg-info/dependency_links.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)       56 2023-05-26 21:59:47.000000 ditty-0.3.0/lib/ditty.egg-info/requires.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)        6 2023-05-26 21:59:47.000000 ditty-0.3.0/lib/ditty.egg-info/top_level.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)      103 2023-05-26 21:59:47.635318 ditty-0.3.0/setup.cfg
+-rw-rw-r--   0 crow      (1000) crow      (1000)      639 2023-05-26 21:58:03.000000 ditty-0.3.0/setup.py
```

### Comparing `ditty-0.2.3/LICENSE` & `ditty-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ditty-0.2.3/PKG-INFO` & `ditty-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ditty
-Version: 0.2.3
+Version: 0.3.0
 Home-page: https://github.com/iantbutler01/ditty
 Author: Ian T Butler (KinglyCrow)
 Author-email: iantbutler01@gmail.com
 License: Apache V2
 Keywords: finetuning,llm,nlp,machine learning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ditty-0.2.3/README.md` & `ditty-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ditty-0.2.3/lib/ditty/data.py` & `ditty-0.3.0/lib/ditty/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         if self.seed:
             generator.manual_seed(self.seed)
 
         # Build the sampler.
         if self.group_by_length:
             lengths = (
                 self.dataset[self.length_column_name]
-                if self.args.length_column_name in self.dataset.column_names
+                if self.length_column_name in self.dataset.column_names
                 else None
             )
             model_input_name = self.tokenizer.model_input_names[0]
             return LengthGroupedSampler(
                 self.batch_size * self.grad_accum,
                 dataset=self.dataset,
                 lengths=lengths,
@@ -95,15 +95,19 @@
 
     def prepare(self, pipeline: list[(str, Callable, dict)]):
         if self.dataset is None:
             raise ValueError("Dataset not set.")
 
         for op_name, func, kwargs in pipeline:
             op = getattr(self.dataset, op_name)
-            self.dataset = op(func, **kwargs)
+
+            if not func:
+                self.dataset = op(**kwargs)
+            else:
+                self.dataset = op(func, **kwargs)
 
         return self._get_dataloader()        
 
     def _seed_worker(self):
         if not self.seed:
             worker_seed = torch.initial_seed() % 2**32
         else:
```

### Comparing `ditty-0.2.3/lib/ditty/pipeline.py` & `ditty-0.3.0/lib/ditty/pipeline.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,57 +14,82 @@
 from torch.utils.data import DataLoader
 from .trainer import Trainer
 from .data import Data
 import logging
 
 logging.basicConfig(level=logging.INFO)
 
-class Pipeline():
+
+class Pipeline:
     def __init__(
         self,
         output_dir="./output",
         dataset_name="code_search_net",
         dataset_language="python",
         model_name_or_path="theblackcat102/pythia-3b-deduped-sft-r1",
         hf_hub_token=None,
         hf_hub_model_id=None,
         fp16=True,
         l8bit=True,
+        l4bit=False,
         seed=None,
         batch_size=4,
         grad_accum=4,
         push_to_hub=True,
         fp32_cpu_offload=False,
         load_checkpoint=True,
         checkpoint_every=1000,
+        gradient_checkpointing=True,
+        experimental=False,
+        block_size=2048,
+        use_bfloat16=False,
     ):
         self.output_dir = output_dir
         self.dataset_name = dataset_name
         self.dataset_language = dataset_language
         self.model_name_or_path = model_name_or_path
         self.hf_hub_token = hf_hub_token
         self.hf_hub_model_id = hf_hub_model_id
         self.fp16 = fp16
         self.seed = seed
         self.epochs = 1
         self.max_steps = None
         self.l8bit = l8bit
+        self.l4bit = l4bit
         self.push_to_hub = push_to_hub
         self.batch_size = batch_size
         self.grad_accum = grad_accum
-        self.block_size = 2048
+        self.block_size = block_size
         self.fp32_cpu_offload = fp32_cpu_offload
-        self.bb_conf = BitsAndBytesConfig(load_in_8bit=l8bit, llm_int8_enable_fp32_cpu_offload=fp32_cpu_offload)
+        self.use_bfloat16 = use_bfloat16
+
+        if self.l8bit and self.l4bit:
+            raise ValueError("Cannot set both l8bit and l4bit to True.")
+
+        if self.l4bit and experimental:
+            self.bnb_config = BitsAndBytesConfig(
+                load_in_4bit=True,
+                bnb_4bit_use_double_quant=True,
+                bnb_4bit_quant_type="nf4",
+                bnb_4bit_compute_dtype=torch.bfloat16,
+            )
+        elif self.l4bit and not experimental:
+            raise ValueError("To use 4bit, `experimental` must be set to True.")
+        elif self.l8bit:
+            self.bnb_config = BitsAndBytesConfig(
+                load_in_8bit=l8bit, llm_int8_enable_fp32_cpu_offload=fp32_cpu_offload
+            )
         self.checkpoint_every = checkpoint_every
         self.load_checkpoint = load_checkpoint
+        self.gradient_checkpointing = gradient_checkpointing
 
     def dataset(self) -> DataLoader:
-        '''
+        """
         Subclass Pipeline and customize for your own dataset.
-        '''
+        """
 
         data = Data(
             load_args=(self.dataset_name, self.dataset_language),
             tokenizer=self.tokenizer,
             seed=self.seed,
             batch_size=self.batch_size,
             grad_accum=self.grad_accum,
@@ -73,29 +98,28 @@
         columns = data.dataset.features
 
         def filter_longer(sample):
             tokens, _attn_mask = self.tokenizer(sample["whole_func_string"])
 
             return len(tokens) <= self.block_size
 
-
         def truncate(sample):
-            sample["attention_mask"] = sample["attention_mask"][:self.block_size]
-            sample["input_ids"] = sample["input_ids"][:self.block_size]
-
+            sample["attention_mask"] = sample["attention_mask"][: self.block_size]
+            sample["input_ids"] = sample["input_ids"][: self.block_size]
             return sample
 
-
         dataloader = data.prepare(
             [
                 ("filter", filter_longer, {}),
                 (
                     "map",
                     lambda sample: self.tokenizer(
-                        sample["whole_func_string"], padding="max_length", max_length=self.block_size
+                        sample["whole_func_string"],
+                        padding="max_length",
+                        max_length=self.block_size,
                     ),
                     dict(batched=True, remove_columns=columns, num_proc=8),
                 ),
                 ("map", truncate, dict(num_proc=8)),
             ]
         )
         return dataloader
@@ -106,32 +130,47 @@
             self.tokenizer.pad_token_id = self.tokenizer.eos_token_id
 
         data = self.dataset()
 
         self.model = AutoModelForCausalLM.from_pretrained(
             self.model_name_or_path,
             device_map="auto",
-            load_in_8bit=self.l8bit,
+            quantization_config=self.bnb_config
         )
 
         target_modules = None
+
+        print(self.model)
+
         if "gpt-neox" in self.model_name_or_path:
             target_modules = ["query_key_value", "xxx"]
 
+        if "rwkv" in self.model_name_or_path:
+            target_modules = ["key", "value", "receptance", "xxx"]
+
         peft_config = LoraConfig(
             task_type=TaskType.CAUSAL_LM,
             target_modules=target_modules,
             inference_mode=False,
-            r=16,
-            lora_alpha=32,
+            r=8,
+            lora_alpha=16,
             lora_dropout=0.05,
+            bias="none"
         )
 
-        if self.l8bit:
-            self.model = prepare_model_for_int8_training(self.model)
+
+        if self.l4bit:
+            from peft import prepare_model_for_kbit_training
+            self.model = prepare_model_for_kbit_training(
+                self.model, use_gradient_checkpointing=self.gradient_checkpointing
+            )
+        elif self.l8bit:
+            self.model = prepare_model_for_int8_training(
+                self.model, use_gradient_checkpointing=self.gradient_checkpointing
+            )
 
         if hasattr(self.model, "embed_out"):
             output_embedding_layer = getattr(self.model, "embed_out")
             input_dtype = output_embedding_layer.weight.dtype
 
             class CastOutputToFloat(torch.nn.Sequential):
                 r"""
@@ -143,39 +182,46 @@
                     return super().forward(x.to(input_dtype)).to(torch.float32)
 
             setattr(self.model, "embed_out", CastOutputToFloat(output_embedding_layer))
 
         self.model = get_peft_model(self.model, peft_config)
 
         ### Training
+        if self.gradient_checkpointing:
+            self.model.gradient_checkpointing_enable()
 
-
-        self.model.gradient_checkpointing_enable()
-        self.model.config.use_cache = False  # silence the warnings. Please re-enable for inference!
+        self.model.config.use_cache = (
+            False  # silence the warnings. Please re-enable for inference!
+        )
 
         adam_beta1 = 0.9
         adam_beta2 = 0.999
         adam_epsilon = 1e-08
         adam_kwargs = {
             "betas": (adam_beta1, adam_beta2),
             "eps": adam_epsilon,
         }
-        optimizer = torch.optim.AdamW(self.model.parameters(), lr=0.97e-5, **adam_kwargs)
+        optimizer = torch.optim.AdamW(
+            self.model.parameters(), lr=0.97e-5, **adam_kwargs
+        )
 
         trainer = Trainer(
             model=self.model,
             optimizer=optimizer,
             dataset=data,
             device="cuda",
             grad_accum=self.grad_accum,
             fp16=self.fp16,
             output_dir=self.output_dir,
             checkpoint_every=self.checkpoint_every,
             load_checkpoint=self.load_checkpoint,
+            use_bfloat16=self.use_bfloat16,
             seed=self.seed,
         )
 
-        trainer.train(epochs=self.epochs, max_steps=self.max_steps if self.max_steps else None)
+        trainer.train(
+            epochs=self.epochs, max_steps=self.max_steps if self.max_steps else None
+        )
 
         # ## Share adapters on the 🤗 Hub
         if self.push_to_hub:
-            self.model.push_to_hub(self.output_dir, use_auth_token=True)
+            self.model.push_to_hub(self.output_dir, use_auth_token=True)
```

### Comparing `ditty-0.2.3/lib/ditty/trainer.py` & `ditty-0.3.0/lib/ditty/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from transformers.trainer_pt_utils import (
     get_model_param_count,
 )
 import atexit
 
 import numpy as np
 import random
+import contextlib
 
 from peft import PeftModelForCausalLM
 from logging import getLogger
 from typing import Optional
 import os
 
 from transformers import (
@@ -52,14 +53,15 @@
     dataset: DataLoader
     device: torch.device
     scheduler: torch.optim.lr_scheduler._LRScheduler | None = None
     use_scheduler: bool = True
     grad_accum: int = 1
     accelerator_kwargs: dict = field(default_factory=dict)
     fp16: bool = False
+    use_bfloat16: bool = False
     output_dir: str = "./output"
     checkpoint_every: int = 1000
     load_checkpoint: bool = False
     seed: Optional[int] = None
 
     def __post_init__(self):
         if self.seed:
@@ -68,14 +70,19 @@
         os.makedirs(self.output_dir, exist_ok=True)
 
         self.batch_size = self.dataset.batch_size
 
         if self.use_scheduler and not self.scheduler:
             self.scheduler = default_scheduler_factory(self.optimizer)
 
+        if self.fp16 and self.use_bfloat16:
+            self.f16_dtype = torch.bfloat16
+        elif self.fp16:
+            self.f16_dtype = torch.float16
+
         acc_kwargs = {
             "gradient_accumulation_steps": self.grad_accum,
             "project_dir": self.output_dir,
             "project_config": ProjectConfiguration(
                 project_dir=self.output_dir,
                 automatic_checkpoint_naming=True,
             )
@@ -105,14 +112,20 @@
     def _save(self, no_dist=False):
         self.accelerator.wait_for_everyone() 
         self.accelerator.save_state()
         if not no_dist:
             self._save_dist()
 
     def _train_accelerate(self, epochs=1, max_steps=None):
+        context_manager =  contextlib.nullcontext()
+
+        if self.fp16:
+            context_manager = torch.cuda.amp.autocast(cache_enabled=False, dtype=self.f16_dtype)
+
+
         self.model.train()
 
         if self.load_checkpoint:
             try:
                 last_cp = sorted(os.listdir(f"{self.output_dir}/checkpoints/"))[-1]
                 logger.info(f"Trying to load checkpoint: {last_cp}....")
                 self.accelerator.load_state(f"{self.output_dir}/checkpoints/{last_cp}")
@@ -133,16 +146,17 @@
             dataset = self.dataset
 
             if self.state.steps > 0:
                 dataset = self.accelerator.skip_first_batches(self.dataset, self.state.steps)
 
             for batch_idx, batch in enumerate(dataset):
                 with self.accelerator.accumulate(self.model):
-                    outputs = self.model(**batch)
-                    loss = outputs["loss"] if isinstance(outputs, dict) else outputs[0]
+                    with context_manager:
+                        outputs = self.model(**batch)
+                        loss = outputs["loss"] if isinstance(outputs, dict) else outputs[0]
 
                     self.accelerator.backward(loss)
 
                     self.optimizer.step()
                     if self.use_scheduler:
                         self.scheduler.step()
                     self.optimizer.zero_grad()
```

### Comparing `ditty-0.2.3/lib/ditty.egg-info/PKG-INFO` & `ditty-0.3.0/lib/ditty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ditty
-Version: 0.2.3
+Version: 0.3.0
 Home-page: https://github.com/iantbutler01/ditty
 Author: Ian T Butler (KinglyCrow)
 Author-email: iantbutler01@gmail.com
 License: Apache V2
 Keywords: finetuning,llm,nlp,machine learning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ditty-0.2.3/setup.py` & `ditty-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='ditty',
-    version='0.2.3',
+    version='0.3.0',
     license='Apache V2',
     author="Ian T Butler (KinglyCrow)",
     author_email='iantbutler01@gmail.com',
     packages=find_packages('lib'),
     package_dir={'': 'lib'},
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

