# Comparing `tmp/Optimized Kalman Filter-0.0.6.tar.gz` & `tmp/Optimized Kalman Filter-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Optimized Kalman Filter-0.0.6.tar", last modified: Wed Jan 18 22:15:01 2023, max compression
+gzip compressed data, was "Optimized Kalman Filter-0.0.7.tar", last modified: Fri May 26 22:43:40 2023, max compression
```

## Comparing `Optimized Kalman Filter-0.0.6.tar` & `Optimized Kalman Filter-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-01-18 22:15:01.152194 Optimized Kalman Filter-0.0.6/
--rw-rw-rw-   0        0        0     1081 2021-11-15 17:37:21.000000 Optimized Kalman Filter-0.0.6/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-01-18 22:15:01.103473 Optimized Kalman Filter-0.0.6/Optimized_Kalman_Filter.egg-info/
--rw-rw-rw-   0        0        0     5590 2023-01-18 22:15:00.000000 Optimized Kalman Filter-0.0.6/Optimized_Kalman_Filter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-01-18 22:15:01.000000 Optimized Kalman Filter-0.0.6/Optimized_Kalman_Filter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-18 22:15:00.000000 Optimized Kalman Filter-0.0.6/Optimized_Kalman_Filter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-01-18 22:15:00.000000 Optimized Kalman Filter-0.0.6/Optimized_Kalman_Filter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-01-18 22:15:00.000000 Optimized Kalman Filter-0.0.6/Optimized_Kalman_Filter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5590 2023-01-18 22:15:01.151242 Optimized Kalman Filter-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5065 2023-01-18 22:13:50.000000 Optimized Kalman Filter-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-01-18 22:15:01.128408 Optimized Kalman Filter-0.0.6/okf/
--rw-rw-rw-   0        0        0      296 2021-11-20 12:37:29.000000 Optimized Kalman Filter-0.0.6/okf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-18 22:15:01.150201 Optimized Kalman Filter-0.0.6/okf/example/
--rw-rw-rw-   0        0        0      160 2021-11-20 12:41:47.000000 Optimized Kalman Filter-0.0.6/okf/example/__init__.py
--rw-rw-rw-   0        0        0     1321 2021-11-15 17:34:24.000000 Optimized Kalman Filter-0.0.6/okf/example/simple_lidar_model.py
--rw-rw-rw-   0        0        0     3943 2021-11-20 11:27:43.000000 Optimized Kalman Filter-0.0.6/okf/example/simple_lidar_simulator.py
--rw-rw-rw-   0        0        0    12996 2023-01-14 16:56:01.000000 Optimized Kalman Filter-0.0.6/okf/model.py
--rw-rw-rw-   0        0        0    17791 2021-11-20 12:03:56.000000 Optimized Kalman Filter-0.0.6/okf/optimizer.py
--rw-rw-rw-   0        0        0     9196 2021-11-13 11:33:49.000000 Optimized Kalman Filter-0.0.6/okf/utils.py
--rw-rw-rw-   0        0        0       42 2023-01-18 22:15:01.152194 Optimized Kalman Filter-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-01-18 22:14:09.000000 Optimized Kalman Filter-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 22:43:40.158587 Optimized Kalman Filter-0.0.7/
+-rw-rw-rw-   0        0        0     1081 2021-11-15 17:37:21.000000 Optimized Kalman Filter-0.0.7/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 22:43:40.114656 Optimized Kalman Filter-0.0.7/Optimized_Kalman_Filter.egg-info/
+-rw-rw-rw-   0        0        0     5590 2023-05-26 22:43:39.000000 Optimized Kalman Filter-0.0.7/Optimized_Kalman_Filter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-05-26 22:43:40.000000 Optimized Kalman Filter-0.0.7/Optimized_Kalman_Filter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 22:43:39.000000 Optimized Kalman Filter-0.0.7/Optimized_Kalman_Filter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-26 22:43:39.000000 Optimized Kalman Filter-0.0.7/Optimized_Kalman_Filter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-26 22:43:39.000000 Optimized Kalman Filter-0.0.7/Optimized_Kalman_Filter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5590 2023-05-26 22:43:40.158587 Optimized Kalman Filter-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5065 2023-01-18 22:13:50.000000 Optimized Kalman Filter-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 22:43:40.137680 Optimized Kalman Filter-0.0.7/okf/
+-rw-rw-rw-   0        0        0      296 2021-11-20 12:37:29.000000 Optimized Kalman Filter-0.0.7/okf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 22:43:40.156586 Optimized Kalman Filter-0.0.7/okf/example/
+-rw-rw-rw-   0        0        0      160 2021-11-20 12:41:47.000000 Optimized Kalman Filter-0.0.7/okf/example/__init__.py
+-rw-rw-rw-   0        0        0     2145 2023-05-26 22:37:19.000000 Optimized Kalman Filter-0.0.7/okf/example/simple_lidar_model.py
+-rw-rw-rw-   0        0        0     3943 2021-11-20 11:27:43.000000 Optimized Kalman Filter-0.0.7/okf/example/simple_lidar_simulator.py
+-rw-rw-rw-   0        0        0    13936 2023-05-26 22:05:01.000000 Optimized Kalman Filter-0.0.7/okf/model.py
+-rw-rw-rw-   0        0        0    17903 2023-05-26 22:09:37.000000 Optimized Kalman Filter-0.0.7/okf/optimizer.py
+-rw-rw-rw-   0        0        0     9196 2021-11-13 11:33:49.000000 Optimized Kalman Filter-0.0.7/okf/utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-26 22:43:40.159587 Optimized Kalman Filter-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-05-26 21:43:49.000000 Optimized Kalman Filter-0.0.7/setup.py
```

### Comparing `Optimized Kalman Filter-0.0.6/LICENSE.txt` & `Optimized Kalman Filter-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Optimized Kalman Filter-0.0.6/Optimized_Kalman_Filter.egg-info/PKG-INFO` & `Optimized Kalman Filter-0.0.7/Optimized_Kalman_Filter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Optimized-Kalman-Filter
-Version: 0.0.6
+Version: 0.0.7
 Summary: Optimization of a Kalman Filter from data of states and their observations.
 Home-page: https://github.com/ido90/Optimized-Kalman-Filter
 Author: Ido Greenberg
 License: MIT
 Keywords: OKF,Optimized Kalman Filter,Kalman Filter
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Optimized Kalman Filter-0.0.6/PKG-INFO` & `Optimized Kalman Filter-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Optimized Kalman Filter
-Version: 0.0.6
+Version: 0.0.7
 Summary: Optimization of a Kalman Filter from data of states and their observations.
 Home-page: https://github.com/ido90/Optimized-Kalman-Filter
 Author: Ido Greenberg
 License: MIT
 Keywords: OKF,Optimized Kalman Filter,Kalman Filter
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Optimized Kalman Filter-0.0.6/README.md` & `Optimized Kalman Filter-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `Optimized Kalman Filter-0.0.6/okf/example/simple_lidar_simulator.py` & `Optimized Kalman Filter-0.0.7/okf/example/simple_lidar_simulator.py`

 * *Files identical despite different names*

### Comparing `Optimized Kalman Filter-0.0.6/okf/model.py` & `Optimized Kalman Filter-0.0.7/okf/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import torch
 import torch.nn as nn
 from torch import matmul as mp
 
 from . import utils
 
 class OKF(nn.Module):
-    def __init__(self, dim_x, dim_z, F, H, model_name='OKF', P0=1e3, Q0=1, R0=1,
+    def __init__(self, dim_x, dim_z, F, H, model_name='OKF', P0=1e3, Q0=1, R0=1, x0=None,
                  init_z2x=None, loss_fun=None, optimize=True, model_files_path='models/'):
         '''
         A model of KF whose parameters (Q,R) are pytorch tensors and can be optimized wrt a loss function.
 
         Under the KF assumptions, such optimization (wrt the MSE of the model-predictions) is equivalent to simply
         calculate the sample covariance matrices of the noise (given corresponding data). However, the KF assumptions
         do not usually hold in practical problems - which is sometimes goes unnoticed. Optimization can obtain better
@@ -53,14 +53,17 @@
                    default=1e3].
         :param Q0: The initial value of the process-noise covariance matrix Q, from which the optimization begins.
                    If scalar, it is used as a scale drawing the initial matrix randomly [positive numeric OR pytorch
                    tensor with type double and shape (dim_x,dim_x); default=1; only used if optimize==True].
         :param R0: The initial value of the observation-noise covariance matrix R, from which the optimization begins.
                    If scalar, it is used as a scale drawing the initial matrix randomly [positive numeric OR pytorch
                    tensor with type double and shape (dim_z,dim_z); default=1; only used if optimize==True].
+        :param x0: The initial value of the state x. If None, then the state will only be initialized after the first
+                   observation z, as x=init_z2x(z). If scalar, x=x0*ones(dim_x) is used [scalar OR pytorch tensor with
+                   type double and shape dim_x OR None; default=None].
         :param init_z2x: A function that receives the first observation and returns the first estimate of the state.
                          If array instead of a callable, just initializing the state to the given array.
                          [fun(z); default=identity function; if dim_x!=dim_z, another function must be specified].
         :param loss_fun: Loss function to optimize [fun(predicted_x, true_x); default=MSE; only used if optimize==True].
         :param optimize: Whether to tune the parameters Q,R by optimization or using the standard sample covariance
                          matrices of the noise.
         :param model_files_path: Directory path to save the model in [str].
@@ -73,46 +76,61 @@
         self.dim_z = dim_z
 
         self.F = F
         self.H = H
         self.is_H_fun = isinstance(self.H, types.FunctionType)
         self.is_F_fun = isinstance(self.F, types.FunctionType)
 
+        if x0 is None:
+            x0 = self.dim_x * [None]
+        elif not torch.is_tensor(x0):
+            x0 = x0 * torch.ones(self.dim_x, dtype=torch.double)
+        self.x0 = x0
+
+        if not torch.is_tensor(P0):
+            P0 = P0 * torch.eye(self.dim_x, dtype=torch.double)
         self.P0 = P0
         self.Q0 = Q0
         self.R0 = R0
         self.Q_D, self.Q_L, self.R_D, self.R_L = 4 * [None]
         self.reset_model()
 
         self.z2x = init_z2x
         if init_z2x is None:
             if self.dim_x != self.dim_z:
-                warnings.warn('No state initialization was provided (init_z2x). Could not initialize '
-                              'x=z either, since dim_x!=dim_z. Instead, x will be initialized to the '
-                              '0-array. Note that this is often highly sub-optimal. which is not recommended.')
+                if x0[0] is None:
+                    warnings.warn('No state initialization was provided (init_z2x). Could not initialize '
+                                  'x=z either, since dim_x!=dim_z. Instead, x will be initialized to the '
+                                  '0-array. Note that this is often highly sub-optimal. which is not recommended.')
                 self.z2x = lambda z: torch.zeros(self.dim_x, dtype=torch.double)
             else:
                 self.z2x = lambda z: z
         elif not callable(self.z2x):
             self.z2x = lambda z: torch.tensor(init_z2x, dtype=torch.double)
 
         self.loss_fun = loss_fun
         if self.loss_fun is None:
             self.loss_fun = lambda pred,x: ((pred-x)**2).sum()
 
+        # verify dimensions
+        if len(self.x0) != self.dim_x:
+            raise ValueError(f'Bad input dimension: len(x0) = {len(self.x0)} != {self.dim_x}.')
+        if self.P0.shape != (self.dim_x, self.dim_x):
+            raise ValueError(f'Bad input dimension: P0.shape = {self.P0.shape} != {(self.dim_x, self.dim_x)}.')
+
         self.x = None
         self.z = None
         self.P = None
         self.init_state()
 
     def init_state(self):
         '''Initialize the estimate (x,P) and the observation (z) before a new sequence of observations (trajectory).'''
-        self.x = self.dim_x * [None]
+        self.x = self.x0
         self.z = self.dim_z * [None]
-        self.P = self.P0 * torch.eye(self.dim_x, dtype=torch.double)
+        self.P = self.P0
 
     def reset_model(self):
         '''Reset the model parameters (Q,R).'''
         # Q
         if isinstance(self.Q0, torch.Tensor) and len(self.Q0.shape):
             # given as a 2D tensor
             Q_D, Q_L = OKF.encode_SPD(self.Q0)
```

### Comparing `Optimized Kalman Filter-0.0.6/okf/optimizer.py` & `Optimized Kalman Filter-0.0.7/okf/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 def train_models(models, X, Y, **kwargs):
     '''Run train() iteratively for every model.'''
     res_per_iter, res_per_sample = pd.DataFrame(), pd.DataFrame()
     for m in models:
         r1, r2 = train(m, X, Y, **kwargs)
         res_per_iter = pd.concat((res_per_iter, r1))
         res_per_sample = pd.concat((res_per_sample, r2))
+    res_per_iter.reset_index(drop=True, inplace=True)
+    res_per_sample.reset_index(drop=True, inplace=True)
     return res_per_iter, res_per_sample
 
 def train(model, X, Y, split_data=None, p_valid=0.15, n_epochs=1, batch_size=10,
           lr=1e-2, lr_decay=0.5, lr_decay_freq=150, optimizer=optim.Adam, weight_decay=0.0,
           loss_after_pred=False, log_interval=300, reset_model=True, noise_estimation_initialization=True,
           best_valid_loss=np.inf, verbose=1, valid_hor=8, to_save=True, save_best=True, **kwargs):
     '''
```

### Comparing `Optimized Kalman Filter-0.0.6/okf/utils.py` & `Optimized Kalman Filter-0.0.7/okf/utils.py`

 * *Files identical despite different names*

### Comparing `Optimized Kalman Filter-0.0.6/setup.py` & `Optimized Kalman Filter-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Optimized Kalman Filter",
-    version="0.0.6",
+    version="0.0.7",
     license='MIT',
     author="Ido Greenberg",
     description="Optimization of a Kalman Filter from data of states and their observations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url="https://github.com/ido90/Optimized-Kalman-Filter",
```

