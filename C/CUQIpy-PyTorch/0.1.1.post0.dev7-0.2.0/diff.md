# Comparing `tmp/CUQIpy-PyTorch-0.1.1.post0.dev7.tar.gz` & `tmp/CUQIpy-PyTorch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CUQIpy-PyTorch-0.1.1.post0.dev7.tar", last modified: Mon Oct 31 21:48:19 2022, max compression
+gzip compressed data, was "CUQIpy-PyTorch-0.2.0.tar", last modified: Sat May 27 08:14:38 2023, max compression
```

## Comparing `CUQIpy-PyTorch-0.1.1.post0.dev7.tar` & `CUQIpy-PyTorch-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 21:48:19.865733 CUQIpy-PyTorch-0.1.1.post0.dev7/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 21:48:19.865733 CUQIpy-PyTorch-0.1.1.post0.dev7/CUQIpy_PyTorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15688 2022-10-31 21:48:19.000000 CUQIpy-PyTorch-0.1.1.post0.dev7/CUQIpy_PyTorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-10-31 21:48:19.000000 CUQIpy-PyTorch-0.1.1.post0.dev7/CUQIpy_PyTorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 21:48:19.000000 CUQIpy-PyTorch-0.1.1.post0.dev7/CUQIpy_PyTorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-31 21:48:19.000000 CUQIpy-PyTorch-0.1.1.post0.dev7/CUQIpy_PyTorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-31 21:48:19.000000 CUQIpy-PyTorch-0.1.1.post0.dev7/CUQIpy_PyTorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-10-31 21:48:10.000000 CUQIpy-PyTorch-0.1.1.post0.dev7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15688 2022-10-31 21:48:19.865733 CUQIpy-PyTorch-0.1.1.post0.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2259 2022-10-31 21:48:10.000000 CUQIpy-PyTorch-0.1.1.post0.dev7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 21:48:19.865733 CUQIpy-PyTorch-0.1.1.post0.dev7/cuqipy_pytorch/
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-10-31 21:48:10.000000 CUQIpy-PyTorch-0.1.1.post0.dev7/cuqipy_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-10-31 21:48:19.865733 CUQIpy-PyTorch-0.1.1.post0.dev7/cuqipy_pytorch/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    13044 2022-10-31 21:48:10.000000 CUQIpy-PyTorch-0.1.1.post0.dev7/cuqipy_pytorch/distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-10-31 21:48:10.000000 CUQIpy-PyTorch-0.1.1.post0.dev7/cuqipy_pytorch/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-10-31 21:48:10.000000 CUQIpy-PyTorch-0.1.1.post0.dev7/cuqipy_pytorch/sampler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-10-31 21:48:10.000000 CUQIpy-PyTorch-0.1.1.post0.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-31 21:48:19.865733 CUQIpy-PyTorch-0.1.1.post0.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-31 21:48:10.000000 CUQIpy-PyTorch-0.1.1.post0.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:14:38.659351 CUQIpy-PyTorch-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:14:38.655351 CUQIpy-PyTorch-0.2.0/CUQIpy_PyTorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15677 2023-05-27 08:14:38.000000 CUQIpy-PyTorch-0.2.0/CUQIpy_PyTorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-27 08:14:38.000000 CUQIpy-PyTorch-0.2.0/CUQIpy_PyTorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 08:14:38.000000 CUQIpy-PyTorch-0.2.0/CUQIpy_PyTorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 08:14:38.000000 CUQIpy-PyTorch-0.2.0/CUQIpy_PyTorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-27 08:14:38.000000 CUQIpy-PyTorch-0.2.0/CUQIpy_PyTorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-27 08:14:26.000000 CUQIpy-PyTorch-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15677 2023-05-27 08:14:38.655351 CUQIpy-PyTorch-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-27 08:14:26.000000 CUQIpy-PyTorch-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:14:38.659351 CUQIpy-PyTorch-0.2.0/cuqipy_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-27 08:14:26.000000 CUQIpy-PyTorch-0.2.0/cuqipy_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-27 08:14:38.659351 CUQIpy-PyTorch-0.2.0/cuqipy_pytorch/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17177 2023-05-27 08:14:26.000000 CUQIpy-PyTorch-0.2.0/cuqipy_pytorch/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-27 08:14:26.000000 CUQIpy-PyTorch-0.2.0/cuqipy_pytorch/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-27 08:14:26.000000 CUQIpy-PyTorch-0.2.0/cuqipy_pytorch/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-27 08:14:26.000000 CUQIpy-PyTorch-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 08:14:26.000000 CUQIpy-PyTorch-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 08:14:38.659351 CUQIpy-PyTorch-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-27 08:14:26.000000 CUQIpy-PyTorch-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:14:38.655351 CUQIpy-PyTorch-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-27 08:14:26.000000 CUQIpy-PyTorch-0.2.0/tests/test_eight_schools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-27 08:14:26.000000 CUQIpy-PyTorch-0.2.0/tests/test_model.py
```

### Comparing `CUQIpy-PyTorch-0.1.1.post0.dev7/CUQIpy_PyTorch.egg-info/PKG-INFO` & `CUQIpy-PyTorch-0.2.0/CUQIpy_PyTorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy-PyTorch
-Version: 0.1.1.post0.dev7
+Version: 0.2.0
 Summary: CUQIpy plugin for PyTorch
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `CUQIpy-PyTorch-0.1.1.post0.dev7/LICENSE` & `CUQIpy-PyTorch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CUQIpy-PyTorch-0.1.1.post0.dev7/PKG-INFO` & `CUQIpy-PyTorch-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy-PyTorch
-Version: 0.1.1.post0.dev7
+Version: 0.2.0
 Summary: CUQIpy plugin for PyTorch
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `CUQIpy-PyTorch-0.1.1.post0.dev7/README.md` & `CUQIpy-PyTorch-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `CUQIpy-PyTorch-0.1.1.post0.dev7/cuqipy_pytorch/distribution.py` & `CUQIpy-PyTorch-0.2.0/cuqipy_pytorch/distribution.py`

 * *Files 12% similar despite different names*

```diff
@@ -391,7 +391,148 @@
             return v1.grad
         else:                       #Likelihood case
             v2.requires_grad = True
             v2.grad = None
             Q = self(v2).logpdf(v1) # Forward pass
             Q.backward()            # Backward pass
             return v2.grad
+
+class Laplace(Distribution):
+    """Laplace distribution constructed via torch.distributions.Laplace.
+
+    Creates a Laplace distribution with location `loc` and scale `scale`. The pdf is given by
+
+    .. math::
+
+        f(x) = \\frac{1}{2 \\sigma} \\exp \\left( - \\frac{|x - \\mu|}{\\sigma} \\right)
+
+    where :math:`\\mu` is the location and :math:`\\sigma` is the scale.
+    
+    Parameters
+    ----------
+    loc : float, ndarray or torch.tensor
+        Location parameter
+        
+    scale : float, ndarray or torch.tensor  
+    
+    """
+
+    def __init__(self, location, scale, is_symmetric=True, **kwargs):
+        super().__init__(is_symmetric=is_symmetric, **kwargs) 
+        self.location = location
+        self.scale = scale
+
+    @property
+    def location(self):
+        return self._location
+
+    @location.setter
+    def location(self, value):
+        self._location = value
+        self._set_dist()
+    
+    @property
+    def scale(self):
+        return self._scale
+
+    @scale.setter
+    def scale(self, value):
+        self._scale = value
+        self._set_dist()
+
+    def _set_dist(self):
+        """ Set the pytorch distribution if both values are specified """
+        if hasattr(self, '_location') and hasattr(self, '_scale'):
+
+            # Define location value
+            loc = self.location
+            if isinstance(loc, numbers.Number):
+                loc = loc*torch.ones(self.dim)
+            if isinstance(loc, np.ndarray):
+                loc = torch.tensor(loc)
+
+            # Define scale value
+            scale = self._scale
+            if isinstance(scale, numbers.Number):
+                scale = scale*torch.ones(self.dim)
+            if isinstance(scale, np.ndarray):
+                scale = torch.tensor(scale)
+
+            # If both are tensors we create dist
+            if torch.is_tensor(loc) and torch.is_tensor(scale):
+                self._dist = torch.distributions.Laplace(loc, scale)
+
+    def logpdf(self, value):
+        return torch.sum(self._dist.log_prob(value))
+
+    def _sample(self, n):
+        return self._dist.sample(torch.Size((n,)))
+
+class Cauchy(Distribution):
+    """Cauchy distribution constructed via torch.distributions.Cauchy.
+
+    Creates a Cauchy distribution with location `loc` and scale `scale`. The pdf is given by
+
+    .. math::
+
+        f(x) = \\frac{1}{\\pi \\sigma (1 + ((x - \\mu)/\\sigma)^2)}
+
+    where :math:`\\mu` is the location and :math:`\\sigma` is the scale.
+
+    Parameters
+    ----------
+    loc : float, ndarray or torch.tensor
+
+    scale : float, ndarray or torch.tensor
+
+    """
+
+    def __init__(self, location, scale, is_symmetric=True, **kwargs):
+        super().__init__(is_symmetric=is_symmetric, **kwargs) 
+        self.location = location
+        self.scale = scale
+
+    @property
+    def location(self):
+        return self._location
+
+    @location.setter
+    def location(self, value):
+        self._location = value
+        self._set_dist()
+    
+    @property
+    def scale(self):
+        return self._scale
+
+    @scale.setter
+    def scale(self, value):
+        self._scale = value
+        self._set_dist()
+
+    def _set_dist(self):
+        """ Set the pytorch distribution if both values are specified """
+        if hasattr(self, '_location') and hasattr(self, '_scale'):
+
+            # Define location value
+            loc = self.location
+            if isinstance(loc, numbers.Number):
+                loc = loc*torch.ones(self.dim)
+            if isinstance(loc, np.ndarray):
+                loc = torch.tensor(loc)
+
+            # Define scale value
+            scale = self._scale
+            if isinstance(scale, numbers.Number):
+                scale = scale*torch.ones(self.dim)
+            if isinstance(scale, np.ndarray):
+                scale = torch.tensor(scale)
+
+            # If both are tensors we create dist
+            if torch.is_tensor(loc) and torch.is_tensor(scale):
+                self._dist = torch.distributions.Cauchy(loc, scale)
+
+    def logpdf(self, value):
+        return torch.sum(self._dist.log_prob(value))
+
+    def _sample(self, n):
+        return self._dist.sample(torch.Size((n,)))
```

### Comparing `CUQIpy-PyTorch-0.1.1.post0.dev7/cuqipy_pytorch/model.py` & `CUQIpy-PyTorch-0.2.0/cuqipy_pytorch/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,13 +22,16 @@
         def backward(ctx, grad_output):
             input, = ctx.saved_tensors
             numpy_grad_output = grad_output.detach().numpy()
             numpy_input = input.detach().numpy()
             grad_input = model.gradient(numpy_grad_output, numpy_input)
             return input.new(grad_input)
 
-    torch_forward = CustomFunction.apply
+    torch_forward = lambda *args: CustomFunction.apply(*args)
 
     # Add to cuqi model
     torch_model = Model(torch_forward, int(model.range_dim), int(model.domain_dim))
 
+    # Set parameter name
+    torch_model._non_default_args = model._non_default_args
+
     return torch_model
```

### Comparing `CUQIpy-PyTorch-0.1.1.post0.dev7/cuqipy_pytorch/sampler.py` & `CUQIpy-PyTorch-0.2.0/cuqipy_pytorch/sampler.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-PyTorch-0.1.1.post0.dev7/pyproject.toml` & `CUQIpy-PyTorch-0.2.0/pyproject.toml`

 * *Files identical despite different names*

