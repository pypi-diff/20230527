# Comparing `tmp/scatterd-1.3.1.tar.gz` & `tmp/scatterd-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatterd-1.3.1.tar", last modified: Sun Apr 23 09:54:36 2023, max compression
+gzip compressed data, was "scatterd-1.3.2.tar", last modified: Sat May 27 12:42:29 2023, max compression
```

## Comparing `scatterd-1.3.1.tar` & `scatterd-1.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 09:54:36.160917 scatterd-1.3.1/
--rw-rw-rw-   0        0        0     1121 2021-11-13 12:45:24.000000 scatterd-1.3.1/LICENSE
--rw-rw-rw-   0        0        0      115 2021-11-13 12:45:24.000000 scatterd-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4994 2023-04-23 09:54:36.161914 scatterd-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4451 2022-12-19 19:17:15.000000 scatterd-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 09:54:36.153303 scatterd-1.3.1/scatterd/
--rw-rw-rw-   0        0        0     1833 2023-04-22 20:09:57.000000 scatterd-1.3.1/scatterd/__init__.py
--rw-rw-rw-   0        0        0     6870 2023-04-22 20:10:09.000000 scatterd-1.3.1/scatterd/examples.py
--rw-rw-rw-   0        0        0    20903 2023-04-22 23:31:27.000000 scatterd-1.3.1/scatterd/scatterd.py
-drwxrwxrwx   0        0        0        0 2023-04-23 09:54:36.160917 scatterd-1.3.1/scatterd.egg-info/
--rw-rw-rw-   0        0        0     4994 2023-04-23 09:54:35.000000 scatterd-1.3.1/scatterd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-23 09:54:36.000000 scatterd-1.3.1/scatterd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 09:54:35.000000 scatterd-1.3.1/scatterd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-23 09:54:35.000000 scatterd-1.3.1/scatterd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-23 09:54:35.000000 scatterd-1.3.1/scatterd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      259 2023-04-23 09:54:36.163306 scatterd-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1419 2023-04-21 11:44:02.000000 scatterd-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 12:42:29.570647 scatterd-1.3.2/
+-rw-rw-rw-   0        0        0     1121 2021-11-13 12:45:24.000000 scatterd-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0      115 2021-11-13 12:45:24.000000 scatterd-1.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4994 2023-05-27 12:42:29.571648 scatterd-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4451 2022-12-19 19:17:15.000000 scatterd-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 12:42:29.553455 scatterd-1.3.2/scatterd/
+-rw-rw-rw-   0        0        0     1817 2023-05-27 12:40:09.000000 scatterd-1.3.2/scatterd/__init__.py
+-rw-rw-rw-   0        0        0     7267 2023-05-27 12:38:44.000000 scatterd-1.3.2/scatterd/examples.py
+-rw-rw-rw-   0        0        0    21943 2023-05-27 12:27:07.000000 scatterd-1.3.2/scatterd/scatterd.py
+drwxrwxrwx   0        0        0        0 2023-05-27 12:42:29.569649 scatterd-1.3.2/scatterd.egg-info/
+-rw-rw-rw-   0        0        0     4994 2023-05-27 12:42:29.000000 scatterd-1.3.2/scatterd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-27 12:42:29.000000 scatterd-1.3.2/scatterd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 12:42:29.000000 scatterd-1.3.2/scatterd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-27 12:42:29.000000 scatterd-1.3.2/scatterd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-27 12:42:29.000000 scatterd-1.3.2/scatterd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      259 2023-05-27 12:42:29.584609 scatterd-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1419 2023-04-21 11:44:02.000000 scatterd-1.3.2/setup.py
```

### Comparing `scatterd-1.3.1/LICENSE` & `scatterd-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scatterd-1.3.1/PKG-INFO` & `scatterd-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scatterd
-Version: 1.3.1
+Version: 1.3.2
 Summary: scatterd is an easy and fast way of creating scatter plots.
 Home-page: https://erdogant.github.io/scatterd
-Download-URL: https://github.com/erdogant/scatterd/archive/1.3.1.tar.gz
+Download-URL: https://github.com/erdogant/scatterd/archive/1.3.2.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: scatterd Version: 1.3.1 Summary: scatterd is an
+Metadata-Version: 2.1 Name: scatterd Version: 1.3.2 Summary: scatterd is an
 easy and fast way of creating scatter plots. Home-page: https://
 erdogant.github.io/scatterd Download-URL: https://github.com/erdogant/scatterd/
-archive/1.3.1.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
+archive/1.3.2.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE # scatterd [![Python](https://img.shields.io/pypi/pyversions/scatterd)]
 (https://img.shields.io/pypi/pyversions/scatterd) [![Pypi](https://
 img.shields.io/pypi/v/scatterd)](https://pypi.org/project/scatterd/) [![Docs]
 (https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
```

### Comparing `scatterd-1.3.1/README.md` & `scatterd-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `scatterd-1.3.1/scatterd/__init__.py` & `scatterd-1.3.2/scatterd/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from scatterd.scatterd import scatterd,import_example, set_colors, _preprocessing, gradient_on_density_color
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.3.1'
+__version__ = '1.3.2'
 
 # module level doc-string
 __doc__ = """
 scatterd
 =====================================================================
 
-Description
------------
-Scatterd is an easy and fast way of creating scatter plots.
+Scatterd is an easy and fast way of creating beautiful scatter plots.
 
 Examples
 --------
 >>> # Import library
 >>> from scatterd import scatterd, import_example
 >>>
 >>> # Import example
```

### Comparing `scatterd-1.3.1/scatterd/examples.py` & `scatterd-1.3.2/scatterd/examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,43 @@
 from scatterd import scatterd, import_example
 import numpy as np
 
-# %%
+df = import_example()
+fig, ax = scatterd(df['tsneX'],
+                   df['tsneY'],
+                   labels=df['labx'],
+                   )
 
+# %%
+from scatterd import scatterd, import_example
 df = import_example()
 fig, ax = scatterd(df['tsneX'],
                    df['tsneY'],
                    labels=df['labx'],
                    density=True,
-                   density_on_top=True,
-                   args_density={'alpha': 0.3},
-                   gradient='#FFFFFF',
-                   edgecolor='#FFFFFF',
+                   density_on_top=False,
+                    # args_density={'alpha': 0.3},
+                    gradient='opaque',
+                    # gradient='#FFFFFF',
+                   edgecolor='#000000',
                    grid=True,
                    fontweight='normal',
                    fontsize=26,
                    legend=2,
                    )
 
+# %%
+# X, y = make_friedman1(n_samples=100000, n_features=5, random_state=0)
+# fig, ax = scatterd(X[:,0], X[:,1], density=False, s=0)
+
+
+# %%
+
+
+
 
 # %%
 # Import example iris dataet
 from sklearn import datasets
 iris = datasets.load_iris()
 X = iris.data[:, :2]
 labels = iris.target
```

### Comparing `scatterd-1.3.1/scatterd/scatterd.py` & `scatterd-1.3.2/scatterd/scatterd.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,29 +18,29 @@
 from urllib.parse import urlparse
 
 # %% Main
 def scatterd(x,
              y,
              z=None,
              s=150,
-             c=[0,0.1,0.4],
+             c=[0, 0.1, 0.4],
              labels=None,
              marker='o',
              alpha=0.8,
              edgecolor='#000000',
-             gradient=None,
-             density=False,
+             gradient='opaque',
+             density=True,
              density_on_top=False,
              norm=False,
              cmap='tab20c',
              figsize=(25, 15),
              dpi=100,
              legend=None,
              jitter=None,
-             xlabel='x-axis', ylabel='y-axis', title='', fontsize=24, fontcolor=None, grid=False, fontweight='normal',
+             xlabel='x-axis', ylabel='y-axis', title='', fontsize=24, fontcolor=None, grid=True, fontweight='normal',
              args_density = {'cmap': 'Reds', 'fill': True, 'thresh': 0.05, 'bw_adjust': .6, 'alpha': 0.66, 'legend': False, 'cbar': False},
              visible=True,
              fig=None,
              ax=None,
              verbose=3):
     """Make scaterplot.
 
@@ -66,17 +66,19 @@
     alpha : float, default: 0.8
         The alpha blending value, between 0 (transparent) and 1 (opaque).
     edgecolors : (default: 'face')
         The edge color of the marker. Possible values:
             * 'face': The edge color will always be the same as the face color.
             * 'none': No patch boundary will be drawn.
             * '#FFFFFF' : A color or sequence of colors.
-    gradient : String, (default: None)
-        Hex color to make a lineair gradient for the scatterplot.
-        '#FFFFFF'
+    gradient : String, (default: 'opaque')
+        Hex color to make a lineair gradient using the density.
+            * None: Do not use gradient.
+            * opaque: Towards the edges the points become more opaque and thus not visible.
+            * '#FFFFFF': Towards the edges it smooths into this color
     density : Bool (default: False)
         Include the kernel density in the scatter plot.
     density_on_top : bool, (default: False)
         True : The density is the highest layer.
         False : The density is the lowest layer.
     xlabel : String, optional
         Xlabel. The default is None.
@@ -184,34 +186,36 @@
     # Defaults
     defaults_density = {'cmap': 'Reds', 'thresh': 0.05, 'bw_adjust': .6, 'alpha': 0.66, 'legend': False, 'cbar': False, 'fill': True}
     args_density = {**defaults_density, **args_density}
 
     # Preprocessing
     X, labels = _preprocessing(x, y, z, labels, jitter, norm)
     # Set color
-    c_rgb = set_colors(X, labels, c, cmap, gradient=gradient, verbose=verbose)
+    c_rgb, opaque = set_colors(X, labels, c, cmap, gradient=gradient, verbose=verbose)
     # Set fontcolor
     fontcolor = set_fontcolor(fontcolor, labels, X, cmap, verbose=2)
     # Set size
     s = set_size(X, s)
     # Set size
-    alpha = set_alpha(X, alpha)
+    alpha = set_alpha(X, alpha, gradient, opaque, verbose)
     # Set marker
     marker = set_marker(X, marker)
     # Bootup figure
     fig, ax = init_figure(ax, z, dpi, figsize, visible, fig)
     # Set figure properties
-    ax = _set_figure_properties(X, labels, fontcolor, fontsize, xlabel, ylabel, title, grid, fontweight, ax)
+    ax = _set_figure_properties(X, labels, fontcolor, fontsize, xlabel, ylabel, title, grid, fontweight, zorder, ax)
 
     # Add density as bottom layer to the scatterplot
     if density:
         ax = sns.kdeplot(x=X[:, 0], y=X[:, 1], ax=ax, **args_density)
 
     # Scatter all at once
     if (labels is None) and isinstance(marker, str):
+        # Do not try to plot legend.
+        legend = -1
         if z is None:
             ax.scatter(X[:, 0], X[:, 1], c=c_rgb, s=s, edgecolor=edgecolor, marker=marker, alpha=alpha, zorder=zorder)
         else:
             ax.scatter(X[:, 0], X[:, 1], X[:, 2], s=s, c=c_rgb, edgecolor=edgecolor, marker=marker, alpha=alpha, zorder=zorder)
     else:
         uilabels = np.unique(labels)
         for label in uilabels:
@@ -231,30 +235,31 @@
     if legend>=0: ax.legend(loc=legend, fontsize=14)
 
     # Return
     return fig, ax
 
 
 # %% Setup figure properties
-def _set_figure_properties(X, labels, fontcolor, fontsize, xlabel, ylabel, title, grid, fontweight, ax):
+def _set_figure_properties(X, labels, fontcolor, fontsize, xlabel, ylabel, title, grid, fontweight, zorder, ax):
     # Set axis fontsizes
     if grid is None: grid=False
     if grid is True: grid='#dddddd'
+    None if zorder is None else zorder + 1
     font = {'family': 'DejaVu Sans', 'weight': fontweight, 'size': fontsize}
     matplotlib.rc('font', **font)
     for item in ([ax.title, ax.xaxis.label, ax.yaxis.label] + ax.get_xticklabels() + ax.get_yticklabels()):
         item.set_fontsize(20)
 
     # Plot labels
     if (labels is not None) and (fontcolor is not None):
         for uilabel in fontcolor.keys():
             # Compute median for better center compared to mean
             XYmean = np.mean(X[labels==uilabel, :], axis=0)
             if X.shape[1]==2:
-                ax.text(XYmean[0], XYmean[1], str(uilabel), color=fontcolor.get(uilabel), fontdict={'weight': fontweight, 'size': fontsize}, zorder=15)
+                ax.text(XYmean[0], XYmean[1], str(uilabel), color=fontcolor.get(uilabel), fontdict={'weight': fontweight, 'size': fontsize}, zorder=zorder)
             else:
                 ax.text(XYmean[0], XYmean[1], XYmean[2], str(uilabel), color=fontcolor.get(uilabel), fontdict={'weight': fontweight, 'size': fontsize})
 
     # Labels on axis
     ax.set_xlabel(xlabel)
     ax.set_ylabel(ylabel)
     if title is not None: ax.set_title(title)
@@ -276,14 +281,16 @@
 # %% Setup colors
 def set_colors(X, labels, c, cmap='tab20c', gradient=None, verbose=3):
     """Set colors."""
     if c is None: return None
 
     # The default is all dots to black
     c_rgb = np.repeat([0, 0, 0], X.shape[0], axis=0).reshape(-1, 3)
+    # Create opaque levels
+    opaque = np.array([0.0] * X.shape[0])
 
     # Change on input c
     if len(c)==1 and isinstance(c, list): c = c[0]
     if len(c)==3 and isinstance(c[0], (int, float)):
         if verbose>=4: print('[scatterd] >Colors are all set to %s.' %(c))
         c_rgb = np.repeat([c], X.shape[0], axis=0).reshape(-1, 3)
 
@@ -291,59 +298,67 @@
         if verbose>=4: print('[scatterd] >Colors are set to input colors defined in [c].')
         c_rgb=c
 
     if labels is not None:
         # Create unqiue colors for labels if there are multiple classes or in case cmap and gradient is used.
         if verbose>=4: print('[scatterd] >Colors are based on the input [labels] and on [cmap].')
         if labels is None: labels = np.repeat(0, X.shape[0])
-        c_rgb, _ = colourmap.fromlist(labels, cmap=cmap, method='matplotlib', gradient=gradient)
+        c_rgb = colourmap.fromlist(labels, X=X, cmap=cmap, method='matplotlib', gradient=gradient)[0]
 
     # Add gradient for each class
-    if (gradient is not None):
-        if verbose>=4: print('[scatterd] >Color [gradient] is included.')
-        c_rgb = gradient_on_density_color(X, c_rgb, labels)
+    # if (gradient is not None):
+    #     if verbose>=4: print('[scatterd] >Color [gradient] is included.')
+    #     c_rgb = gradient_on_density_color(X, c_rgb, labels)
+
+    if gradient=='opaque' and c_rgb.shape[1]==4:
+        opaque = c_rgb[:, -1]
+        c_rgb = c_rgb[:, :3]
 
     # Return
-    return c_rgb
+    return c_rgb, opaque
 
 
 # %% Create gradient based on density.
-def gradient_on_density_color(X, c_rgb, labels):
-    """Set gradient on density color."""
-    if labels is None: labels = np.repeat(0, X.shape[0])
-    from scipy.stats import gaussian_kde
-    uilabels = np.unique(labels)
-    density_colors= np.repeat([1., 1., 1.], len(labels), axis=0).reshape(-1, 3)
+# def gradient_on_density_color(X, c_rgb, labels, showfig=False):
+#     """Set gradient on density color."""
+#     if labels is None: labels = np.repeat(0, X.shape[0])
+#     from scipy.stats import gaussian_kde
+#     uilabels = np.unique(labels)
+#     # density_colors = np.repeat([1., 1., 1.], len(labels), axis=0).reshape(-1, 3)
+#     density_colors = np.ones_like(c_rgb)
+
+#     if (len(uilabels)!=len(labels)):
+#         for label in uilabels:
+#             idx = np.where(labels==label)[0]
+#             if X.shape[1]==2:
+#                 xy = np.vstack([X[idx, 0], X[idx, 1]])
+#             else:
+#                 xy = np.vstack([X[idx, 0], X[idx, 1], X[idx, 2]])
+
+#             try:
+#                 # Compute density
+#                 z = gaussian_kde(xy)(xy)
+#                 # Sort on density
+#                 didx = idx[np.argsort(z)[::-1]]
+#             except:
+#                 didx=idx
+
+#             # order colors correctly based Density
+#             density_colors[didx] = c_rgb[idx, :]
+
+#             if showfig:
+#                 plt.figure()
+#                 fig, ax = plt.subplots(1,2, figsize=(20,10))
+#                 ax[0].scatter(X[didx,0], X[didx,1], color=c_rgb[idx, 0:3], alpha=c_rgb[idx, 3], edgecolor='#000000')
+#                 ax[1].scatter(idx, idx, color=c_rgb[idx, 0:3], alpha=c_rgb[idx, 3], edgecolor='#000000')
 
-    if (len(uilabels)!=len(labels)):
-        for label in uilabels:
-            idx = np.where(labels==label)[0]
-            if X.shape[1]==2:
-                xy = np.vstack([X[idx, 0], X[idx, 1]])
-            else:
-                xy = np.vstack([X[idx, 0], X[idx, 1], X[idx, 2]])
+#         c_rgb=density_colors
 
-            try:
-                # Compute density
-                z = gaussian_kde(xy)(xy)
-                # Sort on density
-                didx = idx[np.argsort(z)[::-1]]
-            except:
-                didx=idx
-
-            # order colors correctly based Density
-            density_colors[didx] = c_rgb[idx, :]
-            # plt.figure()
-            # plt.scatter(X[didx,0], X[didx,1], color=c_rgb[idx, :])
-            # plt.figure()
-            # plt.scatter(idx, idx, color=c_rgb[idx, :])
-        c_rgb=density_colors
-
-    # Return
-    return c_rgb
+#     # Return
+#     return c_rgb
 
 
 # %% Fontcolor
 def _preprocessing(x, y, z, labels, jitter, norm=False):
     if jitter is None or jitter is False: jitter=0
     if jitter is True: jitter=0.01
     if jitter>0:
@@ -408,18 +423,22 @@
     """Set size."""
     if isinstance(s, (int, float)): s = np.repeat(s, X.shape[0])
     # Minimum size should be 0 (dots will not be showed)
     s = np.maximum(s, 0)
     return s
 
 
-def set_alpha(X, alpha):
+def set_alpha(X, alpha, gradient, opaque, verbose):
     """Set alpha."""
     if alpha is None: alpha=0.8
-    if isinstance(alpha, (int, float)): alpha = np.repeat(alpha, X.shape[0])
+    if isinstance(alpha, (int, float)):
+        alpha = np.repeat(alpha, X.shape[0])
+    if gradient=='opaque':
+        if verbose>=3: print('[scatterd]> Set alpha based on density because of the parameter: [%s]' %(gradient))
+        alpha = opaque
     # Minimum size should be 0 (dots will not be showed)
     alpha = np.maximum(alpha, 0)
     return alpha
 
 
 def set_marker(X, marker):
     """Set markers."""
```

### Comparing `scatterd-1.3.1/scatterd.egg-info/PKG-INFO` & `scatterd-1.3.2/scatterd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scatterd
-Version: 1.3.1
+Version: 1.3.2
 Summary: scatterd is an easy and fast way of creating scatter plots.
 Home-page: https://erdogant.github.io/scatterd
-Download-URL: https://github.com/erdogant/scatterd/archive/1.3.1.tar.gz
+Download-URL: https://github.com/erdogant/scatterd/archive/1.3.2.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: scatterd Version: 1.3.1 Summary: scatterd is an
+Metadata-Version: 2.1 Name: scatterd Version: 1.3.2 Summary: scatterd is an
 easy and fast way of creating scatter plots. Home-page: https://
 erdogant.github.io/scatterd Download-URL: https://github.com/erdogant/scatterd/
-archive/1.3.1.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
+archive/1.3.2.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE # scatterd [![Python](https://img.shields.io/pypi/pyversions/scatterd)]
 (https://img.shields.io/pypi/pyversions/scatterd) [![Pypi](https://
 img.shields.io/pypi/v/scatterd)](https://pypi.org/project/scatterd/) [![Docs]
 (https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
```

### Comparing `scatterd-1.3.1/setup.py` & `scatterd-1.3.2/setup.py`

 * *Files identical despite different names*

