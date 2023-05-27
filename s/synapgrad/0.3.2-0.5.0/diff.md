# Comparing `tmp/synapgrad-0.3.2-py3-none-any.whl.zip` & `tmp/synapgrad-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,34 @@
-Zip file size: 29809 bytes, number of entries: 21
--rw-rw-rw-  2.0 fat       72 b- defN 23-Apr-08 18:28 synapgrad/__init__.py
+Zip file size: 56098 bytes, number of entries: 32
+-rw-rw-rw-  2.0 fat      935 b- defN 23-May-27 01:01 synapgrad/__init__.py
+-rw-rw-rw-  2.0 fat    22932 b- defN 23-May-27 01:01 synapgrad/conv_tools.py
+-rw-rw-rw-  2.0 fat    21480 b- defN 23-May-27 13:17 synapgrad/cpu_ops.py
+-rw-rw-rw-  2.0 fat      171 b- defN 23-May-26 20:26 synapgrad/device.py
 -rw-rw-rw-  2.0 fat    32179 b- defN 23-May-05 17:20 synapgrad/engine.py
--rw-rw-rw-  2.0 fat      442 b- defN 23-May-01 13:33 synapgrad/nn/__init__.py
--rw-rw-rw-  2.0 fat     3538 b- defN 23-Apr-20 01:42 synapgrad/nn/activations.py
--rw-rw-rw-  2.0 fat     7831 b- defN 23-May-05 17:20 synapgrad/nn/functional.py
--rw-rw-rw-  2.0 fat     2879 b- defN 23-Apr-20 12:52 synapgrad/nn/initializations.py
--rw-rw-rw-  2.0 fat    18007 b- defN 23-May-06 19:50 synapgrad/nn/layers.py
--rw-rw-rw-  2.0 fat     6809 b- defN 23-Apr-20 01:41 synapgrad/nn/losses.py
--rw-rw-rw-  2.0 fat     2654 b- defN 23-May-05 16:13 synapgrad/nn/modules.py
+-rw-rw-rw-  2.0 fat    36424 b- defN 23-May-27 01:01 synapgrad/functional.py
+-rw-rw-rw-  2.0 fat    20437 b- defN 23-May-27 01:01 synapgrad/tensor.py
+-rw-rw-rw-  2.0 fat     1980 b- defN 23-May-27 01:01 synapgrad/utils.py
+-rw-rw-rw-  2.0 fat      445 b- defN 23-May-26 20:26 synapgrad/nn/__init__.py
+-rw-rw-rw-  2.0 fat     1731 b- defN 23-May-26 20:26 synapgrad/nn/activations.py
+-rw-rw-rw-  2.0 fat    35049 b- defN 23-May-27 12:23 synapgrad/nn/functional.py
+-rw-rw-rw-  2.0 fat     2907 b- defN 23-May-27 01:01 synapgrad/nn/initializations.py
+-rw-rw-rw-  2.0 fat    25851 b- defN 23-May-27 01:01 synapgrad/nn/layers.py
+-rw-rw-rw-  2.0 fat     4321 b- defN 23-May-27 01:01 synapgrad/nn/losses.py
+-rw-rw-rw-  2.0 fat     4967 b- defN 23-May-26 20:26 synapgrad/nn/modules.py
 -rw-rw-rw-  2.0 fat      989 b- defN 23-May-01 11:50 synapgrad/nn/neurons.py
--rw-rw-rw-  2.0 fat       46 b- defN 23-Apr-08 14:30 synapgrad/optim/__init__.py
--rw-rw-rw-  2.0 fat     5398 b- defN 23-May-05 17:24 synapgrad/optim/optimizers.py
+-rw-rw-rw-  2.0 fat      198 b- defN 23-May-26 20:26 synapgrad/nn/utils/__init__.py
+-rw-rw-rw-  2.0 fat     3207 b- defN 23-May-26 20:26 synapgrad/nn/utils/data.py
+-rw-rw-rw-  2.0 fat    10586 b- defN 23-May-26 20:26 synapgrad/nn/utils/train.py
+-rw-rw-rw-  2.0 fat       61 b- defN 23-May-26 20:26 synapgrad/optim/__init__.py
+-rw-rw-rw-  2.0 fat     5426 b- defN 23-May-27 01:01 synapgrad/optim/optimizers.py
 -rw-rw-rw-  2.0 fat      154 b- defN 23-Apr-11 17:18 synapgrad/utils/__init__.py
 -rw-rw-rw-  2.0 fat     3403 b- defN 23-Apr-11 18:19 synapgrad/utils/data.py
 -rw-rw-rw-  2.0 fat     1345 b- defN 23-Apr-21 08:50 synapgrad/utils/graph.py
 -rw-rw-rw-  2.0 fat    10586 b- defN 23-Apr-12 12:20 synapgrad/utils/train.py
--rw-rw-rw-  2.0 fat     1088 b- defN 23-May-07 01:43 synapgrad-0.3.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4960 b- defN 23-May-07 01:43 synapgrad-0.3.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-07 01:43 synapgrad-0.3.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-May-07 01:43 synapgrad-0.3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1696 b- defN 23-May-07 01:43 synapgrad-0.3.2.dist-info/RECORD
-21 files, 104178 bytes uncompressed, 27069 bytes compressed:  74.0%
+-rw-rw-rw-  2.0 fat       34 b- defN 23-May-26 20:26 synapgrad/visual/__init__.py
+-rw-rw-rw-  2.0 fat     1783 b- defN 23-May-27 01:01 synapgrad/visual/graph.py
+-rw-rw-rw-  2.0 fat     1088 b- defN 23-May-27 15:30 synapgrad-0.5.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     5003 b- defN 23-May-27 15:30 synapgrad-0.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-27 15:30 synapgrad-0.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-27 15:30 synapgrad-0.5.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2584 b- defN 23-May-27 15:30 synapgrad-0.5.0.dist-info/RECORD
+32 files, 258358 bytes uncompressed, 52006 bytes compressed:  79.9%
```

## zipnote {}

```diff
@@ -1,13 +1,31 @@
 Filename: synapgrad/__init__.py
 Comment: 
 
+Filename: synapgrad/conv_tools.py
+Comment: 
+
+Filename: synapgrad/cpu_ops.py
+Comment: 
+
+Filename: synapgrad/device.py
+Comment: 
+
 Filename: synapgrad/engine.py
 Comment: 
 
+Filename: synapgrad/functional.py
+Comment: 
+
+Filename: synapgrad/tensor.py
+Comment: 
+
+Filename: synapgrad/utils.py
+Comment: 
+
 Filename: synapgrad/nn/__init__.py
 Comment: 
 
 Filename: synapgrad/nn/activations.py
 Comment: 
 
 Filename: synapgrad/nn/functional.py
@@ -24,14 +42,23 @@
 
 Filename: synapgrad/nn/modules.py
 Comment: 
 
 Filename: synapgrad/nn/neurons.py
 Comment: 
 
+Filename: synapgrad/nn/utils/__init__.py
+Comment: 
+
+Filename: synapgrad/nn/utils/data.py
+Comment: 
+
+Filename: synapgrad/nn/utils/train.py
+Comment: 
+
 Filename: synapgrad/optim/__init__.py
 Comment: 
 
 Filename: synapgrad/optim/optimizers.py
 Comment: 
 
 Filename: synapgrad/utils/__init__.py
@@ -42,23 +69,29 @@
 
 Filename: synapgrad/utils/graph.py
 Comment: 
 
 Filename: synapgrad/utils/train.py
 Comment: 
 
-Filename: synapgrad-0.3.2.dist-info/LICENSE
+Filename: synapgrad/visual/__init__.py
+Comment: 
+
+Filename: synapgrad/visual/graph.py
+Comment: 
+
+Filename: synapgrad-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: synapgrad-0.3.2.dist-info/METADATA
+Filename: synapgrad-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: synapgrad-0.3.2.dist-info/WHEEL
+Filename: synapgrad-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: synapgrad-0.3.2.dist-info/top_level.txt
+Filename: synapgrad-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: synapgrad-0.3.2.dist-info/RECORD
+Filename: synapgrad-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## synapgrad/__init__.py

```diff
@@ -1,2 +1,23 @@
+# from synapgrad.autograd import no_grad, retain_grads, retain_children, retain_all
+from synapgrad.tensor import (
+    Tensor, tensor, ones, ones_like, zeros, zeros_like, 
+    arange, rand, randn, normal, randint, eye, no_grad,
+    retain_grads, no_grad
+)
+from synapgrad.functional import (
+    add, mul, matmul, addmm, pow, rpow, neg, slice,
+    concat, stack, unbind,
+    clone, exp, log, sqrt, sum, mean, max, min, squeeze, unsqueeze,
+    reshape, movedim, transpose, flatten, unfold_dim
+)
+from synapgrad.utils import manual_seed
 
-from .engine import Tensor, tensor, no_grad, manual_seed, retain_grads
+from synapgrad.nn.functional import (
+    relu, tanh, sigmoid, softmax, log_softmax,
+    mse_loss, nll_loss, binary_cross_entropy, binary_cross_entropy_with_logits, cross_entropy,
+    linear, unfold, fold, max_pool1d, max_pool2d, avg_pool1d, avg_pool2d, conv1d, conv2d, batch_norm
+)
+
+from synapgrad import (
+    cpu_ops, conv_tools, device, functional, nn, optim, utils, visual
+)
```

## synapgrad/nn/__init__.py

```diff
@@ -1,8 +1,12 @@
 
-from .modules import Module, Sequential
-from .neurons import Neuron
-from .layers import Linear, Flatten, Unfold, Fold, Conv2d, MaxPool2d, Dropout, BatchNorm, BatchNorm1d, BatchNorm2d
-from .losses import Loss, MSELoss, CrossEntropyLoss, NLLLoss, BCELoss, BCEWithLogitsLoss
-from .activations import relu_fn, ReLU, Tanh, tanh_fn, sigmoid_fn, Sigmoid, softmax_fn, Softmax, LogSoftmax
-from . import functional
-from . import initializations
+from synapgrad.nn.modules import Module, Sequential, Parameter
+from synapgrad.nn.activations import ReLU, Sigmoid, Tanh, Softmax, LogSoftmax
+from synapgrad.nn.losses import (
+    Loss, MSELoss, CrossEntropyLoss, NLLLoss, BCELoss, BCEWithLogitsLoss
+)
+from synapgrad.nn.layers import (
+    Linear, Neuron, Flatten, Unfold, Fold, Dropout,
+    MaxPool1d, MaxPool2d, AvgPool1d, AvgPool2d, Conv1d, Conv2d,
+    BatchNorm1d, BatchNorm2d
+)
+
```

## synapgrad/nn/activations.py

```diff
@@ -1,110 +1,76 @@
-import numpy as np
-from .. import Tensor, nn
-from .functional import relu_fn, tanh_fn, sigmoid_fn, softmax_fn,  log_softmax_fn, epsilon
+from synapgrad.tensor import Tensor
+from synapgrad import nn
+from synapgrad.nn import functional as F
 
 
-# ----------------------------- Modules -----------------------------
-# -------------------------------------------------------------------
+# ************************************
+# ******* Activation Modules *********
+# ************************************
+
 class ReLU(nn.Module):
+    """
+    ReLU activation function. 
+    
+    The ReLU activation function is defined as:
+    f(x) = max(0, x)
+    """
     
     def forward(self, x:Tensor) -> Tensor:
-        relu = relu_fn(x.data)
-        out = Tensor(relu, (x,), '<ReLU>', requires_grad=x.requires_grad)
-
-        def _backward():
-            if x.requires_grad:
-                x._grad += (out.data > 0) * out._grad
-        
-        out._backward = _backward
-
-        return out
+        F.relu.__doc__
+        return F.relu(x)
 
 
 class Tanh(nn.Module):
-    """ np.sinh(x)/np.cosh(x) or -1j * np.tan(1j*x) """
+    """ 
+    Tanh activation function
     
-    def forward(self, x:Tensor) -> Tensor:
-        tanh = tanh_fn(x.data)
-        out = Tensor(tanh, (x,), '<Tanh>', requires_grad=x.requires_grad)
+    It is defined as np.sinh(x)/np.cosh(x) or -1j * np.tan(1j*x) 
+    """
     
-        def _backward():
-            if x.requires_grad:
-                x_grad = 1 - tanh**2
-                x._grad += x_grad * out._grad
-            
-        out._backward = _backward
-        
-        return out
+    def forward(self, x:Tensor) -> Tensor:
+        return F.tanh(x)
 
 
 class Sigmoid(nn.Module):
+    """ 
+    Sigmoid activation function
     
-    def forward(self, x:Tensor) -> Tensor:
-        sigmoid = sigmoid_fn(x.data)
-        out = Tensor(sigmoid, (x,), '<Sigmoid>', requires_grad=x.requires_grad)
+    It is defined as 1/(1+np.exp(-x))
+    """
     
-        def _backward():
-            if x.requires_grad:
-                x_grad = sigmoid * (1 - sigmoid)
-                x._grad += x_grad * out._grad
-            
-        out._backward = _backward
-        
-        return out
+    def forward(self, x:Tensor) -> Tensor:
+        return F.sigmoid(x)
 
     
 class Softmax(nn.Module):
     """ 
-    References: 
-        https://eli.thegreenplace.net/2016/the-softmax-function-and-its-derivative/
-        https://aimatters.wordpress.com/2019/06/17/the-softmax-function-derivative/
+    Softmax activation function
+    
+    It is defined as exp(x)/sum(exp(x))
     """
     
     def __init__(self, dim) -> None:
         super().__init__()
         self.dim = dim
     
     def forward(self, x: Tensor) -> Tensor:
-        softmax = softmax_fn(x.data, self.dim)
-        out = Tensor(softmax, (x,), '<Softmax>', requires_grad=x.requires_grad)
-    
-        def _backward():
-            # Hand made derivation
-            if x.requires_grad:
-                jacobians = np.stack([np.diag(y) - np.outer(y, y) for y in softmax])
-                out_grad = np.expand_dims(out._grad, axis=self.dim)
-                x._grad += (out_grad @ jacobians).sum(axis=self.dim)
-            
-        out._backward = _backward
-        
-        return out
+        return F.softmax(x, self.dim)
 
     
 class LogSoftmax(nn.Module):
     """ 
     Same as Softmax(dim=self.dim)(x).log() but more numerically stable due to the log-sum-exp trick
+    
+    It is defined as log(softmax(x))
             
     Reference to log-sum-exp trick: 
-        https://en.wikipedia.org/wiki/LogSumExp 
+    - https://en.wikipedia.org/wiki/LogSumExp 
     """
     
     def __init__(self, dim) -> None:
         super().__init__()
         self.dim = dim
     
     def forward(self, x: Tensor) -> Tensor:
-        log_softmax = log_softmax_fn(x.data, self.dim)
-        out = Tensor(log_softmax, (x,), '<LogSoftmax>', requires_grad=x.requires_grad)
-    
-        def _backward():
-            if x.requires_grad:
-                softmax = np.exp(log_softmax)
-                jacobians = np.stack([np.diag(y) - np.outer(y, y) for y in softmax])
-                dlog_dsoftmax = (1/(softmax + epsilon)) * out._grad
-                dlog_dsoftmax = np.expand_dims(dlog_dsoftmax, axis=self.dim)
-                x._grad += (dlog_dsoftmax @ jacobians).sum(axis=self.dim)
-            
-        out._backward = _backward
-        
-        return out
+        return F.log_softmax(x, self.dim)
```

## synapgrad/nn/functional.py

```diff
@@ -1,189 +1,937 @@
 import numpy as np
 
+from synapgrad.tensor import Tensor
+from synapgrad import cpu_ops, conv_tools
+from synapgrad.device import Device
+from synapgrad.functional import BackwardFunction
 
-epsilon = 1e-12
 
-# ---------------------------- Functions ----------------------------
-# -------------------------------------------------------------------
-def relu_fn(data:np.ndarray) -> np.ndarray:
-    return np.maximum(0, data)
+# ************************************
+# ******* Activation functions *******
+# ************************************
+
+def relu(x:Tensor):
+    """ 
+    ReLU activation function. 
+    
+    The ReLU activation function is defined as:
+    f(x) = max(0, x)
+
+    Args:
+        x (Tensor): tensor
+
+    Returns:
+        Tensor: result
+    """
+    if not isinstance(x, Tensor):
+        raise TypeError(f"Expected x to be a Tensor but got {type(x)}")
+    
+    if x.device == Device.CPU:
+        out_data = cpu_ops.relu_forward(x.data)
+    else:
+        raise RuntimeError(f"{x.device} not supported")
+
+    out = Tensor(out_data, device=x.device, children=(x,), requires_grad=x.requires_grad, operation="Relu")
+    
+    def backward():
+        grad_output = out.grad
+        if grad_output.device == Device.CPU:
+            a_grad = cpu_ops.relu_backward(grad_output.data, x.data)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if x.requires_grad: x._grad += a_grad 
+    
+    if out.requires_grad: out.grad_fn = BackwardFunction(backward, out._operation)
+        
+    return out
+
+
+def tanh(x:Tensor):
+    """ 
+    Tanh activation function.
+
+    Args:
+        x (Tensor): tensor
+
+    Returns:
+        Tensor: result
+    """
+    if not isinstance(x, Tensor):
+        raise TypeError(f"Expected x to be a Tensor but got {type(x)}")
+    
+    if x.device == Device.CPU:
+        out_data = cpu_ops.tanh_forward(x.data)
+    else:
+        raise RuntimeError(f"{x.device} not supported")
+
+    out = Tensor(out_data, device=x.device, children=(x,), requires_grad=x.requires_grad, operation="Tanh")
+    
+    def backward():
+        grad_output = out.grad
+        if grad_output.device == Device.CPU:
+            a_grad = cpu_ops.tanh_backward(grad_output.data, out.data)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if x.requires_grad: x._grad += a_grad 
+    
+    if out.requires_grad: out.grad_fn = BackwardFunction(backward, out._operation)
+    
+    return out
+
+
+def sigmoid(x:Tensor):
+    """ 
+    Sigmoid activation function. 
+    
+    The Sigmoid activation function is defined as:
+    f(x) = 1 / (1 + exp(-x))
+
+    Args:
+        x (Tensor): tensor
+
+    Returns:
+        Tensor: result
+    """
+    if not isinstance(x, Tensor):
+        raise TypeError(f"Expected x to be a Tensor but got {type(x)}")
+    
+    if x.device == Device.CPU:
+        out_data = cpu_ops.sigmoid_forward(x.data)
+    else:
+        raise RuntimeError(f"{x.device} not supported")
+
+    out = Tensor(out_data, device=x.device, children=(x,), requires_grad=x.requires_grad, operation="Sigmoid")
+    
+    def backward():
+        grad_output = out.grad
+        if grad_output.device == Device.CPU:
+            a_grad = cpu_ops.sigmoid_backward(grad_output.data, out.data)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if x.requires_grad: x._grad += a_grad 
+    
+    if out.requires_grad: out.grad_fn = BackwardFunction(backward, out._operation)
+    
+    return out
 
 
-def tanh_fn(data:np.ndarray) -> np.ndarray:
-    return np.tanh(data)
+def softmax(x:Tensor, dim:int):
+    """ 
+    Softmax activation function. 
+    
+    The Softmax activation function is defined as:
+    f(x) = exp(x) / sum(exp(x))
 
+    Args:
+        x (Tensor): tensor
 
-def sigmoid_fn(data:np.ndarray) -> np.ndarray:
-    return 1/(1 + np.exp(-data))
+    Returns:
+        Tensor: result
+    """
+    if not isinstance(x, Tensor):
+        raise TypeError(f"Expected x to be a Tensor but got {type(x)}")
+    
+    if x.device == Device.CPU:
+        out_data = cpu_ops.softmax_forward(x.data, dim)
+    else:
+        raise RuntimeError(f"{x.device} not supported")
 
+    out = Tensor(out_data, device=x.device, children=(x,), requires_grad=x.requires_grad, operation="Softmax")
+    
+    def backward():
+        grad_output = out.grad
+        if grad_output.device == Device.CPU:
+            a_grad = cpu_ops.softmax_backward(grad_output.data, out.data, dim)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if x.requires_grad: x._grad += a_grad 
+    
+    if out.requires_grad: out.grad_fn = BackwardFunction(backward, out._operation)
+    
+    return out
 
-def softmax_fn(data:np.ndarray, dim:int) -> np.ndarray:
-    # Shift to make it numerically stable (with large values 'inf' appears)
-    shiftx = data - data.max(axis=dim, keepdims=True) 
-    exps = np.exp(shiftx)
-    exp_sums = exps.sum(axis=dim, keepdims=True)
-    return exps / exp_sums
 
+def log_softmax(x:Tensor, dim:int):
+    """ 
+    LogSoftmax activation function. 
+    
+    The LogSoftmax activation function is defined as:
+    f(x) = log(exp(x) / sum(exp(x))) = log(softmax(x))
 
-def log_softmax_fn(data:np.ndarray, dim:int) -> np.ndarray:
-    # Using log-sum-exp trick for numerical stability
-    max_val = data.max(axis=dim, keepdims=True)
-    substract = data - max_val
-    exp = np.exp(substract)
-    lse = max_val + np.log(exp.sum(axis=dim, keepdims=True))
-    log_softmax = data - lse
-    return log_softmax
+    Args:
+        x (Tensor): tensor
 
-# ----------------------------- Losses ------------------------------
-# -------------------------------------------------------------------
-def mse_loss(y_pred: np.ndarray, y_true: np.ndarray) -> np.ndarray:
-    loss = (y_pred - y_true)**2
+    Returns:
+        Tensor: result
+    """
+    if not isinstance(x, Tensor):
+        raise TypeError(f"Expected x to be a Tensor but got {type(x)}")
+    
+    if x.device == Device.CPU:
+        out_data = cpu_ops.log_softmax_forward(x.data, dim)
+    else:
+        raise RuntimeError(f"{x.device} not supported")
+
+    out = Tensor(out_data, device=x.device, children=(x,), requires_grad=x.requires_grad, operation="LogSoftmax")
+
+    def backward():
+        grad_output = out.grad
+        if grad_output.device == Device.CPU:
+            a_grad = cpu_ops.log_softmax_backward(grad_output.data, out.data, dim)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if x.requires_grad: x._grad += a_grad 
+    
+    if out.requires_grad: out.grad_fn = BackwardFunction(backward, out._operation)
+
+    return out
+
+# ******************************
+# ******* Loss functions *******
+# ******************************
+
+def mse_loss(y_pred:Tensor, y_true:Tensor):
+    """ 
+    Mean Squared Error loss function.
+
+    Args:
+        - y_pred (Tensor): tensor
+        - y_true (Tensor): tensor
+
+    Returns:
+        Tensor: result
+    """
+    if not isinstance(y_pred, Tensor):
+        raise TypeError(f"Expected y_pred to be a Tensor but got {type(y_pred)}")
+    if not isinstance(y_true, Tensor):
+        raise TypeError(f"Expected y_true to be a Tensor but got {type(y_true)}")
+    
+    if not y_pred.matches_shape(y_true):
+        raise ValueError(f"Inputs shape don't match y_pred={y_pred.shape}, y_true={y_true.shape}")
+    
+    if y_pred.device == Device.CPU:
+        loss_data = cpu_ops.mse_loss_forward(y_pred.data, y_true.data)
+    else:
+        raise RuntimeError(f"{y_pred.device} not supported")
+
+    inputs = (y_pred, y_true)
+    req_grad = any([inp.requires_grad for inp in inputs])
+    loss = Tensor(loss_data, device=y_pred.device, children=inputs, requires_grad=req_grad, operation="MSELoss")
+    
+    def backward():
+        grad_output = loss.grad
+        if grad_output.device == Device.CPU:
+            loss_grad_data = cpu_ops.mse_loss_backward(grad_output.data, y_pred.data, y_true.data)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if y_pred.requires_grad: y_pred._grad += loss_grad_data
+    
+    if loss.requires_grad: loss.grad_fn = BackwardFunction(backward, loss._operation)
+    
     return loss
+
+
+def nll_loss(y_pred:Tensor, y_true:Tensor):
+    """ 
+    Negative Log Likelihood loss function.
+
+    Args:
+        - y_pred (Tensor): tensor
+        - y_true (Tensor): tensor
+
+    Returns:
+        Tensor: result
+    """
+    if not isinstance(y_pred, Tensor):
+        raise TypeError(f"Expected y_pred to be a Tensor but got {type(y_pred)}")
+    if not isinstance(y_true, Tensor):
+        raise TypeError(f"Expected y_true to be a Tensor but got {type(y_true)}")
+    
+    if y_pred.device == Device.CPU:
+        loss_data = cpu_ops.nll_loss_forward(y_pred.data, y_true.data)
+    else:
+        raise RuntimeError(f"{y_pred.device} not supported")
+
+    inputs = (y_pred, y_true)
+    req_grad = any([inp.requires_grad for inp in inputs])
+    loss = Tensor(loss_data, device=y_pred.device, children=inputs, requires_grad=req_grad, operation="NLLLoss")
     
+    def backward():
+        grad_output = loss.grad
+        if grad_output.device == Device.CPU:
+            loss_grad_data = cpu_ops.nll_loss_backward(grad_output.data, y_pred.data, y_true.data)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if y_pred.requires_grad: y_pred._grad += loss_grad_data
+    
+    if loss.requires_grad: loss.grad_fn = BackwardFunction(backward, loss._operation)
     
-def nll_loss(y_pred: np.ndarray, y_true: np.ndarray) -> np.ndarray:
-    loss = -y_pred[range(len(y_pred)), y_true].reshape((-1, 1))
     return loss
 
 
-def bce_loss(y_pred: np.ndarray, y_true: np.ndarray) -> np.ndarray:
-    assert y_pred.max() <= 1 and y_pred.min() >= 0, "BCELoss inputs must be between 0 and 1"
-    loss = - (y_true * np.log(y_pred + epsilon) + (1 - y_true) * np.log(1 - y_pred + epsilon))
-    # For compatibility with pytorch (returns 100 when y_pred=0 and y_true=1; vice versa)
-    loss = np.where(loss == -np.log(epsilon), 100, loss) 
+def binary_cross_entropy(y_pred:Tensor, y_true:Tensor):
+    """ 
+    Binary Cross Entropy loss function.
+
+    Args:
+        - y_pred (Tensor): tensor
+        - y_true (Tensor): tensor
+
+    Returns:
+        Tensor: result
+    """
+    if not isinstance(y_pred, Tensor):
+        raise TypeError(f"Expected y_pred to be a Tensor but got {type(y_pred)}")
+    if not isinstance(y_true, Tensor):
+        raise TypeError(f"Expected y_true to be a Tensor but got {type(y_true)}")
+    
+    if y_pred.device == Device.CPU:
+        loss_data = cpu_ops.bce_loss_forward(y_pred.data, y_true.data)
+    else:
+        raise RuntimeError(f"{y_pred.device} not supported")
+
+    inputs = (y_pred, y_true)
+    req_grad = any([inp.requires_grad for inp in inputs])
+    loss = Tensor(loss_data, device=y_pred.device, children=inputs, requires_grad=req_grad, operation="BCELoss")
+    
+    def backward():
+        grad_output = loss.grad
+        if grad_output.device == Device.CPU:
+            loss_grad_data = cpu_ops.bce_loss_backward(grad_output.data, y_pred.data, y_true.data)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if y_pred.requires_grad: y_pred._grad += loss_grad_data
+    
+    if loss.requires_grad: loss.grad_fn = BackwardFunction(backward, loss._operation)
+    
     return loss
 
 
-def bce_with_logits_loss(y_pred: np.ndarray, y_true: np.ndarray) -> np.ndarray:
-    tn = -relu_fn(y_pred)
-    loss = (1-y_true) * y_pred + tn + np.log(np.exp(-tn) + np.exp((-y_pred-tn)))
+def binary_cross_entropy_with_logits(y_pred:Tensor, y_true:Tensor):
+    """ 
+    Binary Cross Entropy with Logits loss function.
+
+    Args:
+        - y_pred (Tensor): tensor
+        - y_true (Tensor): tensor
+
+    Returns:
+        Tensor: result
+    """
+    if not isinstance(y_pred, Tensor):
+        raise TypeError(f"Expected y_pred to be a Tensor but got {type(y_pred)}")
+    if not isinstance(y_true, Tensor):
+        raise TypeError(f"Expected y_true to be a Tensor but got {type(y_true)}")
+    
+    if y_pred.device == Device.CPU:
+        loss_data = cpu_ops.bce_with_logits_loss_forward(y_pred.data, y_true.data)
+    else:
+        raise RuntimeError(f"{y_pred.device} not supported")
+
+    inputs = (y_pred, y_true)
+    req_grad = any([inp.requires_grad for inp in inputs])
+    loss = Tensor(loss_data, device=y_pred.device, children=inputs, requires_grad=req_grad, operation="BCEWithLogitsLoss")
+    
+    def backward():
+        grad_output = loss.grad
+        if grad_output.device == Device.CPU:
+            loss_grad_data = cpu_ops.bce_with_logits_loss_backward(grad_output.data, y_pred.data, y_true.data)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if y_pred.requires_grad: y_pred._grad += loss_grad_data
+    
+    if loss.requires_grad: loss.grad_fn = BackwardFunction(backward, loss._operation)
+    
     return loss
+    
+    
+def cross_entropy(y_pred:Tensor, y_true:Tensor):
+    """ 
+    Cross Entropy loss function.
 
+    Args:
+        - y_pred (Tensor): tensor
+        - y_true (Tensor): tensor
 
-def cross_entropy_loss(y_pred: np.ndarray, y_true: np.ndarray) -> np.ndarray:
-    softmax = np.log(softmax_fn(y_pred, 1) + epsilon)
-    log_likelihood = nll_loss(softmax, y_true)
-    return log_likelihood
-
-# ----------------------- Special Functions -------------------------
-# -------------------------------------------------------------------
-def unfold(tensor:np.ndarray, kernel_size, stride=1, padding=0, dilation=1, pad_value=0) -> np.ndarray:
+    Returns:
+        Tensor: result
+    """
+    if not isinstance(y_pred, Tensor):
+        raise TypeError(f"Expected y_pred to be a Tensor but got {type(y_pred)}")
+    if not isinstance(y_true, Tensor):
+        raise TypeError(f"Expected y_true to be a Tensor but got {type(y_true)}")
+    
+    if y_pred.device == Device.CPU:
+        loss_data = cpu_ops.cross_entropy_loss_forward(y_pred.data, y_true.data)
+    else:
+        raise RuntimeError(f"{y_pred.device} not supported")
+
+    inputs = (y_pred, y_true)
+    req_grad = any([inp.requires_grad for inp in inputs])
+    loss = Tensor(loss_data, device=y_pred.device, children=inputs, requires_grad=req_grad, operation="CrossEntropyLoss")
+    
+    def backward():
+        grad_output = loss.grad
+        if grad_output.device == Device.CPU:
+            loss_grad_data = cpu_ops.cross_entropy_loss_backward(grad_output.data, y_pred.data, y_true.data)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if y_pred.requires_grad: y_pred._grad += loss_grad_data
+    
+    if loss.requires_grad: loss.grad_fn = BackwardFunction(backward, loss._operation)
+    
+    return loss
+
+# *********************************
+# ******* Linear functions ********
+# *********************************
+
+def linear(x:Tensor, weight:Tensor, bias:Tensor=None):
+    """ 
+    Linear function. x @ w.T + b
+
+    Args:
+        - x (Tensor): tensor
+        - weight (Tensor): tensor
+        - bias (Tensor): tensor. (default=None)
+
+    Returns:
+        Tensor: result
+    """
+    if not isinstance(x, Tensor):
+        raise TypeError(f"Expected x to be a Tensor but got {type(x)}")
+    if not isinstance(weight, Tensor):
+        raise TypeError(f"Expected weight to be a Tensor but got {type(weight)}")
+    if bias is not None and not isinstance(bias, Tensor):
+        raise TypeError(f"Expected not None bias to be a Tensor but got {type(bias)}")
+    
+    if x.device == Device.CPU:
+        if bias:
+            out_data = cpu_ops.addmm_forward(bias.data, x.data, weight.data.T)
+        else:
+            out_data = cpu_ops.matmul_forward(x.data, weight.data.T)
+    else:
+        raise RuntimeError(f"{x.device} not supported")
+    
+    if bias: inputs = (x, weight, bias)
+    else: inputs = (x, weight)
+    
+    req_grad = any([inp.requires_grad for inp in inputs])
+    out = Tensor(out_data, device=x.device, children=inputs, requires_grad=req_grad, operation="Linear")
+        
+    def backward():
+        grad_output = out.grad
+        if out.device == Device.CPU:
+            if bias:
+                bias_grad, x_grad, weight_grad = cpu_ops.addmm_backward(grad_output.data, bias.data, x.data, weight.data.T)
+            else:
+                x_grad, weight_grad = cpu_ops.matmul_backward(grad_output.data, x.data, weight.data.T)
+        else:
+            raise RuntimeError(f"{out.device} not supported")
+        
+        if x.requires_grad: 
+            x._grad += x_grad
+        if weight.requires_grad: 
+            weight._grad += weight_grad.T
+        if bias and bias.requires_grad: 
+            bias._grad += bias_grad
+            
+    if out.requires_grad: out.grad_fn = BackwardFunction(backward, out._operation)
+    
+    return out
+
+# *******************************
+# ******* Pool functions ********
+# *******************************
+
+def max_pool1d(x:Tensor, kernel_size, stride=None, padding=0, dilation=1):
+    """
+    Max-pooling operation for 1D data.
+    
+    Reference:
+        https://pytorch.org/docs/stable/generated/torch.nn.MaxPool1d.html
+
+    Args:
+        - x (Tensor): Input tensor of shape (N, C, W).
+        - kernel_size (int): Size of the sliding window.
+        - stride (int, optional): Stride size. Defaults to kernel_size.
+        - padding (int, optional): Padding size. Defaults to 0.
+        - dilation (int, optional): Dilation factor. Defaults to 1.
+
+    Returns:
+        Tensor: Output tensor of shape (N, C, L).
+    """
+    if stride is None: stride = kernel_size
+    
+    if not isinstance(x, Tensor):
+        raise TypeError(f"Expected x to be a Tensor but got {type(x)}")
+    
+    if len(x.shape) != 3:
+        raise ValueError(f"Input tensor must be of shape (N, C, L), but got {x.shape}")
+    
+    if x.device == Device.CPU:
+        out_data, *bw_data = cpu_ops.max_pool1d_forward(x.data, kernel_size, stride, padding, dilation)
+    else:
+        raise RuntimeError(f"{x.device} not supported")
+
+    out = Tensor(out_data, device=x.device, children=(x,), requires_grad=x.requires_grad, operation="MaxPool1d")
+    
+    def backward():
+        grad_output = out.grad
+        if grad_output.device == Device.CPU:
+            x_grad = \
+                cpu_ops.max_pool1d_backward(grad_output.data, kernel_size, stride, padding, dilation, *bw_data)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if x.requires_grad: x._grad += x_grad
+            
+    if out.requires_grad: out.grad_fn = BackwardFunction(backward, out._operation)
+    
+    return out
+
+
+def max_pool2d(x:Tensor, kernel_size, stride=None, padding=0, dilation=1):
+    """ 
+    Max-pooling function.
+    
+    Reference:
+        https://pytorch.org/docs/stable/generated/torch.nn.MaxPool2d.html
+
+    Args:
+        - tensor (numpy.ndarray): Input tensor of shape (N, C, H, W).
+        - kernel_size (int or tuple): Size of the sliding window.
+        - stride (int or tuple, optional): Stride size. Defaults to kernel_size.
+        - padding (int or tuple, optional): Padding size. Defaults to 0.
+        - dilation (int or tuple, optional): Dilation factor. Defaults to 1.
+
+    Returns:
+        numpy.ndarray: Output tensor of shape (N, C, lH, lW).
+    """
+    if stride is None: stride = kernel_size
+    
+    if not isinstance(x, Tensor):
+        raise TypeError(f"Expected x to be a Tensor but got {type(x)}")
+    
+    if len(x.shape) != 4:
+        raise ValueError(f"Input tensor must be of shape (N, C, H, W), but got {x.shape}")
+    
+    if x.device == Device.CPU:
+        out_data, *bw_data = cpu_ops.max_pool2d_forward(x.data, kernel_size, stride, padding, dilation)
+    else:
+        raise RuntimeError(f"{x.device} not supported")
+
+    out = Tensor(out_data, device=x.device, children=(x,), requires_grad=x.requires_grad, operation="MaxPool2d")
+    
+    def backward():
+        grad_output = out.grad
+        if grad_output.device == Device.CPU:
+            x_grad = cpu_ops.max_pool2d_backward(grad_output.data, kernel_size, stride, padding, dilation, *bw_data)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if x.requires_grad: x._grad += x_grad
+            
+    if out.requires_grad: out.grad_fn = BackwardFunction(backward, out._operation)
+    
+    return out
+
+
+def avg_pool1d(x:Tensor, kernel_size, stride=None, padding=0, dilation=1):
+    """ 
+    Average-pooling function.
+    
+    Reference:
+        https://pytorch.org/docs/stable/generated/torch.nn.AvgPool1d.html
+
+    Args:
+        - tensor (numpy.ndarray): Input tensor of shape (N, C, W).
+        - kernel_size (int or tuple): Size of the sliding window.
+        - stride (int or tuple, optional): Stride size. Defaults to kernel_size.
+        - padding (int or tuple, optional): Padding size. Defaults to 0.
+        - dilation (int or tuple, optional): Dilation factor. Defaults to 1.
+
+    Returns:
+        numpy.ndarray: Output tensor of shape (N, C, L).
+    """
+    if stride is None: stride = kernel_size
+    
+    if not isinstance(x, Tensor):
+        raise TypeError(f"Expected x to be a Tensor but got {type(x)}")
+    
+    if len(x.shape) != 3:
+        raise ValueError(f"Input tensor must be of shape (N, C, L), but got {x.shape}")
+    
+    if x.device == Device.CPU:
+        out_data, *bw_data = cpu_ops.avg_pool1d_forward(x.data, kernel_size, stride, padding, dilation)
+    else:
+        raise RuntimeError(f"{x.device} not supported")
+
+    out = Tensor(out_data, device=x.device, children=(x,), requires_grad=x.requires_grad, operation="AvgPool1d")
+    
+    def backward():
+        grad_output = out.grad
+        if grad_output.device == Device.CPU:
+            x_grad = cpu_ops.avg_pool1d_backward(grad_output.data, kernel_size, stride, padding, dilation, *bw_data)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if x.requires_grad: x._grad += x_grad
+            
+    if out.requires_grad: out.grad_fn = BackwardFunction(backward, out._operation)
+    
+    return out
+
+
+def avg_pool2d(x:Tensor, kernel_size, stride=None, padding=0, dilation=1):
+    """ 
+    Average-pooling function.
+    
+    Reference:
+        https://pytorch.org/docs/stable/generated/torch.nn.AvgPool2d.html
+
+    Args:
+        - tensor (numpy.ndarray): Input tensor of shape (N, C, H, W).
+        - kernel_size (int or tuple): Size of the sliding window.
+        - stride (int or tuple, optional): Stride size. Defaults to kernel_size.
+        - padding (int or tuple, optional): Padding size. Defaults to 0.
+        - dilation (int or tuple, optional): Dilation factor. Defaults to 1.
+
+    Returns:
+        numpy.ndarray: Output tensor of shape (N, C, lH , lW).
+    """
+    if stride is None: stride = kernel_size
+    
+    if not isinstance(x, Tensor):
+        raise TypeError(f"Expected x to be a Tensor but got {type(x)}")
+    
+    if len(x.shape) != 4:
+        raise ValueError(f"Input tensor must be of shape (N, C, H, W), but got {x.shape}")
+    
+    if x.device == Device.CPU:
+        out_data, *bw_data = cpu_ops.avg_pool2d_forward(x.data, kernel_size, stride, padding, dilation)
+    else:
+        raise RuntimeError(f"{x.device} not supported")
+
+    out = Tensor(out_data, device=x.device, children=(x,), requires_grad=x.requires_grad, operation="AvgPool2d")
+    
+    def backward():
+        grad_output = out.grad
+        if grad_output.device == Device.CPU:
+            x_grad = cpu_ops.avg_pool2d_backward(grad_output.data, kernel_size, stride, padding, dilation, *bw_data)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if x.requires_grad: x._grad += x_grad
+            
+    if out.requires_grad: out.grad_fn = BackwardFunction(backward, out._operation)
+    
+    return out
+
+# *******************************
+# ******* Conv functions ********
+# *******************************
+
+def unfold(x:Tensor, kernel_size:'int | tuple', dilation:'int | tuple'=1, stride:'int | tuple'=1, padding:'int | tuple'=0, pad_value=0) -> Tensor:
     """
     Unfold a tensor of shape (N, C, H, W) to a tensor in the shape of (N, C*kH*kW, L)
     
     Reference: 
         https://pytorch.org/docs/stable/generated/torch.nn.Unfold.html
 
     Args:
-        tensor (numpy.ndarray): Input tensor of shape (N, C, H, W).
-        kernel_size (int or tuple): Size of the sliding window.
-        stride (int or tuple, optional): Stride size. Defaults to 1.
-        padding (int or tuple, optional): Padding size. Defaults to 0.
-        dilation (int or tuple, optional): Dilation factor. Defaults to 1.
+        - tensor (numpy.ndarray): Input tensor of shape (N, C, H, W).
+        - kernel_size (int or tuple): Size of the sliding window.
+        - dilation (int or tuple, optional): Dilation factor. Defaults to 1.
+        - stride (int or tuple, optional): Stride size. Defaults to 1.
+        - padding (int or tuple, optional): Padding size. Defaults to 0.
 
     Returns:
         numpy.ndarray: Output tensor of shape (N, C*kH*kW, L).
     """
-    assert len(tensor.shape) == 4, "Input tensor must be of shape (N, C, H, W)"
-    N, C, H, W = tensor.shape
-    kernel_size = np.broadcast_to(kernel_size, 2)
-    dilation = np.broadcast_to(dilation, 2)
-    padding = np.broadcast_to(padding, 2)
-    stride = np.broadcast_to(stride, 2)
-
-    # Calculate output spatial size
-    lH = int(np.floor((H + 2 * padding[0] - dilation[0] * (kernel_size[0] - 1) - 1) / stride[0] + 1))
-    lW = int(np.floor((W + 2 * padding[1] - dilation[1] * (kernel_size[1] - 1) - 1) / stride[1] + 1))
-    L = lH*lW
-    
-    if L <= 0:
-        raise RuntimeError('Cannot unfold a tensor with zero or negative spatial size (L='+str(L)+
-            ') for kernel_size='+str(kernel_size)+', stride='+str(stride)+', padding='+str(padding)+
-            ', dilation='+str(dilation)+' and tensor shape='+str(tensor.shape))
-    
-    # Pad input
-    padded_input = np.pad(
-        tensor, ((0, 0), (0, 0)) + tuple((padding[d], padding[d]) for d in range(2)),
-        mode='constant', constant_values=pad_value)
-    
-    # Initialize output tensor
-    output_size = (N, C * np.prod(kernel_size), L)
-    output = np.zeros(output_size, dtype=tensor.dtype)
-    
-    # Extract sliding window for each input channel and put it in the output tensor
-    for i in range(lH):
-        for j in range(lW):
-            # Height parameters
-            h_start = i * stride[0]
-            h_end = i * stride[0] + kernel_size[0] + (dilation[0] - 1) * (kernel_size[0] - 1)
-            h_step = dilation[0]
-            # Width parameters
-            w_start = j * stride[1]
-            w_end = j * stride[1] + kernel_size[1] + (dilation[1] - 1) * (kernel_size[1] - 1)
-            w_step = dilation[1]
-            # Extract sliding window
-            window = padded_input[:, :, h_start:h_end:h_step, w_start:w_end:w_step]
-            output[:, :, i*lW + j] = window.ravel().reshape(output[:, :, i*lW + j].shape)
+    if not isinstance(x, Tensor):
+        raise TypeError(f"Expected x to be a Tensor but got {type(x)}")
+    
+    if len(x.shape) != 4:
+        raise ValueError(f"Input tensor must be of shape (N, C, H, W), but got {x.shape}")
+    
+    if x.device == Device.CPU:
+        out_data = \
+            conv_tools.im2col_fast(x.data, kernel_size, dilation, stride, padding, pad_value, as_unfold=True)
+    else:
+        raise RuntimeError(f"{x.device} not supported")
+
+    out = Tensor(out_data, device=x.device, children=(x,), requires_grad=x.requires_grad, operation="Unfold")
+    
+    def backward():
+        grad_output = out.grad
+        if grad_output.device == Device.CPU:
+            x_grad = conv_tools.col2im_fast(grad_output.data, x.shape, kernel_size, dilation, stride, padding)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if x.requires_grad: x._grad += x_grad
             
-    return output
+    if out.requires_grad: out.grad_fn = BackwardFunction(backward, out._operation)
+    
+    return out
 
 
-def fold(tensor:np.ndarray, output_size, kernel_size, stride=1, padding=0, dilation=1):
+def fold(x:Tensor, output_size:tuple, kernel_size:'int | tuple', dilation:'int | tuple'=1, stride:'int | tuple'=1, padding:'int | tuple'=0) -> Tensor:
     """
     Fold a tensor of shape (N, C*kH*kW, L) to a tensor in the shape of (N, C, H, W).
     
     Reference:
         https://pytorch.org/docs/stable/generated/torch.nn.Fold.html
 
     Args:
-        tensor (numpy.ndarray): Input tensor of shape (N, C*kH*kW, L).
-        kernel_size (int or tuple): Size of the sliding window.
-        output_size (tuple): Desired output size of the folded tensor, in the form of (H, W).
-        stride (int or tuple, optional): Stride size. Defaults to 1.
-        padding (int or tuple, optional): Padding size. Defaults to 0.
-        dilation (int or tuple, optional): Dilation factor. Defaults to 1.
+        - tensor (numpy.ndarray): Input tensor of shape (N, C*kH*kW, L).
+        - output_size (tuple): Desired output size of the folded tensor, in the form of (H, W).
+        - kernel_size (int or tuple): Size of the sliding window.
+        - dilation (int or tuple, optional): Dilation factor. Defaults to 1.
+        - stride (int or tuple, optional): Stride size. Defaults to 1.
+        - padding (int or tuple, optional): Padding size. Defaults to 0.
 
     Returns:
         numpy.ndarray: Output tensor of shape (N, C, H, W).
     """
-    N, CkHkW, L = tensor.shape
-    kernel_size = np.broadcast_to(kernel_size, 2)
-    dilation = np.broadcast_to(dilation, 2)
-    padding = np.broadcast_to(padding, 2)
-    stride = np.broadcast_to(stride, 2)
-
-    C = CkHkW // np.prod(kernel_size)
-    H, W = output_size
-    
-    H_with_pad = H + 2 * padding[0]
-    W_with_pad = W + 2 * padding[1]
-    
-    # Calculate input spatial size
-    lH = int(np.floor((H_with_pad - dilation[0] * (kernel_size[0] - 1) - 1) / stride[0] + 1))
-    lW = int(np.floor((W_with_pad - dilation[1] * (kernel_size[1] - 1) - 1) / stride[1] + 1))
-
-    # Initialize output tensor
-    output = np.zeros((N, C, H_with_pad, W_with_pad), dtype=tensor.dtype)
-
-    # Reshape input tensor to match the expected shape of the output tensor
-    tensor = tensor.reshape((N, C, np.prod(kernel_size), L))
-
-    # Undo the sliding window operation and place the values back in the output tensor
-    for i in range(lH):
-        for j in range(lW):
-            h_start = i * stride[0]
-            h_end = i * stride[0] + kernel_size[0] + (dilation[0] - 1) * (kernel_size[0] - 1)
-            h_step = dilation[0]
-            w_start = j * stride[1]
-            w_end = j * stride[1] + kernel_size[1] + (dilation[1] - 1) * (kernel_size[1] - 1)
-            w_step = dilation[1]
-            # Calculate the output window
-            o = output[:, :, h_start:h_end:h_step, w_start:w_end:w_step]
-            window = tensor[:, :, :, i*lW + j].reshape(o.shape)
-            output[:, :, h_start:h_end:h_step, w_start:w_end:w_step] = o + window
-
-    # Remove padding if necessary
-    if padding[0] > 0 or padding[1] > 0:
-        output = output[:, :, padding[0]:H_with_pad-padding[0], padding[1]:W_with_pad-padding[1]]
+    if not isinstance(x, Tensor):
+        raise TypeError(f"Expected x to be a Tensor but got {type(x)}")
+    
+    if len(x.shape) != 3:
+        raise ValueError(f"Input tensor must be of shape (N, C*kH*kW, L), but got {x.shape}")
+    
+    if x.device == Device.CPU:
+        out_data = \
+            conv_tools.col2im_fast(x.data, output_size, kernel_size, dilation, stride, padding)
+    else:
+        raise RuntimeError(f"{x.device} not supported")
+
+    out = Tensor(out_data, device=x.device, children=(x,), requires_grad=x.requires_grad, operation="Fold")
+    
+    def backward():
+        grad_output = out.grad
+        if grad_output.device == Device.CPU:
+            x_grad = \
+                conv_tools.im2col_fast(grad_output.data, kernel_size, dilation, stride, padding, as_unfold=True)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if x.requires_grad: x._grad += x_grad
+            
+    if out.requires_grad: out.grad_fn = BackwardFunction(backward, out._operation)
+    
+    return out
+
+
+def conv1d(x:Tensor, weight:Tensor, bias:Tensor=None, stride:int=1, padding:int=0, dilation:int=1) -> Tensor:
+    """
+    1D convolution.
+    
+    Reference:
+        https://pytorch.org/docs/stable/generated/torch.nn.Conv1d.html
+
+    Args:
+        - x (Tensor): Input tensor of shape (N, C, W).
+        - weight (Tensor): Weight tensor of shape (C_out, C, kW).
+        - bias (Tensor, optional): Bias tensor of shape (C_out,). Defaults to None.
+        - stride (int, optional): Stride size. Defaults to 1.
+        - padding (int, optional): Padding size. Defaults to 0.
+        - dilation (int, optional): Dilation factor. Defaults to 1.
 
-    return output
+    Returns:
+        numpy.ndarray: Output tensor of shape (N, C_out, L).
+    """
+    if not isinstance(x, Tensor):
+        raise TypeError(f"Expected x to be a Tensor but got {type(x)}")
+    
+    if not isinstance(weight, Tensor):
+        raise TypeError(f"Expected weight to be a Tensor but got {type(weight)}")
+    
+    if bias is not None and not isinstance(bias, Tensor):
+        raise TypeError(f"Expected bias to be a Tensor but got {type(bias)}")
+    
+    if x.device == Device.CPU:
+        bias_data = bias.data if bias is not None else None
+        out_data, *bw_data = cpu_ops.conv1d_forward(x.data, weight.data, bias_data, stride, padding, dilation)
+    else:
+        raise RuntimeError(f"{x.device} not supported")
+
+    if bias: inputs = (x, weight, bias)
+    else: inputs = (x, weight)
+    
+    req_grad = any([inp.requires_grad for inp in inputs])
+    out = Tensor(out_data, device=x.device, children=inputs, requires_grad=req_grad, operation="Conv1d")
+
+    def backward():
+        grad_output = out.grad
+        if grad_output.device == Device.CPU:
+            bias_data = bias.data if bias is not None else None
+            x_grad, weight_grad, bias_grad = cpu_ops.conv1d_backward(grad_output.data, x.shape, weight.data,
+                                                        bias_data, stride, padding, dilation, *bw_data)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if x.requires_grad:
+            x._grad += x_grad
+        if weight.requires_grad:
+            weight._grad += weight_grad    
+        if bias and bias.requires_grad:
+            bias._grad += bias_grad
+            
+    if out.requires_grad: out.grad_fn = BackwardFunction(backward, out._operation)
+
+    return out
+
+
+def conv2d(x:Tensor, weight:Tensor, bias:Tensor=None, stride=1, padding=0, dilation=1) -> Tensor:
+    """
+    Applies 2D convolution to an input tensor.
+    
+    Reference:
+        https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html
+
+    Args:
+        - x (Tensor): Input tensor of shape (N, C, H, W).
+        - weight (Tensor): Weight tensor of shape (C_out, C, kH, kW).
+        - bias (Tensor, optional): Bias tensor of shape (C_out). Defaults to None.
+        - stride (tuple | int, optional): Stride size. Defaults to 1.
+        - padding (tuple | int, optional): Padding size. Defaults to 0.
+        - dilation (tuple | int, optional): Dilation factor. Defaults to 1.
+
+    Returns:
+        Tensor: Output tensor of shape (N, C_out, lH, lW).
+    """
+    
+    if not isinstance(x, Tensor):
+        raise TypeError(f"Expected x to be a Tensor but got {type(x)}")
+    
+    if not isinstance(weight, Tensor):
+        raise TypeError(f"Expected weight to be a Tensor but got {type(weight)}")
+    
+    if bias is not None and not isinstance(bias, Tensor):
+        raise TypeError(f"Expected bias to be a Tensor but got {type(bias)}")
+    
+    if x.device == Device.CPU:
+        bias_data = bias.data if bias is not None else None
+        out_data, *bw_data = cpu_ops.conv2d_forward(x.data, weight.data, bias_data, stride, padding, dilation)
+    else:
+        raise RuntimeError(f"{x.device} not supported")
+
+    if bias: inputs = (x, weight, bias)
+    else: inputs = (x, weight)
+    
+    req_grad = any([inp.requires_grad for inp in inputs])
+    out = Tensor(out_data, device=x.device, children=inputs, requires_grad=req_grad, operation="Conv2d")
+    
+    def backward():
+        grad_output = out.grad
+        if grad_output.device == Device.CPU:
+            bias_data = bias.data if bias is not None else None
+            x_grad, weight_grad, bias_grad = cpu_ops.conv2d_backward(grad_output.data, x.shape, weight.data,
+                                                        bias_data, stride, padding, dilation, *bw_data)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if x.requires_grad:
+            x._grad += x_grad
+        if weight.requires_grad:
+            weight._grad += weight_grad    
+        if bias and bias.requires_grad:
+            bias._grad += bias_grad
+            
+    if out.requires_grad: out.grad_fn = BackwardFunction(backward, out._operation)
+    
+    return out
+
+# *************************************
+# ******* Batch norm functions ********
+# *************************************
+
+def batch_norm(x:Tensor, weight:Tensor=None, bias:Tensor=None, running_mean:Tensor=None, running_var:Tensor=None,
+                training=True, momentum=0.1, eps=1e-5) -> Tensor:
+    """
+    Applies batch normalization to an input tensor.
+    
+    Reference:
+        - https://pytorch.org/docs/stable/generated/torch.nn.BatchNorm1d.html
+        - https://pytorch.org/docs/stable/generated/torch.nn.BatchNorm2d.html
+
+    Args:
+        - x (Tensor): Input tensor of shape (N, C, *).
+        - running_mean (Tensor, optional): Running mean tensor of shape (C,). Defaults to None.
+        - running_var (Tensor, optional): Running variance tensor of shape (C,). Defaults to None.
+        - weight (Tensor, optional): Weight tensor of shape (C,) also called `gamma`. Defaults to None.
+        - bias (Tensor, optional): Bias tensor of shape (C,) also called `beta`. Defaults to None.
+        - training (bool, optional): If true, use batch norm in training mode. Defaults to True.
+        - momentum (float, optional): Momentum. Defaults to 0.1.
+        - eps (float, optional): Epsilon. Defaults to 1e-5.
+
+    Returns:
+        Tensor: Output tensor batch normalized of shape (N, C, *)
+    """
+    if not isinstance(x, Tensor):
+        raise TypeError(f"Expected x to be a Tensor but got {type(x)}")
+    
+    if running_mean is not None and not isinstance(running_mean, Tensor):
+        raise TypeError(f"Expected running_mean to be a Tensor but got {type(running_mean)}")
+    
+    if running_var is not None and not isinstance(running_var, Tensor):
+        raise TypeError(f"Expected running_var to be a Tensor but got {type(running_var)}")
+    
+    if weight is not None and not isinstance(weight, Tensor):
+        raise TypeError(f"Expected weight to be a Tensor but got {type(weight)}")
+    
+    if bias is not None and not isinstance(bias, Tensor):
+        raise TypeError(f"Expected bias to be a Tensor but got {type(bias)}")
+    
+    running_mean_data = running_mean.data if running_mean is not None else None
+    running_var_data = running_var.data if running_var is not None else None
+    weight_data = weight.data if weight is not None else None
+    bias_data = bias.data if bias is not None else None
+    
+    if x.device == Device.CPU:
+        out_data, new_running_mean, new_running_var, *bw_data = cpu_ops.batch_norm_forward(x.data, weight_data, bias_data,
+                                              running_mean_data, running_var_data, training, momentum, eps)
+    else:
+        raise RuntimeError(f"{x.device} not supported")
+    
+    if new_running_mean is not None: running_mean.data = new_running_mean
+    if new_running_var is not None: running_var.data = new_running_var
+    
+    inputs = (x,)
+    if weight is not None: inputs += (weight,)
+    if bias is not None: inputs += (bias,)
+    req_grad = any([inp.requires_grad for inp in inputs])
+    out = Tensor(out_data, device=x.device, children=inputs, requires_grad=req_grad, operation="BatchNorm")
+    
+    def backward():
+        grad_output = out.grad
+        if grad_output.device == Device.CPU:
+            track_running_stats = running_mean is not None and running_var is not None
+            x_grad, weight_grad, bias_grad = \
+                cpu_ops.batch_norm_backward(grad_output.data, x.data, weight_data, bias_data,
+                                                            track_running_stats, training, eps, *bw_data)
+        else:
+            raise RuntimeError(f"{grad_output.device} not supported")
+        
+        if x.requires_grad:
+            x._grad += x_grad
+        if weight is not None and weight.requires_grad:
+            weight._grad += weight_grad    
+        if bias is not None and bias.requires_grad:
+            bias._grad += bias_grad
+            
+    if out.requires_grad: out.grad_fn = BackwardFunction(backward, out._operation)
+    
+    return out
```

## synapgrad/nn/initializations.py

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 
-# Referece to keras code: https://github.com/keras-team/keras/blob/998efc04eefa0c14057c1fa87cab71df5b24bf7e/keras/initializations.py
+# Referece to keras code: 
+# https://github.com/keras-team/keras/blob/998efc04eefa0c14057c1fa87cab71df5b24bf7e/keras/initializations.py
 
 
 weight_initializers = ['glorot_normal', 'glorot_uniform', 'he_normal', 'he_uniform', 'lecun_uniform']
 
 
 def init_weights(shape, method) -> np.ndarray:
     if method not in weight_initializers:
@@ -28,52 +29,56 @@
 
 
 def normal(shape, scale=0.05) -> np.ndarray:
     return np.random.normal(loc=0.0, scale=scale, size=shape)
 
 
 def lecun_uniform(shape) -> np.ndarray:
-    ''' Reference: LeCun 98, Efficient Backprop
+    ''' 
+    Reference: LeCun 98, Efficient Backprop
         http://yann.lecun.com/exdb/publis/pdf/lecun-98b.pdf
     '''
     fan_in, fan_out = get_fans(shape)
     scale = np.sqrt(3. / fan_in)
     return uniform(shape, scale)
 
 
 def glorot_normal(shape) -> np.ndarray:
-    ''' Reference: Glorot & Bengio, AISTATS 2010
+    ''' 
+    Reference: Glorot & Bengio, AISTATS 2010
     '''
     fan_in, fan_out = get_fans(shape)
     s = np.sqrt(2. / (fan_in + fan_out))
     return normal(shape, s)
 
 
 def glorot_uniform(shape) -> np.ndarray:
     fan_in, fan_out = get_fans(shape)
     s = np.sqrt(6. / (fan_in + fan_out))
     return uniform(shape, s)
 
 
 def he_normal(shape) -> np.ndarray:
-    ''' Reference:  He et al., http://arxiv.org/abs/1502.01852
+    ''' 
+    Reference:  He et al., http://arxiv.org/abs/1502.01852
     '''
     fan_in, fan_out = get_fans(shape)
     s = np.sqrt(2. / fan_in)
     return normal(shape, s)
 
 
 def he_uniform(shape) -> np.ndarray:
     fan_in, fan_out = get_fans(shape)
     s = np.sqrt(6. / fan_in)
     return uniform(shape, s)
 
 
 def orthogonal(shape, scale=1.1) -> np.ndarray:
-    ''' From Lasagne. Reference: Saxe et al., http://arxiv.org/abs/1312.6120
+    ''' 
+    From Lasagne. Reference: Saxe et al., http://arxiv.org/abs/1312.6120
     '''
     flat_shape = (shape[0], np.prod(shape[1:]))
     a = np.random.normal(0.0, 1.0, flat_shape)
     u, _, v = np.linalg.svd(a, full_matrices=False)
     # pick the one with the correct shape
     q = u if u.shape == flat_shape else v
     q = q.reshape(shape)
```

## synapgrad/nn/layers.py

```diff
@@ -1,91 +1,213 @@
 import numpy as np
-from .. import nn, Tensor, engine
-from .neurons import init_weights
-from .functional import unfold, fold
-from .initializations import init_weights
+import synapgrad
+from synapgrad import nn
+from synapgrad.tensor import Tensor
+from synapgrad.nn import functional as F
+from synapgrad.nn.initializations import init_weights
 
 
 class Linear(nn.Module):
     
-    def __init__(self, input_size:int, output_size:int, weight_init_method='he_normal'):
+    def __init__(self, input_size:int, output_size:int, weight_init_method='he_normal', bias=True):
+        """ 
+        Applies a linear transformation to the incoming data: y = x @ w.T + b. 
+        
+        This layer is also known as Dense layer.
+        
+        Reference:
+            - https://pytorch.org/docs/stable/generated/torch.nn.Linear.html
+        
+        Args:
+            input_size (int): The number of features in the input tensor.
+            output_size (int): The number of features in the output tensor.
+            weight_init_method (str): The method to use for initializing the weights.
+                Options are 'glorot_normal', 'glorot_uniform', 'he_normal', 'he_uniform', 'lecun_uniform'.
+                Defaults to 'he_normal'.
+            bias: Whether to use a bias or not. Defaults to True.
+        
+        Returns:
+            A tensor of shape (batch_size, output_size)
+        
+        Notes:
+            - The weights are initialized using the method specified in `weight_init_method`.
+            - The bias is initialized to zero.
+            - The input tensor is expected to have a shape of (batch_size, input_size).
+            - The output tensor is expected to have a shape of (batch_size, output_size).
+        
+        Example:
+            >>> layer = nn.Linear(input_size=3, output_size=4)
+            >>> x = synapgrad.ones((2, 3))
+            >>> y = layer(x)
+        """
         super().__init__()
         self.input_size = input_size
         self.output_size = output_size
         
         self.weight_init_method = weight_init_method
         weight_values = init_weights((output_size, input_size), weight_init_method).astype(np.float32)
-        self.weight = Tensor(weight_values, requires_grad=True)
-        self.bias = Tensor.zeros((output_size,), dtype=np.float32, requires_grad=True)
+        self.weight = nn.Parameter(weight_values, requires_grad=True, name='weight')
+        if bias: 
+            bias = synapgrad.zeros((output_size,), dtype=np.float32, requires_grad=True, name='bias')
+            self.bias = nn.Parameter(bias)
+        else: self.bias = None
         
     def forward(self, x:Tensor) -> Tensor:
         assert x.shape[1] == self.input_size, f"Expected input size '{self.input_size}' but received '{x.shape[1]}'"
+        return F.linear(x, self.weight, self.bias)
 
-        out = (x @ self.weight.transpose(0,1)) + self.bias
 
-        return out
-    
-    def parameters(self) -> list[Tensor]:
-        return [self.weight, self.bias]
-    
-    def __repr__(self) -> str:
-        return f"Linear(input_size={self.input_size}, neurons={len(self.output_size)})"
+class Neuron(Linear):
 
+    def __init__(self, input_size: int, weight_init_method='he_normal', bias=True):
+        """ 
+        Creates a single Neuron layer. It's just a linear layer with output_size = 1
+        
+        Reference:
+            - https://pytorch.org/docs/stable/generated/torch.nn.Linear.html
+        
+        Args:
+            input_size (int): The number of features in the input tensor.
+            weight_init_method (str): The method to use for initializing the weights.
+                Options are 'glorot_normal', 'glorot_uniform', 'he_normal', 'he_uniform', 'lecun_uniform'.
+                Defaults to 'he_normal'.
+            bias: Whether to use a bias or not. Defaults to True.
+         
+        Returns:
+            A tensor of shape (batch_size, 1)
+        
+        Example:
+            >>> layer = nn.Neuron(input_size=3)
+            >>> x = synapgrad.ones((2, 3))
+        """
+        super().__init__(input_size, 1, weight_init_method=weight_init_method, bias=bias)
+    
 
 class Flatten(nn.Module):
     
     def __init__(self, start_dim=1, end_dim=-1) -> None:
+        """ 
+        Flattens a tensor over the specified start and end dimensions
+        
+        Reference:
+            - https://pytorch.org/docs/stable/generated/torch.flatten.html
+            
+        Args:
+            start_dim (int): The dimension to start flattening.
+            end_dim (int): The dimension to end flattening.
+        
+        Returns:
+            A tensor of shape (batch_size, *output_shape)
+        
+        Example:
+            >>> layer = nn.Flatten()
+            >>> x = synapgrad.ones((2, 3, 4, 5))
+            >>> y = layer(x)
+        """
         super().__init__()
         self.start_dim = start_dim
         self.end_dim = end_dim
     
     def forward(self, x: Tensor) -> Tensor:
         return x.flatten(self.start_dim, self.end_dim)
     
+
+class Dropout(nn.Module):
+
+    def __init__(self, p=0.5) -> None:
+        """
+        Randomly zeroes some of the elements of the input tensor with probability p
+        using samples from a Bernoulli distribution. The values are also scaled by 1/(1-p)
+        
+        Reference:
+            - https://pytorch.org/docs/stable/generated/torch.nn.Dropout.html
+            
+        Args:
+            p (float): The probability of an element to be zeroed.
+        
+        Returns:
+            A tensor of the same shape as the input tensor.
+        
+        Example:
+            >>> layer = nn.Dropout(p=0.5)
+            >>> x = synapgrad.ones((2, 3))
+            >>> y = layer(x)
+        """
+        super().__init__()
+        self.p = p
+        
+    def forward(self, x: Tensor) -> Tensor:
+        if not self.training: return x
+        random_data = np.random.rand(*x.shape)
+        random_data = np.where(random_data <= self.p, 0, 1)
+        if self.p < 1:
+            random_data = random_data / (1-self.p) # scale data
+        random_t = synapgrad.tensor(random_data)
+        
+        return x*random_t
+    
     
 class Unfold(nn.Module):
-    """ Check nn.funcional.unfold for more information """
     
     def __init__(self, kernel_size, stride=1, padding=0, dilation=1, pad_value=0) -> None:
+        """ 
+        Unfolds tensor. See nn.functional.unfold for more information
+        
+        Reference:
+            - https://pytorch.org/docs/stable/generated/torch.nn.Unfold.html
+            
+        Args:
+            kernel_size (int or tuple): The size of the sliding window.
+            stride (int or tuple): The stride of the sliding window.
+            padding (int or tuple): The padding of the sliding window.
+            dilation (int or tuple): The dilation of the sliding window.
+            pad_value: The value to fill the padded area with.
+        
+        Example:
+            >>> layer = nn.Unfold(kernel_size=3, stride=1, padding=1)
+            >>> x = synapgrad.ones((2, 3, 4, 5))
+            >>> y = layer(x) # Shape = (2, 27, 20)
+        """
         super().__init__()
         
         kernel_size = np.broadcast_to(kernel_size, 2)
         dilation = np.broadcast_to(dilation, 2)
         padding = np.broadcast_to(padding, 2)
         stride = np.broadcast_to(stride, 2)
         
         self.kernel_size = kernel_size
         self.stride = stride
         self.padding = padding
         self.dilation = dilation
         self.pad_value = pad_value
         
     def forward(self, x: Tensor) -> Tensor:
-        N, C, H, W = x.shape
-        unfolded = unfold(x.data, kernel_size=self.kernel_size, stride=self.stride, dilation=self.dilation,
-                           padding=self.padding, pad_value=self.pad_value)
-        
-        out = Tensor(unfolded, (x,), "<Unfold>", requires_grad=x.requires_grad)
-        
-        def _backward():
-            if x.requires_grad:
-                grad = fold(out._grad, (H,W), kernel_size=self.kernel_size, stride=self.stride,
-                     dilation=self.dilation, padding=self.padding)
-
-                x._grad += grad
-                
-        out._backward = _backward
-    
-        return out
+        return F.unfold(x, kernel_size=self.kernel_size, stride=self.stride, padding=self.padding,
+                       dilation=self.dilation, pad_value=self.pad_value)
     
     
 class Fold(nn.Module):
-    """ Check nn.funcional.fold for more information """
     
     def __init__(self, output_size, kernel_size, stride=1, padding=0, dilation=1) -> None:
+        """ 
+        Folds a tensor. See nn.functional.fold for more information
+        
+        Args:
+            kernel_size (int or tuple): The size of the sliding window.
+            stride (int or tuple): The stride of the sliding window.
+            padding (int or tuple): The padding of the sliding window.
+            dilation (int or tuple): The dilation of the sliding window.
+            output_size (int or tuple): The size of the output.
+        
+        Example:
+            >>> layer = nn.Fold(output_size=(4,5), kernel_size=3, stride=1, padding=1)
+            >>> x = synapgrad.ones((2, 27, 20))
+            >>> y = layer(x) # Shape = (2, 3, 4, 5)
+        
+        """
         super().__init__()
         
         output_size = np.broadcast_to(output_size, 2)
         kernel_size = np.broadcast_to(kernel_size, 2)
         dilation = np.broadcast_to(dilation, 2)
         padding = np.broadcast_to(padding, 2)
         stride = np.broadcast_to(stride, 2)
@@ -93,120 +215,237 @@
         self.output_size = output_size
         self.kernel_size = kernel_size
         self.stride = stride
         self.padding = padding
         self.dilation = dilation
         
     def forward(self, x: Tensor) -> Tensor:
-        folded = fold(x.data, self.output_size, kernel_size=self.kernel_size, stride=self.stride, dilation=self.dilation,
-                           padding=self.padding)
-        
-        out = Tensor(folded, (x,), "<Fold>", requires_grad=x.requires_grad)
-        
-        def _backward():
-            if x.requires_grad:
-                grad = unfold(out._grad, kernel_size=self.kernel_size, stride=self.stride,
-                     dilation=self.dilation, padding=self.padding)
+        return F.fold(x, output_size=self.output_size, kernel_size=self.kernel_size, stride=self.stride,
+                      padding=self.padding, dilation=self.dilation)
 
-                x._grad += grad
-                
-        out._backward = _backward
-    
-        return out
+
+class MaxPool1d(nn.Module):
     
+    def __init__(self, kernel_size:int, stride:int=None, padding:int=0, dilation:int=1) -> None:
+        """
+        Applies Max Pooling 1D to a batch of N images with C channels (N, C, W).
+        
+        Reference:
+            - https://pytorch.org/docs/stable/generated/torch.nn.MaxPool1d.html
+
+        Args:
+            kernel_size (int): the size of the sliding blocks
+            stride (int, optional): the stride of the sliding blocks in the input 
+                spatial dimensions. If None, it is set to kernel_size. Default: None
+            padding (int, optional): implicit zero padding to be added on both 
+                sides of input. Default: 0
+            dilation (int, optional): controls the spacing between the kernel points. Default: 1
+
+        Output:
+            Tensor of shape (N, C, lW).
+        """
+        super().__init__()
+        
+        self.kernel_size = kernel_size
+        if stride is None: stride = kernel_size
+        self.stride = stride
+        self.padding = padding
+        self.dilation = dilation
+        
+    def forward(self, x: Tensor) -> Tensor: 
+        return F.max_pool1d(x, kernel_size=self.kernel_size, stride=self.stride, padding=self.padding,
+                                dilation=self.dilation)
+        
 
 class MaxPool2d(nn.Module):
     
     def __init__(self, kernel_size, stride=None, padding=0, dilation=1) -> None:
         """
         Applies Max Pooling 2D to a batch of N images with C channels (N, C, H, W).
         References:
             https://pytorch.org/docs/stable/generated/torch.nn.MaxPool2d.html
 
         Args:
             kernel_size (int or tuple): the size of the sliding blocks
-            stride (int or tuple, optional): the stride of the sliding blocks in the input spatial dimensions. Default: 1
-            padding (int or tuple, optional):  implicit zero padding to be added on both sides of input. Default: 0
-            dilation (int or tuple, optional): a parameter that controls the stride of elements within the neighborhood. Default: 1
+            stride (int or tuple, optional): the stride of the sliding blocks in the input 
+                spatial dimensions. Default: 1
+            padding (int or tuple, optional): implicit zero padding to be added on both 
+                sides of input. Default: 0
+            dilation (int or tuple, optional): controls the spacing between the kernel points. Default: 1
 
         Output:
-            Tensor of shape (N, C, H // stride[0], W // stride[1]).
+            Tensor of shape (N, C, lW, lH).
         """
         super().__init__()
         
         kernel_size = np.broadcast_to(kernel_size, 2)
-        if stride is None:
-            stride = kernel_size
-        else:
-            stride = np.broadcast_to(stride, 2)
+        if stride is None: stride = kernel_size
+        else: stride = np.broadcast_to(stride, 2)
         padding = np.broadcast_to(padding, 2)
         dilation = np.broadcast_to(dilation, 2)
         
         self.kernel_size = kernel_size
         self.stride = stride
         self.padding = padding
         self.dilation = dilation
         
     def forward(self, x: Tensor) -> Tensor: 
-        N, C, H, W = x.shape
-        lH = int(np.floor((H + 2 * self.padding[0] - self.dilation[0] * (self.kernel_size[0] - 1) - 1) / self.stride[0] + 1))
-        lW = int(np.floor((W + 2 * self.padding[1] - self.dilation[1] * (self.kernel_size[1] - 1) - 1) / self.stride[1] + 1))
-        
-        unfolded = unfold(x.data, kernel_size=self.kernel_size, stride=self.stride, dilation=self.dilation,
-                           padding=self.padding, pad_value=-np.inf)
+        return F.max_pool2d(x, kernel_size=self.kernel_size, stride=self.stride, padding=self.padding,
+                                dilation=self.dilation)
+
+
+class AvgPool1d(nn.Module):
+    
+    def __init__(self, kernel_size:int, stride:int=None, padding:int=0, dilation:int=1) -> None:
+        """ 
+        Applies Avg Pooling 1D to a batch of N images with C channels (N, C, W).
         
-        N, C_k, L = unfolded.shape
-        split_per_channel = unfolded.reshape(N, C, int(C_k/C), L)
+        Reference:
+            - https://pytorch.org/docs/stable/generated/torch.nn.AvgPool1d.html
+
+        Args:
+            kernel_size (int): the size of the sliding blocks
+            stride (int, optional): the stride of the sliding blocks in the input 
+                spatial dimensions. If None, it is set to kernel_size. Default: None
+            padding (int, optional): implicit zero padding to be added on both 
+                sides of input. Default: 0
+            dilation (int, optional): controls the spacing between the kernel points. Default: 1
+
+        Output:
+            Tensor of shape (N, C, lW).
+        """
+        super().__init__()
+        self.kernel_size = kernel_size
+        if stride is None: stride = kernel_size
+        self.stride = stride
+        self.padding = padding
+        self.dilation = dilation
         
-        unfolded_reorganized = np.moveaxis(split_per_channel, -2, -1).reshape(N, C, lH, lW, -1)
-        pooled, max_indices, selected = Tensor(unfolded_reorganized).max(dim=-1, return_selected=True)
+    def forward(self, x: Tensor) -> Tensor: 
+        return F.avg_pool1d(x, kernel_size=self.kernel_size, stride=self.stride, padding=self.padding,
+                                dilation=self.dilation)
+
     
-        out = Tensor(pooled.data, (x,), "<MaxPool2d>", requires_grad=x.requires_grad)
+class AvgPool2d(nn.Module):
+    
+    def __init__(self, kernel_size, stride=None, padding=0, dilation=1) -> None:
+        """ 
+        Applies Avg Pooling 2D to a batch of N images with C channels (N, C, H, W).
+        
+        Reference:
+            - https://pytorch.org/docs/stable/generated/torch.nn.AvgPool2d.html
+
+        Args:
+            kernel_size (int or tuple): the size of the sliding blocks
+            stride (int or tuple, optional): the stride of the sliding blocks in the input 
+                spatial dimensions. If None, it is set to kernel_size. Default: None
+            padding (int or tuple, optional): implicit zero padding to be added on both 
+                sides of input. Default: 0
+            dilation (int or tuple, optional): controls the spacing between the kernel points. Default: 1
+
+        Output:
+            Tensor of shape (N, C, lW, lH).
+        """
+        super().__init__()
+        
+        kernel_size = np.broadcast_to(kernel_size, 2)
+        if stride is None: stride = kernel_size
+        else: stride = np.broadcast_to(stride, 2)
+        padding = np.broadcast_to(padding, 2)
+        dilation = np.broadcast_to(dilation, 2)
+        
+        self.kernel_size = kernel_size
+        self.stride = stride
+        self.padding = padding
+        self.dilation = dilation
         
-        def _backward():
-            if x.requires_grad:
-                grad = selected * np.expand_dims(out._grad, axis=-1)
+    def forward(self, x: Tensor) -> Tensor: 
+        return F.avg_pool2d(x, kernel_size=self.kernel_size, stride=self.stride, padding=self.padding,
+                                dilation=self.dilation)
 
-                grad = grad.reshape(N, C, L, int(C_k/C))
-                grad = np.moveaxis(grad, -1, -2)
-                grad = grad.reshape(N, C_k, L)
-                
-                grad = fold(grad, (H,W), kernel_size=self.kernel_size, stride=self.stride,
-                     dilation=self.dilation, padding=self.padding)
 
-                x._grad += grad
-                
-        out._backward = _backward
+class Conv1d(nn.Module):
+    
+    def __init__(self, in_channels, out_channels, kernel_size, stride=1, padding=0, dilation=1, bias=True, weight_init_method='he_uniform') -> None:
+        """
+        Applies 1D Convolution to a batch of N images with C channels (N, C, W).
         
-        return out
+        Reference:
+            - https://pytorch.org/docs/stable/generated/torch.nn.Conv1d.html
+
+        Args:
+            in_channels (int): the number of input channels
+            out_channels (int): the number of output channels produced by the convolution
+            kernel_size (int): the size of the sliding blocks
+            stride (int, optional): the stride of the sliding blocks in the input 
+                spatial dimensions. Default: 1
+            padding (int, optional): implicit zero padding to be added on both sides
+                of input. Default: 0
+            dilation (int, optional): controls the spacing between the kernel points. Default: 1
+            bias: Whether to use a bias or not. Defaults to True.
+        
+        Output:
+            Tensor of shape (N, C_out, lW).
+        """
+        super().__init__()
+        
+        if padding == 'same':
+            if stride != 1:
+                raise ValueError("padding='same' is not supported for strided convolutions")
+            padding = int(np.floor(kernel_size / 2))
+        if padding == 'valid':
+            padding = 0
+        
+        self.in_channels = in_channels
+        self.out_channels = out_channels
+        self.kernel_size = kernel_size
+        self.stride = stride
+        self.stride = stride
+        self.padding = padding
+        self.dilation = dilation
+        
+        self.weight_init_method = weight_init_method
+        weight_values = init_weights((out_channels, in_channels, kernel_size), weight_init_method).astype(np.float32)
+        self.weight = nn.Parameter(weight_values, requires_grad=True, name='weight')
+        if bias: 
+            bias = synapgrad.zeros((out_channels,), dtype=np.float32, requires_grad=True, name='bias')
+            self.bias = nn.Parameter(bias)
+        else: self.bias = None
+    
+    def forward(self, x: Tensor) -> Tensor:
+        return F.conv1d(x, self.weight, self.bias, self.stride, self.padding, self.dilation)
 
 
 class Conv2d(nn.Module):
     
-    def __init__(self, in_channels, out_channels, kernel_size, stride=1, padding=0, dilation=1, weight_init_method='he_uniform') -> None:
+    def __init__(self, in_channels, out_channels, kernel_size, stride=1, padding=0, dilation=1, bias=True, weight_init_method='he_uniform') -> None:
         """
         Applies 2D Convolution to a batch of N images with C channels (N, C, H, W).
+        
         Reference:
-            https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html
+            - https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html
 
         Args:
             in_channels (int): the number of input channels
             out_channels (int): the number of output channels produced by the convolution
             kernel_size (int or tuple): the size of the sliding blocks
-            stride (int or tuple, optional): the stride of the sliding blocks in the input spatial dimensions. Default: 1
-            padding (int or tuple, optional):  implicit zero padding to be added on both sides of input. Default: 0
-            dilation (int or tuple, optional): a parameter that controls the stride of elements within the neighborhood. Default: 1
+            stride (int or tuple, optional): the stride of the sliding blocks in the input 
+                spatial dimensions. Default: 1
+            padding (int or tuple, optional): implicit zero padding to be added on both sides
+                of input. Default: 0
+            dilation (int or tuple, optional): controls the spacing between the kernel points. Default: 1
+            bias: Whether to use a bias or not. Defaults to True.
+        
+        Output:
+            Tensor of shape (N, C_out, lW, lH).
         """
         super().__init__()
         
         kernel_size = np.broadcast_to(kernel_size, 2)
-        if stride is None:
-            stride = kernel_size
-        else:
-            stride = np.broadcast_to(stride, 2)
+        stride = np.broadcast_to(stride, 2)
         
         if padding == 'same':
             if any(s != 1 for s in stride):
                 raise ValueError("padding='same' is not supported for strided convolutions")
             padding = int(np.floor(kernel_size[0] / 2))
         if padding == 'valid':
             padding = 0
@@ -219,167 +458,116 @@
         self.stride = stride
         self.stride = stride
         self.padding = padding
         self.dilation = dilation
         
         self.weight_init_method = weight_init_method
         weight_values = init_weights((out_channels, in_channels, *kernel_size), weight_init_method).astype(np.float32)
-        self.weight = Tensor(weight_values, requires_grad=True)
-        self.bias = Tensor.zeros((out_channels,), dtype=np.float32, requires_grad=True)
+        self.weight = nn.Parameter(weight_values, requires_grad=True, name='weight')
+        if bias:
+            bias = synapgrad.zeros((out_channels,), dtype=np.float32, requires_grad=True, name='bias') 
+            self.bias = nn.Parameter(bias)
+        else: self.bias = None
     
     def forward(self, x: Tensor) -> Tensor:
-        N, C, H, W = x.shape
-        lH = int(np.floor((H + 2 * self.padding[0] - self.dilation[0] * (self.kernel_size[0] - 1) - 1) / self.stride[0] + 1))
-        lW = int(np.floor((W + 2 * self.padding[1] - self.dilation[1] * (self.kernel_size[1] - 1) - 1) / self.stride[1] + 1))
-        
-        unfolded = Unfold(kernel_size=self.kernel_size, stride=self.stride, dilation=self.dilation,
-                           padding=self.padding, pad_value=0)(x)
-        
-        weight = self.weight.view(self.weight.shape[0], -1).transpose(0,1) 
-        mult = unfolded.transpose(1,2) @ weight
-        convolved = (mult) + self.bias
-        out = convolved.transpose(1,2).view(N, self.out_channels, lH, lW)
-                
-        return out
-        
-    def parameters(self) -> list['Tensor']:
-        return [self.weight, self.bias]
-    
-    def __repr__(self) -> str:
-        return (f"Conv2d(in_channels={self.in_channels}, out_channels={self.out_channels}, " + 
-                f"kernel_size={self.kernel_size}, stride={self.stride}, padding={self.padding}, " + 
-                f"dilation={self.dilation}")
-    
-
-class Dropout(nn.Module):
-    """ 
-    Reference:
-        https://pytorch.org/docs/stable/generated/torch.nn.Dropout.html
-    
-    """
-
-    def __init__(self, p=0.5, inplace=False) -> None:
-        super().__init__()
-        self.p = p
-        self.inplace = inplace
-        
-    def forward(self, x: Tensor) -> Tensor:
-        if not self.training: return x
-        random_data = np.random.rand(*x.shape)
-        random_data = np.where(random_data <= self.p, 0, 1)
-        if self.p < 1:
-            random_data = random_data / (1-self.p) # scale data
-        random_t = Tensor(random_data)
-        
-        return x*random_t
+        return F.conv2d(x, self.weight, self.bias, self.stride, self.padding, self.dilation)
     
     
 class BatchNorm(nn.Module):
     
-    def __init__(self, mode:str, num_features:int, eps:float=1e-5, momentum:float=0.1, affine:bool=True,
+    def __init__(self, num_features:int, eps:float=1e-5, momentum:float=0.1, affine:bool=True,
                  track_running_stats:bool=True, dtype=None) -> None:
         super().__init__()
         self.num_features = num_features
         self.eps = eps
         self.momentum = momentum
         self.affine = affine
         self.track_running_stats = track_running_stats
         self.num_batches_tracked = 0
-        
-        valid_modes = ['1d', '2d']
-        
-        if mode not in valid_modes:
-            raise ValueError(f"'{mode}' is not a valid mode, expected one of {valid_modes}")
-        self.mode = mode
-        
+
         if dtype is None:
             dtype = np.float32
         
         if self.track_running_stats:
-            self.running_mean = Tensor.zeros(num_features, dtype=dtype, name='running_mean')
-            self.running_var = Tensor.ones(num_features, dtype=dtype, name='running_var')
+            self.running_mean = synapgrad.zeros(num_features, dtype=dtype, name='running_mean')
+            self.running_var = synapgrad.ones(num_features, dtype=dtype, name='running_var')
         else:
             self.running_mean = None
             self.running_var = None
         
         if affine:
             # gamma
-            self.weight = Tensor.ones(num_features, requires_grad=True, dtype=dtype, name="gamma")
+            gamma = synapgrad.ones(num_features, requires_grad=True, dtype=dtype, name="gamma")
+            self.weight = nn.Parameter(gamma)
             # beta
-            self.bias = Tensor.zeros(num_features, requires_grad=True, dtype=dtype, name="beta")
+            beta = synapgrad.zeros(num_features, requires_grad=True, dtype=dtype, name="beta")
+            self.bias = nn.Parameter(beta)
+        else:
+            self.weight = None
+            self.bias = None
                 
     def forward(self, x: Tensor) -> Tensor:
-        if self.mode == '2d':
-            if len(x.shape) == 4:
-                N, C, H, W = x.shape
-                n = N*H*W # num_samples
-                dims = (0,2,3)
-                view_shape = (1,C,1,1)
-            else: raise RuntimeError(f"Expected 4D tensor, but got {len(x.shape)}D")
-        elif self.mode == '1d':
-            if len(x.shape) == 3:
-                N, C, L = x.shape
-                n = N*L # num_samples
-                dims = (0,2)
-                view_shape = (1,C,1)
-            elif len(x.shape) == 2:
-                N, C = x.shape
-                n = N # num_samples
-                dims = (0,)
-                view_shape = (1,C)
-            else: raise RuntimeError(f"Expected 2D or 3D tensor, but got {len(x.shape)}D")
-        assert C == self.num_features, f"Expected {self.num_features} channels, got {C}."
-        
-        exponential_average_factor = 0.0
+        if self.momentum is None:
+            exponential_average_factor = 0.0
+        else:
+            exponential_average_factor = self.momentum
 
         if self.training and self.track_running_stats:
             if self.num_batches_tracked is not None:
                 self.num_batches_tracked += 1
                 if self.momentum is None:  # use cumulative moving average
                     exponential_average_factor = 1.0 / float(self.num_batches_tracked)
                 else:  # use exponential moving average
                     exponential_average_factor = self.momentum
+                    
+        if self.training:
+            bn_training = True
+        else:
+            bn_training = (self.running_mean is None) and (self.running_var is None)
+        
+        running_mean = self.running_mean if not self.training or self.track_running_stats else None
+        running_var = self.running_var if not self.training or self.track_running_stats else None
+            
+        return F.batch_norm(x, self.weight, self.bias, running_mean, running_var,
+                                                bn_training, exponential_average_factor, self.eps)
 
         # calculate running estimates
         if self.training:
             mean = x.mean(dim=dims)
             # use biased var in train
             var_sum = ((x - mean.reshape(view_shape))**2).sum(dim=dims)
             var = var_sum / n
             
-            r_mu = (exponential_average_factor * mean.data + (1 - exponential_average_factor) * self.running_mean.data)
-            self.running_mean = Tensor(r_mu, dtype=x.dtype)
-            
-            unbiased_var = var_sum.data / (n - 1)
-            r_var = (exponential_average_factor * unbiased_var + (1 - exponential_average_factor) * self.running_var.data)
-            self.running_var = Tensor(r_var, dtype=x.dtype)
+            with synapgrad.no_grad():
+                r_mu = (exponential_average_factor * mean.data + (1 - exponential_average_factor) * self.running_mean.data)
+                self.running_mean = synapgrad.tensor(r_mu)
+                
+                unbiased_var = var_sum.data / (n - 1)
+                r_var = (exponential_average_factor * unbiased_var + (1 - exponential_average_factor) * self.running_var.data)
+                self.running_var = synapgrad.tensor(r_var)
         else:
             mean = self.running_mean
             var = self.running_var
 
         out = (x - mean.reshape(view_shape)) / (var.reshape(view_shape) + self.eps).sqrt()
         if self.affine:
             out = out * self.weight.reshape(view_shape) + self.bias.reshape(view_shape)
 
         return out
-        
-    def parameters(self) -> list[Tensor]:
-        return [self.weight, self.bias] if self.affine else []
 
 
 class BatchNorm1d(BatchNorm):
-    """
-    Reference:
-        https://pytorch.org/docs/stable/generated/torch.nn.BatchNorm1d.html
-    """
-    
+
     def __init__(self, num_features:int, eps:float=1e-5, momentum:float=0.1, affine:bool=True,
                  track_running_stats:bool=True, dtype=None) -> None:
         """
         Computes the batchnorm of a 2 or 3 dimensional tensor (N, C) or (N, C, L) 
+        
+        Reference:
+            - https://pytorch.org/docs/stable/generated/torch.nn.BatchNorm1d.html
 
         Arguments:
         num_features (int): C from an expected input size (N, C) or (N, C, L).
         eps (float): small constant to avoid division by zero in variance computation.
         momentum (float): the value used for the running_mean and running_var computation.
             Can be set to None for cumulative moving average (i.e. simple average).
             Default: 0.1.
@@ -388,28 +576,27 @@
         track_running_stats (bool): a boolean value that when set to True, this module 
             tracks the running mean and variance, and when set to False, this 
             module does not track such statistics, and initializes statistics buffers
             running_mean and running_var as None. When these buffers are None, this 
             module always uses batch statistics. in both training and eval modes. 
             Default: True
         """
-        super().__init__('1d', num_features, eps, momentum, affine, track_running_stats, dtype)
+        super().__init__(num_features, eps, momentum, affine, track_running_stats, dtype)
 
     
 class BatchNorm2d(BatchNorm):
-    """
-    Reference:
-        https://pytorch.org/docs/stable/generated/torch.nn.BatchNorm2d.html
-    """
-    
+
     def __init__(self, num_features:int, eps:float=1e-5, momentum:float=0.1, affine:bool=True,
                  track_running_stats:bool=True, dtype=None) -> None:
         """
         Computes the batchnorm of a 4-dimensional tensor (N, C, H, W) 
 
+        Reference:
+            - https://pytorch.org/docs/stable/generated/torch.nn.BatchNorm2d.html
+
         Arguments:
         num_features (int): C from an expected input size (N, C, H, W).
         eps (float): small constant to avoid division by zero in variance computation.
         momentum (float): the value used for the running_mean and running_var computation.
             Can be set to None for cumulative moving average (i.e. simple average).
             Default: 0.1.
         affine (bool): a boolean value that when set to True, this module has 
@@ -417,13 +604,8 @@
         track_running_stats (bool): a boolean value that when set to True, this module 
             tracks the running mean and variance, and when set to False, this 
             module does not track such statistics, and initializes statistics buffers
             running_mean and running_var as None. When these buffers are None, this 
             module always uses batch statistics. in both training and eval modes. 
             Default: True
         """
-        super().__init__('2d', num_features, eps, momentum, affine, track_running_stats, dtype)
-        
-        
-
-        
-    
+        super().__init__(num_features, eps, momentum, affine, track_running_stats, dtype)
```

## synapgrad/nn/losses.py

```diff
@@ -1,175 +1,125 @@
 from typing import Any
-from abc import ABC, abstractmethod
-from .. import Tensor
-from .functional import (
-    mse_loss, nll_loss, cross_entropy_loss, bce_loss, softmax_fn,
-    bce_with_logits_loss, relu_fn, epsilon
-)
-import numpy as np
 
+from synapgrad.nn import Module
+from synapgrad.tensor import Tensor
+from synapgrad.nn import functional as F
 
-# ----------------------------- Modules -----------------------------
-# -------------------------------------------------------------------
-class Loss(ABC):
+
+# ******************************
+# ******* Loss Modules *********
+# ******************************
+
+class Loss(Module):
+    """ 
+    Generic class for loss functions.
+    """
     
     def __init__(self, reduction='mean') -> None:
+        super().__init__()
         self.reduction = reduction
         
     def __call__(self, y_pred:Tensor, y_true:Tensor) -> Any:
-        assert isinstance(y_pred, Tensor) and isinstance(y_true, Tensor), "Inputs must be Tensors"
-
-        loss = self.criterion(y_pred, y_true)
-        
+        loss = super().__call__(y_pred, y_true)
+                
         # Reduction
         if self.reduction == 'sum':
             reduction = loss.sum()
         elif self.reduction == 'mean':
             reduction = loss.mean()
         else:
-            reduction = loss    
-          
-        if self.reduction is not None:
-            reduction._operation = loss._operation.replace(">", reduction._operation.replace("<", ""))
+            reduction = loss 
             
         return reduction
-    
-    @abstractmethod
-    def criterion(self, y_pred:Tensor, y_true:Tensor) -> Tensor:
-        pass
 
 
 class MSELoss(Loss):
-    """ Mean Squared Error Loss: (y_pred - y_true)**2 """
+    """ 
+    Mean Squared Error Loss: (y_pred - y_true) ** 2. It is mostly used for regression problems.
     
-    def criterion(self, y_pred:Tensor, y_true:Tensor) -> Tensor:
-        assert y_pred.matches_shape(y_true), f"Inputs shape don't match y_pred={y_pred.shape}, y_true={y_true.shape}"
-        req_grad = y_pred.requires_grad or y_true.requires_grad
-        mse = mse_loss(y_pred.data, y_true.data)
-        loss = Tensor(mse, (y_pred, y_true), '<MSELoss>', requires_grad=req_grad)
-        
-        def _backward():
-            if y_pred.requires_grad: 
-                grad = 2*(y_pred.data - y_true.data) 
-                y_pred._grad += grad * loss._grad
-        
-        loss._backward = _backward
-        
-        return loss
+    Inputs:
+    - y_pred: output (logits) from fully connected layer (num_examples x num_classes)
+    - y_true: labels (num_examples x num_classes)
+    """
+    
+    def forward(self, y_pred:Tensor, y_true:Tensor) -> Tensor:
+        return F.mse_loss(y_pred, y_true)
 
 
 class NLLLoss(Loss):
     """ 
-    This class expects y_true to be the probabilities of a LogSoftmax function. Also, y_pred 
-    should be shape=(batch, num_classes). It expects to receive the probability of a sample to be of each class.
-    For binary classification problems, output should not be a scalar value (0 <= x <=1) but an array with 
-    the probability of each class [0.3, 0.7]
+    Negative Log Likelihood Loss
+    
+    Inputs:
+    - y_pred: log of the class probabilities returned by LogSoftmax function. shape=(num_examples, num_classes).
+        For binary classification problems, it should not be a scalar value (0 <= x <=1) but an array with 
+        the probability of each class [-0.523, -0.155]
+    - y_true: labels. shape=(num_examples,). Note that y is not a one-hot encoded vector but an array with each value in 
+        the range [0, num_classes-1]
     
     Reference: 
-        https://towardsdatascience.com/cross-entropy-negative-log-likelihood-and-all-that-jazz-47a95bd2e81    
+    - https://towardsdatascience.com/cross-entropy-negative-log-likelihood-and-all-that-jazz-47a95bd2e81    
     """
     
-    def criterion(self, y_pred: Tensor, y_true: Tensor) -> Tensor:
-        req_grad = y_pred.requires_grad or y_true.requires_grad
-        log_likelihood = nll_loss(y_pred.data, y_true.data)
-        loss = Tensor(log_likelihood, (y_pred, y_true), '<NLLLoss>', requires_grad=req_grad)
-        
-        def _backward():
-            # Hand made derivation
-            if y_pred.requires_grad:
-                grad = np.zeros(y_pred.shape)
-                grad[range(len(y_pred.data)), y_true.data] = -1.0
-                # for i, true in enumerate(y_true.data):
-                #     grad[i][true] = -1.0
-                y_pred._grad += (grad * loss._grad)
-        
-        loss._backward = _backward
-        
-        return loss
+    def forward(self, y_pred: Tensor, y_true: Tensor) -> Tensor:
+        return F.nll_loss(y_pred, y_true)
 
    
 class BCELoss(Loss):
+    """
+    Binary Cross Entropy loss function.
+
+    Inputs:
+    - y_pred: probabilities returned by Sigmoid function. Values in range [0, 1], shape=(num_examples,)
+    - y_true: binary labels. 0 or 1, shape=(num_examples,)
     
-    def criterion(self, y_pred: Tensor, y_true: Tensor) -> Tensor:
-        req_grad = y_pred.requires_grad or y_true.requires_grad
-        bce = bce_loss(y_pred.data, y_true.data)
-        loss = Tensor(bce, (y_pred, y_true), '<BCELoss>', requires_grad=req_grad)
-        
-        def _backward():
-            # Hand made derivation
-            if y_pred.requires_grad:
-                term_0 = -(1 - y_true.data + epsilon) / ((1 - y_pred.data) + epsilon)
-                term_1 = (y_true.data + epsilon) / (y_pred.data + epsilon)
-                y_pred._grad += -(term_0 + term_1) * loss._grad
-        
-        loss._backward = _backward
-        
-        return loss
+    References:
+    - https://pytorch.org/docs/stable/generated/torch.nn.BCELoss.html
+    """
+    
+    def forward(self, y_pred: Tensor, y_true: Tensor) -> Tensor:
+        return F.binary_cross_entropy(y_pred, y_true)
 
 
 class BCEWithLogitsLoss(Loss):
     """ 
+    Binary Cross Entropy with Logits loss function.
+    
     This loss combines a Sigmoid layer and the BCELoss in one single class.
     This version is more numerically stable than using a plain Sigmoid followed by a BCELoss as,
     by combining the operations into one layer, we take advantage of the log-sum-exp
     trick for numerical stability
     
+    Inputs:
+    - y_pred: output (logits) from fully connected layer. shape=(num_examples,)
+    - y_true: binary labels. 0 or 1, shape=(num_examples,)
+    
     References:
-        https://pytorch.org/docs/stable/generated/torch.nn.BCEWithLogitsLoss.html
-        https://stackoverflow.com/questions/66906884/how-is-pytorchs-class-bcewithlogitsloss-exactly-implemented
+    - https://pytorch.org/docs/stable/generated/torch.nn.BCEWithLogitsLoss.html
+    - https://stackoverflow.com/questions/66906884/how-is-pytorchs-class-bcewithlogitsloss-exactly-implemented
     """
     
-    def criterion(self, y_pred: Tensor, y_true: Tensor) -> Tensor:
-        req_grad = y_pred.requires_grad or y_true.requires_grad
-        bce = bce_with_logits_loss(y_pred.data, y_true.data)
-        loss = Tensor(bce, (y_pred, y_true), '<BCEWithLogitsLoss>', requires_grad=req_grad)
-        
-        def _backward():
-            # Hand made derivation
-            if y_pred.requires_grad:
-                tn = -relu_fn(y_pred.data)
-                dtn = np.where(tn == 0, 0, -1)
-                div1 = -dtn*np.exp(-tn) + (-1-dtn)*np.exp((-y_pred.data-tn))
-                div2 = np.exp(-tn) + np.exp((-y_pred.data-tn))
-                grad = (1 - y_true.data) + dtn + (div1/(div2 + epsilon))
-                
-                y_pred._grad += grad * loss._grad
-        
-        loss._backward = _backward
-        
-        return loss
+    def forward(self, y_pred: Tensor, y_true: Tensor) -> Tensor:
+        return F.binary_cross_entropy_with_logits(y_pred, y_true)
     
     
 class CrossEntropyLoss(Loss):
     """ 
-    Same as:
-    
-    log_softmax = LogSoftmax(dim=1)(y_pred)
+    Cross Entropy Loss function.
     
-    loss = NLLLoss(reduction=None)(log_softmax, y_true)
+    Same as:
+    - log_probs = LogSoftmax(dim=1)(y_pred)
+    - loss = NLLLoss(reduction=None)(log_probs, y_true)
     
-    Reference: https://deepnotes.io/softmax-crossentropy#:~:text=Cross%20entropy%20indicates%20the%20distance,used%20alternative%20of%20squared%20error
+    Inputs:
+    - y_pred: output (logits) from fully connected layer. shape=(num_examples, num_classes)
+    - y_true: labels. shape=(num_examples,). Note that y is not a one-hot encoded vector but an array with each value in 
+        the range [0, num_classes-1]
+    
+    References: 
+    - https://pytorch.org/docs/stable/generated/torch.nn.CrossEntropyLoss.html
+    - https://deepnotes.io/softmax-crossentropy#:~:text=Cross%20entropy%20indicates%20the%20distance,used%20alternative%20of%20squared%20error
     """
     
-    def criterion(self, y_pred: Tensor, y_true: Tensor) -> Tensor:
-        """
-        y_pred is the output (logits) from fully connected layer (num_examples x num_classes)
-        y_true is labels (num_examples x 1)
-            Note that y is not one-hot encoded vector. 
-            It can be computed as y.argmax(axis=1) from one-hot encoded vectors of labels if required.
-        """
-        req_grad = y_pred.requires_grad or y_true.requires_grad
-        cross_entropy = cross_entropy_loss(y_pred.data, y_true.data)
-        loss = Tensor(cross_entropy, (y_pred, y_true), '<CrossEntropyLoss>', requires_grad=req_grad)
-        
-        def _backward():
-            # Hand made derivation
-            if y_pred.requires_grad:
-                dlogits = softmax_fn(y_pred.data, 1)
-                n = y_pred.shape[0]
-                dlogits[range(n), y_true.data] -= 1
-                y_pred._grad += (dlogits * loss._grad)
-        
-        loss._backward = _backward
-        
-        return loss
+    def forward(self, y_pred: Tensor, y_true: Tensor) -> Tensor:
+        return F.cross_entropy(y_pred, y_true)
```

## synapgrad/nn/modules.py

```diff
@@ -1,84 +1,146 @@
-from abc import ABC, abstractmethod
-from .. import Tensor
-    
+from typing import Any
+from collections import OrderedDict
+from synapgrad.tensor import Tensor
+from synapgrad.device import Device
+
+
+class Parameter(Tensor):
+    """
+    Wrapper class for Tensor that allows it to be used as a module parameter.
+    """ 
+    def __repr__(self) -> str:
+        return f"Parameter containing:\n{super().__repr__()}"
 
-class Module(ABC):
+
+class Module:
     
     def __init__(self) -> None:
-        self.modules = []
+        self._submodules = OrderedDict()
+        self._parameters = OrderedDict()
+        self._initialized = True
         self.training = True
         
     def train(self):
-        """ Set module to train mode"""
+        """ Set module and submodules to train mode"""
         self.training = True
-        for m in self.modules:
+        for m in self.submodules():
             m.train()
+        return self
         
     def eval(self):
-        """ Set module to evaluation mode """
+        """ Set module and submodules to evaluation mode """
         self.training = False
-        for m in self.modules:
+        for m in self.submodules():
             m.eval()
+        return self
         
-    def __call__(self, batch:Tensor) -> Tensor:
-        assert isinstance(batch, Tensor), "Input must be a Tensor" 
-        if len(batch.shape) <= 1:
-            raise ValueError(f"Module '{self.__class__.__name__}' expects a batched input, Shape=(batch_size, *), but received {batch.shape}")
-
-        return self.forward(batch)
+    def __call__(self, *inputs:Tensor, **kwargs) -> Tensor:
+        return self.forward(*inputs, **kwargs)
 
     def zero_grad(self):
         for p in self.parameters():
             if p.requires_grad: p.zero_()
     
     def freeze(self):
-        for p  in self.parameters():
+        for p in self.parameters():
             p.requires_grad = False
     
     def unfreeze(self):
         for p in self.parameters():
             p.requires_grad = True
-            
-    def track_module(self, m:'Module'):
-        self.modules.append(m)
-        
-    def track_modules(self, modules:list['Module']):
-        self.modules += modules
-
-    def parameters(self) -> list['Tensor']:
-        return [p for m in self.modules for p in m.parameters()]
+    
+    def check_is_initialized(self):
+        if not hasattr(self, '_initialized') or not self._initialized:
+            raise RuntimeError("Module is not initialized. Call super().__init__() first")
+        
+    def register_module(self, name:str, module:'Module'):
+        self.check_is_initialized()
+    
+        if not isinstance(module, Module):
+            raise TypeError("All submodules must be of type Module")
+        
+        self._submodules[name] = module
+        object.__setattr__(self, name, module)
+        
+    def register_parameter(self, name:str, parameter:Parameter):
+        self.check_is_initialized()
+        
+        if not isinstance(parameter, Parameter):
+            raise TypeError("All parameters must be of type Parameter")
+        
+        self._parameters[name] = parameter
+        object.__setattr__(self, name, parameter)
+    
+    def __setattr__(self, __name: str, __value: Any) -> None:
+        """
+        Keeps track of the submodules and parameters added to this module 
+        """
+        if isinstance(__value, Module):
+            self.register_module(__name, __value)
+        elif isinstance(__value, Parameter):
+            self.register_parameter(__name, __value)
+        else:  
+            object.__setattr__(self, __name, __value)
+    
+    def parameters(self) -> list['Parameter']:
+        """
+        Returns a list of all parameters in the module
+        """
+        params = list(self._parameters.values())
+        for m in self.submodules():
+            params += m.parameters()
+        return params
+    
+    def submodules(self) -> list['Module']:
+        return [m for m in self._submodules.values()]
     
     def num_params(self, trainable=False, non_trainable=False) -> int:
         num_params = 0; num_trainable = 0; num_non_trainable = 0
         for p in self.parameters():
             num_params += p.size
             if p.requires_grad: num_trainable += p.size
             else: num_non_trainable += p.size
         
         if trainable: return num_trainable
         elif non_trainable: return num_non_trainable
         return num_params
     
-    @abstractmethod
-    def forward(self, x:Tensor) -> Tensor:
-        pass
+    def forward(self, *args, **kwargs) -> Tensor:
+        raise NotImplementedError("All subclasses of Module must implement forward method")
+    
+    def cpu(self):
+        """
+        Move all parameters and submodules to CPU
+        """
+        for p in self.parameters():
+            if p.device != Device.CPU:
+                p.cpu()
+        for module in self.submodules():
+            if p.device != Device.CPU:
+                module.cpu()
+        return self
     
     def __repr__(self) -> str:
-        return (f"{self.__class__.__name__}(tracked_modules={len(self.modules)}, " +
+        return (f"{self.__class__.__name__}(submodules={len(self.submodules())}, " +
                 f"parameters={self.num_params()}, trainable={self.num_params(trainable=True)}, " +
                 f"non_trainable={self.num_params(non_trainable=True)})")
         
         
 class Sequential(Module):
     
     def __init__(self, *modules) -> None:
         super().__init__()
-        self.track_modules(modules)
+        if len(modules) == 1 and isinstance(modules[0], OrderedDict):
+            for key, module in modules[0].items():
+                self.register_module(key, module)
+        else:
+            for idx, module in enumerate(modules):
+                self.register_module(str(idx), module)
         
-    def forward(self, x: Tensor) -> Tensor:
+    def forward(self, x:Tensor) -> Tensor:
         inp = x
-        for module in self.modules:
+        for module in self.submodules():
             out = module(inp)
             inp = out
         return out
```

## synapgrad/optim/__init__.py

```diff
@@ -1,2 +1,2 @@
 
-from .optimizers import Optimizer, SGD, Adam
+from synapgrad.optim.optimizers import Optimizer, SGD, Adam
```

## synapgrad/optim/optimizers.py

```diff
@@ -1,12 +1,12 @@
-
 from abc import ABC, abstractmethod
 
-from .. import engine, Tensor
 import numpy as np
+import synapgrad
+from synapgrad.tensor import Tensor
 
 
 class Optimizer(ABC):
     
     def __init__(self, parameters:list[Tensor], lr=0.001) -> None:
         super().__init__()
         if len(parameters) == 0:
@@ -21,23 +21,22 @@
         
     @abstractmethod
     def step(self):
         self.t += 1
 
 
 class SGD(Optimizer):
-    """
-    Reference: 
-        https://pytorch.org/docs/stable/generated/torch.optim.SGD.html
-    """
     
     def __init__(self, parameters: list[Tensor], lr=0.001, momentum=0, dampening=0,
                  weight_decay=0, nesterov=False, maximize=False) -> None:
         """
         Implements stochastic gradient descent (optionally with momentum).
+        
+        Reference: 
+            - https://pytorch.org/docs/stable/generated/torch.optim.SGD.html
 
         Args:
             params (iterable): Iterable of parameters to optimize.
             lr (float): Learning rate.
             momentum (float, optional): Momentum factor (default: 0).
             dampening (float, optional): Dampening for momentum (default: 0).
             weight_decay (float, optional): Weight decay factor (default: 0).
@@ -54,15 +53,15 @@
         self.weight_decay = weight_decay
         
         if nesterov and (momentum <= 0 or dampening != 0):
             raise ValueError("Nesterov momentum requires a momentum and zero dampening")
     
     def step(self):
         super().step()
-        with engine.no_grad():
+        with synapgrad.no_grad():
             for i, p in enumerate(self.parameters):
                 grad = p._grad
                 
                 # Weight decay
                 if self.weight_decay != 0:
                     grad = grad + self.weight_decay*p.data
                 
@@ -83,24 +82,23 @@
                 if self.maximize:
                     p.data += self.lr*grad
                 else:
                     p.data -= self.lr*grad
         
     
 class Adam(Optimizer):
-    """
-    Reference: 
-        https://pytorch.org/docs/stable/generated/torch.optim.Adam.html
-    """
-    
+
     def __init__(self, parameters: list[Tensor], lr=0.001, betas=(0.9, 0.999), eps=1e-8,
                     weight_decay=0, maximize=False) -> None:
         """
         Implements Adam algorithm.
         
+        Reference: 
+            - https://pytorch.org/docs/stable/generated/torch.optim.Adam.html
+        
         Args:
             params (iterable): Iterable of model parameters to optimize.
             lr (float, optional): Learning rate. Default is 0.001.
             betas (tuple, optional): Coefficients used for computing running averages of gradient and its square.
                                     Default is (0.9, 0.999).
             eps (float, optional): Term added to the denominator to improve numerical stability. Default is 1e-08.
             weight_decay (float, optional): Weight decay (L2 penalty) factor. Default is 0.
@@ -115,15 +113,15 @@
         self.maximize = maximize
         
         self.m1 = [0 for _ in range(len(parameters))]
         self.m2 = [0 for _ in range(len(parameters))]
     
     def step(self):
         super().step()
-        with engine.no_grad():
+        with synapgrad.no_grad():
             for i, p in enumerate(self.parameters):
                 grad = -p._grad if self.maximize else p._grad   
                     
                 # Weight decay
                 if self.weight_decay != 0:
                     grad = grad + self.weight_decay*p.data
```

## Comparing `synapgrad-0.3.2.dist-info/LICENSE` & `synapgrad-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

