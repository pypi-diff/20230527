# Comparing `tmp/ExPSO-0.0.24.tar.gz` & `tmp/ExPSO-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExPSO-0.0.24.tar", last modified: Wed May 24 10:16:36 2023, max compression
+gzip compressed data, was "ExPSO-0.0.25.tar", last modified: Sat May 27 07:24:29 2023, max compression
```

## Comparing `ExPSO-0.0.24.tar` & `ExPSO-0.0.25.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 10:16:36.210047 ExPSO-0.0.24/
--rw-rw-rw-   0        0        0    35560 2023-05-07 11:50:19.000000 ExPSO-0.0.24/LICENSE
--rw-rw-rw-   0        0        0    20528 2023-05-24 10:16:36.208048 ExPSO-0.0.24/PKG-INFO
--rw-rw-rw-   0        0        0    19664 2023-05-24 10:13:04.000000 ExPSO-0.0.24/README.md
--rw-rw-rw-   0        0        0     1042 2023-05-24 10:13:42.000000 ExPSO-0.0.24/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 10:16:36.210047 ExPSO-0.0.24/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-24 10:16:36.157010 ExPSO-0.0.24/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 10:16:36.170019 ExPSO-0.0.24/src/ExPSO/
--rw-rw-rw-   0        0        0    10375 2023-05-22 10:42:29.000000 ExPSO-0.0.24/src/ExPSO/ExPSOClass.py
--rw-rw-rw-   0        0        0      124 2023-05-07 10:18:51.000000 ExPSO-0.0.24/src/ExPSO/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 10:16:36.183028 ExPSO-0.0.24/src/ExPSO.egg-info/
--rw-rw-rw-   0        0        0    20528 2023-05-24 10:16:36.000000 ExPSO-0.0.24/src/ExPSO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-05-24 10:16:36.000000 ExPSO-0.0.24/src/ExPSO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 10:16:36.000000 ExPSO-0.0.24/src/ExPSO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-24 10:16:36.000000 ExPSO-0.0.24/src/ExPSO.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 07:24:29.164837 ExPSO-0.0.25/
+-rw-rw-rw-   0        0        0    35560 2023-05-07 11:50:19.000000 ExPSO-0.0.25/LICENSE
+-rw-rw-rw-   0        0        0      862 2023-05-27 07:24:29.164837 ExPSO-0.0.25/PKG-INFO
+-rw-rw-rw-   0        0        0     1042 2023-05-27 07:20:41.000000 ExPSO-0.0.25/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 07:24:29.165859 ExPSO-0.0.25/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 07:24:29.097881 ExPSO-0.0.25/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 07:24:29.157833 ExPSO-0.0.25/src/ExPSO/
+-rw-rw-rw-   0        0        0     9942 2023-05-27 07:08:41.000000 ExPSO-0.0.25/src/ExPSO/ExPSOClass.py
+-rw-rw-rw-   0        0        0      124 2023-05-07 10:18:51.000000 ExPSO-0.0.25/src/ExPSO/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 07:24:29.163837 ExPSO-0.0.25/src/ExPSO.egg-info/
+-rw-rw-rw-   0        0        0      862 2023-05-27 07:24:28.000000 ExPSO-0.0.25/src/ExPSO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-05-27 07:24:28.000000 ExPSO-0.0.25/src/ExPSO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 07:24:28.000000 ExPSO-0.0.25/src/ExPSO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-27 07:24:28.000000 ExPSO-0.0.25/src/ExPSO.egg-info/top_level.txt
```

### Comparing `ExPSO-0.0.24/LICENSE` & `ExPSO-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `ExPSO-0.0.24/pyproject.toml` & `ExPSO-0.0.25/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   "scikit-learn"
 ]
 
 
 
 [project]
 name = "ExPSO"
-version = "0.0.24"
+version = "0.0.25"
 authors = [
   { name="Insaf Kraidia", email="insaf.kraidia@univ-constantine2.dz" },
   { name="Khelil Kassoul", email="khelil.kassoul@etu.unige.ch" },
   { name="Samir Brahim Belhaouari", email="sbelhaouari@hbku.edu.qa" },
   { name="Naoufel Cheikhrouhou",email="naoufel.cheikhrouhou@hesge.ch"},
   { name="Nicolas Zufferey",email="nicolas.zufferey.1@ulaval.ca"}
```

### Comparing `ExPSO-0.0.24/src/ExPSO/ExPSOClass.py` & `ExPSO-0.0.25/src/ExPSO/ExPSOClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,18 +35,16 @@
         # This line initializes the Position attribute of the instance with a 1 x D zero matrix.
         self.Position = np.zeros((1, D))
         # This line initializes the Cost attribute of the instance with a float 0.0 value.
         self.Cost = 0.0
 
 
 class ExponentialParticleSwarmOptimizer:
-    def __init__(self, ObjFunction, opt, thrshold, D, nPop=50, MaxIt=5000, lb=-100, ub=100, runs=10):
+    def __init__(self, ObjFunction, D, nPop=50, MaxIt=5000, lb=-100, ub=100, runs=10):
         self.ObjFunction = ObjFunction
-        self.opt = opt
-        self.thrshold = thrshold
         self.D = D
         self.nPop = nPop
         self.MaxIt = MaxIt
         self.lb = lb
         self.ub = ub
         self.runs = runs
         self.MeanIter = [[] for _ in range(runs)]
@@ -68,30 +66,24 @@
         self.Worst.Cost = float('-inf')
 
     def optimize(self):
         for k in range(self.runs):
             # Constriction Coefficients
             N1 = 10
             N2 = 10
-            phi1 = 2.05
-            phi2 = 2.05
-            phi = phi1 + phi2
-            m = 0.5
-            xhi = 2 * m / (phi - 2 + (phi ** 2 - 4 * phi) ** 0.5)
             c1 = -1
             c2 = 2
             w = 0.9                      # Inertia Weight
             r = 0.9                      # Coefficient Damping Ratio 1
             a = 2                        # Personal Learning Coefficient
             b = 2                        # Global Learning Coefficient
             c = 2
             d = -1
             e = -1
             alpha = 1e-5
-
             VelMax = self.ub
             VelMin = -VelMax
 
             for i in range(self.nPop):
                 # Initialize Position
                 self.particle[i].Position = self.lb + \
                     (self.ub - self.lb) * np.random.rand(1, self.D)
@@ -119,17 +111,16 @@
                 # Update Global Worst
                 if self.particle[i].Cost > self.Worst.Cost:
                     self.Worst = self.particle[i].Minimum
             import array
             #BestCost = np.zeros(MaxIt)
             BestCost = []
             #BestCost = array.array('i', [0], start=1)
-            gap = 1
             it = 0
-            while it < self.MaxIt and abs(gap) >= self.thrshold:
+            while it < self.MaxIt:
 
                 it += 1
 
                 for i in range(self.nPop):
                     if i <= N1:
                         self.particle[i].Velocity = w * self.particle[i].Velocity \
                             + a * np.exp(1 / (np.linalg.norm(self.particle[i].Best.Position - self.particle[i].Position)) + alpha) * np.random.rand(1, self.D) \
@@ -205,17 +196,15 @@
                     VelMin = -self.ub
                     w = r * ((1 - w) / (1 + w))
 
                 # appends the current global best cost to the BestCost list.
                 BestCost.append(self.GlobalBest.Cost)
                 # appends the current global best cost to the MeanIter list for the current iteration k
                 self.MeanIter[k].append(self.GlobalBest.Cost)
-                # calculates the gap between the current global best cost and the optimal
                 # cost for the current function number func_num.
-                gap = BestCost[-1] - self.opt
 
             self.RunBestCost.append(BestCost[-1])
             #print("run=", k, " Best Cost =", self.RunBestCost[-1])
 
             self.FES.append(it * self.nPop)
 
             for it in range(it, self.MaxIt):
```

