# Comparing `tmp/prfiesta-0.9.1b154.tar.gz` & `tmp/prfiesta-0.9.1b155.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prfiesta-0.9.1b154.tar", max compression
+gzip compressed data, was "prfiesta-0.9.1b155.tar", max compression
```

## Comparing `prfiesta-0.9.1b154.tar` & `prfiesta-0.9.1b155.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2023-05-27 13:57:11.028542 prfiesta-0.9.1b154/LICENSE
--rw-r--r--   0        0        0     9095 2023-05-27 13:57:11.028542 prfiesta-0.9.1b154/README.md
--rw-r--r--   0        0        0      487 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/__init__.py
--rw-r--r--   0        0        0     3799 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/__main__.py
--rw-r--r--   0        0        0        0 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/analysis/__init__.py
--rw-r--r--   0        0        0     4729 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/analysis/plot.py
--rw-r--r--   0        0        0     1007 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/analysis/view.py
--rw-r--r--   0        0        0        0 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/collectors/__init__.py
--rw-r--r--   0        0        0     5929 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/collectors/github.py
--rw-r--r--   0        0        0      571 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/environment.py
--rw-r--r--   0        0        0      975 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/output.py
--rw-r--r--   0        0        0      275 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/spinner.py
--rw-r--r--   0        0        0     3203 2023-05-27 13:57:25.512561 prfiesta-0.9.1b154/pyproject.toml
--rw-r--r--   0        0        0    10501 1970-01-01 00:00:00.000000 prfiesta-0.9.1b154/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-27 15:06:13.760800 prfiesta-0.9.1b155/LICENSE
+-rw-r--r--   0        0        0    10180 2023-05-27 15:06:13.760800 prfiesta-0.9.1b155/README.md
+-rw-r--r--   0        0        0      487 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/__init__.py
+-rw-r--r--   0        0        0     3799 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/analysis/__init__.py
+-rw-r--r--   0        0        0     4729 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/analysis/plot.py
+-rw-r--r--   0        0        0     1007 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/analysis/view.py
+-rw-r--r--   0        0        0        0 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/collectors/__init__.py
+-rw-r--r--   0        0        0     5929 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/collectors/github.py
+-rw-r--r--   0        0        0      571 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/environment.py
+-rw-r--r--   0        0        0      975 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/output.py
+-rw-r--r--   0        0        0      275 2023-05-27 15:06:13.768800 prfiesta-0.9.1b155/prfiesta/spinner.py
+-rw-r--r--   0        0        0     3203 2023-05-27 15:06:24.108863 prfiesta-0.9.1b155/pyproject.toml
+-rw-r--r--   0        0        0    11586 1970-01-01 00:00:00.000000 prfiesta-0.9.1b155/PKG-INFO
```

### Comparing `prfiesta-0.9.1b154/LICENSE` & `prfiesta-0.9.1b155/LICENSE`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b154/README.md` & `prfiesta-0.9.1b155/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -47,14 +47,20 @@
 
 # Get all pull requests and drop specific columns from the output
 prfiesta -u kiran94 -dc events_url -dc comments_url -dc node_id
 
 # Get all pull requests where the user was involved (as opposed to just authored)
 prfiesta -u kiran94 --use-involves
 
+# Get all pull requests where the user reviewed it rather then being the author
+prfiesta -u charliermarsh --after 2023-05-01 --use-reviewed-by
+
+# Get all pull requests where the user was requested a review rather then being the author
+prfiesta -u charliermarsh --after 2023-05-01 --use-review-requested
+
 # Get help
 prfiesta --help
 
 # Show the current version
 prfiesta --version
 ```
 
@@ -81,23 +87,39 @@
 
 You can also customize the output file name using the `--output` option.
 
 ### Author Filter
 
 By default, `prfiesta` will take the users provided in the `--user` option and search the Git provider for any pull requests that the user **authored**. Within more collaborative environments, this may not be what you want as you may want to also gain some visibility into all secondary contributions a user made (e.g commenting on others pull requests).
 
-To help with this, `prfiesta` exposes the `--use-involves` flag which will search for pull requests that were:
+*The options listed here are mutually exclusive.*
+
+#### User Involvement
+
+`prfiesta` exposes the `--use-involves` flag which will search for pull requests that were:
 
 - Created by a certain user
 - Assigned to that user
 - Mention that user
 - commented on by that user
 
 Learn more about `involves` [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-a-user-thats-involved-in-an-issue-or-pull-request).
 
+#### User Reviewed
+
+`prfiesta` exposes a `--use-reviewed-by` flag which will collect pull requests where the user has reviewed others pull requests.
+
+Learn more about searching review requests [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-pull-request-review-status-and-reviewer)
+
+#### User Requested Review
+
+`prfiesta` exposes a `--use-review-requested` flag  which will collect pull requests where the user was *requested* a review from other collaborators.
+
+Learn more about searching review requests [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-pull-request-review-status-and-reviewer)
+
 ### Date Filter
 
 When using the `--after` and `--before` date filters, by default `prfiesta` will use the `created` date dimension with these filters on the Git provider (e.g GitHub). This may not fit your use case and you may want to filter on when a pull request was updated instead. To do this you can use the `--use-updated` flag.
 
 See more information [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-when-an-issue-or-pull-request-was-created-or-last-updated).
 
 ## Analysis
```

### Comparing `prfiesta-0.9.1b154/prfiesta/__main__.py` & `prfiesta-0.9.1b155/prfiesta/__main__.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b154/prfiesta/analysis/plot.py` & `prfiesta-0.9.1b155/prfiesta/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b154/prfiesta/analysis/view.py` & `prfiesta-0.9.1b155/prfiesta/analysis/view.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b154/prfiesta/collectors/github.py` & `prfiesta-0.9.1b155/prfiesta/collectors/github.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b154/prfiesta/environment.py` & `prfiesta-0.9.1b155/prfiesta/environment.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b154/prfiesta/output.py` & `prfiesta-0.9.1b155/prfiesta/output.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b154/pyproject.toml` & `prfiesta-0.9.1b155/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prfiesta"
-version = "0.9.1b154"
+version = "0.9.1b155"
 description = "Collect and Analyze Individual Contributor Pull Requests"
 authors = ["kiran94"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pypi.org/project/prfiesta/"
 repository = "https://github.com/kiran94/prfiesta/pull/40"
 documentation = "https://github.com/kiran94/prfiesta/blob/main/README.md"
```

### Comparing `prfiesta-0.9.1b154/PKG-INFO` & `prfiesta-0.9.1b155/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prfiesta
-Version: 0.9.1b154
+Version: 0.9.1b155
 Summary: Collect and Analyze Individual Contributor Pull Requests
 Home-page: https://pypi.org/project/prfiesta/
 License: MIT
 Keywords: pull-request,pull-request-review,performance-review
 Author: kiran94
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
@@ -81,14 +81,20 @@
 
 # Get all pull requests and drop specific columns from the output
 prfiesta -u kiran94 -dc events_url -dc comments_url -dc node_id
 
 # Get all pull requests where the user was involved (as opposed to just authored)
 prfiesta -u kiran94 --use-involves
 
+# Get all pull requests where the user reviewed it rather then being the author
+prfiesta -u charliermarsh --after 2023-05-01 --use-reviewed-by
+
+# Get all pull requests where the user was requested a review rather then being the author
+prfiesta -u charliermarsh --after 2023-05-01 --use-review-requested
+
 # Get help
 prfiesta --help
 
 # Show the current version
 prfiesta --version
 ```
 
@@ -115,23 +121,39 @@
 
 You can also customize the output file name using the `--output` option.
 
 ### Author Filter
 
 By default, `prfiesta` will take the users provided in the `--user` option and search the Git provider for any pull requests that the user **authored**. Within more collaborative environments, this may not be what you want as you may want to also gain some visibility into all secondary contributions a user made (e.g commenting on others pull requests).
 
-To help with this, `prfiesta` exposes the `--use-involves` flag which will search for pull requests that were:
+*The options listed here are mutually exclusive.*
+
+#### User Involvement
+
+`prfiesta` exposes the `--use-involves` flag which will search for pull requests that were:
 
 - Created by a certain user
 - Assigned to that user
 - Mention that user
 - commented on by that user
 
 Learn more about `involves` [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-a-user-thats-involved-in-an-issue-or-pull-request).
 
+#### User Reviewed
+
+`prfiesta` exposes a `--use-reviewed-by` flag which will collect pull requests where the user has reviewed others pull requests.
+
+Learn more about searching review requests [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-pull-request-review-status-and-reviewer)
+
+#### User Requested Review
+
+`prfiesta` exposes a `--use-review-requested` flag  which will collect pull requests where the user was *requested* a review from other collaborators.
+
+Learn more about searching review requests [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-pull-request-review-status-and-reviewer)
+
 ### Date Filter
 
 When using the `--after` and `--before` date filters, by default `prfiesta` will use the `created` date dimension with these filters on the Git provider (e.g GitHub). This may not fit your use case and you may want to filter on when a pull request was updated instead. To do this you can use the `--use-updated` flag.
 
 See more information [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-when-an-issue-or-pull-request-was-created-or-last-updated).
 
 ## Analysis
```

