# Comparing `tmp/prfiesta-0.8.1b143.tar.gz` & `tmp/prfiesta-0.8.2b145.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prfiesta-0.8.1b143.tar", max compression
+gzip compressed data, was "prfiesta-0.8.2b145.tar", max compression
```

## Comparing `prfiesta-0.8.1b143.tar` & `prfiesta-0.8.2b145.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2023-05-26 20:30:59.057780 prfiesta-0.8.1b143/LICENSE
--rw-r--r--   0        0        0     8016 2023-05-26 20:30:59.057780 prfiesta-0.8.1b143/README.md
--rw-r--r--   0        0        0      487 2023-05-26 20:30:59.065780 prfiesta-0.8.1b143/prfiesta/__init__.py
--rw-r--r--   0        0        0     2763 2023-05-26 20:30:59.065780 prfiesta-0.8.1b143/prfiesta/__main__.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:59.065780 prfiesta-0.8.1b143/prfiesta/analysis/__init__.py
--rw-r--r--   0        0        0     4729 2023-05-26 20:30:59.065780 prfiesta-0.8.1b143/prfiesta/analysis/plot.py
--rw-r--r--   0        0        0     1007 2023-05-26 20:30:59.065780 prfiesta-0.8.1b143/prfiesta/analysis/view.py
--rw-r--r--   0        0        0        0 2023-05-26 20:30:59.065780 prfiesta-0.8.1b143/prfiesta/collectors/__init__.py
--rw-r--r--   0        0        0     4981 2023-05-26 20:30:59.065780 prfiesta-0.8.1b143/prfiesta/collectors/github.py
--rw-r--r--   0        0        0      571 2023-05-26 20:30:59.065780 prfiesta-0.8.1b143/prfiesta/environment.py
--rw-r--r--   0        0        0      975 2023-05-26 20:30:59.065780 prfiesta-0.8.1b143/prfiesta/output.py
--rw-r--r--   0        0        0      275 2023-05-26 20:30:59.065780 prfiesta-0.8.1b143/prfiesta/spinner.py
--rw-r--r--   0        0        0     3199 2023-05-26 20:31:07.641726 prfiesta-0.8.1b143/pyproject.toml
--rw-r--r--   0        0        0     9377 1970-01-01 00:00:00.000000 prfiesta-0.8.1b143/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-27 07:50:05.244779 prfiesta-0.8.2b145/LICENSE
+-rw-r--r--   0        0        0     9115 2023-05-27 07:50:05.244779 prfiesta-0.8.2b145/README.md
+-rw-r--r--   0        0        0      487 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/__init__.py
+-rw-r--r--   0        0        0     2994 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/analysis/__init__.py
+-rw-r--r--   0        0        0     4729 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/analysis/plot.py
+-rw-r--r--   0        0        0     1007 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/analysis/view.py
+-rw-r--r--   0        0        0        0 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/collectors/__init__.py
+-rw-r--r--   0        0        0     5344 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/collectors/github.py
+-rw-r--r--   0        0        0      571 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/environment.py
+-rw-r--r--   0        0        0      975 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/output.py
+-rw-r--r--   0        0        0      275 2023-05-27 07:50:05.252779 prfiesta-0.8.2b145/prfiesta/spinner.py
+-rw-r--r--   0        0        0     3179 2023-05-27 07:50:18.264679 prfiesta-0.8.2b145/pyproject.toml
+-rw-r--r--   0        0        0    10476 1970-01-01 00:00:00.000000 prfiesta-0.8.2b145/PKG-INFO
```

### Comparing `prfiesta-0.8.1b143/LICENSE` & `prfiesta-0.8.2b145/LICENSE`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b143/README.md` & `prfiesta-0.8.2b145/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -44,16 +44,22 @@
 
 # Get all pull requests for more then one user
 prfiesta -u kiran94 -u user2
 
 # Get all pull requests and drop specific columns from the output
 prfiesta -u kiran94 -dc events_url -dc comments_url -dc node_id
 
+# Get all pull requests where the user was involved (as opposed to just authored)
+prfiesta -u kiran94 --use_involves
+
 # Get help
 prfiesta --help
+
+# Show the current version
+prfiesta --version
 ```
 
 You can also leverage `prfiesta` directly in your own application:
 
 ```python
 import pandas as pd
 
@@ -71,14 +77,27 @@
 You can control the output type using the `--output_type` option. Supported options:
 
 - `csv` (default)
 - `parquet`
 
 You can also customize the output file name using the `--output` option.
 
+### Author Filter
+
+By default, `prfiesta` will take the users provided in the `--user` option and search the Git provider for any pull requests that the user **authored**. Within more collaborative environments, this may not be what you want as you may want to also gain some visibility into all secondary contributions a user made (e.g commenting on others pull requests).
+
+To help with this, `prfiesta` exposes the `--use_involves` flag which will search for pull requests that the user either:
+
+- Created by a certain user
+- Assigned to that user
+- Mention that user
+- Were commented on by that user
+
+Learn more about `involves` [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-a-user-thats-involved-in-an-issue-or-pull-request).
+
 ### Date Filter
 
 When using the `--after` and `--before` date filters, by default `prfiesta` will use the `created` date dimension with these filters on the Git provider (e.g GitHub). This may not fit your use case and you may want to filter on when a pull request was updated instead. To do this you can use the `--use_updated` flag.
 
 See more information [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-when-an-issue-or-pull-request-was-created-or-last-updated).
 
 ## Analysis
@@ -160,10 +179,10 @@
 Where
 - `0.8.1` = The bumped version of what is currently within the `pyproject.toml` of that pull request. We don't attempt to do any analysis to figure out if we should be bumping with a higher serverity in this context.
 - `b` = Beta; Indicates to pypi that this is a prerelease package.
 - `125` = The `github.run_number` from [GitHub Actions](https://docs.github.com/en/actions/learn-github-actions/contexts#github-context).
 
 An example prerelease package looks like this: https://pypi.org/project/prfiesta/0.8.1b125/
 
-Downstream users can then do a full end to end test with the prerelease package before the change is merged into `main`.
+Downstream users can then do a full end to end test with the prerelease package before the change is merged into `main`. This will automatically be posted into the pull request [example](https://github.com/kiran94/prfiesta/pull/36#issuecomment-1564909558).
 
 You can find the full version history of package [here](https://pypi.org/project/prfiesta/#history)
```

### Comparing `prfiesta-0.8.1b143/prfiesta/__main__.py` & `prfiesta-0.8.2b145/prfiesta/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,44 +13,46 @@
 
 logger = logging.getLogger(__name__)
 
 github_environment = GitHubEnvironment()
 
 
 @click.command()
-@click.option('-u', '--users', required=True, multiple=True, help='The GitHub Users to search for. Can be multiple (space delimited)')
+@click.option('-u', '--users', required=True, multiple=True, help='The GitHub Users to search for. Can be multiple')
 @click.option('-t', '--token', help='The Authentication token to use')
 @click.option('-x', '--url', help='The URL of the Git provider to use')
 @click.option('-o', '--output', default=None, help='The output location')
-@click.option('-ot', '--output_type', type=click.Choice(['csv', 'parquet']), default='csv', show_default=True, help='The output format')
+@click.option('-ot', '--output_type', type=click.Choice(['csv', 'parquet']), default='csv', show_default=True, show_choices=True, help='The output format')
 @click.option('-dc', '--drop_columns', multiple=True, help='Drop columns from the output dataframe')
 @click.option('--after', type=click.DateTime(formats=['%Y-%m-%d']), help='Only search for pull requests after this date e.g 2023-01-01')
 @click.option('--before', type=click.DateTime(formats=['%Y-%m-%d']), help='Only search for pull requests before this date e.g 2023-04-30')
 @click.option('--use_updated', is_flag=True, default=False, help='filter on when the pr was last updated rather then created')
+@click.option('--use_involves', is_flag=True, default=False, help='include prs where the author was the author or assignee or mentioned or commented')
 @click.version_option(__version__)
 def main(**kwargs) -> None:
 
     users: tuple[str] = kwargs.get('users')
     token: str = kwargs.get('token') or github_environment.get_token()
     url: str = kwargs.get('url') or github_environment.get_url()
     output: str = kwargs.get('output')
     output_type: str = kwargs.get('output_type')
     before: datetime = kwargs.get('before')
     after: datetime = kwargs.get('after')
     drop_columns: list[str] = list(kwargs.get('drop_columns'))
     use_updated: bool = kwargs.get('use_updated')
+    use_involves: bool = kwargs.get('use_involves')
 
     logger.info('[bold green]PR Fiesta 🦜🥳')
 
     spinner = Spinner('dots', text=Text('Loading', style=SPINNER_STYLE))
 
     with Live(spinner, refresh_per_second=20, transient=True):
 
         collector = GitHubCollector(token=token, url=url, spinner=spinner, drop_columns=drop_columns)
-        pr_frame = collector.collect(*users, after=after, before=before, use_updated=use_updated)
+        pr_frame = collector.collect(*users, after=after, before=before, use_updated=use_updated, use_involves=use_involves)
 
         if not pr_frame.empty:
             logger.info('Found [bold green]%s[/bold green] pull requests!', pr_frame.shape[0])
 
             output_frame(pr_frame, output_type, spinner=spinner, output_name=output)
             logger.info('Time to analyze 🔎 See https://github.com/kiran94/prfiesta/blob/main/docs/analysis.md for some inspiration!')
```

### Comparing `prfiesta-0.8.1b143/prfiesta/analysis/plot.py` & `prfiesta-0.8.2b145/prfiesta/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b143/prfiesta/analysis/view.py` & `prfiesta-0.8.2b145/prfiesta/analysis/view.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b143/prfiesta/collectors/github.py` & `prfiesta-0.8.2b145/prfiesta/collectors/github.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,18 +44,19 @@
 
 
     def collect(
             self,
             *users: Tuple[str],
             after: Optional[datetime] = None,
             before: Optional[datetime] = None,
-            use_updated: bool = False,
+            use_updated: Optional[bool] = False,
+            use_involves: Optional[bool] = False,
         ) -> pd.DataFrame:
 
-        query = self._construct_query(users, after, before, use_updated)
+        query = self._construct_query(users, after, before, use_updated, use_involves)
 
         update_spinner(f'Searching {self._url} with[bold blue] {query}', self._spinner,  logger)
 
         pull_request_data = None
         try:
             pulls = self._github.search_issues(query=query)
 
@@ -81,15 +82,21 @@
         pr_frame['repository_name'] = pr_frame['repository_url'].str.extract(r'(.*)\/repos\/(?P<repository_name>(.*))')['repository_name']
         pr_frame = self._move_column_to_end(pr_frame)
 
         return pr_frame
 
 
     @staticmethod
-    def _construct_query(users: List[str], after: Optional[datetime] = None, before: Optional[datetime] = None, use_updated: bool = False) -> str:
+    def _construct_query(
+            users: List[str],
+            after: Optional[datetime] = None,
+            before: Optional[datetime] = None,
+            use_updated: Optional[bool] = False,
+            use_involves: Optional[bool] = False,
+        ) -> str:
         """
         Constructs a GitHub Search Query
         that returns pull requests made by the passed users and options.
 
         Examples
         --------
             type:pr author:user1
@@ -98,16 +105,22 @@
 
         All dates are inclusive.
         See GitHub Docs for full options https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests
         """
         query: List[str] = []
         query.append('type:pr')
 
+        author_filter = 'author'
+        if use_involves:
+            author_filter = 'involves'
+
         for u in users:
-            query.append('author:' + u)
+            query.append(f'{author_filter}:{u}')
+
+        logger.debug('using author filter %s', author_filter)
 
         time_filter = 'created'
         if use_updated:
             time_filter = 'updated'
 
         logger.debug('using time filter %s', time_filter)
```

### Comparing `prfiesta-0.8.1b143/prfiesta/environment.py` & `prfiesta-0.8.2b145/prfiesta/environment.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b143/prfiesta/output.py` & `prfiesta-0.8.2b145/prfiesta/output.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b143/pyproject.toml` & `prfiesta-0.8.2b145/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prfiesta"
-version = "0.8.1b143"
+version = "0.8.2b145"
 description = "Collect and Analyze Individual Contributor Pull Requests"
 authors = ["kiran94"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kiran94/prfiesta"
 repository = "https://github.com/kiran94/prfiesta"
 documentation = "https://github.com/kiran94/prfiesta/blob/main/README.md"
@@ -26,25 +26,24 @@
 rich = "^13.3.5"
 seaborn = "^0.12.2"
 matplotlib = "^3.7.1"
 natural = "^0.2.0"
 urllib3 = "<2"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.0.263"
-polars = "^0.17.10"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 pytest-github-actions-annotate-failures = "^0.2.0"
 jupyterlab = "^3.6.3"
 jupyterlab-widgets = "^3.0.7"
 jupyter-black = "^0.3.4"
 ipywidgets = "^8.0.6"
 pre-commit = "^3.3.2"
 papermill = "^2.4.0"
+ruff = "^0.0.270"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 prfiesta = 'prfiesta.__main__:main'
```

### Comparing `prfiesta-0.8.1b143/PKG-INFO` & `prfiesta-0.8.2b145/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prfiesta
-Version: 0.8.1b143
+Version: 0.8.2b145
 Summary: Collect and Analyze Individual Contributor Pull Requests
 Home-page: https://github.com/kiran94/prfiesta
 License: MIT
 Keywords: pull-request,pull-request-review,performance-review
 Author: kiran94
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
@@ -77,16 +77,22 @@
 
 # Get all pull requests for more then one user
 prfiesta -u kiran94 -u user2
 
 # Get all pull requests and drop specific columns from the output
 prfiesta -u kiran94 -dc events_url -dc comments_url -dc node_id
 
+# Get all pull requests where the user was involved (as opposed to just authored)
+prfiesta -u kiran94 --use_involves
+
 # Get help
 prfiesta --help
+
+# Show the current version
+prfiesta --version
 ```
 
 You can also leverage `prfiesta` directly in your own application:
 
 ```python
 import pandas as pd
 
@@ -104,14 +110,27 @@
 You can control the output type using the `--output_type` option. Supported options:
 
 - `csv` (default)
 - `parquet`
 
 You can also customize the output file name using the `--output` option.
 
+### Author Filter
+
+By default, `prfiesta` will take the users provided in the `--user` option and search the Git provider for any pull requests that the user **authored**. Within more collaborative environments, this may not be what you want as you may want to also gain some visibility into all secondary contributions a user made (e.g commenting on others pull requests).
+
+To help with this, `prfiesta` exposes the `--use_involves` flag which will search for pull requests that the user either:
+
+- Created by a certain user
+- Assigned to that user
+- Mention that user
+- Were commented on by that user
+
+Learn more about `involves` [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-a-user-thats-involved-in-an-issue-or-pull-request).
+
 ### Date Filter
 
 When using the `--after` and `--before` date filters, by default `prfiesta` will use the `created` date dimension with these filters on the Git provider (e.g GitHub). This may not fit your use case and you may want to filter on when a pull request was updated instead. To do this you can use the `--use_updated` flag.
 
 See more information [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-when-an-issue-or-pull-request-was-created-or-last-updated).
 
 ## Analysis
@@ -193,11 +212,11 @@
 Where
 - `0.8.1` = The bumped version of what is currently within the `pyproject.toml` of that pull request. We don't attempt to do any analysis to figure out if we should be bumping with a higher serverity in this context.
 - `b` = Beta; Indicates to pypi that this is a prerelease package.
 - `125` = The `github.run_number` from [GitHub Actions](https://docs.github.com/en/actions/learn-github-actions/contexts#github-context).
 
 An example prerelease package looks like this: https://pypi.org/project/prfiesta/0.8.1b125/
 
-Downstream users can then do a full end to end test with the prerelease package before the change is merged into `main`.
+Downstream users can then do a full end to end test with the prerelease package before the change is merged into `main`. This will automatically be posted into the pull request [example](https://github.com/kiran94/prfiesta/pull/36#issuecomment-1564909558).
 
 You can find the full version history of package [here](https://pypi.org/project/prfiesta/#history)
```

