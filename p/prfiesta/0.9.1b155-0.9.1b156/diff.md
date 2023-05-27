# Comparing `tmp/prfiesta-0.9.1b155.tar.gz` & `tmp/prfiesta-0.9.1b156.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prfiesta-0.9.1b155.tar", max compression
+gzip compressed data, was "prfiesta-0.9.1b156.tar", max compression
```

## Comparing `prfiesta-0.9.1b155.tar` & `prfiesta-0.9.1b156.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2023-05-27 15:06:13.760800 prfiesta-0.9.1b155/LICENSE
--rw-r--r--   0        0        0    10180 2023-05-27 15:06:13.760800 prfiesta-0.9.1b155/README.md
--rw-r--r--   0        0        0      487 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/__init__.py
--rw-r--r--   0        0        0     3799 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/__main__.py
--rw-r--r--   0        0        0        0 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/analysis/__init__.py
--rw-r--r--   0        0        0     4729 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/analysis/plot.py
--rw-r--r--   0        0        0     1007 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/analysis/view.py
--rw-r--r--   0        0        0        0 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/collectors/__init__.py
--rw-r--r--   0        0        0     5929 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/collectors/github.py
--rw-r--r--   0        0        0      571 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/environment.py
--rw-r--r--   0        0        0      975 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/output.py
--rw-r--r--   0        0        0      275 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/spinner.py
--rw-r--r--   0        0        0     3203 2023-05-27 15:06:24.108863 prfiesta-0.9.1b155/pyproject.toml
--rw-r--r--   0        0        0    11586 1970-01-01 00:00:00.000000 prfiesta-0.9.1b155/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-27 15:09:17.703800 prfiesta-0.9.1b156/LICENSE
+-rw-r--r--   0        0        0    10189 2023-05-27 15:09:17.703800 prfiesta-0.9.1b156/README.md
+-rw-r--r--   0        0        0      487 2023-05-27 15:09:17.711800 prfiesta-0.9.1b156/prfiesta/__init__.py
+-rw-r--r--   0        0        0     3799 2023-05-27 15:09:17.711800 prfiesta-0.9.1b156/prfiesta/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-27 15:09:17.711800 prfiesta-0.9.1b156/prfiesta/analysis/__init__.py
+-rw-r--r--   0        0        0     4729 2023-05-27 15:09:17.711800 prfiesta-0.9.1b156/prfiesta/analysis/plot.py
+-rw-r--r--   0        0        0     1007 2023-05-27 15:09:17.711800 prfiesta-0.9.1b156/prfiesta/analysis/view.py
+-rw-r--r--   0        0        0        0 2023-05-27 15:09:17.711800 prfiesta-0.9.1b156/prfiesta/collectors/__init__.py
+-rw-r--r--   0        0        0     5929 2023-05-27 15:09:17.711800 prfiesta-0.9.1b156/prfiesta/collectors/github.py
+-rw-r--r--   0        0        0      571 2023-05-27 15:09:17.711800 prfiesta-0.9.1b156/prfiesta/environment.py
+-rw-r--r--   0        0        0      975 2023-05-27 15:09:17.711800 prfiesta-0.9.1b156/prfiesta/output.py
+-rw-r--r--   0        0        0      275 2023-05-27 15:09:17.711800 prfiesta-0.9.1b156/prfiesta/spinner.py
+-rw-r--r--   0        0        0     3203 2023-05-27 15:09:26.724416 prfiesta-0.9.1b156/pyproject.toml
+-rw-r--r--   0        0        0    11595 1970-01-01 00:00:00.000000 prfiesta-0.9.1b156/PKG-INFO
```

### Comparing `prfiesta-0.9.1b155/LICENSE` & `prfiesta-0.9.1b156/LICENSE`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b155/README.md` & `prfiesta-0.9.1b156/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
 Learn more about searching review requests [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-pull-request-review-status-and-reviewer)
 
 ### Date Filter
 
 When using the `--after` and `--before` date filters, by default `prfiesta` will use the `created` date dimension with these filters on the Git provider (e.g GitHub). This may not fit your use case and you may want to filter on when a pull request was updated instead. To do this you can use the `--use-updated` flag.
 
-See more information [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-when-an-issue-or-pull-request-was-created-or-last-updated).
+Learn more about date filters [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-when-an-issue-or-pull-request-was-created-or-last-updated).
 
 ## Analysis
 
 `prfiesta` ships with built in plots to help analyze your pull request data. These serve as a starting point in your analysis. See more information on the build in plots and views [here](https://github.com/kiran94/prfiesta/blob/main/docs/analysis.md).
 
 ## Using GitHub Enterprise
```

### Comparing `prfiesta-0.9.1b155/prfiesta/__main__.py` & `prfiesta-0.9.1b156/prfiesta/__main__.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b155/prfiesta/analysis/plot.py` & `prfiesta-0.9.1b156/prfiesta/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b155/prfiesta/analysis/view.py` & `prfiesta-0.9.1b156/prfiesta/analysis/view.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b155/prfiesta/collectors/github.py` & `prfiesta-0.9.1b156/prfiesta/collectors/github.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b155/prfiesta/environment.py` & `prfiesta-0.9.1b156/prfiesta/environment.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b155/prfiesta/output.py` & `prfiesta-0.9.1b156/prfiesta/output.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b155/pyproject.toml` & `prfiesta-0.9.1b156/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prfiesta"
-version = "0.9.1b155"
+version = "0.9.1b156"
 description = "Collect and Analyze Individual Contributor Pull Requests"
 authors = ["kiran94"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pypi.org/project/prfiesta/"
 repository = "https://github.com/kiran94/prfiesta/pull/40"
 documentation = "https://github.com/kiran94/prfiesta/blob/main/README.md"
```

### Comparing `prfiesta-0.9.1b155/PKG-INFO` & `prfiesta-0.9.1b156/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prfiesta
-Version: 0.9.1b155
+Version: 0.9.1b156
 Summary: Collect and Analyze Individual Contributor Pull Requests
 Home-page: https://pypi.org/project/prfiesta/
 License: MIT
 Keywords: pull-request,pull-request-review,performance-review
 Author: kiran94
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
@@ -150,15 +150,15 @@
 
 Learn more about searching review requests [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-pull-request-review-status-and-reviewer)
 
 ### Date Filter
 
 When using the `--after` and `--before` date filters, by default `prfiesta` will use the `created` date dimension with these filters on the Git provider (e.g GitHub). This may not fit your use case and you may want to filter on when a pull request was updated instead. To do this you can use the `--use-updated` flag.
 
-See more information [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-when-an-issue-or-pull-request-was-created-or-last-updated).
+Learn more about date filters [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-when-an-issue-or-pull-request-was-created-or-last-updated).
 
 ## Analysis
 
 `prfiesta` ships with built in plots to help analyze your pull request data. These serve as a starting point in your analysis. See more information on the build in plots and views [here](https://github.com/kiran94/prfiesta/blob/main/docs/analysis.md).
 
 ## Using GitHub Enterprise
```

