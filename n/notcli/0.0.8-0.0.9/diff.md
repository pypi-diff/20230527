# Comparing `tmp/notcli-0.0.8.tar.gz` & `tmp/notcli-0.0.9.tar.gz`

## Comparing `notcli-0.0.8.tar` & `notcli-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,43 @@
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 notcli-0.0.8/CONTRIBUTING.md
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 notcli-0.0.8/Makefile
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 notcli-0.0.8/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 notcli-0.0.8/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.8/.ruff_cache/content/1d8fcaa1aec41a57
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.8/.ruff_cache/content/33ac437c97c9ba7f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.8/.ruff_cache/content/51d54a3651c5700d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.8/.ruff_cache/content/632db596ee57b83e
--rw-r--r--   0        0        0     7050 2020-02-02 00:00:00.000000 notcli-0.0.8/.ruff_cache/content/742a7a177a653eaf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.8/.ruff_cache/content/a3343eae45f839a8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.8/.ruff_cache/content/a4c0834c4e94528c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.8/.ruff_cache/content/b0da38d3f5b9c71a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.8/.ruff_cache/content/bb1b9bc214883b06
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.8/.ruff_cache/content/d00de8a95d9bf53e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.8/.ruff_cache/content/d25adf9bbda239ae
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.8/.ruff_cache/content/f4b54a9b80a16016
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 notcli-0.0.8/examples/env_file
--rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 notcli-0.0.8/scripts/format.sh
--rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 notcli-0.0.8/scripts/lint.sh
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 notcli-0.0.8/scripts/test.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 notcli-0.0.8/src/notcli/__init__.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 notcli-0.0.8/src/notcli/app.py
--rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 notcli-0.0.8/src/notcli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notcli-0.0.8/src/notcli/conf/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 notcli-0.0.8/src/notcli/conf/settings.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 notcli-0.0.8/src/notcli/static/demo.css
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 notcli-0.0.8/src/notcli/static/modal.css
--rwxr-xr-x   0        0        0    16504 2020-02-02 00:00:00.000000 notcli-0.0.8/src/tty/ttyecho
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 notcli-0.0.8/tests/test_version.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 notcli-0.0.8/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 notcli-0.0.8/LICENSE
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 notcli-0.0.8/README.md
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 notcli-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 notcli-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 notcli-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 notcli-0.0.9/Makefile
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 notcli-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 notcli-0.0.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/content/1d8fcaa1aec41a57
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/content/33ac437c97c9ba7f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/content/376b931934771011
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/content/51d54a3651c5700d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/content/5d3853d9662ff0cc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/content/632db596ee57b83e
+-rw-r--r--   0        0        0     7050 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/content/742a7a177a653eaf
+-rw-r--r--   0        0        0     7897 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/content/84d6e6d8dcc27855
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/content/a3343eae45f839a8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/content/a4c0834c4e94528c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/content/b0da38d3f5b9c71a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/content/bb1b9bc214883b06
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/content/d00de8a95d9bf53e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/content/d25adf9bbda239ae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/content/d94a6330b5766b62
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/content/f4b54a9b80a16016
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notcli-0.0.9/.ruff_cache/content/ff52395b860061a6
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 notcli-0.0.9/examples/env_file
+-rwxr-xr-x   0        0        0       96 2020-02-02 00:00:00.000000 notcli-0.0.9/scripts/format.sh
+-rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 notcli-0.0.9/scripts/lint.sh
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 notcli-0.0.9/scripts/test.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 notcli-0.0.9/src/notcli/__init__.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 notcli-0.0.9/src/notcli/app.py
+-rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 notcli-0.0.9/src/notcli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notcli-0.0.9/src/notcli/conf/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 notcli-0.0.9/src/notcli/conf/settings.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 notcli-0.0.9/src/notcli/static/demo.css
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 notcli-0.0.9/src/notcli/static/modal.css
+-rwxr-xr-x   0        0        0    16504 2020-02-02 00:00:00.000000 notcli-0.0.9/src/tty/ttyecho
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 notcli-0.0.9/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notcli-0.0.9/tests/test_apps/__init__.py
+-rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 notcli-0.0.9/tests/test_apps/test_load_vars.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 notcli-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 notcli-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 notcli-0.0.9/README.md
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 notcli-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 notcli-0.0.9/PKG-INFO
```

### Comparing `notcli-0.0.8/CONTRIBUTING.md` & `notcli-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `notcli-0.0.8/.ruff_cache/content/742a7a177a653eaf` & `notcli-0.0.9/.ruff_cache/content/742a7a177a653eaf`

 * *Files identical despite different names*

### Comparing `notcli-0.0.8/src/notcli/app.py` & `notcli-0.0.9/src/notcli/app.py`

 * *Files identical despite different names*

### Comparing `notcli-0.0.8/src/notcli/main.py` & `notcli-0.0.9/src/notcli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,28 +144,30 @@
     def build_command(commands):
         if not commands:
             raise ValueError("No commands to run")
         return ";".join(commands)
 
     def export_variables(self) -> None:
         self.add_note("Exporting variables to environment")
-        commands_to_run = []
-        for var, value in self.variables.items():
-            command = f"export {var}={value}"
-            commands_to_run.append(command)
-        self.add_note("Running commands")
-        try:
-            tty = self.get_tty()
-            command_str = self.build_command(commands_to_run) + "; clear"
-            sleep_and_run = (
-                f"sleep 0.3 && {TTY_ECHO_PATH}/ttyecho -n {tty} '{command_str}'"
-            )
-            subprocess.Popen(sleep_and_run, shell=True)
-        except Exception as e:
-            self.add_note(f"Failed to export variables: {str(e)}")
+        commands_to_run = [
+            f"export {var}={value}" for var, value in self.variables.items()
+        ]
+        if commands_to_run:
+            self.add_note("Running commands")
+            try:
+                tty = self.get_tty()
+                command_str = self.build_command(commands_to_run) + "; clear"
+                sleep_and_run = (
+                    f"sleep 0.3 && {TTY_ECHO_PATH}/ttyecho -n {tty} '{command_str}'"
+                )
+                subprocess.Popen(sleep_and_run, shell=True)
+            except Exception as e:
+                self.add_note(f"Failed to export variables: {str(e)}")
+            else:
+                self.app.exit()
         else:
-            self.app.exit()
+            subprocess.Popen("clear", shell=True)
 
 
 app = LoadVars()
 if __name__ == "__main__":
     app.run()
```

### Comparing `notcli-0.0.8/src/tty/ttyecho` & `notcli-0.0.9/src/tty/ttyecho`

 * *Files identical despite different names*

### Comparing `notcli-0.0.8/.gitignore` & `notcli-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `notcli-0.0.8/LICENSE` & `notcli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `notcli-0.0.8/README.md` & `notcli-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `notcli-0.0.8/PKG-INFO` & `notcli-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: notcli
-Version: 0.0.8
-Summary: A CLI application to load variables from a file and export them to the environment, with a Textual-based UI for interactive usage.
+Version: 0.0.9
+Summary: Textual User Interface (TUI) application designed to streamline your command line tasks with easy-to-use shortcuts
 Project-URL: Homepage, https://github.com/godd0t/notcli
 License: MIT
 License-File: LICENSE
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -19,14 +19,16 @@
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Requires-Dist: textual[dev]==0.26.0
 Provides-Extra: dev
 Requires-Dist: black==23.3.0; extra == 'dev'
 Requires-Dist: build==0.10.0; extra == 'dev'
 Requires-Dist: coverage[toml]==7.2.6; extra == 'dev'
+Requires-Dist: pytest-asyncio==0.21.0; extra == 'dev'
+Requires-Dist: pytest-sugar==0.9.7; extra == 'dev'
 Requires-Dist: pytest==7.3.1; extra == 'dev'
 Requires-Dist: ruff==0.0.270; extra == 'dev'
 Requires-Dist: twine==4.0.2; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # NotCLI - An Interactive TUI Application
```

