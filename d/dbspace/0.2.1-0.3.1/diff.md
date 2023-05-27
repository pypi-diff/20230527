# Comparing `tmp/dbspace-0.2.1.tar.gz` & `tmp/dbspace-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbspace-0.2.1.tar", max compression
+gzip compressed data, was "dbspace-0.3.1.tar", max compression
```

## Comparing `dbspace-0.2.1.tar` & `dbspace-0.3.1.tar`

### file list

```diff
@@ -1,64 +1,63 @@
--rw-r--r--   0        0        0    35147 2018-05-29 17:35:40.000000 dbspace-0.2.1/LICENSE
--rw-r--r--   0        0        0      586 2022-12-26 19:10:02.458569 dbspace-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      343 2022-12-26 18:31:12.206409 dbspace-0.2.1/src/dbspace/__init__.py
--rw-r--r--   0        0        0    86780 2022-03-31 05:41:31.000000 dbspace-0.2.1/src/dbspace/__testing__/readout/DSV.py
--rwxr-xr-x   0        0        0     5306 2022-04-02 03:07:17.000000 dbspace-0.2.1/src/dbspace/control/DTI.py
--rwxr-xr-x   0        0        0    21576 2022-04-02 03:07:17.000000 dbspace-0.2.1/src/dbspace/control/DTI_support.py
--rw-r--r--   0        0        0     2907 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/control/VirtTract.py
--rw-r--r--   0        0        0       80 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/control/__init__.py
--rw-r--r--   0        0        0     8038 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/control/dyn_osc.py
--rwxr-xr-x   0        0        0    12509 2022-03-31 22:36:04.000000 dbspace-0.2.1/src/dbspace/control/network_action.py
--rwxr-xr-x   0        0        0    87519 2022-08-28 00:13:31.240005 dbspace-0.2.1/src/dbspace/control/offline_segments.py
--rwxr-xr-x   0        0        0    16656 2022-12-26 17:15:44.287736 dbspace-0.2.1/src/dbspace/control/stream_buffers.py
--rw-r--r--   0        0        0    17734 2022-12-26 17:15:44.287736 dbspace-0.2.1/src/dbspace/readout/BR_DataFrame.py
--rw-r--r--   0        0        0    28991 2022-08-28 03:15:25.330191 dbspace-0.2.1/src/dbspace/readout/ClinVect.py
--rw-r--r--   0        0        0    20590 2022-03-31 03:28:24.000000 dbspace-0.2.1/src/dbspace/readout/OBands.py
--rw-r--r--   0        0        0       81 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/readout/__init__.py
--rw-r--r--   0        0        0    13212 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/readout/__pycache__/BR_DataFrame.cpython-37.pyc
--rw-r--r--   0        0        0    19925 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/readout/__pycache__/ClinVect.cpython-37.pyc
--rw-r--r--   0        0        0    48890 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/readout/__pycache__/DSV.cpython-37.pyc
--rw-r--r--   0        0        0      214 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/readout/__pycache__/__init__.cpython-37.pyc
--rwxr-xr-x   0        0        0    44985 2022-08-01 19:02:31.759999 dbspace-0.2.1/src/dbspace/readout/decoder.py
--rw-r--r--   0        0        0      642 2022-03-24 19:21:20.000000 dbspace-0.2.1/src/dbspace/readout/phases.py
--rw-r--r--   0        0        0    41904 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/signal/PAC/PyPAC.py
--rw-r--r--   0        0        0      176 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/signal/PAC/README
--rw-r--r--   0        0        0     4158 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/signal/PAC/SyntheticSignalTesting.py
--rw-r--r--   0        0        0       35 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/signal/PAC/__init__.py
--rw-r--r--   0        0        0       36 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/signal/PRE/__init__.py
--rwxr-xr-x   0        0        0     4675 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/signal/PRE/tree_view.py
--rw-r--r--   0        0        0        0 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/signal/__init__.py
--rwxr-xr-x   0        0        0     3308 2022-03-31 05:41:31.000000 dbspace-0.2.1/src/dbspace/signal/dEEG/neigh_mont.py
--rw-r--r--   0        0        0      127 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/signal/dLFP/README.md
--rw-r--r--   0        0        0       46 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/signal/dLFP/__init__.py
--rw-r--r--   0        0        0      163 2022-12-26 17:15:44.287736 dbspace-0.2.1/src/dbspace/signal/dLFP/amp_tf_models.py
--rw-r--r--   0        0        0     5369 2022-12-26 17:15:44.287736 dbspace-0.2.1/src/dbspace/signal/dLFP/brain_amp_model.py
--rwxr-xr-x   0        0        0     1564 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/signal/dLFP/db_stim.py
--rw-r--r--   0        0        0     4232 2022-12-26 17:15:44.287736 dbspace-0.2.1/src/dbspace/signal/dLFP/diff_amp_model.py
--rw-r--r--   0        0        0       78 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/signal/dLFP/gcr.py
--rw-r--r--   0        0        0     5823 2022-12-26 17:15:44.291069 dbspace-0.2.1/src/dbspace/signal/dLFP/impedances.py
--rwxr-xr-x   0        0        0     5167 2022-08-28 03:15:25.333525 dbspace-0.2.1/src/dbspace/signal/dLFP/ipg_stim.py
--rw-r--r--   0        0        0     8569 2022-12-26 17:15:44.291069 dbspace-0.2.1/src/dbspace/signal/dLFP/sig_amp_model.py
--rw-r--r--   0        0        0     2066 2022-03-24 19:21:20.000000 dbspace-0.2.1/src/dbspace/signal/hots.py
--rw-r--r--   0        0        0    14892 2022-12-26 17:15:44.291069 dbspace-0.2.1/src/dbspace/signal/oscillations.py
--rwxr-xr-x   0        0        0    10777 2022-12-26 17:15:44.294402 dbspace-0.2.1/src/dbspace/signal/spot_check.py
--rw-r--r--   0        0        0        0 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/utils/__init__.py
--rw-r--r--   0        0        0      149 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/utils/costs.py
--rw-r--r--   0        0        0      309 2022-03-31 05:39:38.000000 dbspace-0.2.1/src/dbspace/utils/functions.py
--rw-r--r--   0        0        0        0 2022-04-02 03:47:19.000000 dbspace-0.2.1/src/dbspace/utils/io/brPY/__init__.py
--rw-r--r--   0        0        0     2776 2022-04-02 03:47:19.000000 dbspace-0.2.1/src/dbspace/utils/io/brPY/brMiscFxns.py
--rw-r--r--   0        0        0    71040 2022-04-02 03:47:19.000000 dbspace-0.2.1/src/dbspace/utils/io/brPY/brpylib.py
--rw-r--r--   0        0        0      511 2022-03-24 19:21:20.000000 dbspace-0.2.1/src/dbspace/utils/io/br_io.py
--rw-r--r--   0        0        0        0 2022-03-24 19:21:20.000000 dbspace-0.2.1/src/dbspace/utils/io/deeg_io.py
--rw-r--r--   0        0        0      725 2022-12-26 17:15:44.294402 dbspace-0.2.1/src/dbspace/utils/io/pcs.py
--rw-r--r--   0        0        0        0 2022-03-24 19:21:20.000000 dbspace-0.2.1/src/dbspace/utils/io/xlt_io.py
--rw-r--r--   0        0        0     1068 2022-08-18 21:40:04.047089 dbspace-0.2.1/src/dbspace/utils/r_pca/LICENSE
--rw-r--r--   0        0        0        0 2022-08-18 21:40:04.047089 dbspace-0.2.1/src/dbspace/utils/r_pca/__init__.py
--rw-r--r--   0        0        0     2642 2022-08-28 00:13:31.243338 dbspace-0.2.1/src/dbspace/utils/r_pca/r_pca.py
--rw-r--r--   0        0        0     1323 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/utils/stats.py
--rw-r--r--   0        0        0      170 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/utils/structures.py
--rw-r--r--   0        0        0    10586 2022-03-31 20:14:31.000000 dbspace-0.2.1/src/dbspace/viz/MM/EEG_Viz.py
--rw-r--r--   0        0        0     2801 2022-04-02 03:47:19.000000 dbspace-0.2.1/src/dbspace/viz/MM/intraop.py
--rw-r--r--   0        0        0        0 2022-03-23 22:30:19.000000 dbspace-0.2.1/src/dbspace/viz/TF/TS_spectrogram.py
--rw-r--r--   0        0        0        0 2022-04-02 03:47:19.000000 dbspace-0.2.1/src/dbspace/viz/__init__.py
--rw-r--r--   0        0        0     1253 1970-01-01 00:00:00.000000 dbspace-0.2.1/setup.py
--rw-r--r--   0        0        0      832 1970-01-01 00:00:00.000000 dbspace-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2018-05-29 17:35:40.000000 dbspace-0.3.1/LICENSE
+-rw-r--r--   0        0        0      586 2023-05-27 19:41:05.817252 dbspace-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      123 2023-05-17 02:58:17.694835 dbspace-0.3.1/src/dbspace/__init__.py
+-rw-r--r--   0        0        0    86780 2022-03-31 05:41:31.000000 dbspace-0.3.1/src/dbspace/__testing__/readout/DSV.py
+-rwxr-xr-x   0        0        0     5306 2022-04-02 03:07:17.000000 dbspace-0.3.1/src/dbspace/control/DTI.py
+-rwxr-xr-x   0        0        0    21576 2022-04-02 03:07:17.000000 dbspace-0.3.1/src/dbspace/control/DTI_support.py
+-rw-r--r--   0        0        0     2907 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/control/VirtTract.py
+-rw-r--r--   0        0        0       80 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/control/__init__.py
+-rw-r--r--   0        0        0     8038 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/control/dyn_osc.py
+-rwxr-xr-x   0        0        0    12509 2022-03-31 22:36:04.000000 dbspace-0.3.1/src/dbspace/control/network_action.py
+-rwxr-xr-x   0        0        0    88041 2023-05-17 02:58:17.698168 dbspace-0.3.1/src/dbspace/control/offline_segments.py
+-rwxr-xr-x   0        0        0    16656 2023-03-23 02:41:01.044928 dbspace-0.3.1/src/dbspace/control/stream_buffers.py
+-rw-r--r--   0        0        0    17734 2023-03-23 02:41:01.048262 dbspace-0.3.1/src/dbspace/readout/BR_DataFrame.py
+-rw-r--r--   0        0        0    29012 2023-05-17 02:58:17.701501 dbspace-0.3.1/src/dbspace/readout/ClinVect.py
+-rw-r--r--   0        0        0    20590 2022-03-31 03:28:24.000000 dbspace-0.3.1/src/dbspace/readout/OBands.py
+-rw-r--r--   0        0        0       81 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/readout/__init__.py
+-rw-r--r--   0        0        0    13212 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/readout/__pycache__/BR_DataFrame.cpython-37.pyc
+-rw-r--r--   0        0        0    19925 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/readout/__pycache__/ClinVect.cpython-37.pyc
+-rw-r--r--   0        0        0    48890 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/readout/__pycache__/DSV.cpython-37.pyc
+-rw-r--r--   0        0        0      214 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/readout/__pycache__/__init__.cpython-37.pyc
+-rwxr-xr-x   0        0        0    44985 2022-08-01 19:02:31.759999 dbspace-0.3.1/src/dbspace/readout/decoder.py
+-rw-r--r--   0        0        0      642 2022-03-24 19:21:20.000000 dbspace-0.3.1/src/dbspace/readout/phases.py
+-rw-r--r--   0        0        0    41904 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/signal/PAC/PyPAC.py
+-rw-r--r--   0        0        0      176 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/signal/PAC/README
+-rw-r--r--   0        0        0     4158 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/signal/PAC/SyntheticSignalTesting.py
+-rw-r--r--   0        0        0       35 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/signal/PAC/__init__.py
+-rw-r--r--   0        0        0       36 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/signal/PRE/__init__.py
+-rwxr-xr-x   0        0        0     4675 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/signal/PRE/tree_view.py
+-rw-r--r--   0        0        0        0 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/signal/__init__.py
+-rwxr-xr-x   0        0        0     3308 2022-03-31 05:41:31.000000 dbspace-0.3.1/src/dbspace/signal/dEEG/neigh_mont.py
+-rw-r--r--   0        0        0      127 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/signal/dLFP/README.md
+-rw-r--r--   0        0        0       46 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/signal/dLFP/__init__.py
+-rw-r--r--   0        0        0      163 2023-03-23 02:41:01.048262 dbspace-0.3.1/src/dbspace/signal/dLFP/amp_tf_models.py
+-rw-r--r--   0        0        0     5369 2023-03-23 02:41:01.048262 dbspace-0.3.1/src/dbspace/signal/dLFP/brain_amp_model.py
+-rwxr-xr-x   0        0        0     1564 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/signal/dLFP/db_stim.py
+-rw-r--r--   0        0        0     4232 2023-03-23 02:41:01.048262 dbspace-0.3.1/src/dbspace/signal/dLFP/diff_amp_model.py
+-rw-r--r--   0        0        0       78 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/signal/dLFP/gcr.py
+-rw-r--r--   0        0        0     5823 2023-03-23 02:41:01.048262 dbspace-0.3.1/src/dbspace/signal/dLFP/impedances.py
+-rwxr-xr-x   0        0        0     5167 2022-08-28 03:15:25.333525 dbspace-0.3.1/src/dbspace/signal/dLFP/ipg_stim.py
+-rw-r--r--   0        0        0     8569 2023-03-23 02:41:01.048262 dbspace-0.3.1/src/dbspace/signal/dLFP/sig_amp_model.py
+-rw-r--r--   0        0        0     2066 2022-03-24 19:21:20.000000 dbspace-0.3.1/src/dbspace/signal/hots.py
+-rw-r--r--   0        0        0    14892 2023-03-23 02:41:01.051595 dbspace-0.3.1/src/dbspace/signal/oscillations.py
+-rwxr-xr-x   0        0        0    10777 2023-03-23 02:41:01.051595 dbspace-0.3.1/src/dbspace/signal/spot_check.py
+-rw-r--r--   0        0        0        0 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/utils/__init__.py
+-rw-r--r--   0        0        0      149 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/utils/costs.py
+-rw-r--r--   0        0        0      309 2022-03-31 05:39:38.000000 dbspace-0.3.1/src/dbspace/utils/functions.py
+-rw-r--r--   0        0        0        0 2022-04-02 03:47:19.000000 dbspace-0.3.1/src/dbspace/utils/io/brPY/__init__.py
+-rw-r--r--   0        0        0     2776 2022-04-02 03:47:19.000000 dbspace-0.3.1/src/dbspace/utils/io/brPY/brMiscFxns.py
+-rw-r--r--   0        0        0    71040 2022-04-02 03:47:19.000000 dbspace-0.3.1/src/dbspace/utils/io/brPY/brpylib.py
+-rw-r--r--   0        0        0      511 2022-03-24 19:21:20.000000 dbspace-0.3.1/src/dbspace/utils/io/br_io.py
+-rw-r--r--   0        0        0        0 2022-03-24 19:21:20.000000 dbspace-0.3.1/src/dbspace/utils/io/deeg_io.py
+-rw-r--r--   0        0        0      725 2023-03-23 02:41:01.051595 dbspace-0.3.1/src/dbspace/utils/io/pcs.py
+-rw-r--r--   0        0        0        0 2022-03-24 19:21:20.000000 dbspace-0.3.1/src/dbspace/utils/io/xlt_io.py
+-rw-r--r--   0        0        0     1068 2022-08-18 21:40:04.047089 dbspace-0.3.1/src/dbspace/utils/r_pca/LICENSE
+-rw-r--r--   0        0        0        0 2022-08-18 21:40:04.047089 dbspace-0.3.1/src/dbspace/utils/r_pca/__init__.py
+-rw-r--r--   0        0        0     2641 2023-05-17 02:58:17.701501 dbspace-0.3.1/src/dbspace/utils/r_pca/robust_pca.py
+-rw-r--r--   0        0        0     1323 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/utils/stats.py
+-rw-r--r--   0        0        0      170 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/utils/structures.py
+-rw-r--r--   0        0        0    10586 2022-03-31 20:14:31.000000 dbspace-0.3.1/src/dbspace/viz/MM/EEG_Viz.py
+-rw-r--r--   0        0        0     2801 2022-04-02 03:47:19.000000 dbspace-0.3.1/src/dbspace/viz/MM/intraop.py
+-rw-r--r--   0        0        0        0 2022-03-23 22:30:19.000000 dbspace-0.3.1/src/dbspace/viz/TF/TS_spectrogram.py
+-rw-r--r--   0        0        0        0 2022-04-02 03:47:19.000000 dbspace-0.3.1/src/dbspace/viz/__init__.py
+-rw-r--r--   0        0        0      832 1970-01-01 00:00:00.000000 dbspace-0.3.1/PKG-INFO
```

### Comparing `dbspace-0.2.1/LICENSE` & `dbspace-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/pyproject.toml` & `dbspace-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "DBSpace"
-version = "0.2.1"
+version = "0.3.1"
 description = "Library for data-congruent, model-centric DBS Research"
 authors = ["Vineet Tiruvadi <vineet.tiruvadi@gmail.com>"]
 license = "GLPv3"
 
 [tool.poetry.dependencies]
 python = "^3.8.12"
 numpy = "^1.21.2"
```

### Comparing `dbspace-0.2.1/src/dbspace/__testing__/readout/DSV.py` & `dbspace-0.3.1/src/dbspace/__testing__/readout/DSV.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/control/DTI.py` & `dbspace-0.3.1/src/dbspace/control/DTI.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/control/DTI_support.py` & `dbspace-0.3.1/src/dbspace/control/DTI_support.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/control/VirtTract.py` & `dbspace-0.3.1/src/dbspace/control/VirtTract.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/control/dyn_osc.py` & `dbspace-0.3.1/src/dbspace/control/dyn_osc.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/control/network_action.py` & `dbspace-0.3.1/src/dbspace/control/network_action.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/control/offline_segments.py` & `dbspace-0.3.1/src/dbspace/control/offline_segments.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,32 +17,37 @@
 import matplotlib.pyplot as plt
 import mne
 import numpy as np
 import scipy.signal as sig
 import scipy.stats as stats
 
 import sklearn
-from dbspace.signal.oscillations import calc_feats, FEAT_DICT, DEFAULT_FEAT_ORDER, gen_psd
+from dbspace.signal.oscillations import (
+    calc_feats,
+    FEAT_DICT,
+    DEFAULT_FEAT_ORDER,
+    gen_psd,
+)
 from dbspace.utils.structures import nestdict
 from dbspace.viz.MM import EEG_Viz
 from scipy.io import loadmat
 from sklearn import mixture, svm
 from sklearn.decomposition import PCA, FastICA
 from sklearn.metrics import auc, confusion_matrix, roc_auc_score, roc_curve
 from sklearn.model_selection import StratifiedKFold, learning_curve
 from sklearn.utils import resample
 from statsmodels import robust
 import json
 import logging
-sys.path.append("/home/virati/Dropbox/projects/libs/robust-pca/")
-import r_pca
+from dbspace.utils.r_pca.robust_pca import rpca
 
 #%%
 #%%
 
+
 class network_action_dEEG:
     keys_of_interest = {"OnT": ["Off_3", "BONT"], "OffT": ["Off_3", "BOFT"]}
 
     def __init__(
         self,
         pts,
         config_file=None,
@@ -89,26 +94,32 @@
         self.targeting_config = Targeting
 
     def gen_output_variables(self):
         # CHECK IF we're still using ANY of these
 
         # sloppy containers for the outputs of our analyses
         self.psd_trans = {
-            pt: {condit: {epoch: [] for epoch in self.keys_of_interest} for condit in self.condits}
+            pt: {
+                condit: {epoch: [] for epoch in self.keys_of_interest}
+                for condit in self.condits
+            }
             for pt in self.do_pts
         }
         self.PSD_diff = {
             pt: {condit: [] for condit in self.condits} for pt in self.do_pts
         }
         self.PSD_var = {
             pt: {condit: [] for condit in self.condits} for pt in self.do_pts
         }
 
         self.Feat_trans = {
-            pt: {condit: {epoch: [] for epoch in self.keys_of_interest} for condit in self.condits}
+            pt: {
+                condit: {epoch: [] for epoch in self.keys_of_interest}
+                for condit in self.condits
+            }
             for pt in self.do_pts
         }
         self.Feat_diff = {
             pt: {condit: [] for condit in self.condits} for pt in self.do_pts
         }
         self.Feat_var = {
             pt: {condit: [] for condit in self.condits} for pt in self.do_pts
@@ -176,15 +187,17 @@
                     seg_psds = gen_psd(
                         data_dict, Fs=self.fs, nfft=self.donfft, polyord=polyorder
                     )
 
                     # gotta flatten the DICTIONARY, so have to do it carefully
                     PSD_matr = np.array([seg_psds[ch] for ch in self.ch_order_list])
 
-                    OSC_matr = np.zeros((seg_psds[0].shape[0], 257, len(DEFAULT_FEAT_ORDER)))
+                    OSC_matr = np.zeros(
+                        (seg_psds[0].shape[0], 257, len(DEFAULT_FEAT_ORDER))
+                    )
                     # middle_osc = {chann:seg_psd for chann,seg_psd in seg_psds.items}
                     middle_osc = np.array([seg_psds[ch] for ch in range(257)])
 
                     # have to go to each segment due to code
                     for ss in range(seg_psds[0].shape[0]):
                         try:
                             state_return = calc_feats(middle_osc[:, ss, :], self.fvect)[
@@ -260,15 +273,16 @@
                     BL[pt][condit] = np.median(
                         self.osc_dict[pt][condit]["Off_3"], axis=0
                     )
                 except:
                     pdb.set_trace()
                 # Now, go to each segment during stim and subtract the BL for that
                 response[pt][condit] = (
-                    self.osc_dict[pt][condit][self.keys_of_interest[condit][1]] - BL[pt][condit]
+                    self.osc_dict[pt][condit][self.keys_of_interest[condit][1]]
+                    - BL[pt][condit]
                 )
 
         self.targ_response = response
 
     def response_stats(self, band="Alpha", plot=False):
         band_idx = DEFAULT_FEAT_ORDER.index(band)
         response_diff_stats = {pt: [] for pt in self.do_pts}
@@ -342,42 +356,51 @@
     """Generate the pooled/ensemble segment response matrices -> dict"""
 
     def pool_patients(self):
         print("Pooling Patient Observations")
         self.osc_bl_norm = {
             pt: {
                 condit: self.osc_dict[pt][condit][self.keys_of_interest[condit][1]]
-                - np.median(self.osc_dict[pt][condit][self.keys_of_interest[condit][0]], axis=0)
+                - np.median(
+                    self.osc_dict[pt][condit][self.keys_of_interest[condit][0]], axis=0
+                )
                 for condit in self.condits
             }
             for pt in self.do_pts
         }
         self.osc_bl_norm["POOL"] = {
             condit: np.concatenate(
                 [
                     self.osc_dict[pt][condit][self.keys_of_interest[condit][1]]
-                    - np.median(self.osc_dict[pt][condit][self.keys_of_interest[condit][0]], axis=0)
+                    - np.median(
+                        self.osc_dict[pt][condit][self.keys_of_interest[condit][0]],
+                        axis=0,
+                    )
                     for pt in self.do_pts
                 ]
             )
             for condit in self.condits
         }
 
         self.osc_stim = nestdict()
         self.osc_stim = {
             pt: {
-                condit: 10 ** (self.osc_dict[pt][condit][self.keys_of_interest[condit][1]] / 10)
+                condit: 10
+                ** (self.osc_dict[pt][condit][self.keys_of_interest[condit][1]] / 10)
                 for condit in self.condits
             }
             for pt in self.do_pts
         }
         self.osc_stim["POOL"] = {
             condit: np.concatenate(
                 [
-                    10 ** (self.osc_dict[pt][condit][self.keys_of_interest[condit][1]] / 10)
+                    10
+                    ** (
+                        self.osc_dict[pt][condit][self.keys_of_interest[condit][1]] / 10
+                    )
                     for pt in self.do_pts
                 ]
             )
             for condit in self.condits
         }
 
     def plot_psd(self, pt, condit, epoch):
@@ -446,21 +469,27 @@
                 # distribution for pre-stimulation period
                 # pdb.set_trace()
                 baseline_distr = []
                 stim_distr = []
                 for ii in range(100):
                     bl_rand_idx = random.sample(
                         range(
-                            0, self.osc_dict[pt][condit][self.keys_of_interest[condit][0]].shape[0]
+                            0,
+                            self.osc_dict[pt][condit][
+                                self.keys_of_interest[condit][0]
+                            ].shape[0],
                         ),
                         10,
                     )
                     stim_rand_idx = random.sample(
                         range(
-                            0, self.osc_dict[pt][condit][self.keys_of_interest[condit][1]].shape[0]
+                            0,
+                            self.osc_dict[pt][condit][
+                                self.keys_of_interest[condit][1]
+                            ].shape[0],
                         ),
                         10,
                     )
 
                     baseline_distr.append(
                         np.mean(
                             self.osc_dict[pt][condit][self.keys_of_interest[condit][0]][
```

### Comparing `dbspace-0.2.1/src/dbspace/control/stream_buffers.py` & `dbspace-0.3.1/src/dbspace/control/stream_buffers.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/readout/BR_DataFrame.py` & `dbspace-0.3.1/src/dbspace/readout/BR_DataFrame.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/readout/ClinVect.py` & `dbspace-0.3.1/src/dbspace/readout/ClinVect.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 import json
 from collections import defaultdict
 import numpy as np
 import sys
 
-from dbspace.utils.r_pca import r_pca
+from dbspace.utils.r_pca import robust_pca
 import dbspace as dbo
 from dbspace.utils.structures import nestdict
 from dbspace.utils.stats import pca
 
 import scipy.stats as stats
 import scipy.signal as sig
 import scipy.io as sio
@@ -98,15 +98,15 @@
 
             # lump it into a big observation vector AS WELL and do the rPCA on the large one later
             allptX.append(sX)
 
             min_changes = 100
             for ll, lmbda_s in enumerate(np.linspace(0.3, 0.5, 50)):
                 # lmbda = 0.33 did very well here
-                RPCA = r_pca.R_pca(sX, lmbda=lmbda_s)
+                RPCA = robust_pca.rpca(sX, lmbda=lmbda_s)
                 L, S = RPCA.fit()
                 Srcomp, Srevals, Srevecs = pca(S)
                 Lrcomp, Lrevals, Lrevecs = pca(L)
 
                 # compare sparse component numbers of nonzero
                 # derivative is best bet here
                 sdiff = np.diff(Srcomp, axis=0)[
@@ -128,15 +128,15 @@
             opt_lam_dict[pat] = {
                 "Deviation": min_changes,
                 "Lambda": best_lmbda_s,
                 "Sparseness": opt_sparseness,
             }
 
             # We have the "optimal" lambda now and we'll do the final rPCA to generate our components
-            RPCA = r_pca.R_pca(sX, lmbda=opt_lam_dict[pat]["Lambda"])
+            RPCA = robust_pca.rpca(sX, lmbda=opt_lam_dict[pat]["Lambda"])
             L, S = RPCA.fit()
             Srcomp, Srevals, Srevecs = pca(S)
             Lrcomp, Lrevals, Lrevecs = pca(L)
 
             # This generates our DSC scores which are just the negative of the mean of the low rank component
             DSC_scores = -np.mean(Lrcomp[:, :], axis=1)
 
@@ -406,15 +406,15 @@
 
             # lump it into a big observation vector AS WELL and do the rPCA on the large one later
             allptX.append(sX)
 
             min_changes = 100
             for ll, lmbda_s in enumerate(np.linspace(0.3, 0.5, 50)):
                 # lmbda = 0.33 did very well here
-                RPCA = r_pca.R_pca(sX, lmbda=lmbda_s)
+                RPCA = robust_pca.rpca(sX, lmbda=lmbda_s)
                 L, S = RPCA.fit()
                 Srcomp, Srevals, Srevecs = pca(S)
                 Lrcomp, Lrevals, Lrevecs = pca(L)
 
                 # compare sparse component numbers of nonzero
                 # derivative is best bet here
                 sdiff = np.diff(Srcomp, axis=0)[
@@ -436,15 +436,15 @@
             opt_lam_dict[pat] = {
                 "Deviation": min_changes,
                 "Lambda": best_lmbda_s,
                 "Sparseness": opt_sparseness,
             }
 
             # We have the "optimal" lambda now and we'll do the final rPCA to generate our components
-            RPCA = r_pca.R_pca(sX, lmbda=opt_lam_dict[pat]["Lambda"])
+            RPCA = robust_pca.rpca(sX, lmbda=opt_lam_dict[pat]["Lambda"])
             L, S = RPCA.fit()
             Srcomp, Srevals, Srevecs = pca(S)
             Lrcomp, Lrevals, Lrevecs = pca(L)
 
             # This generates our DSC scores which are just the negative of the mean of the low rank component
             DSC_scores = -np.mean(Lrcomp[:, :], axis=1)
```

### Comparing `dbspace-0.2.1/src/dbspace/readout/OBands.py` & `dbspace-0.3.1/src/dbspace/readout/OBands.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/readout/__pycache__/BR_DataFrame.cpython-37.pyc` & `dbspace-0.3.1/src/dbspace/readout/__pycache__/BR_DataFrame.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/readout/__pycache__/ClinVect.cpython-37.pyc` & `dbspace-0.3.1/src/dbspace/readout/__pycache__/ClinVect.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/readout/__pycache__/DSV.cpython-37.pyc` & `dbspace-0.3.1/src/dbspace/readout/__pycache__/DSV.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/readout/decoder.py` & `dbspace-0.3.1/src/dbspace/readout/decoder.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/readout/phases.py` & `dbspace-0.3.1/src/dbspace/readout/phases.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/signal/PAC/PyPAC.py` & `dbspace-0.3.1/src/dbspace/signal/PAC/PyPAC.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/signal/PAC/SyntheticSignalTesting.py` & `dbspace-0.3.1/src/dbspace/signal/PAC/SyntheticSignalTesting.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/signal/PRE/tree_view.py` & `dbspace-0.3.1/src/dbspace/signal/PRE/tree_view.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/signal/dEEG/neigh_mont.py` & `dbspace-0.3.1/src/dbspace/signal/dEEG/neigh_mont.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/signal/dLFP/brain_amp_model.py` & `dbspace-0.3.1/src/dbspace/signal/dLFP/brain_amp_model.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/signal/dLFP/db_stim.py` & `dbspace-0.3.1/src/dbspace/signal/dLFP/db_stim.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/signal/dLFP/diff_amp_model.py` & `dbspace-0.3.1/src/dbspace/signal/dLFP/diff_amp_model.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/signal/dLFP/impedances.py` & `dbspace-0.3.1/src/dbspace/signal/dLFP/impedances.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/signal/dLFP/ipg_stim.py` & `dbspace-0.3.1/src/dbspace/signal/dLFP/ipg_stim.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/signal/dLFP/sig_amp_model.py` & `dbspace-0.3.1/src/dbspace/signal/dLFP/sig_amp_model.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/signal/hots.py` & `dbspace-0.3.1/src/dbspace/signal/hots.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/signal/oscillations.py` & `dbspace-0.3.1/src/dbspace/signal/oscillations.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/signal/spot_check.py` & `dbspace-0.3.1/src/dbspace/signal/spot_check.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/utils/io/brPY/brMiscFxns.py` & `dbspace-0.3.1/src/dbspace/utils/io/brPY/brMiscFxns.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/utils/io/brPY/brpylib.py` & `dbspace-0.3.1/src/dbspace/utils/io/brPY/brpylib.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/utils/io/pcs.py` & `dbspace-0.3.1/src/dbspace/utils/io/pcs.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/utils/r_pca/LICENSE` & `dbspace-0.3.1/src/dbspace/utils/r_pca/LICENSE`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/utils/r_pca/r_pca.py` & `dbspace-0.3.1/src/dbspace/utils/r_pca/robust_pca.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 try:
     from pylab import plt
 except ImportError:
     print("Unable to import pylab. R_pca.plot_fit() will not work.")
 
 
-class R_pca:
+class rpca:
     def __init__(self, D, mu=None, lmbda=None):
         self.D = D
         self.S = np.zeros(self.D.shape)
         self.Y = np.zeros(self.D.shape)
 
         if mu:
             self.mu = mu
```

### Comparing `dbspace-0.2.1/src/dbspace/utils/stats.py` & `dbspace-0.3.1/src/dbspace/utils/stats.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/viz/MM/EEG_Viz.py` & `dbspace-0.3.1/src/dbspace/viz/MM/EEG_Viz.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/src/dbspace/viz/MM/intraop.py` & `dbspace-0.3.1/src/dbspace/viz/MM/intraop.py`

 * *Files identical despite different names*

### Comparing `dbspace-0.2.1/PKG-INFO` & `dbspace-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbspace
-Version: 0.2.1
+Version: 0.3.1
 Summary: Library for data-congruent, model-centric DBS Research
 License: GLPv3
 Author: Vineet Tiruvadi
 Author-email: vineet.tiruvadi@gmail.com
 Requires-Python: >=3.8.12,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

