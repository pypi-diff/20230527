# Comparing `tmp/coso-1.1.0.tar.gz` & `tmp/coso-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coso-1.1.0.tar", last modified: Fri May 26 07:49:57 2023, max compression
+gzip compressed data, was "coso-1.1.1.tar", last modified: Sat May 27 09:21:40 2023, max compression
```

## Comparing `coso-1.1.0.tar` & `coso-1.1.1.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 07:49:57.449262 coso-1.1.0/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2020-09-14 09:37:08.000000 coso-1.1.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       18 2023-04-27 08:22:38.000000 coso-1.1.0/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     5718 2023-05-26 07:49:57.449038 coso-1.1.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5161 2023-04-11 08:26:28.000000 coso-1.1.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 07:49:57.435914 coso-1.1.0/coso.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5718 2023-05-26 07:49:57.000000 coso-1.1.0/coso.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      571 2023-05-26 07:49:57.000000 coso-1.1.0/coso.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-26 07:49:57.000000 coso-1.1.0/coso.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       50 2023-05-26 07:49:57.000000 coso-1.1.0/coso.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        5 2023-05-26 07:49:57.000000 coso-1.1.0/coso.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       80 2023-02-06 14:52:53.000000 coso-1.1.0/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-26 07:49:57.449331 coso-1.1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1144 2023-05-26 07:36:22.000000 coso-1.1.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 07:49:57.442917 coso-1.1.0/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 07:49:57.444656 coso-1.1.0/src/VisCoSo/
--rwxrwxrwx   0 root         (0) root         (0)      165 2023-04-27 13:29:49.000000 coso-1.1.0/src/VisCoSo/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1564 2023-04-19 08:54:56.000000 coso-1.1.0/src/VisCoSo/header.html
--rwxrwxrwx   0 root         (0) root         (0)     7399 2023-02-03 10:41:56.000000 coso-1.1.0/src/VisCoSo/viscoso.css
--rwxrwxrwx   0 root         (0) root         (0)   113113 2023-04-27 14:09:51.000000 coso-1.1.0/src/VisCoSo/viscoso.html
--rwxrwxrwx   0 root         (0) root         (0)      532 2023-04-12 11:48:32.000000 coso-1.1.0/src/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11427 2023-04-28 10:26:12.000000 coso-1.1.0/src/cola_parser.py
--rwxrwxrwx   0 root         (0) root         (0)     8197 2023-02-03 09:36:00.000000 coso-1.1.0/src/configuration.py
--rwxrwxrwx   0 root         (0) root         (0)     6447 2023-02-01 02:28:35.000000 coso-1.1.0/src/count.py
--rwxrwxrwx   0 root         (0) root         (0)    15881 2023-04-27 14:10:35.000000 coso-1.1.0/src/gen_plots.py
--rwxrwxrwx   0 root         (0) root         (0)     2003 2023-04-19 13:48:19.000000 coso-1.1.0/src/launcher.py
--rwxrwxrwx   0 root         (0) root         (0)    12744 2023-02-03 09:36:28.000000 coso-1.1.0/src/level_1.py
--rwxrwxrwx   0 root         (0) root         (0)    13329 2023-02-03 09:36:37.000000 coso-1.1.0/src/level_2.py
--rwxrwxrwx   0 root         (0) root         (0)     8705 2023-05-26 06:18:26.000000 coso-1.1.0/src/logger.py
--rwxrwxrwx   0 root         (0) root         (0)     9646 2023-04-27 14:45:44.000000 coso-1.1.0/src/parsetab.py
--rwxrwxrwx   0 root         (0) root         (0)     9515 2023-05-25 10:07:11.000000 coso-1.1.0/src/problem.py
--rwxrwxrwx   0 root         (0) root         (0)    85377 2023-02-03 09:37:17.000000 coso-1.1.0/src/sharpCSP.py
--rwxrwxrwx   0 root         (0) root         (0)     2986 2023-02-03 09:37:23.000000 coso-1.1.0/src/solver.py
--rwxrwxrwx   0 root         (0) root         (0)    43522 2023-04-27 14:11:45.000000 coso-1.1.0/src/tester.py
--rwxrwxrwx   0 root         (0) root         (0)    14491 2023-05-01 09:33:15.000000 coso-1.1.0/src/util.py
--rwxrwxrwx   0 root         (0) root         (0)    21856 2023-05-26 06:54:26.000000 coso-1.1.0/src/venn.py
--rwxrwxrwx   0 root         (0) root         (0)    20217 2023-04-27 13:50:00.000000 coso-1.1.0/src/viscoso.py
--rwxrwxrwx   0 root         (0) root         (0)     3878 2023-04-27 15:07:27.000000 coso-1.1.0/src/viscoso_widget.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:21:40.782474 coso-1.1.1/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2020-09-14 09:37:08.000000 coso-1.1.1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-04-27 08:22:38.000000 coso-1.1.1/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     5718 2023-05-27 09:21:40.782044 coso-1.1.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5161 2023-04-11 08:26:28.000000 coso-1.1.1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:21:40.766744 coso-1.1.1/coso.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5718 2023-05-27 09:21:40.000000 coso-1.1.1/coso.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      629 2023-05-27 09:21:40.000000 coso-1.1.1/coso.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-27 09:21:40.000000 coso-1.1.1/coso.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       50 2023-05-27 09:21:40.000000 coso-1.1.1/coso.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2023-05-27 09:21:40.000000 coso-1.1.1/coso.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       80 2023-02-06 14:52:53.000000 coso-1.1.1/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-27 09:21:40.782592 coso-1.1.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1144 2023-05-27 09:21:30.000000 coso-1.1.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:21:40.777036 coso-1.1.1/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:21:40.779630 coso-1.1.1/src/VisCoSo/
+-rwxrwxrwx   0 root         (0) root         (0)      165 2023-04-27 13:29:49.000000 coso-1.1.1/src/VisCoSo/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1564 2023-04-19 08:54:56.000000 coso-1.1.1/src/VisCoSo/header.html
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 09:21:19.000000 coso-1.1.1/src/VisCoSo/tmpmalie4yl.html
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 13:54:13.000000 coso-1.1.1/src/VisCoSo/tmpyegjl8r4.html
+-rwxrwxrwx   0 root         (0) root         (0)     7399 2023-02-03 10:41:56.000000 coso-1.1.1/src/VisCoSo/viscoso.css
+-rwxrwxrwx   0 root         (0) root         (0)   113113 2023-04-27 14:09:51.000000 coso-1.1.1/src/VisCoSo/viscoso.html
+-rwxrwxrwx   0 root         (0) root         (0)      532 2023-04-12 11:48:32.000000 coso-1.1.1/src/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11427 2023-04-28 10:26:12.000000 coso-1.1.1/src/cola_parser.py
+-rwxrwxrwx   0 root         (0) root         (0)     8197 2023-02-03 09:36:00.000000 coso-1.1.1/src/configuration.py
+-rwxrwxrwx   0 root         (0) root         (0)     6447 2023-02-01 02:28:35.000000 coso-1.1.1/src/count.py
+-rwxrwxrwx   0 root         (0) root         (0)    15881 2023-04-27 14:10:35.000000 coso-1.1.1/src/gen_plots.py
+-rwxrwxrwx   0 root         (0) root         (0)     1998 2023-05-26 15:05:32.000000 coso-1.1.1/src/launcher.py
+-rwxrwxrwx   0 root         (0) root         (0)    12744 2023-02-03 09:36:28.000000 coso-1.1.1/src/level_1.py
+-rwxrwxrwx   0 root         (0) root         (0)    13329 2023-02-03 09:36:37.000000 coso-1.1.1/src/level_2.py
+-rwxrwxrwx   0 root         (0) root         (0)     8705 2023-05-26 06:18:26.000000 coso-1.1.1/src/logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     9646 2023-04-27 14:45:44.000000 coso-1.1.1/src/parsetab.py
+-rwxrwxrwx   0 root         (0) root         (0)     9515 2023-05-25 10:07:11.000000 coso-1.1.1/src/problem.py
+-rwxrwxrwx   0 root         (0) root         (0)    85377 2023-02-03 09:37:17.000000 coso-1.1.1/src/sharpCSP.py
+-rwxrwxrwx   0 root         (0) root         (0)     2986 2023-02-03 09:37:23.000000 coso-1.1.1/src/solver.py
+-rwxrwxrwx   0 root         (0) root         (0)    43522 2023-04-27 14:11:45.000000 coso-1.1.1/src/tester.py
+-rwxrwxrwx   0 root         (0) root         (0)    14518 2023-05-26 09:19:25.000000 coso-1.1.1/src/util.py
+-rwxrwxrwx   0 root         (0) root         (0)    21847 2023-05-26 08:04:01.000000 coso-1.1.1/src/venn.py
+-rwxrwxrwx   0 root         (0) root         (0)    20217 2023-04-27 13:50:00.000000 coso-1.1.1/src/viscoso.py
+-rwxrwxrwx   0 root         (0) root         (0)     3878 2023-04-27 15:07:27.000000 coso-1.1.1/src/viscoso_widget.py
```

### Comparing `coso-1.1.0/LICENSE` & `coso-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/PKG-INFO` & `coso-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coso
-Version: 1.1.0
+Version: 1.1.1
 Summary: A solver for combinatorics math word problems.
 Home-page: https://github.com/PietroTotis/CoSo
 Author: Pietro Totis
 Author-email: pietro.totis@kuleuven.be
 License: GNU General Public License (GPL)
 Keywords: combinatorics automated reasoning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coso-1.1.0/README.md` & `coso-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/coso.egg-info/PKG-INFO` & `coso-1.1.1/coso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coso
-Version: 1.1.0
+Version: 1.1.1
 Summary: A solver for combinatorics math word problems.
 Home-page: https://github.com/PietroTotis/CoSo
 Author: Pietro Totis
 Author-email: pietro.totis@kuleuven.be
 License: GNU General Public License (GPL)
 Keywords: combinatorics automated reasoning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coso-1.1.0/coso.egg-info/SOURCES.txt` & `coso-1.1.1/coso.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -24,9 +24,11 @@
 src/tester.py
 src/util.py
 src/venn.py
 src/viscoso.py
 src/viscoso_widget.py
 src/VisCoSo/__init__.py
 src/VisCoSo/header.html
+src/VisCoSo/tmpmalie4yl.html
+src/VisCoSo/tmpyegjl8r4.html
 src/VisCoSo/viscoso.css
 src/VisCoSo/viscoso.html
```

### Comparing `coso-1.1.0/setup.py` & `coso-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='coso',
-    version='1.1.0',    
+    version='1.1.1',    
     url='https://github.com/PietroTotis/CoSo',
     author='Pietro Totis',
     author_email='pietro.totis@kuleuven.be',
     license='GNU General Public License (GPL)',
 
     # packages=find_packages(),
     packages=['coso'],
```

### Comparing `coso-1.1.0/src/VisCoSo/header.html` & `coso-1.1.1/src/VisCoSo/header.html`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/src/VisCoSo/viscoso.css` & `coso-1.1.1/src/VisCoSo/viscoso.css`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/src/VisCoSo/viscoso.html` & `coso-1.1.1/src/VisCoSo/viscoso.html`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/src/__init__.py` & `coso-1.1.1/src/__init__.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/src/cola_parser.py` & `coso-1.1.1/src/cola_parser.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/src/configuration.py` & `coso-1.1.1/src/configuration.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/src/count.py` & `coso-1.1.1/src/count.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/src/gen_plots.py` & `coso-1.1.1/src/gen_plots.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/src/level_1.py` & `coso-1.1.1/src/level_1.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/src/level_2.py` & `coso-1.1.1/src/level_2.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/src/logger.py` & `coso-1.1.1/src/logger.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/src/parsetab.py` & `coso-1.1.1/src/parsetab.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/src/problem.py` & `coso-1.1.1/src/problem.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/src/sharpCSP.py` & `coso-1.1.1/src/sharpCSP.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/src/solver.py` & `coso-1.1.1/src/solver.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/src/tester.py` & `coso-1.1.1/src/tester.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/src/util.py` & `coso-1.1.1/src/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from portion.dict import IntervalDict
 from typing import Counter
 
 
 # ROOT_DIR = os.path.realpath(os.path.join(os.path.dirname(__file__), ".."))
 # CSS_VISCOSO = os.path.join(ROOT_DIR, "src", "VisCoSo", "viscoso.css")
 ROOT_DIR = Path(__file__).parent.parent
-CSS_VISCOSO = ROOT_DIR / "src" / "VisCoSo" / "viscoso.css"
+VISCOSO_DIR = ROOT_DIR / "src" / "VisCoSo" 
+CSS_VISCOSO = VISCOSO_DIR / "viscoso.css"
 
 ######################
 ## Interval methods ##
 ######################
 
 
 def is_distinguishable(d1, d2):
```

### Comparing `coso-1.1.0/src/venn.py` & `coso-1.1.1/src/venn.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,15 +353,14 @@
         # if there are parts unknown from the set info assume they are empty
         for part in self.universe.parts:
             if part.size is None:
                 part.set_size(0)
         # add sets not explicitly mentioned
         for aset in self.base_sets:
             self.universe += self.create_venn_area(Union(aset))
-        
 
     def area2formula(self, area):
         """
         Convert an area code int
 
         Args:
             area (tuple(-1/1/0)): whether a base set is excluded/included/neither
```

### Comparing `coso-1.1.0/src/viscoso.py` & `coso-1.1.1/src/viscoso.py`

 * *Files identical despite different names*

### Comparing `coso-1.1.0/src/viscoso_widget.py` & `coso-1.1.1/src/viscoso_widget.py`

 * *Files identical despite different names*

