# Comparing `tmp/df2onehot-1.0.3.tar.gz` & `tmp/df2onehot-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "df2onehot-1.0.3.tar", last modified: Mon Apr 17 21:34:03 2023, max compression
+gzip compressed data, was "df2onehot-1.0.4.tar", last modified: Sat May 27 17:29:55 2023, max compression
```

## Comparing `df2onehot-1.0.3.tar` & `df2onehot-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 21:34:03.460909 df2onehot-1.0.3/
--rw-rw-rw-   0        0        0     1122 2021-02-09 21:19:52.000000 df2onehot-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       25 2023-04-17 21:33:01.000000 df2onehot-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3188 2023-04-17 21:34:03.458043 df2onehot-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2616 2022-03-13 15:33:54.000000 df2onehot-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 21:34:03.375160 df2onehot-1.0.3/df2onehot/
--rw-rw-rw-   0        0        0      692 2023-04-17 21:29:35.000000 df2onehot-1.0.3/df2onehot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:34:03.432181 df2onehot-1.0.3/df2onehot/data/
--rw-rw-rw-   0        0        0        0 2021-04-25 14:06:00.000000 df2onehot-1.0.3/df2onehot/data/__init__.py
--rw-rw-rw-   0        0        0    21315 2023-04-17 21:24:53.000000 df2onehot-1.0.3/df2onehot/df2onehot.py
--rw-rw-rw-   0        0        0      968 2023-04-17 19:45:54.000000 df2onehot-1.0.3/df2onehot/examples.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:34:03.453915 df2onehot-1.0.3/df2onehot/tests/
--rw-rw-rw-   0        0        0        0 2021-04-25 14:06:00.000000 df2onehot-1.0.3/df2onehot/tests/__init__.py
--rw-rw-rw-   0        0        0     3813 2022-03-13 13:41:37.000000 df2onehot-1.0.3/df2onehot/tests/test_df2onehot.py
--rw-rw-rw-   0        0        0    10215 2021-02-09 21:19:52.000000 df2onehot-1.0.3/df2onehot/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:34:03.429718 df2onehot-1.0.3/df2onehot.egg-info/
--rw-rw-rw-   0        0        0     3188 2023-04-17 21:34:02.000000 df2onehot-1.0.3/df2onehot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-04-17 21:34:03.000000 df2onehot-1.0.3/df2onehot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 21:34:02.000000 df2onehot-1.0.3/df2onehot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-04-17 21:34:02.000000 df2onehot-1.0.3/df2onehot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-17 21:34:03.000000 df2onehot-1.0.3/df2onehot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 21:34:03.460909 df2onehot-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1420 2022-12-02 15:05:15.000000 df2onehot-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 17:29:55.043703 df2onehot-1.0.4/
+-rw-rw-rw-   0        0        0     1122 2021-02-09 21:19:52.000000 df2onehot-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-04-17 21:33:01.000000 df2onehot-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3188 2023-05-27 17:29:55.043703 df2onehot-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2616 2022-03-13 15:33:54.000000 df2onehot-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 17:29:55.034597 df2onehot-1.0.4/df2onehot/
+-rw-rw-rw-   0        0        0      600 2023-05-27 17:29:46.000000 df2onehot-1.0.4/df2onehot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 17:29:55.040567 df2onehot-1.0.4/df2onehot/data/
+-rw-rw-rw-   0        0        0        0 2021-04-25 14:06:00.000000 df2onehot-1.0.4/df2onehot/data/__init__.py
+-rw-rw-rw-   0        0        0    20842 2023-05-27 17:28:29.000000 df2onehot-1.0.4/df2onehot/df2onehot.py
+-rw-rw-rw-   0        0        0     1053 2023-05-27 17:28:37.000000 df2onehot-1.0.4/df2onehot/examples.py
+drwxrwxrwx   0        0        0        0 2023-05-27 17:29:55.042603 df2onehot-1.0.4/df2onehot/tests/
+-rw-rw-rw-   0        0        0        0 2021-04-25 14:06:00.000000 df2onehot-1.0.4/df2onehot/tests/__init__.py
+-rw-rw-rw-   0        0        0     3813 2022-03-13 13:41:37.000000 df2onehot-1.0.4/df2onehot/tests/test_df2onehot.py
+-rw-rw-rw-   0        0        0    10215 2021-02-09 21:19:52.000000 df2onehot-1.0.4/df2onehot/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-27 17:29:55.040567 df2onehot-1.0.4/df2onehot.egg-info/
+-rw-rw-rw-   0        0        0     3188 2023-05-27 17:29:54.000000 df2onehot-1.0.4/df2onehot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-05-27 17:29:54.000000 df2onehot-1.0.4/df2onehot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 17:29:54.000000 df2onehot-1.0.4/df2onehot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-05-27 17:29:54.000000 df2onehot-1.0.4/df2onehot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-27 17:29:54.000000 df2onehot-1.0.4/df2onehot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 17:29:55.043703 df2onehot-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1424 2023-05-27 16:56:41.000000 df2onehot-1.0.4/setup.py
```

### Comparing `df2onehot-1.0.3/LICENSE` & `df2onehot-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `df2onehot-1.0.3/PKG-INFO` & `df2onehot-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: df2onehot
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python package df2onehot is to convert a pandas dataframe into a stuctured dataframe.
 Home-page: https://erdogant.github.io/df2onehot
-Download-URL: https://github.com/erdogant/df2onehot/archive/1.0.3.tar.gz
+Download-URL: https://github.com/erdogant/df2onehot/archive/1.0.4.tar.gz
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
-Metadata-Version: 2.1 Name: df2onehot Version: 1.0.3 Summary: Python package
+Metadata-Version: 2.1 Name: df2onehot Version: 1.0.4 Summary: Python package
 df2onehot is to convert a pandas dataframe into a stuctured dataframe. Home-
 page: https://erdogant.github.io/df2onehot Download-URL: https://github.com/
-erdogant/df2onehot/archive/1.0.3.tar.gz Author: Erdogan Taskesen Author-email:
+erdogant/df2onehot/archive/1.0.4.tar.gz Author: Erdogan Taskesen Author-email:
 erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 License-File: LICENSE # df2onehot [![Python](https://img.shields.io/pypi/
 pyversions/df2onehot)](https://img.shields.io/pypi/pyversions/df2onehot) [!
 [PyPI Version](https://img.shields.io/pypi/v/df2onehot)](https://pypi.org/
 project/df2onehot/) [![License](https://img.shields.io/badge/license-MIT-
```

### Comparing `df2onehot-1.0.3/README.md` & `df2onehot-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `df2onehot-1.0.3/df2onehot/__init__.py` & `df2onehot-1.0.4/df2onehot/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,25 +7,21 @@
  	set_dtypes,
  	is_DataFrame,
     set_y,
 )
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.0.3'
+__version__ = '1.0.4'
 
 # module level doc-string
 __doc__ = """
 df2onehot is an Python package to convert a pandas dataframe into a stuctured dataframe.
 =============================================================================================
 
-Description
------------
-To convert a pandas dataframe into a more stuctured dataframe.
-
 Example
 -------
 >>> import df2onehot
 >>> df = df2onehot.import_example()
 >>> out = df2onehot.df2onehot(df)
 
 """
```

### Comparing `df2onehot-1.0.3/df2onehot/df2onehot.py` & `df2onehot-1.0.4/df2onehot/df2onehot.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,42 @@
 # Contact     : erdogant@gmail.com
 # github      : https://github.com/erdogant/df2onehot
 # Licence     : MIT
 # ----------------------------------------------------
 
 # %% Libraries
 import warnings
-import wget
+import datazets as dz
 import os
 from tqdm import tqdm
 import numpy as np
 import pandas as pd
 from sklearn.preprocessing import LabelEncoder
 from sklearn.preprocessing import OneHotEncoder
-from df2onehot.utils import set_dtypes
+
+# from df2onehot.utils import set_dtypes
+from utils import set_dtypes
+
 # from set_dtypes import set_dtypes
 label_encoder = LabelEncoder()
 onehot_encoder = OneHotEncoder(sparse=False, categories='auto')
 warnings.filterwarnings('ignore')
 
+
 # %% Dataframe to one-hot
-def df2onehot(df, dtypes='pandas', y_min=None, perc_min_num=None, hot_only=True, deep_extract=False, excl_background=None, remove_mutual_exclusive=False, verbose=3):
+def df2onehot(df,
+              dtypes='pandas',
+              y_min=2,
+              perc_min_num=None,
+              hot_only=True,
+              deep_extract=False,
+              excl_background=None,
+              remove_mutual_exclusive=False,
+              remove_multicollinearity=False,
+              verbose=3):
     """Convert dataframe to one-hot matrix.
 
     Parameters
     ----------
     df : pd.DataFrame()
         Input dataframe for which the rows are the features, and colums are the samples.
     dtypes : list of str or 'pandas', optional
@@ -37,17 +50,20 @@
     perc_min_num : float [None, 0..1], optional
         This parameters can be used to force variables into numeric ones if unique non-zero values are above the percentage. The default is None. Alternative can be 0.8
     hot_only : bool [True, False], optional
         When True; the output of the onehot matrix exclusively contains categorical values that are transformed to one-hot. The default is True.
     deep_extract : bool [False, True] (default : False)
         True: Extract information from a vector that contains a list/array/dict.
         False: converted to a string and treated as catagorical ['cat'].
-    remove_mutual_exclusive : bool [False, True] (default : False)
+    remove_mutual_exclusive: bool [False, True] (default : False)
         True: Remove the mutual exclusive groups. In binairy features; False and 0 are excluded.
         False: Do nothing
+    remove_multicollinearity: bool [False, True] (default : False)
+        True: Remove multicollinear columns by removing one columns for each catagory that is converted into onehot.
+        False: Do nothing
     excl_background : list or None, [0], [0, '0.0', 'unknown', 'nan', 'None' ...], optional
         Remove values/strings that labeled in the list. As an example, the following column: ['yes', 'no', 'yes', 'yes','no','unknown', ...], is split into 'column_yes', 'column_no' and 'column_unknown'. If unknown listed, then 'column_unknown' is not transformed into a new one-hot column.
         The default is None (every possible name is converted into a one-hot column)
     verbose : int, optional
         Print message to screen. The default is 3.
         0: (default), 1: ERROR, 2: WARN, 3: INFO, 4: DEBUG, 5: TRACE
 
@@ -96,15 +112,15 @@
     # Make empty frames
     maxstring=50
     out_numeric = pd.DataFrame()
     out_onehot = pd.DataFrame()
     max_str_len = np.minimum(np.max(list(map(len, df.columns.values.astype(str).tolist()))) + 2, maxstring)
 
     # Run over all columns
-    for i in tqdm(np.arange(0, df.shape[1]), disable=disable):
+    for i in tqdm(np.arange(0, df.shape[1]), disable=disable, desc='[df2onehot]'):
         makespaces = ''.join(['.'] * np.minimum( (max_str_len - len(df.columns[i])), maxstring) )
         # Do not touch a float
         if 'float' in str(df.dtypes[i]):
             # if verbose>=3: print('[df2onehot] >Working on %s' %(df.columns[i]))
             if verbose>=4: print('[df2onehot] >Processing: %s%s [float]' %(df.columns[i][0:maxstring], makespaces))
             out_numeric[df.columns[i]] = df.iloc[:, i]
             if hot_only is False:
@@ -117,32 +133,39 @@
             # integer_encoded = set_y(integer_encoded, y_min=y_min, numeric=True, verbose=0)
             out_numeric[df.columns[i]] = integer_encoded
             out_numeric[df.columns[i]] = out_numeric[df.columns[i]].astype('category')
             if verbose>=4: print('[df2onehot] >Processing: %s%s [%.0f]' %(df.columns[i][0:maxstring], makespaces, len(np.unique(integer_encoded)) ))
 
             # Remove mutual exclusive values
             status_bool=False
-            if remove_mutual_exclusive and len(np.unique(integer_encoded))==2:
+            if (remove_mutual_exclusive or remove_multicollinearity) and len(np.unique(integer_encoded))==2:
                 if np.isin(np.unique(integer_encoded), [0, 1]).sum()>=2:
                     status_bool=True
 
             # Contains a single value or is bool
             if status_bool:
+                if verbose >=3: print('[df2onehot] >Remove mutual exclusive for [%s]' %(df.columns[i]))
                 label = df.columns[i] + '_' + str(df.iloc[integer_encoded==1, i].values[0])
                 out_onehot[label] = integer_encoded.astype('bool')
                 labx.append(label)
             elif (len(np.unique(integer_encoded))<=1) or (str(df.dtypes[i])=='bool'):
                 out_onehot[df.columns[i]] = integer_encoded.astype('bool')
                 labx.append(df.columns[i])
             else:
                 # binary encode
                 onehot_encoded = onehot_encoder.fit_transform(integer_encoded.reshape(-1, 1))
+                total_columns = onehot_encoded.shape[1]
                 # Remove columns if it does not fullfill minimum nr. of samples (>=y_min)
                 if y_min is not None:
                     onehot_encoded = onehot_encoded[:, onehot_encoded.sum(axis=0) >= y_min]
+                # Remove a columns in case to prevent multicollinearity. If a column was already removed for some reason. Do not touch.
+                if remove_multicollinearity and onehot_encoded.shape[1]==total_columns:
+                    if verbose >=3: print('[df2onehot] >Remove multicollinearity for [%s]' %(df.columns[i]))
+                    onehot_encoded = onehot_encoded[:, 1:]
+
                 # Make new one-hot columns
                 for k in range(0, onehot_encoded.shape[1]):
                     # Get the colname based on the value in the orignal dataframe
                     label = df.iloc[onehot_encoded[:, k]==1, i].unique().astype(str)[0]
 
                     # Check whether this is a label that should be excluded.
                     if (isinstance(args['excl_background'], type(None))) or (not np.isin(label, args['excl_background'])):
@@ -307,15 +330,15 @@
 
     # Expand dict
     if np.any(Idict):
         if verbose >=3: print('[df2onehot] >Deep extraction of dictionaries..')
         idxCol = np.where(Idict)[0]
         max_str_len = np.max(list(map(len, df.columns[idxCol].values.astype(str).tolist())))
         # Expand every columns that contains dict
-        for idx in tqdm(idxCol, disable=disable):
+        for idx in tqdm(idxCol, disable=disable, desc='[df2onehot]'):
             makespaces = ''.join([' '] * (max_str_len - len(df.columns[idx])))
             try:
                 dfc, idxempty = dict2df(df.iloc[:, idx])
                 # dfc = pd.DataFrame.from_records(df.iloc[:,idx])
                 # Store the original label
                 label = label + [df.columns[idx]] * dfc.shape[1]
                 if verbose>=4: print('[df2onehot] >[%s]%s >deep extract > [%s]  [%d]' %(df.columns[idx], makespaces, dtypes[idx], dfc.shape[1]))
@@ -342,15 +365,15 @@
     label = []
 
     # Expand list
     if np.any(Ilist):
         idxCol = np.where(Ilist)[0]
         max_str_len = np.max(list(map(len, df.columns[idxCol].values.astype(str).tolist())))
         # Expand every columns that contains either list
-        for idx in tqdm(idxCol, disable=disable):
+        for idx in tqdm(idxCol, disable=disable, desc='[df2onehot]'):
             makespaces = ''.join([' '] * (max_str_len - len(df.columns[idx])))
             # Convert str/float/int to list
             # df, uifeat = _col2type(df, dtypes, idx)
             df.iloc[:, idx], uifeat = _col2type(df.iloc[:, idx], verbose=verbose)
 
             # Convert column into onehot
             if uifeat is not None:
@@ -416,19 +439,17 @@
 # %% Find columns
 def _findcol(x, cols):
     # SLICE COPY WARNING!
     return(np.isin(cols, x))
 
 
 # %% Import example dataset from github.
-def import_example(data='titanic', url=None, sep=',', verbose=3):
+def import_example(data='titanic', url=None, sep=',', overwrite=False, verbose=3):
     """Import example dataset from github source.
 
-    Description
-    -----------
     Import one of the few datasets from github source or specify your own download url link.
 
     Parameters
     ----------
     data : str
         Name of datasets: 'sprinkler', 'titanic', 'student', 'fifa', 'cancer', 'waterpump'
     url : str
@@ -438,57 +459,23 @@
 
     Returns
     -------
     pd.DataFrame()
         Dataset containing mixed features.
 
     """
-    if url is None:
-        if data=='sprinkler':
-            url='https://erdogant.github.io/datasets/sprinkler.zip'
-        elif data=='titanic':
-            url='https://erdogant.github.io/datasets/titanic_train.zip'
-        elif data=='student':
-            url='https://erdogant.github.io/datasets/student_train.zip'
-        elif data=='cancer':
-            url='https://erdogant.github.io/datasets/cancer_dataset.zip'
-        elif data=='fifa':
-            url='https://erdogant.github.io/datasets/FIFA_2018.zip'
-        elif data=='waterpump':
-            url='https://erdogant.github.io/datasets/waterpump/waterpump_test.zip'
-        elif data=='complex':
-            df = pd.DataFrame(index=np.arange(0, 25))
-            df['feat_1'] = np.nan
-            df['feat_1'].iloc[0] = ['3', 4]
-            df['feat_1'].iloc[2] = ['5', '6', '7', '8']
-            df['feat_1'].iloc[20] = ['9', '11', '4']
-            df['feat_1'].iloc[5] = 10
-            df['feat_1'].iloc[15] = 1
-            df['feat_2'] = np.nan
-            df['feat_2'].iloc[0] = ['4', '45']
-            df['feat_2'].iloc[15] = 1
-            df['feat_2'].iloc[20] = 10
-            return df
-        # elif data=='retail':
-            # url='https://erdogant.github.io/datasets/marketing_data_online_retail_small.zip'
+    if data=='complex':
+        df = pd.DataFrame(index=np.arange(0, 25))
+        df['feat_1'] = np.nan
+        df['feat_1'].iloc[0] = ['3', 4]
+        df['feat_1'].iloc[2] = ['5', '6', '7', '8']
+        df['feat_1'].iloc[20] = ['9', '11', '4']
+        df['feat_1'].iloc[5] = 10
+        df['feat_1'].iloc[15] = 1
+        df['feat_2'] = np.nan
+        df['feat_2'].iloc[0] = ['4', '45']
+        df['feat_2'].iloc[15] = 1
+        df['feat_2'].iloc[20] = 10
     else:
-        data = wget.filename_from_url(url)
+        df = dz.get(data=data, url=url, sep=sep, overwrite=overwrite)
 
-    if url is None:
-        if verbose>=3: print('[df2onehot] >Nothing to download.')
-        return None
-
-    curpath = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
-    PATH_TO_DATA = os.path.join(curpath, wget.filename_from_url(url))
-    if not os.path.isdir(curpath):
-        os.makedirs(curpath, exist_ok=True)
-
-    # Check file exists.
-    if not os.path.isfile(PATH_TO_DATA):
-        if verbose>=3: print('[df2onehot] >Downloading [%s] dataset from github source..' %(data))
-        wget.download(url, curpath)
-
-    # Import local dataset
-    if verbose>=3: print('[df2onehot] >Import dataset [%s]' %(data))
-    df = pd.read_csv(PATH_TO_DATA, sep=sep)
-    # Return
     return df
```

### Comparing `df2onehot-1.0.3/df2onehot/examples.py` & `df2onehot-1.0.4/df2onehot/examples.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # %%
-import numpy as np
-from df2onehot import df2onehot, import_example
+# import numpy as np
+# from df2onehot import df2onehot, import_example
 # print(df2onehot.__version__)
 
+# %% Load example
+from df2onehot import df2onehot, import_example
+df = import_example(data="titanic")
+dfhot = df2onehot(df, remove_multicollinearity=True, y_min=2)['onehot']
+
+
+# %%
 df = import_example('complex')
 
 # Run df2onehot
 results = df2onehot(df, deep_extract=True)
 
 results['onehot']
 results['numeric']
 
 
-# %% Load example
-from df2onehot import df2onehot, import_example
-df = import_example(data="titanic")
-
 
 # %% Convert
 results = df2onehot(df)
 results['numeric']
 
 # %% Force feature (int or float) to be numeric if unique non-zero values are above percentage.
 out = df2onehot(df, perc_min_num=0.8)
```

### Comparing `df2onehot-1.0.3/df2onehot/tests/test_df2onehot.py` & `df2onehot-1.0.4/df2onehot/tests/test_df2onehot.py`

 * *Files identical despite different names*

### Comparing `df2onehot-1.0.3/df2onehot/utils.py` & `df2onehot-1.0.4/df2onehot/utils.py`

 * *Files identical despite different names*

### Comparing `df2onehot-1.0.3/df2onehot.egg-info/PKG-INFO` & `df2onehot-1.0.4/df2onehot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: df2onehot
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python package df2onehot is to convert a pandas dataframe into a stuctured dataframe.
 Home-page: https://erdogant.github.io/df2onehot
-Download-URL: https://github.com/erdogant/df2onehot/archive/1.0.3.tar.gz
+Download-URL: https://github.com/erdogant/df2onehot/archive/1.0.4.tar.gz
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
-Metadata-Version: 2.1 Name: df2onehot Version: 1.0.3 Summary: Python package
+Metadata-Version: 2.1 Name: df2onehot Version: 1.0.4 Summary: Python package
 df2onehot is to convert a pandas dataframe into a stuctured dataframe. Home-
 page: https://erdogant.github.io/df2onehot Download-URL: https://github.com/
-erdogant/df2onehot/archive/1.0.3.tar.gz Author: Erdogan Taskesen Author-email:
+erdogant/df2onehot/archive/1.0.4.tar.gz Author: Erdogan Taskesen Author-email:
 erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 License-File: LICENSE # df2onehot [![Python](https://img.shields.io/pypi/
 pyversions/df2onehot)](https://img.shields.io/pypi/pyversions/df2onehot) [!
 [PyPI Version](https://img.shields.io/pypi/v/df2onehot)](https://pypi.org/
 project/df2onehot/) [![License](https://img.shields.io/badge/license-MIT-
```

### Comparing `df2onehot-1.0.3/setup.py` & `df2onehot-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 # Setup ------------
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
-     install_requires=['scikit-learn','numpy','pandas','wget','tqdm'],
+     install_requires=['scikit-learn','numpy','pandas','tqdm','datazets'],
      python_requires='>=3',
      name='df2onehot',
      version=new_version,
      author="Erdogan Taskesen",
      author_email="erdogant@gmail.com",
      description="Python package df2onehot is to convert a pandas dataframe into a stuctured dataframe.",
      long_description=long_description,
```

