# Comparing `tmp/mypy-boto3-s3control-1.34.18.tar.gz` & `tmp/mypy-boto3-s3control-1.34.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-s3control-1.34.18.tar", last modified: Fri Jan 12 21:05:17 2024, max compression
+gzip compressed data, was "mypy-boto3-s3control-1.34.83.tar", last modified: Thu Apr 11 19:18:08 2024, max compression
```

## Comparing `mypy-boto3-s3control-1.34.18.tar` & `mypy-boto3-s3control-1.34.83.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 21:05:17.431042 mypy-boto3-s3control-1.34.18/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-12 21:04:59.000000 mypy-boto3-s3control-1.34.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-01-12 21:05:17.431042 mypy-boto3-s3control-1.34.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-01-12 21:04:59.000000 mypy-boto3-s3control-1.34.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 21:05:17.431042 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-01-12 21:04:59.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-01-12 21:04:59.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-01-12 21:04:59.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57457 2024-01-12 21:05:01.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    57454 2024-01-12 21:05:00.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14525 2024-01-12 21:05:01.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14525 2024-01-12 21:05:01.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-01-12 21:05:01.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-01-12 21:05:01.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 21:04:59.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    80721 2024-01-12 21:05:02.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    80721 2024-01-12 21:05:02.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-12 21:04:59.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 21:05:17.431042 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-01-12 21:05:17.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-01-12 21:05:17.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 21:05:17.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 21:05:17.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-12 21:05:17.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-12 21:05:17.000000 mypy-boto3-s3control-1.34.18/mypy_boto3_s3control.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 21:05:17.431042 mypy-boto3-s3control-1.34.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-01-12 21:04:59.000000 mypy-boto3-s3control-1.34.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:08.847352 mypy-boto3-s3control-1.34.83/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 19:17:52.000000 mypy-boto3-s3control-1.34.83/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-04-11 19:18:08.847352 mypy-boto3-s3control-1.34.83/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-11 19:17:52.000000 mypy-boto3-s3control-1.34.83/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:08.843352 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-11 19:17:52.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-11 19:17:52.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-11 19:17:52.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57493 2024-04-11 19:17:52.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57490 2024-04-11 19:17:52.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14622 2024-04-11 19:17:53.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14622 2024-04-11 19:17:52.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-11 19:17:52.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-11 19:17:52.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:17:52.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    80734 2024-04-11 19:17:55.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80734 2024-04-11 19:17:54.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 19:17:52.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:08.847352 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-04-11 19:18:08.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-11 19:18:08.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:08.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:08.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 19:18:08.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-11 19:18:08.000000 mypy-boto3-s3control-1.34.83/mypy_boto3_s3control.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:18:08.847352 mypy-boto3-s3control-1.34.83/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-11 19:17:52.000000 mypy-boto3-s3control-1.34.83/setup.py
```

### Comparing `mypy-boto3-s3control-1.34.18/LICENSE` & `mypy-boto3-s3control-1.34.83/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.34.18/PKG-INFO` & `mypy-boto3-s3control-1.34.83/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3control
-Version: 1.34.18
-Summary: Type annotations for boto3.S3Control 1.34.18 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.83
+Summary: Type annotations for boto3.S3Control 1.34.83 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-s3control)](https://pepy.tech/project/mypy-boto3-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Control 1.34.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[boto3.S3Control 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-s3control docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-s3control-1.34.18/README.md` & `mypy-boto3-s3control-1.34.83/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-s3control)](https://pepy.tech/project/mypy-boto3-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Control 1.34.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[boto3.S3Control 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-s3control docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/__init__.py` & `mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/__init__.pyi` & `mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/__main__.py` & `mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.S3Control 1.34.18\nVersion:         1.34.18\nBuilder version:"
-        " 7.23.1\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.S3Control 1.34.83\n"
+        "Version:         1.34.83\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.18")
+    print("1.34.83")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/client.py` & `mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -666,15 +666,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_policy_status_for_object_lambda)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#get_access_point_policy_status_for_object_lambda)
         """
 
     def get_bucket(self, *, AccountId: str, Bucket: str) -> GetBucketResultTypeDef:
         """
-        .
+        Gets an Amazon S3 on Outposts bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#get_bucket)
         """
 
     def get_bucket_lifecycle_configuration(
         self, *, AccountId: str, Bucket: str
@@ -897,15 +897,15 @@
         AccountId: str,
         JobStatuses: Sequence[JobStatusType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
     ) -> ListJobsResultTypeDef:
         """
         Lists current S3 Batch Operations jobs as well as the jobs that have ended
-        within the last 30 days for the Amazon Web Services account making the
+        within the last 90 days for the Amazon Web Services account making the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#list_jobs)
         """
 
     def list_multi_region_access_points(
```

### Comparing `mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/client.pyi` & `mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -663,15 +663,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_policy_status_for_object_lambda)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#get_access_point_policy_status_for_object_lambda)
         """
 
     def get_bucket(self, *, AccountId: str, Bucket: str) -> GetBucketResultTypeDef:
         """
-        .
+        Gets an Amazon S3 on Outposts bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_bucket)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#get_bucket)
         """
 
     def get_bucket_lifecycle_configuration(
         self, *, AccountId: str, Bucket: str
@@ -894,15 +894,15 @@
         AccountId: str,
         JobStatuses: Sequence[JobStatusType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
     ) -> ListJobsResultTypeDef:
         """
         Lists current S3 Batch Operations jobs as well as the jobs that have ended
-        within the last 30 days for the Amazon Web Services account making the
+        within the last 90 days for the Amazon Web Services account making the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#list_jobs)
         """
 
     def list_multi_region_access_points(
```

### Comparing `mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/literals.py` & `mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,14 +227,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -245,14 +246,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -270,14 +272,15 @@
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
@@ -290,24 +293,26 @@
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
@@ -368,15 +373,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -556,14 +560,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/literals.pyi` & `mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -227,14 +227,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -245,14 +246,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -270,14 +272,15 @@
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
@@ -290,24 +293,26 @@
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
@@ -368,15 +373,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -556,14 +560,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/paginator.py` & `mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/paginator.pyi` & `mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/type_defs.py` & `mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,18 +458,18 @@
         "Value": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 ObjectLambdaAccessPointAliasTypeDef = TypedDict(
     "ObjectLambdaAccessPointAliasTypeDef",
     {
         "Value": NotRequired[str],
         "Status": NotRequired[ObjectLambdaAccessPointAliasStatusType],
```

### Comparing `mypy-boto3-s3control-1.34.18/mypy_boto3_s3control/type_defs.pyi` & `mypy-boto3-s3control-1.34.83/mypy_boto3_s3control/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -458,18 +458,18 @@
         "Value": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 ObjectLambdaAccessPointAliasTypeDef = TypedDict(
     "ObjectLambdaAccessPointAliasTypeDef",
     {
         "Value": NotRequired[str],
         "Status": NotRequired[ObjectLambdaAccessPointAliasStatusType],
```

### Comparing `mypy-boto3-s3control-1.34.18/mypy_boto3_s3control.egg-info/PKG-INFO` & `mypy-boto3-s3control-1.34.83/mypy_boto3_s3control.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3control
-Version: 1.34.18
-Summary: Type annotations for boto3.S3Control 1.34.18 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.83
+Summary: Type annotations for boto3.S3Control 1.34.83 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-s3control)](https://pepy.tech/project/mypy-boto3-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Control 1.34.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[boto3.S3Control 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-s3control docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-s3control-1.34.18/mypy_boto3_s3control.egg-info/SOURCES.txt` & `mypy-boto3-s3control-1.34.83/mypy_boto3_s3control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.34.18/setup.py` & `mypy-boto3-s3control-1.34.83/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-s3control",
-    version="1.34.18",
+    version="1.34.83",
     packages=["mypy_boto3_s3control"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.S3Control 1.34.18 service generated with mypy-boto3-builder"
-        " 7.23.1"
-    ),
+    description="Type annotations for boto3.S3Control 1.34.83 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

