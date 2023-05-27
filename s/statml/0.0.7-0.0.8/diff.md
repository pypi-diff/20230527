# Comparing `tmp/statml-0.0.7.tar.gz` & `tmp/statml-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statml-0.0.7.tar", last modified: Sat May 27 05:46:15 2023, max compression
+gzip compressed data, was "statml-0.0.8.tar", last modified: Sat May 27 13:10:01 2023, max compression
```

## Comparing `statml-0.0.7.tar` & `statml-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,114 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 05:46:15.224240 statml-0.0.7/
--rw-rw-rw-   0        0        0     1091 2023-05-27 03:19:10.000000 statml-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      518 2023-05-27 05:46:15.224240 statml-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       16 2023-05-20 12:40:16.000000 statml-0.0.7/README.md
--rw-rw-rw-   0        0        0      589 2023-05-27 05:41:07.000000 statml-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      247 2023-05-27 05:46:15.224240 statml-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 05:46:15.207600 statml-0.0.7/statml/
--rw-rw-rw-   0        0        0       21 2023-05-27 05:41:20.000000 statml-0.0.7/statml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 05:46:15.191975 statml-0.0.7/statml/onebook/
-drwxrwxrwx   0        0        0        0 2023-05-27 05:46:15.207600 statml-0.0.7/statml/onebook/1/
--rw-rw-rw-   0        0        0    49814 2023-05-07 11:48:47.000000 statml-0.0.7/statml/onebook/1/Ch2-2.ipynb
--rw-rw-rw-   0        0        0     3621 2023-05-21 11:57:23.000000 statml-0.0.7/statml/playchat.py
--rw-rw-rw-   0        0        0     5209 2023-05-21 11:26:39.000000 statml-0.0.7/statml/stepwise.py
-drwxrwxrwx   0        0        0        0 2023-05-27 05:46:15.207600 statml-0.0.7/statml.egg-info/
--rw-rw-rw-   0        0        0      518 2023-05-27 05:46:15.000000 statml-0.0.7/statml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-05-27 05:46:15.000000 statml-0.0.7/statml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 05:46:15.000000 statml-0.0.7/statml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-27 05:46:15.000000 statml-0.0.7/statml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 13:10:01.295782 statml-0.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-05-27 03:19:10.000000 statml-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-05-27 12:52:37.000000 statml-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      518 2023-05-27 13:10:01.295782 statml-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2023-05-20 12:40:16.000000 statml-0.0.8/README.md
+-rw-rw-rw-   0        0        0      589 2023-05-27 13:09:28.000000 statml-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      262 2023-05-27 13:10:01.295782 statml-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 13:10:01.186403 statml-0.0.8/statml/
+-rw-rw-rw-   0        0        0       21 2023-05-27 12:30:10.000000 statml-0.0.8/statml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 13:10:01.170822 statml-0.0.8/statml/data/
+drwxrwxrwx   0        0        0        0 2023-05-27 13:10:01.186403 statml-0.0.8/statml/data/one/
+drwxrwxrwx   0        0        0        0 2023-05-27 13:10:01.202027 statml-0.0.8/statml/data/one/2_datahandling/
+-rw-rw-rw-   0        0        0     4194 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/2_datahandling/Ch2-10.ipynb
+-rw-rw-rw-   0        0        0     1516 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/2_datahandling/Ch2-11.ipynb
+-rw-rw-rw-   0        0        0    11787 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/2_datahandling/Ch2-2.ipynb
+-rw-rw-rw-   0        0        0     7124 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/2_datahandling/Ch2-3.ipynb
+-rw-rw-rw-   0        0        0    13002 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/2_datahandling/Ch2-4.ipynb
+-rw-rw-rw-   0        0        0     1750 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/2_datahandling/Ch2-5.ipynb
+-rw-rw-rw-   0        0        0     8234 2023-05-27 12:27:41.000000 statml-0.0.8/statml/data/one/2_datahandling/Ch2-6.ipynb
+-rw-rw-rw-   0        0        0     2343 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/2_datahandling/Ch2-7.ipynb
+-rw-rw-rw-   0        0        0     5652 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/2_datahandling/Ch2-8,9.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-27 13:10:01.217650 statml-0.0.8/statml/data/one/3_eda/
+-rw-rw-rw-   0        0        0    57733 2023-05-27 12:27:41.000000 statml-0.0.8/statml/data/one/3_eda/Ch3.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-27 13:10:01.217650 statml-0.0.8/statml/data/one/4_preprocessing/
+-rw-rw-rw-   0        0        0    29100 2023-05-27 12:27:41.000000 statml-0.0.8/statml/data/one/4_preprocessing/Ch 4.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-27 13:10:01.217650 statml-0.0.8/statml/data/one/5_mrprocessing/
+-rw-rw-rw-   0        0        0     5493 2023-05-27 12:27:41.000000 statml-0.0.8/statml/data/one/5_mrprocessing/5_4_testing.ipynb
+-rw-rw-rw-   0        0        0     4675 2023-05-27 12:27:41.000000 statml-0.0.8/statml/data/one/5_mrprocessing/5_class.ipynb
+-rw-rw-rw-   0        0        0     5765 2023-05-27 12:27:41.000000 statml-0.0.8/statml/data/one/5_mrprocessing/5_reg.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-27 13:10:01.217650 statml-0.0.8/statml/data/one/6_mr/
+-rw-rw-rw-   0        0        0   237534 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/6_mr/6_10_nivebasian.ipynb
+-rw-rw-rw-   0        0        0   116961 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/6_mr/6_1_simplereg.ipynb
+-rw-rw-rw-   0        0        0    83246 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/6_mr/6_2_poly.ipynb
+-rw-rw-rw-   0        0        0   324355 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/6_mr/6_3_multi.ipynb
+-rw-rw-rw-   0        0        0    84827 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/6_mr/6_4_log.ipynb
+-rw-rw-rw-   0        0        0   588569 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/6_mr/6_6_svm.ipynb
+-rw-rw-rw-   0        0        0    93036 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/6_mr/6_7_knn.ipynb
+-rw-rw-rw-   0        0        0   639417 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/6_mr/6_8_ds.ipynb
+-rw-rw-rw-   0        0        0   254837 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/6_mr/6_9_ansble.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-27 13:10:01.233276 statml-0.0.8/statml/data/one/7_stats/
+-rw-rw-rw-   0        0        0     7828 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/7_stats/7_2_ttest.ipynb
+-rw-rw-rw-   0        0        0     6897 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/7_stats/7_3_ANOVA.ipynb
+-rw-rw-rw-   0        0        0     3334 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/7_stats/7_4_cross.ipynb
+-rw-rw-rw-   0        0        0    12826 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/7_stats/7_5_reg.ipynb
+-rw-rw-rw-   0        0        0     7799 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/7_stats/7_6_custer.ipynb
+-rw-rw-rw-   0        0        0     6616 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/7_stats/7_7_same.ipynb
+-rw-rw-rw-   0        0        0     8324 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/7_stats/7_8_time.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-27 13:10:01.248906 statml-0.0.8/statml/data/one/8_training/
+-rw-rw-rw-   0        0        0    16443 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/8_training/1_mr.ipynb
+-rw-rw-rw-   0        0        0    11124 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/8_training/1_stat.ipynb
+-rw-rw-rw-   0        0        0    20562 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/8_training/2_mr.ipynb
+-rw-rw-rw-   0        0        0    10214 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/8_training/2_stat.ipynb
+-rw-rw-rw-   0        0        0    13438 2023-05-27 12:27:42.000000 statml-0.0.8/statml/data/one/8_training/3_mrstat.ipynb
+-rw-rw-rw-   0        0        0     5698 2023-05-27 12:27:43.000000 statml-0.0.8/statml/data/one/8_training/4_basian.ipynb
+-rw-rw-rw-   0        0        0    16799 2023-05-27 12:27:43.000000 statml-0.0.8/statml/data/one/8_training/4_cross.ipynb
+-rw-rw-rw-   0        0        0     3615 2023-05-27 12:27:43.000000 statml-0.0.8/statml/data/one/8_training/4_defect.ipynb
+-rw-rw-rw-   0        0        0    15953 2023-05-27 12:27:43.000000 statml-0.0.8/statml/data/one/8_training/4_eda.ipynb
+-rw-rw-rw-   0        0        0     4244 2023-05-27 12:27:43.000000 statml-0.0.8/statml/data/one/8_training/4_price.ipynb
+-rw-rw-rw-   0        0        0     7736 2023-05-27 12:27:43.000000 statml-0.0.8/statml/data/one/8_training/4_ttest.ipynb
+-rw-rw-rw-   0        0        0     2568 2023-05-27 12:27:43.000000 statml-0.0.8/statml/data/one/8_training/5_5.ipynb
+-rw-rw-rw-   0        0        0     1820 2023-05-27 12:27:43.000000 statml-0.0.8/statml/data/one/8_training/5_6.ipynb
+-rw-rw-rw-   0        0        0     3531 2023-05-27 12:27:43.000000 statml-0.0.8/statml/data/one/8_training/5_7.ipynb
+-rw-rw-rw-   0        0        0     3708 2023-05-27 12:27:43.000000 statml-0.0.8/statml/data/one/8_training/5_8.ipynb
+-rw-rw-rw-   0        0        0     4019 2023-05-27 12:27:43.000000 statml-0.0.8/statml/data/one/8_training/5_9.ipynb
+-rw-rw-rw-   0        0        0    25150 2023-05-27 12:27:43.000000 statml-0.0.8/statml/data/one/8_training/5_eda.ipynb
+-rw-rw-rw-   0        0        0    19408 2023-05-27 12:27:43.000000 statml-0.0.8/statml/data/one/8_training/student_data.csv
+drwxrwxrwx   0        0        0        0 2023-05-27 13:10:01.295782 statml-0.0.8/statml/data/one/data/
+-rw-rw-rw-   0        0        0   125272 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/data/26_problem1.csv
+-rw-rw-rw-   0        0        0       84 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/data/26_problem4.csv
+-rw-rw-rw-   0        0        0      316 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/26_problem6.csv
+-rw-rw-rw-   0        0        0    10572 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/data/26_problem7.csv
+-rw-rw-rw-   0        0        0    91664 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/data/27_problem.csv
+-rw-rw-rw-   0        0        0   400565 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/27_problem1.csv
+-rw-rw-rw-   0        0        0       81 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/data/27_problem7.csv
+-rw-rw-rw-   0        0        0    91664 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/data/27_problem8.csv
+-rw-rw-rw-   0        0        0      756 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/data/27_problem9.csv
+-rw-rw-rw-   0        0        0    26717 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/data/CarPrice_Assignment.csv
+-rw-rw-rw-   0        0        0    12872 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/data/Cars93.csv
+-rw-rw-rw-   0        0        0  1387602 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/data/Skyserver.csv
+-rw-rw-rw-   0        0        0     1387 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/data/USArrests.csv
+-rw-rw-rw-   0        0        0     1020 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/arima_data.csv
+-rw-rw-rw-   0        0        0  1989197 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/avocado.csv
+-rw-rw-rw-   0        0        0   761835 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/bodyPerformance.csv
+-rw-rw-rw-   0        0        0   124571 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/breast-cancer.csv
+-rw-rw-rw-   0        0        0     1904 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/cats.csv
+-rw-rw-rw-   0        0        0     5063 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/cereal.csv
+-rw-rw-rw-   0        0        0    12128 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/classification.csv
+-rw-rw-rw-   0        0        0    84134 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/credit_final.csv
+-rw-rw-rw-   0        0        0    23873 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/diabetes.csv
+-rw-rw-rw-   0        0        0    24062 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/diabetes_for_test.csv
+-rw-rw-rw-   0        0        0   526049 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/groceries.csv
+-rw-rw-rw-   0        0        0   809103 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/hotel_bookings.csv
+-rw-rw-rw-   0        0        0    23930 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/indian_liver_patient.csv
+-rw-rw-rw-   0        0        0    55628 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/insurance.csv
+-rw-rw-rw-   0        0        0     4616 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/data/iris.csv
+-rw-rw-rw-   0        0        0  2113257 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/kc_house_data.csv
+-rw-rw-rw-   0        0        0     2326 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/lot_quality.csv
+-rw-rw-rw-   0        0        0     2893 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/data/metalicity.csv
+-rw-rw-rw-   0        0        0     1816 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/mtcars.csv
+-rw-rw-rw-   0        0        0    19760 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/pre_student.csv
+-rw-rw-rw-   0        0        0    93062 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/data/seoul_corona19.csv
+-rw-rw-rw-   0        0        0   504016 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/spam.csv
+-rw-rw-rw-   0        0        0    42379 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/student-mat.csv
+-rw-rw-rw-   0        0        0    93220 2023-05-27 12:27:39.000000 statml-0.0.8/statml/data/one/data/student-por.csv
+-rw-rw-rw-   0        0        0    19408 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/data/student_data.csv
+-rw-rw-rw-   0        0        0    12417 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/data/student_data_2.csv
+-rw-rw-rw-   0        0        0    42999 2023-05-27 12:27:40.000000 statml-0.0.8/statml/data/one/data/titanic.csv
+-rw-rw-rw-   0        0        0     3621 2023-05-21 11:57:23.000000 statml-0.0.8/statml/playchat.py
+-rw-rw-rw-   0        0        0     5209 2023-05-21 11:26:39.000000 statml-0.0.8/statml/stepwise.py
+drwxrwxrwx   0        0        0        0 2023-05-27 13:10:01.202027 statml-0.0.8/statml.egg-info/
+-rw-rw-rw-   0        0        0      518 2023-05-27 13:10:01.000000 statml-0.0.8/statml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3624 2023-05-27 13:10:01.000000 statml-0.0.8/statml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 13:10:01.000000 statml-0.0.8/statml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-27 13:10:01.000000 statml-0.0.8/statml.egg-info/top_level.txt
```

### Comparing `statml-0.0.7/LICENSE` & `statml-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `statml-0.0.7/PKG-INFO` & `statml-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statml
-Version: 0.0.7
+Version: 0.0.8
 Summary: stat and ml example
 Author-email: HaeWoon <likesea7@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `statml-0.0.7/pyproject.toml` & `statml-0.0.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "statml"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="HaeWoon", email="likesea7@gmail.com" },
 ]
 description = "stat and ml example"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `statml-0.0.7/statml/playchat.py` & `statml-0.0.8/statml/playchat.py`

 * *Files identical despite different names*

### Comparing `statml-0.0.7/statml/stepwise.py` & `statml-0.0.8/statml/stepwise.py`

 * *Files identical despite different names*

### Comparing `statml-0.0.7/statml.egg-info/PKG-INFO` & `statml-0.0.8/statml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statml
-Version: 0.0.7
+Version: 0.0.8
 Summary: stat and ml example
 Author-email: HaeWoon <likesea7@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

