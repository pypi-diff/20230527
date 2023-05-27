# Comparing `tmp/opstool-0.8.1.tar.gz` & `tmp/opstool-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opstool-0.8.1.tar", last modified: Sun May 14 11:41:34 2023, max compression
+gzip compressed data, was "opstool-0.8.2.tar", last modified: Sat May 27 08:34:15 2023, max compression
```

## Comparing `opstool-0.8.1.tar` & `opstool-0.8.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.289529 opstool-0.8.1/
--rw-rw-rw-   0        0        0    34817 2022-12-02 05:00:10.000000 opstool-0.8.1/LICENCE.txt
--rw-rw-rw-   0        0        0     6424 2023-05-14 11:41:34.289529 opstool-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     6005 2023-03-31 11:53:22.000000 opstool-0.8.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-14 11:41:34.289529 opstool-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1013 2023-05-07 06:04:08.000000 opstool-0.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.258862 opstool-0.8.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.258862 opstool-0.8.1/src/opstool/
--rw-rw-rw-   0        0        0       23 2023-05-14 11:38:49.000000 opstool-0.8.1/src/opstool/__about__.py
--rw-rw-rw-   0        0        0      560 2023-04-29 15:03:24.000000 opstool-0.8.1/src/opstool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.265888 opstool-0.8.1/src/opstool/analysis/
--rw-rw-rw-   0        0        0      147 2023-03-10 09:13:36.000000 opstool-0.8.1/src/opstool/analysis/__init__.py
--rw-rw-rw-   0        0        0    13408 2023-05-02 13:56:05.000000 opstool-0.8.1/src/opstool/analysis/_sec_analysis.py
--rw-rw-rw-   0        0        0    35206 2023-05-02 13:57:14.000000 opstool-0.8.1/src/opstool/analysis/_smart_analyze.py
-drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.273903 opstool-0.8.1/src/opstool/examples/
--rw-rw-rw-   0        0        0   365987 2022-12-25 13:36:57.000000 opstool-0.8.1/src/opstool/examples/ArchBridge.py
--rw-rw-rw-   0        0        0    96069 2023-01-06 03:19:00.000000 opstool-0.8.1/src/opstool/examples/ArchBridge2.py
--rw-rw-rw-   0        0        0   697240 2022-12-25 13:38:38.000000 opstool-0.8.1/src/opstool/examples/CableStayedBridge.py
--rw-rw-rw-   0        0        0   289022 2022-12-25 13:39:18.000000 opstool-0.8.1/src/opstool/examples/Dam.py
--rw-rw-rw-   0        0        0     1699 2022-12-25 13:39:55.000000 opstool-0.8.1/src/opstool/examples/DamBreak.py
--rw-rw-rw-   0        0        0   241484 2022-12-25 13:40:30.000000 opstool-0.8.1/src/opstool/examples/Frame3D.py
--rw-rw-rw-   0        0        0    15435 2023-05-06 11:58:20.000000 opstool-0.8.1/src/opstool/examples/Frame3D2.py
--rw-rw-rw-   0        0        0    54201 2023-05-06 11:47:25.000000 opstool-0.8.1/src/opstool/examples/GridFrame.py
--rw-rw-rw-   0        0        0   901646 2022-12-25 13:41:16.000000 opstool-0.8.1/src/opstool/examples/Igloo.py
--rw-rw-rw-   0        0        0     2102 2022-12-25 13:41:50.000000 opstool-0.8.1/src/opstool/examples/Pier.py
--rw-rw-rw-   0        0        0     1813 2022-12-25 13:42:23.000000 opstool-0.8.1/src/opstool/examples/SDOF.py
--rw-rw-rw-   0        0        0   110248 2022-12-25 13:43:18.000000 opstool-0.8.1/src/opstool/examples/SuspensionBridge.py
--rw-rw-rw-   0        0        0        2 2022-12-02 13:20:45.000000 opstool-0.8.1/src/opstool/examples/__init__.py
--rw-rw-rw-   0        0        0    16275 2023-05-06 19:15:36.000000 opstool-0.8.1/src/opstool/examples/shell3D.py
-drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.273903 opstool-0.8.1/src/opstool/preprocessing/
--rw-rw-rw-   0        0        0      838 2023-04-02 12:08:20.000000 opstool-0.8.1/src/opstool/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2876 2023-05-09 04:18:48.000000 opstool-0.8.1/src/opstool/preprocessing/geom_transf.py
--rw-rw-rw-   0        0        0     2266 2023-05-02 14:30:35.000000 opstool-0.8.1/src/opstool/preprocessing/load.py
-drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.289529 opstool-0.8.1/src/opstool/preprocessing/section/
--rw-rw-rw-   0        0        0      554 2023-04-02 12:05:56.000000 opstool-0.8.1/src/opstool/preprocessing/section/__init__.py
--rw-rw-rw-   0        0        0     1417 2023-05-02 13:57:22.000000 opstool-0.8.1/src/opstool/preprocessing/section/lib_sec_mesh.py
--rw-rw-rw-   0        0        0    60526 2023-05-13 09:31:14.000000 opstool-0.8.1/src/opstool/preprocessing/section/sec_mesh.py
--rw-rw-rw-   0        0        0    26107 2023-05-02 13:57:35.000000 opstool-0.8.1/src/opstool/preprocessing/section/var_sec_mesh.py
--rw-rw-rw-   0        0        0    53330 2023-03-30 08:56:24.000000 opstool-0.8.1/src/opstool/preprocessing/tcl2py.py
--rw-rw-rw-   0        0        0     5490 2023-03-30 08:58:00.000000 opstool-0.8.1/src/opstool/preprocessing/unit_system.py
--rw-rw-rw-   0        0        0     6848 2023-05-06 15:12:02.000000 opstool-0.8.1/src/opstool/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.289529 opstool-0.8.1/src/opstool/vis/
--rw-rw-rw-   0        0        0      494 2023-05-04 17:23:00.000000 opstool-0.8.1/src/opstool/vis/__init__.py
--rw-rw-rw-   0        0        0    31751 2023-05-13 10:15:56.000000 opstool-0.8.1/src/opstool/vis/_get_model_base.py
--rw-rw-rw-   0        0        0   106637 2023-05-14 11:32:12.000000 opstool-0.8.1/src/opstool/vis/_plotly_base.py
--rw-rw-rw-   0        0        0    61888 2023-05-14 11:24:31.000000 opstool-0.8.1/src/opstool/vis/_pyvista_base.py
--rw-rw-rw-   0        0        0    23046 2023-05-04 17:23:18.000000 opstool-0.8.1/src/opstool/vis/fiber_sec_vis.py
--rw-rw-rw-   0        0        0    32818 2023-05-06 16:41:25.000000 opstool-0.8.1/src/opstool/vis/get_model_data.py
--rw-rw-rw-   0        0        0    28069 2023-05-06 14:31:33.000000 opstool-0.8.1/src/opstool/vis/ops_vis_2d.py
--rw-rw-rw-   0        0        0    25267 2023-05-09 06:37:32.000000 opstool-0.8.1/src/opstool/vis/ops_vis_plotly.py
--rw-rw-rw-   0        0        0    21638 2023-05-03 06:58:59.000000 opstool-0.8.1/src/opstool/vis/ops_vis_pyvista.py
--rw-rw-rw-   0        0        0    10257 2023-05-06 12:44:36.000000 opstool-0.8.1/src/opstool/vis/quick_plot.py
--rw-rw-rw-   0        0        0    14099 2023-05-09 07:53:13.000000 opstool-0.8.1/src/opstool/vis/save_tikz.py
-drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.265888 opstool-0.8.1/src/opstool.egg-info/
--rw-rw-rw-   0        0        0     6424 2023-05-14 11:41:34.000000 opstool-0.8.1/src/opstool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1730 2023-05-14 11:41:34.000000 opstool-0.8.1/src/opstool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 11:41:34.000000 opstool-0.8.1/src/opstool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-05-14 11:41:34.000000 opstool-0.8.1/src/opstool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-14 11:41:34.000000 opstool-0.8.1/src/opstool.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.289529 opstool-0.8.1/tests/
--rw-rw-rw-   0        0        0     2002 2023-01-18 14:49:51.000000 opstool-0.8.1/tests/test_dambreak.py
--rw-rw-rw-   0        0        0     1705 2023-03-27 03:00:39.000000 opstool-0.8.1/tests/test_fiber_sec_vis.py
--rw-rw-rw-   0        0        0     2982 2023-05-09 11:18:04.000000 opstool-0.8.1/tests/test_model_vis.py
--rw-rw-rw-   0        0        0     2261 2023-03-29 06:45:30.000000 opstool-0.8.1/tests/test_sec_analysis.py
--rw-rw-rw-   0        0        0    10302 2023-04-03 08:29:31.000000 opstool-0.8.1/tests/test_sec_mesh.py
--rw-rw-rw-   0        0        0      954 2023-05-09 13:39:18.000000 opstool-0.8.1/tests/test_temp.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.546811 opstool-0.8.2/
+-rw-rw-rw-   0        0        0    34817 2022-12-02 05:00:10.000000 opstool-0.8.2/LICENCE.txt
+-rw-rw-rw-   0        0        0     6424 2023-05-27 08:34:15.545965 opstool-0.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6005 2023-03-31 11:53:22.000000 opstool-0.8.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-27 08:34:15.546811 opstool-0.8.2/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2023-05-07 06:04:08.000000 opstool-0.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.509348 opstool-0.8.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.514176 opstool-0.8.2/src/opstool/
+-rw-rw-rw-   0        0        0       23 2023-05-27 08:32:31.000000 opstool-0.8.2/src/opstool/__about__.py
+-rw-rw-rw-   0        0        0      673 2023-05-25 13:37:11.000000 opstool-0.8.2/src/opstool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.518009 opstool-0.8.2/src/opstool/analysis/
+-rw-rw-rw-   0        0        0      147 2023-03-10 09:13:36.000000 opstool-0.8.2/src/opstool/analysis/__init__.py
+-rw-rw-rw-   0        0        0    13408 2023-05-02 13:56:05.000000 opstool-0.8.2/src/opstool/analysis/_sec_analysis.py
+-rw-rw-rw-   0        0        0    35206 2023-05-02 13:57:14.000000 opstool-0.8.2/src/opstool/analysis/_smart_analyze.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.530550 opstool-0.8.2/src/opstool/examples/
+-rw-rw-rw-   0        0        0   365987 2022-12-25 13:36:57.000000 opstool-0.8.2/src/opstool/examples/ArchBridge.py
+-rw-rw-rw-   0        0        0    96069 2023-01-06 03:19:00.000000 opstool-0.8.2/src/opstool/examples/ArchBridge2.py
+-rw-rw-rw-   0        0        0   697240 2022-12-25 13:38:38.000000 opstool-0.8.2/src/opstool/examples/CableStayedBridge.py
+-rw-rw-rw-   0        0        0   289022 2022-12-25 13:39:18.000000 opstool-0.8.2/src/opstool/examples/Dam.py
+-rw-rw-rw-   0        0        0     1699 2022-12-25 13:39:55.000000 opstool-0.8.2/src/opstool/examples/DamBreak.py
+-rw-rw-rw-   0        0        0   241484 2022-12-25 13:40:30.000000 opstool-0.8.2/src/opstool/examples/Frame3D.py
+-rw-rw-rw-   0        0        0    15435 2023-05-06 11:58:20.000000 opstool-0.8.2/src/opstool/examples/Frame3D2.py
+-rw-rw-rw-   0        0        0    54201 2023-05-06 11:47:25.000000 opstool-0.8.2/src/opstool/examples/GridFrame.py
+-rw-rw-rw-   0        0        0   901646 2022-12-25 13:41:16.000000 opstool-0.8.2/src/opstool/examples/Igloo.py
+-rw-rw-rw-   0        0        0     2102 2022-12-25 13:41:50.000000 opstool-0.8.2/src/opstool/examples/Pier.py
+-rw-rw-rw-   0        0        0     1813 2022-12-25 13:42:23.000000 opstool-0.8.2/src/opstool/examples/SDOF.py
+-rw-rw-rw-   0        0        0   110248 2022-12-25 13:43:18.000000 opstool-0.8.2/src/opstool/examples/SuspensionBridge.py
+-rw-rw-rw-   0        0        0        2 2022-12-02 13:20:45.000000 opstool-0.8.2/src/opstool/examples/__init__.py
+-rw-rw-rw-   0        0        0    16275 2023-05-06 19:15:36.000000 opstool-0.8.2/src/opstool/examples/shell3D.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.533314 opstool-0.8.2/src/opstool/preprocessing/
+-rw-rw-rw-   0        0        0      838 2023-04-02 12:08:20.000000 opstool-0.8.2/src/opstool/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2876 2023-05-09 04:18:48.000000 opstool-0.8.2/src/opstool/preprocessing/geom_transf.py
+-rw-rw-rw-   0        0        0     2266 2023-05-02 14:30:35.000000 opstool-0.8.2/src/opstool/preprocessing/load.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.535704 opstool-0.8.2/src/opstool/preprocessing/section/
+-rw-rw-rw-   0        0        0      554 2023-04-02 12:05:56.000000 opstool-0.8.2/src/opstool/preprocessing/section/__init__.py
+-rw-rw-rw-   0        0        0     1417 2023-05-02 13:57:22.000000 opstool-0.8.2/src/opstool/preprocessing/section/lib_sec_mesh.py
+-rw-rw-rw-   0        0        0    60702 2023-05-23 16:16:51.000000 opstool-0.8.2/src/opstool/preprocessing/section/sec_mesh.py
+-rw-rw-rw-   0        0        0    26107 2023-05-02 13:57:35.000000 opstool-0.8.2/src/opstool/preprocessing/section/var_sec_mesh.py
+-rw-rw-rw-   0        0        0    53581 2023-05-26 07:18:07.000000 opstool-0.8.2/src/opstool/preprocessing/tcl2py.py
+-rw-rw-rw-   0        0        0     5490 2023-03-30 08:58:00.000000 opstool-0.8.2/src/opstool/preprocessing/unit_system.py
+-rw-rw-rw-   0        0        0     8237 2023-05-25 13:58:46.000000 opstool-0.8.2/src/opstool/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.542641 opstool-0.8.2/src/opstool/vis/
+-rw-rw-rw-   0        0        0      494 2023-05-04 17:23:00.000000 opstool-0.8.2/src/opstool/vis/__init__.py
+-rw-rw-rw-   0        0        0    32555 2023-05-23 03:42:47.000000 opstool-0.8.2/src/opstool/vis/_get_model_base.py
+-rw-rw-rw-   0        0        0   106783 2023-05-24 15:15:18.000000 opstool-0.8.2/src/opstool/vis/_plotly_base.py
+-rw-rw-rw-   0        0        0    66174 2023-05-15 10:48:39.000000 opstool-0.8.2/src/opstool/vis/_pyvista_base.py
+-rw-rw-rw-   0        0        0    23046 2023-05-04 17:23:18.000000 opstool-0.8.2/src/opstool/vis/fiber_sec_vis.py
+-rw-rw-rw-   0        0        0    32015 2023-05-23 03:43:37.000000 opstool-0.8.2/src/opstool/vis/get_model_data.py
+-rw-rw-rw-   0        0        0    28645 2023-05-25 15:40:29.000000 opstool-0.8.2/src/opstool/vis/ops_vis_2d.py
+-rw-rw-rw-   0        0        0    25267 2023-05-09 06:37:32.000000 opstool-0.8.2/src/opstool/vis/ops_vis_plotly.py
+-rw-rw-rw-   0        0        0    24060 2023-05-15 10:10:38.000000 opstool-0.8.2/src/opstool/vis/ops_vis_pyvista.py
+-rw-rw-rw-   0        0        0    10494 2023-05-25 15:43:46.000000 opstool-0.8.2/src/opstool/vis/quick_plot.py
+-rw-rw-rw-   0        0        0    14099 2023-05-09 07:53:13.000000 opstool-0.8.2/src/opstool/vis/save_tikz.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.515729 opstool-0.8.2/src/opstool.egg-info/
+-rw-rw-rw-   0        0        0     6424 2023-05-27 08:34:15.000000 opstool-0.8.2/src/opstool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1730 2023-05-27 08:34:15.000000 opstool-0.8.2/src/opstool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 08:34:15.000000 opstool-0.8.2/src/opstool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-05-27 08:34:15.000000 opstool-0.8.2/src/opstool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-27 08:34:15.000000 opstool-0.8.2/src/opstool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 08:34:15.545965 opstool-0.8.2/tests/
+-rw-rw-rw-   0        0        0     2002 2023-01-18 14:49:51.000000 opstool-0.8.2/tests/test_dambreak.py
+-rw-rw-rw-   0        0        0     1705 2023-03-27 03:00:39.000000 opstool-0.8.2/tests/test_fiber_sec_vis.py
+-rw-rw-rw-   0        0        0     2981 2023-05-25 15:47:16.000000 opstool-0.8.2/tests/test_model_vis.py
+-rw-rw-rw-   0        0        0     2261 2023-03-29 06:45:30.000000 opstool-0.8.2/tests/test_sec_analysis.py
+-rw-rw-rw-   0        0        0    10302 2023-04-03 08:29:31.000000 opstool-0.8.2/tests/test_sec_mesh.py
+-rw-rw-rw-   0        0        0      954 2023-05-09 13:39:18.000000 opstool-0.8.2/tests/test_temp.py
```

### Comparing `opstool-0.8.1/LICENCE.txt` & `opstool-0.8.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/PKG-INFO` & `opstool-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opstool
-Version: 0.8.1
+Version: 0.8.2
 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992
 Author: Yexiang Yan
 Author-email: yexiang_yan@outlook.com
 License: GPL Licence
 Keywords: OpenSees Visualization Seismic Simulation
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opstool Version: 0.8.1 Summary: openseespy toolbox
+Metadata-Version: 2.1 Name: opstool Version: 0.8.2 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992 Author: Yexiang Yan Author-email:
 yexiang_yan@outlook.com License: GPL Licence Keywords: OpenSees Visualization
 Seismic Simulation Platform: any Classifier: Programming Language :: Python ::
 3 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENCE.txt
                                     opstool
            modelling, visualization, post-processing for OpenSeesPy.
```

### Comparing `opstool-0.8.1/README.md` & `opstool-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/setup.py` & `opstool-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/__init__.py` & `opstool-0.8.2/src/opstool/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .__about__ import __version__
-from .utils import load_ops_examples
+from .utils import load_ops_examples, run_model, print_version, add_ops_hints_file
 from .vis import *
 from .analysis import *
 from .preprocessing import *
 from . import vis, preprocessing, analysis
 
 
 _membs = dict()
@@ -13,9 +13,12 @@
             _membs[name] = getattr(mod, name)
 cur_dict = globals()
 cur_dict.update(_membs)
 _membs_all = vis.__all__ + preprocessing.__all__ + analysis.__all__
 
 __all__ = [
     "load_ops_examples",
+    "run_model",
+    "print_version",
+    "add_ops_hints_file",
     "__version__",
 ] + _membs_all
```

### Comparing `opstool-0.8.1/src/opstool/analysis/_sec_analysis.py` & `opstool-0.8.2/src/opstool/analysis/_sec_analysis.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/analysis/_smart_analyze.py` & `opstool-0.8.2/src/opstool/analysis/_smart_analyze.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/examples/ArchBridge.py` & `opstool-0.8.2/src/opstool/examples/ArchBridge.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/examples/ArchBridge2.py` & `opstool-0.8.2/src/opstool/examples/ArchBridge2.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/examples/CableStayedBridge.py` & `opstool-0.8.2/src/opstool/examples/CableStayedBridge.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/examples/Dam.py` & `opstool-0.8.2/src/opstool/examples/Dam.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/examples/DamBreak.py` & `opstool-0.8.2/src/opstool/examples/DamBreak.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/examples/Frame3D.py` & `opstool-0.8.2/src/opstool/examples/Frame3D.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/examples/Frame3D2.py` & `opstool-0.8.2/src/opstool/examples/Frame3D2.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/examples/GridFrame.py` & `opstool-0.8.2/src/opstool/examples/GridFrame.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/examples/Igloo.py` & `opstool-0.8.2/src/opstool/examples/Igloo.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/examples/Pier.py` & `opstool-0.8.2/src/opstool/examples/Pier.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/examples/SDOF.py` & `opstool-0.8.2/src/opstool/examples/SDOF.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/examples/SuspensionBridge.py` & `opstool-0.8.2/src/opstool/examples/SuspensionBridge.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/examples/shell3D.py` & `opstool-0.8.2/src/opstool/examples/shell3D.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/preprocessing/__init__.py` & `opstool-0.8.2/src/opstool/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/preprocessing/geom_transf.py` & `opstool-0.8.2/src/opstool/preprocessing/geom_transf.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/preprocessing/load.py` & `opstool-0.8.2/src/opstool/preprocessing/load.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/preprocessing/section/__init__.py` & `opstool-0.8.2/src/opstool/preprocessing/section/__init__.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/preprocessing/section/lib_sec_mesh.py` & `opstool-0.8.2/src/opstool/preprocessing/section/lib_sec_mesh.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/preprocessing/section/sec_mesh.py` & `opstool-0.8.2/src/opstool/preprocessing/section/sec_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,22 +156,25 @@
         mesh_sizes = []
         if not self.color_map:
             for name in self.group_map.keys():
                 self.color_map[name] = _get_random_color()
         # mat_names = [geom.material.name for geom in self.group_map.values()]
         for name, geom in self.group_map.items():
             # if len(mat_names) != len(set(mat_names)):
-            geom.material = add_material(
-                name=name,
-                elastic_modulus=geom.material.elastic_modulus,
-                poissons_ratio=geom.material.poissons_ratio,
-                yield_strength=geom.material.yield_strength,
-                density=geom.material.density,
-                color=self.color_map[name],
-            )
+            if geom.material is None:
+                geom.material = add_material(name=name, color=self.color_map[name])
+            else:
+                geom.material = add_material(
+                    name=name,
+                    elastic_modulus=geom.material.elastic_modulus,
+                    poissons_ratio=geom.material.poissons_ratio,
+                    yield_strength=geom.material.yield_strength,
+                    density=geom.material.density,
+                    color=self.color_map[name],
+                )
             geoms.append(geom)
             mesh_sizes.append(self.mesh_size_map[name])
         geom_obj = CompoundGeometry(geoms)
         mesh_obj = geom_obj.create_mesh(mesh_sizes=mesh_sizes)
         self.section = Section(geom_obj, time_info=False)
         self.mesh_obj = mesh_obj.mesh
         self._get_mesh_data()
@@ -1051,34 +1054,34 @@
     def _to_tcl(self, output_path, names, sec_tag, gj):
         with open(output_path, "w+") as output:
             output.write("# This document was created from opstool.SecMesh\n")
             output.write("# Author: Yexiang Yan  yexiang_yan@outlook.com\n\n")
             output.write(f"set secTag {sec_tag}\n")
             temp = "{"
             output.write(
-                f"section fiberSec $secTag -GJ {gj}{temp};    # Define the fiber section\n"
+                f"section fiberSec $secTag -GJ {gj} {temp};    # Define the fiber section\n"
             )
             for name in names:
                 centers = self.centers_map[name]
                 areas = self.areas_map[name]
                 mat_tag = self.mat_ops_map[name]
                 for center, area in zip(centers, areas):
                     output.write(
-                        f"    fiber  {center[0]:.3E}  {center[1]:.3E}  {area:.3E}  {mat_tag}\n"
+                        f"    fiber  {center[0]:.8E}  {center[1]:.8E}  {area:.8E}  {mat_tag}\n"
                     )
             # rebar
             for data in self.rebar_data:
                 output.write("    # Define Rebar\n")
                 rebar_xy = data["rebar_xy"]
                 dia = data["dia"]
                 mat_tag = data["matTag"]
                 for xy in rebar_xy:
                     area = np.pi / 4 * dia**2
                     output.write(
-                        f"    fiber {xy[0]:.3E} {xy[1]:.3E} {area:.3E} {mat_tag}\n"
+                        f"    fiber {xy[0]:.8E} {xy[1]:.8E} {area:.8E} {mat_tag}\n"
                     )
             output.write("};    # end of fibersection definition")
 
     def _to_py(self, output_path, names, sec_tag, gj):
         with open(output_path, "w+") as output:
             output.write("# This document was created from opstool.SecMesh\n")
             output.write("# Author: Yexiang Yan  yexiang_yan@outlook.com\n\n")
@@ -1088,26 +1091,26 @@
             )
             for name in names:
                 centers = self.centers_map[name]
                 areas = self.areas_map[name]
                 mat_tag = self.mat_ops_map[name]
                 for center, area in zip(centers, areas):
                     output.write(
-                        f"ops.fiber({center[0]:.3E}, {center[1]:.3E}, {area:.3E}, {mat_tag})\n"
+                        f"ops.fiber({center[0]:.8E}, {center[1]:.8E}, {area:.8E}, {mat_tag})\n"
                     )
             # rebar
             for data in self.rebar_data:
                 output.write("# Define Rebar\n")
                 rebar_xy = data["rebar_xy"]
                 dia = data["dia"]
                 mat_tag = data["matTag"]
                 for xy in rebar_xy:
                     area = np.pi / 4 * dia**2
                     output.write(
-                        f"ops.fiber({xy[0]:.3E}, {xy[1]:.3E}, {area:.3E}, {mat_tag})\n"
+                        f"ops.fiber({xy[0]:.8E}, {xy[1]:.8E}, {area:.8E}, {mat_tag})\n"
                     )
 
     def view(
         self,
         fill: bool = True,
         engine: str = "plotly",
         save_html: str = "SecMesh.html",
```

### Comparing `opstool-0.8.1/src/opstool/preprocessing/section/var_sec_mesh.py` & `opstool-0.8.2/src/opstool/preprocessing/section/var_sec_mesh.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/preprocessing/tcl2py.py` & `opstool-0.8.2/src/opstool/preprocessing/tcl2py.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,23 +54,27 @@
     try:
         interp.eval(tcl_src)
     finally:
         with open(output_file, mode='w', encoding=encoding) as fw:
             fw.write(import_txt)
             for line in contents:
                 fw.write(line + "\n")
+    print(f"[bold #34bf49]OpenSeesPy[/bold #34bf49] file "
+          f"[bold #d20962]{output_file}[/bold #d20962] has been created successfully!")
 
 
 def _TclInterp(prefix):
     interp = tkinter.Tcl()
     contents = []
 
     def _puts(*args):
-        # print(*args)
-        pass
+        if len(args) == 1:
+            contents.append(f"print('{args[0]}')")
+        else:
+            contents.append(f"print{args}")
 
     def _wipe(*args):
         args = _remove_commit(args)
         args = tuple([_type_convert(i) for i in args])
         contents.append(f"{prefix}wipe{args}")
 
     def _model(*args):
```

### Comparing `opstool-0.8.1/src/opstool/preprocessing/unit_system.py` & `opstool-0.8.2/src/opstool/preprocessing/unit_system.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/vis/_get_model_base.py` & `opstool-0.8.2/src/opstool/vis/_get_model_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -759,14 +759,37 @@
         # for ii in range(6):
         #     local_forces[ii] = -local_forces[ii]
         beam_resp_steps.append(local_forces)
     beam_resp_steps = np.array(beam_resp_steps)
     return beam_resp_steps
 
 
+def get_fiber_sec_data(ele_tag: int, sec_tag: int = 1):
+    """Get the fiber sec data for a beam element.
+
+    Parameters
+    ----------
+    ele_tag: int
+        The element tag to which the section is to be displayed.
+    sec_tag: int
+        Which integration point section is displayed, tag from 1 from segment i to j.
+
+    Returns
+    -------
+    fiber_data: ArrayLike
+    """
+    # Extract fiber data using eleResponse() command
+    fiber_data = ops.eleResponse(ele_tag, "section", sec_tag, "fiberData2")
+    if len(fiber_data) == 0:
+        fiber_data = ops.eleResponse(ele_tag, "section", "fiberData2")
+    # From column 1 to 6: "yCoord", "zCoord", "area", 'mat', "stress", "strain"
+    fiber_data = np.reshape(fiber_data, (-1, 6))  # to six columns
+    return fiber_data
+
+
 def sort_xy(x, y):
     """
     Sort points counterclockwise
     """
     x0 = np.mean(x)
     y0 = np.mean(y)
     r = np.sqrt((x - x0) ** 2 + (y - y0) ** 2)
```

### Comparing `opstool-0.8.1/src/opstool/vis/_plotly_base.py` & `opstool-0.8.2/src/opstool/vis/_plotly_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,16 @@
     show_ele_label: bool = False,
     show_local_crd: bool = False,
     local_crd_alpha: float = 1.0,
     show_fix_node: bool = True,
     fix_node_alpha: float = 1.0,
     show_load: bool = False,
     load_alpha: float = 1.0,
+    show_beam_sec: bool = False,
+    beam_sec_paras: dict = None,
     show_constrain_dof: bool = False,
     label_size: float = 8,
     show_outline: bool = True,
     opacity: float = 1.0,
     save_html: str = "ModelVis.html",
 ):
     # read hdf5 file
@@ -129,14 +131,16 @@
         show_ele_label=show_ele_label,
         show_local_crd=show_local_crd,
         local_crd_alpha=local_crd_alpha,
         show_fix_node=show_fix_node,
         fix_node_alpha=fix_node_alpha,
         show_load=show_load,
         load_alpha=load_alpha,
+        show_beam_sec=show_beam_sec,
+        beam_sec_paras=beam_sec_paras,
         show_constrain_dof=show_constrain_dof,
         label_size=label_size,
         show_outline=show_outline,
         opacity=opacity,
     )
     if save_html:
         if not save_html.endswith(".html"):
```

### Comparing `opstool-0.8.1/src/opstool/vis/_pyvista_base.py` & `opstool-0.8.2/src/opstool/vis/_pyvista_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import h5py
 import numpy as np
 import matplotlib.pyplot as plt
 import pyvista as pv
 
 from ..utils import check_file, shape_dict
 
-
 def _model_vis(
     obj,
     input_file: str = "ModelData.hdf5",
     show_node_label: bool = False,
     show_ele_label: bool = False,
     label_size: float = 10,
     show_local_crd: bool = False,
@@ -1216,14 +1215,141 @@
     plotter.view_isometric()
     if np.max(model_dims) <= 2:
         plotter.view_xy(negative=False)
     if save_fig:
         plotter.save_graphic(save_fig)
     plotter.enable_anti_aliasing("msaa")
     plotter.show(title=obj.title)
+    plotter.close()
+
+
+def _deform_peak_vis(
+    obj,
+    input_file: str = "NodeRespStepData-1.hdf5",
+    response: str = "disp",
+    alpha: float = 1.0,
+    show_outline: bool = False,
+    show_origin: bool = False,
+    show_face_line: bool = True,
+    opacity: float = 1,
+    save_fig: str = "DefoVis.svg",
+):
+    resp_type = response.lower()
+    if resp_type not in ["disp", "vel", "accel"]:
+        raise ValueError("response must be 'disp', 'vel', or 'accel'!")
+
+    filename = obj.out_dir + "/" + input_file
+    model_info_steps = dict()
+    cell_steps = dict()
+    node_resp_steps = dict()
+    with h5py.File(filename, "r") as f:
+        n = int(f["Nsteps"][...])
+        grp1 = f["ModelInfoSteps"]
+        grp2 = f["CellSteps"]
+        for name, value_ in grp1.items():
+            model_info_steps[name] = value_[...]
+        for name, value_ in grp2.items():
+            cell_steps[name] = value_[...]
+        grp3 = f["NodeRespSteps"]
+        for name, value_ in grp3.items():
+            temp = []
+            for i in range(n):
+                temp.append(value_[f"step{i + 1}"][...])
+            node_resp_steps[name] = temp
+    # ! max response
+    idxs = np.argmax(np.abs(node_resp_steps[resp_type]), axis=0)
+    node_resp = np.zeros_like(idxs, dtype=float)
+    for i in range(idxs.shape[0]):
+        for j in range(idxs.shape[1]):
+            node_resp[i, j] = node_resp_steps[resp_type][idxs[i, j]][i, j]
+    max_resps = np.amax(np.abs(node_resp_steps[resp_type]), axis=0)
+    scalars = np.sqrt(np.sum(max_resps**2, axis=1))
+    cmin, cmax = np.min(scalars), np.max(scalars)
+    bounds = model_info_steps["bound"]
+    model_dims = model_info_steps["model_dims"]
+    # scale factor
+    if resp_type == "disp":
+        max_bound = np.max(
+            [bounds[1] - bounds[0], bounds[3] - bounds[2], bounds[5] - bounds[4]]
+        )
+        value = np.max(scalars)
+        alpha_ = max_bound / obj.bound_fact / value
+        alpha_ = alpha_ * alpha if alpha else alpha_
+    else:
+        alpha_ = 0
+    # ------------------------------------------------------------------------
+    # Start plot
+    # -------------------------------------------------------------------------
+    plotter = pv.Plotter(notebook=obj.notebook, line_smoothing=True)
+    node_nodeform_coords = model_info_steps["coord_no_deform"]
+    lines_cells = cell_steps["all_lines"]
+    faces_cells = cell_steps["all_faces"]
+    node_deform_coords = alpha_ * node_resp + node_nodeform_coords
+    _ = _generate_all_mesh(
+        plotter,
+        node_deform_coords,
+        scalars,
+        opacity,
+        obj.color_map,
+        lines_cells=lines_cells,
+        face_cells=faces_cells,
+        show_origin=show_origin,
+        points_origin=node_nodeform_coords,
+        point_size=obj.point_size,
+        line_width=obj.line_width,
+        show_face_line=show_face_line,
+        clim=[cmin, cmax],
+    )
+
+    plotter.add_scalar_bar(fmt="%.3e", n_labels=10, label_font_size=12)
+
+    plotter.add_text(
+        "OpenSees 3D View",
+        position="upper_left",
+        shadow=True,
+        font_size=18,
+        # color="black",
+        font="courier",
+    )
+    plotter.add_text(
+        "peak of {}\n"
+        "min.x = {:.3E}  max.x = {:.3E}\n"
+        "min.y = {:.3E}  max.y = {:.3E}\n"
+        "min.z = {:.3E}  max.z = {:.3E}\n".format(
+            response,
+            np.min(node_resp[:, 0]),
+            np.max(node_resp[:, 0]),
+            np.min(node_resp[:, 1]),
+            np.max(node_resp[:, 1]),
+            np.min(node_resp[:, 2]),
+            np.max(node_resp[:, 2]),
+        ),
+        position="upper_right",
+        shadow=True,
+        font_size=14,
+        # color="black",
+        font="courier",
+    )
+
+    if show_outline:
+        plotter.show_bounds(
+            grid=False,
+            location="outer",
+            bounds=bounds,
+            show_zaxis=True,
+            # color="black",
+        )
+    plotter.add_axes()
+    plotter.view_isometric()
+    if np.max(model_dims) <= 2:
+        plotter.view_xy(negative=False)
+    if save_fig:
+        plotter.save_graphic(save_fig)
+    plotter.enable_anti_aliasing("msaa")
+    plotter.show(title=obj.title)
     plotter.close()
 
 
 def _deform_anim(
     obj,
     input_file: str = "NodeRespStepData-1.hdf5",
     response: str = "disp",
```

### Comparing `opstool-0.8.1/src/opstool/vis/fiber_sec_vis.py` & `opstool-0.8.2/src/opstool/vis/fiber_sec_vis.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/vis/get_model_data.py` & `opstool-0.8.2/src/opstool/vis/get_model_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 import os
 from itertools import cycle
 from typing import Union
 
 import h5py
 import numpy as np
 import openseespy.opensees as ops
-from numpy.typing import ArrayLike
 from rich import print
 
 from ..utils import check_file
 from ._get_model_base import (
     get_beam_info2,
     get_beam_resp,
     get_model_info,
     get_node_coords,
     get_node_react,
     get_node_resp,
+    get_fiber_sec_data,
 )
 
 
 class GetFEMdata:
     """
     Get the data in the ``openseespy`` current domain.
 
@@ -318,17 +318,17 @@
         ops.reactions(*args)
         fixed_nodes = ops.getFixedNodes()
         self.node_react_steps.append(get_node_react(fixed_nodes))
         self.step_react_track += 1
         # --------------------------------
         if save_file:
             if (
-                self.step_node_track >= num_steps
-                or ops.getTime() >= total_time
-                or stop_cond
+                self.step_node_track >= num_steps or
+                ops.getTime() >= total_time or
+                stop_cond
             ):
                 output_filename = self.out_dir + "/" + save_file
                 self._save_node_react_step(output_filename, "w")
                 print(
                     f"Node reaction data saved in [bold {next(self.colors_cycle)}]{output_filename}[/]!"
                 )
 
@@ -405,15 +405,15 @@
         """
         if save_file:
             check_file(save_file, [".hdf5", ".h5", ".he5"])
         if model_update:
             self.get_model_data(save_file=False)
         else:
             if not self.get_model_data_finished:
-                self.get_model_data()
+                self.get_model_data(save_file=False)
 
         node_tags = self.model_info["NodeTags"]
         (node_disp, node_vel, node_accel, node_deform_coord) = get_node_resp(node_tags)
 
         self.node_resp_steps["disp"].append(node_disp)
         self.node_resp_steps["vel"].append(node_vel)
         self.node_resp_steps["accel"].append(node_accel)
@@ -435,17 +435,17 @@
                 self.cells_steps.update(self.cells)
         # --------------------------------
         self.model_update = model_update
         self.step_node_track += 1
         # --------------------------------
         if save_file:
             if (
-                self.step_node_track >= num_steps
-                or ops.getTime() >= total_time
-                or stop_cond
+                self.step_node_track >= num_steps or
+                ops.getTime() >= total_time or
+                stop_cond
             ):
                 output_filename = self.out_dir + "/" + save_file
                 self._save_node_resp_step(output_filename, "w")
                 print(
                     f"Node response data saved in [bold {next(self.colors_cycle)}]{output_filename}[/]!"
                 )
 
@@ -542,17 +542,17 @@
         beam_resp_steps = get_beam_resp(beam_tags)
         self.beam_resp_step["localForces"].append(beam_resp_steps)
         # ----------------------------------------------------------------
         self.step_beam_track += 1
         # ------------------------------------------
         if save_file:
             if (
-                self.step_beam_track >= num_steps
-                or ops.getTime() >= total_time
-                or stop_cond
+                self.step_beam_track >= num_steps or
+                ops.getTime() >= total_time or
+                stop_cond
             ):
                 output_filename = self.out_dir + "/" + save_file
                 self._save_frame_resp_step(output_filename, "w")
                 print(
                     f"Frame elements response data saved in [bold {next(self.colors_cycle)}]{output_filename}[/]!"
                 )
 
@@ -601,15 +601,15 @@
             self.fiber_sec_data[key] = []
 
         # get data
         for ele_sec_i in self.fiber_sec_tags:
             ele_tag = ele_sec_i[0]
             sec_tag = ele_sec_i[1]
             key = f"{ele_sec_i[0]}-{ele_sec_i[1]}"
-            fiber_data = _get_fiber_sec_data(ele_tag, sec_tag)
+            fiber_data = get_fiber_sec_data(ele_tag, sec_tag)
             self.fiber_sec_data[key] = fiber_data
         # ---------------------------------------------
         if save_file:
             output_filename = self.out_dir + "/" + save_file
             with h5py.File(output_filename, "w") as f:
                 for name, value in self.fiber_sec_data.items():
                     f.create_dataset(name, data=value)
@@ -661,15 +661,15 @@
                 key = f"{ele_sec_i[0]}-{ele_sec_i[1]}"
                 self.fiber_sec_step_data[key] = []
 
         for ele_sec_i in self.fiber_sec_tags:
             ele_tag = ele_sec_i[0]
             sec_tag = ele_sec_i[1]
             key = f"{ele_sec_i[0]}-{ele_sec_i[1]}"
-            fiber_data = _get_fiber_sec_data(ele_tag, sec_tag)
+            fiber_data = get_fiber_sec_data(ele_tag, sec_tag)
             defo_fo = ops.eleResponse(
                 ele_tag, "section", sec_tag, "forceAndDeformation"
             )
             if len(defo_fo) == 4:
                 defo_fo = [
                     defo_fo[0],
                     defo_fo[1],
@@ -684,17 +684,17 @@
             data = np.hstack([fiber_data, sec_defo_fo])
             self.fiber_sec_step_data[key].append(data)
         # ------------------------
         self.step_fiber_track += 1
         # ------------------------
         if save_file:
             if (
-                self.step_fiber_track >= num_steps
-                or ops.getTime() >= total_time
-                or stop_cond
+                self.step_fiber_track >= num_steps or
+                ops.getTime() >= total_time or
+                stop_cond
             ):
                 output_filename = self.out_dir + "/" + save_file
                 self._save_fiber_resp_step(output_filename, "w")
                 print(
                     f"Fiber section responses data saved in [bold {next(self.colors_cycle)}]{output_filename}[/]!"
                 )
 
@@ -770,30 +770,7 @@
         if self.fiber_sec_step_data:
             self._save_fiber_resp_step(filename, "a")
         if reset_state:
             self.reset_steps_state()
         print(
             f"All responses data saved in [bold {next(self.colors_cycle)}]{filename}[/]!"
         )
-
-
-def _get_fiber_sec_data(ele_tag: int, sec_tag: int = 1):
-    """Get the fiber sec data for a beam element.
-
-    Parameters
-    ----------
-    ele_tag: int
-        The element tag to which the section is to be displayed.
-    sec_tag: int
-        Which integration point section is displayed, tag from 1 from segment i to j.
-
-    Returns
-    -------
-    fiber_data: ArrayLike
-    """
-    # Extract fiber data using eleResponse() command
-    fiber_data = ops.eleResponse(ele_tag, "section", sec_tag, "fiberData2")
-    if len(fiber_data) == 0:
-        fiber_data = ops.eleResponse(ele_tag, "section", "fiberData2")
-    # From column 1 to 6: "yCoord", "zCoord", "area", 'mat', "stress", "strain"
-    fiber_data = np.reshape(fiber_data, (-1, 6))  # to six columns
-    return fiber_data
```

### Comparing `opstool-0.8.1/src/opstool/vis/ops_vis_2d.py` & `opstool-0.8.2/src/opstool/vis/ops_vis_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,15 @@
         input_file: str = "EigenData.hdf5",
         subplots: bool = False,
         alpha: float = 1.0,
         show_outline: bool = False,
         show_origin: bool = False,
         show_point: bool = False,
         show_face_line: bool = True,
+        show_cmap: bool = True,
         opacity: float = 1.0,
     ):
         filename = self.out_dir + "/" + input_file
         eigen_data = dict()
         with h5py.File(filename, "r") as f:
             grp = f["EigenInfo"]
             for name, value in grp.items():
@@ -220,14 +221,15 @@
         aspect_ratio = (np.max(ps_[:, 1]) - np.min(ps_[:, 1])) / (
             np.max(ps_[:, 0]) - np.min(ps_[:, 0])
         )
         if aspect_ratio > 2:
             aspect_ratio = 2.0
         if aspect_ratio < 0.5:
             aspect_ratio = 0.5
+        cmap = self.color_map if show_cmap else None
 
         def create_mesh(value_i):
             step = int(round(value_i)) - 1
             eigen_veci = eigenvector[step]
             value_i = np.max(np.sqrt(np.sum(eigen_veci**2, axis=1)))
             alpha_i = eigen_data["max_bound"] / self.bound_fact / value_i
             alpha_i *= alpha if alpha is not None else alpha_i
@@ -236,55 +238,67 @@
 
             ax.clear()
             if show_point:
                 _plot_point(
                     ax,
                     eigen_pointsi,
                     self.point_size,
-                    cmap=self.color_map,
+                    color="blue",
+                    cmap=cmap,
                     scalars=scalarsi,
                     clim=(np.min(scalarsi), np.max(scalarsi)),
                 )
             if len(eigen_data["all_lines"]) > 0:
                 _plot_line(
                     ax,
                     eigen_pointsi,
                     _reshape_cell(eigen_data["all_lines"]),
                     width=self.line_width,
-                    cmap=self.color_map,
+                    color="blue",
+                    cmap=cmap,
                     n_segs=50,
                     scalars=scalarsi,
                     clim=(np.min(scalarsi), np.max(scalarsi)),
                 )
                 if show_origin:
                     _plot_line(
                         ax,
                         eigen_data["coord_no_deform"],
                         _reshape_cell(eigen_data["all_lines"]),
                         width=self.line_width / 3,
                         color="gray",
                     )
             if len(eigen_data["all_faces"]) > 0:
-                _plot_face(
-                    ax,
-                    eigen_pointsi,
-                    _reshape_cell(eigen_data["all_faces"]),
-                    lw=0.75,
-                    cmap=self.color_map,
-                    opacity=opacity,
-                    scalars=scalarsi,
-                    clim=(np.min(scalarsi), np.max(scalarsi)),
-                )
-                if show_face_line:
+                if cmap:
+                    _plot_face(
+                        ax,
+                        eigen_pointsi,
+                        _reshape_cell(eigen_data["all_faces"]),
+                        lw=0.75,
+                        color="blue",
+                        cmap=self.color_map,
+                        opacity=opacity,
+                        scalars=scalarsi,
+                        clim=(np.min(scalarsi), np.max(scalarsi)),
+                    )
+                    if show_face_line:
+                        _plot_wireframe(
+                            ax,
+                            eigen_pointsi,
+                            _reshape_cell(eigen_data["all_faces"]),
+                            lw=self.line_width / 5,
+                            color="k",
+                        )
+                else:
                     _plot_wireframe(
                         ax,
                         eigen_pointsi,
                         _reshape_cell(eigen_data["all_faces"]),
-                        lw=self.line_width / 5,
-                        color="k",
+                        lw=self.line_width,
+                        color="blue",
                     )
                 if show_origin:
                     _plot_wireframe(
                         ax,
                         eigen_data["coord_no_deform"],
                         _reshape_cell(eigen_data["all_faces"]),
                         lw=self.line_width / 3,
```

### Comparing `opstool-0.8.1/src/opstool/vis/ops_vis_plotly.py` & `opstool-0.8.2/src/opstool/vis/ops_vis_plotly.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool/vis/ops_vis_pyvista.py` & `opstool-0.8.2/src/opstool/vis/ops_vis_pyvista.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import pyvista as pv
 
 from ..utils import check_file
 from ._pyvista_base import (
     _deform_anim,
     _deform_vis,
+    _deform_peak_vis,
     _eigen_anim,
     _eigen_vis,
     _frame_resp_vis,
     _model_vis,
     _react_vis,
 )
 
@@ -512,14 +513,81 @@
             opacity=opacity,
             framerate=framerate,
             show_face_line=show_face_line,
             save_fig=save_fig,
             model_update=model_update,
         )
 
+    def deform_peak_vis(
+        self,
+        input_file: str = "NodeRespStepData-1.hdf5",
+        response: str = "disp",
+        alpha: float = 1.0,
+        show_outline: bool = False,
+        show_origin: bool = False,
+        show_face_line: bool = True,
+        opacity: float = 1,
+        save_fig: str = "DefoVis.svg"
+    ):
+        """Visualize the node peak responses of the model at all analysis steps.
+        That is to say, the response of each node in each direction is the absolute maximum
+        value in all its time steps.
+
+        .. note::
+            This method does not support the arg `model_update`,
+            i.e. model nodes and elements do not change during the analysis.
+
+        Parameters
+        ----------
+        input_file: str, default = "NodeRespStepData-1.hdf5",
+            The filename that node responses data saved by
+            :py:meth:`opstool.vis.GetFEMdata.get_node_resp_step`.
+
+            .. warning::
+                Be careful not to include any path, only filename,
+                the file will be loaded from the directory ``results_dir``.
+
+        response: str, default='disp'
+            Response type. Optional, "disp", "vel", "accel".
+        alpha: float, default=1.0
+            Scaling factor, scale further on existing display.
+        show_outline: bool, default=False
+            Whether to display the axes.
+        show_origin: bool, default=False
+            Whether to show undeformed shape.
+        show_face_line: bool, default=True
+            If True, the edges of plate and solid elements will be displayed.
+        opacity: float, default=1.0
+            Plane and solid element transparency.
+        save_fig: str, default='DefoVis.svg'
+            The file name to output. If False or None, the file will not be generated.
+            The supported formats are:
+
+            * '.svg'
+            * '.eps'
+            * '.ps'
+            * '.pdf'
+            * '.tex'
+
+        Returns
+        --------
+        None
+        """
+        _deform_peak_vis(
+            self,
+            input_file=input_file,
+            response=response,
+            alpha=alpha,
+            show_outline=show_outline,
+            show_origin=show_origin,
+            show_face_line=show_face_line,
+            opacity=opacity,
+            save_fig=save_fig
+        )
+
     def frame_resp_vis(
         self,
         input_file: str = "BeamRespStepData-1.hdf5",
         ele_tags: list = None,
         slider: bool = False,
         response: str = "Mz",
         show_values=True,
```

### Comparing `opstool-0.8.1/src/opstool/vis/quick_plot.py` & `opstool-0.8.2/src/opstool/vis/quick_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -163,14 +163,15 @@
     subplots: bool = False,
     link_views: bool = True,
     alpha: float = 1.0,
     show_outline: bool = False,
     show_origin: bool = False,
     opacity: float = 1.0,
     show_face_line: bool = True,
+    show_cmap: bool = True,
 ):
     """Fast eigen visualization.
 
     Parameters
     ----------
     mode_tags: list[int], or tuple[int]
         Mode tags to be shown, if list or tuple [mode1, mode2], display the multiple modes from mode1 to mode2.
@@ -196,14 +197,17 @@
         Whether to display the axes.
     show_origin: bool, default=False
         Whether to show undeformed shape.
     opacity: float, default=1.0
         Plane and solid element transparency.
     show_face_line: bool, default=True
         If True, the edges of plate and solid elements will be displayed.
+    show_cmap: bool, default=True
+        If True, display the cloud plot, else only the deformation with single color.
+        Only supported for `backend="matplotlib"`.
     """
     ModelData = GetFEMdata(results_dir="opstool_output")
     ModelData.get_eigen_data(
         mode_tag=mode_tags[-1], solver=solver, save_file="EigenData.hdf5"
     )
     if backend.lower() == "pyvista":
         opsvis = OpsVisPyvista(
@@ -258,14 +262,15 @@
             input_file="EigenData.hdf5",
             subplots=subplots,
             alpha=alpha,
             show_outline=show_outline,
             show_origin=show_origin,
             opacity=opacity,
             show_face_line=show_face_line,
+            show_cmap=show_cmap,
         )
     else:
         raise ValueError("Arg backend must be one of ['pyvista', 'plotly', 'mpl']!")
 
 
 # def plot_node_resp(disp_file, dof_num, ):
 #     ModelData = GetFEMdata(results_dir="opstool_output")
```

### Comparing `opstool-0.8.1/src/opstool/vis/save_tikz.py` & `opstool-0.8.2/src/opstool/vis/save_tikz.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/src/opstool.egg-info/PKG-INFO` & `opstool-0.8.2/src/opstool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opstool
-Version: 0.8.1
+Version: 0.8.2
 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992
 Author: Yexiang Yan
 Author-email: yexiang_yan@outlook.com
 License: GPL Licence
 Keywords: OpenSees Visualization Seismic Simulation
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opstool Version: 0.8.1 Summary: openseespy toolbox
+Metadata-Version: 2.1 Name: opstool Version: 0.8.2 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992 Author: Yexiang Yan Author-email:
 yexiang_yan@outlook.com License: GPL Licence Keywords: OpenSees Visualization
 Seismic Simulation Platform: any Classifier: Programming Language :: Python ::
 3 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENCE.txt
                                     opstool
            modelling, visualization, post-processing for OpenSeesPy.
```

### Comparing `opstool-0.8.1/src/opstool.egg-info/SOURCES.txt` & `opstool-0.8.2/src/opstool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/tests/test_dambreak.py` & `opstool-0.8.2/tests/test_dambreak.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/tests/test_fiber_sec_vis.py` & `opstool-0.8.2/tests/test_fiber_sec_vis.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/tests/test_model_vis.py` & `opstool-0.8.2/tests/test_model_vis.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # opst.load_ops_examples("SuspensionBridge")
 # opst.plot_model(backend="pyvista")    # or backend="plotly"
 # opst.plot_eigen(mode_tags=[1, 12], backend="pyvista", subplots=True)   # or backend="plotly"
 # opst.gen_grav_load(ts_tag=1, pattern_tag=1, factor=-9.81, direction="Z")
 ModelData = opst.GetFEMdata()
 ModelData.get_model_data()
 ModelData.get_eigen_data(mode_tag=15)
-opsv = opst.OpsVisPyvista(
+opsv = opst.OpsVisPlotly(
     point_size=4,
     line_width=4,
     colors_dict=None,
     color_map="jet",
     on_notebook=False,
     results_dir="opstool_output",
 )
```

### Comparing `opstool-0.8.1/tests/test_sec_analysis.py` & `opstool-0.8.2/tests/test_sec_analysis.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/tests/test_sec_mesh.py` & `opstool-0.8.2/tests/test_sec_mesh.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.1/tests/test_temp.py` & `opstool-0.8.2/tests/test_temp.py`

 * *Files identical despite different names*

