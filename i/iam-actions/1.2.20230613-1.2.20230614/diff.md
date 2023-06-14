# Comparing `tmp/iam_actions-1.2.20230613.tar.gz` & `tmp/iam_actions-1.2.20230614.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230613.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230614.tar", max compression
```

## Comparing `iam_actions-1.2.20230613.tar` & `iam_actions-1.2.20230614.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/README.md
--rw-r--r--   0        0        0      228 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/iam_actions/__init__.py
--rw-r--r--   0        0        0  4304030 2023-06-13 02:38:00.349694 iam_actions-1.2.20230613/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-13 02:36:21.720798 iam_actions-1.2.20230613/iam_actions/generate/services.py
--rw-r--r--   0        0        0   553303 2023-06-13 02:38:00.349694 iam_actions-1.2.20230613/iam_actions/policies.json
--rw-r--r--   0        0        0   195812 2023-06-13 02:38:00.349694 iam_actions-1.2.20230613/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   536622 2023-06-13 02:38:00.349694 iam_actions-1.2.20230613/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-13 02:38:01.097700 iam_actions-1.2.20230613/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230613/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230613/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-14 02:35:37.280813 iam_actions-1.2.20230614/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-14 02:35:37.280813 iam_actions-1.2.20230614/README.md
+-rw-r--r--   0        0        0      228 2023-06-14 02:35:37.280813 iam_actions-1.2.20230614/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4314477 2023-06-14 02:37:54.089213 iam_actions-1.2.20230614/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-14 02:35:37.280813 iam_actions-1.2.20230614/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-14 02:35:37.280813 iam_actions-1.2.20230614/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-14 02:35:37.280813 iam_actions-1.2.20230614/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-14 02:35:37.280813 iam_actions-1.2.20230614/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-14 02:35:37.280813 iam_actions-1.2.20230614/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-14 02:35:37.280813 iam_actions-1.2.20230614/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-14 02:35:37.280813 iam_actions-1.2.20230614/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-14 02:35:37.280813 iam_actions-1.2.20230614/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   554886 2023-06-14 02:37:54.089213 iam_actions-1.2.20230614/iam_actions/policies.json
+-rw-r--r--   0        0        0   195840 2023-06-14 02:37:54.089213 iam_actions-1.2.20230614/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   538200 2023-06-14 02:37:54.089213 iam_actions-1.2.20230614/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-14 02:37:55.209217 iam_actions-1.2.20230614/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230614/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230614/PKG-INFO
```

### Comparing `iam_actions-1.2.20230613/LICENSE` & `iam_actions-1.2.20230614/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230613/README.md` & `iam_actions-1.2.20230614/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230613/iam_actions/actions.json` & `iam_actions-1.2.20230614/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9966910914888276%*

 * *Differences: {"'drs'": "{'DeleteSourceNetwork': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *          "'DeleteSourceNetwork'), ('condition_keys', []), ('description', 'Not Documented by "*

 * *          "AWS'), ('orphan', False), ('resources', [])]), 'DescribeSourceNetworks': "*

 * *          "OrderedDict([('access_level', 'Undocumented'), ('action', 'DescribeSourceNetworks'), "*

 * *          "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', False), "*

 * *          "('resources', [])]), 'StartS […]*

```diff
@@ -40120,14 +40120,22 @@
             "condition_keys": [],
             "description": "Grants permission to get associate failback client to recovery instance",
             "orphan": false,
             "resources": [
                 "RecoveryInstanceResource"
             ]
         },
+        "AssociateSourceNetworkStack": {
+            "access_level": "Undocumented",
+            "action": "AssociateSourceNetworkStack",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "BatchCreateVolumeSnapshotGroupForDrs": {
             "access_level": "Write",
             "action": "BatchCreateVolumeSnapshotGroupForDrs",
             "condition_keys": [],
             "description": "Grants permission to batch create volume snapshot group",
             "orphan": false,
             "resources": [
@@ -40198,14 +40206,22 @@
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create replication configuration template",
             "orphan": false,
             "resources": []
         },
+        "CreateSourceNetwork": {
+            "access_level": "Undocumented",
+            "action": "CreateSourceNetwork",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateSourceServerForDrs": {
             "access_level": "Write",
             "action": "CreateSourceServerForDrs",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -40249,14 +40265,22 @@
             "condition_keys": [],
             "description": "Grants permission to delete replication configuration template",
             "orphan": false,
             "resources": [
                 "ReplicationConfigurationTemplateResource"
             ]
         },
+        "DeleteSourceNetwork": {
+            "access_level": "Undocumented",
+            "action": "DeleteSourceNetwork",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteSourceServer": {
             "access_level": "Write",
             "action": "DeleteSourceServer",
             "condition_keys": [],
             "description": "Grants permission to delete source server",
             "orphan": false,
             "resources": [
@@ -40327,14 +40351,22 @@
             "access_level": "Read",
             "action": "DescribeSnapshotRequestsForDrs",
             "condition_keys": [],
             "description": "Grants permission to describe snapshot requests",
             "orphan": false,
             "resources": []
         },
+        "DescribeSourceNetworks": {
+            "access_level": "Undocumented",
+            "action": "DescribeSourceNetworks",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeSourceServers": {
             "access_level": "Read",
             "action": "DescribeSourceServers",
             "condition_keys": [],
             "description": "Grants permission to describe source servers",
             "orphan": false,
             "resources": []
@@ -40355,14 +40387,22 @@
             "condition_keys": [],
             "description": "Grants permission to disconnect source server",
             "orphan": false,
             "resources": [
                 "SourceServerResource"
             ]
         },
+        "ExportSourceNetworkCfnTemplate": {
+            "access_level": "Undocumented",
+            "action": "ExportSourceNetworkCfnTemplate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetAgentCommandForDrs": {
             "access_level": "Read",
             "action": "GetAgentCommandForDrs",
             "condition_keys": [],
             "description": "Grants permission to get agent command",
             "orphan": false,
             "resources": [
@@ -40718,14 +40758,30 @@
             "condition_keys": [],
             "description": "Grants permission to start replication",
             "orphan": false,
             "resources": [
                 "SourceServerResource"
             ]
         },
+        "StartSourceNetworkRecovery": {
+            "access_level": "Undocumented",
+            "action": "StartSourceNetworkRecovery",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StartSourceNetworkReplication": {
+            "access_level": "Undocumented",
+            "action": "StartSourceNetworkReplication",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StopFailback": {
             "access_level": "Write",
             "action": "StopFailback",
             "condition_keys": [],
             "description": "Grants permission to stop failback",
             "orphan": false,
             "resources": [
@@ -40738,14 +40794,22 @@
             "condition_keys": [],
             "description": "Grants permission to stop replication",
             "orphan": false,
             "resources": [
                 "SourceServerResource"
             ]
         },
+        "StopSourceNetworkReplication": {
+            "access_level": "Undocumented",
+            "action": "StopSourceNetworkReplication",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
                 "drs:CreateAction"
@@ -130166,14 +130230,22 @@
             "condition_keys": [],
             "description": "Grants permission to accept Security Hub invitations to become a member account",
             "orphan": false,
             "resources": [
                 "hub"
             ]
         },
+        "BatchDeleteAutomationRules": {
+            "access_level": "Undocumented",
+            "action": "BatchDeleteAutomationRules",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "BatchDisableStandards": {
             "access_level": "Write",
             "action": "BatchDisableStandards",
             "condition_keys": [],
             "description": "Grants permission to disable standards in Security Hub",
             "orphan": false,
             "resources": [
@@ -130186,14 +130258,22 @@
             "condition_keys": [],
             "description": "Grants permission to enable standards in Security Hub",
             "orphan": false,
             "resources": [
                 "hub"
             ]
         },
+        "BatchGetAutomationRules": {
+            "access_level": "Undocumented",
+            "action": "BatchGetAutomationRules",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "BatchGetControlEvaluations": {
             "access_level": "Read",
             "action": "BatchGetControlEvaluations",
             "condition_keys": [],
             "description": "Grants permission to get the enablement and compliance status of controls, the findings count for controls, and the overall security score for controls on the Security Hub console",
             "orphan": false,
             "resources": [
@@ -130224,14 +130304,22 @@
             ],
             "description": "Grants permission to import findings into Security Hub from an integrated product",
             "orphan": false,
             "resources": [
                 "product"
             ]
         },
+        "BatchUpdateAutomationRules": {
+            "access_level": "Undocumented",
+            "action": "BatchUpdateAutomationRules",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "BatchUpdateFindings": {
             "access_level": "Write",
             "action": "BatchUpdateFindings",
             "condition_keys": [
                 "securityhub:ASFFSyntaxPath/${ASFFSyntaxPath}"
             ],
             "description": "Grants permission to update customer-controlled fields for a selected set of Security Hub findings",
@@ -130254,14 +130342,22 @@
             "condition_keys": [],
             "description": "Grants permission to create custom actions in Security Hub",
             "orphan": false,
             "resources": [
                 "hub"
             ]
         },
+        "CreateAutomationRule": {
+            "access_level": "Undocumented",
+            "action": "CreateAutomationRule",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateFindingAggregator": {
             "access_level": "Write",
             "action": "CreateFindingAggregator",
             "condition_keys": [],
             "description": "Grants permission to create a finding aggregator, which contains the cross-Region finding aggregation configuration",
             "orphan": false,
             "resources": []
@@ -130665,14 +130761,22 @@
             "condition_keys": [],
             "description": "Grants permission to invite other AWS accounts to become Security Hub member accounts",
             "orphan": false,
             "resources": [
                 "hub"
             ]
         },
+        "ListAutomationRules": {
+            "access_level": "Undocumented",
+            "action": "ListAutomationRules",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListControlEvaluationSummaries": {
             "access_level": "Read",
             "action": "ListControlEvaluationSummaries",
             "condition_keys": [],
             "description": "Grants permission to retrieve a list of controls for a standard, including the control IDs, statuses and finding counts",
             "orphan": false,
             "resources": [
@@ -146630,14 +146734,208 @@
             "action": "AllowVerifiedAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
+    "verifiedpermissions": {
+        "CreateIdentitySource": {
+            "access_level": "Undocumented",
+            "action": "CreateIdentitySource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreatePolicy": {
+            "access_level": "Undocumented",
+            "action": "CreatePolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreatePolicyStore": {
+            "access_level": "Undocumented",
+            "action": "CreatePolicyStore",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreatePolicyTemplate": {
+            "access_level": "Undocumented",
+            "action": "CreatePolicyTemplate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteIdentitySource": {
+            "access_level": "Undocumented",
+            "action": "DeleteIdentitySource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeletePolicy": {
+            "access_level": "Undocumented",
+            "action": "DeletePolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeletePolicyStore": {
+            "access_level": "Undocumented",
+            "action": "DeletePolicyStore",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeletePolicyTemplate": {
+            "access_level": "Undocumented",
+            "action": "DeletePolicyTemplate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetIdentitySource": {
+            "access_level": "Undocumented",
+            "action": "GetIdentitySource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetPolicy": {
+            "access_level": "Undocumented",
+            "action": "GetPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetPolicyStore": {
+            "access_level": "Undocumented",
+            "action": "GetPolicyStore",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetPolicyTemplate": {
+            "access_level": "Undocumented",
+            "action": "GetPolicyTemplate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetSchema": {
+            "access_level": "Undocumented",
+            "action": "GetSchema",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "IsAuthorized": {
+            "access_level": "Undocumented",
+            "action": "IsAuthorized",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "IsAuthorizedWithToken": {
+            "access_level": "Undocumented",
+            "action": "IsAuthorizedWithToken",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListIdentitySources": {
+            "access_level": "Undocumented",
+            "action": "ListIdentitySources",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListPolicies": {
+            "access_level": "Undocumented",
+            "action": "ListPolicies",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListPolicyStores": {
+            "access_level": "Undocumented",
+            "action": "ListPolicyStores",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListPolicyTemplates": {
+            "access_level": "Undocumented",
+            "action": "ListPolicyTemplates",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "PutSchema": {
+            "access_level": "Undocumented",
+            "action": "PutSchema",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateIdentitySource": {
+            "access_level": "Undocumented",
+            "action": "UpdateIdentitySource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdatePolicy": {
+            "access_level": "Undocumented",
+            "action": "UpdatePolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdatePolicyStore": {
+            "access_level": "Undocumented",
+            "action": "UpdatePolicyStore",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdatePolicyTemplate": {
+            "access_level": "Undocumented",
+            "action": "UpdatePolicyTemplate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        }
+    },
     "voiceid": {
         "AssociateFraudster": {
             "access_level": "Write",
             "action": "AssociateFraudster",
             "condition_keys": [],
             "description": "Grants permission to associate a fraudster with a watchlist",
             "orphan": false,
@@ -149773,14 +150071,22 @@
             "condition_keys": [],
             "description": "Grants permission to associate a lens to the specified workload",
             "orphan": false,
             "resources": [
                 "workload"
             ]
         },
+        "AssociateProfiles": {
+            "access_level": "Undocumented",
+            "action": "AssociateProfiles",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateLensShare": {
             "access_level": "Write",
             "action": "CreateLensShare",
             "condition_keys": [],
             "description": "Grants permission to an owner of a lens to share with other AWS accounts and IAM Users",
             "orphan": false,
             "resources": [
@@ -149803,14 +150109,30 @@
             "condition_keys": [],
             "description": "Grants permission to create a new milestone for the specified workload",
             "orphan": false,
             "resources": [
                 "workload"
             ]
         },
+        "CreateProfile": {
+            "access_level": "Undocumented",
+            "action": "CreateProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateProfileShare": {
+            "access_level": "Undocumented",
+            "action": "CreateProfileShare",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateWorkload": {
             "access_level": "Write",
             "action": "CreateWorkload",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -149844,14 +150166,30 @@
             "condition_keys": [],
             "description": "Grants permission to delete an existing lens share",
             "orphan": false,
             "resources": [
                 "lens"
             ]
         },
+        "DeleteProfile": {
+            "access_level": "Undocumented",
+            "action": "DeleteProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteProfileShare": {
+            "access_level": "Undocumented",
+            "action": "DeleteProfileShare",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteWorkload": {
             "access_level": "Write",
             "action": "DeleteWorkload",
             "condition_keys": [],
             "description": "Grants permission to delete an existing workload",
             "orphan": false,
             "resources": [
@@ -149874,14 +150212,22 @@
             "condition_keys": [],
             "description": "Grants permission to disassociate a lens from the specified workload",
             "orphan": false,
             "resources": [
                 "workload"
             ]
         },
+        "DisassociateProfiles": {
+            "access_level": "Undocumented",
+            "action": "DisassociateProfiles",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ExportLens": {
             "access_level": "Read",
             "action": "ExportLens",
             "condition_keys": [],
             "description": "Grants permission to export an existing lens",
             "orphan": false,
             "resources": [
@@ -149954,14 +150300,30 @@
             "condition_keys": [],
             "description": "Grants permission to retrieve the specified milestone of the specified workload",
             "orphan": false,
             "resources": [
                 "workload"
             ]
         },
+        "GetProfile": {
+            "access_level": "Undocumented",
+            "action": "GetProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetProfileTemplate": {
+            "access_level": "Undocumented",
+            "action": "GetProfileTemplate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetWorkload": {
             "access_level": "Read",
             "action": "GetWorkload",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to retrieve the specified workload",
@@ -150063,14 +150425,38 @@
             "access_level": "List",
             "action": "ListNotifications",
             "condition_keys": [],
             "description": "Grants permission to list notifications related to the account or specified resource",
             "orphan": false,
             "resources": []
         },
+        "ListProfileNotifications": {
+            "access_level": "Undocumented",
+            "action": "ListProfileNotifications",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListProfileShares": {
+            "access_level": "Undocumented",
+            "action": "ListProfileShares",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListProfiles": {
+            "access_level": "Undocumented",
+            "action": "ListProfiles",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListShareInvitations": {
             "access_level": "List",
             "action": "ListShareInvitations",
             "condition_keys": [],
             "description": "Grants permission to list the workload share invitations of the specified account or user",
             "orphan": false,
             "resources": []
@@ -150157,14 +150543,22 @@
             "condition_keys": [],
             "description": "Grants permission to update properties of the specified lens review",
             "orphan": false,
             "resources": [
                 "workload"
             ]
         },
+        "UpdateProfile": {
+            "access_level": "Undocumented",
+            "action": "UpdateProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateShareInvitation": {
             "access_level": "Write",
             "action": "UpdateShareInvitation",
             "condition_keys": [],
             "description": "Grants permission to update status of the specified workload share invitation",
             "orphan": false,
             "resources": []
@@ -150194,14 +150588,22 @@
             "action": "UpgradeLensReview",
             "condition_keys": [],
             "description": "Grants permission to upgrade the specified lens review to use the latest version of the associated lens",
             "orphan": false,
             "resources": [
                 "workload"
             ]
+        },
+        "UpgradeProfileVersion": {
+            "access_level": "Undocumented",
+            "action": "UpgradeProfileVersion",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         }
     },
     "wickr": {
         "CreateAdminSession": {
             "access_level": "Write",
             "action": "CreateAdminSession",
             "condition_keys": [],
```

### Comparing `iam_actions-1.2.20230613/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230614/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230613/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230614/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230613/iam_actions/generate/generate.py` & `iam_actions-1.2.20230614/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230613/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230614/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230613/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230614/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230613/iam_actions/generate/services.py` & `iam_actions-1.2.20230614/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230613/iam_actions/policies.json` & `iam_actions-1.2.20230614/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997311614644504%*

 * *Differences: {"'serviceMap'": "{'AWS Well-Architected Tool': {'Actions': {insert: [(1, 'AssociateProfiles'), "*

 * *                 "(5, 'CreateProfile'), (6, 'CreateProfileShare'), (11, 'DeleteProfile'), (12, "*

 * *                 "'DeleteProfileShare'), (16, 'DisassociateProfiles'), (25, 'GetProfile'), (26, "*

 * *                 "'GetProfileTemplate'), (38, 'ListProfileNotifications'), (39, "*

 * *                 "'ListProfileShares'), (40, 'ListProfiles'), (50, 'UpdateProfile'), (55, "*

 * *                 "'UpgradeProfileVersion')]}} […]*

```diff
@@ -3223,38 +3223,43 @@
             ]
         },
         "AWS Elastic Disaster Recovery": {
             "ARNFormat": "arn:aws:drs:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:drs:.+",
             "Actions": [
                 "AssociateFailbackClientToRecoveryInstanceForDrs",
+                "AssociateSourceNetworkStack",
                 "BatchCreateVolumeSnapshotGroupForDrs",
                 "BatchDeleteSnapshotRequestForDrs",
                 "CreateConvertedSnapshotForDrs",
                 "CreateExtendedSourceServer",
                 "CreateLaunchConfigurationTemplate",
                 "CreateRecoveryInstanceForDrs",
                 "CreateReplicationConfigurationTemplate",
+                "CreateSourceNetwork",
                 "CreateSourceServerForDrs",
                 "DeleteJob",
                 "DeleteLaunchConfigurationTemplate",
                 "DeleteRecoveryInstance",
                 "DeleteReplicationConfigurationTemplate",
+                "DeleteSourceNetwork",
                 "DeleteSourceServer",
                 "DescribeJobLogItems",
                 "DescribeJobs",
                 "DescribeLaunchConfigurationTemplates",
                 "DescribeRecoveryInstances",
                 "DescribeRecoverySnapshots",
                 "DescribeReplicationConfigurationTemplates",
                 "DescribeReplicationServerAssociationsForDrs",
                 "DescribeSnapshotRequestsForDrs",
+                "DescribeSourceNetworks",
                 "DescribeSourceServers",
                 "DisconnectRecoveryInstance",
                 "DisconnectSourceServer",
+                "ExportSourceNetworkCfnTemplate",
                 "GetAgentCommandForDrs",
                 "GetAgentConfirmedResumeInfoForDrs",
                 "GetAgentInstallationAssetsForDrs",
                 "GetAgentReplicationInfoForDrs",
                 "GetAgentRuntimeConfigurationForDrs",
                 "GetAgentSnapshotCreditsForDrs",
                 "GetChannelCommandsForDrs",
@@ -3283,16 +3288,19 @@
                 "SendChannelCommandResultForDrs",
                 "SendClientLogsForDrs",
                 "SendClientMetricsForDrs",
                 "SendVolumeStatsForDrs",
                 "StartFailbackLaunch",
                 "StartRecovery",
                 "StartReplication",
+                "StartSourceNetworkRecovery",
+                "StartSourceNetworkReplication",
                 "StopFailback",
                 "StopReplication",
+                "StopSourceNetworkReplication",
                 "TagResource",
                 "TerminateRecoveryInstances",
                 "UntagResource",
                 "UpdateAgentBacklogForDrs",
                 "UpdateAgentConversionInfoForDrs",
                 "UpdateAgentReplicationInfoForDrs",
                 "UpdateAgentReplicationProcessStateForDrs",
@@ -7854,23 +7862,27 @@
         },
         "AWS Security Hub": {
             "ARNFormat": "arn:aws:securityhub:${Region}:${Account}:.+",
             "ARNRegex": "^arn:aws:securityhub:.+",
             "Actions": [
                 "AcceptAdministratorInvitation",
                 "AcceptInvitation",
+                "BatchDeleteAutomationRules",
                 "BatchDisableStandards",
                 "BatchEnableStandards",
+                "BatchGetAutomationRules",
                 "BatchGetControlEvaluations",
                 "BatchGetSecurityControls",
                 "BatchGetStandardsControlAssociations",
                 "BatchImportFindings",
+                "BatchUpdateAutomationRules",
                 "BatchUpdateFindings",
                 "BatchUpdateStandardsControlAssociations",
                 "CreateActionTarget",
+                "CreateAutomationRule",
                 "CreateFindingAggregator",
                 "CreateInsight",
                 "CreateMembers",
                 "DeclineInvitations",
                 "DeleteActionTarget",
                 "DeleteFindingAggregator",
                 "DeleteInsight",
@@ -7904,14 +7916,15 @@
                 "GetInsightResults",
                 "GetInsights",
                 "GetInvitationsCount",
                 "GetMasterAccount",
                 "GetMembers",
                 "GetUsage",
                 "InviteMembers",
+                "ListAutomationRules",
                 "ListControlEvaluationSummaries",
                 "ListEnabledProductsForImport",
                 "ListFindingAggregators",
                 "ListInvitations",
                 "ListMembers",
                 "ListOrganizationAdminAccounts",
                 "ListSecurityControlDefinitions",
@@ -9449,56 +9462,69 @@
             ]
         },
         "AWS Well-Architected Tool": {
             "ARNFormat": "arn:aws:wellarchitected:${Region}:${Account}:${ResourceName}/${ResourceId}",
             "ARNRegex": "^arn:aws:wellarchitected:.+",
             "Actions": [
                 "AssociateLenses",
+                "AssociateProfiles",
                 "CreateLensShare",
                 "CreateLensVersion",
                 "CreateMilestone",
+                "CreateProfile",
+                "CreateProfileShare",
                 "CreateWorkload",
                 "CreateWorkloadShare",
                 "DeleteLens",
                 "DeleteLensShare",
+                "DeleteProfile",
+                "DeleteProfileShare",
                 "DeleteWorkload",
                 "DeleteWorkloadShare",
                 "DisassociateLenses",
+                "DisassociateProfiles",
                 "ExportLens",
                 "GetAnswer",
                 "GetConsolidatedReport",
                 "GetLens",
                 "GetLensReview",
                 "GetLensReviewReport",
                 "GetLensVersionDifference",
                 "GetMilestone",
+                "GetProfile",
+                "GetProfileTemplate",
                 "GetWorkload",
                 "ImportLens",
                 "ListAnswers",
                 "ListCheckDetails",
                 "ListCheckSummaries",
                 "ListLensReviewImprovements",
                 "ListLensReviews",
                 "ListLensShares",
                 "ListLenses",
                 "ListMilestones",
                 "ListNotifications",
+                "ListProfileNotifications",
+                "ListProfileShares",
+                "ListProfiles",
                 "ListShareInvitations",
                 "ListTagsForResource",
                 "ListWorkloadShares",
                 "ListWorkloads",
                 "TagResource",
                 "UntagResource",
                 "UpdateAnswer",
                 "UpdateGlobalSettings",
                 "UpdateLensReview",
+                "UpdateProfile",
                 "UpdateShareInvitation",
                 "UpdateWorkload",
                 "UpdateWorkloadShare",
-                "UpgradeLensReview"
+                "UpgradeLensReview",
+                "UpgradeProfileVersion"
             ],
             "HasResource": true,
             "StringPrefix": "wellarchitected",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
@@ -19344,14 +19370,46 @@
                 "vpc-lattice-svcs:RequestQueryString/${QueryStringKey}",
                 "vpc-lattice-svcs:ServiceArn",
                 "vpc-lattice-svcs:ServiceNetworkArn",
                 "vpc-lattice-svcs:SourceVpc",
                 "vpc-lattice-svcs:SourceVpcOwnerAccount"
             ]
         },
+        "Amazon Verified Permissions": {
+            "ARNFormat": "arn:aws:verifiedpermissions:${Region}:${Account}:${ResourceType}/${ResourceId}",
+            "ARNRegex": "^arn:aws:verifiedpermissions:.+",
+            "Actions": [
+                "CreateIdentitySource",
+                "CreatePolicy",
+                "CreatePolicyStore",
+                "CreatePolicyTemplate",
+                "DeleteIdentitySource",
+                "DeletePolicy",
+                "DeletePolicyStore",
+                "DeletePolicyTemplate",
+                "GetIdentitySource",
+                "GetPolicy",
+                "GetPolicyStore",
+                "GetPolicyTemplate",
+                "GetSchema",
+                "IsAuthorized",
+                "IsAuthorizedWithToken",
+                "ListIdentitySources",
+                "ListPolicies",
+                "ListPolicyStores",
+                "ListPolicyTemplates",
+                "PutSchema",
+                "UpdateIdentitySource",
+                "UpdatePolicy",
+                "UpdatePolicyStore",
+                "UpdatePolicyTemplate"
+            ],
+            "HasResource": true,
+            "StringPrefix": "verifiedpermissions"
+        },
         "Amazon WorkDocs": {
             "Actions": [
                 "AbortDocumentVersionUpload",
                 "ActivateUser",
                 "AddNotificationPermissions",
                 "AddResourcePermissions",
                 "AddUserToGroup",
```

### Comparing `iam_actions-1.2.20230613/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230614/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997229916897507%*

 * *Differences: {"'verifiedpermissions'": 'OrderedDict()'}*

```diff
@@ -6334,14 +6334,15 @@
         },
         "SecurityProfile": {
             "arn_pattern": "arn:*:vendor-insights:::security-profile:*",
             "condition_keys": "aws:RequestTag/${TagKey}"
         }
     },
     "verified-access": {},
+    "verifiedpermissions": {},
     "voiceid": {
         "domain": {
             "arn_pattern": "arn:*:voiceid:*:*:domain/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "vpc-lattice": {
```

### Comparing `iam_actions-1.2.20230613/iam_actions/services.json` & `iam_actions-1.2.20230614/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971850147801172%*

 * *Differences: {"'drs'": "{'Actions': {insert: [(1, 'AssociateSourceNetworkStack'), (9, 'CreateSourceNetwork'), "*

 * *          "(15, 'DeleteSourceNetwork'), (25, 'DescribeSourceNetworks'), (29, "*

 * *          "'ExportSourceNetworkCfnTemplate'), (66, 'StartSourceNetworkRecovery'), (67, "*

 * *          "'StartSourceNetworkReplication'), (70, 'StopSourceNetworkReplication')]}}",*

 * * "'securityhub'": "{'Actions': {insert: [(2, 'BatchDeleteAutomationRules'), (5, "*

 * *                  "'BatchGetAutomationRules'), (10, 'BatchUpdateAutomationRu […]*

```diff
@@ -5996,38 +5996,43 @@
             "arn:aws:drs:${Region}:${Account}:${ResourceType}/${ResourceName}"
         ],
         "ARNRegexes": [
             "^arn:aws:drs:.+"
         ],
         "Actions": [
             "AssociateFailbackClientToRecoveryInstanceForDrs",
+            "AssociateSourceNetworkStack",
             "BatchCreateVolumeSnapshotGroupForDrs",
             "BatchDeleteSnapshotRequestForDrs",
             "CreateConvertedSnapshotForDrs",
             "CreateExtendedSourceServer",
             "CreateLaunchConfigurationTemplate",
             "CreateRecoveryInstanceForDrs",
             "CreateReplicationConfigurationTemplate",
+            "CreateSourceNetwork",
             "CreateSourceServerForDrs",
             "DeleteJob",
             "DeleteLaunchConfigurationTemplate",
             "DeleteRecoveryInstance",
             "DeleteReplicationConfigurationTemplate",
+            "DeleteSourceNetwork",
             "DeleteSourceServer",
             "DescribeJobLogItems",
             "DescribeJobs",
             "DescribeLaunchConfigurationTemplates",
             "DescribeRecoveryInstances",
             "DescribeRecoverySnapshots",
             "DescribeReplicationConfigurationTemplates",
             "DescribeReplicationServerAssociationsForDrs",
             "DescribeSnapshotRequestsForDrs",
+            "DescribeSourceNetworks",
             "DescribeSourceServers",
             "DisconnectRecoveryInstance",
             "DisconnectSourceServer",
+            "ExportSourceNetworkCfnTemplate",
             "GetAgentCommandForDrs",
             "GetAgentConfirmedResumeInfoForDrs",
             "GetAgentInstallationAssetsForDrs",
             "GetAgentReplicationInfoForDrs",
             "GetAgentRuntimeConfigurationForDrs",
             "GetAgentSnapshotCreditsForDrs",
             "GetChannelCommandsForDrs",
@@ -6056,16 +6061,19 @@
             "SendChannelCommandResultForDrs",
             "SendClientLogsForDrs",
             "SendClientMetricsForDrs",
             "SendVolumeStatsForDrs",
             "StartFailbackLaunch",
             "StartRecovery",
             "StartReplication",
+            "StartSourceNetworkRecovery",
+            "StartSourceNetworkReplication",
             "StopFailback",
             "StopReplication",
+            "StopSourceNetworkReplication",
             "TagResource",
             "TerminateRecoveryInstances",
             "UntagResource",
             "UpdateAgentBacklogForDrs",
             "UpdateAgentConversionInfoForDrs",
             "UpdateAgentReplicationInfoForDrs",
             "UpdateAgentReplicationProcessStateForDrs",
@@ -18042,23 +18050,27 @@
         ],
         "ARNRegexes": [
             "^arn:aws:securityhub:.+"
         ],
         "Actions": [
             "AcceptAdministratorInvitation",
             "AcceptInvitation",
+            "BatchDeleteAutomationRules",
             "BatchDisableStandards",
             "BatchEnableStandards",
+            "BatchGetAutomationRules",
             "BatchGetControlEvaluations",
             "BatchGetSecurityControls",
             "BatchGetStandardsControlAssociations",
             "BatchImportFindings",
+            "BatchUpdateAutomationRules",
             "BatchUpdateFindings",
             "BatchUpdateStandardsControlAssociations",
             "CreateActionTarget",
+            "CreateAutomationRule",
             "CreateFindingAggregator",
             "CreateInsight",
             "CreateMembers",
             "DeclineInvitations",
             "DeleteActionTarget",
             "DeleteFindingAggregator",
             "DeleteInsight",
@@ -18092,14 +18104,15 @@
             "GetInsightResults",
             "GetInsights",
             "GetInvitationsCount",
             "GetMasterAccount",
             "GetMembers",
             "GetUsage",
             "InviteMembers",
+            "ListAutomationRules",
             "ListControlEvaluationSummaries",
             "ListEnabledProductsForImport",
             "ListFindingAggregators",
             "ListInvitations",
             "ListMembers",
             "ListOrganizationAdminAccounts",
             "ListSecurityControlDefinitions",
@@ -20586,14 +20599,53 @@
         ],
         "ConditionKeys": [],
         "HasResource": false,
         "ServiceNames": [
             "AWS Verified Access"
         ]
     },
+    "verifiedpermissions": {
+        "ARNFormats": [
+            "arn:aws:verifiedpermissions:${Region}:${Account}:${ResourceType}/${ResourceId}"
+        ],
+        "ARNRegexes": [
+            "^arn:aws:verifiedpermissions:.+"
+        ],
+        "Actions": [
+            "CreateIdentitySource",
+            "CreatePolicy",
+            "CreatePolicyStore",
+            "CreatePolicyTemplate",
+            "DeleteIdentitySource",
+            "DeletePolicy",
+            "DeletePolicyStore",
+            "DeletePolicyTemplate",
+            "GetIdentitySource",
+            "GetPolicy",
+            "GetPolicyStore",
+            "GetPolicyTemplate",
+            "GetSchema",
+            "IsAuthorized",
+            "IsAuthorizedWithToken",
+            "ListIdentitySources",
+            "ListPolicies",
+            "ListPolicyStores",
+            "ListPolicyTemplates",
+            "PutSchema",
+            "UpdateIdentitySource",
+            "UpdatePolicy",
+            "UpdatePolicyStore",
+            "UpdatePolicyTemplate"
+        ],
+        "ConditionKeys": [],
+        "HasResource": true,
+        "ServiceNames": [
+            "Amazon Verified Permissions"
+        ]
+    },
     "voiceid": {
         "ARNFormats": [
             "arn:aws:voiceid:${Region}:${Account}:${ResourceType}/${ResourceId}"
         ],
         "ARNRegexes": [
             "^arn:aws:voiceid:.+"
         ],
@@ -21029,56 +21081,69 @@
             "arn:aws:wellarchitected:${Region}:${Account}:${ResourceName}/${ResourceId}"
         ],
         "ARNRegexes": [
             "^arn:aws:wellarchitected:.+"
         ],
         "Actions": [
             "AssociateLenses",
+            "AssociateProfiles",
             "CreateLensShare",
             "CreateLensVersion",
             "CreateMilestone",
+            "CreateProfile",
+            "CreateProfileShare",
             "CreateWorkload",
             "CreateWorkloadShare",
             "DeleteLens",
             "DeleteLensShare",
+            "DeleteProfile",
+            "DeleteProfileShare",
             "DeleteWorkload",
             "DeleteWorkloadShare",
             "DisassociateLenses",
+            "DisassociateProfiles",
             "ExportLens",
             "GetAnswer",
             "GetConsolidatedReport",
             "GetLens",
             "GetLensReview",
             "GetLensReviewReport",
             "GetLensVersionDifference",
             "GetMilestone",
+            "GetProfile",
+            "GetProfileTemplate",
             "GetWorkload",
             "ImportLens",
             "ListAnswers",
             "ListCheckDetails",
             "ListCheckSummaries",
             "ListLensReviewImprovements",
             "ListLensReviews",
             "ListLensShares",
             "ListLenses",
             "ListMilestones",
             "ListNotifications",
+            "ListProfileNotifications",
+            "ListProfileShares",
+            "ListProfiles",
             "ListShareInvitations",
             "ListTagsForResource",
             "ListWorkloadShares",
             "ListWorkloads",
             "TagResource",
             "UntagResource",
             "UpdateAnswer",
             "UpdateGlobalSettings",
             "UpdateLensReview",
+            "UpdateProfile",
             "UpdateShareInvitation",
             "UpdateWorkload",
             "UpdateWorkloadShare",
-            "UpgradeLensReview"
+            "UpgradeLensReview",
+            "UpgradeProfileVersion"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys"
         ],
         "HasResource": true,
```

### Comparing `iam_actions-1.2.20230613/pyproject.toml` & `iam_actions-1.2.20230614/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230613"
+version = "1.2.20230614"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230613/setup.py` & `iam_actions-1.2.20230614/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230613',
+    'version': '1.2.20230614',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230613/PKG-INFO` & `iam_actions-1.2.20230614/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230613
+Version: 1.2.20230614
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

