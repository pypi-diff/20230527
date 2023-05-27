# Comparing `tmp/git4net-0.0.0.tar.gz` & `tmp/git4net-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git4net-0.0.0.tar", last modified: Mon May 22 11:54:57 2023, max compression
+gzip compressed data, was "git4net-0.0.1.tar", last modified: Sat May 27 04:02:14 2023, max compression
```

## Comparing `git4net-0.0.0.tar` & `git4net-0.0.1.tar`

### file list

```diff
@@ -1,26 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:54:57.906069 git4net-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-22 11:54:41.000000 git4net-0.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-05-22 11:54:57.906069 git4net-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-05-22 11:54:41.000000 git4net-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:54:57.902069 git4net-0.0.0/git2net/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-22 11:54:41.000000 git4net-0.0.0/git2net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-05-22 11:54:41.000000 git4net-0.0.0/git2net/command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    19362 2023-05-22 11:54:41.000000 git4net-0.0.0/git2net/complexity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-22 11:54:41.000000 git4net-0.0.0/git2net/disambiguation.py
--rw-r--r--   0 runner    (1001) docker     (123)    81636 2023-05-22 11:54:41.000000 git4net-0.0.0/git2net/extraction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:54:57.902069 git4net-0.0.0/git2net/helpers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:54:57.902069 git4net-0.0.0/git2net/helpers/binary-extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-22 11:54:41.000000 git4net-0.0.0/git2net/helpers/binary-extensions/binary-extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)    27015 2023-05-22 11:54:41.000000 git4net-0.0.0/git2net/visualisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:54:57.902069 git4net-0.0.0/git4net.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-05-22 11:54:57.000000 git4net-0.0.0/git4net.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-22 11:54:57.000000 git4net-0.0.0/git4net.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 11:54:57.000000 git4net-0.0.0/git4net.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 11:54:57.000000 git4net-0.0.0/git4net.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-22 11:54:57.000000 git4net-0.0.0/git4net.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 11:54:57.000000 git4net-0.0.0/git4net.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-22 11:54:41.000000 git4net-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-22 11:54:57.906069 git4net-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-22 11:54:41.000000 git4net-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:54:57.902069 git4net-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    35028 2023-05-22 11:54:41.000000 git4net-0.0.0/tests/test_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:02:14.111338 git4net-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-27 04:02:01.000000 git4net-0.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-05-27 04:02:14.111338 git4net-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-05-27 04:02:01.000000 git4net-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:02:14.111338 git4net-0.0.1/git4net/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-27 04:02:01.000000 git4net-0.0.1/git4net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-05-27 04:02:01.000000 git4net-0.0.1/git4net/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19362 2023-05-27 04:02:01.000000 git4net-0.0.1/git4net/complexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-27 04:02:01.000000 git4net-0.0.1/git4net/disambiguation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81642 2023-05-27 04:02:01.000000 git4net-0.0.1/git4net/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27015 2023-05-27 04:02:01.000000 git4net-0.0.1/git4net/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:02:14.111338 git4net-0.0.1/git4net.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-05-27 04:02:14.000000 git4net-0.0.1/git4net.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-27 04:02:14.000000 git4net-0.0.1/git4net.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 04:02:14.000000 git4net-0.0.1/git4net.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-27 04:02:14.000000 git4net-0.0.1/git4net.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-27 04:02:14.000000 git4net-0.0.1/git4net.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-27 04:02:14.000000 git4net-0.0.1/git4net.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-27 04:02:01.000000 git4net-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-27 04:02:14.111338 git4net-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-27 04:02:01.000000 git4net-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:02:14.111338 git4net-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    35028 2023-05-27 04:02:01.000000 git4net-0.0.1/tests/test_functions.py
```

### Comparing `git4net-0.0.0/LICENSE.txt` & `git4net-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `git4net-0.0.0/PKG-INFO` & `git4net-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git4net
-Version: 0.0.0
+Version: 0.0.1
 Summary: My short description for my project.
 Home-page: https://github.com/franceme/git4net
 Author: Miles Frantz
 Author-email: frantzme@vt.edu
 License: AGPL-3.0+
 Keywords: co-editing,networks,repository,mining,network,analysis
 Classifier: Programming Language :: Python
```

### Comparing `git4net-0.0.0/README.md` & `git4net-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `git4net-0.0.0/git2net/__init__.py` & `git4net-0.0.1/git4net/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 and time-stamped co-editing networks from git repositories.
 """
 
 from pkg_resources import get_distribution
 
 __author__ = "Christoph Gote"
 __email__ = "cgote@ethz.ch"
-__version__ = get_distribution('git2net').version
+__version__ = get_distribution('git4net').version
 
 from .extraction import mine_git_repo
 from .extraction import mine_github
 from .extraction import get_unified_changes
 from .extraction import get_commit_dag
 from .extraction import identify_file_renaming
 from .extraction import text_entropy
```

### Comparing `git4net-0.0.0/git2net/command_line.py` & `git4net-0.0.1/git4net/command_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import argparse
 import os
 import datetime
 
 
 def main():
-    parser = argparse.ArgumentParser(description=("Allows git2net to be used "
+    parser = argparse.ArgumentParser(description=("Allows git4net to be used "
                                                   "from the command line."))
 
     subparsers = parser.add_subparsers(dest='command',
                                        help=("Mine a repository, disambiguate "
                                              "author aliases, create graph "
                                              "projections, or compute file "
                                              "complexities for a git "
@@ -37,15 +37,15 @@
     graph = subparsers.add_parser('graph',
                                   description=("Generate graph projections "
                                                "from commit and edit "
                                                "information stored in a "
                                                "provided SQLite database. The "
                                                "database needs to be created "
                                                "using the 'mine' command in "
-                                               "git2net. Graphs will be output "
+                                               "git4net. Graphs will be output "
                                                "as csv files at the given "
                                                "path."))
 
     complexity = subparsers.add_parser('complexity',
                                        description=("Compute file complexities "
                                                     "for a given git repository. "
                                                     "The results are added to an "
@@ -167,15 +167,15 @@
     has_time = [graph_coedit, graph_bipartite, graph_coauthor,
                 graph_commit_editing]
     has_filename = [graph_commit_editing, graph_line_editing]
 
     for sp in graph_priojections:
         sp.add_argument('database',
                         help=("Path to the database previously mined with "
-                              "git2net."),
+                              "git4net."),
                         type=str)
         sp.add_argument('csvfile',
                         help=("Path where the resulting graph will be stored "
                               "as csv."),
                         type=str)
 
     for sp in has_time:
```

### Comparing `git4net-0.0.0/git2net/complexity.py` & `git4net-0.0.1/git4net/complexity.py`

 * *Files identical despite different names*

### Comparing `git4net-0.0.0/git2net/disambiguation.py` & `git4net-0.0.1/git4net/disambiguation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import gambit
 import sqlite3
 import pandas as pd
 
 
 def disambiguate_aliases_db(sqlite_db_file, method='gambit', **quargs):
     """
-    Disambiguates author aliases in a given SQLite database mined with `git2net`.
+    Disambiguates author aliases in a given SQLite database mined with `git4net`.
     The disambiguation is performed using the Python package `gambit`.
     Internally, `disambiguate_aliases_db` calls the function `gambit.disambiguate_aliases <https://github.com/gotec/gambit/blob/main/gambit/main.py>`_.
     
     :param str sqlite_db_file: path to SQLite database
     :param str method: disambiguation method from {"gambit", "bird", "simple"}
     :param \**quargs: hyperparameters for the gambit and bird algorithms;
         **gambit**:
```

### Comparing `git4net-0.0.0/git2net/extraction.py` & `git4net-0.0.1/git4net/extraction.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import sqlite3
 import os
 from subprocess import check_output
 
 import multiprocessing
 
-import pandas as pd
+import pandas as pdlizard
 from tqdm import tqdm
 from tqdm.contrib.logging import logging_redirect_tqdm
 import numpy as np
 from scipy.stats import entropy
 
 import pydriller as pydriller
 from Levenshtein import distance as lev_dist
@@ -23,15 +23,15 @@
 import pathpy as pp
 import re
 import lizard
 import collections
 import git
 from git.exc import GitCommandError
 
-from git2net import __version__
+from git4net import __version__
 
 import time
 import sys
 
 import json
 
 import contextlib
@@ -596,15 +596,15 @@
         # Levenshtein edit distance set to 0 to distinguish from deletion
         if extraction_settings['extract_text']:
             e['pre_text'] = None
             e['post_text'] = None
         e['levenshtein_dist'] = 0
 
     else:
-        LOG = logging.getLogger('git2net')
+        LOG = logging.getLogger('git4net')
         LOG.error(edit.type)
         raise Exception("Unexpected error in '_get_edit_details'.")
 
     return e
 
 
 def is_binary_file(filename, file_content):
@@ -1094,15 +1094,15 @@
     else:
         test_str = '{} <{}>'.format(name, email)
     out_str = git.Git(str(git_repo.path)).check_mailmap(test_str)
 
     matches = re.findall("^(.*) <(.*)>$", out_str)
     if len(matches) > 1:
         raise Exception(("Error in mailmap check. Please report on "
-                         "https://github.com/gotec/git2net."))
+                         "https://github.com/gotec/git4net."))
     elif len(matches) == 1:
         name, email = matches[0]
     # else name and email remain the same as the ones passed
 
     return name, email
 
 
@@ -1269,15 +1269,15 @@
         redirected_stderr = redirected_stderr_ctx_mgr.getvalue().strip()
 
         if redirected_stderr:
             # Something was written to stderr. This could be a real error, however, often 
             # it is just a notification that an exception was ignored while deleting an object
             # after the threading timeout triggered. In this case, we ignore the message.
             if not (redirected_stderr.startswith('Exception ignored in:') and \
-                    redirected_stderr.endswith('git2net.extraction.TimeoutException:')):
+                    redirected_stderr.endswith('git4net.extraction.TimeoutException:')):
                 extracted_result = {'commit': pd.DataFrame(), 'edits': pd.DataFrame()}
                 log = ('error', 'processing error: ' + commit.hash)
                 exception = redirected_stderr
 
         if pd.isnull(exception) and timeout.timed_out:
             log = ('warning', 'processing timeout: ' + commit.hash)
             extracted_result = {'commit': pd.DataFrame(), 'edits': pd.DataFrame()}
@@ -1294,25 +1294,25 @@
     :param tuple log: tuple of logging type and logging message if any were created, otherwise None
     :param str exception: text of exception if any was raised, otherwise None
     
     :return:
         log message will be written and exception raised if one occurred
     """
     
-    LOG = logging.getLogger('git2net')
+    LOG = logging.getLogger('git4net')
 
     if pd.notnull(log):
         if log[0] == 'warning':
             LOG.warning(log[1])
         elif log[0] == 'error':
             LOG.error(log[1])
             raise Exception(exception)
         else:
             Exception(("Not implemented logging type. Please report on "
-                       "https://github.com/gotec/git2net."))
+                       "https://github.com/gotec/git4net."))
 
             
 def _process_repo_serial(git_repo_dir, sqlite_db_file, commits,
                          extraction_settings):
     """
     Processes all commits in a given git repository in a serial manner.
 
@@ -1321,15 +1321,15 @@
     :param List[str] commits: list of commits that have to be processed
     :param dict extraction_settings: settings for the extraction
 
     :return:
         SQLite database will be written at specified location
     """
 
-    LOG = logging.getLogger('git2net')
+    LOG = logging.getLogger('git4net')
     
     for commit in tqdm(commits, desc='Serial'):
         with logging_redirect_tqdm(tqdm_class=tqdm):            
             args = {'git_repo_dir': git_repo_dir, 'commit_hash': commit.hash,
                     'extraction_settings': extraction_settings}
             res = _process_commit(args)
 
@@ -1364,15 +1364,15 @@
     :param List[str] commits: list of commits that are already in the database
     :param dict extraction_settings: settings for the extraction
 
     :return:
         SQLite database will be written at specified location
     """
 
-    LOG = logging.getLogger('git2net')
+    LOG = logging.getLogger('git4net')
     
     args = [{'git_repo_dir': git_repo_dir, 'commit_hash': commit.hash,
              'extraction_settings': extraction_settings}
             for commit in commits]
 
     with multiprocessing.Pool(extraction_settings['no_of_processes'],
                               initializer=_init,
@@ -1524,15 +1524,15 @@
     :param str git_repo_dir: path to the git repository that is mined
     :param str sqlite_db_file: path (including database name) where with sqlite database
     :param List[str] commits: only consider specific set of commits, considers all if empty
 
     :return:
         *bool* – True if all commits are included in the database, otherwise False
     """
-    LOG = logging.getLogger('git2net')
+    LOG = logging.getLogger('git4net')
     
     git_repo = pydriller.Git(git_repo_dir)
     if os.path.exists(sqlite_db_file):
         try:
             with sqlite3.connect(sqlite_db_file) as con:
                 try:
                     p_commits = set(x[0] for x in
@@ -1567,15 +1567,15 @@
 
     :param str git_repo_dir: path to the git repository that is mined
     :param str sqlite_db_file: path (including database name) where with sqlite database
 
     :return:
         *pandas.DataFrame* – dataframe with details on missing commits
     """
-    LOG = logging.getLogger('git2net')
+    LOG = logging.getLogger('git4net')
     
     git_repo = pydriller.Git(git_repo_dir)
     if os.path.exists(sqlite_db_file):
         try:
             with sqlite3.connect(sqlite_db_file) as con:
                 try:
                     p_commits = set(x[0] for x in
@@ -1590,15 +1590,15 @@
         raise Exception("Found no database at provided path.")
 
     commits = [c for c in git_repo.get_list_commits(all=all_branches)]
     if not p_commits.issubset({c.hash for c in commits}):
         raise Exception("The database does not match the provided repository.")
 
     no_of_commits = len({c.hash for c in commits})
-    LOG = logging.getLogger('git2net')
+    LOG = logging.getLogger('git4net')
     LOG.info('{} / {} ({:.2f}%) of commits were successfully mined.'.format(
         len(p_commits), no_of_commits,
         len(p_commits) / no_of_commits * 100))
 
     u_commits = [c for c in commits if c.hash not in p_commits]
 
     u_commit_info = {'hash': [],
@@ -1671,15 +1671,15 @@
     :param bool extract_text: extract the commit message and line texts
     :param bool extract_merges: process merges
     :param bool extract_merge_deletions: extract lines that are not accepted during a merge as 'deletions'
 
     :return:
         SQLite database will be written at specified location
     """
-    LOG = logging.getLogger('git2net')
+    LOG = logging.getLogger('git4net')
     
     git_version = check_output(['git', '--version']).strip().decode("utf-8")
 
     parsed_git_version = re.search(r'(\d+)\.(\d+)\.(\d+)', git_version) \
                            .groups()
 
     if int(parsed_git_version[0]) < 2 or \
@@ -1689,15 +1689,15 @@
                 (int(parsed_git_version[0]) == 2) and
                 (int(parsed_git_version[1]) < 11)
             ) or
             (int(parsed_git_version[1]) == 11) and
             (int(parsed_git_version[2]) == 0)
        ):
         raise Exception("Your system is using " + git_version +
-                        " which is not supported by git2net. " +
+                        " which is not supported by git4net. " +
                         " Please update to git >= 2.11.1")
 
     blame_options = _parse_blame_C(blame_C) + ['--show-number',
                                                '--line-porcelain']
     if blame_w:
         blame_options += ['-w']
 
@@ -1767,15 +1767,15 @@
                                      "was created with settings not matching "
                                      "the ones selected for the current run. A "
                                      "path to either no database or a database "
                                      "from a previously paused run with "
                                      "identical settings is required."))
         except sqlite3.OperationalError:
             raise Exception(("Found a database on provided path that was "
-                             "likely not created with git2net. A path to "
+                             "likely not created with git4net. A path to "
                              "either no database or a database from a "
                              "previously paused run with identical settings "
                              "is required."))
     else:
         LOG.info("Found no database on provided path. Starting from scratch.")
         try:
             repo_url = git_repo.repo.remotes.origin.url
@@ -1794,15 +1794,15 @@
                                                   'method',
                                                   'extract_text')
                         VALUES (:version,
                                 :repository,
                                 :date,
                                 :method,
                                 :extract_text)""",
-                        {'version': 'git2net ' + str(__version__),
+                        {'version': 'git4net ' + str(__version__),
                          'repository': repo_url,
                          'date': datetime.datetime.now()
                                          .strftime('%Y-%m-%d %H:%M:%S'),
                          'method': 'blocks' if use_blocks else 'lines',
                          'extract_text': str(extract_text)})
             con.commit()
             p_commits = set()
@@ -1868,15 +1868,15 @@
     :param str branch: The branch of the github project that will be checked out and mined. If no branch is provided the default branch of the repository is used.
     :param \**kwargs: arguments that will be passed on to mine_git_repo
 
     :return:
         - git repository will be cloned to specified location
         - SQLite database will be written at specified location
     """
-    LOG = logging.getLogger('git2net')    
+    LOG = logging.getLogger('git4net')    
     
     # github_url can either be provided as full url or as in form <USER>/<REPO>
     user_repo_pattern = r'^([^\/]*)\/([^\/]*)$'
     full_url_pattern = r'^https:\/\/github\.com\/([^\/]*)\/([^\/.]*)(\.git)?$'
 
     match = re.match(user_repo_pattern, github_url)
     if match:
```

### Comparing `git4net-0.0.0/git2net/visualisation.py` & `git4net-0.0.1/git4net/visualisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,40 +20,40 @@
 
 def _ensure_author_id_exists(sqlite_db_file):
     with sqlite3.connect(sqlite_db_file) as con:
         cur = con.cursor()
         cols = [i[1] for i in cur.execute('PRAGMA table_info(commits)')]
         if 'author_id' not in cols:
             raise Exception("The author_id is not yet computed. To use author_id as identifier, please " + 
-                            "run git2net.disambiguate_aliases_db on the database before visualisation.")
+                            "run git4net.disambiguate_aliases_db on the database before visualisation.")
         elif pd.isnull(pd.read_sql('''SELECT author_id FROM commits''', con).author_id).sum() > 0:
             raise Exception("The author_id is missing entries. To use author_id as identifier, please " + 
-                            "rerun git2net.disambiguate_aliases_db on the database before visualisation.")
+                            "rerun git4net.disambiguate_aliases_db on the database before visualisation.")
     return True
                 
 def get_line_editing_paths(sqlite_db_file, git_repo_dir, author_identifier='author_id', commit_hashes=None,
                            file_paths=None, with_start=False, merge_renaming=False):
     """
     Returns line editing DAG as well as line editing paths.
 
-    :param str sqlite_db_file: path to SQLite database mined with git2net line method
+    :param str sqlite_db_file: path to SQLite database mined with git4net line method
     :param str git_repo_dir: path to the git repository that is mined
     :param List[str] commit_hashes: list of commits to consider, by default all commits are considered
     :param List[str] file_paths: list of files to consider, by default all files are considered
     :param bool with_start: determines if node for filename is included as start for all editing paths
     :param bool merge_renaming: determines if file renaming is considered
 
     :return:
         - *pathpy.Paths* – line editing paths
         - *pathpy.DAG* – line editing directed acyclic graph
         - *dict* – info on node charactaristics
         - *dict* – info on edge characteristics
     """
 
-    LOG = logging.getLogger('git2net')
+    LOG = logging.getLogger('git4net')
     
     if author_identifier == 'author_id':
         _ensure_author_id_exists(sqlite_db_file)
     
     # Connect to provided database.
     con = sqlite3.connect(sqlite_db_file)
 
@@ -61,15 +61,15 @@
     try:
         path = con.execute("SELECT repository FROM _metadata").fetchall()[0][0]
         method = con.execute("SELECT method FROM _metadata").fetchall()[0][0]
         if method == 'blocks':
             raise Exception("Invalid database. A database mined with 'use_blocks=False' is " +
                             "required.")
     except sqlite3.OperationalError:
-        raise Exception("You either provided no database or a database not created with git2net. " +
+        raise Exception("You either provided no database or a database not created with git4net. " +
                         "Please provide a valid datatabase mined with 'use_blocks=False'.")
 
     if file_paths is not None:
         assert type(file_paths) is list
 
     if merge_renaming:
         LOG.info('Searching for aliases')
@@ -226,15 +226,15 @@
                     node_info['time'][target] = edit.author_date
                     node_info['time'][source_addition] = edit.author_date_addition
             elif edit.edit_type == 'file_renaming' or edit.edit_type == 'binary_file_change':
                 pass
             else:
                 raise Exception("Unexpected error in 'extract_editing_paths' ({})."
                                     .format(edit.edit_type) + " Please report on " +
-                                "https://github.com/gotec/git2net.")
+                                "https://github.com/gotec/git4net.")
 
     for node in tqdm(dag.nodes):
         if node in file_paths_dag:
             node_info['colors'][node] = 'gray'
         else:
             if '#FBB13C' in [edge_info['colors'][n] for n in [(x, node)
                                                     for x in dag.predecessors[node]]]:
```

### Comparing `git4net-0.0.0/git4net.egg-info/PKG-INFO` & `git4net-0.0.1/git4net.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git4net
-Version: 0.0.0
+Version: 0.0.1
 Summary: My short description for my project.
 Home-page: https://github.com/franceme/git4net
 Author: Miles Frantz
 Author-email: frantzme@vt.edu
 License: AGPL-3.0+
 Keywords: co-editing,networks,repository,mining,network,analysis
 Classifier: Programming Language :: Python
```

### Comparing `git4net-0.0.0/setup.cfg` & `git4net-0.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `git4net-0.0.0/setup.py` & `git4net-0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 EMAIL = 'frantzme@vt.edu'
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
-entry_point = f"git2net"
-VERSION = "0.0.0"
+entry_point = f"git4net"
+VERSION = "0.0.1"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

### Comparing `git4net-0.0.0/tests/test_functions.py` & `git4net-0.0.1/tests/test_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import git2net
+import git4net
 import pathpy as pp
 import pytest
 import pydriller
 import numpy as np
 import lizard
 import os
 from datetime import datetime
@@ -15,25 +15,25 @@
 
 @pytest.fixture(scope="function")
 def git_repo_dir():
     yield 'test_repos/test_repo_1'
 
 @pytest.fixture(scope="function")
 def github_repo_dir():
-    repo_dir = 'test_repos/git2net_test'
+    repo_dir = 'test_repos/git4net_test'
     yield repo_dir
     shutil.rmtree(repo_dir)
     
 @pytest.fixture(scope="function")
 def github_url_short():
-    yield 'gotec/git2net'
+    yield 'gotec/git4net'
     
 @pytest.fixture(scope="function")
 def github_url_full():
-    yield 'https://github.com/gotec/git2net'
+    yield 'https://github.com/gotec/git4net'
 
 @pytest.fixture(scope="function")
 def github_url_invalid():
     yield 'invalid'
 
 @pytest.fixture(scope="function")
 def sqlite_db_file():
@@ -46,15 +46,15 @@
 
     
 def test_get_commit_dag(git_repo_dir):
     print('rootdir', [f for f in os.listdir('.')])
     print('rootdir-1', [f for f in os.listdir('test_repos')])
     print('test_repos', [f for f in os.listdir('test_repos/test_repo_1')])
     
-    dag = git2net.get_commit_dag(git_repo_dir)
+    dag = git4net.get_commit_dag(git_repo_dir)
     expected_edges = [('e4448e8', 'f343ed5'), ('f343ed5', '6b531fc'), ('6b531fc', 'b17c2c3'),
                       ('b17c2c3', '2b00f48'), ('2b00f48', '59da499'), ('2b00f48', 'b21583e'),
                       ('b21583e', '7d140b9'), ('59da499', '7d140b9'), ('7d140b9', '9e28e38'),
                       ('7d140b9', '16bbc87'), ('9e28e38', '080220d'), ('16bbc87', '080220d'),
                       ('16bbc87', 'eadd9d4'), ('080220d', '02b4a6f'), ('02b4a6f', '9798c44'),
                       ('eadd9d4', '9798c44'), ('9798c44', '2f4f139'), ('9798c44', '2ce5105'),
                       ('2ce5105', '9602507'), ('2f4f139', '9602507'), ('9602507', '2edf3d9'),
@@ -80,15 +80,15 @@
                            'blame_options': ['-C', '-C', '-C4', '--show-number', '--line-porcelain'],
                            'extract_complexity': True,
                            'extract_text': True}
     git_repo = pydriller.Git(git_repo_dir)
     commit = git_repo.get_commit(commit_hash)
     for mod in commit.modified_files:
         if mod.filename == filename:
-            df = git2net.extraction._extract_edits(git_repo, commit, mod, extraction_settings)
+            df = git4net.extraction._extract_edits(git_repo, commit, mod, extraction_settings)
             
     assert len(df) == 3
     assert df.at[0, 'original_commit_addition'] == 'e4448e87541d19d139b9d033b2578941a53d1f97'
     assert df.at[1, 'original_commit_addition'] == '6b531fcb57d5b9d98dd983cb65357d82ccca647b'
     assert df.at[2, 'original_commit_addition'] == None # as there is no match due to line ending
     # to obtain match, the -w option is required in git blame, however this leads to wrong matches
     # with lines that were not copied.
@@ -104,15 +104,15 @@
                            'extract_text': True}
     
     git_repo = pydriller.Git(git_repo_dir)
     commit = git_repo.get_commit(commit_hash)
     df = None
     for mod in commit.modified_files:
         if mod.filename == filename:
-            df = git2net.extraction._extract_edits(git_repo, commit, mod, extraction_settings)
+            df = git4net.extraction._extract_edits(git_repo, commit, mod, extraction_settings)
     assert len(df) == 1
     assert df.at[0, 'original_commit_addition'] == 'not available with use_blocks'
 
 
 def test_identify_edits(git_repo_dir):
     commit_hash = 'f343ed53ee64717f85135c4b8d3f6bd018be80ad'
     filename = 'text_file.txt'
@@ -126,15 +126,15 @@
             mod = x
 
     parsed_lines = mod.diff_parsed
 
     deleted_lines = { x[0]:x[1] for x in parsed_lines['deleted'] }
     added_lines = { x[0]:x[1] for x in parsed_lines['added'] }
 
-    _, edits = git2net.extraction._identify_edits(deleted_lines, added_lines, extraction_settings)
+    _, edits = git4net.extraction._identify_edits(deleted_lines, added_lines, extraction_settings)
     assert list(edits.type) == ['deletion', 'replacement', 'deletion', 'replacement', 'addition',
                                 'addition', 'addition']
 
 def test_process_commit(git_repo_dir):
     commit_hash = 'f343ed53ee64717f85135c4b8d3f6bd018be80ad'
     
     extraction_settings = {'use_blocks': False,
@@ -146,158 +146,158 @@
                            'extract_text': True,
                            'extract_complexity': True,
                            'timeout': 0}
     
     args = {'git_repo_dir': git_repo_dir, 'commit_hash': commit_hash,
             'extraction_settings': extraction_settings}
 
-    res_dict, _, _ = git2net.extraction._process_commit(args)
+    res_dict, _, _ = git4net.extraction._process_commit(args)
     assert list(res_dict.keys()) == ['commit', 'edits']
 
 
 def test_get_unified_changes(git_repo_dir):
     commit_hash = 'e8be9c6abe76c809a567866e411350e76eb45e49'
     filename = 'text_file.txt'
-    unified_changes = git2net.get_unified_changes(git_repo_dir, commit_hash, filename)
+    unified_changes = git4net.get_unified_changes(git_repo_dir, commit_hash, filename)
     expected_code = ['A0', 'B1', 'B2', 'B3', 'A1', 'C2', 'C3', 'C4', 'B2', 'B3', 'B4', 'A5', 'A6',
                      'A7', 'F8', 'F9', 'F10', 'F11', 'F12', 'B8', 'B9', 'B10', 'B11', 'B12']
     assert list(unified_changes.code) == expected_code
 
 
 def test_mine_git_repo_sequential(git_repo_dir, sqlite_db_file):
-    git2net.mine_git_repo(git_repo_dir, sqlite_db_file, blame_C='CCC4', no_of_processes=1)
-    assert git2net.check_mining_complete(git_repo_dir, sqlite_db_file)
+    git4net.mine_git_repo(git_repo_dir, sqlite_db_file, blame_C='CCC4', no_of_processes=1)
+    assert git4net.check_mining_complete(git_repo_dir, sqlite_db_file)
 
 
 def test_mine_git_repo(git_repo_dir, sqlite_db_file):
-    git2net.mine_git_repo(git_repo_dir, sqlite_db_file, blame_C='CCC4', extract_merge_deletions=True,
+    git4net.mine_git_repo(git_repo_dir, sqlite_db_file, blame_C='CCC4', extract_merge_deletions=True,
                           extract_merges=True, extract_text=True)
-    assert git2net.check_mining_complete(git_repo_dir, sqlite_db_file)
+    assert git4net.check_mining_complete(git_repo_dir, sqlite_db_file)
 
 def test_disambiguation(git_repo_dir, sqlite_db_file):
-    git2net.mine_git_repo(git_repo_dir, sqlite_db_file)
-    git2net.disambiguate_aliases_db(sqlite_db_file)
+    git4net.mine_git_repo(git_repo_dir, sqlite_db_file)
+    git4net.disambiguate_aliases_db(sqlite_db_file)
     
     with sqlite3.connect(sqlite_db_file) as con:
         author_id = pd.read_sql('SELECT author_id FROM commits', con)
     
     assert not author_id.empty
 
 def test_get_line_editing_paths_1(sqlite_db_file, git_repo_dir):
     # No database exists
     with pytest.raises(Exception) as e:
-        _ = git2net.get_line_editing_paths(sqlite_db_file, git_repo_dir, author_identifier='author_name')
+        _ = git4net.get_line_editing_paths(sqlite_db_file, git_repo_dir, author_identifier='author_name')
     assert e.value.args[0].startswith('You either provided no database')
 
         
 def test_get_line_editing_paths_2(sqlite_db_file, git_repo_dir):
     # An empty database exists
     with sqlite3.connect(sqlite_db_file) as con:
-        pd.DataFrame().to_sql('git2net', con)
+        pd.DataFrame().to_sql('git4net', con)
     with pytest.raises(Exception) as e:
-        _ = git2net.get_line_editing_paths(sqlite_db_file, git_repo_dir, author_identifier='author_name')
+        _ = git4net.get_line_editing_paths(sqlite_db_file, git_repo_dir, author_identifier='author_name')
     assert e.value.args[0].startswith('You either provided no database')
     
     
 def test_get_line_editing_paths_3(sqlite_db_file, git_repo_dir):
-    git2net.mine_git_repo(git_repo_dir, sqlite_db_file, use_blocks=True)
+    git4net.mine_git_repo(git_repo_dir, sqlite_db_file, use_blocks=True)
     
     with sqlite3.connect(sqlite_db_file) as con:
-        pd.DataFrame().to_sql('git2net', con)
+        pd.DataFrame().to_sql('git4net', con)
     with pytest.raises(Exception) as e:
-        _ = git2net.get_line_editing_paths(sqlite_db_file, git_repo_dir, author_identifier='author_name')
+        _ = git4net.get_line_editing_paths(sqlite_db_file, git_repo_dir, author_identifier='author_name')
     assert e.value.args[0].startswith('Invalid database. A database mined with')
     
     
 def test_get_line_editing_paths_4(sqlite_db_file, git_repo_dir):
-    git2net.mine_git_repo(git_repo_dir, sqlite_db_file)
-    git2net.disambiguate_aliases_db(sqlite_db_file)
+    git4net.mine_git_repo(git_repo_dir, sqlite_db_file)
+    git4net.disambiguate_aliases_db(sqlite_db_file)
     
-    paths, dag, node_info, edge_info = git2net.get_line_editing_paths(sqlite_db_file, git_repo_dir,
+    paths, dag, node_info, edge_info = git4net.get_line_editing_paths(sqlite_db_file, git_repo_dir,
                                                                       with_start=True)
     
     assert len(dag.isolate_nodes()) == 0
     
-    _ = git2net.get_line_editing_paths(sqlite_db_file, git_repo_dir,
+    _ = git4net.get_line_editing_paths(sqlite_db_file, git_repo_dir,
                                        with_start=False,
                                        commit_hashes= ['e4448e87541d19d139b9d033b2578941a53d1f97',
                                                        'f343ed53ee64717f85135c4b8d3f6bd018be80ad', 
                                                        '6b531fcb57d5b9d98dd983cb65357d82ccca647b', 
                                                        'b17c2c321ce8d299de3d063ca0a1b0b363477505', 
                                                        '2b00f48ff42cf5c12646cb0553e5481b49bd78f7'],
                                        author_identifier='author_name')
-    _ = git2net.get_line_editing_paths(sqlite_db_file, git_repo_dir,
+    _ = git4net.get_line_editing_paths(sqlite_db_file, git_repo_dir,
                                        with_start=True, merge_renaming=True,
                                        file_paths=['text_file.txt'],
                                        author_identifier='author_email')
     
     with pytest.raises(Exception) as e:
-        _ = git2net.get_line_editing_paths(sqlite_db_file, git_repo_dir,
+        _ = git4net.get_line_editing_paths(sqlite_db_file, git_repo_dir,
                                            with_start=True,
                                            author_identifier='invalid')
     assert e.value.args[0].startswith('author_identifier must be from')
     
     
 
 
 def test_get_commit_editing_dag_1(sqlite_db_file, git_repo_dir):
-    git2net.mine_git_repo(git_repo_dir, sqlite_db_file, blame_C='CCC4', extract_merge_deletions=True,
+    git4net.mine_git_repo(git_repo_dir, sqlite_db_file, blame_C='CCC4', extract_merge_deletions=True,
                           extract_merges=True, extract_text=True)
     
-    dag, node_info, edge_info = git2net.get_commit_editing_dag(sqlite_db_file)
+    dag, node_info, edge_info = git4net.get_commit_editing_dag(sqlite_db_file)
 
     assert len(dag.isolate_nodes()) == 0
     assert len(dag.nodes) == 36
     assert len(dag.successors[None]) == 12
 
 
 def test_get_commit_editing_dag_2(sqlite_db_file, git_repo_dir):
-    git2net.mine_git_repo(git_repo_dir, sqlite_db_file, blame_C='CCC4', extract_merge_deletions=True,
+    git4net.mine_git_repo(git_repo_dir, sqlite_db_file, blame_C='CCC4', extract_merge_deletions=True,
                           extract_merges=True, extract_text=True)
     
     time_from = datetime(2019, 2, 12, 11, 0, 0)
     time_to = datetime(2019, 2, 12, 12, 0, 0)
 
-    dag, node_info, edge_info = git2net.get_commit_editing_dag(sqlite_db_file,
+    dag, node_info, edge_info = git4net.get_commit_editing_dag(sqlite_db_file,
                                                                time_from=time_from,
                                                                time_to=time_to)
 
     assert len(dag.isolate_nodes()) == 0
     assert len(dag.nodes) == 15
     assert len(dag.successors[None]) == 6
 
 
 def test_get_commit_editing_dag_3(sqlite_db_file, git_repo_dir):
-    git2net.mine_git_repo(git_repo_dir, sqlite_db_file, blame_C='CCC4', extract_merge_deletions=True,
+    git4net.mine_git_repo(git_repo_dir, sqlite_db_file, blame_C='CCC4', extract_merge_deletions=True,
                           extract_merges=True, extract_text=True)
     
     time_from = datetime(2019, 2, 12, 12, 0, 0)
     time_to = datetime(2019, 2, 12, 13, 0, 0)
     filename = 'text_file.txt'
 
-    dag, node_info, edge_info = git2net.get_commit_editing_dag(sqlite_db_file,
+    dag, node_info, edge_info = git4net.get_commit_editing_dag(sqlite_db_file,
                                                                time_from=time_from,
                                                                time_to=time_to,
                                                                filename=filename)
 
     assert len(dag.isolate_nodes()) == 0
     assert len(dag.nodes) == 17
     assert len(dag.successors[None]) == 1
 
 
 def test_get_coediting_network(sqlite_db_file, git_repo_dir):
-    git2net.mine_git_repo(git_repo_dir, sqlite_db_file)
-    git2net.disambiguate_aliases_db(sqlite_db_file)
+    git4net.mine_git_repo(git_repo_dir, sqlite_db_file)
+    git4net.disambiguate_aliases_db(sqlite_db_file)
     
-    _ = git2net.get_coediting_network(sqlite_db_file)
+    _ = git4net.get_coediting_network(sqlite_db_file)
     
     time_from = datetime(2019, 2, 12, 11, 0, 0)
     time_to = datetime(2019, 2, 12, 11, 15, 0)
 
-    t, node_info, edge_info = git2net.get_coediting_network(sqlite_db_file, time_from=time_from,
+    t, node_info, edge_info = git4net.get_coediting_network(sqlite_db_file, time_from=time_from,
                                                             time_to=time_to)
 
     expected_edges = [('Author B', 'Author A', 1549965657),
                       ('Author A', 'Author B', 1549966134),
                       ('Author B', 'Author A', 1549966184),
                       ('Author C', 'Author B', 1549966309),
                       ('Author C', 'Author A', 1549966309),
@@ -306,88 +306,88 @@
                       ('Author B', 'Author A', 1549965738),
                       ('Author C', 'Author A', 1549966451),
                       ('Author C', 'Author A', 1549966451),
                       ('Author C', 'Author A', 1549966451)]
 
     assert len(set(t.tedges).difference(set(expected_edges))) == 0
 
-    t, node_info, edge_info = git2net.get_coediting_network(sqlite_db_file, time_from=time_from,
+    t, node_info, edge_info = git4net.get_coediting_network(sqlite_db_file, time_from=time_from,
                                                             time_to=time_to,
                                                             author_identifier='author_name')
-    t, node_info, edge_info = git2net.get_coediting_network(sqlite_db_file, time_from=time_from,
+    t, node_info, edge_info = git4net.get_coediting_network(sqlite_db_file, time_from=time_from,
                                                             time_to=time_to,
                                                             author_identifier='author_email')
     
     with pytest.raises(Exception) as e:
-        t, node_info, edge_info = git2net.get_coediting_network(sqlite_db_file, time_from=time_from,
+        t, node_info, edge_info = git4net.get_coediting_network(sqlite_db_file, time_from=time_from,
                                                                 time_to=time_to,
                                                                 author_identifier='invalid')
     assert e.value.args[0].startswith('author_identifier must be from')
     
     
     
     
 
 def test_get_coauthorship_network(sqlite_db_file, git_repo_dir):
-    git2net.mine_git_repo(git_repo_dir, sqlite_db_file)
-    git2net.disambiguate_aliases_db(sqlite_db_file)
+    git4net.mine_git_repo(git_repo_dir, sqlite_db_file)
+    git4net.disambiguate_aliases_db(sqlite_db_file)
     
     time_from = datetime(2019, 2, 12, 12, 0, 0)
     time_to = datetime(2019, 2, 12, 12, 15, 0)
 
-    n, node_info, edge_info = git2net.get_coauthorship_network(sqlite_db_file, time_from=time_from,
+    n, node_info, edge_info = git4net.get_coauthorship_network(sqlite_db_file, time_from=time_from,
                                                                time_to=time_to)
 
     expected_nonzero_rows = [0, 0, 1, 1, 2, 2]
     expected_nonzero_columns = [1, 2, 0, 2, 0, 1]
 
     assert list(n.adjacency_matrix().nonzero()[0]) == expected_nonzero_rows
     assert list(n.adjacency_matrix().nonzero()[1]) == expected_nonzero_columns
     
-    n, node_info, edge_info = git2net.get_coauthorship_network(sqlite_db_file, time_from=time_from,
+    n, node_info, edge_info = git4net.get_coauthorship_network(sqlite_db_file, time_from=time_from,
                                                                time_to=time_to,
                                                                author_identifier='author_name')
-    n, node_info, edge_info = git2net.get_coauthorship_network(sqlite_db_file, time_from=time_from,
+    n, node_info, edge_info = git4net.get_coauthorship_network(sqlite_db_file, time_from=time_from,
                                                                time_to=time_to,
                                                                author_identifier='author_email')
     
     with pytest.raises(Exception) as e:
-        n, node_info, edge_info = git2net.get_coauthorship_network(sqlite_db_file, time_from=time_from,
+        n, node_info, edge_info = git4net.get_coauthorship_network(sqlite_db_file, time_from=time_from,
                                                                    time_to=time_to,
                                                                    author_identifier='invalid')
     assert e.value.args[0].startswith('author_identifier must be from')
 
 
 def test_get_bipartite_network(sqlite_db_file, git_repo_dir):
-    git2net.mine_git_repo(git_repo_dir, sqlite_db_file)
-    git2net.disambiguate_aliases_db(sqlite_db_file)
+    git4net.mine_git_repo(git_repo_dir, sqlite_db_file)
+    git4net.disambiguate_aliases_db(sqlite_db_file)
     
     time_from = datetime(2019, 2, 12, 11, 0, 0)
     time_to = datetime(2019, 2, 12, 11, 10, 0)
 
-    t, node_info, edge_info = git2net.get_bipartite_network(sqlite_db_file, time_from=time_from,
+    t, node_info, edge_info = git4net.get_bipartite_network(sqlite_db_file, time_from=time_from,
                                                             time_to=time_to)
 
     expected_edges = [('Author A', 'text_file.txt', 1549965641),
     ('Author B', 'text_file.txt', 1549965657),
     ('Author A', 'text_file.txt', 1549966134),
     ('Author B', 'text_file.txt', 1549966184),
     ('Author B', 'text_file.txt', 1549965738)]
 
     assert len(set(t.tedges).difference(set(expected_edges))) == 0
 
-    t, node_info, edge_info = git2net.get_bipartite_network(sqlite_db_file, time_from=time_from,
+    t, node_info, edge_info = git4net.get_bipartite_network(sqlite_db_file, time_from=time_from,
                                                             time_to=time_to,
                                                             author_identifier='author_name')
-    t, node_info, edge_info = git2net.get_bipartite_network(sqlite_db_file, time_from=time_from,
+    t, node_info, edge_info = git4net.get_bipartite_network(sqlite_db_file, time_from=time_from,
                                                             time_to=time_to,
                                                             author_identifier='author_email')
     
     with pytest.raises(Exception) as e:
-        t, node_info, edge_info = git2net.get_bipartite_network(sqlite_db_file, time_from=time_from,
+        t, node_info, edge_info = git4net.get_bipartite_network(sqlite_db_file, time_from=time_from,
                                                                 time_to=time_to,
                                                                 author_identifier='invalid')
     assert e.value.args[0].startswith('author_identifier must be from')
         
     
 def test_process_commit_merge(git_repo_dir):
     commit_hash = 'dcf060d5aa93077c84552ce6ed56a0f0a37e4dca'
@@ -402,15 +402,15 @@
                            'extract_merges': True,
                            'extract_complexity': True,
                            'extract_merge_deletions': True}
     
     args = {'git_repo_dir': git_repo_dir, 'commit_hash': commit_hash,
             'extraction_settings': extraction_settings}
 
-    res_dict, _, _ = git2net.extraction._process_commit(args)
+    res_dict, _, _ = git4net.extraction._process_commit(args)
 
     assert list(res_dict['edits']['edit_type']) == ['deletion']*7
     assert list(res_dict['edits']['pre_starting_line_no']) == [6,7,8,12,13,1,2]
 
 
 def test_process_commit_merge2(git_repo_dir):
     commit_hash = '96025072a3e1b2f466ef56053bbdf4c9c0e927f0'
@@ -425,15 +425,15 @@
                            'extract_merges': True,
                            'extract_complexity': True,
                            'extract_merge_deletions': True}
     
     args = {'git_repo_dir': git_repo_dir, 'commit_hash': commit_hash,
             'extraction_settings': extraction_settings}
 
-    res_dict, _, _ = git2net.extraction._process_commit(args)
+    res_dict, _, _ = git4net.extraction._process_commit(args)
 
     assert list(res_dict['edits']['edit_type']) == ['replacement']*6
     assert list(res_dict['edits']['pre_starting_line_no']) == [1,2,3,1,2,3]
     
     
 def test_compute_halstead_effort():
     filename = 'test.c'
@@ -443,32 +443,32 @@
                       int a, b, c, avg;
                       scanf("%d %d %d", &a, &b, &c);
                       avg = (a+b+c)/3;
                       printf("avg = %d", avg);
                   }
                   """
     
-    unknown_filename = 'test.git2net'
+    unknown_filename = 'test.git4net'
     
-    HE = git2net.complexity._compute_halstead_effort(filename, source_code)
-    HE_unknown = git2net.complexity._compute_halstead_effort(unknown_filename, source_code)
+    HE = git4net.complexity._compute_halstead_effort(filename, source_code)
+    HE_unknown = git4net.complexity._compute_halstead_effort(unknown_filename, source_code)
     assert HE == 2196.1587113893806 # obtained from run of multimetric
     assert HE_unknown == 0
     
     
 def test_compute_complexity_measures(git_repo_dir):
     # Addition
-    args = {'git_repo_dir': '../git2net/test_repos/test_repo_1/',
+    args = {'git_repo_dir': '../git4net/test_repos/test_repo_1/',
             'commit_hash': 'e4448e87541d19d139b9d033b2578941a53d1f97',
             'old_path': 'None',
             'new_path': 'text_file.txt',
             'events': -1,
             'levenshtein_distance': -1}
 
-    res = git2net.complexity._compute_complexity_measures(args)
+    res = git4net.complexity._compute_complexity_measures(args)
 
     assert res.old_path.values[0] == args['old_path']
     assert res.new_path.values[0] == args['new_path']
     assert res.events.values[0] == args['events']
     assert res.levenshtein_distance.values[0] == args['levenshtein_distance']
     assert res.HE_pre.values[0] == 0
     assert res.CCN_pre.values[0] == 0
@@ -483,22 +483,22 @@
     assert res.HE_delta.values[0] == 1
     assert res.CCN_delta.values[0] == 0
     assert res.NLOC_delta.values[0] == 10
     assert res.TOK_delta.values[0] == 10
     assert res.FUN_delta.values[0] == 0
     
     # Replacement
-    args = {'git_repo_dir': '../git2net/test_repos/test_repo_1/',
+    args = {'git_repo_dir': '../git4net/test_repos/test_repo_1/',
             'commit_hash': 'b17c2c321ce8d299de3d063ca0a1b0b363477505',
             'old_path': 'text_file.txt',
             'new_path': 'text_file.txt',
             'events': -1,
             'levenshtein_distance': -1}
     
-    res = git2net.complexity._compute_complexity_measures(args)
+    res = git4net.complexity._compute_complexity_measures(args)
 
     assert res.old_path.values[0] == args['old_path']
     assert res.new_path.values[0] == args['new_path']
     assert res.events.values[0] == args['events']
     assert res.levenshtein_distance.values[0] == args['levenshtein_distance']
     assert res.HE_pre.values[0] == 1
     assert res.CCN_pre.values[0] == 0
@@ -514,22 +514,22 @@
     assert res.CCN_delta.values[0] == 0
     assert res.NLOC_delta.values[0] == -6
     assert res.TOK_delta.values[0] == -6
     assert res.FUN_delta.values[0] == 0
     
     
     # Deletion
-    args = {'git_repo_dir': '../git2net/test_repos/test_repo_1/',
+    args = {'git_repo_dir': '../git4net/test_repos/test_repo_1/',
             'commit_hash': '7df20cba2ba34e1e316d19a23e4f573e1007ec75',
             'old_path': 'test_file_2.txt',
             'new_path': 'None',
             'events': -1,
             'levenshtein_distance': -1}
     
-    res = git2net.complexity._compute_complexity_measures(args)
+    res = git4net.complexity._compute_complexity_measures(args)
 
     assert res.old_path.values[0] == args['old_path']
     assert res.new_path.values[0] == args['new_path']
     assert res.events.values[0] == args['events']
     assert res.levenshtein_distance.values[0] == args['levenshtein_distance']
     assert res.HE_pre.values[0] == 1
     assert res.CCN_pre.values[0] == 0
@@ -545,168 +545,168 @@
     assert res.CCN_delta.values[0] == 0
     assert res.NLOC_delta.values[0] == -10
     assert res.TOK_delta.values[0] == -10
     assert res.FUN_delta.values[0] == 0
     
     
 def test_compute_complexity(git_repo_dir, sqlite_db_file):
-    git2net.mine_git_repo(git_repo_dir, sqlite_db_file)
+    git4net.mine_git_repo(git_repo_dir, sqlite_db_file)
     
     # compute the complexity for everything in the database
-    git2net.compute_complexity(git_repo_dir, sqlite_db_file, read_chunksize = 1, write_chunksize = 20)
+    git4net.compute_complexity(git_repo_dir, sqlite_db_file, read_chunksize = 1, write_chunksize = 20)
     
     with sqlite3.connect(sqlite_db_file) as con:
         complexity = pd.read_sql('SELECT * FROM complexity', con)
     
     assert not complexity.empty
     
     # Repeat the computation. Now nothing should happen.
-    git2net.compute_complexity(git_repo_dir, sqlite_db_file)
+    git4net.compute_complexity(git_repo_dir, sqlite_db_file)
         
     with sqlite3.connect(sqlite_db_file) as con:
         complexity2 = pd.read_sql('SELECT * FROM complexity', con)
         
     assert complexity.equals(complexity2)
     
     
 def test_Timeout():
     finished = False
-    with git2net.extraction.Timeout(2) as timeout:
+    with git4net.extraction.Timeout(2) as timeout:
         time.sleep(10)
         finished = True
     assert not finished
     assert timeout.timed_out
     
     finished = False
-    with git2net.extraction.Timeout(2) as timeout:
+    with git4net.extraction.Timeout(2) as timeout:
         time.sleep(1)
         finished = True
     assert finished
     assert not timeout.timed_out
     
     
 def test_mine_github(github_url_short, github_repo_dir, sqlite_db_file):
-    git2net.mine_github(github_url_short, github_repo_dir, sqlite_db_file)
-    assert git2net.check_mining_complete(github_repo_dir, sqlite_db_file)
+    git4net.mine_github(github_url_short, github_repo_dir, sqlite_db_file)
+    assert git4net.check_mining_complete(github_repo_dir, sqlite_db_file)
 
     
 def test_mine_github_2(github_url_full, github_repo_dir, sqlite_db_file):
-    git2net.mine_github(github_url_full, github_repo_dir, sqlite_db_file, branch='object-oriented', use_blocks=True)
-    assert git2net.check_mining_complete(github_repo_dir, sqlite_db_file)
+    git4net.mine_github(github_url_full, github_repo_dir, sqlite_db_file, branch='object-oriented', use_blocks=True)
+    assert git4net.check_mining_complete(github_repo_dir, sqlite_db_file)
     
     
 def test_mine_github_3(github_url_invalid):
     github_repo_dir = 'invalid'
     sqlite_db_file = 'invalid'
     
     with pytest.raises(Exception) as e:
-        git2net.mine_github(github_url_invalid, github_repo_dir, sqlite_db_file)
+        git4net.mine_github(github_url_invalid, github_repo_dir, sqlite_db_file)
     assert e.value.args[0].startswith('Invalid github_url provided.')
 
         
 def test_mine_git_repo_resume(github_url_full, github_repo_dir, sqlite_db_file):
     local_directory = '/'.join(github_repo_dir.split('/')[:-1])
     git_repo_folder = github_repo_dir.split('/')[-1]
     
     git.Git(local_directory).clone(github_url_full, git_repo_folder)
     
     with pytest.raises(Exception) as e:
-        git2net.mining_state_summary(github_repo_dir, sqlite_db_file, all_branches=True)
+        git4net.mining_state_summary(github_repo_dir, sqlite_db_file, all_branches=True)
     assert e.value.args[0].startswith('Found no database at provided path.')
         
     with pytest.raises(Exception) as e:
-        git2net.check_mining_complete(github_repo_dir, sqlite_db_file)
+        git4net.check_mining_complete(github_repo_dir, sqlite_db_file)
     assert e.value.args[0].startswith('Found no database at provided path.')
         
     git_repo = pydriller.Git(github_repo_dir)
     commits = [c.hash for c in git_repo.get_list_commits()]
     
-    git2net.mine_git_repo(github_repo_dir, sqlite_db_file, commits=commits[:10])
+    git4net.mine_git_repo(github_repo_dir, sqlite_db_file, commits=commits[:10])
 
     with pytest.raises(Exception) as e:
-        git2net.visualisation._ensure_author_id_exists(sqlite_db_file)
+        git4net.visualisation._ensure_author_id_exists(sqlite_db_file)
     assert e.value.args[0].startswith('The author_id is not yet computed.')
     
-    assert not git2net.check_mining_complete(github_repo_dir, sqlite_db_file)
+    assert not git4net.check_mining_complete(github_repo_dir, sqlite_db_file)
     
-    u_commits_info = git2net.mining_state_summary(github_repo_dir, sqlite_db_file, all_branches=True)
-    complete, missing = git2net.check_mining_complete(github_repo_dir, sqlite_db_file, return_number_missing=True)
+    u_commits_info = git4net.mining_state_summary(github_repo_dir, sqlite_db_file, all_branches=True)
+    complete, missing = git4net.check_mining_complete(github_repo_dir, sqlite_db_file, return_number_missing=True)
     
     assert len(u_commits_info) == (len(commits) - 10)       
     assert missing == (len(commits) - 10) 
     
-    git2net.disambiguate_aliases_db(sqlite_db_file)
+    git4net.disambiguate_aliases_db(sqlite_db_file)
         
-    git2net.mine_git_repo(github_repo_dir, sqlite_db_file)
-    assert git2net.check_mining_complete(github_repo_dir, sqlite_db_file)
+    git4net.mine_git_repo(github_repo_dir, sqlite_db_file)
+    assert git4net.check_mining_complete(github_repo_dir, sqlite_db_file)
     
     with pytest.raises(Exception) as e:
-        git2net.visualisation._ensure_author_id_exists(sqlite_db_file)
+        git4net.visualisation._ensure_author_id_exists(sqlite_db_file)
     assert e.value.args[0].startswith('The author_id is missing entries.')
     
     
 def test_mine_git_repo_exceptions_1(git_repo_dir, sqlite_db_file):
     with pytest.raises(Exception) as e:
-        git2net.check_mining_complete(git_repo_dir, sqlite_db_file)
+        git4net.check_mining_complete(git_repo_dir, sqlite_db_file)
     assert e.value.args[0] == 'Found no database at provided path.'
 
     with open(sqlite_db_file, 'w') as f:
         f.write('Hello World!')
 
     with pytest.raises(Exception) as e:
-        git2net.check_mining_complete(git_repo_dir, sqlite_db_file)
+        git4net.check_mining_complete(git_repo_dir, sqlite_db_file)
     assert e.value.args[0] == 'The provided file is not a compatible database.'
 
     assert os.path.exists(sqlite_db_file)
     os.remove(sqlite_db_file)
     with sqlite3.connect(sqlite_db_file) as con:
-        pd.DataFrame().to_sql('git2net', con)
+        pd.DataFrame().to_sql('git4net', con)
 
-    assert not git2net.check_mining_complete(git_repo_dir, sqlite_db_file)
+    assert not git4net.check_mining_complete(git_repo_dir, sqlite_db_file)
 
     with pytest.raises(Exception) as e:
-        git2net.mine_git_repo(git_repo_dir, sqlite_db_file)
+        git4net.mine_git_repo(git_repo_dir, sqlite_db_file)
     assert e.value.args[0].startswith('Found a database on provided path that was likely not created')
         
         
 def test_mine_git_repo_exceptions_2(git_repo_dir, sqlite_db_file):
     git_repo = pydriller.Git(git_repo_dir)
     commits = [c.hash for c in git_repo.get_list_commits()]
 
-    git2net.mine_git_repo(git_repo_dir, sqlite_db_file, commits=commits[:1])
+    git4net.mine_git_repo(git_repo_dir, sqlite_db_file, commits=commits[:1])
 
     with pytest.raises(Exception) as e:
-        git2net.mine_git_repo(git_repo_dir, sqlite_db_file, use_blocks=True)
+        git4net.mine_git_repo(git_repo_dir, sqlite_db_file, use_blocks=True)
     assert e.value.args[0].startswith('Found a database on provided path that was created')
         
     
 def test_mine_git_repo_exceptions_3(git_repo_dir, github_url_short, github_repo_dir, sqlite_db_file):
-    git2net.mine_github(github_url_short, github_repo_dir, sqlite_db_file)
+    git4net.mine_github(github_url_short, github_repo_dir, sqlite_db_file)
 
     with pytest.raises(Exception) as e:
-        git2net.mining_state_summary(git_repo_dir, sqlite_db_file)
+        git4net.mining_state_summary(git_repo_dir, sqlite_db_file)
     assert e.value.args[0].startswith('The database does not match the provided repository.')
         
     with pytest.raises(Exception) as e:
-        git2net.mine_git_repo(git_repo_dir, sqlite_db_file)
+        git4net.mine_git_repo(git_repo_dir, sqlite_db_file)
     assert e.value.args[0].startswith('Found a database that was created with identical settings. However')
     
 def test_get_edited_file_paths_since_split(git_repo_dir):
     
     git_repo = pydriller.Git(git_repo_dir)
     commit = git_repo.get_commit('a1b3307e5066455508447e5d2811cc1eacb10a0c')
     
-    edited_file_paths = git2net.extraction._get_edited_file_paths_since_split(git_repo, commit)
+    edited_file_paths = git4net.extraction._get_edited_file_paths_since_split(git_repo, commit)
     
     assert edited_file_paths == {'test_file_2.txt', 'test_file_3.txt', 'test_folder/text_file_changed_name.txt'}
     
 
 def test_identify_file_renaming(git_repo_dir):
     
-    dag, aliases = git2net.identify_file_renaming(git_repo_dir)
+    dag, aliases = git4net.identify_file_renaming(git_repo_dir)
     
     expected_aliases = {'test_file_2.txt': 'text_file.txt',
                         'test_folder/text_file_changed_name.txt': 'text_file.txt',
                         'text_file_changed_name.txt': 'text_file.txt'}
     
     expected_edges = [('text_file_changed_name.txt', 'text_file.txt'), 
                       ('test_folder/text_file_changed_name.txt', 'text_file_changed_name.txt'),
@@ -717,97 +717,97 @@
     assert len(dag.nodes) == 8
     assert len(dag.roots) == 5
     assert len(dag.leafs) == 5
     assert list(dag.edges.keys()) == expected_edges
 
     
 def test_visualisation_github(github_url_short, github_repo_dir, sqlite_db_file):
-    git2net.mine_github(github_url_short, github_repo_dir, sqlite_db_file)
-    assert git2net.check_mining_complete(github_repo_dir, sqlite_db_file)
+    git4net.mine_github(github_url_short, github_repo_dir, sqlite_db_file)
+    assert git4net.check_mining_complete(github_repo_dir, sqlite_db_file)
     
-    git2net.disambiguate_aliases_db(sqlite_db_file)
-    assert git2net.visualisation._ensure_author_id_exists(sqlite_db_file)
+    git4net.disambiguate_aliases_db(sqlite_db_file)
+    assert git4net.visualisation._ensure_author_id_exists(sqlite_db_file)
     
     # Assures no visualisation function throws error on real data
-    paths, dag, node_info, edge_info = git2net.get_line_editing_paths(sqlite_db_file, github_repo_dir)
+    paths, dag, node_info, edge_info = git4net.get_line_editing_paths(sqlite_db_file, github_repo_dir)
     assert type(paths) == pp.Paths
     assert type(dag) == pp.DAG
     assert type(node_info) == dict
     assert type(edge_info) == dict
     
-    dag, node_info, edge_info = git2net.get_commit_editing_dag(sqlite_db_file)
+    dag, node_info, edge_info = git4net.get_commit_editing_dag(sqlite_db_file)
     assert type(dag) == pp.DAG
     assert type(node_info) == dict
     assert type(edge_info) == dict
     
-    t, node_info, edge_info = git2net.get_coediting_network(sqlite_db_file)
+    t, node_info, edge_info = git4net.get_coediting_network(sqlite_db_file)
     assert type(t) == pp.TemporalNetwork
     assert type(node_info) == dict
     assert type(edge_info) == dict
     
-    n, node_info, edge_info = git2net.get_coauthorship_network(sqlite_db_file)
+    n, node_info, edge_info = git4net.get_coauthorship_network(sqlite_db_file)
     assert type(n) == pp.Network
     assert type(node_info) == dict
     assert type(edge_info) == dict
     
-    t, node_info, edge_info = git2net.get_bipartite_network(sqlite_db_file)
+    t, node_info, edge_info = git4net.get_bipartite_network(sqlite_db_file)
     assert type(t) == pp.TemporalNetwork
     assert type(node_info) == dict
     assert type(edge_info) == dict
     
     
 def test_parse_blame_C():
     with pytest.raises(Exception) as e:
-        git2net.extraction._parse_blame_C('invalid') == []
+        git4net.extraction._parse_blame_C('invalid') == []
     assert e.value.args[0].startswith("Invalid 'blame_C' supplied.")
     
-    assert git2net.extraction._parse_blame_C('') == []
+    assert git4net.extraction._parse_blame_C('') == []
     
-    assert git2net.extraction._parse_blame_C('-CCC42') == ['-C', '-C', '-C42']
+    assert git4net.extraction._parse_blame_C('-CCC42') == ['-C', '-C', '-C42']
     
     
 def test_mining_options(github_url_short, github_repo_dir, sqlite_db_file):
-    git2net.mine_github(github_url_short, github_repo_dir, sqlite_db_file, blame_w=True)
-    assert git2net.check_mining_complete(github_repo_dir, sqlite_db_file)
+    git4net.mine_github(github_url_short, github_repo_dir, sqlite_db_file, blame_w=True)
+    assert git4net.check_mining_complete(github_repo_dir, sqlite_db_file)
     # add information from other branches
-    git2net.mine_github(github_url_short, github_repo_dir, sqlite_db_file, blame_w=True, all_branches=True)
-    assert git2net.check_mining_complete(github_repo_dir, sqlite_db_file)
+    git4net.mine_github(github_url_short, github_repo_dir, sqlite_db_file, blame_w=True, all_branches=True)
+    assert git4net.check_mining_complete(github_repo_dir, sqlite_db_file)
     
     
 def test_check_mailmap(git_repo_dir):
     git_repo = pydriller.Git(git_repo_dir)
 
     example = ('Joe', 'joe@example.com')
     result = ('Joe R. Developer', 'joe@example.com')
-    assert git2net.extraction._check_mailmap(*example, git_repo) == result
+    assert git4net.extraction._check_mailmap(*example, git_repo) == result
 
     example = ('Test', 'jane@laptop.(none)')
     result = ('Jane Doe', 'jane@example.com')
-    assert git2net.extraction._check_mailmap(*example, git_repo) == result
+    assert git4net.extraction._check_mailmap(*example, git_repo) == result
 
     example = ('Jane Doe', 'jane@desktop.(none)')
     result = ('Jane Doe', 'jane@example.com')
-    assert git2net.extraction._check_mailmap(*example, git_repo) == result
+    assert git4net.extraction._check_mailmap(*example, git_repo) == result
 
     example = ('Joe', 'bugs@example.com')
     result = ('Joe R. Developer', 'joe@example.com')
-    assert git2net.extraction._check_mailmap(*example, git_repo) == result
+    assert git4net.extraction._check_mailmap(*example, git_repo) == result
 
     example = ('Jane', 'bugs@example.com')
     result = ('Jane Doe', 'jane@example.com')
-    assert git2net.extraction._check_mailmap(*example, git_repo) == result
+    assert git4net.extraction._check_mailmap(*example, git_repo) == result
 
     example = ('SomeoneElse', 'bugs@example.com')
     result = example
-    assert git2net.extraction._check_mailmap(*example, git_repo) == result
+    assert git4net.extraction._check_mailmap(*example, git_repo) == result
 
     example = ('invalid', 'invalid@invalid.com')
     result = example
-    assert git2net.extraction._check_mailmap(*example, git_repo) == result
+    assert git4net.extraction._check_mailmap(*example, git_repo) == result
 
     example = ('--', '--')
     result = example
-    assert git2net.extraction._check_mailmap(*example, git_repo) == result
+    assert git4net.extraction._check_mailmap(*example, git_repo) == result
 
     example = ('-', '-')
     result = example
-    assert git2net.extraction._check_mailmap(*example, git_repo) == result
+    assert git4net.extraction._check_mailmap(*example, git_repo) == result
```

