# Comparing `tmp/crackerjack-0.1.9.tar.gz` & `tmp/crackerjack-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.1.9.tar", last modified: Tue May  2 08:30:38 2023, max compression
+gzip compressed data, was "crackerjack-0.2.0.tar", last modified: Sat May 27 13:06:06 2023, max compression
```

## Comparing `crackerjack-0.1.9.tar` & `crackerjack-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.1.9/LICENSE
--rw-r--r--   0        0        0     2856 2023-04-26 12:28:28.914334 crackerjack-0.1.9/README.md
--rw-r--r--   0        0        0        0 2023-05-02 08:30:21.144672 crackerjack-0.1.9/crackerjack/.crackerjack-config.yaml
--rw-r--r--   0        0        0      197 2023-05-02 08:30:21.083979 crackerjack-0.1.9/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-05-02 08:30:21.125590 crackerjack-0.1.9/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     2055 2023-05-02 08:30:36.204284 crackerjack-0.1.9/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.1.9/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.1.9/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.1.9/crackerjack/__init__.py
--rw-r--r--   0        0        0     1099 2023-05-01 23:08:32.884408 crackerjack-0.1.9/crackerjack/__main__.py
--rw-r--r--   0        0        0     4968 2023-05-02 08:30:36.204493 crackerjack-0.1.9/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     1690 2023-05-02 08:30:36.204656 crackerjack-0.1.9/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     5606 2023-04-25 20:30:39.178113 crackerjack-0.1.9/crackerjack/test1.py
--rw-r--r--   0        0        0     1687 2023-05-02 08:30:38.171002 crackerjack-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3860 1970-01-01 00:00:00.000000 crackerjack-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3142 2023-05-26 14:01:21.577314 crackerjack-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 13:05:35.403736 crackerjack-0.2.0/crackerjack/.crackerjack-config.yaml
+-rw-r--r--   0        0        0      163 2023-05-27 13:05:35.393891 crackerjack-0.2.0/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-05-27 13:05:35.401181 crackerjack-0.2.0/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     2055 2023-05-27 13:05:35.398223 crackerjack-0.2.0/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.2.0/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.2.0/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.2.0/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1238 2023-05-27 10:07:36.046052 crackerjack-0.2.0/crackerjack/__main__.py
+-rw-r--r--   0        0        0     5548 2023-05-27 13:01:29.970006 crackerjack-0.2.0/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     1603 2023-05-27 13:05:36.137385 crackerjack-0.2.0/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     1722 2023-05-27 13:06:06.916928 crackerjack-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4146 1970-01-01 00:00:00.000000 crackerjack-0.2.0/PKG-INFO
```

### Comparing `crackerjack-0.1.9/LICENSE` & `crackerjack-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.1.9/README.md` & `crackerjack-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 
 [![Python: 3.7](https://img.shields.io/badge/python-3.11%2B-blue)](https://docs.python.org/3/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Code style: crackerjack](https://img.shields.io/badge/code%20style-crackerjack-000042)](https://github.com/lesleslie/crackerjack)
 
 Crackerjack is a python coding style which uses a minimalist approach to produce elegant, easy to read, code.
 
+crack·​er·​jack ˈkra-kər-ˌjak
+: a person or thing of marked excellence
+
 ### **Why Crackerjack?**
 
-Crackerjack works on the theory that with static typing and explicit classes,
-functions, variables, and other object names - the code should be
+Crackerjack works on the theory that with static typing and explicit class,
+function, variable, and other object names - the code should be
 straight forward to read and the documentation should pretty much be able to write
 itself. Crackerjack provides a set of guidelines and utilities to keep the codebase clean, elegant, standardized, and
 easily readable.
 
 ### **What does this package do?**
 
 This package:
@@ -26,23 +29,25 @@
 
 - does import sorting, linting, and complexity analysis with ruff
 
 - uses mypy for type checking
 
 - streamlines code with refurb
 
-- converts/creates documentation in Markdown (md)
-
-- installs, or updates, a projects pre-commit tools and gitignore
+- installs, or updates, a project's pre-commit tools and gitignore
   to comply with evolving crackerjack standards
 
 - removes pipenv, poetry, and hatch build, dependency management, and virtual environment
-  management packages and replace them with PDM using PEP 582
+  management packages and replaces them with PDM using PEP 582
+
+- converts/creates documentation in Markdown (md) - Coming Soon!
 
-- generates pytest mock stubs if needed
+- runs tests and generates pytest mock stubs if needed - Coming Soon!
+
+- bumps the project version and publishes it to PyPI
 
 ### **What are the rules?**
 
 (...more what you'd call "guidelines" than actual rules. -Captain Barbossa )
 
 - all docstrings, README's, and other documentation is to be done in Markdown (md)
 
@@ -81,13 +86,23 @@
 
 From your projects root directory:
 
 ```python -m crackerjack```
 
 Cracker jack will take care of the rest.
 
+For a full list of options:
+
+```python -m crackerjack -h```
+
 When you ready to publish your project:
 
 ``python -m crackerjack -p micro``
 
 The -p option not only publishes your project but will bump your
 project version for you. The options are 'micro', 'minor', and 'major'.
+
+## Acknowledgements
+
+## License
+
+BSD-3-Clause
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crackerjack-0.1.9/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.2.0/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.1.9/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.2.0/crackerjack/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         name: check-added-large-files
   - repo: https://github.com/psf/black
     rev: '23.3.0'
     hooks:
       - id: black
         language_version: python3.11
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.264
+    rev: v0.0.270
     hooks:
       - id: ruff
   - repo: https://github.com/fredrikaverpil/creosote
     rev: v2.6.1
     hooks:
       - id: creosote
         args:
@@ -46,29 +46,29 @@
         types_or: [ python, pyi ]
         language: python
         files: \.py$
         additional_dependencies:
           - autotyping==23.3.0
           - libcst==0.4.9
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.3.0
     hooks:
       - id: mypy
   #  - repo: https://github.com/pdoc3/pdoc
   #    rev: master
   #    hooks:
   #      - id: pdoc
   #        name: pdoc
   #        entry: pdoc --html -f -o docs module1 module2 module3
   #        language_version: python3.11
   #        require_serial: true
   #        types: [ python ]
   #        always_run: true
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.264
+    rev: v0.0.270
     hooks:
       - id: ruff
   - repo: https://github.com/psf/black
     rev: '23.3.0'
     hooks:
       - id: black
         language_version: python3.11
```

### Comparing `crackerjack-0.1.9/crackerjack/__main__.py` & `crackerjack-0.2.0/crackerjack/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,49 @@
 import asyncio
 
-from addict import Dict
 from click import command
 from click import help_option
 from click import option
 from crackerjack import crackerjack_it
+from pydantic import BaseModel
+
+
+class Options(BaseModel):
+    commit = False
+    interactive = False
+    doc = False
+    do_not_update_configs = False
+    publish: str | bool = False
+    verbose = False
+
+
+options = Options()
 
 
 @command()
 @help_option("-h", is_flag=True, help="help")
 @option("-c", is_flag=True, help="commit")
 @option("-i", is_flag=True, help="interactive")
 @option("-d", is_flag=True, help="doc")
 @option("-x", is_flag=True, help="do not update configs")
 @option("-v", is_flag=True, help="verbose")
 @option("-p", help="publish: -p [micro, minor, major]")
 # @option("-f", help="format: -f [module]")
 def crackerjack(c: bool, i: bool, d: bool, v: bool, x: bool, p: str) -> None:
-    options: Dict[str, str | bool] = Dict()
     if c:
-        options["commit"] = c
+        options.commit = c
     if i:
-        options["interactive"] = i
+        options.interactive = i
     if d:
-        options["doc"] = d
+        options.doc = d
     if x:
-        options["do_not_update_configs"] = x
+        options.do_not_update_configs = x
     if p in ("micro", "minor", "major"):
-        options["publish"] = p
+        options.publish = p
     if v:
-        print("-v not currently implemented.")
-        options["verbose"] = v
+        print("-v not currently implemented")
+        options.verbose = v
     asyncio.run(crackerjack_it(options))
 
 
 if __name__ == "__main__":
     crackerjack()
```

### Comparing `crackerjack-0.1.9/crackerjack/crackerjack.py` & `crackerjack-0.2.0/crackerjack/crackerjack.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 from subprocess import check_output
 from subprocess import run
 
 import pdm_bump
 import pdoc
 from acb.actions import dump
 from acb.actions import load
-from addict import Dict
+
+# from addict import Dict
 from aioconsole import ainput
 from aiopath import AsyncPath
 from inflection import underscore
+from inflection import camelize
 from pydantic import BaseModel
+from pydantic import create_model
+from pydantic import Extra
 
 for mod in (pdm_bump, pdoc):  # look ruff / isort to get rid of this
     pass
 
 
 # Crackerjack
 
@@ -28,23 +32,36 @@
     pkg_name: str = "crackerjack"
     our_toml: t.Optional[dict] = None
     pkg_toml: t.Optional[dict] = None
     our_toml_path: t.Optional[AsyncPath] = None
     pkg_toml_path: t.Optional[AsyncPath] = None
     poetry_pip_env: bool = False
 
+    async def get_toml_config(self, path: AsyncPath):
+        class Config(BaseModel.Config):  # type: ignore
+            extra = Extra.allow
+
+        return create_model(
+            camelize(path.stem),
+            __config__=Config,
+            **(await load.toml(path)),
+        )()
+
     async def update_pyproject_configs(self) -> None:
-        our_toml_config = await load.toml(self.our_toml_path)
-        pkg_toml_config = await load.toml(self.pkg_toml_path)
+        our_toml_config = await self.get_toml_config(self.our_toml_path)
+        pkg_toml_config = await self.get_toml_config(self.pkg_toml_path)
         if self.poetry_pip_env:
             del pkg_toml_config.tool.poetry
         old_deps = pkg_toml_config.tool.pdm["dev-dependencies"]
         pkg_toml_config.tool = our_toml_config.tool
         pkg_toml_config.tool.pdm["dev-dependencies"] = old_deps
-        await dump.toml(pkg_toml_config, self.pkg_toml_path)
+        if self.pkg_path.stem == "crackerjack":
+            await dump.toml(pkg_toml_config.dict(), self.our_toml_path)
+        else:
+            await dump.toml(pkg_toml_config.dict(), self.pkg_toml_path)
 
     async def clean_poetry_pip_env(self) -> None:
         root_files = [
             file
             async for file in self.pkg_path.iterdir()
             if ("poetry" or "Pip") in file.name
         ]
@@ -59,29 +76,28 @@
             ".pre-commit-config.yaml",
             ".libcst.codemod.yaml",
             ".crackerjack-config.yaml",
         ):
             config_path = self.our_path.parent / config
             pkg_config_path = self.pkg_path / config
             await pkg_config_path.touch(exist_ok=True)
-            run(["git", "add", str(pkg_config_path)])
             if self.pkg_path.stem == "crackerjack":
                 await config_path.write_text(await pkg_config_path.read_text())
             # if poetry_pip_env:
             #     await config_pkg_path.unlink()
             config_text = await config_path.read_text()
             await pkg_config_path.write_text(
                 config_text.replace("crackerjack", self.pkg_name)
             )
 
     @staticmethod
     async def run_interactive(hook: str) -> None:
         success = False
         while not success:
-            fail = call(["pre-commit", "run", hook.lower()])
+            fail = call(["pre-commit", "run", hook.lower(), "--all-files"])
             if fail > 0:
                 retry = await ainput(f"\n{hook} failed. Retry? (y/n): ")
                 if retry.lower() == "y":
                     continue
                 sys.exit()
             success = True
 
@@ -89,48 +105,47 @@
         await self.clean_poetry_pip_env()
         await self.copy_configs()
         toml_file = "pyproject.toml"
         self.our_toml_path = self.our_path.parent / toml_file
         self.pkg_toml_path = self.pkg_path / toml_file
         if not await self.pkg_toml_path.exists():
             run(["pdm", "init"])
+            run(["pdm", "self", "add", "keyring"])
             run(["git", "add", "pyproject.toml"])
-            # run(["git", "add", "pdm.lock"])
         installed_pkgs = check_output(
             ["pdm", "list", "--freeze"],
             universal_newlines=True,
         ).splitlines()
         if not len([pkg for pkg in installed_pkgs if "pre-commit" in pkg]):
             run(["pdm", "add", "-d", "pre_commit"])
             run(["pre-commit", "install"])
             run(["git", "add", "pdm.lock"])
         await self.update_pyproject_configs()
 
-    async def process(
-        self,
-        options: Dict[str, str | bool],
-    ) -> None:
+    async def process(self, options: t.Any) -> None:
         imp_dir = self.pkg_path / "__pypackages__"
         sys.path.append(str(imp_dir))
         self.pkg_name = underscore(self.pkg_path.stem.lower())
         self.pkg_dir = self.pkg_path / self.pkg_name
         await self.pkg_dir.mkdir(exist_ok=True)
         print("\nCrackerjacking...\n")
         if self.pkg_path.stem == "crackerjack":
+            run(["git", "add", ".pre-commit-config.yaml"])
             run(["pre-commit", "autoupdate"])
+        if options.publish:
+            check_output(["pdm", "bump", options.publish])
         if not options.do_not_update_configs:
             await self.update_pkg_configs()
         if options.interactive:
             for hook in ("refurb", "mypy"):
                 await self.run_interactive(hook)
-        check_all = call(["pre-commit", "run"])
+        check_all = call(["pre-commit", "run", "--all-files"])
         if check_all > 0:
             call(["pre-commit", "run", "--all-files"])
         if options.publish:
-            check_output(["pdm", "bump", options.publish])
             run(["pdm", "publish"])
         if options.commit:
             commit_msg = input("Commit message: ")
             call(["git", "commit", "-m", f"'{commit_msg}'", "--", "."])
             call(["git", "push", "origin", "main"])
```

### Comparing `crackerjack-0.1.9/crackerjack/pyproject.toml` & `crackerjack-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -26,29 +26,29 @@
     "py311",
 ]
 
 [tool.mypy]
 strict = false
 pretty = true
 ignore_missing_imports = false
-
+plugins = [
+    "pydantic.mypy",
+]
 
 [tool.refurb]
 enable_all = true
 
-
-
 [tool.pytype]
 inputs = [
     "package_name",
 ]
 
 [project]
 name = "Crackerjack"
-version = "0.1.6"
+version = "0.2.0"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
```

### Comparing `crackerjack-0.1.9/pyproject.toml` & `crackerjack-0.2.0/crackerjack/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,10 @@
+[tool]
 [tool.pdm.dev-dependencies]
-dev = [
-    "pytest>=7.3.0",
-    "icecream>=2.1.3",
-    "pre-commit>=3.2.2",
-]
+dev = ["pytest>=7.3.0", "icecream>=2.1.3", "pre-commit>=3.2.2"]
 
 [tool.ruff]
 line-length = 88
 target-version = "py311"
 fix = true
 show-fixes = true
 show-source = true
@@ -18,66 +15,45 @@
 [tool.ruff.mccabe]
 max-complexity = 10
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.black]
-target-version = [
-    "py311",
-]
+target-version = ["py311"]
 
 [tool.mypy]
 strict = false
 pretty = true
 ignore_missing_imports = false
+plugins = ["pydantic.mypy"]
 
 [tool.refurb]
 enable_all = true
 
 [tool.pytype]
-inputs = [
-    "package_name",
-]
+inputs = ["package_name"]
 
 [project]
 name = "Crackerjack"
-version = "0.1.9"
+version = "0.2.0"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
-keywords = [
-    "black",
-    "ruff",
-    "mypy",
-    "creosote",
-    "refurb",
-]
-classifiers = [
-    "Environment :: Console",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3.11",
-]
-dependencies = [
-    "click>=8.1.3",
-    "pdoc3>=0.10.0",
-    "pdm-bump>=0.7.0",
-    "pydantic>=1.10.7",
-    "aiopath>=0.6.11",
-    "acb>=0.1.2",
-    "aioconsole>=0.6.1",
-    "inflection>=0.5.1",
-]
-authors = [
-    { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
-]
-maintainers = [
-    { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
-]
+keywords = ["black", "ruff", "mypy", "creosote", "refurb"]
+classifiers = ["Environment :: Console", "Operating System :: OS Independent", "Programming Language :: Python", "Programming Language :: Python :: 3.11"]
+dependencies = ["click>=8.1.3", "pdoc3>=0.10.0", "pdm-bump>=0.7.0", "pydantic>=1.10.7", "aiopath>=0.6.11", "acb>=0.1.2", "aioconsole>=0.6.1", "inflection>=0.5.1"]
+
+[[project.authors]]
+name = "lesleslie"
+email = "les@wedgwoodwebworks.com"
+
+[[project.maintainers]]
+name = "lesleslie"
+email = "les@wedgwoodwebworks.com"
 
 [project.license]
 text = "BSD-3-Clause"
 
 [project.optional-dependencies]
 
 [project.urls]
@@ -86,11 +62,9 @@
 repository = "https://github.com/lesleslie/crackerjack"
 
 [project.scripts]
 
 [project.entry-points]
 
 [build-system]
-requires = [
-    "pdm-backend",
-]
+requires = ["pdm-backend"]
 build-backend = "pdm.backend"
```

### Comparing `crackerjack-0.1.9/PKG-INFO` & `crackerjack-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crackerjack
-Version: 0.1.9
+Version: 0.2.0
 Summary: Crackerjack code formatting style.
 Keywords: black ruff mypy creosote refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
@@ -29,18 +29,21 @@
 
 [![Python: 3.7](https://img.shields.io/badge/python-3.11%2B-blue)](https://docs.python.org/3/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Code style: crackerjack](https://img.shields.io/badge/code%20style-crackerjack-000042)](https://github.com/lesleslie/crackerjack)
 
 Crackerjack is a python coding style which uses a minimalist approach to produce elegant, easy to read, code.
 
+crack·​er·​jack ˈkra-kər-ˌjak
+: a person or thing of marked excellence
+
 ### **Why Crackerjack?**
 
-Crackerjack works on the theory that with static typing and explicit classes,
-functions, variables, and other object names - the code should be
+Crackerjack works on the theory that with static typing and explicit class,
+function, variable, and other object names - the code should be
 straight forward to read and the documentation should pretty much be able to write
 itself. Crackerjack provides a set of guidelines and utilities to keep the codebase clean, elegant, standardized, and
 easily readable.
 
 ### **What does this package do?**
 
 This package:
@@ -53,23 +56,25 @@
 
 - does import sorting, linting, and complexity analysis with ruff
 
 - uses mypy for type checking
 
 - streamlines code with refurb
 
-- converts/creates documentation in Markdown (md)
-
-- installs, or updates, a projects pre-commit tools and gitignore
+- installs, or updates, a project's pre-commit tools and gitignore
   to comply with evolving crackerjack standards
 
 - removes pipenv, poetry, and hatch build, dependency management, and virtual environment
-  management packages and replace them with PDM using PEP 582
+  management packages and replaces them with PDM using PEP 582
+
+- converts/creates documentation in Markdown (md) - Coming Soon!
 
-- generates pytest mock stubs if needed
+- runs tests and generates pytest mock stubs if needed - Coming Soon!
+
+- bumps the project version and publishes it to PyPI
 
 ### **What are the rules?**
 
 (...more what you'd call "guidelines" than actual rules. -Captain Barbossa )
 
 - all docstrings, README's, and other documentation is to be done in Markdown (md)
 
@@ -108,13 +113,23 @@
 
 From your projects root directory:
 
 ```python -m crackerjack```
 
 Cracker jack will take care of the rest.
 
+For a full list of options:
+
+```python -m crackerjack -h```
+
 When you ready to publish your project:
 
 ``python -m crackerjack -p micro``
 
 The -p option not only publishes your project but will bump your
 project version for you. The options are 'micro', 'minor', and 'major'.
+
+## Acknowledgements
+
+## License
+
+BSD-3-Clause
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

