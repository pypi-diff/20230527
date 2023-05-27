# Comparing `tmp/setup2upypackage-0.1.1.tar.gz` & `tmp/setup2upypackage-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setup2upypackage-0.1.1.tar", last modified: Tue Apr 18 20:32:35 2023, max compression
+gzip compressed data, was "setup2upypackage-0.2.0.tar", last modified: Sat May 27 09:36:37 2023, max compression
```

## Comparing `setup2upypackage-0.1.1.tar` & `setup2upypackage-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:32:35.754973 setup2upypackage-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-18 20:32:19.000000 setup2upypackage-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-18 20:32:35.754973 setup2upypackage-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-04-18 20:32:19.000000 setup2upypackage-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-18 20:32:19.000000 setup2upypackage-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-18 20:32:35.758973 setup2upypackage-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-18 20:32:19.000000 setup2upypackage-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:32:35.750972 setup2upypackage-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:32:35.754973 setup2upypackage-0.1.1/src/setup2upypackage/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-18 20:32:19.000000 setup2upypackage-0.1.1/src/setup2upypackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-04-18 20:32:19.000000 setup2upypackage-0.1.1/src/setup2upypackage/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-04-18 20:32:19.000000 setup2upypackage-0.1.1/src/setup2upypackage/setup2upypackage.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-18 20:32:29.000000 setup2upypackage-0.1.1/src/setup2upypackage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:32:35.754973 setup2upypackage-0.1.1/src/setup2upypackage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-18 20:32:35.000000 setup2upypackage-0.1.1/src/setup2upypackage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-18 20:32:35.000000 setup2upypackage-0.1.1/src/setup2upypackage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:32:35.000000 setup2upypackage-0.1.1/src/setup2upypackage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-18 20:32:35.000000 setup2upypackage-0.1.1/src/setup2upypackage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-18 20:32:35.000000 setup2upypackage-0.1.1/src/setup2upypackage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 20:32:35.000000 setup2upypackage-0.1.1/src/setup2upypackage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:32:35.754973 setup2upypackage-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-18 20:32:19.000000 setup2upypackage-0.1.1/tests/test_absolute_truth.py
--rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-04-18 20:32:19.000000 setup2upypackage-0.1.1/tests/test_setup2upypackage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:36:37.583165 setup2upypackage-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-27 09:36:18.000000 setup2upypackage-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-05-27 09:36:37.583165 setup2upypackage-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-05-27 09:36:18.000000 setup2upypackage-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-27 09:36:18.000000 setup2upypackage-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-27 09:36:37.583165 setup2upypackage-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-05-27 09:36:18.000000 setup2upypackage-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:36:37.579165 setup2upypackage-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:36:37.583165 setup2upypackage-0.2.0/src/setup2upypackage/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-27 09:36:18.000000 setup2upypackage-0.2.0/src/setup2upypackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-05-27 09:36:18.000000 setup2upypackage-0.2.0/src/setup2upypackage/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-05-27 09:36:18.000000 setup2upypackage-0.2.0/src/setup2upypackage/setup2upypackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-27 09:36:29.000000 setup2upypackage-0.2.0/src/setup2upypackage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:36:37.583165 setup2upypackage-0.2.0/src/setup2upypackage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-05-27 09:36:37.000000 setup2upypackage-0.2.0/src/setup2upypackage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-27 09:36:37.000000 setup2upypackage-0.2.0/src/setup2upypackage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 09:36:37.000000 setup2upypackage-0.2.0/src/setup2upypackage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-27 09:36:37.000000 setup2upypackage-0.2.0/src/setup2upypackage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-27 09:36:37.000000 setup2upypackage-0.2.0/src/setup2upypackage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-27 09:36:37.000000 setup2upypackage-0.2.0/src/setup2upypackage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:36:37.583165 setup2upypackage-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-27 09:36:18.000000 setup2upypackage-0.2.0/tests/test_absolute_truth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13763 2023-05-27 09:36:18.000000 setup2upypackage-0.2.0/tests/test_setup2upypackage.py
```

### Comparing `setup2upypackage-0.1.1/LICENSE.txt` & `setup2upypackage-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.1.1/PKG-INFO` & `setup2upypackage-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setup2upypackage
-Version: 0.1.1
+Version: 0.2.0
 Summary: Validate and create MicroPython package JSON file
 Home-page: https://github.com/brainelectronics/micropython-package-validation
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-package-validation/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-package-validation/
 Keywords: micropython,package,mip-helper,validation
@@ -99,15 +99,15 @@
 The following command will exit with a non-zero code in case of a difference
 between the generated (based on `setup.py`) and existing package
 (`package.json`) content.
 
 ```bash
 upy-package \
     --setup_file tests/data/setup.py \
-    --package_changelog_file tests/data/changelog.md \
+    --package_changelog_file tests/data/sample_changelog.md \
     --package_file tests/data/package.json \
     --validate
 ```
 
 #### Validate package JSON file from changelog
 
 In case the package version is defined by a changelog and the `version` entry
```

### Comparing `setup2upypackage-0.1.1/README.md` & `setup2upypackage-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 The following command will exit with a non-zero code in case of a difference
 between the generated (based on `setup.py`) and existing package
 (`package.json`) content.
 
 ```bash
 upy-package \
     --setup_file tests/data/setup.py \
-    --package_changelog_file tests/data/changelog.md \
+    --package_changelog_file tests/data/sample_changelog.md \
     --package_file tests/data/package.json \
     --validate
 ```
 
 #### Validate package JSON file from changelog
 
 In case the package version is defined by a changelog and the `version` entry
```

### Comparing `setup2upypackage-0.1.1/setup.py` & `setup2upypackage-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.1.1/src/setup2upypackage/main.py` & `setup2upypackage-0.2.0/src/setup2upypackage/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,14 +93,20 @@
 
     parser.add_argument('--validate',
                         dest='do_validate',
                         action='store_true',
                         required=False,
                         help='Validate existing package.json with setup.py based data')  # noqa: E501
 
+    parser.add_argument('--ignore-version',
+                        dest='ignore_version',
+                        action='store_true',
+                        required=False,
+                        help='Exclude version value from check ')
+
     parser.add_argument('--print',
                         dest='print_result',
                         required=False,
                         action='store_true',
                         help='Print parsed setup.py as JSON to stdout')
 
     parser.add_argument('--pretty',
@@ -137,25 +143,26 @@
     setup_file = args.setup_file
     package_file = args.package_file
     package_changelog_file = args.package_changelog_file
     do_validate = args.do_validate
     dump_to_file = args.dump_to_file
     print_result = args.print_result
     pretty_output = args.pretty_output
+    ignore_version = args.ignore_version
 
     setup_2_upy_package = Setup2uPyPackage(
         setup_file=setup_file,
         package_file=package_file,
         package_changelog_file=package_changelog_file,
         logger=logger)
 
     package_data = setup_2_upy_package.package_data
 
     if do_validate:
-        if not setup_2_upy_package.validate():
+        if not setup_2_upy_package.validate(ignore_version=ignore_version):
             diff = setup_2_upy_package.validation_diff
 
             if pretty_output:
                 stdout.write(json.dumps(diff, indent=4))
             else:
                 stdout.write(json.dumps(diff))
             raise SystemExit('Mismatch between setup.py data and package.json')
```

### Comparing `setup2upypackage-0.1.1/src/setup2upypackage/setup2upypackage.py` & `setup2upypackage-0.2.0/src/setup2upypackage/setup2upypackage.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,25 +302,32 @@
             with open(self._package_file, 'r') as f:
                 existing_data = json.load(f)
         else:
             raise Setup2uPyPackageError("No package.json data specified")
 
         return existing_data
 
-    def validate(self) -> bool:
+    def validate(self, ignore_version: bool = False) -> bool:
         """
         Validate existing package.json with setup.py based data
 
+        :param      ignore_version:  Indicates if the version is ignored
+        :type       ignore_version:  bool
+
         :returns:   Result of validation, True on success, False otherwise
         :rtype:     bool
         """
         # list of URL entries might be sorted differently
         package_json_data = dict(self.package_json_data)
         package_data = dict(self.package_data)
 
+        if ignore_version:
+            package_json_data.pop("version")
+            package_data.pop("version")
+
         package_json_data.get("urls", []).sort()
         package_data.get("urls", []).sort()
 
         return package_json_data == package_data
 
     @property
     def validation_diff(self) -> DeepDiff:
```

### Comparing `setup2upypackage-0.1.1/src/setup2upypackage.egg-info/PKG-INFO` & `setup2upypackage-0.2.0/src/setup2upypackage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setup2upypackage
-Version: 0.1.1
+Version: 0.2.0
 Summary: Validate and create MicroPython package JSON file
 Home-page: https://github.com/brainelectronics/micropython-package-validation
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-package-validation/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-package-validation/
 Keywords: micropython,package,mip-helper,validation
@@ -99,15 +99,15 @@
 The following command will exit with a non-zero code in case of a difference
 between the generated (based on `setup.py`) and existing package
 (`package.json`) content.
 
 ```bash
 upy-package \
     --setup_file tests/data/setup.py \
-    --package_changelog_file tests/data/changelog.md \
+    --package_changelog_file tests/data/sample_changelog.md \
     --package_file tests/data/package.json \
     --validate
 ```
 
 #### Validate package JSON file from changelog
 
 In case the package version is defined by a changelog and the `version` entry
```

### Comparing `setup2upypackage-0.1.1/src/setup2upypackage.egg-info/SOURCES.txt` & `setup2upypackage-0.2.0/src/setup2upypackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.1.1/tests/test_absolute_truth.py` & `setup2upypackage-0.2.0/tests/test_absolute_truth.py`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.1.1/tests/test_setup2upypackage.py` & `setup2upypackage-0.2.0/tests/test_setup2upypackage.py`

 * *Files 6% similar despite different names*

```diff
@@ -318,14 +318,29 @@
             patched.return_value = shuffeled_package_json_data
             is_valid = s2pp.validate()
             if is_valid:
                 self.assertTrue(is_valid)
             else:
                 self.test_logger.warning(s2pp.validation_diff)
 
+        # check for different version entries
+        diff_version_package_json_data = dict(s2pp.package_json_data)
+        diff_version_package_json_data["version"] = "93.10.22"
+        self.assertNotEqual(
+            diff_version_package_json_data["version"],
+            s2pp.package_json_data
+        )
+        with patch('setup2upypackage.setup2upypackage.Setup2uPyPackage.package_json_data', new_callable=PropertyMock) as patched:     # noqa: E501
+            patched.return_value = diff_version_package_json_data
+            is_valid = s2pp.validate(ignore_version=True)
+            if is_valid:
+                self.assertTrue(is_valid)
+            else:
+                self.test_logger.warning(s2pp.validation_diff)
+
     @unittest.skip("Not yet implemented")
     def test_validation_diff(self) -> None:
         """Test validation difference property"""
         pass
 
     @params(
         ("asdf.json", False),   # path, pretty
```

