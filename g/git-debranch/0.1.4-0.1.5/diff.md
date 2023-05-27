# Comparing `tmp/git-debranch-0.1.4.tar.gz` & `tmp/git-debranch-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-debranch-0.1.4.tar", last modified: Fri May 26 17:55:27 2023, max compression
+gzip compressed data, was "git-debranch-0.1.5.tar", last modified: Sat May 27 12:59:01 2023, max compression
```

## Comparing `git-debranch-0.1.4.tar` & `git-debranch-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:55:27.119764 git-debranch-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-26 17:55:18.000000 git-debranch-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-26 17:55:27.119764 git-debranch-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-26 17:55:18.000000 git-debranch-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 17:55:27.119764 git-debranch-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-26 17:55:18.000000 git-debranch-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:55:27.111765 git-debranch-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:55:27.115764 git-debranch-0.1.4/src/git_debranch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:55:27.119764 git-debranch-0.1.4/src/git_debranch/bpmn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:55:27.119764 git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/
--rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/all_branches.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/branch_parser.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/confirm_deletion.json
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/git-debranch.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/process_model.json
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/spawn.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/bpmn/process_group.json
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/console_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/script_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-26 17:55:18.000000 git-debranch-0.1.4/src/git_debranch/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:55:27.119764 git-debranch-0.1.4/src/git_debranch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-26 17:55:27.000000 git-debranch-0.1.4/src/git_debranch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-26 17:55:27.000000 git-debranch-0.1.4/src/git_debranch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 17:55:27.000000 git-debranch-0.1.4/src/git_debranch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-26 17:55:27.000000 git-debranch-0.1.4/src/git_debranch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-26 17:55:27.000000 git-debranch-0.1.4/src/git_debranch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 17:55:27.000000 git-debranch-0.1.4/src/git_debranch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:59:01.539928 git-debranch-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-27 12:58:51.000000 git-debranch-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-27 12:59:01.539928 git-debranch-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-27 12:58:51.000000 git-debranch-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 12:59:01.539928 git-debranch-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-27 12:58:51.000000 git-debranch-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:59:01.535928 git-debranch-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:59:01.535928 git-debranch-0.1.5/src/git_debranch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:59:01.539928 git-debranch-0.1.5/src/git_debranch/bpmn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:59:01.539928 git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/
+-rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/all_branches.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/branch_parser.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/confirm_deletion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/git-debranch.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/process_model.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/spawn.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/bpmn/process_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/console_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/script_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:59:01.539928 git-debranch-0.1.5/src/git_debranch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-27 12:59:01.000000 git-debranch-0.1.5/src/git_debranch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-27 12:59:01.000000 git-debranch-0.1.5/src/git_debranch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 12:59:01.000000 git-debranch-0.1.5/src/git_debranch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-27 12:59:01.000000 git-debranch-0.1.5/src/git_debranch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-27 12:59:01.000000 git-debranch-0.1.5/src/git_debranch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-27 12:59:01.000000 git-debranch-0.1.5/src/git_debranch.egg-info/top_level.txt
```

### Comparing `git-debranch-0.1.4/LICENSE` & `git-debranch-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.4/PKG-INFO` & `git-debranch-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-debranch
-Version: 0.1.4
+Version: 0.1.5
 Summary: Remove git branches
 Author: Jon Herron
 Author-email: jon.herron@yahoo.com
 License: lGPLv2
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,17 +15,14 @@
 
 ## Installation
 
 ```
 pip install git-debranch
 ```
 
-_Note: This is currently blocked on an upcoming release of SpiffWorkflow. Once resolved this will work.
-For now you need to clone the repo and do a local install: pip install -r requirements.txt_
-
 ## Usage
 
 ```
 git debranch
 ```
 
 From inside a git repository, running `git debranch` will present you with a list of branches that could
```

### Comparing `git-debranch-0.1.4/README.md` & `git-debranch-0.1.5/src/git_debranch.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,28 @@
+Metadata-Version: 2.1
+Name: git-debranch
+Version: 0.1.5
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
 pip install git-debranch
 ```
 
-_Note: This is currently blocked on an upcoming release of SpiffWorkflow. Once resolved this will work.
-For now you need to clone the repo and do a local install: pip install -r requirements.txt_
-
 ## Usage
 
 ```
 git debranch
 ```
 
 From inside a git repository, running `git debranch` will present you with a list of branches that could
```

### Comparing `git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/all_branches.bpmn` & `git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/all_branches.bpmn`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn` & `git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn` & `git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/branch_parser.bpmn`

 * *Files 27% similar despite different names*

#### Comparing `git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn` & `git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/branch_parser.bpmn`

```diff
@@ -1,160 +1,262 @@
 <?xml version="1.0" encoding="utf-8"?>
 <bpmn:definitions xmlns:bpmn="http://www.omg.org/spec/BPMN/20100524/MODEL" xmlns:bpmndi="http://www.omg.org/spec/BPMN/20100524/DI" xmlns:dc="http://www.omg.org/spec/DD/20100524/DC" xmlns:di="http://www.omg.org/spec/DD/20100524/DI" xmlns:spiffworkflow="http://spiffworkflow.org/bpmn/schema/1.0/core" id="Definitions_96f6665" targetNamespace="http://bpmn.io/schema/bpmn" exporter="Camunda Modeler" exporterVersion="3.0.0-dev">
-  <bpmn:process id="deletion_prompt" name="Deletion Prompt" isExecutable="true">
+  <bpmn:process id="branch_parser" name="Branch parser" isExecutable="true">
     <bpmn:startEvent id="StartEvent_1">
-      <bpmn:outgoing>Flow_0p7er6v</bpmn:outgoing>
+      <bpmn:outgoing>Flow_0zt50xr</bpmn:outgoing>
     </bpmn:startEvent>
-    <bpmn:sequenceFlow id="Flow_0p7er6v" sourceRef="StartEvent_1" targetRef="Activity_1sjkjk0"/>
-    <bpmn:endEvent id="Event_185zs44">
-      <bpmn:incoming>Flow_1lsziov</bpmn:incoming>
+    <bpmn:sequenceFlow id="Flow_0zt50xr" sourceRef="StartEvent_1" targetRef="Activity_0v238ap"/>
+    <bpmn:endEvent id="Event_1ts0rz7">
+      <bpmn:incoming>Flow_1icfqqq</bpmn:incoming>
     </bpmn:endEvent>
-    <bpmn:sequenceFlow id="Flow_0pqk0gt" sourceRef="Activity_1sjkjk0" targetRef="confirm_deletion"/>
-    <bpmn:scriptTask id="Activity_1sjkjk0" name="Build branch report">
-      <bpmn:incoming>Flow_0p7er6v</bpmn:incoming>
-      <bpmn:outgoing>Flow_0pqk0gt</bpmn:outgoing>
-      <bpmn:script>def local_only(branches):
-    return sorted(filter(lambda b: b not in head and b not in remote, branches))
-
-def has_remote(branches):
-    return sorted(filter(lambda b: b not in head and b in remote, branches))
-
-def add_section(lines, section_lines, comment, header):
-    if len(section_lines) == 0:
-        return
-    lines.extend(header)
-    lines.append(&quot;&quot;)
-    if comment:
-        section_lines = map(lambda l: f&quot;# {l}&quot;, section_lines)
-    lines.extend(section_lines)
-    lines.append(&quot;&quot;)
-
-def build_branch_report():
-    lines = [
-        &quot;## git debranch&quot;,
-        &quot;##&quot;,
-        &quot;## Select branches to delete.&quot;,
-        &quot;##&quot;,
-        &quot;## Any lines that are non empty and do not start with a # are assumed to &quot;,
-        &quot;## be branch names, one per line. Each uncommented branch name will be &quot;,
-        &quot;## marked for deletion. HEAD and current branches are not shown.&quot;,
-        &quot;&quot;,
-    ]
-
-    merged_local_only = local_only(merged)
-
-    add_section(lines, merged_local_only, False, [
-        &quot;## The following branches appear safe to delete. They exist locally &quot;,
-        &quot;## but not on any remote and have been merged:&quot;,
-    ])
-
-    unmerged_local_only = local_only(unmerged)
-
-    add_section(lines, unmerged_local_only, True, [
-        &quot;## The following branches only exist locally but not may not have &quot;, 
-        &quot;## been merged:&quot;,
-    ])
-
-    merged_has_remote_branch = has_remote(merged)
-
-    add_section(lines, merged_has_remote_branch, True, [
-        &quot;## The following branches exist locally as well as on a remote and &quot;,
-        &quot;## have been merged:&quot;,
-    ])
-
-    unmerged_has_remote_branch = has_remote(unmerged)
-
-    add_section(lines, unmerged_has_remote_branch, True, [
-        &quot;## The following branches exist locally as well as on a remote and &quot;,
-        &quot;## may not have been merged:&quot;,
-    ])
-
-    return &quot;\n&quot;.join(lines)
-
-branch_report = build_branch_report()</bpmn:script>
-    </bpmn:scriptTask>
-    <bpmn:sequenceFlow id="Flow_0povx4i" sourceRef="confirm_deletion" targetRef="Activity_0a61ymz"/>
-    <bpmn:userTask id="confirm_deletion" name="Prompt for confirmation">
-      <bpmn:incoming>Flow_0pqk0gt</bpmn:incoming>
-      <bpmn:outgoing>Flow_0povx4i</bpmn:outgoing>
-    </bpmn:userTask>
-    <bpmn:sequenceFlow id="Flow_1lsziov" sourceRef="Activity_0a61ymz" targetRef="Event_185zs44"/>
-    <bpmn:scriptTask id="Activity_0a61ymz" name="Parse user response">
+    <bpmn:scriptTask id="Activity_0v238ap" name="Parse branch strings">
       <bpmn:extensionElements>
         <spiffworkflow:unitTests>
           <spiffworkflow:unitTest id="happy_path">
             <spiffworkflow:inputJson>{
-    &quot;branch_report&quot;: &quot;# some comment\nbranch1\n\n\n# not-this-branch\nbranch2&quot;
+  &quot;result&quot;: {
+    &quot;returncode&quot;: 0
+  },
+  &quot;current&quot;: &quot;j\n&quot;,
+  &quot;merged&quot;: &quot; a\n b\n c\n\n&quot;,
+  &quot;remote&quot;: &quot; g\n h\n i\n\n&quot;,
+  &quot;unmerged&quot;: &quot; d\n e\n f\n\n&quot;
 }</spiffworkflow:inputJson>
             <spiffworkflow:expectedOutputJson>{
-    &quot;branches_to_delete&quot;: [&quot;branch1&quot;, &quot;branch2&quot;]
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
 }</spiffworkflow:expectedOutputJson>
           </spiffworkflow:unitTest>
-          <spiffworkflow:unitTest id="strips_names">
+        </spiffworkflow:unitTests>
+      </bpmn:extensionElements>
+      <bpmn:incoming>Flow_0zt50xr</bpmn:incoming>
+      <bpmn:outgoing>Flow_0c9l7wr</bpmn:outgoing>
+      <bpmn:script>def to_list(branches):
+    parts = branches.split(&quot;\n&quot;)
+    non_empty_parts = filter(len, parts)
+    return list(non_empty_parts)
+
+merged = to_list(merged)
+unmerged = to_list(unmerged)
+remote = to_list(remote)
+current = current.strip()</bpmn:script>
+    </bpmn:scriptTask>
+    <bpmn:sequenceFlow id="Flow_0c9l7wr" sourceRef="Activity_0v238ap" targetRef="Activity_1k4pxd0"/>
+    <bpmn:sequenceFlow id="Flow_1qhumuz" sourceRef="Activity_1k4pxd0" targetRef="Activity_0qmu4iv"/>
+    <bpmn:scriptTask id="Activity_1k4pxd0" name="Handle branch marker prefix">
+      <bpmn:extensionElements>
+        <spiffworkflow:unitTests>
+          <spiffworkflow:unitTest id="happy_path">
             <spiffworkflow:inputJson>{
-  &quot;branch_report&quot;: &quot;# some comment\n branch1\n\n\n# not-this-branch\n   branch2   &quot;
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
 }</spiffworkflow:inputJson>
             <spiffworkflow:expectedOutputJson>{
-  &quot;branches_to_delete&quot;: [
-    &quot;branch1&quot;,
-    &quot;branch2&quot;
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
   ]
 }</spiffworkflow:expectedOutputJson>
           </spiffworkflow:unitTest>
         </spiffworkflow:unitTests>
       </bpmn:extensionElements>
-      <bpmn:incoming>Flow_0povx4i</bpmn:incoming>
-      <bpmn:outgoing>Flow_1lsziov</bpmn:outgoing>
-      <bpmn:script>def branch_line(line):
-    line = line.strip()
-    if len(line) == 0 or line.startswith(&quot;#&quot;):
+      <bpmn:incoming>Flow_0c9l7wr</bpmn:incoming>
+      <bpmn:outgoing>Flow_1qhumuz</bpmn:outgoing>
+      <bpmn:script>def branch_with_empty_prefix(branch):
+    if len(branch) &lt; 2 or branch[:2] != &quot;  &quot;:
         return None
-    return line
-
-def user_confirmed_branches():
-    lines = branch_report.split(&quot;\n&quot;)
-    return list(filter(None, map(branch_line, lines)))
+    return branch[2:]
 
-branches_to_delete = user_confirmed_branches()
+def branches_with_empty_prefix(branches):
+    return list(filter(None, map(branch_with_empty_prefix, branches)))
 
-del(branch_report)</bpmn:script>
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
     </bpmn:scriptTask>
   </bpmn:process>
   <bpmndi:BPMNDiagram id="BPMNDiagram_1">
-    <bpmndi:BPMNPlane id="BPMNPlane_1" bpmnElement="deletion_prompt">
+    <bpmndi:BPMNPlane id="BPMNPlane_1" bpmnElement="branch_parser">
       <bpmndi:BPMNShape id="_BPMNShape_StartEvent_2" bpmnElement="StartEvent_1">
         <dc:Bounds x="179" y="159" width="36" height="36"/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Event_185zs44_di" bpmnElement="Event_185zs44">
-        <dc:Bounds x="692" y="159" width="36" height="36"/>
+      <bpmndi:BPMNShape id="Event_1ts0rz7_di" bpmnElement="Event_1ts0rz7">
+        <dc:Bounds x="682" y="159" width="36" height="36"/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Activity_0wzugcm_di" bpmnElement="Activity_1sjkjk0">
+      <bpmndi:BPMNShape id="Activity_1b18f37_di" bpmnElement="Activity_0v238ap">
         <dc:Bounds x="270" y="137" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Activity_18aapsf_di" bpmnElement="confirm_deletion">
+      <bpmndi:BPMNShape id="Activity_0wzmkrf_di" bpmnElement="Activity_1k4pxd0">
         <dc:Bounds x="400" y="137" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Activity_14dv693_di" bpmnElement="Activity_0a61ymz">
+      <bpmndi:BPMNShape id="Activity_1y7rvuw_di" bpmnElement="Activity_0qmu4iv">
         <dc:Bounds x="530" y="137" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNEdge id="Flow_0p7er6v_di" bpmnElement="Flow_0p7er6v">
+      <bpmndi:BPMNEdge id="Flow_0zt50xr_di" bpmnElement="Flow_0zt50xr">
         <di:waypoint x="215" y="177"/>
         <di:waypoint x="270" y="177"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_0pqk0gt_di" bpmnElement="Flow_0pqk0gt">
+      <bpmndi:BPMNEdge id="Flow_0c9l7wr_di" bpmnElement="Flow_0c9l7wr">
         <di:waypoint x="370" y="177"/>
         <di:waypoint x="400" y="177"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_0povx4i_di" bpmnElement="Flow_0povx4i">
+      <bpmndi:BPMNEdge id="Flow_1qhumuz_di" bpmnElement="Flow_1qhumuz">
         <di:waypoint x="500" y="177"/>
         <di:waypoint x="530" y="177"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_1lsziov_di" bpmnElement="Flow_1lsziov">
+      <bpmndi:BPMNEdge id="Flow_1icfqqq_di" bpmnElement="Flow_1icfqqq">
         <di:waypoint x="630" y="177"/>
-        <di:waypoint x="692" y="177"/>
+        <di:waypoint x="682" y="177"/>
       </bpmndi:BPMNEdge>
     </bpmndi:BPMNPlane>
   </bpmndi:BPMNDiagram>
 </bpmn:definitions>
```

### Comparing `git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/git-debranch.bpmn` & `git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/git-debranch.bpmn`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.4/src/git_debranch/bpmn/git-debranch/spawn.bpmn` & `git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/spawn.bpmn`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.4/src/git_debranch/loader.py` & `git-debranch-0.1.5/src/git_debranch/loader.py`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.4/src/git_debranch/runner.py` & `git-debranch-0.1.5/src/git_debranch/runner.py`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.4/src/git_debranch/script_engine.py` & `git-debranch-0.1.5/src/git_debranch/script_engine.py`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.4/src/git_debranch/workflow.py` & `git-debranch-0.1.5/src/git_debranch/workflow.py`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.4/src/git_debranch.egg-info/PKG-INFO` & `git-debranch-0.1.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,17 @@
-Metadata-Version: 2.1
-Name: git-debranch
-Version: 0.1.4
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
 pip install git-debranch
 ```
 
-_Note: This is currently blocked on an upcoming release of SpiffWorkflow. Once resolved this will work.
-For now you need to clone the repo and do a local install: pip install -r requirements.txt_
-
 ## Usage
 
 ```
 git debranch
 ```
 
 From inside a git repository, running `git debranch` will present you with a list of branches that could
```

### Comparing `git-debranch-0.1.4/src/git_debranch.egg-info/SOURCES.txt` & `git-debranch-0.1.5/src/git_debranch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

