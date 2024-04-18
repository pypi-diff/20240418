# Comparing `tmp/iam_actions-1.2.20240416.tar.gz` & `tmp/iam_actions-1.2.20240417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240416.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240417.tar", max compression
```

## Comparing `iam_actions-1.2.20240416.tar` & `iam_actions-1.2.20240417.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-04-16 02:15:51.732083 iam_actions-1.2.20240416/LICENSE
--rw-r--r--   0        0        0     2302 2024-04-16 02:15:51.732083 iam_actions-1.2.20240416/README.md
--rw-r--r--   0        0        0      228 2024-04-16 02:15:51.732083 iam_actions-1.2.20240416/iam_actions/__init__.py
--rw-r--r--   0        0        0  4798523 2024-04-16 02:18:02.225469 iam_actions-1.2.20240416/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-04-16 02:15:51.732083 iam_actions-1.2.20240416/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-04-16 02:15:51.732083 iam_actions-1.2.20240416/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-04-16 02:15:51.732083 iam_actions-1.2.20240416/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-04-16 02:15:51.732083 iam_actions-1.2.20240416/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-04-16 02:15:51.732083 iam_actions-1.2.20240416/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-04-16 02:15:51.732083 iam_actions-1.2.20240416/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-04-16 02:15:51.732083 iam_actions-1.2.20240416/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-04-16 02:15:51.732083 iam_actions-1.2.20240416/iam_actions/generate/services.py
--rw-r--r--   0        0        0   623594 2024-04-16 02:18:02.225469 iam_actions-1.2.20240416/iam_actions/policies.json
--rw-r--r--   0        0        0   208021 2024-04-16 02:18:02.225469 iam_actions-1.2.20240416/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   604984 2024-04-16 02:18:02.225469 iam_actions-1.2.20240416/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-04-16 02:18:02.921476 iam_actions-1.2.20240416/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240416/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240416/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/LICENSE
+-rw-r--r--   0        0        0     2302 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/README.md
+-rw-r--r--   0        0        0      228 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4801338 2024-04-17 02:19:16.413418 iam_actions-1.2.20240417/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   623955 2024-04-17 02:19:16.413418 iam_actions-1.2.20240417/iam_actions/policies.json
+-rw-r--r--   0        0        0   208021 2024-04-17 02:19:16.413418 iam_actions-1.2.20240417/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   605333 2024-04-17 02:19:16.413418 iam_actions-1.2.20240417/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-04-17 02:19:17.053403 iam_actions-1.2.20240417/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240417/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240417/PKG-INFO
```

### Comparing `iam_actions-1.2.20240416/LICENSE` & `iam_actions-1.2.20240417/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240416/README.md` & `iam_actions-1.2.20240417/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240416/iam_actions/actions.json` & `iam_actions-1.2.20240417/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995741665921225%*

 * *Differences: {"'emr-containers'": "{'DescribeSecurityConfiguration': OrderedDict([('access_level', "*

 * *                     "'Undocumented'), ('action', 'DescribeSecurityConfiguration'), "*

 * *                     "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', "*

 * *                     "False), ('resources', [])]), 'CreateSecurityConfiguration': "*

 * *                     "OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *                     "'CreateSecurityConfiguration'), ('condition_keys' […]*

```diff
@@ -66385,14 +66385,22 @@
             ],
             "description": "Grants permission to create a managed endpoint",
             "orphan": false,
             "resources": [
                 "virtualCluster"
             ]
         },
+        "CreateSecurityConfiguration": {
+            "access_level": "Undocumented",
+            "action": "CreateSecurityConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateVirtualCluster": {
             "access_level": "Write",
             "action": "CreateVirtualCluster",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -66456,14 +66464,22 @@
             "condition_keys": [],
             "description": "Grants permission to describe a managed endpoint",
             "orphan": false,
             "resources": [
                 "managedEndpoint"
             ]
         },
+        "DescribeSecurityConfiguration": {
+            "access_level": "Undocumented",
+            "action": "DescribeSecurityConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeVirtualCluster": {
             "access_level": "Read",
             "action": "DescribeVirtualCluster",
             "condition_keys": [],
             "description": "Grants permission to describe a virtual cluster",
             "orphan": false,
             "resources": [
@@ -66504,14 +66520,22 @@
             "condition_keys": [],
             "description": "Grants permission to list managed endpoints associated with a virtual cluster",
             "orphan": false,
             "resources": [
                 "virtualCluster"
             ]
         },
+        "ListSecurityConfigurations": {
+            "access_level": "Undocumented",
+            "action": "ListSecurityConfigurations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListTagsForResource": {
             "access_level": "List",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to list tags for the specified resource",
             "orphan": false,
             "resources": [
@@ -96008,14 +96032,15 @@
             ]
         },
         "EnableKeyRotation": {
             "access_level": "Write",
             "action": "EnableKeyRotation",
             "condition_keys": [
                 "kms:CallerAccount",
+                "kms:RotationPeriodInDays",
                 "kms:ViaService"
             ],
             "description": "Controls permission to enable automatic rotation of the cryptographic material in an AWS KMS key",
             "orphan": false,
             "resources": [
                 "key"
             ]
@@ -96149,15 +96174,15 @@
         "GetKeyRotationStatus": {
             "access_level": "Read",
             "action": "GetKeyRotationStatus",
             "condition_keys": [
                 "kms:CallerAccount",
                 "kms:ViaService"
             ],
-            "description": "Controls permission to determine whether automatic key rotation is enabled on the AWS KMS key",
+            "description": "Controls permission to view the key rotation status for an AWS KMS key",
             "orphan": false,
             "resources": [
                 "key"
             ]
         },
         "GetParametersForImport": {
             "access_level": "Read",
@@ -96235,20 +96260,25 @@
             "description": "Controls permission to view the names of key policies for an AWS KMS key",
             "orphan": false,
             "resources": [
                 "key"
             ]
         },
         "ListKeyRotations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListKeyRotations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "kms:CallerAccount",
+                "kms:ViaService"
+            ],
+            "description": "Controls permission to view the list of completed key rotations for an AWS KMS key",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "key"
+            ]
         },
         "ListKeys": {
             "access_level": "List",
             "action": "ListKeys",
             "condition_keys": [],
             "description": "Controls permission to view the key ID and Amazon Resource Name (ARN) of all AWS KMS keys in the account",
             "orphan": false,
@@ -96360,20 +96390,25 @@
             "description": "Controls permission to revoke a grant, which denies permission for all operations that depend on the grant",
             "orphan": false,
             "resources": [
                 "key"
             ]
         },
         "RotateKeyOnDemand": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RotateKeyOnDemand",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "kms:CallerAccount",
+                "kms:ViaService"
+            ],
+            "description": "Controls permission to invoke on-demand rotation of the cryptographic material in an AWS KMS key",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "key"
+            ]
         },
         "ScheduleKeyDeletion": {
             "access_level": "Write",
             "action": "ScheduleKeyDeletion",
             "condition_keys": [
                 "kms:CallerAccount",
                 "kms:ScheduleKeyDeletionPendingWindowInDays",
@@ -118443,14 +118478,22 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "outposts": {
+        "CancelCapacityTask": {
+            "access_level": "Undocumented",
+            "action": "CancelCapacityTask",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CancelOrder": {
             "access_level": "Write",
             "action": "CancelOrder",
             "condition_keys": [],
             "description": "Grants permission to cancel an order",
             "orphan": false,
             "resources": []
@@ -118513,14 +118556,22 @@
             "condition_keys": [],
             "description": "Grants permission to delete a site",
             "orphan": false,
             "resources": [
                 "site"
             ]
         },
+        "GetCapacityTask": {
+            "access_level": "Undocumented",
+            "action": "GetCapacityTask",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetCatalogItem": {
             "access_level": "Read",
             "action": "GetCatalogItem",
             "condition_keys": [],
             "description": "Grants permission to get a catalog item",
             "orphan": false,
             "resources": []
@@ -118557,14 +118608,22 @@
             "condition_keys": [],
             "description": "Grants permission to get the instance types for the specified Outpost",
             "orphan": false,
             "resources": [
                 "outpost"
             ]
         },
+        "GetOutpostSupportedInstanceTypes": {
+            "access_level": "Undocumented",
+            "action": "GetOutpostSupportedInstanceTypes",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetPrivateConnectivityConfig": {
             "access_level": "Read",
             "action": "GetPrivateConnectivityConfig",
             "condition_keys": [],
             "description": "Grants permission to get a private connectivity configuration",
             "orphan": false,
             "resources": []
@@ -118593,14 +118652,22 @@
             "access_level": "List",
             "action": "ListAssets",
             "condition_keys": [],
             "description": "Grants permission to list the assets for your Outpost",
             "orphan": false,
             "resources": []
         },
+        "ListCapacityTasks": {
+            "access_level": "Undocumented",
+            "action": "ListCapacityTasks",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListCatalogItems": {
             "access_level": "List",
             "action": "ListCatalogItems",
             "condition_keys": [],
             "description": "Grants permission to list all catalog items",
             "orphan": false,
             "resources": []
@@ -118633,14 +118700,22 @@
             "access_level": "Read",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to list tags for a resource",
             "orphan": false,
             "resources": []
         },
+        "StartCapacityTask": {
+            "access_level": "Undocumented",
+            "action": "StartCapacityTask",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StartConnection": {
             "access_level": "Write",
             "action": "StartConnection",
             "condition_keys": [],
             "description": "Grants permission to start a connection for your Outpost server",
             "orphan": false,
             "resources": []
@@ -167217,14 +167292,22 @@
             "condition_keys": [],
             "description": "Grants permission to associate a profile to the specified workload",
             "orphan": false,
             "resources": [
                 "workload"
             ]
         },
+        "ConfigureIntegration": {
+            "access_level": "Write",
+            "action": "ConfigureIntegration",
+            "condition_keys": [],
+            "description": "Grants permission to configure the integration",
+            "orphan": false,
+            "resources": []
+        },
         "CreateLensShare": {
             "access_level": "Write",
             "action": "CreateLensShare",
             "condition_keys": [],
             "description": "Grants permission to an owner of a lens to share with other AWS accounts and IAM users",
             "orphan": false,
             "resources": [
@@ -167294,15 +167377,16 @@
             ]
         },
         "CreateWorkload": {
             "access_level": "Write",
             "action": "CreateWorkload",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
+                "aws:TagKeys",
+                "wellarchitected:JiraProjectKey"
             ],
             "description": "Grants permission to create a new workload",
             "orphan": false,
             "resources": []
         },
         "CreateWorkloadShare": {
             "access_level": "Write",
@@ -167438,14 +167522,22 @@
             "access_level": "Read",
             "action": "GetConsolidatedReport",
             "condition_keys": [],
             "description": "Grants permission to get consolidated report metrics or to generate the consolidated report PDF in this account",
             "orphan": false,
             "resources": []
         },
+        "GetGlobalSettings": {
+            "access_level": "Read",
+            "action": "GetGlobalSettings",
+            "condition_keys": [],
+            "description": "Grants permission to get all settings for the account",
+            "orphan": false,
+            "resources": []
+        },
         "GetLens": {
             "access_level": "Read",
             "action": "GetLens",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to get an existing lens",
@@ -167790,19 +167882,31 @@
             "resources": [
                 "workload"
             ]
         },
         "UpdateGlobalSettings": {
             "access_level": "Write",
             "action": "UpdateGlobalSettings",
-            "condition_keys": [],
-            "description": "Grants permission to update settings to enable aws-organization support",
+            "condition_keys": [
+                "wellarchitected:JiraProjectKey"
+            ],
+            "description": "Grants permission to manage all settings for the account",
             "orphan": false,
             "resources": []
         },
+        "UpdateIntegration": {
+            "access_level": "Write",
+            "action": "UpdateIntegration",
+            "condition_keys": [],
+            "description": "Grants permission to update properties of the integration",
+            "orphan": false,
+            "resources": [
+                "workload"
+            ]
+        },
         "UpdateLensReview": {
             "access_level": "Write",
             "action": "UpdateLensReview",
             "condition_keys": [],
             "description": "Grants permission to update properties of the specified lens review",
             "orphan": false,
             "resources": [
@@ -167856,15 +167960,17 @@
             "description": "Grants permission to update status of the specified workload share invitation",
             "orphan": false,
             "resources": []
         },
         "UpdateWorkload": {
             "access_level": "Write",
             "action": "UpdateWorkload",
-            "condition_keys": [],
+            "condition_keys": [
+                "wellarchitected:JiraProjectKey"
+            ],
             "description": "Grants permission to update properties of the specified workload",
             "orphan": false,
             "resources": [
                 "workload"
             ]
         },
         "UpdateWorkloadShare": {
```

### Comparing `iam_actions-1.2.20240416/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240417/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240416/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240417/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240416/iam_actions/generate/generate.py` & `iam_actions-1.2.20240417/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240416/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240417/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240416/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240417/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240416/iam_actions/generate/services.py` & `iam_actions-1.2.20240417/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240416/iam_actions/policies.json` & `iam_actions-1.2.20240417/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999941478163343%*

 * *Differences: {"'serviceMap'": "{'Amazon EMR on EKS (EMR Containers)': {'Actions': {insert: [(3, "*

 * *                 "'CreateSecurityConfiguration'), (11, 'DescribeSecurityConfiguration'), (17, "*

 * *                 "'ListSecurityConfigurations')]}}, 'AWS Outposts': {'Actions': {insert: [(0, "*

 * *                 "'CancelCapacityTask'), (8, 'GetCapacityTask'), (14, "*

 * *                 "'GetOutpostSupportedInstanceTypes'), (19, 'ListCapacityTasks'), (25, "*

 * *                 "'StartCapacityTask')]}}, 'AWS Well-Architected Tool': {' […]*

```diff
@@ -8190,35 +8190,40 @@
                 "organizations:ServicePrincipal"
             ]
         },
         "AWS Outposts": {
             "ARNFormat": "arn:aws:outposts:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:outposts:.+",
             "Actions": [
+                "CancelCapacityTask",
                 "CancelOrder",
                 "CreateOrder",
                 "CreateOutpost",
                 "CreatePrivateConnectivityConfig",
                 "CreateSite",
                 "DeleteOutpost",
                 "DeleteSite",
+                "GetCapacityTask",
                 "GetCatalogItem",
                 "GetConnection",
                 "GetOrder",
                 "GetOutpost",
                 "GetOutpostInstanceTypes",
+                "GetOutpostSupportedInstanceTypes",
                 "GetPrivateConnectivityConfig",
                 "GetSite",
                 "GetSiteAddress",
                 "ListAssets",
+                "ListCapacityTasks",
                 "ListCatalogItems",
                 "ListOrders",
                 "ListOutposts",
                 "ListSites",
                 "ListTagsForResource",
+                "StartCapacityTask",
                 "StartConnection",
                 "TagResource",
                 "UntagResource",
                 "UpdateOutpost",
                 "UpdateSite",
                 "UpdateSiteAddress",
                 "UpdateSiteRackPhysicalProperties"
@@ -10724,14 +10729,15 @@
         },
         "AWS Well-Architected Tool": {
             "ARNFormat": "arn:aws:wellarchitected:${Region}:${Account}:${ResourceName}/${ResourceId}",
             "ARNRegex": "^arn:aws:wellarchitected:.+",
             "Actions": [
                 "AssociateLenses",
                 "AssociateProfiles",
+                "ConfigureIntegration",
                 "CreateLensShare",
                 "CreateLensVersion",
                 "CreateMilestone",
                 "CreateProfile",
                 "CreateProfileShare",
                 "CreateReviewTemplate",
                 "CreateTemplateShare",
@@ -10746,14 +10752,15 @@
                 "DeleteWorkload",
                 "DeleteWorkloadShare",
                 "DisassociateLenses",
                 "DisassociateProfiles",
                 "ExportLens",
                 "GetAnswer",
                 "GetConsolidatedReport",
+                "GetGlobalSettings",
                 "GetLens",
                 "GetLensReview",
                 "GetLensReviewReport",
                 "GetLensVersionDifference",
                 "GetMilestone",
                 "GetProfile",
                 "GetProfileTemplate",
@@ -10781,14 +10788,15 @@
                 "ListTemplateShares",
                 "ListWorkloadShares",
                 "ListWorkloads",
                 "TagResource",
                 "UntagResource",
                 "UpdateAnswer",
                 "UpdateGlobalSettings",
+                "UpdateIntegration",
                 "UpdateLensReview",
                 "UpdateProfile",
                 "UpdateReviewTemplate",
                 "UpdateReviewTemplateAnswer",
                 "UpdateReviewTemplateLensReview",
                 "UpdateShareInvitation",
                 "UpdateWorkload",
@@ -10798,15 +10806,16 @@
                 "UpgradeReviewTemplateLensReview"
             ],
             "HasResource": true,
             "StringPrefix": "wellarchitected",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys"
+                "aws:TagKeys",
+                "wellarchitected:JiraProjectKey"
             ]
         },
         "AWS Wickr": {
             "ARNFormat": "arn:aws:wickr:${Region}:${Account}:${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:wickr:.+:.+:.+",
             "Actions": [
                 "CreateAdminSession",
@@ -14840,26 +14849,29 @@
         "Amazon EMR on EKS (EMR Containers)": {
             "ARNFormat": "arn:aws:emr-containers:${Region}:${Account}:/${ResourceType}/${ResourcePath}",
             "ARNRegex": "^arn:aws:emr-containers:.+",
             "Actions": [
                 "CancelJobRun",
                 "CreateJobTemplate",
                 "CreateManagedEndpoint",
+                "CreateSecurityConfiguration",
                 "CreateVirtualCluster",
                 "DeleteJobTemplate",
                 "DeleteManagedEndpoint",
                 "DeleteVirtualCluster",
                 "DescribeJobRun",
                 "DescribeJobTemplate",
                 "DescribeManagedEndpoint",
+                "DescribeSecurityConfiguration",
                 "DescribeVirtualCluster",
                 "GetManagedEndpointSessionCredentials",
                 "ListJobRuns",
                 "ListJobTemplates",
                 "ListManagedEndpoints",
+                "ListSecurityConfigurations",
                 "ListTagsForResource",
                 "ListVirtualClusters",
                 "StartJobRun",
                 "TagResource",
                 "UntagResource"
             ],
             "HasResource": true,
```

### Comparing `iam_actions-1.2.20240416/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240417/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240416/iam_actions/services.json` & `iam_actions-1.2.20240417/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999387771554985%*

 * *Differences: {"'emr-containers'": "{'Actions': {insert: [(3, 'CreateSecurityConfiguration'), (11, "*

 * *                     "'DescribeSecurityConfiguration'), (17, 'ListSecurityConfigurations')]}}",*

 * * "'outposts'": "{'Actions': {insert: [(0, 'CancelCapacityTask'), (8, 'GetCapacityTask'), (14, "*

 * *               "'GetOutpostSupportedInstanceTypes'), (19, 'ListCapacityTasks'), (25, "*

 * *               "'StartCapacityTask')]}}",*

 * * "'wellarchitected'": "{'Actions': {insert: [(2, 'ConfigureIntegration'), (25, "*

 * *                      " […]*

```diff
@@ -9052,26 +9052,29 @@
         "ARNRegexes": [
             "^arn:aws:emr-containers:.+"
         ],
         "Actions": [
             "CancelJobRun",
             "CreateJobTemplate",
             "CreateManagedEndpoint",
+            "CreateSecurityConfiguration",
             "CreateVirtualCluster",
             "DeleteJobTemplate",
             "DeleteManagedEndpoint",
             "DeleteVirtualCluster",
             "DescribeJobRun",
             "DescribeJobTemplate",
             "DescribeManagedEndpoint",
+            "DescribeSecurityConfiguration",
             "DescribeVirtualCluster",
             "GetManagedEndpointSessionCredentials",
             "ListJobRuns",
             "ListJobTemplates",
             "ListManagedEndpoints",
+            "ListSecurityConfigurations",
             "ListTagsForResource",
             "ListVirtualClusters",
             "StartJobRun",
             "TagResource",
             "UntagResource"
         ],
         "ConditionKeys": [
@@ -16600,35 +16603,40 @@
         "ARNFormats": [
             "arn:aws:outposts:${Region}:${Account}:${ResourceType}/${ResourceName}"
         ],
         "ARNRegexes": [
             "^arn:aws:outposts:.+"
         ],
         "Actions": [
+            "CancelCapacityTask",
             "CancelOrder",
             "CreateOrder",
             "CreateOutpost",
             "CreatePrivateConnectivityConfig",
             "CreateSite",
             "DeleteOutpost",
             "DeleteSite",
+            "GetCapacityTask",
             "GetCatalogItem",
             "GetConnection",
             "GetOrder",
             "GetOutpost",
             "GetOutpostInstanceTypes",
+            "GetOutpostSupportedInstanceTypes",
             "GetPrivateConnectivityConfig",
             "GetSite",
             "GetSiteAddress",
             "ListAssets",
+            "ListCapacityTasks",
             "ListCatalogItems",
             "ListOrders",
             "ListOutposts",
             "ListSites",
             "ListTagsForResource",
+            "StartCapacityTask",
             "StartConnection",
             "TagResource",
             "UntagResource",
             "UpdateOutpost",
             "UpdateSite",
             "UpdateSiteAddress",
             "UpdateSiteRackPhysicalProperties"
@@ -23576,14 +23584,15 @@
         ],
         "ARNRegexes": [
             "^arn:aws:wellarchitected:.+"
         ],
         "Actions": [
             "AssociateLenses",
             "AssociateProfiles",
+            "ConfigureIntegration",
             "CreateLensShare",
             "CreateLensVersion",
             "CreateMilestone",
             "CreateProfile",
             "CreateProfileShare",
             "CreateReviewTemplate",
             "CreateTemplateShare",
@@ -23598,14 +23607,15 @@
             "DeleteWorkload",
             "DeleteWorkloadShare",
             "DisassociateLenses",
             "DisassociateProfiles",
             "ExportLens",
             "GetAnswer",
             "GetConsolidatedReport",
+            "GetGlobalSettings",
             "GetLens",
             "GetLensReview",
             "GetLensReviewReport",
             "GetLensVersionDifference",
             "GetMilestone",
             "GetProfile",
             "GetProfileTemplate",
@@ -23633,14 +23643,15 @@
             "ListTemplateShares",
             "ListWorkloadShares",
             "ListWorkloads",
             "TagResource",
             "UntagResource",
             "UpdateAnswer",
             "UpdateGlobalSettings",
+            "UpdateIntegration",
             "UpdateLensReview",
             "UpdateProfile",
             "UpdateReviewTemplate",
             "UpdateReviewTemplateAnswer",
             "UpdateReviewTemplateLensReview",
             "UpdateShareInvitation",
             "UpdateWorkload",
@@ -23648,15 +23659,16 @@
             "UpgradeLensReview",
             "UpgradeProfileVersion",
             "UpgradeReviewTemplateLensReview"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
-            "aws:TagKeys"
+            "aws:TagKeys",
+            "wellarchitected:JiraProjectKey"
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS Well-Architected Tool"
         ]
     },
     "wickr": {
```

### Comparing `iam_actions-1.2.20240416/pyproject.toml` & `iam_actions-1.2.20240417/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240416"
+version = "1.2.20240417"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240416/setup.py` & `iam_actions-1.2.20240417/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240416',
+    'version': '1.2.20240417',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240416/PKG-INFO` & `iam_actions-1.2.20240417/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240416
+Version: 1.2.20240417
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

