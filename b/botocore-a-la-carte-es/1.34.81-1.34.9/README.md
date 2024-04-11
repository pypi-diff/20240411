# Comparing `tmp/botocore-a-la-carte-es-1.34.81.tar.gz` & `tmp/botocore-a-la-carte-es-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-es-1.34.81.tar", last modified: Wed Apr 10 01:00:03 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-es-1.34.9.tar", last modified: Thu Dec 28 01:06:45 2023, max compression
```

## Comparing `botocore-a-la-carte-es-1.34.81.tar` & `botocore-a-la-carte-es-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:03.848250 botocore-a-la-carte-es-1.34.81/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-10 01:00:03.000000 botocore-a-la-carte-es-1.34.81/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-10 01:00:03.848250 botocore-a-la-carte-es-1.34.81/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:03.844250 botocore-a-la-carte-es-1.34.81/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:03.844250 botocore-a-la-carte-es-1.34.81/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:03.844250 botocore-a-la-carte-es-1.34.81/botocore/data/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:03.844250 botocore-a-la-carte-es-1.34.81/botocore/data/es/2015-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-04-10 00:59:41.000000 botocore-a-la-carte-es-1.34.81/botocore/data/es/2015-01-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 00:59:41.000000 botocore-a-la-carte-es-1.34.81/botocore/data/es/2015-01-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-10 00:59:41.000000 botocore-a-la-carte-es-1.34.81/botocore/data/es/2015-01-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   220049 2024-04-10 00:59:41.000000 botocore-a-la-carte-es-1.34.81/botocore/data/es/2015-01-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:03.848250 botocore-a-la-carte-es-1.34.81/botocore_a_la_carte_es.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-10 01:00:03.000000 botocore-a-la-carte-es-1.34.81/botocore_a_la_carte_es.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-10 01:00:03.000000 botocore-a-la-carte-es-1.34.81/botocore_a_la_carte_es.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 01:00:03.000000 botocore-a-la-carte-es-1.34.81/botocore_a_la_carte_es.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 01:00:03.000000 botocore-a-la-carte-es-1.34.81/botocore_a_la_carte_es.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 01:00:03.848250 botocore-a-la-carte-es-1.34.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-10 01:00:03.000000 botocore-a-la-carte-es-1.34.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:45.174306 botocore-a-la-carte-es-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:44.000000 botocore-a-la-carte-es-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2023-12-28 01:06:45.174306 botocore-a-la-carte-es-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:45.170305 botocore-a-la-carte-es-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:45.170305 botocore-a-la-carte-es-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:45.170305 botocore-a-la-carte-es-1.34.9/botocore/data/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:45.174306 botocore-a-la-carte-es-1.34.9/botocore/data/es/2015-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)    13710 2023-12-28 01:06:26.000000 botocore-a-la-carte-es-1.34.9/botocore/data/es/2015-01-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-es-1.34.9/botocore/data/es/2015-01-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-12-28 01:06:26.000000 botocore-a-la-carte-es-1.34.9/botocore/data/es/2015-01-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   213004 2023-12-28 01:06:26.000000 botocore-a-la-carte-es-1.34.9/botocore/data/es/2015-01-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:45.174306 botocore-a-la-carte-es-1.34.9/botocore_a_la_carte_es.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2023-12-28 01:06:45.000000 botocore-a-la-carte-es-1.34.9/botocore_a_la_carte_es.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-12-28 01:06:45.000000 botocore-a-la-carte-es-1.34.9/botocore_a_la_carte_es.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:45.000000 botocore-a-la-carte-es-1.34.9/botocore_a_la_carte_es.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:45.000000 botocore-a-la-carte-es-1.34.9/botocore_a_la_carte_es.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:45.174306 botocore-a-la-carte-es-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-12-28 01:06:44.000000 botocore-a-la-carte-es-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-es-1.34.81/LICENSE.txt` & `botocore-a-la-carte-es-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-es-1.34.81/PKG-INFO` & `botocore-a-la-carte-es-1.34.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-es
-Version: 1.34.81
+Version: 1.34.9
 Summary: es data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-es-1.34.81/botocore/data/es/2015-01-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-es-1.34.9/botocore/data/es/2015-01-01/endpoint-rule-set-1.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999950881630086%*

 * *Differences: {"'rules'": "{1: {'rules': {0: {'rules': {1: {'rules': {0: {'conditions': {0: {'argv': {insert: "*

 * *            "[(1, OrderedDict([('fn', 'getAttr'), ('argv', [OrderedDict([('ref', "*

 * *            "'PartitionResult')]), 'supportsFIPS'])]))], delete: [0]}}}}}}, 2: {'rules': {0: "*

 * *            "{'rules': {delete: [2, 1, 0]}}}}}}}}}"}*

```diff
@@ -198,24 +198,24 @@
                                 }
                             ],
                             "rules": [
                                 {
                                     "conditions": [
                                         {
                                             "argv": [
+                                                true,
                                                 {
                                                     "argv": [
                                                         {
                                                             "ref": "PartitionResult"
                                                         },
                                                         "supportsFIPS"
                                                     ],
                                                     "fn": "getAttr"
-                                                },
-                                                true
+                                                }
                                             ],
                                             "fn": "booleanEquals"
                                         }
                                     ],
                                     "rules": [
                                         {
                                             "conditions": [],
@@ -266,89 +266,14 @@
                                                 }
                                             ],
                                             "fn": "booleanEquals"
                                         }
                                     ],
                                     "rules": [
                                         {
-                                            "conditions": [
-                                                {
-                                                    "argv": [
-                                                        "aws",
-                                                        {
-                                                            "argv": [
-                                                                {
-                                                                    "ref": "PartitionResult"
-                                                                },
-                                                                "name"
-                                                            ],
-                                                            "fn": "getAttr"
-                                                        }
-                                                    ],
-                                                    "fn": "stringEquals"
-                                                }
-                                            ],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {},
-                                                "url": "https://aos.{Region}.api.aws"
-                                            },
-                                            "type": "endpoint"
-                                        },
-                                        {
-                                            "conditions": [
-                                                {
-                                                    "argv": [
-                                                        "aws-cn",
-                                                        {
-                                                            "argv": [
-                                                                {
-                                                                    "ref": "PartitionResult"
-                                                                },
-                                                                "name"
-                                                            ],
-                                                            "fn": "getAttr"
-                                                        }
-                                                    ],
-                                                    "fn": "stringEquals"
-                                                }
-                                            ],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {},
-                                                "url": "https://aos.{Region}.api.amazonwebservices.com.cn"
-                                            },
-                                            "type": "endpoint"
-                                        },
-                                        {
-                                            "conditions": [
-                                                {
-                                                    "argv": [
-                                                        "aws-us-gov",
-                                                        {
-                                                            "argv": [
-                                                                {
-                                                                    "ref": "PartitionResult"
-                                                                },
-                                                                "name"
-                                                            ],
-                                                            "fn": "getAttr"
-                                                        }
-                                                    ],
-                                                    "fn": "stringEquals"
-                                                }
-                                            ],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {},
-                                                "url": "https://aos.{Region}.api.aws"
-                                            },
-                                            "type": "endpoint"
-                                        },
-                                        {
                                             "conditions": [],
                                             "endpoint": {
                                                 "headers": {},
                                                 "properties": {},
                                                 "url": "https://es.{Region}.{PartitionResult#dualStackDnsSuffix}"
                                             },
                                             "type": "endpoint"
```

### Comparing `botocore-a-la-carte-es-1.34.81/botocore/data/es/2015-01-01/paginators-1.json` & `botocore-a-la-carte-es-1.34.9/botocore/data/es/2015-01-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-es-1.34.81/botocore/data/es/2015-01-01/service-2.json` & `botocore-a-la-carte-es-1.34.9/botocore/data/es/2015-01-01/service-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99478361816624%*

 * *Differences: {"'operations'": "{delete: ['CancelDomainConfigChange']}",*

 * * "'shapes'": "{'ChangeProgressDetails': {'members': {delete: ['ConfigChangeStatus', 'StartTime', "*

 * *             "'LastUpdatedTime', 'InitiatedBy']}}, 'ChangeProgressStatusDetails': {'members': "*

 * *             "{delete: ['ConfigChangeStatus', 'LastUpdatedTime', 'InitiatedBy']}}, "*

 * *             "'DomainEndpointOptions': {'members': {'TLSSecurityPolicy': {'documentation': "*

 * *             "'<p>Specify the TLS security policy that needs to be applied to th […]*

```diff
@@ -124,45 +124,14 @@
                 "shape": "AuthorizeVpcEndpointAccessRequest"
             },
             "name": "AuthorizeVpcEndpointAccess",
             "output": {
                 "shape": "AuthorizeVpcEndpointAccessResponse"
             }
         },
-        "CancelDomainConfigChange": {
-            "documentation": "<p>Cancels a pending configuration change on an Amazon OpenSearch Service domain.</p>",
-            "errors": [
-                {
-                    "shape": "BaseException"
-                },
-                {
-                    "shape": "InternalException"
-                },
-                {
-                    "shape": "ResourceNotFoundException"
-                },
-                {
-                    "shape": "ValidationException"
-                },
-                {
-                    "shape": "DisabledOperationException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/2015-01-01/es/domain/{DomainName}/config/cancel"
-            },
-            "input": {
-                "shape": "CancelDomainConfigChangeRequest"
-            },
-            "name": "CancelDomainConfigChange",
-            "output": {
-                "shape": "CancelDomainConfigChangeResponse"
-            }
-        },
         "CancelElasticsearchServiceSoftwareUpdate": {
             "documentation": "<p>Cancels a scheduled service software update for an Amazon ES domain. You can only perform this operation before the <code>AutomatedUpdateDate</code> and when the <code>UpdateStatus</code> is in the <code>PENDING_UPDATE</code> state.</p>",
             "errors": [
                 {
                     "shape": "BaseException"
                 },
                 {
@@ -1967,51 +1936,14 @@
                 }
             },
             "type": "structure"
         },
         "Boolean": {
             "type": "boolean"
         },
-        "CancelDomainConfigChangeRequest": {
-            "documentation": "<p>Container for parameters of the <code>CancelDomainConfigChange</code> operation.</p>",
-            "members": {
-                "DomainName": {
-                    "documentation": "<p>Name of the OpenSearch Service domain configuration request to cancel.</p>",
-                    "location": "uri",
-                    "locationName": "DomainName",
-                    "shape": "DomainName"
-                },
-                "DryRun": {
-                    "documentation": "<p>When set to <b>True</b>, returns the list of change IDs and properties that will be cancelled without actually cancelling the change.</p>",
-                    "shape": "DryRun"
-                }
-            },
-            "required": [
-                "DomainName"
-            ],
-            "type": "structure"
-        },
-        "CancelDomainConfigChangeResponse": {
-            "documentation": "<p>Contains the details of the cancelled domain config change.</p>",
-            "members": {
-                "CancelledChangeIds": {
-                    "documentation": "<p>The unique identifiers of the changes that were cancelled.</p>",
-                    "shape": "GUIDList"
-                },
-                "CancelledChangeProperties": {
-                    "documentation": "<p>The domain change properties that were cancelled.</p>",
-                    "shape": "CancelledChangePropertyList"
-                },
-                "DryRun": {
-                    "documentation": "<p>Whether or not the request was a dry run. If <b>True</b>, the changes were not actually cancelled.</p>",
-                    "shape": "DryRun"
-                }
-            },
-            "type": "structure"
-        },
         "CancelElasticsearchServiceSoftwareUpdateRequest": {
             "documentation": "<p>Container for the parameters to the <code><a>CancelElasticsearchServiceSoftwareUpdate</a></code> operation. Specifies the name of the Elasticsearch domain that you wish to cancel a service software update on.</p>",
             "members": {
                 "DomainName": {
                     "documentation": "<p>The name of the domain that you want to stop the latest service software update on.</p>",
                     "shape": "DomainName"
                 }
@@ -2027,64 +1959,24 @@
                 "ServiceSoftwareOptions": {
                     "documentation": "<p>The current status of the Elasticsearch service software update.</p>",
                     "shape": "ServiceSoftwareOptions"
                 }
             },
             "type": "structure"
         },
-        "CancelledChangeProperty": {
-            "documentation": "<p>A property change that was cancelled for an Amazon OpenSearch Service domain.</p>",
-            "members": {
-                "ActiveValue": {
-                    "documentation": "<p>The current value of the property, after the change was cancelled.</p>",
-                    "shape": "String"
-                },
-                "CancelledValue": {
-                    "documentation": "<p>The pending value of the property that was cancelled. This would have been the eventual value of the property if the chance had not been cancelled.</p>",
-                    "shape": "String"
-                },
-                "PropertyName": {
-                    "documentation": "<p>The name of the property whose change was cancelled.</p>",
-                    "shape": "String"
-                }
-            },
-            "type": "structure"
-        },
-        "CancelledChangePropertyList": {
-            "member": {
-                "shape": "CancelledChangeProperty"
-            },
-            "type": "list"
-        },
         "ChangeProgressDetails": {
             "documentation": "<p>Specifies change details of the domain configuration change.</p>",
             "members": {
                 "ChangeId": {
                     "documentation": "<p>The unique change identifier associated with a specific domain configuration change.</p>",
                     "shape": "GUID"
                 },
-                "ConfigChangeStatus": {
-                    "documentation": "<p>The current status of the configuration change.</p>",
-                    "shape": "ConfigChangeStatus"
-                },
-                "InitiatedBy": {
-                    "documentation": "<p>The IAM principal who initiated the configuration change.</p>",
-                    "shape": "InitiatedBy"
-                },
-                "LastUpdatedTime": {
-                    "documentation": "<p>The last time that the configuration change was updated.</p>",
-                    "shape": "UpdateTimestamp"
-                },
                 "Message": {
                     "documentation": "<p>Contains an optional message associated with the domain configuration change.</p>",
                     "shape": "Message"
-                },
-                "StartTime": {
-                    "documentation": "<p>The time that the configuration change was initiated, in Universal Coordinated Time (UTC).</p>",
-                    "shape": "UpdateTimestamp"
                 }
             },
             "type": "structure"
         },
         "ChangeProgressStage": {
             "documentation": "<p>A progress stage details of a specific domain configuration change.</p>",
             "members": {
@@ -2135,26 +2027,14 @@
                     "documentation": "<p>The specific stages that the domain is going through to perform the configuration change.</p>",
                     "shape": "ChangeProgressStageList"
                 },
                 "CompletedProperties": {
                     "documentation": "<p>The list of properties involved in the domain configuration change that are completed.</p>",
                     "shape": "StringList"
                 },
-                "ConfigChangeStatus": {
-                    "documentation": "<p>The current status of the configuration change.</p>",
-                    "shape": "ConfigChangeStatus"
-                },
-                "InitiatedBy": {
-                    "documentation": "<p>The IAM principal who initiated the configuration change.</p>",
-                    "shape": "InitiatedBy"
-                },
-                "LastUpdatedTime": {
-                    "documentation": "<p>The last time that the status of the configuration change was updated.</p>",
-                    "shape": "UpdateTimestamp"
-                },
                 "PendingProperties": {
                     "documentation": "<p>The list of properties involved in the domain configuration change that are still in pending.</p>",
                     "shape": "StringList"
                 },
                 "StartTime": {
                     "documentation": "<p>The time at which the configuration change is made on the domain.</p>",
                     "shape": "UpdateTimestamp"
@@ -2251,27 +2131,14 @@
                 },
                 "TargetVersions": {
                     "shape": "ElasticsearchVersionList"
                 }
             },
             "type": "structure"
         },
-        "ConfigChangeStatus": {
-            "enum": [
-                "Pending",
-                "Initializing",
-                "Validating",
-                "ValidationFailed",
-                "ApplyingChanges",
-                "Completed",
-                "PendingUserInput",
-                "Cancelled"
-            ],
-            "type": "string"
-        },
         "ConflictException": {
             "documentation": "<p>An error occurred because the client attempts to remove a resource that is currently in use. Returns HTTP status code 409.</p>",
             "error": {
                 "httpStatusCode": 409
             },
             "exception": true,
             "members": {},
@@ -3137,15 +3004,15 @@
                     "shape": "Boolean"
                 },
                 "EnforceHTTPS": {
                     "documentation": "<p>Specify if only HTTPS endpoint should be enabled for the Elasticsearch domain.</p>",
                     "shape": "Boolean"
                 },
                 "TLSSecurityPolicy": {
-                    "documentation": "<p>Specify the TLS security policy that needs to be applied to the HTTPS endpoint of Elasticsearch domain. <br/> It can be one of the following values: <ul> <li><b>Policy-Min-TLS-1-0-2019-07: </b> TLS security policy that supports TLS version 1.0 to TLS version 1.2</li> <li><b>Policy-Min-TLS-1-2-2019-07: </b> TLS security policy that supports only TLS version 1.2</li> <li><b>Policy-Min-TLS-1-2-PFS-2023-10: </b> TLS security policy that supports TLS version 1.2 to TLS version 1.3 with perfect forward secrecy cipher suites</li> </ul> </p>",
+                    "documentation": "<p>Specify the TLS security policy that needs to be applied to the HTTPS endpoint of Elasticsearch domain. <br/> It can be one of the following values: <ul> <li><b>Policy-Min-TLS-1-0-2019-07: </b> TLS security policy which supports TLSv1.0 and higher.</li> <li><b>Policy-Min-TLS-1-2-2019-07: </b> TLS security policy which supports only TLSv1.2</li> </ul> </p>",
                     "shape": "TLSSecurityPolicy"
                 }
             },
             "type": "structure"
         },
         "DomainEndpointOptionsStatus": {
             "documentation": "<p>The configured endpoint options for the domain and their current status.</p>",
@@ -3281,26 +3148,14 @@
                 "ASSOCIATION_FAILED",
                 "ACTIVE",
                 "DISSOCIATING",
                 "DISSOCIATION_FAILED"
             ],
             "type": "string"
         },
-        "DomainProcessingStatusType": {
-            "enum": [
-                "Creating",
-                "Active",
-                "Modifying",
-                "UpgradingEngineVersion",
-                "UpdatingServiceSoftware",
-                "Isolated",
-                "Deleting"
-            ],
-            "type": "string"
-        },
         "Double": {
             "type": "double"
         },
         "DryRun": {
             "type": "boolean"
         },
         "DryRunResults": {
@@ -3565,18 +3420,14 @@
                     "documentation": "<p>Specifies the <code>EncryptionAtRestOptions</code> for the Elasticsearch domain.</p>",
                     "shape": "EncryptionAtRestOptionsStatus"
                 },
                 "LogPublishingOptions": {
                     "documentation": "<p>Log publishing options for the given domain.</p>",
                     "shape": "LogPublishingOptionsStatus"
                 },
-                "ModifyingProperties": {
-                    "documentation": "<p>Information about the domain properties that are currently being modified.</p>",
-                    "shape": "ModifyingPropertiesList"
-                },
                 "NodeToNodeEncryptionOptions": {
                     "documentation": "<p>Specifies the <code>NodeToNodeEncryptionOptions</code> for the Elasticsearch domain.</p>",
                     "shape": "NodeToNodeEncryptionOptionsStatus"
                 },
                 "SnapshotOptions": {
                     "documentation": "<p>Specifies the <code>SnapshotOptions</code> for the Elasticsearch domain.</p>",
                     "shape": "SnapshotOptionsStatus"
@@ -3635,18 +3486,14 @@
                     "documentation": "<p>The unique identifier for the specified Elasticsearch domain.</p>",
                     "shape": "DomainId"
                 },
                 "DomainName": {
                     "documentation": "<p>The name of an Elasticsearch domain. Domain names are unique across the domains owned by an account within an AWS region. Domain names start with a letter or number and can contain the following characters: a-z (lowercase), 0-9, and - (hyphen).</p>",
                     "shape": "DomainName"
                 },
-                "DomainProcessingStatus": {
-                    "documentation": "<p>The status of any changes that are currently in progress for the domain.</p>",
-                    "shape": "DomainProcessingStatusType"
-                },
                 "EBSOptions": {
                     "documentation": "<p>The <code>EBSOptions</code> for the specified domain. See <a href=\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-createupdatedomains.html#es-createdomain-configure-ebs\" target=\"_blank\">Configuring EBS-based Storage</a> for more information.</p>",
                     "shape": "EBSOptions"
                 },
                 "ElasticsearchClusterConfig": {
                     "documentation": "<p>The type and number of instances in the domain cluster.</p>",
                     "shape": "ElasticsearchClusterConfig"
@@ -3666,18 +3513,14 @@
                     "documentation": "<p>Map containing the Elasticsearch domain endpoints used to submit index and search requests. Example <code>key, value</code>: <code>'vpc','vpc-endpoint-h2dsd34efgyghrtguk5gt6j2foh4.us-east-1.es.amazonaws.com'</code>.</p>",
                     "shape": "EndpointsMap"
                 },
                 "LogPublishingOptions": {
                     "documentation": "<p>Log publishing options for the given domain.</p>",
                     "shape": "LogPublishingOptions"
                 },
-                "ModifyingProperties": {
-                    "documentation": "<p>Information about the domain properties that are currently being modified.</p>",
-                    "shape": "ModifyingPropertiesList"
-                },
                 "NodeToNodeEncryptionOptions": {
                     "documentation": "<p>Specifies the status of the <code>NodeToNodeEncryptionOptions</code>.</p>",
                     "shape": "NodeToNodeEncryptionOptions"
                 },
                 "Processing": {
                     "documentation": "<p>The status of the Elasticsearch domain configuration. <code>True</code> if Amazon Elasticsearch Service is processing configuration changes. <code>False</code> if the configuration is active.</p>",
                     "shape": "Boolean"
@@ -3839,20 +3682,14 @@
             },
             "type": "list"
         },
         "GUID": {
             "pattern": "\\p{XDigit}{8}-\\p{XDigit}{4}-\\p{XDigit}{4}-\\p{XDigit}{4}-\\p{XDigit}{12}",
             "type": "string"
         },
-        "GUIDList": {
-            "member": {
-                "shape": "GUID"
-            },
-            "type": "list"
-        },
         "GetCompatibleElasticsearchVersionsRequest": {
             "documentation": "<p> Container for request parameters to <code> <a>GetCompatibleElasticsearchVersions</a> </code> operation. </p>",
             "members": {
                 "DomainName": {
                     "location": "querystring",
                     "locationName": "domainName",
                     "shape": "DomainName"
@@ -4038,21 +3875,14 @@
         },
         "InboundCrossClusterSearchConnections": {
             "member": {
                 "shape": "InboundCrossClusterSearchConnection"
             },
             "type": "list"
         },
-        "InitiatedBy": {
-            "enum": [
-                "CUSTOMER",
-                "SERVICE"
-            ],
-            "type": "string"
-        },
         "InstanceCount": {
             "documentation": "<p>Specifies the number of EC2 instances in the Elasticsearch domain.</p>",
             "min": 1,
             "type": "integer"
         },
         "InstanceCountLimits": {
             "documentation": "<p> InstanceCountLimits represents the limits on number of instances that be created in Amazon Elasticsearch for given InstanceType. </p>",
@@ -4566,42 +4396,14 @@
             "min": 0,
             "type": "string"
         },
         "MinimumInstanceCount": {
             "documentation": "<p> Minimum number of Instances that can be instantiated for given InstanceType. </p>",
             "type": "integer"
         },
-        "ModifyingProperties": {
-            "documentation": "<p>Information about the domain properties that are currently being modified.</p>",
-            "members": {
-                "ActiveValue": {
-                    "documentation": "<p>The current value of the domain property that is being modified.</p>",
-                    "shape": "String"
-                },
-                "Name": {
-                    "documentation": "<p>The name of the property that is currently being modified.</p>",
-                    "shape": "String"
-                },
-                "PendingValue": {
-                    "documentation": "<p>The value that the property that is currently being modified will eventually have.</p>",
-                    "shape": "String"
-                },
-                "ValueType": {
-                    "documentation": "<p>The type of value that is currently being modified. Properties can have two types:</p> <ul> <li><b>PLAIN_TEXT</b>: Contain direct values such as \"1\", \"True\", or \"c5.large.search\".</li> <li><b>STRINGIFIED_JSON</b>: Contain content in JSON format, such as {\"Enabled\":\"True\"}\".</li> </ul>",
-                    "shape": "PropertyValueType"
-                }
-            },
-            "type": "structure"
-        },
-        "ModifyingPropertiesList": {
-            "member": {
-                "shape": "ModifyingProperties"
-            },
-            "type": "list"
-        },
         "NextToken": {
             "documentation": "<p> Paginated APIs accepts NextToken input to returns next page results and provides a NextToken output in the response which can be used by the client to retrieve more results. </p>",
             "type": "string"
         },
         "NodeToNodeEncryptionOptions": {
             "documentation": "<p>Specifies the node-to-node encryption options.</p>",
             "members": {
@@ -4880,21 +4682,14 @@
             "documentation": "<p>Specifies the type of AWS account permitted to manage VPC endpoints.: <ul> <li>AWS_ACCOUNT: Indicates that the account is owned by an AWS user.</li> <li>AWS_SERVICE: Indicates the the account is owned by an AWS service.</li> </ul> </p>",
             "enum": [
                 "AWS_ACCOUNT",
                 "AWS_SERVICE"
             ],
             "type": "string"
         },
-        "PropertyValueType": {
-            "enum": [
-                "PLAIN_TEXT",
-                "STRINGIFIED_JSON"
-            ],
-            "type": "string"
-        },
         "PurchaseReservedElasticsearchInstanceOfferingRequest": {
             "documentation": "<p>Container for parameters to <code>PurchaseReservedElasticsearchInstanceOffering</code></p>",
             "members": {
                 "InstanceCount": {
                     "documentation": "<p>The number of Elasticsearch instances to reserve.</p>",
                     "shape": "InstanceCount"
                 },
@@ -5469,16 +5264,15 @@
                 "shape": "String"
             },
             "type": "list"
         },
         "TLSSecurityPolicy": {
             "enum": [
                 "Policy-Min-TLS-1-0-2019-07",
-                "Policy-Min-TLS-1-2-2019-07",
-                "Policy-Min-TLS-1-2-PFS-2023-10"
+                "Policy-Min-TLS-1-2-2019-07"
             ],
             "type": "string"
         },
         "Tag": {
             "documentation": "<p>Specifies a key value pair for a resource tag.</p>",
             "members": {
                 "Key": {
```

### Comparing `botocore-a-la-carte-es-1.34.81/botocore_a_la_carte_es.egg-info/PKG-INFO` & `botocore-a-la-carte-es-1.34.9/botocore_a_la_carte_es.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-es
-Version: 1.34.81
+Version: 1.34.9
 Summary: es data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-es-1.34.81/setup.py` & `botocore-a-la-carte-es-1.34.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-es',
-    version="1.34.81",
+    version="1.34.9",
     description='es data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/es/*/*.json'],
```

