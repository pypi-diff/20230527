# Comparing `tmp/PayEquity-0.1.4.tar.gz` & `tmp/PayEquity-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PayEquity-0.1.4.tar", last modified: Wed May 24 01:30:57 2023, max compression
+gzip compressed data, was "PayEquity-0.1.5.tar", last modified: Sat May 27 15:33:53 2023, max compression
```

## Comparing `PayEquity-0.1.4.tar` & `PayEquity-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 01:30:57.868500 PayEquity-0.1.4/
--rw-rw-rw-   0        0        0      541 2023-05-24 01:29:55.000000 PayEquity-0.1.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-05-06 14:58:44.000000 PayEquity-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1087 2022-07-25 19:00:43.000000 PayEquity-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     7576 2023-05-24 01:30:57.867499 PayEquity-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-24 01:30:57.845494 PayEquity-0.1.4/PayEquity.egg-info/
--rw-rw-rw-   0        0        0     7576 2023-05-24 01:30:57.000000 PayEquity-0.1.4/PayEquity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-05-24 01:30:57.000000 PayEquity-0.1.4/PayEquity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 01:30:57.000000 PayEquity-0.1.4/PayEquity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-24 01:30:57.000000 PayEquity-0.1.4/PayEquity.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-24 01:30:57.000000 PayEquity-0.1.4/PayEquity.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7300 2023-02-06 20:33:18.000000 PayEquity-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 01:30:57.860497 PayEquity-0.1.4/payequity/
--rw-rw-rw-   0        0        0    16221 2023-05-06 18:30:03.000000 PayEquity-0.1.4/payequity/Audit.py
--rw-rw-rw-   0        0        0    21932 2023-02-21 20:25:58.000000 PayEquity-0.1.4/payequity/JobGroup.py
--rw-rw-rw-   0        0        0     4276 2023-05-01 01:42:07.000000 PayEquity-0.1.4/payequity/JobGroupEnssemble.py
--rw-rw-rw-   0        0        0    22448 2023-05-24 01:30:47.000000 PayEquity-0.1.4/payequity/Regressor.py
--rw-rw-rw-   0        0        0      176 2022-08-10 16:46:06.000000 PayEquity-0.1.4/payequity/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 01:30:57.866500 PayEquity-0.1.4/payequity/tests/
--rw-rw-rw-   0        0        0        0 2022-07-25 19:50:42.000000 PayEquity-0.1.4/payequity/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2022-07-25 19:55:45.000000 PayEquity-0.1.4/payequity/tests/test_audit.py
--rw-rw-rw-   0        0        0     1714 2022-07-25 20:30:46.000000 PayEquity-0.1.4/payequity/tests/test_job_group.py
--rw-rw-rw-   0        0        0     1799 2022-08-24 14:55:43.000000 PayEquity-0.1.4/payequity/tests/test_job_group_enssemble.py
--rw-rw-rw-   0        0        0        0 2022-07-25 19:55:36.000000 PayEquity-0.1.4/payequity/tests/test_regressor.py
--rw-rw-rw-   0        0        0       21 2023-05-24 01:30:34.000000 PayEquity-0.1.4/payequity/version.py
--rw-rw-rw-   0        0        0       42 2023-05-24 01:30:57.868500 PayEquity-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      837 2023-05-06 14:59:20.000000 PayEquity-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 15:33:53.418177 PayEquity-0.1.5/
+-rw-rw-rw-   0        0        0      654 2023-05-27 15:33:03.000000 PayEquity-0.1.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-05-06 14:58:44.000000 PayEquity-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     1087 2022-07-25 19:00:43.000000 PayEquity-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     7576 2023-05-27 15:33:53.417175 PayEquity-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-27 15:33:53.395171 PayEquity-0.1.5/PayEquity.egg-info/
+-rw-rw-rw-   0        0        0     7576 2023-05-27 15:33:53.000000 PayEquity-0.1.5/PayEquity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-05-27 15:33:53.000000 PayEquity-0.1.5/PayEquity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 15:33:53.000000 PayEquity-0.1.5/PayEquity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-27 15:33:53.000000 PayEquity-0.1.5/PayEquity.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-27 15:33:53.000000 PayEquity-0.1.5/PayEquity.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7300 2023-02-06 20:33:18.000000 PayEquity-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 15:33:53.410174 PayEquity-0.1.5/payequity/
+-rw-rw-rw-   0        0        0    16221 2023-05-06 18:30:03.000000 PayEquity-0.1.5/payequity/Audit.py
+-rw-rw-rw-   0        0        0    21932 2023-02-21 20:25:58.000000 PayEquity-0.1.5/payequity/JobGroup.py
+-rw-rw-rw-   0        0        0     4276 2023-05-01 01:42:07.000000 PayEquity-0.1.5/payequity/JobGroupEnssemble.py
+-rw-rw-rw-   0        0        0    22462 2023-05-27 15:32:06.000000 PayEquity-0.1.5/payequity/Regressor.py
+-rw-rw-rw-   0        0        0      176 2022-08-10 16:46:06.000000 PayEquity-0.1.5/payequity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 15:33:53.416176 PayEquity-0.1.5/payequity/tests/
+-rw-rw-rw-   0        0        0        0 2022-07-25 19:50:42.000000 PayEquity-0.1.5/payequity/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-07-25 19:55:45.000000 PayEquity-0.1.5/payequity/tests/test_audit.py
+-rw-rw-rw-   0        0        0     1714 2022-07-25 20:30:46.000000 PayEquity-0.1.5/payequity/tests/test_job_group.py
+-rw-rw-rw-   0        0        0     1799 2022-08-24 14:55:43.000000 PayEquity-0.1.5/payequity/tests/test_job_group_enssemble.py
+-rw-rw-rw-   0        0        0        0 2022-07-25 19:55:36.000000 PayEquity-0.1.5/payequity/tests/test_regressor.py
+-rw-rw-rw-   0        0        0       21 2023-05-27 15:33:00.000000 PayEquity-0.1.5/payequity/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-27 15:33:53.418177 PayEquity-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      837 2023-05-06 14:59:20.000000 PayEquity-0.1.5/setup.py
```

### Comparing `PayEquity-0.1.4/LICENSE.txt` & `PayEquity-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.4/MANIFEST.in` & `PayEquity-0.1.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.4/PKG-INFO` & `PayEquity-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PayEquity
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pay Equity Library
 Home-page: https://github.com/scunden/pay-equity
 Author: Steven Cunden
 Author-email: slcunden@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `PayEquity-0.1.4/PayEquity.egg-info/PKG-INFO` & `PayEquity-0.1.5/PayEquity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PayEquity
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pay Equity Library
 Home-page: https://github.com/scunden/pay-equity
 Author: Steven Cunden
 Author-email: slcunden@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `PayEquity-0.1.4/PayEquity.egg-info/SOURCES.txt` & `PayEquity-0.1.5/PayEquity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.4/README.md` & `PayEquity-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.4/payequity/Audit.py` & `PayEquity-0.1.5/payequity/Audit.py`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.4/payequity/JobGroup.py` & `PayEquity-0.1.5/payequity/JobGroup.py`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.4/payequity/JobGroupEnssemble.py` & `PayEquity-0.1.5/payequity/JobGroupEnssemble.py`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.4/payequity/Regressor.py` & `PayEquity-0.1.5/payequity/Regressor.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
             return self.hug_iter_coef
 
     def _generate_predictions(self, X, results, alpha=0.05, y=None):
         
         self.logger.debug("Generating predictions")
 
         y = self.y if y is None else y
-        pred = results.get_prediction(X)
+        pred = results.get_prediction(X).astype(float)
         pred = np.exp(pred.summary_frame(alpha=alpha))
         pred = pred[['mean','obs_ci_lower','obs_ci_upper']]
         pred.rename({ 'mean':'Prediction',
                                  'obs_ci_lower':"Lower",
                                  'obs_ci_upper':"Upper"}, 
                                 axis=1, inplace=True)
```

### Comparing `PayEquity-0.1.4/payequity/tests/test_job_group.py` & `PayEquity-0.1.5/payequity/tests/test_job_group.py`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.4/payequity/tests/test_job_group_enssemble.py` & `PayEquity-0.1.5/payequity/tests/test_job_group_enssemble.py`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.4/setup.py` & `PayEquity-0.1.5/setup.py`

 * *Files identical despite different names*

