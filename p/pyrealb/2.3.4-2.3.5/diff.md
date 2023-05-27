# Comparing `tmp/pyrealb-2.3.4.tar.gz` & `tmp/pyrealb-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrealb-2.3.4.tar", last modified: Wed May 24 15:28:17 2023, max compression
+gzip compressed data, was "pyrealb-2.3.5.tar", last modified: Sat May 27 19:28:10 2023, max compression
```

## Comparing `pyrealb-2.3.4.tar` & `pyrealb-2.3.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-24 15:28:17.997204 pyrealb-2.3.4/
--rw-r--r--   0 lapalme    (503) staff       (20)    35129 2021-12-01 22:24:50.000000 pyrealb-2.3.4/LICENSE
--rw-r--r--   0 lapalme    (503) staff       (20)       23 2022-01-27 01:45:34.000000 pyrealb-2.3.4/MANIFEST.in
--rw-r--r--   0 lapalme    (503) staff       (20)     7577 2023-05-24 15:28:17.997257 pyrealb-2.3.4/PKG-INFO
--rw-r--r--   0 lapalme    (503) staff       (20)     7080 2023-05-24 15:15:37.000000 pyrealb-2.3.4/README.md
--rw-r--r--   0 lapalme    (503) staff       (20)      104 2021-12-13 01:31:17.000000 pyrealb-2.3.4/pyproject.toml
--rw-r--r--   0 lapalme    (503) staff       (20)      649 2023-05-24 15:28:17.997477 pyrealb-2.3.4/setup.cfg
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-24 15:28:17.982825 pyrealb-2.3.4/src/
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-24 15:28:17.986068 pyrealb-2.3.4/src/pyrealb/
--rw-r--r--   0 lapalme    (503) staff       (20)    44540 2023-05-24 14:55:41.000000 pyrealb-2.3.4/src/pyrealb/Constituent.py
--rw-r--r--   0 lapalme    (503) staff       (20)    40808 2023-05-24 14:36:19.000000 pyrealb-2.3.4/src/pyrealb/Dependent.py
--rw-r--r--   0 lapalme    (503) staff       (20)     3050 2023-05-24 14:52:06.000000 pyrealb-2.3.4/src/pyrealb/Lexicon.py
--rw-r--r--   0 lapalme    (503) staff       (20)     7663 2023-03-22 14:56:11.000000 pyrealb-2.3.4/src/pyrealb/Number.py
--rw-r--r--   0 lapalme    (503) staff       (20)    57924 2023-05-24 14:43:55.000000 pyrealb-2.3.4/src/pyrealb/Phrase.py
--rw-r--r--   0 lapalme    (503) staff       (20)    37505 2023-05-23 20:26:22.000000 pyrealb-2.3.4/src/pyrealb/Terminal.py
--rw-r--r--   0 lapalme    (503) staff       (20)    14266 2023-03-27 13:03:50.000000 pyrealb-2.3.4/src/pyrealb/Warning.py
--rw-r--r--   0 lapalme    (503) staff       (20)      857 2023-05-24 14:58:21.000000 pyrealb-2.3.4/src/pyrealb/__init__.py
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-24 15:28:17.991475 pyrealb-2.3.4/src/pyrealb/data/
--rw-r--r--   0 lapalme    (503) staff       (20)  1321684 2023-02-14 02:05:27.000000 pyrealb-2.3.4/src/pyrealb/data/lexicon-en.json
--rw-r--r--   0 lapalme    (503) staff       (20)  2476751 2023-05-23 21:08:01.000000 pyrealb-2.3.4/src/pyrealb/data/lexicon-fr.json
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-24 15:28:17.996651 pyrealb-2.3.4/src/pyrealb/data/pyrealb.egg-info/
--rw-r--r--   0 lapalme    (503) staff       (20)     4155 2022-01-26 22:41:53.000000 pyrealb-2.3.4/src/pyrealb/data/pyrealb.egg-info/PKG-INFO
--rw-r--r--   0 lapalme    (503) staff       (20)        0 2022-01-26 22:41:53.000000 pyrealb-2.3.4/src/pyrealb/data/pyrealb.egg-info/SOURCES.txt
--rw-r--r--   0 lapalme    (503) staff       (20)        1 2022-01-26 22:41:53.000000 pyrealb-2.3.4/src/pyrealb/data/pyrealb.egg-info/dependency_links.txt
--rw-r--r--   0 lapalme    (503) staff       (20)        8 2022-01-26 22:41:53.000000 pyrealb-2.3.4/src/pyrealb/data/pyrealb.egg-info/top_level.txt
--rw-r--r--   0 lapalme    (503) staff       (20)    85976 2023-05-24 15:04:29.000000 pyrealb-2.3.4/src/pyrealb/data/rules-en.json
--rw-r--r--   0 lapalme    (503) staff       (20)   173554 2022-06-14 19:51:41.000000 pyrealb-2.3.4/src/pyrealb/data/rules-fr.json
--rw-r--r--   0 lapalme    (503) staff       (20)     2953 2023-05-24 15:15:37.000000 pyrealb-2.3.4/src/pyrealb/utils.py
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-24 15:28:17.986591 pyrealb-2.3.4/src/pyrealb.egg-info/
--rw-r--r--   0 lapalme    (503) staff       (20)     7577 2023-05-24 15:28:17.000000 pyrealb-2.3.4/src/pyrealb.egg-info/PKG-INFO
--rw-r--r--   0 lapalme    (503) staff       (20)      756 2023-05-24 15:28:17.000000 pyrealb-2.3.4/src/pyrealb.egg-info/SOURCES.txt
--rw-r--r--   0 lapalme    (503) staff       (20)        1 2023-05-24 15:28:17.000000 pyrealb-2.3.4/src/pyrealb.egg-info/dependency_links.txt
--rw-r--r--   0 lapalme    (503) staff       (20)        8 2023-05-24 15:28:17.000000 pyrealb-2.3.4/src/pyrealb.egg-info/top_level.txt
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-24 15:28:17.997062 pyrealb-2.3.4/tests/
--rw-r--r--   0 lapalme    (503) staff       (20)     1879 2023-03-04 13:28:19.000000 pyrealb-2.3.4/tests/test.py
--rw-r--r--   0 lapalme    (503) staff       (20)     2870 2023-02-24 19:49:08.000000 pyrealb-2.3.4/tests/testAll.py
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-27 19:28:10.932472 pyrealb-2.3.5/
+-rw-r--r--   0 lapalme    (503) staff       (20)    35129 2021-12-01 22:24:50.000000 pyrealb-2.3.5/LICENSE
+-rw-r--r--   0 lapalme    (503) staff       (20)       23 2022-01-27 01:45:34.000000 pyrealb-2.3.5/MANIFEST.in
+-rw-r--r--   0 lapalme    (503) staff       (20)     7577 2023-05-27 19:28:10.932522 pyrealb-2.3.5/PKG-INFO
+-rw-r--r--   0 lapalme    (503) staff       (20)     7080 2023-05-27 19:23:04.000000 pyrealb-2.3.5/README.md
+-rw-r--r--   0 lapalme    (503) staff       (20)      104 2021-12-13 01:31:17.000000 pyrealb-2.3.5/pyproject.toml
+-rw-r--r--   0 lapalme    (503) staff       (20)      649 2023-05-27 19:28:10.932745 pyrealb-2.3.5/setup.cfg
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-27 19:28:10.923357 pyrealb-2.3.5/src/
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-27 19:28:10.925145 pyrealb-2.3.5/src/pyrealb/
+-rw-r--r--   0 lapalme    (503) staff       (20)    44540 2023-05-24 14:55:41.000000 pyrealb-2.3.5/src/pyrealb/Constituent.py
+-rw-r--r--   0 lapalme    (503) staff       (20)    40808 2023-05-24 14:36:19.000000 pyrealb-2.3.5/src/pyrealb/Dependent.py
+-rw-r--r--   0 lapalme    (503) staff       (20)     3050 2023-05-24 14:52:06.000000 pyrealb-2.3.5/src/pyrealb/Lexicon.py
+-rw-r--r--   0 lapalme    (503) staff       (20)     7609 2023-05-25 19:51:40.000000 pyrealb-2.3.5/src/pyrealb/Number.py
+-rw-r--r--   0 lapalme    (503) staff       (20)    57924 2023-05-24 14:43:55.000000 pyrealb-2.3.5/src/pyrealb/Phrase.py
+-rw-r--r--   0 lapalme    (503) staff       (20)    37885 2023-05-26 01:43:01.000000 pyrealb-2.3.5/src/pyrealb/Terminal.py
+-rw-r--r--   0 lapalme    (503) staff       (20)    14266 2023-03-27 13:03:50.000000 pyrealb-2.3.5/src/pyrealb/Warning.py
+-rw-r--r--   0 lapalme    (503) staff       (20)      857 2023-05-24 14:58:21.000000 pyrealb-2.3.5/src/pyrealb/__init__.py
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-27 19:28:10.927754 pyrealb-2.3.5/src/pyrealb/data/
+-rw-r--r--   0 lapalme    (503) staff       (20)  1324969 2023-05-25 18:45:57.000000 pyrealb-2.3.5/src/pyrealb/data/lexicon-en.json
+-rw-r--r--   0 lapalme    (503) staff       (20)  2479817 2023-05-25 18:45:57.000000 pyrealb-2.3.5/src/pyrealb/data/lexicon-fr.json
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-27 19:28:10.931892 pyrealb-2.3.5/src/pyrealb/data/pyrealb.egg-info/
+-rw-r--r--   0 lapalme    (503) staff       (20)     4155 2022-01-26 22:41:53.000000 pyrealb-2.3.5/src/pyrealb/data/pyrealb.egg-info/PKG-INFO
+-rw-r--r--   0 lapalme    (503) staff       (20)        0 2022-01-26 22:41:53.000000 pyrealb-2.3.5/src/pyrealb/data/pyrealb.egg-info/SOURCES.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)        1 2022-01-26 22:41:53.000000 pyrealb-2.3.5/src/pyrealb/data/pyrealb.egg-info/dependency_links.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)        8 2022-01-26 22:41:53.000000 pyrealb-2.3.5/src/pyrealb/data/pyrealb.egg-info/top_level.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)    85976 2023-05-24 15:04:29.000000 pyrealb-2.3.5/src/pyrealb/data/rules-en.json
+-rw-r--r--   0 lapalme    (503) staff       (20)   173554 2022-06-14 19:51:41.000000 pyrealb-2.3.5/src/pyrealb/data/rules-fr.json
+-rw-r--r--   0 lapalme    (503) staff       (20)     2953 2023-05-27 19:23:04.000000 pyrealb-2.3.5/src/pyrealb/utils.py
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-27 19:28:10.925628 pyrealb-2.3.5/src/pyrealb.egg-info/
+-rw-r--r--   0 lapalme    (503) staff       (20)     7577 2023-05-27 19:28:10.000000 pyrealb-2.3.5/src/pyrealb.egg-info/PKG-INFO
+-rw-r--r--   0 lapalme    (503) staff       (20)      756 2023-05-27 19:28:10.000000 pyrealb-2.3.5/src/pyrealb.egg-info/SOURCES.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)        1 2023-05-27 19:28:10.000000 pyrealb-2.3.5/src/pyrealb.egg-info/dependency_links.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)        8 2023-05-27 19:28:10.000000 pyrealb-2.3.5/src/pyrealb.egg-info/top_level.txt
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-27 19:28:10.932363 pyrealb-2.3.5/tests/
+-rw-r--r--   0 lapalme    (503) staff       (20)     1879 2023-03-04 13:28:19.000000 pyrealb-2.3.5/tests/test.py
+-rw-r--r--   0 lapalme    (503) staff       (20)     2870 2023-02-24 19:49:08.000000 pyrealb-2.3.5/tests/testAll.py
```

### Comparing `pyrealb-2.3.4/LICENSE` & `pyrealb-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.4/PKG-INFO` & `pyrealb-2.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyrealb
-Version: 2.3.4
+Version: 2.3.5
 Summary: A French-English text realizer
 Home-page: https://github.com/lapalme/pyrealb
 Author: Guy Lapalme
 Author-email: lapalme@iro.umontreal.ca
 Project-URL: Bug Tracker, https://github.com/lapalme/pyrealb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # *pyRealB* - A Python Bilingual Text Realizer
 
-*Version 2.3.4 - May 2023*
+*Version 2.3.5 - May 2023*
 
 *pyRealB* is a Python adaptation of the JavaScript [**jsRealB**](http://rali.iro.umontreal.ca/jsRealB) 
 text realizer with the same constituent and dependency syntax notation. 
 It facilitates its integration within Python applications by simply adding
 
 	from pyrealb import *
```

### Comparing `pyrealb-2.3.4/README.md` & `pyrealb-2.3.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # *pyRealB* - A Python Bilingual Text Realizer
 
-*Version 2.3.4 - May 2023*
+*Version 2.3.5 - May 2023*
 
 *pyRealB* is a Python adaptation of the JavaScript [**jsRealB**](http://rali.iro.umontreal.ca/jsRealB) 
 text realizer with the same constituent and dependency syntax notation. 
 It facilitates its integration within Python applications by simply adding
 
 	from pyrealb import *
```

### Comparing `pyrealb-2.3.4/setup.cfg` & `pyrealb-2.3.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyrealb
-version = 2.3.4
+version = 2.3.5
 author = Guy Lapalme
 author_email = lapalme@iro.umontreal.ca
 description = A French-English text realizer
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/lapalme/pyrealb
 project_urls =
```

### Comparing `pyrealb-2.3.4/src/pyrealb/Constituent.py` & `pyrealb-2.3.5/src/pyrealb/Constituent.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.4/src/pyrealb/Dependent.py` & `pyrealb-2.3.5/src/pyrealb/Dependent.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.4/src/pyrealb/Lexicon.py` & `pyrealb-2.3.5/src/pyrealb/Lexicon.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.4/src/pyrealb/Number.py` & `pyrealb-2.3.5/src/pyrealb/Number.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,30 +50,28 @@
         if head=="000": return grouper(tail)
         uM=unitsM if en else unitesM
         return (uM[l-2]["sing"] if head=="001" else grouper([head])+" "+uM[l-2]["plur"])\
                 +" "+("" if tousZero(tail) else grouper(tail))
 
     # traiter un nombre entre 0 et 999
     def centaines(ns): # ns est une chaine d'au plus trois chiffres
-        if trace:print("centaines:"+ns)
         if len(ns)==1: return unites(ns)
         if len(ns)==2: return dizaines(ns)
         c=ns[0]       # centaines
         du=ns[1:] # dizaines+unités
         if c=="0": return dizaines(du)
         cent="hundred" if en else "cent"
         if du=="00":
             if c=="1":return ("one " if en else "")+cent
             return unites(c)+" "+cent+("" if en else "s")
         if c=="1": return ("one " if en else "")+cent+" "+dizaines(du)
         return unites(c)+" "+cent+(" and " if en else" ")+dizaines(du)
 
     # traiter un nombre entre 10 et 99
     def dizaines(ns):# ns est une chaine de deux chiffres
-        if trace: print("dizaines:",ns);
         d=ns[0] # dizaines
         u=ns[1] # unités
         if d=="0": return unites(u)
         elif d=="1":
             if en: 
                 return ["ten","eleven","twelve","thirteen","fourteen","fifteen","sixteen","seventeen","eighteen","nineteen"][int(u)]
             else:
@@ -81,15 +79,15 @@
         elif d in "23456":
             tens = (["twenty","thirty","forty","fifty","sixty"] if en else 
                     ["vingt","trente","quarante","cinquante","soixante"])[int(d)-2]
             if u=="0": return tens
             return tens + ( ("-one" if en else " et un") if u=="1" else ("-"+unites(u)))
         elif d=="7":
             if u=="0": return "seventy" if en else "soixante-dix"
-            return ("seventy-"+unites(u))if en else ("soixante-"+dizaines("1"+u))
+            return ("seventy-"+unites(u))if en else ("soixante"+(" et " if u=="1" else "-")+dizaines("1"+u))
         elif d=="8":
             if u=="0": return "eighty" if en else "quatre-vingts"
             return ("eighty-" if en else "quatre-vingt-")+unites(u)
         elif d=="9":
             if u=="0": return "ninety" if en else "quatre-vingt-dix"
             return ("ninety-"+unites(u))if en else ("quatre-vingt-"+dizaines("1"+u))
         else:
```

### Comparing `pyrealb-2.3.4/src/pyrealb/Phrase.py` & `pyrealb-2.3.5/src/pyrealb/Phrase.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.4/src/pyrealb/Terminal.py` & `pyrealb-2.3.5/src/pyrealb/Terminal.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,29 +56,37 @@
                         "hour":True,"minute":True,"second":True,
                         "nat":True,"det":True,"rtime":False}
         elif terminalType=="NO":
             if not isinstance(lemma,(str,int,float)):
                 self.warn("bad parameter",["str","int","float"],type(lemma).__name__)
                 self.lemma=0
             elif isinstance(lemma,str):
+                lexInfo = getLemma(self.lemma)
+                if "value" in lexInfo:
+                    self.lemma=self.value=lexInfo["value"]
+                    self.nbDecimals=0
+                    self.props["dOpt"] = {"nat":True}
+                    self.addOptSource("nat",True)
+                    return
                 # check if this looks like a legal number
-                if not re.match(r"^[-+]?[0-9]+([., ][0-9]*)?([Ee][-+][0-9]+)?$",lemma):
-                    self.warn("bad parameter","number",type(lemma).__name__)
-                    self.lemma=0
                 else:
-                    self.lemma=re.sub(r"," if self.isEn() else r" ","",self.lemma)
-                try:
-                    self.value=int(self.lemma)
-                except ValueError:
-                    self.value=float(self.lemma)
-                self.nbDecimals=str(self.lemma)[::-1].find(".")
+                    if not re.match(r"^[-+]?[0-9]+([., ][0-9]*)?([Ee][-+][0-9]+)?$",lemma):
+                        self.warn("bad parameter","number",type(lemma).__name__)
+                        self.lemma=0
+                    else:
+                        self.lemma=re.sub(r"," if self.isEn() else r" ","",self.lemma)
+                    try:
+                        self.value=int(self.lemma)
+                    except ValueError:
+                        self.value=float(self.lemma)
+                    self.nbDecimals=str(self.lemma)[::-1].find(".")
             else:
                 self.value=lemma
                 self.nbDecimals=str(lemma)[::-1].find(".")
-            if self.nbDecimals<0:self.nbDecimals=0
+                if self.nbDecimals<0:self.nbDecimals=0
             self.props["dOpt"]={"mprecision":2,"raw":False,"ord":False}
         elif terminalType=="Q":
             self.lemma=str(lemma)
         elif terminalType in ["N","A","Pro","D","V","Adv","C","P"]:
             if not isinstance(lemma,str):
                 self.tab=None 
                 self.realization=f"[[{lemma}]]"
```

### Comparing `pyrealb-2.3.4/src/pyrealb/Warning.py` & `pyrealb-2.3.5/src/pyrealb/Warning.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.4/src/pyrealb/__init__.py` & `pyrealb-2.3.5/src/pyrealb/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.4/src/pyrealb/data/lexicon-en.json` & `pyrealb-2.3.5/src/pyrealb/data/lexicon-en.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983150502937058%*

 * *Differences: {"'billion'": "{'D': {delete: ['value']}, 'value': 1000000000}",*

 * * "'billionth'": "{'A': {delete: ['value']}, 'value': 1000000000}",*

 * * "'cloudiness'": "OrderedDict([('N', OrderedDict([('tab', 'n5')]))])",*

 * * "'eight'": "{'D': {delete: ['value']}, 'value': 8}",*

 * * "'eighteen'": "{'D': {delete: ['value']}, 'value': 18}",*

 * * "'eighteenth'": "{'A': {delete: ['value']}, 'value': 18}",*

 * * "'eighth'": "{'A': {delete: ['value']}, 'value': 8}",*

 * * "'eightieth'": "{'A': {delete: ['value']}, 'value': 80}",*

 * * "'eighty'": "{'D': {de […]*

```diff
@@ -19329,29 +19329,29 @@
         "N": {
             "tab": "n5"
         }
     },
     "billion": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "1000000000"
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 1000000000
     },
     "billionth": {
         "A": {
-            "tab": "a1",
-            "value": 1000000000
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 1000000000
     },
     "billow": {
         "N": {
             "tab": "n1"
         },
         "V": {
             "tab": "v1"
@@ -32224,14 +32224,19 @@
         }
     },
     "cloud-cuckoo-land": {
         "N": {
             "tab": "n5"
         }
     },
+    "cloudiness": {
+        "N": {
+            "tab": "n5"
+        }
+    },
     "cloudless": {
         "A": {
             "tab": "a1"
         }
     },
     "cloudy": {
         "A": {
@@ -54860,62 +54865,62 @@
         "N": {
             "tab": "n1"
         }
     },
     "eight": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "8"
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 8
     },
     "eighteen": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "18"
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 18
     },
     "eighteenth": {
         "A": {
-            "tab": "a1",
-            "value": 18
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 18
     },
     "eighth": {
         "A": {
-            "tab": "a1",
-            "value": 8
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 8
     },
     "eighthly": {
         "Adv": {
             "tab": "b1"
         }
     },
     "eightieth": {
         "A": {
-            "tab": "a1",
-            "value": 80
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 80
     },
     "eightpence": {
         "N": {
             "tab": "n1"
         }
     },
     "eightpenny": {
@@ -54927,137 +54932,137 @@
         "N": {
             "tab": "n1"
         }
     },
     "eighty": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "80"
+            "tab": "d4"
         },
         "N": {
             "tab": "n3"
-        }
+        },
+        "value": 80
     },
     "eighty-eight": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "88"
-        }
+            "tab": "d4"
+        },
+        "value": 88
     },
     "eighty-eighth": {
         "A": {
-            "tab": "a1",
-            "value": 88
-        }
+            "tab": "a1"
+        },
+        "value": 88
     },
     "eighty-fifth": {
         "A": {
-            "tab": "a1",
-            "value": 85
-        }
+            "tab": "a1"
+        },
+        "value": 85
     },
     "eighty-first": {
         "A": {
-            "tab": "a1",
-            "value": 81
-        }
+            "tab": "a1"
+        },
+        "value": 81
     },
     "eighty-five": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "85"
-        }
+            "tab": "d4"
+        },
+        "value": 85
     },
     "eighty-four": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "84"
-        }
+            "tab": "d4"
+        },
+        "value": 84
     },
     "eighty-fourth": {
         "A": {
-            "tab": "a1",
-            "value": 84
-        }
+            "tab": "a1"
+        },
+        "value": 84
     },
     "eighty-nine": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "89"
-        }
+            "tab": "d4"
+        },
+        "value": 89
     },
     "eighty-ninth": {
         "A": {
-            "tab": "a1",
-            "value": 89
-        }
+            "tab": "a1"
+        },
+        "value": 89
     },
     "eighty-one": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "81"
-        }
+            "tab": "d4"
+        },
+        "value": 81
     },
     "eighty-second": {
         "A": {
-            "tab": "a1",
-            "value": 82
-        }
+            "tab": "a1"
+        },
+        "value": 82
     },
     "eighty-seven": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "87"
-        }
+            "tab": "d4"
+        },
+        "value": 87
     },
     "eighty-seventh": {
         "A": {
-            "tab": "a1",
-            "value": 87
-        }
+            "tab": "a1"
+        },
+        "value": 87
     },
     "eighty-six": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "86"
-        }
+            "tab": "d4"
+        },
+        "value": 86
     },
     "eighty-sixth": {
         "A": {
-            "tab": "a1",
-            "value": 86
-        }
+            "tab": "a1"
+        },
+        "value": 86
     },
     "eighty-third": {
         "A": {
-            "tab": "a1",
-            "value": 83
-        }
+            "tab": "a1"
+        },
+        "value": 83
     },
     "eighty-three": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "83"
-        }
+            "tab": "d4"
+        },
+        "value": 83
     },
     "eighty-two": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "82"
-        }
+            "tab": "d4"
+        },
+        "value": 82
     },
     "eisteddfod": {
         "N": {
             "tab": "n1"
         }
     },
     "either": {
@@ -55426,34 +55431,34 @@
         "N": {
             "tab": "n1"
         }
     },
     "eleven": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "11"
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 11
     },
     "elevenses": {
         "N": {
             "tab": "n6"
         }
     },
     "eleventh": {
         "A": {
-            "tab": "a1",
-            "value": 11
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 11
     },
     "eleventhly": {
         "Adv": {
             "tab": "b1"
         }
     },
     "elf": {
@@ -63120,179 +63125,179 @@
         "N": {
             "tab": "n1"
         }
     },
     "fifteen": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "15"
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 15
     },
     "fifteenth": {
         "A": {
-            "tab": "a1",
-            "value": 15
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 15
     },
     "fifth": {
         "A": {
-            "tab": "a1",
-            "value": 5
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 5
     },
     "fifthly": {
         "Adv": {
             "tab": "b1"
         }
     },
     "fiftieth": {
         "A": {
-            "tab": "a1",
-            "value": 50
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 50
     },
     "fifty": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "50"
+            "tab": "d4"
         },
         "N": {
             "tab": "n3"
-        }
+        },
+        "value": 50
     },
     "fifty-eight": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "58"
-        }
+            "tab": "d4"
+        },
+        "value": 58
     },
     "fifty-eighth": {
         "A": {
-            "tab": "a1",
-            "value": 58
-        }
+            "tab": "a1"
+        },
+        "value": 58
     },
     "fifty-fifth": {
         "A": {
-            "tab": "a1",
-            "value": 55
-        }
+            "tab": "a1"
+        },
+        "value": 55
     },
     "fifty-first": {
         "A": {
-            "tab": "a1",
-            "value": 51
-        }
+            "tab": "a1"
+        },
+        "value": 51
     },
     "fifty-five": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "55"
-        }
+            "tab": "d4"
+        },
+        "value": 55
     },
     "fifty-four": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "54"
-        }
+            "tab": "d4"
+        },
+        "value": 54
     },
     "fifty-fourth": {
         "A": {
-            "tab": "a1",
-            "value": 54
-        }
+            "tab": "a1"
+        },
+        "value": 54
     },
     "fifty-nine": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "59"
-        }
+            "tab": "d4"
+        },
+        "value": 59
     },
     "fifty-ninth": {
         "A": {
-            "tab": "a1",
-            "value": 59
-        }
+            "tab": "a1"
+        },
+        "value": 59
     },
     "fifty-one": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "51"
-        }
+            "tab": "d4"
+        },
+        "value": 51
     },
     "fifty-second": {
         "A": {
-            "tab": "a1",
-            "value": 52
-        }
+            "tab": "a1"
+        },
+        "value": 52
     },
     "fifty-seven": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "57"
-        }
+            "tab": "d4"
+        },
+        "value": 57
     },
     "fifty-seventh": {
         "A": {
-            "tab": "a1",
-            "value": 57
-        }
+            "tab": "a1"
+        },
+        "value": 57
     },
     "fifty-six": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "56"
-        }
+            "tab": "d4"
+        },
+        "value": 56
     },
     "fifty-sixth": {
         "A": {
-            "tab": "a1",
-            "value": 56
-        }
+            "tab": "a1"
+        },
+        "value": 56
     },
     "fifty-third": {
         "A": {
-            "tab": "a1",
-            "value": 53
-        }
+            "tab": "a1"
+        },
+        "value": 53
     },
     "fifty-three": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "53"
-        }
+            "tab": "d4"
+        },
+        "value": 53
     },
     "fifty-two": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "52"
-        }
+            "tab": "d4"
+        },
+        "value": 52
     },
     "fig": {
         "N": {
             "tab": "n1"
         },
         "basic": true
     },
@@ -64027,23 +64032,23 @@
     "firmness": {
         "N": {
             "tab": "n5"
         }
     },
     "first": {
         "A": {
-            "tab": "a1",
-            "value": 1
+            "tab": "a1"
         },
         "Adv": {
             "tab": "b1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 1
     },
     "first-class": {
         "A": {
             "tab": "a1"
         },
         "Adv": {
             "tab": "b1"
@@ -64294,20 +64299,20 @@
             "tab": "n1"
         },
         "basic": true
     },
     "five": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "5"
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 5
     },
     "fivefold": {
         "A": {
             "tab": "a1"
         }
     },
     "fivepence": {
@@ -66990,20 +66995,20 @@
     "forthwith": {
         "Adv": {
             "tab": "b1"
         }
     },
     "fortieth": {
         "A": {
-            "tab": "a1",
-            "value": 40
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 40
     },
     "fortification": {
         "N": {
             "tab": "n1"
         }
     },
     "fortify": {
@@ -67070,137 +67075,137 @@
             "tab": "n1"
         },
         "basic": true
     },
     "forty": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "40"
+            "tab": "d4"
         },
         "N": {
             "tab": "n3"
-        }
+        },
+        "value": 40
     },
     "forty-eight": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "48"
-        }
+            "tab": "d4"
+        },
+        "value": 48
     },
     "forty-eighth": {
         "A": {
-            "tab": "a1",
-            "value": 48
-        }
+            "tab": "a1"
+        },
+        "value": 48
     },
     "forty-fifth": {
         "A": {
-            "tab": "a1",
-            "value": 45
-        }
+            "tab": "a1"
+        },
+        "value": 45
     },
     "forty-first": {
         "A": {
-            "tab": "a1",
-            "value": 41
-        }
+            "tab": "a1"
+        },
+        "value": 41
     },
     "forty-five": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "45"
-        }
+            "tab": "d4"
+        },
+        "value": 45
     },
     "forty-four": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "44"
-        }
+            "tab": "d4"
+        },
+        "value": 44
     },
     "forty-fourth": {
         "A": {
-            "tab": "a1",
-            "value": 44
-        }
+            "tab": "a1"
+        },
+        "value": 44
     },
     "forty-nine": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "49"
-        }
+            "tab": "d4"
+        },
+        "value": 49
     },
     "forty-ninth": {
         "A": {
-            "tab": "a1",
-            "value": 49
-        }
+            "tab": "a1"
+        },
+        "value": 49
     },
     "forty-one": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "41"
-        }
+            "tab": "d4"
+        },
+        "value": 41
     },
     "forty-second": {
         "A": {
-            "tab": "a1",
-            "value": 42
-        }
+            "tab": "a1"
+        },
+        "value": 42
     },
     "forty-seven": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "47"
-        }
+            "tab": "d4"
+        },
+        "value": 47
     },
     "forty-seventh": {
         "A": {
-            "tab": "a1",
-            "value": 47
-        }
+            "tab": "a1"
+        },
+        "value": 47
     },
     "forty-six": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "46"
-        }
+            "tab": "d4"
+        },
+        "value": 46
     },
     "forty-sixth": {
         "A": {
-            "tab": "a1",
-            "value": 46
-        }
+            "tab": "a1"
+        },
+        "value": 46
     },
     "forty-third": {
         "A": {
-            "tab": "a1",
-            "value": 43
-        }
+            "tab": "a1"
+        },
+        "value": 43
     },
     "forty-three": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "43"
-        }
+            "tab": "d4"
+        },
+        "value": 43
     },
     "forty-two": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "42"
-        }
+            "tab": "d4"
+        },
+        "value": 42
     },
     "forum": {
         "N": {
             "tab": "n1"
         },
         "basic": true
     },
@@ -67379,20 +67384,20 @@
         "N": {
             "tab": "n1"
         }
     },
     "four": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "4"
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 4
     },
     "four-in-hand": {
         "N": {
             "tab": "n1"
         }
     },
     "four-part": {
@@ -67455,38 +67460,38 @@
         "A": {
             "tab": "a1"
         }
     },
     "fourteen": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "14"
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 14
     },
     "fourteenth": {
         "A": {
-            "tab": "a1",
-            "value": 14
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 14
     },
     "fourth": {
         "A": {
-            "tab": "a1",
-            "value": 4
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 4
     },
     "fourthly": {
         "Adv": {
             "tab": "b1"
         }
     },
     "fowl": {
@@ -75025,14 +75030,17 @@
         "N": {
             "tab": "n1"
         }
     },
     "gust": {
         "N": {
             "tab": "n1"
+        },
+        "V": {
+            "tab": "v1"
         }
     },
     "gustation": {
         "N": {
             "tab": "n5"
         }
     },
@@ -81236,34 +81244,34 @@
         "A": {
             "tab": "a1"
         }
     },
     "hundred": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "100"
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 100
     },
     "hundredfold": {
         "Adv": {
             "tab": "b1"
         }
     },
     "hundredth": {
         "A": {
-            "tab": "a1",
-            "value": 100
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 100
     },
     "hundredweight": {
         "N": {
             "tab": "n1"
         }
     },
     "hunger": {
@@ -104206,40 +104214,40 @@
         "N": {
             "tab": "n5"
         }
     },
     "million": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "1000000"
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 1000000
     },
     "millionaire": {
         "N": {
             "g": "x",
             "tab": "n1"
         }
     },
     "millionfold": {
         "Adv": {
             "tab": "b1"
         }
     },
     "millionth": {
         "A": {
-            "tab": "a1",
-            "value": 1000000
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 1000000
     },
     "millipede": {
         "N": {
             "tab": "n1"
         }
     },
     "millstone": {
@@ -110361,20 +110369,20 @@
         "N": {
             "tab": "n1"
         }
     },
     "nine": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "9"
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 9
     },
     "ninefold": {
         "A": {
             "tab": "a1"
         },
         "Adv": {
             "tab": "b1"
@@ -110394,179 +110402,179 @@
         "N": {
             "tab": "n5"
         }
     },
     "nineteen": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "19"
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 19
     },
     "nineteenth": {
         "A": {
-            "tab": "a1",
-            "value": 19
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 19
     },
     "ninetieth": {
         "A": {
-            "tab": "a1",
-            "value": 90
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 90
     },
     "ninety": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "90"
+            "tab": "d4"
         },
         "N": {
             "tab": "n3"
-        }
+        },
+        "value": 90
     },
     "ninety-eight": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "98"
-        }
+            "tab": "d4"
+        },
+        "value": 98
     },
     "ninety-eighth": {
         "A": {
-            "tab": "a1",
-            "value": 98
-        }
+            "tab": "a1"
+        },
+        "value": 98
     },
     "ninety-fifth": {
         "A": {
-            "tab": "a1",
-            "value": 95
-        }
+            "tab": "a1"
+        },
+        "value": 95
     },
     "ninety-first": {
         "A": {
-            "tab": "a1",
-            "value": 91
-        }
+            "tab": "a1"
+        },
+        "value": 91
     },
     "ninety-five": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "95"
-        }
+            "tab": "d4"
+        },
+        "value": 95
     },
     "ninety-four": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "94"
-        }
+            "tab": "d4"
+        },
+        "value": 94
     },
     "ninety-fourth": {
         "A": {
-            "tab": "a1",
-            "value": 94
-        }
+            "tab": "a1"
+        },
+        "value": 94
     },
     "ninety-nine": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "99"
-        }
+            "tab": "d4"
+        },
+        "value": 99
     },
     "ninety-ninth": {
         "A": {
-            "tab": "a1",
-            "value": 99
-        }
+            "tab": "a1"
+        },
+        "value": 99
     },
     "ninety-one": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "91"
-        }
+            "tab": "d4"
+        },
+        "value": 91
     },
     "ninety-second": {
         "A": {
-            "tab": "a1",
-            "value": 92
-        }
+            "tab": "a1"
+        },
+        "value": 92
     },
     "ninety-seven": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "97"
-        }
+            "tab": "d4"
+        },
+        "value": 97
     },
     "ninety-seventh": {
         "A": {
-            "tab": "a1",
-            "value": 97
-        }
+            "tab": "a1"
+        },
+        "value": 97
     },
     "ninety-six": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "96"
-        }
+            "tab": "d4"
+        },
+        "value": 96
     },
     "ninety-sixth": {
         "A": {
-            "tab": "a1",
-            "value": 96
-        }
+            "tab": "a1"
+        },
+        "value": 96
     },
     "ninety-third": {
         "A": {
-            "tab": "a1",
-            "value": 93
-        }
+            "tab": "a1"
+        },
+        "value": 93
     },
     "ninety-three": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "93"
-        }
+            "tab": "d4"
+        },
+        "value": 93
     },
     "ninety-two": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "92"
-        }
+            "tab": "d4"
+        },
+        "value": 92
     },
     "ninny": {
         "N": {
             "tab": "n3"
         }
     },
     "ninth": {
         "A": {
-            "tab": "a1",
-            "value": 9
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 9
     },
     "ninthly": {
         "Adv": {
             "tab": "b1"
         }
     },
     "nip": {
@@ -113762,24 +113770,24 @@
         },
         "N": {
             "tab": "n5"
         }
     },
     "one": {
         "D": {
-            "tab": "d4",
-            "value": "1"
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
         },
         "Pro": {
             "tab": "pn6"
         },
-        "basic": true
+        "basic": true,
+        "value": 1
     },
     "one-armed": {
         "A": {
             "tab": "a1"
         }
     },
     "one-eyed": {
@@ -147304,27 +147312,27 @@
     "seclusion": {
         "N": {
             "tab": "n5"
         }
     },
     "second": {
         "A": {
-            "tab": "a1",
-            "value": 2
+            "tab": "a1"
         },
         "Adv": {
             "tab": "b1"
         },
         "N": {
             "tab": "n1"
         },
         "V": {
             "tab": "v1"
         },
-        "basic": true
+        "basic": true,
+        "value": 2
     },
     "second-best": {
         "A": {
             "tab": "a1"
         },
         "Adv": {
             "tab": "b1"
@@ -149319,197 +149327,197 @@
         "N": {
             "tab": "n1"
         }
     },
     "seven": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "7"
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 7
     },
     "sevenfold": {
         "A": {
             "tab": "a1"
         },
         "Adv": {
             "tab": "b1"
         }
     },
     "seventeen": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "17"
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 17
     },
     "seventeenth": {
         "A": {
-            "tab": "a1",
-            "value": 17
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 17
     },
     "seventh": {
         "A": {
-            "tab": "a1",
-            "value": 7
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 7
     },
     "seventhly": {
         "Adv": {
             "tab": "b1"
         }
     },
     "seventieth": {
         "A": {
-            "tab": "a1",
-            "value": 70
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 70
     },
     "seventy": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "70"
+            "tab": "d4"
         },
         "N": {
             "tab": "n3"
-        }
+        },
+        "value": 70
     },
     "seventy-eight": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "78"
-        }
+            "tab": "d4"
+        },
+        "value": 78
     },
     "seventy-eighth": {
         "A": {
-            "tab": "a1",
-            "value": 78
-        }
+            "tab": "a1"
+        },
+        "value": 78
     },
     "seventy-fifth": {
         "A": {
-            "tab": "a1",
-            "value": 75
-        }
+            "tab": "a1"
+        },
+        "value": 75
     },
     "seventy-first": {
         "A": {
-            "tab": "a1",
-            "value": 71
-        }
+            "tab": "a1"
+        },
+        "value": 71
     },
     "seventy-five": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "75"
-        }
+            "tab": "d4"
+        },
+        "value": 75
     },
     "seventy-four": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "74"
-        }
+            "tab": "d4"
+        },
+        "value": 74
     },
     "seventy-fourth": {
         "A": {
-            "tab": "a1",
-            "value": 74
-        }
+            "tab": "a1"
+        },
+        "value": 74
     },
     "seventy-nine": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "79"
-        }
+            "tab": "d4"
+        },
+        "value": 79
     },
     "seventy-ninth": {
         "A": {
-            "tab": "a1",
-            "value": 79
-        }
+            "tab": "a1"
+        },
+        "value": 79
     },
     "seventy-one": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "71"
-        }
+            "tab": "d4"
+        },
+        "value": 71
     },
     "seventy-second": {
         "A": {
-            "tab": "a1",
-            "value": 72
-        }
+            "tab": "a1"
+        },
+        "value": 72
     },
     "seventy-seven": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "77"
-        }
+            "tab": "d4"
+        },
+        "value": 77
     },
     "seventy-seventh": {
         "A": {
-            "tab": "a1",
-            "value": 77
-        }
+            "tab": "a1"
+        },
+        "value": 77
     },
     "seventy-six": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": "76"
-        }
+            "tab": "d4"
+        },
+        "value": 76
     },
     "seventy-sixth": {
         "A": {
-            "tab": "a1",
-            "value": 76
-        }
+            "tab": "a1"
+        },
+        "value": 76
     },
     "seventy-third": {
         "A": {
-            "tab": "a1",
-            "value": 73
-        }
+            "tab": "a1"
+        },
+        "value": 73
     },
     "seventy-three": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 73
-        }
+            "tab": "d4"
+        },
+        "value": 73
     },
     "seventy-two": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 72
-        }
+            "tab": "d4"
+        },
+        "value": 72
     },
     "sever": {
         "V": {
             "tab": "v1"
         }
     },
     "several": {
@@ -151271,15 +151279,15 @@
         }
     },
     "show": {
         "N": {
             "tab": "n1"
         },
         "V": {
-            "tab": "v57"
+            "tab": "v90"
         },
         "basic": true
     },
     "show-biz": {
         "N": {
             "tab": "n5"
         }
@@ -152917,20 +152925,20 @@
             "tab": "n1"
         },
         "basic": true
     },
     "six": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 6
+            "tab": "d4"
         },
         "N": {
             "tab": "n2"
-        }
+        },
+        "value": 6
     },
     "six-footer": {
         "N": {
             "tab": "n1"
         }
     },
     "six-shooter": {
@@ -152955,184 +152963,184 @@
         "A": {
             "tab": "a1"
         }
     },
     "sixteen": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 16
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 16
     },
     "sixteenth": {
         "A": {
-            "tab": "a1",
-            "value": 16
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 16
     },
     "sixth": {
         "A": {
-            "tab": "a1",
-            "value": 6
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 6
     },
     "sixth-former": {
         "N": {
             "tab": "n1"
         }
     },
     "sixthly": {
         "Adv": {
             "tab": "b1"
         }
     },
     "sixtieth": {
         "A": {
-            "tab": "a1",
-            "value": 60
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 60
     },
     "sixty": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 60
+            "tab": "d4"
         },
         "N": {
             "tab": "n3"
-        }
+        },
+        "value": 60
     },
     "sixty-eight": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 68
-        }
+            "tab": "d4"
+        },
+        "value": 68
     },
     "sixty-eighth": {
         "A": {
-            "tab": "a1",
-            "value": 68
-        }
+            "tab": "a1"
+        },
+        "value": 68
     },
     "sixty-fifth": {
         "A": {
-            "tab": "a1",
-            "value": 65
-        }
+            "tab": "a1"
+        },
+        "value": 65
     },
     "sixty-first": {
         "A": {
-            "tab": "a1",
-            "value": 61
-        }
+            "tab": "a1"
+        },
+        "value": 61
     },
     "sixty-five": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 65
-        }
+            "tab": "d4"
+        },
+        "value": 65
     },
     "sixty-four": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 64
-        }
+            "tab": "d4"
+        },
+        "value": 64
     },
     "sixty-fourth": {
         "A": {
-            "tab": "a1",
-            "value": 64
-        }
+            "tab": "a1"
+        },
+        "value": 64
     },
     "sixty-nine": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 69
-        }
+            "tab": "d4"
+        },
+        "value": 69
     },
     "sixty-ninth": {
         "A": {
-            "tab": "a1",
-            "value": 69
-        }
+            "tab": "a1"
+        },
+        "value": 69
     },
     "sixty-one": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 61
-        }
+            "tab": "d4"
+        },
+        "value": 61
     },
     "sixty-second": {
         "A": {
-            "tab": "a1",
-            "value": 62
-        }
+            "tab": "a1"
+        },
+        "value": 62
     },
     "sixty-seven": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 67
-        }
+            "tab": "d4"
+        },
+        "value": 67
     },
     "sixty-seventh": {
         "A": {
-            "tab": "a1",
-            "value": 67
-        }
+            "tab": "a1"
+        },
+        "value": 67
     },
     "sixty-six": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 66
-        }
+            "tab": "d4"
+        },
+        "value": 66
     },
     "sixty-sixth": {
         "A": {
-            "tab": "a1",
-            "value": 66
-        }
+            "tab": "a1"
+        },
+        "value": 66
     },
     "sixty-third": {
         "A": {
-            "tab": "a1",
-            "value": 63
-        }
+            "tab": "a1"
+        },
+        "value": 63
     },
     "sixty-three": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 63
-        }
+            "tab": "d4"
+        },
+        "value": 63
     },
     "sixty-two": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 62
-        }
+            "tab": "d4"
+        },
+        "value": 62
     },
     "sizable": {
         "A": {
             "tab": "a1"
         }
     },
     "size": {
@@ -169126,20 +169134,20 @@
         "N": {
             "tab": "n2"
         }
     },
     "ten": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 10
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 10
     },
     "tenability": {
         "N": {
             "tab": "n5"
         }
     },
     "tenable": {
@@ -169393,20 +169401,20 @@
     "tenterhook": {
         "N": {
             "tab": "n1"
         }
     },
     "tenth": {
         "A": {
-            "tab": "a1",
-            "value": 10
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 10
     },
     "tenthly": {
         "Adv": {
             "tab": "b1"
         }
     },
     "tenuity": {
@@ -170502,20 +170510,20 @@
     "thinness": {
         "N": {
             "tab": "n5"
         }
     },
     "third": {
         "A": {
-            "tab": "a1",
-            "value": 3
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 3
     },
     "third-rate": {
         "A": {
             "tab": "a1"
         }
     },
     "third-rater": {
@@ -170545,165 +170553,165 @@
         "A": {
             "tab": "a4"
         }
     },
     "thirteen": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 13
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 13
     },
     "thirteenth": {
         "A": {
-            "tab": "a1",
-            "value": 13
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 13
     },
     "thirtieth": {
         "A": {
-            "tab": "a1",
-            "value": 30
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 30
     },
     "thirty": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 30
+            "tab": "d4"
         },
         "N": {
             "tab": "n3"
-        }
+        },
+        "value": 30
     },
     "thirty-eight": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 38
-        }
+            "tab": "d4"
+        },
+        "value": 38
     },
     "thirty-eighth": {
         "A": {
-            "tab": "a1",
-            "value": 38
-        }
+            "tab": "a1"
+        },
+        "value": 38
     },
     "thirty-fifth": {
         "A": {
-            "tab": "a1",
-            "value": 35
-        }
+            "tab": "a1"
+        },
+        "value": 35
     },
     "thirty-first": {
         "A": {
-            "tab": "a1",
-            "value": 31
-        }
+            "tab": "a1"
+        },
+        "value": 31
     },
     "thirty-five": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 35
-        }
+            "tab": "d4"
+        },
+        "value": 35
     },
     "thirty-four": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 34
-        }
+            "tab": "d4"
+        },
+        "value": 34
     },
     "thirty-fourth": {
         "A": {
-            "tab": "a1",
-            "value": 34
-        }
+            "tab": "a1"
+        },
+        "value": 34
     },
     "thirty-nine": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 39
-        }
+            "tab": "d4"
+        },
+        "value": 39
     },
     "thirty-ninth": {
         "A": {
-            "tab": "a1",
-            "value": 39
-        }
+            "tab": "a1"
+        },
+        "value": 39
     },
     "thirty-one": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 31
-        }
+            "tab": "d4"
+        },
+        "value": 31
     },
     "thirty-second": {
         "A": {
-            "tab": "a1",
-            "value": 32
-        }
+            "tab": "a1"
+        },
+        "value": 32
     },
     "thirty-seven": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 37
-        }
+            "tab": "d4"
+        },
+        "value": 37
     },
     "thirty-seventh": {
         "A": {
-            "tab": "a1",
-            "value": 37
-        }
+            "tab": "a1"
+        },
+        "value": 37
     },
     "thirty-six": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 36
-        }
+            "tab": "d4"
+        },
+        "value": 36
     },
     "thirty-sixth": {
         "A": {
-            "tab": "a1",
-            "value": 36
-        }
+            "tab": "a1"
+        },
+        "value": 36
     },
     "thirty-third": {
         "A": {
-            "tab": "a1",
-            "value": 33
-        }
+            "tab": "a1"
+        },
+        "value": 33
     },
     "thirty-three": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 33
-        }
+            "tab": "d4"
+        },
+        "value": 33
     },
     "thirty-two": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 32
-        }
+            "tab": "d4"
+        },
+        "value": 32
     },
     "this": {
         "Adv": {
             "tab": "b1"
         },
         "D": {
             "tab": "d5"
@@ -170842,37 +170850,37 @@
         "N": {
             "tab": "n5"
         }
     },
     "thousand": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 1000
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 1000
     },
     "thousandfold": {
         "A": {
             "tab": "a1"
         },
         "Adv": {
             "tab": "b1"
         }
     },
     "thousandth": {
         "A": {
-            "tab": "a1",
-            "value": 1000
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 1000
     },
     "thraldom": {
         "N": {
             "tab": "n5"
         }
     },
     "thrall": {
@@ -170925,20 +170933,20 @@
         "Adv": {
             "tab": "b1"
         }
     },
     "three": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 3
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 3
     },
     "three-D": {
         "A": {
             "tab": "a1"
         },
         "N": {
             "tab": "n5"
@@ -176786,176 +176794,176 @@
     "tweezers": {
         "N": {
             "tab": "n6"
         }
     },
     "twelfth": {
         "A": {
-            "tab": "a1",
-            "value": 12
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 12
     },
     "twelfthly": {
         "Adv": {
             "tab": "b1"
         }
     },
     "twelve": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 12
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 12
     },
     "twelvemonth": {
         "N": {
             "tab": "n1"
         }
     },
     "twentieth": {
         "A": {
-            "tab": "a1",
-            "value": 20
+            "tab": "a1"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 20
     },
     "twenty": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 20
+            "tab": "d4"
         },
         "N": {
             "tab": "n3"
-        }
+        },
+        "value": 20
     },
     "twenty-eight": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 28
-        }
+            "tab": "d4"
+        },
+        "value": 28
     },
     "twenty-eighth": {
         "A": {
-            "tab": "a1",
-            "value": 28
-        }
+            "tab": "a1"
+        },
+        "value": 28
     },
     "twenty-fifth": {
         "A": {
-            "tab": "a1",
-            "value": 25
-        }
+            "tab": "a1"
+        },
+        "value": 25
     },
     "twenty-first": {
         "A": {
-            "tab": "a1",
-            "value": 21
-        }
+            "tab": "a1"
+        },
+        "value": 21
     },
     "twenty-five": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 25
-        }
+            "tab": "d4"
+        },
+        "value": 25
     },
     "twenty-four": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 24
-        }
+            "tab": "d4"
+        },
+        "value": 24
     },
     "twenty-fourth": {
         "A": {
-            "tab": "a1",
-            "value": 24
-        }
+            "tab": "a1"
+        },
+        "value": 24
     },
     "twenty-nine": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 29
-        }
+            "tab": "d4"
+        },
+        "value": 29
     },
     "twenty-ninth": {
         "A": {
-            "tab": "a1",
-            "value": 29
-        }
+            "tab": "a1"
+        },
+        "value": 29
     },
     "twenty-one": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 21
-        }
+            "tab": "d4"
+        },
+        "value": 21
     },
     "twenty-second": {
         "A": {
-            "tab": "a1",
-            "value": 22
-        }
+            "tab": "a1"
+        },
+        "value": 22
     },
     "twenty-seven": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 27
-        }
+            "tab": "d4"
+        },
+        "value": 27
     },
     "twenty-seventh": {
         "A": {
-            "tab": "a1",
-            "value": 27
-        }
+            "tab": "a1"
+        },
+        "value": 27
     },
     "twenty-six": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 26
-        }
+            "tab": "d4"
+        },
+        "value": 26
     },
     "twenty-sixth": {
         "A": {
-            "tab": "a1",
-            "value": 26
-        }
+            "tab": "a1"
+        },
+        "value": 26
     },
     "twenty-third": {
         "A": {
-            "tab": "a1",
-            "value": 23
-        }
+            "tab": "a1"
+        },
+        "value": 23
     },
     "twenty-three": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 23
-        }
+            "tab": "d4"
+        },
+        "value": 23
     },
     "twenty-two": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 22
-        }
+            "tab": "d4"
+        },
+        "value": 22
     },
     "twerp": {
         "N": {
             "tab": "n1"
         }
     },
     "twice": {
@@ -177099,20 +177107,20 @@
         "V": {
             "tab": "v1"
         }
     },
     "two": {
         "D": {
             "n": "p",
-            "tab": "d4",
-            "value": 2
+            "tab": "d4"
         },
         "N": {
             "tab": "n1"
-        }
+        },
+        "value": 2
     },
     "two-a-penny": {
         "A": {
             "tab": "a1"
         }
     },
     "two-edged": {
@@ -189993,15 +190001,16 @@
     "zero": {
         "N": {
             "tab": "n1"
         },
         "V": {
             "tab": "v1"
         },
-        "basic": true
+        "basic": true,
+        "value": 0
     },
     "zest": {
         "N": {
             "tab": "n5"
         }
     },
     "zestfully": {
```

### Comparing `pyrealb-2.3.4/src/pyrealb/data/lexicon-fr.json` & `pyrealb-2.3.5/src/pyrealb/data/lexicon-fr.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994617057980392%*

 * *Differences: {"'cent'": "{'value': 100}",*

 * * "'centième'": "{'value': 100}",*

 * * "'cinq'": "{'value': 5}",*

 * * "'cinquante'": "{'value': 50}",*

 * * "'cinquante-cinq'": "{'value': 55}",*

 * * "'cinquante-deux'": "{'value': 52}",*

 * * "'cinquante-huit'": "{'value': 58}",*

 * * "'cinquante-neuf'": "{'value': 59}",*

 * * "'cinquante-quatre'": "{'value': 54}",*

 * * "'cinquante-sept'": "{'value': 57}",*

 * * "'cinquante-six'": "{'value': 56}",*

 * * "'cinquante-trois'": "{'value': 53}",*

 * * "'cinquième'": "{'value': 5}",*

 * * "'deux'": "{'value': 2}",*

 * * "'deuxième'": "{'value': […]*

```diff
@@ -53895,15 +53895,16 @@
     "cent": {
         "Adv": {
             "tab": "av"
         },
         "N": {
             "g": "m",
             "tab": "n3"
-        }
+        },
+        "value": 100
     },
     "cent-garde": {
         "N": {
             "g": "m",
             "tab": "n3"
         }
     },
@@ -54011,15 +54012,16 @@
         },
         "basic": true
     },
     "centi\u00e8me": {
         "N": {
             "g": "m",
             "tab": "n3"
-        }
+        },
+        "value": 100
     },
     "centrage": {
         "N": {
             "g": "m",
             "tab": "n3"
         }
     },
@@ -60301,66 +60303,76 @@
         "A": {
             "tab": "n24"
         }
     },
     "cinq": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 5
     },
     "cinquantaine": {
         "N": {
             "g": "f",
             "tab": "n17"
         }
     },
     "cinquante": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 50
     },
     "cinquante-cinq": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 55
     },
     "cinquante-deux": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 52
     },
     "cinquante-huit": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 58
     },
     "cinquante-neuf": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 59
     },
     "cinquante-quatre": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 54
     },
     "cinquante-sept": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 57
     },
     "cinquante-six": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 56
     },
     "cinquante-trois": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 53
     },
     "cinquantenaire": {
         "A": {
             "tab": "n25"
         },
         "N": {
             "g": "x",
@@ -60371,15 +60383,16 @@
         "A": {
             "pos": "pre",
             "tab": "n25"
         },
         "N": {
             "g": "x",
             "tab": "n17"
-        }
+        },
+        "value": 5
     },
     "cinqui\u00e8mement": {
         "Adv": {
             "tab": "av"
         }
     },
     "cintrage": {
@@ -85074,15 +85087,16 @@
             "g": "m",
             "tab": "n3"
         }
     },
     "deux": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 2
     },
     "deux-huit": {
         "N": {
             "g": "m",
             "tab": "n2"
         }
     },
@@ -85144,15 +85158,16 @@
         "A": {
             "pos": "pre",
             "tab": "n25"
         },
         "N": {
             "g": "x",
             "tab": "n17"
-        }
+        },
+        "value": 2
     },
     "deuxi\u00e8mement": {
         "Adv": {
             "tab": "av"
         }
     },
     "deuzio": {
@@ -89328,40 +89343,45 @@
             "g": "f",
             "tab": "n17"
         }
     },
     "dix": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 10
     },
     "dix-huit": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 18
     },
     "dix-neuf": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 19
     },
     "dix-sept": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 17
     },
     "dixi\u00e8me": {
         "A": {
             "pos": "pre",
             "tab": "n25"
         },
         "N": {
             "g": "x",
             "tab": "n17"
-        }
+        },
+        "value": 10
     },
     "dixi\u00e8mement": {
         "Adv": {
             "tab": "av"
         }
     },
     "dizain": {
@@ -91005,15 +91025,16 @@
             "tab": "n17"
         },
         "basic": true
     },
     "douze": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 12
     },
     "douzi\u00e8mement": {
         "Adv": {
             "tab": "av"
         }
     },
     "dou\u00e7ain": {
@@ -115358,14 +115379,20 @@
             "aux": "av",
             "pat": [
                 "tdir"
             ],
             "tab": "v5"
         }
     },
+    "ennuagement": {
+        "N": {
+            "g": "m",
+            "tab": "n3"
+        }
+    },
     "ennuager": {
         "V": {
             "aux": "av",
             "pat": [
                 "tdir",
                 "r\u00e9fl"
             ],
@@ -154284,15 +154311,16 @@
             "tab": "n3"
         }
     },
     "huit": {
         "Adv": {
             "h": 1,
             "tab": "av"
-        }
+        },
+        "value": 8
     },
     "huit-reflets": {
         "N": {
             "g": "m",
             "tab": "n2"
         }
     },
@@ -154315,15 +154343,16 @@
             "h": 1,
             "pos": "pre",
             "tab": "n25"
         },
         "N": {
             "g": "x",
             "tab": "n17"
-        }
+        },
+        "value": 8
     },
     "huiti\u00e8mement": {
         "Adv": {
             "tab": "av"
         }
     },
     "hulotte": {
@@ -196077,15 +196106,16 @@
     "mille": {
         "Adv": {
             "tab": "av"
         },
         "N": {
             "g": "m",
             "tab": "n3"
-        }
+        },
+        "value": 1000
     },
     "mille-feuille": {
         "N": {
             "g": "f",
             "tab": "n17"
         }
     },
@@ -196151,15 +196181,16 @@
             "tab": "n3"
         }
     },
     "milliard": {
         "N": {
             "g": "m",
             "tab": "n3"
-        }
+        },
+        "value": 1000000000
     },
     "milliardaire": {
         "A": {
             "tab": "n25"
         },
         "N": {
             "g": "x",
@@ -196220,15 +196251,16 @@
         }
     },
     "million": {
         "N": {
             "g": "m",
             "tab": "n3"
         },
-        "basic": true
+        "basic": true,
+        "value": 1000000
     },
     "millionnaire": {
         "A": {
             "tab": "n25"
         },
         "N": {
             "g": "x",
@@ -208527,15 +208559,16 @@
     "neuf": {
         "A": {
             "tab": "n46"
         },
         "Adv": {
             "tab": "av"
         },
-        "basic": true
+        "basic": true,
+        "value": 9
     },
     "neufchatel": {
         "N": {
             "g": "m",
             "tab": "n3"
         }
     },
@@ -208819,15 +208852,16 @@
         "A": {
             "pos": "pre",
             "tab": "n25"
         },
         "N": {
             "g": "x",
             "tab": "n17"
-        }
+        },
+        "value": 9
     },
     "neuvi\u00e8mement": {
         "Adv": {
             "tab": "av"
         }
     },
     "neveu": {
@@ -216183,15 +216217,16 @@
             "g": "m",
             "tab": "n3"
         }
     },
     "onze": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 11
     },
     "onzi\u00e8mement": {
         "Adv": {
             "tab": "av"
         }
     },
     "on\u00e9reusement": {
@@ -242962,15 +242997,16 @@
             "pos": "pre",
             "tab": "n39"
         },
         "N": {
             "g": "x",
             "tab": "n39"
         },
-        "basic": true
+        "basic": true,
+        "value": 1
     },
     "premier-Paris": {
         "N": {
             "g": "m",
             "tab": "nI"
         }
     },
@@ -254440,64 +254476,73 @@
             "g": "f",
             "tab": "n17"
         }
     },
     "quarante": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 40
     },
     "quarante-cinq": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 45
     },
     "quarante-deux": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 42
     },
     "quarante-huit": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 48
     },
     "quarante-huitard": {
         "A": {
             "tab": "n28"
         },
         "N": {
             "g": "x",
             "tab": "n28"
         }
     },
     "quarante-neuf": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 49
     },
     "quarante-quatre": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 44
     },
     "quarante-sept": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 47
     },
     "quarante-six": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 46
     },
     "quarante-trois": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 43
     },
     "quarantenaire": {
         "A": {
             "tab": "n25"
         },
         "N": {
             "g": "m",
@@ -254758,15 +254803,16 @@
             "g": "m",
             "tab": "n3"
         }
     },
     "quatorze": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 14
     },
     "quatorzi\u00e8mement": {
         "Adv": {
             "tab": "av"
         }
     },
     "quatrain": {
@@ -254774,15 +254820,16 @@
             "g": "m",
             "tab": "n3"
         }
     },
     "quatre": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 4
     },
     "quatre-cent-vingt-et-un": {
         "N": {
             "g": "m",
             "tab": "n2"
         }
     },
@@ -254830,114 +254877,133 @@
     },
     "quatre-temps": {
         "N": {
             "g": "m",
             "tab": "n1"
         }
     },
-    "quatre-vingt": {
-        "Adv": {
-            "tab": "av"
-        }
-    },
     "quatre-vingt-cinq": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 85
     },
     "quatre-vingt-deux": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 82
     },
     "quatre-vingt-dix": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 90
     },
     "quatre-vingt-dix-huit": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 98
     },
     "quatre-vingt-dix-neuf": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 99
     },
     "quatre-vingt-dix-sept": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 97
     },
     "quatre-vingt-douze": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 92
     },
     "quatre-vingt-et-un": {
         "N": {
             "g": "m",
             "tab": "n2"
         }
     },
     "quatre-vingt-huit": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 88
     },
     "quatre-vingt-neuf": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 89
     },
     "quatre-vingt-onze": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 91
     },
     "quatre-vingt-quatorze": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 94
     },
     "quatre-vingt-quatre": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 84
     },
     "quatre-vingt-quinze": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 95
     },
     "quatre-vingt-seize": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 96
     },
     "quatre-vingt-sept": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 87
     },
     "quatre-vingt-six": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 86
     },
     "quatre-vingt-treize": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 93
     },
     "quatre-vingt-trois": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 83
+    },
+    "quatre-vingts": {
+        "Adv": {
+            "tab": "av"
+        },
+        "value": 80
     },
     "quatre-\u00e9pices": {
         "N": {
             "g": "m",
             "tab": "n2"
         }
     },
@@ -254951,15 +255017,16 @@
         "A": {
             "pos": "pre",
             "tab": "n25"
         },
         "N": {
             "g": "x",
             "tab": "n17"
-        }
+        },
+        "value": 4
     },
     "quatri\u00e8mement": {
         "Adv": {
             "tab": "av"
         }
     },
     "quatuor": {
@@ -255476,15 +255543,16 @@
             "tab": "n17"
         },
         "basic": true
     },
     "quinze": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 15
     },
     "quinzi\u00e8mement": {
         "Adv": {
             "tab": "av"
         }
     },
     "quin\u00e9": {
@@ -285786,15 +285854,16 @@
             "g": "f",
             "tab": "n17"
         }
     },
     "seize": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 16
     },
     "seizi\u00e8mement": {
         "Adv": {
             "tab": "av"
         }
     },
     "seizi\u00e9misme": {
@@ -286620,15 +286689,16 @@
             "g": "m",
             "tab": "n2"
         }
     },
     "sept": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 7
     },
     "septain": {
         "N": {
             "g": "m",
             "tab": "n3"
         }
     },
@@ -286733,15 +286803,16 @@
         "A": {
             "pos": "pre",
             "tab": "n25"
         },
         "N": {
             "g": "x",
             "tab": "n17"
-        }
+        },
+        "value": 7
     },
     "septi\u00e8mement": {
         "Adv": {
             "tab": "av"
         }
     },
     "septmoncel": {
@@ -289332,15 +289403,16 @@
             "g": "m",
             "tab": "n3"
         }
     },
     "six": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 6
     },
     "six-huit": {
         "N": {
             "g": "m",
             "tab": "n2"
         }
     },
@@ -289348,15 +289420,16 @@
         "A": {
             "pos": "pre",
             "tab": "n25"
         },
         "N": {
             "g": "x",
             "tab": "n17"
-        }
+        },
+        "value": 6
     },
     "sixi\u00e8mement": {
         "Adv": {
             "tab": "av"
         }
     },
     "sixte": {
@@ -290087,100 +290160,118 @@
             "g": "f",
             "tab": "n17"
         }
     },
     "soixante": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 60
     },
     "soixante-cinq": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 65
     },
     "soixante-deux": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 62
     },
     "soixante-dix": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 70
     },
     "soixante-dix-huit": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 78
     },
     "soixante-dix-neuf": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 79
     },
     "soixante-dix-sept": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 77
     },
     "soixante-douze": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 72
     },
     "soixante-huit": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 68
     },
     "soixante-neuf": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 69
     },
     "soixante-quatorze": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 74
     },
     "soixante-quatre": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 64
     },
     "soixante-quinze": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 75
     },
     "soixante-seize": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 76
     },
     "soixante-sept": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 67
     },
     "soixante-six": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 66
     },
     "soixante-treize": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 73
     },
     "soixante-trois": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 63
     },
     "soja": {
         "N": {
             "g": "m",
             "tab": "n3"
         }
     },
@@ -316891,15 +316982,16 @@
             ],
             "tab": "v36"
         }
     },
     "treize": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 13
     },
     "treiziste": {
         "N": {
             "g": "m",
             "tab": "n3"
         }
     },
@@ -317073,65 +317165,74 @@
             "g": "f",
             "tab": "n17"
         }
     },
     "trente": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 30
     },
     "trente-cinq": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 35
     },
     "trente-deux": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 32
     },
     "trente-et-quarante": {
         "N": {
             "g": "m",
             "tab": "n2"
         }
     },
     "trente-huit": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 38
     },
     "trente-neuf": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 39
     },
     "trente-quatre": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 34
     },
     "trente-sept": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 37
     },
     "trente-six": {
         "Adv": {
             "tab": "av"
         },
         "N": {
             "g": "m",
             "tab": "n35"
-        }
+        },
+        "value": 36
     },
     "trente-trois": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 33
     },
     "trentenaire": {
         "A": {
             "tab": "n25"
         }
     },
     "trescheur": {
@@ -318942,15 +319043,16 @@
             "g": "m",
             "tab": "n3"
         }
     },
     "trois": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 3
     },
     "trois-deux": {
         "N": {
             "g": "m",
             "tab": "n2"
         }
     },
@@ -318999,15 +319101,16 @@
         "A": {
             "pos": "pre",
             "tab": "n25"
         },
         "N": {
             "g": "x",
             "tab": "n17"
-        }
+        },
+        "value": 3
     },
     "troisi\u00e8mement": {
         "Adv": {
             "tab": "av"
         }
     },
     "troll": {
@@ -323736,15 +323839,16 @@
     "un": {
         "D": {
             "tab": "d4"
         },
         "Pro": {
             "tab": "n27"
         },
-        "basic": true
+        "basic": true,
+        "value": 1
     },
     "unanime": {
         "A": {
             "tab": "n25"
         }
     },
     "unanimement": {
@@ -329913,55 +330017,64 @@
         "A": {
             "tab": "n54"
         }
     },
     "vingt": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 20
     },
     "vingt-cinq": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 25
     },
     "vingt-deux": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 22
     },
     "vingt-huit": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 28
     },
     "vingt-neuf": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 29
     },
     "vingt-quatre": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 24
     },
     "vingt-sept": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 27
     },
     "vingt-six": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 26
     },
     "vingt-trois": {
         "Adv": {
             "tab": "av"
-        }
+        },
+        "value": 23
     },
     "vingtaine": {
         "N": {
             "g": "f",
             "tab": "n17"
         }
     },
@@ -335191,15 +335304,16 @@
             "tab": "n17"
         }
     },
     "z\u00e9ro": {
         "N": {
             "g": "m",
             "tab": "n3"
-        }
+        },
+        "value": 0
     },
     "z\u00e9rotage": {
         "N": {
             "g": "m",
             "tab": "n3"
         }
     },
```

### Comparing `pyrealb-2.3.4/src/pyrealb/data/pyrealb.egg-info/PKG-INFO` & `pyrealb-2.3.5/src/pyrealb/data/pyrealb.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.4/src/pyrealb/data/rules-en.json` & `pyrealb-2.3.5/src/pyrealb/data/rules-en.json`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.4/src/pyrealb/data/rules-fr.json` & `pyrealb-2.3.5/src/pyrealb/data/rules-fr.json`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.4/src/pyrealb/utils.py` & `pyrealb-2.3.5/src/pyrealb/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,9 +71,9 @@
 
 # useful variables for using expressions written originally for the javascript version
 false = False
 true = True
 null = None
 
 # version and date informations
-pyrealb_version = "2.3.4"
+pyrealb_version = "2.3.5"
 pyrealb_datecreated = datetime.datetime.today()
```

### Comparing `pyrealb-2.3.4/src/pyrealb.egg-info/PKG-INFO` & `pyrealb-2.3.5/src/pyrealb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyrealb
-Version: 2.3.4
+Version: 2.3.5
 Summary: A French-English text realizer
 Home-page: https://github.com/lapalme/pyrealb
 Author: Guy Lapalme
 Author-email: lapalme@iro.umontreal.ca
 Project-URL: Bug Tracker, https://github.com/lapalme/pyrealb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # *pyRealB* - A Python Bilingual Text Realizer
 
-*Version 2.3.4 - May 2023*
+*Version 2.3.5 - May 2023*
 
 *pyRealB* is a Python adaptation of the JavaScript [**jsRealB**](http://rali.iro.umontreal.ca/jsRealB) 
 text realizer with the same constituent and dependency syntax notation. 
 It facilitates its integration within Python applications by simply adding
 
 	from pyrealb import *
```

### Comparing `pyrealb-2.3.4/src/pyrealb.egg-info/SOURCES.txt` & `pyrealb-2.3.5/src/pyrealb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.4/tests/test.py` & `pyrealb-2.3.5/tests/test.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.4/tests/testAll.py` & `pyrealb-2.3.5/tests/testAll.py`

 * *Files identical despite different names*

