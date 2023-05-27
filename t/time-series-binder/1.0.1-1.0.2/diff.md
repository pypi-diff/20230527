# Comparing `tmp/time_series_binder-1.0.1.tar.gz` & `tmp/time_series_binder-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\time_series_binder-1.0.1.tar", last modified: Sat May 27 14:07:35 2023, max compression
+gzip compressed data, was "dist\time_series_binder-1.0.2.tar", last modified: Sat May 27 14:11:38 2023, max compression
```

## Comparing `time_series_binder-1.0.1.tar` & `time_series_binder-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 14:07:35.059115 time_series_binder-1.0.1/
--rw-rw-rw-   0        0        0       87 2023-05-27 11:53:42.000000 time_series_binder-1.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1079 2023-05-27 11:53:42.000000 time_series_binder-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-05-27 11:53:42.000000 time_series_binder-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2249 2023-05-27 14:07:35.058261 time_series_binder-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2023-05-27 12:30:40.000000 time_series_binder-1.0.1/README.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 14:07:35.060112 time_series_binder-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1390 2023-05-27 14:01:25.000000 time_series_binder-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 14:07:35.044559 time_series_binder-1.0.1/time_series_binder.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-05-27 14:07:34.000000 time_series_binder-1.0.1/time_series_binder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-05-27 14:07:34.000000 time_series_binder-1.0.1/time_series_binder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 14:07:34.000000 time_series_binder-1.0.1/time_series_binder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-05-27 14:07:34.000000 time_series_binder-1.0.1/time_series_binder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-27 14:07:34.000000 time_series_binder-1.0.1/time_series_binder.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 14:07:35.056409 time_series_binder-1.0.1/ts_binder/
--rw-rw-rw-   0        0        0       45 2023-05-27 12:36:11.000000 time_series_binder-1.0.1/ts_binder/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-05-27 13:08:55.000000 time_series_binder-1.0.1/ts_binder/data_processing.py
--rw-rw-rw-   0        0        0     4258 2023-05-27 13:13:03.000000 time_series_binder-1.0.1/ts_binder/forecaster.py
--rw-rw-rw-   0        0        0     3778 2023-05-27 13:31:35.000000 time_series_binder-1.0.1/ts_binder/helpers.py
--rw-rw-rw-   0        0        0     5989 2023-05-27 13:08:52.000000 time_series_binder-1.0.1/ts_binder/trainer.py
+drwxrwxrwx   0        0        0        0 2023-05-27 14:11:38.923941 time_series_binder-1.0.2/
+-rw-rw-rw-   0        0        0       87 2023-05-27 11:53:42.000000 time_series_binder-1.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1079 2023-05-27 11:53:42.000000 time_series_binder-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-05-27 11:53:42.000000 time_series_binder-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2249 2023-05-27 14:11:38.922977 time_series_binder-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1067 2023-05-27 12:30:40.000000 time_series_binder-1.0.2/README.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 14:11:38.924972 time_series_binder-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1362 2023-05-27 14:10:18.000000 time_series_binder-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 14:11:38.906024 time_series_binder-1.0.2/time_series_binder.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-05-27 14:11:38.000000 time_series_binder-1.0.2/time_series_binder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-05-27 14:11:38.000000 time_series_binder-1.0.2/time_series_binder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 14:11:38.000000 time_series_binder-1.0.2/time_series_binder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-05-27 14:11:38.000000 time_series_binder-1.0.2/time_series_binder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-27 14:11:38.000000 time_series_binder-1.0.2/time_series_binder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 14:11:38.919991 time_series_binder-1.0.2/ts_binder/
+-rw-rw-rw-   0        0        0       45 2023-05-27 12:36:11.000000 time_series_binder-1.0.2/ts_binder/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-05-27 13:08:55.000000 time_series_binder-1.0.2/ts_binder/data_processing.py
+-rw-rw-rw-   0        0        0     4258 2023-05-27 13:13:03.000000 time_series_binder-1.0.2/ts_binder/forecaster.py
+-rw-rw-rw-   0        0        0     3778 2023-05-27 13:31:35.000000 time_series_binder-1.0.2/ts_binder/helpers.py
+-rw-rw-rw-   0        0        0     5989 2023-05-27 13:08:52.000000 time_series_binder-1.0.2/ts_binder/trainer.py
```

### Comparing `time_series_binder-1.0.1/LICENSE.txt` & `time_series_binder-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `time_series_binder-1.0.1/PKG-INFO` & `time_series_binder-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: time_series_binder
-Version: 1.0.1
+Version: 1.0.2
 Summary: Time Series Binder is a Python library for time series analysis and forecasting. It offers a comprehensive set of tools and models, including Pandas integration, statistical methods, neural networks with Keras, and the NeuralProphet library. With Time Series Binder, you can easily manipulate, visualize, and predict time series data, making it an essential toolkit for researchers and analysts.
 Home-page: UNKNOWN
 Author: Jhun Brian Andam
 Author-email: brianandam123@gmail.com
 License: MIT
 Description: # Time Series Binder
```

### Comparing `time_series_binder-1.0.1/README.txt` & `time_series_binder-1.0.2/README.txt`

 * *Files identical despite different names*

### Comparing `time_series_binder-1.0.1/setup.py` & `time_series_binder-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,19 @@
                 'numpy', 
                 'matplotlib', 
                 'statsmodels', 
                 'keras', 
                 'neuralprophet', 
                 'scikit-learn', 
                 'tqdm', 
-                'tabulate', 
-                'inspect']
+                'tabulate']
 
 setup(
   name='time_series_binder',
-  version='1.0.1',
+  version='1.0.2',
   description=desc,
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Jhun Brian Andam',
   author_email='brianandam123@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `time_series_binder-1.0.1/time_series_binder.egg-info/PKG-INFO` & `time_series_binder-1.0.2/time_series_binder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: time-series-binder
-Version: 1.0.1
+Version: 1.0.2
 Summary: Time Series Binder is a Python library for time series analysis and forecasting. It offers a comprehensive set of tools and models, including Pandas integration, statistical methods, neural networks with Keras, and the NeuralProphet library. With Time Series Binder, you can easily manipulate, visualize, and predict time series data, making it an essential toolkit for researchers and analysts.
 Home-page: UNKNOWN
 Author: Jhun Brian Andam
 Author-email: brianandam123@gmail.com
 License: MIT
 Description: # Time Series Binder
```

### Comparing `time_series_binder-1.0.1/ts_binder/data_processing.py` & `time_series_binder-1.0.2/ts_binder/data_processing.py`

 * *Files identical despite different names*

### Comparing `time_series_binder-1.0.1/ts_binder/forecaster.py` & `time_series_binder-1.0.2/ts_binder/forecaster.py`

 * *Files identical despite different names*

### Comparing `time_series_binder-1.0.1/ts_binder/helpers.py` & `time_series_binder-1.0.2/ts_binder/helpers.py`

 * *Files identical despite different names*

### Comparing `time_series_binder-1.0.1/ts_binder/trainer.py` & `time_series_binder-1.0.2/ts_binder/trainer.py`

 * *Files identical despite different names*

