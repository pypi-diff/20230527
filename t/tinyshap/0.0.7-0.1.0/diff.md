# Comparing `tmp/tinyshap-0.0.7.tar.gz` & `tmp/tinyshap-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyshap-0.0.7.tar", last modified: Sun May 21 15:51:46 2023, max compression
+gzip compressed data, was "tinyshap-0.1.0.tar", last modified: Sat May 27 10:11:29 2023, max compression
```

## Comparing `tinyshap-0.0.7.tar` & `tinyshap-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:51:46.163189 tinyshap-0.0.7/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1089 2023-04-29 16:41:09.000000 tinyshap-0.0.7/LICENCE
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2154 2023-05-21 15:51:46.156188 tinyshap-0.0.7/PKG-INFO
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1316 2023-05-20 20:04:45.000000 tinyshap-0.0.7/README.md
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1144 2023-05-21 15:50:21.000000 tinyshap-0.0.7/pyproject.toml
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       38 2023-05-21 15:51:46.168192 tinyshap-0.0.7/setup.cfg
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:51:44.931242 tinyshap-0.0.7/src/
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:51:45.611373 tinyshap-0.0.7/src/tinyshap/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       46 2023-04-24 17:25:47.000000 tinyshap-0.0.7/src/tinyshap/__init__.py
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     4034 2023-05-21 15:47:22.000000 tinyshap-0.0.7/src/tinyshap/explainer.py
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:51:46.000581 tinyshap-0.0.7/src/tinyshap.egg-info/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2154 2023-05-21 15:51:44.000000 tinyshap-0.0.7/src/tinyshap.egg-info/PKG-INFO
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      286 2023-05-21 15:51:44.000000 tinyshap-0.0.7/src/tinyshap.egg-info/SOURCES.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        1 2023-05-21 15:51:44.000000 tinyshap-0.0.7/src/tinyshap.egg-info/dependency_links.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       55 2023-05-21 15:51:44.000000 tinyshap-0.0.7/src/tinyshap.egg-info/requires.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        9 2023-05-21 15:51:44.000000 tinyshap-0.0.7/src/tinyshap.egg-info/top_level.txt
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:51:46.058574 tinyshap-0.0.7/tests/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2634 2023-05-20 19:59:07.000000 tinyshap-0.0.7/tests/test_explainer.py
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-27 10:11:29.335526 tinyshap-0.1.0/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1089 2023-04-29 16:41:09.000000 tinyshap-0.1.0/LICENCE
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2154 2023-05-27 10:11:29.326008 tinyshap-0.1.0/PKG-INFO
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1316 2023-05-20 20:04:45.000000 tinyshap-0.1.0/README.md
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1144 2023-05-27 10:10:14.000000 tinyshap-0.1.0/pyproject.toml
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       38 2023-05-27 10:11:29.337775 tinyshap-0.1.0/setup.cfg
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-27 10:11:28.630694 tinyshap-0.1.0/src/
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-27 10:11:28.868042 tinyshap-0.1.0/src/tinyshap/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       46 2023-04-24 17:25:47.000000 tinyshap-0.1.0/src/tinyshap/__init__.py
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     4241 2023-05-27 09:51:45.000000 tinyshap-0.1.0/src/tinyshap/explainer.py
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-27 10:11:29.219144 tinyshap-0.1.0/src/tinyshap.egg-info/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2154 2023-05-27 10:11:28.000000 tinyshap-0.1.0/src/tinyshap.egg-info/PKG-INFO
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      286 2023-05-27 10:11:28.000000 tinyshap-0.1.0/src/tinyshap.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        1 2023-05-27 10:11:28.000000 tinyshap-0.1.0/src/tinyshap.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       55 2023-05-27 10:11:28.000000 tinyshap-0.1.0/src/tinyshap.egg-info/requires.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        9 2023-05-27 10:11:28.000000 tinyshap-0.1.0/src/tinyshap.egg-info/top_level.txt
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-27 10:11:29.267674 tinyshap-0.1.0/tests/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2933 2023-05-27 10:05:55.000000 tinyshap-0.1.0/tests/test_explainer.py
```

### Comparing `tinyshap-0.0.7/LICENCE` & `tinyshap-0.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `tinyshap-0.0.7/PKG-INFO` & `tinyshap-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyshap
-Version: 0.0.7
+Version: 0.1.0
 Summary: Minimal implementation of approximate Kernel SHAP algorithm
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Project-URL: Homepage, https://github.com/tsitsimis/tinyshap
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyshap Version: 0.0.7 Summary: Minimal
+Metadata-Version: 2.1 Name: tinyshap Version: 0.1.0 Summary: Minimal
 implementation of approximate Kernel SHAP algorithm Author-email: Theodore
 Tsitsimis
 tsitsimis@gmail.com> Project-URL: Homepage, https://github.com/tsitsimis/
 tinyshap Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `tinyshap-0.0.7/README.md` & `tinyshap-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tinyshap-0.0.7/pyproject.toml` & `tinyshap-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'tinyshap'
-version = '0.0.7'
+version = '0.1.0'
 description = 'Minimal implementation of approximate Kernel SHAP algorithm'
 readme = 'README.md'
 authors = [
   { name = 'Theodore Tsitsimis', email='th.tsitsimis@gmail.com' },
 ]
 license = {file = 'LICENSE'}
 requires-python = '>=3.7'
```

### Comparing `tinyshap-0.0.7/src/tinyshap/explainer.py` & `tinyshap-0.1.0/src/tinyshap/explainer.py`

 * *Files 13% similar despite different names*

```diff
@@ -66,32 +66,38 @@
         """
         dim = self.X.shape[1]
 
         weights = coalitions.apply(lambda row: shap_kernel(coalition=row.tolist(), dim=dim), axis=1)
         weights = weights.values
         return weights
 
-    def _explain_sample(self, x_test: np.ndarray) -> pd.Series:
+    def _explain_sample(self, x_test: np.ndarray, sign_constraints: dict = {}) -> pd.Series:
         """
         Calculates SHAP values of a single sample using approximate KernelSHAP
         """
         assert x_test.ndim == 1
 
         model_prediction = self.model(pd.DataFrame(x_test.reshape(1, -1), columns=self.X.columns))
 
         coalitions = self._generate_coalitions()
         feature_values = self._get_feature_values(coalitions, x_test)
         predictions = self.model(feature_values)
         weights = self._get_coalition_weights(coalitions)
 
-        lr = ConstrainedLinearRegression(fit_intercept=True)
-        lr.fit(coalitions, predictions, sample_weight=weights, coefficients_sum_constraint=model_prediction)
+        lr = ConstrainedLinearRegression(fit_intercept=False)
+        lr.fit(
+            coalitions,
+            predictions,
+            sample_weight=weights,
+            coefficients_sum_constraint=model_prediction,
+            coefficients_sign_constraints=sign_constraints,
+        )
         shap_values = pd.Series(data=lr.coef_, index=self.X.columns)
-        shap_values["avg_prediction"] = lr.intercept_
+        shap_values["avg_prediction"] = 0  # lr.intercept_
         return shap_values
 
-    def shap_values(self, X: pd.DataFrame) -> pd.DataFrame:
+    def shap_values(self, X: pd.DataFrame, sign_constraints: dict = {}) -> pd.DataFrame:
         """
         Calculates SHAP values of multiple samples in `X`
         """
-        shap_values = X.apply(lambda row: self._explain_sample(np.array(row.tolist())), axis=1)
+        shap_values = X.apply(lambda row: self._explain_sample(np.array(row.tolist()), sign_constraints), axis=1)
         return shap_values
```

### Comparing `tinyshap-0.0.7/src/tinyshap.egg-info/PKG-INFO` & `tinyshap-0.1.0/src/tinyshap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyshap
-Version: 0.0.7
+Version: 0.1.0
 Summary: Minimal implementation of approximate Kernel SHAP algorithm
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Project-URL: Homepage, https://github.com/tsitsimis/tinyshap
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyshap Version: 0.0.7 Summary: Minimal
+Metadata-Version: 2.1 Name: tinyshap Version: 0.1.0 Summary: Minimal
 implementation of approximate Kernel SHAP algorithm Author-email: Theodore
 Tsitsimis
 tsitsimis@gmail.com> Project-URL: Homepage, https://github.com/tsitsimis/
 tinyshap Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `tinyshap-0.0.7/tests/test_explainer.py` & `tinyshap-0.1.0/tests/test_explainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,7 +67,15 @@
 def test_shap_values():
     explainer = SHAPExplainer(model.predict, X=X_train_summary)
     shap_values = explainer.shap_values(X_test)
 
     assert shap_values.shape[0] == X_test.shape[0]
     assert shap_values.shape[1] == X_test.shape[1] + 1
     assert np.allclose(shap_values.sum(axis=1).values, explainer.model(X_test), rtol=0.01)
+
+
+def test_sign_constraints():
+    explainer = SHAPExplainer(model.predict, X=X_train_summary)
+    shap_values = explainer.shap_values(X_test, sign_constraints={0: -1, 1: 1})
+
+    assert all((shap_values.iloc[:, 0] < 1e-5).tolist())
+    assert all((shap_values.iloc[:, 1] > -1e-5).tolist())
```

