# Comparing `tmp/iam_actions-1.2.20240409.tar.gz` & `tmp/iam_actions-1.2.20240410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240409.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240410.tar", max compression
```

## Comparing `iam_actions-1.2.20240409.tar` & `iam_actions-1.2.20240410.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-04-09 02:15:53.162940 iam_actions-1.2.20240409/LICENSE
--rw-r--r--   0        0        0     2302 2024-04-09 02:15:53.162940 iam_actions-1.2.20240409/README.md
--rw-r--r--   0        0        0      228 2024-04-09 02:15:53.162940 iam_actions-1.2.20240409/iam_actions/__init__.py
--rw-r--r--   0        0        0  4784341 2024-04-09 02:17:42.030314 iam_actions-1.2.20240409/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-04-09 02:15:53.162940 iam_actions-1.2.20240409/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-04-09 02:15:53.162940 iam_actions-1.2.20240409/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-04-09 02:15:53.162940 iam_actions-1.2.20240409/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-04-09 02:15:53.162940 iam_actions-1.2.20240409/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-04-09 02:15:53.162940 iam_actions-1.2.20240409/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-04-09 02:15:53.162940 iam_actions-1.2.20240409/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-04-09 02:15:53.162940 iam_actions-1.2.20240409/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-04-09 02:15:53.162940 iam_actions-1.2.20240409/iam_actions/generate/services.py
--rw-r--r--   0        0        0   622012 2024-04-09 02:17:42.030314 iam_actions-1.2.20240409/iam_actions/policies.json
--rw-r--r--   0        0        0   207247 2024-04-09 02:17:42.030314 iam_actions-1.2.20240409/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   603475 2024-04-09 02:17:42.030314 iam_actions-1.2.20240409/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-04-09 02:17:42.730310 iam_actions-1.2.20240409/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240409/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240409/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/LICENSE
+-rw-r--r--   0        0        0     2302 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/README.md
+-rw-r--r--   0        0        0      228 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4785181 2024-04-10 02:17:05.526347 iam_actions-1.2.20240410/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   622141 2024-04-10 02:17:05.526347 iam_actions-1.2.20240410/iam_actions/policies.json
+-rw-r--r--   0        0        0   207247 2024-04-10 02:17:05.526347 iam_actions-1.2.20240410/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   603579 2024-04-10 02:17:05.526347 iam_actions-1.2.20240410/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-04-10 02:17:06.182354 iam_actions-1.2.20240410/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240410/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240410/PKG-INFO
```

### Comparing `iam_actions-1.2.20240409/LICENSE` & `iam_actions-1.2.20240410/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240409/README.md` & `iam_actions-1.2.20240410/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240409/iam_actions/actions.json` & `iam_actions-1.2.20240410/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99996114996115%*

 * *Differences: {"'datazone'": "{'RemovePolicyGrant': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *               "'RemovePolicyGrant'), ('condition_keys', []), ('description', 'Not Documented by "*

 * *               "AWS'), ('orphan', False), ('resources', [])]), 'UpdateDataSourceRunActivities': "*

 * *               "OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *               "'UpdateDataSourceRunActivities'), ('condition_keys', []), ('description', 'Not "*

 * *               "Documented by AWS'), ('orpha […]*

```diff
@@ -40020,14 +40020,22 @@
             "access_level": "Undocumented",
             "action": "AcceptSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "AddPolicyGrant": {
+            "access_level": "Undocumented",
+            "action": "AddPolicyGrant",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CancelMetadataGenerationRun": {
             "access_level": "Undocumented",
             "action": "CancelMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -40668,14 +40676,22 @@
             "access_level": "Undocumented",
             "action": "ListNotifications",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "ListPolicyGrants": {
+            "access_level": "Undocumented",
+            "action": "ListPolicyGrants",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListProjectMemberships": {
             "access_level": "Undocumented",
             "action": "ListProjectMemberships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -40796,14 +40812,22 @@
             "access_level": "Undocumented",
             "action": "RejectSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "RemovePolicyGrant": {
+            "access_level": "Undocumented",
+            "action": "RemovePolicyGrant",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "RevokeSubscription": {
             "access_level": "Undocumented",
             "action": "RevokeSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -40908,14 +40932,22 @@
             "access_level": "Undocumented",
             "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "UpdateDataSourceRunActivities": {
+            "access_level": "Undocumented",
+            "action": "UpdateDataSourceRunActivities",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateDomain": {
             "access_level": "Undocumented",
             "action": "UpdateDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
```

### Comparing `iam_actions-1.2.20240409/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240410/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240409/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240410/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240409/iam_actions/generate/generate.py` & `iam_actions-1.2.20240410/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240409/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240410/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240409/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240410/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240409/iam_actions/generate/services.py` & `iam_actions-1.2.20240410/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240409/iam_actions/policies.json` & `iam_actions-1.2.20240410/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958330238661122%*

 * *Differences: {"'conditionKeys'": "{insert: [(21, 'aws:VpcSourceIp')]}",*

 * * "'serviceMap'": "{'Amazon DataZone': {'Actions': {insert: [(2, 'AddPolicyGrant'), (84, "*

 * *                 "'ListPolicyGrants'), (101, 'RemovePolicyGrant'), (116, "*

 * *                 "'UpdateDataSourceRunActivities')]}}}"}*

```diff
@@ -44,14 +44,15 @@
         "aws:SourceIp",
         "aws:SourceVpc",
         "aws:SourceVpce",
         "aws:TagKeys",
         "aws:TokenIssueTime",
         "aws:UserAgent",
         "aws:ViaAWSService",
+        "aws:VpcSourceIp",
         "aws:userid",
         "aws:username"
     ],
     "conditionOperators": [
         "ArnEquals",
         "ArnEqualsIfExists",
         "ArnLike",
@@ -13398,14 +13399,15 @@
         },
         "Amazon DataZone": {
             "ARNFormat": "arn:aws:datazone:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:datazone:.+:.+:.+",
             "Actions": [
                 "AcceptPredictions",
                 "AcceptSubscriptionRequest",
+                "AddPolicyGrant",
                 "CancelMetadataGenerationRun",
                 "CancelSubscription",
                 "CreateAsset",
                 "CreateAssetRevision",
                 "CreateAssetType",
                 "CreateDataSource",
                 "CreateDomain",
@@ -13479,14 +13481,15 @@
                 "ListEnvironmentBlueprintConfigurations",
                 "ListEnvironmentBlueprints",
                 "ListEnvironmentProfiles",
                 "ListEnvironments",
                 "ListGroupsForUser",
                 "ListMetadataGenerationRuns",
                 "ListNotifications",
+                "ListPolicyGrants",
                 "ListProjectMemberships",
                 "ListProjects",
                 "ListSubscriptionGrants",
                 "ListSubscriptionRequests",
                 "ListSubscriptionTargets",
                 "ListSubscriptions",
                 "ListTagsForResource",
@@ -13495,28 +13498,30 @@
                 "PostTimeSeriesDataPoints",
                 "ProvisionDomain",
                 "PutDomainSharingPolicy",
                 "PutEnvironmentBlueprintConfiguration",
                 "RefreshToken",
                 "RejectPredictions",
                 "RejectSubscriptionRequest",
+                "RemovePolicyGrant",
                 "RevokeSubscription",
                 "Search",
                 "SearchGroupProfiles",
                 "SearchListings",
                 "SearchTypes",
                 "SearchUserProfiles",
                 "SsoLogin",
                 "SsoLogout",
                 "StartDataSourceRun",
                 "StartMetadataGenerationRun",
                 "StopMetadataGenerationRun",
                 "TagResource",
                 "UntagResource",
                 "UpdateDataSource",
+                "UpdateDataSourceRunActivities",
                 "UpdateDomain",
                 "UpdateEnvironment",
                 "UpdateEnvironmentBlueprint",
                 "UpdateEnvironmentConfiguration",
                 "UpdateEnvironmentDeploymentStatus",
                 "UpdateEnvironmentProfile",
                 "UpdateGlossary",
```

### Comparing `iam_actions-1.2.20240409/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240410/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240409/iam_actions/services.json` & `iam_actions-1.2.20240410/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999967624967625%*

 * *Differences: {"'datazone'": "{'Actions': {insert: [(2, 'AddPolicyGrant'), (84, 'ListPolicyGrants'), (101, "*

 * *               "'RemovePolicyGrant'), (116, 'UpdateDataSourceRunActivities')]}}"}*

```diff
@@ -5955,14 +5955,15 @@
         ],
         "ARNRegexes": [
             "^arn:aws:datazone:.+:.+:.+"
         ],
         "Actions": [
             "AcceptPredictions",
             "AcceptSubscriptionRequest",
+            "AddPolicyGrant",
             "CancelMetadataGenerationRun",
             "CancelSubscription",
             "CreateAsset",
             "CreateAssetRevision",
             "CreateAssetType",
             "CreateDataSource",
             "CreateDomain",
@@ -6036,14 +6037,15 @@
             "ListEnvironmentBlueprintConfigurations",
             "ListEnvironmentBlueprints",
             "ListEnvironmentProfiles",
             "ListEnvironments",
             "ListGroupsForUser",
             "ListMetadataGenerationRuns",
             "ListNotifications",
+            "ListPolicyGrants",
             "ListProjectMemberships",
             "ListProjects",
             "ListSubscriptionGrants",
             "ListSubscriptionRequests",
             "ListSubscriptionTargets",
             "ListSubscriptions",
             "ListTagsForResource",
@@ -6052,28 +6054,30 @@
             "PostTimeSeriesDataPoints",
             "ProvisionDomain",
             "PutDomainSharingPolicy",
             "PutEnvironmentBlueprintConfiguration",
             "RefreshToken",
             "RejectPredictions",
             "RejectSubscriptionRequest",
+            "RemovePolicyGrant",
             "RevokeSubscription",
             "Search",
             "SearchGroupProfiles",
             "SearchListings",
             "SearchTypes",
             "SearchUserProfiles",
             "SsoLogin",
             "SsoLogout",
             "StartDataSourceRun",
             "StartMetadataGenerationRun",
             "StopMetadataGenerationRun",
             "TagResource",
             "UntagResource",
             "UpdateDataSource",
+            "UpdateDataSourceRunActivities",
             "UpdateDomain",
             "UpdateEnvironment",
             "UpdateEnvironmentBlueprint",
             "UpdateEnvironmentConfiguration",
             "UpdateEnvironmentDeploymentStatus",
             "UpdateEnvironmentProfile",
             "UpdateGlossary",
```

### Comparing `iam_actions-1.2.20240409/pyproject.toml` & `iam_actions-1.2.20240410/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240409"
+version = "1.2.20240410"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240409/setup.py` & `iam_actions-1.2.20240410/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240409',
+    'version': '1.2.20240410',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240409/PKG-INFO` & `iam_actions-1.2.20240410/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240409
+Version: 1.2.20240410
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

