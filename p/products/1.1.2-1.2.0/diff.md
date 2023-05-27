# Comparing `tmp/products-1.1.2.tar.gz` & `tmp/products-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "products-1.1.2.tar", last modified: Mon Aug  1 07:18:03 2022, max compression
+gzip compressed data, was "products-1.2.0.tar", last modified: Sat May 27 21:34:27 2023, max compression
```

## Comparing `products-1.1.2.tar` & `products-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-08-01 07:18:03.224267 products-1.1.2/
--rw-rw-rw-   0        0        0     1091 2022-05-09 00:08:37.000000 products-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     7650 2022-08-01 07:18:03.224022 products-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     7080 2022-08-01 07:04:37.000000 products-1.1.2/README.rst
--rw-rw-rw-   0        0        0     1086 2022-08-01 07:04:20.000000 products-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-01 07:18:03.224267 products-1.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-01 07:18:03.213492 products-1.1.2/src/
-drwxrwxrwx   0        0        0        0 2022-08-01 07:18:03.215106 products-1.1.2/src/products/
--rw-rw-rw-   0        0        0       90 2022-05-09 00:08:37.000000 products-1.1.2/src/products/__init__.py
--rw-rw-rw-   0        0        0     6327 2022-08-01 07:13:30.000000 products-1.1.2/src/products/products.py
-drwxrwxrwx   0        0        0        0 2022-08-01 07:18:03.223295 products-1.1.2/src/products.egg-info/
--rw-rw-rw-   0        0        0     7650 2022-08-01 07:18:02.000000 products-1.1.2/src/products.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2022-08-01 07:18:03.000000 products-1.1.2/src/products.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-01 07:18:02.000000 products-1.1.2/src/products.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      225 2022-08-01 07:18:03.000000 products-1.1.2/src/products.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-08-01 07:18:03.000000 products-1.1.2/src/products.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 21:34:27.320603 products-1.2.0/
+-rw-rw-rw-   0        0        0     1091 2022-05-09 00:08:37.000000 products-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     7960 2023-05-27 21:34:27.320603 products-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7390 2023-05-05 04:44:45.000000 products-1.2.0/README.rst
+-rw-rw-rw-   0        0        0     1087 2023-05-05 04:48:21.000000 products-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 21:34:27.320603 products-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 21:34:27.301598 products-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 21:34:27.311099 products-1.2.0/src/products/
+-rw-rw-rw-   0        0        0       90 2022-05-09 00:08:37.000000 products-1.2.0/src/products/__init__.py
+-rw-rw-rw-   0        0        0     6327 2022-08-01 07:13:30.000000 products-1.2.0/src/products/products.py
+drwxrwxrwx   0        0        0        0 2023-05-27 21:34:27.320603 products-1.2.0/src/products.egg-info/
+-rw-rw-rw-   0        0        0     7960 2023-05-27 21:34:27.000000 products-1.2.0/src/products.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-05-27 21:34:27.000000 products-1.2.0/src/products.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 21:34:27.000000 products-1.2.0/src/products.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      226 2023-05-27 21:34:27.000000 products-1.2.0/src/products.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-27 21:34:27.000000 products-1.2.0/src/products.egg-info/top_level.txt
```

### Comparing `products-1.1.2/LICENSE` & `products-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `products-1.1.2/PKG-INFO` & `products-1.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: products
-Version: 1.1.2
+Version: 1.2.0
 Summary: Simple function for building ensembles of iterables that are disjoint partitions of an overall Cartesian product.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/lapets/products
 Project-URL: Documentation, https://products.readthedocs.io
 Requires-Python: >=3.7
@@ -45,113 +45,139 @@
 
 .. |itertools_product| replace:: ``itertools.product``
 .. _itertools_product: https://docs.python.org/3/library/itertools.html#itertools.product
 
 Once the |itertools_product|_ has been used to build an iterable representing a `Cartesian product <https://en.wikipedia.org/wiki/Cartesian_product>`__, it is already too late to partition that iterable into multiple iterables where each one represents a subset of the product set. Iterables representing disjoint subsets can, for example, make it easier to employ parallelization when processing the product set.
 
 .. |products| replace:: ``products``
-.. _products: https://products.readthedocs.io/en/1.1.2/_source/products.html#products.products.products
+.. _products: https://products.readthedocs.io/en/1.2.0/_source/products.html#products.products.products
 
 The |products|_ function in this package constructs a list of independent `iterators <https://docs.python.org/3/glossary.html#term-iterator>`__ for a specified number of disjoint subsets of a product set (in the manner of the `parts <https://pypi.org/project/parts>`__ library), exploiting as much information as is available about the constituent factor sets of the overall product set in order to do so.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/products>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/products>`__:
+
+.. code-block:: bash
 
     python -m pip install products
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import products
     from products import products
 
 Examples
 ^^^^^^^^
 
 .. |product| replace:: ``product``
 .. _product: https://docs.python.org/3/library/itertools.html#itertools.product
 
-This library provides an alternative to the built-in Cartesian product function |product|_ found in `itertools <https://docs.python.org/3/library/itertools.html>`__, making it possible to iterate over multiple disjoint subsets of a Cartesian product (even in parallel). Consider the Cartesian product below::
+This library provides an alternative to the built-in Cartesian product function |product|_ found in `itertools <https://docs.python.org/3/library/itertools.html>`__, making it possible to iterate over multiple disjoint subsets of a Cartesian product (even in parallel). Consider the Cartesian product below:
+
+.. code-block:: python
 
     >>> from itertools import product
     >>> p = product([1, 2], {'a', 'b'}, (False, True))
     >>> for t in p:
     ...     print(t)
     (1, 'a', False)
     (1, 'a', True)
     (1, 'b', False)
     (1, 'b', True)
     (2, 'a', False)
     (2, 'a', True)
     (2, 'b', False)
     (2, 'b', True)
 
-This library makes it possible to create a number of iterators such that each iterator represents a disjoint subset of the overall Cartesian product. The example below does so for the Cartesian product introduced above, creating four disjoint subsets (rather than one overall set)::
+This library makes it possible to create a number of iterators such that each iterator represents a disjoint subset of the overall Cartesian product. The example below does so for the Cartesian product introduced above, creating four disjoint subsets (rather than one overall set):
+
+.. code-block:: python
 
     >>> from products import products
     >>> ss = products([1, 2], {'a', 'b'}, (True, False), number=4)
     >>> for s in ss:
     ...     print(list(s))
     [(1, 'a', True), (1, 'a', False)]
     [(1, 'b', True), (1, 'b', False)]
     [(2, 'a', True), (2, 'a', False)]
     [(2, 'b', True), (2, 'b', False)]
 
 The `iterable <https://docs.python.org/3/glossary.html#term-iterable>`__ corresponding to each subset is *independent* from the others, making it possible to employ techniques such parallelization (*e.g.*, using the built-in `multiprocessing <https://docs.python.org/3/library/multiprocessing.html>`__ library) when operating on the elements of the overall Cartesian product.
 
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
 
     python src/products/products.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/products
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/products>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/products>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/products>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `products-1.1.2/README.rst` & `products-1.2.0/src/products.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: products
+Version: 1.2.0
+Summary: Simple function for building ensembles of iterables that are disjoint partitions of an overall Cartesian product.
+Author: Andrei Lapets
+Author-email: a@lapets.io
+License: MIT
+Project-URL: Repository, https://github.com/lapets/products
+Project-URL: Documentation, https://products.readthedocs.io
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: coveralls
+Provides-Extra: publish
+License-File: LICENSE
+
 ========
 products
 ========
 
 Simple function for building ensembles of iterables that are disjoint partitions of an overall Cartesian product.
 
 |pypi| |readthedocs| |actions| |coveralls|
@@ -27,113 +45,139 @@
 
 .. |itertools_product| replace:: ``itertools.product``
 .. _itertools_product: https://docs.python.org/3/library/itertools.html#itertools.product
 
 Once the |itertools_product|_ has been used to build an iterable representing a `Cartesian product <https://en.wikipedia.org/wiki/Cartesian_product>`__, it is already too late to partition that iterable into multiple iterables where each one represents a subset of the product set. Iterables representing disjoint subsets can, for example, make it easier to employ parallelization when processing the product set.
 
 .. |products| replace:: ``products``
-.. _products: https://products.readthedocs.io/en/1.1.2/_source/products.html#products.products.products
+.. _products: https://products.readthedocs.io/en/1.2.0/_source/products.html#products.products.products
 
 The |products|_ function in this package constructs a list of independent `iterators <https://docs.python.org/3/glossary.html#term-iterator>`__ for a specified number of disjoint subsets of a product set (in the manner of the `parts <https://pypi.org/project/parts>`__ library), exploiting as much information as is available about the constituent factor sets of the overall product set in order to do so.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/products>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/products>`__:
+
+.. code-block:: bash
 
     python -m pip install products
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import products
     from products import products
 
 Examples
 ^^^^^^^^
 
 .. |product| replace:: ``product``
 .. _product: https://docs.python.org/3/library/itertools.html#itertools.product
 
-This library provides an alternative to the built-in Cartesian product function |product|_ found in `itertools <https://docs.python.org/3/library/itertools.html>`__, making it possible to iterate over multiple disjoint subsets of a Cartesian product (even in parallel). Consider the Cartesian product below::
+This library provides an alternative to the built-in Cartesian product function |product|_ found in `itertools <https://docs.python.org/3/library/itertools.html>`__, making it possible to iterate over multiple disjoint subsets of a Cartesian product (even in parallel). Consider the Cartesian product below:
+
+.. code-block:: python
 
     >>> from itertools import product
     >>> p = product([1, 2], {'a', 'b'}, (False, True))
     >>> for t in p:
     ...     print(t)
     (1, 'a', False)
     (1, 'a', True)
     (1, 'b', False)
     (1, 'b', True)
     (2, 'a', False)
     (2, 'a', True)
     (2, 'b', False)
     (2, 'b', True)
 
-This library makes it possible to create a number of iterators such that each iterator represents a disjoint subset of the overall Cartesian product. The example below does so for the Cartesian product introduced above, creating four disjoint subsets (rather than one overall set)::
+This library makes it possible to create a number of iterators such that each iterator represents a disjoint subset of the overall Cartesian product. The example below does so for the Cartesian product introduced above, creating four disjoint subsets (rather than one overall set):
+
+.. code-block:: python
 
     >>> from products import products
     >>> ss = products([1, 2], {'a', 'b'}, (True, False), number=4)
     >>> for s in ss:
     ...     print(list(s))
     [(1, 'a', True), (1, 'a', False)]
     [(1, 'b', True), (1, 'b', False)]
     [(2, 'a', True), (2, 'a', False)]
     [(2, 'b', True), (2, 'b', False)]
 
 The `iterable <https://docs.python.org/3/glossary.html#term-iterable>`__ corresponding to each subset is *independent* from the others, making it possible to employ techniques such parallelization (*e.g.*, using the built-in `multiprocessing <https://docs.python.org/3/library/multiprocessing.html>`__ library) when operating on the elements of the overall Cartesian product.
 
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
 
     python src/products/products.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/products
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/products>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/products>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/products>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `products-1.1.2/pyproject.toml` & `products-1.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 [project]
 name = "products"
-version = "1.1.2"
+version = "1.2.0"
 description = """\
     Simple function for building ensembles of iterables \
     that are disjoint partitions of an overall Cartesian \
     product.
     """
 license = {text = "MIT"}
 authors = [
     {name = "Andrei Lapets"},
     {email = "a@lapets.io"}
 ]
 readme = "README.rst"
 requires-python = ">=3.7"
 dependencies = [
-    "parts~=1.5"
+    "parts~=1.6"
 ]
 
 [project.urls]
 Repository = "https://github.com/lapets/products"
 Documentation = "https://products.readthedocs.io"
 
 [project.optional-dependencies]
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
 addopts = "--doctest-modules --ignore=docs --cov=products --cov-report term-missing"
```

### Comparing `products-1.1.2/src/products/products.py` & `products-1.2.0/src/products/products.py`

 * *Files identical despite different names*

