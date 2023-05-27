# Comparing `tmp/finddd-0.2.0.tar.gz` & `tmp/finddd-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finddd-0.2.0.tar", last modified: Fri May 26 21:46:10 2023, max compression
+gzip compressed data, was "finddd-0.2.1.tar", last modified: Sat May 27 14:40:40 2023, max compression
```

## Comparing `finddd-0.2.0.tar` & `finddd-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      192 2023-05-26 21:37:40.678372 finddd-0.2.0/README.md
--rw-r--r--   0        0        0      436 2023-05-26 21:46:10.467428 finddd-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       80 2023-05-23 16:46:41.626983 finddd-0.2.0/src/finddd/__init__.py
--rw-r--r--   0        0        0      183 2023-05-24 07:49:06.111382 finddd-0.2.0/src/finddd/const.py
--rw-r--r--   0        0        0     3379 2023-05-24 18:24:11.411402 finddd-0.2.0/src/finddd/find.py
--rw-r--r--   0        0        0     9571 2023-05-26 21:28:44.039733 finddd-0.2.0/src/finddd/match.py
--rw-r--r--   0        0        0        0 2023-05-23 18:15:54.195230 finddd-0.2.0/src/finddd/py.typed
--rw-r--r--   0        0        0      190 2023-05-26 21:44:14.370483 finddd-0.2.0/src/finddd/test_find.py
--rw-r--r--   0        0        0     6373 2023-05-26 21:44:14.492275 finddd-0.2.0/src/finddd/test_match.py
--rw-r--r--   0        0        0      383 1970-01-01 00:00:00.000000 finddd-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      192 2023-05-26 21:37:40.678372 finddd-0.2.1/README.md
+-rw-r--r--   0        0        0      436 2023-05-27 14:40:40.019614 finddd-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-05-23 16:46:41.626983 finddd-0.2.1/src/finddd/__init__.py
+-rw-r--r--   0        0        0      183 2023-05-24 07:49:06.111382 finddd-0.2.1/src/finddd/const.py
+-rw-r--r--   0        0        0     3379 2023-05-27 14:37:27.751186 finddd-0.2.1/src/finddd/find.py
+-rw-r--r--   0        0        0     9571 2023-05-26 21:28:44.039733 finddd-0.2.1/src/finddd/match.py
+-rw-r--r--   0        0        0        0 2023-05-23 18:15:54.195230 finddd-0.2.1/src/finddd/py.typed
+-rw-r--r--   0        0        0      190 2023-05-26 21:44:14.370483 finddd-0.2.1/src/finddd/test_find.py
+-rw-r--r--   0        0        0     6373 2023-05-26 21:44:14.492275 finddd-0.2.1/src/finddd/test_match.py
+-rw-r--r--   0        0        0      383 1970-01-01 00:00:00.000000 finddd-0.2.1/PKG-INFO
```

### Comparing `finddd-0.2.0/src/finddd/find.py` & `finddd-0.2.1/src/finddd/find.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,17 +78,17 @@
                 within=depth_within,
             )
         )
         cmm.add(
             ChangeTimeMatcher(older=time_older, newer=time_newer, within=time_within)
         )
         cmm.add(FilenameMather(pattern, ignore_case=self.ignore_case))
+        cmm.add(SuffixMatcher(*suffixes))
 
         fmm.add(SizeMatcher(min=size_min, max=size_max, within=size_within))
-        fmm.add(SuffixMatcher(*suffixes))
 
         # add MaxResultMatcher last
         mrm = MaxResultMatcher(max_result)
         fmm.add(cmm, mrm, post_matcher)
         dmm.add(cmm, mrm, post_matcher)
 
         def g(cwd: str, l: list[str], m: Matcher):
```

### Comparing `finddd-0.2.0/src/finddd/match.py` & `finddd-0.2.1/src/finddd/match.py`

 * *Files identical despite different names*

### Comparing `finddd-0.2.0/src/finddd/test_match.py` & `finddd-0.2.1/src/finddd/test_match.py`

 * *Files identical despite different names*

