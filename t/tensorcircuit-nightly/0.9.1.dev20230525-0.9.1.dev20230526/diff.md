# Comparing `tmp/tensorcircuit-nightly-0.9.1.dev20230525.tar.gz` & `tmp/tensorcircuit-nightly-0.9.1.dev20230526.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcircuit-nightly-0.9.1.dev20230525.tar", last modified: Thu May 25 12:44:26 2023, max compression
+gzip compressed data, was "tensorcircuit-nightly-0.9.1.dev20230526.tar", last modified: Fri May 26 12:39:19 2023, max compression
```

## Comparing `tensorcircuit-nightly-0.9.1.dev20230525.tar` & `tensorcircuit-nightly-0.9.1.dev20230526.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 12:44:26.136425 tensorcircuit-nightly-0.9.1.dev20230525/
--rw-r--r--   0 runner    (1001) docker     (122)    25259 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    21379 2023-05-25 12:44:26.136425 tensorcircuit-nightly-0.9.1.dev20230525/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    18925 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     6311 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/README_cn.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 12:44:26.116424 tensorcircuit-nightly-0.9.1.dev20230525/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 12:44:26.120425 tensorcircuit-nightly-0.9.1.dev20230525/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/docs/source/advance.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/docs/source/cnconf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6440 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/docs/source/contribution.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/docs/source/generate_rst.py
--rw-r--r--   0 runner    (1001) docker     (122)     3326 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10071 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/docs/source/infras.rst
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/docs/source/modules.rst.backup
--rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/docs/source/sharpbits.rst
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/docs/source/textbooktoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/docs/source/tutorial_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/docs/source/whitepapertoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/docs/source/whitepapertoc_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 12:44:26.136425 tensorcircuit-nightly-0.9.1.dev20230525/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-25 12:44:18.000000 tensorcircuit-nightly-0.9.1.dev20230525/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 12:44:26.124425 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-25 12:44:18.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/about.py
--rw-r--r--   0 runner    (1001) docker     (122)    43418 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/abstractcircuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 12:44:26.124425 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/applications/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/applications/dqas.py
--rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/applications/graphdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/applications/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/applications/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/applications/vags.py
--rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/applications/van.py
--rw-r--r--   0 runner    (1001) docker     (122)    23416 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/applications/vqes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/asciiart.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 12:44:26.128425 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/abstract_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/cupy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/jax_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/jax_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/pytorch_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    35980 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/tf_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/basecircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 12:44:26.128425 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cloud/abstraction.py
--rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cloud/apis.py
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cloud/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cloud/quafu_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)    14228 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cloud/tencent.py
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10737 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cloud/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 12:44:26.128425 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/compiler/composed_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     6032 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/compiler/qiskit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/compiler/simple_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cons.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/densitymatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/gates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 12:44:26.128425 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      545 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/interfaces/numpy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/interfaces/scipy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/interfaces/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/interfaces/tensortrans.py
--rw-r--r--   0 runner    (1001) docker     (122)     5117 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/interfaces/torch.py
--rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/keras.py
--rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/mps_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/quantum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 12:44:26.128425 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/results/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3435 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/results/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/results/readout_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/simplify.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 12:44:26.128425 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/templates/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/templates/chems.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/templates/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/templates/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/templates/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/templates/measurements.py
--rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 12:44:26.132425 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    21379 2023-05-25 12:44:25.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-05-25 12:44:25.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 12:44:25.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-25 12:44:25.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-25 12:44:25.000000 tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 12:44:26.132425 tensorcircuit-nightly-0.9.1.dev20230525/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    33735 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_calibrating.py
--rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    47713 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_dmcircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_miscs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_qaoa.py
--rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_quantum_attr.py
--rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-05-25 12:16:53.000000 tensorcircuit-nightly-0.9.1.dev20230525/tests/test_van.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.821004 tensorcircuit-nightly-0.9.1.dev20230526/
+-rw-r--r--   0 runner    (1001) docker     (122)    25259 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    21432 2023-05-26 12:39:19.821004 tensorcircuit-nightly-0.9.1.dev20230526/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    18978 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6448 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/README_cn.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.797004 tensorcircuit-nightly-0.9.1.dev20230526/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.801004 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/advance.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/cnconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6440 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/generate_rst.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3326 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10071 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/infras.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/modules.rst.backup
+-rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/sharpbits.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/textbooktoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/tutorial_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/whitepapertoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/docs/source/whitepapertoc_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-26 12:39:19.821004 tensorcircuit-nightly-0.9.1.dev20230526/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-26 12:39:13.000000 tensorcircuit-nightly-0.9.1.dev20230526/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.809004 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-26 12:39:13.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/about.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43418 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/abstractcircuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.809004 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/dqas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/graphdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/vags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/van.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23416 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/vqes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/asciiart.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.809004 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/abstract_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/cupy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/jax_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/jax_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/pytorch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35980 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/tf_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/basecircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.813004 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/abstraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/apis.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2613 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/quafu_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14228 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/tencent.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10766 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.813004 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/compiler/composed_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6032 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/compiler/qiskit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/compiler/simple_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/densitymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/gates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.813004 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/tensortrans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5117 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/mps_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/quantum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.817004 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/results/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3435 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/results/counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/results/readout_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/simplify.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.817004 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/chems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.817004 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    21432 2023-05-26 12:39:19.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-05-26 12:39:19.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-26 12:39:19.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-26 12:39:19.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-26 12:39:19.000000 tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 12:39:19.817004 tensorcircuit-nightly-0.9.1.dev20230526/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33735 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_calibrating.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47713 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_dmcircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_miscs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_quantum_attr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-05-26 12:16:10.000000 tensorcircuit-nightly-0.9.1.dev20230526/tests/test_van.py
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/CHANGELOG.md` & `tensorcircuit-nightly-0.9.1.dev20230526/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/HISTORY.md` & `tensorcircuit-nightly-0.9.1.dev20230526/HISTORY.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/LICENSE` & `tensorcircuit-nightly-0.9.1.dev20230526/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/PKG-INFO` & `tensorcircuit-nightly-0.9.1.dev20230526/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.1.dev20230525
+Version: 0.9.1.dev20230526
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
@@ -35,15 +35,15 @@
           </a>
         </p>
         
         <p align="center"> English | <a href="README_cn.md"> 简体中文 </a></p>
         
         TensorCircuit is the next generation of quantum software framework with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
         
-        TensorCircuit is built on top of modern machine learning frameworks and is machine learning backend agnostic. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms. It also supports real quantum hardware access and provides CPU/GPU/QPU hybrid deployment solutions since v0.9.
+        TensorCircuit is built on top of modern machine learning frameworks: Jax, TensorFlow, and PyTorch. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms in ideal, noisy and approximation cases. It also supports real quantum hardware access and provides CPU/GPU/QPU hybrid deployment solutions since v0.9.
         
         ## Getting Started
         
         Please begin with [Quick Start](/docs/source/quickstart.rst).
         
         For more information and introductions, please refer to helpful [example scripts](/examples) and [full documentation](https://tensorcircuit.readthedocs.io/). API docstrings and test cases in [tests](/tests) are also informative.
         
@@ -121,15 +121,15 @@
         
           - Time: 10 to 10^6+ times acceleration compared to TensorFlow Quantum, Pennylane or Qiskit
         
           - Space: 600+ qubits 1D VQE workflow (converged energy inaccuracy: < 1%)
         
         - Elegance
         
-          - Flexibility: customized contraction, multiple ML backend/interface choices, multiple dtype precisions
+          - Flexibility: customized contraction, multiple ML backend/interface choices, multiple dtype precisions, multiple QPU providers
         
           - API design: quantum for humans, less code, more power
         
         ## Contributing
         
         ### Status
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/README.md` & `tensorcircuit-nightly-0.9.1.dev20230526/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   </a>
 </p>
 
 <p align="center"> English | <a href="README_cn.md"> 简体中文 </a></p>
 
 TensorCircuit is the next generation of quantum software framework with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
 
-TensorCircuit is built on top of modern machine learning frameworks and is machine learning backend agnostic. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms. It also supports real quantum hardware access and provides CPU/GPU/QPU hybrid deployment solutions since v0.9.
+TensorCircuit is built on top of modern machine learning frameworks: Jax, TensorFlow, and PyTorch. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms in ideal, noisy and approximation cases. It also supports real quantum hardware access and provides CPU/GPU/QPU hybrid deployment solutions since v0.9.
 
 ## Getting Started
 
 Please begin with [Quick Start](/docs/source/quickstart.rst).
 
 For more information and introductions, please refer to helpful [example scripts](/examples) and [full documentation](https://tensorcircuit.readthedocs.io/). API docstrings and test cases in [tests](/tests) are also informative.
 
@@ -113,15 +113,15 @@
 
   - Time: 10 to 10^6+ times acceleration compared to TensorFlow Quantum, Pennylane or Qiskit
 
   - Space: 600+ qubits 1D VQE workflow (converged energy inaccuracy: < 1%)
 
 - Elegance
 
-  - Flexibility: customized contraction, multiple ML backend/interface choices, multiple dtype precisions
+  - Flexibility: customized contraction, multiple ML backend/interface choices, multiple dtype precisions, multiple QPU providers
 
   - API design: quantum for humans, less code, more power
 
 ## Contributing
 
 ### Status
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/README_cn.md` & `tensorcircuit-nightly-0.9.1.dev20230526/README_cn.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,19 +21,19 @@
   <a href="./LICENSE">
     <img src="https://img.shields.io/badge/license-Apache%202.0-blue.svg?logo=apache"/>
   </a>
 </p>
 
 <p align="center"> <a href="README.md">English</a> |  简体中文 </p>
 
-TensorCircuit 是下一代量子软件框架，支持自动微分、即时编译、硬件加速和向量并行化。
+TensorCircuit 是下一代量子软件框架，完美支持自动微分、即时编译、硬件加速和向量并行化。
 
-TensorCircuit 建立在现代机器学习框架之上，并且与机器学习后端无关。 它特别适用于量子经典混合范式和变分量子算法的高效模拟。
+TensorCircuit 建立在现代机器学习框架 Jax, TensorFlow, PyTorch 之上，支持机器学习后端无关的统一界面。 其特别适用于理想情况、含噪声情况及可控近似情况下，大规模量子经典混合范式和变分量子算法的高效模拟。
 
-TensorCircuit 现在支持真实量子硬件连接和实验，并提供优雅的 CPU/GPU/QPU 混合部署方案（v0.9+）。
+TensorCircuit 现在支持真实量子硬件连接和实验，并提供优雅的 CPU/GPU/QPU 混合部署训练方案（v0.9+）。
 
 ## 入门
 
 请从 [快速上手](/docs/source/quickstart.rst) 和 [Jupyter 教程](/docs/source/tutorials) 开始。
 
 有关更多信息和介绍，请参阅有用的 [示例脚本](/examples) 和 [完整文档](https://tensorcircuit.readthedocs.io/zh/latest/)。 [测试](/tests)用例和 API docstring 也提供了丰富的使用信息。
 
@@ -48,15 +48,15 @@
 c.CNOT(0,1)
 c.rx(1, theta=0.2)
 print(c.wavefunction())
 print(c.expectation_ps(z=[0, 1]))
 print(c.sample(allow_state=True, batch=1024, format="count_dict_bin"))
 ```
 
-- 运行时特性定制:
+- 运行时特性设置:
 
 ```python
 tc.set_backend("tensorflow")
 tc.set_dtype("complex128")
 tc.set_contractor("greedy")
 ```
 
@@ -111,15 +111,15 @@
 
   - 时间：与 TFQ, Pennylane, 或 Qiskit 相比，加速 10 到 10^6+ 倍
 
   - 空间：600+ qubits 1D VQE 工作流（收敛能量误差：< 1%）
 
 - 优雅
 
-  - 灵活性：自定义张量收缩、多种 ML 后端/接口选择、多种数值精度
+  - 灵活性：自定义张量收缩、多种 ML 后端/接口选择、多种数值精度、多种量子硬件
 
   - API 设计：人类可理解的量子，更少的代码，更多的可能
 
 ## 贡献
 
 ### 现况
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/docs/source/advance.rst` & `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/advance.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/docs/source/cnconf.py` & `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/cnconf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/docs/source/conf.py` & `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/docs/source/contribution.rst` & `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/docs/source/faq.rst` & `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/docs/source/generate_rst.py` & `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/generate_rst.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/docs/source/index.rst` & `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/docs/source/infras.rst` & `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/infras.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/docs/source/modules.rst` & `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/docs/source/modules.rst.backup` & `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/modules.rst.backup`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/docs/source/quickstart.rst` & `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/docs/source/sharpbits.rst` & `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/sharpbits.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/docs/source/tutorial.rst` & `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/docs/source/tutorial_cn.rst` & `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/tutorial_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/docs/source/whitepapertoc_cn.rst` & `tensorcircuit-nightly-0.9.1.dev20230526/docs/source/whitepapertoc_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/setup.py` & `tensorcircuit-nightly-0.9.1.dev20230526/setup.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/__init__.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.1.dev20230525"
+__version__ = "0.9.1.dev20230526"
 __author__ = "TensorCircuit Authors"
 __creator__ = "refraction-ray"
 
 from .utils import gpu_memory_share
 
 gpu_memory_share()
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/about.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/about.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/abstractcircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/abstractcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/applications/dqas.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/dqas.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/applications/graphdata.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/graphdata.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/applications/layers.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/layers.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/applications/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/applications/vags.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/vags.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/applications/van.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/van.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/applications/vqes.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/applications/vqes.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/asciiart.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/asciiart.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/abstract_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/backend_factory.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/backend_factory.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/cupy_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/cupy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/jax_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/jax_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/jax_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/jax_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/numpy_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/pytorch_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/pytorch_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/tensorflow_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/backends/tf_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/backends/tf_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/basecircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/basecircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/channels.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/circuit.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cloud/abstraction.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/abstraction.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cloud/apis.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/apis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cloud/local.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/local.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cloud/quafu_provider.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/quafu_provider.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import logging
 
 from quafu import User, QuantumCircuit
 from quafu import Task as Task_
 
 from .abstraction import Device, sep, Task
 from ..abstractcircuit import AbstractCircuit
+from ..utils import is_sequence
 
 logger = logging.getLogger(__name__)
 
 
 def list_devices(token: Optional[str] = None, **kws: Any) -> List[Device]:
     raise NotImplementedError
 
@@ -39,26 +40,36 @@
             if isinstance(c, QuantumCircuit):
                 s = c.qasm()
                 # nq = c.num_qubits
             else:
                 s = c.to_openqasm()
             return s  # type: ignore
 
-        source = c2qasm(circuit)
+        if not is_sequence(circuit):
+            source = c2qasm(circuit)
+        else:
+            source = [c2qasm(c) for c in circuit]  # type: ignore
     user = User()
     user.save_apitoken(token)
-    nq = int(source.split("\n")[2].split("[")[1].split("]")[0])  # type: ignore
-    qc = QuantumCircuit(nq)
-    qc.from_openqasm(source)
-    task = Task_()
-    device_name = device.name.split(sep)[-1]
-    task.config(backend=device_name, shots=shots, compile=compile)
-    res = task.send(qc, wait=False)
-    wrapper = Task(res.taskid, device=device)
-    return wrapper
+
+    def c2task(source: str) -> Task:
+        nq = int(source.split("\n")[2].split("[")[1].split("]")[0])  # type: ignore
+        qc = QuantumCircuit(nq)
+        qc.from_openqasm(source)
+        task = Task_()
+        device_name = device.name.split(sep)[-1]
+        task.config(backend=device_name, shots=shots, compile=compile)
+        res = task.send(qc, wait=False)
+        wrapper = Task(res.taskid, device=device)
+        return wrapper
+
+    if not is_sequence(source):
+        return c2task(source)  # type: ignore
+    else:
+        return [c2task(s) for s in source]  # type: ignore
 
 
 def resubmit_task(task: Task, token: str) -> Task:
     raise NotImplementedError
 
 
 def remove_task(task: Task, token: str) -> Any:
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cloud/tencent.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/tencent.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cloud/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cloud/wrapper.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cloud/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,16 @@
     if device is None:
         results = []
         for ps in pss:
             results.append(c.expectation_ps(**ps2xyz(ps)))  # type: ignore
         if ws is None:
             return backend.real(backend.stack(results))
         else:
-            return backend.real(backend.sum([w * r for w, r in zip(ws, results)]))
+            sumr = sum([w * r for w, r in zip(ws, results)])
+            return backend.convert_to_tensor(sumr)
     cs = []
     infos = []
     exps = []
     if isinstance(device, str):
         device = get_device(device)
 
     dc = DefaultCompiler(
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/compiler/composed_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/compiler/composed_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/compiler/qiskit_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/compiler/qiskit_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/compiler/simple_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/compiler/simple_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/cons.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/cons.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/densitymatrix.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/experimental.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/experimental.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/gates.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/interfaces/__init__.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/interfaces/numpy.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/numpy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/interfaces/scipy.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/scipy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/interfaces/tensorflow.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/interfaces/tensortrans.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/tensortrans.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/interfaces/torch.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/interfaces/torch.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/keras.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/mps_base.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/mps_base.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/mpscircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/noisemodel.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/quantum.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/results/counts.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/results/counts.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/results/readout_mitigation.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/results/readout_mitigation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/simplify.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/templates/blocks.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/blocks.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/templates/chems.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/chems.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/templates/dataset.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/templates/ensemble.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/templates/graphs.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/graphs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/templates/measurements.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/templates/measurements.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/torchnn.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/translation.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/translation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit/vis.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit/vis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit_nightly.egg-info/PKG-INFO` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.1.dev20230525
+Version: 0.9.1.dev20230526
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
@@ -35,15 +35,15 @@
           </a>
         </p>
         
         <p align="center"> English | <a href="README_cn.md"> 简体中文 </a></p>
         
         TensorCircuit is the next generation of quantum software framework with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
         
-        TensorCircuit is built on top of modern machine learning frameworks and is machine learning backend agnostic. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms. It also supports real quantum hardware access and provides CPU/GPU/QPU hybrid deployment solutions since v0.9.
+        TensorCircuit is built on top of modern machine learning frameworks: Jax, TensorFlow, and PyTorch. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms in ideal, noisy and approximation cases. It also supports real quantum hardware access and provides CPU/GPU/QPU hybrid deployment solutions since v0.9.
         
         ## Getting Started
         
         Please begin with [Quick Start](/docs/source/quickstart.rst).
         
         For more information and introductions, please refer to helpful [example scripts](/examples) and [full documentation](https://tensorcircuit.readthedocs.io/). API docstrings and test cases in [tests](/tests) are also informative.
         
@@ -121,15 +121,15 @@
         
           - Time: 10 to 10^6+ times acceleration compared to TensorFlow Quantum, Pennylane or Qiskit
         
           - Space: 600+ qubits 1D VQE workflow (converged energy inaccuracy: < 1%)
         
         - Elegance
         
-          - Flexibility: customized contraction, multiple ML backend/interface choices, multiple dtype precisions
+          - Flexibility: customized contraction, multiple ML backend/interface choices, multiple dtype precisions, multiple QPU providers
         
           - API design: quantum for humans, less code, more power
         
         ## Contributing
         
         ### Status
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tensorcircuit_nightly.egg-info/SOURCES.txt` & `tensorcircuit-nightly-0.9.1.dev20230526/tensorcircuit_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/conftest.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_backends.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_calibrating.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_calibrating.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_channels.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_circuit.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_cloud.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_dmcircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_dmcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_ensemble.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_gates.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_interfaces.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_keras.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_miscs.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_miscs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_mpscircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_noisemodel.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_qaoa.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_quantum.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_quantum_attr.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_quantum_attr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_results.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_simplify.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_templates.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_torchnn.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230525/tests/test_van.py` & `tensorcircuit-nightly-0.9.1.dev20230526/tests/test_van.py`

 * *Files identical despite different names*

