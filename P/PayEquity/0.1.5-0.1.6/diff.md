# Comparing `tmp/PayEquity-0.1.5.tar.gz` & `tmp/PayEquity-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PayEquity-0.1.5.tar", last modified: Sat May 27 15:33:53 2023, max compression
+gzip compressed data, was "PayEquity-0.1.6.tar", last modified: Sat May 27 15:45:13 2023, max compression
```

## Comparing `PayEquity-0.1.5.tar` & `PayEquity-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 15:33:53.418177 PayEquity-0.1.5/
--rw-rw-rw-   0        0        0      654 2023-05-27 15:33:03.000000 PayEquity-0.1.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-05-06 14:58:44.000000 PayEquity-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0     1087 2022-07-25 19:00:43.000000 PayEquity-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     7576 2023-05-27 15:33:53.417175 PayEquity-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-27 15:33:53.395171 PayEquity-0.1.5/PayEquity.egg-info/
--rw-rw-rw-   0        0        0     7576 2023-05-27 15:33:53.000000 PayEquity-0.1.5/PayEquity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-05-27 15:33:53.000000 PayEquity-0.1.5/PayEquity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 15:33:53.000000 PayEquity-0.1.5/PayEquity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-27 15:33:53.000000 PayEquity-0.1.5/PayEquity.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-27 15:33:53.000000 PayEquity-0.1.5/PayEquity.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7300 2023-02-06 20:33:18.000000 PayEquity-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 15:33:53.410174 PayEquity-0.1.5/payequity/
--rw-rw-rw-   0        0        0    16221 2023-05-06 18:30:03.000000 PayEquity-0.1.5/payequity/Audit.py
--rw-rw-rw-   0        0        0    21932 2023-02-21 20:25:58.000000 PayEquity-0.1.5/payequity/JobGroup.py
--rw-rw-rw-   0        0        0     4276 2023-05-01 01:42:07.000000 PayEquity-0.1.5/payequity/JobGroupEnssemble.py
--rw-rw-rw-   0        0        0    22462 2023-05-27 15:32:06.000000 PayEquity-0.1.5/payequity/Regressor.py
--rw-rw-rw-   0        0        0      176 2022-08-10 16:46:06.000000 PayEquity-0.1.5/payequity/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 15:33:53.416176 PayEquity-0.1.5/payequity/tests/
--rw-rw-rw-   0        0        0        0 2022-07-25 19:50:42.000000 PayEquity-0.1.5/payequity/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2022-07-25 19:55:45.000000 PayEquity-0.1.5/payequity/tests/test_audit.py
--rw-rw-rw-   0        0        0     1714 2022-07-25 20:30:46.000000 PayEquity-0.1.5/payequity/tests/test_job_group.py
--rw-rw-rw-   0        0        0     1799 2022-08-24 14:55:43.000000 PayEquity-0.1.5/payequity/tests/test_job_group_enssemble.py
--rw-rw-rw-   0        0        0        0 2022-07-25 19:55:36.000000 PayEquity-0.1.5/payequity/tests/test_regressor.py
--rw-rw-rw-   0        0        0       21 2023-05-27 15:33:00.000000 PayEquity-0.1.5/payequity/version.py
--rw-rw-rw-   0        0        0       42 2023-05-27 15:33:53.418177 PayEquity-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      837 2023-05-06 14:59:20.000000 PayEquity-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 15:45:13.507523 PayEquity-0.1.6/
+-rw-rw-rw-   0        0        0      792 2023-05-27 15:44:46.000000 PayEquity-0.1.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-05-06 14:58:44.000000 PayEquity-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     1087 2022-07-25 19:00:43.000000 PayEquity-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     7576 2023-05-27 15:45:13.506523 PayEquity-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-27 15:45:13.484517 PayEquity-0.1.6/PayEquity.egg-info/
+-rw-rw-rw-   0        0        0     7576 2023-05-27 15:45:13.000000 PayEquity-0.1.6/PayEquity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-05-27 15:45:13.000000 PayEquity-0.1.6/PayEquity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 15:45:13.000000 PayEquity-0.1.6/PayEquity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-27 15:45:13.000000 PayEquity-0.1.6/PayEquity.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-27 15:45:13.000000 PayEquity-0.1.6/PayEquity.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7300 2023-02-06 20:33:18.000000 PayEquity-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 15:45:13.498520 PayEquity-0.1.6/payequity/
+-rw-rw-rw-   0        0        0    16221 2023-05-06 18:30:03.000000 PayEquity-0.1.6/payequity/Audit.py
+-rw-rw-rw-   0        0        0    21932 2023-02-21 20:25:58.000000 PayEquity-0.1.6/payequity/JobGroup.py
+-rw-rw-rw-   0        0        0     4276 2023-05-01 01:42:07.000000 PayEquity-0.1.6/payequity/JobGroupEnssemble.py
+-rw-rw-rw-   0        0        0    22462 2023-05-27 15:43:45.000000 PayEquity-0.1.6/payequity/Regressor.py
+-rw-rw-rw-   0        0        0      176 2022-08-10 16:46:06.000000 PayEquity-0.1.6/payequity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 15:45:13.505522 PayEquity-0.1.6/payequity/tests/
+-rw-rw-rw-   0        0        0        0 2022-07-25 19:50:42.000000 PayEquity-0.1.6/payequity/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-07-25 19:55:45.000000 PayEquity-0.1.6/payequity/tests/test_audit.py
+-rw-rw-rw-   0        0        0     1714 2022-07-25 20:30:46.000000 PayEquity-0.1.6/payequity/tests/test_job_group.py
+-rw-rw-rw-   0        0        0     1799 2022-08-24 14:55:43.000000 PayEquity-0.1.6/payequity/tests/test_job_group_enssemble.py
+-rw-rw-rw-   0        0        0        0 2022-07-25 19:55:36.000000 PayEquity-0.1.6/payequity/tests/test_regressor.py
+-rw-rw-rw-   0        0        0       21 2023-05-27 15:43:49.000000 PayEquity-0.1.6/payequity/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-27 15:45:13.507523 PayEquity-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      837 2023-05-27 15:44:59.000000 PayEquity-0.1.6/setup.py
```

### Comparing `PayEquity-0.1.5/CHANGELOG.txt` & `PayEquity-0.1.6/CHANGELOG.txt`

 * *Files 17% similar despite different names*

```diff
@@ -29,8 +29,16 @@
 ------------------
 ### Added
 - Force converted dummy dataframe to float
 
 0.1.5 (5/27/23)
 ------------------
 ### Added
-- Force converted dummy dataframe to float x2 ln277 regressor
+- Force converted dummy dataframe to float x2 ln277 regressor
+
+0.1.6 (5/27/23)
+------------------
+### Added
+- pred.summary_frame(alpha=alpha).astype(float)
+
+### Remove
+- float ln277 regressor
```

### Comparing `PayEquity-0.1.5/LICENSE.txt` & `PayEquity-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.5/MANIFEST.in` & `PayEquity-0.1.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.5/PKG-INFO` & `PayEquity-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PayEquity
-Version: 0.1.5
+Version: 0.1.6
 Summary: Pay Equity Library
 Home-page: https://github.com/scunden/pay-equity
 Author: Steven Cunden
 Author-email: slcunden@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `PayEquity-0.1.5/PayEquity.egg-info/PKG-INFO` & `PayEquity-0.1.6/PayEquity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PayEquity
-Version: 0.1.5
+Version: 0.1.6
 Summary: Pay Equity Library
 Home-page: https://github.com/scunden/pay-equity
 Author: Steven Cunden
 Author-email: slcunden@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `PayEquity-0.1.5/PayEquity.egg-info/SOURCES.txt` & `PayEquity-0.1.6/PayEquity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.5/README.md` & `PayEquity-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.5/payequity/Audit.py` & `PayEquity-0.1.6/payequity/Audit.py`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.5/payequity/JobGroup.py` & `PayEquity-0.1.6/payequity/JobGroup.py`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.5/payequity/JobGroupEnssemble.py` & `PayEquity-0.1.6/payequity/JobGroupEnssemble.py`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.5/payequity/Regressor.py` & `PayEquity-0.1.6/payequity/Regressor.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,16 +270,16 @@
             return self.hug_iter_coef
 
     def _generate_predictions(self, X, results, alpha=0.05, y=None):
         
         self.logger.debug("Generating predictions")
 
         y = self.y if y is None else y
-        pred = results.get_prediction(X).astype(float)
-        pred = np.exp(pred.summary_frame(alpha=alpha))
+        pred = results.get_prediction(X)
+        pred = np.exp(pred.summary_frame(alpha=alpha).astype(float))
         pred = pred[['mean','obs_ci_lower','obs_ci_upper']]
         pred.rename({ 'mean':'Prediction',
                                  'obs_ci_lower':"Lower",
                                  'obs_ci_upper':"Upper"}, 
                                 axis=1, inplace=True)
 
         pred['Job Group'] = self.name
```

### Comparing `PayEquity-0.1.5/payequity/tests/test_job_group.py` & `PayEquity-0.1.6/payequity/tests/test_job_group.py`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.5/payequity/tests/test_job_group_enssemble.py` & `PayEquity-0.1.6/payequity/tests/test_job_group_enssemble.py`

 * *Files identical despite different names*

### Comparing `PayEquity-0.1.5/setup.py` & `PayEquity-0.1.6/setup.py`

 * *Files identical despite different names*

