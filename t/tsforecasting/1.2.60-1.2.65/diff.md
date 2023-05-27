# Comparing `tmp/tsforecasting-1.2.60-py3-none-any.whl.zip` & `tmp/tsforecasting-1.2.65-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18625 bytes, number of entries: 12
+Zip file size: 18593 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      393 b- defN 23-Feb-21 11:35 tsforecasting/__init__.py
 -rw-rw-rw-  2.0 fat    10033 b- defN 23-Apr-17 15:36 tsforecasting/tsf_data_eng.py
 -rw-rw-rw-  2.0 fat    10134 b- defN 23-Apr-17 16:08 tsforecasting/tsf_expanding_window.py
 -rw-rw-rw-  2.0 fat     1684 b- defN 23-Mar-02 11:05 tsforecasting/tsf_model_configs.py
 -rw-rw-rw-  2.0 fat     4009 b- defN 23-Apr-17 15:43 tsforecasting/tsf_model_selection.py
 -rw-rw-rw-  2.0 fat     7891 b- defN 23-Apr-17 15:44 tsforecasting/tsf_performance.py
--rw-rw-rw-  2.0 fat     8381 b- defN 23-Apr-17 15:57 tsforecasting/tsf_predictions.py
--rw-rw-rw-  2.0 fat     1078 b- defN 23-Apr-17 16:25 tsforecasting-1.2.60.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    11282 b- defN 23-Apr-17 16:25 tsforecasting-1.2.60.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-17 16:25 tsforecasting-1.2.60.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Apr-17 16:25 tsforecasting-1.2.60.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1047 b- defN 23-Apr-17 16:25 tsforecasting-1.2.60.dist-info/RECORD
-12 files, 56038 bytes uncompressed, 16853 bytes compressed:  69.9%
+-rw-rw-rw-  2.0 fat     8385 b- defN 23-May-27 21:19 tsforecasting/tsf_predictions.py
+-rw-rw-rw-  2.0 fat     1078 b- defN 23-May-27 21:24 tsforecasting-1.2.65.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    11121 b- defN 23-May-27 21:24 tsforecasting-1.2.65.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-27 21:24 tsforecasting-1.2.65.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-May-27 21:24 tsforecasting-1.2.65.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1047 b- defN 23-May-27 21:24 tsforecasting-1.2.65.dist-info/RECORD
+12 files, 55881 bytes uncompressed, 16821 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: tsforecasting/tsf_performance.py
 Comment: 
 
 Filename: tsforecasting/tsf_predictions.py
 Comment: 
 
-Filename: tsforecasting-1.2.60.dist-info/LICENSE
+Filename: tsforecasting-1.2.65.dist-info/LICENSE
 Comment: 
 
-Filename: tsforecasting-1.2.60.dist-info/METADATA
+Filename: tsforecasting-1.2.65.dist-info/METADATA
 Comment: 
 
-Filename: tsforecasting-1.2.60.dist-info/WHEEL
+Filename: tsforecasting-1.2.65.dist-info/WHEEL
 Comment: 
 
-Filename: tsforecasting-1.2.60.dist-info/top_level.txt
+Filename: tsforecasting-1.2.65.dist-info/top_level.txt
 Comment: 
 
-Filename: tsforecasting-1.2.60.dist-info/RECORD
+Filename: tsforecasting-1.2.65.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tsforecasting/tsf_predictions.py

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 import numpy as np
 import sys
 import datetime
 from datetime import timedelta
 from dateutil.relativedelta import relativedelta
-from sklearn.preprocessing import MinMaxScaler
+from sklearn.preprocessing import StandardScaler
 from prophet import Prophet
 from pmdarima.arima import auto_arima
 from .tsf_data_eng import slice_timestamp, round_cols, engin_date, multivariable_lag
 from .tsf_model_selection import model_prediction
 from .tsf_model_configs import model_configurations
 
 h_parameters=model_configurations()
@@ -173,15 +173,15 @@
         
         train=df_final.iloc[:len(df_final)-forecast_size,:]
         test=df_final.iloc[len(df_final)-forecast_size:,:]
 
         input_cols=list(df_final.columns)
         input_cols.remove(target)  
         
-        scaler = MinMaxScaler()
+        scaler = StandardScaler()
         scaler = scaler.fit(train[input_cols])
         
         train[input_cols] = scaler.transform(train[input_cols])
         test[input_cols] = scaler.transform(test[input_cols])
 
         y_pred=model_prediction(train, test,target,model_configs=model_configs,algo=selected_model)
         df_final['y'][len(df_final)-forecast_size:]=y_pred
```

## Comparing `tsforecasting-1.2.60.dist-info/LICENSE` & `tsforecasting-1.2.65.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tsforecasting-1.2.60.dist-info/METADATA` & `tsforecasting-1.2.65.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsforecasting
-Version: 1.2.60
+Version: 1.2.65
 Summary: TSForecasting is an Automated Time Series Forecasting Framework
 Home-page: https://github.com/TsLu1s/TSForecasting
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,time series forecasting,automated time series,multivariate time series,univariate time series,automated machine learning,automl
 Classifier: Intended Audience :: Education
@@ -14,15 +14,14 @@
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas (>=1.3.5)
 Requires-Dist: numpy (>=1.21.5)
 Requires-Dist: python-dateutil (>=2.8.2)
 Requires-Dist: scikit-learn (>=1.0.2)
@@ -40,15 +39,15 @@
 
 The `TSForecasting` project constitutes an complete and integrated pipeline to Automate Time Series Forecasting applications through the implementation of multivariate approaches integrating regression models referring to modules such as SKLearn, H2O.ai, XGBoost and also univariate approaches of more classics methods such as Prophet and AutoArima, this following an 'Expanding Window' performance evaluation.
 
 The architecture design includes five main sections, these being: data preprocessing, feature engineering, hyperparameter optimization, forecast ensembling and forecasting method selection which are organized and customizable in a pipeline structure.
 
 This project aims at providing the following application capabilities:
 
-* General applicability on tabular datasets: The developed forecasting procedures are applicable on any data table associated with any Time Series Forecasting scopes, based on DateTime and Target columns to be predicted.
+* General applicability on tabular datasets: The developed forecasting procedures are applicable on any data table associated with any Time Series Forecasting scopes.
 
 * Hyperparameter optimization and customization: It provides full configuration for each model hyperparameter through the customization of `model_configs` parameter variable values, allowing optimal performance to be obtained for each use case.
     
 * Robustness and improvement of predictive results: The implementation of the TSForecasting pipeline aims to improve the predictive performance directly associated with the application of the best performing forecasting method. 
    
 #### Main Development Tools <a name = "pre1"></a>
 
@@ -198,9 +197,7 @@
 ## License
 
 Distributed under the MIT License. See [LICENSE](https://github.com/TsLu1s/TSForecasting/blob/main/LICENSE) for more information.
 
 ## Contact 
  
 Luis Santos - [LinkedIn](https://www.linkedin.com/in/lu%C3%ADsfssantos/)
-    
-Feel free to contact me and share your feedback.
```

