# Comparing `tmp/troubleshooter-1.0.7.tar.gz` & `tmp/troubleshooter-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/troubleshooter-1.0.7.tar", last modified: Thu Apr 27 11:50:31 2023, max compression
+gzip compressed data, was "dist/troubleshooter-1.0.8.tar", last modified: Sat May 27 01:52:00 2023, max compression
```

## Comparing `troubleshooter-1.0.7.tar` & `troubleshooter-1.0.8.tar`

### file list

```diff
@@ -1,80 +1,96 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/
--rwxrwxrwx   0 root         (0) root         (0)    11357 2023-04-19 06:32:30.000000 troubleshooter-1.0.7/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      472 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)    24285 2023-04-25 02:43:53.000000 troubleshooter-1.0.7/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3997 2023-04-27 11:38:56.000000 troubleshooter-1.0.7/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/tests/
--rwxrwxrwx   0 root         (0) root         (0)      668 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/tests/diff_handler/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/diff_handler/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      440 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/diff_handler/test_compare.py
--rwxrwxrwx   0 root         (0) root         (0)    12415 2023-04-27 09:26:12.000000 troubleshooter-1.0.7/tests/diff_handler/test_migrator.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/tests/proposer/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/tests/proposer/1_9/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/1_9/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3537 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/1_9/test_compile.py
--rwxrwxrwx   0 root         (0) root         (0)      482 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/1_9/test_ops.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/tests/proposer/master/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/master/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7485 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/master/test_ascend_vm.py
--rwxrwxrwx   0 root         (0) root         (0)    14663 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/master/test_compile.py
--rwxrwxrwx   0 root         (0) root         (0)     9667 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/master/test_dataset.py
--rwxrwxrwx   0 root         (0) root         (0)     3163 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/master/test_me_front.py
--rwxrwxrwx   0 root         (0) root         (0)     4310 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/master/test_ops.py
--rwxrwxrwx   0 root         (0) root         (0)     2572 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/proposer/master/test_st_output.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/tests/tracker/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/tracker/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    10544 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/tracker/test_tracking.py
--rwxrwxrwx   0 root         (0) root         (0)     1395 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/tests/util.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/troubleshooter/
--rwxrwxrwx   0 root         (0) root         (0)     1415 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/troubleshooter/common/
--rwxrwxrwx   0 root         (0) root         (0)      668 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/common/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11931 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/common/format_msg.py
--rwxrwxrwx   0 root         (0) root         (0)     1511 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/common/ms_callback.py
--rwxrwxrwx   0 root         (0) root         (0)     3785 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/common/ms_utils.py
--rwxrwxrwx   0 root         (0) root         (0)     3958 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/common/util.py
--rwxrwxrwx   0 root         (0) root         (0)     3255 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/log.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/troubleshooter/migrator/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/migrator/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    14445 2023-04-27 03:46:52.000000 troubleshooter-1.0.7/troubleshooter/migrator/diff_handler.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/troubleshooter/migrator/mapping_relation/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/migrator/mapping_relation/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      801 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/migrator/mapping_relation/weight_adapter.py
--rwxrwxrwx   0 root         (0) root         (0)     1457 2023-04-20 12:28:36.000000 troubleshooter-1.0.7/troubleshooter/migrator/mapping_relation/weight_mapping_lib.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/troubleshooter/proposer/
--rwxrwxrwx   0 root         (0) root         (0)      793 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/
--rwxrwxrwx   0 root         (0) root         (0)     1834 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3238 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/base_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1529 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/compiler_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1544 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/compiler_scene_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1475 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/dataset_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1434 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/dataset_scene_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1239 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/default_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1678 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/front_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1472 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/operators_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1566 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/operators_scene_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     2561 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/allproposers/vm_proposer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/
--rwxrwxrwx   0 root         (0) root         (0)      669 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1747 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/common_exp_lib.py
--rwxrwxrwx   0 root         (0) root         (0)    36584 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/compiler_exp_lib.py
--rwxrwxrwx   0 root         (0) root         (0)    16638 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/dataset_exp_lib.py
--rwxrwxrwx   0 root         (0) root         (0)     6740 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/front_exp_lib.py
--rwxrwxrwx   0 root         (0) root         (0)    28384 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/operators_exp_lib.py
--rwxrwxrwx   0 root         (0) root         (0)    19783 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/vm_exp_lib.py
--rwxrwxrwx   0 root         (0) root         (0)     3425 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/proposal_action.py
--rwxrwxrwx   0 root         (0) root         (0)     2233 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/proposer/proposer_factory.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/troubleshooter/tracker/
--rwxrwxrwx   0 root         (0) root         (0)      770 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/tracker/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6630 2023-04-19 06:32:34.000000 troubleshooter-1.0.7/troubleshooter/tracker/tracker.py
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/troubleshooter/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-27 11:50:31.000000 troubleshooter-1.0.7/troubleshooter.egg-info/
--r-xr-xr-x   0 root         (0) root         (0)      472 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/troubleshooter.egg-info/PKG-INFO
--r-xr-xr-x   0 root         (0) root         (0)     2509 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/troubleshooter.egg-info/SOURCES.txt
--r-xr-xr-x   0 root         (0) root         (0)        1 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/troubleshooter.egg-info/dependency_links.txt
--r-xr-xr-x   0 root         (0) root         (0)       36 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/troubleshooter.egg-info/requires.txt
--r-xr-xr-x   0 root         (0) root         (0)       21 2023-04-27 11:50:30.000000 troubleshooter-1.0.7/troubleshooter.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:01.000000 troubleshooter-1.0.8/
+-rwxrwxrwx   0 root         (0) root         (0)    11357 2023-04-19 06:32:30.000000 troubleshooter-1.0.8/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      472 2023-05-27 01:52:01.000000 troubleshooter-1.0.8/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2224 2023-05-16 11:01:20.000000 troubleshooter-1.0.8/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-27 01:52:01.000000 troubleshooter-1.0.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     4001 2023-05-27 01:49:35.000000 troubleshooter-1.0.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/tests/
+-rwxrwxrwx   0 root         (0) root         (0)      668 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/tests/proposer/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/tests/proposer/1_9/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/1_9/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3537 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/1_9/test_compile.py
+-rwxrwxrwx   0 root         (0) root         (0)      482 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/1_9/test_ops.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/tests/proposer/master/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/master/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7485 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/master/test_ascend_vm.py
+-rwxrwxrwx   0 root         (0) root         (0)    14663 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/master/test_compile.py
+-rwxrwxrwx   0 root         (0) root         (0)     9667 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/master/test_dataset.py
+-rwxrwxrwx   0 root         (0) root         (0)     3163 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/master/test_me_front.py
+-rwxrwxrwx   0 root         (0) root         (0)     4310 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/master/test_ops.py
+-rwxrwxrwx   0 root         (0) root         (0)     2572 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/master/test_st_output.py
+-rwxrwxrwx   0 root         (0) root         (0)     1395 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/util.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/
+-rwxrwxrwx   0 root         (0) root         (0)     1432 2023-05-27 01:47:49.000000 troubleshooter-1.0.8/troubleshooter/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/common/
+-rwxrwxrwx   0 root         (0) root         (0)      893 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/common/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    13403 2023-05-26 01:41:35.000000 troubleshooter-1.0.8/troubleshooter/common/format_msg.py
+-rwxrwxrwx   0 root         (0) root         (0)     2071 2023-05-20 07:28:58.000000 troubleshooter-1.0.8/troubleshooter/common/framework_detection.py
+-rwxrwxrwx   0 root         (0) root         (0)     1515 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/common/ms_callback.py
+-rwxrwxrwx   0 root         (0) root         (0)     3789 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/common/ms_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     6105 2023-05-26 09:04:19.000000 troubleshooter-1.0.8/troubleshooter/common/util.py
+-rwxrwxrwx   0 root         (0) root         (0)     3259 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/log.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/migrator/
+-rwxrwxrwx   0 root         (0) root         (0)     1314 2023-05-27 01:47:49.000000 troubleshooter-1.0.8/troubleshooter/migrator/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6523 2023-05-27 01:47:49.000000 troubleshooter-1.0.8/troubleshooter/migrator/diff_handler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/migrator/mapping_relation/
+-rwxrwxrwx   0 root         (0) root         (0)      686 2023-05-20 07:28:58.000000 troubleshooter-1.0.8/troubleshooter/migrator/mapping_relation/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      805 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/migrator/mapping_relation/weight_adapter.py
+-rwxrwxrwx   0 root         (0) root         (0)     1461 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/migrator/mapping_relation/weight_mapping_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)    12331 2023-05-27 01:47:49.000000 troubleshooter-1.0.8/troubleshooter/migrator/net_diff_finder.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/migrator/save/
+-rwxrwxrwx   0 root         (0) root         (0)     1207 2023-05-24 09:27:50.000000 troubleshooter-1.0.8/troubleshooter/migrator/save/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3022 2023-05-26 00:34:42.000000 troubleshooter-1.0.8/troubleshooter/migrator/save/base_saver.py
+-rwxrwxrwx   0 root         (0) root         (0)     1786 2023-05-26 00:34:42.000000 troubleshooter-1.0.8/troubleshooter/migrator/save/mindspore_saver.py
+-rwxrwxrwx   0 root         (0) root         (0)     1646 2023-05-26 00:34:42.000000 troubleshooter-1.0.8/troubleshooter/migrator/save/torch_saver.py
+-rwxrwxrwx   0 root         (0) root         (0)     2706 2023-05-24 09:27:50.000000 troubleshooter-1.0.8/troubleshooter/migrator/save/unified_saver.py
+-rwxrwxrwx   0 root         (0) root         (0)    12874 2023-05-27 01:47:49.000000 troubleshooter-1.0.8/troubleshooter/migrator/weight_migrator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/proposer/
+-rwxrwxrwx   0 root         (0) root         (0)      797 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/
+-rwxrwxrwx   0 root         (0) root         (0)     1838 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3242 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/base_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1533 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/compiler_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1548 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/compiler_scene_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1479 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/dataset_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1438 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/dataset_scene_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1243 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/default_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1682 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/front_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1476 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/operators_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1570 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/operators_scene_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     2565 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/vm_proposer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/
+-rwxrwxrwx   0 root         (0) root         (0)      673 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1751 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/common_exp_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)    36588 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/compiler_exp_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)    16642 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/dataset_exp_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)     6744 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/front_exp_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)    28388 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/operators_exp_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)    19787 2023-05-20 07:26:22.000000 troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/vm_exp_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)     3429 2023-05-20 07:27:16.000000 troubleshooter-1.0.8/troubleshooter/proposer/proposal_action.py
+-rwxrwxrwx   0 root         (0) root         (0)     2237 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/proposer_factory.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/toolbox/
+-rwxrwxrwx   0 root         (0) root         (0)      776 2023-05-25 01:37:45.000000 troubleshooter-1.0.8/troubleshooter/toolbox/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/
+-rwxrwxrwx   0 root         (0) root         (0)      686 2023-05-20 07:28:58.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4161 2023-05-18 12:36:19.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/alexnet.py
+-rwxrwxrwx   0 root         (0) root         (0)     1762 2023-05-18 12:36:19.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/cell.py
+-rwxrwxrwx   0 root         (0) root         (0)     1128 2023-05-18 12:36:19.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/demo.py
+-rwxrwxrwx   0 root         (0) root         (0)    12883 2023-05-20 07:21:24.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/hooks.py
+-rwxrwxrwx   0 root         (0) root         (0)     2557 2023-05-24 09:27:50.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/initialize.py
+-rwxrwxrwx   0 root         (0) root         (0)     8212 2023-05-18 12:36:19.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     1950 2023-05-18 12:36:19.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/wrap_functional.py
+-rwxrwxrwx   0 root         (0) root         (0)     2131 2023-05-20 07:21:24.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/wrap_nn.py
+-rwxrwxrwx   0 root         (0) root         (0)     1890 2023-05-18 12:36:19.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/wrap_tensor.py
+-rwxrwxrwx   0 root         (0) root         (0)     2803 2023-05-26 10:02:37.000000 troubleshooter-1.0.8/troubleshooter/toolbox/widget_pocket.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/tracker/
+-rwxrwxrwx   0 root         (0) root         (0)      774 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/tracker/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6685 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/tracker/tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/troubleshooter/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter.egg-info/
+-r-xr-xr-x   0 root         (0) root         (0)      472 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/troubleshooter.egg-info/PKG-INFO
+-r-xr-xr-x   0 root         (0) root         (0)     3174 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/troubleshooter.egg-info/SOURCES.txt
+-r-xr-xr-x   0 root         (0) root         (0)        1 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/troubleshooter.egg-info/dependency_links.txt
+-r-xr-xr-x   0 root         (0) root         (0)       36 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/troubleshooter.egg-info/requires.txt
+-r-xr-xr-x   0 root         (0) root         (0)       21 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/troubleshooter.egg-info/top_level.txt
```

### Comparing `troubleshooter-1.0.7/LICENSE` & `troubleshooter-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.7/setup.py` & `troubleshooter-1.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -20,15 +20,15 @@
 import shutil
 import subprocess
 from setuptools import find_packages
 from setuptools import setup
 from setuptools.command.egg_info import egg_info
 from setuptools.command.build_py import build_py
 
-version = '1.0.7'
+version = '1.0.8'
 cur_dir = os.path.dirname(os.path.realpath(__file__))
 pkg_dir = os.path.join(cur_dir, 'build')
 
 
 def clean():
     """clean"""
     def readonly_handler(func, path, execinfo):
```

### Comparing `troubleshooter-1.0.7/tests/__init__.py` & `troubleshooter-1.0.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.7/tests/proposer/1_9/test_compile.py` & `troubleshooter-1.0.8/tests/proposer/1_9/test_compile.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.7/tests/proposer/master/test_ascend_vm.py` & `troubleshooter-1.0.8/tests/proposer/master/test_ascend_vm.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.7/tests/proposer/master/test_compile.py` & `troubleshooter-1.0.8/tests/proposer/master/test_compile.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.7/tests/proposer/master/test_dataset.py` & `troubleshooter-1.0.8/tests/proposer/master/test_dataset.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.7/tests/proposer/master/test_me_front.py` & `troubleshooter-1.0.8/tests/proposer/master/test_me_front.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.7/tests/proposer/master/test_ops.py` & `troubleshooter-1.0.8/tests/proposer/master/test_ops.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.7/tests/proposer/master/test_st_output.py` & `troubleshooter-1.0.8/tests/proposer/master/test_st_output.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.7/tests/util.py` & `troubleshooter-1.0.8/tests/util.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.7/troubleshooter/__init__.py` & `troubleshooter-1.0.8/troubleshooter/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,17 +14,17 @@
 # ============================================================================
 
 """
 TroubleShooter Module Introduction.
 
 This module provides Python APIs to shoot trouble of MindSpore neural networks.
 Users can import the proposal, initialize the ProposalAction object to start analyse,
-and use @proposal() to analyse the Traceback error message .
+and use @proposal() to analyse the Traceback error message.
 Users can import the snooping, initialize the Snooper object to start debug,
 and use @snooping(...) to print the running result information of echo line code of neural networks.
 """
-
-from .migrator.diff_handler import TensorRecorder as tensor_recorder
-from .migrator.diff_handler import DifferenceFinder as diff_finder
-from .migrator.diff_handler import WeightMigrator as weight_migrator
-from .proposer import ProposalAction as proposal
-from .tracker import Tracker as tracking
+from __future__ import absolute_import
+from troubleshooter.common import FRAMEWORK_TYPE
+from troubleshooter import common, migrator, proposer, tracker
+from troubleshooter.migrator import save
+from troubleshooter.proposer import ProposalAction as proposal
+from troubleshooter.tracker import Tracker as tracking
```

### Comparing `troubleshooter-1.0.7/troubleshooter/common/__init__.py` & `troubleshooter-1.0.8/troubleshooter/tracker/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
+"""Proposer for profiler."""
+from troubleshooter.tracker.tracker import Tracker
+__all__ = ["Tracker"]
```

### Comparing `troubleshooter-1.0.7/troubleshooter/common/format_msg.py` & `troubleshooter-1.0.8/troubleshooter/common/format_msg.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -44,73 +44,125 @@
 }
 
 
 def _add_row(x, item, message, width=TABLE_WIDTH, break_long_words=False, break_on_hyphens=False):
     if message is None:
         return
     item_cn = _item_to_cn.get(item)
-    format_message = _format_str_length(message) if os.linesep in message else message
+    format_message = _format_str_length(
+        message) if os.linesep in message else message
     x.add_row([item_cn, fill(format_message, width=width, break_long_words=break_long_words,
                              break_on_hyphens=break_on_hyphens)])
 
 
-def print_weight_compare_result(result_list, print_type=1):
+def print_weight_compare_result(result_list, print_type=1, **kwargs):
+    # 0 Do not print
+    # Print All
+    # print False
+    if print_type == 0:
+        return
+    title = kwargs.get('title', None)
+    field_names = kwargs.get('field_names', None)
     x = PrettyTable()
-    x.title = 'The list of comparison results'
-    x.field_names = ["Parameter name of input ckpt", "Parameter name of converted ckpt", "Whether shape are equal", "Parameter shape of input ckpt", "Parameter shape of converted ckpt"]
+    if title is None:
+        x.title = 'The list of comparison results for shapes'
+    else:
+        x.title = title
+
+    if field_names is None:
+        x.field_names = ["Parameter name of original ckpt", "Parameter name of target ckpt", "Whether shape are equal",
+                     "Parameter shape of original ckpt", "Parameter shape of target ckpt"]
+    else:
+        x.field_names = field_names
+
     for result in result_list:
         if print_type == 1:
-            x.add_row([result[0],result[1],result[2],result[3],result[4]])
-        elif result[2] is not True:
+            x.add_row([result[0], result[1], result[2], result[3], result[4]])
+        elif print_type == 2 and result[2] is not True:
             x.add_row([result[0], result[1], result[2], result[3], result[4]])
     print(x.get_string())
 
 
 def print_convert_result(result_list):
     x = PrettyTable()
     x.title = 'The list of conversion result'
-    x.field_names = ["Parameter name of pth", "Parameter name of converted ckpt", "Whether the name is converted",
-                     "Whether the weight value is converted","Parameter shape of pth","Parameter shape of ckpt"]
+    x.field_names = ["Parameter name of torch", "Parameter name of MindSpore", "Whether the name is converted",
+                     "Whether the weight value is converted", "Parameter shape of torch",
+                     "Parameter shape of MindSpore"]
+    for result in result_list:
+        x.add_row([result[0], result[1], result[2],
+                  result[3], result[4], result[5]])
+    print(x.get_string())
+
+
+def print_diff_result(result_list, title=None, field_names=None):
+    if not result_list:
+        return
+
+    x = PrettyTable()
+    if title is None:
+        x.title = 'The list of comparison results'
+    else:
+        x.title = title
+
+    if field_names is None:
+        x.field_names = ["orig array name", "target array name",
+                         "results of comparison", "match ratio", "cosine similarity", "(mean, max, min)"]
+    else:
+        x.field_names = field_names
+
     for result in result_list:
-        x.add_row([result[0],result[1],result[2],result[3],result[4],result[5]])
+        ratio = "%.2f" % float(result[3] * 100)
+        cos_sim = "%.5f" % float(result[4])
+        min_max = ['%.6f' % r for r in result[5]]
+        x.add_row([result[0], result[1], result[2], ratio, cos_sim, min_max])
     print(x.get_string())
 
-def print_diff_result(result_list):
+
+def print_net_infer_diff_result(result_list):
     x = PrettyTable()
     x.title = 'The list of comparison results'
-    x.field_names = ["orig array name", "target array name", "Results of comparison", "(mean,max,min)"]
+    x.field_names = ["Pytorch data", "MindSpore data",
+                     "results of comparison", "cosine similarity", "(mean, max, min)"]
     for result in result_list:
-        x.add_row([result[0],result[1],result[2],result[3]])
+        x.add_row([result[0], result[1], result[2], result[3], result[4]])
     print(x.get_string())
 
+
 def print_result(expert_experience, write_file_path):
     """
     print MindSpore FAR
     """
     x = PrettyTable()
     item_desc = _item_to_cn
     x.title = 'MindSpore FAR(Failure Analysis Report)'
     x.field_names = [item_desc.get("item"), item_desc.get("desc")]
     x.align[item_desc.get("desc")] = 'l'
     mindspore_version = expert_experience.get("mindspore_version")
     mindspore_mode = expert_experience.get("mindspore_mode")
     mindspore_device = expert_experience.get("Device Type")
-    x.add_row([item_desc.get("ms_version"), fill(mindspore_version, width=TABLE_WIDTH)])
-    x.add_row([item_desc.get("ms_mode"), fill(mindspore_mode, width=TABLE_WIDTH)])
+    x.add_row([item_desc.get("ms_version"), fill(
+        mindspore_version, width=TABLE_WIDTH)])
+    x.add_row([item_desc.get("ms_mode"), fill(
+        mindspore_mode, width=TABLE_WIDTH)])
     if mindspore_device:
-        x.add_row([item_desc.get("ms_device"), fill(mindspore_device, width=TABLE_WIDTH)])
+        x.add_row([item_desc.get("ms_device"), fill(
+            mindspore_device, width=TABLE_WIDTH)])
     ms_status = expert_experience.get("ms_status")
     code_line = expert_experience.get("code_line")
     sink_mode = expert_experience.get("Sink Mode")
     if ms_status:
-        x.add_row([item_desc.get("ms_status"), fill(ms_status, width=TABLE_WIDTH)])
+        x.add_row([item_desc.get("ms_status"),
+                  fill(ms_status, width=TABLE_WIDTH)])
     if code_line:
-        x.add_row([item_desc.get("code_line"), fill(code_line, width=TABLE_WIDTH)])
+        x.add_row([item_desc.get("code_line"),
+                  fill(code_line, width=TABLE_WIDTH)])
     if sink_mode:
-        x.add_row([item_desc.get("sink_mode"), fill(sink_mode, width=TABLE_WIDTH)])
+        x.add_row([item_desc.get("sink_mode"),
+                  fill(sink_mode, width=TABLE_WIDTH)])
 
     # 可能原因
     fault_cause = expert_experience.get('Fault Cause')
     _add_row(x, "cause", fault_cause)
 
     # 错误代码
     err_code = expert_experience.get("Error Case")
@@ -127,15 +179,16 @@
     # 相关案例
     fault_case = expert_experience.get("Fault Case")
     fault_case = _format_case_str(fault_case, mindspore_version)
     _add_row(x, "case", fault_case)
     if write_file_path:
         case_id = expert_experience.get("ID")
         _add_row(x, "case_id", case_id)
-        file = os.path.join(write_file_path, "mindspore_failure_analysis_report.log")
+        file = os.path.join(
+            write_file_path, "mindspore_failure_analysis_report.log")
         with open(file, "w") as f:
             f.write(x.get_string() + os.linesep)
     print(x.get_string())
 
 
 def _print_msg(title, msg=None, print_msg=True):
     if msg:
@@ -239,15 +292,16 @@
             match = re.search(mindspore_version, line)
             if not match:
                 key = r"(r1.[6-9])|(r2.[0-9])"
                 match = re.search(key, line)
                 # no mindspore link, return
                 if match:
                     link_version = line[match.start():match.end()]
-                    line = _replace_link_version(line, link_version, mindspore_version)
+                    line = _replace_link_version(
+                        line, link_version, mindspore_version)
                 result += line + os.linesep
             else:  # link version same with mindspore version, no replace
                 return content
         content = result
     return content
 
 
@@ -267,16 +321,18 @@
             result = False
             break
     return result
 
 
 def print_clear_exception(exc_type, exc_value, exc_traceback_obj):
     if exc_traceback_obj:
-        _print_msg("[TroubleShooter-Clear Stack] Python Traceback (most recent call last):", "NULL", False)
-        org_err_stack = traceback.format_exception(exc_type, exc_value, exc_traceback_obj)
+        _print_msg(
+            "[TroubleShooter-Clear Stack] Python Traceback (most recent call last):", "NULL", False)
+        org_err_stack = traceback.format_exception(
+            exc_type, exc_value, exc_traceback_obj)
         for stack in org_err_stack:
             if _filter_stack(stack):
                 print(stack.rstrip(os.linesep))
 
 
 def print_format_exception(exc_type, exc_value, exc_traceback_obj):
     """
@@ -289,26 +345,29 @@
         return
 
     msg_dict = get_errmsg_dict(exc_type, exc_value)
     _print_stack(exc_traceback_obj)
     _print_msg("Error Message:", msg_dict.get("err_msg"))
 
     if msg_dict.get("construct_stack_msg"):
-        _print_msg("The Traceback of Net Construct Code:", msg_dict.get("construct_stack_msg"))
+        _print_msg("The Traceback of Net Construct Code:",
+                   msg_dict.get("construct_stack_msg"))
     else:
-        _print_msg("The Traceback of Net Construct Code:", msg_dict.get("construct_stack_in_file_msg"))
+        _print_msg("The Traceback of Net Construct Code:",
+                   msg_dict.get("construct_stack_in_file_msg"))
     _print_msg("C++ Function:", msg_dict.get("cpp_fun_msg"))
     _print_msg("Inner Message:", msg_dict.get("abstract_inner_msg"))
 
 
 def format_error_message(error_message):
     """
     format error message, from string to dict
     """
-    msg_list = error_message.split('----------------------------------------------------')
+    msg_list = error_message.split(
+        '----------------------------------------------------')
     format_msg_dict = {}
     current_key = None
     for msg in msg_list:
         if msg_list.index(msg) == 0:
             format_msg_dict["error_message"] = msg
             continue
         msg = msg.strip().strip(os.linesep)
```

### Comparing `troubleshooter-1.0.7/troubleshooter/common/ms_callback.py` & `troubleshooter-1.0.8/troubleshooter/common/ms_callback.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/common/ms_utils.py` & `troubleshooter-1.0.8/troubleshooter/common/ms_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/log.py` & `troubleshooter-1.0.8/troubleshooter/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/migrator/diff_handler.py` & `troubleshooter-1.0.8/troubleshooter/migrator/weight_migrator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,356 +1,294 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
-"""compare tools"""
 import os
+import mindspore as ms
 import torch
-import numpy as np
+import time
 from collections import OrderedDict
 from pprint import pprint
-from troubleshooter import log as logger
-from troubleshooter.common.util import validate_and_normalize_path, find_file, make_directory
+from troubleshooter.common.format_msg import print_weight_compare_result, print_convert_result ,print_diff_result
 from troubleshooter.migrator.mapping_relation.weight_mapping_lib import weight_name_map, weight_value_map
-from troubleshooter.common.format_msg import print_diff_result, print_weight_compare_result, print_convert_result
+from troubleshooter.migrator.diff_handler import cal_algorithm
+from troubleshooter.toolbox.widget_pocket import object_load ,object_dump
+from troubleshooter import log as logger
+from troubleshooter.common.util import isfile_check, validate_and_normalize_path,\
+    none_and_isfile_check, all_none_or_isfile_check, dir_exist_check, type_check, clear_tmp_file
+
+__all__ = [
+    "get_weight_map",
+    "convert_weight",
+    "compare_ms_ckpt",
+    "compare_pth_and_ckpt",
+]
+
+
+def _get_para_dict(pth_file_path):
+    pt_object = torch.load(pth_file_path, map_location='cpu')
+    if isinstance(pt_object, OrderedDict):
+        pt_para_dict = pt_object
+    elif isinstance(pt_object, torch.nn.Module):
+        pt_para_dict = pt_object.state_dict()
+    else:
+        raise ValueError("PTH file parsing failed, possible reasons: "
+                         "1) If using a custom method to save parameter files, please load and set "
+                         "the 'pth_para_dict' parameter yourself to use the conversion tool."
+                         "2) If the input is an optimizer parameter, this tool does not support "
+                         "the conversion of optimizer parameters.")
+
+    values = list(pt_para_dict.values())
+    if values and not isinstance(values[0], torch.Tensor):
+        raise ValueError("PTH file parsing failed, possible reasons: "
+                         "1) If using a custom method to save parameter files, please load and set "
+                         "the 'pth_para_dict' parameter yourself to use the conversion tool."
+                         "2) If the input is an optimizer parameter, this tool does not support "
+                         "the conversion of optimizer parameters.")
+    return pt_para_dict
+
+
+def _get_object(name):
+    object_res = None
+    index = name.rfind(".")
+    if index:
+        module_name = name[:index]
+        class_name = name[index + 1:]
+        import importlib
+        imp_module = importlib.import_module(module_name)
+        object_res = getattr(imp_module, class_name)
+    return object_res
+
+
+def _get_trans_map(weight_name, module, weight_map, igone_name=False):
+    res_weight_map = {}
+    for api_name in weight_map:
+        obj = _get_object(api_name)
+        if isinstance(module, obj):
+            para_map = weight_map.get(api_name)
+            for pt_para_name, ms_para_name in para_map.items():
+                pt_para_item = weight_name + "." + pt_para_name
+                if igone_name:
+                    ms_para_item = ms_para_name
+                else:
+                    ms_para_item = weight_name + "." + ms_para_name
+                res_weight_map[pt_para_item] = ms_para_item
+            break
+
+    return res_weight_map
 
-FRAMEWORK_TYPE = "ms"
 
-try:
-    import mindspore as ms
-except ModuleNotFoundError as e:
-    e_msg = e.msg
-    no_module_msg = "No module named 'mindspore'"
-    if e_msg == no_module_msg:
-        FRAMEWORK_TYPE = 'pt'
+def _custorm_weight_name_prefix(weight_name_map, prefix=None):
+    if prefix:
+        custorm_name_map = {}
+        for key, value in weight_name_map.items():
+            # print(key, ":", prefix + '.' + value)
+            custorm_name_map[key] = str(prefix) + '.' + str(value)
+        return custorm_name_map
     else:
-        raise e
+        return weight_name_map
 
-class TensorRecorder:
-    def __init__(self):
-        self.summary_record = None
-        self.count = 1
-
-    def init_tensor_summary(self, record_path=None, record_mode=None):
-        if record_mode is None:
-            record_mode = ms.get_context("mode")
-
-        if record_mode == 0:
-            self.summary_record = ms.SummaryRecord(record_path, export_options={'tensor_format': 'npy'})
-
-    def record(self):
-        if not self.summary_record:
-            self.summary_record.record()
-            self.summary_record.flush()
-
-    @staticmethod
-    def record_op(record_dir=None, record_mode=None, framework=None):
-        normal_dir = None
-
-        if framework is None:
-            framework = FRAMEWORK_TYPE
-
-        if record_dir is not None:
-            normal_dir = validate_and_normalize_path(record_dir)
-            make_directory(normal_dir)
-
-        if framework=="ms":
-            if record_mode is None:
-                record_mode = ms.get_context("mode")
-            if record_mode == 0:
-                if record_dir is not None:
-                    logger.user_warning("In MindSpore graph mode, only TensorSummary can be used to record data. "
-                                        "In this mode, The parameter 'record_dir' is not valid")
-                save_op = ms.ops.TensorSummary()
-            else:
-                def save_t2n(name, value):
-                    if normal_dir is not None:
-                        name = os.path.join(normal_dir, name)
-                    np.save(name+".npy", value.asnumpy())
-                save_op = save_t2n
-        else:
-            def save_t2n(name, value):
-                if normal_dir is not None:
-                    name = os.path.join(normal_dir, name)
-                np.save(name + ".npy", value.detach().numpy())
-            save_op = save_t2n
-
-        return save_op
-
-class DifferenceFinder:
-
-    def __init__(self, orig_dir, target_dir):
-        self.orig_dir = orig_dir
-        self.target_dir = target_dir
-    def get_filename_map_list(self):
-        name_map_list = []
-        orig_name_list = find_file(self.orig_dir)
-        orig_name_list.sort()
-        target_name_list = find_file(self.target_dir)
-        none_flag = False
-
-        if not (orig_name_list and target_name_list):
-            logger.user_error("The comparison file is not found in the directory. "
-                              "Please check whether the directory is correct")
-            exit(1)
-
-        for name in orig_name_list:
-            if name in target_name_list:
-                name_map_list.append((name, name))
-                target_name_list.remove(name)
-            else:
-                name_map_list.append((name, None))
-                none_flag = True
-
-        if target_name_list:
-            target_name_list.sort()
-            for name in target_name_list:
-                name_map_list.append((None, name))
-            none_flag = True
-
-        if none_flag:
-            logger.user_warning("The files in the original directory and the target directory cannot be fully mapped. "
-                                "Please manually complete the mapping of file names")
-            print("filename mapping list:" + str(name_map_list))
-        return name_map_list
-
-
-    def compare_npy_dir(self, name_map_list=None, **kwargs):
-        """
-        """
-        if name_map_list is None:
-            name_map_list = self.get_filename_map_list()
-
-        rtol = kwargs.get('rtol', 1e-05)
-        atol = kwargs.get('atol', 1e-08)
-        equal_nan = kwargs.get('equal_nan', False)
-
-        result_list = []
-        normal_orig_dir = validate_and_normalize_path(self.orig_dir)
-        normal_target_dir = validate_and_normalize_path(self.target_dir)
-        for name_map in name_map_list:
-            orig_name = name_map[0]
-            target_name = name_map[1]
-
-            if orig_name is None or target_name is None:
-                result = False
-                diff_detail = ()
-                result_list.append((orig_name, target_name, result, diff_detail))
-                continue
-
-            orig_file = os.path.join(normal_orig_dir, orig_name)
-            target_file = os.path.join(normal_target_dir, target_name)
-
-            if not os.path.isfile(orig_file) or not os.path.isfile(target_file):
-                continue
-
-            orig_value = np.load(orig_file)
-            target_value = np.load(target_file)
-            if orig_value.shape == target_value.shape:
-                result = np.allclose(orig_value, target_value, rtol=rtol, atol=atol, equal_nan=equal_nan)
-
-                if not result:
-                    value_diff = np.abs(orig_value - target_value)
-                    value_mean = value_diff.mean()
-                    value_max = value_diff.max()
-                    value_min = value_diff.min()
-                    diff_detail = value_mean, value_max, value_min
-                else:
-                    diff_detail = ()
-            else:
-                result = False
-                diff_detail = ("Shape is inconsistent", orig_value.shape, target_value.shape)
-
-            result_list.append((orig_name, target_name, result, diff_detail))
-        logger.user_attention("The compare directory information:\n The orig dir: %s \n The target dir: %s",
-                              self.orig_dir, self.target_dir)
-        print_diff_result(result_list)
-
-class WeightMigrator:
-
-    def __init__(self, pt_model=None, pth_file_path=None, pth_para_dict=None, ckpt_save_path=None):
-        self.weight_map = weight_name_map
-        self.ckpt_path = ckpt_save_path
-        self.pt_model = pt_model
-        self.pt_para_dict = self._get_para_dict(pth_file_path, pth_para_dict)
-        self.print_params_list = []
-
-
-    def _get_para_dict(self, pth_file_path, pth_para_dict):
-        if pth_para_dict:
-            return pth_para_dict
-
-        pt_para_dict = {}
-        pt_object = torch.load(pth_file_path, map_location='cpu')
-        if isinstance(pt_object, OrderedDict):
-            pt_para_dict = pt_object
-        elif isinstance(pt_object, torch.nn.Module):
-            pt_para_dict = pt_object.state_dict()
-        else:
-            raise ValueError("PTH file parsing failed, possible reasons: "
-                             "1) If using a custom method to save parameter files, please load and set "
-                             "the 'pth_para_dict' parameter yourself to use the conversion tool."
-                             "2) If the input is an optimizer parameter, this tool does not support "
-                             "the conversion of optimizer parameters.")
-
-        values = list(pt_para_dict.values())
-        if values and not isinstance(values[0], torch.Tensor):
-            raise ValueError("PTH file parsing failed, possible reasons: "
-                             "1) If using a custom method to save parameter files, please load and set "
-                             "the 'pth_para_dict' parameter yourself to use the conversion tool."
-                             "2) If the input is an optimizer parameter, this tool does not support "
-                             "the conversion of optimizer parameters.")
-        return pt_para_dict
-
-    def _get_object(self, name):
-        object_res = None
-        index = name.rfind(".")
-        if index:
-            module_name = name[:index]
-            class_name = name[index + 1:]
-            import importlib
-            imp_module = importlib.import_module(module_name)
-            object_res = getattr(imp_module, class_name)
-        return object_res
-
-
-    def _get_trans_map(self, weight_name, module, weight_map, igone_name=False):
-        res_weight_map = {}
-        for api_name in weight_map:
-            obj = self._get_object(api_name)
-            if isinstance(module, obj):
-                para_map = weight_map.get(api_name)
-                for pt_para_name, ms_para_name in para_map.items():
-                    pt_para_item = weight_name + "." + pt_para_name
-                    if igone_name:
-                        ms_para_item = ms_para_name
-                    else:
-                        ms_para_item = weight_name + "." + ms_para_name
-                    res_weight_map[pt_para_item] = ms_para_item
-                break
-
-        return res_weight_map
-
-
-    def _custorm_weight_name_prefix(self, weight_name_map, prefix=None):
-        if prefix:
-            custorm_name_map = {}
-            for key, value in weight_name_map.items():
-                # print(key, ":", prefix + '.' + value)
-                custorm_name_map[key] = str(prefix) + '.' + str(value)
-            return custorm_name_map
-        else:
-            return weight_name_map
 
+def get_weight_map(pt_model=None, weight_map_save_path=None, weight_name_prefix=None, custom_name_func=None, print_map=False, **kwargs):
+    res_weight_name_map = {}
+    res_weight_value_map = {}
+    full_weight_name_map = {}
 
-    def get_weight_map(self, print_map=False, full_name_map=False):
-        res_weight_name_map = {}
-        res_weight_value_map = {}
-        full_weight_name_map = {}
-
-        for name, module in self.pt_model.named_modules():
-            tmp_name_map = self._get_trans_map(name, module, weight_name_map)
-            if tmp_name_map:
-                res_weight_name_map.update(tmp_name_map)
-            tmp_value_map = self._get_trans_map(name, module, weight_value_map, igone_name=True)
-            if tmp_value_map:
-                res_weight_value_map.update(tmp_value_map)
-        if full_name_map:
-            for key, value in self.pt_para_dict.items():
-                full_weight_name_map[key]=key
-            full_weight_name_map.update(res_weight_name_map)
-            res_weight_name_map =  full_weight_name_map
-
-        if print_map:
-            pprint(res_weight_name_map)
-            pprint(res_weight_value_map)
-        return res_weight_name_map, res_weight_value_map
-
-
-    def _get_name_and_value(self, pth_param_name, name_map, value_map):
-        new_name = pth_param_name
-        parameter = self.pt_para_dict[pth_param_name]
-        ms_tensor = ms.Tensor(parameter.numpy())
+    if not isinstance(pt_model, torch.nn.Module):
+        raise TypeError("The parameter 'pt_model' must be torch.nn.Module")
+
+    if custom_name_func and not callable(custom_name_func):
+        raise TypeError("The parameter 'custom_name_func' must be a function")
+
+    dir_exist_check(weight_map_save_path, 'weight_map_save_path')
+    type_check(weight_name_prefix, 'weight_name_prefix', str)
+    type_check(print_map, 'print_map', bool)
+
+    for name, module in pt_model.named_modules():
+        tmp_name_map = _get_trans_map(name, module, weight_name_map)
+        if tmp_name_map:
+            res_weight_name_map.update(tmp_name_map)
+
+        tmp_value_map = _get_trans_map(name, module, weight_value_map, igone_name=True)
+        if tmp_value_map:
+            res_weight_value_map.update(tmp_value_map)
+
+    for key, value in pt_model.state_dict().items():
+        full_weight_name_map[key] = key
+
+    full_weight_name_map.update(res_weight_name_map)
+    res_weight_name_map = full_weight_name_map
+    res_weight_name_map = _custorm_weight_name_prefix(res_weight_name_map, weight_name_prefix)
+
+    if custom_name_func:
+        res_weight_name_map = custom_name_func(res_weight_name_map)
+
+    if print_map:
+        pprint(res_weight_name_map)
+        pprint(res_weight_value_map)
+    if weight_map_save_path:
+        object_dump([res_weight_name_map,res_weight_value_map], weight_map_save_path)
+    return res_weight_name_map, res_weight_value_map
 
+weight_map_dump=object_dump
+
+def convert_weight(weight_map_path=None, pt_file_path=None, ms_file_save_path=None, **kwargs):
+    print_params_list = []
+
+    print_conv_info = kwargs.get('print_conv_info', True)
+    pt_param_dict = kwargs.get('pt_param_dict', None)
+    weight_map = kwargs.get('weight_map', None)
+
+    all_none_or_isfile_check(weight_map_path,'weight_map_path',weight_map ,'weight_map')
+    all_none_or_isfile_check(pt_file_path, 'pt_file_path', pt_param_dict, 'pt_param_dict')
+    dir_exist_check(ms_file_save_path,'ms_file_save_path')
+    type_check(print_conv_info,'print_conv_info', bool)
+
+    if weight_map:
+        name_map, value_map = weight_map
+    else:
+        name_map, value_map = object_load(weight_map_path)
+
+    if pt_param_dict:
+        pt_param_dict = pt_param_dict
+    else:
+        pt_param_dict = _get_para_dict(pt_file_path)
+
+    new_params_list = []
+
+    for pth_param_name in pt_param_dict:
+        # get ckpt name and value
+        parameter = pt_param_dict[pth_param_name]
+        ms_tensor = ms.Tensor(parameter.numpy())
         # Update name based on name mapping
         ms_para_item = name_map.get(pth_param_name)
-        if ms_para_item:
-            new_name = ms_para_item
 
         # Update values based on parameter value mapping
         if value_map is not None:
-            fun = value_map.get(pth_param_name)
-
-        if fun:
-            def_get_value = self._get_object(fun)
+            func = value_map.get(pth_param_name)
+        if func:
+            def_get_value = _get_object(func)
             ms_tensor = def_get_value(ms_tensor)
+        print_params_list.append((pth_param_name, ms_para_item, bool(ms_para_item!=pth_param_name),
+                                  bool(func), parameter.size(), ms_tensor.shape))
+        # add name and value to list
+        new_params_list.append({"name": ms_para_item, "data": ms_tensor})
+
+    if new_params_list is None:
+        logger.user_warning("There are no parameters to be converted. Parameter conversion failed. "
+                            "Please check whether the configuration is correct")
+    if ms_file_save_path:
+        ms.save_checkpoint(new_params_list, ms_file_save_path)
+
+    if print_conv_info:
+        print_convert_result(print_params_list)
+    logger.user_attention("The PTH has been converted to the checkpoint of MindSpore. "
+                          "Please check whether the conversion result is correct. "
+                          "The saved path is: %s", ms_file_save_path)
+
+
+def compare_ms_ckpt(orig_file_path=None, target_file_path=None, **kwargs):
+    name_map_list = []
+    value_map_list = []
+    name_map = None
+    title = 'The list of comparison results for values'
+    field_names = ["Parameter name of original ckpt", "Parameter name of target ckpt",
+                   "results of comparison", "match ratio",
+                   "cosine similarity", "(mean, max, min)"]
+    field_names_pth = ["Parameter name of torch", "Parameter name of MindSpore",
+                   "results of comparison", "match ratio",
+                   "cosine similarity", "(mean, max, min)"]
+    field_names_shape_pth=["Parameter name of torch", "Parameter name of MindSpore",
+                           "Whether shape are equal", "Parameter shape of torch",
+                           "Parameter shape of MindSpore"]
+
+    compare_value = kwargs.get('compare_value', False)
+    weight_map_path = kwargs.get('weight_map_path', None)
+    weight_map = kwargs.get('weight_map', None)
+    orig_ckpt_dict = kwargs.get('orig_ckpt_dict', None)
+    target_ckpt_dict = kwargs.get('target_ckpt_dict', None)
+    print_level = kwargs.get('print_level', 1)
+    rtol = kwargs.get('rtol', 1e-04)
+    atol = kwargs.get('atol', 1e-08)
+    equal_nan = kwargs.get('equal_nan', False)
+
+    all_none_or_isfile_check(orig_file_path, 'orig_file_path', orig_ckpt_dict, 'orig_ckpt_dict')
+    all_none_or_isfile_check(target_file_path, 'target_file_path', target_ckpt_dict, 'target_ckpt_dict')
+    type_check(compare_value,'compare_value', bool)
+    type_check(print_level, 'print_level', int)
+    isfile_check(weight_map_path,'weight_map_path')
+
+    if orig_file_path:
+        orig_ckpt_dict = ms.load_checkpoint(orig_file_path)
+    if target_file_path:
+        target_ckpt_dict = ms.load_checkpoint(target_file_path)
+
+    if weight_map_path:
+        name_map, _ = object_load(weight_map_path)
+        name_map =  dict(zip(name_map.values(), name_map.keys()))
+
+    if weight_map:
+        name_map, _ = weight_map
+        name_map = dict(zip(name_map.values(), name_map.keys()))
+
+    for orig_name, orig_parameter in orig_ckpt_dict.items():
+        if name_map:
+            new_orig_name = name_map.get(orig_name)
+        else:
+            new_orig_name = orig_name
 
-        self.print_params_list.append((pth_param_name, new_name, bool(ms_para_item), bool(fun) , parameter.size(),
-                                       ms_tensor.shape))
-        return new_name, ms_tensor
-
-
-    def convert(self, weight_name_map=None, weight_value_map=None ,weight_name_prefix=None, print_conv_info=True):
+        target_para = target_ckpt_dict.get(orig_name)
+        target_para_name = orig_name
 
-        if weight_name_prefix:
-            name_map, value_map = self.get_weight_map(full_name_map=True)
-            name_map = self._custorm_weight_name_prefix(name_map, weight_name_prefix)
+        if target_para is not None:
+            name_map_list.append((new_orig_name, target_para_name, (target_para.shape == orig_parameter.shape),
+                                  orig_parameter.shape, target_para.shape))
+            if compare_value:
+                result, rel_ratio, cosine_sim, diff_detail =cal_algorithm(orig_parameter.value().asnumpy(),
+                                                                          target_para.value().asnumpy(),
+                                                                          rtol,
+                                                                          atol,
+                                                                          equal_nan)
+                value_map_list.append((new_orig_name, target_para_name, result, rel_ratio, cosine_sim, diff_detail))
+            target_ckpt_dict.pop(target_para_name)
         else:
-            name_map, value_map = self.get_weight_map()
+            name_map_list.append((new_orig_name, None, None, orig_parameter.shape, None))
 
-        if weight_name_map is not None:
-            name_map =  weight_name_map
-        if weight_value_map is not None:
-            value_map =  weight_value_map
-
-        new_params_list = []
-
-        for pth_param_name in self.pt_para_dict:
-            # get ckpt name and value
-            new_name, ms_tensor = self._get_name_and_value(pth_param_name,name_map,value_map)
-            # add name and value to list
-            new_params_list.append({"name": new_name, "data": ms_tensor})
+    for name, target_para in target_ckpt_dict.items():
+        name_map_list.append((None, name, None, None, target_para.shape))
+
+    if weight_map_path:
+        print_weight_compare_result(name_map_list, print_type=print_level, field_names=field_names_shape_pth)
+        print_diff_result(value_map_list, title, field_names_pth)
+    else:
+        print_weight_compare_result(name_map_list, print_type=print_level)
+        print_diff_result(value_map_list, title, field_names)
 
-        if new_params_list:
-            ms.save_checkpoint(new_params_list , self.ckpt_path)
-        else:
-            logger.user_warning("There are no parameters to be converted. Parameter conversion failed. "
-                                "Please check whether the configuration is correct")
 
-        if print_conv_info:
-             print_convert_result(self.print_params_list)
+def compare_pth_and_ckpt(weight_map_path=None, pt_file_path=None, ms_file_path=None, **kwargs):
+    temp_save_path = validate_and_normalize_path(kwargs.get('temp_save_path', './'))
+    timestamp = time.time()
+    formatted_time = time.strftime('%Y%m%d-%H%M%S', time.localtime(timestamp))
+    temp_name = formatted_time + "_ts_temp_file.ckpt"
+    tmp_ckpt_file = os.path.join(temp_save_path, temp_name)
+    print_level = kwargs.get('print_level', 1)
+
+    none_and_isfile_check(weight_map_path, 'weight_map_path')
+    none_and_isfile_check(pt_file_path, 'pt_file_path')
+    none_and_isfile_check(ms_file_path, 'ms_file_path')
+
+    convert_weight(weight_map_path=weight_map_path, pt_file_path=pt_file_path, ms_file_save_path=tmp_ckpt_file,
+                                  print_level=print_level)
+    compare_ms_ckpt(orig_file_path=tmp_ckpt_file, target_file_path=ms_file_path,
+                    compare_value=True, weight_map_path=weight_map_path)
+    clear_tmp_file(tmp_ckpt_file)
 
-        logger.user_attention("The PTH has been converted to the checkpoint of MindSpore. "
-                              "Please check whether the conversion result is correct. "
-                              "The saved path is: %s",self.ckpt_path)
-
-
-    def compare_ckpt(self, ckpt_path=None, converted_ckpt_path=None, print_result=1):
-        name_map_list = []
-        if converted_ckpt_path is None:
-            ckpt_after_convert_path = self.ckpt_path
-        ckpt_dict = ms.load_checkpoint(ckpt_path)
-        ckpt_after_conv_dict = ms.load_checkpoint(ckpt_after_convert_path)
-
-        for ms_para_name, ms_para in ckpt_dict.items():
-            ms_para_after_conv = ckpt_after_conv_dict.get(ms_para_name)
-
-            if ms_para_after_conv is not None:
-                name_map_list.append((ms_para_name, ms_para_name, (ms_para.shape == ms_para_after_conv.shape),
-                                      ms_para.shape, ms_para_after_conv.shape))
-                ckpt_after_conv_dict.pop(ms_para_name)
-            else:
-                name_map_list.append((ms_para_name, None, None, ms_para.shape, None))
-
-        for name, ms_para in ckpt_after_conv_dict.items():
-            name_map_list.append((None, name, None, None, ms_para.shape))
-        print_weight_compare_result(name_map_list, print_type=print_result)
```

### Comparing `troubleshooter-1.0.7/troubleshooter/migrator/mapping_relation/weight_adapter.py` & `troubleshooter-1.0.8/troubleshooter/migrator/mapping_relation/weight_adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/migrator/mapping_relation/weight_mapping_lib.py` & `troubleshooter-1.0.8/troubleshooter/migrator/mapping_relation/weight_mapping_lib.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/__init__.py` & `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/base_proposer.py` & `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/base_proposer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/compiler_proposer.py` & `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/compiler_proposer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/compiler_scene_proposer.py` & `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/compiler_scene_proposer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/dataset_proposer.py` & `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/dataset_proposer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/dataset_scene_proposer.py` & `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/dataset_scene_proposer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/default_proposer.py` & `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/default_proposer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/front_proposer.py` & `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/front_proposer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/operators_proposer.py` & `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/operators_proposer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/operators_scene_proposer.py` & `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/operators_scene_proposer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/allproposers/vm_proposer.py` & `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/vm_proposer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/__init__.py` & `troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/common_exp_lib.py` & `troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/common_exp_lib.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/compiler_exp_lib.py` & `troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/compiler_exp_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/dataset_exp_lib.py` & `troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/dataset_exp_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/front_exp_lib.py` & `troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/front_exp_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/operators_exp_lib.py` & `troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/operators_exp_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/knowledge_base/vm_exp_lib.py` & `troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/vm_exp_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/proposal_action.py` & `troubleshooter-1.0.8/troubleshooter/proposer/proposal_action.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/proposer/proposer_factory.py` & `troubleshooter-1.0.8/troubleshooter/proposer/proposer_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `troubleshooter-1.0.7/troubleshooter/tracker/__init__.py` & `troubleshooter-1.0.8/troubleshooter/common/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
-"""Proposer for profiler."""
-from troubleshooter.tracker.tracker import Tracker
-__all__ = ["Tracker"]
+from __future__ import absolute_import
+
+from troubleshooter.common import framework_detection
+from troubleshooter.common.framework_detection import FRAMEWORK_TYPE
+
+__all__ = []
+__all__.extend(framework_detection.__all__)
```

### Comparing `troubleshooter-1.0.7/troubleshooter/tracker/tracker.py` & `troubleshooter-1.0.8/troubleshooter/tracker/tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Tiger Miao and collaborators.
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -74,17 +74,18 @@
         if self.event_list and 'call' in self.event_list and 'return' not in self.event_list:
             self.event_list.append('return')
         if self.level == 2:
             blacklist = {"__setattr__": "nn/cell.py", "__getattr__": "nn/cell.py"}
             self.ms_func_blacklist.update(blacklist)
 
         self.pop_key_list = ['event_list', 'func_wl', 'path_wl', 'depth', 'max_variable_length', 'check_keyword',
-                             'path_bl', 'check_mode']
+                             'path_bl', 'check_mode', 'framework']
         for key in self.pop_key_list:
-            if kwargs.get(key):
+            value = kwargs.get(key)
+            if value is not None:
                 kwargs.pop(key)
         super(Tracker, self).__init__(depth=self.depth, max_variable_length=self.max_variable_length, **kwargs)
 
     def _frame_filter(self, frame, event):
         if self.framework == _FRAMEWORK_MS:
             return self._frame_filter_ms(frame, event)
         return True
```

### Comparing `troubleshooter-1.0.7/troubleshooter.egg-info/SOURCES.txt` & `troubleshooter-1.0.8/troubleshooter.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 LICENSE
 README.md
 setup.py
 tests/__init__.py
 tests/util.py
-tests/diff_handler/__init__.py
-tests/diff_handler/test_compare.py
-tests/diff_handler/test_migrator.py
 tests/proposer/__init__.py
 tests/proposer/1_9/__init__.py
 tests/proposer/1_9/test_compile.py
 tests/proposer/1_9/test_ops.py
 tests/proposer/master/__init__.py
 tests/proposer/master/test_ascend_vm.py
 tests/proposer/master/test_compile.py
 tests/proposer/master/test_dataset.py
 tests/proposer/master/test_me_front.py
 tests/proposer/master/test_ops.py
 tests/proposer/master/test_st_output.py
-tests/tracker/__init__.py
-tests/tracker/test_tracking.py
 troubleshooter/__init__.py
 troubleshooter/log.py
 troubleshooter/version.py
 troubleshooter.egg-info/PKG-INFO
 troubleshooter.egg-info/SOURCES.txt
 troubleshooter.egg-info/dependency_links.txt
 troubleshooter.egg-info/requires.txt
 troubleshooter.egg-info/top_level.txt
 troubleshooter/common/__init__.py
 troubleshooter/common/format_msg.py
+troubleshooter/common/framework_detection.py
 troubleshooter/common/ms_callback.py
 troubleshooter/common/ms_utils.py
 troubleshooter/common/util.py
 troubleshooter/migrator/__init__.py
 troubleshooter/migrator/diff_handler.py
+troubleshooter/migrator/net_diff_finder.py
+troubleshooter/migrator/weight_migrator.py
 troubleshooter/migrator/mapping_relation/__init__.py
 troubleshooter/migrator/mapping_relation/weight_adapter.py
 troubleshooter/migrator/mapping_relation/weight_mapping_lib.py
+troubleshooter/migrator/save/__init__.py
+troubleshooter/migrator/save/base_saver.py
+troubleshooter/migrator/save/mindspore_saver.py
+troubleshooter/migrator/save/torch_saver.py
+troubleshooter/migrator/save/unified_saver.py
 troubleshooter/proposer/__init__.py
 troubleshooter/proposer/proposal_action.py
 troubleshooter/proposer/proposer_factory.py
 troubleshooter/proposer/allproposers/__init__.py
 troubleshooter/proposer/allproposers/base_proposer.py
 troubleshooter/proposer/allproposers/compiler_proposer.py
 troubleshooter/proposer/allproposers/compiler_scene_proposer.py
@@ -54,9 +57,21 @@
 troubleshooter/proposer/knowledge_base/__init__.py
 troubleshooter/proposer/knowledge_base/common_exp_lib.py
 troubleshooter/proposer/knowledge_base/compiler_exp_lib.py
 troubleshooter/proposer/knowledge_base/dataset_exp_lib.py
 troubleshooter/proposer/knowledge_base/front_exp_lib.py
 troubleshooter/proposer/knowledge_base/operators_exp_lib.py
 troubleshooter/proposer/knowledge_base/vm_exp_lib.py
+troubleshooter/toolbox/__init__.py
+troubleshooter/toolbox/widget_pocket.py
+troubleshooter/toolbox/dump/__init__.py
+troubleshooter/toolbox/dump/alexnet.py
+troubleshooter/toolbox/dump/cell.py
+troubleshooter/toolbox/dump/demo.py
+troubleshooter/toolbox/dump/hooks.py
+troubleshooter/toolbox/dump/initialize.py
+troubleshooter/toolbox/dump/utils.py
+troubleshooter/toolbox/dump/wrap_functional.py
+troubleshooter/toolbox/dump/wrap_nn.py
+troubleshooter/toolbox/dump/wrap_tensor.py
 troubleshooter/tracker/__init__.py
 troubleshooter/tracker/tracker.py
```

