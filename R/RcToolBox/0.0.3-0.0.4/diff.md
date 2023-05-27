# Comparing `tmp/RcToolBox-0.0.3.tar.gz` & `tmp/RcToolBox-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RcToolBox-0.0.3.tar", last modified: Sun Apr  9 10:38:53 2023, max compression
+gzip compressed data, was "RcToolBox-0.0.4.tar", last modified: Sat May 27 09:17:49 2023, max compression
```

## Comparing `RcToolBox-0.0.3.tar` & `RcToolBox-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-09 10:38:53.618720 RcToolBox-0.0.3/
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      223 2023-04-09 10:38:53.617127 RcToolBox-0.0.3/PKG-INFO
-drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-09 10:38:53.565690 RcToolBox-0.0.3/RcToolBox/
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        0 2023-03-07 20:28:07.000000 RcToolBox-0.0.3/RcToolBox/__init__.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     2222 2023-04-04 21:00:33.000000 RcToolBox-0.0.3/RcToolBox/basic_op.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     6647 2023-04-09 10:37:05.000000 RcToolBox-0.0.3/RcToolBox/dataset_op.py
-drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-09 10:38:53.597955 RcToolBox-0.0.3/RcToolBox/draw/
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-05 11:05:14.000000 RcToolBox-0.0.3/RcToolBox/draw/__init__.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     2614 2023-04-09 10:09:08.000000 RcToolBox-0.0.3/RcToolBox/draw/df_plot.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     3737 2023-04-06 22:20:13.000000 RcToolBox-0.0.3/RcToolBox/nifti_op.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     4412 2023-04-01 22:32:30.000000 RcToolBox-0.0.3/RcToolBox/pandas_op.py
-drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-09 10:38:53.611976 RcToolBox-0.0.3/RcToolBox/segmentation/
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-05 11:05:02.000000 RcToolBox-0.0.3/RcToolBox/segmentation/__init__.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     2832 2023-04-09 10:37:38.000000 RcToolBox-0.0.3/RcToolBox/segmentation/evaluation.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     1704 2023-04-09 10:07:40.000000 RcToolBox-0.0.3/RcToolBox/segmentation/metric.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      928 2023-04-09 10:06:45.000000 RcToolBox-0.0.3/RcToolBox/xeon_op.py
-drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-09 10:38:53.589137 RcToolBox-0.0.3/RcToolBox.egg-info/
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      223 2023-04-09 10:38:53.000000 RcToolBox-0.0.3/RcToolBox.egg-info/PKG-INFO
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      464 2023-04-09 10:38:53.000000 RcToolBox-0.0.3/RcToolBox.egg-info/SOURCES.txt
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        1 2023-04-09 10:38:53.000000 RcToolBox-0.0.3/RcToolBox.egg-info/dependency_links.txt
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)       68 2023-04-09 10:38:53.000000 RcToolBox-0.0.3/RcToolBox.egg-info/requires.txt
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)       10 2023-04-09 10:38:53.000000 RcToolBox-0.0.3/RcToolBox.egg-info/top_level.txt
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)       38 2023-04-09 10:38:53.619935 RcToolBox-0.0.3/setup.cfg
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      840 2023-04-09 10:37:18.000000 RcToolBox-0.0.3/setup.py
+drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-05-27 09:17:49.552139 RcToolBox-0.0.4/
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      223 2023-05-27 09:17:49.550529 RcToolBox-0.0.4/PKG-INFO
+drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-05-27 09:17:49.507301 RcToolBox-0.0.4/RcToolBox/
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        0 2023-03-07 20:28:07.000000 RcToolBox-0.0.4/RcToolBox/__init__.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     4075 2023-05-27 09:09:01.000000 RcToolBox-0.0.4/RcToolBox/basic_op.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     6635 2023-04-09 10:46:20.000000 RcToolBox-0.0.4/RcToolBox/dataset_op.py
+drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-05-27 09:17:49.534760 RcToolBox-0.0.4/RcToolBox/draw/
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-05 11:05:14.000000 RcToolBox-0.0.4/RcToolBox/draw/__init__.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     2614 2023-04-09 10:09:08.000000 RcToolBox-0.0.4/RcToolBox/draw/df_plot.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     3737 2023-04-06 22:20:13.000000 RcToolBox-0.0.4/RcToolBox/nifti_op.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     4412 2023-04-01 22:32:30.000000 RcToolBox-0.0.4/RcToolBox/pandas_op.py
+drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-05-27 09:17:49.546235 RcToolBox-0.0.4/RcToolBox/segmentation/
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-05 11:05:02.000000 RcToolBox-0.0.4/RcToolBox/segmentation/__init__.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     2802 2023-04-17 23:00:58.000000 RcToolBox-0.0.4/RcToolBox/segmentation/evaluation.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     1718 2023-05-26 19:08:31.000000 RcToolBox-0.0.4/RcToolBox/segmentation/metric.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      928 2023-04-09 10:06:45.000000 RcToolBox-0.0.4/RcToolBox/xeon_op.py
+drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-05-27 09:17:49.526865 RcToolBox-0.0.4/RcToolBox.egg-info/
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      223 2023-05-27 09:17:49.000000 RcToolBox-0.0.4/RcToolBox.egg-info/PKG-INFO
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      464 2023-05-27 09:17:49.000000 RcToolBox-0.0.4/RcToolBox.egg-info/SOURCES.txt
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        1 2023-05-27 09:17:49.000000 RcToolBox-0.0.4/RcToolBox.egg-info/dependency_links.txt
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)       68 2023-05-27 09:17:49.000000 RcToolBox-0.0.4/RcToolBox.egg-info/requires.txt
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)       10 2023-05-27 09:17:49.000000 RcToolBox-0.0.4/RcToolBox.egg-info/top_level.txt
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)       38 2023-05-27 09:17:49.553180 RcToolBox-0.0.4/setup.cfg
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      840 2023-05-27 09:11:03.000000 RcToolBox-0.0.4/setup.py
```

### Comparing `RcToolBox-0.0.3/RcToolBox/dataset_op.py` & `RcToolBox-0.0.4/RcToolBox/dataset_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # /usr/bin/env python
 import os
 import glob
 import numpy as np
-from RcToolBox.nifti_op import load_nifti, get_nifti_mask_bbox
+from RcToolBox.nifti_op import load_nifti, get_mask_bbox
 from RcToolBox.xeon_op import hardcore_process
 from RcToolBox.pandas_op import generate_dataframe
 from RcToolBox.basic_op import *
 import warnings
 warnings.filterwarnings("ignore")
 
 # calculate file size, return in MB
@@ -82,15 +82,15 @@
             np.sum(mask_npy == i + 1) * img_spacing[0] * img_spacing[1] *
             img_spacing[2])
 
     img_file_size = get_file_size(img_path)
 
     label_num = len(np.unique(mask_npy)) - 1
 
-    foreground_coord = get_nifti_mask_bbox(mask_npy,
+    foreground_coord = get_mask_bbox(mask_npy,
                                            return_mask=False,
                                            return_coord=True)
     bbox_z, bbox_h, bbox_w = foreground_coord[1] - foreground_coord[0], foreground_coord[3] - foreground_coord[2],\
                             foreground_coord[5] - foreground_coord[4]
 
     if len(label_name) == 1:
         return patient_id, img_min, img_max, label_num,  str(round(foreground_ratio,2))+"%",\
```

### Comparing `RcToolBox-0.0.3/RcToolBox/draw/df_plot.py` & `RcToolBox-0.0.4/RcToolBox/draw/df_plot.py`

 * *Files identical despite different names*

### Comparing `RcToolBox-0.0.3/RcToolBox/nifti_op.py` & `RcToolBox-0.0.4/RcToolBox/nifti_op.py`

 * *Files identical despite different names*

### Comparing `RcToolBox-0.0.3/RcToolBox/pandas_op.py` & `RcToolBox-0.0.4/RcToolBox/pandas_op.py`

 * *Files identical despite different names*

### Comparing `RcToolBox-0.0.3/RcToolBox/segmentation/evaluation.py` & `RcToolBox-0.0.4/RcToolBox/segmentation/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import sys
-from metric import cal_dice
-# from RcToolBox.segmentation.metric import cal_dice
+from RcToolBox.segmentation.metric import cal_dice
 from RcToolBox.basic_op import *
 from RcToolBox.xeon_op import hardcore_process
 from RcToolBox.pandas_op import generate_dataframe
 from copy import deepcopy
 import numpy as np
 import pandas as pd
```

### Comparing `RcToolBox-0.0.3/RcToolBox/segmentation/metric.py` & `RcToolBox-0.0.4/RcToolBox/segmentation/metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import sys
 import numpy as np
 from RcToolBox.nifti_op import load_nifti
 
 # From https://github.com/frankkramer-lab/miseval/blob/master/miseval/dice.py
-def cal_dice(patient_id, prediction, groundtruth, num_label, additional_info=None,individual_mean=False):
+def cal_dice(patient_id, prediction, groundtruth, num_label, 
+             additional_info=None,individual_mean=False):
     """_summary_
 
     Parameters
     ----------
     patient_id : str
     prediction : nifti path, np.ndarray
     groundtruth : nifti path, np.ndarray
```

### Comparing `RcToolBox-0.0.3/RcToolBox/xeon_op.py` & `RcToolBox-0.0.4/RcToolBox/xeon_op.py`

 * *Files identical despite different names*

### Comparing `RcToolBox-0.0.3/setup.py` & `RcToolBox-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages            
 
 setup(
     name = "RcToolBox",      # 这里是pip项目发布的名称
-    version = "0.0.3",  # 版本号，数值大的会优先被pip
+    version = "0.0.4",  # 版本号，数值大的会优先被pip
     keywords = ["pip", "RcToolBox"],			# 关键字
     description = "RC personal ToolBox",	# 描述
     long_description = "RC personal ToolBox",
     license = "MIT Licence",		# 许可证
 
     url = "",     #项目相关文件地址，一般是github项目地址即可
     author = "RC",			# 作者
```

