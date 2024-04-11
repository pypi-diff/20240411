# Comparing `tmp/mypy-boto3-batch-1.34.72.tar.gz` & `tmp/mypy-boto3-batch-1.34.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-batch-1.34.72.tar", last modified: Wed Mar 27 19:47:05 2024, max compression
+gzip compressed data, was "mypy-boto3-batch-1.34.83.tar", last modified: Thu Apr 11 19:18:05 2024, max compression
```

## Comparing `mypy-boto3-batch-1.34.72.tar` & `mypy-boto3-batch-1.34.83.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:47:05.046887 mypy-boto3-batch-1.34.72/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-27 19:46:44.000000 mypy-boto3-batch-1.34.72/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-03-27 19:47:05.046887 mypy-boto3-batch-1.34.72/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11658 2024-03-27 19:46:44.000000 mypy-boto3-batch-1.34.72/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:47:05.046887 mypy-boto3-batch-1.34.72/mypy_boto3_batch/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-27 19:46:44.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-27 19:46:44.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-27 19:46:44.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20910 2024-03-27 19:46:44.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20907 2024-03-27 19:46:44.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-03-27 19:46:45.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-03-27 19:46:45.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-03-27 19:46:44.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-03-27 19:46:44.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 19:46:44.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    50019 2024-03-27 19:46:46.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    50019 2024-03-27 19:46:46.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-27 19:46:44.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:47:05.046887 mypy-boto3-batch-1.34.72/mypy_boto3_batch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-03-27 19:47:05.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-27 19:47:05.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:47:05.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:47:05.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-27 19:47:05.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-27 19:47:05.000000 mypy-boto3-batch-1.34.72/mypy_boto3_batch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 19:47:05.046887 mypy-boto3-batch-1.34.72/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-03-27 19:46:44.000000 mypy-boto3-batch-1.34.72/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:05.679390 mypy-boto3-batch-1.34.83/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 19:17:07.000000 mypy-boto3-batch-1.34.83/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-04-11 19:18:05.679390 mypy-boto3-batch-1.34.83/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11658 2024-04-11 19:17:07.000000 mypy-boto3-batch-1.34.83/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:05.675390 mypy-boto3-batch-1.34.83/mypy_boto3_batch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-11 19:17:07.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-11 19:17:07.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-11 19:17:07.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20910 2024-04-11 19:17:07.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20907 2024-04-11 19:17:07.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11661 2024-04-11 19:17:07.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11661 2024-04-11 19:17:07.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-04-11 19:17:07.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-11 19:17:07.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:17:07.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    50792 2024-04-11 19:17:09.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50792 2024-04-11 19:17:08.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 19:17:07.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:05.679390 mypy-boto3-batch-1.34.83/mypy_boto3_batch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-04-11 19:18:05.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-11 19:18:05.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:05.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:05.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 19:18:05.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 19:18:05.000000 mypy-boto3-batch-1.34.83/mypy_boto3_batch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:18:05.679390 mypy-boto3-batch-1.34.83/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-11 19:17:07.000000 mypy-boto3-batch-1.34.83/setup.py
```

### Comparing `mypy-boto3-batch-1.34.72/LICENSE` & `mypy-boto3-batch-1.34.83/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.34.72/PKG-INFO` & `mypy-boto3-batch-1.34.83/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-batch
-Version: 1.34.72
-Summary: Type annotations for boto3.Batch 1.34.72 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.83
+Summary: Type annotations for boto3.Batch 1.34.83 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-batch)](https://pepy.tech/project/mypy-boto3-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Batch 1.34.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[boto3.Batch 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-batch-1.34.72/README.md` & `mypy-boto3-batch-1.34.83/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-batch)](https://pepy.tech/project/mypy-boto3-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Batch 1.34.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[boto3.Batch 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-batch-1.34.72/mypy_boto3_batch/__init__.py` & `mypy-boto3-batch-1.34.83/mypy_boto3_batch/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.34.72/mypy_boto3_batch/__init__.pyi` & `mypy-boto3-batch-1.34.83/mypy_boto3_batch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.34.72/mypy_boto3_batch/__main__.py` & `mypy-boto3-batch-1.34.83/mypy_boto3_batch/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Batch 1.34.72\n"
-        "Version:         1.34.72\n"
+        "Type annotations for boto3.Batch 1.34.83\n"
+        "Version:         1.34.83\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.72")
+    print("1.34.83")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-batch-1.34.72/mypy_boto3_batch/client.py` & `mypy-boto3-batch-1.34.83/mypy_boto3_batch/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.34.72/mypy_boto3_batch/client.pyi` & `mypy-boto3-batch-1.34.83/mypy_boto3_batch/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.34.72/mypy_boto3_batch/literals.py` & `mypy-boto3-batch-1.34.83/mypy_boto3_batch/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -175,24 +176,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
```

### Comparing `mypy-boto3-batch-1.34.72/mypy_boto3_batch/literals.pyi` & `mypy-boto3-batch-1.34.83/mypy_boto3_batch/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -175,24 +176,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
```

### Comparing `mypy-boto3-batch-1.34.72/mypy_boto3_batch/paginator.py` & `mypy-boto3-batch-1.34.83/mypy_boto3_batch/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.34.72/mypy_boto3_batch/paginator.pyi` & `mypy-boto3-batch-1.34.83/mypy_boto3_batch/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.34.72/mypy_boto3_batch/type_defs.py` & `mypy-boto3-batch-1.34.83/mypy_boto3_batch/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,14 +110,15 @@
     "SchedulingPolicyListingDetailTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TaskContainerDependencyTypeDef",
     "TerminateJobRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AttemptContainerDetailTypeDef",
+    "AttemptTaskContainerDetailsTypeDef",
     "ComputeResourcePaginatorTypeDef",
     "ComputeResourceTypeDef",
     "ComputeResourceUpdateTypeDef",
     "ContainerOverridesTypeDef",
     "TaskContainerOverridesTypeDef",
     "LogConfigurationTypeDef",
     "CreateComputeEnvironmentResponseTypeDef",
@@ -144,15 +145,15 @@
     "RetryStrategyTypeDef",
     "FairsharePolicyTypeDef",
     "JobSummaryTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
     "LinuxParametersTypeDef",
     "ListSchedulingPoliciesResponseTypeDef",
-    "AttemptDetailTypeDef",
+    "AttemptEcsTaskDetailsTypeDef",
     "ComputeEnvironmentDetailPaginatorTypeDef",
     "ComputeEnvironmentDetailTypeDef",
     "CreateComputeEnvironmentRequestRequestTypeDef",
     "UpdateComputeEnvironmentRequestRequestTypeDef",
     "TaskPropertiesOverrideTypeDef",
     "DescribeJobQueuesResponseTypeDef",
     "VolumeTypeDef",
@@ -161,14 +162,15 @@
     "EksPodPropertiesTypeDef",
     "CreateSchedulingPolicyRequestRequestTypeDef",
     "SchedulingPolicyDetailTypeDef",
     "UpdateSchedulingPolicyRequestRequestTypeDef",
     "ListJobsResponseTypeDef",
     "TaskContainerDetailsTypeDef",
     "TaskContainerPropertiesTypeDef",
+    "AttemptDetailTypeDef",
     "DescribeComputeEnvironmentsResponsePaginatorTypeDef",
     "DescribeComputeEnvironmentsResponseTypeDef",
     "EcsPropertiesOverrideTypeDef",
     "ContainerDetailTypeDef",
     "ContainerPropertiesTypeDef",
     "EksPropertiesOverrideTypeDef",
     "EksPropertiesDetailTypeDef",
@@ -441,14 +443,15 @@
         "accessPointId": NotRequired[str],
         "iam": NotRequired[EFSAuthorizationConfigIAMType],
     },
 )
 EksAttemptContainerDetailTypeDef = TypedDict(
     "EksAttemptContainerDetailTypeDef",
     {
+        "name": NotRequired[str],
         "exitCode": NotRequired[int],
         "reason": NotRequired[str],
     },
 )
 EksContainerEnvironmentVariableTypeDef = TypedDict(
     "EksContainerEnvironmentVariableTypeDef",
     {
@@ -633,14 +636,24 @@
         "taskArn": NotRequired[str],
         "exitCode": NotRequired[int],
         "reason": NotRequired[str],
         "logStreamName": NotRequired[str],
         "networkInterfaces": NotRequired[List[NetworkInterfaceTypeDef]],
     },
 )
+AttemptTaskContainerDetailsTypeDef = TypedDict(
+    "AttemptTaskContainerDetailsTypeDef",
+    {
+        "exitCode": NotRequired[int],
+        "name": NotRequired[str],
+        "reason": NotRequired[str],
+        "logStreamName": NotRequired[str],
+        "networkInterfaces": NotRequired[List[NetworkInterfaceTypeDef]],
+    },
+)
 ComputeResourcePaginatorTypeDef = TypedDict(
     "ComputeResourcePaginatorTypeDef",
     {
         "type": CRTypeType,
         "maxvCpus": int,
         "subnets": List[str],
         "allocationStrategy": NotRequired[CRAllocationStrategyType],
@@ -1005,21 +1018,20 @@
     "ListSchedulingPoliciesResponseTypeDef",
     {
         "schedulingPolicies": List[SchedulingPolicyListingDetailTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-AttemptDetailTypeDef = TypedDict(
-    "AttemptDetailTypeDef",
+AttemptEcsTaskDetailsTypeDef = TypedDict(
+    "AttemptEcsTaskDetailsTypeDef",
     {
-        "container": NotRequired[AttemptContainerDetailTypeDef],
-        "startedAt": NotRequired[int],
-        "stoppedAt": NotRequired[int],
-        "statusReason": NotRequired[str],
+        "containerInstanceArn": NotRequired[str],
+        "taskArn": NotRequired[str],
+        "containers": NotRequired[List[AttemptTaskContainerDetailsTypeDef]],
     },
 )
 ComputeEnvironmentDetailPaginatorTypeDef = TypedDict(
     "ComputeEnvironmentDetailPaginatorTypeDef",
     {
         "computeEnvironmentName": str,
         "computeEnvironmentArn": str,
@@ -1216,14 +1228,24 @@
         "repositoryCredentials": NotRequired[RepositoryCredentialsTypeDef],
         "resourceRequirements": NotRequired[List[ResourceRequirementTypeDef]],
         "secrets": NotRequired[List[SecretTypeDef]],
         "ulimits": NotRequired[List[UlimitTypeDef]],
         "user": NotRequired[str],
     },
 )
+AttemptDetailTypeDef = TypedDict(
+    "AttemptDetailTypeDef",
+    {
+        "container": NotRequired[AttemptContainerDetailTypeDef],
+        "startedAt": NotRequired[int],
+        "stoppedAt": NotRequired[int],
+        "statusReason": NotRequired[str],
+        "taskProperties": NotRequired[List[AttemptEcsTaskDetailsTypeDef]],
+    },
+)
 DescribeComputeEnvironmentsResponsePaginatorTypeDef = TypedDict(
     "DescribeComputeEnvironmentsResponsePaginatorTypeDef",
     {
         "computeEnvironments": List[ComputeEnvironmentDetailPaginatorTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-batch-1.34.72/mypy_boto3_batch/type_defs.pyi` & `mypy-boto3-batch-1.34.83/mypy_boto3_batch/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -110,14 +110,15 @@
     "SchedulingPolicyListingDetailTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TaskContainerDependencyTypeDef",
     "TerminateJobRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AttemptContainerDetailTypeDef",
+    "AttemptTaskContainerDetailsTypeDef",
     "ComputeResourcePaginatorTypeDef",
     "ComputeResourceTypeDef",
     "ComputeResourceUpdateTypeDef",
     "ContainerOverridesTypeDef",
     "TaskContainerOverridesTypeDef",
     "LogConfigurationTypeDef",
     "CreateComputeEnvironmentResponseTypeDef",
@@ -144,15 +145,15 @@
     "RetryStrategyTypeDef",
     "FairsharePolicyTypeDef",
     "JobSummaryTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
     "LinuxParametersTypeDef",
     "ListSchedulingPoliciesResponseTypeDef",
-    "AttemptDetailTypeDef",
+    "AttemptEcsTaskDetailsTypeDef",
     "ComputeEnvironmentDetailPaginatorTypeDef",
     "ComputeEnvironmentDetailTypeDef",
     "CreateComputeEnvironmentRequestRequestTypeDef",
     "UpdateComputeEnvironmentRequestRequestTypeDef",
     "TaskPropertiesOverrideTypeDef",
     "DescribeJobQueuesResponseTypeDef",
     "VolumeTypeDef",
@@ -161,14 +162,15 @@
     "EksPodPropertiesTypeDef",
     "CreateSchedulingPolicyRequestRequestTypeDef",
     "SchedulingPolicyDetailTypeDef",
     "UpdateSchedulingPolicyRequestRequestTypeDef",
     "ListJobsResponseTypeDef",
     "TaskContainerDetailsTypeDef",
     "TaskContainerPropertiesTypeDef",
+    "AttemptDetailTypeDef",
     "DescribeComputeEnvironmentsResponsePaginatorTypeDef",
     "DescribeComputeEnvironmentsResponseTypeDef",
     "EcsPropertiesOverrideTypeDef",
     "ContainerDetailTypeDef",
     "ContainerPropertiesTypeDef",
     "EksPropertiesOverrideTypeDef",
     "EksPropertiesDetailTypeDef",
@@ -441,14 +443,15 @@
         "accessPointId": NotRequired[str],
         "iam": NotRequired[EFSAuthorizationConfigIAMType],
     },
 )
 EksAttemptContainerDetailTypeDef = TypedDict(
     "EksAttemptContainerDetailTypeDef",
     {
+        "name": NotRequired[str],
         "exitCode": NotRequired[int],
         "reason": NotRequired[str],
     },
 )
 EksContainerEnvironmentVariableTypeDef = TypedDict(
     "EksContainerEnvironmentVariableTypeDef",
     {
@@ -633,14 +636,24 @@
         "taskArn": NotRequired[str],
         "exitCode": NotRequired[int],
         "reason": NotRequired[str],
         "logStreamName": NotRequired[str],
         "networkInterfaces": NotRequired[List[NetworkInterfaceTypeDef]],
     },
 )
+AttemptTaskContainerDetailsTypeDef = TypedDict(
+    "AttemptTaskContainerDetailsTypeDef",
+    {
+        "exitCode": NotRequired[int],
+        "name": NotRequired[str],
+        "reason": NotRequired[str],
+        "logStreamName": NotRequired[str],
+        "networkInterfaces": NotRequired[List[NetworkInterfaceTypeDef]],
+    },
+)
 ComputeResourcePaginatorTypeDef = TypedDict(
     "ComputeResourcePaginatorTypeDef",
     {
         "type": CRTypeType,
         "maxvCpus": int,
         "subnets": List[str],
         "allocationStrategy": NotRequired[CRAllocationStrategyType],
@@ -1005,21 +1018,20 @@
     "ListSchedulingPoliciesResponseTypeDef",
     {
         "schedulingPolicies": List[SchedulingPolicyListingDetailTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-AttemptDetailTypeDef = TypedDict(
-    "AttemptDetailTypeDef",
+AttemptEcsTaskDetailsTypeDef = TypedDict(
+    "AttemptEcsTaskDetailsTypeDef",
     {
-        "container": NotRequired[AttemptContainerDetailTypeDef],
-        "startedAt": NotRequired[int],
-        "stoppedAt": NotRequired[int],
-        "statusReason": NotRequired[str],
+        "containerInstanceArn": NotRequired[str],
+        "taskArn": NotRequired[str],
+        "containers": NotRequired[List[AttemptTaskContainerDetailsTypeDef]],
     },
 )
 ComputeEnvironmentDetailPaginatorTypeDef = TypedDict(
     "ComputeEnvironmentDetailPaginatorTypeDef",
     {
         "computeEnvironmentName": str,
         "computeEnvironmentArn": str,
@@ -1216,14 +1228,24 @@
         "repositoryCredentials": NotRequired[RepositoryCredentialsTypeDef],
         "resourceRequirements": NotRequired[List[ResourceRequirementTypeDef]],
         "secrets": NotRequired[List[SecretTypeDef]],
         "ulimits": NotRequired[List[UlimitTypeDef]],
         "user": NotRequired[str],
     },
 )
+AttemptDetailTypeDef = TypedDict(
+    "AttemptDetailTypeDef",
+    {
+        "container": NotRequired[AttemptContainerDetailTypeDef],
+        "startedAt": NotRequired[int],
+        "stoppedAt": NotRequired[int],
+        "statusReason": NotRequired[str],
+        "taskProperties": NotRequired[List[AttemptEcsTaskDetailsTypeDef]],
+    },
+)
 DescribeComputeEnvironmentsResponsePaginatorTypeDef = TypedDict(
     "DescribeComputeEnvironmentsResponsePaginatorTypeDef",
     {
         "computeEnvironments": List[ComputeEnvironmentDetailPaginatorTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-batch-1.34.72/mypy_boto3_batch.egg-info/PKG-INFO` & `mypy-boto3-batch-1.34.83/mypy_boto3_batch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-batch
-Version: 1.34.72
-Summary: Type annotations for boto3.Batch 1.34.72 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.83
+Summary: Type annotations for boto3.Batch 1.34.83 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-batch)](https://pepy.tech/project/mypy-boto3-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Batch 1.34.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[boto3.Batch 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-batch-1.34.72/mypy_boto3_batch.egg-info/SOURCES.txt` & `mypy-boto3-batch-1.34.83/mypy_boto3_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.34.72/setup.py` & `mypy-boto3-batch-1.34.83/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-batch",
-    version="1.34.72",
+    version="1.34.83",
     packages=["mypy_boto3_batch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Batch 1.34.72 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.Batch 1.34.83 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

