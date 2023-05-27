# Comparing `tmp/prfiesta-0.8.2b145.tar.gz` & `tmp/prfiesta-0.8.2b146.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prfiesta-0.8.2b145.tar", max compression
+gzip compressed data, was "prfiesta-0.8.2b146.tar", max compression
```

## Comparing `prfiesta-0.8.2b145.tar` & `prfiesta-0.8.2b146.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2023-05-27 07:50:05.244779 prfiesta-0.8.2b145/LICENSE
--rw-r--r--   0        0        0     9115 2023-05-27 07:50:05.244779 prfiesta-0.8.2b145/README.md
--rw-r--r--   0        0        0      487 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/__init__.py
--rw-r--r--   0        0        0     2994 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/__main__.py
--rw-r--r--   0        0        0        0 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/analysis/__init__.py
--rw-r--r--   0        0        0     4729 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/analysis/plot.py
--rw-r--r--   0        0        0     1007 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/analysis/view.py
--rw-r--r--   0        0        0        0 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/collectors/__init__.py
--rw-r--r--   0        0        0     5344 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/collectors/github.py
--rw-r--r--   0        0        0      571 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/environment.py
--rw-r--r--   0        0        0      975 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/output.py
--rw-r--r--   0        0        0      275 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/spinner.py
--rw-r--r--   0        0        0     3179 2023-05-27 07:50:18.264679 prfiesta-0.8.2b145/pyproject.toml
--rw-r--r--   0        0        0    10476 1970-01-01 00:00:00.000000 prfiesta-0.8.2b145/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-27 08:00:23.120097 prfiesta-0.8.2b146/LICENSE
+-rw-r--r--   0        0        0     9115 2023-05-27 08:00:23.120097 prfiesta-0.8.2b146/README.md
+-rw-r--r--   0        0        0      487 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/__init__.py
+-rw-r--r--   0        0        0     3018 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/analysis/__init__.py
+-rw-r--r--   0        0        0     4729 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/analysis/plot.py
+-rw-r--r--   0        0        0     1007 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/analysis/view.py
+-rw-r--r--   0        0        0        0 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/collectors/__init__.py
+-rw-r--r--   0        0        0     5344 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/collectors/github.py
+-rw-r--r--   0        0        0      571 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/environment.py
+-rw-r--r--   0        0        0      975 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/output.py
+-rw-r--r--   0        0        0      275 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/spinner.py
+-rw-r--r--   0        0        0     3179 2023-05-27 08:00:31.912191 prfiesta-0.8.2b146/pyproject.toml
+-rw-r--r--   0        0        0    10476 1970-01-01 00:00:00.000000 prfiesta-0.8.2b146/PKG-INFO
```

### Comparing `prfiesta-0.8.2b145/LICENSE` & `prfiesta-0.8.2b146/LICENSE`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.2b145/README.md` & `prfiesta-0.8.2b146/README.md`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.2b145/prfiesta/__main__.py` & `prfiesta-0.8.2b146/prfiesta/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 logger = logging.getLogger(__name__)
 
 github_environment = GitHubEnvironment()
 
 
 @click.command()
 @click.option('-u', '--users', required=True, multiple=True, help='The GitHub Users to search for. Can be multiple')
-@click.option('-t', '--token', help='The Authentication token to use')
+@click.option('-a', '--after', type=click.DateTime(formats=['%Y-%m-%d']), help='Only search for pull requests after this date e.g 2023-01-01')
+@click.option('-b', '--before', type=click.DateTime(formats=['%Y-%m-%d']), help='Only search for pull requests before this date e.g 2023-04-30')
+@click.option('-d', '--use_updated', is_flag=True, default=False, help='filter on when the pr was last updated rather then created')
+@click.option('-i', '--use_involves', is_flag=True, default=False, help='include prs where the author was the author or assignee or mentioned or commented')
+@click.option('-dc', '--drop_columns', multiple=True, help='Drop columns from the output dataframe')
 @click.option('-x', '--url', help='The URL of the Git provider to use')
+@click.option('-t', '--token', help='The Authentication token to use')
 @click.option('-o', '--output', default=None, help='The output location')
 @click.option('-ot', '--output_type', type=click.Choice(['csv', 'parquet']), default='csv', show_default=True, show_choices=True, help='The output format')
-@click.option('-dc', '--drop_columns', multiple=True, help='Drop columns from the output dataframe')
-@click.option('--after', type=click.DateTime(formats=['%Y-%m-%d']), help='Only search for pull requests after this date e.g 2023-01-01')
-@click.option('--before', type=click.DateTime(formats=['%Y-%m-%d']), help='Only search for pull requests before this date e.g 2023-04-30')
-@click.option('--use_updated', is_flag=True, default=False, help='filter on when the pr was last updated rather then created')
-@click.option('--use_involves', is_flag=True, default=False, help='include prs where the author was the author or assignee or mentioned or commented')
 @click.version_option(__version__)
 def main(**kwargs) -> None:
 
     users: tuple[str] = kwargs.get('users')
     token: str = kwargs.get('token') or github_environment.get_token()
     url: str = kwargs.get('url') or github_environment.get_url()
     output: str = kwargs.get('output')
```

### Comparing `prfiesta-0.8.2b145/prfiesta/analysis/plot.py` & `prfiesta-0.8.2b146/prfiesta/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.2b145/prfiesta/analysis/view.py` & `prfiesta-0.8.2b146/prfiesta/analysis/view.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.2b145/prfiesta/collectors/github.py` & `prfiesta-0.8.2b146/prfiesta/collectors/github.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.2b145/prfiesta/environment.py` & `prfiesta-0.8.2b146/prfiesta/environment.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.2b145/prfiesta/output.py` & `prfiesta-0.8.2b146/prfiesta/output.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.2b145/pyproject.toml` & `prfiesta-0.8.2b146/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prfiesta"
-version = "0.8.2b145"
+version = "0.8.2b146"
 description = "Collect and Analyze Individual Contributor Pull Requests"
 authors = ["kiran94"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kiran94/prfiesta"
 repository = "https://github.com/kiran94/prfiesta"
 documentation = "https://github.com/kiran94/prfiesta/blob/main/README.md"
```

### Comparing `prfiesta-0.8.2b145/PKG-INFO` & `prfiesta-0.8.2b146/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prfiesta
-Version: 0.8.2b145
+Version: 0.8.2b146
 Summary: Collect and Analyze Individual Contributor Pull Requests
 Home-page: https://github.com/kiran94/prfiesta
 License: MIT
 Keywords: pull-request,pull-request-review,performance-review
 Author: kiran94
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

