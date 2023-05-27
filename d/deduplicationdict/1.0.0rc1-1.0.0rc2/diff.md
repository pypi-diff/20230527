# Comparing `tmp/deduplicationdict-1.0.0rc1.tar.gz` & `tmp/deduplicationdict-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deduplicationdict-1.0.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "deduplicationdict-1.0.0rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deduplicationdict-1.0.0rc1.tar` & `deduplicationdict-1.0.0rc2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    17190 2023-05-27 06:10:01.043229 deduplicationdict-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0     1326 2023-05-27 07:55:44.010882 deduplicationdict-1.0.0rc1/README.md
--rw-r--r--   0        0        0    10020 2023-05-27 06:44:12.394368 deduplicationdict-1.0.0rc1/deduplicationdict/__init__.py
--rw-r--r--   0        0        0     4008 2023-05-27 07:58:37.854292 deduplicationdict-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4250 1970-01-01 00:00:00.000000 deduplicationdict-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    17190 2023-05-27 06:10:01.043229 deduplicationdict-1.0.0rc2/LICENSE
+-rw-r--r--   0        0        0     1369 2023-05-27 08:06:02.215188 deduplicationdict-1.0.0rc2/README.md
+-rw-r--r--   0        0        0    10020 2023-05-27 06:44:12.394368 deduplicationdict-1.0.0rc2/deduplicationdict/__init__.py
+-rw-r--r--   0        0        0     3748 2023-05-27 08:09:53.417806 deduplicationdict-1.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4487 1970-01-01 00:00:00.000000 deduplicationdict-1.0.0rc2/PKG-INFO
```

### Comparing `deduplicationdict-1.0.0rc1/LICENSE` & `deduplicationdict-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `deduplicationdict-1.0.0rc1/README.md` & `deduplicationdict-1.0.0rc2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # DeDuplicationDict
 
 [![PyPI version](https://badge.fury.io/py/deduplicationdict.svg)](https://badge.fury.io/py/deduplicationdict)
 [![Documentation Status](https://readthedocs.org/projects/deduplicationdict/badge/?version=stable)](https://deduplicationdict.readthedocs.io/en/stable/?badge=stable)
-[![Python](https://img.shields.io/badge/python-3.7--3.11-blue)](https://badge.fury.io/py/deduplicationdict)
+[![Python](https://img.shields.io/badge/python-3.7--3.12-blue)](https://badge.fury.io/py/deduplicationdict)
 [![License: MPL 2.0](https://img.shields.io/badge/License-MPL_2.0-blue.svg)](https://opensource.org/licenses/MPL-2.0)
 
 [![Github](https://img.shields.io/badge/GitHub-Vivswan%2FDeDuplicationDict-blue)](https://github.com/Vivswan/DeDuplicationDict)
 
+A dictionary that de-duplicates values.
+
 A dictionary-like class that deduplicates values by storing them in a separate dictionary and replacing
 them with their corresponding hash values. This class is particularly useful for large dictionaries with
 repetitive entries, as it can save memory by storing values only once and substituting recurring values
 with their hash representations.
 
 This class supports nested structures by automatically converting nested dictionaries into
 `DeDuplicationDict` instances. It also provides various conversion methods to convert between regular
```

### Comparing `deduplicationdict-1.0.0rc1/deduplicationdict/__init__.py` & `deduplicationdict-1.0.0rc2/deduplicationdict/__init__.py`

 * *Files identical despite different names*

### Comparing `deduplicationdict-1.0.0rc1/pyproject.toml` & `deduplicationdict-1.0.0rc2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -10,49 +10,43 @@
 
 [tool.setuptools]
 py-modules = ['deduplicationdict']
 
 [project]
 # $ pip install deduplicationdict
 name = "deduplicationdict"
-version = "1.0.0rc1"
-description = ""  # Optional
+version = "1.0.0rc2"
+description = "A dictionary that de-duplicates values."
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
-keywords = ["python", "dict", "de"]
+keywords = ["python", "dict", "deduplication", "optimization", ]
 authors = [
     { name = "Vivswan Shah", email = "vivswanshah@pitt.edu" }
 ]
 maintainers = [
     { name = "Vivswan Shah", email = "vivswanshah@pitt.edu" }
 ]
 # For a list of valid classifiers, see https://pypi.org/classifiers/
-classifiers = [# Optional
-    # How mature is this project? Common values are
-    #   3 - Alpha
-    #   4 - Beta
-    #   5 - Production/Stable
+classifiers = [
     "Development Status :: 5 - Production/Stable",
-    # Indicate who your project is intended for
     "Intended Audience :: Developers",
-    "Intended Audience :: Science/Research",
+    "Intended Audience :: Information Technology",
     "Topic :: Software Development :: Build Tools",
-    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
-    # Pick your license as you wish
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    # Specify the Python versions you support here. In particular, ensure
-    # that you indicate you support Python 3. These classifiers are *not*
-    # checked by "pip install". See instead "python_requires" below.
+    "Topic :: File Formats :: JSON",
+    "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
 ]
 
 # This field lists other packages that your project depends on to run.
 # Any package you put here will be installed by pip when your project is
 # installed, so they must be valid existing projects.
 #
```

### Comparing `deduplicationdict-1.0.0rc1/PKG-INFO` & `deduplicationdict-1.0.0rc2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: deduplicationdict
-Version: 1.0.0rc1
-Summary: 
-Keywords: python,dict,de
+Version: 1.0.0rc2
+Summary: A dictionary that de-duplicates values.
+Keywords: python,dict,deduplication,optimization
 Author-email: Vivswan Shah <vivswanshah@pitt.edu>
 Maintainer-email: Vivswan Shah <vivswanshah@pitt.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Build Tools
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Topic :: File Formats :: JSON
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: deduplicationdict[dev,doc,test] ; extra == "all"
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: setuptools>=61.0.0 ; extra == "dev"
 Requires-Dist: build ; extra == "dev"
 Requires-Dist: twine ; extra == "dev"
 Requires-Dist: johnnydep ; extra == "dev"
@@ -62,19 +65,21 @@
 Provides-Extra: flake8
 Provides-Extra: test
 
 # DeDuplicationDict
 
 [![PyPI version](https://badge.fury.io/py/deduplicationdict.svg)](https://badge.fury.io/py/deduplicationdict)
 [![Documentation Status](https://readthedocs.org/projects/deduplicationdict/badge/?version=stable)](https://deduplicationdict.readthedocs.io/en/stable/?badge=stable)
-[![Python](https://img.shields.io/badge/python-3.7--3.11-blue)](https://badge.fury.io/py/deduplicationdict)
+[![Python](https://img.shields.io/badge/python-3.7--3.12-blue)](https://badge.fury.io/py/deduplicationdict)
 [![License: MPL 2.0](https://img.shields.io/badge/License-MPL_2.0-blue.svg)](https://opensource.org/licenses/MPL-2.0)
 
 [![Github](https://img.shields.io/badge/GitHub-Vivswan%2FDeDuplicationDict-blue)](https://github.com/Vivswan/DeDuplicationDict)
 
+A dictionary that de-duplicates values.
+
 A dictionary-like class that deduplicates values by storing them in a separate dictionary and replacing
 them with their corresponding hash values. This class is particularly useful for large dictionaries with
 repetitive entries, as it can save memory by storing values only once and substituting recurring values
 with their hash representations.
 
 This class supports nested structures by automatically converting nested dictionaries into
 `DeDuplicationDict` instances. It also provides various conversion methods to convert between regular
```

