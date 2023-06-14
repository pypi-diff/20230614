# Comparing `tmp/iam_actions-1.2.20230612.tar.gz` & `tmp/iam_actions-1.2.20230613.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230612.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230613.tar", max compression
```

## Comparing `iam_actions-1.2.20230612.tar` & `iam_actions-1.2.20230613.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-12 02:47:58.739458 iam_actions-1.2.20230612/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-12 02:47:58.739458 iam_actions-1.2.20230612/README.md
--rw-r--r--   0        0        0      228 2023-06-12 02:47:58.739458 iam_actions-1.2.20230612/iam_actions/__init__.py
--rw-r--r--   0        0        0  4302399 2023-06-12 02:49:42.064139 iam_actions-1.2.20230612/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-12 02:47:58.739458 iam_actions-1.2.20230612/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-12 02:47:58.739458 iam_actions-1.2.20230612/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-12 02:47:58.739458 iam_actions-1.2.20230612/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-12 02:47:58.739458 iam_actions-1.2.20230612/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-12 02:47:58.739458 iam_actions-1.2.20230612/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-12 02:47:58.739458 iam_actions-1.2.20230612/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-12 02:47:58.739458 iam_actions-1.2.20230612/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-12 02:47:58.739458 iam_actions-1.2.20230612/iam_actions/generate/services.py
--rw-r--r--   0        0        0   553126 2023-06-12 02:49:42.064139 iam_actions-1.2.20230612/iam_actions/policies.json
--rw-r--r--   0        0        0   195812 2023-06-12 02:49:42.064139 iam_actions-1.2.20230612/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   536452 2023-06-12 02:49:42.064139 iam_actions-1.2.20230612/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-12 02:49:42.820144 iam_actions-1.2.20230612/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230612/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230612/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/README.md
+-rw-r--r--   0        0        0      228 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4304030 2023-06-13 02:38:00.349694 iam_actions-1.2.20230613/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   553303 2023-06-13 02:38:00.349694 iam_actions-1.2.20230613/iam_actions/policies.json
+-rw-r--r--   0        0        0   195812 2023-06-13 02:38:00.349694 iam_actions-1.2.20230613/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   536622 2023-06-13 02:38:00.349694 iam_actions-1.2.20230613/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-13 02:38:01.097700 iam_actions-1.2.20230613/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230613/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230613/PKG-INFO
```

### Comparing `iam_actions-1.2.20230612/LICENSE` & `iam_actions-1.2.20230613/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230612/README.md` & `iam_actions-1.2.20230613/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230612/iam_actions/actions.json` & `iam_actions-1.2.20230613/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998113769710304%*

 * *Differences: {"'connect'": "{'SearchPrompts': {'access_level': 'Read', 'condition_keys': ['connect:InstanceId', "*

 * *              "'connect:SearchTag/${TagKey}'], 'description': 'Grants permission to search prompt "*

 * *              "resources in an Amazon Connect instance', 'resources': ['instance']}, "*

 * *              "'SearchHoursOfOperations': {'access_level': 'Read', 'condition_keys': "*

 * *              "['connect:InstanceId', 'connect:SearchTag/${TagKey}'], 'description': 'Grants "*

 * *              "permission to search hours  […]*

```diff
@@ -31550,28 +31550,38 @@
             "description": "Grants permission to search phone number resources in an Amazon Connect instance or traffic distribution group",
             "orphan": false,
             "resources": [
                 "wildcard-phone-number"
             ]
         },
         "SearchHoursOfOperations": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "SearchHoursOfOperations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "connect:InstanceId",
+                "connect:SearchTag/${TagKey}"
+            ],
+            "description": "Grants permission to search hours of opeartion resources in an Amazon Connect instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "SearchPrompts": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "SearchPrompts",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "connect:InstanceId",
+                "connect:SearchTag/${TagKey}"
+            ],
+            "description": "Grants permission to search prompt resources in an Amazon Connect instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "SearchQueues": {
             "access_level": "Read",
             "action": "SearchQueues",
             "condition_keys": [
                 "connect:InstanceId",
                 "connect:SearchTag/${TagKey}"
@@ -31579,20 +31589,25 @@
             "description": "Grants permission to search queue resources in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "instance"
             ]
         },
         "SearchQuickConnects": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "SearchQuickConnects",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "connect:InstanceId",
+                "connect:SearchTag/${TagKey}"
+            ],
+            "description": "Grants permission to search quick connect resources in an Amazon Connect instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "SearchRoutingProfiles": {
             "access_level": "Read",
             "action": "SearchRoutingProfiles",
             "condition_keys": [
                 "connect:InstanceId",
                 "connect:SearchTag/${TagKey}"
@@ -74426,14 +74441,22 @@
             "access_level": "Write",
             "action": "CancelFindingsReport",
             "condition_keys": [],
             "description": "Grants permission to cancel the generation of a findings report",
             "orphan": false,
             "resources": []
         },
+        "CancelSbomExport": {
+            "access_level": "Undocumented",
+            "action": "CancelSbomExport",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateFilter": {
             "access_level": "Write",
             "action": "CreateFilter",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -74447,14 +74470,22 @@
             "access_level": "Write",
             "action": "CreateFindingsReport",
             "condition_keys": [],
             "description": "Grants permission to request the generation of a findings report",
             "orphan": false,
             "resources": []
         },
+        "CreateSbomExport": {
+            "access_level": "Undocumented",
+            "action": "CreateSbomExport",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteFilter": {
             "access_level": "Write",
             "action": "DeleteFilter",
             "condition_keys": [],
             "description": "Grants permission to delete a findings filter",
             "orphan": false,
             "resources": [
@@ -74529,14 +74560,22 @@
             "access_level": "Read",
             "action": "GetEc2DeepInspectionConfiguration",
             "condition_keys": [],
             "description": "Grants permission to retrieve ec2 deep inspection configuration for standalone accounts, delegated administrator and member account",
             "orphan": false,
             "resources": []
         },
+        "GetEncryptionKey": {
+            "access_level": "Undocumented",
+            "action": "GetEncryptionKey",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetFindingsReportStatus": {
             "access_level": "Read",
             "action": "GetFindingsReportStatus",
             "condition_keys": [],
             "description": "Grants permission to retrieve status for a requested findings report",
             "orphan": false,
             "resources": []
@@ -74545,14 +74584,22 @@
             "access_level": "Read",
             "action": "GetMember",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about an account that's associated with an Amazon Inspector administrator account",
             "orphan": false,
             "resources": []
         },
+        "GetSbomExport": {
+            "access_level": "Undocumented",
+            "action": "GetSbomExport",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListAccountPermissions": {
             "access_level": "List",
             "action": "ListAccountPermissions",
             "condition_keys": [],
             "description": "Grants permission to retrieve feature configuration permissions associated with an Amazon Inspector account within an organization",
             "orphan": false,
             "resources": []
@@ -74625,14 +74672,22 @@
             "access_level": "List",
             "action": "ListUsageTotals",
             "condition_keys": [],
             "description": "Grants permission to retrieve aggregated usage data for an account",
             "orphan": false,
             "resources": []
         },
+        "ResetEncryptionKey": {
+            "access_level": "Undocumented",
+            "action": "ResetEncryptionKey",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "SearchVulnerabilities": {
             "access_level": "Read",
             "action": "SearchVulnerabilities",
             "condition_keys": [],
             "description": "Grants permission to list Amazon Inspector coverage details for a specific vulnerability",
             "orphan": false,
             "resources": []
@@ -74671,14 +74726,22 @@
             "access_level": "Write",
             "action": "UpdateEc2DeepInspectionConfiguration",
             "condition_keys": [],
             "description": "Grants permission to update ec2 deep inspection configuration by delegated administrator, member and standalone account",
             "orphan": false,
             "resources": []
         },
+        "UpdateEncryptionKey": {
+            "access_level": "Undocumented",
+            "action": "UpdateEncryptionKey",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateFilter": {
             "access_level": "Write",
             "action": "UpdateFilter",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
```

### Comparing `iam_actions-1.2.20230612/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230613/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230612/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230613/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230612/iam_actions/generate/generate.py` & `iam_actions-1.2.20230613/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230612/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230613/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230612/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230613/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230612/iam_actions/generate/services.py` & `iam_actions-1.2.20230613/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230612/iam_actions/policies.json` & `iam_actions-1.2.20230613/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999982693507153%*

 * *Differences: {"'serviceMap'": "{'Amazon SageMaker': {'conditionKeys': {insert: [(36, "*

 * *                 "'sagemaker:TaggingAction')]}}, 'Amazon Inspector2': {'Actions': {insert: [(7, "*

 * *                 "'CancelSbomExport'), (10, 'CreateSbomExport'), (21, 'GetEncryptionKey'), (24, "*

 * *                 "'GetSbomExport'), (35, 'ResetEncryptionKey'), (41, 'UpdateEncryptionKey')]}}}"}*

```diff
@@ -14521,43 +14521,49 @@
                 "AssociateMember",
                 "BatchGetAccountStatus",
                 "BatchGetCodeSnippet",
                 "BatchGetFreeTrialInfo",
                 "BatchGetMemberEc2DeepInspectionStatus",
                 "BatchUpdateMemberEc2DeepInspectionStatus",
                 "CancelFindingsReport",
+                "CancelSbomExport",
                 "CreateFilter",
                 "CreateFindingsReport",
+                "CreateSbomExport",
                 "DeleteFilter",
                 "DescribeOrganizationConfiguration",
                 "Disable",
                 "DisableDelegatedAdminAccount",
                 "DisassociateMember",
                 "Enable",
                 "EnableDelegatedAdminAccount",
                 "GetConfiguration",
                 "GetDelegatedAdminAccount",
                 "GetEc2DeepInspectionConfiguration",
+                "GetEncryptionKey",
                 "GetFindingsReportStatus",
                 "GetMember",
+                "GetSbomExport",
                 "ListAccountPermissions",
                 "ListCoverage",
                 "ListCoverageStatistics",
                 "ListDelegatedAdminAccounts",
                 "ListFilters",
                 "ListFindingAggregations",
                 "ListFindings",
                 "ListMembers",
                 "ListTagsForResource",
                 "ListUsageTotals",
+                "ResetEncryptionKey",
                 "SearchVulnerabilities",
                 "TagResource",
                 "UntagResource",
                 "UpdateConfiguration",
                 "UpdateEc2DeepInspectionConfiguration",
+                "UpdateEncryptionKey",
                 "UpdateFilter",
                 "UpdateOrgEc2DeepInspectionConfiguration",
                 "UpdateOrganizationConfiguration"
             ],
             "HasResource": true,
             "StringPrefix": "inspector2",
             "conditionKeys": [
@@ -18774,14 +18780,15 @@
                 "sagemaker:NetworkIsolation",
                 "sagemaker:OutputKmsKey",
                 "sagemaker:ResourceTag/",
                 "sagemaker:ResourceTag/${TagKey}",
                 "sagemaker:RootAccess",
                 "sagemaker:ServerlessMaxConcurrency",
                 "sagemaker:ServerlessMemorySize",
+                "sagemaker:TaggingAction",
                 "sagemaker:TargetModel",
                 "sagemaker:VolumeKmsKey",
                 "sagemaker:VpcSecurityGroupIds",
                 "sagemaker:VpcSubnets",
                 "sagemaker:WorkteamArn",
                 "sagemaker:WorkteamType"
             ]
```

### Comparing `iam_actions-1.2.20230612/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230613/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230612/iam_actions/services.json` & `iam_actions-1.2.20230613/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999981876256101%*

 * *Differences: {"'inspector2'": "{'Actions': {insert: [(7, 'CancelSbomExport'), (10, 'CreateSbomExport'), (21, "*

 * *                 "'GetEncryptionKey'), (24, 'GetSbomExport'), (35, 'ResetEncryptionKey'), (41, "*

 * *                 "'UpdateEncryptionKey')]}}",*

 * * "'sagemaker'": "{'ConditionKeys': {insert: [(36, 'sagemaker:TaggingAction')]}}"}*

```diff
@@ -10246,43 +10246,49 @@
             "AssociateMember",
             "BatchGetAccountStatus",
             "BatchGetCodeSnippet",
             "BatchGetFreeTrialInfo",
             "BatchGetMemberEc2DeepInspectionStatus",
             "BatchUpdateMemberEc2DeepInspectionStatus",
             "CancelFindingsReport",
+            "CancelSbomExport",
             "CreateFilter",
             "CreateFindingsReport",
+            "CreateSbomExport",
             "DeleteFilter",
             "DescribeOrganizationConfiguration",
             "Disable",
             "DisableDelegatedAdminAccount",
             "DisassociateMember",
             "Enable",
             "EnableDelegatedAdminAccount",
             "GetConfiguration",
             "GetDelegatedAdminAccount",
             "GetEc2DeepInspectionConfiguration",
+            "GetEncryptionKey",
             "GetFindingsReportStatus",
             "GetMember",
+            "GetSbomExport",
             "ListAccountPermissions",
             "ListCoverage",
             "ListCoverageStatistics",
             "ListDelegatedAdminAccounts",
             "ListFilters",
             "ListFindingAggregations",
             "ListFindings",
             "ListMembers",
             "ListTagsForResource",
             "ListUsageTotals",
+            "ResetEncryptionKey",
             "SearchVulnerabilities",
             "TagResource",
             "UntagResource",
             "UpdateConfiguration",
             "UpdateEc2DeepInspectionConfiguration",
+            "UpdateEncryptionKey",
             "UpdateFilter",
             "UpdateOrgEc2DeepInspectionConfiguration",
             "UpdateOrganizationConfiguration"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
@@ -17724,14 +17730,15 @@
             "sagemaker:NetworkIsolation",
             "sagemaker:OutputKmsKey",
             "sagemaker:ResourceTag/",
             "sagemaker:ResourceTag/${TagKey}",
             "sagemaker:RootAccess",
             "sagemaker:ServerlessMaxConcurrency",
             "sagemaker:ServerlessMemorySize",
+            "sagemaker:TaggingAction",
             "sagemaker:TargetModel",
             "sagemaker:VolumeKmsKey",
             "sagemaker:VpcSecurityGroupIds",
             "sagemaker:VpcSubnets",
             "sagemaker:WorkteamArn",
             "sagemaker:WorkteamType"
         ],
```

### Comparing `iam_actions-1.2.20230612/pyproject.toml` & `iam_actions-1.2.20230613/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230612"
+version = "1.2.20230613"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230612/setup.py` & `iam_actions-1.2.20230613/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230612',
+    'version': '1.2.20230613',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230612/PKG-INFO` & `iam_actions-1.2.20230613/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230612
+Version: 1.2.20230613
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

