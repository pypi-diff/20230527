# Comparing `tmp/torchbones-1.0.5.tar.gz` & `tmp/torchbones-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.0.5.tar", last modified: Fri May 26 20:19:54 2023, max compression
+gzip compressed data, was "torchbones-1.0.7.tar", last modified: Fri May 26 20:48:20 2023, max compression
```

## Comparing `torchbones-1.0.5.tar` & `torchbones-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-26 20:19:53.994946 torchbones-1.0.5/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-26 20:19:53.994946 torchbones-1.0.5/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-05-26 20:19:53.994946 torchbones-1.0.5/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      441 2023-05-26 20:19:03.000000 torchbones-1.0.5/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-26 20:19:53.994946 torchbones-1.0.5/torchbones/
--rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.0.5/torchbones/__init__.py
--rw-r--r--   0 oross314  (1000) oross314  (1000)    15442 2023-05-26 20:18:52.000000 torchbones-1.0.5/torchbones/main.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-26 20:19:53.994946 torchbones-1.0.5/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-26 20:19:53.000000 torchbones-1.0.5/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-05-26 20:19:53.000000 torchbones-1.0.5/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-05-26 20:19:53.000000 torchbones-1.0.5/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       30 2023-05-26 20:19:53.000000 torchbones-1.0.5/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-05-26 20:19:53.000000 torchbones-1.0.5/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-26 20:48:20.266615 torchbones-1.0.7/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-26 20:48:20.255781 torchbones-1.0.7/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-05-26 20:48:20.266615 torchbones-1.0.7/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      441 2023-05-26 20:48:09.000000 torchbones-1.0.7/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-26 20:48:20.255781 torchbones-1.0.7/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.0.7/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    15240 2023-05-26 20:47:48.000000 torchbones-1.0.7/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-26 20:48:20.255781 torchbones-1.0.7/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-26 20:48:20.000000 torchbones-1.0.7/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-05-26 20:48:20.000000 torchbones-1.0.7/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-05-26 20:48:20.000000 torchbones-1.0.7/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       30 2023-05-26 20:48:20.000000 torchbones-1.0.7/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-05-26 20:48:20.000000 torchbones-1.0.7/torchbones.egg-info/top_level.txt
```

### Comparing `torchbones-1.0.5/torchbones/main.py` & `torchbones-1.0.7/torchbones/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,15 +314,15 @@
             self.oldlr = 1*self.lr
             self.countcheck = 0 
             
 
 
 
             
-    def plot(self, med = True, log = True):
+    def plot(self, med = True):
         ###make log an input
         testtruth = self.data[5]
         output = self.testout
         if len(self.testerr) > 1:
             fig, ax = plt.subplots(1,3, figsize = (15,4))
             xs = np.arange(len(self.trainerr))
             ax[2].plot(xs, self.trainerr, label = 'train error')
@@ -330,21 +330,15 @@
             ax[2].set_xlabel('epoch')
             ax[2].set_ylabel('mean abs err')
             ax[2].legend()
             ax[2].set_yscale('log')
         else: fig, ax = plt.subplots(1, 2, figsize = (15, 4))
             
         x, y = self.data[4], np.squeeze(np.squeeze(self.testout.detach().numpy()))
-        
-        if not log:
-            bins = 30
-        else:
-            bins = np.logspace(np.log10(min(x)), np.log10(max(x)), 30)
-            ax[0].loglog()
-            ax[1].loglog()
+        bins = 30
         ax[0].hist2d(x, y, bins = bins)
 
         ax[0].set_xlabel('test truth')
         ax[0].set_ylabel('test predication') 
 
         yt, xt = torch.squeeze(torch.squeeze(self.output)).detach().numpy(), self.truetrain
         ax[1].hist2d(xt, yt, bins = bins)
@@ -368,8 +362,8 @@
             traincov = cov[:split]
             testcov = cov[split:]
         else:
             traincov, testcov = 1, 1
         return train, traintruth, traincov, test, testtruth, testcov
 
             
-                            
+
```

