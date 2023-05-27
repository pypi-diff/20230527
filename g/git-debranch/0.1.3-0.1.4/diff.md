# Comparing `tmp/git-debranch-0.1.3.tar.gz` & `tmp/git-debranch-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-debranch-0.1.3.tar", last modified: Mon May 22 02:20:05 2023, max compression
+gzip compressed data, was "git-debranch-0.1.4.tar", last modified: Fri May 26 17:55:27 2023, max compression
```

## Comparing `git-debranch-0.1.3.tar` & `git-debranch-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:20:05.023182 git-debranch-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-22 02:19:55.000000 git-debranch-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-22 02:20:05.023182 git-debranch-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-22 02:19:55.000000 git-debranch-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 02:20:05.023182 git-debranch-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-22 02:19:55.000000 git-debranch-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:20:05.019183 git-debranch-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:20:05.019183 git-debranch-0.1.3/src/git_debranch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 02:19:55.000000 git-debranch-0.1.3/src/git_debranch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:20:05.019183 git-debranch-0.1.3/src/git_debranch/bpmn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:20:05.019183 git-debranch-0.1.3/src/git_debranch/bpmn/git-debranch/
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-05-22 02:19:55.000000 git-debranch-0.1.3/src/git_debranch/bpmn/git-debranch/all_branches.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-05-22 02:19:55.000000 git-debranch-0.1.3/src/git_debranch/bpmn/git-debranch/branch_parser.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-22 02:19:55.000000 git-debranch-0.1.3/src/git_debranch/bpmn/git-debranch/confirm_deletion.json
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-22 02:19:55.000000 git-debranch-0.1.3/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-05-22 02:19:55.000000 git-debranch-0.1.3/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-05-22 02:19:55.000000 git-debranch-0.1.3/src/git_debranch/bpmn/git-debranch/git-debranch.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-22 02:19:55.000000 git-debranch-0.1.3/src/git_debranch/bpmn/git-debranch/process_model.json
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-22 02:19:55.000000 git-debranch-0.1.3/src/git_debranch/bpmn/process_group.json
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-22 02:19:55.000000 git-debranch-0.1.3/src/git_debranch/console_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-22 02:19:55.000000 git-debranch-0.1.3/src/git_debranch/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-22 02:19:55.000000 git-debranch-0.1.3/src/git_debranch/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-22 02:19:55.000000 git-debranch-0.1.3/src/git_debranch/script_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-22 02:19:55.000000 git-debranch-0.1.3/src/git_debranch/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:20:05.019183 git-debranch-0.1.3/src/git_debranch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-22 02:20:05.000000 git-debranch-0.1.3/src/git_debranch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-22 02:20:05.000000 git-debranch-0.1.3/src/git_debranch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 02:20:05.000000 git-debranch-0.1.3/src/git_debranch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-22 02:20:05.000000 git-debranch-0.1.3/src/git_debranch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 02:20:05.000000 git-debranch-0.1.3/src/git_debranch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:55:27.119764 git-debranch-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-26 17:55:18.000000 git-debranch-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-26 17:55:27.119764 git-debranch-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-26 17:55:18.000000 git-debranch-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 17:55:27.119764 git-debranch-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-26 17:55:18.000000 git-debranch-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:55:27.111765 git-debranch-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:55:27.115764 git-debranch-0.1.4/src/git_debranch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:55:27.119764 git-debranch-0.1.4/src/git_debranch/bpmn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:55:27.119764 git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/
+-rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/all_branches.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/branch_parser.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/confirm_deletion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/git-debranch.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/process_model.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/spawn.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/bpmn/process_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/console_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/script_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:55:27.119764 git-debranch-0.1.4/src/git_debranch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-26 17:55:27.000000 git-debranch-0.1.4/src/git_debranch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-26 17:55:27.000000 git-debranch-0.1.4/src/git_debranch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 17:55:27.000000 git-debranch-0.1.4/src/git_debranch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-26 17:55:27.000000 git-debranch-0.1.4/src/git_debranch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-26 17:55:27.000000 git-debranch-0.1.4/src/git_debranch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 17:55:27.000000 git-debranch-0.1.4/src/git_debranch.egg-info/top_level.txt
```

### Comparing `git-debranch-0.1.3/LICENSE` & `git-debranch-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.3/PKG-INFO` & `git-debranch-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: git-debranch
-Version: 0.1.3
-Summary: Remove git branches
-Author: Jon Herron
-Author-email: jon.herron@yahoo.com
-License: lGPLv2
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # git-debranch
 
 Git subcommand that uses [SpiffWorkflow](https://github.com/sartography/SpiffWorkflow) to remove branches that are no longer needed.
 
 ## Installation
 
 ```
@@ -55,21 +44,17 @@
 
 You likely want to be inside a venv. This wlll give you an editable installation so you can run the program 
 and see changes. If you add a new bpmn/json file then you need to re-run this command.
 
 ### Using SpiffArena for BPMN edits
 
 [SpiffArena](https://github.com/sartography/spiff-arena) is used to make edits to the BPMN files that are 
-bundled with this program. Currently it is assumed that you have a working copy, possibly from the 
-[Getting Started Guide](https://www.spiffworkflow.org/posts/articles/get_started/). When using SpiffArena as 
-the editor you need to set the following environment variable:
-
-```
-SPIFFWORKFLOW_BACKEND_BPMN_SPEC_ABSOLUTE_DIR
-```
-
-to point to `src/git_debranch` inside this repository. If using docker, the volume that is used for the 
-process models will need to be updated to point to this location.
+bundled with this program. To start the editor run `make run-editor`. You will be presented with a message
+once started to go to `http://localhost:8001` (assuming the default configuration is used). The editor
+requires `docker` and `docker compose` to run.
 
 From there you can edit the diagrams but you cannot run them from within SpiffArena at this time. Some work 
 would need to be done to support our custom `Connector Proxy` that is not http based. You can however run 
 the `Script Task` unit tests, which were very helpful during development.
+
+When finished you can `make stop-editor`. If you would like to pull the latest version of SpiffArena use
+`make update-editor`.
```

### Comparing `git-debranch-0.1.3/README.md` & `git-debranch-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: git-debranch
+Version: 0.1.4
+Summary: Remove git branches
+Author: Jon Herron
+Author-email: jon.herron@yahoo.com
+License: lGPLv2
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # git-debranch
 
 Git subcommand that uses [SpiffWorkflow](https://github.com/sartography/SpiffWorkflow) to remove branches that are no longer needed.
 
 ## Installation
 
 ```
@@ -44,21 +55,17 @@
 
 You likely want to be inside a venv. This wlll give you an editable installation so you can run the program 
 and see changes. If you add a new bpmn/json file then you need to re-run this command.
 
 ### Using SpiffArena for BPMN edits
 
 [SpiffArena](https://github.com/sartography/spiff-arena) is used to make edits to the BPMN files that are 
-bundled with this program. Currently it is assumed that you have a working copy, possibly from the 
-[Getting Started Guide](https://www.spiffworkflow.org/posts/articles/get_started/). When using SpiffArena as 
-the editor you need to set the following environment variable:
-
-```
-SPIFFWORKFLOW_BACKEND_BPMN_SPEC_ABSOLUTE_DIR
-```
-
-to point to `src/git_debranch` inside this repository. If using docker, the volume that is used for the 
-process models will need to be updated to point to this location.
+bundled with this program. To start the editor run `make run-editor`. You will be presented with a message
+once started to go to `http://localhost:8001` (assuming the default configuration is used). The editor
+requires `docker` and `docker compose` to run.
 
 From there you can edit the diagrams but you cannot run them from within SpiffArena at this time. Some work 
 would need to be done to support our custom `Connector Proxy` that is not http based. You can however run 
 the `Script Task` unit tests, which were very helpful during development.
+
+When finished you can `make stop-editor`. If you would like to pull the latest version of SpiffArena use
+`make update-editor`.
```

### Comparing `git-debranch-0.1.3/setup.py` & `git-debranch-0.1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 
 def contents_of(filename):
     with open(filename) as f:
         return f.read()
 
 setup(
     name = "git-debranch",
-    version = "0.1.3",
+    version = "0.1.4",
     description = "Remove git branches",
     long_description = contents_of("README.md"),
     long_description_content_type = "text/markdown",
 
     license = "lGPLv2",
     author = "Jon Herron",
     author_email = "jon.herron@yahoo.com",
 
-    # uncomment after SpiffWorkflow 2.0 release
-    #install_requires = contents_of("requirements.txt"),
+    install_requires = contents_of("requirements.txt"),
     python_requires = ">=3.9",
 
     package_dir = {"": "src"},
     packages = find_packages(where="src"),
 
     package_data = {
         "git_debranch": [
```

### Comparing `git-debranch-0.1.3/src/git_debranch/bpmn/git-debranch/all_branches.bpmn` & `git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/all_branches.bpmn`

 * *Files 21% similar despite different names*

#### Comparing `git-debranch-0.1.3/src/git_debranch/bpmn/git-debranch/all_branches.bpmn` & `git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/all_branches.bpmn`

```diff
@@ -2,394 +2,257 @@
 <bpmn:definitions xmlns:bpmn="http://www.omg.org/spec/BPMN/20100524/MODEL" xmlns:bpmndi="http://www.omg.org/spec/BPMN/20100524/DI" xmlns:dc="http://www.omg.org/spec/DD/20100524/DC" xmlns:spiffworkflow="http://spiffworkflow.org/bpmn/schema/1.0/core" xmlns:di="http://www.omg.org/spec/DD/20100524/DI" id="Definitions_96f6665" targetNamespace="http://bpmn.io/schema/bpmn" exporter="Camunda Modeler" exporterVersion="3.0.0-dev">
   <bpmn:process id="get_all_branches" name="Get all branches" isExecutable="true">
     <bpmn:startEvent id="StartEvent_1">
       <bpmn:outgoing>Flow_0hezl4t</bpmn:outgoing>
     </bpmn:startEvent>
     <bpmn:sequenceFlow id="Flow_0hezl4t" sourceRef="StartEvent_1" targetRef="Activity_0lb6dii"/>
     <bpmn:parallelGateway id="Gateway_07vk4jr">
-      <bpmn:incoming>Flow_1yblrd3</bpmn:incoming>
+      <bpmn:incoming>Flow_1ogqfb8</bpmn:incoming>
       <bpmn:outgoing>Flow_0889ozu</bpmn:outgoing>
-      <bpmn:outgoing>Flow_083ij9n</bpmn:outgoing>
+      <bpmn:outgoing>Flow_05auvqd</bpmn:outgoing>
+      <bpmn:outgoing>Flow_1nxzhsg</bpmn:outgoing>
+      <bpmn:outgoing>Flow_02avd0d</bpmn:outgoing>
     </bpmn:parallelGateway>
-    <bpmn:sequenceFlow id="Flow_0889ozu" sourceRef="Gateway_07vk4jr" targetRef="Activity_09co3ki"/>
-    <bpmn:sequenceFlow id="Flow_083ij9n" sourceRef="Gateway_07vk4jr" targetRef="Activity_18f4cgn"/>
-    <bpmn:sequenceFlow id="Flow_0auw9z4" sourceRef="Activity_18f4cgn" targetRef="Gateway_0gmspex"/>
+    <bpmn:sequenceFlow id="Flow_0889ozu" sourceRef="Gateway_07vk4jr" targetRef="Activity_09d782o"/>
     <bpmn:parallelGateway id="Gateway_0gmspex">
-      <bpmn:incoming>Flow_0auw9z4</bpmn:incoming>
-      <bpmn:incoming>Flow_0rz5563</bpmn:incoming>
-      <bpmn:outgoing>Flow_1g5uuim</bpmn:outgoing>
+      <bpmn:incoming>Flow_02q163a</bpmn:incoming>
+      <bpmn:incoming>Flow_1msiwsx</bpmn:incoming>
+      <bpmn:incoming>Flow_1p2ht7u</bpmn:incoming>
+      <bpmn:incoming>Flow_0ua7und</bpmn:incoming>
+      <bpmn:outgoing>Flow_0plnctp</bpmn:outgoing>
     </bpmn:parallelGateway>
-    <bpmn:sequenceFlow id="Flow_0rz5563" sourceRef="Activity_09co3ki" targetRef="Gateway_0gmspex"/>
-    <bpmn:sequenceFlow id="Flow_1g5uuim" sourceRef="Gateway_0gmspex" targetRef="Gateway_05kek6w"/>
-    <bpmn:scriptTask id="Activity_1rwssw3" name="Add merged and unmerged to result">
+    <bpmn:scriptTask id="Activity_1rwssw3" name="Extract results">
       <bpmn:extensionElements>
         <spiffworkflow:unitTests>
           <spiffworkflow:unitTest id="happiest_of_paths">
             <spiffworkflow:inputJson>{
   &quot;merged_branches_result&quot;: {
     &quot;returncode&quot;: 0,
     &quot;stdout&quot;: &quot; a\n b\n c\n\n&quot;,
     &quot;stderr&quot;: &quot;&quot;
   },
   &quot;unmerged_branches_result&quot;: {
     &quot;returncode&quot;: 0,
     &quot;stdout&quot;: &quot; d\n e\n f\n\n&quot;,
     &quot;stderr&quot;: &quot;&quot;
-  }
-}</spiffworkflow:inputJson>
-            <spiffworkflow:expectedOutputJson>{
-  &quot;merged_branches_result&quot;: {
-    &quot;returncode&quot;: 0,
-    &quot;stderr&quot;: &quot;&quot;,
-    &quot;stdout&quot;: &quot; a\n b\n c\n\n&quot;
   },
-  &quot;result&quot;: {
-    &quot;merged&quot;: &quot; a\n b\n c\n\n&quot;,
+  &quot;remote_branches_result&quot;: {
     &quot;returncode&quot;: 0,
-    &quot;unmerged&quot;: &quot; d\n e\n f\n\n&quot;
+    &quot;stdout&quot;: &quot; g\n h\n i\n\n&quot;,
+    &quot;stderr&quot;: &quot;&quot;
   },
-  &quot;unmerged_branches_result&quot;: {
+  &quot;current_branch_result&quot;: {
     &quot;returncode&quot;: 0,
-    &quot;stderr&quot;: &quot;&quot;,
-    &quot;stdout&quot;: &quot; d\n e\n f\n\n&quot;
+    &quot;stdout&quot;: &quot;j\n&quot;,
+    &quot;stderr&quot;: &quot;&quot;
   }
+}</spiffworkflow:inputJson>
+            <spiffworkflow:expectedOutputJson>{
+  &quot;result&quot;: { &quot;returncode&quot;: 0 },
+  &quot;current&quot;: &quot;j\n&quot;,
+  &quot;merged&quot;: &quot; a\n b\n c\n\n&quot;,
+  &quot;remote&quot;: &quot; g\n h\n i\n\n&quot;,
+  &quot;unmerged&quot;: &quot; d\n e\n f\n\n&quot;
 }</spiffworkflow:expectedOutputJson>
           </spiffworkflow:unitTest>
         </spiffworkflow:unitTests>
       </bpmn:extensionElements>
-      <bpmn:incoming>Flow_0edbiko</bpmn:incoming>
+      <bpmn:incoming>Flow_0plnctp</bpmn:incoming>
       <bpmn:outgoing>Flow_04ggq0k</bpmn:outgoing>
       <bpmn:script># pre-conditions of this script, would love to move to pre script
 # or have contract support
 assert merged_branches_result[&quot;returncode&quot;] == 0
 assert unmerged_branches_result[&quot;returncode&quot;] == 0
+assert remote_branches_result[&quot;returncode&quot;] == 0
+assert current_branch_result[&quot;returncode&quot;] == 0
 
-result = {
-    &quot;returncode&quot;: 0,
-    &quot;merged&quot;: merged_branches_result[&quot;stdout&quot;],
-    &quot;unmerged&quot;: unmerged_branches_result[&quot;stdout&quot;],
-}</bpmn:script>
+result = { &quot;returncode&quot;: 0 }
+
+merged = merged_branches_result[&quot;stdout&quot;]
+unmerged = unmerged_branches_result[&quot;stdout&quot;]
+remote = remote_branches_result[&quot;stdout&quot;]
+current = current_branch_result[&quot;stdout&quot;]
+
+del(merged_branches_result)
+del(unmerged_branches_result)
+del(remote_branches_result)
+del(current_branch_result)
+del(spawn_args)</bpmn:script>
     </bpmn:scriptTask>
-    <bpmn:serviceTask id="Activity_09co3ki" name="Get all merged branches">
+    <bpmn:sequenceFlow id="Flow_04ggq0k" sourceRef="Activity_1rwssw3" targetRef="Event_1y1qa7g"/>
+    <bpmn:endEvent id="Event_1y1qa7g">
+      <bpmn:incoming>Flow_04ggq0k</bpmn:incoming>
+    </bpmn:endEvent>
+    <bpmn:sequenceFlow id="Flow_1ogqfb8" sourceRef="Activity_0lb6dii" targetRef="Gateway_07vk4jr"/>
+    <bpmn:sequenceFlow id="Flow_0plnctp" sourceRef="Gateway_0gmspex" targetRef="Activity_1rwssw3"/>
+    <bpmn:callActivity id="Activity_09d782o" name="Get merged branches" calledElement="spawn_process">
       <bpmn:extensionElements>
-        <spiffworkflow:serviceTaskOperator id="git/ListAllMergedBranches" resultVariable="merged_branches_result"/>
+        <spiffworkflow:preScript>spawn_args = [&quot;git&quot;, &quot;branch&quot;, &quot;--merged&quot;]</spiffworkflow:preScript>
+        <spiffworkflow:postScript>merged_branches_result = result</spiffworkflow:postScript>
       </bpmn:extensionElements>
       <bpmn:incoming>Flow_0889ozu</bpmn:incoming>
-      <bpmn:outgoing>Flow_0rz5563</bpmn:outgoing>
-    </bpmn:serviceTask>
-    <bpmn:serviceTask id="Activity_18f4cgn" name="Get all unmerged branches">
+      <bpmn:outgoing>Flow_02q163a</bpmn:outgoing>
+    </bpmn:callActivity>
+    <bpmn:sequenceFlow id="Flow_02q163a" sourceRef="Activity_09d782o" targetRef="Gateway_0gmspex"/>
+    <bpmn:callActivity id="Activity_1qlm0jm" name="Get unmerged branches" calledElement="spawn_process">
       <bpmn:extensionElements>
-        <spiffworkflow:serviceTaskOperator id="git/ListAllUnmergedBranches" resultVariable="unmerged_branches_result"/>
+        <spiffworkflow:preScript>spawn_args = [&quot;git&quot;, &quot;branch&quot;, &quot;--no-merged&quot;]</spiffworkflow:preScript>
+        <spiffworkflow:postScript>unmerged_branches_result = result</spiffworkflow:postScript>
       </bpmn:extensionElements>
-      <bpmn:incoming>Flow_083ij9n</bpmn:incoming>
-      <bpmn:outgoing>Flow_0auw9z4</bpmn:outgoing>
-    </bpmn:serviceTask>
-    <bpmn:exclusiveGateway id="Gateway_05kek6w" default="Flow_0edbiko">
-      <bpmn:incoming>Flow_1g5uuim</bpmn:incoming>
-      <bpmn:outgoing>Flow_0edbiko</bpmn:outgoing>
-      <bpmn:outgoing>Flow_1sqrwy8</bpmn:outgoing>
-    </bpmn:exclusiveGateway>
-    <bpmn:sequenceFlow id="Flow_0edbiko" sourceRef="Gateway_05kek6w" targetRef="Activity_1rwssw3"/>
-    <bpmn:sequenceFlow id="Flow_1sqrwy8" sourceRef="Gateway_05kek6w" targetRef="Activity_0jtu6nb">
-      <bpmn:conditionExpression>merged_branches_result[&quot;returncode&quot;] != 0 or unmerged_branches_result[&quot;returncode&quot;] != 0</bpmn:conditionExpression>
-    </bpmn:sequenceFlow>
-    <bpmn:exclusiveGateway id="Gateway_0pemmv3">
-      <bpmn:incoming>Flow_18ez3n1</bpmn:incoming>
-      <bpmn:incoming>Flow_04ggq0k</bpmn:incoming>
-      <bpmn:outgoing>Flow_01pmr38</bpmn:outgoing>
-    </bpmn:exclusiveGateway>
-    <bpmn:sequenceFlow id="Flow_18ez3n1" sourceRef="Activity_0jtu6nb" targetRef="Gateway_0pemmv3"/>
-    <bpmn:sequenceFlow id="Flow_04ggq0k" sourceRef="Activity_1rwssw3" targetRef="Gateway_0pemmv3"/>
-    <bpmn:endEvent id="Event_1y1qa7g">
-      <bpmn:incoming>Flow_1w9g09q</bpmn:incoming>
-    </bpmn:endEvent>
-    <bpmn:sequenceFlow id="Flow_01pmr38" sourceRef="Gateway_0pemmv3" targetRef="Activity_0bjc1ye"/>
-    <bpmn:scriptTask id="Activity_0jtu6nb" name="Promote an error to result">
+      <bpmn:incoming>Flow_05auvqd</bpmn:incoming>
+      <bpmn:outgoing>Flow_1msiwsx</bpmn:outgoing>
+    </bpmn:callActivity>
+    <bpmn:sequenceFlow id="Flow_05auvqd" sourceRef="Gateway_07vk4jr" targetRef="Activity_1qlm0jm"/>
+    <bpmn:sequenceFlow id="Flow_1msiwsx" sourceRef="Activity_1qlm0jm" targetRef="Gateway_0gmspex"/>
+    <bpmn:callActivity id="Activity_1ntduty" name="Get remote branches" calledElement="spawn_process">
       <bpmn:extensionElements>
-        <spiffworkflow:unitTests>
-          <spiffworkflow:unitTest id="merged_and_unmerged_failure">
-            <spiffworkflow:inputJson>{
-  &quot;merged_branches_result&quot;: {
-    &quot;returncode&quot;: 1,
-    &quot;stdout&quot;: &quot;&quot;,
-    &quot;stderr&quot;: &quot;merged error&quot;
-  },
-  &quot;unmerged_branches_result&quot;: {
-    &quot;returncode&quot;: 2,
-    &quot;stdout&quot;: &quot;&quot;,
-    &quot;stderr&quot;: &quot;unmerged_error&quot;
-  }
-}</spiffworkflow:inputJson>
-            <spiffworkflow:expectedOutputJson>{
-  &quot;merged_branches_result&quot;: {
-    &quot;returncode&quot;: 1,
-    &quot;stderr&quot;: &quot;merged error&quot;,
-    &quot;stdout&quot;: &quot;&quot;
-  },
-  &quot;result&quot;: {
-    &quot;returncode&quot;: 1,
-    &quot;stderr&quot;: &quot;merged error&quot;,
-    &quot;stdout&quot;: &quot;&quot;
-  },
-  &quot;unmerged_branches_result&quot;: {
-    &quot;returncode&quot;: 2,
-    &quot;stderr&quot;: &quot;unmerged_error&quot;,
-    &quot;stdout&quot;: &quot;&quot;
-  }
-}</spiffworkflow:expectedOutputJson>
-          </spiffworkflow:unitTest>
-          <spiffworkflow:unitTest id="merged_failture">
-            <spiffworkflow:inputJson>{
-  &quot;merged_branches_result&quot;: {
-    &quot;returncode&quot;: 1,
-    &quot;stdout&quot;: &quot;&quot;,
-    &quot;stderr&quot;: &quot;merged error&quot;
-  },
-  &quot;unmerged_branches_result&quot;: {
-    &quot;returncode&quot;: 0,
-    &quot;stdout&quot;: &quot;&quot;,
-    &quot;stderr&quot;: &quot;&quot;
-  }
-}</spiffworkflow:inputJson>
-            <spiffworkflow:expectedOutputJson>{
-  &quot;merged_branches_result&quot;: {
-    &quot;returncode&quot;: 1,
-    &quot;stderr&quot;: &quot;merged error&quot;,
-    &quot;stdout&quot;: &quot;&quot;
-  },
-  &quot;result&quot;: {
-    &quot;returncode&quot;: 1,
-    &quot;stderr&quot;: &quot;merged error&quot;,
-    &quot;stdout&quot;: &quot;&quot;
-  },
-  &quot;unmerged_branches_result&quot;: {
-    &quot;returncode&quot;: 0,
-    &quot;stderr&quot;: &quot;&quot;,
-    &quot;stdout&quot;: &quot;&quot;
-  }
-}</spiffworkflow:expectedOutputJson>
-          </spiffworkflow:unitTest>
-          <spiffworkflow:unitTest id="unmerged_failure">
-            <spiffworkflow:inputJson>{
-  &quot;merged_branches_result&quot;: {
-    &quot;returncode&quot;: 0,
-    &quot;stdout&quot;: &quot;&quot;,
-    &quot;stderr&quot;: &quot;&quot;
-  },
-  &quot;unmerged_branches_result&quot;: {
-    &quot;returncode&quot;: 2,
-    &quot;stdout&quot;: &quot;&quot;,
-    &quot;stderr&quot;: &quot;unmerged error&quot;
-  }
-}</spiffworkflow:inputJson>
-            <spiffworkflow:expectedOutputJson>{
-  &quot;merged_branches_result&quot;: {
-    &quot;returncode&quot;: 0,
-    &quot;stderr&quot;: &quot;&quot;,
-    &quot;stdout&quot;: &quot;&quot;
-  },
-  &quot;result&quot;: {
-    &quot;returncode&quot;: 2,
-    &quot;stderr&quot;: &quot;unmerged error&quot;,
-    &quot;stdout&quot;: &quot;&quot;
-  },
-  &quot;unmerged_branches_result&quot;: {
-    &quot;returncode&quot;: 2,
-    &quot;stderr&quot;: &quot;unmerged error&quot;,
-    &quot;stdout&quot;: &quot;&quot;
-  }
-}</spiffworkflow:expectedOutputJson>
-          </spiffworkflow:unitTest>
-        </spiffworkflow:unitTests>
+        <spiffworkflow:preScript>spawn_args = [&quot;git&quot;, &quot;branch&quot;, &quot;--remotes&quot;]</spiffworkflow:preScript>
+        <spiffworkflow:postScript>remote_branches_result = result</spiffworkflow:postScript>
       </bpmn:extensionElements>
-      <bpmn:incoming>Flow_1sqrwy8</bpmn:incoming>
-      <bpmn:outgoing>Flow_18ez3n1</bpmn:outgoing>
-      <bpmn:script># pre-conditions of this script, would love to move to pre script
-assert merged_branches_result[&quot;returncode&quot;] != 0 or unmerged_branches_result[&quot;returncode&quot;] != 0
-
-result = merged_branches_result if merged_branches_result[&quot;returncode&quot;] else unmerged_branches_result</bpmn:script>
-    </bpmn:scriptTask>
-    <bpmn:sequenceFlow id="Flow_1w9g09q" sourceRef="Activity_0bjc1ye" targetRef="Event_1y1qa7g"/>
-    <bpmn:scriptTask id="Activity_0bjc1ye" name="Cleanup variables">
-      <bpmn:incoming>Flow_01pmr38</bpmn:incoming>
-      <bpmn:outgoing>Flow_1w9g09q</bpmn:outgoing>
-      <bpmn:script>del(merged_branches_result)
-del(unmerged_branches_result)</bpmn:script>
-    </bpmn:scriptTask>
-    <bpmn:sequenceFlow id="Flow_1gttvuv" sourceRef="Activity_0lb6dii" targetRef="Gateway_0baiicz"/>
-    <bpmn:serviceTask id="Activity_0lb6dii" name="Fetch and prune branches">
+      <bpmn:incoming>Flow_1nxzhsg</bpmn:incoming>
+      <bpmn:outgoing>Flow_1p2ht7u</bpmn:outgoing>
+    </bpmn:callActivity>
+    <bpmn:sequenceFlow id="Flow_1nxzhsg" sourceRef="Gateway_07vk4jr" targetRef="Activity_1ntduty"/>
+    <bpmn:sequenceFlow id="Flow_1p2ht7u" sourceRef="Activity_1ntduty" targetRef="Gateway_0gmspex"/>
+    <bpmn:callActivity id="Activity_0wtw0rj" name="Get current branch" calledElement="spawn_process">
       <bpmn:extensionElements>
-        <spiffworkflow:serviceTaskOperator id="git/FetchAndPrune" resultVariable="result"/>
+        <spiffworkflow:preScript>spawn_args = [&quot;git&quot;, &quot;branch&quot;, &quot;--show-current&quot;]</spiffworkflow:preScript>
+        <spiffworkflow:postScript>current_branch_result = result</spiffworkflow:postScript>
+      </bpmn:extensionElements>
+      <bpmn:incoming>Flow_02avd0d</bpmn:incoming>
+      <bpmn:outgoing>Flow_0ua7und</bpmn:outgoing>
+    </bpmn:callActivity>
+    <bpmn:sequenceFlow id="Flow_02avd0d" sourceRef="Gateway_07vk4jr" targetRef="Activity_0wtw0rj"/>
+    <bpmn:sequenceFlow id="Flow_0ua7und" sourceRef="Activity_0wtw0rj" targetRef="Gateway_0gmspex"/>
+    <bpmn:callActivity id="Activity_0lb6dii" name="Fetch and prune branches" calledElement="spawn_process">
+      <bpmn:extensionElements>
+        <spiffworkflow:serviceTaskOperator id="os/SpawnProcess" resultVariable="result">
+          <spiffworkflow:parameters>
+            <spiffworkflow:parameter id="args" type="any" value="[&quot;git&quot;, &quot;fetch&quot;, &quot;-p&quot;]"/>
+          </spiffworkflow:parameters>
+        </spiffworkflow:serviceTaskOperator>
+        <spiffworkflow:preScript>spawn_args = [&quot;git&quot;, &quot;fetch&quot;, &quot;-p&quot;]</spiffworkflow:preScript>
       </bpmn:extensionElements>
       <bpmn:incoming>Flow_0hezl4t</bpmn:incoming>
-      <bpmn:outgoing>Flow_1gttvuv</bpmn:outgoing>
-    </bpmn:serviceTask>
-    <bpmn:exclusiveGateway id="Gateway_0baiicz" default="Flow_1yblrd3">
-      <bpmn:incoming>Flow_1gttvuv</bpmn:incoming>
-      <bpmn:outgoing>Flow_1yblrd3</bpmn:outgoing>
-      <bpmn:outgoing>Flow_1gxd6ng</bpmn:outgoing>
-    </bpmn:exclusiveGateway>
-    <bpmn:sequenceFlow id="Flow_1yblrd3" sourceRef="Gateway_0baiicz" targetRef="Gateway_07vk4jr"/>
-    <bpmn:endEvent id="Event_1ionpa7">
-      <bpmn:incoming>Flow_1gxd6ng</bpmn:incoming>
-    </bpmn:endEvent>
-    <bpmn:sequenceFlow id="Flow_1gxd6ng" sourceRef="Gateway_0baiicz" targetRef="Event_1ionpa7">
-      <bpmn:conditionExpression>result[&quot;returncode&quot;] != 0</bpmn:conditionExpression>
-    </bpmn:sequenceFlow>
-    <bpmn:textAnnotation id="TextAnnotation_14hvdjh">
-      <bpmn:text>If either git operation fails, return an error, else return the merged and unmerged branch lists.</bpmn:text>
-    </bpmn:textAnnotation>
-    <bpmn:association id="Association_08z4539" sourceRef="Gateway_05kek6w" targetRef="TextAnnotation_14hvdjh"/>
+      <bpmn:outgoing>Flow_1ogqfb8</bpmn:outgoing>
+    </bpmn:callActivity>
     <bpmn:textAnnotation id="TextAnnotation_1b81gty">
-      <bpmn:text>We want to present both merged and unmerged branches. As far as I know this requires two calls to git branches.</bpmn:text>
+      <bpmn:text>Would like to look at making this a multi-instance once things are merged.</bpmn:text>
     </bpmn:textAnnotation>
     <bpmn:association id="Association_06jn47e" sourceRef="Gateway_07vk4jr" targetRef="TextAnnotation_1b81gty"/>
     <bpmn:textAnnotation id="TextAnnotation_1wtp9ek">
-      <bpmn:text>Before checking local branches we want to fetch and prune branches. If this fails exit early</bpmn:text>
+      <bpmn:text>Before checking local branches we want to fetch and prune branches. This will be arg driven soon.</bpmn:text>
     </bpmn:textAnnotation>
     <bpmn:association id="Association_1uty3t0" sourceRef="Activity_0lb6dii" targetRef="TextAnnotation_1wtp9ek"/>
   </bpmn:process>
   <bpmndi:BPMNDiagram id="BPMNDiagram_1">
     <bpmndi:BPMNPlane id="BPMNPlane_1" bpmnElement="get_all_branches">
       <bpmndi:BPMNShape id="_BPMNShape_StartEvent_2" bpmnElement="StartEvent_1">
-        <dc:Bounds x="-88" y="159" width="36" height="36"/>
+        <dc:Bounds x="32" y="159" width="36" height="36"/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Gateway_120o0l4_di" bpmnElement="Gateway_07vk4jr">
         <dc:Bounds x="265" y="152" width="50" height="50"/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Gateway_1v3pb50_di" bpmnElement="Gateway_0gmspex">
         <dc:Bounds x="525" y="152" width="50" height="50"/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Activity_097d5gt_di" bpmnElement="Activity_1rwssw3">
-        <dc:Bounds x="720" y="220" width="100" height="80"/>
+        <dc:Bounds x="610" y="137" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Activity_0cbkwti_di" bpmnElement="Activity_09co3ki">
-        <dc:Bounds x="370" y="60" width="100" height="80"/>
-        <bpmndi:BPMNLabel/>
-      </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Activity_0segx3a_di" bpmnElement="Activity_18f4cgn">
-        <dc:Bounds x="370" y="220" width="100" height="80"/>
-        <bpmndi:BPMNLabel/>
-      </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Gateway_05kek6w_di" bpmnElement="Gateway_05kek6w" isMarkerVisible="true">
-        <dc:Bounds x="615" y="152" width="50" height="50"/>
-      </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Gateway_0pemmv3_di" bpmnElement="Gateway_0pemmv3" isMarkerVisible="true">
-        <dc:Bounds x="875" y="152" width="50" height="50"/>
-      </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Event_1y1qa7g_di" bpmnElement="Event_1y1qa7g">
-        <dc:Bounds x="1102" y="159" width="36" height="36"/>
+        <dc:Bounds x="752" y="159" width="36" height="36"/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Activity_0cytush_di" bpmnElement="Activity_0jtu6nb">
-        <dc:Bounds x="720" y="60" width="100" height="80"/>
+      <bpmndi:BPMNShape id="Activity_1lc0i0u_di" bpmnElement="Activity_09d782o">
+        <dc:Bounds x="370" y="-20" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Activity_09otoif_di" bpmnElement="Activity_0bjc1ye">
-        <dc:Bounds x="960" y="137" width="100" height="80"/>
+      <bpmndi:BPMNShape id="TextAnnotation_1b81gty_di" bpmnElement="TextAnnotation_1b81gty">
+        <dc:Bounds x="160" y="-63" width="100" height="98"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Activity_0lbqcba_di" bpmnElement="Activity_0lb6dii">
-        <dc:Bounds x="-10" y="137" width="100" height="80"/>
+      <bpmndi:BPMNShape id="TextAnnotation_1wtp9ek_di" bpmnElement="TextAnnotation_1wtp9ek">
+        <dc:Bounds x="-30" y="-63" width="100" height="127"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Gateway_0baiicz_di" bpmnElement="Gateway_0baiicz" isMarkerVisible="true">
-        <dc:Bounds x="145" y="152" width="50" height="50"/>
-      </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Event_1ionpa7_di" bpmnElement="Event_1ionpa7">
-        <dc:Bounds x="152" y="282" width="36" height="36"/>
-      </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="TextAnnotation_14hvdjh_di" bpmnElement="TextAnnotation_14hvdjh">
-        <dc:Bounds x="540" y="-63" width="100" height="113"/>
+      <bpmndi:BPMNShape id="BPMNShape_0apvxkl" bpmnElement="Activity_1qlm0jm">
+        <dc:Bounds x="370" y="80" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="TextAnnotation_1b81gty_di" bpmnElement="TextAnnotation_1b81gty">
-        <dc:Bounds x="160" y="-63" width="100" height="142"/>
+      <bpmndi:BPMNShape id="BPMNShape_0w43oon" bpmnElement="Activity_1ntduty">
+        <dc:Bounds x="370" y="190" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="TextAnnotation_1wtp9ek_di" bpmnElement="TextAnnotation_1wtp9ek">
-        <dc:Bounds x="-30" y="-63" width="100" height="113"/>
+      <bpmndi:BPMNShape id="BPMNShape_10pp7pw" bpmnElement="Activity_0wtw0rj">
+        <dc:Bounds x="370" y="290" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
+      <bpmndi:BPMNShape id="Activity_0gv5hia_di" bpmnElement="Activity_0lb6dii">
+        <dc:Bounds x="120" y="137" width="100" height="80"/>
+      </bpmndi:BPMNShape>
       <bpmndi:BPMNEdge id="Flow_0hezl4t_di" bpmnElement="Flow_0hezl4t">
-        <di:waypoint x="-52" y="177"/>
-        <di:waypoint x="-10" y="177"/>
+        <di:waypoint x="68" y="177"/>
+        <di:waypoint x="120" y="177"/>
       </bpmndi:BPMNEdge>
       <bpmndi:BPMNEdge id="Flow_0889ozu_di" bpmnElement="Flow_0889ozu">
         <di:waypoint x="290" y="152"/>
-        <di:waypoint x="290" y="100"/>
-        <di:waypoint x="370" y="100"/>
+        <di:waypoint x="290" y="20"/>
+        <di:waypoint x="370" y="20"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_083ij9n_di" bpmnElement="Flow_083ij9n">
-        <di:waypoint x="290" y="202"/>
-        <di:waypoint x="290" y="260"/>
-        <di:waypoint x="370" y="260"/>
+      <bpmndi:BPMNEdge id="Flow_04ggq0k_di" bpmnElement="Flow_04ggq0k">
+        <di:waypoint x="710" y="177"/>
+        <di:waypoint x="752" y="177"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_0auw9z4_di" bpmnElement="Flow_0auw9z4">
-        <di:waypoint x="470" y="260"/>
-        <di:waypoint x="550" y="260"/>
-        <di:waypoint x="550" y="202"/>
+      <bpmndi:BPMNEdge id="Flow_1ogqfb8_di" bpmnElement="Flow_1ogqfb8">
+        <di:waypoint x="220" y="177"/>
+        <di:waypoint x="265" y="177"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_0rz5563_di" bpmnElement="Flow_0rz5563">
-        <di:waypoint x="470" y="100"/>
-        <di:waypoint x="550" y="100"/>
+      <bpmndi:BPMNEdge id="Flow_0plnctp_di" bpmnElement="Flow_0plnctp">
+        <di:waypoint x="575" y="177"/>
+        <di:waypoint x="610" y="177"/>
+      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Flow_02q163a_di" bpmnElement="Flow_02q163a">
+        <di:waypoint x="470" y="20"/>
+        <di:waypoint x="550" y="20"/>
         <di:waypoint x="550" y="152"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_1g5uuim_di" bpmnElement="Flow_1g5uuim">
-        <di:waypoint x="575" y="177"/>
-        <di:waypoint x="615" y="177"/>
+      <bpmndi:BPMNEdge id="Association_06jn47e_di" bpmnElement="Association_06jn47e">
+        <di:waypoint x="283" y="159"/>
+        <di:waypoint x="239" y="35"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_0edbiko_di" bpmnElement="Flow_0edbiko">
-        <di:waypoint x="640" y="202"/>
-        <di:waypoint x="640" y="260"/>
-        <di:waypoint x="720" y="260"/>
-      </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_1sqrwy8_di" bpmnElement="Flow_1sqrwy8">
-        <di:waypoint x="640" y="152"/>
-        <di:waypoint x="640" y="100"/>
-        <di:waypoint x="720" y="100"/>
-      </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_18ez3n1_di" bpmnElement="Flow_18ez3n1">
-        <di:waypoint x="820" y="100"/>
-        <di:waypoint x="900" y="100"/>
-        <di:waypoint x="900" y="152"/>
+      <bpmndi:BPMNEdge id="Association_1uty3t0_di" bpmnElement="Association_1uty3t0">
+        <di:waypoint x="137" y="137"/>
+        <di:waypoint x="70" y="52"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_04ggq0k_di" bpmnElement="Flow_04ggq0k">
-        <di:waypoint x="820" y="260"/>
-        <di:waypoint x="900" y="260"/>
-        <di:waypoint x="900" y="202"/>
-      </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_01pmr38_di" bpmnElement="Flow_01pmr38">
-        <di:waypoint x="925" y="177"/>
-        <di:waypoint x="960" y="177"/>
-      </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_1w9g09q_di" bpmnElement="Flow_1w9g09q">
-        <di:waypoint x="1060" y="177"/>
-        <di:waypoint x="1102" y="177"/>
-      </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_1gttvuv_di" bpmnElement="Flow_1gttvuv">
-        <di:waypoint x="90" y="177"/>
-        <di:waypoint x="145" y="177"/>
+      <bpmndi:BPMNEdge id="Flow_05auvqd_di" bpmnElement="Flow_05auvqd">
+        <di:waypoint x="290" y="152"/>
+        <di:waypoint x="290" y="120"/>
+        <di:waypoint x="370" y="120"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_1yblrd3_di" bpmnElement="Flow_1yblrd3">
-        <di:waypoint x="195" y="177"/>
-        <di:waypoint x="265" y="177"/>
+      <bpmndi:BPMNEdge id="Flow_1msiwsx_di" bpmnElement="Flow_1msiwsx">
+        <di:waypoint x="470" y="120"/>
+        <di:waypoint x="550" y="120"/>
+        <di:waypoint x="550" y="152"/>
+      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Flow_1nxzhsg_di" bpmnElement="Flow_1nxzhsg">
+        <di:waypoint x="290" y="202"/>
+        <di:waypoint x="290" y="230"/>
+        <di:waypoint x="370" y="230"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_1gxd6ng_di" bpmnElement="Flow_1gxd6ng">
-        <di:waypoint x="170" y="202"/>
-        <di:waypoint x="170" y="282"/>
-      </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Association_08z4539_di" bpmnElement="Association_08z4539">
-        <di:waypoint x="635" y="157"/>
-        <di:waypoint x="612" y="50"/>
+      <bpmndi:BPMNEdge id="Flow_1p2ht7u_di" bpmnElement="Flow_1p2ht7u">
+        <di:waypoint x="470" y="230"/>
+        <di:waypoint x="550" y="230"/>
+        <di:waypoint x="550" y="202"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Association_06jn47e_di" bpmnElement="Association_06jn47e">
-        <di:waypoint x="283" y="159"/>
-        <di:waypoint x="255" y="79"/>
+      <bpmndi:BPMNEdge id="Flow_02avd0d_di" bpmnElement="Flow_02avd0d">
+        <di:waypoint x="290" y="202"/>
+        <di:waypoint x="290" y="330"/>
+        <di:waypoint x="370" y="330"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Association_1uty3t0_di" bpmnElement="Association_1uty3t0">
-        <di:waypoint x="36" y="137"/>
-        <di:waypoint x="29" y="50"/>
+      <bpmndi:BPMNEdge id="Flow_0ua7und_di" bpmnElement="Flow_0ua7und">
+        <di:waypoint x="470" y="330"/>
+        <di:waypoint x="550" y="330"/>
+        <di:waypoint x="550" y="202"/>
       </bpmndi:BPMNEdge>
     </bpmndi:BPMNPlane>
   </bpmndi:BPMNDiagram>
 </bpmn:definitions>
```

### Comparing `git-debranch-0.1.3/src/git_debranch/bpmn/git-debranch/branch_parser.bpmn` & `git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/branch_parser.bpmn`

 * *Files 25% similar despite different names*

#### Comparing `git-debranch-0.1.3/src/git_debranch/bpmn/git-debranch/branch_parser.bpmn` & `git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/branch_parser.bpmn`

```diff
@@ -2,30 +2,64 @@
 <bpmn:definitions xmlns:bpmn="http://www.omg.org/spec/BPMN/20100524/MODEL" xmlns:bpmndi="http://www.omg.org/spec/BPMN/20100524/DI" xmlns:dc="http://www.omg.org/spec/DD/20100524/DC" xmlns:di="http://www.omg.org/spec/DD/20100524/DI" xmlns:spiffworkflow="http://spiffworkflow.org/bpmn/schema/1.0/core" id="Definitions_96f6665" targetNamespace="http://bpmn.io/schema/bpmn" exporter="Camunda Modeler" exporterVersion="3.0.0-dev">
   <bpmn:process id="branch_parser" name="Branch parser" isExecutable="true">
     <bpmn:startEvent id="StartEvent_1">
       <bpmn:outgoing>Flow_0zt50xr</bpmn:outgoing>
     </bpmn:startEvent>
     <bpmn:sequenceFlow id="Flow_0zt50xr" sourceRef="StartEvent_1" targetRef="Activity_0v238ap"/>
     <bpmn:endEvent id="Event_1ts0rz7">
-      <bpmn:incoming>Flow_14g5ljd</bpmn:incoming>
+      <bpmn:incoming>Flow_1icfqqq</bpmn:incoming>
     </bpmn:endEvent>
-    <bpmn:sequenceFlow id="Flow_1345wuj" sourceRef="Activity_0v238ap" targetRef="Activity_0sdmpoy"/>
-    <bpmn:scriptTask id="Activity_0v238ap" name="Split branch strings">
+    <bpmn:scriptTask id="Activity_0v238ap" name="Parse branch strings">
+      <bpmn:extensionElements>
+        <spiffworkflow:unitTests>
+          <spiffworkflow:unitTest id="happy_path">
+            <spiffworkflow:inputJson>{
+  &quot;result&quot;: {
+    &quot;returncode&quot;: 0
+  },
+  &quot;current&quot;: &quot;j\n&quot;,
+  &quot;merged&quot;: &quot; a\n b\n c\n\n&quot;,
+  &quot;remote&quot;: &quot; g\n h\n i\n\n&quot;,
+  &quot;unmerged&quot;: &quot; d\n e\n f\n\n&quot;
+}</spiffworkflow:inputJson>
+            <spiffworkflow:expectedOutputJson>{
+  &quot;result&quot;: {
+    &quot;returncode&quot;: 0
+  },
+  &quot;current&quot;: &quot;j&quot;,
+  &quot;merged&quot;: [
+    &quot; a&quot;,
+    &quot; b&quot;,
+    &quot; c&quot;
+  ],
+  &quot;remote&quot;: [
+    &quot; g&quot;,
+    &quot; h&quot;,
+    &quot; i&quot;
+  ],
+  &quot;unmerged&quot;: [
+    &quot; d&quot;,
+    &quot; e&quot;,
+    &quot; f&quot;
+  ]
+}</spiffworkflow:expectedOutputJson>
+          </spiffworkflow:unitTest>
+        </spiffworkflow:unitTests>
+      </bpmn:extensionElements>
       <bpmn:incoming>Flow_0zt50xr</bpmn:incoming>
-      <bpmn:outgoing>Flow_1345wuj</bpmn:outgoing>
+      <bpmn:outgoing>Flow_0c9l7wr</bpmn:outgoing>
       <bpmn:script>def to_list(branches):
     parts = branches.split(&quot;\n&quot;)
     non_empty_parts = filter(len, parts)
     return list(non_empty_parts)
 
-merged = result.pop(&quot;merged&quot;)
 merged = to_list(merged)
-
-unmerged = result.pop(&quot;unmerged&quot;)
-unmerged = to_list(unmerged)</bpmn:script>
+unmerged = to_list(unmerged)
+remote = to_list(remote)
+current = current.strip()</bpmn:script>
     </bpmn:scriptTask>
     <bpmn:sequenceFlow id="Flow_0edxyrj" sourceRef="Activity_0sdmpoy" targetRef="Activity_1n9ykr2"/>
     <bpmn:scriptTask id="Activity_0sdmpoy" name="Group branches">
       <bpmn:extensionElements>
         <spiffworkflow:unitTests>
           <spiffworkflow:unitTest id="happy_path">
             <spiffworkflow:inputJson>{
@@ -70,15 +104,14 @@
       ]
     }
   }
 }</spiffworkflow:expectedOutputJson>
           </spiffworkflow:unitTest>
         </spiffworkflow:unitTests>
       </bpmn:extensionElements>
-      <bpmn:incoming>Flow_1345wuj</bpmn:incoming>
       <bpmn:outgoing>Flow_0edxyrj</bpmn:outgoing>
       <bpmn:script>def branch_components(branch):
     branch_name = branch[2:]
     branch_type = branch[:2] 
     if &quot; -&gt; &quot; in branch_name:
         branch_type = &quot;&gt; &quot;
     return branch_name, branch_type
@@ -109,15 +142,14 @@
             add_branch(branch_name, local_branches, remote_branches)
     
     return result
 
 merged = group_branches(merged)
 unmerged = group_branches(unmerged)</bpmn:script>
     </bpmn:scriptTask>
-    <bpmn:sequenceFlow id="Flow_14g5ljd" sourceRef="Activity_1n9ykr2" targetRef="Event_1ts0rz7"/>
     <bpmn:scriptTask id="Activity_1n9ykr2" name="Finalize collections">
       <bpmn:extensionElements>
         <spiffworkflow:unitTests>
           <spiffworkflow:unitTest id="happy path">
             <spiffworkflow:inputJson>{
   &quot;result&quot;: {
     &quot;returncode&quot;: 0
@@ -173,15 +205,14 @@
     &quot;returncode&quot;: 0
   }
 }</spiffworkflow:expectedOutputJson>
           </spiffworkflow:unitTest>
         </spiffworkflow:unitTests>
       </bpmn:extensionElements>
       <bpmn:incoming>Flow_0edxyrj</bpmn:incoming>
-      <bpmn:outgoing>Flow_14g5ljd</bpmn:outgoing>
       <bpmn:script>def branch_groups(branch_dict):
     local = branch_dict.get(&quot;local&quot;, [])
     remote = branch_dict.get(&quot;remote&quot;, {})
     current = branch_dict.get(&quot;current&quot;)
     local_only = list(filter(lambda b: b not in remote, local))
     has_remote_branch = list(remote.keys())
     return current, local_only, has_remote_branch
@@ -210,47 +241,222 @@
     return branches
 
 branches = build_branches()
 
 del(merged)
 del(unmerged)</bpmn:script>
     </bpmn:scriptTask>
+    <bpmn:sequenceFlow id="Flow_0c9l7wr" sourceRef="Activity_0v238ap" targetRef="Activity_1k4pxd0"/>
+    <bpmn:sequenceFlow id="Flow_1qhumuz" sourceRef="Activity_1k4pxd0" targetRef="Activity_0qmu4iv"/>
+    <bpmn:scriptTask id="Activity_1k4pxd0" name="Handle branch marker prefix">
+      <bpmn:extensionElements>
+        <spiffworkflow:unitTests>
+          <spiffworkflow:unitTest id="happy_path">
+            <spiffworkflow:inputJson>{
+  &quot;result&quot;: {
+    &quot;returncode&quot;: 0
+  },
+  &quot;current&quot;: &quot;a&quot;,
+  &quot;merged&quot;: [
+    &quot;* a&quot;,
+    &quot;  b&quot;,
+    &quot;  c&quot;
+  ],
+  &quot;remote&quot;: [
+    &quot;  g&quot;,
+    &quot;  h&quot;,
+    &quot;  i&quot;
+  ],
+  &quot;unmerged&quot;: [
+    &quot;  d&quot;,
+    &quot;  e&quot;,
+    &quot;  f&quot;
+  ]
+}</spiffworkflow:inputJson>
+            <spiffworkflow:expectedOutputJson>{
+  &quot;result&quot;: {
+    &quot;returncode&quot;: 0
+  },
+  &quot;current&quot;: &quot;a&quot;,
+  &quot;merged&quot;: [
+    &quot;b&quot;,
+    &quot;c&quot;
+  ],
+  &quot;remote&quot;: [
+    &quot;g&quot;,
+    &quot;h&quot;,
+    &quot;i&quot;
+  ],
+  &quot;unmerged&quot;: [
+    &quot;d&quot;,
+    &quot;e&quot;,
+    &quot;f&quot;
+  ]
+}</spiffworkflow:expectedOutputJson>
+          </spiffworkflow:unitTest>
+        </spiffworkflow:unitTests>
+      </bpmn:extensionElements>
+      <bpmn:incoming>Flow_0c9l7wr</bpmn:incoming>
+      <bpmn:outgoing>Flow_1qhumuz</bpmn:outgoing>
+      <bpmn:script>def branch_with_empty_prefix(branch):
+    if len(branch) &lt; 2 or branch[:2] != &quot;  &quot;:
+        return None
+    return branch[2:]
+
+def branches_with_empty_prefix(branches):
+    return list(filter(None, map(branch_with_empty_prefix, branches)))
+
+merged = branches_with_empty_prefix(merged)
+unmerged = branches_with_empty_prefix(unmerged)
+remote = branches_with_empty_prefix(remote)</bpmn:script>
+    </bpmn:scriptTask>
+    <bpmn:sequenceFlow id="Flow_1icfqqq" sourceRef="Activity_0qmu4iv" targetRef="Event_1ts0rz7"/>
+    <bpmn:scriptTask id="Activity_0qmu4iv" name="Parse remote branches">
+      <bpmn:extensionElements>
+        <spiffworkflow:unitTests>
+          <spiffworkflow:unitTest id="happy_path">
+            <spiffworkflow:inputJson>{
+  &quot;result&quot;: {
+    &quot;returncode&quot;: 0
+  },
+  &quot;current&quot;: &quot;j&quot;,
+  &quot;merged&quot;: [
+    &quot;b&quot;,
+    &quot;c&quot;
+  ],
+  &quot;remote&quot;: [
+    &quot;origin/HEAD -&gt; origin/main&quot;,
+    &quot;origin/g&quot;,
+    &quot;origin/h&quot;,
+    &quot;origin/i&quot;,
+    &quot;origin/j/k&quot;
+  ],
+  &quot;unmerged&quot;: [
+    &quot;d&quot;,
+    &quot;e&quot;,
+    &quot;f&quot;
+  ]
+}</spiffworkflow:inputJson>
+            <spiffworkflow:expectedOutputJson>{
+  &quot;result&quot;: {
+    &quot;returncode&quot;: 0
+  },
+  &quot;current&quot;: &quot;j&quot;,
+  &quot;merged&quot;: [
+    &quot;b&quot;,
+    &quot;c&quot;
+  ],
+  &quot;head&quot;: {
+    &quot;main&quot;: [
+      &quot;origin/HEAD -&gt; origin/main&quot;
+    ]
+  },
+  &quot;remote&quot;: {
+    &quot;g&quot;: [
+      &quot;origin/g&quot;
+    ],
+    &quot;h&quot;: [
+      &quot;origin/h&quot;
+    ],
+    &quot;i&quot;: [
+      &quot;origin/i&quot;
+    ],
+    &quot;j/k&quot;: [
+      &quot;origin/j/k&quot;
+    ]
+  },
+  &quot;unmerged&quot;: [
+    &quot;d&quot;,
+    &quot;e&quot;,
+    &quot;f&quot;
+  ]
+}</spiffworkflow:expectedOutputJson>
+          </spiffworkflow:unitTest>
+        </spiffworkflow:unitTests>
+      </bpmn:extensionElements>
+      <bpmn:incoming>Flow_1qhumuz</bpmn:incoming>
+      <bpmn:outgoing>Flow_1icfqqq</bpmn:outgoing>
+      <bpmn:script>def separate_heads(remote_branches):
+    head = []
+    remote = []
+    for branch in remote_branches:
+        if &quot;HEAD -&gt; &quot; in branch:
+            head.append(branch)
+        else:
+            remote.append(branch)
+    return head, remote
+
+def group_heads(head_branches):
+    head = {}
+    for branch in head_branches:
+        parts = branch.split(&quot;-&gt;&quot;)
+        branch_name = parts[1].split(&quot;/&quot;, maxsplit=1)[1]
+        if branch_name not in head:
+            head[branch_name] = []
+        head[branch_name].append(branch)
+    return head
+
+def group_remotes(remote_branches):
+    remote = {}
+    for branch in remote_branches:
+        branch_name = branch.split(&quot;/&quot;, maxsplit=1)[1]
+        if branch_name not in remote:
+            remote[branch_name] = []
+        remote[branch_name].append(branch)
+    return remote
+
+head, remote = separate_heads(remote)
+head = group_heads(head)
+remote = group_remotes(remote)</bpmn:script>
+    </bpmn:scriptTask>
   </bpmn:process>
   <bpmndi:BPMNDiagram id="BPMNDiagram_1">
     <bpmndi:BPMNPlane id="BPMNPlane_1" bpmnElement="branch_parser">
       <bpmndi:BPMNShape id="_BPMNShape_StartEvent_2" bpmnElement="StartEvent_1">
         <dc:Bounds x="179" y="159" width="36" height="36"/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Event_1ts0rz7_di" bpmnElement="Event_1ts0rz7">
-        <dc:Bounds x="672" y="159" width="36" height="36"/>
-      </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Activity_1b18f37_di" bpmnElement="Activity_0v238ap">
         <dc:Bounds x="270" y="137" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Activity_1ui38ib_di" bpmnElement="Activity_0sdmpoy">
-        <dc:Bounds x="400" y="137" width="100" height="80"/>
+        <dc:Bounds x="400" y="280" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Activity_0ag9jkv_di" bpmnElement="Activity_1n9ykr2">
+        <dc:Bounds x="530" y="280" width="100" height="80"/>
+        <bpmndi:BPMNLabel/>
+      </bpmndi:BPMNShape>
+      <bpmndi:BPMNShape id="Activity_0wzmkrf_di" bpmnElement="Activity_1k4pxd0">
+        <dc:Bounds x="400" y="137" width="100" height="80"/>
+        <bpmndi:BPMNLabel/>
+      </bpmndi:BPMNShape>
+      <bpmndi:BPMNShape id="Event_1ts0rz7_di" bpmnElement="Event_1ts0rz7">
+        <dc:Bounds x="682" y="159" width="36" height="36"/>
+      </bpmndi:BPMNShape>
+      <bpmndi:BPMNShape id="Activity_1y7rvuw_di" bpmnElement="Activity_0qmu4iv">
         <dc:Bounds x="530" y="137" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNEdge id="Flow_0zt50xr_di" bpmnElement="Flow_0zt50xr">
         <di:waypoint x="215" y="177"/>
         <di:waypoint x="270" y="177"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_1345wuj_di" bpmnElement="Flow_1345wuj">
+      <bpmndi:BPMNEdge id="Flow_0edxyrj_di" bpmnElement="Flow_0edxyrj">
+        <di:waypoint x="500" y="320"/>
+        <di:waypoint x="530" y="320"/>
+      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Flow_0c9l7wr_di" bpmnElement="Flow_0c9l7wr">
         <di:waypoint x="370" y="177"/>
         <di:waypoint x="400" y="177"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_0edxyrj_di" bpmnElement="Flow_0edxyrj">
+      <bpmndi:BPMNEdge id="Flow_1qhumuz_di" bpmnElement="Flow_1qhumuz">
         <di:waypoint x="500" y="177"/>
         <di:waypoint x="530" y="177"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_14g5ljd_di" bpmnElement="Flow_14g5ljd">
+      <bpmndi:BPMNEdge id="Flow_1icfqqq_di" bpmnElement="Flow_1icfqqq">
         <di:waypoint x="630" y="177"/>
-        <di:waypoint x="672" y="177"/>
+        <di:waypoint x="682" y="177"/>
       </bpmndi:BPMNEdge>
     </bpmndi:BPMNPlane>
   </bpmndi:BPMNDiagram>
 </bpmn:definitions>
```

### Comparing `git-debranch-0.1.3/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn` & `git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn`

 * *Files 4% similar despite different names*

#### Comparing `git-debranch-0.1.3/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn` & `git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn`

```diff
@@ -22,15 +22,19 @@
       <bpmn:incoming>Flow_1iyvi2c</bpmn:incoming>
       <bpmn:outgoing>Flow_0v4mach</bpmn:outgoing>
     </bpmn:exclusiveGateway>
     <bpmn:sequenceFlow id="Flow_0v4mach" sourceRef="Gateway_0w96sv3" targetRef="Event_1bsl2ov"/>
     <bpmn:sequenceFlow id="Flow_1iyvi2c" sourceRef="Activity_1yt24dj" targetRef="Gateway_0w96sv3"/>
     <bpmn:serviceTask id="Activity_1yt24dj" name="Delete selected branches">
       <bpmn:extensionElements>
-        <spiffworkflow:serviceTaskOperator id="git/DeleteBranches" resultVariable="result"/>
+        <spiffworkflow:serviceTaskOperator id="os/SpawnProcess" resultVariable="result">
+          <spiffworkflow:parameters>
+            <spiffworkflow:parameter id="args" type="any" value="[&quot;git&quot;, &quot;branch&quot;, &quot;-D&quot;] + branches_to_delete"/>
+          </spiffworkflow:parameters>
+        </spiffworkflow:serviceTaskOperator>
       </bpmn:extensionElements>
       <bpmn:incoming>Flow_1lxcorc</bpmn:incoming>
       <bpmn:outgoing>Flow_1iyvi2c</bpmn:outgoing>
     </bpmn:serviceTask>
   </bpmn:process>
   <bpmndi:BPMNDiagram id="BPMNDiagram_1">
     <bpmndi:BPMNPlane id="BPMNPlane_1" bpmnElement="delete_branches">
```

### Comparing `git-debranch-0.1.3/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn` & `git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn`

 * *Files 6% similar despite different names*

#### Comparing `git-debranch-0.1.3/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn` & `git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn`

```diff
@@ -8,15 +8,21 @@
     <bpmn:endEvent id="Event_185zs44">
       <bpmn:incoming>Flow_1lsziov</bpmn:incoming>
     </bpmn:endEvent>
     <bpmn:sequenceFlow id="Flow_0pqk0gt" sourceRef="Activity_1sjkjk0" targetRef="confirm_deletion"/>
     <bpmn:scriptTask id="Activity_1sjkjk0" name="Build branch report">
       <bpmn:incoming>Flow_0p7er6v</bpmn:incoming>
       <bpmn:outgoing>Flow_0pqk0gt</bpmn:outgoing>
-      <bpmn:script>def add_section(lines, section_lines, comment, header):
+      <bpmn:script>def local_only(branches):
+    return sorted(filter(lambda b: b not in head and b not in remote, branches))
+
+def has_remote(branches):
+    return sorted(filter(lambda b: b not in head and b in remote, branches))
+
+def add_section(lines, section_lines, comment, header):
     if len(section_lines) == 0:
         return
     lines.extend(header)
     lines.append(&quot;&quot;)
     if comment:
         section_lines = map(lambda l: f&quot;# {l}&quot;, section_lines)
     lines.extend(section_lines)
@@ -26,43 +32,49 @@
     lines = [
         &quot;## git debranch&quot;,
         &quot;##&quot;,
         &quot;## Select branches to delete.&quot;,
         &quot;##&quot;,
         &quot;## Any lines that are non empty and do not start with a # are assumed to &quot;,
         &quot;## be branch names, one per line. Each uncommented branch name will be &quot;,
-        &quot;## marked for deletion.&quot;,
+        &quot;## marked for deletion. HEAD and current branches are not shown.&quot;,
         &quot;&quot;,
     ]
 
-    add_section(lines, branches[&quot;merged_local_only&quot;], False, [
+    merged_local_only = local_only(merged)
+
+    add_section(lines, merged_local_only, False, [
         &quot;## The following branches appear safe to delete. They exist locally &quot;,
         &quot;## but not on any remote and have been merged:&quot;,
     ])
 
-    add_section(lines, branches[&quot;merged_has_remote_branch&quot;], True, [
-        &quot;## The following branches exist locally as well as on a remote and &quot;,
-        &quot;## have been merged:&quot;,
-    ])
+    unmerged_local_only = local_only(unmerged)
 
-    add_section(lines, branches[&quot;unmerged_local_only&quot;], True, [
+    add_section(lines, unmerged_local_only, True, [
         &quot;## The following branches only exist locally but not may not have &quot;, 
         &quot;## been merged:&quot;,
     ])
 
-    add_section(lines, branches[&quot;unmerged_has_remote_branch&quot;], True, [
+    merged_has_remote_branch = has_remote(merged)
+
+    add_section(lines, merged_has_remote_branch, True, [
+        &quot;## The following branches exist locally as well as on a remote and &quot;,
+        &quot;## have been merged:&quot;,
+    ])
+
+    unmerged_has_remote_branch = has_remote(unmerged)
+
+    add_section(lines, unmerged_has_remote_branch, True, [
         &quot;## The following branches exist locally as well as on a remote and &quot;,
         &quot;## may not have been merged:&quot;,
     ])
 
     return &quot;\n&quot;.join(lines)
 
-branch_report = build_branch_report()
-
-del(branches)</bpmn:script>
+branch_report = build_branch_report()</bpmn:script>
     </bpmn:scriptTask>
     <bpmn:sequenceFlow id="Flow_0povx4i" sourceRef="confirm_deletion" targetRef="Activity_0a61ymz"/>
     <bpmn:userTask id="confirm_deletion" name="Prompt for confirmation">
       <bpmn:incoming>Flow_0pqk0gt</bpmn:incoming>
       <bpmn:outgoing>Flow_0povx4i</bpmn:outgoing>
     </bpmn:userTask>
     <bpmn:sequenceFlow id="Flow_1lsziov" sourceRef="Activity_0a61ymz" targetRef="Event_185zs44"/>
```

### Comparing `git-debranch-0.1.3/src/git_debranch/bpmn/git-debranch/git-debranch.bpmn` & `git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/spawn.bpmn`

 * *Files 22% similar despite different names*

#### Comparing `git-debranch-0.1.3/src/git_debranch/bpmn/git-debranch/git-debranch.bpmn` & `git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/spawn.bpmn`

```diff
@@ -1,128 +1,86 @@
 <?xml version="1.0" encoding="utf-8"?>
-<bpmn:definitions xmlns:bpmn="http://www.omg.org/spec/BPMN/20100524/MODEL" xmlns:bpmndi="http://www.omg.org/spec/BPMN/20100524/DI" xmlns:dc="http://www.omg.org/spec/DD/20100524/DC" xmlns:di="http://www.omg.org/spec/DD/20100524/DI" id="Definitions_96f6665" targetNamespace="http://bpmn.io/schema/bpmn" exporter="Camunda Modeler" exporterVersion="3.0.0-dev">
-  <bpmn:process id="git-debranch" name="Git Debranch" isExecutable="true">
+<bpmn:definitions xmlns:bpmn="http://www.omg.org/spec/BPMN/20100524/MODEL" xmlns:bpmndi="http://www.omg.org/spec/BPMN/20100524/DI" xmlns:dc="http://www.omg.org/spec/DD/20100524/DC" xmlns:spiffworkflow="http://spiffworkflow.org/bpmn/schema/1.0/core" xmlns:di="http://www.omg.org/spec/DD/20100524/DI" id="Definitions_96f6665" targetNamespace="http://bpmn.io/schema/bpmn" exporter="Camunda Modeler" exporterVersion="3.0.0-dev">
+  <bpmn:process id="spawn_process" name="Spawn a New Process" isExecutable="true">
     <bpmn:startEvent id="StartEvent_1">
-      <bpmn:outgoing>Flow_13piout</bpmn:outgoing>
+      <bpmn:outgoing>Flow_090xnqj</bpmn:outgoing>
     </bpmn:startEvent>
-    <bpmn:endEvent id="Event_1wlwe0w">
-      <bpmn:incoming>Flow_1uy858t</bpmn:incoming>
-    </bpmn:endEvent>
-    <bpmn:exclusiveGateway id="Gateway_1p0jed3" default="Flow_11swttm">
-      <bpmn:incoming>Flow_1b4tqmf</bpmn:incoming>
-      <bpmn:outgoing>Flow_1rwpp5i</bpmn:outgoing>
-      <bpmn:outgoing>Flow_11swttm</bpmn:outgoing>
+    <bpmn:sequenceFlow id="Flow_090xnqj" sourceRef="StartEvent_1" targetRef="Activity_1wobbp0"/>
+    <bpmn:exclusiveGateway id="Gateway_0o5auw6" default="Flow_1gimdqy">
+      <bpmn:incoming>Flow_1cl2vgj</bpmn:incoming>
+      <bpmn:outgoing>Flow_1gimdqy</bpmn:outgoing>
+      <bpmn:outgoing>Flow_1msh4mr</bpmn:outgoing>
     </bpmn:exclusiveGateway>
-    <bpmn:endEvent id="Event_132ve90">
-      <bpmn:incoming>Flow_1rwpp5i</bpmn:incoming>
+    <bpmn:sequenceFlow id="Flow_1cl2vgj" sourceRef="Activity_1wobbp0" targetRef="Gateway_0o5auw6"/>
+    <bpmn:endEvent id="Event_1vc03l8">
+      <bpmn:incoming>Flow_1gimdqy</bpmn:incoming>
     </bpmn:endEvent>
-    <bpmn:sequenceFlow id="Flow_1rwpp5i" sourceRef="Gateway_1p0jed3" targetRef="Event_132ve90">
+    <bpmn:sequenceFlow id="Flow_1gimdqy" sourceRef="Gateway_0o5auw6" targetRef="Event_1vc03l8"/>
+    <bpmn:sequenceFlow id="Flow_1msh4mr" sourceRef="Gateway_0o5auw6" targetRef="Event_08pdzal">
       <bpmn:conditionExpression>result[&quot;returncode&quot;] != 0</bpmn:conditionExpression>
     </bpmn:sequenceFlow>
-    <bpmn:sequenceFlow id="Flow_11swttm" sourceRef="Gateway_1p0jed3" targetRef="Activity_0k872kx"/>
-    <bpmn:sequenceFlow id="Flow_1b4tqmf" sourceRef="Activity_19gnuol" targetRef="Gateway_1p0jed3"/>
-    <bpmn:callActivity id="Activity_19gnuol" name="Find all branches" calledElement="get_all_branches">
-      <bpmn:incoming>Flow_13piout</bpmn:incoming>
-      <bpmn:outgoing>Flow_1b4tqmf</bpmn:outgoing>
-    </bpmn:callActivity>
-    <bpmn:sequenceFlow id="Flow_13piout" sourceRef="StartEvent_1" targetRef="Activity_19gnuol"/>
-    <bpmn:sequenceFlow id="Flow_1026mcr" sourceRef="Activity_0k872kx" targetRef="Activity_10dkgjv"/>
-    <bpmn:callActivity id="Activity_0k872kx" name="Parse branches" calledElement="branch_parser">
-      <bpmn:incoming>Flow_11swttm</bpmn:incoming>
-      <bpmn:outgoing>Flow_1026mcr</bpmn:outgoing>
-    </bpmn:callActivity>
-    <bpmn:sequenceFlow id="Flow_1ikchnf" sourceRef="Activity_10dkgjv" targetRef="Activity_1h49w3b"/>
-    <bpmn:callActivity id="Activity_10dkgjv" name="Prompt for branches to delete" calledElement="deletion_prompt">
-      <bpmn:incoming>Flow_1026mcr</bpmn:incoming>
-      <bpmn:outgoing>Flow_1ikchnf</bpmn:outgoing>
-    </bpmn:callActivity>
-    <bpmn:sequenceFlow id="Flow_1uy858t" sourceRef="Activity_1h49w3b" targetRef="Event_1wlwe0w"/>
-    <bpmn:callActivity id="Activity_1h49w3b" name="Delete branches" calledElement="delete_branches">
-      <bpmn:incoming>Flow_1ikchnf</bpmn:incoming>
-      <bpmn:outgoing>Flow_1uy858t</bpmn:outgoing>
-    </bpmn:callActivity>
-    <bpmn:textAnnotation id="TextAnnotation_1b3js8g">
-      <bpmn:text>git operation was not successful, best to bail now</bpmn:text>
-    </bpmn:textAnnotation>
-    <bpmn:association id="Association_0h4hzko" sourceRef="Flow_1rwpp5i" targetRef="TextAnnotation_1b3js8g"/>
-    <bpmn:textAnnotation id="TextAnnotation_02uv528">
-      <bpmn:text>TODO: is there a way to make the subprocess terminate the process? This would be cleaner at the top level</bpmn:text>
+    <bpmn:endEvent id="Event_08pdzal">
+      <bpmn:incoming>Flow_1msh4mr</bpmn:incoming>
+      <bpmn:terminateEventDefinition id="TerminateEventDefinition_16l45dq"/>
+    </bpmn:endEvent>
+    <bpmn:serviceTask id="Activity_1wobbp0" name="Spawn a process">
+      <bpmn:extensionElements>
+        <spiffworkflow:serviceTaskOperator id="os/SpawnProcess" resultVariable="result">
+          <spiffworkflow:parameters>
+            <spiffworkflow:parameter id="args" type="any" value="spawn_args"/>
+          </spiffworkflow:parameters>
+        </spiffworkflow:serviceTaskOperator>
+      </bpmn:extensionElements>
+      <bpmn:incoming>Flow_090xnqj</bpmn:incoming>
+      <bpmn:outgoing>Flow_1cl2vgj</bpmn:outgoing>
+    </bpmn:serviceTask>
+    <bpmn:textAnnotation id="TextAnnotation_0kuplex">
+      <bpmn:text>This behaves like spawn+unwrap. Maybe rename if reusing or make spawn_unwrap.bpmn</bpmn:text>
     </bpmn:textAnnotation>
-    <bpmn:association id="Association_1ykz79g" sourceRef="Flow_1rwpp5i" targetRef="TextAnnotation_02uv528"/>
+    <bpmn:association id="Association_06bmaew" sourceRef="Gateway_0o5auw6" targetRef="TextAnnotation_0kuplex"/>
   </bpmn:process>
   <bpmndi:BPMNDiagram id="BPMNDiagram_1">
-    <bpmndi:BPMNPlane id="BPMNPlane_1" bpmnElement="git-debranch">
+    <bpmndi:BPMNPlane id="BPMNPlane_1" bpmnElement="spawn_process">
       <bpmndi:BPMNShape id="_BPMNShape_StartEvent_2" bpmnElement="StartEvent_1">
-        <dc:Bounds x="382" y="162" width="36" height="36"/>
-      </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="BPMNShape_0z9jlas" bpmnElement="Gateway_1p0jed3" isMarkerVisible="true">
-        <dc:Bounds x="625" y="152" width="50" height="50"/>
+        <dc:Bounds x="179" y="159" width="36" height="36"/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="BPMNShape_0pzmt8d" bpmnElement="Event_132ve90">
-        <dc:Bounds x="632" y="32" width="36" height="36"/>
+      <bpmndi:BPMNShape id="Gateway_0o5auw6_di" bpmnElement="Gateway_0o5auw6" isMarkerVisible="true">
+        <dc:Bounds x="425" y="152" width="50" height="50"/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Activity_0sh6juq_di" bpmnElement="Activity_19gnuol">
-        <dc:Bounds x="480" y="137" width="100" height="80"/>
-        <bpmndi:BPMNLabel/>
-      </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Activity_0f41p31_di" bpmnElement="Activity_0k872kx">
-        <dc:Bounds x="740" y="137" width="100" height="80"/>
-        <bpmndi:BPMNLabel/>
+      <bpmndi:BPMNShape id="Event_1vc03l8_di" bpmnElement="Event_1vc03l8">
+        <dc:Bounds x="532" y="159" width="36" height="36"/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Activity_1gy062s_di" bpmnElement="Activity_10dkgjv">
-        <dc:Bounds x="880" y="137" width="100" height="80"/>
-        <bpmndi:BPMNLabel/>
+      <bpmndi:BPMNShape id="Event_1vzcyjv_di" bpmnElement="Event_08pdzal">
+        <dc:Bounds x="532" y="272" width="36" height="36"/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="BPMNShape_01l9klp" bpmnElement="TextAnnotation_1b3js8g">
-        <dc:Bounds x="720" y="30" width="100" height="70"/>
+      <bpmndi:BPMNShape id="Activity_1qk1mwi_di" bpmnElement="Activity_1wobbp0">
+        <dc:Bounds x="270" y="137" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="TextAnnotation_02uv528_di" bpmnElement="TextAnnotation_02uv528">
-        <dc:Bounds x="480" y="-30" width="100" height="127"/>
+      <bpmndi:BPMNShape id="TextAnnotation_0kuplex_di" bpmnElement="TextAnnotation_0kuplex">
+        <dc:Bounds x="480" y="-20" width="100" height="127"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Event_1wlwe0w_di" bpmnElement="Event_1wlwe0w">
-        <dc:Bounds x="1152" y="159" width="36" height="36"/>
-      </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Activity_0tq5gom_di" bpmnElement="Activity_1h49w3b">
-        <dc:Bounds x="1020" y="137" width="100" height="80"/>
-        <bpmndi:BPMNLabel/>
-      </bpmndi:BPMNShape>
-      <bpmndi:BPMNEdge id="BPMNEdge_0xjlr6e" bpmnElement="Flow_1rwpp5i">
-        <di:waypoint x="650" y="152"/>
-        <di:waypoint x="650" y="68"/>
-      </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_11swttm_di" bpmnElement="Flow_11swttm">
-        <di:waypoint x="675" y="177"/>
-        <di:waypoint x="740" y="177"/>
-      </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_1b4tqmf_di" bpmnElement="Flow_1b4tqmf">
-        <di:waypoint x="580" y="177"/>
-        <di:waypoint x="625" y="177"/>
-      </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_13piout_di" bpmnElement="Flow_13piout">
-        <di:waypoint x="418" y="180"/>
-        <di:waypoint x="480" y="180"/>
-      </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_1026mcr_di" bpmnElement="Flow_1026mcr">
-        <di:waypoint x="840" y="177"/>
-        <di:waypoint x="880" y="177"/>
+      <bpmndi:BPMNEdge id="Flow_090xnqj_di" bpmnElement="Flow_090xnqj">
+        <di:waypoint x="215" y="177"/>
+        <di:waypoint x="270" y="177"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_1ikchnf_di" bpmnElement="Flow_1ikchnf">
-        <di:waypoint x="980" y="177"/>
-        <di:waypoint x="1020" y="177"/>
+      <bpmndi:BPMNEdge id="Flow_1cl2vgj_di" bpmnElement="Flow_1cl2vgj">
+        <di:waypoint x="370" y="177"/>
+        <di:waypoint x="425" y="177"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="BPMNEdge_03yfwrz" bpmnElement="Association_0h4hzko">
-        <di:waypoint x="650" y="110"/>
-        <di:waypoint x="720" y="78"/>
+      <bpmndi:BPMNEdge id="Flow_1gimdqy_di" bpmnElement="Flow_1gimdqy">
+        <di:waypoint x="475" y="177"/>
+        <di:waypoint x="532" y="177"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Association_1ykz79g_di" bpmnElement="Association_1ykz79g">
-        <di:waypoint x="650" y="110"/>
-        <di:waypoint x="580" y="37"/>
+      <bpmndi:BPMNEdge id="Flow_1msh4mr_di" bpmnElement="Flow_1msh4mr">
+        <di:waypoint x="450" y="202"/>
+        <di:waypoint x="450" y="290"/>
+        <di:waypoint x="532" y="290"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_1uy858t_di" bpmnElement="Flow_1uy858t">
-        <di:waypoint x="1120" y="177"/>
-        <di:waypoint x="1152" y="177"/>
+      <bpmndi:BPMNEdge id="Association_06bmaew_di" bpmnElement="Association_06bmaew">
+        <di:waypoint x="458" y="160"/>
+        <di:waypoint x="480" y="107"/>
       </bpmndi:BPMNEdge>
     </bpmndi:BPMNPlane>
   </bpmndi:BPMNDiagram>
 </bpmn:definitions>
```

### Comparing `git-debranch-0.1.3/src/git_debranch/loader.py` & `git-debranch-0.1.4/src/git_debranch/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 def _bpmn_data_paths():
     bpmn_filenames = [
         "git-debranch.bpmn",
         "all_branches.bpmn",
         "branch_parser.bpmn",
         "deletion_prompt.bpmn",
         "delete_branches.bpmn",
+        "spawn.bpmn",
     ]
     return map(_bpmn_data_path, bpmn_filenames)
 
 def _get_data_str(data_path):
     return pkgutil.get_data("git_debranch", data_path).decode("utf-8")
 
 def _bpmn_strs():
```

### Comparing `git-debranch-0.1.3/src/git_debranch/runner.py` & `git-debranch-0.1.4/src/git_debranch/runner.py`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.3/src/git_debranch/workflow.py` & `git-debranch-0.1.4/src/git_debranch/workflow.py`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.3/src/git_debranch.egg-info/PKG-INFO` & `git-debranch-0.1.4/src/git_debranch.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-debranch
-Version: 0.1.3
+Version: 0.1.4
 Summary: Remove git branches
 Author: Jon Herron
 Author-email: jon.herron@yahoo.com
 License: lGPLv2
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -55,21 +55,17 @@
 
 You likely want to be inside a venv. This wlll give you an editable installation so you can run the program 
 and see changes. If you add a new bpmn/json file then you need to re-run this command.
 
 ### Using SpiffArena for BPMN edits
 
 [SpiffArena](https://github.com/sartography/spiff-arena) is used to make edits to the BPMN files that are 
-bundled with this program. Currently it is assumed that you have a working copy, possibly from the 
-[Getting Started Guide](https://www.spiffworkflow.org/posts/articles/get_started/). When using SpiffArena as 
-the editor you need to set the following environment variable:
-
-```
-SPIFFWORKFLOW_BACKEND_BPMN_SPEC_ABSOLUTE_DIR
-```
-
-to point to `src/git_debranch` inside this repository. If using docker, the volume that is used for the 
-process models will need to be updated to point to this location.
+bundled with this program. To start the editor run `make run-editor`. You will be presented with a message
+once started to go to `http://localhost:8001` (assuming the default configuration is used). The editor
+requires `docker` and `docker compose` to run.
 
 From there you can edit the diagrams but you cannot run them from within SpiffArena at this time. Some work 
 would need to be done to support our custom `Connector Proxy` that is not http based. You can however run 
 the `Script Task` unit tests, which were very helpful during development.
+
+When finished you can `make stop-editor`. If you would like to pull the latest version of SpiffArena use
+`make update-editor`.
```

### Comparing `git-debranch-0.1.3/src/git_debranch.egg-info/SOURCES.txt` & `git-debranch-0.1.4/src/git_debranch.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 src/git_debranch/runner.py
 src/git_debranch/script_engine.py
 src/git_debranch/workflow.py
 src/git_debranch.egg-info/PKG-INFO
 src/git_debranch.egg-info/SOURCES.txt
 src/git_debranch.egg-info/dependency_links.txt
 src/git_debranch.egg-info/entry_points.txt
+src/git_debranch.egg-info/requires.txt
 src/git_debranch.egg-info/top_level.txt
 src/git_debranch/bpmn/process_group.json
 src/git_debranch/bpmn/git-debranch/all_branches.bpmn
 src/git_debranch/bpmn/git-debranch/branch_parser.bpmn
 src/git_debranch/bpmn/git-debranch/confirm_deletion.json
 src/git_debranch/bpmn/git-debranch/delete_branches.bpmn
 src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn
 src/git_debranch/bpmn/git-debranch/git-debranch.bpmn
-src/git_debranch/bpmn/git-debranch/process_model.json
+src/git_debranch/bpmn/git-debranch/process_model.json
+src/git_debranch/bpmn/git-debranch/spawn.bpmn
```

