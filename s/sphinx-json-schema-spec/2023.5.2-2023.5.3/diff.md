# Comparing `tmp/sphinx_json_schema_spec-2023.5.2.tar.gz` & `tmp/sphinx_json_schema_spec-2023.5.3.tar.gz`

## Comparing `sphinx_json_schema_spec-2023.5.2.tar` & `sphinx_json_schema_spec-2023.5.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/.flake8
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/.readthedocs.yml
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/noxfile.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/.github/release.yml
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/docs/Makefile
--rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/docs/conf.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/docs/index.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/docs/requirements.in
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/docs/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/sphinx_json_schema_spec/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/sphinx_json_schema_spec/tests/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/sphinx_json_schema_spec/tests/test_sphinx.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/COPYING
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/README.rst
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/pyproject.toml
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.2/PKG-INFO
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/.flake8
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/.readthedocs.yml
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/noxfile.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/.github/FUNDING.yml
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/.github/release.yml
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/docs/Makefile
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/docs/conf.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/docs/index.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/docs/requirements.in
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/docs/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/sphinx_json_schema_spec/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/sphinx_json_schema_spec/tests/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/sphinx_json_schema_spec/tests/test_sphinx.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/COPYING
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/README.rst
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.5.3/PKG-INFO
```

### Comparing `sphinx_json_schema_spec-2023.5.2/.pre-commit-config.yaml` & `sphinx_json_schema_spec-2023.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.2/noxfile.py` & `sphinx_json_schema_spec-2023.5.3/noxfile.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pathlib import Path
 
 import nox
 
 ROOT = Path(__file__).parent
+PYPROJECT = ROOT / "pyproject.toml"
 DOCS = ROOT / "docs"
 PACKAGE = ROOT / "sphinx_json_schema_spec"
 
 
 nox.options.sessions = []
 
 
@@ -15,52 +16,51 @@
         if default:
             nox.options.sessions.append(kwargs.get("name", fn.__name__))
         return nox.session(**kwargs)(fn)
 
     return _session
 
 
-@session(python=["3.7", "3.8", "3.9", "3.10", "3.11", "pypy3"])
+@session(python=["3.8", "3.9", "3.10", "3.11", "pypy3"])
 def tests(session):
-    session.install("pytest", str(ROOT))
-    session.run("pytest", "--verbosity=3")
+    session.install("pytest", ROOT)
+    session.run("pytest", *session.posargs, PACKAGE)
+
+
+@session()
+def audit(session):
+    session.install("pip-audit", ROOT)
+    session.run("python", "-m", "pip_audit")
 
 
 @session(tags=["build"])
 def build(session):
     session.install("build")
     tmpdir = session.create_tmp()
-    session.run("python", "-m", "build", str(ROOT), "--outdir", tmpdir)
+    session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
 
 
 @session(tags=["style"])
 def readme(session):
     session.install("build", "twine")
     tmpdir = session.create_tmp()
-    session.run("python", "-m", "build", str(ROOT), "--outdir", tmpdir)
+    session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
     session.run("python", "-m", "twine", "check", tmpdir + "/*")
 
 
 @session(tags=["style"])
 def style(session):
-    session.install(
-        "flake8",
-        "flake8-broken-line",
-        "flake8-bugbear",
-        "flake8-commas",
-        "flake8-quotes",
-        "flake8-tidy-imports",
-    )
-    session.run("python", "-m", "flake8", str(PACKAGE), __file__)
+    session.install("ruff")
+    session.run("ruff", "check", ROOT)
 
 
 @session()
 def typing(session):
-    session.install("mypy", "types-docutils", "types-lxml", str(ROOT))
-    session.run("python", "-m", "mypy", str(PACKAGE))
+    session.install("mypy", "types-docutils", "types-lxml", ROOT)
+    session.run("python", "-m", "mypy", PACKAGE)
 
 
 @session(tags=["docs"])
 @nox.parametrize(
     "builder",
     [
         nox.param(name, id=name)
@@ -70,32 +70,32 @@
             "linkcheck",
             "man",
             "spelling",
         ]
     ],
 )
 def docs(session, builder):
-    session.install("-r", str(DOCS / "requirements.txt"))
+    session.install("-r", DOCS / "requirements.txt")
     tmpdir = Path(session.create_tmp())
     argv = ["-n", "-T", "-W"]
     if builder != "spelling":
         argv += ["-q"]
     session.run(
         "python",
         "-m",
         "sphinx",
         "-b",
         builder,
-        str(DOCS),
-        str(tmpdir / builder),
+        DOCS,
+        tmpdir / builder,
         *argv,
     )
 
 
 @session(tags=["docs", "style"], name="docs(style)")
 def docs_style(session):
     session.install(
         "doc8",
         "pygments",
         "pygments-github-lexers",
     )
-    session.run("python", "-m", "doc8", "--max-line-length", "1000", str(DOCS))
+    session.run("python", "-m", "doc8", "--config", PYPROJECT, DOCS)
```

### Comparing `sphinx_json_schema_spec-2023.5.2/.github/SECURITY.md` & `sphinx_json_schema_spec-2023.5.3/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.2/.github/workflows/ci.yml` & `sphinx_json_schema_spec-2023.5.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.2/docs/Makefile` & `sphinx_json_schema_spec-2023.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.2/docs/index.rst` & `sphinx_json_schema_spec-2023.5.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.2/docs/requirements.txt` & `sphinx_json_schema_spec-2023.5.3/docs/requirements.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,98 @@
 #
-# This file is autogenerated by pip-compile with python 3.11
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.11
+# by the following command:
 #
-#    pip-compile docs/requirements.in
+#    pip-compile --resolver=backtracking docs/requirements.in
 #
-alabaster==0.7.12
+alabaster==0.7.13
     # via sphinx
-babel==2.11.0
+babel==2.12.1
     # via sphinx
-beautifulsoup4==4.11.1
+beautifulsoup4==4.12.2
     # via furo
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
     # via requests
-docutils==0.19
-    # via sphinx
-furo==2022.12.7
+contourpy==1.0.7
+    # via matplotlib
+cycler==0.11.0
+    # via matplotlib
+docutils==0.20.1
+    # via sphinx
+fonttools==4.39.4
+    # via matplotlib
+furo==2023.5.20
     # via -r docs/requirements.in
 idna==3.4
     # via requests
 imagesize==1.4.1
     # via sphinx
 jinja2==3.1.2
     # via sphinx
+kiwisolver==1.4.4
+    # via matplotlib
 lxml==4.9.2
     # via sphinx-json-schema-spec
-markupsafe==2.1.1
+markupsafe==2.1.2
     # via jinja2
-packaging==22.0
-    # via sphinx
+matplotlib==3.7.1
+    # via sphinxext-opengraph
+numpy==1.24.3
+    # via
+    #   contourpy
+    #   matplotlib
+packaging==23.1
+    # via
+    #   matplotlib
+    #   sphinx
+pillow==9.5.0
+    # via matplotlib
 pyenchant==3.2.2
     # via sphinxcontrib-spelling
-pygments==2.13.0
+pygments==2.15.1
     # via
     #   furo
     #   sphinx
-pytz==2022.6
-    # via babel
-requests==2.28.1
+pyparsing==3.0.9
+    # via matplotlib
+python-dateutil==2.8.2
+    # via matplotlib
+requests==2.31.0
     # via sphinx
+six==1.16.0
+    # via python-dateutil
 snowballstemmer==2.2.0
     # via sphinx
-soupsieve==2.3.2.post1
+soupsieve==2.4.1
     # via beautifulsoup4
-sphinx==5.3.0
+sphinx==7.0.1
     # via
     #   -r docs/requirements.in
     #   furo
     #   sphinx-basic-ng
     #   sphinx-json-schema-spec
     #   sphinxcontrib-spelling
+    #   sphinxext-opengraph
 sphinx-basic-ng==1.0.0b1
     # via furo
 file:.#egg=sphinx_json_schema_spec
     # via -r docs/requirements.in
-sphinxcontrib-applehelp==1.0.2
+sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sphinxcontrib-spelling==7.7.0
+sphinxcontrib-spelling==8.0.0
+    # via -r docs/requirements.in
+sphinxext-opengraph==0.8.2
     # via -r docs/requirements.in
-urllib3==1.26.13
+urllib3==2.0.2
     # via requests
```

### Comparing `sphinx_json_schema_spec-2023.5.2/sphinx_json_schema_spec/__init__.py` & `sphinx_json_schema_spec-2023.5.3/sphinx_json_schema_spec/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Sphinx support for interlinking to the JSON Schema specifications.
+"""
 from contextlib import suppress
 from datetime import datetime
 from pathlib import Path
 from urllib.parse import urljoin
 import ssl
 import urllib.request
 
@@ -31,15 +34,14 @@
 
     Arguments:
 
         app (sphinx.application.Sphinx):
 
             the Sphinx application context
     """
-
     app.add_config_value("cache_path", "_cache", "")
 
     CACHE = Path(app.config.cache_path)
     CACHE.mkdir(exist_ok=True)
 
     documents = {
         url: fetch_or_load(cache_path=CACHE / f"{name}.html", url=url)
@@ -66,15 +68,14 @@
 
             the local path to a (possibly not yet existing) cache for the file
 
         url:
 
             the URL of the document
     """
-
     version = metadata.version("sphinx-json-schema-spec")
     headers = {"User-Agent": f"sphinx-json-schema-spec v{version}"}
 
     with suppress(FileNotFoundError):
         modified = datetime.utcfromtimestamp(cache_path.stat().st_mtime)
         date = modified.strftime("%a, %d %b %Y %I:%M:%S UTC")
         headers["If-Modified-Since"] = date
@@ -107,15 +108,15 @@
 
         Arguments:
 
             name (str):
 
                 the name of the role in the document
 
-            raw_source (str):
+            raw_text (str):
 
                 the raw text (role with argument)
 
             text (str):
 
                 the argument given to the role
 
@@ -130,15 +131,14 @@
         Returns:
 
             tuple:
 
                 a 2-tuple of nodes to insert into the document and an
                 iterable of system messages, both possibly empty
         """
-
         hardcoded = HARDCODED.get(text)
         if hardcoded is not None:
             return [nodes.reference(raw_text, text, refuri=hardcoded)], []
 
         # find the header in the validation spec containing matching text
         for vocabulary_url, spec in vocabularies.items():
             lower = text.lstrip("$").lower()
@@ -149,38 +149,37 @@
                     None,
                 )
 
             if header is not None:
                 uri = urljoin(vocabulary_url, header.find("a").attrib["href"])
                 break
         else:
-            inliner.reporter.warning(
-                "Didn't find a target for {0}".format(text),
-            )
+            inliner.reporter.warning(f"Didn't find a target for {text}")
             uri = BASE_URL
 
         reference = nodes.reference(raw_text, text, refuri=uri)
         return [reference], []
 
     return keyword
 
 
 def missing_reference(glossary):
-
+    """
+    Get callbacked for Sphinx's missing reference hook.
+    """
     terms = {
         link.lstrip("#")
         for _, _, link, _ in glossary.iterlinks()
         if link.startswith("#")
     }
 
     def _missing_reference(app, env, node, contnod):
         """
         Resolve a reference to a JSON Schema Glossary term.
         """
-
         if node["reftype"] != "term":
             return
 
         target = node["reftarget"]
         if target not in terms:
             return
```

### Comparing `sphinx_json_schema_spec-2023.5.2/.gitignore` & `sphinx_json_schema_spec-2023.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.2/COPYING` & `sphinx_json_schema_spec-2023.5.3/COPYING`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.2/README.rst` & `sphinx_json_schema_spec-2023.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.5.2/PKG-INFO` & `sphinx_json_schema_spec-2023.5.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: sphinx_json_schema_spec
-Version: 2023.5.2
+Version: 2023.5.3
 Summary: Sphinx support for the JSON Schema specifications
+Project-URL: Documentation, https://sphinx-json-schema-spec.readthedocs.io/
 Project-URL: Homepage, https://github.com/python-jsonschema/sphinx-json-schema-spec
 Project-URL: Issues, https://github.com/python-jsonschema/sphinx-json-schema-spec/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/python-jsonschema/sphinx-json-schema-spec
 Author: Julian Berman
 Author-email: Julian+sphinx-json-schema-spec@GrayVines.com
 License: MIT
@@ -14,24 +15,23 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Documentation :: Sphinx
-Requires-Python: >=3.7
-Requires-Dist: importlib-metadata; python_version < '3.8'
+Classifier: Topic :: File Formats :: JSON :: JSON Schema
+Requires-Python: >=3.8
 Requires-Dist: lxml
 Requires-Dist: sphinx>=5.1.1
 Description-Content-Type: text/x-rst
 
 ===========================
 ``sphinx-json-schema-spec``
 ===========================
```

