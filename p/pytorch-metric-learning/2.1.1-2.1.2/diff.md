# Comparing `tmp/pytorch-metric-learning-2.1.1.tar.gz` & `tmp/pytorch-metric-learning-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-metric-learning-2.1.1.tar", last modified: Wed May  3 11:53:00 2023, max compression
+gzip compressed data, was "pytorch-metric-learning-2.1.2.tar", last modified: Sat May 27 21:20:23 2023, max compression
```

## Comparing `pytorch-metric-learning-2.1.1.tar` & `pytorch-metric-learning-2.1.2.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:53:00.114436 pytorch-metric-learning-2.1.1/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1090 2019-10-24 20:18:14.000000 pytorch-metric-learning-2.1.1/LICENSE
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    16202 2023-05-03 11:53:00.114436 pytorch-metric-learning-2.1.1/PKG-INFO
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15547 2023-04-05 22:59:33.000000 pytorch-metric-learning-2.1.1/README.md
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)       38 2023-05-03 11:53:00.114436 pytorch-metric-learning-2.1.1/setup.cfg
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1507 2023-01-29 03:05:20.000000 pytorch-metric-learning-2.1.1/setup.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:52:59.926434 pytorch-metric-learning-2.1.1/src/
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:52:59.946434 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)       22 2023-05-03 11:30:04.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/__init__.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:52:59.966434 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      265 2023-01-29 03:05:20.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3508 2023-05-03 11:30:19.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/base_distance.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      755 2023-01-29 03:05:20.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/batched_distance.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      274 2021-02-11 13:46:54.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/cosine_similarity.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      424 2021-02-11 13:46:54.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/dot_product_similarity.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1042 2021-02-11 13:46:55.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/lp_distance.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      714 2021-02-11 13:46:55.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/snr_distance.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:53:00.022435 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1617 2023-04-05 22:50:01.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/__init__.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3061 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/angular_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1386 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/arcface_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      391 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/base_loss_wrapper.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2456 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/base_metric_loss_function.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2832 2021-02-11 13:46:55.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/circle_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2005 2021-02-11 13:46:56.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/contrastive_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      939 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/cosface_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     5333 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/cross_batch_memory.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2833 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/fast_ap_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1492 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/generic_pair_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1689 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/instance_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2047 2021-02-11 13:46:56.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/intra_pair_variance_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     5674 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/large_margin_softmax_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3034 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/lifted_structure_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3288 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/margin_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2863 2021-02-11 13:46:57.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/mixins.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1558 2021-02-11 13:46:57.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/multi_similarity_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2351 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/multiple_losses.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1463 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/n_pairs_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1957 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/nca_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2173 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/normalized_softmax_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1778 2021-05-08 22:57:02.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/ntxent_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3506 2023-04-05 22:50:12.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/pnp_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3469 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/proxy_anchor_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1376 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/proxy_losses.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2021 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/self_supervised_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      373 2021-02-11 13:46:56.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/signal_to_noise_ratio_losses.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3230 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/soft_triple_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      360 2021-02-11 13:46:57.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/sphereface_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2600 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/subcenter_arcface_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1715 2021-05-08 22:57:02.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/supcon_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2290 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/triplet_margin_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2049 2022-06-29 19:51:55.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/tuplet_margin_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3374 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/vicreg_loss.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:53:00.038435 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      569 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2874 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/angular_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2201 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/base_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     8131 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/batch_easy_hard_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      404 2021-02-11 13:46:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/batch_hard_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2066 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/distance_weighted_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      493 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/embeddings_already_packaged_as_triplets.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2192 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/hdc_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2315 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/multi_similarity_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1742 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/pair_margin_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2403 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/triplet_margin_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2303 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/uniform_histogram_miner.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:53:00.058436 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      459 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      169 2021-02-11 13:46:59.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/avg_non_zero_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3816 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/base_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1130 2021-02-11 14:13:23.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/class_weighted_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1551 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/divisor_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      156 2021-02-11 13:47:00.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/do_nothing_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      473 2021-02-11 13:47:00.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/mean_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1214 2021-02-11 14:13:01.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/multiple_reducers.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2149 2021-05-08 22:57:04.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/per_anchor_reducer.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      182 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/sum_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2211 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/threshold_reducer.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:53:00.066436 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      338 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      499 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/base_regularizer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      871 2022-03-01 01:50:13.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/center_invariant_regularizer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      723 2022-03-01 01:50:13.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/lp_regularizer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1229 2021-02-11 14:20:16.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/regular_face_regularizer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2697 2021-05-08 22:57:05.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/sparse_centers_regularizer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      432 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/zero_mean_regularizer.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:53:00.074436 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      220 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2132 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/fixed_set_of_triplets.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3856 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/hierarchical_sampler.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2555 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/m_per_class_sampler.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1696 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/tuples_to_weights_sampler.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:53:00.082436 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      243 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    12495 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/base_tester.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1371 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/global_embedding_space.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2820 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/global_twostream_embedding_space.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2791 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/with_same_parent_label.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:53:00.094436 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      321 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    11599 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/base_trainer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3002 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/cascaded_embeddings.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     6807 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/deep_adversarial_metric_learning.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      625 2021-02-11 13:47:02.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/metric_loss_only.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1224 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/train_with_classifier.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2295 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/twostream_metric_loss.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:53:00.114436 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2020-05-18 23:01:59.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    18488 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/accuracy_calculator.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15447 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/common_functions.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     6399 2023-01-29 22:17:17.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/distributed.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    11776 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/inference.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1801 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/key_checker.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15836 2023-02-21 17:27:25.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/logging_presets.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     9444 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/loss_and_miner_utils.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1078 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/loss_tracker.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      661 2022-03-01 01:50:13.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/module_with_records.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1624 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/module_with_records_and_reducer.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:52:59.954434 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning.egg-info/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    16202 2023-05-03 11:52:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning.egg-info/PKG-INFO
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     5985 2023-05-03 11:52:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning.egg-info/SOURCES.txt
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)        1 2023-05-03 11:52:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning.egg-info/dependency_links.txt
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      226 2023-05-03 11:52:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning.egg-info/requires.txt
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)       24 2023-05-03 11:52:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning.egg-info/top_level.txt
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.880570 pytorch-metric-learning-2.1.2/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1090 2019-10-24 20:18:14.000000 pytorch-metric-learning-2.1.2/LICENSE
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15724 2023-05-27 21:20:23.880570 pytorch-metric-learning-2.1.2/PKG-INFO
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15069 2023-05-26 16:32:49.000000 pytorch-metric-learning-2.1.2/README.md
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)       38 2023-05-27 21:20:23.880570 pytorch-metric-learning-2.1.2/setup.cfg
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1507 2023-01-29 03:05:20.000000 pytorch-metric-learning-2.1.2/setup.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.352563 pytorch-metric-learning-2.1.2/src/
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.376563 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)       23 2023-05-26 17:54:49.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/__init__.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.424564 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      265 2023-01-29 03:05:20.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/__init__.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3508 2023-05-03 11:30:19.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/base_distance.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      755 2023-01-29 03:05:20.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/batched_distance.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      274 2021-02-11 13:46:54.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/cosine_similarity.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      424 2021-02-11 13:46:54.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/dot_product_similarity.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1042 2021-02-11 13:46:55.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/lp_distance.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      714 2021-02-11 13:46:55.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/snr_distance.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.576566 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1617 2023-04-05 22:50:01.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/__init__.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3061 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/angular_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1386 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/arcface_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      391 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/base_loss_wrapper.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2456 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/base_metric_loss_function.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2832 2021-02-11 13:46:55.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/circle_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2005 2021-02-11 13:46:56.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/contrastive_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      939 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/cosface_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     5333 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/cross_batch_memory.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2833 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/fast_ap_loss.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1492 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/generic_pair_loss.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1689 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/instance_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2047 2021-02-11 13:46:56.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/intra_pair_variance_loss.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     5674 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/large_margin_softmax_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3034 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/lifted_structure_loss.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3288 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/margin_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2863 2021-02-11 13:46:57.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/mixins.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1558 2021-02-11 13:46:57.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/multi_similarity_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2351 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/multiple_losses.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1463 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/n_pairs_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1957 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/nca_loss.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2173 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/normalized_softmax_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1778 2021-05-08 22:57:02.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/ntxent_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3506 2023-04-05 22:50:12.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/pnp_loss.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3469 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/proxy_anchor_loss.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1376 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/proxy_losses.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2021 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/self_supervised_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      373 2021-02-11 13:46:56.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/signal_to_noise_ratio_losses.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3230 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/soft_triple_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      360 2021-02-11 13:46:57.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/sphereface_loss.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2600 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/subcenter_arcface_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1715 2021-05-08 22:57:02.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/supcon_loss.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2290 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/triplet_margin_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2049 2022-06-29 19:51:55.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/tuplet_margin_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3374 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/vicreg_loss.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.640566 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      569 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/__init__.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2874 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/angular_miner.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2201 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/base_miner.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     8131 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/batch_easy_hard_miner.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      404 2021-02-11 13:46:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/batch_hard_miner.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2066 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/distance_weighted_miner.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      493 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/embeddings_already_packaged_as_triplets.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2192 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/hdc_miner.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2315 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/multi_similarity_miner.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1742 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/pair_margin_miner.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2461 2023-05-26 16:17:34.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/triplet_margin_miner.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2303 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/uniform_histogram_miner.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.692567 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      459 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/__init__.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      169 2021-02-11 13:46:59.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/avg_non_zero_reducer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3816 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/base_reducer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1130 2021-02-11 14:13:23.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/class_weighted_reducer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1551 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/divisor_reducer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      156 2021-02-11 13:47:00.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/do_nothing_reducer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      473 2021-02-11 13:47:00.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/mean_reducer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1214 2021-02-11 14:13:01.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/multiple_reducers.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2149 2021-05-08 22:57:04.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/per_anchor_reducer.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      182 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/sum_reducer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2211 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/threshold_reducer.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.716567 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      338 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/__init__.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      499 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/base_regularizer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      871 2022-03-01 01:50:13.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/center_invariant_regularizer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      723 2022-03-01 01:50:13.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/lp_regularizer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1229 2021-02-11 14:20:16.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/regular_face_regularizer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2697 2021-05-08 22:57:05.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/sparse_centers_regularizer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      432 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/zero_mean_regularizer.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.744568 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      220 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/__init__.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2132 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/fixed_set_of_triplets.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3846 2023-05-26 17:52:27.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/hierarchical_sampler.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2555 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/m_per_class_sampler.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1696 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/tuples_to_weights_sampler.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.772568 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      243 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/__init__.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    12495 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/base_tester.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1371 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/global_embedding_space.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2820 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/global_twostream_embedding_space.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2791 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/with_same_parent_label.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.796568 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      321 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/__init__.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    11599 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/base_trainer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3002 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/cascaded_embeddings.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     6807 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/deep_adversarial_metric_learning.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      625 2021-02-11 13:47:02.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/metric_loss_only.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1224 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/train_with_classifier.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2295 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/twostream_metric_loss.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.880570 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2020-05-18 23:01:59.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/__init__.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    18488 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/accuracy_calculator.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15447 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/common_functions.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     6399 2023-01-29 22:17:17.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/distributed.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    11776 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/inference.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1801 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/key_checker.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15836 2023-02-21 17:27:25.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/logging_presets.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     9444 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/loss_and_miner_utils.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1078 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/loss_tracker.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      661 2022-03-01 01:50:13.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/module_with_records.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1624 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/module_with_records_and_reducer.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.384563 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning.egg-info/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15724 2023-05-27 21:20:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning.egg-info/PKG-INFO
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     5985 2023-05-27 21:20:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning.egg-info/SOURCES.txt
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)        1 2023-05-27 21:20:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning.egg-info/dependency_links.txt
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      226 2023-05-27 21:20:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning.egg-info/requires.txt
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)       24 2023-05-27 21:20:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning.egg-info/top_level.txt
```

### Comparing `pytorch-metric-learning-2.1.1/LICENSE` & `pytorch-metric-learning-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/PKG-INFO` & `pytorch-metric-learning-2.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-metric-learning
-Version: 2.1.1
+Version: 2.1.2
 Summary: The easiest way to use deep metric learning in your application. Modular, flexible, and extensible. Written in PyTorch.
 Home-page: https://github.com/KevinMusgrave/pytorch-metric-learning
 Author: Kevin Musgrave
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -33,21 +33,22 @@
  <a href="https://anaconda.org/conda-forge/pytorch-metric-learning">
      <img alt="Anaconda version" src="https://img.shields.io/conda/v/conda-forge/pytorch-metric-learning?color=bright-green">
  </a>
 </p>
 
 ## News
 
-**January 16**: v1.7.0
-- Fixes an edge case in ArcFaceLoss. See the [release notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/v1.7.0).
-- Thanks to contributor [ElisonSherton](https://github.com/ElisonSherton).
-
-**September 3**: v1.6.0
-- `DistributedLossWrapper` and `DistributedMinerWrapper` now support `ref_emb` and `ref_labels`.
-- Thanks to contributor [NoTody](https://github.com/NoTody).
+**April 5**: v2.1.0
+- Added [PNPLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#pnploss)
+- Thanks to contributor [interestingzhuo](https://github.com/interestingzhuo).
+
+**January 29**: v2.0.0
+- Added SelfSupervisedLoss, plus various API improvements. See the [release notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/v2.0.0).
+- Thanks to contributor [cwkeam](https://github.com/cwkeam).
+
 
 ## Documentation
 - [**View the documentation here**](https://kevinmusgrave.github.io/pytorch-metric-learning/)
 - [**View the installation instructions here**](https://github.com/KevinMusgrave/pytorch-metric-learning#installation)
 - [**View the available losses, miners etc. here**](https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/CONTENTS.md) 
 
 
@@ -121,30 +122,26 @@
 
  - The loss will be computed using cosine similarity instead of Euclidean distance.
  - All triplet losses that are higher than 0.3 will be discarded.
  - The embeddings will be L2 regularized.  
 
 ### Using loss functions for unsupervised / self-supervised learning
 
-The TripletMarginLoss is an embedding-based or tuple-based loss. This means that internally, there is no real notion of "classes". Tuples (pairs or triplets) are formed at each iteration, based on the labels it receives. The labels don't have to represent classes. They simply need to indicate the positive and negative relationships between the embeddings. Thus, it is easy to use these loss functions for unsupervised or self-supervised learning. 
-
-For example, the code below is a simplified version of the augmentation strategy commonly used in self-supervision. The dataset does not come with any labels. Instead, the labels are created in the training loop, solely to indicate which embeddings are positive pairs.
+A `SelfSupervisedLoss` wrapper is provided for self-supervised learning:
 
 ```python
+from pytorch_metric_learning.losses import SelfSupervisedLoss
+loss_func = SelfSupervisedLoss(TripletMarginLoss())
+
 # your training for-loop
 for i, data in enumerate(dataloader):
 	optimizer.zero_grad()
 	embeddings = your_model(data)
 	augmented = your_model(your_augmentation(data))
-	labels = torch.arange(embeddings.size(0))
-
-	embeddings = torch.cat([embeddings, augmented], dim=0)
-	labels = torch.cat([labels, labels], dim=0)
-
-	loss = loss_func(embeddings, labels)
+	loss = loss_func(embeddings, augmented)
 	loss.backward()
 	optimizer.step()
 ```
 
 If you're interested in [MoCo](https://arxiv.org/pdf/1911.05722.pdf)-style self-supervision, take a look at the [MoCo on CIFAR10](https://github.com/KevinMusgrave/pytorch-metric-learning/tree/master/examples#simple-examples) notebook. It uses CrossBatchMemory to implement the momentum encoder queue, which means you can use any tuple loss, and any tuple miner to extract hard samples from the queue.
 
 
@@ -244,21 +241,21 @@
 
 ### Contributors
 Thanks to the contributors who made pull requests!
 
 | Contributor | Highlights |
 | -- | -- |
 |[mlopezantequera](https://github.com/mlopezantequera) | - Made the [testers](https://kevinmusgrave.github.io/pytorch-metric-learning/testers) work on any combination of query and reference sets <br/> - Made [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) work with arbitrary label comparisons |
-|[cwkeam](https://github.com/cwkeam) | - [VICRegLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#vicregloss) <br/> - Added mean reciprocal rank accuracy to [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) |
+|[cwkeam](https://github.com/cwkeam) | - [SelfSupervisedLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#selfsupervisedloss) <br/> - [VICRegLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#vicregloss) <br/> - Added mean reciprocal rank accuracy to [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) <br/> - BaseLossWrapper|
 |[marijnl](https://github.com/marijnl)| - [BatchEasyHardMiner](https://kevinmusgrave.github.io/pytorch-metric-learning/miners/#batcheasyhardminer) <br/> - [TwoStreamMetricLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/trainers/#twostreammetricloss) <br/> - [GlobalTwoStreamEmbeddingSpaceTester](https://kevinmusgrave.github.io/pytorch-metric-learning/testers/#globaltwostreamembeddingspacetester) <br/> - [Example using trainers.TwoStreamMetricLoss](https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/examples/notebooks/TwoStreamMetricLoss.ipynb) |
 | [chingisooinar](https://github.com/chingisooinar) | [SubCenterArcFaceLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#subcenterarcfaceloss) |
 | [elias-ramzi](https://github.com/elias-ramzi) | [HierarchicalSampler](https://kevinmusgrave.github.io/pytorch-metric-learning/samplers/#hierarchicalsampler) |
 | [fjsj](https://github.com/fjsj) | [SupConLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#supconloss) |
 | [AlenUbuntu](https://github.com/AlenUbuntu) | [CircleLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#circleloss) |
-| [interestingzhuo](https://github.com/interestingzhuo) | [**PNPLoss**](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#pnploss) |
+| [interestingzhuo](https://github.com/interestingzhuo) | [PNPLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#pnploss) |
 | [wconnell](https://github.com/wconnell) | [Learning a scRNAseq Metric Embedding](https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/examples/notebooks/scRNAseq_MetricEmbedding.ipynb) |
 | [AlexSchuy](https://github.com/AlexSchuy) | optimized ```utils.loss_and_miner_utils.get_random_triplet_indices``` |
 | [JohnGiorgi](https://github.com/JohnGiorgi) | ```all_gather``` in [utils.distributed](https://kevinmusgrave.github.io/pytorch-metric-learning/distributed) |
 | [Hummer12007](https://github.com/Hummer12007) | ```utils.key_checker``` |
 | [vltanh](https://github.com/vltanh) | Made ```InferenceModel.train_indexer``` accept datasets |
 | [btseytlin](https://github.com/btseytlin) | ```get_nearest_neighbors``` in [InferenceModel](https://kevinmusgrave.github.io/pytorch-metric-learning/inference_models) |
 | [mlw214](https://github.com/mlw214) | Added ```return_per_class``` to [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) |
@@ -272,14 +269,15 @@
 | [joaqo](https://github.com/joaqo) | |
 | [JoOkuma](https://github.com/JoOkuma) | |
 | [gkouros](https://github.com/gkouros) | |
 | [yutanakamura-tky](https://github.com/yutanakamura-tky) | |
 | [KinglittleQ](https://github.com/KinglittleQ) | |
 | [martin0258](https://github.com/martin0258) | |
 | [michaeldeyzel](https://github.com/michaeldeyzel) | |
+| [HSinger04](https://github.com/HSinger04) | |
 
 
 
 ### Facebook AI
 Thank you to [Ser-Nam Lim](https://research.fb.com/people/lim-ser-nam/) at [Facebook AI](https://ai.facebook.com/), and my research advisor, [Professor Serge Belongie](https://vision.cornell.edu/se3/people/serge-belongie/). This project began during my internship at Facebook AI where I received valuable feedback from Ser-Nam, and his team of computer vision and machine learning engineers and research scientists. In particular, thanks to [Ashish Shah](https://www.linkedin.com/in/ashish217/) and [Austin Reiter](https://www.linkedin.com/in/austin-reiter-3962aa7/) for reviewing my code during its early stages of development.
 
 ### Open-source repos
```

#### html2text {}

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 2.1 Name: pytorch-metric-learning Version: 2.1.1 Summary: The
+Metadata-Version: 2.1 Name: pytorch-metric-learning Version: 2.1.2 Summary: The
 easiest way to use deep metric learning in your application. Modular, flexible,
 and extensible. Written in PyTorch. Home-page: https://github.com/
 KevinMusgrave/pytorch-metric-learning Author: Kevin Musgrave License: UNKNOWN
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.0 Description-Content-Type: text/markdown
 Provides-Extra: with-hooks Provides-Extra: with-hooks-cpu Provides-Extra: docs
 Provides-Extra: dev License-File: LICENSE
 ****** [PyTorch_Metric_Learning] ******
                        [PyPi_version] [Anaconda_version]
-## News **January 16**: v1.7.0 - Fixes an edge case in ArcFaceLoss. See the
-[release notes](https://github.com/KevinMusgrave/pytorch-metric-learning/
-releases/tag/v1.7.0). - Thanks to contributor [ElisonSherton](https://
-github.com/ElisonSherton). **September 3**: v1.6.0 - `DistributedLossWrapper`
-and `DistributedMinerWrapper` now support `ref_emb` and `ref_labels`. - Thanks
-to contributor [NoTody](https://github.com/NoTody). ## Documentation - [**View
-the documentation here**](https://kevinmusgrave.github.io/pytorch-metric-
-learning/) - [**View the installation instructions here**](https://github.com/
-KevinMusgrave/pytorch-metric-learning#installation) - [**View the available
-losses, miners etc. here**](https://github.com/KevinMusgrave/pytorch-metric-
-learning/blob/master/CONTENTS.md) ## Google Colab Examples See the [examples
-folder](https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/
-examples/README.md) for notebooks you can download or run on Google Colab. ##
-PyTorch Metric Learning Overview This library contains 9 modules, each of which
-can be used independently within your existing codebase, or combined together
-for a complete train/test workflow. ![high_level_module_overview](docs/imgs/
+## News **April 5**: v2.1.0 - Added [PNPLoss](https://kevinmusgrave.github.io/
+pytorch-metric-learning/losses/#pnploss) - Thanks to contributor
+[interestingzhuo](https://github.com/interestingzhuo). **January 29**: v2.0.0 -
+Added SelfSupervisedLoss, plus various API improvements. See the [release
+notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/
+v2.0.0). - Thanks to contributor [cwkeam](https://github.com/cwkeam). ##
+Documentation - [**View the documentation here**](https://
+kevinmusgrave.github.io/pytorch-metric-learning/) - [**View the installation
+instructions here**](https://github.com/KevinMusgrave/pytorch-metric-
+learning#installation) - [**View the available losses, miners etc. here**]
+(https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/
+CONTENTS.md) ## Google Colab Examples See the [examples folder](https://
+github.com/KevinMusgrave/pytorch-metric-learning/blob/master/examples/
+README.md) for notebooks you can download or run on Google Colab. ## PyTorch
+Metric Learning Overview This library contains 9 modules, each of which can be
+used independently within your existing codebase, or combined together for a
+complete train/test workflow. ![high_level_module_overview](docs/imgs/
 high_level_module_overview.png) ## How loss functions work ### Using losses and
 miners in your training loop Letâs initialize a plain [TripletMarginLoss]
 (https://kevinmusgrave.github.io/pytorch-metric-learning/losses/
 #tripletmarginloss): ```python from pytorch_metric_learning import losses
 loss_func = losses.TripletMarginLoss() ``` To compute the loss in your training
 loop, pass in the embeddings computed by your model, and the corresponding
 labels. The embeddings should have size (N, embedding_size), and the labels
@@ -68,86 +69,81 @@
 from pytorch_metric_learning.regularizers import LpRegularizer from
 pytorch_metric_learning import losses loss_func = losses.TripletMarginLoss
 (distance = CosineSimilarity(), reducer = ThresholdReducer(high=0.3),
 embedding_regularizer = LpRegularizer()) ``` This customized triplet loss has
 the following properties: - The loss will be computed using cosine similarity
 instead of Euclidean distance. - All triplet losses that are higher than 0.3
 will be discarded. - The embeddings will be L2 regularized. ### Using loss
-functions for unsupervised / self-supervised learning The TripletMarginLoss is
-an embedding-based or tuple-based loss. This means that internally, there is no
-real notion of "classes". Tuples (pairs or triplets) are formed at each
-iteration, based on the labels it receives. The labels don't have to represent
-classes. They simply need to indicate the positive and negative relationships
-between the embeddings. Thus, it is easy to use these loss functions for
-unsupervised or self-supervised learning. For example, the code below is a
-simplified version of the augmentation strategy commonly used in self-
-supervision. The dataset does not come with any labels. Instead, the labels are
-created in the training loop, solely to indicate which embeddings are positive
-pairs. ```python # your training for-loop for i, data in enumerate(dataloader):
-optimizer.zero_grad() embeddings = your_model(data) augmented = your_model
-(your_augmentation(data)) labels = torch.arange(embeddings.size(0)) embeddings
-= torch.cat([embeddings, augmented], dim=0) labels = torch.cat([labels,
-labels], dim=0) loss = loss_func(embeddings, labels) loss.backward()
-optimizer.step() ``` If you're interested in [MoCo](https://arxiv.org/pdf/
-1911.05722.pdf)-style self-supervision, take a look at the [MoCo on CIFAR10]
-(https://github.com/KevinMusgrave/pytorch-metric-learning/tree/master/
-examples#simple-examples) notebook. It uses CrossBatchMemory to implement the
-momentum encoder queue, which means you can use any tuple loss, and any tuple
-miner to extract hard samples from the queue. ## Highlights of the rest of the
-library - For a convenient way to train your model, take a look at the
-[trainers](https://kevinmusgrave.github.io/pytorch-metric-learning/trainers/).
-- Want to test your model's accuracy on a dataset? Try the [testers](https://
-kevinmusgrave.github.io/pytorch-metric-learning/testers/). - To compute the
-accuracy of an embedding space directly, use [AccuracyCalculator](https://
-kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/). If
-you're short of time and want a complete train/test workflow, check out the
-[example Google Colab notebooks](https://github.com/KevinMusgrave/pytorch-
-metric-learning/tree/master/examples). To learn more about all of the above,
-[see the documentation](https://kevinmusgrave.github.io/pytorch-metric-
-learning). ## Installation ### Required PyTorch version - ```pytorch-metric-
-learning >= v0.9.90``` requires ```torch >= 1.6``` - ```pytorch-metric-learning
-< v0.9.90``` doesn't have a version requirement, but was tested with ```torch
->= 1.2``` Other dependencies: ```numpy, scikit-learn, tqdm, torchvision``` ###
-Pip ``` pip install pytorch-metric-learning ``` **To get the latest dev
-version**: ``` pip install pytorch-metric-learning --pre ``` **To install on
-Windows**: ``` pip install torch===1.6.0 torchvision===0.7.0 -f https://
-download.pytorch.org/whl/torch_stable.html pip install pytorch-metric-learning
-``` **To install with evaluation and logging capabilities** (This will install
-the unofficial pypi version of faiss-gpu, plus record-keeper and tensorboard):
-``` pip install pytorch-metric-learning[with-hooks] ``` **To install with
-evaluation and logging capabilities (CPU)** (This will install the unofficial
-pypi version of faiss-cpu, plus record-keeper and tensorboard): ``` pip install
-pytorch-metric-learning[with-hooks-cpu] ``` ### Conda ``` conda install -
-c conda-forge pytorch-metric-learning ``` **To use the testing module, you'll
-need faiss, which can be installed via conda as well. See the [installation
-instructions for faiss](https://github.com/facebookresearch/faiss/blob/master/
-INSTALL.md).**  ## Benchmark results See [powerful-benchmarker](https://
-github.com/KevinMusgrave/powerful-benchmarker/) to view benchmark results and
-to use the benchmarking tool. ## Development Development is done on the
-```dev``` branch: ``` git checkout dev ``` Unit tests can be run with the
-default ```unittest``` library: ```bash python -m unittest discover ``` You can
-specify the test datatypes and test device as environment variables. For
-example, to test using float32 and float64 on the CPU: ```bash
-TEST_DTYPES=float32,float64 TEST_DEVICE=cpu python -m unittest discover ``` To
-run a single test file instead of the entire test suite, specify the file name:
-```bash python -m unittest tests/losses/test_angular_loss.py ``` Code is
-formatted using ```black``` and ```isort```: ```bash pip install black isort ./
-format_code.sh ``` ## Acknowledgements ### Contributors Thanks to the
-contributors who made pull requests! | Contributor | Highlights | | -- | -- | |
-[mlopezantequera](https://github.com/mlopezantequera) | - Made the [testers]
-(https://kevinmusgrave.github.io/pytorch-metric-learning/testers) work on any
+functions for unsupervised / self-supervised learning A `SelfSupervisedLoss`
+wrapper is provided for self-supervised learning: ```python from
+pytorch_metric_learning.losses import SelfSupervisedLoss loss_func =
+SelfSupervisedLoss(TripletMarginLoss()) # your training for-loop for i, data in
+enumerate(dataloader): optimizer.zero_grad() embeddings = your_model(data)
+augmented = your_model(your_augmentation(data)) loss = loss_func(embeddings,
+augmented) loss.backward() optimizer.step() ``` If you're interested in [MoCo]
+(https://arxiv.org/pdf/1911.05722.pdf)-style self-supervision, take a look at
+the [MoCo on CIFAR10](https://github.com/KevinMusgrave/pytorch-metric-learning/
+tree/master/examples#simple-examples) notebook. It uses CrossBatchMemory to
+implement the momentum encoder queue, which means you can use any tuple loss,
+and any tuple miner to extract hard samples from the queue. ## Highlights of
+the rest of the library - For a convenient way to train your model, take a look
+at the [trainers](https://kevinmusgrave.github.io/pytorch-metric-learning/
+trainers/). - Want to test your model's accuracy on a dataset? Try the
+[testers](https://kevinmusgrave.github.io/pytorch-metric-learning/testers/). -
+To compute the accuracy of an embedding space directly, use
+[AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/
+accuracy_calculation/). If you're short of time and want a complete train/test
+workflow, check out the [example Google Colab notebooks](https://github.com/
+KevinMusgrave/pytorch-metric-learning/tree/master/examples). To learn more
+about all of the above, [see the documentation](https://
+kevinmusgrave.github.io/pytorch-metric-learning). ## Installation ### Required
+PyTorch version - ```pytorch-metric-learning >= v0.9.90``` requires ```torch >=
+1.6``` - ```pytorch-metric-learning < v0.9.90``` doesn't have a version
+requirement, but was tested with ```torch >= 1.2``` Other dependencies:
+```numpy, scikit-learn, tqdm, torchvision``` ### Pip ``` pip install pytorch-
+metric-learning ``` **To get the latest dev version**: ``` pip install pytorch-
+metric-learning --pre ``` **To install on Windows**: ``` pip install
+torch===1.6.0 torchvision===0.7.0 -f https://download.pytorch.org/whl/
+torch_stable.html pip install pytorch-metric-learning ``` **To install with
+evaluation and logging capabilities** (This will install the unofficial pypi
+version of faiss-gpu, plus record-keeper and tensorboard): ``` pip install
+pytorch-metric-learning[with-hooks] ``` **To install with evaluation and
+logging capabilities (CPU)** (This will install the unofficial pypi version of
+faiss-cpu, plus record-keeper and tensorboard): ``` pip install pytorch-metric-
+learning[with-hooks-cpu] ``` ### Conda ``` conda install -c conda-forge
+pytorch-metric-learning ``` **To use the testing module, you'll need faiss,
+which can be installed via conda as well. See the [installation instructions
+for faiss](https://github.com/facebookresearch/faiss/blob/master/INSTALL.md).**
+## Benchmark results See [powerful-benchmarker](https://github.com/
+KevinMusgrave/powerful-benchmarker/) to view benchmark results and to use the
+benchmarking tool. ## Development Development is done on the ```dev``` branch:
+``` git checkout dev ``` Unit tests can be run with the default ```unittest```
+library: ```bash python -m unittest discover ``` You can specify the test
+datatypes and test device as environment variables. For example, to test using
+float32 and float64 on the CPU: ```bash TEST_DTYPES=float32,float64
+TEST_DEVICE=cpu python -m unittest discover ``` To run a single test file
+instead of the entire test suite, specify the file name: ```bash python -
+m unittest tests/losses/test_angular_loss.py ``` Code is formatted using
+```black``` and ```isort```: ```bash pip install black isort ./format_code.sh
+``` ## Acknowledgements ### Contributors Thanks to the contributors who made
+pull requests! | Contributor | Highlights | | -- | -- | |[mlopezantequera]
+(https://github.com/mlopezantequera) | - Made the [testers](https://
+kevinmusgrave.github.io/pytorch-metric-learning/testers) work on any
 combination of query and reference sets
 - Made [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-
 learning/accuracy_calculation/) work with arbitrary label comparisons | |
-[cwkeam](https://github.com/cwkeam) | - [VICRegLoss](https://
-kevinmusgrave.github.io/pytorch-metric-learning/losses/#vicregloss)
+[cwkeam](https://github.com/cwkeam) | - [SelfSupervisedLoss](https://
+kevinmusgrave.github.io/pytorch-metric-learning/losses/#selfsupervisedloss)
+- [VICRegLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/
+#vicregloss)
 - Added mean reciprocal rank accuracy to [AccuracyCalculator](https://
-kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) | |
-[marijnl](https://github.com/marijnl)| - [BatchEasyHardMiner](https://
-kevinmusgrave.github.io/pytorch-metric-learning/miners/#batcheasyhardminer)
+kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/)
+- BaseLossWrapper| |[marijnl](https://github.com/marijnl)| -
+[BatchEasyHardMiner](https://kevinmusgrave.github.io/pytorch-metric-learning/
+miners/#batcheasyhardminer)
 - [TwoStreamMetricLoss](https://kevinmusgrave.github.io/pytorch-metric-
 learning/trainers/#twostreammetricloss)
 - [GlobalTwoStreamEmbeddingSpaceTester](https://kevinmusgrave.github.io/
 pytorch-metric-learning/testers/#globaltwostreamembeddingspacetester)
 - [Example using trainers.TwoStreamMetricLoss](https://github.com/
 KevinMusgrave/pytorch-metric-learning/blob/master/examples/notebooks/
 TwoStreamMetricLoss.ipynb) | | [chingisooinar](https://github.com/
@@ -155,15 +151,15 @@
 pytorch-metric-learning/losses/#subcenterarcfaceloss) | | [elias-ramzi](https:/
 /github.com/elias-ramzi) | [HierarchicalSampler](https://
 kevinmusgrave.github.io/pytorch-metric-learning/samplers/#hierarchicalsampler)
 | | [fjsj](https://github.com/fjsj) | [SupConLoss](https://
 kevinmusgrave.github.io/pytorch-metric-learning/losses/#supconloss) | |
 [AlenUbuntu](https://github.com/AlenUbuntu) | [CircleLoss](https://
 kevinmusgrave.github.io/pytorch-metric-learning/losses/#circleloss) | |
-[interestingzhuo](https://github.com/interestingzhuo) | [**PNPLoss**](https://
+[interestingzhuo](https://github.com/interestingzhuo) | [PNPLoss](https://
 kevinmusgrave.github.io/pytorch-metric-learning/losses/#pnploss) | | [wconnell]
 (https://github.com/wconnell) | [Learning a scRNAseq Metric Embedding](https://
 github.com/KevinMusgrave/pytorch-metric-learning/blob/master/examples/
 notebooks/scRNAseq_MetricEmbedding.ipynb) | | [AlexSchuy](https://github.com/
 AlexSchuy) | optimized
 ```utils.loss_and_miner_utils.get_random_triplet_indices``` | | [JohnGiorgi]
 (https://github.com/JohnGiorgi) | ```all_gather``` in [utils.distributed]
@@ -182,30 +178,30 @@
 ElisonSherton) | Fixed an edge case in ArcFaceLoss. | | [z1w](https://
 github.com/z1w) | | | [thinline72](https://github.com/thinline72) | | |
 [tpanum](https://github.com/tpanum) | | | [fralik](https://github.com/fralik) |
 | | [joaqo](https://github.com/joaqo) | | | [JoOkuma](https://github.com/
 JoOkuma) | | | [gkouros](https://github.com/gkouros) | | | [yutanakamura-tky]
 (https://github.com/yutanakamura-tky) | | | [KinglittleQ](https://github.com/
 KinglittleQ) | | | [martin0258](https://github.com/martin0258) | | |
-[michaeldeyzel](https://github.com/michaeldeyzel) | | ### Facebook AI Thank you
-to [Ser-Nam Lim](https://research.fb.com/people/lim-ser-nam/) at [Facebook AI]
-(https://ai.facebook.com/), and my research advisor, [Professor Serge Belongie]
-(https://vision.cornell.edu/se3/people/serge-belongie/). This project began
-during my internship at Facebook AI where I received valuable feedback from
-Ser-Nam, and his team of computer vision and machine learning engineers and
-research scientists. In particular, thanks to [Ashish Shah](https://
-www.linkedin.com/in/ashish217/) and [Austin Reiter](https://www.linkedin.com/
-in/austin-reiter-3962aa7/) for reviewing my code during its early stages of
-development. ### Open-source repos This library contains code that has been
-adapted and modified from the following great open-source repos: - https://
-github.com/bnu-wangxun/Deep_Metric - https://github.com/chaoyuaw/incubator-
-mxnet/blob/master/example/gluon/embedding_learning - https://github.com/
-facebookresearch/deepcluster - https://github.com/geonm/proxy-anchor-loss -
-https://github.com/idstcv/SoftTriple - https://github.com/kunhe/FastAP-metric-
-learning - https://github.com/ronekko/deep_metric_learning - https://
-github.com/tjddus9597/Proxy-Anchor-CVPR2020 - http://kaizhao.net/regularface
-### Logo Thanks to [Jeff Musgrave](https://www.designgenius.ca/) for designing
-the logo. ## Citing this library If you'd like to cite pytorch-metric-learning
-in your paper, you can use this bibtex: ```latex @article
-{Musgrave2020PyTorchML, title={PyTorch Metric Learning}, author={Kevin Musgrave
-and Serge J. Belongie and Ser-Nam Lim}, journal={ArXiv}, year={2020}, volume=
-{abs/2008.09164} } ```
+[michaeldeyzel](https://github.com/michaeldeyzel) | | | [HSinger04](https://
+github.com/HSinger04) | | ### Facebook AI Thank you to [Ser-Nam Lim](https://
+research.fb.com/people/lim-ser-nam/) at [Facebook AI](https://ai.facebook.com/
+), and my research advisor, [Professor Serge Belongie](https://
+vision.cornell.edu/se3/people/serge-belongie/). This project began during my
+internship at Facebook AI where I received valuable feedback from Ser-Nam, and
+his team of computer vision and machine learning engineers and research
+scientists. In particular, thanks to [Ashish Shah](https://www.linkedin.com/in/
+ashish217/) and [Austin Reiter](https://www.linkedin.com/in/austin-reiter-
+3962aa7/) for reviewing my code during its early stages of development. ###
+Open-source repos This library contains code that has been adapted and modified
+from the following great open-source repos: - https://github.com/bnu-wangxun/
+Deep_Metric - https://github.com/chaoyuaw/incubator-mxnet/blob/master/example/
+gluon/embedding_learning - https://github.com/facebookresearch/deepcluster -
+https://github.com/geonm/proxy-anchor-loss - https://github.com/idstcv/
+SoftTriple - https://github.com/kunhe/FastAP-metric-learning - https://
+github.com/ronekko/deep_metric_learning - https://github.com/tjddus9597/Proxy-
+Anchor-CVPR2020 - http://kaizhao.net/regularface ### Logo Thanks to [Jeff
+Musgrave](https://www.designgenius.ca/) for designing the logo. ## Citing this
+library If you'd like to cite pytorch-metric-learning in your paper, you can
+use this bibtex: ```latex @article{Musgrave2020PyTorchML, title={PyTorch Metric
+Learning}, author={Kevin Musgrave and Serge J. Belongie and Ser-Nam Lim},
+journal={ArXiv}, year={2020}, volume={abs/2008.09164} } ```
```

### Comparing `pytorch-metric-learning-2.1.1/README.md` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: pytorch-metric-learning
+Version: 2.1.2
+Summary: The easiest way to use deep metric learning in your application. Modular, flexible, and extensible. Written in PyTorch.
+Home-page: https://github.com/KevinMusgrave/pytorch-metric-learning
+Author: Kevin Musgrave
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.0
+Description-Content-Type: text/markdown
+Provides-Extra: with-hooks
+Provides-Extra: with-hooks-cpu
+Provides-Extra: docs
+Provides-Extra: dev
+License-File: LICENSE
+
 <h1>
 <a href="https://github.com/KevinMusgrave/pytorch-metric-learning">
 <img alt="PyTorch Metric Learning" src="https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/docs/imgs/Logo2.png">
 </a>
 </h1>
 
 <p align="center">
@@ -14,21 +33,22 @@
  <a href="https://anaconda.org/conda-forge/pytorch-metric-learning">
      <img alt="Anaconda version" src="https://img.shields.io/conda/v/conda-forge/pytorch-metric-learning?color=bright-green">
  </a>
 </p>
 
 ## News
 
-**January 16**: v1.7.0
-- Fixes an edge case in ArcFaceLoss. See the [release notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/v1.7.0).
-- Thanks to contributor [ElisonSherton](https://github.com/ElisonSherton).
-
-**September 3**: v1.6.0
-- `DistributedLossWrapper` and `DistributedMinerWrapper` now support `ref_emb` and `ref_labels`.
-- Thanks to contributor [NoTody](https://github.com/NoTody).
+**April 5**: v2.1.0
+- Added [PNPLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#pnploss)
+- Thanks to contributor [interestingzhuo](https://github.com/interestingzhuo).
+
+**January 29**: v2.0.0
+- Added SelfSupervisedLoss, plus various API improvements. See the [release notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/v2.0.0).
+- Thanks to contributor [cwkeam](https://github.com/cwkeam).
+
 
 ## Documentation
 - [**View the documentation here**](https://kevinmusgrave.github.io/pytorch-metric-learning/)
 - [**View the installation instructions here**](https://github.com/KevinMusgrave/pytorch-metric-learning#installation)
 - [**View the available losses, miners etc. here**](https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/CONTENTS.md) 
 
 
@@ -102,30 +122,26 @@
 
  - The loss will be computed using cosine similarity instead of Euclidean distance.
  - All triplet losses that are higher than 0.3 will be discarded.
  - The embeddings will be L2 regularized.  
 
 ### Using loss functions for unsupervised / self-supervised learning
 
-The TripletMarginLoss is an embedding-based or tuple-based loss. This means that internally, there is no real notion of "classes". Tuples (pairs or triplets) are formed at each iteration, based on the labels it receives. The labels don't have to represent classes. They simply need to indicate the positive and negative relationships between the embeddings. Thus, it is easy to use these loss functions for unsupervised or self-supervised learning. 
-
-For example, the code below is a simplified version of the augmentation strategy commonly used in self-supervision. The dataset does not come with any labels. Instead, the labels are created in the training loop, solely to indicate which embeddings are positive pairs.
+A `SelfSupervisedLoss` wrapper is provided for self-supervised learning:
 
 ```python
+from pytorch_metric_learning.losses import SelfSupervisedLoss
+loss_func = SelfSupervisedLoss(TripletMarginLoss())
+
 # your training for-loop
 for i, data in enumerate(dataloader):
 	optimizer.zero_grad()
 	embeddings = your_model(data)
 	augmented = your_model(your_augmentation(data))
-	labels = torch.arange(embeddings.size(0))
-
-	embeddings = torch.cat([embeddings, augmented], dim=0)
-	labels = torch.cat([labels, labels], dim=0)
-
-	loss = loss_func(embeddings, labels)
+	loss = loss_func(embeddings, augmented)
 	loss.backward()
 	optimizer.step()
 ```
 
 If you're interested in [MoCo](https://arxiv.org/pdf/1911.05722.pdf)-style self-supervision, take a look at the [MoCo on CIFAR10](https://github.com/KevinMusgrave/pytorch-metric-learning/tree/master/examples#simple-examples) notebook. It uses CrossBatchMemory to implement the momentum encoder queue, which means you can use any tuple loss, and any tuple miner to extract hard samples from the queue.
 
 
@@ -225,21 +241,21 @@
 
 ### Contributors
 Thanks to the contributors who made pull requests!
 
 | Contributor | Highlights |
 | -- | -- |
 |[mlopezantequera](https://github.com/mlopezantequera) | - Made the [testers](https://kevinmusgrave.github.io/pytorch-metric-learning/testers) work on any combination of query and reference sets <br/> - Made [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) work with arbitrary label comparisons |
-|[cwkeam](https://github.com/cwkeam) | - [VICRegLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#vicregloss) <br/> - Added mean reciprocal rank accuracy to [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) |
+|[cwkeam](https://github.com/cwkeam) | - [SelfSupervisedLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#selfsupervisedloss) <br/> - [VICRegLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#vicregloss) <br/> - Added mean reciprocal rank accuracy to [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) <br/> - BaseLossWrapper|
 |[marijnl](https://github.com/marijnl)| - [BatchEasyHardMiner](https://kevinmusgrave.github.io/pytorch-metric-learning/miners/#batcheasyhardminer) <br/> - [TwoStreamMetricLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/trainers/#twostreammetricloss) <br/> - [GlobalTwoStreamEmbeddingSpaceTester](https://kevinmusgrave.github.io/pytorch-metric-learning/testers/#globaltwostreamembeddingspacetester) <br/> - [Example using trainers.TwoStreamMetricLoss](https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/examples/notebooks/TwoStreamMetricLoss.ipynb) |
 | [chingisooinar](https://github.com/chingisooinar) | [SubCenterArcFaceLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#subcenterarcfaceloss) |
 | [elias-ramzi](https://github.com/elias-ramzi) | [HierarchicalSampler](https://kevinmusgrave.github.io/pytorch-metric-learning/samplers/#hierarchicalsampler) |
 | [fjsj](https://github.com/fjsj) | [SupConLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#supconloss) |
 | [AlenUbuntu](https://github.com/AlenUbuntu) | [CircleLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#circleloss) |
-| [interestingzhuo](https://github.com/interestingzhuo) | [**PNPLoss**](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#pnploss) |
+| [interestingzhuo](https://github.com/interestingzhuo) | [PNPLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#pnploss) |
 | [wconnell](https://github.com/wconnell) | [Learning a scRNAseq Metric Embedding](https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/examples/notebooks/scRNAseq_MetricEmbedding.ipynb) |
 | [AlexSchuy](https://github.com/AlexSchuy) | optimized ```utils.loss_and_miner_utils.get_random_triplet_indices``` |
 | [JohnGiorgi](https://github.com/JohnGiorgi) | ```all_gather``` in [utils.distributed](https://kevinmusgrave.github.io/pytorch-metric-learning/distributed) |
 | [Hummer12007](https://github.com/Hummer12007) | ```utils.key_checker``` |
 | [vltanh](https://github.com/vltanh) | Made ```InferenceModel.train_indexer``` accept datasets |
 | [btseytlin](https://github.com/btseytlin) | ```get_nearest_neighbors``` in [InferenceModel](https://kevinmusgrave.github.io/pytorch-metric-learning/inference_models) |
 | [mlw214](https://github.com/mlw214) | Added ```return_per_class``` to [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) |
@@ -253,14 +269,15 @@
 | [joaqo](https://github.com/joaqo) | |
 | [JoOkuma](https://github.com/JoOkuma) | |
 | [gkouros](https://github.com/gkouros) | |
 | [yutanakamura-tky](https://github.com/yutanakamura-tky) | |
 | [KinglittleQ](https://github.com/KinglittleQ) | |
 | [martin0258](https://github.com/martin0258) | |
 | [michaeldeyzel](https://github.com/michaeldeyzel) | |
+| [HSinger04](https://github.com/HSinger04) | |
 
 
 
 ### Facebook AI
 Thank you to [Ser-Nam Lim](https://research.fb.com/people/lim-ser-nam/) at [Facebook AI](https://ai.facebook.com/), and my research advisor, [Professor Serge Belongie](https://vision.cornell.edu/se3/people/serge-belongie/). This project began during my internship at Facebook AI where I received valuable feedback from Ser-Nam, and his team of computer vision and machine learning engineers and research scientists. In particular, thanks to [Ashish Shah](https://www.linkedin.com/in/ashish217/) and [Austin Reiter](https://www.linkedin.com/in/austin-reiter-3962aa7/) for reviewing my code during its early stages of development.
 
 ### Open-source repos
@@ -285,7 +302,9 @@
   title={PyTorch Metric Learning},
   author={Kevin Musgrave and Serge J. Belongie and Ser-Nam Lim},
   journal={ArXiv},
   year={2020},
   volume={abs/2008.09164}
 }
 ```
+
+
```

#### html2text {}

```diff
@@ -1,25 +1,35 @@
+Metadata-Version: 2.1 Name: pytorch-metric-learning Version: 2.1.2 Summary: The
+easiest way to use deep metric learning in your application. Modular, flexible,
+and extensible. Written in PyTorch. Home-page: https://github.com/
+KevinMusgrave/pytorch-metric-learning Author: Kevin Musgrave License: UNKNOWN
+Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.0 Description-Content-Type: text/markdown
+Provides-Extra: with-hooks Provides-Extra: with-hooks-cpu Provides-Extra: docs
+Provides-Extra: dev License-File: LICENSE
 ****** [PyTorch_Metric_Learning] ******
                        [PyPi_version] [Anaconda_version]
-## News **January 16**: v1.7.0 - Fixes an edge case in ArcFaceLoss. See the
-[release notes](https://github.com/KevinMusgrave/pytorch-metric-learning/
-releases/tag/v1.7.0). - Thanks to contributor [ElisonSherton](https://
-github.com/ElisonSherton). **September 3**: v1.6.0 - `DistributedLossWrapper`
-and `DistributedMinerWrapper` now support `ref_emb` and `ref_labels`. - Thanks
-to contributor [NoTody](https://github.com/NoTody). ## Documentation - [**View
-the documentation here**](https://kevinmusgrave.github.io/pytorch-metric-
-learning/) - [**View the installation instructions here**](https://github.com/
-KevinMusgrave/pytorch-metric-learning#installation) - [**View the available
-losses, miners etc. here**](https://github.com/KevinMusgrave/pytorch-metric-
-learning/blob/master/CONTENTS.md) ## Google Colab Examples See the [examples
-folder](https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/
-examples/README.md) for notebooks you can download or run on Google Colab. ##
-PyTorch Metric Learning Overview This library contains 9 modules, each of which
-can be used independently within your existing codebase, or combined together
-for a complete train/test workflow. ![high_level_module_overview](docs/imgs/
+## News **April 5**: v2.1.0 - Added [PNPLoss](https://kevinmusgrave.github.io/
+pytorch-metric-learning/losses/#pnploss) - Thanks to contributor
+[interestingzhuo](https://github.com/interestingzhuo). **January 29**: v2.0.0 -
+Added SelfSupervisedLoss, plus various API improvements. See the [release
+notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/
+v2.0.0). - Thanks to contributor [cwkeam](https://github.com/cwkeam). ##
+Documentation - [**View the documentation here**](https://
+kevinmusgrave.github.io/pytorch-metric-learning/) - [**View the installation
+instructions here**](https://github.com/KevinMusgrave/pytorch-metric-
+learning#installation) - [**View the available losses, miners etc. here**]
+(https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/
+CONTENTS.md) ## Google Colab Examples See the [examples folder](https://
+github.com/KevinMusgrave/pytorch-metric-learning/blob/master/examples/
+README.md) for notebooks you can download or run on Google Colab. ## PyTorch
+Metric Learning Overview This library contains 9 modules, each of which can be
+used independently within your existing codebase, or combined together for a
+complete train/test workflow. ![high_level_module_overview](docs/imgs/
 high_level_module_overview.png) ## How loss functions work ### Using losses and
 miners in your training loop Letâs initialize a plain [TripletMarginLoss]
 (https://kevinmusgrave.github.io/pytorch-metric-learning/losses/
 #tripletmarginloss): ```python from pytorch_metric_learning import losses
 loss_func = losses.TripletMarginLoss() ``` To compute the loss in your training
 loop, pass in the embeddings computed by your model, and the corresponding
 labels. The embeddings should have size (N, embedding_size), and the labels
@@ -59,86 +69,81 @@
 from pytorch_metric_learning.regularizers import LpRegularizer from
 pytorch_metric_learning import losses loss_func = losses.TripletMarginLoss
 (distance = CosineSimilarity(), reducer = ThresholdReducer(high=0.3),
 embedding_regularizer = LpRegularizer()) ``` This customized triplet loss has
 the following properties: - The loss will be computed using cosine similarity
 instead of Euclidean distance. - All triplet losses that are higher than 0.3
 will be discarded. - The embeddings will be L2 regularized. ### Using loss
-functions for unsupervised / self-supervised learning The TripletMarginLoss is
-an embedding-based or tuple-based loss. This means that internally, there is no
-real notion of "classes". Tuples (pairs or triplets) are formed at each
-iteration, based on the labels it receives. The labels don't have to represent
-classes. They simply need to indicate the positive and negative relationships
-between the embeddings. Thus, it is easy to use these loss functions for
-unsupervised or self-supervised learning. For example, the code below is a
-simplified version of the augmentation strategy commonly used in self-
-supervision. The dataset does not come with any labels. Instead, the labels are
-created in the training loop, solely to indicate which embeddings are positive
-pairs. ```python # your training for-loop for i, data in enumerate(dataloader):
-optimizer.zero_grad() embeddings = your_model(data) augmented = your_model
-(your_augmentation(data)) labels = torch.arange(embeddings.size(0)) embeddings
-= torch.cat([embeddings, augmented], dim=0) labels = torch.cat([labels,
-labels], dim=0) loss = loss_func(embeddings, labels) loss.backward()
-optimizer.step() ``` If you're interested in [MoCo](https://arxiv.org/pdf/
-1911.05722.pdf)-style self-supervision, take a look at the [MoCo on CIFAR10]
-(https://github.com/KevinMusgrave/pytorch-metric-learning/tree/master/
-examples#simple-examples) notebook. It uses CrossBatchMemory to implement the
-momentum encoder queue, which means you can use any tuple loss, and any tuple
-miner to extract hard samples from the queue. ## Highlights of the rest of the
-library - For a convenient way to train your model, take a look at the
-[trainers](https://kevinmusgrave.github.io/pytorch-metric-learning/trainers/).
-- Want to test your model's accuracy on a dataset? Try the [testers](https://
-kevinmusgrave.github.io/pytorch-metric-learning/testers/). - To compute the
-accuracy of an embedding space directly, use [AccuracyCalculator](https://
-kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/). If
-you're short of time and want a complete train/test workflow, check out the
-[example Google Colab notebooks](https://github.com/KevinMusgrave/pytorch-
-metric-learning/tree/master/examples). To learn more about all of the above,
-[see the documentation](https://kevinmusgrave.github.io/pytorch-metric-
-learning). ## Installation ### Required PyTorch version - ```pytorch-metric-
-learning >= v0.9.90``` requires ```torch >= 1.6``` - ```pytorch-metric-learning
-< v0.9.90``` doesn't have a version requirement, but was tested with ```torch
->= 1.2``` Other dependencies: ```numpy, scikit-learn, tqdm, torchvision``` ###
-Pip ``` pip install pytorch-metric-learning ``` **To get the latest dev
-version**: ``` pip install pytorch-metric-learning --pre ``` **To install on
-Windows**: ``` pip install torch===1.6.0 torchvision===0.7.0 -f https://
-download.pytorch.org/whl/torch_stable.html pip install pytorch-metric-learning
-``` **To install with evaluation and logging capabilities** (This will install
-the unofficial pypi version of faiss-gpu, plus record-keeper and tensorboard):
-``` pip install pytorch-metric-learning[with-hooks] ``` **To install with
-evaluation and logging capabilities (CPU)** (This will install the unofficial
-pypi version of faiss-cpu, plus record-keeper and tensorboard): ``` pip install
-pytorch-metric-learning[with-hooks-cpu] ``` ### Conda ``` conda install -
-c conda-forge pytorch-metric-learning ``` **To use the testing module, you'll
-need faiss, which can be installed via conda as well. See the [installation
-instructions for faiss](https://github.com/facebookresearch/faiss/blob/master/
-INSTALL.md).**  ## Benchmark results See [powerful-benchmarker](https://
-github.com/KevinMusgrave/powerful-benchmarker/) to view benchmark results and
-to use the benchmarking tool. ## Development Development is done on the
-```dev``` branch: ``` git checkout dev ``` Unit tests can be run with the
-default ```unittest``` library: ```bash python -m unittest discover ``` You can
-specify the test datatypes and test device as environment variables. For
-example, to test using float32 and float64 on the CPU: ```bash
-TEST_DTYPES=float32,float64 TEST_DEVICE=cpu python -m unittest discover ``` To
-run a single test file instead of the entire test suite, specify the file name:
-```bash python -m unittest tests/losses/test_angular_loss.py ``` Code is
-formatted using ```black``` and ```isort```: ```bash pip install black isort ./
-format_code.sh ``` ## Acknowledgements ### Contributors Thanks to the
-contributors who made pull requests! | Contributor | Highlights | | -- | -- | |
-[mlopezantequera](https://github.com/mlopezantequera) | - Made the [testers]
-(https://kevinmusgrave.github.io/pytorch-metric-learning/testers) work on any
+functions for unsupervised / self-supervised learning A `SelfSupervisedLoss`
+wrapper is provided for self-supervised learning: ```python from
+pytorch_metric_learning.losses import SelfSupervisedLoss loss_func =
+SelfSupervisedLoss(TripletMarginLoss()) # your training for-loop for i, data in
+enumerate(dataloader): optimizer.zero_grad() embeddings = your_model(data)
+augmented = your_model(your_augmentation(data)) loss = loss_func(embeddings,
+augmented) loss.backward() optimizer.step() ``` If you're interested in [MoCo]
+(https://arxiv.org/pdf/1911.05722.pdf)-style self-supervision, take a look at
+the [MoCo on CIFAR10](https://github.com/KevinMusgrave/pytorch-metric-learning/
+tree/master/examples#simple-examples) notebook. It uses CrossBatchMemory to
+implement the momentum encoder queue, which means you can use any tuple loss,
+and any tuple miner to extract hard samples from the queue. ## Highlights of
+the rest of the library - For a convenient way to train your model, take a look
+at the [trainers](https://kevinmusgrave.github.io/pytorch-metric-learning/
+trainers/). - Want to test your model's accuracy on a dataset? Try the
+[testers](https://kevinmusgrave.github.io/pytorch-metric-learning/testers/). -
+To compute the accuracy of an embedding space directly, use
+[AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/
+accuracy_calculation/). If you're short of time and want a complete train/test
+workflow, check out the [example Google Colab notebooks](https://github.com/
+KevinMusgrave/pytorch-metric-learning/tree/master/examples). To learn more
+about all of the above, [see the documentation](https://
+kevinmusgrave.github.io/pytorch-metric-learning). ## Installation ### Required
+PyTorch version - ```pytorch-metric-learning >= v0.9.90``` requires ```torch >=
+1.6``` - ```pytorch-metric-learning < v0.9.90``` doesn't have a version
+requirement, but was tested with ```torch >= 1.2``` Other dependencies:
+```numpy, scikit-learn, tqdm, torchvision``` ### Pip ``` pip install pytorch-
+metric-learning ``` **To get the latest dev version**: ``` pip install pytorch-
+metric-learning --pre ``` **To install on Windows**: ``` pip install
+torch===1.6.0 torchvision===0.7.0 -f https://download.pytorch.org/whl/
+torch_stable.html pip install pytorch-metric-learning ``` **To install with
+evaluation and logging capabilities** (This will install the unofficial pypi
+version of faiss-gpu, plus record-keeper and tensorboard): ``` pip install
+pytorch-metric-learning[with-hooks] ``` **To install with evaluation and
+logging capabilities (CPU)** (This will install the unofficial pypi version of
+faiss-cpu, plus record-keeper and tensorboard): ``` pip install pytorch-metric-
+learning[with-hooks-cpu] ``` ### Conda ``` conda install -c conda-forge
+pytorch-metric-learning ``` **To use the testing module, you'll need faiss,
+which can be installed via conda as well. See the [installation instructions
+for faiss](https://github.com/facebookresearch/faiss/blob/master/INSTALL.md).**
+## Benchmark results See [powerful-benchmarker](https://github.com/
+KevinMusgrave/powerful-benchmarker/) to view benchmark results and to use the
+benchmarking tool. ## Development Development is done on the ```dev``` branch:
+``` git checkout dev ``` Unit tests can be run with the default ```unittest```
+library: ```bash python -m unittest discover ``` You can specify the test
+datatypes and test device as environment variables. For example, to test using
+float32 and float64 on the CPU: ```bash TEST_DTYPES=float32,float64
+TEST_DEVICE=cpu python -m unittest discover ``` To run a single test file
+instead of the entire test suite, specify the file name: ```bash python -
+m unittest tests/losses/test_angular_loss.py ``` Code is formatted using
+```black``` and ```isort```: ```bash pip install black isort ./format_code.sh
+``` ## Acknowledgements ### Contributors Thanks to the contributors who made
+pull requests! | Contributor | Highlights | | -- | -- | |[mlopezantequera]
+(https://github.com/mlopezantequera) | - Made the [testers](https://
+kevinmusgrave.github.io/pytorch-metric-learning/testers) work on any
 combination of query and reference sets
 - Made [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-
 learning/accuracy_calculation/) work with arbitrary label comparisons | |
-[cwkeam](https://github.com/cwkeam) | - [VICRegLoss](https://
-kevinmusgrave.github.io/pytorch-metric-learning/losses/#vicregloss)
+[cwkeam](https://github.com/cwkeam) | - [SelfSupervisedLoss](https://
+kevinmusgrave.github.io/pytorch-metric-learning/losses/#selfsupervisedloss)
+- [VICRegLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/
+#vicregloss)
 - Added mean reciprocal rank accuracy to [AccuracyCalculator](https://
-kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) | |
-[marijnl](https://github.com/marijnl)| - [BatchEasyHardMiner](https://
-kevinmusgrave.github.io/pytorch-metric-learning/miners/#batcheasyhardminer)
+kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/)
+- BaseLossWrapper| |[marijnl](https://github.com/marijnl)| -
+[BatchEasyHardMiner](https://kevinmusgrave.github.io/pytorch-metric-learning/
+miners/#batcheasyhardminer)
 - [TwoStreamMetricLoss](https://kevinmusgrave.github.io/pytorch-metric-
 learning/trainers/#twostreammetricloss)
 - [GlobalTwoStreamEmbeddingSpaceTester](https://kevinmusgrave.github.io/
 pytorch-metric-learning/testers/#globaltwostreamembeddingspacetester)
 - [Example using trainers.TwoStreamMetricLoss](https://github.com/
 KevinMusgrave/pytorch-metric-learning/blob/master/examples/notebooks/
 TwoStreamMetricLoss.ipynb) | | [chingisooinar](https://github.com/
@@ -146,15 +151,15 @@
 pytorch-metric-learning/losses/#subcenterarcfaceloss) | | [elias-ramzi](https:/
 /github.com/elias-ramzi) | [HierarchicalSampler](https://
 kevinmusgrave.github.io/pytorch-metric-learning/samplers/#hierarchicalsampler)
 | | [fjsj](https://github.com/fjsj) | [SupConLoss](https://
 kevinmusgrave.github.io/pytorch-metric-learning/losses/#supconloss) | |
 [AlenUbuntu](https://github.com/AlenUbuntu) | [CircleLoss](https://
 kevinmusgrave.github.io/pytorch-metric-learning/losses/#circleloss) | |
-[interestingzhuo](https://github.com/interestingzhuo) | [**PNPLoss**](https://
+[interestingzhuo](https://github.com/interestingzhuo) | [PNPLoss](https://
 kevinmusgrave.github.io/pytorch-metric-learning/losses/#pnploss) | | [wconnell]
 (https://github.com/wconnell) | [Learning a scRNAseq Metric Embedding](https://
 github.com/KevinMusgrave/pytorch-metric-learning/blob/master/examples/
 notebooks/scRNAseq_MetricEmbedding.ipynb) | | [AlexSchuy](https://github.com/
 AlexSchuy) | optimized
 ```utils.loss_and_miner_utils.get_random_triplet_indices``` | | [JohnGiorgi]
 (https://github.com/JohnGiorgi) | ```all_gather``` in [utils.distributed]
@@ -173,30 +178,30 @@
 ElisonSherton) | Fixed an edge case in ArcFaceLoss. | | [z1w](https://
 github.com/z1w) | | | [thinline72](https://github.com/thinline72) | | |
 [tpanum](https://github.com/tpanum) | | | [fralik](https://github.com/fralik) |
 | | [joaqo](https://github.com/joaqo) | | | [JoOkuma](https://github.com/
 JoOkuma) | | | [gkouros](https://github.com/gkouros) | | | [yutanakamura-tky]
 (https://github.com/yutanakamura-tky) | | | [KinglittleQ](https://github.com/
 KinglittleQ) | | | [martin0258](https://github.com/martin0258) | | |
-[michaeldeyzel](https://github.com/michaeldeyzel) | | ### Facebook AI Thank you
-to [Ser-Nam Lim](https://research.fb.com/people/lim-ser-nam/) at [Facebook AI]
-(https://ai.facebook.com/), and my research advisor, [Professor Serge Belongie]
-(https://vision.cornell.edu/se3/people/serge-belongie/). This project began
-during my internship at Facebook AI where I received valuable feedback from
-Ser-Nam, and his team of computer vision and machine learning engineers and
-research scientists. In particular, thanks to [Ashish Shah](https://
-www.linkedin.com/in/ashish217/) and [Austin Reiter](https://www.linkedin.com/
-in/austin-reiter-3962aa7/) for reviewing my code during its early stages of
-development. ### Open-source repos This library contains code that has been
-adapted and modified from the following great open-source repos: - https://
-github.com/bnu-wangxun/Deep_Metric - https://github.com/chaoyuaw/incubator-
-mxnet/blob/master/example/gluon/embedding_learning - https://github.com/
-facebookresearch/deepcluster - https://github.com/geonm/proxy-anchor-loss -
-https://github.com/idstcv/SoftTriple - https://github.com/kunhe/FastAP-metric-
-learning - https://github.com/ronekko/deep_metric_learning - https://
-github.com/tjddus9597/Proxy-Anchor-CVPR2020 - http://kaizhao.net/regularface
-### Logo Thanks to [Jeff Musgrave](https://www.designgenius.ca/) for designing
-the logo. ## Citing this library If you'd like to cite pytorch-metric-learning
-in your paper, you can use this bibtex: ```latex @article
-{Musgrave2020PyTorchML, title={PyTorch Metric Learning}, author={Kevin Musgrave
-and Serge J. Belongie and Ser-Nam Lim}, journal={ArXiv}, year={2020}, volume=
-{abs/2008.09164} } ```
+[michaeldeyzel](https://github.com/michaeldeyzel) | | | [HSinger04](https://
+github.com/HSinger04) | | ### Facebook AI Thank you to [Ser-Nam Lim](https://
+research.fb.com/people/lim-ser-nam/) at [Facebook AI](https://ai.facebook.com/
+), and my research advisor, [Professor Serge Belongie](https://
+vision.cornell.edu/se3/people/serge-belongie/). This project began during my
+internship at Facebook AI where I received valuable feedback from Ser-Nam, and
+his team of computer vision and machine learning engineers and research
+scientists. In particular, thanks to [Ashish Shah](https://www.linkedin.com/in/
+ashish217/) and [Austin Reiter](https://www.linkedin.com/in/austin-reiter-
+3962aa7/) for reviewing my code during its early stages of development. ###
+Open-source repos This library contains code that has been adapted and modified
+from the following great open-source repos: - https://github.com/bnu-wangxun/
+Deep_Metric - https://github.com/chaoyuaw/incubator-mxnet/blob/master/example/
+gluon/embedding_learning - https://github.com/facebookresearch/deepcluster -
+https://github.com/geonm/proxy-anchor-loss - https://github.com/idstcv/
+SoftTriple - https://github.com/kunhe/FastAP-metric-learning - https://
+github.com/ronekko/deep_metric_learning - https://github.com/tjddus9597/Proxy-
+Anchor-CVPR2020 - http://kaizhao.net/regularface ### Logo Thanks to [Jeff
+Musgrave](https://www.designgenius.ca/) for designing the logo. ## Citing this
+library If you'd like to cite pytorch-metric-learning in your paper, you can
+use this bibtex: ```latex @article{Musgrave2020PyTorchML, title={PyTorch Metric
+Learning}, author={Kevin Musgrave and Serge J. Belongie and Ser-Nam Lim},
+journal={ArXiv}, year={2020}, volume={abs/2008.09164} } ```
```

### Comparing `pytorch-metric-learning-2.1.1/setup.py` & `pytorch-metric-learning-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/base_distance.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/base_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/batched_distance.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/batched_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/lp_distance.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/lp_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/snr_distance.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/snr_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/__init__.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/angular_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/angular_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/arcface_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/arcface_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/base_metric_loss_function.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/base_metric_loss_function.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/circle_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/circle_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/contrastive_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/cosface_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/cosface_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/cross_batch_memory.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/cross_batch_memory.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/fast_ap_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/fast_ap_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/generic_pair_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/generic_pair_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/instance_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/instance_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/intra_pair_variance_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/intra_pair_variance_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/large_margin_softmax_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/large_margin_softmax_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/lifted_structure_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/lifted_structure_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/margin_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/margin_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/mixins.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/mixins.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/multi_similarity_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/multi_similarity_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/multiple_losses.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/multiple_losses.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/n_pairs_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/n_pairs_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/nca_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/nca_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/normalized_softmax_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/normalized_softmax_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/ntxent_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/ntxent_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/pnp_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/pnp_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/proxy_anchor_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/proxy_anchor_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/proxy_losses.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/proxy_losses.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/self_supervised_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/self_supervised_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/soft_triple_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/soft_triple_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/subcenter_arcface_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/subcenter_arcface_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/supcon_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/supcon_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/triplet_margin_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/triplet_margin_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/tuplet_margin_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/tuplet_margin_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/vicreg_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/vicreg_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/__init__.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/angular_miner.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/angular_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/base_miner.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/base_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/batch_easy_hard_miner.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/batch_easy_hard_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/distance_weighted_miner.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/distance_weighted_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/hdc_miner.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/hdc_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/multi_similarity_miner.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/multi_similarity_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/pair_margin_miner.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/pair_margin_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/triplet_margin_miner.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/triplet_margin_miner.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,16 @@
         mat = self.distance(embeddings, ref_emb)
         ap_dist = mat[anchor_idx, positive_idx]
         an_dist = mat[anchor_idx, negative_idx]
         triplet_margin = (
             ap_dist - an_dist if self.distance.is_inverted else an_dist - ap_dist
         )
 
+        self.set_stats(ap_dist, an_dist, triplet_margin)
+
         if self.type_of_triplets == "easy":
             threshold_condition = triplet_margin > self.margin
         else:
             threshold_condition = triplet_margin <= self.margin
             if self.type_of_triplets == "hard":
                 threshold_condition &= triplet_margin <= 0
             elif self.type_of_triplets == "semihard":
```

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/uniform_histogram_miner.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/uniform_histogram_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/base_reducer.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/base_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/class_weighted_reducer.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/class_weighted_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/divisor_reducer.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/divisor_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/multiple_reducers.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/multiple_reducers.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/per_anchor_reducer.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/per_anchor_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/threshold_reducer.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/threshold_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/center_invariant_regularizer.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/center_invariant_regularizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/lp_regularizer.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/lp_regularizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/regular_face_regularizer.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/regular_face_regularizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/sparse_centers_regularizer.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/sparse_centers_regularizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/fixed_set_of_triplets.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/fixed_set_of_triplets.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/hierarchical_sampler.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/hierarchical_sampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import itertools
 from collections import defaultdict
 
 import torch
-from torch.utils.data.sampler import BatchSampler
+from torch.utils.data.sampler import Sampler
 
 from ..utils import common_functions as c_f
 
 
 # Inspired by
 # https://github.com/kunhe/Deep-Metric-Learning-Baselines/blob/master/datasets.py
-class HierarchicalSampler(BatchSampler):
+class HierarchicalSampler(Sampler):
     def __init__(
         self,
         labels,
         batch_size,
         samples_per_class,
         batches_per_super_tuple=4,
         super_classes_per_batch=2,
```

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/m_per_class_sampler.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/m_per_class_sampler.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/tuples_to_weights_sampler.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/tuples_to_weights_sampler.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/base_tester.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/base_tester.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/global_embedding_space.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/global_embedding_space.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/global_twostream_embedding_space.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/global_twostream_embedding_space.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/with_same_parent_label.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/with_same_parent_label.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/base_trainer.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/base_trainer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/cascaded_embeddings.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/cascaded_embeddings.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/deep_adversarial_metric_learning.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/deep_adversarial_metric_learning.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/metric_loss_only.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/metric_loss_only.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/train_with_classifier.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/train_with_classifier.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/twostream_metric_loss.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/twostream_metric_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/accuracy_calculator.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/accuracy_calculator.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/common_functions.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/common_functions.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/distributed.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/inference.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/inference.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/key_checker.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/key_checker.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/logging_presets.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/logging_presets.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/loss_and_miner_utils.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/loss_and_miner_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/loss_tracker.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/loss_tracker.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/module_with_records.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/module_with_records.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/module_with_records_and_reducer.py` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/module_with_records_and_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning.egg-info/PKG-INFO` & `pytorch-metric-learning-2.1.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: pytorch-metric-learning
-Version: 2.1.1
-Summary: The easiest way to use deep metric learning in your application. Modular, flexible, and extensible. Written in PyTorch.
-Home-page: https://github.com/KevinMusgrave/pytorch-metric-learning
-Author: Kevin Musgrave
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-Provides-Extra: with-hooks
-Provides-Extra: with-hooks-cpu
-Provides-Extra: docs
-Provides-Extra: dev
-License-File: LICENSE
-
 <h1>
 <a href="https://github.com/KevinMusgrave/pytorch-metric-learning">
 <img alt="PyTorch Metric Learning" src="https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/docs/imgs/Logo2.png">
 </a>
 </h1>
 
 <p align="center">
@@ -33,21 +14,22 @@
  <a href="https://anaconda.org/conda-forge/pytorch-metric-learning">
      <img alt="Anaconda version" src="https://img.shields.io/conda/v/conda-forge/pytorch-metric-learning?color=bright-green">
  </a>
 </p>
 
 ## News
 
-**January 16**: v1.7.0
-- Fixes an edge case in ArcFaceLoss. See the [release notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/v1.7.0).
-- Thanks to contributor [ElisonSherton](https://github.com/ElisonSherton).
-
-**September 3**: v1.6.0
-- `DistributedLossWrapper` and `DistributedMinerWrapper` now support `ref_emb` and `ref_labels`.
-- Thanks to contributor [NoTody](https://github.com/NoTody).
+**April 5**: v2.1.0
+- Added [PNPLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#pnploss)
+- Thanks to contributor [interestingzhuo](https://github.com/interestingzhuo).
+
+**January 29**: v2.0.0
+- Added SelfSupervisedLoss, plus various API improvements. See the [release notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/v2.0.0).
+- Thanks to contributor [cwkeam](https://github.com/cwkeam).
+
 
 ## Documentation
 - [**View the documentation here**](https://kevinmusgrave.github.io/pytorch-metric-learning/)
 - [**View the installation instructions here**](https://github.com/KevinMusgrave/pytorch-metric-learning#installation)
 - [**View the available losses, miners etc. here**](https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/CONTENTS.md) 
 
 
@@ -121,30 +103,26 @@
 
  - The loss will be computed using cosine similarity instead of Euclidean distance.
  - All triplet losses that are higher than 0.3 will be discarded.
  - The embeddings will be L2 regularized.  
 
 ### Using loss functions for unsupervised / self-supervised learning
 
-The TripletMarginLoss is an embedding-based or tuple-based loss. This means that internally, there is no real notion of "classes". Tuples (pairs or triplets) are formed at each iteration, based on the labels it receives. The labels don't have to represent classes. They simply need to indicate the positive and negative relationships between the embeddings. Thus, it is easy to use these loss functions for unsupervised or self-supervised learning. 
-
-For example, the code below is a simplified version of the augmentation strategy commonly used in self-supervision. The dataset does not come with any labels. Instead, the labels are created in the training loop, solely to indicate which embeddings are positive pairs.
+A `SelfSupervisedLoss` wrapper is provided for self-supervised learning:
 
 ```python
+from pytorch_metric_learning.losses import SelfSupervisedLoss
+loss_func = SelfSupervisedLoss(TripletMarginLoss())
+
 # your training for-loop
 for i, data in enumerate(dataloader):
 	optimizer.zero_grad()
 	embeddings = your_model(data)
 	augmented = your_model(your_augmentation(data))
-	labels = torch.arange(embeddings.size(0))
-
-	embeddings = torch.cat([embeddings, augmented], dim=0)
-	labels = torch.cat([labels, labels], dim=0)
-
-	loss = loss_func(embeddings, labels)
+	loss = loss_func(embeddings, augmented)
 	loss.backward()
 	optimizer.step()
 ```
 
 If you're interested in [MoCo](https://arxiv.org/pdf/1911.05722.pdf)-style self-supervision, take a look at the [MoCo on CIFAR10](https://github.com/KevinMusgrave/pytorch-metric-learning/tree/master/examples#simple-examples) notebook. It uses CrossBatchMemory to implement the momentum encoder queue, which means you can use any tuple loss, and any tuple miner to extract hard samples from the queue.
 
 
@@ -244,21 +222,21 @@
 
 ### Contributors
 Thanks to the contributors who made pull requests!
 
 | Contributor | Highlights |
 | -- | -- |
 |[mlopezantequera](https://github.com/mlopezantequera) | - Made the [testers](https://kevinmusgrave.github.io/pytorch-metric-learning/testers) work on any combination of query and reference sets <br/> - Made [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) work with arbitrary label comparisons |
-|[cwkeam](https://github.com/cwkeam) | - [VICRegLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#vicregloss) <br/> - Added mean reciprocal rank accuracy to [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) |
+|[cwkeam](https://github.com/cwkeam) | - [SelfSupervisedLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#selfsupervisedloss) <br/> - [VICRegLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#vicregloss) <br/> - Added mean reciprocal rank accuracy to [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) <br/> - BaseLossWrapper|
 |[marijnl](https://github.com/marijnl)| - [BatchEasyHardMiner](https://kevinmusgrave.github.io/pytorch-metric-learning/miners/#batcheasyhardminer) <br/> - [TwoStreamMetricLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/trainers/#twostreammetricloss) <br/> - [GlobalTwoStreamEmbeddingSpaceTester](https://kevinmusgrave.github.io/pytorch-metric-learning/testers/#globaltwostreamembeddingspacetester) <br/> - [Example using trainers.TwoStreamMetricLoss](https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/examples/notebooks/TwoStreamMetricLoss.ipynb) |
 | [chingisooinar](https://github.com/chingisooinar) | [SubCenterArcFaceLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#subcenterarcfaceloss) |
 | [elias-ramzi](https://github.com/elias-ramzi) | [HierarchicalSampler](https://kevinmusgrave.github.io/pytorch-metric-learning/samplers/#hierarchicalsampler) |
 | [fjsj](https://github.com/fjsj) | [SupConLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#supconloss) |
 | [AlenUbuntu](https://github.com/AlenUbuntu) | [CircleLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#circleloss) |
-| [interestingzhuo](https://github.com/interestingzhuo) | [**PNPLoss**](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#pnploss) |
+| [interestingzhuo](https://github.com/interestingzhuo) | [PNPLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#pnploss) |
 | [wconnell](https://github.com/wconnell) | [Learning a scRNAseq Metric Embedding](https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/examples/notebooks/scRNAseq_MetricEmbedding.ipynb) |
 | [AlexSchuy](https://github.com/AlexSchuy) | optimized ```utils.loss_and_miner_utils.get_random_triplet_indices``` |
 | [JohnGiorgi](https://github.com/JohnGiorgi) | ```all_gather``` in [utils.distributed](https://kevinmusgrave.github.io/pytorch-metric-learning/distributed) |
 | [Hummer12007](https://github.com/Hummer12007) | ```utils.key_checker``` |
 | [vltanh](https://github.com/vltanh) | Made ```InferenceModel.train_indexer``` accept datasets |
 | [btseytlin](https://github.com/btseytlin) | ```get_nearest_neighbors``` in [InferenceModel](https://kevinmusgrave.github.io/pytorch-metric-learning/inference_models) |
 | [mlw214](https://github.com/mlw214) | Added ```return_per_class``` to [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) |
@@ -272,14 +250,15 @@
 | [joaqo](https://github.com/joaqo) | |
 | [JoOkuma](https://github.com/JoOkuma) | |
 | [gkouros](https://github.com/gkouros) | |
 | [yutanakamura-tky](https://github.com/yutanakamura-tky) | |
 | [KinglittleQ](https://github.com/KinglittleQ) | |
 | [martin0258](https://github.com/martin0258) | |
 | [michaeldeyzel](https://github.com/michaeldeyzel) | |
+| [HSinger04](https://github.com/HSinger04) | |
 
 
 
 ### Facebook AI
 Thank you to [Ser-Nam Lim](https://research.fb.com/people/lim-ser-nam/) at [Facebook AI](https://ai.facebook.com/), and my research advisor, [Professor Serge Belongie](https://vision.cornell.edu/se3/people/serge-belongie/). This project began during my internship at Facebook AI where I received valuable feedback from Ser-Nam, and his team of computer vision and machine learning engineers and research scientists. In particular, thanks to [Ashish Shah](https://www.linkedin.com/in/ashish217/) and [Austin Reiter](https://www.linkedin.com/in/austin-reiter-3962aa7/) for reviewing my code during its early stages of development.
 
 ### Open-source repos
@@ -304,9 +283,7 @@
   title={PyTorch Metric Learning},
   author={Kevin Musgrave and Serge J. Belongie and Ser-Nam Lim},
   journal={ArXiv},
   year={2020},
   volume={abs/2008.09164}
 }
 ```
-
-
```

#### html2text {}

```diff
@@ -1,34 +1,26 @@
-Metadata-Version: 2.1 Name: pytorch-metric-learning Version: 2.1.1 Summary: The
-easiest way to use deep metric learning in your application. Modular, flexible,
-and extensible. Written in PyTorch. Home-page: https://github.com/
-KevinMusgrave/pytorch-metric-learning Author: Kevin Musgrave License: UNKNOWN
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.0 Description-Content-Type: text/markdown
-Provides-Extra: with-hooks Provides-Extra: with-hooks-cpu Provides-Extra: docs
-Provides-Extra: dev License-File: LICENSE
 ****** [PyTorch_Metric_Learning] ******
                        [PyPi_version] [Anaconda_version]
-## News **January 16**: v1.7.0 - Fixes an edge case in ArcFaceLoss. See the
-[release notes](https://github.com/KevinMusgrave/pytorch-metric-learning/
-releases/tag/v1.7.0). - Thanks to contributor [ElisonSherton](https://
-github.com/ElisonSherton). **September 3**: v1.6.0 - `DistributedLossWrapper`
-and `DistributedMinerWrapper` now support `ref_emb` and `ref_labels`. - Thanks
-to contributor [NoTody](https://github.com/NoTody). ## Documentation - [**View
-the documentation here**](https://kevinmusgrave.github.io/pytorch-metric-
-learning/) - [**View the installation instructions here**](https://github.com/
-KevinMusgrave/pytorch-metric-learning#installation) - [**View the available
-losses, miners etc. here**](https://github.com/KevinMusgrave/pytorch-metric-
-learning/blob/master/CONTENTS.md) ## Google Colab Examples See the [examples
-folder](https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/
-examples/README.md) for notebooks you can download or run on Google Colab. ##
-PyTorch Metric Learning Overview This library contains 9 modules, each of which
-can be used independently within your existing codebase, or combined together
-for a complete train/test workflow. ![high_level_module_overview](docs/imgs/
+## News **April 5**: v2.1.0 - Added [PNPLoss](https://kevinmusgrave.github.io/
+pytorch-metric-learning/losses/#pnploss) - Thanks to contributor
+[interestingzhuo](https://github.com/interestingzhuo). **January 29**: v2.0.0 -
+Added SelfSupervisedLoss, plus various API improvements. See the [release
+notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/
+v2.0.0). - Thanks to contributor [cwkeam](https://github.com/cwkeam). ##
+Documentation - [**View the documentation here**](https://
+kevinmusgrave.github.io/pytorch-metric-learning/) - [**View the installation
+instructions here**](https://github.com/KevinMusgrave/pytorch-metric-
+learning#installation) - [**View the available losses, miners etc. here**]
+(https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/
+CONTENTS.md) ## Google Colab Examples See the [examples folder](https://
+github.com/KevinMusgrave/pytorch-metric-learning/blob/master/examples/
+README.md) for notebooks you can download or run on Google Colab. ## PyTorch
+Metric Learning Overview This library contains 9 modules, each of which can be
+used independently within your existing codebase, or combined together for a
+complete train/test workflow. ![high_level_module_overview](docs/imgs/
 high_level_module_overview.png) ## How loss functions work ### Using losses and
 miners in your training loop Letâs initialize a plain [TripletMarginLoss]
 (https://kevinmusgrave.github.io/pytorch-metric-learning/losses/
 #tripletmarginloss): ```python from pytorch_metric_learning import losses
 loss_func = losses.TripletMarginLoss() ``` To compute the loss in your training
 loop, pass in the embeddings computed by your model, and the corresponding
 labels. The embeddings should have size (N, embedding_size), and the labels
@@ -68,86 +60,81 @@
 from pytorch_metric_learning.regularizers import LpRegularizer from
 pytorch_metric_learning import losses loss_func = losses.TripletMarginLoss
 (distance = CosineSimilarity(), reducer = ThresholdReducer(high=0.3),
 embedding_regularizer = LpRegularizer()) ``` This customized triplet loss has
 the following properties: - The loss will be computed using cosine similarity
 instead of Euclidean distance. - All triplet losses that are higher than 0.3
 will be discarded. - The embeddings will be L2 regularized. ### Using loss
-functions for unsupervised / self-supervised learning The TripletMarginLoss is
-an embedding-based or tuple-based loss. This means that internally, there is no
-real notion of "classes". Tuples (pairs or triplets) are formed at each
-iteration, based on the labels it receives. The labels don't have to represent
-classes. They simply need to indicate the positive and negative relationships
-between the embeddings. Thus, it is easy to use these loss functions for
-unsupervised or self-supervised learning. For example, the code below is a
-simplified version of the augmentation strategy commonly used in self-
-supervision. The dataset does not come with any labels. Instead, the labels are
-created in the training loop, solely to indicate which embeddings are positive
-pairs. ```python # your training for-loop for i, data in enumerate(dataloader):
-optimizer.zero_grad() embeddings = your_model(data) augmented = your_model
-(your_augmentation(data)) labels = torch.arange(embeddings.size(0)) embeddings
-= torch.cat([embeddings, augmented], dim=0) labels = torch.cat([labels,
-labels], dim=0) loss = loss_func(embeddings, labels) loss.backward()
-optimizer.step() ``` If you're interested in [MoCo](https://arxiv.org/pdf/
-1911.05722.pdf)-style self-supervision, take a look at the [MoCo on CIFAR10]
-(https://github.com/KevinMusgrave/pytorch-metric-learning/tree/master/
-examples#simple-examples) notebook. It uses CrossBatchMemory to implement the
-momentum encoder queue, which means you can use any tuple loss, and any tuple
-miner to extract hard samples from the queue. ## Highlights of the rest of the
-library - For a convenient way to train your model, take a look at the
-[trainers](https://kevinmusgrave.github.io/pytorch-metric-learning/trainers/).
-- Want to test your model's accuracy on a dataset? Try the [testers](https://
-kevinmusgrave.github.io/pytorch-metric-learning/testers/). - To compute the
-accuracy of an embedding space directly, use [AccuracyCalculator](https://
-kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/). If
-you're short of time and want a complete train/test workflow, check out the
-[example Google Colab notebooks](https://github.com/KevinMusgrave/pytorch-
-metric-learning/tree/master/examples). To learn more about all of the above,
-[see the documentation](https://kevinmusgrave.github.io/pytorch-metric-
-learning). ## Installation ### Required PyTorch version - ```pytorch-metric-
-learning >= v0.9.90``` requires ```torch >= 1.6``` - ```pytorch-metric-learning
-< v0.9.90``` doesn't have a version requirement, but was tested with ```torch
->= 1.2``` Other dependencies: ```numpy, scikit-learn, tqdm, torchvision``` ###
-Pip ``` pip install pytorch-metric-learning ``` **To get the latest dev
-version**: ``` pip install pytorch-metric-learning --pre ``` **To install on
-Windows**: ``` pip install torch===1.6.0 torchvision===0.7.0 -f https://
-download.pytorch.org/whl/torch_stable.html pip install pytorch-metric-learning
-``` **To install with evaluation and logging capabilities** (This will install
-the unofficial pypi version of faiss-gpu, plus record-keeper and tensorboard):
-``` pip install pytorch-metric-learning[with-hooks] ``` **To install with
-evaluation and logging capabilities (CPU)** (This will install the unofficial
-pypi version of faiss-cpu, plus record-keeper and tensorboard): ``` pip install
-pytorch-metric-learning[with-hooks-cpu] ``` ### Conda ``` conda install -
-c conda-forge pytorch-metric-learning ``` **To use the testing module, you'll
-need faiss, which can be installed via conda as well. See the [installation
-instructions for faiss](https://github.com/facebookresearch/faiss/blob/master/
-INSTALL.md).**  ## Benchmark results See [powerful-benchmarker](https://
-github.com/KevinMusgrave/powerful-benchmarker/) to view benchmark results and
-to use the benchmarking tool. ## Development Development is done on the
-```dev``` branch: ``` git checkout dev ``` Unit tests can be run with the
-default ```unittest``` library: ```bash python -m unittest discover ``` You can
-specify the test datatypes and test device as environment variables. For
-example, to test using float32 and float64 on the CPU: ```bash
-TEST_DTYPES=float32,float64 TEST_DEVICE=cpu python -m unittest discover ``` To
-run a single test file instead of the entire test suite, specify the file name:
-```bash python -m unittest tests/losses/test_angular_loss.py ``` Code is
-formatted using ```black``` and ```isort```: ```bash pip install black isort ./
-format_code.sh ``` ## Acknowledgements ### Contributors Thanks to the
-contributors who made pull requests! | Contributor | Highlights | | -- | -- | |
-[mlopezantequera](https://github.com/mlopezantequera) | - Made the [testers]
-(https://kevinmusgrave.github.io/pytorch-metric-learning/testers) work on any
+functions for unsupervised / self-supervised learning A `SelfSupervisedLoss`
+wrapper is provided for self-supervised learning: ```python from
+pytorch_metric_learning.losses import SelfSupervisedLoss loss_func =
+SelfSupervisedLoss(TripletMarginLoss()) # your training for-loop for i, data in
+enumerate(dataloader): optimizer.zero_grad() embeddings = your_model(data)
+augmented = your_model(your_augmentation(data)) loss = loss_func(embeddings,
+augmented) loss.backward() optimizer.step() ``` If you're interested in [MoCo]
+(https://arxiv.org/pdf/1911.05722.pdf)-style self-supervision, take a look at
+the [MoCo on CIFAR10](https://github.com/KevinMusgrave/pytorch-metric-learning/
+tree/master/examples#simple-examples) notebook. It uses CrossBatchMemory to
+implement the momentum encoder queue, which means you can use any tuple loss,
+and any tuple miner to extract hard samples from the queue. ## Highlights of
+the rest of the library - For a convenient way to train your model, take a look
+at the [trainers](https://kevinmusgrave.github.io/pytorch-metric-learning/
+trainers/). - Want to test your model's accuracy on a dataset? Try the
+[testers](https://kevinmusgrave.github.io/pytorch-metric-learning/testers/). -
+To compute the accuracy of an embedding space directly, use
+[AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/
+accuracy_calculation/). If you're short of time and want a complete train/test
+workflow, check out the [example Google Colab notebooks](https://github.com/
+KevinMusgrave/pytorch-metric-learning/tree/master/examples). To learn more
+about all of the above, [see the documentation](https://
+kevinmusgrave.github.io/pytorch-metric-learning). ## Installation ### Required
+PyTorch version - ```pytorch-metric-learning >= v0.9.90``` requires ```torch >=
+1.6``` - ```pytorch-metric-learning < v0.9.90``` doesn't have a version
+requirement, but was tested with ```torch >= 1.2``` Other dependencies:
+```numpy, scikit-learn, tqdm, torchvision``` ### Pip ``` pip install pytorch-
+metric-learning ``` **To get the latest dev version**: ``` pip install pytorch-
+metric-learning --pre ``` **To install on Windows**: ``` pip install
+torch===1.6.0 torchvision===0.7.0 -f https://download.pytorch.org/whl/
+torch_stable.html pip install pytorch-metric-learning ``` **To install with
+evaluation and logging capabilities** (This will install the unofficial pypi
+version of faiss-gpu, plus record-keeper and tensorboard): ``` pip install
+pytorch-metric-learning[with-hooks] ``` **To install with evaluation and
+logging capabilities (CPU)** (This will install the unofficial pypi version of
+faiss-cpu, plus record-keeper and tensorboard): ``` pip install pytorch-metric-
+learning[with-hooks-cpu] ``` ### Conda ``` conda install -c conda-forge
+pytorch-metric-learning ``` **To use the testing module, you'll need faiss,
+which can be installed via conda as well. See the [installation instructions
+for faiss](https://github.com/facebookresearch/faiss/blob/master/INSTALL.md).**
+## Benchmark results See [powerful-benchmarker](https://github.com/
+KevinMusgrave/powerful-benchmarker/) to view benchmark results and to use the
+benchmarking tool. ## Development Development is done on the ```dev``` branch:
+``` git checkout dev ``` Unit tests can be run with the default ```unittest```
+library: ```bash python -m unittest discover ``` You can specify the test
+datatypes and test device as environment variables. For example, to test using
+float32 and float64 on the CPU: ```bash TEST_DTYPES=float32,float64
+TEST_DEVICE=cpu python -m unittest discover ``` To run a single test file
+instead of the entire test suite, specify the file name: ```bash python -
+m unittest tests/losses/test_angular_loss.py ``` Code is formatted using
+```black``` and ```isort```: ```bash pip install black isort ./format_code.sh
+``` ## Acknowledgements ### Contributors Thanks to the contributors who made
+pull requests! | Contributor | Highlights | | -- | -- | |[mlopezantequera]
+(https://github.com/mlopezantequera) | - Made the [testers](https://
+kevinmusgrave.github.io/pytorch-metric-learning/testers) work on any
 combination of query and reference sets
 - Made [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-
 learning/accuracy_calculation/) work with arbitrary label comparisons | |
-[cwkeam](https://github.com/cwkeam) | - [VICRegLoss](https://
-kevinmusgrave.github.io/pytorch-metric-learning/losses/#vicregloss)
+[cwkeam](https://github.com/cwkeam) | - [SelfSupervisedLoss](https://
+kevinmusgrave.github.io/pytorch-metric-learning/losses/#selfsupervisedloss)
+- [VICRegLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/
+#vicregloss)
 - Added mean reciprocal rank accuracy to [AccuracyCalculator](https://
-kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) | |
-[marijnl](https://github.com/marijnl)| - [BatchEasyHardMiner](https://
-kevinmusgrave.github.io/pytorch-metric-learning/miners/#batcheasyhardminer)
+kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/)
+- BaseLossWrapper| |[marijnl](https://github.com/marijnl)| -
+[BatchEasyHardMiner](https://kevinmusgrave.github.io/pytorch-metric-learning/
+miners/#batcheasyhardminer)
 - [TwoStreamMetricLoss](https://kevinmusgrave.github.io/pytorch-metric-
 learning/trainers/#twostreammetricloss)
 - [GlobalTwoStreamEmbeddingSpaceTester](https://kevinmusgrave.github.io/
 pytorch-metric-learning/testers/#globaltwostreamembeddingspacetester)
 - [Example using trainers.TwoStreamMetricLoss](https://github.com/
 KevinMusgrave/pytorch-metric-learning/blob/master/examples/notebooks/
 TwoStreamMetricLoss.ipynb) | | [chingisooinar](https://github.com/
@@ -155,15 +142,15 @@
 pytorch-metric-learning/losses/#subcenterarcfaceloss) | | [elias-ramzi](https:/
 /github.com/elias-ramzi) | [HierarchicalSampler](https://
 kevinmusgrave.github.io/pytorch-metric-learning/samplers/#hierarchicalsampler)
 | | [fjsj](https://github.com/fjsj) | [SupConLoss](https://
 kevinmusgrave.github.io/pytorch-metric-learning/losses/#supconloss) | |
 [AlenUbuntu](https://github.com/AlenUbuntu) | [CircleLoss](https://
 kevinmusgrave.github.io/pytorch-metric-learning/losses/#circleloss) | |
-[interestingzhuo](https://github.com/interestingzhuo) | [**PNPLoss**](https://
+[interestingzhuo](https://github.com/interestingzhuo) | [PNPLoss](https://
 kevinmusgrave.github.io/pytorch-metric-learning/losses/#pnploss) | | [wconnell]
 (https://github.com/wconnell) | [Learning a scRNAseq Metric Embedding](https://
 github.com/KevinMusgrave/pytorch-metric-learning/blob/master/examples/
 notebooks/scRNAseq_MetricEmbedding.ipynb) | | [AlexSchuy](https://github.com/
 AlexSchuy) | optimized
 ```utils.loss_and_miner_utils.get_random_triplet_indices``` | | [JohnGiorgi]
 (https://github.com/JohnGiorgi) | ```all_gather``` in [utils.distributed]
@@ -182,30 +169,30 @@
 ElisonSherton) | Fixed an edge case in ArcFaceLoss. | | [z1w](https://
 github.com/z1w) | | | [thinline72](https://github.com/thinline72) | | |
 [tpanum](https://github.com/tpanum) | | | [fralik](https://github.com/fralik) |
 | | [joaqo](https://github.com/joaqo) | | | [JoOkuma](https://github.com/
 JoOkuma) | | | [gkouros](https://github.com/gkouros) | | | [yutanakamura-tky]
 (https://github.com/yutanakamura-tky) | | | [KinglittleQ](https://github.com/
 KinglittleQ) | | | [martin0258](https://github.com/martin0258) | | |
-[michaeldeyzel](https://github.com/michaeldeyzel) | | ### Facebook AI Thank you
-to [Ser-Nam Lim](https://research.fb.com/people/lim-ser-nam/) at [Facebook AI]
-(https://ai.facebook.com/), and my research advisor, [Professor Serge Belongie]
-(https://vision.cornell.edu/se3/people/serge-belongie/). This project began
-during my internship at Facebook AI where I received valuable feedback from
-Ser-Nam, and his team of computer vision and machine learning engineers and
-research scientists. In particular, thanks to [Ashish Shah](https://
-www.linkedin.com/in/ashish217/) and [Austin Reiter](https://www.linkedin.com/
-in/austin-reiter-3962aa7/) for reviewing my code during its early stages of
-development. ### Open-source repos This library contains code that has been
-adapted and modified from the following great open-source repos: - https://
-github.com/bnu-wangxun/Deep_Metric - https://github.com/chaoyuaw/incubator-
-mxnet/blob/master/example/gluon/embedding_learning - https://github.com/
-facebookresearch/deepcluster - https://github.com/geonm/proxy-anchor-loss -
-https://github.com/idstcv/SoftTriple - https://github.com/kunhe/FastAP-metric-
-learning - https://github.com/ronekko/deep_metric_learning - https://
-github.com/tjddus9597/Proxy-Anchor-CVPR2020 - http://kaizhao.net/regularface
-### Logo Thanks to [Jeff Musgrave](https://www.designgenius.ca/) for designing
-the logo. ## Citing this library If you'd like to cite pytorch-metric-learning
-in your paper, you can use this bibtex: ```latex @article
-{Musgrave2020PyTorchML, title={PyTorch Metric Learning}, author={Kevin Musgrave
-and Serge J. Belongie and Ser-Nam Lim}, journal={ArXiv}, year={2020}, volume=
-{abs/2008.09164} } ```
+[michaeldeyzel](https://github.com/michaeldeyzel) | | | [HSinger04](https://
+github.com/HSinger04) | | ### Facebook AI Thank you to [Ser-Nam Lim](https://
+research.fb.com/people/lim-ser-nam/) at [Facebook AI](https://ai.facebook.com/
+), and my research advisor, [Professor Serge Belongie](https://
+vision.cornell.edu/se3/people/serge-belongie/). This project began during my
+internship at Facebook AI where I received valuable feedback from Ser-Nam, and
+his team of computer vision and machine learning engineers and research
+scientists. In particular, thanks to [Ashish Shah](https://www.linkedin.com/in/
+ashish217/) and [Austin Reiter](https://www.linkedin.com/in/austin-reiter-
+3962aa7/) for reviewing my code during its early stages of development. ###
+Open-source repos This library contains code that has been adapted and modified
+from the following great open-source repos: - https://github.com/bnu-wangxun/
+Deep_Metric - https://github.com/chaoyuaw/incubator-mxnet/blob/master/example/
+gluon/embedding_learning - https://github.com/facebookresearch/deepcluster -
+https://github.com/geonm/proxy-anchor-loss - https://github.com/idstcv/
+SoftTriple - https://github.com/kunhe/FastAP-metric-learning - https://
+github.com/ronekko/deep_metric_learning - https://github.com/tjddus9597/Proxy-
+Anchor-CVPR2020 - http://kaizhao.net/regularface ### Logo Thanks to [Jeff
+Musgrave](https://www.designgenius.ca/) for designing the logo. ## Citing this
+library If you'd like to cite pytorch-metric-learning in your paper, you can
+use this bibtex: ```latex @article{Musgrave2020PyTorchML, title={PyTorch Metric
+Learning}, author={Kevin Musgrave and Serge J. Belongie and Ser-Nam Lim},
+journal={ArXiv}, year={2020}, volume={abs/2008.09164} } ```
```

### Comparing `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning.egg-info/SOURCES.txt` & `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

