# Comparing `tmp/mypy-boto3-cloudfront-1.34.0.tar.gz` & `tmp/mypy-boto3-cloudfront-1.34.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudfront-1.34.0.tar", last modified: Wed Dec 13 21:22:10 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudfront-1.34.83.tar", last modified: Thu Apr 11 19:18:06 2024, max compression
```

## Comparing `mypy-boto3-cloudfront-1.34.0.tar` & `mypy-boto3-cloudfront-1.34.83.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:10.423153 mypy-boto3-cloudfront-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:06:53.000000 mypy-boto3-cloudfront-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14531 2023-12-13 21:22:10.423153 mypy-boto3-cloudfront-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12986 2023-12-13 21:06:53.000000 mypy-boto3-cloudfront-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:10.423153 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2023-12-13 21:06:53.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2023-12-13 21:06:53.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-13 21:06:53.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    82884 2023-12-13 21:06:55.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    82880 2023-12-13 21:06:54.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13241 2023-12-13 21:06:55.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2023-12-13 21:06:55.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6559 2023-12-13 21:06:55.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2023-12-13 21:06:55.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:06:53.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   105107 2023-12-13 21:06:57.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   105106 2023-12-13 21:06:56.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:06:53.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2023-12-13 21:06:55.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2023-12-13 21:06:55.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:10.423153 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14531 2023-12-13 21:22:10.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-13 21:22:10.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:10.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:10.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:22:10.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 21:22:10.000000 mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:22:10.423153 mypy-boto3-cloudfront-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2023-12-13 21:06:53.000000 mypy-boto3-cloudfront-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:06.011387 mypy-boto3-cloudfront-1.34.83/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14554 2024-04-11 19:18:06.011387 mypy-boto3-cloudfront-1.34.83/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:06.011387 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82896 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82893 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-04-11 19:17:12.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-04-11 19:17:12.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   105119 2024-04-11 19:17:14.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105119 2024-04-11 19:17:13.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:06.011387 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14554 2024-04-11 19:18:05.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-11 19:18:05.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:05.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:05.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 19:18:05.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 19:18:05.000000 mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:18:06.011387 mypy-boto3-cloudfront-1.34.83/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-11 19:17:11.000000 mypy-boto3-cloudfront-1.34.83/setup.py
```

### Comparing `mypy-boto3-cloudfront-1.34.0/LICENSE` & `mypy-boto3-cloudfront-1.34.83/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-cloudfront-1.34.0/PKG-INFO` & `mypy-boto3-cloudfront-1.34.83/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudfront
-Version: 1.34.0
-Summary: Type annotations for boto3.CloudFront 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.83
+Summary: Type annotations for boto3.CloudFront 1.34.83 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-cloudfront"></a>
 
 # mypy-boto3-cloudfront
 
 [![PyPI - mypy-boto3-cloudfront](https://img.shields.io/pypi/v/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudfront)](https://pepy.tech/project/mypy-boto3-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFront 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[boto3.CloudFront 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudfront-1.34.0/README.md` & `mypy-boto3-cloudfront-1.34.83/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudfront)](https://pepy.tech/project/mypy-boto3-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFront 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[boto3.CloudFront 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/__init__.py` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     DistributionDeployedWaiter,
     InvalidationCompletedWaiter,
     StreamingDistributionDeployedWaiter,
 )
 
 Client = CloudFrontClient
 
-
 __all__ = (
     "Client",
     "CloudFrontClient",
     "DistributionDeployedWaiter",
     "InvalidationCompletedWaiter",
     "ListCloudFrontOriginAccessIdentitiesPaginator",
     "ListDistributionsPaginator",
```

### Comparing `mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/__init__.pyi` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/__main__.py` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudFront 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.CloudFront 1.34.83\n"
+        "Version:         1.34.83\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.83")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/client.py` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CloudFrontClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -373,15 +372,15 @@
     def copy_distribution(
         self,
         *,
         PrimaryDistributionId: str,
         CallerReference: str,
         Staging: bool = ...,
         IfMatch: str = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> CopyDistributionResultTypeDef:
         """
         Creates a staging distribution using the configuration of the provided primary
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#copy_distribution)
@@ -490,15 +489,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_key_group)
         """
 
     def create_key_value_store(
         self, *, Name: str, Comment: str = ..., ImportSource: ImportSourceTypeDef = ...
     ) -> CreateKeyValueStoreResultTypeDef:
         """
-        Specifies the Key Value Store resource to add to your account.
+        Specifies the key value store resource to add to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_key_value_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_key_value_store)
         """
 
     def create_monitoring_subscription(
         self, *, DistributionId: str, MonitoringSubscription: MonitoringSubscriptionTypeDef
@@ -546,15 +545,15 @@
 
     def create_realtime_log_config(
         self,
         *,
         EndPoints: Sequence[EndPointTypeDef],
         Fields: Sequence[str],
         Name: str,
-        SamplingRate: int
+        SamplingRate: int,
     ) -> CreateRealtimeLogConfigResultTypeDef:
         """
         Creates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_realtime_log_config)
         """
@@ -659,15 +658,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_key_group)
         """
 
     def delete_key_value_store(self, *, Name: str, IfMatch: str) -> EmptyResponseMetadataTypeDef:
         """
-        Specifies the Key Value Store to delete.
+        Specifies the key value store to delete.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_key_value_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_key_value_store)
         """
 
     def delete_monitoring_subscription(self, *, DistributionId: str) -> Dict[str, Any]:
         """
@@ -746,15 +745,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.describe_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#describe_function)
         """
 
     def describe_key_value_store(self, *, Name: str) -> DescribeKeyValueStoreResultTypeDef:
         """
-        Specifies the Key Value Store and its configuration.
+        Specifies the key value store and its configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.describe_key_value_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#describe_key_value_store)
         """
 
     def generate_presigned_url(
         self,
@@ -1125,15 +1124,15 @@
 
     def list_distributions_by_realtime_log_config(
         self,
         *,
         Marker: str = ...,
         MaxItems: str = ...,
         RealtimeLogConfigName: str = ...,
-        RealtimeLogConfigArn: str = ...
+        RealtimeLogConfigArn: str = ...,
     ) -> ListDistributionsByRealtimeLogConfigResultTypeDef:
         """
         Gets a list of distributions that have a cache behavior that's associated with
         the specified real-time log
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_realtime_log_config)
@@ -1216,15 +1215,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_key_groups)
         """
 
     def list_key_value_stores(
         self, *, Marker: str = ..., MaxItems: str = ..., Status: str = ...
     ) -> ListKeyValueStoresResultTypeDef:
         """
-        Specifies the Key Value Stores to list.
+        Specifies the key value stores to list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_key_value_stores)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_key_value_stores)
         """
 
     def list_origin_access_controls(
         self, *, Marker: str = ..., MaxItems: str = ...
@@ -1344,29 +1343,29 @@
         """
 
     def update_cloud_front_origin_access_identity(
         self,
         *,
         CloudFrontOriginAccessIdentityConfig: CloudFrontOriginAccessIdentityConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateCloudFrontOriginAccessIdentityResultTypeDef:
         """
         Update an origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_cloud_front_origin_access_identity)
         """
 
     def update_continuous_deployment_policy(
         self,
         *,
         ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateContinuousDeploymentPolicyResultTypeDef:
         """
         Updates a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_continuous_deployment_policy)
         """
@@ -1393,44 +1392,44 @@
         """
 
     def update_field_level_encryption_config(
         self,
         *,
         FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateFieldLevelEncryptionConfigResultTypeDef:
         """
         Update a field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_field_level_encryption_config)
         """
 
     def update_field_level_encryption_profile(
         self,
         *,
         FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateFieldLevelEncryptionProfileResultTypeDef:
         """
         Update a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_field_level_encryption_profile)
         """
 
     def update_function(
         self,
         *,
         Name: str,
         IfMatch: str,
         FunctionConfig: FunctionConfigTypeDef,
-        FunctionCode: BlobTypeDef
+        FunctionCode: BlobTypeDef,
     ) -> UpdateFunctionResultTypeDef:
         """
         Updates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_function)
         """
@@ -1445,40 +1444,40 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_key_group)
         """
 
     def update_key_value_store(
         self, *, Name: str, Comment: str, IfMatch: str
     ) -> UpdateKeyValueStoreResultTypeDef:
         """
-        Specifies the Key Value Store to update.
+        Specifies the key value store to update.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_key_value_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_key_value_store)
         """
 
     def update_origin_access_control(
         self,
         *,
         OriginAccessControlConfig: OriginAccessControlConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateOriginAccessControlResultTypeDef:
         """
         Updates a CloudFront origin access control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_origin_access_control)
         """
 
     def update_origin_request_policy(
         self,
         *,
         OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateOriginRequestPolicyResultTypeDef:
         """
         Updates an origin request policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_request_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_origin_request_policy)
         """
@@ -1496,43 +1495,43 @@
     def update_realtime_log_config(
         self,
         *,
         EndPoints: Sequence[EndPointTypeDef] = ...,
         Fields: Sequence[str] = ...,
         Name: str = ...,
         ARN: str = ...,
-        SamplingRate: int = ...
+        SamplingRate: int = ...,
     ) -> UpdateRealtimeLogConfigResultTypeDef:
         """
         Updates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_realtime_log_config)
         """
 
     def update_response_headers_policy(
         self,
         *,
         ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateResponseHeadersPolicyResultTypeDef:
         """
         Updates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_response_headers_policy)
         """
 
     def update_streaming_distribution(
         self,
         *,
         StreamingDistributionConfig: StreamingDistributionConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateStreamingDistributionResultTypeDef:
         """
         Update a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_streaming_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_streaming_distribution)
         """
```

### Comparing `mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/client.pyi` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -369,15 +369,15 @@
     def copy_distribution(
         self,
         *,
         PrimaryDistributionId: str,
         CallerReference: str,
         Staging: bool = ...,
         IfMatch: str = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> CopyDistributionResultTypeDef:
         """
         Creates a staging distribution using the configuration of the provided primary
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#copy_distribution)
@@ -486,15 +486,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_key_group)
         """
 
     def create_key_value_store(
         self, *, Name: str, Comment: str = ..., ImportSource: ImportSourceTypeDef = ...
     ) -> CreateKeyValueStoreResultTypeDef:
         """
-        Specifies the Key Value Store resource to add to your account.
+        Specifies the key value store resource to add to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_key_value_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_key_value_store)
         """
 
     def create_monitoring_subscription(
         self, *, DistributionId: str, MonitoringSubscription: MonitoringSubscriptionTypeDef
@@ -542,15 +542,15 @@
 
     def create_realtime_log_config(
         self,
         *,
         EndPoints: Sequence[EndPointTypeDef],
         Fields: Sequence[str],
         Name: str,
-        SamplingRate: int
+        SamplingRate: int,
     ) -> CreateRealtimeLogConfigResultTypeDef:
         """
         Creates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_realtime_log_config)
         """
@@ -655,15 +655,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_key_group)
         """
 
     def delete_key_value_store(self, *, Name: str, IfMatch: str) -> EmptyResponseMetadataTypeDef:
         """
-        Specifies the Key Value Store to delete.
+        Specifies the key value store to delete.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_key_value_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_key_value_store)
         """
 
     def delete_monitoring_subscription(self, *, DistributionId: str) -> Dict[str, Any]:
         """
@@ -742,15 +742,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.describe_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#describe_function)
         """
 
     def describe_key_value_store(self, *, Name: str) -> DescribeKeyValueStoreResultTypeDef:
         """
-        Specifies the Key Value Store and its configuration.
+        Specifies the key value store and its configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.describe_key_value_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#describe_key_value_store)
         """
 
     def generate_presigned_url(
         self,
@@ -1121,15 +1121,15 @@
 
     def list_distributions_by_realtime_log_config(
         self,
         *,
         Marker: str = ...,
         MaxItems: str = ...,
         RealtimeLogConfigName: str = ...,
-        RealtimeLogConfigArn: str = ...
+        RealtimeLogConfigArn: str = ...,
     ) -> ListDistributionsByRealtimeLogConfigResultTypeDef:
         """
         Gets a list of distributions that have a cache behavior that's associated with
         the specified real-time log
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_realtime_log_config)
@@ -1212,15 +1212,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_key_groups)
         """
 
     def list_key_value_stores(
         self, *, Marker: str = ..., MaxItems: str = ..., Status: str = ...
     ) -> ListKeyValueStoresResultTypeDef:
         """
-        Specifies the Key Value Stores to list.
+        Specifies the key value stores to list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_key_value_stores)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_key_value_stores)
         """
 
     def list_origin_access_controls(
         self, *, Marker: str = ..., MaxItems: str = ...
@@ -1340,29 +1340,29 @@
         """
 
     def update_cloud_front_origin_access_identity(
         self,
         *,
         CloudFrontOriginAccessIdentityConfig: CloudFrontOriginAccessIdentityConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateCloudFrontOriginAccessIdentityResultTypeDef:
         """
         Update an origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_cloud_front_origin_access_identity)
         """
 
     def update_continuous_deployment_policy(
         self,
         *,
         ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateContinuousDeploymentPolicyResultTypeDef:
         """
         Updates a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_continuous_deployment_policy)
         """
@@ -1389,44 +1389,44 @@
         """
 
     def update_field_level_encryption_config(
         self,
         *,
         FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateFieldLevelEncryptionConfigResultTypeDef:
         """
         Update a field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_field_level_encryption_config)
         """
 
     def update_field_level_encryption_profile(
         self,
         *,
         FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateFieldLevelEncryptionProfileResultTypeDef:
         """
         Update a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_field_level_encryption_profile)
         """
 
     def update_function(
         self,
         *,
         Name: str,
         IfMatch: str,
         FunctionConfig: FunctionConfigTypeDef,
-        FunctionCode: BlobTypeDef
+        FunctionCode: BlobTypeDef,
     ) -> UpdateFunctionResultTypeDef:
         """
         Updates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_function)
         """
@@ -1441,40 +1441,40 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_key_group)
         """
 
     def update_key_value_store(
         self, *, Name: str, Comment: str, IfMatch: str
     ) -> UpdateKeyValueStoreResultTypeDef:
         """
-        Specifies the Key Value Store to update.
+        Specifies the key value store to update.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_key_value_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_key_value_store)
         """
 
     def update_origin_access_control(
         self,
         *,
         OriginAccessControlConfig: OriginAccessControlConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateOriginAccessControlResultTypeDef:
         """
         Updates a CloudFront origin access control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_origin_access_control)
         """
 
     def update_origin_request_policy(
         self,
         *,
         OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateOriginRequestPolicyResultTypeDef:
         """
         Updates an origin request policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_request_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_origin_request_policy)
         """
@@ -1492,43 +1492,43 @@
     def update_realtime_log_config(
         self,
         *,
         EndPoints: Sequence[EndPointTypeDef] = ...,
         Fields: Sequence[str] = ...,
         Name: str = ...,
         ARN: str = ...,
-        SamplingRate: int = ...
+        SamplingRate: int = ...,
     ) -> UpdateRealtimeLogConfigResultTypeDef:
         """
         Updates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_realtime_log_config)
         """
 
     def update_response_headers_policy(
         self,
         *,
         ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateResponseHeadersPolicyResultTypeDef:
         """
         Updates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_response_headers_policy)
         """
 
     def update_streaming_distribution(
         self,
         *,
         StreamingDistributionConfig: StreamingDistributionConfigTypeDef,
         Id: str,
-        IfMatch: str = ...
+        IfMatch: str = ...,
     ) -> UpdateStreamingDistributionResultTypeDef:
         """
         Update a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_streaming_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_streaming_distribution)
         """
```

### Comparing `mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/literals.py` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "CachePolicyCookieBehaviorType",
     "CachePolicyHeaderBehaviorType",
     "CachePolicyQueryStringBehaviorType",
     "CachePolicyTypeType",
     "CertificateSourceType",
     "ContinuousDeploymentPolicyTypeType",
@@ -66,15 +65,14 @@
     "CloudFrontServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
 )
 
-
 CachePolicyCookieBehaviorType = Literal["all", "allExcept", "none", "whitelist"]
 CachePolicyHeaderBehaviorType = Literal["none", "whitelist"]
 CachePolicyQueryStringBehaviorType = Literal["all", "allExcept", "none", "whitelist"]
 CachePolicyTypeType = Literal["custom", "managed"]
 CertificateSourceType = Literal["acm", "cloudfront", "iam"]
 ContinuousDeploymentPolicyTypeType = Literal["SingleHeader", "SingleWeight"]
 DistributionDeployedWaiterName = Literal["distribution_deployed"]
@@ -96,15 +94,15 @@
 ListInvalidationsPaginatorName = Literal["list_invalidations"]
 ListKeyValueStoresPaginatorName = Literal["list_key_value_stores"]
 ListStreamingDistributionsPaginatorName = Literal["list_streaming_distributions"]
 MethodType = Literal["DELETE", "GET", "HEAD", "OPTIONS", "PATCH", "POST", "PUT"]
 MinimumProtocolVersionType = Literal[
     "SSLv3", "TLSv1", "TLSv1.1_2016", "TLSv1.2_2018", "TLSv1.2_2019", "TLSv1.2_2021", "TLSv1_2016"
 ]
-OriginAccessControlOriginTypesType = Literal["mediastore", "s3"]
+OriginAccessControlOriginTypesType = Literal["lambda", "mediapackagev2", "mediastore", "s3"]
 OriginAccessControlSigningBehaviorsType = Literal["always", "never", "no-override"]
 OriginAccessControlSigningProtocolsType = Literal["sigv4"]
 OriginProtocolPolicyType = Literal["http-only", "https-only", "match-viewer"]
 OriginRequestPolicyCookieBehaviorType = Literal["all", "allExcept", "none", "whitelist"]
 OriginRequestPolicyHeaderBehaviorType = Literal[
     "allExcept", "allViewer", "allViewerAndWhitelistCloudFront", "none", "whitelist"
 ]
@@ -153,14 +151,15 @@
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
@@ -171,14 +170,15 @@
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
@@ -196,14 +196,15 @@
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
@@ -216,24 +217,26 @@
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
@@ -294,15 +297,14 @@
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
@@ -374,17 +376,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -474,19 +478,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
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

### Comparing `mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/literals.pyi` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 ListInvalidationsPaginatorName = Literal["list_invalidations"]
 ListKeyValueStoresPaginatorName = Literal["list_key_value_stores"]
 ListStreamingDistributionsPaginatorName = Literal["list_streaming_distributions"]
 MethodType = Literal["DELETE", "GET", "HEAD", "OPTIONS", "PATCH", "POST", "PUT"]
 MinimumProtocolVersionType = Literal[
     "SSLv3", "TLSv1", "TLSv1.1_2016", "TLSv1.2_2018", "TLSv1.2_2019", "TLSv1.2_2021", "TLSv1_2016"
 ]
-OriginAccessControlOriginTypesType = Literal["mediastore", "s3"]
+OriginAccessControlOriginTypesType = Literal["lambda", "mediapackagev2", "mediastore", "s3"]
 OriginAccessControlSigningBehaviorsType = Literal["always", "never", "no-override"]
 OriginAccessControlSigningProtocolsType = Literal["sigv4"]
 OriginProtocolPolicyType = Literal["http-only", "https-only", "match-viewer"]
 OriginRequestPolicyCookieBehaviorType = Literal["all", "allExcept", "none", "whitelist"]
 OriginRequestPolicyHeaderBehaviorType = Literal[
     "allExcept", "allViewer", "allViewerAndWhitelistCloudFront", "none", "whitelist"
 ]
@@ -151,14 +151,15 @@
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
@@ -169,14 +170,15 @@
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
@@ -194,14 +196,15 @@
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
@@ -214,24 +217,26 @@
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
@@ -292,15 +297,14 @@
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
@@ -372,17 +376,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -472,19 +478,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
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

### Comparing `mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/paginator.py` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -45,85 +45,78 @@
     "ListCloudFrontOriginAccessIdentitiesPaginator",
     "ListDistributionsPaginator",
     "ListInvalidationsPaginator",
     "ListKeyValueStoresPaginator",
     "ListStreamingDistributionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListCloudFrontOriginAccessIdentitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listcloudfrontoriginaccessidentitiespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCloudFrontOriginAccessIdentitiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listcloudfrontoriginaccessidentitiespaginator)
         """
 
-
 class ListDistributionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListDistributions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listdistributionspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDistributionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListDistributions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listdistributionspaginator)
         """
 
-
 class ListInvalidationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListInvalidations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listinvalidationspaginator)
     """
 
     def paginate(
         self, *, DistributionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInvalidationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListInvalidations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listinvalidationspaginator)
         """
 
-
 class ListKeyValueStoresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListKeyValueStores)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listkeyvaluestorespaginator)
     """
 
     def paginate(
         self, *, Status: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKeyValueStoresResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListKeyValueStores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listkeyvaluestorespaginator)
         """
 
-
 class ListStreamingDistributionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListStreamingDistributions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#liststreamingdistributionspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/paginator.pyi` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,76 +47,82 @@
     "ListInvalidationsPaginator",
     "ListKeyValueStoresPaginator",
     "ListStreamingDistributionsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListCloudFrontOriginAccessIdentitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listcloudfrontoriginaccessidentitiespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCloudFrontOriginAccessIdentitiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listcloudfrontoriginaccessidentitiespaginator)
         """
 
+
 class ListDistributionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListDistributions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listdistributionspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDistributionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListDistributions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listdistributionspaginator)
         """
 
+
 class ListInvalidationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListInvalidations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listinvalidationspaginator)
     """
 
     def paginate(
         self, *, DistributionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInvalidationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListInvalidations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listinvalidationspaginator)
         """
 
+
 class ListKeyValueStoresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListKeyValueStores)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listkeyvaluestorespaginator)
     """
 
     def paginate(
         self, *, Status: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKeyValueStoresResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListKeyValueStores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listkeyvaluestorespaginator)
         """
 
+
 class ListStreamingDistributionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListStreamingDistributions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#liststreamingdistributionspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/type_defs.py` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AliasICPRecordalTypeDef",
     "AliasesTypeDef",
     "CachedMethodsTypeDef",
     "AssociateAliasRequestRequestTypeDef",
     "BlobTypeDef",
     "TrustedKeyGroupsTypeDef",
@@ -574,18 +573,18 @@
         "Enabled": NotRequired[bool],
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
 KeyGroupConfigTypeDef = TypedDict(
     "KeyGroupConfigTypeDef",
     {
         "Name": str,
         "Items": Sequence[str],
```

### Comparing `mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/type_defs.pyi` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -573,18 +573,18 @@
         "Enabled": NotRequired[bool],
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
 KeyGroupConfigTypeDef = TypedDict(
     "KeyGroupConfigTypeDef",
     {
         "Name": str,
         "Items": Sequence[str],
```

### Comparing `mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/waiter.py` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront/waiter.pyi` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront.egg-info/PKG-INFO` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudfront
-Version: 1.34.0
-Summary: Type annotations for boto3.CloudFront 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.83
+Summary: Type annotations for boto3.CloudFront 1.34.83 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-cloudfront"></a>
 
 # mypy-boto3-cloudfront
 
 [![PyPI - mypy-boto3-cloudfront](https://img.shields.io/pypi/v/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudfront)](https://pepy.tech/project/mypy-boto3-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFront 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[boto3.CloudFront 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudfront-1.34.0/mypy_boto3_cloudfront.egg-info/SOURCES.txt` & `mypy-boto3-cloudfront-1.34.83/mypy_boto3_cloudfront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.34.0/setup.py` & `mypy-boto3-cloudfront-1.34.83/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudfront",
-    version="1.34.0",
+    version="1.34.83",
     packages=["mypy_boto3_cloudfront"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.CloudFront 1.34.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
-    ),
+    description="Type annotations for boto3.CloudFront 1.34.83 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 cloudfront type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_cloudfront": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

