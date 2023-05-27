# Comparing `tmp/iam_actions-1.2.20230526.tar.gz` & `tmp/iam_actions-1.2.20230527.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230526.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230527.tar", max compression
```

## Comparing `iam_actions-1.2.20230526.tar` & `iam_actions-1.2.20230527.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/LICENSE
--rw-r--r--   0        0        0     2302 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/README.md
--rw-r--r--   0        0        0      228 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/iam_actions/__init__.py
--rw-r--r--   0        0        0  4273676 2023-05-26 02:29:01.701737 iam_actions-1.2.20230526/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-05-26 02:26:59.648847 iam_actions-1.2.20230526/iam_actions/generate/services.py
--rw-r--r--   0        0        0   549435 2023-05-26 02:29:01.701737 iam_actions-1.2.20230526/iam_actions/policies.json
--rw-r--r--   0        0        0   194779 2023-05-26 02:29:01.701737 iam_actions-1.2.20230526/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   532983 2023-05-26 02:29:01.701737 iam_actions-1.2.20230526/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-05-26 02:29:02.685779 iam_actions-1.2.20230526/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230526/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230526/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-27 02:25:44.275060 iam_actions-1.2.20230527/LICENSE
+-rw-r--r--   0        0        0     2302 2023-05-27 02:25:44.275060 iam_actions-1.2.20230527/README.md
+-rw-r--r--   0        0        0      228 2023-05-27 02:25:44.275060 iam_actions-1.2.20230527/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4275135 2023-05-27 02:27:54.083969 iam_actions-1.2.20230527/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-05-27 02:25:44.275060 iam_actions-1.2.20230527/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-05-27 02:25:44.275060 iam_actions-1.2.20230527/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-27 02:25:44.275060 iam_actions-1.2.20230527/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-05-27 02:25:44.275060 iam_actions-1.2.20230527/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-05-27 02:25:44.275060 iam_actions-1.2.20230527/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-05-27 02:25:44.275060 iam_actions-1.2.20230527/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-05-27 02:25:44.275060 iam_actions-1.2.20230527/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-05-27 02:25:44.275060 iam_actions-1.2.20230527/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   549639 2023-05-27 02:27:54.083969 iam_actions-1.2.20230527/iam_actions/policies.json
+-rw-r--r--   0        0        0   194779 2023-05-27 02:27:54.083969 iam_actions-1.2.20230527/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   533181 2023-05-27 02:27:54.083969 iam_actions-1.2.20230527/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-05-27 02:27:55.079976 iam_actions-1.2.20230527/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230527/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230527/PKG-INFO
```

### Comparing `iam_actions-1.2.20230526/LICENSE` & `iam_actions-1.2.20230527/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230526/README.md` & `iam_actions-1.2.20230527/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230526/iam_actions/actions.json` & `iam_actions-1.2.20230527/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999405084347633%*

 * *Differences: {"'proton'": "{'ListEnvironmentAccountConnections': {'resources': []}}",*

 * * "'quicksight'": "{'StartAssetBundleExportJob': OrderedDict([('access_level', 'Undocumented'), "*

 * *                 "('action', 'StartAssetBundleExportJob'), ('condition_keys', []), ('description', "*

 * *                 "'Not Documented by AWS'), ('orphan', False), ('resources', [])]), "*

 * *                 "'DescribeAssetBundleImportJob': OrderedDict([('access_level', 'Undocumented'), "*

 * *                 "('action', 'DescribeAssetBundleImportJ […]*

```diff
@@ -108016,17 +108016,15 @@
         },
         "ListEnvironmentAccountConnections": {
             "access_level": "List",
             "action": "ListEnvironmentAccountConnections",
             "condition_keys": [],
             "description": "Grants permission to list environment account connections",
             "orphan": false,
-            "resources": [
-                "environment-account-connection"
-            ]
+            "resources": []
         },
         "ListEnvironmentOutputs": {
             "access_level": "List",
             "action": "ListEnvironmentOutputs",
             "condition_keys": [],
             "description": "Grants permission to list environment outputs",
             "orphan": false,
@@ -109583,14 +109581,30 @@
             "condition_keys": [],
             "description": "Grants permission to describe permissions for an analysis",
             "orphan": false,
             "resources": [
                 "analysis"
             ]
         },
+        "DescribeAssetBundleExportJob": {
+            "access_level": "Undocumented",
+            "action": "DescribeAssetBundleExportJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DescribeAssetBundleImportJob": {
+            "access_level": "Undocumented",
+            "action": "DescribeAssetBundleImportJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeCustomPermissions": {
             "access_level": "Write",
             "action": "DescribeCustomPermissions",
             "condition_keys": [],
             "description": "Grants permission to describe a custom permissions resource in a QuickSight account",
             "orphan": false,
             "resources": []
@@ -110000,14 +110014,30 @@
             "condition_keys": [],
             "description": "Grants permission to list all analyses in an account",
             "orphan": false,
             "resources": [
                 "analysis"
             ]
         },
+        "ListAssetBundleExportJobs": {
+            "access_level": "Undocumented",
+            "action": "ListAssetBundleExportJobs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListAssetBundleImportJobs": {
+            "access_level": "Undocumented",
+            "action": "ListAssetBundleImportJobs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListCustomPermissions": {
             "access_level": "Write",
             "action": "ListCustomPermissions",
             "condition_keys": [],
             "description": "Grants permission to list custom permissions resources in QuickSight account",
             "orphan": false,
             "resources": []
@@ -110405,14 +110435,30 @@
             "access_level": "Write",
             "action": "SetGroupMapping",
             "condition_keys": [],
             "description": "Grants permission to use Amazon QuickSight, in Enterprise edition, to display your Microsoft Active Directory directory groups so that you can choose which ones to map to roles in Amazon QuickSight",
             "orphan": false,
             "resources": []
         },
+        "StartAssetBundleExportJob": {
+            "access_level": "Undocumented",
+            "action": "StartAssetBundleExportJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StartAssetBundleImportJob": {
+            "access_level": "Undocumented",
+            "action": "StartAssetBundleImportJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "Subscribe": {
             "access_level": "Write",
             "action": "Subscribe",
             "condition_keys": [
                 "quicksight:DirectoryType",
                 "quicksight:Edition"
             ],
@@ -117561,28 +117607,32 @@
             "action": "ListTrustAnchors",
             "condition_keys": [],
             "description": "Grants permission to list trust anchors",
             "orphan": false,
             "resources": []
         },
         "PutNotificationSettings": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PutNotificationSettings",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to attach notification settings to a trust anchor",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "trust-anchor"
+            ]
         },
         "ResetNotificationSettings": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ResetNotificationSettings",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to reset custom notification settings to IAM Roles Anywhere defined default state",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "trust-anchor"
+            ]
         },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
```

### Comparing `iam_actions-1.2.20230526/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230527/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230526/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230527/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230526/iam_actions/generate/generate.py` & `iam_actions-1.2.20230527/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230526/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230527/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230526/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230527/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230526/iam_actions/generate/services.py` & `iam_actions-1.2.20230527/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230526/iam_actions/policies.json` & `iam_actions-1.2.20230527/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999996295363276%*

 * *Differences: {"'serviceMap'": "{'Amazon QuickSight': {'Actions': {insert: [(58, "*

 * *                 "'DescribeAssetBundleExportJob'), (59, 'DescribeAssetBundleImportJob'), (99, "*

 * *                 "'ListAssetBundleExportJobs'), (100, 'ListAssetBundleImportJobs'), (141, "*

 * *                 "'StartAssetBundleExportJob'), (142, 'StartAssetBundleImportJob')]}}}"}*

```diff
@@ -16727,14 +16727,16 @@
                 "DeleteUserByPrincipalId",
                 "DeleteVPCConnection",
                 "DescribeAccountCustomization",
                 "DescribeAccountSettings",
                 "DescribeAccountSubscription",
                 "DescribeAnalysis",
                 "DescribeAnalysisPermissions",
+                "DescribeAssetBundleExportJob",
+                "DescribeAssetBundleImportJob",
                 "DescribeCustomPermissions",
                 "DescribeDashboard",
                 "DescribeDashboardPermissions",
                 "DescribeDataSet",
                 "DescribeDataSetPermissions",
                 "DescribeDataSetRefreshProperties",
                 "DescribeDataSource",
@@ -16766,14 +16768,16 @@
                 "GenerateEmbedUrlForRegisteredUser",
                 "GetAnonymousUserEmbedUrl",
                 "GetAuthCode",
                 "GetDashboardEmbedUrl",
                 "GetGroupMapping",
                 "GetSessionEmbedUrl",
                 "ListAnalyses",
+                "ListAssetBundleExportJobs",
+                "ListAssetBundleImportJobs",
                 "ListCustomPermissions",
                 "ListDashboardVersions",
                 "ListDashboards",
                 "ListDataSets",
                 "ListDataSources",
                 "ListFolderMembers",
                 "ListFolders",
@@ -16806,14 +16810,16 @@
                 "SearchDashboards",
                 "SearchDataSets",
                 "SearchDataSources",
                 "SearchDirectoryGroups",
                 "SearchFolders",
                 "SearchGroups",
                 "SetGroupMapping",
+                "StartAssetBundleExportJob",
+                "StartAssetBundleImportJob",
                 "Subscribe",
                 "TagResource",
                 "Unsubscribe",
                 "UntagResource",
                 "UpdateAccountCustomization",
                 "UpdateAccountSettings",
                 "UpdateAnalysis",
```

### Comparing `iam_actions-1.2.20230526/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230527/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230526/iam_actions/services.json` & `iam_actions-1.2.20230527/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999961204220981%*

 * *Differences: {"'quicksight'": "{'Actions': {insert: [(58, 'DescribeAssetBundleExportJob'), (59, "*

 * *                 "'DescribeAssetBundleImportJob'), (99, 'ListAssetBundleExportJobs'), (100, "*

 * *                 "'ListAssetBundleImportJobs'), (141, 'StartAssetBundleExportJob'), (142, "*

 * *                 "'StartAssetBundleImportJob')]}}"}*

```diff
@@ -15409,14 +15409,16 @@
             "DeleteUserByPrincipalId",
             "DeleteVPCConnection",
             "DescribeAccountCustomization",
             "DescribeAccountSettings",
             "DescribeAccountSubscription",
             "DescribeAnalysis",
             "DescribeAnalysisPermissions",
+            "DescribeAssetBundleExportJob",
+            "DescribeAssetBundleImportJob",
             "DescribeCustomPermissions",
             "DescribeDashboard",
             "DescribeDashboardPermissions",
             "DescribeDataSet",
             "DescribeDataSetPermissions",
             "DescribeDataSetRefreshProperties",
             "DescribeDataSource",
@@ -15448,14 +15450,16 @@
             "GenerateEmbedUrlForRegisteredUser",
             "GetAnonymousUserEmbedUrl",
             "GetAuthCode",
             "GetDashboardEmbedUrl",
             "GetGroupMapping",
             "GetSessionEmbedUrl",
             "ListAnalyses",
+            "ListAssetBundleExportJobs",
+            "ListAssetBundleImportJobs",
             "ListCustomPermissions",
             "ListDashboardVersions",
             "ListDashboards",
             "ListDataSets",
             "ListDataSources",
             "ListFolderMembers",
             "ListFolders",
@@ -15488,14 +15492,16 @@
             "SearchDashboards",
             "SearchDataSets",
             "SearchDataSources",
             "SearchDirectoryGroups",
             "SearchFolders",
             "SearchGroups",
             "SetGroupMapping",
+            "StartAssetBundleExportJob",
+            "StartAssetBundleImportJob",
             "Subscribe",
             "TagResource",
             "Unsubscribe",
             "UntagResource",
             "UpdateAccountCustomization",
             "UpdateAccountSettings",
             "UpdateAnalysis",
```

### Comparing `iam_actions-1.2.20230526/pyproject.toml` & `iam_actions-1.2.20230527/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230526"
+version = "1.2.20230527"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230526/setup.py` & `iam_actions-1.2.20230527/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230526',
+    'version': '1.2.20230527',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230526/PKG-INFO` & `iam_actions-1.2.20230527/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230526
+Version: 1.2.20230527
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

