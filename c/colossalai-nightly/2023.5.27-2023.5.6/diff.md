# Comparing `tmp/colossalai-nightly-2023.5.27.tar.gz` & `tmp/colossalai-nightly-2023.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colossalai-nightly-2023.5.27.tar", last modified: Sat May 27 00:15:14 2023, max compression
+gzip compressed data, was "colossalai-nightly-2023.5.6.tar", last modified: Sat May  6 00:13:49 2023, max compression
```

## Comparing `colossalai-nightly-2023.5.27.tar` & `colossalai-nightly-2023.5.6.tar`

### file list

```diff
@@ -1,901 +1,873 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.596653 colossalai-nightly-2023.5.27/
--rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25400 2023-05-27 00:15:14.596653 colossalai-nightly-2023.5.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20789 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.516652 colossalai-nightly-2023.5.27/colossalai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.516652 colossalai-nightly-2023.5.27/colossalai/_C/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_C/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.516652 colossalai-nightly-2023.5.27/colossalai/_analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.516652 colossalai-nightly-2023.5.27/colossalai/_analyzer/_subclasses/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/_subclasses/_meta_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/_subclasses/_monkey_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    18694 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/_subclasses/flop_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/_subclasses/meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/envs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.516652 colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/graph_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/node_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.516652 colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/passes/graph_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/passes/shape_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/symbolic_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.516652 colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/tracer/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/tracer/bias_addition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/tracer/custom_leaf_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/tracer/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/tracer/symbolic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/tracer/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.516652 colossalai-nightly-2023.5.27/colossalai/amp/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/amp/amp_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.516652 colossalai-nightly-2023.5.27/colossalai/amp/apex_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/amp/apex_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/amp/apex_amp/apex_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.520652 colossalai-nightly-2023.5.27/colossalai/amp/naive_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/amp/naive_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/amp/naive_amp/_fp16_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/amp/naive_amp/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.520652 colossalai-nightly-2023.5.27/colossalai/amp/naive_amp/grad_scaler/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/amp/naive_amp/grad_scaler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/amp/naive_amp/naive_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.520652 colossalai-nightly-2023.5.27/colossalai/amp/torch_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/amp/torch_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/amp/torch_amp/_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/amp/torch_amp/torch_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.520652 colossalai-nightly-2023.5.27/colossalai/auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.520652 colossalai-nightly-2023.5.27/colossalai/auto_parallel/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/checkpoint/build_c_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
--rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/checkpoint/operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.520652 colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.520652 colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.524652 colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/amp_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/base_offload_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/mem_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/region.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/region_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/training_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.524652 colossalai-nightly-2023.5.27/colossalai/auto_parallel/passes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/passes/comm_metainfo_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/passes/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/passes/runtime_apply_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    22686 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/passes/runtime_preparation_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.524652 colossalai-nightly-2023.5.27/colossalai/auto_parallel/pipeline_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/pipeline_shard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.524652 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.524652 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.528652 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43503 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.528652 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/solver/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.528652 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/utils/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/utils/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/utils/sharding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.528652 colossalai-nightly-2023.5.27/colossalai/booster/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/booster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/booster/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11106 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/booster/booster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.528652 colossalai-nightly-2023.5.27/colossalai/booster/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/booster/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/booster/mixed_precision/bf16.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/booster/mixed_precision/fp16_apex.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/booster/mixed_precision/fp16_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/booster/mixed_precision/fp16_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/booster/mixed_precision/fp8.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/booster/mixed_precision/mixed_precision_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.532652 colossalai-nightly-2023.5.27/colossalai/booster/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/booster/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/booster/plugin/dp_plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13628 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/booster/plugin/gemini_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/booster/plugin/low_level_zero_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/booster/plugin/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/booster/plugin/torch_ddp_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/booster/plugin/torch_fsdp_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.532652 colossalai-nightly-2023.5.27/colossalai/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/builder/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.532652 colossalai-nightly-2023.5.27/colossalai/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/checkpoint_io/checkpoint_io_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/checkpoint_io/general_checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/checkpoint_io/index_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/checkpoint_io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.532652 colossalai-nightly-2023.5.27/colossalai/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.532652 colossalai-nightly-2023.5.27/colossalai/cli/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/cli/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/cli/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/cli/benchmark/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/cli/benchmark/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.532652 colossalai-nightly-2023.5.27/colossalai/cli/check/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/cli/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/cli/check/check_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.532652 colossalai-nightly-2023.5.27/colossalai/cli/launcher/
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/cli/launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/cli/launcher/hostinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/cli/launcher/multinode_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/cli/launcher/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.532652 colossalai-nightly-2023.5.27/colossalai/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/cluster/device_mesh_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/cluster/dist_coordinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/cluster/process_group_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.532652 colossalai-nightly-2023.5.27/colossalai/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/communication/collective.py
--rw-r--r--   0 runner    (1001) docker     (123)    19462 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/communication/p2p.py
--rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/communication/p2p_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/communication/ring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/communication/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.532652 colossalai-nightly-2023.5.27/colossalai/context/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/moe_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/parallel_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/parallel_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.536652 colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/initializer_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/initializer_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/initializer_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/initializer_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/initializer_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/initializer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/initializer_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/initializer_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/initializer_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/process_group_initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.536652 colossalai-nightly-2023.5.27/colossalai/context/random/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/random/_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/random/seed_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/context/singleton_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.536652 colossalai-nightly-2023.5.27/colossalai/device/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17419 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/device/alpha_beta_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/device/calc_pipeline_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/device/device_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.536652 colossalai-nightly-2023.5.27/colossalai/engine/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/engine/_base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.536652 colossalai-nightly-2023.5.27/colossalai/engine/gradient_accumulation/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/engine/gradient_accumulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/engine/gradient_accumulation/_gradient_accumulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.536652 colossalai-nightly-2023.5.27/colossalai/engine/gradient_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/engine/gradient_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/engine/gradient_handler/_base_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/engine/gradient_handler/_moe_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/engine/gradient_handler/_zero_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/engine/gradient_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.536652 colossalai-nightly-2023.5.27/colossalai/engine/schedule/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/engine/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/engine/schedule/_base_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/engine/schedule/_non_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/engine/schedule/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/engine/schedule/_pipeline_schedule_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.536652 colossalai-nightly-2023.5.27/colossalai/fx/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/_meta_regist_12.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/_meta_regist_13.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.536652 colossalai-nightly-2023.5.27/colossalai/fx/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44753 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/codegen/activation_checkpoint_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/graph_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.540652 colossalai-nightly-2023.5.27/colossalai/fx/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/passes/adding_split_node_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/passes/concrete_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/passes/passes_for_gpt2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/passes/shard_1d_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/passes/split_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/passes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.540652 colossalai-nightly-2023.5.27/colossalai/fx/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.540652 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.540652 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_function/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_function/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_function/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.540652 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_module/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_module/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_module/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/memory_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/opcount.py
--rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/profiler/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.540652 colossalai-nightly-2023.5.27/colossalai/fx/tracer/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/_meta_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/_symbolic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/_tracer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.540652 colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.544653 colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.544653 colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.544653 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.544653 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_function/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.544653 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_module/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    24623 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/fx/tracer/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/global_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.544653 colossalai-nightly-2023.5.27/colossalai/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/interface/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/interface/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.544653 colossalai-nightly-2023.5.27/colossalai/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.544653 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.548653 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/compat.h
--rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/cpu_adam.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.548653 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu
--rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.548653 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/context.h
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
--rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/type_shim.h
--rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/scaled_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.548653 colossalai-nightly-2023.5.27/colossalai/kernel/jit/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/jit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/jit/bias_dropout_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/jit/bias_gelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/jit/option.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.552652 colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/fused_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/moe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/multi_head_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/scaled_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.552652 colossalai-nightly-2023.5.27/colossalai/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.552652 colossalai-nightly-2023.5.27/colossalai/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.552652 colossalai-nightly-2023.5.27/colossalai/nn/_ops/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/_ops/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/_ops/addmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/_ops/batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/_ops/element_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/_ops/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/_ops/embedding_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/_ops/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/_ops/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/_ops/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/_ops/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.552652 colossalai-nightly-2023.5.27/colossalai/nn/layer/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/base_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.552652 colossalai-nightly-2023.5.27/colossalai/nn/layer/colossalai_layer/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/colossalai_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/colossalai_layer/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/colossalai_layer/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/colossalai_layer/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/colossalai_layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/colossalai_layer/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.552652 colossalai-nightly-2023.5.27/colossalai/nn/layer/moe/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/moe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/moe/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/moe/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/moe/experts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/moe/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/moe/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/moe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.552652 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_1d/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_1d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_1d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49753 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_1d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.556653 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_2d/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_2d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_2d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50524 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_2d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.556653 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_2p5d/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_2p5d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37643 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_2p5d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_2p5d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_2p5d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.556653 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_3d/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_3d/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22769 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_3d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_3d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_3d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.560653 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_sequence/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_sequence/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_sequence/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.560653 colossalai-nightly-2023.5.27/colossalai/nn/layer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.560653 colossalai-nightly-2023.5.27/colossalai/nn/layer/vanilla/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/vanilla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/vanilla/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.560653 colossalai-nightly-2023.5.27/colossalai/nn/layer/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/layer/wrapper/pipeline_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.560653 colossalai-nightly-2023.5.27/colossalai/nn/loss/
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/loss/loss_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/loss/loss_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/loss/loss_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/loss/loss_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/loss/loss_moe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.560653 colossalai-nightly-2023.5.27/colossalai/nn/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/lr_scheduler/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/lr_scheduler/delayed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/lr_scheduler/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/lr_scheduler/multistep.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/lr_scheduler/onecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/lr_scheduler/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/lr_scheduler/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.560653 colossalai-nightly-2023.5.27/colossalai/nn/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/metric/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/metric/accuracy_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/metric/accuracy_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/metric/accuracy_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.560653 colossalai-nightly-2023.5.27/colossalai/nn/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/optimizer/colossalai_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/optimizer/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/optimizer/fused_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/optimizer/fused_lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/optimizer/fused_sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/optimizer/hybrid_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/optimizer/lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/optimizer/lars.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/optimizer/nvme_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.564653 colossalai-nightly-2023.5.27/colossalai/nn/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/parallel/data_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.564653 colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.564653 colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/copyer.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/colo_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/nn/parallel/reducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.564653 colossalai-nightly-2023.5.27/colossalai/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/pipeline/layer_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.564653 colossalai-nightly-2023.5.27/colossalai/pipeline/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/pipeline/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.564653 colossalai-nightly-2023.5.27/colossalai/pipeline/middleware/adaptor/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/pipeline/middleware/adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/pipeline/middleware/adaptor/fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/pipeline/middleware/topo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/pipeline/pipelinable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/pipeline/pipeline_process_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.564653 colossalai-nightly-2023.5.27/colossalai/pipeline/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/pipeline/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59163 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/pipeline/rpc/_pipeline_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/pipeline/rpc/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/pipeline/rpc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.564653 colossalai-nightly-2023.5.27/colossalai/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/registry/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.568653 colossalai-nightly-2023.5.27/colossalai/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/colo_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/colo_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22269 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/compute_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.568653 colossalai-nightly-2023.5.27/colossalai/tensor/d_tensor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/d_tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/d_tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/d_tensor/d_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/d_tensor/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    25229 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/d_tensor/layout_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/d_tensor/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/d_tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/d_tensor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/dist_spec_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/distspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/op_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/param_op_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/process_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    36495 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/shape_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/tensor_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.568653 colossalai-nightly-2023.5.27/colossalai/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/testing/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/testing/pytest_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/testing/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.568653 colossalai-nightly-2023.5.27/colossalai/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/trainer/_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.568653 colossalai-nightly-2023.5.27/colossalai/trainer/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/trainer/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/trainer/hooks/_base_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/trainer/hooks/_checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/trainer/hooks/_commons_.py
--rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/trainer/hooks/_log_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/trainer/hooks/_lr_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/trainer/hooks/_metric_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.572653 colossalai-nightly-2023.5.27/colossalai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/activation_checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.572653 colossalai-nightly-2023.5.27/colossalai/utils/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/checkpoint/module_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/checkpoint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.572653 colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/convertor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.572653 colossalai-nightly-2023.5.27/colossalai/utils/data_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/data_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/data_sampler/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/data_sampler/data_parallel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.572653 colossalai-nightly-2023.5.27/colossalai/utils/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/model/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/model/lazy_init_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/moe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.572653 colossalai-nightly-2023.5.27/colossalai/utils/multi_tensor_apply/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/multi_tensor_apply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.572653 colossalai-nightly-2023.5.27/colossalai/utils/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/profiler/extention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.572653 colossalai-nightly-2023.5.27/colossalai/utils/profiler/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/profiler/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/profiler/legacy/comm_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/profiler/legacy/pcie_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/profiler/legacy/prof_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/profiler/stateful_tensor_mem_extention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.576653 colossalai-nightly-2023.5.27/colossalai/utils/rank_recorder/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/rank_recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/rank_recorder/rank_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.576653 colossalai-nightly-2023.5.27/colossalai/utils/tensor_detector/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/tensor_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/tensor_detector/tensor_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.576653 colossalai-nightly-2023.5.27/colossalai/zero/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.576653 colossalai-nightly-2023.5.27/colossalai/zero/gemini/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.576653 colossalai-nightly-2023.5.27/colossalai/zero/gemini/chunk/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/chunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/chunk/chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/chunk/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/chunk/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/chunk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/colo_init_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/gemini_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/gemini_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/gemini_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/gemini_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.576653 colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/memory_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/gemini/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.576653 colossalai-nightly-2023.5.27/colossalai/zero/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.580653 colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/gemini_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.580653 colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/ophooks/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/ophooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/ophooks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.580653 colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/paramhooks/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/paramhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/stateful_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/tensor_placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/tensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.580653 colossalai-nightly-2023.5.27/colossalai/zero/legacy/init_ctx/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/init_ctx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/init_ctx/init_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.580653 colossalai-nightly-2023.5.27/colossalai/zero/legacy/shard_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/shard_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/shard_utils/base_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/shard_utils/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.580653 colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_model/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_model/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_model/reduce_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29015 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_model/sharded_model_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_model/zero_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.580653 colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_optim/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.580653 colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_param/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_param/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_param/sharded_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_param/sharded_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.584653 colossalai-nightly-2023.5.27/colossalai/zero/low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/low_level/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.584653 colossalai-nightly-2023.5.27/colossalai/zero/low_level/bookkeeping/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/low_level/bookkeeping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/low_level/bookkeeping/base_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/low_level/bookkeeping/bucket_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/low_level/bookkeeping/gradient_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/low_level/bookkeeping/parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    25694 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/low_level/low_level_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/colossalai/zero/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.584653 colossalai-nightly-2023.5.27/colossalai_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25400 2023-05-27 00:15:14.000000 colossalai-nightly-2023.5.27/colossalai_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37387 2023-05-27 00:15:14.000000 colossalai-nightly-2023.5.27/colossalai_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 00:15:14.000000 colossalai-nightly-2023.5.27/colossalai_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-27 00:15:14.000000 colossalai-nightly-2023.5.27/colossalai_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-27 00:15:14.000000 colossalai-nightly-2023.5.27/colossalai_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-27 00:15:14.000000 colossalai-nightly-2023.5.27/colossalai_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.584653 colossalai-nightly-2023.5.27/op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/op_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/op_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/op_builder/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/op_builder/fused_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/op_builder/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/op_builder/moe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/op_builder/multi_head_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/op_builder/scaled_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/op_builder/scaled_upper_triangle_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/op_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.584653 colossalai-nightly-2023.5.27/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 00:15:14.596653 colossalai-nightly-2023.5.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.512652 colossalai-nightly-2023.5.27/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.588653 colossalai-nightly-2023.5.27/tests/components_to_test/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/components_to_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/components_to_test/albert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/components_to_test/beit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/components_to_test/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/components_to_test/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/components_to_test/hanging_param_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/components_to_test/inline_op_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/components_to_test/nested_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/components_to_test/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/components_to_test/repeated_computed_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/components_to_test/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/components_to_test/simple_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.588653 colossalai-nightly-2023.5.27/tests/components_to_test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/components_to_test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/components_to_test/utils/dummy_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/components_to_test/utils/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.588653 colossalai-nightly-2023.5.27/tests/kit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.588653 colossalai-nightly-2023.5.27/tests/kit/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/model_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.588653 colossalai-nightly-2023.5.27/tests/kit/model_zoo/diffusers/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/model_zoo/diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/model_zoo/diffusers/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/model_zoo/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.588653 colossalai-nightly-2023.5.27/tests/kit/model_zoo/timm/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/model_zoo/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/model_zoo/timm/timm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.588653 colossalai-nightly-2023.5.27/tests/kit/model_zoo/torchaudio/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/model_zoo/torchaudio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/model_zoo/torchaudio/torchaudio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.588653 colossalai-nightly-2023.5.27/tests/kit/model_zoo/torchrec/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/model_zoo/torchrec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/model_zoo/torchrec/torchrec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.588653 colossalai-nightly-2023.5.27/tests/kit/model_zoo/torchvision/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/model_zoo/torchvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/model_zoo/torchvision/torchvision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.588653 colossalai-nightly-2023.5.27/tests/kit/model_zoo/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/model_zoo/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/model_zoo/transformers/albert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/model_zoo/transformers/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/model_zoo/transformers/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/model_zoo/transformers/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/kit/model_zoo/transformers/t5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.588653 colossalai-nightly-2023.5.27/tests/test_analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.592653 colossalai-nightly-2023.5.27/tests/test_analyzer/test_fx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_analyzer/test_fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_analyzer/test_fx/test_bias_addition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_analyzer/test_fx/test_mod_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_analyzer/test_fx/test_nested_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_analyzer/test_fx/test_shape_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_analyzer/test_fx/test_symbolic_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_analyzer/test_fx/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.592653 colossalai-nightly-2023.5.27/tests/test_analyzer/test_subclasses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_analyzer/test_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_analyzer/test_subclasses/test_aten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_analyzer/test_subclasses/test_flop_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_analyzer/test_subclasses/test_meta_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.592653 colossalai-nightly-2023.5.27/tests/test_auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.592653 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_pass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_pass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.592653 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.592653 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:15:14.596653 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 00:14:57.000000 colossalai-nightly-2023.5.27/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.503494 colossalai-nightly-2023.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    24364 2023-05-06 00:13:49.503494 colossalai-nightly-2023.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19962 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.411486 colossalai-nightly-2023.5.6/colossalai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.411486 colossalai-nightly-2023.5.6/colossalai/_C/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/_C/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.415486 colossalai-nightly-2023.5.6/colossalai/amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/amp_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.415486 colossalai-nightly-2023.5.6/colossalai/amp/apex_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/apex_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/apex_amp/apex_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.415486 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/_fp16_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.415486 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/grad_scaler/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/grad_scaler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/naive_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.415486 colossalai-nightly-2023.5.6/colossalai/amp/torch_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/torch_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/torch_amp/_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/amp/torch_amp/torch_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.415486 colossalai-nightly-2023.5.6/colossalai/auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.415486 colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/build_c_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.415486 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.419486 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.419486 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/amp_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/base_offload_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/mem_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/region_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/training_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.419486 colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/comm_metainfo_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/runtime_apply_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22689 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/runtime_preparation_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.419486 colossalai-nightly-2023.5.6/colossalai/auto_parallel/pipeline_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/pipeline_shard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.419486 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.423487 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14745 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20533 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.427487 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43503 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.427487 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9987 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.427487 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/sharding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.427487 colossalai-nightly-2023.5.6/colossalai/booster/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/booster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.427487 colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/bf16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/fp16_apex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/fp16_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/fp8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/mixed_precision_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.431487 colossalai-nightly-2023.5.6/colossalai/booster/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/plugin/dp_plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/plugin/gemini_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/plugin/low_level_zero_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/plugin/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/booster/plugin/torch_ddp_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.431487 colossalai-nightly-2023.5.6/colossalai/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/builder/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.431487 colossalai-nightly-2023.5.6/colossalai/checkpoint_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/checkpoint_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/checkpoint_io/checkpoint_io_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/checkpoint_io/general_checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/checkpoint_io/index_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/checkpoint_io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.431487 colossalai-nightly-2023.5.6/colossalai/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.431487 colossalai-nightly-2023.5.6/colossalai/cli/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/benchmark/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/benchmark/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.431487 colossalai-nightly-2023.5.6/colossalai/cli/check/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/check/check_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.431487 colossalai-nightly-2023.5.6/colossalai/cli/launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/launcher/hostinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/launcher/multinode_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cli/launcher/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.431487 colossalai-nightly-2023.5.6/colossalai/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cluster/device_mesh_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cluster/dist_coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/cluster/process_group_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.435488 colossalai-nightly-2023.5.6/colossalai/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/communication/collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19463 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/communication/p2p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/communication/p2p_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/communication/ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/communication/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.435488 colossalai-nightly-2023.5.6/colossalai/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/moe_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/parallel_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/parallel_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.435488 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/process_group_initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.435488 colossalai-nightly-2023.5.6/colossalai/context/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/random/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/random/seed_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/context/singleton_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.435488 colossalai-nightly-2023.5.6/colossalai/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/device/alpha_beta_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/device/calc_pipeline_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/device/device_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.435488 colossalai-nightly-2023.5.6/colossalai/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/_base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.435488 colossalai-nightly-2023.5.6/colossalai/engine/gradient_accumulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_accumulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_accumulation/_gradient_accumulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.439488 colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_base_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_moe_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_zero_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.439488 colossalai-nightly-2023.5.6/colossalai/engine/schedule/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/schedule/_base_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/schedule/_non_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/schedule/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/engine/schedule/_pipeline_schedule_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.439488 colossalai-nightly-2023.5.6/colossalai/fx/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/_meta_regist_12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/_meta_regist_13.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.439488 colossalai-nightly-2023.5.6/colossalai/fx/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44751 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/codegen/activation_checkpoint_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/graph_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.439488 colossalai-nightly-2023.5.6/colossalai/fx/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/passes/adding_split_node_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/passes/concrete_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/passes/passes_for_gpt2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/passes/shard_1d_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/passes/split_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/passes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.443488 colossalai-nightly-2023.5.6/colossalai/fx/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.443488 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.443488 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.443488 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/memory_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/opcount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/profiler/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.447489 colossalai-nightly-2023.5.6/colossalai/fx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/_meta_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/_symbolic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/_tracer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.447489 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.447489 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.447489 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.447489 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.447489 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.451489 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24623 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/fx/tracer/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/global_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.451489 colossalai-nightly-2023.5.6/colossalai/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/interface/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/interface/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.451489 colossalai-nightly-2023.5.6/colossalai/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.451489 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.455490 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/cpu_adam.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.455490 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.459490 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/context.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/type_shim.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/scaled_softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.459490 colossalai-nightly-2023.5.6/colossalai/kernel/jit/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/jit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/jit/bias_dropout_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/jit/bias_gelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/jit/option.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.459490 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/fused_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/multi_head_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/scaled_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.459490 colossalai-nightly-2023.5.6/colossalai/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.459490 colossalai-nightly-2023.5.6/colossalai/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.459490 colossalai-nightly-2023.5.6/colossalai/nn/_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/element_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/embedding_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/_ops/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.459490 colossalai-nightly-2023.5.6/colossalai/nn/layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/base_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.463490 colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.463490 colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/experts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.463490 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_1d/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_1d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_1d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_1d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49753 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_1d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.463490 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2d/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50524 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.463490 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2p5d/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2p5d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37643 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2p5d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2p5d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2p5d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.463490 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_3d/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22769 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_3d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_3d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_3d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.463490 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_sequence/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_sequence/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_sequence/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.467491 colossalai-nightly-2023.5.6/colossalai/nn/layer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.467491 colossalai-nightly-2023.5.6/colossalai/nn/layer/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/vanilla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/vanilla/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.467491 colossalai-nightly-2023.5.6/colossalai/nn/layer/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/layer/wrapper/pipeline_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.467491 colossalai-nightly-2023.5.6/colossalai/nn/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_moe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.467491 colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/delayed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/multistep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/onecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.467491 colossalai-nightly-2023.5.6/colossalai/nn/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/metric/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/metric/accuracy_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/metric/accuracy_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/metric/accuracy_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.471491 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/colossalai_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/fused_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/fused_lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/fused_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/hybrid_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/lars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/optimizer/nvme_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.471491 colossalai-nightly-2023.5.6/colossalai/nn/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/data_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.471491 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.471491 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/copyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/colo_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/nn/parallel/reducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.471491 colossalai-nightly-2023.5.6/colossalai/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/layer_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.471491 colossalai-nightly-2023.5.6/colossalai/pipeline/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/middleware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.471491 colossalai-nightly-2023.5.6/colossalai/pipeline/middleware/adaptor/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/middleware/adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/middleware/adaptor/fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/middleware/topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/pipelinable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/pipeline_process_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.471491 colossalai-nightly-2023.5.6/colossalai/pipeline/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59163 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/rpc/_pipeline_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/rpc/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/rpc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.475492 colossalai-nightly-2023.5.6/colossalai/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/registry/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.475492 colossalai-nightly-2023.5.6/colossalai/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/colo_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/colo_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22269 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/compute_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.475492 colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/d_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25229 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/layout_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/dist_spec_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/distspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/op_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/param_op_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/process_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36495 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/shape_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/tensor_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.475492 colossalai-nightly-2023.5.6/colossalai/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/testing/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/testing/pytest_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/testing/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.475492 colossalai-nightly-2023.5.6/colossalai/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/trainer/_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.479492 colossalai-nightly-2023.5.6/colossalai/trainer/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/trainer/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_base_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_commons_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_log_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_lr_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_metric_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.479492 colossalai-nightly-2023.5.6/colossalai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/activation_checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.479492 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint/module_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.479492 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/convertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17451 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.479492 colossalai-nightly-2023.5.6/colossalai/utils/data_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/data_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/data_sampler/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/data_sampler/data_parallel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.479492 colossalai-nightly-2023.5.6/colossalai/utils/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/model/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/model/lazy_init_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/moe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.483492 colossalai-nightly-2023.5.6/colossalai/utils/multi_tensor_apply/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/multi_tensor_apply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.483492 colossalai-nightly-2023.5.6/colossalai/utils/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/profiler/extention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.483492 colossalai-nightly-2023.5.6/colossalai/utils/profiler/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/profiler/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/profiler/legacy/comm_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/profiler/legacy/pcie_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/profiler/legacy/prof_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/profiler/stateful_tensor_mem_extention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.483492 colossalai-nightly-2023.5.6/colossalai/utils/rank_recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/rank_recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/rank_recorder/rank_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.483492 colossalai-nightly-2023.5.6/colossalai/utils/tensor_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/tensor_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/tensor_detector/tensor_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.483492 colossalai-nightly-2023.5.6/colossalai/zero/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.483492 colossalai-nightly-2023.5.6/colossalai/zero/gemini/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.483492 colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/colo_init_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/gemini_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/gemini_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/gemini_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/gemini_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.487493 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/memory_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/gemini/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.487493 colossalai-nightly-2023.5.6/colossalai/zero/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.487493 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/gemini_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.487493 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.487493 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/paramhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/paramhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/stateful_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/tensor_placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/tensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.487493 colossalai-nightly-2023.5.6/colossalai/zero/legacy/init_ctx/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/init_ctx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/init_ctx/init_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.487493 colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/base_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.491493 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/reduce_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29015 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/sharded_model_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/zero_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.491493 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.491493 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_param/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_param/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_param/sharded_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_param/sharded_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.491493 colossalai-nightly-2023.5.6/colossalai/zero/low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/low_level/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.491493 colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/base_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/bucket_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/gradient_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25694 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/low_level/low_level_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/colossalai/zero/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.491493 colossalai-nightly-2023.5.6/colossalai_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24364 2023-05-06 00:13:49.000000 colossalai-nightly-2023.5.6/colossalai_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36381 2023-05-06 00:13:49.000000 colossalai-nightly-2023.5.6/colossalai_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:13:49.000000 colossalai-nightly-2023.5.6/colossalai_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-06 00:13:49.000000 colossalai-nightly-2023.5.6/colossalai_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-06 00:13:49.000000 colossalai-nightly-2023.5.6/colossalai_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-06 00:13:49.000000 colossalai-nightly-2023.5.6/colossalai_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.491493 colossalai-nightly-2023.5.6/op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/fused_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/multi_head_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/scaled_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/scaled_upper_triangle_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/op_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.491493 colossalai-nightly-2023.5.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 00:13:49.503494 colossalai-nightly-2023.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.411486 colossalai-nightly-2023.5.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/components_to_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/albert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/beit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/hanging_param_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/inline_op_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/nested_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/repeated_computed_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/simple_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/components_to_test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/utils/dummy_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/components_to_test/utils/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/kit/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/kit/model_zoo/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/diffusers/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/kit/model_zoo/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/timm/timm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchaudio/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchaudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchaudio/torchaudio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchrec/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchrec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchrec/torchrec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchvision/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchvision/torchvision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.495493 colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/albert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/t5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.499494 colossalai-nightly-2023.5.6/tests/test_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.499494 colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_bias_addition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_mod_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_nested_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_shape_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_symbolic_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.499494 colossalai-nightly-2023.5.6/tests/test_analyzer/test_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_subclasses/test_aten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_subclasses/test_flop_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_analyzer/test_subclasses/test_meta_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.499494 colossalai-nightly-2023.5.6/tests/test_auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.499494 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_pass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.499494 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.499494 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:49.503494 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-06 00:13:37.000000 colossalai-nightly-2023.5.6/version.txt
```

### Comparing `colossalai-nightly-2023.5.27/LICENSE` & `colossalai-nightly-2023.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/PKG-INFO` & `colossalai-nightly-2023.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai-nightly
-Version: 2023.5.27
+Version: 2023.5.6
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
@@ -134,30 +134,20 @@
         <p align="right">(<a href="#top">back to top</a>)</p>
         
         ## Colossal-AI in the Real World
         
         ### ColossalChat
         
         <div align="center">
-           <a href="https://www.youtube.com/watch?v=HcTiHzApHm0">
-           <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chat/ColossalChat%20YouTube.png" width="700" />
+           <a href="https://chat.colossalai.org/">
+           <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Chat-demo.png" width="700" />
            </a>
         </div>
         
-        [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline.
-        [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat)
-        [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b)
-        [[demo]](https://www.youtube.com/watch?v=HcTiHzApHm0)
-        [[tutorial]](https://www.youtube.com/watch?v=-qFBZFmOJfg)
-        
-        <p id="ColossalChat-Speed" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chat/ColossalChat%20Speed.jpg" width=450/>
-        </p>
-        
-        - Up to 10 times faster for RLHF PPO Stage3 Training
+        [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://chat.colossalai.org)
         
         <p id="ColossalChat_scaling" align="center">
         <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT%20scaling.png" width=800/>
         </p>
         
         - Up to 7.73 times faster for single server training and 1.42 times faster for single-GPU inference
         
@@ -369,30 +359,14 @@
         By default, we do not compile CUDA/C++ kernels. ColossalAI will build them during runtime.
         If you want to install and enable CUDA kernel fusion (compulsory installation when using fused optimizer):
         
         ```shell
         CUDA_EXT=1 pip install .
         ```
         
-        For Users with CUDA 10.2, you can still build ColossalAI from source. However, you need to manually download the cub library and copy it to the corresponding directory.
-        
-        ```bash
-        # clone the repository
-        git clone https://github.com/hpcaitech/ColossalAI.git
-        cd ColossalAI
-        
-        # download the cub library
-        wget https://github.com/NVIDIA/cub/archive/refs/tags/1.8.0.zip
-        unzip 1.8.0.zip
-        cp -r cub-1.8.0/cub/ colossalai/kernel/cuda_native/csrc/kernels/include/
-        
-        # install
-        CUDA_EXT=1 pip install .
-        ```
-        
         <p align="right">(<a href="#top">back to top</a>)</p>
         
         ## Use Docker
         
         ### Pull from DockerHub
         
         You can directly pull the docker image from our [DockerHub page](https://hub.docker.com/r/hpcaitech/colossalai). The image is automatically uploaded upon release.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.5.27 Summary: An
+Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.5.6 Summary: An
 integrated large-scale model training system with efficient parallelization
 techniques Home-page: https://www.colossalai.org License: Apache Software
 License 2.0 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/
 discussions Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/
 issues Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
@@ -92,26 +92,23 @@
 /arxiv.org/abs/1910.02054) - [Auto-Parallelism](https://arxiv.org/abs/
 2302.02599) - Heterogeneous Memory Management - [PatrickStar](https://
 arxiv.org/abs/2108.05818) - Friendly Usage - Parallelism based on the
 configuration file - Inference - [Energon-AI](https://github.com/hpcaitech/
 EnergonAI)
                                                                   (back_to_top)
 ## Colossal-AI in the Real World ### ColossalChat
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                       chat/ColossalChat%20YouTube.png]
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                Chat-demo.png]
 [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/
 Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/
 chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/
 ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/
 @yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://www.youtube.com/
-watch?v=HcTiHzApHm0) [[tutorial]](https://www.youtube.com/watch?v=-qFBZFmOJfg)
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                        chat/ColossalChat%20Speed.jpg]
-- Up to 10 times faster for RLHF PPO Stage3 Training
+with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://
+chat.colossalai.org)
  [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
                         chatgpt/ChatGPT%20scaling.png]
 - Up to 7.73 times faster for single server training and 1.42 times faster for
 single-GPU inference
  [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
                            chatgpt/ChatGPT-1GPU.jpg]
 - Up to 10.3x growth in model capacity on one GPU - A mini demo training
@@ -228,22 +225,15 @@
 main branch. Installation can be made via ```bash pip install colossalai-
 nightly ``` ### Download From Source > The version of Colossal-AI will be in
 line with the main branch of the repository. Feel free to raise an issue if you
 encounter any problems. :) ```shell git clone https://github.com/hpcaitech/
 ColossalAI.git cd ColossalAI # install colossalai pip install . ``` By default,
 we do not compile CUDA/C++ kernels. ColossalAI will build them during runtime.
 If you want to install and enable CUDA kernel fusion (compulsory installation
-when using fused optimizer): ```shell CUDA_EXT=1 pip install . ``` For Users
-with CUDA 10.2, you can still build ColossalAI from source. However, you need
-to manually download the cub library and copy it to the corresponding
-directory. ```bash # clone the repository git clone https://github.com/
-hpcaitech/ColossalAI.git cd ColossalAI # download the cub library wget https://
-github.com/NVIDIA/cub/archive/refs/tags/1.8.0.zip unzip 1.8.0.zip cp -r cub-
-1.8.0/cub/ colossalai/kernel/cuda_native/csrc/kernels/include/ # install
-CUDA_EXT=1 pip install . ```
+when using fused optimizer): ```shell CUDA_EXT=1 pip install . ```
                                                                   (back_to_top)
 ## Use Docker ### Pull from DockerHub You can directly pull the docker image
 from our [DockerHub page](https://hub.docker.com/r/hpcaitech/colossalai). The
 image is automatically uploaded upon release. ### Build On Your Own Run the
 following command to build a docker image from Dockerfile provided. > Building
 Colossal-AI from scratch requires GPU support, you need to use Nvidia Docker
 Runtime as the default when doing `docker build`. More details can be found
```

### Comparing `colossalai-nightly-2023.5.27/README.md` & `colossalai-nightly-2023.5.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -123,30 +123,20 @@
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Colossal-AI in the Real World
 
 ### ColossalChat
 
 <div align="center">
-   <a href="https://www.youtube.com/watch?v=HcTiHzApHm0">
-   <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chat/ColossalChat%20YouTube.png" width="700" />
+   <a href="https://chat.colossalai.org/">
+   <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Chat-demo.png" width="700" />
    </a>
 </div>
 
-[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline.
-[[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat)
-[[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b)
-[[demo]](https://www.youtube.com/watch?v=HcTiHzApHm0)
-[[tutorial]](https://www.youtube.com/watch?v=-qFBZFmOJfg)
-
-<p id="ColossalChat-Speed" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chat/ColossalChat%20Speed.jpg" width=450/>
-</p>
-
-- Up to 10 times faster for RLHF PPO Stage3 Training
+[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://chat.colossalai.org)
 
 <p id="ColossalChat_scaling" align="center">
 <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT%20scaling.png" width=800/>
 </p>
 
 - Up to 7.73 times faster for single server training and 1.42 times faster for single-GPU inference
 
@@ -358,30 +348,14 @@
 By default, we do not compile CUDA/C++ kernels. ColossalAI will build them during runtime.
 If you want to install and enable CUDA kernel fusion (compulsory installation when using fused optimizer):
 
 ```shell
 CUDA_EXT=1 pip install .
 ```
 
-For Users with CUDA 10.2, you can still build ColossalAI from source. However, you need to manually download the cub library and copy it to the corresponding directory.
-
-```bash
-# clone the repository
-git clone https://github.com/hpcaitech/ColossalAI.git
-cd ColossalAI
-
-# download the cub library
-wget https://github.com/NVIDIA/cub/archive/refs/tags/1.8.0.zip
-unzip 1.8.0.zip
-cp -r cub-1.8.0/cub/ colossalai/kernel/cuda_native/csrc/kernels/include/
-
-# install
-CUDA_EXT=1 pip install .
-```
-
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Use Docker
 
 ### Pull from DockerHub
 
 You can directly pull the docker image from our [DockerHub page](https://hub.docker.com/r/hpcaitech/colossalai). The image is automatically uploaded upon release.
```

#### html2text {}

```diff
@@ -85,26 +85,23 @@
 /arxiv.org/abs/1910.02054) - [Auto-Parallelism](https://arxiv.org/abs/
 2302.02599) - Heterogeneous Memory Management - [PatrickStar](https://
 arxiv.org/abs/2108.05818) - Friendly Usage - Parallelism based on the
 configuration file - Inference - [Energon-AI](https://github.com/hpcaitech/
 EnergonAI)
                                                                   (back_to_top)
 ## Colossal-AI in the Real World ### ColossalChat
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                       chat/ColossalChat%20YouTube.png]
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                Chat-demo.png]
 [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/
 Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/
 chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/
 ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/
 @yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://www.youtube.com/
-watch?v=HcTiHzApHm0) [[tutorial]](https://www.youtube.com/watch?v=-qFBZFmOJfg)
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                        chat/ColossalChat%20Speed.jpg]
-- Up to 10 times faster for RLHF PPO Stage3 Training
+with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://
+chat.colossalai.org)
  [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
                         chatgpt/ChatGPT%20scaling.png]
 - Up to 7.73 times faster for single server training and 1.42 times faster for
 single-GPU inference
  [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
                            chatgpt/ChatGPT-1GPU.jpg]
 - Up to 10.3x growth in model capacity on one GPU - A mini demo training
@@ -221,22 +218,15 @@
 main branch. Installation can be made via ```bash pip install colossalai-
 nightly ``` ### Download From Source > The version of Colossal-AI will be in
 line with the main branch of the repository. Feel free to raise an issue if you
 encounter any problems. :) ```shell git clone https://github.com/hpcaitech/
 ColossalAI.git cd ColossalAI # install colossalai pip install . ``` By default,
 we do not compile CUDA/C++ kernels. ColossalAI will build them during runtime.
 If you want to install and enable CUDA kernel fusion (compulsory installation
-when using fused optimizer): ```shell CUDA_EXT=1 pip install . ``` For Users
-with CUDA 10.2, you can still build ColossalAI from source. However, you need
-to manually download the cub library and copy it to the corresponding
-directory. ```bash # clone the repository git clone https://github.com/
-hpcaitech/ColossalAI.git cd ColossalAI # download the cub library wget https://
-github.com/NVIDIA/cub/archive/refs/tags/1.8.0.zip unzip 1.8.0.zip cp -r cub-
-1.8.0/cub/ colossalai/kernel/cuda_native/csrc/kernels/include/ # install
-CUDA_EXT=1 pip install . ```
+when using fused optimizer): ```shell CUDA_EXT=1 pip install . ```
                                                                   (back_to_top)
 ## Use Docker ### Pull from DockerHub You can directly pull the docker image
 from our [DockerHub page](https://hub.docker.com/r/hpcaitech/colossalai). The
 image is automatically uploaded upon release. ### Build On Your Own Run the
 following command to build a docker image from Dockerfile provided. > Building
 Colossal-AI from scratch requires GPU support, you need to use Nvidia Docker
 Runtime as the default when doing `docker build`. More details can be found
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/_analyzer/_subclasses/_meta_registration.py` & `colossalai-nightly-2023.5.6/colossalai/fx/_meta_regist_12.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,42 +2,22 @@
 # should be activated for PyTorch version 1.12.0 and below
 # refer to https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/native_functions.yaml
 # for more meta_registrations
 
 from typing import Callable, List, Optional, Tuple, Union
 
 import torch
-from packaging import version
 from torch.utils._pytree import tree_map
 
 aten = torch.ops.aten
 
-try:
-    meta_lib = torch.library.Library("aten", "IMPL", "Meta")
-except AttributeError:
-    meta_lib = None
+meta_lib = torch.library.Library("aten", "IMPL", "Meta")
 
 meta_table = {}
 
-orig_empty = torch.empty
-orig_empty_strided = torch.empty_strided
-orig_empty_like = torch.empty_like
-
-
-def new(*args, **kwargs):
-    return orig_empty(*args, **kwargs, device=torch.device('meta'))
-
-
-def new_strided(*args, **kwargs):
-    return orig_empty_strided(*args, **kwargs, device=torch.device('meta'))
-
-
-def new_like(*args, **kwargs):
-    return orig_empty_like(*args, **kwargs, device=torch.device('meta'))
-
 
 def register_meta(op, register_dispatcher=True):
 
     def wrapper(f):
 
         def add_func(op):
             meta_table[op] = f
@@ -50,419 +30,477 @@
 
         tree_map(add_func, op)
         return f
 
     return wrapper
 
 
-if version.parse(torch.__version__) >= version.parse('1.12.0'):
-    # ============================== Convolutions ======================================
-    # https://github.com/pytorch/pytorch/pull/79834
-    @register_meta(aten.convolution.default)
-    def meta_conv(
-        input_tensor: torch.Tensor,
-        weight: torch.Tensor,
-        bias: torch.Tensor,
-        stride: List[int],
-        padding: List[int],
-        dilation: List[int],
-        is_transposed: bool,
-        output_padding: List[int],
-        groups: int,
+# ============================== Convolutions ======================================
+# https://github.com/pytorch/pytorch/pull/79834
+@register_meta(aten.convolution.default)
+def meta_conv(
+    input_tensor: torch.Tensor,
+    weight: torch.Tensor,
+    bias: torch.Tensor,
+    stride: List[int],
+    padding: List[int],
+    dilation: List[int],
+    is_transposed: bool,
+    output_padding: List[int],
+    groups: int,
+):
+
+    def _formula(ln: int, p: int, d: int, k: int, s: int) -> int:
+        """
+        Formula to apply to calculate the length of some dimension of the output
+        See: https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html
+        Args:
+            ln: length of the dimension
+            p: padding in that dim
+            d: dilation in that dim
+            k: kernel size in that dim
+            s: stride in that dim
+        Returns:
+            The output length
+        """
+        return (ln + 2 * p - d * (k - 1) - 1) // s + 1
+
+    def _formula_transposed(ln: int, p: int, d: int, k: int, s: int, op: int) -> int:
+        """
+        Formula to apply to calculate the length of some dimension of the output
+        if transposed convolution is used.
+        See: https://pytorch.org/docs/stable/generated/torch.nn.ConvTranspose2d.html
+        Args:
+            ln: length of the dimension
+            p: padding in that dim
+            d: dilation in that dim
+            k: kernel size in that dim
+            s: stride in that dim
+            op: output padding in that dim
+        Returns:
+            The output length
+        """
+        return (ln - 1) * s - 2 * p + d * (k - 1) + op + 1
+
+    def calc_conv_nd_return_shape(
+        dims: torch.Size,
+        kernel_size: torch.Size,
+        stride: Union[List[int], int],
+        padding: Union[List[int], int],
+        dilation: Union[List[int], int],
+        output_padding: Optional[Union[List[int], int]] = None,
     ):
+        ret_shape = []
+        if isinstance(stride, int):
+            stride = [stride] * len(dims)
+        elif len(stride) == 1:
+            stride = [stride[0]] * len(dims)
+
+        if isinstance(padding, int):
+            padding = [padding] * len(dims)
+        elif len(padding) == 1:
+            padding = [padding[0]] * len(dims)
+
+        if isinstance(dilation, int):
+            dilation = [dilation] * len(dims)
+        elif len(dilation) == 1:
+            dilation = [dilation[0]] * len(dims)
+
+        output_padding_list: Optional[List[int]] = None
+        if output_padding:
+            if isinstance(output_padding, int):
+                output_padding_list = [output_padding] * len(dims)
+            elif len(output_padding) == 1:
+                output_padding_list = [output_padding[0]] * len(dims)
+            else:
+                output_padding_list = output_padding
 
-        def _formula(ln: int, p: int, d: int, k: int, s: int) -> int:
-            """
-            Formula to apply to calculate the length of some dimension of the output
-            See: https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html
-            Args:
-                ln: length of the dimension
-                p: padding in that dim
-                d: dilation in that dim
-                k: kernel size in that dim
-                s: stride in that dim
-            Returns:
-                The output length
-            """
-            return (ln + 2 * p - d * (k - 1) - 1) // s + 1
-
-        def _formula_transposed(ln: int, p: int, d: int, k: int, s: int, op: int) -> int:
-            """
-            Formula to apply to calculate the length of some dimension of the output
-            if transposed convolution is used.
-            See: https://pytorch.org/docs/stable/generated/torch.nn.ConvTranspose2d.html
-            Args:
-                ln: length of the dimension
-                p: padding in that dim
-                d: dilation in that dim
-                k: kernel size in that dim
-                s: stride in that dim
-                op: output padding in that dim
-            Returns:
-                The output length
-            """
-            return (ln - 1) * s - 2 * p + d * (k - 1) + op + 1
-
-        def calc_conv_nd_return_shape(
-            dims: torch.Size,
-            kernel_size: torch.Size,
-            stride: Union[List[int], int],
-            padding: Union[List[int], int],
-            dilation: Union[List[int], int],
-            output_padding: Optional[Union[List[int], int]] = None,
-        ):
-            ret_shape = []
-            if isinstance(stride, int):
-                stride = [stride] * len(dims)
-            elif len(stride) == 1:
-                stride = [stride[0]] * len(dims)
-
-            if isinstance(padding, int):
-                padding = [padding] * len(dims)
-            elif len(padding) == 1:
-                padding = [padding[0]] * len(dims)
-
-            if isinstance(dilation, int):
-                dilation = [dilation] * len(dims)
-            elif len(dilation) == 1:
-                dilation = [dilation[0]] * len(dims)
-
-            output_padding_list: Optional[List[int]] = None
-            if output_padding:
-                if isinstance(output_padding, int):
-                    output_padding_list = [output_padding] * len(dims)
-                elif len(output_padding) == 1:
-                    output_padding_list = [output_padding[0]] * len(dims)
-                else:
-                    output_padding_list = output_padding
-
-            for i in range(len(dims)):
-                # If output_padding is present, we are dealing with a transposed convolution
-                if output_padding_list:
-                    ret_shape.append(
-                        _formula_transposed(
-                            dims[i],
-                            padding[i],
-                            dilation[i],
-                            kernel_size[i],
-                            stride[i],
-                            output_padding_list[i],
-                        ))
-                else:
-                    ret_shape.append(_formula(dims[i], padding[i], dilation[i], kernel_size[i], stride[i]))
-            return ret_shape
-
-        def pick_memory_format():
-            if input_tensor.is_contiguous(memory_format=torch.channels_last):
-                return torch.channels_last
-            elif input_tensor.is_contiguous(memory_format=torch.contiguous_format):
-                return torch.contiguous_format
-            elif input_tensor.is_contiguous(memory_format=torch.preserve_format):
-                return torch.preserve_format
-
-        kernel_size = weight.shape[2:]
-        dims = input_tensor.shape[2:]
-        if is_transposed:
-            out_channels = groups * weight.shape[1]
-
-            shape_out = calc_conv_nd_return_shape(
-                dims,
-                kernel_size,
-                stride,
-                padding,
-                dilation,
-                output_padding,
-            )
-
-        else:
-            out_channels = weight.shape[0]
-            if weight.shape[1] != input_tensor.shape[1] / groups:
-                raise RuntimeError("Invalid channel dimensions")
-            shape_out = calc_conv_nd_return_shape(dims, kernel_size, stride, padding, dilation)
-        out = input_tensor.new_empty((input_tensor.shape[0], out_channels, *shape_out))
-        mem_fmt = pick_memory_format()
-        out = out.to(memory_format=mem_fmt)    # type: ignore[call-overload]
-        return out
-
-    @register_meta(aten._convolution.default)
-    def meta__conv(input_tensor: torch.Tensor, weight: torch.Tensor, bias: torch.Tensor, stride: List[int],
-                   padding: List[int], dilation: List[int], is_transposed: bool, output_padding: List[int], groups: int,
-                   *extra_args):
-        out = meta_conv(input_tensor, weight, bias, stride, padding, dilation, is_transposed, output_padding, groups)
-        return out
-
-    @register_meta(aten.convolution_backward.default)
-    def meta_conv_backward(grad_output: torch.Tensor, input: torch.Tensor, weight: torch.Tensor, bias_sizes, stride,
-                           padding, dilation, transposed, output_padding, groups, output_mask):
-        return new_like(input), new_like(weight), new((bias_sizes))
-
-    # https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/AdaptiveAveragePooling.cpp
-    @register_meta(aten._adaptive_avg_pool2d_backward.default)
-    def meta_adaptive_avg_pool2d_backward(
-        grad_output: torch.Tensor,
-        input: torch.Tensor,
-    ):
-        return new_like(input)
-
-    # ================================ RNN =============================================
-    # https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/cudnn/RNN.cpp
-    @register_meta(aten._cudnn_rnn.default)
-    def meta_cuda_rnn(
-        input,
-        weight,
-        weight_stride0,
-        weight_buf,
-        hx,
-        cx,
-        mode,
-        hidden_size,
-        proj_size,
-        num_layers,
-        batch_first,
-        dropout,
-        train,
-        bidirectional,
-        batch_sizes,
-        dropout_state,
-    ):
+        for i in range(len(dims)):
+            # If output_padding is present, we are dealing with a transposed convolution
+            if output_padding_list:
+                ret_shape.append(
+                    _formula_transposed(
+                        dims[i],
+                        padding[i],
+                        dilation[i],
+                        kernel_size[i],
+                        stride[i],
+                        output_padding_list[i],
+                    ))
+            else:
+                ret_shape.append(_formula(dims[i], padding[i], dilation[i], kernel_size[i], stride[i]))
+        return ret_shape
 
-        is_input_packed = len(batch_sizes) != 0
-        if is_input_packed:
-            seq_length = len(batch_sizes)
-            mini_batch = batch_sizes[0]
-            batch_sizes_sum = input.shape[0]
+    def pick_memory_format():
+        if input_tensor.is_contiguous(memory_format=torch.channels_last):
+            return torch.channels_last
+        elif input_tensor.is_contiguous(memory_format=torch.contiguous_format):
+            return torch.contiguous_format
+        elif input_tensor.is_contiguous(memory_format=torch.preserve_format):
+            return torch.preserve_format
+
+    kernel_size = weight.shape[2:]
+    dims = input_tensor.shape[2:]
+    if is_transposed:
+        out_channels = groups * weight.shape[1]
+
+        shape_out = calc_conv_nd_return_shape(
+            dims,
+            kernel_size,
+            stride,
+            padding,
+            dilation,
+            output_padding,
+        )
+
+    else:
+        out_channels = weight.shape[0]
+        if weight.shape[1] != input_tensor.shape[1] / groups:
+            raise RuntimeError("Invalid channel dimensions")
+        shape_out = calc_conv_nd_return_shape(dims, kernel_size, stride, padding, dilation)
+    out = input_tensor.new_empty((input_tensor.shape[0], out_channels, *shape_out))
+    mem_fmt = pick_memory_format()
+    out = out.to(memory_format=mem_fmt)    # type: ignore[call-overload]
+    return out
+
+
+@register_meta(aten._convolution.default)
+def meta_conv_1(input_tensor: torch.Tensor, weight: torch.Tensor, bias: torch.Tensor, stride: List[int],
+                padding: List[int], dilation: List[int], is_transposed: bool, output_padding: List[int], groups: int,
+                *extra_args):
+    out = meta_conv(input_tensor, weight, bias, stride, padding, dilation, is_transposed, output_padding, groups)
+    return out
+
+
+@register_meta(aten.convolution_backward.default)
+def meta_conv_backward(grad_output: torch.Tensor, input: torch.Tensor, weight: torch.Tensor, bias_sizes, stride,
+                       padding, dilation, transposed, output_padding, groups, output_mask):
+    return torch.empty_like(input), torch.empty_like(weight), torch.empty((bias_sizes), device='meta')
+
+
+# https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/AdaptiveAveragePooling.cpp
+@register_meta(aten._adaptive_avg_pool2d_backward.default)
+def meta_adaptive_avg_pool2d_backward(
+    grad_output: torch.Tensor,
+    input: torch.Tensor,
+):
+    grad_input = torch.empty_like(input)
+    return grad_input
+
+
+# ================================ RNN =============================================
+# https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/cudnn/RNN.cpp
+@register_meta(aten._cudnn_rnn.default)
+def meta_cuda_rnn(
+    input,
+    weight,
+    weight_stride0,
+    weight_buf,
+    hx,
+    cx,
+    mode,
+    hidden_size,
+    proj_size,
+    num_layers,
+    batch_first,
+    dropout,
+    train,
+    bidirectional,
+    batch_sizes,
+    dropout_state,
+):
+
+    is_input_packed = len(batch_sizes) != 0
+    if is_input_packed:
+        seq_length = len(batch_sizes)
+        mini_batch = batch_sizes[0]
+        batch_sizes_sum = input.shape[0]
+    else:
+        seq_length = input.shape[1] if batch_first else input.shape[0]
+        mini_batch = input.shape[0] if batch_first else input.shape[1]
+        batch_sizes_sum = -1
+
+    num_directions = 2 if bidirectional else 1
+    out_size = proj_size if proj_size != 0 else hidden_size
+    if is_input_packed:
+        out_shape = [batch_sizes_sum, out_size * num_directions]
+    else:
+        out_shape = ([mini_batch, seq_length, out_size *
+                      num_directions] if batch_first else [seq_length, mini_batch, out_size * num_directions])
+    output = input.new_empty(out_shape)
+
+    cell_shape = [num_layers * num_directions, mini_batch, hidden_size]
+    cy = torch.empty(0) if cx is None else cx.new_empty(cell_shape)
+
+    hy = hx.new_empty([num_layers * num_directions, mini_batch, out_size])
+
+    # TODO: Query cudnnGetRNNTrainingReserveSize (expose to python)
+    reserve_shape = 0 if train else 0
+    reserve = input.new_empty(reserve_shape, dtype=torch.uint8)
+
+    return output, hy, cy, reserve, weight_buf
+
+
+# https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/cudnn/RNN.cpp
+@register_meta(aten._cudnn_rnn_backward.default)
+def meta_cudnn_rnn_backward(input: torch.Tensor,
+                            weight: torch.Tensor,
+                            weight_stride0: int,
+                            hx: torch.Tensor,
+                            cx: Optional[torch.Tensor] = None,
+                            *args,
+                            **kwargs):
+    print(input, weight, hx, cx)
+    grad_input = torch.empty_like(input)
+    grad_weight = torch.empty_like(weight)
+    grad_hx = torch.empty_like(hx)
+    grad_cx = torch.empty_like(cx) if cx is not None else torch.empty((), device='meta')
+    return grad_input, grad_weight, grad_hx, grad_cx
+
+
+# https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/Activation.cpp
+# ============================== Activations =======================================
+@register_meta(aten.relu.default)
+def meta_relu(input: torch.Tensor):
+    return torch.empty_like(input)
+
+
+@register_meta(aten.prelu.default)
+def meta_prelu(input: torch.Tensor, weight: torch.Tensor):
+    return torch.empty_like(input)
+
+
+@register_meta(aten.hardswish.default)
+def meta_hardswish(input: torch.Tensor):
+    return torch.empty_like(input)
+
+
+@register_meta(aten.hardtanh.default)
+def meta_hardtanh(input: torch.Tensor, min, max):
+    return torch.empty_like(input)
+
+
+@register_meta(aten.hardswish_backward.default)
+def meta_hardswish_backward(grad_out: torch.Tensor, input: torch.Tensor):
+    grad_in = torch.empty_like(input)
+    return grad_in
+
+
+@register_meta(aten.hardtanh_backward.default)
+def meta_hardtanh_backward(grad_out: torch.Tensor, input: torch.Tensor, min_val: int, max_val: int):
+    grad_in = torch.empty_like(input)
+    return grad_in
+
+
+# ============================== Normalization =====================================
+# https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/cudnn/BatchNorm.cpp
+@register_meta(aten.native_batch_norm.default)
+def meta_bn(input: torch.Tensor, weight, bias, running_mean, running_var, training, momentum, eps):
+    n_input = input.size(1)
+
+    output = torch.empty_like(input)
+    running_mean = torch.empty((n_input), device='meta')
+    running_var = torch.empty((n_input), device='meta')
+    return output, running_mean, running_var
+
+
+# https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/cudnn/BatchNorm.cpp
+@register_meta(aten.native_batch_norm_backward.default)
+def meta_bn_backward(dY: torch.Tensor, input: torch.Tensor, weight: torch.Tensor, running_mean, running_var, save_mean,
+                     save_invstd, train, eps, output_mask):
+    dX = torch.empty_like(input)
+    dgamma = torch.empty_like(weight)
+    dbeta = torch.empty_like(weight)
+    return dX, dgamma, dbeta
+
+
+# https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/cudnn/BatchNorm.cpp
+@register_meta(aten.cudnn_batch_norm.default)
+def meta_cudnn_bn(input: torch.Tensor, weight, bias, running_mean, running_var, training, momentum, eps):
+    n_input = input.size(1)
+
+    output = torch.empty_like(input)
+    running_mean = torch.empty((n_input), device='meta')
+    running_var = torch.empty((n_input), device='meta')
+    reserve = torch.empty((0), dtype=torch.uint8, device='meta')
+    return output, running_mean, running_var, reserve
+
+
+# https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/cudnn/BatchNorm.cpp
+# NB: CuDNN only implements the backward algorithm for batchnorm
+# in training mode (evaluation mode batchnorm has a different algorithm),
+# which is why this doesn't accept a 'training' parameter.
+@register_meta(aten.cudnn_batch_norm_backward.default)
+def meta_cudnn_bn_backward(dY: torch.Tensor, input: torch.Tensor, weight: torch.Tensor, running_mean, running_var,
+                           save_mean, save_invstd, eps, reserve):
+    dX = torch.empty_like(input)
+    dgamma = torch.empty_like(weight)
+    dbeta = torch.empty_like(weight)
+    return dX, dgamma, dbeta
+
+
+# https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/layer_norm.cpp
+@register_meta(aten.native_layer_norm.default)
+def meta_ln(input: torch.Tensor, normalized_shape, weight, bias, eps):
+    bs = input.size(0)
+    n_input = input.size(1)
+
+    output = torch.empty_like(input)
+    running_mean = torch.empty((bs, n_input, 1), device='meta')
+    running_var = torch.empty((bs, n_input, 1), device='meta')
+    return output, running_mean, running_var
+
+
+# https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/layer_norm.cpp
+@register_meta(aten.native_layer_norm_backward.default)
+def meta_ln_backward(dY: torch.Tensor, input: torch.Tensor, normalized_shape, mean, rstd, weight, bias,
+                     grad_input_mask):
+    dX = torch.empty_like(input)
+    dgamma = torch.empty_like(weight)
+    dbeta = torch.empty_like(bias)
+    return dX, dgamma, dbeta
+
+
+# https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/group_norm.cpp
+@register_meta(aten.native_group_norm_backward.default)
+def meta_gn_backward(dY: torch.Tensor, input: torch.Tensor, mean, rstd, gamma, N, C, HxW, group, grad_input_mask):
+    dX = torch.empty_like(input)
+    dgamma = torch.empty_like(gamma)
+    dbeta = torch.empty_like(gamma)
+    return dX, dgamma, dbeta
+
+
+# ================================== Misc ==========================================
+# https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/native_functions.yaml
+@register_meta(aten.roll.default)
+def meta_roll(input: torch.Tensor, shifts, dims):
+    return input
+
+
+# https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/Scalar.cpp
+@register_meta(aten._local_scalar_dense.default)
+def meta_local_scalar_dense(self: torch.Tensor):
+    return 0
+
+
+# https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/TensorCompare.cpp
+@register_meta(aten.where.self)
+def meta_where_self(condition: torch.Tensor, self: torch.Tensor, other: torch.Tensor):
+    result_type = torch.result_type(self, other)
+    return torch.empty_like(condition + self + other, dtype=result_type)
+
+
+@register_meta(aten.index.Tensor)
+def meta_index_Tensor(self, indices):
+    assert indices, "at least one index must be provided"
+    # aten::index is the internal advanced indexing implementation
+    # checkIndexTensorTypes and expandTensors
+    result: List[Optional[torch.Tensor]] = []
+    for i, index in enumerate(indices):
+        if index is not None:
+            assert index.dtype in [torch.long, torch.int8, torch.bool],\
+                "tensors used as indices must be long, byte or bool tensors"
+            if index.dtype in [torch.int8, torch.bool]:
+                nonzero = index.nonzero()
+                k = len(result)
+                assert k + index.ndim <= self.ndim, f"too many indices for tensor of dimension {self.ndim}"
+                for j in range(index.ndim):
+                    assert index.shape[j] == self.shape[
+                        k +
+                        j], f"The shape of the mask {index.shape} at index {i} does not match the shape of the indexed tensor {self.shape} at index {k + j}"
+                    result.append(nonzero.select(1, j))
+            else:
+                result.append(index)
         else:
-            seq_length = input.shape[1] if batch_first else input.shape[0]
-            mini_batch = input.shape[0] if batch_first else input.shape[1]
-            batch_sizes_sum = -1
-
-        num_directions = 2 if bidirectional else 1
-        out_size = proj_size if proj_size != 0 else hidden_size
-        if is_input_packed:
-            out_shape = [batch_sizes_sum, out_size * num_directions]
+            result.append(index)
+    indices = result
+    assert len(indices) <= self.ndim, f"too many indices for tensor of dimension {self.ndim} (got {len(indices)})"
+    # expand_outplace
+    import torch._refs as refs
+
+    indices = list(refs._maybe_broadcast(*indices))
+    # add missing null tensors
+    while len(indices) < self.ndim:
+        indices.append(None)
+
+    # hasContiguousSubspace
+    #   true if all non-null tensors are adjacent
+    # See:
+    # https://numpy.org/doc/stable/user/basics.indexing.html#combining-advanced-and-basic-indexing
+    # https://stackoverflow.com/questions/53841497/why-does-numpy-mixed-basic-advanced-indexing-depend-on-slice-adjacency
+    state = 0
+    has_contiguous_subspace = False
+    for index in indices:
+        if state == 0:
+            if index is not None:
+                state = 1
+        elif state == 1:
+            if index is None:
+                state = 2
         else:
-            out_shape = ([mini_batch, seq_length, out_size *
-                          num_directions] if batch_first else [seq_length, mini_batch, out_size * num_directions])
-        output = input.new_empty(out_shape)
-
-        cell_shape = [num_layers * num_directions, mini_batch, hidden_size]
-        cy = new(0) if cx is None else cx.new_empty(cell_shape)
-
-        hy = hx.new_empty([num_layers * num_directions, mini_batch, out_size])
-
-        # TODO: Query cudnnGetRNNTrainingReserveSize (expose to python)
-        reserve_shape = 0 if train else 0
-        reserve = input.new_empty(reserve_shape, dtype=torch.uint8)
-
-        return output, hy, cy, reserve, weight_buf
-
-    # https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/cudnn/RNN.cpp
-    @register_meta(aten._cudnn_rnn_backward.default)
-    def meta_cudnn_rnn_backward(input: torch.Tensor,
-                                weight: torch.Tensor,
-                                weight_stride0: int,
-                                hx: torch.Tensor,
-                                cx: Optional[torch.Tensor] = None,
-                                *args,
-                                **kwargs):
-        return new_like(input), new_like(weight), new_like(hx), new_like(cx) if cx is not None else new(
-            ())    # (grad_input, grad_weight, grad_hx, grad_cx)
-
-    # https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/Activation.cpp
-    # ============================== Activations =======================================
-    _unregistered_ewise = [
-        aten.relu.default,
-        aten.prelu.default,
-        aten.hardswish.default,
-        aten.hardtanh.default,
-        aten.hardswish_backward.default,
-        aten.hardtanh_backward.default,
-    ]
-
-    if version.parse(torch.__version__) < version.parse('2.0.0'):
-        _unregistered_ewise += [
-            aten.prelu_backward.default,
-        ]
-
-    @register_meta(_unregistered_ewise)
-    def meta_unregistered_ewise(input: torch.Tensor, *args):
-        return new_like(input)
-
-    # ============================== Normalization =====================================
-    # https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/cudnn/BatchNorm.cpp
-    @register_meta(aten.native_batch_norm.default)
-    def meta_bn(input: torch.Tensor, weight, bias, running_mean, running_var, training, momentum, eps):
-        n_input = input.size(1)
-        return new_like(input), new((n_input)), new((n_input))
-
-    # https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/cudnn/BatchNorm.cpp
-    @register_meta(aten.native_batch_norm_backward.default)
-    def meta_bn_backward(dY: torch.Tensor, input: torch.Tensor, weight: torch.Tensor, running_mean, running_var,
-                         save_mean, save_invstd, train, eps, output_mask):
-        return new_like(input), new_like(weight), new_like(weight)    # (dX, dgamma, dbeta)
-
-    # https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/cudnn/BatchNorm.cpp
-    @register_meta(aten.cudnn_batch_norm.default)
-    def meta_cudnn_bn(input: torch.Tensor, weight, bias, running_mean, running_var, training, momentum, eps):
-        n_input = input.size(1)
-        return new_like(input), new((n_input)), new((n_input)), new(
-            (0), dtype=torch.uint8)    # (output, running_mean, running_var, reserve)
-
-    # https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/cudnn/BatchNorm.cpp
-    # NB: CuDNN only implements the backward algorithm for batchnorm
-    # in training mode (evaluation mode batchnorm has a different algorithm),
-    # which is why this doesn't accept a 'training' parameter.
-    @register_meta(aten.cudnn_batch_norm_backward.default)
-    def meta_cudnn_bn_backward(dY: torch.Tensor, input: torch.Tensor, weight: torch.Tensor, running_mean, running_var,
-                               save_mean, save_invstd, eps, reserve):
-        return new_like(input), new_like(weight), new_like(weight)    # (dX, dgamma, dbeta)
-
-    # https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/layer_norm.cpp
-    @register_meta(aten.native_layer_norm.default)
-    def meta_ln(input: torch.Tensor, normalized_shape, weight, bias, eps):
-        bs, n_input = input.size(0), input.size(1)
-        return new_like(input), new((bs, n_input, 1)), new((bs, n_input, 1))    # (output, running_mean, running_var)
-
-    # https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/layer_norm.cpp
-    @register_meta(aten.native_layer_norm_backward.default)
-    def meta_ln_backward(dY: torch.Tensor, input: torch.Tensor, normalized_shape, mean, rstd, weight, bias,
-                         grad_input_mask):
-        return new_like(input), new_like(weight), new_like(bias)    # (dX, dgamma, dbeta)
-
-    # ================================== Misc ==========================================
-    # Maybe incorrect
-    # https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/Im2Col.cpp
-    @register_meta(aten.im2col.default)
-    def meta_im2col(input: torch.Tensor, kernel_size, dilation, padding, stride):
-        return new_like(input)
-
-    # https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/native_functions.yaml
-    @register_meta(aten.roll.default)
-    def meta_roll(input: torch.Tensor, shifts, dims):
-        return input
-
-    # https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/Scalar.cpp
-    @register_meta(aten._local_scalar_dense.default)
-    def meta_local_scalar_dense(self: torch.Tensor):
-        return 0
-
-    # https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/TensorCompare.cpp
-    @register_meta(aten.where.self)
-    def meta_where_self(condition: torch.Tensor, self: torch.Tensor, other: torch.Tensor):
-        result_type = torch.result_type(self, other)
-        return new_like(condition + self + other, dtype=result_type)
-
-    # ============================== Embedding =========================================
-    # https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/Embedding.cpp
-
-    @register_meta(aten.embedding_dense_backward.default)
-    def meta_embedding_dense_backward(grad_output: torch.Tensor, indices: torch.Tensor, num_weights, padding_idx,
-                                      scale_grad_by_freq):
-        return new((num_weights, grad_output.size(-1)), dtype=grad_output.dtype, layout=grad_output.layout)
-
-    # ============================== Dropout ===========================================
-    # https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/Dropout.cpp
-    @register_meta(aten.native_dropout.default)
-    def meta_native_dropout_default(input: torch.Tensor, p: float, train: bool = False):
-        # notice that mask is bool
-        return new_like(input), new_like(input, dtype=torch.bool)    # (output, mask)
-
-    # https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/Dropout.cpp
-    @register_meta(aten.native_dropout_backward.default)
-    def meta_native_dropout_backward_default(grad: torch.Tensor, mask: torch.Tensor, scale: float):
-        return new_like(grad)    # (grad_in)
-
-    if version.parse(torch.__version__) < version.parse('1.13.0'):
-        # https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/native_functions.yaml
-        @register_meta(aten.eye.m_out)
-        def meta_eye(n: int, m: int, out: torch.Tensor):
-            return out
-
-        @register_meta(aten.index.Tensor)
-        def meta_index_Tensor(self, indices):
-            assert indices, "at least one index must be provided"
-            # aten::index is the internal advanced indexing implementation
-            # checkIndexTensorTypes and expandTensors
-            result: List[Optional[torch.Tensor]] = []
-            for i, index in enumerate(indices):
-                if index is not None:
-                    assert index.dtype in [torch.long, torch.int8, torch.bool],\
-                        "tensors used as indices must be long, byte or bool tensors"
-                    if index.dtype in [torch.int8, torch.bool]:
-                        nonzero = index.nonzero()
-                        k = len(result)
-                        assert k + index.ndim <= self.ndim, f"too many indices for tensor of dimension {self.ndim}"
-                        for j in range(index.ndim):
-                            assert index.shape[j] == self.shape[
-                                k +
-                                j], f"The shape of the mask {index.shape} at index {i} does not match the shape of the indexed tensor {self.shape} at index {k + j}"
-                            result.append(nonzero.select(1, j))
-                    else:
-                        result.append(index)
-                else:
-                    result.append(index)
-            indices = result
-            assert len(
-                indices) <= self.ndim, f"too many indices for tensor of dimension {self.ndim} (got {len(indices)})"
-            # expand_outplace
-            import torch._refs as refs
-
-            indices = list(refs._maybe_broadcast(*indices))
-            # add missing null tensors
-            while len(indices) < self.ndim:
-                indices.append(None)
-
-            # hasContiguousSubspace
-            #   true if all non-null tensors are adjacent
-            # See:
-            # https://numpy.org/doc/stable/user/basics.indexing.html#combining-advanced-and-basic-indexing
-            # https://stackoverflow.com/questions/53841497/why-does-numpy-mixed-basic-advanced-indexing-depend-on-slice-adjacency
-            state = 0
-            has_contiguous_subspace = False
-            for index in indices:
-                if state == 0:
-                    if index is not None:
-                        state = 1
-                elif state == 1:
-                    if index is None:
-                        state = 2
-                else:
-                    if index is not None:
-                        break
+            if index is not None:
+                break
+    else:
+        has_contiguous_subspace = True
+
+    # transposeToFront
+    # This is the logic that causes the newly inserted dimensions to show up
+    # at the beginning of the tensor, if they're not contiguous
+    if not has_contiguous_subspace:
+        dims = []
+        transposed_indices = []
+        for i, index in enumerate(indices):
+            if index is not None:
+                dims.append(i)
+                transposed_indices.append(index)
+        for i, index in enumerate(indices):
+            if index is None:
+                dims.append(i)
+                transposed_indices.append(index)
+        self = self.permute(dims)
+        indices = transposed_indices
+
+    # AdvancedIndex::AdvancedIndex
+    # Now we can assume the indices have contiguous subspace
+    # This is simplified from AdvancedIndex which goes to more effort
+    # to put the input and indices in a form so that TensorIterator can
+    # take them.  If we write a ref for this, probably that logic should
+    # get implemented
+    before_shape: List[int] = []
+    after_shape: List[int] = []
+    replacement_shape: List[int] = []
+    for dim, index in enumerate(indices):
+        if index is None:
+            if replacement_shape:
+                after_shape.append(self.shape[dim])
             else:
-                has_contiguous_subspace = True
+                before_shape.append(self.shape[dim])
+        else:
+            replacement_shape = list(index.shape)
+    return self.new_empty(before_shape + replacement_shape + after_shape)
+
 
-            # transposeToFront
-            # This is the logic that causes the newly inserted dimensions to show up
-            # at the beginning of the tensor, if they're not contiguous
-            if not has_contiguous_subspace:
-                dims = []
-                transposed_indices = []
-                for i, index in enumerate(indices):
-                    if index is not None:
-                        dims.append(i)
-                        transposed_indices.append(index)
-                for i, index in enumerate(indices):
-                    if index is None:
-                        dims.append(i)
-                        transposed_indices.append(index)
-                self = self.permute(dims)
-                indices = transposed_indices
-
-            # AdvancedIndex::AdvancedIndex
-            # Now we can assume the indices have contiguous subspace
-            # This is simplified from AdvancedIndex which goes to more effort
-            # to put the input and indices in a form so that TensorIterator can
-            # take them.  If we write a ref for this, probably that logic should
-            # get implemented
-            before_shape: List[int] = []
-            after_shape: List[int] = []
-            replacement_shape: List[int] = []
-            for dim, index in enumerate(indices):
-                if index is None:
-                    if replacement_shape:
-                        after_shape.append(self.shape[dim])
-                    else:
-                        before_shape.append(self.shape[dim])
-                else:
-                    replacement_shape = list(index.shape)
-            return self.new_empty(before_shape + replacement_shape + after_shape)
+# ============================== Embedding =========================================
+# https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/Embedding.cpp
+@register_meta(aten.embedding_dense_backward.default)
+def meta_embedding_dense_backward(grad_output: torch.Tensor, indices: torch.Tensor, num_weights, padding_idx,
+                                  scale_grad_by_freq):
+    return torch.empty((num_weights, grad_output.size(-1)),
+                       dtype=grad_output.dtype,
+                       device=grad_output.device,
+                       layout=grad_output.layout)
+
+
+# ============================== Dropout ===========================================
+# https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/Dropout.cpp
+@register_meta(aten.native_dropout.default)
+def meta_native_dropout_default(input: torch.Tensor, p: float, train: bool = False):
+    # notice that mask is bool
+    output = torch.empty_like(input)
+    mask = torch.empty_like(input, dtype=torch.bool)
+    return output, mask
+
+
+# https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/Dropout.cpp
+@register_meta(aten.native_dropout_backward.default)
+def meta_native_dropout_backward_default(grad: torch.Tensor, mask: torch.Tensor, scale: float):
+    return torch.empty_like(grad)
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/_analyzer/_subclasses/meta_tensor.py` & `colossalai-nightly-2023.5.6/colossalai/utils/model/lazy_init_context.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,207 +1,242 @@
-import uuid
-from functools import partial
+#!/usr/bin/env python
+# coding: utf-8
 
-import torch
-import torch.distributed as dist
-from torch.types import _bool, _device, _dtype
-from torch.utils._pytree import tree_flatten, tree_map
+import inspect
+import types
+from typing import Callable, List
 
-from ._monkey_patch import _AliasATen, _DistCommMethod, _InplaceATen, _MaybeInplaceATen, _TorchOverrideableFactoryMethod
+import torch
+import torch.nn as nn
 
-__all__ = ['MetaTensor', 'MetaTensorMode']
+from colossalai.tensor import ColoParameter, ColoTensor
+from colossalai.utils.model.utils import substitute_init_recursively
 
 
-def register_storage(r, data_ptr_fn=None):
-    if isinstance(r, torch.Tensor):
-        if data_ptr_fn is not None:
-            r.data_ptr = data_ptr_fn
-        elif not r.data_ptr():
-            data_ptr = uuid.uuid1()
-            r.data_ptr = lambda: data_ptr
+class LazyInitContext():
+    """
+    A context to allow for lazy weight initialization of PyTorch modules. It intercepts the tensor
+    initialization functions for lazy initialization
 
+    Note:
+        This API is only experimental and subject to future changes.
 
-def _normalize_tuple(x):
-    if not isinstance(x, tuple):
-        return (x,)
-    return x
+    Usage:
+        with LazyInitContext() as ctx:
+            model = nn.Linear(10, 10)
+            model.weight.zero_()
+
+        # make sure the weight is a meta tensor
+        assert model.weight.is_meta
+
+        # initialize weights
+        ctx.lazy_init_parameters(model)
+
+        # make sure the weight is not a meta tensor
+        # and initialized correctly
+        assert not model.weight.is_meta and torch.all(model.weight == 0)
+
+    Args:
+        to_meta (bool): optional, whether to initialize the model with meta tensors, default is True. This
+            argument exists for now because some corner cases such as self.weight = torch.zeros(...) cannot be captured yet.
+        extra_torch_tensor_func (List[str]): extra torch tensor functions related
+            to value setting, such as `zero_` and `triu_`. `zero_` is pre-added by default.
+    """
 
+    tensor_set_value_func = ['zero_', 'fill_']
 
-# a hack of inplace execution in PyTorch
-def _assert_alias(func):
-    return func in (_AliasATen + _InplaceATen + _MaybeInplaceATen    # TODO: check if should be this aggressive
-                   )
+    def __init__(self, to_meta: bool = True, extra_torch_tensor_func: List[str] = None):
+        # TODO: hijack the torch constructor functions as well
+        self._to_meta = to_meta
+        self._intercepted_nn_init_func_cache = {}
+        self._nn_init_methods = self._get_nn_init_methods()
+        self._torch_mod_cls = torch.nn.modules.module.Module
+
+        if extra_torch_tensor_func:
+            # use tuple to remove duplicates
+            self._torch_tensor_funcs = tuple(self.tensor_set_value_func + extra_torch_tensor_func)
+        else:
+            self._torch_tensor_funcs = self.tensor_set_value_func
+
+    @property
+    def to_meta(self):
+        return self._to_meta
 
+    def _cache_init_func(self, func):
+        """
+        This method wraps the ``torch.nn.init`` method and torch tensor value-setting functions
+        so that the function call is cached instead of being executed.
+        """
 
-class MetaTensor(torch.Tensor):
-    """
-    A wrapping tensor that hacks ``torch.autograd`` without patching more ``torch.ops.aten`` ops.
-    `device` is the device that ``MetaTensor`` is supposed to run on. Meta tensors give you the
-    ability to run PyTorch code without having to actually do computation through tensors
-    allocated on a `meta` device. Because the device is `meta`, meta tensors do not model
-    device propagation. ``MetaTensor`` extends its usage by carrying an additional `device`
-    which tracks devices that would have been used.
+        def wrapped_init_func(tensor, *args, **kwargs):
+            if tensor not in self._intercepted_nn_init_func_cache:
+                self._intercepted_nn_init_func_cache[tensor] = []
+            self._intercepted_nn_init_func_cache[tensor].append((func, args, kwargs))
 
-    Reference:
-        https://github.com/pytorch/pytorch/blob/master/torch/_subclasses/fake_tensor.py
-    """
+        return wrapped_init_func
 
-    _tensor: torch.Tensor
+    def _get_nn_init_methods(self):
+        """
+        This method looks for all available functions in the ``torch.nn.init``
+        module.
+        """
+        nn_init_method_names = dir(torch.nn.init)
+        nn_init_methods = []
 
-    @staticmethod
-    def __new__(cls, elem, device=None, data_ptr_fn=None):
-        requires_grad = elem.requires_grad
-        # Avoid multiple wrapping
-        while isinstance(elem, MetaTensor):
-            device = elem.device if device is None else device
-            elem = elem._tensor
-
-        # The wrapping tensor (MetaTensor) shouldn't hold any
-        # memory for the class in question, but it should still
-        # advertise the same device as before
-        r = torch.Tensor._make_wrapper_subclass(
-            cls,
-            elem.size(),
-            strides=elem.stride(),
-            storage_offset=elem.storage_offset(),
-            dtype=elem.dtype,
-            layout=elem.layout,
-            device=device or (elem.device if elem.device.type != 'meta' else torch.device('cpu')),
-            requires_grad=requires_grad)    # deceive the frontend for aten selections
-        r._tensor = elem
-        # ...the real tensor is held as an element on the tensor.
-        if not r._tensor.is_meta:
-            val = elem.data_ptr()
-            data_ptr_fn = lambda: val
-            r._tensor = r._tensor.to(torch.device('meta'))
-
-        # only tensor not on `meta` should be copied to `meta`
-        register_storage(r._tensor, data_ptr_fn)
-        if isinstance(elem, torch.nn.Parameter):
-            r = torch.nn.Parameter(r)
-        return r
-
-    def __repr__(self):
-        name = 'MetaParameter' if getattr(self, '_is_param', False) else 'MetaTensor'
-        if self.grad_fn:
-            return f"{name}(..., size={tuple(self.shape)}, device='{self.device}', dtype={self.dtype}, grad_fn={self.grad_fn})"
-        return f"{name}(..., size={tuple(self.shape)}, device='{self.device}', dtype={self.dtype})"
-
-    @classmethod
-    def __torch_dispatch__(cls, func, types, args=(), kwargs=None):
-        device = None
-
-        def unwrap(x):
-            nonlocal device
-            if isinstance(x, MetaTensor):
-                device = x.device
-                x = x._tensor
-            elif isinstance(x, torch.Tensor):
-                device = x.device
-                x = x.to(torch.device('meta'))
-            return x
-
-        args = tree_map(unwrap, args)
-        kwargs = tree_map(unwrap, kwargs)
-
-        if 'device' in kwargs:
-            device = kwargs['device']
-            kwargs['device'] = torch.device('meta')
-
-        # run aten for backend=CPU but actually on backend=Meta
-        # here we detect whether or not the execution generates a physical copy
-        # of the input tensor
-        ret = func(*args, **kwargs)
-
-        if _assert_alias(func):
-            val = args[0].data_ptr()
-            tree_map(partial(register_storage, data_ptr_fn=lambda: val), _normalize_tuple(ret))
-
-        # Now, we want to continue propagating this tensor, so we rewrap Tensors in
-        # our custom tensor subclass
-        def wrap(x):
-            return MetaTensor(x, device=device) if isinstance(x, torch.Tensor) else x
-
-        return tree_map(wrap, ret)
-
-    def to(self, *args, **kwargs) -> torch.Tensor:
-        """An extension of `torch.Tensor.to()` to MetaTensor
-        Returns:
-            result (MetaTensor): MetaTensor
-        Usage:
-            >>> tensor = MetaTensor(torch.rand(10), device='cuda:100')
-            >>> tensor.to(torch.uint8)
-            MetaTensor(tensor(..., device='meta', size=(10,), dtype=torch.uint8), device='cuda:100')
-            >>> tensor.to(torch.device('cuda:42'))
-            MetaTensor(tensor(..., device='meta', size=(10,)), device='cuda:42')
-            >>> tensor.to('vulkan')
-            MetaTensor(tensor(..., device='meta', size=(10,)), device='vulkan')
-        """
-        # this imitates c++ function in the way of @overload
-        device = None
-
-        def replace(x):
-            nonlocal device
-            if isinstance(x, str) or isinstance(x, _device):
-                device = x
-                return torch.device('meta')
-            return x
-
-        elem = self._tensor.to(*tree_map(replace, args), **tree_map(replace, kwargs))
-        return MetaTensor(elem, device=device)
-
-    def cpu(self, *args, **kwargs):
-        if self.device.type == 'cpu':
-            return self.to(*args, **kwargs)
-        return self.to(*args, device='cpu', **kwargs)
-
-    def cuda(self, device=None, non_blocking=False):
-        if device is not None:
-            return self.to(device=device, non_blocking=non_blocking)
-        return self.to(device='cuda:0', non_blocking=non_blocking)
+        # look for all methods in ``torch.nn.init`` module
+        for name in nn_init_method_names:
+            nn_init_methods.append((name, getattr(torch.nn.init, name)))
+
+        def _is_init_method(item):
+            name, func = item
+
+            if (not isinstance(func, types.FunctionType) or name.startswith('_') or not name.endswith('_')):
+                return False
+            else:
+                return True
+
+        # remove methods which are not init functions
+        nn_init_methods = list(filter(_is_init_method, nn_init_methods))
+        return nn_init_methods
 
-    def data_ptr(self):
-        return self._tensor.data_ptr()
+    def _wrap_module_init(self, func):
+        """
+        This method wraps the calls to the `__init__` of ``torch.nn.Module`` and replaces
+        the argument device with value 'meta' so that all modules are created as meta tensors.
+        """
+        has_device = 'device' in inspect.signature(func).parameters
 
+        def layer_lazy_init(module, *args, **kwargs):
+            # if this module contains device argument
+            # we set it to meta to initialize as meta backend
+            if has_device:
+                kwargs['device'] = 'meta'
+            func(module, *args, **kwargs)
+
+            # if device is not found, we intialize it and convert to meta
+            if not has_device:
+                module.to('meta')
 
-class MetaTensorMode(object):
-    """
-    A context manager that enables MetaTensor mode.
+        return layer_lazy_init
 
-    Usage:
-        >>> with MetaTensorMode():
-        >>>     # all torch.xxx and torch.distributed.xxx will be replaced by patched functions
-        >>>     # and the actual execution will be on torch.device('meta')
-        >>>     a = torch.rand(100000, 100000)
-        >>>     b = torch.rand(100000, 100000)
-        >>>     c = torch.mm(a, b)
-    """
+    def _get_tmp_origin_func_ref(self, name):
+        """
+        Generate a function name for consistency during caching and retrieving.
+        """
+        return f'_orig_{name}'
 
-    def __init__(self):
-        self.torch_overrides = {}    # override torch.xxx
-        self.dist_overrides = {}    # override torch.distributed.xxx
+    def _patch_nn_init_funcs(self):
+        # patch nn.init functions
+        for name, func in self._nn_init_methods:
+            setattr(torch.nn.init, name, self._cache_init_func(func))
+
+    def _unpatch_nn_init_funcs(self):
+        # unpatch nn.init functions
+        for name, func in self._nn_init_methods:
+            setattr(torch.nn.init, name, func)
+
+    def _patch_submodule_init(self):
+        # patch classes __init__ methods
+        def _activate_wrap_init(cls):
+            cls.__orig_init__ = cls.__init__
+            cls.__init__ = self._wrap_module_init(cls.__init__)
+
+        substitute_init_recursively(self._torch_mod_cls, _activate_wrap_init, set())
+
+    def _unpatch_submodule_init(self):
+
+        def _recover_orig_init(cls):
+            cls.__init__ = cls.__orig_init__
+
+        substitute_init_recursively(self._torch_mod_cls, _recover_orig_init, set())
+
+    def _patch_torch_tensor_funcs(self):
+        # patch tensor value-setting functions
+        for func_name in self._torch_tensor_funcs:
+            origin_func_name = self._get_tmp_origin_func_ref(func_name)
+            origin_func = getattr(torch.Tensor, func_name)
+            setattr(torch.Tensor, origin_func_name, origin_func)
+            setattr(torch.Tensor, func_name, self._cache_init_func(origin_func))
+
+    def _unpatch_torch_tensor_funcs(self):
+        for func_name in self._torch_tensor_funcs:
+            origin_func_name = self._get_tmp_origin_func_ref(func_name)
+            origin_func = getattr(torch.Tensor, origin_func_name)
+            setattr(torch.Tensor, func_name, origin_func)
 
     def __enter__(self):
+        self._patch_torch_tensor_funcs()
+        self._patch_nn_init_funcs()
+
+        if self._to_meta:
+            self._patch_submodule_init()
+        return self
+
+    def __exit__(self, *args, **kwargs):
+        if self._to_meta:
+            self._unpatch_submodule_init()
+        self._unpatch_nn_init_funcs()
+        self._unpatch_torch_tensor_funcs()
+
+    def lazy_init_parameters(self, model: torch.nn.Module, device='cpu'):
+        """
+        Initialize the weights of the meta-tensor model.
+
+        Args:
+            model (`torch.nn.Module`): the model instantiated under the context.
+            device (str): the device on which weights are initialized
+
+        """
 
-        def _dummy(*args, **kwargs):
-            pass
+        def _init_recursively(module: nn.Module):
+            # recursively initialize the module
+            for mod in module.children():
+                _init_recursively(mod)
+
+            # initialize and shard tensors directly attached to the current module
+            for name, param in module.named_parameters(recurse=False):
+                _init_and_shard(module, name, param)
+
+            for name, buf in module.named_buffers(recurse=False):
+                _init_and_shard(module, name, buf)
+
+        @torch.no_grad()
+        def _init_and_shard(module, name, tensor):
+            # check whether the tensor is a buffer or parameter
+            is_param = isinstance(tensor, nn.parameter.Parameter)
+
+            # get sharding spec
+            dist_spec = getattr(tensor, 'dist_spec', None)
+            pg = getattr(tensor, 'pg', None)
+            comp_spec = getattr(tensor, 'comp_spec', None)
+
+            # convert the tensor from meta to materialized one
+            if tensor.is_meta:
+                materialized_tensor = torch.empty_like(tensor, device=device)
+                # if this tensor is a meta tensor, it must have an init function
+                assert tensor in self._intercepted_nn_init_func_cache
+            else:
+                materialized_tensor = tensor
+
+            # apply init function
+            if tensor in self._intercepted_nn_init_func_cache:
+                init_func, args, kwargs = self._intercepted_nn_init_func_cache[tensor][-1]
+                init_func(materialized_tensor, *args, **kwargs)
+
+            # convert it to ColoTensor or ColoParameter
+            if is_param:
+                tensor = ColoParameter.from_torch_tensor(materialized_tensor, requires_grad=tensor.requires_grad)
+            else:
+                tensor = ColoTensor.from_torch_tensor(materialized_tensor)
+
+            # override the original tensor
+            with torch.no_grad():
+                setattr(module, name, tensor)
+
+            # apply sharding
+            if dist_spec:
+                tensor.process_group = pg
+                tensor.set_tensor_spec(dist_spec, comp_spec)
 
-        def _new(*args, orig_new=torch.empty, **kwargs):
-            return MetaTensor(orig_new(*args, **{
-                **kwargs, 'device': 'meta'
-            }),
-                              device=kwargs.get('device', torch.device('cpu')))
-
-        for func in _TorchOverrideableFactoryMethod:
-            self.torch_overrides[func] = getattr(torch, func)
-            setattr(torch, func, partial(_new, orig_new=getattr(torch, func)))
-
-        for func in _DistCommMethod:
-            self.dist_overrides[func] = getattr(dist, func)
-            setattr(dist, func, _dummy)
-
-    def __exit__(self, exc_type, exc_value, traceback):
-        for func, func_impl in self.torch_overrides.items():
-            setattr(torch, func, func_impl)
+        _init_recursively(model)
 
-        for func, func_impl in self.dist_overrides.items():
-            setattr(dist, func, func_impl)
+        return model
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/codegen.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,459 +1,439 @@
-from typing import Any, Callable, Dict, Iterable, List, Tuple
+from copy import deepcopy
+from typing import Any, Dict, List, Tuple
 
-import torch
+from torch import Tensor
+from torch.fx import Graph, Node
 
-try:
-    from torch.fx.graph import CodeGen
-except:
-    pass
-from torch.fx.graph import (
-    PythonCode,
-    _custom_builtins,
-    _format_target,
-    _is_from_torch,
-    _Namespace,
-    _origin_type_map,
-    _register_custom_builtin,
-    inplace_methods,
-    magic_methods,
+from colossalai.auto_parallel.passes.runtime_apply_pass import runtime_apply, runtime_comm_spec_apply
+from colossalai.fx.codegen.activation_checkpoint_codegen import _find_nested_ckpt_regions
+from colossalai.fx.profiler import (
+    activation_size,
+    calculate_bwd_time,
+    calculate_fwd_out,
+    calculate_fwd_time,
+    calculate_fwd_tmp,
 )
-from torch.fx.node import Argument, Node, _get_qualified_name, _type_repr, map_arg
+from colossalai.logging import get_dist_logger
 
-import colossalai
-from colossalai.fx._compatibility import compatibility
+from .ckpt_solver_base import CheckpointSolverBase
+from .operation import Backward, Chain, ForwardCheck, ForwardEnable, ForwardNograd, Loss, Sequence
 
-_register_custom_builtin('colossalai', 'import colossalai', colossalai)
+__all__ = ['CheckpointSolverRotor']
 
 
-def _gen_ckpt_fn_def(label, free_vars: List[str]) -> str:
-    """
-    Generate the checkpoint function definition
-    """
-    return f"def checkpoint_{label}({', '.join(['self'] + free_vars)}):"
-
-
-def _gen_ckpt_output(output_vars: List[str]) -> str:
-    """
-    Generate the return statement for checkpoint region
-    """
-    return f"return {', '.join(output_vars)}"
-
-
-def _gen_ckpt_usage(label, input_vars, output_vars, use_reentrant=True):
-    """
-    Generate the checkpoint function call code text
-    """
-    outputs = ', '.join(output_vars)
-    inputs = ', '.join(input_vars)
-    return f'{outputs} = torch.utils.checkpoint.checkpoint(self.checkpoint_{label}, {inputs}, use_reentrant={use_reentrant})'
-
-
-def _end_of_ckpt(node: Node, ckpt_level: int) -> bool:
-    """
-    Check if the node could end the ckpt region at `ckpt_level`
-    """
-    if len(node.meta['info'].activation_checkpoint) > ckpt_level:
-        return node.meta['info'].activation_checkpoint[ckpt_level] is not None
-    return True
-
-
-def _find_input_and_output_nodes(nodes: List[Node]):
-    """
-    Find the input and output node names which are not found in the given list of nodes.
-    """
-    input_nodes = []
-    output_nodes = []
-
-    # if a node has an input node which is not in the node list
-    # we treat that input node as the input of the checkpoint function
-    for node in nodes:
-        for input_node in node._input_nodes.keys():
-            node_repr = repr(input_node)
-            if input_node not in nodes and node_repr not in input_nodes:
-                input_nodes.append(node_repr)
-
-    # if a node has a user node which is not in the node list
-    # we treat that user node as the node receiving the current node output
-    for node in nodes:
-        for output_node in node.users.keys():
-            node_repr = repr(node)
-            if output_node not in nodes and node_repr not in output_nodes:
-                output_nodes.append(node_repr)
-
-    return input_nodes, output_nodes
-
-
-def _find_nested_ckpt_regions(node_list: List[Node], ckpt_level: int = 0):
-    """
-    Find the nested checkpoint regions given a list of consecutive nodes. The outputs
-    will be list of tuples, each tuple is in the form of (start_index, end_index).
-    """
-    ckpt_regions = []
-    start = -1
-    end = -1
-    current_region = None
-
-    for idx, node in enumerate(node_list):
-        if len(node.meta['info'].activation_checkpoint) > ckpt_level:
-            act_ckpt_label = node.meta['info'].activation_checkpoint[ckpt_level]
-
-            # this activation checkpoint label is not set yet
-            # meaning this is the first node of the activation ckpt region
-            if current_region is None:
-                current_region = act_ckpt_label
-                start = idx
-
-            # if activation checkpoint has changed
-            # we restart the tracking
-            # e.g. node ckpt states = [ckpt1, ckpt2, ckpt2, ckpt2]
-            if act_ckpt_label != current_region:
-                assert start != -1
-                ckpt_regions.append((start, idx - 1))
-                current_region = act_ckpt_label
-                start = idx
-                end = -1
-
-        elif current_region is not None and _end_of_ckpt(node, ckpt_level):
-            # used to check the case below
-            # node ckpt states = [ckpt, ckpt, non-ckpt]
-            end = idx - 1
-            assert start != -1 and end != -1
-            ckpt_regions.append((start, end))
-            start = end = -1
-            current_region = None
-
+class CheckpointSolverRotor(CheckpointSolverBase):
+
+    def __init__(self,
+                 graph: Graph,
+                 free_memory: float = -1,
+                 cnode: List[str] = None,
+                 memory_slots: int = 500,
+                 optim_multiplier: float = 1.0):
+        """This is the simple implementation of dynamic programming algorithm rotor
+        in https://hal.inria.fr/hal-02352969. Some code are adapted from
+        https://gitlab.inria.fr/hiepacs/rotor.
+
+        Usage:
+            Assume that we have a ``GraphModule``, and we have already done the extractions
+            to the graph to retrieve all information needed, then we could use the following
+            code to find a solution using ``CheckpointSolverRotor``:
+            >>> solver = CheckpointSolverRotor(gm.graph, free_memory=torch.cuda.mem_get_info(device=0)[0])
+            >>> rotor_graph = solver.solve(force_python=True)   # otherwise use C solver
+            >>> gm.graph = rotor_graph    # set the graph to a new graph
+
+        Args:
+            graph (Graph): The computing graph to be optimized.
+            free_memory (float, optional): Memory constraint for the solution, unit is byte.
+                Use ``torch.cuda.mem_get_info(device=0)[0]`` to estimate the free_memory. Defaults to -1.
+            cnode (List[str], optional): Common node List, should be the subset of input. Defaults to None.
+            memory_slots (int, optional): Number of slots for discretizing memory budget. Defaults to 500.
+            optim_multiplier (float, optional): The multiplier of extra weight storage for the
+            ``torch.optim.Optimizer``. Default to 1.0.
+        """
+        super().__init__(graph, free_memory, True, cnode, optim_multiplier)
+        self.memory_slots = memory_slots
+
+        # construct chain
+        unit = self.free_memory // self.memory_slots
+        self.chain = self._construct_chain(self.graph, self.node_list)
+        self.chain.discretize_all(unit)
+
+        self.cost_table = None
+        self.back_ptr = None
+        self.sequence = None
+
+    def solve(self, force_python: bool = False, verbose: bool = False) -> Graph:
+        """Solve the checkpointing problem using rotor algorithm.
+
+        Args:
+            force_python (bool, optional): Use Python version of solver, else use C version. Defaults to False.
+            verbose (bool, optional): Print verbose information. Defaults to False.
+
+        Returns:
+            graph (Graph): The optimized graph, should be a copy of the original graph.
+        """
+        chain = self.chain
+
+        # compute cost table
+        if force_python:
+            self.cost_table, self.back_ptr = self._compute_table(chain, self.memory_slots)
         else:
-            pass
-
-    if current_region is not None:
-        end = len(node_list) - 1
-        ckpt_regions.append((start, end))
-    return ckpt_regions
-
-
-def emit_ckpt_func(body,
-                   ckpt_func,
-                   node_list: List[Node],
-                   emit_node_func,
-                   delete_unused_value_func,
-                   ckpt_level=0,
-                   in_ckpt=False):
-    """Emit ckpt function in nested way
-
-    Args:
-        body: forward code - in recursive calls, this part will be checkpoint
-        functions code
-        ckpt_func: checkpoint functions code - in recursive calls, this part
-        will be a buffer
-        node_list (List[Node]): list of torch.fx.Node
-        emit_node_func: function to emit a node
-        delete_unused_value_func: function to delete unused value
-        level (int, optional): checkpoint level. Defaults to 0.
-        in_ckpt (bool, optional): indicates wether the func is in recursive
-        call. Defaults to False.
-    """
-    inputs, outputs = _find_input_and_output_nodes(node_list)
-
-    # label given by each layer, e.g. if you are currently at level (0, 1, 1)
-    # the label will be '0_1_1'
-    label = "_".join([str(idx) for idx in node_list[0].meta['info'].activation_checkpoint[:ckpt_level + 1]])
-    ckpt_fn_def = _gen_ckpt_fn_def(label, inputs)
-    ckpt_func.append(f'{ckpt_fn_def}\n')
-
-    # if there is more level to fetch
-    if ckpt_level + 1 < max(map(lambda node: len(node.meta['info'].activation_checkpoint), node_list)):
-        ckpt_regions = _find_nested_ckpt_regions(node_list, ckpt_level + 1)
-        start_idx = [item[0] for item in ckpt_regions]
-        end_idx = [item[1] for item in ckpt_regions]
-
-        # use ckpt_func_buffer to store nested checkpoint functions
-        ckpt_func_buffer = []
-        node_idx = 0
-        while 1:
-            if node_idx >= len(node_list):
-                break
-
-            if node_idx in start_idx:
-                ckpt_node_list = node_list[node_idx:end_idx[start_idx.index(node_idx)] + 1]
-                emit_ckpt_func(ckpt_func, ckpt_func_buffer, ckpt_node_list, emit_node_func, delete_unused_value_func,
-                               ckpt_level + 1, True)
-                node_idx += len(ckpt_node_list)
+            self.cost_table, self.back_ptr = self._compute_table_c(chain, self.memory_slots)
 
-            else:
-                node = node_list[node_idx]
-                emit_node_func(node, ckpt_func)
-                ckpt_func[-1] = '    ' + ckpt_func[-1]
-                delete_unused_value_func(node, ckpt_func)
-                node_idx += 1
+        if verbose:
+            self.print_chain()
 
-        ckpt_func.append('    ' + _gen_ckpt_output(outputs) + '\n\n')
-        ckpt_func += ckpt_func_buffer
+        # backtrack
+        try:
+            self.sequence = self._backtrack(chain, 0, len(chain), self.memory_slots - chain.x[0], self.cost_table,
+                                            self.back_ptr)
+            self._annotate_from_sequence(self.sequence, self.node_list)
+        except ValueError as e:
+            # using logger to annonce that the solver is failed
+            logger = get_dist_logger()
+            logger.warning(f'Checkpoint solver failed: {e}')
+            raise ValueError
+
+        if verbose:
+            self.print_sequence()
+
+        return deepcopy(self.graph)
+
+    def print_chain(self):
+        print('[input]', self.chain.x[0], self.chain.xbar[0], self.chain.ftmp[0], self.chain.btmp[0])
+        for idx in range(len(self.node_list) - 1):
+            print(self.node_list[idx], self.chain.x[idx + 1], self.chain.xbar[idx + 1], self.chain.ftmp[idx],
+                  self.chain.btmp[idx])
+        print(f'Chain = {self.chain}')
+
+    def print_sequence(self):
+        print(f'Sequence = {self.sequence}')
+
+    @classmethod
+    def _construct_chain(cls, graph: Graph, node_list: List[List[Node]]) -> Chain:
+        input_tensors = cls._extract_input(graph)
+        ftime, btime, ftmp, btmp = list(), list(), list(), list()
+        xbar, x = [activation_size(input_tensors)], [activation_size(input_tensors)]
 
-    # last level
-    else:
         for node in node_list:
-            emit_node_func(node, ckpt_func)
-            ckpt_func[-1] = '    ' + ckpt_func[-1]
-            delete_unused_value_func(node, ckpt_func)
-
-        ckpt_func.append('    ' + _gen_ckpt_output(outputs) + '\n\n')
-
-    usage = _gen_ckpt_usage(label, inputs, outputs, False) + '\n'
-    if in_ckpt:
-        usage = '    ' + usage
-    body.append(usage)
-
-
-def emit_code_with_activation_checkpoint(body, ckpt_func, nodes, emit_node_func, delete_unused_value_func):
-    """Emit code with nested activation checkpoint
-    When we detect some of the annotation is a , we will use
-    this function to emit the activation checkpoint codes.
-
-    Args:
-        body: forward code
-        ckpt_func: checkpoint functions code
-        nodes: graph.nodes
-        emit_node_func: function to emit node
-        delete_unused_value_func: function to remove the unused value
-    """
-    ckpt_regions = _find_nested_ckpt_regions(nodes, 0)
-    start_idx = [item[0] for item in ckpt_regions]
-    end_idx = [item[1] for item in ckpt_regions]
-    node_list = list(nodes)
-
-    node_idx = 0
-    while 1:
-        # break if we finish the processing all the nodes
-        if node_idx >= len(node_list):
-            break
-
-        # process ckpt_regions
-        if node_idx in start_idx:
-            ckpt_node_list = node_list[node_idx:end_idx[start_idx.index(node_idx)] + 1]
-            emit_ckpt_func(body, ckpt_func, ckpt_node_list, emit_node_func, delete_unused_value_func)
-            node_idx += len(ckpt_node_list)
+            node_info = cls._extract_node_info(node)
+            ftime.append(node_info[0])
+            btime.append(node_info[1])
+            x.append(node_info[2])
+            xbar.append(node_info[3])
+            ftmp.append(node_info[4])
+            btmp.append(node_info[5])
+
+        # currently we view loss backward temp as zero
+        btime.append(0)
+        btmp.append(0)
+
+        return Chain(ftime, btime, x, xbar, ftmp, btmp)
+
+    @classmethod
+    def _extract_node_info(cls, node: List[Node]) -> Tuple[int, ...]:
+        """Extract node info from a list of nodes"""
+        xbar = 0
+        ftime = 0
+        btime = 0
+        fwd_mem_peak = 0
+        for n in node:
+            assert isinstance(n, Node), f'{n} is not a Node'
+            if n.target == runtime_apply or n.target == runtime_comm_spec_apply:
+                # in this case we need to calculate memory usage directly based on the statics that hooked in node.meta
+                xbar += n.meta['fwd_mem_out']
+                fwd_mem_peak = max(fwd_mem_peak, xbar + n.meta['fwd_mem_tmp'])
+            else:
+                xbar += calculate_fwd_tmp(n) + calculate_fwd_out(n)
+                fwd_mem_peak = max(fwd_mem_peak, xbar + n.meta['fwd_mem_tmp'] + cls._extract_unused_output(n))
 
-        # process node in forward function
-        else:
-            node = node_list[node_idx]
-            emit_node_func(node, body)
-            delete_unused_value_func(node, body)
-            node_idx += 1
-
-
-@compatibility(is_backward_compatible=True)
-class ActivationCheckpointCodeGen(CodeGen):
-
-    def _gen_python_code(self, nodes, root_module: str, namespace: _Namespace) -> PythonCode:
-        free_vars: List[str] = []
-        body: List[str] = []
-        globals_: Dict[str, Any] = {}
-        wrapped_fns: Dict[str, None] = {}
-
-        # Wrap string in list to pass by reference
-        maybe_return_annotation: List[str] = ['']
-
-        def add_global(name_hint: str, obj: Any):
-            """Add an obj to be tracked as a global.
-            We call this for names that reference objects external to the
-            Graph, like functions or types.
-            Returns: the global name that should be used to reference 'obj' in generated source.
-            """
-            if _is_from_torch(obj) and obj != torch.device:    # to support registering torch.device
-                # HACK: workaround for how torch custom ops are registered. We
-                # can't import them like normal modules so they must retain their
-                # fully qualified name.
-                return _get_qualified_name(obj)
-
-            # normalize the name hint to get a proper identifier
-            global_name = namespace.create_name(name_hint, obj)
-
-            if global_name in globals_:
-                assert globals_[global_name] is obj
-                return global_name
-            globals_[global_name] = obj
-            return global_name
-
-        # Pre-fill the globals table with registered builtins.
-        for name, (_, obj) in _custom_builtins.items():
-            add_global(name, obj)
-
-        def type_repr(o: Any):
-            if o == ():
-                # Empty tuple is used for empty tuple type annotation Tuple[()]
-                return '()'
-
-            typename = _type_repr(o)
-
-            if hasattr(o, '__origin__'):
-                # This is a generic type, e.g. typing.List[torch.Tensor]
-                origin_type = _origin_type_map.get(o.__origin__, o.__origin__)
-                origin_typename = add_global(_type_repr(origin_type), origin_type)
-
-                if hasattr(o, '__args__'):
-                    # Assign global names for each of the inner type variables.
-                    args = [type_repr(arg) for arg in o.__args__]
-
-                    if len(args) == 0:
-                        # Bare type, such as `typing.Tuple` with no subscript
-                        # This code-path used in Python < 3.9
-                        return origin_typename
+            # minimum flop count is required
+            ftime += max(calculate_fwd_time(n), 1.0)
+            btime += max(calculate_bwd_time(n), 1.0)
+
+        x = calculate_fwd_out(node[-1])
+        xbar = max(x, xbar)
+        ftmp = fwd_mem_peak - xbar
+        btmp = cls._extract_btmp(node)
+        return ftime, btime, x, xbar, ftmp, btmp
+
+    @staticmethod
+    def _extract_input(graph: Graph) -> Tuple[Tensor, ...]:
+        """Extract input tensors from a Graph"""
+        input_tensors = []
+        for node in graph.nodes:
+            if node.op == 'placeholder':
+                input_tensors.append(node.meta['fwd_out'])
+        return input_tensors
 
-                    return f'{origin_typename}[{",".join(args)}]'
+    @staticmethod
+    def _extract_unused_output(node: Node) -> int:
+        """Extract unused output from `torch.fx.Node`"""
+        return activation_size(node.meta['fwd_out']) - calculate_fwd_out(node)
+
+    @staticmethod
+    def _extract_btmp(node: List[Node]) -> int:
+        """Extract btmp from a list of nodes"""
+
+        def _extract_deps_size():
+            deps_size = 0
+            for k, v in deps.items():
+                k: Node
+                if v > 0:
+                    deps_size += k.meta['bwd_mem_out']
+                if v == float('-inf'):
+                    deps_size -= calculate_fwd_tmp(k) + calculate_fwd_out(k)
+
+            return deps_size
+
+        btmp = 0
+        deps = {}
+        for n in reversed(node):
+            deps[n] = len(n.all_input_nodes)
+            btmp = max(btmp, _extract_deps_size() + n.meta['bwd_mem_tmp'])
+            for child in n.users:
+                if child in deps:
+                    deps[child] -= 1
+                    if deps[child] <= 0:
+                        deps[child] = float('-inf')    # free
+        return btmp
+
+    @staticmethod
+    def _compute_table(chain: Chain, mmax: int) -> Tuple:
+        """Compute the table using dynamic programming. Returns the cost table and the backtracking pointer.
+
+        Args:
+            chain (Chain): A basic linearized structure for solving the dynamic programming problem.
+            mmax (int): Maximum number of memory slots.
+
+        Returns:
+            cost_table (List): cost_table[m][lhs][rhs] indicates the optimal cost of the subproblem from lhs to rhs
+            with m memory slots.
+            back_ptr (List): back_ptr[m][lhs][rhs] indicates the best operation at this point. It is (True,) if the optimal choice
+            is a chain checkpoint, it is (False, j) if the optimal choice is a leaf checkpoint of length j
+        """
+
+        ftime = chain.ftime + [0.0]
+        btime = chain.btime
+        x = chain.x + [0]
+        xbar = chain.xbar + [0]
+        ftmp = chain.ftmp + [0]
+        btmp = chain.btmp + [0]
+
+        # Build table
+        cost_table = [[{} for _ in range(len(chain) + 1)] for _ in range(mmax + 1)]
+        back_ptr = [[{} for _ in range(len(chain) + 1)] for _ in range(mmax + 1)]
+
+        # Initialize corner cases where length of sequence equals to 1, i.e. lhs == rhs
+        for m in range(mmax + 1):
+            for i in range(len(chain) + 1):
+                limit = max(x[i + 1] + xbar[i + 1] + ftmp[i], x[i + 1] + xbar[i + 1] + btmp[i])
+                if m >= limit:
+                    cost_table[m][i][i] = ftime[i] + btime[i]
                 else:
-                    # Bare type, such as `typing.Tuple` with no subscript
-                    # This code-path used in Python 3.9+
-                    return origin_typename
-
-            # Common case: this is a regular module name like 'foo.bar.baz'
-            return add_global(typename, o)
-
-        def _format_args(args: Tuple[Argument, ...], kwargs: Dict[str, Argument]) -> str:
-
-            def _get_repr(arg):
-                # Handle NamedTuples (if it has `_fields`) via add_global.
-                if isinstance(arg, tuple) and hasattr(arg, '_fields'):
-                    qualified_name = _get_qualified_name(type(arg))
-                    global_name = add_global(qualified_name, type(arg))
-                    return f"{global_name}{repr(tuple(arg))}"
-                return repr(arg)
-
-            args_s = ', '.join(_get_repr(a) for a in args)
-            kwargs_s = ', '.join(f'{k} = {_get_repr(v)}' for k, v in kwargs.items())
-            if args_s and kwargs_s:
-                return f'{args_s}, {kwargs_s}'
-            return args_s or kwargs_s
-
-        # Run through reverse nodes and record the first instance of a use
-        # of a given node. This represents the *last* use of the node in the
-        # execution order of the program, which we will use to free unused
-        # values
-        node_to_last_use: Dict[Node, Node] = {}
-        user_to_last_uses: Dict[Node, List[Node]] = {}
-
-        def register_last_uses(n: Node, user: Node):
-            if n not in node_to_last_use:
-                node_to_last_use[n] = user
-                user_to_last_uses.setdefault(user, []).append(n)
-
-        for node in reversed(nodes):
-            map_arg(node.args, lambda n: register_last_uses(n, node))
-            map_arg(node.kwargs, lambda n: register_last_uses(n, node))
-
-        # NOTE: we add a variable to distinguish body and ckpt_func
-        def delete_unused_values(user: Node, body):
-            """
-            Delete values after their last use. This ensures that values that are
-            not used in the remainder of the code are freed and the memory usage
-            of the code is optimal.
-            """
-            if user.op == 'placeholder':
-                return
-            if user.op == 'output':
-                body.append('\n')
-                return
-            nodes_to_delete = user_to_last_uses.get(user, [])
-            if len(nodes_to_delete):
-                to_delete_str = ' = '.join([repr(n) for n in nodes_to_delete] + ['None'])
-                body.append(f';  {to_delete_str}\n')
+                    cost_table[m][i][i] = float("inf")
+
+        # Compute tables
+        for m in range(mmax + 1):
+            for d in range(1, len(chain) + 1):
+                for i in range(len(chain) + 1 - d):
+                    idx = i + d
+                    mmin = x[idx + 1] + x[i + 1] + ftmp[i]
+                    if idx > i + 1:
+                        mmin = max(mmin, x[idx + 1] + max(x[j] + x[j + 1] + ftmp[j] for j in range(i + 1, idx)))
+                    if m < mmin:
+                        cost_table[m][i][idx] = float("inf")
+                    else:
+                        leaf_checkpoints = [(j,
+                                             sum(ftime[i:j]) + cost_table[m - x[j]][j][idx] + cost_table[m][i][j - 1])
+                                            for j in range(i + 1, idx + 1)
+                                            if m >= x[j]]
+                        if leaf_checkpoints:
+                            best_leaf = min(leaf_checkpoints, key=lambda t: t[1])
+                        else:
+                            best_leaf = None
+                        if m >= xbar[i + 1]:
+                            chain_checkpoint = cost_table[m][i][i] + cost_table[m - xbar[i + 1]][i + 1][idx]
+                        else:
+                            chain_checkpoint = float("inf")
+                        if best_leaf and best_leaf[1] <= chain_checkpoint:
+                            cost_table[m][i][idx] = best_leaf[1]
+                            back_ptr[m][i][idx] = (False, best_leaf[0])
+                        else:
+                            cost_table[m][i][idx] = chain_checkpoint
+                            back_ptr[m][i][idx] = (True,)
+        return cost_table, back_ptr
+
+    @staticmethod
+    def _compute_table_c(chain: Chain, mmax: int) -> Tuple:
+        try:
+            from .rotorc import compute_table
+
+        # build module if module not found
+        except ModuleNotFoundError:
+            import os
+            import subprocess
+            import sys
+            logger = get_dist_logger()
+            logger.info("rotorc hasn't been built! Building library...", ranks=[0])
+            this_dir = os.path.dirname(os.path.abspath(__file__))
+            result = subprocess.Popen(
+                [
+                    f"{sys.executable}", f"{os.path.join(this_dir, 'build_c_ext.py')}", "build_ext",
+                    f"--build-lib={this_dir}"
+                ],
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            )
+            if result.wait() == 0:
+                logger.info("rotorc has been built!", ranks=[0])
+                from .rotorc import compute_table
             else:
-                body.append('\n')
+                logger.warning("rotorc built failed! Using python version!", ranks=[0])
+                return CheckpointSolverRotor._compute_table(chain, mmax)
+        return compute_table(chain, mmax)
+
+    @staticmethod
+    def _backtrack(chain: Chain, lhs: int, rhs: int, budget: int, cost_table: List[Any],
+                   back_ptr: List[Any]) -> "Sequence":
+        """Backtrack the cost table and retrieve the optimal checkpointing strategy.
+
+        Args:
+            chain (Chain): A basic linearized structure for solving the dynamic programming problem.
+            lhs (int): The left index of the interval to backtrack.
+            rhs (int): The right index of the interval to backtrack.
+            budget (int): The memory budget for processing this interval.
+            cost_table (List[Any]): See ``._compute_table()`` for definitions
+            back_ptr (List[Any]): See ``._compute_table()`` for definitions
+
+        Raises:
+            ValueError: Can not process the chain.
+
+        Returns:
+            sequence (Sequence): The sequence of executing nodes with checkpoints.
+        """
+        if budget <= 0:
+            raise ValueError(f"Can not process a chain with negative memory {budget}")
+        elif cost_table[budget][lhs][rhs] == float("inf"):
+            raise ValueError(f"Can not process this chain from index {lhs} to {rhs} with memory {budget}")
+
+        sequence = Sequence()
+        if rhs == lhs:
+            if lhs == len(chain):
+                sequence += [Loss()]
+            else:
+                sequence += [ForwardEnable(lhs), Backward(lhs)]
+            return sequence
 
-        # NOTE: we add a variable to distinguish body and ckpt_func
-        def emit_node(node: Node, body):
-            maybe_type_annotation = '' if node.type is None else f' : {type_repr(node.type)}'
-            if node.op == 'placeholder':
-                assert isinstance(node.target, str)
-                maybe_default_arg = '' if not node.args else f' = {repr(node.args[0])}'
-                free_vars.append(f'{node.target}{maybe_type_annotation}{maybe_default_arg}')
-                raw_name = node.target.replace('*', '')
-                if raw_name != repr(node):
-                    body.append(f'{repr(node)} = {raw_name}\n')
-                return
-            elif node.op == 'call_method':
-                assert isinstance(node.target, str)
-                body.append(f'{repr(node)}{maybe_type_annotation} = {_format_target(repr(node.args[0]), node.target)}'
-                            f'({_format_args(node.args[1:], node.kwargs)})')
-                return
-            elif node.op == 'call_function':
-                assert callable(node.target)
-                # pretty print operators
-                if node.target.__module__ == '_operator' and node.target.__name__ in magic_methods:
-                    assert isinstance(node.args, tuple)
-                    body.append(f'{repr(node)}{maybe_type_annotation} = '
-                                f'{magic_methods[node.target.__name__].format(*(repr(a) for a in node.args))}')
-                    return
-
-                # pretty print inplace operators; required for jit.script to work properly
-                # not currently supported in normal FX graphs, but generated by torchdynamo
-                if node.target.__module__ == '_operator' and node.target.__name__ in inplace_methods:
-                    body.append(f'{inplace_methods[node.target.__name__].format(*(repr(a) for a in node.args))};  '
-                                f'{repr(node)}{maybe_type_annotation} = {repr(node.args[0])}')
-                    return
-
-                qualified_name = _get_qualified_name(node.target)
-                global_name = add_global(qualified_name, node.target)
-                # special case for getattr: node.args could be 2-argument or 3-argument
-                # 2-argument: attribute access; 3-argument: fall through to attrib function call with default value
-                if global_name == 'getattr' and \
-                isinstance(node.args, tuple) and \
-                isinstance(node.args[1], str) and \
-                node.args[1].isidentifier() and \
-                len(node.args) == 2:
-                    body.append(
-                        f'{repr(node)}{maybe_type_annotation} = {_format_target(repr(node.args[0]), node.args[1])}')
-                    return
-                body.append(
-                    f'{repr(node)}{maybe_type_annotation} = {global_name}({_format_args(node.args, node.kwargs)})')
-                if node.meta.get('is_wrapped', False):
-                    wrapped_fns.setdefault(global_name)
-                return
-            elif node.op == 'call_module':
-                assert isinstance(node.target, str)
-                body.append(f'{repr(node)}{maybe_type_annotation} = '
-                            f'{_format_target(root_module, node.target)}({_format_args(node.args, node.kwargs)})')
-                return
-            elif node.op == 'get_attr':
-                assert isinstance(node.target, str)
-                body.append(f'{repr(node)}{maybe_type_annotation} = {_format_target(root_module, node.target)}')
-                return
-            elif node.op == 'output':
-                if node.type is not None:
-                    maybe_return_annotation[0] = f" -> {type_repr(node.type)}"
-                body.append(self.generate_output(node.args[0]))
-                return
-            raise NotImplementedError(f'node: {node.op} {node.target}')
-
-        # Modified for activation checkpointing
-        ckpt_func = []
-        emit_code_with_activation_checkpoint(body, ckpt_func, nodes, emit_node, delete_unused_values)
-
-        if len(body) == 0:
-            # If the Graph has no non-placeholder nodes, no lines for the body
-            # have been emitted. To continue to have valid Python code, emit a
-            # single pass statement
-            body.append('pass\n')
-
-        if len(wrapped_fns) > 0:
-            wrap_name = add_global('wrap', torch.fx.wrap)
-            wrap_stmts = '\n'.join([f'{wrap_name}("{name}")' for name in wrapped_fns])
+        if back_ptr[budget][lhs][rhs][0]:
+            sequence += [
+                ForwardEnable(lhs),
+                CheckpointSolverRotor._backtrack(chain, lhs + 1, rhs, budget - chain.xbar[lhs + 1], cost_table,
+                                                 back_ptr),
+                Backward(lhs),
+            ]
         else:
-            wrap_stmts = ''
+            best_leaf = back_ptr[budget][lhs][rhs][1]
+            sequence += [ForwardCheck(lhs)]
+            sequence += [ForwardNograd(k) for k in range(lhs + 1, best_leaf)]
+            sequence += [
+                CheckpointSolverRotor._backtrack(chain, best_leaf, rhs, budget - chain.x[best_leaf], cost_table,
+                                                 back_ptr),
+                CheckpointSolverRotor._backtrack(chain, lhs, best_leaf - 1, budget, cost_table, back_ptr),
+            ]
+        return sequence
+
+    @staticmethod
+    def _annotate_from_sequence(sequence: Sequence, node_list: List[List[Node]]):
+        """Annotate the nodes in the ``node_list`` with activation checkpoint from the sequence.
+
+        Args:
+            sequence (Sequence): The sequence of executing nodes with activation checkpoint annotations.
+            node_list (List[List[Node]]): The list of nodes to annotate.
+        """
+        op_list = sequence.list_operations()
+        loss_op = next(op for op in op_list if isinstance(op, Loss))
+        fwd_list = op_list[:op_list.index(loss_op)]
+        bwd_list = op_list[op_list.index(loss_op) + 1:]
+        ckpt_idx = 0
+        in_ckpt = False
+        ckpt_region = []
+
+        # forward annotation
+        for idx, op in enumerate(fwd_list, 0):
+            if in_ckpt:
+                if isinstance(op, ForwardNograd):
+                    ckpt_region.append(idx)
+
+                elif isinstance(op, ForwardEnable):
+                    in_ckpt = False
+                    for node_idx in ckpt_region:
+                        for n in node_list[node_idx]:
+                            n.meta['activation_checkpoint'] = [ckpt_idx]
+
+                    ckpt_idx += 1
+                    ckpt_region = []
+
+                elif isinstance(op, ForwardCheck):
+                    for node_idx in ckpt_region:
+                        for n in node_list[node_idx]:
+                            n.meta['activation_checkpoint'] = [ckpt_idx]
+
+                    ckpt_idx += 1
+                    ckpt_region = [idx]
 
-        if self._body_transformer:
-            body = self._body_transformer(body)
+            else:
+                if isinstance(op, ForwardCheck):
+                    in_ckpt = True
+                    ckpt_region.append(idx)
+
+        # annotate the backward if there is any nested activation checkpoint
+        in_recompute = False
+        for op in bwd_list:
+            if in_recompute:
+                if isinstance(op, ForwardNograd):
+                    ckpt_region.append(op.index)
+
+                elif isinstance(op, ForwardEnable):
+                    for node_idx in ckpt_region:
+                        for n in node_list[node_idx]:
+                            n.meta['activation_checkpoint'].append(ckpt_idx)
+
+                    ckpt_idx += 1
+                    ckpt_region = []
+
+                elif isinstance(op, ForwardCheck):
+                    for node_idx in ckpt_region:
+                        for n in node_list[node_idx]:
+                            n.meta['activation_checkpoint'].append(ckpt_idx)
+
+                    ckpt_idx += 1
+                    ckpt_region = [op.index]
+
+                elif isinstance(op, Backward):
+                    for node_idx in ckpt_region:
+                        for n in node_list[node_idx]:
+                            n.meta['activation_checkpoint'].append(ckpt_idx)
 
-        for name, value in self.additional_globals():
-            add_global(name, value)
+                    in_recompute = False
 
-        prologue = self.gen_fn_def(free_vars, maybe_return_annotation[0])
-        prologue = ''.join(ckpt_func) + prologue
-        prologue = prologue
-
-        code = ''.join(body)
-        code = '\n'.join('    ' + line for line in code.split('\n'))
-        fn_code = f"""
-{wrap_stmts}
-{prologue}
-{code}"""
-        return PythonCode(fn_code, globals_)
+            else:
+                if not isinstance(op, Backward):
+                    in_recompute = True
+                    ckpt_idx = 0
+                    ckpt_region = []
+                    if isinstance(op, ForwardCheck):
+                        ckpt_region.append(op.index)
+
+        # postprocess, make sure every activation checkpoint label in the
+        # same activation checkpoint region (level = 0) has the same length
+        op_list = []
+        for node in node_list:
+            op_list += node
+        ckpt_regions = _find_nested_ckpt_regions(op_list)
+        for (start_idx, end_idx) in ckpt_regions:
+            nested_length = max(
+                len(op_list[idx].meta['activation_checkpoint']) for idx in range(start_idx, end_idx + 1))
+            for idx in range(start_idx, end_idx + 1):
+                op_list[idx].meta['activation_checkpoint'] += [None] * (nested_length -
+                                                                        len(op_list[idx].meta['activation_checkpoint']))
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/graph_module.py` & `colossalai-nightly-2023.5.6/colossalai/pipeline/pipelinable.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,239 +1,254 @@
-import linecache
-import os
-import sys
-import traceback
-import warnings
-from pathlib import Path
-from typing import Any, Dict, Optional, Union
-
 import torch
-import torch.fx
-import torch.nn as nn
-from torch.fx.graph import PythonCode
-
-try:
-    from torch.fx.graph import _PyTreeCodeGen
-    SUPPORT_PT_CODEGEN = True
-except ImportError:
-    SUPPORT_PT_CODEGEN = False
-
-from torch.fx.graph_module import _exec_with_source, _forward_from_src
-from torch.nn.modules.module import _addindent
-
-
-# This is a copy of torch.fx.graph_module._WrappedCall.
-# It should be removed when we stop supporting torch < 1.12.0.
-class _WrappedCall:
-
-    def __init__(self, cls, cls_call):
-        self.cls = cls
-        self.cls_call = cls_call
-
-    # Previously, if an error occurred when valid
-    # symbolically-traced code was run with an invalid input, the
-    # user would see the source of the error as coming from
-    # `File "<eval_with_key_N">`, where N is some number. We use
-    # this function to generate a more informative error message. We
-    # return the traceback itself, a message explaining that the
-    # error occurred in a traced Module's generated forward
-    # function, and five lines of context surrounding the faulty
-    # line
-    @staticmethod
-    def _generate_error_message(frame_summary: traceback.FrameSummary) -> str:
-        # auxiliary variables (for readability)
-        err_lineno = frame_summary.lineno
-        assert err_lineno is not None
-        line = frame_summary.line
-        assert line is not None
-        err_line_len = len(line)
-        all_src_lines = linecache.getlines(frame_summary.filename)
-
-        # constituent substrings of the error message
-        tb_repr = traceback.format_exc()
-        custom_msg = ("Call using an FX-traced Module, "
-                      f"line {err_lineno} of the traced Module's "
-                      "generated forward function:")
-        before_err = "".join(all_src_lines[err_lineno - 2:err_lineno])
-        marker = "~" * err_line_len + "~~~ <--- HERE"
-        err_and_after_err = "\n".join(all_src_lines[err_lineno:err_lineno + 2])
-
-        # joined message
-        return "\n".join([tb_repr, custom_msg, before_err, marker, err_and_after_err])
-
-    def __call__(self, obj, *args, **kwargs):
-        try:
-            if self.cls_call is not None:
-                return self.cls_call(obj, *args, **kwargs)
-            else:
-                return super(self.cls, obj).__call__(*args, **kwargs)    # type: ignore[misc]
-        except Exception as e:
-            assert e.__traceback__
-            topmost_framesummary: traceback.FrameSummary = \
-                traceback.StackSummary.extract(traceback.walk_tb(e.__traceback__))[-1]  # type: ignore[arg-type]
-            if "eval_with_key" in topmost_framesummary.filename:
-                print(_WrappedCall._generate_error_message(topmost_framesummary), file=sys.stderr)
-                raise e.with_traceback(None)
-            else:
-                raise e
+import inspect
+from colossalai.utils.model.utils import InsertPostInitMethodToModuleSubClasses
+
+from .utils import partition_uniform, partition_balanced, build_kwargs_for_function, \
+                build_kwargs_for_module, exec_func_with_kwargs, exec_funcs_with_kwargs, \
+                call_module, customized_partition
+from colossalai.nn.layer.utils import CheckpointModule
+from colossalai.tensor import ColoParameter
+from colossalai.core import global_context as gpc
+from colossalai.context import ParallelMode
+from .layer_spec import LayerSpec
 
 
-class ColoGraphModule(torch.fx.GraphModule):
+class PipelinableContext(InsertPostInitMethodToModuleSubClasses):
     """
-    ColoGraphGraphModule is an nn.Module generated from an fx.Graph.
-    ColoGraphmodule has a ``graph`` attribute, as well as ``code`` and ``forward``
-    attributes generated from that ``graph``.
-
-    The difference between ``ColoGraphModule`` and ``torch.fx.GraphModule`` is that
-    ``ColoGraphModule`` has a ``bind()`` function to bind customized functions
-    (i.e. activation checkpoint) to ``code`` of ``nn.Module``. If you want to use
-    specific features in Colossal-AI that are not supported by ``torch.fx.GraphModule``,
-    you can use ``ColoGraphModule`` instead.
-
-    ``colossalai.fx.symbolic_trace()`` will return a ``ColoGraphModule`` as default.
-
-    .. warning::
-
-        When ``graph`` is reassigned, ``code`` and ``forward`` will be automatically
-        regenerated. However, if you edit the contents of the ``graph`` without reassigning
-        the ``graph`` attribute itself, you must call ``recompile()`` to update the generated
-        code.
+    A context manager to split the model into pipeline stages.
     """
 
-    def __init__(self,
-                 root: Union[torch.nn.Module, Dict[str, Any]],
-                 graph: torch.fx.Graph,
-                 class_name: str = 'GraphModule'):
-        super().__init__(root, graph, class_name)
-
-    def bind(self, ckpt_def, globals):
-        """Bind function needed for correctly execute ``GraphModule.forward()``
-
-        We need to bind checkpoint functions to ``ColoGraphModule`` so that we could
-        correctly execute ``GraphModule.forward()``
-
-        Args:
-            ckpt_def (List[str]): definition before the forward function
-            globals (Dict[str, Any]): global variables
-        """
-
-        ckpt_code = "\n".join(ckpt_def)
-        globals_copy = globals.copy()
-        _exec_with_source(ckpt_code, globals_copy)
-        func_list = [func for func in globals_copy.keys() if "checkpoint" in func or "pack" in func]
-        for func in func_list:
-            tmp_func = globals_copy[func]
-            setattr(self, func, tmp_func.__get__(self, self.__class__))
-            del globals_copy[func]
-
-    def recompile(self) -> PythonCode:
-        """
-        Recompile this GraphModule from its ``graph`` attribute. This should be
-        called after editing the contained ``graph``, otherwise the generated
-        code of this ``GraphModule`` will be out of date.
-        """
-        if SUPPORT_PT_CODEGEN and isinstance(self._graph._codegen, _PyTreeCodeGen):
-            self._in_spec = self._graph._codegen.pytree_info.in_spec
-            self._out_spec = self._graph._codegen.pytree_info.out_spec
-        python_code = self._graph.python_code(root_module='self')
-        self._code = python_code.src
-
-        # To split ckpt functions code and forward code
-        _code_list = self._code.split("\n")
-        _fwd_def = [item for item in _code_list if "def forward" in item][0]
-        _fwd_idx = _code_list.index(_fwd_def)
-        ckpt_def = _code_list[:_fwd_idx]
-        self._code = "\n".join(_code_list[_fwd_idx:])
-
-        self.bind(ckpt_def, python_code.globals)
-
-        cls = type(self)
-        cls.forward = _forward_from_src(self._code, python_code.globals)
-
-        # Determine whether this class explicitly defines a __call__ implementation
-        # to wrap. If it does, save it in order to have wrapped_call invoke it.
-        # If it does not, wrapped_call can use a dynamic call to super() instead.
-        # In most cases, super().__call__ should be torch.nn.Module.__call__.
-        # We do not want to hold a reference to Module.__call__ here; doing so will
-        # bypass patching of torch.nn.Module.__call__ done while symbolic tracing.
-        cls_call = cls.__call__ if "__call__" in vars(cls) else None
-
-        if '_wrapped_call' not in vars(cls):
-            cls._wrapped_call = _WrappedCall(cls, cls_call)    # type: ignore[attr-defined]
-
-        def call_wrapped(self, *args, **kwargs):
-            return self._wrapped_call(self, *args, **kwargs)
-
-        cls.__call__ = call_wrapped
-
-        # reset self._code to original src, otherwise to_folder will be wrong
-        self._code = python_code.src
-        return python_code
-
-    def to_folder(self, folder: Union[str, os.PathLike], module_name: str = "FxModule"):
-        """Dumps out module to ``folder`` with ``module_name`` so that it can be
-        imported with ``from <folder> import <module_name>``
-
-        Args:
-
-            folder (Union[str, os.PathLike]): The folder to write the code out to
-
-            module_name (str): Top-level name to use for the ``Module`` while
-                writing out the code
-        """
-        folder = Path(folder)
-        Path(folder).mkdir(exist_ok=True)
-        torch.save(self.state_dict(), folder / 'state_dict.pt')
-        tab = " " * 4
+    def __init__(self, policy: str = "balanced"):
+        super().__init__()
+        self._layer_spec_dict = {}
+        self._root_children = None
+        self._model = None
+        self._layer_spec_list = []
+        self._func_dict = {}
+        self._policy = policy
+
+    @property
+    def policy(self):
+        return self._policy
+
+    @policy.setter
+    def policy(self, policy: str):
+        self._policy = policy
+
+    @property
+    def layers_count(self):
+        return len(self._layer_spec_list)
+
+    @property
+    def funcs_count(self):
+        return len(self._func_dict)
 
-        # we add import colossalai here
-        model_str = f"""
-import torch
-from torch.nn import *
-import colossalai
+    def _pre_context_exec(self):
+        """
+        The Callback function when entering the context
+        """
+        # reserve rng states
+        self.cpu_rng_state = torch.get_rng_state()
+        self.cuda_rng_state = torch.cuda.get_rng_state()
 
+    def _post_context_exec(self):
+        """
+        The callback function when exiting context.
+        """
 
-class {module_name}(torch.nn.Module):
-    def __init__(self):
-        super().__init__()
-"""
+        # reset rng states
+        torch.set_rng_state(self.cpu_rng_state)
+        torch.cuda.set_rng_state(self.cuda_rng_state)
+
+    def _post_init_method(self, module: torch.nn.Module, *args, **kwargs):
+        """
+        The function to call at the end of the constructor of each module.
+        NOTE() The module may be passed to this function multiple times.
+        """
+        # iterate over the positional arguments
+        # to check if an argument is a torch Module
+        # if found any torch Module, replace it with its layer spec
+        # for storage purpose
+        modified_args = []
+        for arg in args:
+            if isinstance(arg, torch.nn.Module):
+                # if nn.Module is an argument of a non-root module, then we should convert it to layer spec, which make sure the correct init method used in the real build.
+                # if nn.Module is an argument of the root module, then we should just record the module instance itself, because those instance has been built outside of the context.
+                if id(arg) in self._layer_spec_dict:
+                    arg = self._layer_spec_dict[id(arg)]
+
+            modified_args.append(arg)
+
+        # to the same for the keyword arguments
+        modified_kwargs = {}
+        for k, v in kwargs.items():
+            if isinstance(v, torch.nn.Module):
+                v = self._layer_spec_dict[id(v)]
+            # (lyl)TODO: analyse ColoTensor as well
+            modified_kwargs[k] = v
+
+        # keep track of the module children
+        # as torch.nn.Module.__init__ is called from inner module to outer module,
+        # the final value of self._model will be the outermost model
+        # e.g. if the model is torchvision.models.resnet18, then the final value of self._model
+        # will be the ``ResNet`` object.
+        self._root_children = list(module.children())
+        self._model = module
+
+        # store the children to keep the module hierarchy
+        layer_spec = LayerSpec(module.__class__, *modified_args, **modified_kwargs)
+        layer_spec.set_children(module.children())
+
+        # store the layer spec in this context
+        module_id = id(module)
+        self._layer_spec_dict[module_id] = layer_spec
+
+        # convert all torch.nn.Parameter to colossalai.tensor.ColoParameter
+        name_list = []
+        for name, param in module.named_parameters():
+            if isinstance(param, ColoParameter):
+                continue
+            name_list.append((name, param))
 
-        def _gen_model_repr(module_name: str, module: torch.nn.Module) -> Optional[str]:
-            safe_reprs = [nn.Linear, nn.Conv1d, nn.Conv2d, nn.Conv3d, nn.BatchNorm1d, nn.BatchNorm2d, nn.BatchNorm3d]
-            if type(module) in safe_reprs:
-                return f"{module.__repr__()}"
+        for name, param in name_list:
+            if hasattr(module, name):
+                delattr(module, name)
+            setattr(module, name, ColoParameter.from_torch_tensor(tensor=param.data, requires_grad=param.requires_grad))
+
+    def to_layer_list(self, exec_seq=None):
+        """
+        Create a layer spec list and func list with execution sequence given by user.
+        If exec_seq is None, we will take the module initizing order as execution order.
+        """
+
+        self._exec_seq = exec_seq
+        if exec_seq is None:
+            # if user do not provide the model executing sequence, we use the initialization order as the executing order.
+            children_name = []
+            for child in self._root_children:
+                layer_spec = self._layer_spec_dict[id(child)]
+                if layer_spec.typename in (torch.nn.modules.container.ModuleList,
+                                           torch.nn.modules.container.Sequential):
+                    for child_in_container in layer_spec.children:
+                        self._layer_spec_list.append(self._layer_spec_dict[id(child_in_container)])
+                        for name, module in self._model.named_modules():
+                            if id(module) == id(child_in_container):
+                                children_name.append(name)
+                                break
+                else:
+                    self._layer_spec_list.append(layer_spec)
+                    for name, module in self._model.named_modules():
+                        if id(module) == id(child):
+                            children_name.append(name)
+                            break
+
+        else:
+            front_funcs_list = []
+            named_modules = dict(self._model.named_modules())
+            for index, element in enumerate(exec_seq):
+                if isinstance(element, str):
+                    if element == 'SPLIT_NODE':
+                        continue
+                    assert element in named_modules, f'Found invalid module name {element}, please check if you spell the module name correctly.'
+
+                    # get the layer spec based on the module ID
+                    module = named_modules[element]
+                    layer_spec = self._layer_spec_dict[id(module)]
+
+                    # check whether there are functions which should be executed before this module
+                    if len(front_funcs_list) != 0:
+                        func_key = (layer_spec, "front")
+                        if func_key not in self._func_dict:
+                            self._func_dict[func_key] = []
+                        for f in front_funcs_list:
+                            self._func_dict[func_key].append(f)
+                        front_funcs_list = []
+
+                    func_key = (layer_spec, "behind")
+                    self._layer_spec_list.append(layer_spec)
+                elif isinstance(element, tuple) and element[1] == "front":
+                    front_funcs_list.append(element[0])
+                else:
+                    if func_key not in self._func_dict:
+                        self._func_dict[func_key] = []
+                    if isinstance(element, tuple):
+                        self._func_dict[func_key].append(element[0])
+                    else:
+                        self._func_dict[func_key].append(element)
+
+    def partition(self, num_chunks, pipeline_size, rank):
+        """
+        Partitioned model will be built respect to partion policy.
+        The real module instance will be built in this method.
+        """
+        if isinstance(self._policy, str):
+            if self._policy == "uniform":
+                parts = partition_uniform(len(self._layer_spec_list), pipeline_size, num_chunks)[rank]
+            elif self._policy == "balanced":
+                param_counts = []
+                for layer_spec in self._layer_spec_list:
+                    param_counts.append(layer_spec.count_params())
+                parts = partition_balanced(param_counts, pipeline_size, num_chunks)[rank]
+            elif self._policy == "customized":
+                assert self._exec_seq is not None, f'An explicit exec_seq must be defined by user in customized policy mode.'
+                self.customized_parts = customized_partition(self._exec_seq)
+                assert len(self.customized_parts) == gpc.get_world_size(
+                    ParallelMode.PIPELINE
+                ), f'World size is {gpc.get_world_size(ParallelMode.PIPELINE)}, but the number of partions is {len(self.customized_parts)}'
+                parts = self.customized_parts[rank]
             else:
-                return None
+                raise ValueError("A string partition policy should be one of ['uniform', 'balanced', 'customized'].")
+        elif isinstance(self._policy, dict):
+            parts = self._policy[rank]
+        else:
+            raise ValueError("A partition policy should be either a string or a dictionary.")
+
+        layers_to_build = []
+        for start, end in parts:
+            layers_to_build += self._layer_spec_list[start:end]
+        behind_func_dict_in_partition = {}
+        front_func_dict_in_partition = {}
+        module_list_in_partition = []
+        for layer in layers_to_build:
+            module = layer.build()
+            module_list_in_partition.append(module)
+            if (layer, "front") in self._func_dict:
+                front_func_dict_in_partition[id(module)] = self._func_dict[(layer, "front")]
+            elif (layer, "behind") in self._func_dict:
+                behind_func_dict_in_partition[id(module)] = self._func_dict[(layer, "behind")]
+        module_list_in_partition = torch.nn.ModuleList(module_list_in_partition)
+        pipeline_model = PipelinableModel(module_list_in_partition, front_func_dict_in_partition,
+                                          behind_func_dict_in_partition)
 
-        blobified_modules = []
-        for module_name, module in self.named_children():
-            module_str = _gen_model_repr(module_name, module)
-            if module_str is None:
-                module_file = folder / f'{module_name}.pt'
-                torch.save(module, module_file)
-                blobified_modules.append(module_name)
-                module_repr = module.__repr__().replace('\r', ' ').replace('\n', ' ')
-                module_str = f"torch.load(r'{module_file}') # {module_repr}"
-            model_str += f"{tab*2}self.{module_name} = {module_str}\n"
+        return pipeline_model
 
-        for buffer_name, buffer in self._buffers.items():
-            if buffer is None:
-                continue
-            model_str += f"{tab*2}self.register_buffer('{buffer_name}', torch.empty({list(buffer.shape)}, dtype={buffer.dtype}))\n"
 
-        for param_name, param in self._parameters.items():
-            if param is None:
-                continue
-            model_str += f"{tab*2}self.{param_name} = torch.nn.Parameter(torch.empty({list(param.shape)}, dtype={param.dtype}))\n"
+class PipelinableModel(torch.nn.Module):
+
+    def __init__(self, module_list, front_func_dict, behind_func_dict):
+        super().__init__()
+        self._module_list = module_list
+        self._front_func_dict = front_func_dict
+        self._behind_func_dict = behind_func_dict
 
-        model_str += f"{tab*2}self.load_state_dict(torch.load(r'{folder}/state_dict.pt'))\n"
-        model_str += f"{_addindent(self.code, 4)}\n"
+    def forward(self, *input_tensor, **kwargs):
+        for module in self._module_list:
 
-        module_file = folder / 'module.py'
-        module_file.write_text(model_str)
+            if id(module) in self._front_func_dict:
+                input_tensor = exec_funcs_with_kwargs(self._front_func_dict, id(module), input_tensor, kwargs)
+
+            if isinstance(module, CheckpointModule):
+                forward_func = module._forward
+            else:
+                forward_func = module.forward
+            module_kwargs = build_kwargs_for_module(forward_func, input_tensor, kwargs)
+            if input_tensor is None:
+                input_tensor = call_module(module, kwargs=module_kwargs)
+            elif isinstance(input_tensor, torch.Tensor):
+                input_tensor = call_module(module, args=(input_tensor,), kwargs=module_kwargs)
+            else:
+                input_tensor = call_module(module, args=input_tensor, kwargs=module_kwargs)
 
-        init_file = folder / '__init__.py'
-        init_file.write_text('from .module import *')
+            if id(module) in self._behind_func_dict:
+                input_tensor = exec_funcs_with_kwargs(self._behind_func_dict, id(module), input_tensor, kwargs)
 
-        if len(blobified_modules) > 0:
-            warnings.warn("Was not able to save the following children modules as reprs -"
-                          f"saved as pickled files instead: {blobified_modules}")
+        return input_tensor
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/passes/shape_prop.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/reduce_scatter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,266 +1,200 @@
-"""``torch.fx.ShapeProp``, but with ``MetaTensor``"""
-
-from typing import Any, Callable, Dict, Optional, Tuple, Union
+# Copyright (c) Facebook, Inc. and its affiliates.
+#
+# This source code is licensed under the BSD license found in the
+# LICENSE file in the root directory of this source tree.
+
+import functools
+import os
+from typing import Callable, Dict, List, Optional, Tuple
 
 import torch
-import torch.fx
-from torch.autograd.graph import saved_tensors_hooks
-from torch.utils._pytree import tree_map
-
-from colossalai._analyzer._subclasses import MetaTensor, MetaTensorMode
-from colossalai._analyzer.fx.node_util import MetaInfo
-from colossalai.fx._compatibility import compatibility
-
-Target = Union[Callable[..., Any], str]
-
-
-class sim_env(saved_tensors_hooks):
-    """
-    A simulation of memory allocation and deallocation in the forward pass
-    using ``saved_tensor_hooks``.
-
-    Attributes:
-        ctx (Dict[int, torch.Tensor]): A dictionary that maps the
-            data pointer of a tensor to the tensor itself. This is used
-            to track the memory allocation and deallocation.
-
-        param_ctx (Dict[int, torch.Tensor]): A dictionary that maps the
-            data pointer of all model parameters to the parameter itself.
-            This avoids overestimating the memory usage of the intermediate activations.
-    """
-
-    def __init__(self, module: Optional[torch.nn.Module] = None):
-        super().__init__(self.pack_hook, self.unpack_hook)
-        self.ctx = {}
-        self.param_ctx = {param.data_ptr(): param for param in module.parameters()}
-        self.buffer_ctx = {buffer.data_ptr(): buffer for buffer in module.buffers()} if module else {}
-
-    def pack_hook(self, tensor: torch.Tensor):
-        if tensor.data_ptr() not in self.param_ctx and tensor.data_ptr() not in self.buffer_ctx:
-            self.ctx[tensor.data_ptr()] = tensor
-        return tensor
-
-    def unpack_hook(self, tensor):
-        return tensor
-
-
-def _normalize_tuple(x):
-    if not isinstance(x, tuple):
-        return (x,)
-    return x
-
-
-def _current_device(module):
-    try:
-        return next(module.parameters()).device
-    except StopIteration:
-        return torch.device('cpu')
-
-
-@compatibility(is_backward_compatible=False)
-class ShapeProp(torch.fx.Interpreter):
-    """
-    Execute an FX graph Node-by-Node and record the meta data of the result
-    into the corresponding node.
-
-    Usage:
-        >>> model = MyModule()
-        >>> x = torch.rand(10, 10)
-        >>> gm = colossalai.fx.symbolic_trace(model, meta_args = {'x': x})
-        >>> interp = ShapeProp(gm)
-        >>> interp.propagate(x)
+import torch.distributed as dist
+from torch import Tensor
+from torch.distributed import ProcessGroup
+
+# TODO: Remove the toggle-enable_nccl_base_collectives when github open issue #801 is resolved.
+if os.getenv("ENABLE_NCCL_BASE_COLLECTIVES", "1") == "0":
+    enable_nccl_base_collectives = False
+else:
+    enable_nccl_base_collectives = True
+
+
+class Bucket:
+
+    def __init__(self, shard_size: int, dtype: torch.dtype, device: torch.device, group: ProcessGroup):
+        self.buffer = torch.zeros((group.size(), shard_size), dtype=dtype, device=device)
+        self.group = group
+        self.offset = 0
+        self.callbacks: List[Callable] = []
+        self.output_shard = torch.zeros_like(self.buffer[0])
+
+    def flush(self) -> None:
+        """Flush content of the bucket."""
+        if self.offset == 0:
+            assert len(self.callbacks) == 0
+            return
+        # reduce-scatter bucket
+        if hasattr(dist, "_reduce_scatter_base") and enable_nccl_base_collectives:
+            dist._reduce_scatter_base(self.output_shard[:self.offset],
+                                      self.buffer[:, :self.offset].contiguous(),
+                                      group=self.group)
+        else:
+            dist.reduce_scatter(self.output_shard[:self.offset],
+                                list(self.buffer[:, :self.offset].unbind(0)),
+                                group=self.group)
+        # execute post-reduction callbacks
+        for callback_fn in self.callbacks:
+            callback_fn()
+        # reuse input bucket but allocate a fresh output shard
+        self.buffer[:, :self.offset].zero_()
+        self.offset = 0
+        self.callbacks.clear()
+        self.output_shard = torch.zeros_like(self.buffer[0])
+
+    def alloc(self) -> None:
+        """Setup the buffers if they are not allocated.
+
+        Using ``setup`` and ``teardown``, we can ensure that the bucket
+        buffers are only allocated during the backward pass, hence saving more
+        memory to other parts of the training process, such as the forward pass
+        for activation memory.
+        """
+        for tensor in [self.buffer, self.output_shard]:
+            if tensor.storage().size() == 0:
+                tensor.storage().resize_(tensor.size().numel())
+
+    def free(self) -> None:
+        """Tear down the bucket by freeing the memory"""
+        assert self.offset == 0 and self.callbacks == [], "Incorrect call of teardown"
+        for tensor in [self.buffer, self.output_shard]:
+            tensor.storage().resize_(0)
+
+    def append(self, tensor_list: List[Tensor], callback_fn: Callable):
+        # copy data from input_list into bucket
+        tensor_size = tensor_list[0].numel()
+        stacked_input = torch.stack(tensor_list).view(self.group.size(), tensor_size)
+        offset = self.offset
+        self.buffer[:, offset:offset + tensor_size].copy_(stacked_input)
+        self.offset += tensor_size
+
+        # callback will be given the reduced result
+        if callback_fn is not None:
+            result_view = self.output_shard[offset:offset + tensor_size].view_as(tensor_list[0])
+            self.callbacks.append(functools.partial(callback_fn, result_view))
+
+
+class ReduceScatterBucketer:
+    """
+    Helper for bucketing multiple reduce-scatter operations on small tensors
+    into larger reduce-scatter ops to improve communication efficiency.
+
+    Usage::
+
+        bucketer = ReduceScatterBucketer()
+        bucketer.reduce_scatter_async(
+            small_tensors, callback_fn=lambda result: print("small")
+        )
+        bucketer.reduce_scatter_async(
+            big_tensors, callback_fn=lambda result: print("big")
+        )
+        bucketer.reduce_scatter_async(
+            more_small_tensors, callback_fn=lambda result: print("small2")
+        )
+        bucketer.flush()  # callbacks only guaranteed to be called after flush()
+        # Example output (note that it is out of order, due to bucketing):
+        # big
+        # small
+        # small2
 
     Args:
-        module (GraphModule): The module to be executed
-
-    Hints:
-        If you want to add a new shape propagation rule, you can do so by
-        adding a new method to this class with the ``@register_shape_impl``
-        decorator. The method should take (*args, **kwargs) instance as its
-        input and generate output.
-
-        For example, if you want to add a shape propagation rule for
-        ``torch.nn.functional.linear``, you can do so by adding a new method
-        to this class with the ``@register_shape_impl`` decorator (Since the
-        ``MetaTensorMode`` is compatible with ``torch.nn.functional.linear``,
-        in practice you don't have to do as follows):
-
-        >>> @register_shape_impl(torch.nn.functional.linear)
-        >>> def linear_shape_impl(*args, **kwargs):
-        >>>     # do something here
-        >>>     return torch.empty(output_shape, device=output_device)
+        bucket_size_mb (int, Optional): bucket size for communicating. Buckets
+            are sub-divided based on world_size. Values <= 0 disable bucketing.
     """
-    _custom_dispatch_func = {}
-    _mode = MetaTensorMode()
 
-    def __init__(self, module: torch.fx.GraphModule, garbage_collect_values: bool = True):
-        super().__init__(module, garbage_collect_values)
-        self.global_hook = sim_env(module=self.module)
+    def __init__(self, bucket_size_mb: int = 25):
+        self.bucket_size_mb = bucket_size_mb
+        self.buckets: Dict[Tuple[torch.dtype, torch.device, ProcessGroup], Bucket] = {}
+
+    @torch.no_grad()
+    def reduce_scatter_async(
+        self,
+        input_list: List[Tensor],
+        group: ProcessGroup,
+        callback_fn: Optional[Callable] = None,
+    ) -> None:
+        """
+        Reduce-scatter a list of tensors asynchronously, so smaller reductions
+        can be bucketed together. The given callback (``callback_fn``) will be
+        called with the reduced result at some later time. Call ``flush()`` to
+        force all queued ops and callbacks to be executed.
 
-    def run_node(self, n: torch.fx.Node) -> Any:
-        """
-        Run a specific node ``n`` and return the result. Attach
-        (
-            ``inputs``, ``outputs``, ``parameters``, ``buffers``
-        ) to ``n``.
+        Note that large inputs will be reduced immediately, and this function
+        may also flush the relevant bucket to make room for ``input_list``.
 
         Args:
-            n (Node): The ``Node`` to execute
-
-        Returns:
-            Any: The result of executing ``n``
-        """
-        args, kwargs = self.fetch_args_kwargs_from_env(n)
-        with self.global_hook:
-            r = getattr(self, n.op)(n.target, args, kwargs)
-
-        def unwrap_fn(elem):
-
-            def _convert_meta(t: torch.Tensor):
-                if t.device == 'meta':
-                    return t
-                else:
-                    return t.to('meta')
-
-            if isinstance(elem, MetaTensor):
-                if getattr(self, '_is_param', False):
-                    return torch.nn.Parameter(_convert_meta(elem._tensor))
-                return _convert_meta(elem._tensor)
-
-            elif isinstance(elem, torch.Tensor):
-                if isinstance(elem, torch.nn.Parameter):
-                    return torch.nn.Parameter(_convert_meta(elem))
-                return _convert_meta(elem)
-
+            input_list (List[Tensor]): list of tensors to reduce-scatter. List
+                should contain ``group.size()`` tensors and each tensor should
+                have identical shape, dtype and device.
+            group (ProcessGroup): process group for reduction
+            callback_fn (Callable, Optional): callback function to call after
+                the reduction executes. Function will be called with a single
+                argument corresponding to the reduced result.
+        """
+        world_size = group.size()
+
+        assert (len(input_list) == world_size
+               ), f"reduce_scatter received {len(input_list)} inputs, expected group.size() ({world_size})"
+
+        first_input = input_list[0]
+        first_input_size = first_input.numel()
+
+        bucket_shard_size = self._get_shard_size(first_input.element_size(), world_size)
+        if first_input_size > bucket_shard_size:
+            # TODO: investigate how to avoid using torch.cat (because it seems to be slow for CPU tensors)
+            # input is too big to fit in the bucket, reduce-scatter directly
+            output = torch.zeros_like(input_list[0])
+            if hasattr(dist, "_reduce_scatter_base") and enable_nccl_base_collectives:
+                input_flattened = torch.cat(input_list)
+                dist._reduce_scatter_base(output, input_flattened, group=group)
             else:
-                return elem
-
-        is_pure_tensor = lambda elem: isinstance(elem, MetaTensor) and not isinstance(elem, torch.nn.Parameter)
-        n_info = MetaInfo(n)
-        n_info.outputs = _normalize_tuple(r)
-
-        if n.op == 'call_module':
-            submod = self.fetch_attr(n.target)
-            n_info.parameters.update({k: MetaTensor(v) for k, v in submod.named_parameters()})
-            n_info.buffers.update({k: MetaTensor(v) for k, v in submod.named_buffers()})
-
-        else:
-            n_info.parameters.update({
-                k.name: MetaTensor(v)
-                for k, v in zip(n.args, args)
-                if isinstance(k, torch.fx.Node) and isinstance(v, torch.nn.Parameter)
-            })
-            n_info.parameters.update({k: MetaTensor(v) for k, v in kwargs.items() if isinstance(v, torch.nn.Parameter)})
-
-        n_info.inputs = tuple(v for v in args if is_pure_tensor(v)) + \
-                        tuple(v for v in kwargs.values() if is_pure_tensor(v))
-
-        # align with SPMD
-        if isinstance(r, (tuple, list)):
-            n._meta_data = tree_map(unwrap_fn, _normalize_tuple(r))
-        else:
-            n._meta_data = unwrap_fn(r)
-
-        n_info.global_ctx = self.global_hook.ctx
-        n_info.curr_ctx = self.global_hook.ctx.copy()
-
-        crit = lambda x: x.data_ptr() in self.global_hook.ctx if isinstance(x, torch.Tensor) else False
-        n_info.is_alias = _normalize_tuple(tree_map(crit, n_info.outputs))
-        return r
-
-    def call_function(self, target: 'Target', args: Tuple[Any, ...], kwargs: Dict[str, Any]) -> Any:
-        """
-        Execute a ``call_function`` node and return the result.
-        If the target of ``Node`` is registered with ``@register_shape_impl``,
-        the registered function will be used to execute the node. This is common
-        if we insert some customized kernels.
-
-        Args:
-            target (Target): The call target for this node. See
-                `Node <https://pytorch.org/docs/master/fx.html#torch.fx.Node>`__ for
-                details on semantics
-            args (Tuple): Tuple of positional args for this invocation
-            kwargs (Dict): Dict of keyword arguments for this invocation
-
-        Return
-            Any: The value returned by the function invocation
-        """
-        convert_to_param = False
-        if target in (torch.transpose, torch.reshape) and isinstance(args[0], torch.nn.parameter.Parameter):
-            convert_to_param = True
-        if target in self._custom_dispatch_func:
-            res = self._custom_dispatch_func[target](*args, **kwargs)
-        else:
-            res = super().call_function(target, args, kwargs)
-        if convert_to_param:
-            return torch.nn.Parameter(res)
-        else:
-            return res
-
-    def call_method(self, target: 'Target', args: Tuple[Any, ...], kwargs: Dict[str, Any]) -> Any:
-        """
-        Execute a ``call_method`` node and return the result.
-
-        Args:
-            target (Target): The call target for this node. See
-                `Node <https://pytorch.org/docs/master/fx.html#torch.fx.Node>`__ for
-                details on semantics
-            args (Tuple): Tuple of positional args for this invocation
-            kwargs (Dict): Dict of keyword arguments for this invocation
-
-        Return
-            Any: The value returned by the method invocation
-        """
-        # args[0] is the `self` object for this method call
-        self_obj, *args_tail = args
-
-        target_method = getattr(self_obj.__class__, target)
-
-        convert_to_parameter = False
-        if target_method in (torch.Tensor.view, torch.Tensor.transpose) and isinstance(
-                args[0], torch.nn.parameter.Parameter):
-            convert_to_parameter = True
-        # Execute the method and return the result
-        assert isinstance(target, str)
-        res = getattr(self_obj, target)(*args_tail, **kwargs)
-        if convert_to_parameter:
-            return torch.nn.Parameter(res)
-        else:
-            return res
-
-    def propagate(self, *args, device=None):
-        """
-        Run `module` via interpretation and return the result and record the
-        shape of each node.
-        Args:
-            *args (Tensor): The sample input.
-        Returns:
-            Any: The value returned from executing the Module
-        """
-
-        # wrap_fn = lambda elem: MetaTensor(elem, device=device)
-        def wrap_fn(elem, device=device):
-            if isinstance(elem, torch.Tensor):
-                return MetaTensor(elem, device=device)
-            else:
-                return elem
-
-        with self._mode:
-            return super().run(*tree_map(wrap_fn, args))
-
-
-def shape_prop_pass(module: torch.fx.GraphModule, *args) -> torch.fx.GraphModule:
-    """
-    Run ``module`` via interpretation and return the result and record the
-    shape of each ``Node``.
-
-    Args:
-        module (GraphModule): The GraphModule to profile
-        *args (Any): The sample input
-
-    Returns:
-        GraphModule: The same GraphModule with shape information
-    """
-
-    ShapeProp(module).propagate(*args, device=_current_device(module))
-    return module
+                # fallback
+                dist.reduce_scatter(output, input_list, group=group)
+            if callback_fn is not None:
+                callback_fn(output)
+            return
+
+        bucket = self._get_bucket(first_input, group)
+        if first_input_size > bucket.buffer.size(1) - bucket.offset:
+            # not enough space remaining in bucket, flush it now
+            bucket.flush()
+        bucket.append(input_list, callback_fn)
+
+    @torch.no_grad()
+    def flush(self) -> None:
+        """Reduce-scatter any partial buckets."""
+        for bucket in self.buckets.values():
+            bucket.flush()
+
+    @torch.no_grad()
+    def free(self) -> None:
+        """Free buffers from all buckets."""
+        for bucket in self.buckets.values():
+            bucket.free()
+
+    @functools.lru_cache()
+    def _get_shard_size(self, element_size: int, num_shards: int) -> int:
+        if self.bucket_size_mb <= 0:    # Values <= 0 disable bucketing.
+            return 0
+        MB = 1024 * 1024
+        bucket_size = self.bucket_size_mb * MB / element_size
+        return int(bucket_size // num_shards)
+
+    def _get_bucket(self, tensor: Tensor, group: ProcessGroup) -> Bucket:
+        key = (tensor.dtype, tensor.device, group)
+        if key not in self.buckets:
+            # buckets are divided into world_size pieces, bucket.data shaped (world_size, shard_size)
+            world_size = group.size()
+            shard_size = self._get_shard_size(tensor.element_size(), world_size)
+            self.buckets[key] = Bucket(shard_size, tensor.dtype, tensor.device, group)
+        self.buckets[key].alloc()
+        return self.buckets[key]
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/_analyzer/fx/tracer/custom_leaf_module.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/normalization.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import torch
 
-from .tracer import register_leaf_module, register_leaf_module_impl
+from ...registry import meta_patched_module
 
-try:
-    import apex
-    register_leaf_module(apex.normalization.FusedLayerNorm)
-    register_leaf_module(apex.normalization.FusedRMSNorm)
-    register_leaf_module(apex.normalization.MixedFusedLayerNorm)
-    register_leaf_module(apex.normalization.MixedFusedRMSNorm)
-
-    @register_leaf_module_impl(apex.normalization.FusedLayerNorm)
-    @register_leaf_module_impl(apex.normalization.FusedRMSNorm)
-    @register_leaf_module_impl(apex.normalization.MixedFusedLayerNorm)
-    @register_leaf_module_impl(apex.normalization.MixedFusedRMSNorm)
-    def torch_nn_normalize(self, input: torch.Tensor):
-        # check shape
-        if isinstance(self, torch.nn.BatchNorm1d):
-            assert input.dim() in [2, 3]
-        elif isinstance(self, torch.nn.BatchNorm2d):
-            assert input.dim() == 4
-        elif isinstance(self, torch.nn.BatchNorm3d):
-            assert input.dim() == 5
 
-        # normalization maintain the same shape as the input
-        return input.clone()
+@meta_patched_module.register(torch.nn.LayerNorm)
+@meta_patched_module.register(torch.nn.GroupNorm)
+@meta_patched_module.register(torch.nn.BatchNorm1d)
+@meta_patched_module.register(torch.nn.BatchNorm2d)
+@meta_patched_module.register(torch.nn.BatchNorm3d)
+def torch_nn_normalize(self, input):
+    # check shape
+    if isinstance(self, torch.nn.BatchNorm1d):
+        assert input.dim() in [2, 3]
+    elif isinstance(self, torch.nn.BatchNorm2d):
+        assert input.dim() == 4
+    elif isinstance(self, torch.nn.BatchNorm3d):
+        assert input.dim() == 5
+
+    # normalization maintain the same shape as the input
+    return input.clone()
 
+
+try:
+    import apex
+    meta_patched_module.register(apex.normalization.FusedLayerNorm)(torch_nn_normalize)
+    meta_patched_module.register(apex.normalization.FusedRMSNorm)(torch_nn_normalize)
+    meta_patched_module.register(apex.normalization.MixedFusedLayerNorm)(torch_nn_normalize)
+    meta_patched_module.register(apex.normalization.MixedFusedRMSNorm)(torch_nn_normalize)
 except (ImportError, AttributeError):
     pass
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/amp/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/amp/apex_amp/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/amp/apex_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/amp/apex_amp/apex_amp.py` & `colossalai-nightly-2023.5.6/colossalai/amp/apex_amp/apex_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/amp/naive_amp/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/amp/naive_amp/_fp16_optimizer.py` & `colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/_fp16_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/amp/naive_amp/_utils.py` & `colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py` & `colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py` & `colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py` & `colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/amp/naive_amp/naive_amp.py` & `colossalai-nightly-2023.5.6/colossalai/amp/naive_amp/naive_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/amp/torch_amp/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/amp/torch_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/amp/torch_amp/_grad_scaler.py` & `colossalai-nightly-2023.5.6/colossalai/amp/torch_amp/_grad_scaler.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
                     # TODO: is there a way to split by device and dtype without appending in the inner loop?
                     per_device_and_dtype_grads[to_unscale.device][to_unscale.dtype].append(to_unscale)
 
             for device, per_dtype_grads in per_device_and_dtype_grads.items():
                 for grads in per_dtype_grads.values():
                     torch._amp_foreach_non_finite_check_and_unscale_(grads, per_device_found_inf.get(device),
                                                                      per_device_inv_scale.get(device))
-        # For tensor parallel parameters it should be all-reduced over tensor parallel process group
+        # For tensor parallel paramters it should be all-reduced over tensor parallel process group
         if gpc.is_initialized(ParallelMode.MODEL) and gpc.get_world_size(ParallelMode.MODEL) > 1:
             vals = [val for val in per_device_found_inf._per_device_tensors.values()]
             coalesced = _flatten_dense_tensors(vals)
             dist.all_reduce(coalesced, op=dist.ReduceOp.MAX, group=gpc.get_group(ParallelMode.MODEL))
             for buf, synced in zip(vals, _unflatten_dense_tensors(coalesced, vals)):
                 buf.copy_(synced)
         return per_device_found_inf._per_device_tensors
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/amp/torch_amp/torch_amp.py` & `colossalai-nightly-2023.5.6/colossalai/amp/torch_amp/torch_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/checkpoint/operation.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/checkpoint/operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
             for (shape_0, shape_1) in zip(input_tensors[0].shape[:-2], input_tensors[1].shape[:-2]):
                 if shape_0 != shape_1:
                     _is_batch_dims_same = False
                     break
         else:
             _is_batch_dims_same = False
 
-        # retrieve dimensions
+        # retireve dimensions
         input_dim_00 = input_tensors[0].shape[-2]
         input_dim_01 = input_tensors[0].shape[-1]
         input_dim_10 = input_tensors[1].shape[-2]
         input_dim_11 = input_tensors[1].shape[-1]
         output_dim_0 = output_tensors[0].shape[-2]
         output_dim_1 = output_tensors[0].shape[-1]
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/meta_registry/where.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/meta_registry/where.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/registry.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/meta_profiler/shard_metainfo.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/meta_profiler/shard_metainfo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/amp_optimizer.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/amp_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/base_offload_module.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/base_offload_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/mem_optimize.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/mem_optimize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/region.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/region.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/region_manager.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/region_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/runtime.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/runtime.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/solver.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/solver.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/training_simulator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/training_simulator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/offload/util.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/offload/util.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/passes/comm_metainfo_pass.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/comm_metainfo_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/passes/meta_info_prop.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/meta_info_prop.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
                 self._set_data_ptr(tensor)
 
         # attach them to graph_info
         graph_info.fwd_in = input_tensors
         graph_info.fwd_tmp = buffer_tensors
         graph_info.fwd_out = output_tensors
 
-        # fetch other memory information
+        # fetch other memory informations
         memory_cost = meta_info.memory_cost
         graph_info.fwd_mem_tmp = memory_cost.fwd.temp
         graph_info.fwd_mem_out = memory_cost.fwd.activation
         graph_info.bwd_mem_tmp = memory_cost.bwd.temp
         graph_info.bwd_mem_out = memory_cost.bwd.activation
 
         # fetch flop information
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/passes/runtime_apply_pass.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/runtime_apply_pass.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
                 MetaInfo(comm_spec_apply_node,
                          mod_dir=node.meta['info'].mod_dir,
                          activation_checkpoint=tuple(node.meta['info'].activation_checkpoint))
 
     return gm
 
 
-def _act_annotation_pass(gm: torch.fx.GraphModule):
+def _act_annotataion_pass(gm: torch.fx.GraphModule):
     """
     This pass is used to add the act annotation to the new inserted nodes.
     """
     mod_graph = gm.graph
     nodes = tuple(mod_graph.nodes)
 
     for node in nodes:
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/passes/runtime_preparation_pass.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/passes/runtime_preparation_pass.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                     total_shard_size *= device_mesh_info[shard_dim]
                 size[dim] = dim_size * total_shard_size
         size = torch.Size(size)
 
     return size
 
 
-def solution_annotation_pass(gm: torch.fx.GraphModule, solution: List[int],
+def solution_annotatation_pass(gm: torch.fx.GraphModule, solution: List[int],
                                strategies_constructor: StrategiesConstructor):
     """
     This method is used to stick the solution strategy to the nodes and add the information
     required in runtime into graph as placeholder nodes.
     """
     mod_graph = gm.graph
 
@@ -165,15 +165,15 @@
         return target_dim
 
     def _post_processing(node, size_processing_node):
         '''
         This function is used to process the dependency between the size node and its users after
         inserting the size_process_node.
         '''
-        # store original node and processing node pair in node_pairs dictionary
+        # store original node and processing node pair in node_pairs dictioanry
         # It will be used to replace the original node with processing node in slice object
         node_pairs[node] = size_processing_node
         size_processing_node._meta_data = node._meta_data
 
         if hasattr(node.meta['info'], 'activation_checkpoint'):
             MetaInfo(size_processing_node,
                      mod_dir=node.meta['info'].mod_dir,
@@ -384,15 +384,15 @@
 def module_params_sharding_pass(gm: torch.fx.GraphModule, device_mesh: DeviceMesh, overlap=False):
     """
     Apply the sharding action to the module parameters and buffers following the
     instructions of solver solution.
     """
     mod_graph = gm.graph
     nodes = tuple(mod_graph.nodes)
-    # This stream is created for overlapping the communication and computation.
+    # This stream is created for overlaping the communication and computation.
     reduction_stream = torch.cuda.Stream()
 
     def _add_hook_for_grad_communication(node, param, name=None):
 
         comm_actions = node.best_strategy.communication_actions
 
         def _filter_param_to_hook(node, op_data, comm_action, name):
@@ -492,15 +492,15 @@
 
 
 def runtime_preparation_pass(gm: torch.fx.GraphModule,
                              solution: List[int],
                              device_mesh: DeviceMesh,
                              strategies_constructor: StrategiesConstructor,
                              overlap=False):
-    gm, sharding_spec_convert_dict, origin_node_sharding_spec_dict, comm_actions_dict = solution_annotation_pass(
+    gm, sharding_spec_convert_dict, origin_node_sharding_spec_dict, comm_actions_dict = solution_annotatation_pass(
         gm, solution, strategies_constructor)
     gm = size_value_converting_pass(gm, device_mesh)
     gm = node_args_converting_pass(gm, device_mesh)
     # TODO: the pass below should be uncommented after the implementation of implicit_comm_action_apply_pass completed.
     # gm = implicit_comm_action_apply(gm)
     gm = module_params_sharding_pass(gm, device_mesh, overlap=overlap)
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/constants.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/initialize.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         return mapping
 
     def post_process(self, strategy: ShardingStrategy) -> Union[ShardingStrategy, List[ShardingStrategy]]:
         """
         Convert the sharding spec from the logical shape to the physical shape.
         """
         # create multiple sharding strategies for the inputs
-        # as input can be multi-dimensional and the partition dim is only 2D,
+        # as input can be multi-dimensinal and the partition dim is only 2D,
         # we need to map the partition at logical dim 0 to one of the first few dimensions of the input and output
         strategies = _convert_logical_sharding_to_physical_sharding_spec_for_embedding(strategy=strategy,
                                                                                        input_name=str(
                                                                                            self.node.args[0]),
                                                                                        output_name=str(self.node))
         return strategies
 
@@ -217,14 +217,14 @@
         return mapping
 
     def post_process(self, strategy: ShardingStrategy):
         """
         Convert the sharding spec from the logical shape to the physical shape.
         """
         # create multiple sharding strategies for the inputs
-        # as input can be multi-dimensional and the partition dim is only 2D,
+        # as input can be multi-dimensinal and the partition dim is only 2D,
         # we need to map the partition at logical dim 0 to one of the first few dimensions of the input and output
         strategies = _convert_logical_sharding_to_physical_sharding_spec_for_embedding(strategy=strategy,
                                                                                        input_name=str(
                                                                                            self.node.args[0]),
                                                                                        output_name=str(self.node))
         return strategies
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 __all__ = ['LinearModuleHandler', 'LinearFunctionHandler']
 
 
 def _update_sharding_spec_for_transposed_weight_for_linear(strategy: ShardingStrategy,
                                                            weight_name: str) -> ShardingStrategy:
     """
     This function is a helper function used by both module node handler and function node handler. This function will
-    convert the sharding spec for the transposed weight to the correct partition spec.
+    convert the sharding spec for the transposed weight to the correct partititon spec.
 
     Args:
         strategy (ShardingStrategy): the strategy generated by the strategy generator.
         weight_name (str): the name of the OperationData object for the weight.
     """
     # switch the dimensions of the transposed weight
     sharding_spec = strategy.get_sharding_spec_by_name(weight_name)
@@ -193,15 +193,15 @@
         1. the sharding spec is updated for the transposed weight
         2. the input and output sharding specs are updated to physical shape.
         """
         # switch the dimensions of the transposed weight
         strategy = _update_sharding_spec_for_transposed_weight_for_linear(strategy=strategy, weight_name='weight')
 
         # create multiple sharding strategies for the inputs
-        # as input can be multi-dimensional and the partition dim is only 2D,
+        # as input can be multi-dimensinal and the partition dim is only 2D,
         # we need to map the partition at dim 0 to one of the first few dimensions of the input
         strategies = _convert_logical_sharding_to_physical_sharding_spec_for_linear(strategy=strategy,
                                                                                     input_name=str(self.node.args[0]),
                                                                                     output_name=str(self.node))
         return strategies
 
 
@@ -263,13 +263,13 @@
         return mapping
 
     def post_process(self, strategy: ShardingStrategy):
         # switch the dimensions of the transposed weight
         strategy = _update_sharding_spec_for_transposed_weight_for_linear(strategy=strategy,
                                                                           weight_name=str(self.node.args[1]))
         # create multiple sharding strategies for the inputs
-        # as input can be multi-dimensional and the partition dim is only 2D,
+        # as input can be multi-dimensinal and the partition dim is only 2D,
         # we need to map the partition at dim 0 to one of the first few dimensions of the input
         strategies = _convert_logical_sharding_to_physical_sharding_spec_for_linear(strategy=strategy,
                                                                                     input_name=str(self.node.args[0]),
                                                                                     output_name=str(self.node))
         return strategies
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 
 
 def get_matmul_type(input_dim: int, other_dim: int):
     """
     Determine which type of matmul operation should be executed for the given tensor dimensions.
 
     Args:
-        input_dim (int): the number of dimensions for the input tensor
-        other_dim (int): the number of dimensions for the other tensor
+        input_dim (int): the number of dimensions for the input tenosr
+        other_dim (int): the number of dimensions for the other tenosr
     """
     if input_dim == 1 and other_dim == 1:
         matmul_type = MatMulType.DOT
     elif input_dim in [1, 2] and other_dim == 2:
         matmul_type = MatMulType.MM
     elif input_dim == 2 and other_dim == 1:
         matmul_type = MatMulType.MV
@@ -202,15 +202,15 @@
             for dim_idx, broadcast_type in self.broadcast_dim_info[key].items():
                 if broadcast_type == BroadcastType.MULTIPLE:
                     # if the dim is originally 1 and multiplied during broadcast
                     # we set its sharding to R
                     # e.g. [1, 2, 4] x [4, 4, 8] -> [4, 2, 8]
                     # the dim 0 of [1, 2, 4] is multiplied to 4
                     tensor_shape[dim_idx] = 1
-                elif broadcast_type == BroadcastType.PADDING:
+                elif broadcast_type == BroadcastType.PADDDING:
                     # if the dim is padded
                     # we remove its sharding
                     tensor_shape[dim_idx] = None
 
             tensor_shape_before_broadcast = [dim for dim in tensor_shape if dim is not None]
 
             physical_sharding_spec, removed_dims = recover_sharding_spec_for_broadcast_shape(
@@ -264,21 +264,21 @@
             Map the logical batch dim to the physical batch dim
             """
             op_data = op_data_mapping[key]
             sharding_spec = strategy.get_sharding_spec_by_name(op_data.name)
             dim_partition_dict = sharding_spec.dim_partition_dict
             entire_shape = sharding_spec.entire_shape
 
-            # update the dimension index for the matrix dimensions
+            # upddate the dimension index for the matrix dimensions
             if 2 in dim_partition_dict:
                 dim_partition_dict[len(self.batch_dims_before_view) + 1] = dim_partition_dict.pop(2)
             if 1 in dim_partition_dict:
                 dim_partition_dict[len(self.batch_dims_before_view)] = dim_partition_dict.pop(1)
 
-            # map the logical batch dim to physical batch dim
+            # map the logical batch dim to phyiscal batch dim
             if 0 in dim_partition_dict:
                 batch_dim_shard = dim_partition_dict.pop(0)
                 dim_partition_dict[physical_batch_dim] = batch_dim_shard
 
             # the new shape will be the batch dims + the last 2 matrix dims
             shape_before_view = self.batch_dims_before_view + list(entire_shape[-2:])
             sharding_spec.__init__(sharding_spec.device_mesh, shape_before_view, dim_partition_dict)
@@ -410,15 +410,15 @@
         """
         The operands for the dot operation have the same logical shape as the physical shape
         """
         return None, None, None
 
     def _get_logical_shape_for_mm(self):
         """
-        We need to handle the input tensor for a matrix-matrix multiplication as the input
+        We need to handle the input tensor for a matrix-matrix multiplcation as the input
         tensor can be a 1D or 2D tensor. If it is a 1D tensor, 1 will be prepended to its shape
         (e.g. [4] -> [1, 4]).
         """
         if self.input_meta_data.dim() == 1:
             input_logical_shape = [1] + list(self.input_meta_data.shape)
             input_logical_shape = torch.Size(input_logical_shape)
         else:
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             assert hasattr(node, 'strategies_vector'), \
                 f'The predecessor node {node_name} has no strategy vector to compute the resharding cost.'
             prev_strategy_vector = node.strategies_vector
             prev_sharding_specs = [
                 prev_strategy.get_sharding_spec_by_name(node_name) for prev_strategy in prev_strategy_vector
             ]
 
-            # create data structure to store costs
+            # create data structrure to store costs
             if node not in resharding_costs:
                 resharding_costs[node] = []
 
             def _compute_resharding_cost(
                     prev_sharding_spec: Union[ShardingSpec,
                                               List[ShardingSpec]], current_sharding_spec: Union[ShardingSpec,
                                                                                                 List[ShardingSpec]],
@@ -208,15 +208,15 @@
 
         for strategy in remove_strategy_list:
             self.strategies_vector.remove(strategy)
 
         return self.strategies_vector
 
     def post_process(self, strategy: ShardingStrategy) -> Union[ShardingStrategy, List[ShardingStrategy]]:
-        # transform the strategy generated
+        # tranform the strategy generated
         # e.g. to process the sharding strategy for the transposed weights
         return strategy
 
     @abstractmethod
     def get_strategy_generator(self) -> List[StrategyGenerator]:
         """
         Define which generators should be used by this NodeHandler object.
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/registry.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 class BatchNormStrategyGenerator(StrategyGenerator):
     """
     A StrategyGenerator which deals with the sharding strategies of batch normalization.
 
     To keep the math consistency, there are two way to do BatchNorm if the input
     shards on batch dimension:
     1. We gather the input partitions through batch dimension, then do the normal BatchNorm.
-    2. We do the SyncBatchNorm on the each input partition separately, the SyncBN op will help
+    2. We do the SyncBatchNorm on the each input partition seperately, the SyncBN op will help
        us to keep the computing correctness.
     In this generator, both methods will be considered.
     """
 
     def validate(self) -> bool:
         '''
         In sanity check, we need make sure the input data having correct dimension size.
@@ -40,15 +40,15 @@
         assert input_op_data.data.dim() in (
             3, 4, 5), f'We suppose the dim of input fed into conv op should in range of [3, 5].'
 
     def update_compute_cost(self, strategy: ShardingStrategy):
         '''
         Compute the computation cost per device with this specific strategy.
 
-        Note: compute_cost need to be divided by TFLOPS, now it just shows the computation size.
+        Note: compute_cost need to be devided by TFLOPS, now it just shows the computation size.
         '''
         # TODO: a constant coefficient need to be added.
         # 1D: (L) * N * Cin
         # 2D: (H * W) * N  * Cin
         # 3D: (H * W  * D) * N  * Cin
         sharded_input_shape = strategy.sharding_specs[self.op_data['input']].get_sharded_shape_per_device()
         sharded_output_shape = strategy.sharding_specs[self.op_data['output']].get_sharded_shape_per_device()
@@ -208,15 +208,15 @@
         if self.has_bias:
             dim_partition_dict_mapping["bias"] = {}
 
         sharding_spec_mapping = self.to_sharding_spec_mapping(dim_partition_dict_mapping)
 
         # set communication action
         # For SyncBN case, we don't need to do communication for weight and bias.
-        # TODO: the communication happens internally at SyncBN operation. We need to replace the BN operation
+        # TODO: the communication happens interally at SyncBN operation. We need to replace the BN operation
         # to SyncBN operation instead of inserting a communication node.
         output_comm_action = self.get_communication_action(
             sharding_spec=sharding_spec_mapping["output"],
             communication_pattern=CollectiveCommPattern.ALLREDUCE_FWD_IDENTITY_BWD,
             logical_process_axis=mesh_dim_0,
             comm_type=CommType.IMPLICIT)
 
@@ -246,15 +246,15 @@
         if self.has_bias:
             dim_partition_dict_mapping["bias"] = {}
 
         sharding_spec_mapping = self.to_sharding_spec_mapping(dim_partition_dict_mapping)
 
         # set communication action
         # For SyncBN case, we don't need to do communication for gradients of weight and bias.
-        # TODO: the communication happens internally at SyncBN operation. We need to replace the BN operation
+        # TODO: the communication happens interally at SyncBN operation. We need to replace the BN operation
         # to SyncBN operation instead of inserting a communication node.
         output_comm_action = self.get_communication_action(
             sharding_spec=sharding_spec_mapping["output"],
             communication_pattern=CollectiveCommPattern.ALLREDUCE_FWD_IDENTITY_BWD,
             logical_process_axis=[mesh_dim_0, mesh_dim_1],
             comm_type=CommType.IMPLICIT)
 
@@ -294,15 +294,15 @@
                 0: [mesh_dim_1],
             }
 
         sharding_spec_mapping = self.to_sharding_spec_mapping(dim_partition_dict_mapping)
 
         # set communication action
         # For SyncBN case, we don't need to do communication for gradients of weight and bias.
-        # TODO: the communication happens internally at SyncBN operation. We need to replace the BN operation
+        # TODO: the communication happens interally at SyncBN operation. We need to replace the BN operation
         # to SyncBN operation instead of inserting a communication node.
         output_comm_action = self.get_communication_action(
             sharding_spec=sharding_spec_mapping["output"],
             communication_pattern=CollectiveCommPattern.ALLREDUCE_FWD_IDENTITY_BWD,
             logical_process_axis=[mesh_dim_0],
             comm_type=CommType.IMPLICIT)
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     def update_memory_cost(self, strategy: ShardingStrategy) -> ShardingStrategy:
         # all input, output and outputs have the same shape
         shape = strategy.sharding_specs[self.op_data['input']].get_sharded_shape_per_device()
 
         # compute fwd memory cost in bytes
         # as the elementwise ops are not memory-intensive
-        # we approximate the fwd memory cost to be the output
+        # we approximate the fwd memroy cost to be the output
         # and the backward memory cost to be grad of input and other
         input_bytes = self._compute_size_in_bytes(strategy, 'input')
         other_bytes = self._compute_size_in_bytes(strategy, 'other')
         output_bytes = self._compute_size_in_bytes(strategy, 'output')
         fwd_memory_cost = MemoryCost(activation=output_bytes)
         bwd_memory_cost = MemoryCost(activation=input_bytes + other_bytes)
         total_memory_cost = MemoryCost(activation=input_bytes + other_bytes + output_bytes)
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,17 +34,17 @@
         assert input_op_data.data.dim() in (
             3, 4, 5), f'We suppose the dim of input fed into conv op should in range of [3, 5].'
 
     def update_compute_cost(self, strategy: ShardingStrategy):
         '''
         Compute the computation cost per device with this specific strategy.
 
-        Note: compute_cost need to be divided by TFLOPS, now it just shows the computation size.
+        Note: compute_cost need to be devided by TFLOPS, now it just shows the computation size.
         '''
-        # TODO: compute_cost need to be divided by TFLOPS, now it just shows the computation size.
+        # TODO: compute_cost need to be devided by TFLOPS, now it just shows the computation size.
         # 1D: (L) * N * Cout * Cin * kernel
         # 2D: (H * W) * N * Cout * Cin * kernel
         # 3D: (H * W  * D) * N * Cout * Cin * kernel
         sharded_input_shape = strategy.sharding_specs[self.op_data['input']].get_sharded_shape_per_device()
         sharded_other_shape = strategy.sharding_specs[self.op_data['other']].get_sharded_shape_per_device()
         sharded_output_shape = strategy.sharding_specs[self.op_data['output']].get_sharded_shape_per_device()
         if self.has_bias:
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     def validate(self) -> bool:
         return super().validate()
 
     def update_compute_cost(self, strategy: ShardingStrategy):
         '''
         Compute the computation cost per device with this specific strategy.
 
-        Note: compute_cost need to be divided by TFLOPS, now it just shows the computation size.
+        Note: compute_cost need to be devided by TFLOPS, now it just shows the computation size.
         '''
-        # TODO: compute_cost need to be divided by TFLOPS, now it just shows the computation size.
+        # TODO: compute_cost need to be devided by TFLOPS, now it just shows the computation size.
         # TODO: a constant coefficient need to be added.
 
         sharded_input_shape = strategy.sharding_specs[self.op_data['input']].get_sharded_shape_per_device()
         sharded_weight_shape = strategy.sharding_specs[self.op_data['other']].get_sharded_shape_per_device()
         if self.has_bias:
             # bias add is an element wise operation, so the cost is equal to product of output shape.
             bias_compute_cost = reduce(operator.mul, sharded_weight_shape)
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .strategy_generator import StrategyGenerator
 
 
 class NormalPoolStrategyGenerator(StrategyGenerator):
     """
     NormalPoolStrategyGenerator is a generic class to generate strategies for pool operation like MaxPoolxd.
     The reason we call this normal pool is AvgPoolxd and MaxPoolxd are taking the kernel size element from image,
-    and reduce them depending on the operation type.
+    and reduce them depening on the operation type.
     """
 
     def validate(self) -> bool:
         '''
         In sanity check, we need make sure the input data having correct dimension size.
         For Pool1d, the dim of input data should be 3([N, C, L]).
         For Pool2d, the dim of input data should be 4([N, C, H, W]).
@@ -31,17 +31,17 @@
         assert input_op_data.data.dim() in (
             3, 4, 5), f'We suppose the dim of input fed into Pool op should in range of [3, 5].'
 
     def update_compute_cost(self, strategy: ShardingStrategy) -> TrainCycleItem:
         '''
         Compute the computation cost per device with this specific strategy.
 
-        Note: compute_cost need to be divided by TFLOPS, now it just shows the computation size.
+        Note: compute_cost need to be devided by TFLOPS, now it just shows the computation size.
         '''
-        # TODO: compute_cost need to be divided by TFLOPS, now it just shows the computation size.
+        # TODO: compute_cost need to be devided by TFLOPS, now it just shows the computation size.
         # 1D: (Lout) * N * C * kernel
         # 2D: (H * W) * N * Cout * Cin * kernel
         # 3D: (H * W  * D) * N * Cout * Cin * kernel
         sharded_output_shape = strategy.sharding_specs[self.op_data['output']].get_sharded_shape_per_device()
         sharded_input_shape = strategy.sharding_specs[self.op_data['input']].get_sharded_shape_per_device()
 
         kernel_size = self.op_data["other"].data
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,23 +221,23 @@
                 'sharding_spec of op_data should be a list of sharding specs if op_data.data is a tuple.'
             total_bytes = 0
             for index, sharding_spec in enumerate(strategy.sharding_specs[op_data]):
                 meta_data = op_data.data[index]
                 if isinstance(meta_data, torch.Tensor):
                     element_bytes = _compute_size_in_bytes_helper(sharding_spec, meta_data)
                 else:
-                    # if meta_data is not a tensor, we count the memory as 0
+                    # if meta_data is not a tensor, we count the memroy as 0
                     element_bytes = 0
                 total_bytes += element_bytes
 
         else:
             if isinstance(op_data.data, torch.Tensor):
                 total_bytes = _compute_size_in_bytes_helper(strategy.sharding_specs[op_data], op_data.data)
             else:
-                # if op_data.data is not a tensor, we count the memory as 0
+                # if op_data.data is not a tensor, we count the memroy as 0
                 total_bytes = 0
 
         return total_bytes
 
     def generate(self) -> List[ShardingStrategy]:
         """
         Generate all possible sharding strategies for this operation.
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/options.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/options.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/sharding_strategy.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/sharding_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class CostGraph:
     '''
     A graph data structure to simplify the edge cost graph. It has two main functions:
     1. To feed the quadratic resharding costs into solver, we need to linearize it. We build edge_cost in
     CostGraph, and it stored every combinations of strategies for a src-dst node pair in an 1D list.
     2. To reduce the searching space, we merge computationally-trivial operators, such as
-    element-wise operators, transpose, and reduction, into their following nodes. The merging information will
+    element-wise operators, transpose, and reduction, into their following nodes. The merging infomation will
     be given by the StrategiesVector depending on the type of target node and following nodes.
 
     Argument:
         leaf_strategies(List[StrategiesVector]): It stores StrategiesVector of every nodes on the graph.
         simplify(bool, optional): The generated cost graph will be simplified if it is true. (default to True)
     '''
 
@@ -86,15 +86,15 @@
 
             setattr(dst_node, 'parents', parent_nodes)
             setattr(dst_node, 'children', children_nodes)
 
             if self.simplify and strategies_vector.check_merge():
                 for followed_node in strategies_vector.predecessor_nodes:
                     # we only merge node pairs which src node has a tensor element inside.
-                    # This is necessary because the node without a tensor element inside will not
+                    # This is necessay because the node without a tensor element inside will not
                     # be assigned any strategy.
                     if _check_tensor_in_node(followed_node._meta_data):
                         self.merge_pair.append((followed_node, dst_node))
 
     def get_edge_cost(self, src_node, dst_node):
         return self.edge_costs[(src_node, dst_node)]
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,35 +79,35 @@
         """
         Return the Graph object associated with this analyser.
         """
         return self._graph
 
     def liveness_analysis(self) -> List[LiveStage]:
         """
-        Analyses the graph to obtain the variable liveness information. This function returns
+        Analyse the graph to obtain the variable liveness information. This function returns
         an ordered dictionary where the key is the compute stage ID and the value is a LivenessStage object.
         """
         compute_nodes = self.graph.nodes
         liveness_list = []
 
         # checked: record all variables created since the first stage
         # all: record the live variables only exist until the current stage.
-        #       this can be different from the `checked list`` as some variables may be destroyed prior to this stage.
+        #       this can be different from the `checked list`` as some varialbes may be destroyed prior to this stage.
         # unique: record the unique live variables only exist until the current stage.
         #       this is different from `all list` as some variables are duplicated.
         checked_variables = LiveVariableVector()
         all_live_variables = LiveVariableVector()
         unique_live_vars = LiveVariableVector()
 
         for idx, node in enumerate(compute_nodes):
             #############################
             # find new living variables #
             #############################
             # detect whether the current op is an in-place op
-            # if it is an in-place op, we would deem it as a duplicate var
+            # if it is an in-place op, we would deem it as a duplciate var
             is_inplace = False
             if node.op == 'call_function':
                 # check if this is an inplace op such as torch.nn.functional.relu(x, inplace=True)
                 if node.kwargs.get('inplace', False):
                     is_inplace = True
             elif node.op == 'call_module':
                 # to check if this is an inplace op such as torch.nn.Relu(inplace=True)
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/solver/solver.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                  verbose=False):
         '''
         Solver class will integrate information provided by the components and use ILP solver to find a possible optimal strategies combination for target computing graph.
         Argument:
             graph: The computing graph to be optimized.
             strategies_constructor: It will provide all the possible strategies for each node in the computing graph.
             cost_graph: A graph data structure to simplify the edge cost graph.
-            graph_analyser: graph_analyser will analyses the graph to obtain the variable liveness information, which will be used to generate memory constraints.
+            graph_analyser: graph_analyser will analyse the graph to obtain the variable liveness information, which will be used to generate memory constraints.
             memory_budget: Memory constraint for the solution.
             solution_numbers: If solution_numbers is larger than one, solver will us a serious of solutions based on different memory budget.
             memory_increasing_coefficient: If solution_numbers is larger than one, we will use this coefficient to generate new memory budget.
         '''
         self.graph = graph
         self.strategies_constructor = strategies_constructor
         self.cost_graph = cost_graph
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/utils/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/utils/broadcast.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/broadcast.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     'BroadcastType', 'is_broadcastable', 'get_broadcast_shape', 'recover_sharding_spec_for_broadcast_shape',
     'comm_actions_for_oprands'
 ]
 
 
 class BroadcastType(Enum):
     EQUAL = auto()
-    PADDING = auto()
+    PADDDING = auto()
     MULTIPLE = auto()
 
 
 def is_broadcastable(shape1: torch.Size, shape2: torch.Size) -> bool:
     """
     Check if two shapes are broadcastable to each other.
     """
@@ -65,26 +65,26 @@
 
     # track the dim and its broadcasting type
     logical_dim_broadcast_info = {}
 
     for i in range(logical_num_dims):
         # get the trailing dim size
         logical_dim_idx = logical_num_dims - i - 1
-        physical_dim_idx = physical_num_dims - i - 1
+        phyiscal_dim_idx = physical_num_dims - i - 1
         logical_dim_size = logical_shape[logical_dim_idx]
 
-        if physical_dim_idx >= 0:
-            physical_dim_size = physical_shape[physical_dim_idx]
+        if phyiscal_dim_idx >= 0:
+            physical_dim_size = physical_shape[phyiscal_dim_idx]
 
             if physical_dim_size == logical_dim_size:
                 logical_dim_broadcast_info[logical_dim_idx] = BroadcastType.EQUAL
             elif physical_dim_size == 1 and physical_dim_size != logical_dim_size:
                 logical_dim_broadcast_info[logical_dim_idx] = BroadcastType.MULTIPLE
         else:
-            logical_dim_broadcast_info[logical_dim_idx] = BroadcastType.PADDING
+            logical_dim_broadcast_info[logical_dim_idx] = BroadcastType.PADDDING
 
     return logical_dim_broadcast_info
 
 
 def recover_sharding_spec_for_broadcast_shape(logical_sharding_spec: ShardingSpec, logical_shape: torch.Size,
                                               physical_shape: torch.Size) -> ShardingSpec:
     """
@@ -113,15 +113,15 @@
     # generate the sharding spec for the physical shape
     physical_dim_partition = {}
     logical_dim_partition = logical_sharding_spec.dim_partition_dict
 
     for shape_dim, mesh_dim in logical_dim_partition.items():
         logical_broadcast_type = logical_dim_broadcast_info[shape_dim]
 
-        if logical_broadcast_type == BroadcastType.PADDING or logical_broadcast_type == BroadcastType.MULTIPLE:
+        if logical_broadcast_type == BroadcastType.PADDDING or logical_broadcast_type == BroadcastType.MULTIPLE:
             removed_dims.extend(mesh_dim)
         else:
             # get the corresponding physical dim
             physical_dim = physical_num_dims - (logical_num_dims - shape_dim)
             physical_dim_partition[physical_dim] = mesh_dim
 
     physical_sharding_spec = ShardingSpec(device_mesh=logical_sharding_spec.device_mesh,
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/utils/factory.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     Args:
         input_ (Union[Node, torch.Tensor]): the input can be a Node object or a PyTorch tensor. If a node is used, it will look for its meta data associated with this node.
         device_mesh (DeviceMesh): a DeviceMesh object which contains the meta information about the cluster.
         dim_partition_dict (Dict[int, List[int]]): a dictionary to specify the sharding specs, the key is the tensor dimension and the value is the mesh dimension for sharding.
     """
 
     if isinstance(input_, Node):
-        assert hasattr(input_, '_meta_data'), f'The given node has no attribute _meta_data'
+        assert hasattr(input_, '_meta_data'), f'The given node has no attribte _meta_data'
         meta_tensor = input_._meta_data
         assert meta_tensor is not None, "The given node's _meta_data attribute is None"
         shape = meta_tensor.shape
     elif isinstance(input_, torch.Tensor):
         shape = input_.shape
     else:
         raise TypeError(
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/utils/misc.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/misc.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/utils/reshape.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/reshape.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from typing import Dict, List, Tuple
 
 import torch
 
 
 class PreviousStatus(Enum):
     """
-    This class shows the status of previous comparison.
+    This class shows the status of previous comparision.
     """
     RESET = 0
-    # ORIGIN means the dimension size of original tensor is larger in the previous comparison.
+    # ORIGIN means the dimension size of original tensor is larger in the previous comparision.
     ORIGIN = 1
-    # TGT means the dimension size of target tensor is larger in the previous comparison.
+    # TGT means the dimension size of target tensor is larger in the previous comparision.
     TGT = 2
 
 
 def detect_reshape_mapping(origin_shape: torch.Size, tgt_shape: torch.Size) -> Dict[Tuple[int], Tuple[int]]:
     """
     This method is used to detect the reshape mapping between original tensor and target tensor.
 
@@ -87,15 +87,15 @@
 
             previous_label = PreviousStatus.RESET
 
         elif original_dimension_size > tgt_dimension_size:
             tgt_index += 1
 
             if previous_label == PreviousStatus.TGT:
-                # if the target dimension size is larger in the previous comparison, which means
+                # if the target dimension size is larger in the previous comparision, which means
                 # the origin dimension size has already accumulated larger than target dimension size, so
                 # we need to offload the origin dims and tgt dims into the reshape_mapping_dict.
                 reshape_mapping_dict[tuple(origin_dims)] = tuple(tgt_dims)
                 original_dimension_size = original_dimension_size // tgt_dimension_size
                 origin_dims = [origin_len - origin_index - 1]
                 tgt_dimension_size = tgt_shape[tgt_index]
                 tgt_dims = [tgt_len - tgt_index - 1, tgt_len - tgt_index]
@@ -107,15 +107,15 @@
                 tgt_dims.append(tgt_len - tgt_index - 1)
                 previous_label = PreviousStatus.ORIGIN
 
         else:
             origin_index += 1
 
             if previous_label == PreviousStatus.ORIGIN:
-                # if the origin element is larger in the previous comparison, which means
+                # if the origin element is larger in the previous comparision, which means
                 # the target element has already accumulated larger than origin element, so
                 # we need to offload the origin dims and tgt dims into the reshape_mapping_dict.
                 reshape_mapping_dict[tuple(origin_dims)] = tuple(tgt_dims)
                 tgt_dimension_size = tgt_dimension_size // original_dimension_size
                 tgt_dims = [tgt_len - tgt_index - 1]
                 original_dimension_size = origin_shape[origin_index]
                 origin_dims = [origin_len - origin_index - 1, origin_len - origin_index]
@@ -135,15 +135,15 @@
     """
     This method is used to check whether the reshape operation could implement without converting
     the input to fully replicated status.
 
     Rule:
         For a sharded dimension of input tensor, if it is not the minimum element of the input tuple,
         the function will return false.
-        To illustrate this issue, there are two cases to analyze:
+        To illustrate this issue, there are two cases to analyse:
         1. no sharded dims in the input tuple: we could do the reshape operation safely just as the normal
         operation without distributed tensor.
         2. sharded dims in the input tuple: the sharded dim must be the minimum element, then during shape
         consistency process, torch.cat will be implemented on the sharded dim, and everything after the sharded
         dim get recovered.
 
     Examples:
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/auto_parallel/tensor_shard/utils/sharding.py` & `colossalai-nightly-2023.5.6/colossalai/auto_parallel/tensor_shard/utils/sharding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/booster/accelerator.py` & `colossalai-nightly-2023.5.6/colossalai/booster/accelerator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/booster/mixed_precision/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from .bf16 import BF16MixedPrecision
 from .fp8 import FP8MixedPrecision
 from .fp16_apex import FP16ApexMixedPrecision
-from .fp16_naive import FP16NaiveMixedPrecision
 from .fp16_torch import FP16TorchMixedPrecision
 from .mixed_precision_base import MixedPrecision
 
 __all__ = [
     'MixedPrecision', 'mixed_precision_factory', 'FP16_Apex_MixedPrecision', 'FP16_Torch_MixedPrecision',
-    'FP32_MixedPrecision', 'BF16_MixedPrecision', 'FP8_MixedPrecision', 'FP16NaiveMixedPrecision'
+    'FP32_MixedPrecision', 'BF16_MixedPrecision', 'FP8_MixedPrecision'
 ]
 
 _mixed_precision_mapping = {
     'fp16': FP16TorchMixedPrecision,
     'fp16_apex': FP16ApexMixedPrecision,
-    'fp16_naive': FP16NaiveMixedPrecision,
     'bf16': BF16MixedPrecision,
     'fp8': FP8MixedPrecision
 }
 
 
 def mixed_precision_factory(mixed_precision_type: str) -> MixedPrecision:
     """
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/booster/mixed_precision/fp16_torch.py` & `colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/fp16_torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/booster/mixed_precision/mixed_precision_base.py` & `colossalai-nightly-2023.5.6/colossalai/booster/mixed_precision/mixed_precision_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/booster/plugin/dp_plugin_base.py` & `colossalai-nightly-2023.5.6/colossalai/booster/plugin/dp_plugin_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,27 +16,29 @@
     def __init__(self) -> None:
         super().__init__()
         assert dist.is_initialized(
         ), 'torch.distributed is not initialized, please use colossalai.launch to create the distributed environment'
         self.rank = dist.get_rank()
         self.world_size = dist.get_world_size()
 
-    def prepare_dataloader(self,
-                           dataset,
-                           batch_size,
-                           shuffle=False,
-                           seed=1024,
-                           drop_last=False,
-                           pin_memory=False,
-                           num_workers=0,
-                           **kwargs):
+    def prepare_train_dataloader(self,
+                                 dataset,
+                                 batch_size,
+                                 shuffle=False,
+                                 seed=1024,
+                                 drop_last=False,
+                                 pin_memory=False,
+                                 num_workers=0,
+                                 **kwargs):
         r"""
         Prepare a dataloader for distributed training. The dataloader will be wrapped by
         `torch.utils.data.DataLoader` and `torch.utils.data.DistributedSampler`.
 
+        Note:
+            1. Evaluation datasets should not be passed to this function.
 
         Args:
             dataset (`torch.utils.data.Dataset`): The dataset to be loaded.
             shuffle (bool, optional): Whether to shuffle the dataset. Defaults to False.
             seed (int, optional): Random worker seed for sampling, defaults to 1024.
             add_sampler: Whether to add ``DistributedDataParallelSampler`` to the dataset. Defaults to True.
             drop_last (bool, optional): Set to True to drop the last incomplete batch, if the dataset size
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/booster/plugin/gemini_plugin.py` & `colossalai-nightly-2023.5.6/colossalai/booster/plugin/gemini_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import os
 import warnings
 from pathlib import Path
-from typing import Callable, Iterator, List, Optional, Tuple, Union
+from typing import Callable, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 from torch import Tensor
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 from torch.utils.data import DataLoader
@@ -48,24 +48,16 @@
             save_state_dict(state_dict, checkpoint, use_safetensors)
 
     def save_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool):
         """
         Save optimizer to checkpoint but only on master process.
         """
         # TODO(ver217): optimizer state dict is sharded
-        warnings.warn('GeminiPlugin does not support save full optimizer checkpoint now. Save it on every process.')
-        checkpoint = f'{checkpoint}.rank{self.coordinator.rank}'
         super().save_unsharded_optimizer(optimizer, checkpoint, gather_dtensor)
 
-    def load_optimizer(self, optimizer: Optimizer, checkpoint: str):
-        warnings.warn(
-            'GeminiPlugin can only load optimizer checkpoint saved by itself with the same number of processes.')
-        checkpoint = f'{checkpoint}.rank{self.coordinator.rank}'
-        super().load_optimizer(optimizer, checkpoint)
-
     def save_lr_scheduler(self, lr_scheduler: LRScheduler, checkpoint: str):
         """
         Save model to checkpoint but only on master process.
         """
         if self.coordinator.is_master():
             super().save_lr_scheduler(lr_scheduler, checkpoint)
 
@@ -160,30 +152,30 @@
     Example:
         >>> from colossalai.booster import Booster
         >>> from colossalai.booster.plugin import GeminiPlugin
         >>>
         >>> model, train_dataset, optimizer, criterion = ...
         >>> plugin = GeminiPlugin()
 
-        >>> train_dataloader = plugin.prepare_dataloader(train_dataset, batch_size=8)
+        >>> train_dataloader = plugin.prepare_train_dataloader(train_dataset, batch_size=8)
         >>> booster = Booster(plugin=plugin)
         >>> model, optimizer, train_dataloader, criterion = booster.boost(model, optimizer, train_dataloader, criterion)
 
     Args:
         device (torch.device): device to place the model.
         placement_policy (str, optional): "cpu", "cuda", "auto". Defaults to "cpu".
         pin_memory (bool, optional): use pin memory on CPU. Defaults to False.
         force_outputs_fp32 (bool, optional): force outputs are fp32. Defaults to False.
         strict_ddp_mode (bool, optional): use strict ddp mode (only use dp without other parallelism). Defaults to False.
         search_range_mb (int, optional): chunk size searching range in MegaByte. Defaults to 32.
         hidden_dim (int, optional): the hidden dimension of DNN.
             Users can provide this argument to speed up searching.
             If users do not know this argument before training, it is ok. We will use a default value 1024.
         min_chunk_size_mb (float, optional): the minimum chunk size in MegaByte.
-            If the aggregate size of parameters is still smaller than the minimum chunk size,
+            If the aggregate size of parameters is still samller than the minimum chunk size,
             all parameters will be compacted into one small chunk.
         memstats (MemStats, optional) the memory statistics collector by a runtime memory tracer.
         gpu_margin_mem_ratio (float, optional): The ratio of GPU remaining memory (after the first forward-backward)
             which will be used when using hybrid CPU optimizer.
             This argument is meaningless when `placement_policy` of `GeminiManager` is not "auto".
             Defaults to 0.0.
         initial_scale (float, optional): Initial scale used by DynamicGradScaler. Defaults to 2**32.
@@ -290,10 +282,7 @@
         return model, optimizer, criterion, dataloader, lr_scheduler
 
     def control_checkpoint_io(self) -> bool:
         return True
 
     def get_checkpoint_io(self) -> CheckpointIO:
         return GeminiCheckpointIO()
-
-    def no_sync(self, model: nn.Module) -> Iterator[None]:
-        raise NotImplementedError
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/booster/plugin/low_level_zero_plugin.py` & `colossalai-nightly-2023.5.6/colossalai/booster/plugin/low_level_zero_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import warnings
-from typing import Callable, Iterator, List, Optional, Tuple, Union
+from typing import Callable, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 from torch import Tensor
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 from torch.utils._pytree import tree_map
 from torch.utils.data import DataLoader
 
-from colossalai.checkpoint_io import CheckpointIO, GeneralCheckpointIO
+from colossalai.checkpoint_io import CheckpointIO
 from colossalai.interface import ModelWrapper, OptimizerWrapper
 from colossalai.utils import get_current_device
 from colossalai.zero import zero_model_wrapper, zero_optim_wrapper
 
 from .dp_plugin_base import DPPluginBase
 from .torch_ddp_plugin import TorchDDPCheckpointIO
 
@@ -28,25 +28,16 @@
 
 class LowLevelZeroCheckpointIO(TorchDDPCheckpointIO):
 
     def save_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool):
         """
         Save optimizer to checkpoint but only on master process.
         """
-        # TODO(ver217): optimizer state dict is sharded, and cannot get full state dict now
-        warnings.warn(
-            'LowLevelZeroPlugin does not support save full optimizer checkpoint now. Save it on every process.')
-        checkpoint = f'{checkpoint}.rank{self.coordinator.rank}'
-        GeneralCheckpointIO.save_unsharded_optimizer(self, optimizer, checkpoint, gather_dtensor)
-
-    def load_optimizer(self, optimizer: Optimizer, checkpoint: str):
-        warnings.warn(
-            'LowLevelZeroPlugin can only load optimizer checkpoint saved by itself with the same number of processes.')
-        checkpoint = f'{checkpoint}.rank{self.coordinator.rank}'
-        super().load_optimizer(optimizer, checkpoint)
+        # TODO(ver217): optimizer state dict is sharded
+        super().save_unsharded_optimizer(optimizer, checkpoint, gather_dtensor)
 
 
 class LowLevelZeroModel(ModelWrapper):
 
     def __init__(self, module: nn.Module, stage: int, precision: str) -> None:
         super().__init__(module)
         self.convert_inputs = (precision == 'fp16')
@@ -100,15 +91,15 @@
     Example:
         >>> from colossalai.booster import Booster
         >>> from colossalai.booster.plugin import LowLevelZeroPlugin
         >>>
         >>> model, train_dataset, optimizer, criterion = ...
         >>> plugin = LowLevelZeroPlugin()
 
-        >>> train_dataloader = plugin.prepare_dataloader(train_dataset, batch_size=8)
+        >>> train_dataloader = plugin.prepare_train_dataloader(train_dataset, batch_size=8)
         >>> booster = Booster(plugin=plugin)
         >>> model, optimizer, train_dataloader, criterion = booster.boost(model, optimizer, train_dataloader, criterion)
 
     Args:
         strage (int, optional): ZeRO stage. Defaults to 1.
         precision (str, optional): precision. Support 'fp16' and 'fp32'. Defaults to 'fp16'.
         initial_scale (float, optional): Initial scale used by DynamicGradScaler. Defaults to 2**32.
@@ -202,10 +193,7 @@
         return model, optimizer, criterion, dataloader, lr_scheduler
 
     def control_checkpoint_io(self) -> bool:
         return True
 
     def get_checkpoint_io(self) -> CheckpointIO:
         return LowLevelZeroCheckpointIO()
-
-    def no_sync(self, model: nn.Module) -> Iterator[None]:
-        raise NotImplementedError
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/booster/plugin/plugin_base.py` & `colossalai-nightly-2023.5.6/colossalai/booster/plugin/plugin_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
-from typing import Callable, Iterator, List, Tuple, Union
+from typing import Callable, List, Tuple, Union
 
 import torch.nn as nn
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
-from torch.utils.data import DataLoader, Dataset
+from torch.utils.data import DataLoader
 
 from colossalai.checkpoint_io import CheckpointIO
 from colossalai.interface import OptimizerWrapper
 
 __all__ = ['Plugin']
 
 
@@ -55,29 +55,7 @@
 
     @abstractmethod
     def get_checkpoint_io(self) -> CheckpointIO:
         """
         Get checkpoint io object for this plugin, only invoked when control_checkpoint_io is True.
         """
         pass
-
-    @abstractmethod
-    def no_sync(self, model: nn.Module) -> Iterator[None]:
-        """
-        Context manager to disable gradient synchronization.
-        """
-        pass
-
-    @abstractmethod
-    def prepare_dataloader(self,
-                           dataset: Dataset,
-                           batch_size: int,
-                           shuffle: bool = False,
-                           seed: int = 1024,
-                           drop_last: bool = False,
-                           pin_memory: bool = False,
-                           num_workers: int = 0,
-                           **kwargs):
-        """Prepare a dataloader for distributed training. The dataloader will be wrapped by
-        `torch.utils.data.DataLoader`
-        """
-        pass
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/booster/plugin/torch_ddp_plugin.py` & `colossalai-nightly-2023.5.6/colossalai/booster/plugin/torch_ddp_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, Iterator, List, Optional, Tuple, Union
+from typing import Callable, List, Tuple, Union
 
 import torch.nn as nn
 from torch.nn.parallel import DistributedDataParallel as DDP
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 from torch.utils.data import DataLoader
 
@@ -46,24 +46,14 @@
     def save_lr_scheduler(self, lr_scheduler: LRScheduler, checkpoint: str):
         """
         Save model to checkpoint but only on master process.
         """
         if self.coordinator.is_master():
             super().save_lr_scheduler(lr_scheduler, checkpoint)
 
-    def save_sharded_model(self,
-                           model: nn.Module,
-                           checkpoint_path: str,
-                           gather_dtensor: bool = False,
-                           variant: Optional[str] = None,
-                           max_shard_size: int = 1024,
-                           use_safetensors: bool = False):
-        if self.coordinator.is_master():
-            super().save_sharded_model(model, checkpoint_path, gather_dtensor, variant, max_shard_size, use_safetensors)
-
 
 class TorchDDPModel(ModelWrapper):
 
     def __init__(self, module: nn.Module, *args, **kwargs) -> None:
         super().__init__(module)
         self.module = DDP(module, *args, **kwargs)
 
@@ -78,15 +68,15 @@
     Example:
         >>> from colossalai.booster import Booster
         >>> from colossalai.booster.plugin import TorchDDPPlugin
         >>>
         >>> model, train_dataset, optimizer, criterion = ...
         >>> plugin = TorchDDPPlugin()
 
-        >>> train_dataloader = plugin.prepare_dataloader(train_dataset, batch_size=8)
+        >>> train_dataloader = plugin.prepare_train_dataloader(train_dataset, batch_size=8)
         >>> booster = Booster(plugin=plugin)
         >>> model, optimizer, train_dataloader, criterion = booster.boost(model, optimizer, train_dataloader, criterion)
 
     Args:
         broadcast_buffers (bool, optional): Whether to broadcast buffers in the beginning of training. Defaults to True.
         bucket_cap_mb (int, optional): The bucket size in MB. Defaults to 25.
         find_unused_parameters (bool, optional): Whether to find unused parameters. Defaults to False.
@@ -148,11 +138,7 @@
         return model, optimizer, criterion, dataloader, lr_scheduler
 
     def control_checkpoint_io(self) -> bool:
         return True
 
     def get_checkpoint_io(self) -> CheckpointIO:
         return TorchDDPCheckpointIO()
-
-    def no_sync(self, model: nn.Module) -> Iterator[None]:
-        assert isinstance(model, TorchDDPModel), 'Model is not boosted by TorchDDPPlugin.'
-        return model.module.no_sync()
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/booster/plugin/torch_fsdp_plugin.py` & `colossalai-nightly-2023.5.6/colossalai/booster/booster.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,221 +1,174 @@
-from pathlib import Path
-from typing import Callable, Iterable, Iterator, List, Optional, Tuple, Union
+import warnings
+from contextlib import contextmanager
+from typing import Callable, Iterator, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
-import warnings
-from packaging import version
-from torch.distributed import ProcessGroup
-
-if version.parse(torch.__version__) >= version.parse('1.12.0'):
-    from torch.distributed.fsdp import FullStateDictConfig
-    from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
-    from torch.distributed.fsdp import StateDictType
-    from torch.distributed.fsdp.fully_sharded_data_parallel import (
-        BackwardPrefetch,
-        CPUOffload,
-        FullStateDictConfig,
-        MixedPrecision,
-        ShardingStrategy,
-    )
-else:
-    raise RuntimeError("FSDP is not supported while torch version under 1.12.0.")
-
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 from torch.utils.data import DataLoader
 
-from colossalai.checkpoint_io import CheckpointIO, GeneralCheckpointIO, utils
-from colossalai.cluster import DistCoordinator
-from colossalai.interface import ModelWrapper, OptimizerWrapper
-
-from .dp_plugin_base import DPPluginBase
-
-__all__ = ['TorchFSDPPlugin']
-
-
-class TorchFSDPCheckpointIO(GeneralCheckpointIO):
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.coordinator = DistCoordinator()
-
-    def load_unsharded_model(self, model: nn.Module, checkpoint: str, strict: bool):
-        checkpoint = utils.load_state_dict(checkpoint)
-        model.load_state_dict(checkpoint)
-
-    def load_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: Path):
-        checkpoint = utils.load_state_dict(checkpoint)
-        fsdp_model = optimizer.unwrap_model()
-        sharded_osd = FSDP.scatter_full_optim_state_dict(checkpoint, fsdp_model)
-        optimizer.load_state_dict(sharded_osd)
-
-    def save_unsharded_model(self, model: nn.Module, checkpoint: str, gather_dtensor: bool, use_safetensors: bool):
-        """
-        Save model to checkpoint but only on master process.
-        """
-        # the model should be unwrapped in self.load_model via ModelWrapper.unwrap
-        cfg = FullStateDictConfig(offload_to_cpu=True, rank0_only=True)
-        with FSDP.state_dict_type(model, StateDictType.FULL_STATE_DICT, cfg):
-            full_model_state = model.state_dict()
-        utils.save_state_dict(full_model_state, checkpoint_file_path=checkpoint, use_safetensors=use_safetensors)
-
-    def save_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool):
-        """
-        Save optimizer to checkpoint but only on master process.
-        """
-        assert isinstance(optimizer, FSDPOptimizerWrapper)
-        fsdp_model = optimizer.unwrap_model()
-        full_optimizer_state = FSDP.full_optim_state_dict(fsdp_model, optim=optimizer, rank0_only=True)
-        utils.save_state_dict(full_optimizer_state, checkpoint_file_path=checkpoint, use_safetensors=False)
+from colossalai.checkpoint_io import GeneralCheckpointIO
 
-    def save_sharded_model(self, model: nn.Module, checkpoint: str, gather_dtensor: bool, variant: Optional[str],
-                           size_per_shard: int, use_safetensors: bool):
-        """
-        Save model to checkpoint but only on master process.
-        """
-        raise NotImplementedError("Sharded model checkpoint is not supported yet.")
+from .accelerator import Accelerator
+from .mixed_precision import MixedPrecision, mixed_precision_factory
+from .plugin import Plugin
 
-    def load_sharded_model(self,
-                           model: nn.Module,
-                           checkpoint_index_file: Path,
-                           strict: bool = False,
-                           use_safetensors: bool = False,
-                           load_sub_module: bool = True):
-        """
-        Load model to checkpoint but only on master process.
-        """
-        raise NotImplementedError("Sharded model checkpoint is not supported yet.")
+__all__ = ['Booster']
 
-    def save_sharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool):
-        """
-        Save optimizer to checkpoint but only on master process.
-        """
-        raise NotImplementedError("Sharded optimizer checkpoint is not supported yet.")
 
-    def load_sharded_optimizer(self, optimizer: Optimizer, index_file_path: str, prefix: str, size_per_shard: int):
-        """
-        Load optimizer to checkpoint but only on master process.
-        """
-        raise NotImplementedError("Sharded optimizer checkpoint is not supported yet.")
-
-    def save_lr_scheduler(self, lr_scheduler: LRScheduler, checkpoint: str):
-        """
-        Save model to checkpoint but only on master process.
-        """
-        if self.coordinator.is_master():
-            super().save_lr_scheduler(lr_scheduler, checkpoint)
-
-
-class TorchFSDPModel(ModelWrapper):
-
-    def __init__(self, module: nn.Module, *args, **kwargs) -> None:
-        super().__init__(module)
-        self.module = FSDP(module, *args, **kwargs)
-
-    def unwrap(self):
-        return self.module
-
-
-class FSDPOptimizerWrapper(OptimizerWrapper):
-
-    def __init__(self, optimizer: Optimizer, model: nn.Module):
-        self.model = model
-        super().__init__(optimizer)
-
-    def unwrap_model(self) -> nn.Module:
-        return self.model
-
-
-class TorchFSDPPlugin(DPPluginBase):
+class Booster:
     """
-    Plugin for PyTorch FSDP.
+    Booster is a high-level API for training neural networks. It provides a unified interface for
+    training with different precision, accelerator, and plugin.
 
-    Example:
-        >>> from colossalai.booster import Booster
-        >>> from colossalai.booster.plugin import TorchFSDPPlugin
+    Examples:
+        >>> colossalai.launch(...)
+        >>> plugin = GeminiPlugin(stage=3, ...)
+        >>> booster = Booster(precision='fp16', plugin=plugin)
         >>>
-        >>> model, train_dataset, optimizer, criterion = ...
-        >>> plugin = TorchFSDPPlugin()
+        >>> model = GPT2()
+        >>> optimizer = Adam(model.parameters())
+        >>> dataloader = Dataloader(Dataset)
+        >>> lr_scheduler = LinearWarmupScheduler()
+        >>> criterion = GPTLMLoss()
+        >>>
+        >>> model, optimizer, lr_scheduler, dataloader = booster.boost(model, optimizer, lr_scheduler, dataloader)
+        >>>
+        >>> for epoch in range(max_epochs):
+        >>>     for input_ids, attention_mask in dataloader:
+        >>>         outputs = model(input_ids, attention_mask)
+        >>>         loss = criterion(outputs.logits, input_ids)
+        >>>         booster.backward(loss, optimizer)
+        >>>         optimizer.step()
+        >>>         lr_scheduler.step()
+        >>>         optimizer.zero_grad()
 
-        >>> train_dataloader = plugin.prepare_train_dataloader(train_dataset, batch_size=8)
-        >>> booster = Booster(plugin=plugin)
-        >>> model, optimizer, train_dataloader, criterion = booster.boost(model, optimizer, train_dataloader, criterion)
 
     Args:
-        See https://pytorch.org/docs/stable/fsdp.html for details.
+        device (str or torch.device): The device to run the training. Default: 'cuda'.
+        mixed_precision (str or MixedPrecision): The mixed precision to run the training. Default: None.
+                                If the argument is a string, it can be 'fp16', 'fp16_apex', 'bf16', or 'fp8'.
+                                'fp16' would use PyTorch AMP while `fp16_apex` would use Nvidia Apex.
+        plugin (Plugin): The plugin to run the training. Default: None.
     """
 
-    if version.parse(torch.__version__) >= version.parse('1.12.0'):
-
-        def __init__(
-            self,
-            process_group: Optional[ProcessGroup] = None,
-            sharding_strategy: Optional[ShardingStrategy] = None,
-            cpu_offload: Optional[CPUOffload] = None,
-            auto_wrap_policy: Optional[Callable] = None,
-            backward_prefetch: Optional[BackwardPrefetch] = None,
-            mixed_precision: Optional[MixedPrecision] = None,
-            ignored_modules: Optional[Iterable[torch.nn.Module]] = None,
-            param_init_fn: Optional[Callable[[nn.Module], None]] = None,
-            sync_module_states: bool = False,
-        ):
-            super().__init__()
-            self.fsdp_kwargs = dict(process_group=process_group,
-                                    sharding_strategy=sharding_strategy,
-                                    cpu_offload=cpu_offload,
-                                    auto_wrap_policy=auto_wrap_policy,
-                                    backward_prefetch=backward_prefetch,
-                                    mixed_precision=mixed_precision,
-                                    ignored_modules=ignored_modules,
-                                    param_init_fn=param_init_fn,
-                                    sync_module_states=sync_module_states)
-    else:
-        raise RuntimeError("FSDP is not supported while torch version under 1.12.0.")
-
-    def support_no_sync(self) -> bool:
-        False
-
-    def no_sync(self, model: nn.Module) -> Iterator[None]:
-        raise NotImplementedError("Torch fsdp no_sync func not supported yet.")
-
-    def control_precision(self) -> bool:
-        return True
-
-    def supported_precisions(self) -> List[str]:
-        return ['fp16', 'bf16']
+    def __init__(self,
+                 device: str = 'cuda',
+                 mixed_precision: Union[MixedPrecision, str] = None,
+                 plugin: Optional[Plugin] = None) -> None:
+        if plugin is not None:
+            assert isinstance(
+                plugin, Plugin), f'Expected the argument plugin to be an instance of Plugin, but got {type(plugin)}.'
+        self.plugin = plugin
+
+        # set accelerator
+        if self.plugin and self.plugin.control_device():
+            self.accelerator = None
+            warnings.warn('The plugin will control the accelerator, so the device argument will be ignored.')
+        else:
+            self.accelerator = Accelerator(device)
+
+        # set precision
+        if self.plugin and self.plugin.control_precision():
+            warnings.warn('The plugin will control the precision, so the mixed_precision argument will be ignored.')
+            self.mixed_precision = None
+        elif mixed_precision is None:
+            self.mixed_precision = None
+        else:
+            # validate and set precision
+            if isinstance(mixed_precision, str):
+                # the user will take the default arguments for amp training
+                self.mixed_precision = mixed_precision_factory(mixed_precision)
+            elif isinstance(mixed_precision, MixedPrecision):
+                # the user can customize the arguments by passing the precision object
+                self.mixed_precision = mixed_precision
+            else:
+                raise ValueError(
+                    f'Expected the argument mixed_precision to be a string or an instance of Precision, but got {type(mixed_precision)}.'
+                )
+
+        if self.plugin is not None and self.plugin.control_checkpoint_io():
+            self.checkpoint_io = self.plugin.get_checkpoint_io()
+        else:
+            self.checkpoint_io = GeneralCheckpointIO()
 
-    def control_device(self) -> bool:
-        return True
-
-    def supported_devices(self) -> List[str]:
-        return ['cuda']
-
-    def configure(
+    def boost(
         self,
         model: nn.Module,
         optimizer: Optimizer,
         criterion: Callable = None,
         dataloader: DataLoader = None,
         lr_scheduler: LRScheduler = None,
-    ) -> Tuple[Union[nn.Module, OptimizerWrapper, LRScheduler, DataLoader]]:
-
-        # wrap the model with PyTorch FSDP
-        fsdp_model = TorchFSDPModel(model, device_id=torch.cuda.current_device(), **self.fsdp_kwargs)
+    ) -> List[Union[nn.Module, Optimizer, LRScheduler, DataLoader]]:
+        """
+        Boost the model, optimizer, criterion, lr_scheduler, and dataloader.
 
-        if len(optimizer.param_groups) > 1:
-            warnings.warn(
-                'TorchFSDPPlugin does not support optimizer that use multi param groups. The results may not be as expected if used.'
-            )
-        optimizer.__init__(fsdp_model.parameters(), **optimizer.defaults)
+        Args:
+            model (nn.Module): The model to be boosted.
+            optimizer (Optimizer): The optimizer to be boosted.
+            criterion (Callable): The criterion to be boosted.
+            dataloader (DataLoader): The dataloader to be boosted.
+            lr_scheduler (LRScheduler): The lr_scheduler to be boosted.
+        """
+        # TODO(FrankLeeeee): consider multi-model and multi-optimizer case
+        # TODO(FrankLeeeee): consider multi-dataloader case
+        # transform model for mixed precision
+        if self.plugin:
+            model, optimizer, criterion, dataloader, lr_scheduler = self.plugin.configure(
+                model, optimizer, criterion, dataloader, lr_scheduler)
+
+        if self.plugin and not self.plugin.control_device():
+            # transform model for accelerator
+            model = self.accelerator.configure(model)
+
+        if self.mixed_precision and (self.plugin is None or self.plugin and not self.plugin.control_precision()):
+            # transform model for mixed precision
+            # when mixed_precision is specified and the plugin is not given or does not control the precision
+            model, optimizer, criterion = self.mixed_precision.configure(model, optimizer, criterion)
+
+        return model, optimizer, criterion, dataloader, lr_scheduler
+
+    def backward(self, loss: torch.Tensor, optimizer: Optimizer) -> None:
+        # TODO: implement this method with plugin
+        optimizer.backward(loss)
+
+    def execute_pipeline(self,
+                         data_iter: Iterator,
+                         model: nn.Module,
+                         criterion: Callable[[torch.Tensor], torch.Tensor],
+                         optimizer: Optimizer,
+                         return_loss: bool = True,
+                         return_outputs: bool = False) -> Tuple[Optional[torch.Tensor], ...]:
+        # TODO: implement this method
+        # run pipeline forward backward pass
+        # return loss or outputs if needed
+        pass
+
+    def no_sync(self, model: nn.Module) -> contextmanager:
+        assert self.plugin is not None, f'no_sync is only enabled when a plugin is provided and the plugin supports no_sync.'
+        assert self.plugin.support_no_sync, f'The plugin {self.plugin.__class__.__name__} does not support no_sync.'
+        return self.plugin.no_sync(model)
+
+    def load_model(self, model: nn.Module, checkpoint: str, strict: bool = True):
+        self.checkpoint_io.load_model(model, checkpoint, strict)
+
+    def save_model(self,
+                   model: nn.Module,
+                   checkpoint: str,
+                   prefix: str = None,
+                   shard: bool = False,
+                   size_per_shard: int = 1024):
+        self.checkpoint_io.save_model(model, checkpoint, prefix, shard, size_per_shard)
 
-        if not isinstance(optimizer, FSDPOptimizerWrapper):
-            optimizer = FSDPOptimizerWrapper(optimizer, fsdp_model)
+    def load_optimizer(self, optimizer: Optimizer, checkpoint: str):
+        self.checkpoint_io.load_optimizer(optimizer, checkpoint)
 
-        return fsdp_model, optimizer, criterion, dataloader, lr_scheduler
+    def save_optimizer(self, optimizer: Optimizer, checkpoint: str, shard: bool = False, size_per_shard: int = 1024):
+        self.checkpoint_io.save_optimizer(optimizer, checkpoint, shard, size_per_shard)
 
-    def control_checkpoint_io(self) -> bool:
-        return True
+    def save_lr_scheduler(self, lr_scheduler: LRScheduler, checkpoint: str):
+        self.checkpoint_io.save_lr_scheduler(lr_scheduler, checkpoint)
 
-    def get_checkpoint_io(self) -> CheckpointIO:
-        return TorchFSDPCheckpointIO()
+    def load_lr_scheduler(self, lr_scheduler: LRScheduler, checkpoint: str):
+        self.checkpoint_io.load_lr_scheduler(lr_scheduler, checkpoint)
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/builder/builder.py` & `colossalai-nightly-2023.5.6/colossalai/builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/checkpoint_io/checkpoint_io_base.py` & `colossalai-nightly-2023.5.6/colossalai/checkpoint_io/checkpoint_io_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Optional, Union
+from typing import Union
+from typing import Optional
 
 import torch
 import torch.nn as nn
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 
 from colossalai.interface import ModelWrapper
@@ -79,16 +80,17 @@
             strict (bool): whether to strictly enforce that the param name in
                 the checkpoint match the keys returned by this module's.
         """
         # since we only support loaded sharded and unsharded weight format
         # containing no distributed tensors, dtensor -> full tensor conversion
         # should be done offline via our CLI
         # the existence of index file means it is a sharded checkpoint
+        ckpt_path = Path(checkpoint)
         index_file_exists, index_file_path = has_index_file(checkpoint)
-
+        
         # return the origin model instead of the unwrapped model
         origin_model = model
 
         if isinstance(model, ModelWrapper):
             model = model.unwrap()
 
         if index_file_exists:
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/checkpoint_io/general_checkpoint_io.py` & `colossalai-nightly-2023.5.6/colossalai/checkpoint_io/general_checkpoint_io.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-import gc
-import logging
-import os
-from functools import reduce
 from pathlib import Path
-from typing import Iterator, Optional, OrderedDict, Tuple
+from functools import reduce
 
 import torch.nn as nn
 from torch.optim import Optimizer
+import logging
+import os
+import gc
+from typing import Optional, Iterator, OrderedDict, Tuple
 
 from .checkpoint_io_base import CheckpointIO
 from .index_file import CheckpointIndexFile
 from .utils import (
-    get_base_filenames,
-    get_shard_filename,
-    has_index_file,
+    has_index_file, 
+    load_state_dict, 
+    save_state_dict, 
     is_safetensors_available,
+    shard_checkpoint,
     load_shard_state_dict,
-    load_state_dict,
     load_state_dict_into_model,
-    save_state_dict,
-    shard_checkpoint,
-)
+    get_shard_filename,
+    get_base_filenames
+    )
 
 __all__ = ['GeneralCheckpointIO']
 
 
 class GeneralCheckpointIO(CheckpointIO):
     """
     Checkpoint IO
     """
-
     def load_unsharded_model(self, model: nn.Module, checkpoint: str, strict: bool):
         checkpoint = load_state_dict(checkpoint)
         model.load_state_dict(checkpoint, strict=strict)
 
     def save_unsharded_model(self, model: nn.Module, checkpoint: str, gather_dtensor: bool, use_safetensors: bool):
         state_dict = model.state_dict()
 
@@ -66,81 +65,79 @@
         optimizer: Optimizer,
         checkpoint: Path,
         gather_dtensor: bool,
     ):
         # TODO(FrankLeeeee): handle distributed tensors
         save_state_dict(optimizer.state_dict(), checkpoint, use_safetensors=False)
 
-    def save_sharded_model(self,
-                           model: nn.Module,
-                           checkpoint_path: str,
-                           gather_dtensor: bool = False,
-                           variant: Optional[str] = None,
-                           max_shard_size: int = 1024,
-                           use_safetensors: bool = False):
-        """
+
+    def save_sharded_model(self, model: nn.Module, checkpoint_path: str, gather_dtensor:bool = False, 
+                           variant: Optional[str] = None, max_shard_size: int = 1024, use_safetensors: bool = False):
+        """ 
         implement this method as it can be supported by Huggingface model,
         save shard model, save model to multiple files
         """
         if os.path.isfile(checkpoint_path):
             logging.error(f"Provided path ({checkpoint_path}) should be a directory, not a file")
             return
-
+        
         Path(checkpoint_path).mkdir(parents=True, exist_ok=True)
-
+        
         # shard checkpoint
         state_dict = model.state_dict()
         state_dict_shard = shard_checkpoint(state_dict, max_shard_size=max_shard_size)
 
         weights_name, save_index_file = get_base_filenames(variant, use_safetensors)
         total_size = 0
         index_file = CheckpointIndexFile(checkpoint_path)
         for idx, shard_pair in enumerate(state_dict_shard):
             shard = shard_pair[0]
             shard_file = get_shard_filename(weights_name, idx)
             total_size = total_size + shard_pair[1]
             for key in shard.keys():
                 index_file.append_weight_map(key, shard_file)
-
+            
             checkpoint_file_path = os.path.join(checkpoint_path, shard_file)
             save_state_dict(shard, checkpoint_file_path, use_safetensors)
-
+        
         index_file.append_meta_data("total_size", total_size)
         index_file.write_index_file(save_index_file)
-        logging.info(f"The model is going to be split to checkpoint shards. "
-                     f"You can find where each parameters has been saved in the "
-                     f"index located at {save_index_file}.")
-
-    def load_sharded_model(self,
-                           model: nn.Module,
-                           checkpoint_index_file: Path,
-                           strict: bool = False,
-                           use_safetensors: bool = False,
-                           load_sub_module: bool = True):
+        logging.info(
+            f"The model is going to be split to checkpoint shards. "
+            f"You can find where each parameters has been saved in the "
+            f"index located at {save_index_file}."
+        )
+
+
+    def load_sharded_model(self, model: nn.Module, checkpoint_index_file: Path, strict: bool = False, 
+                           use_safetensors: bool = False, load_sub_module: bool = True):
         """
         load shard model, load model from multiple files
         """
         use_safetensors = False
         if "safetensors" in checkpoint_index_file.name:
             use_safetensors = True
 
         if use_safetensors and not is_safetensors_available():
             raise ImportError("`safe_serialization` requires the `safetensors` library: `pip install safetensors`.")
-
+        
         # read checkpoint index file
         ckpt_index_file = CheckpointIndexFile.from_file(checkpoint_index_file)
         checkpoint_files, _ = ckpt_index_file.get_checkpoint_fileanames()
         missing_keys = []
 
         for shard_file in checkpoint_files:
             state_dict = load_shard_state_dict(Path(shard_file), use_safetensors)
             load_state_dict_into_model(model, state_dict, missing_keys, strict, load_sub_module)
             del state_dict
             gc.collect()
 
         if strict:
             remain_keys = reduce(lambda a, b: a & b, map(set, missing_keys))
             if len(remain_keys) > 0:
-                error_msgs = 'Missing key(s) in state_dict: {}. '.format(', '.join(
-                    '"{}"'.format(k) for k in missing_keys))
+                error_msgs = 'Missing key(s) in state_dict: {}. '.format(
+                            ', '.join('"{}"'.format(k) for k in missing_keys))
                 raise RuntimeError('Error(s) in loading state_dict for {}:\n\t{}'.format(
-                    self.__class__.__name__, "\n\t".join(error_msgs)))
+                                self.__class__.__name__, "\n\t".join(error_msgs)))
+
+
+
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/checkpoint_io/index_file.py` & `colossalai-nightly-2023.5.6/colossalai/checkpoint_io/index_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,14 @@
         """
         Get all the weight keys.
         """
         return list(self.weight_map.keys())
     
     def write_index_file(self, save_index_file):
         """
-        Write index file.
+        Wriete index file.
         """
         save_index_file = os.path.join(self.root_path, save_index_file)
         index = {"metadata": self.metadata, "weight_map": self.weight_map}
         with open(save_index_file, "w", encoding="utf-8") as f:
             content = json.dumps(index, indent=2, sort_keys=True) + "\n"
             f.write(content)
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/checkpoint_io/utils.py` & `colossalai-nightly-2023.5.6/colossalai/checkpoint_io/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 # coding=utf-8
-import re
 from pathlib import Path
-from typing import Iterator, List, Mapping, Optional, OrderedDict, Tuple
-
 import torch
 import torch.nn as nn
-
+from typing import List, Mapping, OrderedDict, Optional, Tuple, Iterator
 from colossalai.tensor.d_tensor.d_tensor import DTensor
+import re
 
 SAFE_WEIGHTS_NAME = "model.safetensors"
 WEIGHTS_NAME = "pytorch_model.bin"
 SAFE_WEIGHTS_INDEX_NAME = "model.safetensors.index.json"
 WEIGHTS_INDEX_NAME = "pytorch_model.bin.index.json"
 
 # ======================================
 # General helper functions
 # ======================================
 
-
 def calculate_tensor_size(tensor: torch.Tensor) -> float:
     """
     Calculate the size of a parameter in MB. Used to compute whether a group of params exceed the shard size.
     If so, a new shard should be created.
 
     Args:
-        tensor (torch.Tensor): the tensor to calculate size for.
+        tenosr (torch.Tensor): the tensor to calculate size for.
 
     Returns:
         float: size of the tensor in MB.
     """
     return tensor.numel() * tensor.element_size() / 1024 / 1024
 
-
 def is_safetensors_available() -> bool:
     """
     Check whether safetensors is available.
 
     Returns:
         bool: whether safetensors is available.
     """
@@ -78,14 +74,15 @@
         return False
 
 
 # ======================================
 # Helper functions for saving shard file
 # ======================================
 def shard_checkpoint(state_dict: torch.Tensor, max_shard_size: int = 1024) -> Iterator[Tuple[OrderedDict, int]]:
+ 
     """
     Splits a model state dictionary in sub-checkpoints so that the final size of each sub-checkpoint does not exceed a
     given size.
     """
     current_block = {}
     current_block_size = 0
 
@@ -99,47 +96,43 @@
             if current_block_size + weight_size > max_shard_size:
                 ret_block = current_block
                 ret_block_size = current_block_size
                 current_block = {}
                 current_block_size = 0
             current_block[key] = weight
             current_block_size += weight_size
-
+            
         if ret_block != None:
             yield ret_block, ret_block_size
 
     yield current_block, current_block_size
 
 
-def load_shard_state_dict(checkpoint_file: Path, use_safetensors: bool = False):
+def load_shard_state_dict(checkpoint_file: Path, use_safetensors: bool =False):
     """
     load shard state dict into model
     """
     if use_safetensors and not checkpoint_file.suffix == ".safetensors":
         raise Exception("load the model using `safetensors`, but no file endwith .safetensors")
     if use_safetensors:
-        from safetensors.torch import load_file as safe_load_file
         from safetensors.torch import safe_open
+        from safetensors.torch import load_file as safe_load_file
         with safe_open(checkpoint_file, framework="pt") as f:
             metadata = f.metadata()
         if metadata["format"] != "pt":
             raise NotImplementedError(
-                f"Conversion from a {metadata['format']} safetensors archive to PyTorch is not implemented yet.")
+                f"Conversion from a {metadata['format']} safetensors archive to PyTorch is not implemented yet."
+            )
         return safe_load_file(checkpoint_file)
     else:
         return torch.load(checkpoint_file)
-
-
-def load_state_dict_into_model(model: nn.Module,
-                               state_dict: torch.Tensor,
-                               missing_keys: List,
-                               strict: bool = False,
-                               load_sub_module: bool = True):
+    
+def load_state_dict_into_model(model: nn.Module, state_dict: torch.Tensor, missing_keys: List, strict: bool = False, load_sub_module: bool = True):
     r"""Copies parameters and buffers from :attr:`state_dict` into
-    this module and its descendants.
+    this module and its descendants. 
 
     Args:
         state_dict (dict): a dict containing parameters and
             persistent buffers.
     """
     if not isinstance(state_dict, Mapping):
         raise TypeError("Expected state_dict to be dict-like, got {}.".format(type(state_dict)))
@@ -169,20 +162,19 @@
     load(model, state_dict, "", load_sub_module)
     del load
 
     missing_keys = missing_keys.append(sub_missing_keys)
 
     if strict:
         if len(unexpected_keys) > 0:
-            error_msgs = 'Unexpected key(s) in state_dict: {}. '.format(', '.join(
-                '"{}"'.format(k) for k in unexpected_keys))
+            error_msgs = 'Unexpected key(s) in state_dict: {}. '.format(
+                        ', '.join('"{}"'.format(k) for k in unexpected_keys))
             raise RuntimeError('Error(s) in loading state_dict for {}:\n\t{}'.format(
-                model.__class__.__name__, "\n\t".join(error_msgs)))
-
-
+                               model.__class__.__name__, "\n\t".join(error_msgs)))
+        
 # ======================================
 # Helper functions for saving state dict
 # ======================================
 
 
 def save_state_dict(state_dict: dict, checkpoint_file_path: str, use_safetensors: bool) -> None:
     """
@@ -354,16 +346,14 @@
                 index_files
             ) == 1, f'Expected to find one .index.json file in {checkpoint_path}, but found {len(index_files)}'
 
         if len(index_files) == 1:
             return True, index_files[0]
         else:
             return False, None
-    else:
-        raise RuntimeError(f'Invalid checkpoint path {checkpoint_path}. Expected a file or a directory.')
 
 
 def load_state_dict(checkpoint_file_path: Path):
     """
     Load state dict from checkpoint.
 
     Args:
@@ -386,38 +376,38 @@
             for k in f.keys():
                 state_dict[k] = f.get_tensor(k)
         return state_dict
 
     else:
         # load with torch
         return torch.load(checkpoint_file_path)
+    
 
 
 def add_variant(weights_name: str, variant: Optional[str] = None) -> str:
     if variant is not None and len(variant) > 0:
         splits = weights_name.split(".")
         splits = splits[:-1] + [variant] + splits[-1:]
         weights_name = ".".join(splits)
 
     return weights_name
 
 
-def get_base_filenames(variant: str = None, use_safetensors: bool = False):
-    """
-    generate base weight filenames
-    """
-    weights_name = SAFE_WEIGHTS_NAME if use_safetensors else WEIGHTS_NAME
-    weights_name = add_variant(weights_name, variant)
-
-    save_index_file = SAFE_WEIGHTS_INDEX_NAME if use_safetensors else WEIGHTS_INDEX_NAME
-    save_index_file = add_variant(save_index_file, variant)
+def get_base_filenames(variant: str=None, use_safetensors: bool=False):
+        """
+        generate base weight filenames
+        """
+        weights_name = SAFE_WEIGHTS_NAME if use_safetensors else WEIGHTS_NAME
+        weights_name = add_variant(weights_name, variant)
 
-    return weights_name, save_index_file
+        save_index_file = SAFE_WEIGHTS_INDEX_NAME if use_safetensors else WEIGHTS_INDEX_NAME
+        save_index_file = add_variant(save_index_file, variant)
 
+        return weights_name, save_index_file
 
 def get_shard_filename(weights_name: str, idx: int):
     """
     get shard file name
     """
     shard_file = weights_name.replace(".bin", f"-{idx+1:05d}.bin")
     shard_file = shard_file.replace(".safetensors", f"-{idx + 1:05d}.safetensors")
-    return shard_file
+    return shard_file
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/cli/benchmark/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/cli/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/cli/benchmark/benchmark.py` & `colossalai-nightly-2023.5.6/colossalai/cli/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/cli/benchmark/utils.py` & `colossalai-nightly-2023.5.6/colossalai/cli/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/cli/check/check_installation.py` & `colossalai-nightly-2023.5.6/colossalai/cli/check/check_installation.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ```
 
     Returns: A table of installation information.
     """
     found_aot_cuda_ext = _check_aot_built_cuda_extension_installed()
     cuda_version = _check_cuda_version()
     torch_version, torch_cuda_version = _check_torch_version()
-    colossalai_version, prebuilt_torch_version_required, prebuilt_cuda_version_required = _parse_colossalai_version()
+    colossalai_verison, prebuilt_torch_version_required, prebuilt_cuda_version_required = _parse_colossalai_version()
 
     # if cuda_version is None, that means either
     # CUDA_HOME is not found, thus cannot compare the version compatibility
     if not cuda_version:
         sys_torch_cuda_compatibility = None
     else:
         sys_torch_cuda_compatibility = _is_compatible([cuda_version, torch_cuda_version])
@@ -53,15 +53,15 @@
     if prebuilt_torch_version_required is None:
         torch_compatibility = None
     else:
         torch_compatibility = _is_compatible([torch_version, prebuilt_torch_version_required])
 
     click.echo(f'#### Installation Report ####')
     click.echo(f'\n------------ Environment ------------')
-    click.echo(f"Colossal-AI version: {to_click_output(colossalai_version)}")
+    click.echo(f"Colossal-AI version: {to_click_output(colossalai_verison)}")
     click.echo(f"PyTorch version: {to_click_output(torch_version)}")
     click.echo(f"System CUDA version: {to_click_output(cuda_version)}")
     click.echo(f"CUDA version required by PyTorch: {to_click_output(torch_cuda_version)}")
     click.echo("")
     click.echo(f"Note:")
     click.echo(f"1. The table above checks the versions of the libraries/tools in the current environment")
     click.echo(f"2. If the System CUDA version is N/A, you can set the CUDA_HOME environment variable to locate it")
@@ -133,23 +133,23 @@
         torch_version_for_aot_build: PyTorch version used for AOT compilation of CUDA kernels.
         cuda_version_for_aot_build: CUDA version used for AOT compilation of CUDA kernels.
     """
     # colossalai version can be in two formats
     # 1. X.X.X+torchX.XXcuXX.X (when colossalai is installed with CUDA extensions)
     # 2. X.X.X (when colossalai is not installed with CUDA extensions)
     # where X represents an integer.
-    colossalai_version = colossalai.__version__.split('+')[0]
+    colossalai_verison = colossalai.__version__.split('+')[0]
 
     try:
         torch_version_for_aot_build = colossalai.__version__.split('torch')[1].split('cu')[0]
         cuda_version_for_aot_build = colossalai.__version__.split('cu')[1]
     except:
         torch_version_for_aot_build = None
         cuda_version_for_aot_build = None
-    return colossalai_version, torch_version_for_aot_build, cuda_version_for_aot_build
+    return colossalai_verison, torch_version_for_aot_build, cuda_version_for_aot_build
 
 
 def _check_aot_built_cuda_extension_installed():
     """
     According to `op_builder/README.md`, the CUDA extension can be built with either
     AOT (ahead-of-time) or JIT (just-in-time) compilation.
     AOT compilation will build CUDA extensions to `colossalai._C` during installation.
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/cli/launcher/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/cli/launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/cli/launcher/hostinfo.py` & `colossalai-nightly-2023.5.6/colossalai/cli/launcher/hostinfo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/cli/launcher/multinode_runner.py` & `colossalai-nightly-2023.5.6/colossalai/cli/launcher/multinode_runner.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/cli/launcher/run.py` & `colossalai-nightly-2023.5.6/colossalai/cli/launcher/run.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/cluster/device_mesh_manager.py` & `colossalai-nightly-2023.5.6/colossalai/cluster/device_mesh_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/cluster/dist_coordinator.py` & `colossalai-nightly-2023.5.6/colossalai/cluster/dist_coordinator.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,15 @@
             >>>
             >>> @dist_coordinator.on_master_only()
             >>> def print_on_master(msg):
             >>>     print(msg)
         """
         is_master = self.is_master(process_group)
 
-        # define an inner function
+        # define an inner functiuon
         def decorator(func):
 
             @functools.wraps(func)
             def wrapper(*args, **kwargs):
                 if is_master:
                     return func(*args, **kwargs)
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/cluster/process_group_manager.py` & `colossalai-nightly-2023.5.6/colossalai/cluster/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/communication/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/communication/collective.py` & `colossalai-nightly-2023.5.6/colossalai/communication/collective.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/communication/p2p.py` & `colossalai-nightly-2023.5.6/colossalai/communication/p2p.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
     """Copy the gradient tensor from the next stage in pipeline as the input gradient of this stage.
 
     Args:
         output_grad_shape (Union[:class:`torch.Size`, List[:class:`torch.Size`]]): The shape of the tensor to be received.
         next_rank (int, optional): The rank of the source of the tensor.
 
     Returns:
-        Union[:class:`torch.Tensor`, List[:class:`torch.Tensor`]]: The input gradient tensor or gradient tensor list.
+        Union[:class:`torch.Tensor`, List[:class:`torch.Tensor`]]: The input gradient tensor or gradident tensor list.
     """
     if gpc.is_pipeline_last_stage():
         output_tensor_grad = None
     else:
         _, output_tensor_grad = _communicate(recv_next=True,
                                              recv_next_shape=output_grad_shape,
                                              next_rank=next_rank,
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/communication/p2p_v2.py` & `colossalai-nightly-2023.5.6/colossalai/communication/p2p_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 TensorShape = Union[torch.Size, List[int], Tuple[int]]
 _pg_manager = {}
 _unpickler = pickle.Unpickler
 
 
 def init_process_group():
-    """initialise process group by dist.new_group in the adjacent stages
+    """intialise process group by dist.new_group in the adjacent stages
 
     Args:
         None
 
     Returns:
         None
     """
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/communication/ring.py` & `colossalai-nightly-2023.5.6/colossalai/communication/ring.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/communication/utils.py` & `colossalai-nightly-2023.5.6/colossalai/communication/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/constants.py` & `colossalai-nightly-2023.5.6/colossalai/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/context/config.py` & `colossalai-nightly-2023.5.6/colossalai/context/config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/context/moe_context.py` & `colossalai-nightly-2023.5.6/colossalai/context/moe_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/context/parallel_context.py` & `colossalai-nightly-2023.5.6/colossalai/context/parallel_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/context/parallel_mode.py` & `colossalai-nightly-2023.5.6/colossalai/context/parallel_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/initializer_1d.py` & `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_1d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/initializer_2d.py` & `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/initializer_2p5d.py` & `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/initializer_3d.py` & `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/initializer_data.py` & `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_data.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/initializer_model.py` & `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/initializer_pipeline.py` & `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_pipeline.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/initializer_sequence.py` & `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         Returns:
             List[Tuple (local_rank, group_world_size, process_group, ranks_in_group, mode)]:
                 A Sequence parallelism's information in list of tuples.
         """
 
         parallel_setting = []
 
-        local_rank, group_world_size, process_group, cpu_group, ranks_in_group, mode = \
+        local_rank, group_world_size, process_group, cpu_grop, ranks_in_group, mode = \
             self._sequence_initializer.init_dist_group()
         # change mode to sequence
         mode = ParallelMode.SEQUENCE
 
-        parallel_setting.append((local_rank, group_world_size, process_group, cpu_group, ranks_in_group, mode))
+        parallel_setting.append((local_rank, group_world_size, process_group, cpu_grop, ranks_in_group, mode))
         parallel_setting.append(self._sequence_dp_initializer.init_dist_group())
         return parallel_setting
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/initializer_tensor.py` & `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/initializer_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/context/process_group_initializer/process_group_initializer.py` & `colossalai-nightly-2023.5.6/colossalai/context/process_group_initializer/process_group_initializer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/context/random/_helper.py` & `colossalai-nightly-2023.5.6/colossalai/context/random/_helper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/context/random/seed_manager.py` & `colossalai-nightly-2023.5.6/colossalai/context/random/seed_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/context/singleton_meta.py` & `colossalai-nightly-2023.5.6/colossalai/context/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/device/alpha_beta_profiler.py` & `colossalai-nightly-2023.5.6/colossalai/device/alpha_beta_profiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,12 +377,12 @@
             broadcast_object = [latency, bandwidth]
             dist.broadcast_object_list(broadcast_object, src=pg[0])
             return broadcast_object
 
         first_latency, first_bandwidth = _extract_alpha_beta(first_axis, first_axis_process_group)
         second_latency, second_bandwidth = _extract_alpha_beta(second_axis, second_axis_process_group)
         mesh_alpha = [first_latency, second_latency]
-        # The beta values have been enlarged by 1e10 times temporarily because the computation cost
+        # The beta values have been enlarged by 1e10 times temporarilly because the computation cost
         # is still estimated in the unit of TFLOPs instead of time. We will remove this factor in future.
         mesh_beta = [1e10 / first_bandwidth, 1e10 / second_bandwidth]
 
         return mesh_alpha, mesh_beta
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/device/calc_pipeline_strategy.py` & `colossalai-nightly-2023.5.6/colossalai/device/calc_pipeline_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/device/device_mesh.py` & `colossalai-nightly-2023.5.6/colossalai/device/device_mesh.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/engine/_base_engine.py` & `colossalai-nightly-2023.5.6/colossalai/engine/_base_engine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/engine/gradient_accumulation/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/engine/gradient_accumulation/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/engine/gradient_accumulation/_gradient_accumulation.py` & `colossalai-nightly-2023.5.6/colossalai/engine/gradient_accumulation/_gradient_accumulation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/engine/gradient_handler/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/engine/gradient_handler/_base_gradient_handler.py` & `colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_base_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py` & `colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/engine/gradient_handler/_moe_gradient_handler.py` & `colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_moe_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py` & `colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py` & `colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/engine/gradient_handler/_zero_gradient_handler.py` & `colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/_zero_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/engine/gradient_handler/utils.py` & `colossalai-nightly-2023.5.6/colossalai/engine/gradient_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/engine/schedule/_base_schedule.py` & `colossalai-nightly-2023.5.6/colossalai/engine/schedule/_base_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/engine/schedule/_non_pipeline_schedule.py` & `colossalai-nightly-2023.5.6/colossalai/engine/schedule/_non_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/engine/schedule/_pipeline_schedule.py` & `colossalai-nightly-2023.5.6/colossalai/engine/schedule/_pipeline_schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,17 +148,17 @@
             return [val[offset:offset + self.microbatch_size] for val in data]
         elif isinstance(data, dict):
             return {k: v[offset:offset + self.microbatch_size] for k, v in data.items()}
         else:
             raise TypeError(f"Expected data to be of type torch.Tensor, list, tuple, or dict, but got {type(data)}")
 
     def load_micro_batch(self):
-        micro_batch_data = self._get_data_slice(self.batch_data, self.microbatch_offset)
+        mciro_batch_data = self._get_data_slice(self.batch_data, self.microbatch_offset)
         self.microbatch_offset += self.microbatch_size
-        return self._move_to_device(micro_batch_data)
+        return self._move_to_device(mciro_batch_data)
 
     def pre_processing(self, engine):
         from colossalai.zero.legacy import ShardedModelV2
 
         # TODO: remove this after testing new zero with pipeline parallelism
         model = engine.model
         if isinstance(model, NaiveAMPModel):
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/engine/schedule/_pipeline_schedule_v2.py` & `colossalai-nightly-2023.5.6/colossalai/engine/schedule/_pipeline_schedule_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             Tuple[:class:`torch.Tensor`]: A tuple of (output, label, loss), loss and label could be None.
         """
 
         assert forward_only or return_loss, \
             'The argument \'return_loss\' has to be True when \'forward_only\' is False, but got False.'
         self.load_batch(data_iter)
 
-        # num_warmup_microbatches is the step when not all the processes are working
+        # num_warmup_microbatches is the step when not all the processers are working
         num_warmup_microbatches = \
             (gpc.get_world_size(ParallelMode.PIPELINE)
              - gpc.get_local_rank(ParallelMode.PIPELINE) - 1)
         num_warmup_microbatches = min(num_warmup_microbatches, self.num_microbatches)
         num_microbatches_remaining = self.num_microbatches - num_warmup_microbatches
 
         # Input, output tensors only need to be saved when doing backward passes
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/_compatibility.py` & `colossalai-nightly-2023.5.6/colossalai/fx/_compatibility.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/_meta_regist_13.py` & `colossalai-nightly-2023.5.6/colossalai/fx/_meta_regist_13.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/codegen/activation_checkpoint_codegen.py` & `colossalai-nightly-2023.5.6/colossalai/fx/codegen/activation_checkpoint_codegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -519,15 +519,15 @@
         inputs, outputs = _find_input_and_output_nodes(offload_node_list)
         offload_inputs.append(inputs)
         offload_outputs.append(outputs)
 
     # append code text to body
     for idx, node in enumerate(node_list):
         # if this is the first node of the ckpt region
-        # append the ckpt function definition
+        # append the ckpt function defition
         if idx in start_idx:
             label = start_idx.index(idx)
             ckpt_fn_def = _gen_ckpt_fn_def(label, input_vars[label])
             ckpt_func.append(f'{ckpt_fn_def}\n')
             within_ckpt_region = True
 
         if idx in offload_starts:
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/graph_module.py` & `colossalai-nightly-2023.5.6/colossalai/fx/graph_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/passes/adding_split_node_pass.py` & `colossalai-nightly-2023.5.6/colossalai/fx/passes/adding_split_node_pass.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
                 split_node = mod_graph.create_node('call_function', pipe_split)
     gm.recompile()
     return gm
 
 
 def avgnode_split_pass(gm: torch.fx.GraphModule, pp_size: int):
     """
-    In avgnode_split_pass, simply split graph by node number.
+    In avgnode_split_pass, simpliy split graph by node number.
     """
     mod_graph = gm.graph
     avg_num_node = len(mod_graph.nodes) // pp_size
     accumulate_num_node = 0
     for node in mod_graph.nodes:
         if pp_size <= 1:
             break
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/passes/concrete_info_prop.py` & `colossalai-nightly-2023.5.6/colossalai/fx/passes/concrete_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/passes/meta_info_prop.py` & `colossalai-nightly-2023.5.6/colossalai/fx/passes/meta_info_prop.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     shape: torch.Size
     dtype: torch.dtype
     requires_grad: bool
     stride: Tuple[int]
     numel: int
     is_tensor: bool
     # TODO: we can add a list of sharding spec here, and record the sharding
-    # behavior by appending sharding spec into list.
+    # behaviour by appending sharding spec into list.
 
 
 def _extract_tensor_metadata(result: torch.Tensor) -> TensorMetadata:
     """
     Extract a TensorMetadata NamedTuple describing `result`.
     """
     shape = result.shape
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/passes/passes_for_gpt2_test.py` & `colossalai-nightly-2023.5.6/colossalai/fx/passes/passes_for_gpt2_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
             if use_partition_name is not None:
                 use_partition = partitions[use_partition_name]
                 use_partition.inputs.setdefault(def_node.name)
                 if def_partition_name is not None:
                     use_partition.partitions_dependent_on.setdefault(def_partition_name)
 
     node_process_list = list(m.graph.nodes)
-    # split nodes into partitions
+    # split nodes into parititons
     while node_process_list:
         node = node_process_list.pop(0)
         orig_nodes[node.name] = node
 
         if node.op in ["placeholder"]:
             continue
         if node.op == 'output':
@@ -273,15 +273,15 @@
         for dependent in partitions[root_partition].partition_dependents:
             partitions[dependent].partitions_dependent_on.pop(root_partition)
             if not partitions[dependent].partitions_dependent_on:
                 root_partitions.append(dependent)
     if len(sorted_partitions) != len(partitions):
         raise RuntimeError("cycle exists between partitions!")
 
-    # add placeholders to partitions
+    # add placeholders to parititons
     for partition_name in sorted_partitions:
         partition = partitions[partition_name]
         for input in partition.inputs:
             placeholder = partition.graph.placeholder(input)
             placeholder.meta = orig_nodes[input].meta.copy()
             partition.environment[orig_nodes[input]] = placeholder
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/passes/shard_1d_pass.py` & `colossalai-nightly-2023.5.6/colossalai/fx/passes/shard_1d_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/passes/split_module.py` & `colossalai-nightly-2023.5.6/colossalai/fx/passes/split_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,16 @@
         self.targets: Dict[str, Any] = {}
 
     def __repr__(self) -> str:
         return f"name: {self.name},\n" \
             f" nodes: {self.node_names},\n" \
             f" inputs: {self.inputs},\n" \
             f" outputs: {self.outputs},\n" \
-            f" partitions dependent on: {self.partitions_dependent_on},\n" \
-            f" partition dependents: {self.partition_dependents}"
+            f" partitions depenent on: {self.partitions_dependent_on},\n" \
+            f" parition dependents: {self.partition_dependents}"
 
 
 # Creates subgraphs out of main graph
 @compatibility(is_backward_compatible=True)
 def split_module(
     m: GraphModule,
     root_m: torch.nn.Module,
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/passes/utils.py` & `colossalai-nightly-2023.5.6/colossalai/fx/passes/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/constants.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/dataflow.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/dataflow.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/constants.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_function/activation_function.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_function/embedding.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_function/normalization.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_function/pooling.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_module/activation_function.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_module/attention.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_module/convolution.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_module/normalization.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_module/pooling.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/profiler_module/rnn.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/profiler_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/registry.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/experimental/shard_utils.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/experimental/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/memory_utils.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/memory_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/opcount.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/opcount.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/profiler.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/shard_utils.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/profiler/tensor.py` & `colossalai-nightly-2023.5.6/colossalai/fx/profiler/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/proxy.py` & `colossalai-nightly-2023.5.6/colossalai/fx/proxy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/_meta_trace.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/_meta_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/_symbolic_trace.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/_symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/_tracer_utils.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/_tracer_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/experimental.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/experimental.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_function/convolution.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_function/embedding.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_function/normalization.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_module/convolution.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_module/pooling.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/meta_patch/patched_module/rnn.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/meta_patch/patched_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/registry.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/fx/tracer/tracer.py` & `colossalai-nightly-2023.5.6/colossalai/fx/tracer/tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/global_variables.py` & `colossalai-nightly-2023.5.6/colossalai/global_variables.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/initialize.py` & `colossalai-nightly-2023.5.6/colossalai/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/interface/model.py` & `colossalai-nightly-2023.5.6/colossalai/interface/model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/interface/optimizer.py` & `colossalai-nightly-2023.5.6/colossalai/interface/optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/cpu_adam.h` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/context.h` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/context.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/csrc/type_shim.h` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/csrc/type_shim.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/flash_attention.py` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/flash_attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/layer_norm.py` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/layer_norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/multihead_attention.py` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/cuda_native/scaled_softmax.py` & `colossalai-nightly-2023.5.6/colossalai/kernel/cuda_native/scaled_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/jit/bias_dropout_add.py` & `colossalai-nightly-2023.5.6/colossalai/kernel/jit/bias_dropout_add.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/jit/bias_gelu.py` & `colossalai-nightly-2023.5.6/colossalai/kernel/jit/bias_gelu.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/jit/option.py` & `colossalai-nightly-2023.5.6/colossalai/kernel/jit/option.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/builder.py` & `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/cpu_adam.py` & `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/fused_optim.py` & `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/fused_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/layernorm.py` & `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/moe.py` & `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/multi_head_attn.py` & `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/scaled_masked_softmax.py` & `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/scaled_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py` & `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/kernel/op_builder/utils.py` & `colossalai-nightly-2023.5.6/colossalai/kernel/op_builder/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     import torch
 
     try:
         torch_cuda_major = torch.version.cuda.split(".")[0]
         torch_cuda_minor = torch.version.cuda.split(".")[1]
     except:
         raise ValueError(
-            "[extension] Cannot retrieve the CUDA version in the PyTorch binary given by torch.version.cuda")
+            "[extension] Cannot retrive the CUDA version in the PyTorch binary given by torch.version.cuda")
     return torch_cuda_major, torch_cuda_minor
 
 
 def get_cuda_bare_metal_version(cuda_dir) -> List[int]:
     """
     Get the System CUDA version from nvcc.
 
@@ -106,15 +106,15 @@
     Returns:
         A tuple of integers in the form of (major, minor, patch).
     """
     import torch
     torch_version = torch.__version__.split('+')[0]
     TORCH_MAJOR = int(torch_version.split('.')[0])
     TORCH_MINOR = int(torch_version.split('.')[1])
-    TORCH_PATCH = int(torch_version.split('.')[2], 16)
+    TORCH_PATCH = int(torch_version.split('.')[2])
     return TORCH_MAJOR, TORCH_MINOR, TORCH_PATCH
 
 
 def check_pytorch_version(min_major_version, min_minor_version) -> bool:
     """
     Compare the current PyTorch version with the minium required version.
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/logging/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/logging/logger.py` & `colossalai-nightly-2023.5.6/colossalai/logging/logger.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/_ops/_utils.py` & `colossalai-nightly-2023.5.6/colossalai/nn/_ops/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/_ops/addmm.py` & `colossalai-nightly-2023.5.6/colossalai/nn/_ops/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/_ops/batch_norm.py` & `colossalai-nightly-2023.5.6/colossalai/nn/_ops/batch_norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/_ops/element_wise.py` & `colossalai-nightly-2023.5.6/colossalai/nn/_ops/element_wise.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/_ops/embedding.py` & `colossalai-nightly-2023.5.6/colossalai/nn/_ops/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/_ops/embedding_bag.py` & `colossalai-nightly-2023.5.6/colossalai/nn/_ops/embedding_bag.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/_ops/layernorm.py` & `colossalai-nightly-2023.5.6/colossalai/nn/_ops/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/_ops/linear.py` & `colossalai-nightly-2023.5.6/colossalai/nn/_ops/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/_ops/loss.py` & `colossalai-nightly-2023.5.6/colossalai/nn/_ops/loss.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/_ops/view.py` & `colossalai-nightly-2023.5.6/colossalai/nn/_ops/view.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/init.py` & `colossalai-nightly-2023.5.6/colossalai/nn/init.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/base_layer.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/base_layer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/colossalai_layer/_utils.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/colossalai_layer/dropout.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/dropout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/colossalai_layer/embedding.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/colossalai_layer/linear.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/colossalai_layer/normalization.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/colossalai_layer/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/moe/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/moe/_operation.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/moe/checkpoint.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/moe/experts.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/experts.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/moe/layers.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/moe/routers.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/routers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/moe/utils.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/moe/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_1d/_operation.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_1d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_1d/_utils.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_1d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_1d/layers.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_1d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_2d/_operation.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_2d/_utils.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_2d/layers.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_2p5d/_operation.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2p5d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_2p5d/_utils.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2p5d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_2p5d/layers.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_2p5d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_3d/_operation.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_3d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_3d/_utils.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_3d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_3d/layers.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_3d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_sequence/_operation.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_sequence/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/parallel_sequence/layers.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/parallel_sequence/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/utils/common.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/vanilla/layers.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/vanilla/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/layer/wrapper/pipeline_wrapper.py` & `colossalai-nightly-2023.5.6/colossalai/nn/layer/wrapper/pipeline_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/loss/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/nn/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/loss/loss_1d.py` & `colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_1d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/loss/loss_2d.py` & `colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/loss/loss_2p5d.py` & `colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/loss/loss_3d.py` & `colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/loss/loss_moe.py` & `colossalai-nightly-2023.5.6/colossalai/nn/loss/loss_moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/lr_scheduler/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/lr_scheduler/cosine.py` & `colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/cosine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/lr_scheduler/delayed.py` & `colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/delayed.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/lr_scheduler/linear.py` & `colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/lr_scheduler/multistep.py` & `colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/multistep.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/lr_scheduler/onecycle.py` & `colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/onecycle.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/lr_scheduler/poly.py` & `colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/poly.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/lr_scheduler/torch.py` & `colossalai-nightly-2023.5.6/colossalai/nn/lr_scheduler/torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/metric/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/nn/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/metric/accuracy_2d.py` & `colossalai-nightly-2023.5.6/colossalai/nn/metric/accuracy_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/metric/accuracy_2p5d.py` & `colossalai-nightly-2023.5.6/colossalai/nn/metric/accuracy_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/metric/accuracy_3d.py` & `colossalai-nightly-2023.5.6/colossalai/nn/metric/accuracy_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/optimizer/colossalai_optimizer.py` & `colossalai-nightly-2023.5.6/colossalai/nn/optimizer/colossalai_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/optimizer/cpu_adam.py` & `colossalai-nightly-2023.5.6/colossalai/nn/optimizer/cpu_adam.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .nvme_optimizer import NVMeOptimizer
 
 
 @OPTIMIZERS.register_module
 class CPUAdam(NVMeOptimizer):
     """Implements Adam algorithm.
 
-    Supports parameters updating on both GPU and CPU, depanding on the device of parameters.
+    Supports parameters updating on both GPU and CPU, depanding on the device of paramters.
     But the parameters and gradients should on the same device:
       * Parameters on CPU and gradients on CPU is allowed.
       * Parameters on GPU and gradients on GPU is allowed.
       * Parameters on GPU and gradients on CPU is **not** allowed.
 
     `CPUAdam` requires CUDA extensions which can be built during installation or runtime.
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/optimizer/fused_adam.py` & `colossalai-nightly-2023.5.6/colossalai/nn/optimizer/fused_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/optimizer/fused_lamb.py` & `colossalai-nightly-2023.5.6/colossalai/nn/optimizer/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/optimizer/fused_sgd.py` & `colossalai-nightly-2023.5.6/colossalai/nn/optimizer/fused_sgd.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/optimizer/hybrid_adam.py` & `colossalai-nightly-2023.5.6/colossalai/nn/optimizer/hybrid_adam.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 from .nvme_optimizer import NVMeOptimizer
 
 
 @OPTIMIZERS.register_module
 class HybridAdam(NVMeOptimizer):
     """Implements Adam algorithm.
 
-    Supports parameters updating on both GPU and CPU, depanding on the device of parameters.
+    Supports parameters updating on both GPU and CPU, depanding on the device of paramters.
     But the parameters and gradients should on the same device:
       * Parameters on CPU and gradients on CPU is allowed.
       * Parameters on GPU and gradients on GPU is allowed.
       * Parameters on GPU and gradients on CPU is **not** allowed.
 
-    `HybridAdam` requires CUDA extensions which can be built during installation or runtime.
+    `HybriadAdam` requires CUDA extensions which can be built during installation or runtime.
 
     This version of Hybrid Adam is an hybrid of CPUAdam and FusedAdam.
 
     * For parameters updating on CPU, it uses CPUAdam.
     * For parameters updating on GPU, it uses FusedAdam.
-    * Hybrid precision calculation of fp16 and fp32 is supported, eg fp32 parameters and fp16 gradients.
+    * Hybird precision calculation of fp16 and fp32 is supported, eg fp32 parameters and fp16 gradients.
 
     :class:`colossalai.nn.optimizer.HybridAdam` may be used as a drop-in replacement for ``torch.optim.AdamW``,
     or ``torch.optim.Adam`` with ``adamw_mode=False``
 
     Adam was been proposed in `Adam: A Method for Stochastic Optimization`_.
 
     Arguments:
@@ -127,15 +127,15 @@
                                           state['exp_avg_sq'], div_scale)
                     self._post_update(p, 'exp_avg', 'exp_avg_sq')
 
                 elif target_device.type == 'cuda':
                     assert state['exp_avg'].device.type == 'cuda', "exp_avg should stay on cuda"
                     assert state['exp_avg_sq'].device.type == 'cuda', "exp_avg should stay on cuda"
 
-                    # record the state by group and update at once
+                    # record the state by gruop and update at once
                     g_l.append(p.grad.data)
                     p_l.append(p.data)
                     m_l.append(state['exp_avg'])
                     v_l.append(state['exp_avg_sq'])
 
                 else:
                     raise RuntimeError
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/optimizer/lamb.py` & `colossalai-nightly-2023.5.6/colossalai/nn/optimizer/lamb.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/optimizer/lars.py` & `colossalai-nightly-2023.5.6/colossalai/nn/optimizer/lars.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/optimizer/nvme_optimizer.py` & `colossalai-nightly-2023.5.6/colossalai/nn/optimizer/nvme_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/parallel/data_parallel.py` & `colossalai-nightly-2023.5.6/colossalai/nn/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py` & `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py` & `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 
 def _wait_for_data(t, stream: Optional[torch.cuda.streams.Stream]) -> None:
     if stream is None:
         return
     torch.cuda.current_stream().wait_stream(stream)
     # As mentioned in https://pytorch.org/docs/stable/generated/torch.Tensor.record_stream.html,
-    # PyTorch uses the "caching allocator" for memory allocation for tensors. When a tensor is
-    # freed, its memory is likely to be reused by newly constructed tensors.  By default,
+    # PyTorch uses the "caching allocator" for memroy allocation for tensors. When a tensor is
+    # freed, its memory is likely to be reused by newly constructed tenosrs.  By default,
     # this allocator traces whether a tensor is still in use by only the CUDA stream where it
     # was created.   When a tensor is used by additional CUDA streams, we need to call record_stream
     # to tell the allocator about all these streams.  Otherwise, the allocator might free the
     # underlying memory of the tensor once it is no longer used by the creator stream.  This is
     # a notable programming trick when we write programs using multi CUDA streams.
     cur_stream = torch.cuda.current_stream()
     assert isinstance(t, torch.Tensor)
@@ -290,15 +290,15 @@
             )
             print(f'cuda_to_cpu_elapse {elapsed} sec')
         if self._cpu_to_cuda_numel > 0 and "5_evict_in" in self._elapsed_dict:
             elapsed = self._elapsed_dict["5_evict_in"]
             print(
                 f"CPU->CUDA BWD {self._cpu_to_cuda_numel * self.elem_size_in_byte / 1e6 / elapsed} MB/s {self._cpu_to_cuda_numel / 1e6} M elem"
             )
-            print(f'cpu_to_cuda_elapse {elapsed} sec')
+            print(f'cpu_to_cuda_elpase {elapsed} sec')
 
         for k, v in self._elapsed_dict.items():
             print(f'{k}: {v}')
 
         print(f'cache miss ratio {self._cache_miss / self._total_cache}')
 
     @torch.no_grad()
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py` & `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/copyer.py` & `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/copyer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py` & `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py` & `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py` & `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py` & `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/colo_module.py` & `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/colo_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/embedding.py` & `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/linear.py` & `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/parallel/layers/module_utils.py` & `colossalai-nightly-2023.5.6/colossalai/nn/parallel/layers/module_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/nn/parallel/reducer.py` & `colossalai-nightly-2023.5.6/colossalai/nn/parallel/reducer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/pipeline/layer_spec.py` & `colossalai-nightly-2023.5.6/colossalai/pipeline/layer_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/pipeline/middleware/adaptor/fx.py` & `colossalai-nightly-2023.5.6/colossalai/pipeline/middleware/adaptor/fx.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/pipeline/middleware/topo.py` & `colossalai-nightly-2023.5.6/colossalai/pipeline/middleware/topo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/pipeline/pipeline_process_group.py` & `colossalai-nightly-2023.5.6/colossalai/pipeline/pipeline_process_group.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/pipeline/rpc/_pipeline_base.py` & `colossalai-nightly-2023.5.6/colossalai/pipeline/rpc/_pipeline_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/pipeline/rpc/_pipeline_schedule.py` & `colossalai-nightly-2023.5.6/colossalai/pipeline/rpc/_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/pipeline/rpc/utils.py` & `colossalai-nightly-2023.5.6/colossalai/pipeline/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/pipeline/utils.py` & `colossalai-nightly-2023.5.6/colossalai/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/registry/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/registry/registry.py` & `colossalai-nightly-2023.5.6/colossalai/registry/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/colo_parameter.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/colo_parameter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/colo_tensor.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/colo_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/comm_spec.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/comm_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/compute_spec.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/compute_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/d_tensor/comm_spec.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/comm_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/d_tensor/d_tensor.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/d_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/d_tensor/layout.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/layout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/d_tensor/layout_converter.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/layout_converter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/d_tensor/sharding_spec.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/sharding_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/d_tensor/utils.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/d_tensor/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/dist_spec_mgr.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/dist_spec_mgr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from contextlib import contextmanager
 
 import torch
 import torch.distributed as dist
 # from colossalai.nn.layer.utils import divide
 from numpy import prod
+from packaging import version
 
-from colossalai.tensor.distspec import DistPlacementPattern, _DistSpec
+from colossalai.logging import get_dist_logger
+from colossalai.tensor.distspec import _DistSpec
 from colossalai.tensor.process_group import ProcessGroup
 
 
 # TODO(jiaruifang) circle import, move the divide to colossalai.commons.
 # colossalai.tensor shall not import any submodule from colossal.nn
 def divide(numerator, denominator):
     """Only allow exact division.
@@ -165,29 +167,19 @@
         return DistSpecManager._shard_as(tensor, old_dist_spec, dist_spec, pg)
 
     @staticmethod
     def handle_trans_spec(tensor: torch.Tensor, old_dist_spec: _DistSpec, dist_spec: _DistSpec,
                           pg: ProcessGroup) -> torch.Tensor:
         assert isinstance(old_dist_spec, _DistSpec), f"{type(old_dist_spec)} should be _DistSpec"
         assert isinstance(dist_spec, _DistSpec), f"{type(dist_spec)} should be _DistSpec"
-
-        trans_func_key = (old_dist_spec.placement, dist_spec.placement)
-        trans_funcs = {
-            (DistPlacementPattern.REPLICATE, DistPlacementPattern.REPLICATE): DistSpecManager._r2r,
-            (DistPlacementPattern.REPLICATE, DistPlacementPattern.SHARD): DistSpecManager._r2s,
-            (DistPlacementPattern.SHARD, DistPlacementPattern.REPLICATE): DistSpecManager._s2r,
-            (DistPlacementPattern.SHARD, DistPlacementPattern.SHARD): DistSpecManager._s2s
-        }
-
-        forward_trans_handle = trans_funcs[trans_func_key]
+        forward_trans_handle = getattr(DistSpecManager, f'_{old_dist_spec.placement.value}2{dist_spec.placement.value}')
         if not DistSpecManager._use_autograd_function:
             return forward_trans_handle(tensor, old_dist_spec, dist_spec, pg)
-
-        backward_trans_handle = trans_funcs[(dist_spec.placement, old_dist_spec.placement)]
-
+        backward_trans_handle = getattr(DistSpecManager,
+                                        f'_{dist_spec.placement.value}2{old_dist_spec.placement.value}')
         return TransformDistSpec.apply(tensor, old_dist_spec, dist_spec, pg, forward_trans_handle,
                                        backward_trans_handle)
 
     @staticmethod
     @contextmanager
     def no_grad():
         try:
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/distspec.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/distspec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/op_wrapper.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/op_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/param_op_hook.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/param_op_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/process_group.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/process_group.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/shape_consistency.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/shape_consistency.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/sharding_spec.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/sharding_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/tensor_spec.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/tensor_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/tensor/utils.py` & `colossalai-nightly-2023.5.6/colossalai/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/testing/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/testing/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-from .comparison import (
-    assert_close,
-    assert_close_loose,
-    assert_equal,
-    assert_equal_in_group,
-    assert_not_equal,
-    check_state_dict_equal,
-)
+from .comparison import assert_close, assert_close_loose, assert_equal, assert_equal_in_group, assert_not_equal
 from .pytest_wrapper import run_on_environment_flag
 from .utils import (
     clear_cache_before_run,
     free_port,
     parameterize,
     rerun_if_address_is_in_use,
     rerun_on_exception,
     skip_if_not_enough_gpus,
     spawn,
 )
 
 __all__ = [
     'assert_equal', 'assert_not_equal', 'assert_close', 'assert_close_loose', 'assert_equal_in_group', 'parameterize',
     'rerun_on_exception', 'rerun_if_address_is_in_use', 'skip_if_not_enough_gpus', 'free_port', 'spawn',
-    'clear_cache_before_run', 'run_on_environment_flag', 'check_state_dict_equal'
+    'clear_cache_before_run', 'run_on_environment_flag'
 ]
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/testing/pytest_wrapper.py` & `colossalai-nightly-2023.5.6/colossalai/testing/pytest_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,12 +29,12 @@
         # this will skip your test
         pytest test_for_something.py
 
     """
     assert isinstance(name, str)
     flag = os.environ.get(name.upper(), '0')
 
-    reason = f'Environment variable {name} is {flag}'
+    reason = f'Environment varialbe {name} is {flag}'
     if flag == '1':
         return pytest.mark.skipif(False, reason=reason)
     else:
         return pytest.mark.skipif(True, reason=reason)
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/testing/random.py` & `colossalai-nightly-2023.5.6/colossalai/testing/random.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/testing/utils.py` & `colossalai-nightly-2023.5.6/colossalai/testing/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,18 +163,18 @@
         @rerun_if_address_is_in_use()
         def test_something():
             ...
 
     """
     # check version
     torch_version = version.parse(torch.__version__)
-    assert torch_version.major >= 1
+    assert torch_version.major == 1
 
     # only torch >= 1.8 has ProcessRaisedException
-    if torch_version >= version.parse("1.8.0"):
+    if torch_version.minor >= 8:
         exception = torch.multiprocessing.ProcessRaisedException
     else:
         exception = Exception
 
     func_wrapper = rerun_on_exception(exception_type=exception, pattern=".*Address already in use.*")
     return func_wrapper
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/trainer/_trainer.py` & `colossalai-nightly-2023.5.6/colossalai/trainer/_trainer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/trainer/hooks/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/trainer/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/trainer/hooks/_base_hook.py` & `colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_base_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/trainer/hooks/_checkpoint_hook.py` & `colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_checkpoint_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/trainer/hooks/_log_hook.py` & `colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_log_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/trainer/hooks/_lr_scheduler_hook.py` & `colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_lr_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/trainer/hooks/_metric_hook.py` & `colossalai-nightly-2023.5.6/colossalai/trainer/hooks/_metric_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/activation_checkpoint.py` & `colossalai-nightly-2023.5.6/colossalai/utils/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/checkpoint/module_checkpoint.py` & `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint/module_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/checkpoint/utils.py` & `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/backend.py` & `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/backend.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/convertor.py` & `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/convertor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/distributed.py` & `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/distributed.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/io.py` & `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/io.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/meta.py` & `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/meta.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/reader.py` & `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/reader.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/utils.py` & `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/checkpoint_io/writer.py` & `colossalai-nightly-2023.5.6/colossalai/utils/checkpoint_io/writer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/checkpointing.py` & `colossalai-nightly-2023.5.6/colossalai/utils/checkpointing.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/common.py` & `colossalai-nightly-2023.5.6/colossalai/utils/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,15 @@
     else:
         enable_cuda_kernels = params[0].grad.device.type == 'cuda'
     # Norm parameters.
     max_norm = float(max_norm)
     norm_type = float(norm_type)
 
     # Parameters can be on CPU or CUDA
-    # If parameters are on CPU, disable CUDA kernels
+    # If parameters are on CPU, disable CUDA kernerls
 
     # Calculate norm.
     if norm_type == inf:
         total_norm = max(p.grad.data.abs().max() for p in params)
         total_norm_cuda = torch.cuda.FloatTensor([float(total_norm)])
         # Take max across all model-parallel GPUs.
         if gpc.is_initialized(ParallelMode.MODEL) and gpc.get_world_size(ParallelMode.MODEL) > 1:
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/cuda.py` & `colossalai-nightly-2023.5.6/colossalai/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/data_sampler/data_parallel_sampler.py` & `colossalai-nightly-2023.5.6/colossalai/utils/data_sampler/data_parallel_sampler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/memory.py` & `colossalai-nightly-2023.5.6/colossalai/utils/memory.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/model/experimental.py` & `colossalai-nightly-2023.5.6/colossalai/utils/model/experimental.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/model/utils.py` & `colossalai-nightly-2023.5.6/colossalai/utils/model/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/moe.py` & `colossalai-nightly-2023.5.6/colossalai/utils/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py` & `colossalai-nightly-2023.5.6/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/profiler/legacy/comm_profiler.py` & `colossalai-nightly-2023.5.6/colossalai/utils/profiler/legacy/comm_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/profiler/legacy/pcie_profiler.py` & `colossalai-nightly-2023.5.6/colossalai/utils/profiler/legacy/pcie_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/profiler/legacy/prof_utils.py` & `colossalai-nightly-2023.5.6/colossalai/utils/profiler/legacy/prof_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/profiler/profiler.py` & `colossalai-nightly-2023.5.6/colossalai/utils/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/profiler/stateful_tensor_mem_extention.py` & `colossalai-nightly-2023.5.6/colossalai/utils/profiler/stateful_tensor_mem_extention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/rank_recorder/rank_recorder.py` & `colossalai-nightly-2023.5.6/colossalai/utils/rank_recorder/rank_recorder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/tensor_detector/tensor_detector.py` & `colossalai-nightly-2023.5.6/colossalai/utils/tensor_detector/tensor_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         memory_size = tensor.element_size() * tensor.storage().size()
         if (tensor.is_leaf or tensor.retains_grad) and tensor.grad is not None:
             grad_memory_size = tensor.grad.element_size() * tensor.grad.storage().size()
             memory_size += grad_memory_size
         return self.mem_format(memory_size)
 
     def mem_format(self, real_memory_size):
-        # format the tensor memory into a reasonable magnitude
+        # format the tensor memory into a reasonal magnitude
         if real_memory_size >= 2**30:
             return str(real_memory_size / (2**30)) + ' GB'
         if real_memory_size >= 2**20:
             return str(real_memory_size / (2**20)) + ' MB'
         if real_memory_size >= 2**10:
             return str(real_memory_size / (2**10)) + ' KB'
         return str(real_memory_size) + ' B'
@@ -67,28 +67,28 @@
     def collect_tensors_state(self):
         for obj in gc.get_objects():
             if torch.is_tensor(obj):
                 # skip cpu tensor when include_cpu is false and the tensor we have collected before
                 if (not self.include_cpu) and obj.device == torch.device('cpu'):
                     continue
                 self.detected.append(id(obj))
-                # skip parameters we had added in __init__ when module is an instance of nn.Module for the first epoch
+                # skip paramters we had added in __init__ when module is an instance of nn.Module for the first epoch
                 if id(obj) not in self.tensor_info:
 
                     name = type(obj).__name__
                     # after backward, we want to update the records, to show you the change
                     if isinstance(self.module, nn.Module) and name == 'Parameter':
                         if obj.grad is not None:
                             # with grad attached
                             for par_name, param in self.module.named_parameters():
                                 if param.requires_grad and param.grad.equal(obj.grad):
                                     name = par_name + ' (with grad)'
                         else:
                             # with no grad attached
-                            # there will be no new parameters created during running
+                            # there will be no new paramters created during running
                             # so it must be in saved_tensor_info
                             continue
                     # we can also marked common tensors as tensor(with grad)
                     if name == 'Tensor' and (obj.is_leaf or obj.retains_grad):
                         if obj.grad is not None:
                             name = name + ' (with grad)'
                     # in fact, common tensor have no grad
@@ -151,15 +151,15 @@
 
         self.info += LINE
         self.info += f"Detect Location: {locate_msg}\n"
         for device in self.devices:
             if device == torch.device('cpu'):
                 continue
             gpu_mem_alloc = self.mem_format(torch.cuda.memory_allocated(device))
-            self.info += f"Total GPU Memory Allocated on {device} is {gpu_mem_alloc}\n"
+            self.info += f"Totle GPU Memery Allocated on {device} is {gpu_mem_alloc}\n"
         self.info += LINE
         self.info += '\n\n'
         if self.show_info:
             print(self.info)
         if self.log is not None:
             with open(self.log + '.log', 'a') as f:
                 f.write(self.info)
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/utils/timer.py` & `colossalai-nightly-2023.5.6/colossalai/utils/timer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/zero/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/chunk/chunk.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/chunk.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/chunk/manager.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,51 +98,51 @@
             self.__close_one_chunk(self.chunk_groups[group_name][-1])
 
     def access_chunk(self, chunk: Chunk) -> None:
         """Make the chunk can be used for calculation.
         """
         if chunk in self.accessed_chunks:
             return
-        self.__sub_memory_usage(chunk.memory_usage)
+        self.__sub_memroy_usage(chunk.memory_usage)
         if chunk.device_type == 'cpu':
             chunk.shard_move(get_current_device())
         self.__add_accessed_chunk(chunk)
         self.__add_memory_usage(chunk.memory_usage)
 
     def release_chunk(self, chunk: Chunk) -> None:
         """Scatter the chunk in CUDA.
         """
         if chunk not in self.accessed_chunks:
             return
         if chunk.can_release:
-            self.__sub_memory_usage(chunk.memory_usage)
+            self.__sub_memroy_usage(chunk.memory_usage)
             self.__sub_accessed_chunk(chunk)
             self.__add_memory_usage(chunk.memory_usage)
 
     def move_chunk(self, chunk: Chunk, device: torch.device, force_copy: bool = False) -> None:
         """Move the shard of the chunk to the target device.
         """
         if not chunk.can_move or chunk.device_type == device.type:
             return
-        self.__sub_memory_usage(chunk.memory_usage)
+        self.__sub_memroy_usage(chunk.memory_usage)
         chunk.shard_move(device, force_copy)
         self.__add_memory_usage(chunk.memory_usage)
 
     def trans_tensor_state(self, tensor: torch.Tensor, state: TensorState) -> None:
         """Transit tensor state according to pre-defined state machine.
         """
         chunk = self.tensor_chunk_map[tensor]
         chunk.tensor_trans_state(tensor, state)
 
     def reduce_chunk(self, chunk: Chunk) -> bool:
         """Reduce or all reduce the chunk.
         """
         if not chunk.can_reduce:
             return False
-        self.__sub_memory_usage(chunk.memory_usage)
+        self.__sub_memroy_usage(chunk.memory_usage)
         chunk.reduce()
         self.__sub_accessed_chunk(chunk)
         self.__add_memory_usage(chunk.memory_usage)
         return True
 
     def fake_release_chunk(self, chunk: Chunk) -> None:
         """Release gathered chunk in a fake mode.
@@ -224,19 +224,19 @@
         """Register a chunk group.
         """
         if group_name not in self.chunk_groups:
             self.chunk_groups[group_name] = deque()
         return self.chunk_groups[group_name]
 
     def __close_one_chunk(self, chunk: Chunk):
-        self.__sub_memory_usage(chunk.memory_usage)
+        self.__sub_memroy_usage(chunk.memory_usage)
         chunk.close_chunk()
         self.__add_memory_usage(chunk.memory_usage)
 
-    def __sub_memory_usage(self, usage: Dict[str, int]):
+    def __sub_memroy_usage(self, usage: Dict[str, int]):
         for k, v in usage.items():
             self.total_mem[k] -= v
 
     def __add_memory_usage(self, usage: Dict[str, int]):
         for k, v in usage.items():
             self.total_mem[k] += v
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/chunk/search_utils.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/search_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 def classify_params_by_dp_degree(param_order: OrderedParamGenerator,
                                  strict_ddp_flag: bool = False) -> Dict[int, List[ColoParameter]]:
     """classify_params_by_dp_degree
 
     Classify the parameters by their dp degree
 
     Args:
-        param_order (OrderedParamGenerator): the order of param be vised
+        param_order (OrderedParamGenerator): the order of param be visied
         strict_ddp_flag (bool, optional): whether to enable the strict ddp mode. Defaults to False.
 
     Returns:
         Dict[int, List[ColoParameter]]: a dict contains the classification results.
         The keys are dp_degrees and the values are parameters.
     """
     params_dict: Dict[int, List[ColoParameter]] = dict()
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/chunk/utils.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/chunk/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/colo_init_context.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/colo_init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/gemini_ddp.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/gemini_ddp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/gemini_hook.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/gemini_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/gemini_mgr.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/gemini_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/gemini_optimizer.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/gemini_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/memory_monitor.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/memory_monitor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/memory_stats.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/memory_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     def increase_preop_step(self, param_list: List[torch.nn.Parameter]):
         """
         the time step is increased. param list is used between current and the next
         time step.
 
         Args:
-            param_list (List[torch.nn.Parameter]): a list of torch parameters.
+            param_list (List[torch.nn.Parameter]): a list of torch paramters.
         """
         for p in param_list:
             if p not in self._param_step_dict:
                 self._param_step_dict[p] = [self._preop_step]
             else:
                 self._param_step_dict[p].append(self._preop_step)
             self._param_runtime_order.append(p)
```

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/memstats_collector.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/param_runtime_order.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/param_runtime_order.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/memory_tracer/utils.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/memory_tracer/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/placement_policy.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/gemini/utils.py` & `colossalai-nightly-2023.5.6/colossalai/zero/gemini/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/__init__.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/gemini_context.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/gemini_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/ophooks/utils.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/ophooks/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/stateful_tensor.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/stateful_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/tensor_placement_policy.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/tensor_placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/gemini/tensor_utils.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/gemini/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/init_ctx/init_context.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/init_ctx/init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/shard_utils/base_shard_strategy.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/base_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/shard_utils/commons.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/commons.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_model/_utils.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_model/sharded_model_v2.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/sharded_model_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_model/utils.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_model/zero_hook.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_model/zero_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_param/sharded_param.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_param/sharded_param.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/legacy/sharded_param/sharded_tensor.py` & `colossalai-nightly-2023.5.6/colossalai/zero/legacy/sharded_param/sharded_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/low_level/_utils.py` & `colossalai-nightly-2023.5.6/colossalai/zero/low_level/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/low_level/bookkeeping/bucket_store.py` & `colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/bucket_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/low_level/bookkeeping/gradient_store.py` & `colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/gradient_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/low_level/bookkeeping/parameter_store.py` & `colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/parameter_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/low_level/bookkeeping/tensor_bucket.py` & `colossalai-nightly-2023.5.6/colossalai/zero/low_level/bookkeeping/tensor_bucket.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/low_level/low_level_optim.py` & `colossalai-nightly-2023.5.6/colossalai/zero/low_level/low_level_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai/zero/wrapper.py` & `colossalai-nightly-2023.5.6/colossalai/zero/wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/colossalai_nightly.egg-info/PKG-INFO` & `colossalai-nightly-2023.5.6/colossalai_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai-nightly
-Version: 2023.5.27
+Version: 2023.5.6
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
@@ -134,30 +134,20 @@
         <p align="right">(<a href="#top">back to top</a>)</p>
         
         ## Colossal-AI in the Real World
         
         ### ColossalChat
         
         <div align="center">
-           <a href="https://www.youtube.com/watch?v=HcTiHzApHm0">
-           <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chat/ColossalChat%20YouTube.png" width="700" />
+           <a href="https://chat.colossalai.org/">
+           <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Chat-demo.png" width="700" />
            </a>
         </div>
         
-        [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline.
-        [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat)
-        [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b)
-        [[demo]](https://www.youtube.com/watch?v=HcTiHzApHm0)
-        [[tutorial]](https://www.youtube.com/watch?v=-qFBZFmOJfg)
-        
-        <p id="ColossalChat-Speed" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chat/ColossalChat%20Speed.jpg" width=450/>
-        </p>
-        
-        - Up to 10 times faster for RLHF PPO Stage3 Training
+        [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://chat.colossalai.org)
         
         <p id="ColossalChat_scaling" align="center">
         <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT%20scaling.png" width=800/>
         </p>
         
         - Up to 7.73 times faster for single server training and 1.42 times faster for single-GPU inference
         
@@ -369,30 +359,14 @@
         By default, we do not compile CUDA/C++ kernels. ColossalAI will build them during runtime.
         If you want to install and enable CUDA kernel fusion (compulsory installation when using fused optimizer):
         
         ```shell
         CUDA_EXT=1 pip install .
         ```
         
-        For Users with CUDA 10.2, you can still build ColossalAI from source. However, you need to manually download the cub library and copy it to the corresponding directory.
-        
-        ```bash
-        # clone the repository
-        git clone https://github.com/hpcaitech/ColossalAI.git
-        cd ColossalAI
-        
-        # download the cub library
-        wget https://github.com/NVIDIA/cub/archive/refs/tags/1.8.0.zip
-        unzip 1.8.0.zip
-        cp -r cub-1.8.0/cub/ colossalai/kernel/cuda_native/csrc/kernels/include/
-        
-        # install
-        CUDA_EXT=1 pip install .
-        ```
-        
         <p align="right">(<a href="#top">back to top</a>)</p>
         
         ## Use Docker
         
         ### Pull from DockerHub
         
         You can directly pull the docker image from our [DockerHub page](https://hub.docker.com/r/hpcaitech/colossalai). The image is automatically uploaded upon release.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.5.27 Summary: An
+Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.5.6 Summary: An
 integrated large-scale model training system with efficient parallelization
 techniques Home-page: https://www.colossalai.org License: Apache Software
 License 2.0 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/
 discussions Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/
 issues Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
@@ -92,26 +92,23 @@
 /arxiv.org/abs/1910.02054) - [Auto-Parallelism](https://arxiv.org/abs/
 2302.02599) - Heterogeneous Memory Management - [PatrickStar](https://
 arxiv.org/abs/2108.05818) - Friendly Usage - Parallelism based on the
 configuration file - Inference - [Energon-AI](https://github.com/hpcaitech/
 EnergonAI)
                                                                   (back_to_top)
 ## Colossal-AI in the Real World ### ColossalChat
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                       chat/ColossalChat%20YouTube.png]
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                Chat-demo.png]
 [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/
 Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/
 chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/
 ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/
 @yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://www.youtube.com/
-watch?v=HcTiHzApHm0) [[tutorial]](https://www.youtube.com/watch?v=-qFBZFmOJfg)
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                        chat/ColossalChat%20Speed.jpg]
-- Up to 10 times faster for RLHF PPO Stage3 Training
+with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://
+chat.colossalai.org)
  [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
                         chatgpt/ChatGPT%20scaling.png]
 - Up to 7.73 times faster for single server training and 1.42 times faster for
 single-GPU inference
  [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
                            chatgpt/ChatGPT-1GPU.jpg]
 - Up to 10.3x growth in model capacity on one GPU - A mini demo training
@@ -228,22 +225,15 @@
 main branch. Installation can be made via ```bash pip install colossalai-
 nightly ``` ### Download From Source > The version of Colossal-AI will be in
 line with the main branch of the repository. Feel free to raise an issue if you
 encounter any problems. :) ```shell git clone https://github.com/hpcaitech/
 ColossalAI.git cd ColossalAI # install colossalai pip install . ``` By default,
 we do not compile CUDA/C++ kernels. ColossalAI will build them during runtime.
 If you want to install and enable CUDA kernel fusion (compulsory installation
-when using fused optimizer): ```shell CUDA_EXT=1 pip install . ``` For Users
-with CUDA 10.2, you can still build ColossalAI from source. However, you need
-to manually download the cub library and copy it to the corresponding
-directory. ```bash # clone the repository git clone https://github.com/
-hpcaitech/ColossalAI.git cd ColossalAI # download the cub library wget https://
-github.com/NVIDIA/cub/archive/refs/tags/1.8.0.zip unzip 1.8.0.zip cp -r cub-
-1.8.0/cub/ colossalai/kernel/cuda_native/csrc/kernels/include/ # install
-CUDA_EXT=1 pip install . ```
+when using fused optimizer): ```shell CUDA_EXT=1 pip install . ```
                                                                   (back_to_top)
 ## Use Docker ### Pull from DockerHub You can directly pull the docker image
 from our [DockerHub page](https://hub.docker.com/r/hpcaitech/colossalai). The
 image is automatically uploaded upon release. ### Build On Your Own Run the
 following command to build a docker image from Dockerfile provided. > Building
 Colossal-AI from scratch requires GPU support, you need to use Nvidia Docker
 Runtime as the default when doing `docker build`. More details can be found
```

### Comparing `colossalai-nightly-2023.5.27/colossalai_nightly.egg-info/SOURCES.txt` & `colossalai-nightly-2023.5.6/colossalai_nightly.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,35 +5,14 @@
 version.txt
 colossalai/__init__.py
 colossalai/constants.py
 colossalai/core.py
 colossalai/global_variables.py
 colossalai/initialize.py
 colossalai/_C/__init__.py
-colossalai/_analyzer/__init__.py
-colossalai/_analyzer/envs.py
-colossalai/_analyzer/_subclasses/__init__.py
-colossalai/_analyzer/_subclasses/_meta_registration.py
-colossalai/_analyzer/_subclasses/_monkey_patch.py
-colossalai/_analyzer/_subclasses/flop_tensor.py
-colossalai/_analyzer/_subclasses/meta_tensor.py
-colossalai/_analyzer/fx/__init__.py
-colossalai/_analyzer/fx/codegen.py
-colossalai/_analyzer/fx/graph_module.py
-colossalai/_analyzer/fx/node_util.py
-colossalai/_analyzer/fx/symbolic_profile.py
-colossalai/_analyzer/fx/passes/__init__.py
-colossalai/_analyzer/fx/passes/graph_profile.py
-colossalai/_analyzer/fx/passes/shape_prop.py
-colossalai/_analyzer/fx/tracer/__init__.py
-colossalai/_analyzer/fx/tracer/bias_addition.py
-colossalai/_analyzer/fx/tracer/custom_leaf_module.py
-colossalai/_analyzer/fx/tracer/proxy.py
-colossalai/_analyzer/fx/tracer/symbolic_trace.py
-colossalai/_analyzer/fx/tracer/tracer.py
 colossalai/amp/__init__.py
 colossalai/amp/amp_type.py
 colossalai/amp/apex_amp/__init__.py
 colossalai/amp/apex_amp/apex_amp.py
 colossalai/amp/naive_amp/__init__.py
 colossalai/amp/naive_amp/_fp16_optimizer.py
 colossalai/amp/naive_amp/_utils.py
@@ -148,25 +127,23 @@
 colossalai/auto_parallel/tensor_shard/utils/sharding.py
 colossalai/booster/__init__.py
 colossalai/booster/accelerator.py
 colossalai/booster/booster.py
 colossalai/booster/mixed_precision/__init__.py
 colossalai/booster/mixed_precision/bf16.py
 colossalai/booster/mixed_precision/fp16_apex.py
-colossalai/booster/mixed_precision/fp16_naive.py
 colossalai/booster/mixed_precision/fp16_torch.py
 colossalai/booster/mixed_precision/fp8.py
 colossalai/booster/mixed_precision/mixed_precision_base.py
 colossalai/booster/plugin/__init__.py
 colossalai/booster/plugin/dp_plugin_base.py
 colossalai/booster/plugin/gemini_plugin.py
 colossalai/booster/plugin/low_level_zero_plugin.py
 colossalai/booster/plugin/plugin_base.py
 colossalai/booster/plugin/torch_ddp_plugin.py
-colossalai/booster/plugin/torch_fsdp_plugin.py
 colossalai/builder/__init__.py
 colossalai/builder/builder.py
 colossalai/checkpoint_io/__init__.py
 colossalai/checkpoint_io/checkpoint_io_base.py
 colossalai/checkpoint_io/general_checkpoint_io.py
 colossalai/checkpoint_io/index_file.py
 colossalai/checkpoint_io/utils.py
```

### Comparing `colossalai-nightly-2023.5.27/op_builder/__init__.py` & `colossalai-nightly-2023.5.6/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/op_builder/builder.py` & `colossalai-nightly-2023.5.6/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/op_builder/cpu_adam.py` & `colossalai-nightly-2023.5.6/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/op_builder/fused_optim.py` & `colossalai-nightly-2023.5.6/op_builder/fused_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/op_builder/layernorm.py` & `colossalai-nightly-2023.5.6/op_builder/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/op_builder/moe.py` & `colossalai-nightly-2023.5.6/op_builder/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/op_builder/multi_head_attn.py` & `colossalai-nightly-2023.5.6/op_builder/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/op_builder/scaled_masked_softmax.py` & `colossalai-nightly-2023.5.6/op_builder/scaled_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/op_builder/scaled_upper_triangle_masked_softmax.py` & `colossalai-nightly-2023.5.6/op_builder/scaled_upper_triangle_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/op_builder/utils.py` & `colossalai-nightly-2023.5.6/op_builder/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     import torch
 
     try:
         torch_cuda_major = torch.version.cuda.split(".")[0]
         torch_cuda_minor = torch.version.cuda.split(".")[1]
     except:
         raise ValueError(
-            "[extension] Cannot retrieve the CUDA version in the PyTorch binary given by torch.version.cuda")
+            "[extension] Cannot retrive the CUDA version in the PyTorch binary given by torch.version.cuda")
     return torch_cuda_major, torch_cuda_minor
 
 
 def get_cuda_bare_metal_version(cuda_dir) -> List[int]:
     """
     Get the System CUDA version from nvcc.
 
@@ -106,15 +106,15 @@
     Returns:
         A tuple of integers in the form of (major, minor, patch).
     """
     import torch
     torch_version = torch.__version__.split('+')[0]
     TORCH_MAJOR = int(torch_version.split('.')[0])
     TORCH_MINOR = int(torch_version.split('.')[1])
-    TORCH_PATCH = int(torch_version.split('.')[2], 16)
+    TORCH_PATCH = int(torch_version.split('.')[2])
     return TORCH_MAJOR, TORCH_MINOR, TORCH_PATCH
 
 
 def check_pytorch_version(min_major_version, min_minor_version) -> bool:
     """
     Compare the current PyTorch version with the minium required version.
```

### Comparing `colossalai-nightly-2023.5.27/setup.py` & `colossalai-nightly-2023.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/components_to_test/albert.py` & `colossalai-nightly-2023.5.6/tests/components_to_test/albert.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,37 +23,37 @@
                               num_attention_heads=num_head,
                               max_position_embeddings=sequence_length,
                               num_hidden_layers=num_layer,
                               hidden_dropout_prob=0.,
                               attention_probs_dropout_prob=0.)
         print('building AlbertForSequenceClassification model')
 
-        # adapting huggingface BertForSequenceClassification for single unittest calling interface
-        class ModelAdaptor(AlbertForSequenceClassification):
+        # adapting huggingface BertForSequenceClassification for single unitest calling interface
+        class ModelAaptor(AlbertForSequenceClassification):
 
             def forward(self, input_ids, labels):
                 """
                 inputs: data, label
                 outputs: loss
                 """
                 return super().forward(input_ids=input_ids, labels=labels)[0]
 
-        model = ModelAdaptor(config)
+        model = ModelAaptor(config)
         # if checkpoint and version.parse(transformers.__version__) >= version.parse("4.11.0"):
         #     model.gradient_checkpointing_enable()
 
         return model
 
-    is_distributed = torch.distributed.is_initialized()
+    is_distrbuted = torch.distributed.is_initialized()
     trainloader = get_bert_data_loader(n_class=vocab_size,
                                        batch_size=2,
                                        total_samples=10000,
                                        sequence_length=sequence_length,
-                                       is_distributed=is_distributed)
+                                       is_distrbuted=is_distrbuted)
     testloader = get_bert_data_loader(n_class=vocab_size,
                                       batch_size=2,
                                       total_samples=10000,
                                       sequence_length=sequence_length,
-                                      is_distributed=is_distributed)
+                                      is_distrbuted=is_distrbuted)
 
     criterion = None
     return bert_model_builder, trainloader, testloader, torch.optim.Adam, criterion
```

### Comparing `colossalai-nightly-2023.5.27/tests/components_to_test/beit.py` & `colossalai-nightly-2023.5.6/tests/components_to_test/beit.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,20 +23,20 @@
                               device=get_current_device())
         return data, label
 
 
 @non_distributed_component_funcs.register(name='beit')
 def get_training_components():
 
-    def model_builder(checkpoint=False):
+    def model_buider(checkpoint=False):
         model = Beit(img_size=DummyDataLoader.img_size,
                      num_classes=DummyDataLoader.num_class,
                      embed_dim=32,
                      depth=2,
                      num_heads=4)
         return model
 
     trainloader = DummyDataLoader()
     testloader = DummyDataLoader()
 
     criterion = torch.nn.CrossEntropyLoss()
-    return model_builder, trainloader, testloader, torch.optim.Adam, criterion
+    return model_buider, trainloader, testloader, torch.optim.Adam, criterion
```

### Comparing `colossalai-nightly-2023.5.27/tests/components_to_test/bert.py` & `colossalai-nightly-2023.5.6/tests/components_to_test/bert.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 
 def get_bert_data_loader(
         n_class,
         batch_size,
         total_samples,
         sequence_length,
         device=torch.device('cpu:0'),
-        is_distributed=False,
+        is_distrbuted=False,
 ):
     train_data = torch.randint(
         low=0,
         high=n_class,
         size=(total_samples, sequence_length),
         device=device,
         dtype=torch.long,
     )
     train_label = torch.randint(low=0, high=2, size=(total_samples,), device=device, dtype=torch.long)
     train_dataset = torch.utils.data.TensorDataset(train_data, train_label)
-    if is_distributed:
+    if is_distrbuted:
         sampler = torch.utils.data.distributed.DistributedSampler(train_dataset)
     else:
         sampler = SequentialSampler(train_dataset)
     train_loader = torch.utils.data.DataLoader(train_dataset, batch_size=batch_size, sampler=sampler)
     return train_loader
 
 
@@ -48,37 +48,37 @@
                             num_attention_heads=num_head,
                             max_position_embeddings=sequence_length,
                             num_hidden_layers=num_layer,
                             hidden_dropout_prob=0.,
                             attention_probs_dropout_prob=0.)
         print('building BertForSequenceClassification model')
 
-        # adapting huggingface BertForSequenceClassification for single unittest calling interface
-        class ModelAdaptor(BertForSequenceClassification):
+        # adapting huggingface BertForSequenceClassification for single unitest calling interface
+        class ModelAaptor(BertForSequenceClassification):
 
             def forward(self, input_ids, labels):
                 """
                 inputs: data, label
                 outputs: loss
                 """
                 return super().forward(input_ids=input_ids, labels=labels)[0]
 
-        model = ModelAdaptor(config)
+        model = ModelAaptor(config)
         if checkpoint and version.parse(transformers.__version__) >= version.parse("4.11.0"):
             model.gradient_checkpointing_enable()
 
         return model
 
-    is_distributed = torch.distributed.is_initialized()
+    is_distrbuted = torch.distributed.is_initialized()
     trainloader = get_bert_data_loader(n_class=vocab_size,
                                        batch_size=2,
                                        total_samples=10000,
                                        sequence_length=sequence_length,
-                                       is_distributed=is_distributed)
+                                       is_distrbuted=is_distrbuted)
     testloader = get_bert_data_loader(n_class=vocab_size,
                                       batch_size=2,
                                       total_samples=10000,
                                       sequence_length=sequence_length,
-                                      is_distributed=is_distributed)
+                                      is_distrbuted=is_distrbuted)
 
     criterion = None
     return bert_model_builder, trainloader, testloader, torch.optim.Adam, criterion
```

### Comparing `colossalai-nightly-2023.5.27/tests/components_to_test/gpt2.py` & `colossalai-nightly-2023.5.6/tests/components_to_test/gpt2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/components_to_test/hanging_param_model.py` & `colossalai-nightly-2023.5.6/tests/components_to_test/hanging_param_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/components_to_test/inline_op_model.py` & `colossalai-nightly-2023.5.6/tests/components_to_test/inline_op_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/components_to_test/nested_model.py` & `colossalai-nightly-2023.5.6/tests/components_to_test/nested_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/components_to_test/registry.py` & `colossalai-nightly-2023.5.6/tests/components_to_test/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
     def __init__(self):
         self._registry = dict()
 
     def register(self, name):
         assert name not in self._registry
 
-        def _register(callable_):
+        def _regsiter(callable_):
             self._registry[name] = callable_
 
-        return _register
+        return _regsiter
 
     def get_callable(self, name: str):
         return self._registry[name]
 
     def __iter__(self):
         self._idx = 0
         self._len = len(self._registry)
@@ -30,10 +30,10 @@
             self._idx += 1
             return callable_
         else:
             raise StopIteration
 
 
 non_distributed_component_funcs = Registry()
-model_parallel_component_funcs = Registry()
+model_paralle_component_funcs = Registry()
 
-__all__ = ['non_distributed_component_funcs', 'model_parallel_component_funcs']
+__all__ = ['non_distributed_component_funcs', 'model_paralle_component_funcs']
```

### Comparing `colossalai-nightly-2023.5.27/tests/components_to_test/repeated_computed_layers.py` & `colossalai-nightly-2023.5.6/tests/components_to_test/repeated_computed_layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/components_to_test/resnet.py` & `colossalai-nightly-2023.5.6/tests/components_to_test/resnet.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/components_to_test/simple_net.py` & `colossalai-nightly-2023.5.6/tests/components_to_test/simple_net.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/components_to_test/utils/executor.py` & `colossalai-nightly-2023.5.6/tests/components_to_test/utils/executor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/kit/model_zoo/diffusers/diffusers.py` & `colossalai-nightly-2023.5.6/tests/kit/model_zoo/diffusers/diffusers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/kit/model_zoo/registry.py` & `colossalai-nightly-2023.5.6/tests/kit/model_zoo/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/kit/model_zoo/timm/timm.py` & `colossalai-nightly-2023.5.6/tests/kit/model_zoo/timm/timm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/kit/model_zoo/torchaudio/torchaudio.py` & `colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchaudio/torchaudio.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/kit/model_zoo/torchrec/torchrec.py` & `colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchrec/torchrec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/kit/model_zoo/torchvision/torchvision.py` & `colossalai-nightly-2023.5.6/tests/kit/model_zoo/torchvision/torchvision.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/kit/model_zoo/transformers/albert.py` & `colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/albert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/kit/model_zoo/transformers/bert.py` & `colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/kit/model_zoo/transformers/gpt.py` & `colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/gpt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/kit/model_zoo/transformers/opt.py` & `colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/opt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/kit/model_zoo/transformers/t5.py` & `colossalai-nightly-2023.5.6/tests/kit/model_zoo/transformers/t5.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_analyzer/test_fx/test_bias_addition.py` & `colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_bias_addition.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_analyzer/test_fx/test_mod_dir.py` & `colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_mod_dir.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_analyzer/test_fx/test_nested_ckpt.py` & `colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_nested_ckpt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_analyzer/test_fx/test_shape_prop.py` & `colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_shape_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_analyzer/test_fx/test_symbolic_profile.py` & `colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/test_symbolic_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_analyzer/test_fx/zoo.py` & `colossalai-nightly-2023.5.6/tests/test_analyzer/test_fx/zoo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_analyzer/test_subclasses/test_aten.py` & `colossalai-nightly-2023.5.6/tests/test_analyzer/test_subclasses/test_aten.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_analyzer/test_subclasses/test_flop_tensor.py` & `colossalai-nightly-2023.5.6/tests/test_analyzer/test_subclasses/test_flop_tensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,16 @@
     }),
     (torch.where, (torch.rand(2, 3, 224, 224) > 0.5, torch.rand(2, 3, 224, 224, requires_grad=True),
                    torch.rand(2, 3, 224, 224, requires_grad=True)), {}),
 ]
 
 
 @pytest.mark.skipif(version.parse(torch.__version__) < version.parse('1.12.0'), reason='torch version < 12')
-@pytest.mark.parametrize('func, args, kwargs', odd_cases)
+@clear_cache_before_run()
+@parameterize('func, args, kwargs', odd_cases)
 def test_flop_count_function(func, args, kwargs):
     rs_fwd, rs_bwd = flop_count(func, *args, **kwargs, verbose=True)
     assert rs_fwd > 0, f'fwd flop count of {func.__name__} is {rs_fwd}'
     assert rs_bwd > 0, f'bwd flop count of {func.__name__} is {rs_bwd}'
 
 
 if __name__ == '__main__':
```

### Comparing `colossalai-nightly-2023.5.27/tests/test_analyzer/test_subclasses/test_meta_mode.py` & `colossalai-nightly-2023.5.6/tests/test_analyzer/test_subclasses/test_meta_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_pass/test_node_converting_pass.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_pass/test_node_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.5.27/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py` & `colossalai-nightly-2023.5.6/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py`

 * *Files identical despite different names*

