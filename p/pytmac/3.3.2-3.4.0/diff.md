# Comparing `tmp/pytmac-3.3.2.tar.gz` & `tmp/pytmac-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytmac-3.3.2.tar", last modified: Thu May 25 20:04:52 2023, max compression
+gzip compressed data, was "pytmac-3.4.0.tar", last modified: Sat May 27 09:26:52 2023, max compression
```

## Comparing `pytmac-3.3.2.tar` & `pytmac-3.4.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:04:52.015907 pytmac-3.3.2/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-05-25 20:04:48.000000 pytmac-3.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7413 2023-05-25 20:04:52.015907 pytmac-3.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7300 2023-05-25 20:04:48.000000 pytmac-3.3.2/README.md
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-25 20:04:49.000000 pytmac-3.3.2/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:04:52.011907 pytmac-3.3.2/bin/
--rw-r--r--   0 root         (0) root         (0)     5175 2023-05-25 20:04:48.000000 pytmac-3.3.2/bin/get_config.py
--rw-r--r--   0 root         (0) root         (0)     6326 2023-05-25 20:04:48.000000 pytmac-3.3.2/bin/input_validator.py
--rw-r--r--   0 root         (0) root         (0)     2823 2023-05-25 20:04:48.000000 pytmac-3.3.2/bin/resource_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:04:52.011907 pytmac-3.3.2/docs/
--rw-r--r--   0 root         (0) root         (0)      241 2023-05-25 20:04:48.000000 pytmac-3.3.2/docs/config.yaml
--rw-r--r--   0 root         (0) root         (0)     2089 2023-05-25 20:04:48.000000 pytmac-3.3.2/docs/defaults.yaml
--rw-r--r--   0 root         (0) root         (0)     1075 2023-05-25 20:04:48.000000 pytmac-3.3.2/docs/resources.yaml
--rw-r--r--   0 root         (0) root         (0)     7555 2023-05-25 20:04:48.000000 pytmac-3.3.2/docs/security_checks.yaml
--rw-r--r--   0 root         (0) root         (0)     1474 2023-05-25 20:04:48.000000 pytmac-3.3.2/docs/swagger.json
--rw-r--r--   0 root         (0) root         (0)      242 2023-05-25 20:04:48.000000 pytmac-3.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)    21594 2023-05-25 20:04:51.000000 pytmac-3.3.2/pytmac
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 20:04:52.015907 pytmac-3.3.2/pytmac.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7413 2023-05-25 20:04:51.000000 pytmac-3.3.2/pytmac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      376 2023-05-25 20:04:52.000000 pytmac-3.3.2/pytmac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 20:04:51.000000 pytmac-3.3.2/pytmac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-25 20:04:51.000000 pytmac-3.3.2/pytmac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-25 20:04:51.000000 pytmac-3.3.2/pytmac.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 20:04:52.015907 pytmac-3.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      868 2023-05-25 20:04:48.000000 pytmac-3.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 09:26:52.337334 pytmac-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-05-27 09:26:49.000000 pytmac-3.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7054 2023-05-27 09:26:52.337334 pytmac-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6941 2023-05-27 09:26:49.000000 pytmac-3.4.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-27 09:26:50.000000 pytmac-3.4.0/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 09:26:52.337334 pytmac-3.4.0/bin/
+-rw-r--r--   0 root         (0) root         (0)     5175 2023-05-27 09:26:49.000000 pytmac-3.4.0/bin/get_config.py
+-rw-r--r--   0 root         (0) root         (0)    12122 2023-05-27 09:26:49.000000 pytmac-3.4.0/bin/init.py
+-rw-r--r--   0 root         (0) root         (0)     6326 2023-05-27 09:26:49.000000 pytmac-3.4.0/bin/input_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2823 2023-05-27 09:26:49.000000 pytmac-3.4.0/bin/resource_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 09:26:52.337334 pytmac-3.4.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-05-27 09:26:49.000000 pytmac-3.4.0/docs/config.yaml
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-05-27 09:26:49.000000 pytmac-3.4.0/docs/defaults.yaml
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-27 09:26:49.000000 pytmac-3.4.0/docs/resources.yaml
+-rw-r--r--   0 root         (0) root         (0)     7555 2023-05-27 09:26:49.000000 pytmac-3.4.0/docs/security_checks.yaml
+-rw-r--r--   0 root         (0) root         (0)     1474 2023-05-27 09:26:49.000000 pytmac-3.4.0/docs/swagger.json
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-27 09:26:49.000000 pytmac-3.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)    25738 2023-05-27 09:26:52.000000 pytmac-3.4.0/pytmac
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 09:26:52.337334 pytmac-3.4.0/pytmac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7054 2023-05-27 09:26:52.000000 pytmac-3.4.0/pytmac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      388 2023-05-27 09:26:52.000000 pytmac-3.4.0/pytmac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-27 09:26:52.000000 pytmac-3.4.0/pytmac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-27 09:26:52.000000 pytmac-3.4.0/pytmac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-27 09:26:52.000000 pytmac-3.4.0/pytmac.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-27 09:26:52.337334 pytmac-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      868 2023-05-27 09:26:49.000000 pytmac-3.4.0/setup.py
```

### Comparing `pytmac-3.3.2/LICENSE` & `pytmac-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytmac-3.3.2/PKG-INFO` & `pytmac-3.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmac
-Version: 3.3.2
+Version: 3.4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git?ref=badge_shield)
 ![Workflow Actionlint](https://github.com/tjtharrison/pytmac/actions/workflows/pr-actionlint.yaml/badge.svg)
 ![Workflow Checkov](https://github.com/tjtharrison/pytmac/actions/workflows/pr-checkov.yaml/badge.svg)
 ![Workflow Linting](https://github.com/tjtharrison/pytmac/actions/workflows/pr-linting.yaml/badge.svg)
@@ -32,45 +32,38 @@
 
 # Usage
 
 Once installed, pytmac can be called from the command line with an array of arguments which are described in the help page:
 
 ```
 pytmac --help
-
-options:
-  -h, --help            show this help message and exit
-  --version             Option to print the current version only
-  --demo                Run pytmac in demo mode using the demo config and resources
-  --output-dir OUTPUT_DIR
-                        [Default: reports] Set the directory for report output
-  --resources-file RESOURCES_FILE
-                        The path to the resources file
-  --config-file CONFIG_FILE
-                        The path to the config file
-  --defaults-file DEFAULTS_FILE
-                        The path to the defaults file
-  --security-checks-file SECURITY_CHECKS_FILE
-                        [Default: security_checks.yaml] The path to the security-checks file
-  --swagger-file SWAGGER_FILE
-                        [Default: None] The path to the swagger file (optional)
 ```
 
 ## Demonstration
 
 To generate an example report based on some pre-defined resources, run the following command:
 
 ```
 pytmac --demo
 ```
 
 This will write to a file called `report-[today-date].md` which can be viewed in a markdown viewer.
 
 # Configuration
 
+## Init mode
+
+pytmac can be run in init mode to generate configuration files using a combination of inputs provided and default project settings. This can be done with the following command:
+
+```bash
+pytmac --init
+```
+
+Once the initialisation has completed, you should review the generated files and make any changes required (Primary focus should be on the defaults file as this will globally define security settings for all generated resources in your project.
+
 ## Config file
 
 pytmac on launch will look for a file in the current directory named `.pytmac` as a source of settings. This file can be used to set the following settings:
 
 ```
 resource_file: "docs/resources.yaml"
 config_file: "docs/config.yaml"
```

### Comparing `pytmac-3.3.2/README.md` & `pytmac-3.4.0/pytmac.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: pytmac
+Version: 3.4.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git?ref=badge_shield)
 ![Workflow Actionlint](https://github.com/tjtharrison/pytmac/actions/workflows/pr-actionlint.yaml/badge.svg)
 ![Workflow Checkov](https://github.com/tjtharrison/pytmac/actions/workflows/pr-checkov.yaml/badge.svg)
 ![Workflow Linting](https://github.com/tjtharrison/pytmac/actions/workflows/pr-linting.yaml/badge.svg)
 ![Workflow Unit Tests](https://github.com/tjtharrison/pytmac/actions/workflows/pr-tests.yaml/badge.svg)
 ![Workflow CodeQL](https://github.com/tjtharrison/pytmac/actions/workflows/pr-codeql.yaml/badge.svg)
 
@@ -26,45 +32,38 @@
 
 # Usage
 
 Once installed, pytmac can be called from the command line with an array of arguments which are described in the help page:
 
 ```
 pytmac --help
-
-options:
-  -h, --help            show this help message and exit
-  --version             Option to print the current version only
-  --demo                Run pytmac in demo mode using the demo config and resources
-  --output-dir OUTPUT_DIR
-                        [Default: reports] Set the directory for report output
-  --resources-file RESOURCES_FILE
-                        The path to the resources file
-  --config-file CONFIG_FILE
-                        The path to the config file
-  --defaults-file DEFAULTS_FILE
-                        The path to the defaults file
-  --security-checks-file SECURITY_CHECKS_FILE
-                        [Default: security_checks.yaml] The path to the security-checks file
-  --swagger-file SWAGGER_FILE
-                        [Default: None] The path to the swagger file (optional)
 ```
 
 ## Demonstration
 
 To generate an example report based on some pre-defined resources, run the following command:
 
 ```
 pytmac --demo
 ```
 
 This will write to a file called `report-[today-date].md` which can be viewed in a markdown viewer.
 
 # Configuration
 
+## Init mode
+
+pytmac can be run in init mode to generate configuration files using a combination of inputs provided and default project settings. This can be done with the following command:
+
+```bash
+pytmac --init
+```
+
+Once the initialisation has completed, you should review the generated files and make any changes required (Primary focus should be on the defaults file as this will globally define security settings for all generated resources in your project.
+
 ## Config file
 
 pytmac on launch will look for a file in the current directory named `.pytmac` as a source of settings. This file can be used to set the following settings:
 
 ```
 resource_file: "docs/resources.yaml"
 config_file: "docs/config.yaml"
```

### Comparing `pytmac-3.3.2/bin/get_config.py` & `pytmac-3.4.0/bin/get_config.py`

 * *Files identical despite different names*

### Comparing `pytmac-3.3.2/bin/input_validator.py` & `pytmac-3.4.0/bin/input_validator.py`

 * *Files identical despite different names*

### Comparing `pytmac-3.3.2/bin/resource_validator.py` & `pytmac-3.4.0/bin/resource_validator.py`

 * *Files identical despite different names*

### Comparing `pytmac-3.3.2/docs/defaults.yaml` & `pytmac-3.4.0/docs/defaults.yaml`

 * *Files identical despite different names*

### Comparing `pytmac-3.3.2/docs/resources.yaml` & `pytmac-3.4.0/docs/resources.yaml`

 * *Files identical despite different names*

### Comparing `pytmac-3.3.2/docs/security_checks.yaml` & `pytmac-3.4.0/docs/security_checks.yaml`

 * *Files identical despite different names*

### Comparing `pytmac-3.3.2/docs/swagger.json` & `pytmac-3.4.0/docs/swagger.json`

 * *Files identical despite different names*

### Comparing `pytmac-3.3.2/pytmac` & `pytmac-3.4.0/pytmac`

 * *Files 14% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 import logging
 import os
 import subprocess
 import sys
 from copy import deepcopy
 from datetime import date
 
+import inquirer
 import yaml
 
 from _version import __version__
-from bin import get_config, input_validator, resource_validator
+from bin import get_config, init, input_validator, resource_validator
 
 VERSION = __version__
 
 # Configure logging
 logging.basicConfig(
     format=(
         "{"
@@ -78,14 +79,19 @@
 )
 parser.add_argument(
     "--swagger-file",
     action="store",
     default="None",
     help="[Default: None] The path to the swagger file (optional)",
 )
+parser.add_argument(
+    "--init",
+    action="store_true",
+    help="Enable directory initialisation mode",
+)
 
 args = parser.parse_args()
 
 
 def main(
     resources_yaml,
     config_yaml,
@@ -191,26 +197,32 @@
         with open(
             output_file_dir + "/" + output_file_name + ".yaml", "w", encoding="UTF-8"
         ) as output_yaml:
             # Start empty json for output report
             output_yaml_report = {}
             # Write intro into markdown
             output_file.write("# " + config_yaml["title"] + "\n")
-            for description_line in config_yaml["description"]:
-                output_file.write(description_line + "\n\n")
+            if type(config_yaml["description"]) == list:
+                for description_line in config_yaml["description"]:
+                    output_file.write(description_line + "\n")
+            else:
+                output_file.write(config_yaml["description"])
+            output_file.write("\n\n")
 
             # Write wrapper for DFD
             output_file.write("# Data Flow Diagram\n")
             output_file.write("```plantuml\n")
             output_file.write("@startuml " + output_file_name + "\n")
             output_file.write(
-                "!include https://raw.githubusercontent.com/plantuml-stdlib/C4-PlantUML/master/C4_Container.puml\n"
+                "!include https://raw.githubusercontent.com/"
+                "plantuml-stdlib/C4-PlantUML/master/C4_Container.puml\n"
             )
             output_file.write(
-                "!include https://raw.githubusercontent.com/geret1/plantuml-schemas/main/stride.puml\n"
+                "!include https://raw.githubusercontent.com/"
+                "geret1/plantuml-schemas/main/stride.puml\n"
             )
             output_file.write("\n")
 
             # Write networks wrapper
             output_yaml_report["networks"] = {}
             output_yaml_report["databases"] = {}
             output_yaml_report["users"] = {}
@@ -449,21 +461,146 @@
 
     return True
 
 
 if __name__ == "__main__":
     if args.version:
         print(VERSION)
+        sys.exit(0)
+    elif args.init:
+        # Get config inputs from user
+        try:
+            project_config = init.get_inputs()
+        except KeyboardInterrupt:
+            print("\n\nOkay, maybe later!")
+            sys.exit(1)
+
+        # Create config file directory
+        try:
+            init.create_directory(project_config["config_directory"])
+        except OSError:
+            logging.error("Unable to create %s", project_config["config_directory"])
+            sys.exit(1)
+
+        # Create config file
+        try:
+            init.create_config_file(project_config)
+        except OSError as error_message:
+            print("Unable to get demo config file: " + str(error_message))
+            sys.exit(1)
+        except KeyError as error_message:
+            print("Values provided are not valid" + str(error_message))
+            sys.exit(1)
+        except yaml.YAMLError as error_message:
+            print("Unable to write config file: " + str(error_message))
+            sys.exit(1)
+
+        # Create defaults file
+        try:
+            init.create_defaults_file(project_config)
+        except OSError:
+            logging.error("Unable to write defaults file")
+            sys.exit(1)
+        except yaml.YAMLError:
+            logging.error("Unable to write defaults file")
+            sys.exit(1)
+
+        # Set lists to blank
+        users = []
+        databases = []
+        systems = []
+        # Get networks
+        try:
+            networks = init.get_networks()
+        except KeyboardInterrupt:
+            print("\n\nOkay, maybe later!")
+            sys.exit(1)
+
+        for network in networks:
+            network = network["name"]
+
+            # Add some users
+            try:
+                users = init.get_users(network, users)
+            except KeyboardInterrupt:
+                print("\n\nOkay, maybe later!")
+                sys.exit(1)
+
+            # Add some databases
+            try:
+                databases = init.get_databases(network, databases)
+            except KeyboardInterrupt:
+                print("\n\nOkay, maybe later!")
+                sys.exit(1)
+
+            # Add some systems
+            try:
+                systems = init.get_systems(network, systems)
+            except KeyboardInterrupt:
+                print("\n\nOkay, maybe later!")
+                sys.exit(1)
+
+        all_resources = {
+            "resources": {
+                "networks": networks,
+                "users": users,
+                "databases": databases,
+                "systems": systems,
+            }
+        }
+
+        # Get all resources
+        all_resource_names = init.get_resource_names(all_resources)
+
+        # Create some links between resources
+        try:
+            links = init.get_links(all_resource_names)
+        except KeyboardInterrupt:
+            print("\n\nOkay, maybe later!")
+            sys.exit(1)
+
+        final_resources = {
+            "resources": {
+                "networks": networks,
+                "users": users,
+                "databases": databases,
+                "systems": systems,
+                "res_links": links,
+                "containers": [],
+            }
+        }
+
+        # Write resources to file
+        try:
+            init.create_resources_file(project_config, final_resources)
+        except OSError:
+            logging.error("Unable to write resources file")
+            sys.exit(1)
+        except yaml.YAMLError:
+            logging.error("Unable to write resources file")
+            sys.exit(1)
+
+        # Create .pytmac file
+        try:
+            init.create_settings_file(project_config)
+        except OSError:
+            logging.error("Unable to write settings file")
+            sys.exit(1)
+
+        # Return summary
+        init.return_summary(project_config)
+        sys.exit(0)
+
     elif args.demo:
         logging.info("Running in demonstration mode")
         resources_input = get_config.resources("demo")
         config_input = get_config.config("demo")
         defaults_input = get_config.defaults("demo")
         security_checks_input = get_config.security_checks("default")
-        swagger_input = get_config.swagger("demo")
+        SWAGGER_INPUT = get_config.swagger("demo")
     else:
         # Check if .pytmac file exists
         if os.path.isfile(".pytmac"):
             SETTINGS_FILE_EXISTS = True
             logging.info("Found .pytmac settings file")
             settings_input = get_config.settings()
         else:
@@ -542,15 +679,15 @@
             logging.error(
                 "Error loading configuration files: "
                 + ", ".join(error_response_list)
                 + ". See --help for details"
             )
             sys.exit(1)
 
-        main(
-            resources_input,
-            config_input,
-            defaults_input,
-            security_checks_input,
-            args.output_dir,
-            SWAGGER_INPUT,
-        )
+    main(
+        resources_input,
+        config_input,
+        defaults_input,
+        security_checks_input,
+        args.output_dir,
+        SWAGGER_INPUT,
+    )
```

### Comparing `pytmac-3.3.2/pytmac.egg-info/PKG-INFO` & `pytmac-3.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: pytmac
-Version: 3.3.2
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git?ref=badge_shield)
 ![Workflow Actionlint](https://github.com/tjtharrison/pytmac/actions/workflows/pr-actionlint.yaml/badge.svg)
 ![Workflow Checkov](https://github.com/tjtharrison/pytmac/actions/workflows/pr-checkov.yaml/badge.svg)
 ![Workflow Linting](https://github.com/tjtharrison/pytmac/actions/workflows/pr-linting.yaml/badge.svg)
 ![Workflow Unit Tests](https://github.com/tjtharrison/pytmac/actions/workflows/pr-tests.yaml/badge.svg)
 ![Workflow CodeQL](https://github.com/tjtharrison/pytmac/actions/workflows/pr-codeql.yaml/badge.svg)
 
@@ -32,45 +26,38 @@
 
 # Usage
 
 Once installed, pytmac can be called from the command line with an array of arguments which are described in the help page:
 
 ```
 pytmac --help
-
-options:
-  -h, --help            show this help message and exit
-  --version             Option to print the current version only
-  --demo                Run pytmac in demo mode using the demo config and resources
-  --output-dir OUTPUT_DIR
-                        [Default: reports] Set the directory for report output
-  --resources-file RESOURCES_FILE
-                        The path to the resources file
-  --config-file CONFIG_FILE
-                        The path to the config file
-  --defaults-file DEFAULTS_FILE
-                        The path to the defaults file
-  --security-checks-file SECURITY_CHECKS_FILE
-                        [Default: security_checks.yaml] The path to the security-checks file
-  --swagger-file SWAGGER_FILE
-                        [Default: None] The path to the swagger file (optional)
 ```
 
 ## Demonstration
 
 To generate an example report based on some pre-defined resources, run the following command:
 
 ```
 pytmac --demo
 ```
 
 This will write to a file called `report-[today-date].md` which can be viewed in a markdown viewer.
 
 # Configuration
 
+## Init mode
+
+pytmac can be run in init mode to generate configuration files using a combination of inputs provided and default project settings. This can be done with the following command:
+
+```bash
+pytmac --init
+```
+
+Once the initialisation has completed, you should review the generated files and make any changes required (Primary focus should be on the defaults file as this will globally define security settings for all generated resources in your project.
+
 ## Config file
 
 pytmac on launch will look for a file in the current directory named `.pytmac` as a source of settings. This file can be used to set the following settings:
 
 ```
 resource_file: "docs/resources.yaml"
 config_file: "docs/config.yaml"
```

### Comparing `pytmac-3.3.2/setup.py` & `pytmac-3.4.0/setup.py`

 * *Files identical despite different names*

