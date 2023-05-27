# Comparing `tmp/prfiesta-0.9.0.tar.gz` & `tmp/prfiesta-0.9.1b148.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prfiesta-0.9.0.tar", max compression
+gzip compressed data, was "prfiesta-0.9.1b148.tar", max compression
```

## Comparing `prfiesta-0.9.0.tar` & `prfiesta-0.9.1b148.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2023-05-27 08:10:57.151480 prfiesta-0.9.0/LICENSE
--rw-r--r--   0        0        0     9115 2023-05-27 08:10:57.151480 prfiesta-0.9.0/README.md
--rw-r--r--   0        0        0      487 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/__init__.py
--rw-r--r--   0        0        0     3018 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/__main__.py
--rw-r--r--   0        0        0        0 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/analysis/__init__.py
--rw-r--r--   0        0        0     4729 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/analysis/plot.py
--rw-r--r--   0        0        0     1007 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/analysis/view.py
--rw-r--r--   0        0        0        0 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/collectors/__init__.py
--rw-r--r--   0        0        0     5344 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/collectors/github.py
--rw-r--r--   0        0        0      571 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/environment.py
--rw-r--r--   0        0        0      975 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/output.py
--rw-r--r--   0        0        0      275 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/spinner.py
--rw-r--r--   0        0        0     3175 2023-05-27 08:11:15.324779 prfiesta-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    10472 1970-01-01 00:00:00.000000 prfiesta-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-27 08:20:03.023018 prfiesta-0.9.1b148/LICENSE
+-rw-r--r--   0        0        0     9115 2023-05-27 08:20:03.023018 prfiesta-0.9.1b148/README.md
+-rw-r--r--   0        0        0      487 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/__init__.py
+-rw-r--r--   0        0        0     3018 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/analysis/__init__.py
+-rw-r--r--   0        0        0     4729 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/analysis/plot.py
+-rw-r--r--   0        0        0     1007 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/analysis/view.py
+-rw-r--r--   0        0        0        0 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/collectors/__init__.py
+-rw-r--r--   0        0        0     5344 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/collectors/github.py
+-rw-r--r--   0        0        0      571 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/environment.py
+-rw-r--r--   0        0        0      975 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/output.py
+-rw-r--r--   0        0        0      275 2023-05-27 08:20:03.035018 prfiesta-0.9.1b148/prfiesta/spinner.py
+-rw-r--r--   0        0        0     3179 2023-05-27 08:20:13.147527 prfiesta-0.9.1b148/pyproject.toml
+-rw-r--r--   0        0        0    10476 1970-01-01 00:00:00.000000 prfiesta-0.9.1b148/PKG-INFO
```

### Comparing `prfiesta-0.9.0/LICENSE` & `prfiesta-0.9.1b148/LICENSE`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.0/README.md` & `prfiesta-0.9.1b148/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,30 +30,30 @@
 # Get all pull requests for a user created after a date
 prfiesta -u kiran94 --after 2023-01-01
 
 # Get all pull requests for a user created between two dates
 prfiesta -u kiran94 --after 2023-01-01 --before 2023-06-01
 
 # Get all pull requests for a user updated after a date
-prfiesta -u kiran94 --after 2023-01-01 --use_updated
+prfiesta -u kiran94 --after 2023-01-01 --use-updated
 
 # Get all pull requests with a custom output file name
 prfiesta -u kiran94 --output my_pull_requests.csv
 
 # Get all pull requests in parquet format with a custom file name
-prfiesta -u kiran94 --output_type parquet --output my_pull_requests.parquet
+prfiesta -u kiran94 --output-type parquet --output my_pull_requests.parquet
 
 # Get all pull requests for more then one user
 prfiesta -u kiran94 -u user2
 
 # Get all pull requests and drop specific columns from the output
 prfiesta -u kiran94 -dc events_url -dc comments_url -dc node_id
 
 # Get all pull requests where the user was involved (as opposed to just authored)
-prfiesta -u kiran94 --use_involves
+prfiesta -u kiran94 --use-involves
 
 # Get help
 prfiesta --help
 
 # Show the current version
 prfiesta --version
 ```
@@ -70,37 +70,37 @@
 frame: pd.DataFrame = github.collect('kiran94', 'user2', after=datetime(2023, 1, 1))
 
 print(frame)
 ```
 
 ### Output
 
-You can control the output type using the `--output_type` option. Supported options:
+You can control the output type using the `--output-type` option. Supported options:
 
 - `csv` (default)
 - `parquet`
 
 You can also customize the output file name using the `--output` option.
 
 ### Author Filter
 
 By default, `prfiesta` will take the users provided in the `--user` option and search the Git provider for any pull requests that the user **authored**. Within more collaborative environments, this may not be what you want as you may want to also gain some visibility into all secondary contributions a user made (e.g commenting on others pull requests).
 
-To help with this, `prfiesta` exposes the `--use_involves` flag which will search for pull requests that the user either:
+To help with this, `prfiesta` exposes the `--use-involves` flag which will search for pull requests that the user either:
 
 - Created by a certain user
 - Assigned to that user
 - Mention that user
 - Were commented on by that user
 
 Learn more about `involves` [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-a-user-thats-involved-in-an-issue-or-pull-request).
 
 ### Date Filter
 
-When using the `--after` and `--before` date filters, by default `prfiesta` will use the `created` date dimension with these filters on the Git provider (e.g GitHub). This may not fit your use case and you may want to filter on when a pull request was updated instead. To do this you can use the `--use_updated` flag.
+When using the `--after` and `--before` date filters, by default `prfiesta` will use the `created` date dimension with these filters on the Git provider (e.g GitHub). This may not fit your use case and you may want to filter on when a pull request was updated instead. To do this you can use the `--use-updated` flag.
 
 See more information [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-when-an-issue-or-pull-request-was-created-or-last-updated).
 
 ## Analysis
 
 `prfiesta` ships with built in plots to help analyze your pull request data. These serve as a starting point in your analysis. See more information on the build in plots and views [here](https://github.com/kiran94/prfiesta/blob/main/docs/analysis.md).
```

### Comparing `prfiesta-0.9.0/prfiesta/__main__.py` & `prfiesta-0.9.1b148/prfiesta/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 github_environment = GitHubEnvironment()
 
 
 @click.command()
 @click.option('-u', '--users', required=True, multiple=True, help='The GitHub Users to search for. Can be multiple')
 @click.option('-a', '--after', type=click.DateTime(formats=['%Y-%m-%d']), help='Only search for pull requests after this date e.g 2023-01-01')
 @click.option('-b', '--before', type=click.DateTime(formats=['%Y-%m-%d']), help='Only search for pull requests before this date e.g 2023-04-30')
-@click.option('-d', '--use_updated', is_flag=True, default=False, help='filter on when the pr was last updated rather then created')
-@click.option('-i', '--use_involves', is_flag=True, default=False, help='include prs where the author was the author or assignee or mentioned or commented')
-@click.option('-dc', '--drop_columns', multiple=True, help='Drop columns from the output dataframe')
+@click.option('-d', '--use-updated', is_flag=True, default=False, help='filter on when the pr was last updated rather then created')
+@click.option('-i', '--use-involves', is_flag=True, default=False, help='include prs where the author was the author or assignee or mentioned or commented')
+@click.option('-dc', '--drop-columns', multiple=True, help='Drop columns from the output dataframe')
 @click.option('-x', '--url', help='The URL of the Git provider to use')
 @click.option('-t', '--token', help='The Authentication token to use')
 @click.option('-o', '--output', default=None, help='The output location')
-@click.option('-ot', '--output_type', type=click.Choice(['csv', 'parquet']), default='csv', show_default=True, show_choices=True, help='The output format')
+@click.option('-ot', '--output-type', type=click.Choice(['csv', 'parquet']), default='csv', show_default=True, show_choices=True, help='The output format')
 @click.version_option(__version__)
 def main(**kwargs) -> None:
 
     users: tuple[str] = kwargs.get('users')
     token: str = kwargs.get('token') or github_environment.get_token()
     url: str = kwargs.get('url') or github_environment.get_url()
     output: str = kwargs.get('output')
```

### Comparing `prfiesta-0.9.0/prfiesta/analysis/plot.py` & `prfiesta-0.9.1b148/prfiesta/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.0/prfiesta/analysis/view.py` & `prfiesta-0.9.1b148/prfiesta/analysis/view.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.0/prfiesta/collectors/github.py` & `prfiesta-0.9.1b148/prfiesta/collectors/github.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.0/prfiesta/environment.py` & `prfiesta-0.9.1b148/prfiesta/environment.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.0/prfiesta/output.py` & `prfiesta-0.9.1b148/prfiesta/output.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.0/pyproject.toml` & `prfiesta-0.9.1b148/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prfiesta"
-version = "0.9.0"
+version = "0.9.1b148"
 description = "Collect and Analyze Individual Contributor Pull Requests"
 authors = ["kiran94"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kiran94/prfiesta"
 repository = "https://github.com/kiran94/prfiesta"
 documentation = "https://github.com/kiran94/prfiesta/blob/main/README.md"
```

### Comparing `prfiesta-0.9.0/PKG-INFO` & `prfiesta-0.9.1b148/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prfiesta
-Version: 0.9.0
+Version: 0.9.1b148
 Summary: Collect and Analyze Individual Contributor Pull Requests
 Home-page: https://github.com/kiran94/prfiesta
 License: MIT
 Keywords: pull-request,pull-request-review,performance-review
 Author: kiran94
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
@@ -63,30 +63,30 @@
 # Get all pull requests for a user created after a date
 prfiesta -u kiran94 --after 2023-01-01
 
 # Get all pull requests for a user created between two dates
 prfiesta -u kiran94 --after 2023-01-01 --before 2023-06-01
 
 # Get all pull requests for a user updated after a date
-prfiesta -u kiran94 --after 2023-01-01 --use_updated
+prfiesta -u kiran94 --after 2023-01-01 --use-updated
 
 # Get all pull requests with a custom output file name
 prfiesta -u kiran94 --output my_pull_requests.csv
 
 # Get all pull requests in parquet format with a custom file name
-prfiesta -u kiran94 --output_type parquet --output my_pull_requests.parquet
+prfiesta -u kiran94 --output-type parquet --output my_pull_requests.parquet
 
 # Get all pull requests for more then one user
 prfiesta -u kiran94 -u user2
 
 # Get all pull requests and drop specific columns from the output
 prfiesta -u kiran94 -dc events_url -dc comments_url -dc node_id
 
 # Get all pull requests where the user was involved (as opposed to just authored)
-prfiesta -u kiran94 --use_involves
+prfiesta -u kiran94 --use-involves
 
 # Get help
 prfiesta --help
 
 # Show the current version
 prfiesta --version
 ```
@@ -103,37 +103,37 @@
 frame: pd.DataFrame = github.collect('kiran94', 'user2', after=datetime(2023, 1, 1))
 
 print(frame)
 ```
 
 ### Output
 
-You can control the output type using the `--output_type` option. Supported options:
+You can control the output type using the `--output-type` option. Supported options:
 
 - `csv` (default)
 - `parquet`
 
 You can also customize the output file name using the `--output` option.
 
 ### Author Filter
 
 By default, `prfiesta` will take the users provided in the `--user` option and search the Git provider for any pull requests that the user **authored**. Within more collaborative environments, this may not be what you want as you may want to also gain some visibility into all secondary contributions a user made (e.g commenting on others pull requests).
 
-To help with this, `prfiesta` exposes the `--use_involves` flag which will search for pull requests that the user either:
+To help with this, `prfiesta` exposes the `--use-involves` flag which will search for pull requests that the user either:
 
 - Created by a certain user
 - Assigned to that user
 - Mention that user
 - Were commented on by that user
 
 Learn more about `involves` [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-a-user-thats-involved-in-an-issue-or-pull-request).
 
 ### Date Filter
 
-When using the `--after` and `--before` date filters, by default `prfiesta` will use the `created` date dimension with these filters on the Git provider (e.g GitHub). This may not fit your use case and you may want to filter on when a pull request was updated instead. To do this you can use the `--use_updated` flag.
+When using the `--after` and `--before` date filters, by default `prfiesta` will use the `created` date dimension with these filters on the Git provider (e.g GitHub). This may not fit your use case and you may want to filter on when a pull request was updated instead. To do this you can use the `--use-updated` flag.
 
 See more information [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-when-an-issue-or-pull-request-was-created-or-last-updated).
 
 ## Analysis
 
 `prfiesta` ships with built in plots to help analyze your pull request data. These serve as a starting point in your analysis. See more information on the build in plots and views [here](https://github.com/kiran94/prfiesta/blob/main/docs/analysis.md).
```

