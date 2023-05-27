# Comparing `tmp/prfiesta-0.9.1b148.tar.gz` & `tmp/prfiesta-0.9.1b149.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prfiesta-0.9.1b148.tar", max compression
+gzip compressed data, was "prfiesta-0.9.1b149.tar", max compression
```

## Comparing `prfiesta-0.9.1b148.tar` & `prfiesta-0.9.1b149.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2023-05-27 08:20:03.023018 prfiesta-0.9.1b148/LICENSE
--rw-r--r--   0        0        0     9115 2023-05-27 08:20:03.023018 prfiesta-0.9.1b148/README.md
--rw-r--r--   0        0        0      487 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/__init__.py
--rw-r--r--   0        0        0     3018 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/__main__.py
--rw-r--r--   0        0        0        0 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/analysis/__init__.py
--rw-r--r--   0        0        0     4729 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/analysis/plot.py
--rw-r--r--   0        0        0     1007 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/analysis/view.py
--rw-r--r--   0        0        0        0 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/collectors/__init__.py
--rw-r--r--   0        0        0     5344 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/collectors/github.py
--rw-r--r--   0        0        0      571 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/environment.py
--rw-r--r--   0        0        0      975 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/output.py
--rw-r--r--   0        0        0      275 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/spinner.py
--rw-r--r--   0        0        0     3179 2023-05-27 08:20:13.147527 prfiesta-0.9.1b148/pyproject.toml
--rw-r--r--   0        0        0    10476 1970-01-01 00:00:00.000000 prfiesta-0.9.1b148/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-27 08:38:42.086292 prfiesta-0.9.1b149/LICENSE
+-rw-r--r--   0        0        0     9095 2023-05-27 08:38:42.086292 prfiesta-0.9.1b149/README.md
+-rw-r--r--   0        0        0      487 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/__init__.py
+-rw-r--r--   0        0        0     3018 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/analysis/__init__.py
+-rw-r--r--   0        0        0     4729 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/analysis/plot.py
+-rw-r--r--   0        0        0     1007 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/analysis/view.py
+-rw-r--r--   0        0        0        0 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/collectors/__init__.py
+-rw-r--r--   0        0        0     5344 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/collectors/github.py
+-rw-r--r--   0        0        0      571 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/environment.py
+-rw-r--r--   0        0        0      975 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/output.py
+-rw-r--r--   0        0        0      275 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/spinner.py
+-rw-r--r--   0        0        0     3179 2023-05-27 08:38:49.834370 prfiesta-0.9.1b149/pyproject.toml
+-rw-r--r--   0        0        0    10456 1970-01-01 00:00:00.000000 prfiesta-0.9.1b149/PKG-INFO
```

### Comparing `prfiesta-0.9.1b148/LICENSE` & `prfiesta-0.9.1b149/LICENSE`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b148/README.md` & `prfiesta-0.9.1b149/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -81,20 +81,20 @@
 
 You can also customize the output file name using the `--output` option.
 
 ### Author Filter
 
 By default, `prfiesta` will take the users provided in the `--user` option and search the Git provider for any pull requests that the user **authored**. Within more collaborative environments, this may not be what you want as you may want to also gain some visibility into all secondary contributions a user made (e.g commenting on others pull requests).
 
-To help with this, `prfiesta` exposes the `--use-involves` flag which will search for pull requests that the user either:
+To help with this, `prfiesta` exposes the `--use-involves` flag which will search for pull requests that were:
 
 - Created by a certain user
 - Assigned to that user
 - Mention that user
-- Were commented on by that user
+- commented on by that user
 
 Learn more about `involves` [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-a-user-thats-involved-in-an-issue-or-pull-request).
 
 ### Date Filter
 
 When using the `--after` and `--before` date filters, by default `prfiesta` will use the `created` date dimension with these filters on the Git provider (e.g GitHub). This may not fit your use case and you may want to filter on when a pull request was updated instead. To do this you can use the `--use-updated` flag.
 
@@ -164,15 +164,15 @@
 precommit_run
 ```
 
 ### Creating Prereleases
 
 When you create a pull request on this repository, various CI checks are run, towards the end of those checks there is a `release` job.
 
-Usually when running under `main`, this job is responsible for publishing new versions to the pypi. However when running under a pull request, this will create a special prerelease package specific to that pull reuqest.
+Usually when running under `main`, this job is responsible for publishing new versions to pypi. However when running under a pull request, this will create a special prerelease package specific to that pull reuqest.
 
 The versioning of this package follows [PEP-440](https://peps.python.org/pep-0440/#pre-releases) and will look something like this:
 
 ```
 0.8.1b125
 ```
```

### Comparing `prfiesta-0.9.1b148/prfiesta/__main__.py` & `prfiesta-0.9.1b149/prfiesta/__main__.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b148/prfiesta/analysis/plot.py` & `prfiesta-0.9.1b149/prfiesta/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b148/prfiesta/analysis/view.py` & `prfiesta-0.9.1b149/prfiesta/analysis/view.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b148/prfiesta/collectors/github.py` & `prfiesta-0.9.1b149/prfiesta/collectors/github.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b148/prfiesta/environment.py` & `prfiesta-0.9.1b149/prfiesta/environment.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b148/prfiesta/output.py` & `prfiesta-0.9.1b149/prfiesta/output.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b148/pyproject.toml` & `prfiesta-0.9.1b149/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prfiesta"
-version = "0.9.1b148"
+version = "0.9.1b149"
 description = "Collect and Analyze Individual Contributor Pull Requests"
 authors = ["kiran94"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kiran94/prfiesta"
 repository = "https://github.com/kiran94/prfiesta"
 documentation = "https://github.com/kiran94/prfiesta/blob/main/README.md"
```

### Comparing `prfiesta-0.9.1b148/PKG-INFO` & `prfiesta-0.9.1b149/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prfiesta
-Version: 0.9.1b148
+Version: 0.9.1b149
 Summary: Collect and Analyze Individual Contributor Pull Requests
 Home-page: https://github.com/kiran94/prfiesta
 License: MIT
 Keywords: pull-request,pull-request-review,performance-review
 Author: kiran94
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
@@ -114,20 +114,20 @@
 
 You can also customize the output file name using the `--output` option.
 
 ### Author Filter
 
 By default, `prfiesta` will take the users provided in the `--user` option and search the Git provider for any pull requests that the user **authored**. Within more collaborative environments, this may not be what you want as you may want to also gain some visibility into all secondary contributions a user made (e.g commenting on others pull requests).
 
-To help with this, `prfiesta` exposes the `--use-involves` flag which will search for pull requests that the user either:
+To help with this, `prfiesta` exposes the `--use-involves` flag which will search for pull requests that were:
 
 - Created by a certain user
 - Assigned to that user
 - Mention that user
-- Were commented on by that user
+- commented on by that user
 
 Learn more about `involves` [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-a-user-thats-involved-in-an-issue-or-pull-request).
 
 ### Date Filter
 
 When using the `--after` and `--before` date filters, by default `prfiesta` will use the `created` date dimension with these filters on the Git provider (e.g GitHub). This may not fit your use case and you may want to filter on when a pull request was updated instead. To do this you can use the `--use-updated` flag.
 
@@ -197,15 +197,15 @@
 precommit_run
 ```
 
 ### Creating Prereleases
 
 When you create a pull request on this repository, various CI checks are run, towards the end of those checks there is a `release` job.
 
-Usually when running under `main`, this job is responsible for publishing new versions to the pypi. However when running under a pull request, this will create a special prerelease package specific to that pull reuqest.
+Usually when running under `main`, this job is responsible for publishing new versions to pypi. However when running under a pull request, this will create a special prerelease package specific to that pull reuqest.
 
 The versioning of this package follows [PEP-440](https://peps.python.org/pep-0440/#pre-releases) and will look something like this:
 
 ```
 0.8.1b125
 ```
```

