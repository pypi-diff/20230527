# Comparing `tmp/cli-test-helpers-3.2.0.tar.gz` & `tmp/cli-test-helpers-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-test-helpers-3.2.0.tar", last modified: Thu Feb 23 15:17:55 2023, max compression
+gzip compressed data, was "cli-test-helpers-3.3.0.tar", last modified: Fri May 26 23:51:45 2023, max compression
```

## Comparing `cli-test-helpers-3.2.0.tar` & `cli-test-helpers-3.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:17:55.731777 cli-test-helpers-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-23 15:17:42.000000 cli-test-helpers-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-23 15:17:42.000000 cli-test-helpers-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-02-23 15:17:55.731777 cli-test-helpers-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-02-23 15:17:42.000000 cli-test-helpers-3.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:17:55.727777 cli-test-helpers-3.2.0/cli_test_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-02-23 15:17:42.000000 cli-test-helpers-3.2.0/cli_test_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-02-23 15:17:42.000000 cli-test-helpers-3.2.0/cli_test_helpers/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-23 15:17:42.000000 cli-test-helpers-3.2.0/cli_test_helpers/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:17:55.731777 cli-test-helpers-3.2.0/cli_test_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-02-23 15:17:55.000000 cli-test-helpers-3.2.0/cli_test_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-23 15:17:55.000000 cli-test-helpers-3.2.0/cli_test_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 15:17:55.000000 cli-test-helpers-3.2.0/cli_test_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-23 15:17:55.000000 cli-test-helpers-3.2.0/cli_test_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-23 15:17:55.000000 cli-test-helpers-3.2.0/cli_test_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-02-23 15:17:42.000000 cli-test-helpers-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 15:17:55.731777 cli-test-helpers-3.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2221 2023-02-23 15:17:42.000000 cli-test-helpers-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:17:55.731777 cli-test-helpers-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-02-23 15:17:42.000000 cli-test-helpers-3.2.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-02-23 15:17:42.000000 cli-test-helpers-3.2.0/tests/test_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:51:45.649797 cli-test-helpers-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 23:51:32.000000 cli-test-helpers-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 23:51:32.000000 cli-test-helpers-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-26 23:51:45.649797 cli-test-helpers-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-26 23:51:32.000000 cli-test-helpers-3.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:51:45.649797 cli-test-helpers-3.3.0/cli_test_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-26 23:51:32.000000 cli-test-helpers-3.3.0/cli_test_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-26 23:51:32.000000 cli-test-helpers-3.3.0/cli_test_helpers/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-26 23:51:32.000000 cli-test-helpers-3.3.0/cli_test_helpers/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:51:45.649797 cli-test-helpers-3.3.0/cli_test_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-26 23:51:45.000000 cli-test-helpers-3.3.0/cli_test_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-26 23:51:45.000000 cli-test-helpers-3.3.0/cli_test_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 23:51:45.000000 cli-test-helpers-3.3.0/cli_test_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 23:51:45.000000 cli-test-helpers-3.3.0/cli_test_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 23:51:45.000000 cli-test-helpers-3.3.0/cli_test_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-26 23:51:32.000000 cli-test-helpers-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 23:51:45.649797 cli-test-helpers-3.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2253 2023-05-26 23:51:32.000000 cli-test-helpers-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:51:45.649797 cli-test-helpers-3.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-26 23:51:32.000000 cli-test-helpers-3.3.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-26 23:51:32.000000 cli-test-helpers-3.3.0/tests/test_decorators.py
```

### Comparing `cli-test-helpers-3.2.0/LICENSE` & `cli-test-helpers-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cli-test-helpers-3.2.0/PKG-INFO` & `cli-test-helpers-3.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: cli-test-helpers
-Version: 3.2.0
+Version: 3.3.0
 Summary: Useful helpers for writing tests for your Python CLI program.
 Home-page: https://github.com/painless-software/python-cli-test-helpers
 Author: Peter Bittner
 Author-email: peter@painless.software
+License: GPL-3.0-or-later
 Project-URL: Documentation, https://python-cli-test-helpers.readthedocs.io/
 Project-URL: Examples, https://github.com/painless-software/python-cli-test-helpers/tree/main/examples
 Keywords: python,cli,testing,helpers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
@@ -87,22 +88,27 @@
 -----------
 
 This project uses Tox to run its test suite. Install and use it locally like
 this:
 
 .. code-block:: shell
 
-    python3 -m pip install tox
+    python3 -m pip install tox 'virtualenv<20.22'
+
+.. note::
+
+   Virtualenv 20.22 dropped support for Python 2.7 and <3.6, which most
+   notably makes Tox fail to detect the PyPy2 executable.
 
 .. code-block:: shell
 
-    tox -lv               # list available environments
-    tox -e flake8,py310   # run a few environments
-    tox -e py             # run tests with default Python
-    tox                   # run entire suite
+    tox list            # list available environments
+    tox -e ruff,py311   # run a few environments
+    tox -e py           # run tests with local default Python
+    tox                 # run entire suite
 
 The included example projects can be tested independently with their dedicated
 environments, e.g.
 
 .. code-block:: shell
 
     tox -e example-docopt
```

### Comparing `cli-test-helpers-3.2.0/README.rst` & `cli-test-helpers-3.3.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -55,22 +55,27 @@
 -----------
 
 This project uses Tox to run its test suite. Install and use it locally like
 this:
 
 .. code-block:: shell
 
-    python3 -m pip install tox
+    python3 -m pip install tox 'virtualenv<20.22'
+
+.. note::
+
+   Virtualenv 20.22 dropped support for Python 2.7 and <3.6, which most
+   notably makes Tox fail to detect the PyPy2 executable.
 
 .. code-block:: shell
 
-    tox -lv               # list available environments
-    tox -e flake8,py310   # run a few environments
-    tox -e py             # run tests with default Python
-    tox                   # run entire suite
+    tox list            # list available environments
+    tox -e ruff,py311   # run a few environments
+    tox -e py           # run tests with local default Python
+    tox                 # run entire suite
 
 The included example projects can be tested independently with their dedicated
 environments, e.g.
 
 .. code-block:: shell
 
     tox -e example-docopt
```

### Comparing `cli-test-helpers-3.2.0/cli_test_helpers/commands.py` & `cli-test-helpers-3.3.0/cli_test_helpers/commands.py`

 * *Files identical despite different names*

### Comparing `cli-test-helpers-3.2.0/cli_test_helpers/decorators.py` & `cli-test-helpers-3.3.0/cli_test_helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `cli-test-helpers-3.2.0/cli_test_helpers.egg-info/PKG-INFO` & `cli-test-helpers-3.3.0/cli_test_helpers.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: cli-test-helpers
-Version: 3.2.0
+Version: 3.3.0
 Summary: Useful helpers for writing tests for your Python CLI program.
 Home-page: https://github.com/painless-software/python-cli-test-helpers
 Author: Peter Bittner
 Author-email: peter@painless.software
+License: GPL-3.0-or-later
 Project-URL: Documentation, https://python-cli-test-helpers.readthedocs.io/
 Project-URL: Examples, https://github.com/painless-software/python-cli-test-helpers/tree/main/examples
 Keywords: python,cli,testing,helpers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
@@ -87,22 +88,27 @@
 -----------
 
 This project uses Tox to run its test suite. Install and use it locally like
 this:
 
 .. code-block:: shell
 
-    python3 -m pip install tox
+    python3 -m pip install tox 'virtualenv<20.22'
+
+.. note::
+
+   Virtualenv 20.22 dropped support for Python 2.7 and <3.6, which most
+   notably makes Tox fail to detect the PyPy2 executable.
 
 .. code-block:: shell
 
-    tox -lv               # list available environments
-    tox -e flake8,py310   # run a few environments
-    tox -e py             # run tests with default Python
-    tox                   # run entire suite
+    tox list            # list available environments
+    tox -e ruff,py311   # run a few environments
+    tox -e py           # run tests with local default Python
+    tox                 # run entire suite
 
 The included example projects can be tested independently with their dedicated
 environments, e.g.
 
 .. code-block:: shell
 
     tox -e example-docopt
```

### Comparing `cli-test-helpers-3.2.0/setup.py` & `cli-test-helpers-3.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,28 +13,29 @@
     # pylint: disable=unspecified-encoding
     with open(join(abspath(dirname(__file__)), filename)) as file:
         return file.read()
 
 
 setup(
     name='cli-test-helpers',
-    version='3.2.0',
+    version='3.3.0',
     author='Peter Bittner',
     author_email='peter@painless.software',
     description='Useful helpers for writing tests for your Python CLI program.',
     long_description=read_file('README.rst'),
     long_description_content_type='text/x-rst',
     url='https://github.com/painless-software/python-cli-test-helpers',
     project_urls={
         'Documentation': 'https://python-cli-test-helpers.readthedocs.io/',
         'Examples': 'https://github.com/painless-software/'
                     'python-cli-test-helpers/tree/main/examples',
     },
     packages=find_packages(exclude=['test*', 'examples']),
     include_package_data=True,
+    license='GPL-3.0-or-later',
     keywords=['python', 'cli', 'testing', 'helpers'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
```

### Comparing `cli-test-helpers-3.2.0/tests/test_commands.py` & `cli-test-helpers-3.3.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `cli-test-helpers-3.2.0/tests/test_decorators.py` & `cli-test-helpers-3.3.0/tests/test_decorators.py`

 * *Files identical despite different names*

