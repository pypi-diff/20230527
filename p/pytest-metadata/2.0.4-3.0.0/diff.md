# Comparing `tmp/pytest_metadata-2.0.4.tar.gz` & `tmp/pytest_metadata-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_metadata-2.0.4.tar", max compression
+gzip compressed data, last modified: Sat May 27 18:29:13 2023, max compression
```

## Comparing `pytest_metadata-2.0.4.tar` & `pytest_metadata-3.0.0.tar`

### file list

```diff
@@ -1,18 +1,24 @@
--rw-r--r--   0        0        0      193 2022-10-30 21:14:24.004578 pytest_metadata-2.0.4/LICENSE
--rw-r--r--   0        0        0     6760 2022-10-30 21:14:24.004578 pytest_metadata-2.0.4/README.rst
--rw-r--r--   0        0        0     1310 2022-10-30 21:14:24.004578 pytest_metadata-2.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-30 21:14:24.004578 pytest_metadata-2.0.4/src/pytest_metadata/__init__.py
--rw-r--r--   0        0        0        0 2022-10-30 21:14:24.004578 pytest_metadata-2.0.4/src/pytest_metadata/ci/__init__.py
--rw-r--r--   0        0        0     1108 2022-10-30 21:14:24.004578 pytest_metadata-2.0.4/src/pytest_metadata/ci/appveyor.py
--rw-r--r--   0        0        0      573 2022-10-30 21:14:24.004578 pytest_metadata-2.0.4/src/pytest_metadata/ci/bitbucket.py
--rw-r--r--   0        0        0      757 2022-10-30 21:14:24.004578 pytest_metadata-2.0.4/src/pytest_metadata/ci/circleci.py
--rw-r--r--   0        0        0     1060 2022-10-30 21:14:24.004578 pytest_metadata-2.0.4/src/pytest_metadata/ci/gitlab_ci.py
--rw-r--r--   0        0        0      496 2022-10-30 21:14:24.004578 pytest_metadata-2.0.4/src/pytest_metadata/ci/jenkins.py
--rw-r--r--   0        0        0      246 2022-10-30 21:14:24.004578 pytest_metadata-2.0.4/src/pytest_metadata/ci/taskcluster.py
--rw-r--r--   0        0        0      654 2022-10-30 21:14:24.004578 pytest_metadata-2.0.4/src/pytest_metadata/ci/travis_ci.py
--rw-r--r--   0        0        0      275 2022-10-30 21:14:24.004578 pytest_metadata-2.0.4/src/pytest_metadata/hooks.py
--rw-r--r--   0        0        0     3620 2022-10-30 21:14:24.004578 pytest_metadata-2.0.4/src/pytest_metadata/plugin.py
--rw-r--r--   0        0        0        0 2022-10-30 21:14:24.004578 pytest_metadata-2.0.4/tests/__init__.py
--rw-r--r--   0        0        0     4364 2022-10-30 21:14:24.004578 pytest_metadata-2.0.4/tests/test_metadata.py
--rw-r--r--   0        0        0     7877 1970-01-01 00:00:00.000000 pytest_metadata-2.0.4/setup.py
--rw-r--r--   0        0        0     7950 1970-01-01 00:00:00.000000 pytest_metadata-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0      448 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3228 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/CHANGES.rst
+-rw-r--r--   0        0        0     1757 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/development.rst
+-rw-r--r--   0        0        0      670 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/tox.ini
+-rw-r--r--   0        0        0        0 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/src/pytest_metadata/__init__.py
+-rw-r--r--   0        0        0      160 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/src/pytest_metadata/__version.py
+-rw-r--r--   0        0        0      283 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/src/pytest_metadata/hooks.py
+-rw-r--r--   0        0        0     3848 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/src/pytest_metadata/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/src/pytest_metadata/ci/__init__.py
+-rw-r--r--   0        0        0     1108 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/src/pytest_metadata/ci/appveyor.py
+-rw-r--r--   0        0        0      573 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/src/pytest_metadata/ci/bitbucket.py
+-rw-r--r--   0        0        0      757 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/src/pytest_metadata/ci/circleci.py
+-rw-r--r--   0        0        0     1060 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/src/pytest_metadata/ci/gitlab_ci.py
+-rw-r--r--   0        0        0      496 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/src/pytest_metadata/ci/jenkins.py
+-rw-r--r--   0        0        0      246 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/src/pytest_metadata/ci/taskcluster.py
+-rw-r--r--   0        0        0      654 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/src/pytest_metadata/ci/travis_ci.py
+-rw-r--r--   0        0        0        0 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     4374 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/tests/test_metadata.py
+-rw-r--r--   0        0        0       73 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/.gitignore
+-rw-r--r--   0        0        0      120 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/AUTHORS
+-rw-r--r--   0        0        0      193 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/LICENSE
+-rw-r--r--   0        0        0     6870 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/README.rst
+-rw-r--r--   0        0        0     1924 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8575 2023-05-27 18:29:13.000000 pytest_metadata-3.0.0/PKG-INFO
```

### Comparing `pytest_metadata-2.0.4/README.rst` & `pytest_metadata-3.0.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -147,34 +147,36 @@
 ------------------
 
 To add/modify/delete metadata at the end of metadata collection, you can use the ``pytest_metadata`` hook:
 
 .. code-block:: python
 
   import pytest
-  @pytest.mark.optionalhook
+  @pytest.hookimpl(optionalhook=True)
   def pytest_metadata(metadata):
       metadata.pop("password", None)
 
 To access the metadata from a test or fixture, you can use the ``metadata``
 fixture:
 
 .. code-block:: python
 
   def test_metadata(metadata):
       assert 'metadata' in metadata['Plugins']
 
-To access the metadata from a plugin, you can use the ``_metadata`` attribute of
+To access the metadata from a plugin, you can use the ``stash`` attribute of
 the ``config`` object. This can be used to read/add/modify the metadata:
 
 .. code-block:: python
 
   def pytest_configure(config):
-    if hasattr(config, '_metadata'):
-        config._metadata['foo'] = 'bar'
+    metadata = config.pluginmanager.getplugin("metadata")
+    if metadata:
+        from pytest_metadata.plugin import metadata_key
+        config.stash[metadata_key]['foo'] = 'bar'
 
 Plugin integrations
 -------------------
 
 Here's a handy list of plugins that either read or contribute to the metadata:
 
 * `pytest-base-url <https://pypi.python.org/pypi/pytest-base-url/>`_ - Adds the
```

### Comparing `pytest_metadata-2.0.4/src/pytest_metadata/ci/appveyor.py` & `pytest_metadata-3.0.0/src/pytest_metadata/ci/appveyor.py`

 * *Files identical despite different names*

### Comparing `pytest_metadata-2.0.4/src/pytest_metadata/ci/bitbucket.py` & `pytest_metadata-3.0.0/src/pytest_metadata/ci/bitbucket.py`

 * *Files identical despite different names*

### Comparing `pytest_metadata-2.0.4/src/pytest_metadata/ci/circleci.py` & `pytest_metadata-3.0.0/src/pytest_metadata/ci/circleci.py`

 * *Files identical despite different names*

### Comparing `pytest_metadata-2.0.4/src/pytest_metadata/ci/gitlab_ci.py` & `pytest_metadata-3.0.0/src/pytest_metadata/ci/gitlab_ci.py`

 * *Files identical despite different names*

### Comparing `pytest_metadata-2.0.4/src/pytest_metadata/ci/travis_ci.py` & `pytest_metadata-3.0.0/src/pytest_metadata/ci/travis_ci.py`

 * *Files identical despite different names*

### Comparing `pytest_metadata-2.0.4/src/pytest_metadata/plugin.py` & `pytest_metadata-3.0.0/src/pytest_metadata/plugin.py`

 * *Files 25% similar despite different names*

```diff
@@ -27,100 +27,102 @@
     circleci.ENVIRONMENT_VARIABLES,
     gitlab_ci.ENVIRONMENT_VARIABLES,
     jenkins.ENVIRONMENT_VARIABLES,
     taskcluster.ENVIRONMENT_VARIABLES,
     travis_ci.ENVIRONMENT_VARIABLES,
 ]
 
+metadata_key = pytest.StashKey[dict]()
+
 
 def pytest_addhooks(pluginmanager):
-    from . import hooks
+    from pytest_metadata import hooks
 
     pluginmanager.add_hookspecs(hooks)
 
 
 @pytest.fixture(scope="session")
 def metadata(pytestconfig):
     """Provide test session metadata"""
-    return pytestconfig._metadata
+    return pytestconfig.stash[metadata_key]
 
 
 @pytest.fixture(scope="session")
 def include_metadata_in_junit_xml(metadata, pytestconfig, record_testsuite_property):
     """Provide test session metadata"""
-    metadata_ = pytestconfig._metadata
+    metadata_ = pytestconfig.stash[metadata_key]
     for name, value in metadata_.items():
         record_testsuite_property(name, value)
 
 
 def pytest_addoption(parser):
-    parser.addoption(
+    group = parser.getgroup("pytest-metadata")
+    group.addoption(
         "--metadata",
         action="append",
         default=[],
         dest="metadata",
         metavar=("key", "value"),
         nargs=2,
         help="additional metadata.",
     )
-    parser.addoption(
+    group.addoption(
         "--metadata-from-json",
         action="store",
         default="{}",
         dest="metadata_from_json",
         help="additional metadata from a json string.",
     )
-    parser.addoption(
+    group.addoption(
         "--metadata-from-json-file",
         type=str,
         dest="metadata_from_json_file",
         help="additional metadata from a json file.",
     )
 
 
 @pytest.hookimpl(tryfirst=True)
 def pytest_configure(config):
-    config._metadata = {
+    config.stash[metadata_key] = {
         "Python": platform.python_version(),
         "Platform": platform.platform(),
         "Packages": {
             "pytest": pytest.__version__,
             "pluggy": pluggy.__version__,
         },
     }
-    config._metadata.update({k: v for k, v in config.getoption("metadata")})
-    config._metadata.update(json.loads(config.getoption("metadata_from_json")))
+    config.stash[metadata_key].update({k: v for k, v in config.getoption("metadata")})
+    config.stash[metadata_key].update(
+        json.loads(config.getoption("metadata_from_json"))
+    )
     if config.getoption("metadata_from_json_file"):
         with open(config.getoption("metadata_from_json_file"), "r") as json_file:
-            config._metadata.update(json.load(json_file))
+            config.stash[metadata_key].update(json.load(json_file))
     plugins = dict()
     for plugin, dist in config.pluginmanager.list_plugin_distinfo():
         name, version = dist.project_name, dist.version
         if name.startswith("pytest-"):
             name = name[7:]
         plugins[name] = version
-    config._metadata["Plugins"] = plugins
+    config.stash[metadata_key]["Plugins"] = plugins
 
     for provider in CONTINUOUS_INTEGRATION:
-        [
-            config._metadata.update({var: os.environ.get(var)})
-            for var in provider
-            if os.environ.get(var)
-        ]
+        for var in provider:
+            if os.environ.get(var):
+                config.stash[metadata_key].update({var: os.environ.get(var)})
 
     if hasattr(config, "workeroutput"):
-        config.workeroutput["metadata"] = config._metadata
-
-    config.hook.pytest_metadata(metadata=config._metadata)
+        config.workeroutput["metadata"] = config.stash[metadata_key]
+    config.hook.pytest_metadata(metadata=config.stash[metadata_key], config=config)
 
 
 def pytest_report_header(config):
     if config.getoption("verbose") > 0:
-        return "metadata: {0}".format(config._metadata)
+        return "metadata: {0}".format(config.stash[metadata_key])
 
 
 @pytest.hookimpl(optionalhook=True)
 def pytest_testnodedown(node):
     # note that any metadata from remote workers will be replaced with the
     # environment from the final worker to quit
     if hasattr(node, "workeroutput"):
-        node.config._metadata.update(node.workeroutput["metadata"])
+        node.config.stash[metadata_key].update(node.workeroutput["metadata"])
```

### Comparing `pytest_metadata-2.0.4/tests/test_metadata.py` & `pytest_metadata-3.0.0/tests/test_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     assert result.ret == 0
 
 
 def test_metadata_hook(testdir):
     testdir.makeconftest(
         """
         import pytest
-        @pytest.mark.optionalhook
+        @pytest.hookimpl(optionalhook=True)
         def pytest_metadata(metadata):
             metadata['Dave'] = 'Hunt'
     """
     )
     testdir.makepyfile(
         """
         def test_pass(metadata):
```

### Comparing `pytest_metadata-2.0.4/setup.py` & `pytest_metadata-3.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,235 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pytest-metadata
+Version: 3.0.0
+Summary: pytest plugin for test session metadata
+Project-URL: Homepage, https://github.com/pytest-dev/pytest-metadata
+Project-URL: Tracker, https://github.com/pytest-dev/pytest-metadata/issues
+Project-URL: Source, https://github.com/pytest-dev/pytest-metadata
+Author-email: Dave Hunt <dhunt@mozilla.com>, Jim Brannlund <jimbrannlund@fastmail.com>
+License-Expression: MPL-2.0
+License-File: AUTHORS
+License-File: LICENSE
+Keywords: metadata,pytest
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Requires-Dist: pytest>=7.0.0
+Provides-Extra: test
+Requires-Dist: black>=22.1.0; extra == 'test'
+Requires-Dist: flake8>=4.0.1; extra == 'test'
+Requires-Dist: pre-commit>=2.17.0; extra == 'test'
+Requires-Dist: tox>=3.24.5; extra == 'test'
+Description-Content-Type: text/x-rst
 
-package_dir = \
-{'': 'src'}
+pytest-metadata
+===============
 
-packages = \
-['pytest_metadata', 'pytest_metadata.ci']
+pytest-metadata is a plugin for `pytest <http://pytest.org>`_ that provides
+access to test session metadata.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pytest>=3.0.0,<8.0.0']
-
-entry_points = \
-{'pytest11': ['metadata = pytest_metadata.plugin']}
-
-setup_kwargs = {
-    'name': 'pytest-metadata',
-    'version': '2.0.4',
-    'description': 'pytest plugin for test session metadata',
-    'long_description': 'pytest-metadata\n===============\n\npytest-metadata is a plugin for `pytest <http://pytest.org>`_ that provides\naccess to test session metadata.\n\n.. image:: https://img.shields.io/badge/license-MPL%202.0-blue.svg\n   :target: https://github.com/pytest-dev/pytest-metadata/blob/master/LICENSE\n   :alt: License\n.. image:: https://img.shields.io/pypi/v/pytest-metadata.svg\n   :target: https://pypi.python.org/pypi/pytest-metadata/\n   :alt: PyPI\n.. image:: https://img.shields.io/travis/pytest-dev/pytest-metadata.svg\n   :target: https://travis-ci.org/pytest-dev/pytest-metadata/\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/ambv/black\n   :alt: Travis\n.. image:: https://img.shields.io/github/issues-raw/pytest-dev/pytest-metadata.svg\n   :target: https://github.com/pytest-dev/pytest-metadata/issues\n   :alt: Issues\n.. image:: https://img.shields.io/requires/github/pytest-dev/pytest-metadata.svg\n   :target: https://requires.io/github/pytest-dev/pytest-metadata/requirements/?branch=master\n   :alt: Requirements\n\nRequirements\n------------\n\nYou will need the following in order to use pytest-metadata:\n\n- Python 3.7+ or PyPy3\n\nInstallation\n------------\n\nTo install pytest-metadata:\n\n.. code-block:: bash\n\n  $ pip install pytest-metadata\n\nContributing\n------------\n\nWe welcome contributions.\n\nTo learn more, see `Development <https://github.com/pytest-dev/pytest-metadata/blob/master/development.rst>`_\n\nAvailable metadata\n------------------\n\nThe following metadata is gathered by this plugin:\n\n========  =============== ===================================\nKey       Description     Example\n========  =============== ===================================\nPython    Python version  3.6.4\nPlatform  Platform        Darwin-17.4.0-x86_64-i386-64bit\nPackages  pytest packages {\'py\': \'1.5.2\', \'pytest\': \'3.4.1\'}\nPlugins   pytest plugins  {\'metadata\': \'1.6.0\'}\n========  =============== ===================================\n\nAdditional metadata\n-------------------\n\nYou can provide your own metadata (key, value pair) by specifying ``--metadata`` on the commandline::\n\n   pytest --metadata foo bar\n\nNote: You can provide multiple sets of ``--metadata``::\n\n   pytest --metadata foo bar --metadata baz zoo\n\nThere\'s also the possibility of passing in metadata as a JSON string::\n\n    pytest --metadata-from-json \'{"cat_says": "bring the cat nip", "human_says": "yes kitty"}\'\n\nAlternatively a JSON can be read from a given file::\n\n    pytest --metadata-from-json-file path/to/valid/file.json\n\nContinuous integration\n----------------------\n\nWhen run in a continuous integration environment, additional metadata is added\nfrom environment variables. Below is a list of the supported continuous\nintegration providers, along with links to the environment variables that are\nadded to metadata if they\'re present.\n\n* `AppVeyor <https://www.appveyor.com/docs/environment-variables/>`_\n* `Bitbucket <https://confluence.atlassian.com/bitbucket/environment-variables-794502608.html>`_\n* `CircleCI <https://circleci.com/docs/1.0/environment-variables/>`_\n* `GitLab CI <http://docs.gitlab.com/ce/ci/variables/README.html>`_\n* `Jenkins <https://wiki.jenkins-ci.org/display/JENKINS/Building+a+software+project#Buildingasoftwareproject-JenkinsSetEnvironmentVariables>`_\n* `TaskCluster <https://docs.taskcluster.net/reference/workers/docker-worker/environment>`_\n* `Travis CI <https://docs.travis-ci.com/user/environment-variables/>`_\n\nNote that if you\'re using `Tox <http://tox.readthedocs.io/>`_ to run your tests\nthen you will need to `pass down any additional environment variables <http://tox.readthedocs.io/en/latest/example/basic.html#passing-down-environment-variables>`_\nfor these to be picked up.\n\nViewing metadata\n----------------\n\nIf you pass ``--verbose`` on the command line when running your tests, then the\nmetadata will be displayed in the terminal report header::\n\n  pytest --verbose\n  ============================ test session starts ============================\n  platform darwin -- Python 3.6.4, pytest-3.4.1, py-1.5.2, pluggy-0.6.0 -- /usr/bin/python\n  cachedir: .pytest_cache\n  metadata: {\'Python\': \'3.6.4\', \'Platform\': \'Darwin-17.4.0-x86_64-i386-64bit\', \'Packages\': {\'pytest\': \'3.4.1\', \'py\': \'1.5.2\', \'pluggy\': \'0.6.0\'}, \'Plugins\': {\'metadata\': \'1.6.0\'}}\n  plugins: metadata-1.6.0\n\nIncluding metadata in Junit XML\n-------------------------------\n\nPytest-metadata provides the session scoped fixture :code:`include_metadata_in_junit_xml` that you may use to include any metadata in Junit XML as ``property`` tags.\nFor example the following test module\n\n.. code-block:: python\n\n  import pytest\n\n  pytestmark = pytest.mark.usefixtures(\'include_metadata_in_junit_xml\')\n\n  def test():\n      pass\n\nwhen called with\n\n.. code-block:: bash\n\n  pytest --metadata Daffy Duck --junit-xml=results.xml\n\nwould produce the following XML\n\n.. code-block:: xml\n\n  <?xml version="1.0" encoding="utf-8"?>\n  <testsuites>\n    <testsuite name="pytest" errors="0" failures="0" skipped="0" tests="1" time="0.009" timestamp="2020-11-27T06:38:44.407674" hostname="sam">\n      <properties>\n        <property name="Daffy" value="Duck"/>\n  ...\n\nAccessing metadata\n------------------\n\nTo add/modify/delete metadata at the end of metadata collection, you can use the ``pytest_metadata`` hook:\n\n.. code-block:: python\n\n  import pytest\n  @pytest.mark.optionalhook\n  def pytest_metadata(metadata):\n      metadata.pop("password", None)\n\nTo access the metadata from a test or fixture, you can use the ``metadata``\nfixture:\n\n.. code-block:: python\n\n  def test_metadata(metadata):\n      assert \'metadata\' in metadata[\'Plugins\']\n\nTo access the metadata from a plugin, you can use the ``_metadata`` attribute of\nthe ``config`` object. This can be used to read/add/modify the metadata:\n\n.. code-block:: python\n\n  def pytest_configure(config):\n    if hasattr(config, \'_metadata\'):\n        config._metadata[\'foo\'] = \'bar\'\n\nPlugin integrations\n-------------------\n\nHere\'s a handy list of plugins that either read or contribute to the metadata:\n\n* `pytest-base-url <https://pypi.python.org/pypi/pytest-base-url/>`_ - Adds the\n  base URL to the metadata.\n* `pytest-html <https://pypi.python.org/pypi/pytest-html/>`_ - Displays the\n  metadata at the start of each report.\n* `pytest-reporter-html1 <https://pypi.org/project/pytest-reporter-html1/>`_ -\n  Presents metadata as part of the report.\n* `pytest-selenium <https://pypi.python.org/pypi/pytest-selenium/>`_ - Adds the\n  driver, capabilities, and remote server to the metadata.\n\nResources\n---------\n\n- `Release Notes <http://github.com/davehunt/pytest-metadata/blob/master/CHANGES.rst>`_\n- `Issue Tracker <http://github.com/davehunt/pytest-metadata/issues>`_\n- `Code <http://github.com/davehunt/pytest-metadata/>`_\n',
-    'author': 'Dave Hunt',
-    'author_email': 'dhunt@mozilla.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/pytest-dev/pytest-metadata',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+.. image:: https://img.shields.io/badge/license-MPL%202.0-blue.svg
+   :target: https://github.com/pytest-dev/pytest-metadata/blob/master/LICENSE
+   :alt: License
+.. image:: https://img.shields.io/pypi/v/pytest-metadata.svg
+   :target: https://pypi.python.org/pypi/pytest-metadata/
+   :alt: PyPI
+.. image:: https://img.shields.io/travis/pytest-dev/pytest-metadata.svg
+   :target: https://travis-ci.org/pytest-dev/pytest-metadata/
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/ambv/black
+   :alt: Travis
+.. image:: https://img.shields.io/github/issues-raw/pytest-dev/pytest-metadata.svg
+   :target: https://github.com/pytest-dev/pytest-metadata/issues
+   :alt: Issues
+.. image:: https://img.shields.io/requires/github/pytest-dev/pytest-metadata.svg
+   :target: https://requires.io/github/pytest-dev/pytest-metadata/requirements/?branch=master
+   :alt: Requirements
 
+Requirements
+------------
 
-setup(**setup_kwargs)
+You will need the following in order to use pytest-metadata:
+
+- Python 3.7+ or PyPy3
+
+Installation
+------------
+
+To install pytest-metadata:
+
+.. code-block:: bash
+
+  $ pip install pytest-metadata
+
+Contributing
+------------
+
+We welcome contributions.
+
+To learn more, see `Development <https://github.com/pytest-dev/pytest-metadata/blob/master/development.rst>`_
+
+Available metadata
+------------------
+
+The following metadata is gathered by this plugin:
+
+========  =============== ===================================
+Key       Description     Example
+========  =============== ===================================
+Python    Python version  3.6.4
+Platform  Platform        Darwin-17.4.0-x86_64-i386-64bit
+Packages  pytest packages {'py': '1.5.2', 'pytest': '3.4.1'}
+Plugins   pytest plugins  {'metadata': '1.6.0'}
+========  =============== ===================================
+
+Additional metadata
+-------------------
+
+You can provide your own metadata (key, value pair) by specifying ``--metadata`` on the commandline::
+
+   pytest --metadata foo bar
+
+Note: You can provide multiple sets of ``--metadata``::
+
+   pytest --metadata foo bar --metadata baz zoo
+
+There's also the possibility of passing in metadata as a JSON string::
+
+    pytest --metadata-from-json '{"cat_says": "bring the cat nip", "human_says": "yes kitty"}'
+
+Alternatively a JSON can be read from a given file::
+
+    pytest --metadata-from-json-file path/to/valid/file.json
+
+Continuous integration
+----------------------
+
+When run in a continuous integration environment, additional metadata is added
+from environment variables. Below is a list of the supported continuous
+integration providers, along with links to the environment variables that are
+added to metadata if they're present.
+
+* `AppVeyor <https://www.appveyor.com/docs/environment-variables/>`_
+* `Bitbucket <https://confluence.atlassian.com/bitbucket/environment-variables-794502608.html>`_
+* `CircleCI <https://circleci.com/docs/1.0/environment-variables/>`_
+* `GitLab CI <http://docs.gitlab.com/ce/ci/variables/README.html>`_
+* `Jenkins <https://wiki.jenkins-ci.org/display/JENKINS/Building+a+software+project#Buildingasoftwareproject-JenkinsSetEnvironmentVariables>`_
+* `TaskCluster <https://docs.taskcluster.net/reference/workers/docker-worker/environment>`_
+* `Travis CI <https://docs.travis-ci.com/user/environment-variables/>`_
+
+Note that if you're using `Tox <http://tox.readthedocs.io/>`_ to run your tests
+then you will need to `pass down any additional environment variables <http://tox.readthedocs.io/en/latest/example/basic.html#passing-down-environment-variables>`_
+for these to be picked up.
+
+Viewing metadata
+----------------
+
+If you pass ``--verbose`` on the command line when running your tests, then the
+metadata will be displayed in the terminal report header::
+
+  pytest --verbose
+  ============================ test session starts ============================
+  platform darwin -- Python 3.6.4, pytest-3.4.1, py-1.5.2, pluggy-0.6.0 -- /usr/bin/python
+  cachedir: .pytest_cache
+  metadata: {'Python': '3.6.4', 'Platform': 'Darwin-17.4.0-x86_64-i386-64bit', 'Packages': {'pytest': '3.4.1', 'py': '1.5.2', 'pluggy': '0.6.0'}, 'Plugins': {'metadata': '1.6.0'}}
+  plugins: metadata-1.6.0
+
+Including metadata in Junit XML
+-------------------------------
+
+Pytest-metadata provides the session scoped fixture :code:`include_metadata_in_junit_xml` that you may use to include any metadata in Junit XML as ``property`` tags.
+For example the following test module
+
+.. code-block:: python
+
+  import pytest
+
+  pytestmark = pytest.mark.usefixtures('include_metadata_in_junit_xml')
+
+  def test():
+      pass
+
+when called with
+
+.. code-block:: bash
+
+  pytest --metadata Daffy Duck --junit-xml=results.xml
+
+would produce the following XML
+
+.. code-block:: xml
+
+  <?xml version="1.0" encoding="utf-8"?>
+  <testsuites>
+    <testsuite name="pytest" errors="0" failures="0" skipped="0" tests="1" time="0.009" timestamp="2020-11-27T06:38:44.407674" hostname="sam">
+      <properties>
+        <property name="Daffy" value="Duck"/>
+  ...
+
+Accessing metadata
+------------------
+
+To add/modify/delete metadata at the end of metadata collection, you can use the ``pytest_metadata`` hook:
+
+.. code-block:: python
+
+  import pytest
+  @pytest.hookimpl(optionalhook=True)
+  def pytest_metadata(metadata):
+      metadata.pop("password", None)
+
+To access the metadata from a test or fixture, you can use the ``metadata``
+fixture:
+
+.. code-block:: python
+
+  def test_metadata(metadata):
+      assert 'metadata' in metadata['Plugins']
+
+To access the metadata from a plugin, you can use the ``stash`` attribute of
+the ``config`` object. This can be used to read/add/modify the metadata:
+
+.. code-block:: python
+
+  def pytest_configure(config):
+    metadata = config.pluginmanager.getplugin("metadata")
+    if metadata:
+        from pytest_metadata.plugin import metadata_key
+        config.stash[metadata_key]['foo'] = 'bar'
+
+Plugin integrations
+-------------------
+
+Here's a handy list of plugins that either read or contribute to the metadata:
+
+* `pytest-base-url <https://pypi.python.org/pypi/pytest-base-url/>`_ - Adds the
+  base URL to the metadata.
+* `pytest-html <https://pypi.python.org/pypi/pytest-html/>`_ - Displays the
+  metadata at the start of each report.
+* `pytest-reporter-html1 <https://pypi.org/project/pytest-reporter-html1/>`_ -
+  Presents metadata as part of the report.
+* `pytest-selenium <https://pypi.python.org/pypi/pytest-selenium/>`_ - Adds the
+  driver, capabilities, and remote server to the metadata.
+
+Resources
+---------
+
+- `Release Notes <http://github.com/davehunt/pytest-metadata/blob/master/CHANGES.rst>`_
+- `Issue Tracker <http://github.com/davehunt/pytest-metadata/issues>`_
+- `Code <http://github.com/davehunt/pytest-metadata/>`_
```

