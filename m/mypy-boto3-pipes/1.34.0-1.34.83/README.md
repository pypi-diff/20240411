# Comparing `tmp/mypy-boto3-pipes-1.34.0.tar.gz` & `tmp/mypy-boto3-pipes-1.34.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pipes-1.34.0.tar", last modified: Wed Dec 13 21:23:31 2023, max compression
+gzip compressed data, was "mypy-boto3-pipes-1.34.83.tar", last modified: Thu Apr 11 19:18:08 2024, max compression
```

## Comparing `mypy-boto3-pipes-1.34.0.tar` & `mypy-boto3-pipes-1.34.83.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:31.479322 mypy-boto3-pipes-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:15:33.000000 mypy-boto3-pipes-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2023-12-13 21:23:31.479322 mypy-boto3-pipes-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11111 2023-12-13 21:15:33.000000 mypy-boto3-pipes-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:31.475322 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2023-12-13 21:15:33.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2023-12-13 21:15:33.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-12-13 21:15:33.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9828 2023-12-13 21:15:33.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9824 2023-12-13 21:15:33.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11023 2023-12-13 21:15:33.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11021 2023-12-13 21:15:33.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2023-12-13 21:15:33.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2023-12-13 21:15:33.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:15:33.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    31887 2023-12-13 21:15:33.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    31886 2023-12-13 21:15:33.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:15:33.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:31.475322 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2023-12-13 21:23:31.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2023-12-13 21:23:31.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:31.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:31.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:23:31.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-13 21:23:31.000000 mypy-boto3-pipes-1.34.0/mypy_boto3_pipes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:23:31.479322 mypy-boto3-pipes-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2023-12-13 21:15:33.000000 mypy-boto3-pipes-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:08.139362 mypy-boto3-pipes-1.34.83/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 19:17:40.000000 mypy-boto3-pipes-1.34.83/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-04-11 19:18:08.139362 mypy-boto3-pipes-1.34.83/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-04-11 19:17:40.000000 mypy-boto3-pipes-1.34.83/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:08.135362 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-11 19:17:40.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-11 19:17:40.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-11 19:17:40.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-04-11 19:17:40.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-11 19:17:40.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11180 2024-04-11 19:17:40.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11180 2024-04-11 19:17:40.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-11 19:17:40.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-11 19:17:40.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:17:40.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    31899 2024-04-11 19:17:40.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31899 2024-04-11 19:17:40.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 19:17:40.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:08.139362 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-04-11 19:18:08.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-11 19:18:08.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:08.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:08.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 19:18:08.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 19:18:08.000000 mypy-boto3-pipes-1.34.83/mypy_boto3_pipes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:18:08.139362 mypy-boto3-pipes-1.34.83/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-11 19:17:40.000000 mypy-boto3-pipes-1.34.83/setup.py
```

### Comparing `mypy-boto3-pipes-1.34.0/LICENSE` & `mypy-boto3-pipes-1.34.83/LICENSE`

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

### Comparing `mypy-boto3-pipes-1.34.0/PKG-INFO` & `mypy-boto3-pipes-1.34.83/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pipes
-Version: 1.34.0
-Summary: Type annotations for boto3.EventBridgePipes 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.83
+Summary: Type annotations for boto3.EventBridgePipes 1.34.83 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/
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
 
 <a id="mypy-boto3-pipes"></a>
 
 # mypy-boto3-pipes
 
 [![PyPI - mypy-boto3-pipes](https://img.shields.io/pypi/v/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pipes)](https://pepy.tech/project/mypy-boto3-pipes)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgePipes 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
+[boto3.EventBridgePipes 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
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
 [mypy-boto3-pipes docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-pipes-1.34.0/README.md` & `mypy-boto3-pipes-1.34.83/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pipes)](https://pepy.tech/project/mypy-boto3-pipes)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgePipes 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
+[boto3.EventBridgePipes 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
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
 [mypy-boto3-pipes docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/__init__.py` & `mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,9 +19,8 @@
 """
 
 from .client import EventBridgePipesClient
 from .paginator import ListPipesPaginator
 
 Client = EventBridgePipesClient
 
-
 __all__ = ("Client", "EventBridgePipesClient", "ListPipesPaginator")
```

### Comparing `mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/__init__.pyi` & `mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/__main__.py` & `mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EventBridgePipes 1.34.0\nVersion:         1.34.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.EventBridgePipes 1.34.83\n"
+        "Version:         1.34.83\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes\n"
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

### Comparing `mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/client.py` & `mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("EventBridgePipesClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -107,15 +106,15 @@
         Description: str = ...,
         DesiredState: RequestedPipeStateType = ...,
         Enrichment: str = ...,
         EnrichmentParameters: PipeEnrichmentParametersTypeDef = ...,
         LogConfiguration: PipeLogConfigurationParametersTypeDef = ...,
         SourceParameters: PipeSourceParametersTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        TargetParameters: PipeTargetParametersTypeDef = ...
+        TargetParameters: PipeTargetParametersTypeDef = ...,
     ) -> CreatePipeResponseTypeDef:
         """
         Create a pipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client.create_pipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/client/#create_pipe)
         """
@@ -155,15 +154,15 @@
         *,
         CurrentState: PipeStateType = ...,
         DesiredState: RequestedPipeStateType = ...,
         Limit: int = ...,
         NamePrefix: str = ...,
         NextToken: str = ...,
         SourcePrefix: str = ...,
-        TargetPrefix: str = ...
+        TargetPrefix: str = ...,
     ) -> ListPipesResponseTypeDef:
         """
         Get the pipes associated with this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client.list_pipes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/client/#list_pipes)
         """
@@ -216,15 +215,15 @@
         Description: str = ...,
         DesiredState: RequestedPipeStateType = ...,
         Enrichment: str = ...,
         EnrichmentParameters: PipeEnrichmentParametersTypeDef = ...,
         LogConfiguration: PipeLogConfigurationParametersTypeDef = ...,
         SourceParameters: UpdatePipeSourceParametersTypeDef = ...,
         Target: str = ...,
-        TargetParameters: PipeTargetParametersTypeDef = ...
+        TargetParameters: PipeTargetParametersTypeDef = ...,
     ) -> UpdatePipeResponseTypeDef:
         """
         Update an existing pipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client.update_pipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/client/#update_pipe)
         """
```

### Comparing `mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/client.pyi` & `mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         Description: str = ...,
         DesiredState: RequestedPipeStateType = ...,
         Enrichment: str = ...,
         EnrichmentParameters: PipeEnrichmentParametersTypeDef = ...,
         LogConfiguration: PipeLogConfigurationParametersTypeDef = ...,
         SourceParameters: PipeSourceParametersTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        TargetParameters: PipeTargetParametersTypeDef = ...
+        TargetParameters: PipeTargetParametersTypeDef = ...,
     ) -> CreatePipeResponseTypeDef:
         """
         Create a pipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client.create_pipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/client/#create_pipe)
         """
@@ -151,15 +151,15 @@
         *,
         CurrentState: PipeStateType = ...,
         DesiredState: RequestedPipeStateType = ...,
         Limit: int = ...,
         NamePrefix: str = ...,
         NextToken: str = ...,
         SourcePrefix: str = ...,
-        TargetPrefix: str = ...
+        TargetPrefix: str = ...,
     ) -> ListPipesResponseTypeDef:
         """
         Get the pipes associated with this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client.list_pipes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/client/#list_pipes)
         """
@@ -212,15 +212,15 @@
         Description: str = ...,
         DesiredState: RequestedPipeStateType = ...,
         Enrichment: str = ...,
         EnrichmentParameters: PipeEnrichmentParametersTypeDef = ...,
         LogConfiguration: PipeLogConfigurationParametersTypeDef = ...,
         SourceParameters: UpdatePipeSourceParametersTypeDef = ...,
         Target: str = ...,
-        TargetParameters: PipeTargetParametersTypeDef = ...
+        TargetParameters: PipeTargetParametersTypeDef = ...,
     ) -> UpdatePipeResponseTypeDef:
         """
         Update an existing pipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client.update_pipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/client/#update_pipe)
         """
```

### Comparing `mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/literals.py` & `mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/literals.py`

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
     "AssignPublicIpType",
     "BatchJobDependencyTypeType",
     "BatchResourceRequirementTypeType",
     "DynamoDBStreamStartPositionType",
     "EcsEnvironmentFileTypeType",
     "EcsResourceRequirementTypeType",
@@ -46,15 +45,14 @@
     "EventBridgePipesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 BatchJobDependencyTypeType = Literal["N_TO_N", "SEQUENTIAL"]
 BatchResourceRequirementTypeType = Literal["GPU", "MEMORY", "VCPU"]
 DynamoDBStreamStartPositionType = Literal["LATEST", "TRIM_HORIZON"]
 EcsEnvironmentFileTypeType = Literal["s3"]
 EcsResourceRequirementTypeType = Literal["GPU", "InferenceAccelerator"]
 IncludeExecutionDataOptionType = Literal["ALL"]
@@ -112,14 +110,15 @@
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
@@ -130,14 +129,15 @@
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
@@ -253,15 +256,14 @@
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
@@ -333,17 +335,19 @@
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
@@ -433,19 +437,21 @@
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

### Comparing `mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/literals.pyi` & `mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,15 @@
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
@@ -128,14 +129,15 @@
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
@@ -153,14 +155,15 @@
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
@@ -173,24 +176,26 @@
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
@@ -251,15 +256,14 @@
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
@@ -331,17 +335,19 @@
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
@@ -431,19 +437,21 @@
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

### Comparing `mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/paginator.py` & `mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import PipeStateType, RequestedPipeStateType
 from .type_defs import ListPipesResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListPipesPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -50,13 +49,13 @@
         self,
         *,
         CurrentState: PipeStateType = ...,
         DesiredState: RequestedPipeStateType = ...,
         NamePrefix: str = ...,
         SourcePrefix: str = ...,
         TargetPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListPipesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Paginator.ListPipes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/paginators/#listpipespaginator)
         """
```

### Comparing `mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/paginator.pyi` & `mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -47,13 +47,13 @@
         self,
         *,
         CurrentState: PipeStateType = ...,
         DesiredState: RequestedPipeStateType = ...,
         NamePrefix: str = ...,
         SourcePrefix: str = ...,
         TargetPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListPipesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Paginator.ListPipes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/paginators/#listpipespaginator)
         """
```

### Comparing `mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/type_defs.py` & `mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AwsVpcConfigurationTypeDef",
     "BatchArrayPropertiesTypeDef",
     "BatchEnvironmentVariableTypeDef",
     "BatchResourceRequirementTypeDef",
     "BatchJobDependencyTypeDef",
     "BatchRetryStrategyTypeDef",
@@ -202,18 +201,18 @@
         "LogGroupArn": NotRequired[str],
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
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "Arn": NotRequired[str],
     },
```

### Comparing `mypy-boto3-pipes-1.34.0/mypy_boto3_pipes/type_defs.pyi` & `mypy-boto3-pipes-1.34.83/mypy_boto3_pipes/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -201,18 +201,18 @@
         "LogGroupArn": NotRequired[str],
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
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "Arn": NotRequired[str],
     },
```

### Comparing `mypy-boto3-pipes-1.34.0/mypy_boto3_pipes.egg-info/PKG-INFO` & `mypy-boto3-pipes-1.34.83/mypy_boto3_pipes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pipes
-Version: 1.34.0
-Summary: Type annotations for boto3.EventBridgePipes 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.83
+Summary: Type annotations for boto3.EventBridgePipes 1.34.83 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/
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
 
 <a id="mypy-boto3-pipes"></a>
 
 # mypy-boto3-pipes
 
 [![PyPI - mypy-boto3-pipes](https://img.shields.io/pypi/v/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pipes)](https://pepy.tech/project/mypy-boto3-pipes)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgePipes 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
+[boto3.EventBridgePipes 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
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
 [mypy-boto3-pipes docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-pipes-1.34.0/mypy_boto3_pipes.egg-info/SOURCES.txt` & `mypy-boto3-pipes-1.34.83/mypy_boto3_pipes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.34.0/setup.py` & `mypy-boto3-pipes-1.34.83/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pipes",
-    version="1.34.0",
+    version="1.34.83",
     packages=["mypy_boto3_pipes"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.EventBridgePipes 1.34.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.EventBridgePipes 1.34.83 service generated with mypy-boto3-builder 7.23.2",
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
     keywords="boto3 pipes type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_pipes": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

