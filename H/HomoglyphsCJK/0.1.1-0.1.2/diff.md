# Comparing `tmp/HomoglyphsCJK-0.1.1.tar.gz` & `tmp/HomoglyphsCJK-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HomoglyphsCJK-0.1.1.tar", last modified: Thu May 25 03:10:08 2023, max compression
+gzip compressed data, was "HomoglyphsCJK-0.1.2.tar", last modified: Sat May 27 06:51:10 2023, max compression
```

## Comparing `HomoglyphsCJK-0.1.1.tar` & `HomoglyphsCJK-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-25 03:10:08.447877 HomoglyphsCJK-0.1.1/
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-25 03:10:08.446570 HomoglyphsCJK-0.1.1/HomoglyphsCJK/
--rw-r--r--   0 yangxinmei   (501) staff       (20)       93 2023-05-22 03:32:58.000000 HomoglyphsCJK-0.1.1/HomoglyphsCJK/__init__.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     9649 2023-05-25 03:06:03.000000 HomoglyphsCJK-0.1.1/HomoglyphsCJK/hg_functions.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.1.1/HomoglyphsCJK/test_run.py
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-25 03:10:08.447534 HomoglyphsCJK-0.1.1/HomoglyphsCJK.egg-info/
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3989 2023-05-25 03:10:08.000000 HomoglyphsCJK-0.1.1/HomoglyphsCJK.egg-info/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-05-25 03:10:08.000000 HomoglyphsCJK-0.1.1/HomoglyphsCJK.egg-info/SOURCES.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-25 03:10:08.000000 HomoglyphsCJK-0.1.1/HomoglyphsCJK.egg-info/dependency_links.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-25 03:10:08.000000 HomoglyphsCJK-0.1.1/HomoglyphsCJK.egg-info/requires.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-05-25 03:10:08.000000 HomoglyphsCJK-0.1.1/HomoglyphsCJK.egg-info/top_level.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3989 2023-05-25 03:10:08.447718 HomoglyphsCJK-0.1.1/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3445 2023-05-25 03:09:44.000000 HomoglyphsCJK-0.1.1/README.md
--rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-25 03:10:08.447923 HomoglyphsCJK-0.1.1/setup.cfg
--rw-r--r--   0 yangxinmei   (501) staff       (20)      950 2023-05-25 03:10:01.000000 HomoglyphsCJK-0.1.1/setup.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-27 06:51:10.965134 HomoglyphsCJK-0.1.2/
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-27 06:51:10.963614 HomoglyphsCJK-0.1.2/HomoglyphsCJK/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      122 2023-05-27 06:49:16.000000 HomoglyphsCJK-0.1.2/HomoglyphsCJK/__init__.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)    10932 2023-05-27 06:46:27.000000 HomoglyphsCJK-0.1.2/HomoglyphsCJK/hg_functions.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.1.2/HomoglyphsCJK/test_run.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-27 06:51:10.964700 HomoglyphsCJK-0.1.2/HomoglyphsCJK.egg-info/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     4363 2023-05-27 06:51:10.000000 HomoglyphsCJK-0.1.2/HomoglyphsCJK.egg-info/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-05-27 06:51:10.000000 HomoglyphsCJK-0.1.2/HomoglyphsCJK.egg-info/SOURCES.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-27 06:51:10.000000 HomoglyphsCJK-0.1.2/HomoglyphsCJK.egg-info/dependency_links.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-27 06:51:10.000000 HomoglyphsCJK-0.1.2/HomoglyphsCJK.egg-info/requires.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-05-27 06:51:10.000000 HomoglyphsCJK-0.1.2/HomoglyphsCJK.egg-info/top_level.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     4363 2023-05-27 06:51:10.964963 HomoglyphsCJK-0.1.2/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3819 2023-05-27 06:49:58.000000 HomoglyphsCJK-0.1.2/README.md
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-27 06:51:10.965186 HomoglyphsCJK-0.1.2/setup.cfg
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      950 2023-05-27 06:37:22.000000 HomoglyphsCJK-0.1.2/setup.py
```

### Comparing `HomoglyphsCJK-0.1.1/HomoglyphsCJK/hg_functions.py` & `HomoglyphsCJK-0.1.2/HomoglyphsCJK/hg_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,14 +54,47 @@
         cluster_dict_path = './zht/char_char_dist_dict_800_t_chinese_expanded_easy.pickle'
 
     global cluster_dict
     with open(cluster_dict_path,'rb') as f:
         cluster_dict = pickle.load(f) 
     # return cluster_dict
 
+def homoglyph_pairwise_distance(str1,str2, lang, homo_lambda=1,insertion=1,deletion=1):
+    global cluster_dict
+    download_dict(lang)
+    m = len(str1)
+    n = len(str2)
+    #dp = np.zeros([m+1,n+1]) # it is m rows, n columns
+    dp = [[0 for x in range(n + 1)] for x in range(m + 1)] # This list is quicker than the above numpy array.
+    for i in range(m+1):
+        for j in range(n+1):
+            if i==0 and j==0:
+                dp[i][j]=0
+            elif i==0:
+                dp[i][j]=dp[i][j-1]+1
+            elif j==0:
+                dp[i][j]=dp[i-1][j]+1         
+            elif str1[i-1]==str2[j-1]:
+                dp[i][j]=dp[i-1][j-1]
+            else:
+                global cluster_dict
+                if str1[i-1] in cluster_dict:
+                    if str2[j-1] in cluster_dict[str1[i-1]]:
+                        dist=homo_lambda*(1-cluster_dict[str1[i-1]][str2[j-1]]) # This is gamma actually, the substitution cost is the homoglyphic distance
+                    else:
+                        dist=1 
+                else:
+                    dist=1
+
+                dp[i][j] =  min(dp[i][j-1]+insertion,	 # Insert
+                                dp[i-1][j]+deletion,	 # Remove
+                                dp[i-1][j-1]+dist) 
+
+    return dp[m][n]
+
 def homoglyph_distance(str1,str2, homo_lambda=1,insertion=1,deletion=1):
     m = len(str1)
     n = len(str2)
     #dp = np.zeros([m+1,n+1]) # it is m rows, n columns
     dp = [[0 for x in range(n + 1)] for x in range(m + 1)] # This list is quicker than the above numpy array.
     for i in range(m+1):
         for j in range(n+1):
```

### Comparing `HomoglyphsCJK-0.1.1/HomoglyphsCJK/test_run.py` & `HomoglyphsCJK-0.1.2/HomoglyphsCJK/test_run.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.1.1/HomoglyphsCJK.egg-info/PKG-INFO` & `HomoglyphsCJK-0.1.2/HomoglyphsCJK.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.1.1
+Version: 0.1.2
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 HomoglyphsCJK
 =====
 
-An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words.
+An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words, using character visual similarity.
 
 ## Installation
 ```
 pip install HomoglyphsCJK
 ```
 
 ## Usage
-There are two functionalities of this package: calculate homoglyph distance between two strings, or merge two dataframes based on keys using homoglyph distance.
+There are two functionalities of this package: calculate homoglyph distance between two strings, or merge two dataframes based on keys using homoglyphic edit distance which uses substitution cost considering character visual similarity.
 + If you use homoglyph_merge on specific language, the dict will be downloaded automatically. If you want to calculate pair wise homoglyphic edit distance, before using homoglyph_distance(str1, str2), you need to download_dict(lang) to either download or load the homoglyphs dict.
 + When you firstly use this on one language, the homoglyph dict will be downloaded automatically in the current directory you run your script. So please make sure you run the script from a folder that has permission to write. The available languages are [zhs, zht, ko, ja] for simplified Chinese, traditional Chinese, Korean and Japanese respectively.
 + Merge two dataframes. When you merge two dataframes, you can specify the parallel argument to run multiprocessing. If you don't specify the num_workers when using parallel, it will automatically use the number of all detected CPU cores
 
 ```python
-from HomoglyphsCJK import homoglyph_distance,homoglyph_merge,download_dict
+from HomoglyphsCJK import  homoglyph_pairwise_distance,homoglyph_merge
 import pandas as pd
 df_1 = pd.DataFrame(list(['苏萃乡','办雄','虐格给','雪拉普岗']),columns=['query'])
 df_2 = pd.DataFrame(list(['雪拉普岗日','小苏莽乡','协雄','唐格给','太阳村','月亮湾']),columns=['key'])
 
 # merge two dataframes, note that the homoglyph dict of specified language will be downloaded automatically when first run.
 ## run in parallel with pool of 4, if num_workers is not specified, all available CPU cores are used.
 dataframe_merged = homoglyph_merge('zhs',df_1,df_2,'query','key',homo_lambda=1, insertion=1, deletion=1,parallel=True,num_workers=4)
@@ -58,23 +58,27 @@
 | 雪拉普岗    | 雪拉普岗日                | 1.0       | 
 
 + Homoglyph distance between two strings. The default weight on substitution, insertion, deletion is 1.
 + download_dict will trigger downloading homoglyph dicts to your current directory if it does not already exist, otherwise it just load the existing dict from your local computer.
 
 ```python
     
-download_dict('zhs')
-homoglyph_distance('苏萃乡','小苏莽乡',homo_lambda=1, insertion=1, deletion=1)
+homoglyph_pairwise_distance('苏萃乡','小苏莽乡','zhs',homo_lambda=1, insertion=1, deletion=1)
 # 1.88
 ```
 ## Contributing
 We encourage you to contribute to HomoglyphsCJK!
 
 ## Questions
 If you have any questions using this package, you can open an issue under our [GitHub repository](https://github.com/dell-research-harvard/HomoglyphsCJK/issues). We are maintaining and updating this package, so stay tuned!
 
 ## Citation
-
-Coming Soon
 ```bibtex
-
+@misc{yang2023quantifying,
+      title={Quantifying Character Similarity with Vision Transformers}, 
+      author={Xinmei Yang and Abhishek Arora and Shao-Yu Jheng and Melissa Dell},
+      year={2023},
+      eprint={2305.14672},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
+}
 ```
```

### Comparing `HomoglyphsCJK-0.1.1/PKG-INFO` & `HomoglyphsCJK-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.1.1
+Version: 0.1.2
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 HomoglyphsCJK
 =====
 
-An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words.
+An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words, using character visual similarity.
 
 ## Installation
 ```
 pip install HomoglyphsCJK
 ```
 
 ## Usage
-There are two functionalities of this package: calculate homoglyph distance between two strings, or merge two dataframes based on keys using homoglyph distance.
+There are two functionalities of this package: calculate homoglyph distance between two strings, or merge two dataframes based on keys using homoglyphic edit distance which uses substitution cost considering character visual similarity.
 + If you use homoglyph_merge on specific language, the dict will be downloaded automatically. If you want to calculate pair wise homoglyphic edit distance, before using homoglyph_distance(str1, str2), you need to download_dict(lang) to either download or load the homoglyphs dict.
 + When you firstly use this on one language, the homoglyph dict will be downloaded automatically in the current directory you run your script. So please make sure you run the script from a folder that has permission to write. The available languages are [zhs, zht, ko, ja] for simplified Chinese, traditional Chinese, Korean and Japanese respectively.
 + Merge two dataframes. When you merge two dataframes, you can specify the parallel argument to run multiprocessing. If you don't specify the num_workers when using parallel, it will automatically use the number of all detected CPU cores
 
 ```python
-from HomoglyphsCJK import homoglyph_distance,homoglyph_merge,download_dict
+from HomoglyphsCJK import  homoglyph_pairwise_distance,homoglyph_merge
 import pandas as pd
 df_1 = pd.DataFrame(list(['苏萃乡','办雄','虐格给','雪拉普岗']),columns=['query'])
 df_2 = pd.DataFrame(list(['雪拉普岗日','小苏莽乡','协雄','唐格给','太阳村','月亮湾']),columns=['key'])
 
 # merge two dataframes, note that the homoglyph dict of specified language will be downloaded automatically when first run.
 ## run in parallel with pool of 4, if num_workers is not specified, all available CPU cores are used.
 dataframe_merged = homoglyph_merge('zhs',df_1,df_2,'query','key',homo_lambda=1, insertion=1, deletion=1,parallel=True,num_workers=4)
@@ -58,23 +58,27 @@
 | 雪拉普岗    | 雪拉普岗日                | 1.0       | 
 
 + Homoglyph distance between two strings. The default weight on substitution, insertion, deletion is 1.
 + download_dict will trigger downloading homoglyph dicts to your current directory if it does not already exist, otherwise it just load the existing dict from your local computer.
 
 ```python
     
-download_dict('zhs')
-homoglyph_distance('苏萃乡','小苏莽乡',homo_lambda=1, insertion=1, deletion=1)
+homoglyph_pairwise_distance('苏萃乡','小苏莽乡','zhs',homo_lambda=1, insertion=1, deletion=1)
 # 1.88
 ```
 ## Contributing
 We encourage you to contribute to HomoglyphsCJK!
 
 ## Questions
 If you have any questions using this package, you can open an issue under our [GitHub repository](https://github.com/dell-research-harvard/HomoglyphsCJK/issues). We are maintaining and updating this package, so stay tuned!
 
 ## Citation
-
-Coming Soon
 ```bibtex
-
+@misc{yang2023quantifying,
+      title={Quantifying Character Similarity with Vision Transformers}, 
+      author={Xinmei Yang and Abhishek Arora and Shao-Yu Jheng and Melissa Dell},
+      year={2023},
+      eprint={2305.14672},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
+}
 ```
```

### Comparing `HomoglyphsCJK-0.1.1/README.md` & `HomoglyphsCJK-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 HomoglyphsCJK
 =====
 
-An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words.
+An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words, using character visual similarity.
 
 ## Installation
 ```
 pip install HomoglyphsCJK
 ```
 
 ## Usage
-There are two functionalities of this package: calculate homoglyph distance between two strings, or merge two dataframes based on keys using homoglyph distance.
+There are two functionalities of this package: calculate homoglyph distance between two strings, or merge two dataframes based on keys using homoglyphic edit distance which uses substitution cost considering character visual similarity.
 + If you use homoglyph_merge on specific language, the dict will be downloaded automatically. If you want to calculate pair wise homoglyphic edit distance, before using homoglyph_distance(str1, str2), you need to download_dict(lang) to either download or load the homoglyphs dict.
 + When you firstly use this on one language, the homoglyph dict will be downloaded automatically in the current directory you run your script. So please make sure you run the script from a folder that has permission to write. The available languages are [zhs, zht, ko, ja] for simplified Chinese, traditional Chinese, Korean and Japanese respectively.
 + Merge two dataframes. When you merge two dataframes, you can specify the parallel argument to run multiprocessing. If you don't specify the num_workers when using parallel, it will automatically use the number of all detected CPU cores
 
 ```python
-from HomoglyphsCJK import homoglyph_distance,homoglyph_merge,download_dict
+from HomoglyphsCJK import  homoglyph_pairwise_distance,homoglyph_merge
 import pandas as pd
 df_1 = pd.DataFrame(list(['苏萃乡','办雄','虐格给','雪拉普岗']),columns=['query'])
 df_2 = pd.DataFrame(list(['雪拉普岗日','小苏莽乡','协雄','唐格给','太阳村','月亮湾']),columns=['key'])
 
 # merge two dataframes, note that the homoglyph dict of specified language will be downloaded automatically when first run.
 ## run in parallel with pool of 4, if num_workers is not specified, all available CPU cores are used.
 dataframe_merged = homoglyph_merge('zhs',df_1,df_2,'query','key',homo_lambda=1, insertion=1, deletion=1,parallel=True,num_workers=4)
@@ -46,23 +46,27 @@
 | 雪拉普岗    | 雪拉普岗日                | 1.0       | 
 
 + Homoglyph distance between two strings. The default weight on substitution, insertion, deletion is 1.
 + download_dict will trigger downloading homoglyph dicts to your current directory if it does not already exist, otherwise it just load the existing dict from your local computer.
 
 ```python
     
-download_dict('zhs')
-homoglyph_distance('苏萃乡','小苏莽乡',homo_lambda=1, insertion=1, deletion=1)
+homoglyph_pairwise_distance('苏萃乡','小苏莽乡','zhs',homo_lambda=1, insertion=1, deletion=1)
 # 1.88
 ```
 ## Contributing
 We encourage you to contribute to HomoglyphsCJK!
 
 ## Questions
 If you have any questions using this package, you can open an issue under our [GitHub repository](https://github.com/dell-research-harvard/HomoglyphsCJK/issues). We are maintaining and updating this package, so stay tuned!
 
 ## Citation
-
-Coming Soon
 ```bibtex
-
+@misc{yang2023quantifying,
+      title={Quantifying Character Similarity with Vision Transformers}, 
+      author={Xinmei Yang and Abhishek Arora and Shao-Yu Jheng and Melissa Dell},
+      year={2023},
+      eprint={2305.14672},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
+}
 ```
```

### Comparing `HomoglyphsCJK-0.1.1/setup.py` & `HomoglyphsCJK-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md","r") as fh:
     long_des = fh.read()
 
 setup(
     name="HomoglyphsCJK",
     packages=["HomoglyphsCJK"],
-    version="0.1.1",
+    version="0.1.2",
     author="HomoglyphsCJK Team",
     author_email="homoglyphscjk@gmail.com",
     description="An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer",
     long_description=long_des,
     long_description_content_type="text/markdown",
     url="https://github.com/dell-research-harvard/HomoglyphsCJK.git",
     classifiers=[
```

