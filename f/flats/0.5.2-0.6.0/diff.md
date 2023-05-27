# Comparing `tmp/flats-0.5.2.tar.gz` & `tmp/flats-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flats-0.5.2.tar", last modified: Mon Aug  1 06:47:54 2022, max compression
+gzip compressed data, was "flats-0.6.0.tar", last modified: Sat May 27 21:31:35 2023, max compression
```

## Comparing `flats-0.5.2.tar` & `flats-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-08-01 06:47:54.593426 flats-0.5.2/
--rw-rw-rw-   0        0        0     1091 2022-05-09 00:01:59.000000 flats-0.5.2/LICENSE
--rw-rw-rw-   0        0        0     6303 2022-08-01 06:47:54.593361 flats-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     5776 2022-08-01 06:45:42.000000 flats-0.5.2/README.rst
--rw-rw-rw-   0        0        0      995 2022-08-01 06:34:51.000000 flats-0.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-01 06:47:54.593426 flats-0.5.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-01 06:47:54.580892 flats-0.5.2/src/
-drwxrwxrwx   0        0        0        0 2022-08-01 06:47:54.584481 flats-0.5.2/src/flats/
--rw-rw-rw-   0        0        0       81 2022-05-09 00:01:59.000000 flats-0.5.2/src/flats/__init__.py
--rw-rw-rw-   0        0        0     5768 2022-08-01 06:40:08.000000 flats-0.5.2/src/flats/flats.py
-drwxrwxrwx   0        0        0        0 2022-08-01 06:47:54.592558 flats-0.5.2/src/flats.egg-info/
--rw-rw-rw-   0        0        0     6303 2022-08-01 06:47:54.000000 flats-0.5.2/src/flats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2022-08-01 06:47:54.000000 flats-0.5.2/src/flats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-01 06:47:54.000000 flats-0.5.2/src/flats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2022-08-01 06:47:54.000000 flats-0.5.2/src/flats.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-08-01 06:47:54.000000 flats-0.5.2/src/flats.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 21:31:35.495849 flats-0.6.0/
+-rw-rw-rw-   0        0        0     1091 2022-05-09 00:01:59.000000 flats-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     6638 2023-05-27 21:31:35.495849 flats-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6111 2023-05-25 22:02:44.000000 flats-0.6.0/README.rst
+-rw-rw-rw-   0        0        0      996 2023-05-25 22:02:44.000000 flats-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 21:31:35.495849 flats-0.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 21:31:35.470241 flats-0.6.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 21:31:35.481967 flats-0.6.0/src/flats/
+-rw-rw-rw-   0        0        0       81 2022-05-09 00:01:59.000000 flats-0.6.0/src/flats/__init__.py
+-rw-rw-rw-   0        0        0     5766 2023-05-02 16:05:34.000000 flats-0.6.0/src/flats/flats.py
+drwxrwxrwx   0        0        0        0 2023-05-27 21:31:35.494847 flats-0.6.0/src/flats.egg-info/
+-rw-rw-rw-   0        0        0     6638 2023-05-27 21:31:35.000000 flats-0.6.0/src/flats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-05-27 21:31:35.000000 flats-0.6.0/src/flats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 21:31:35.000000 flats-0.6.0/src/flats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      215 2023-05-27 21:31:35.000000 flats-0.6.0/src/flats.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-27 21:31:35.000000 flats-0.6.0/src/flats.egg-info/top_level.txt
```

### Comparing `flats-0.5.2/LICENSE` & `flats-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flats-0.5.2/PKG-INFO` & `flats-0.6.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flats
-Version: 0.5.2
+Version: 0.6.0
 Summary: Minimal library that enables flattening of nested instances of container types.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/lapets/flats
 Project-URL: Documentation, https://flats.readthedocs.io
 Requires-Python: >=3.7
@@ -38,106 +38,134 @@
 
 .. |coveralls| image:: https://coveralls.io/repos/github/lapets/flats/badge.svg?branch=main
    :target: https://coveralls.io/github/lapets/flats?branch=main
    :alt: Coveralls test coverage summary.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/flats>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/flats>`__:
+
+.. code-block:: bash
 
     python -m pip install flats
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import flats
     from flats import flats
 
 Examples
 ^^^^^^^^
 
 .. |Iterable| replace:: ``Iterable``
 .. _Iterable: https://docs.python.org/3/library/collections.abc.html#collections.abc.Iterable
 
 .. |Generator| replace:: ``Generator``
 .. _Generator: https://docs.python.org/3/library/collections.abc.html#collections.abc.Generator
 
-This library provides a function that can flatten any instance of a container type that is the root of a tree of nested instances of container types, returning as an iterable the sequence of all objects or values (that are not of a container type) encountered during an in-order traversal. Any instance of the |Iterable|_ class or the |Generator|_ class is considered to be an instance of a container type by this library::
+This library provides a function that can flatten any instance of a container type that is the root of a tree of nested instances of container types, returning as an iterable the sequence of all objects or values (that are not of a container type) encountered during an in-order traversal. Any instance of the |Iterable|_ class or the |Generator|_ class is considered to be an instance of a container type by this library:
+
+.. code-block:: python
 
     >>> from flats import flats
     >>> list(flats([[1, 2, 3], [4, 5, 6, 7]]))
     [1, 2, 3, 4, 5, 6, 7]
 
-The nested instances need not be of the same type::
+The nested instances need not be of the same type:
+
+.. code-block:: python
 
     >>> tuple(flats([{1}, {2}, {3}, frozenset({4}), iter([5, 6, 7])]))
     (1, 2, 3, 4, 5, 6, 7)
     >>> list(flats(['abc', 'xyz']))
     ['a', 'b', 'c', 'x', 'y', 'z']
     >>> list(flats([range(3), range(3)]))
     [0, 1, 2, 0, 1, 2]
 
-It is also possible to limit the depth to which nested instances of a container type are recursively traversed during the flattening process (leaving unmodified the nesting of any instances that are found at a greater depth)::
+It is also possible to limit the depth to which nested instances of a container type are recursively traversed during the flattening process (leaving unmodified the nesting of any instances that are found at a greater depth):
+
+.. code-block:: python
 
     >>> list(flats([[[1, 2], 3], [4, 5, 6, 7]], depth=1))
     [[1, 2], 3, 4, 5, 6, 7]
     >>> list(flats([[[1, 2], 3], [4, 5, 6, 7]], depth=2))
     [1, 2, 3, 4, 5, 6, 7]
     >>> list(flats([[[1, [2]], 3], [4, [[[5]]], 6, 7]], depth=float('inf')))
     [1, 2, 3, 4, 5, 6, 7]
 
 Development
 -----------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs,lint]
 
 Documentation
 ^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs]
     cd docs
     sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/flats/flats.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/flats
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/flats>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/flats>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/flats>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
     python -m build --sdist --wheel .
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

### Comparing `flats-0.5.2/pyproject.toml` & `flats-0.6.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flats"
-version = "0.5.2"
+version = "0.6.0"
 description = """\
     Minimal library that enables flattening \
     of nested instances of container types.\
     """
 license = {text = "MIT"}
 authors = [
     {name = "Andrei Lapets"},
@@ -21,29 +21,29 @@
 docs = [
     "toml~=0.10.2",
     "sphinx~=4.2.0",
     "sphinx-rtd-theme~=1.0.0",
     "sphinx-autodoc-typehints~=1.12.0"
 ]
 test = [
-    "pytest~=7.0",
-    "pytest-cov~=3.0"
+    "pytest~=7.2",
+    "pytest-cov~=4.0"
 ]
 lint = [
-    "pylint~=2.14.0"
+    "pylint~=2.17.0"
 ]
 coveralls = [
     "coveralls~=3.3.1"
 ]
 publish = [
-    "build~=0.8",
+    "build~=0.10",
     "twine~=4.0"
 ]
 
 [build-system]
 requires = [
-    "setuptools~=62.0"
+    "setuptools~=67.6"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --ignore=docs --cov=flats --cov-report term-missing"
```

### Comparing `flats-0.5.2/src/flats/flats.py` & `flats-0.6.0/src/flats/flats.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     elif depth == 0: # For consistency, base case is also a generator.
         for xs in xss:
             yield xs
     else: # General recursive case.
         for xs in xss:
             if isinstance(depth, int) and depth >= 1:
                 if _is_container(xs):
-                    for x in flats(xs, depth=(depth - 1)):
+                    for x in flats(xs, depth=depth - 1):
                         yield x
                 else:
                     yield xs
             elif depth == float('inf'):
                 if _is_container(xs):
                     for x in flats(xs, depth=float('inf')):
                         yield x
```

### Comparing `flats-0.5.2/src/flats.egg-info/PKG-INFO` & `flats-0.6.0/src/flats.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flats
-Version: 0.5.2
+Version: 0.6.0
 Summary: Minimal library that enables flattening of nested instances of container types.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/lapets/flats
 Project-URL: Documentation, https://flats.readthedocs.io
 Requires-Python: >=3.7
@@ -38,106 +38,134 @@
 
 .. |coveralls| image:: https://coveralls.io/repos/github/lapets/flats/badge.svg?branch=main
    :target: https://coveralls.io/github/lapets/flats?branch=main
    :alt: Coveralls test coverage summary.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/flats>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/flats>`__:
+
+.. code-block:: bash
 
     python -m pip install flats
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import flats
     from flats import flats
 
 Examples
 ^^^^^^^^
 
 .. |Iterable| replace:: ``Iterable``
 .. _Iterable: https://docs.python.org/3/library/collections.abc.html#collections.abc.Iterable
 
 .. |Generator| replace:: ``Generator``
 .. _Generator: https://docs.python.org/3/library/collections.abc.html#collections.abc.Generator
 
-This library provides a function that can flatten any instance of a container type that is the root of a tree of nested instances of container types, returning as an iterable the sequence of all objects or values (that are not of a container type) encountered during an in-order traversal. Any instance of the |Iterable|_ class or the |Generator|_ class is considered to be an instance of a container type by this library::
+This library provides a function that can flatten any instance of a container type that is the root of a tree of nested instances of container types, returning as an iterable the sequence of all objects or values (that are not of a container type) encountered during an in-order traversal. Any instance of the |Iterable|_ class or the |Generator|_ class is considered to be an instance of a container type by this library:
+
+.. code-block:: python
 
     >>> from flats import flats
     >>> list(flats([[1, 2, 3], [4, 5, 6, 7]]))
     [1, 2, 3, 4, 5, 6, 7]
 
-The nested instances need not be of the same type::
+The nested instances need not be of the same type:
+
+.. code-block:: python
 
     >>> tuple(flats([{1}, {2}, {3}, frozenset({4}), iter([5, 6, 7])]))
     (1, 2, 3, 4, 5, 6, 7)
     >>> list(flats(['abc', 'xyz']))
     ['a', 'b', 'c', 'x', 'y', 'z']
     >>> list(flats([range(3), range(3)]))
     [0, 1, 2, 0, 1, 2]
 
-It is also possible to limit the depth to which nested instances of a container type are recursively traversed during the flattening process (leaving unmodified the nesting of any instances that are found at a greater depth)::
+It is also possible to limit the depth to which nested instances of a container type are recursively traversed during the flattening process (leaving unmodified the nesting of any instances that are found at a greater depth):
+
+.. code-block:: python
 
     >>> list(flats([[[1, 2], 3], [4, 5, 6, 7]], depth=1))
     [[1, 2], 3, 4, 5, 6, 7]
     >>> list(flats([[[1, 2], 3], [4, 5, 6, 7]], depth=2))
     [1, 2, 3, 4, 5, 6, 7]
     >>> list(flats([[[1, [2]], 3], [4, [[[5]]], 6, 7]], depth=float('inf')))
     [1, 2, 3, 4, 5, 6, 7]
 
 Development
 -----------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs,lint]
 
 Documentation
 ^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs]
     cd docs
     sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/flats/flats.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/flats
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/flats>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/flats>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/flats>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
     python -m build --sdist --wheel .
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

