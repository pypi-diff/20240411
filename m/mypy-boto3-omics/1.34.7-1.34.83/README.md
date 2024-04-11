# Comparing `tmp/mypy-boto3-omics-1.34.7.tar.gz` & `tmp/mypy-boto3-omics-1.34.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-omics-1.34.7.tar", last modified: Fri Dec 22 20:32:31 2023, max compression
+gzip compressed data, was "mypy-boto3-omics-1.34.83.tar", last modified: Thu Apr 11 19:18:07 2024, max compression
```

## Comparing `mypy-boto3-omics-1.34.7.tar` & `mypy-boto3-omics-1.34.83.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:31.788707 mypy-boto3-omics-1.34.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-22 20:32:14.000000 mypy-boto3-omics-1.34.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18260 2023-12-22 20:32:31.788707 mypy-boto3-omics-1.34.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16780 2023-12-22 20:32:14.000000 mypy-boto3-omics-1.34.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:31.788707 mypy-boto3-omics-1.34.7/mypy_boto3_omics/
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2023-12-22 20:32:14.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2023-12-22 20:32:14.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      897 2023-12-22 20:32:14.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    69253 2023-12-22 20:32:15.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    69250 2023-12-22 20:32:15.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17568 2023-12-22 20:32:16.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    17568 2023-12-22 20:32:15.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24406 2023-12-22 20:32:15.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24385 2023-12-22 20:32:15.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:14.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    84762 2023-12-22 20:32:17.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    84762 2023-12-22 20:32:16.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-22 20:32:14.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    17184 2023-12-22 20:32:15.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17167 2023-12-22 20:32:15.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:31.788707 mypy-boto3-omics-1.34.7/mypy_boto3_omics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18260 2023-12-22 20:32:31.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      697 2023-12-22 20:32:31.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 20:32:31.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 20:32:31.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-22 20:32:31.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-22 20:32:31.000000 mypy-boto3-omics-1.34.7/mypy_boto3_omics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 20:32:31.788707 mypy-boto3-omics-1.34.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2023-12-22 20:32:14.000000 mypy-boto3-omics-1.34.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:07.791367 mypy-boto3-omics-1.34.83/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 19:17:36.000000 mypy-boto3-omics-1.34.83/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18328 2024-04-11 19:18:07.791367 mypy-boto3-omics-1.34.83/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16781 2024-04-11 19:17:36.000000 mypy-boto3-omics-1.34.83/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:07.791367 mypy-boto3-omics-1.34.83/mypy_boto3_omics/
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-04-11 19:17:36.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-04-11 19:17:36.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-11 19:17:36.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69342 2024-04-11 19:17:37.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69339 2024-04-11 19:17:37.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17923 2024-04-11 19:17:37.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17923 2024-04-11 19:17:37.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24406 2024-04-11 19:17:37.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24385 2024-04-11 19:17:37.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:17:36.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    85517 2024-04-11 19:17:39.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85517 2024-04-11 19:17:38.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 19:17:36.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17184 2024-04-11 19:17:37.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17167 2024-04-11 19:17:37.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:07.791367 mypy-boto3-omics-1.34.83/mypy_boto3_omics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18328 2024-04-11 19:18:07.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-11 19:18:07.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:07.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:07.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 19:18:07.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 19:18:07.000000 mypy-boto3-omics-1.34.83/mypy_boto3_omics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:18:07.791367 mypy-boto3-omics-1.34.83/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-11 19:17:36.000000 mypy-boto3-omics-1.34.83/setup.py
```

### Comparing `mypy-boto3-omics-1.34.7/LICENSE` & `mypy-boto3-omics-1.34.83/LICENSE`

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

### Comparing `mypy-boto3-omics-1.34.7/PKG-INFO` & `mypy-boto3-omics-1.34.83/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-omics
-Version: 1.34.7
-Summary: Type annotations for boto3.Omics 1.34.7 service generated with mypy-boto3-builder 7.23.0
+Version: 1.34.83
+Summary: Type annotations for boto3.Omics 1.34.83 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -25,37 +25,38 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-omics"></a>
 
 # mypy-boto3-omics
 
 [![PyPI - mypy-boto3-omics](https://img.shields.io/pypi/v/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-omics)](https://pepy.tech/project/mypy-boto3-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Omics 1.34.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[boto3.Omics 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-omics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-omics-1.34.7/README.md` & `mypy-boto3-omics-1.34.83/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-omics)](https://pepy.tech/project/mypy-boto3-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Omics 1.34.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[boto3.Omics 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-omics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-omics-1.34.7/mypy_boto3_omics/__init__.py` & `mypy-boto3-omics-1.34.83/mypy_boto3_omics/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.34.7/mypy_boto3_omics/__init__.pyi` & `mypy-boto3-omics-1.34.83/mypy_boto3_omics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.34.7/mypy_boto3_omics/__main__.py` & `mypy-boto3-omics-1.34.83/mypy_boto3_omics/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Omics 1.34.7\nVersion:         1.34.7\nBuilder version:"
-        " 7.23.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.Omics 1.34.83\n"
+        "Version:         1.34.83\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.7")
+    print("1.34.83")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-omics-1.34.7/mypy_boto3_omics/client.py` & `mypy-boto3-omics-1.34.83/mypy_boto3_omics/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    ETagAlgorithmFamilyType,
     FileTypeType,
     ReadSetFileType,
     ReadSetPartSourceType,
     ReferenceFileType,
     ResourceOwnerType,
     RunLogLevelType,
     RunRetentionModeType,
@@ -178,37 +179,34 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("OmicsClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     NotSupportedOperationException: Type[BotocoreClientError]
     RangeNotSatisfiableException: Type[BotocoreClientError]
     RequestTimeoutException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class OmicsClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/)
     """
 
     meta: ClientMeta
@@ -399,14 +397,15 @@
         *,
         name: str,
         description: str = ...,
         sseConfig: SseConfigTypeDef = ...,
         tags: Mapping[str, str] = ...,
         clientToken: str = ...,
         fallbackLocation: str = ...,
+        eTagAlgorithmFamily: ETagAlgorithmFamilyType = ...,
     ) -> CreateSequenceStoreResponseTypeDef:
         """
         Creates a sequence store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_sequence_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#create_sequence_store)
         """
```

### Comparing `mypy-boto3-omics-1.34.7/mypy_boto3_omics/client.pyi` & `mypy-boto3-omics-1.34.83/mypy_boto3_omics/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    ETagAlgorithmFamilyType,
     FileTypeType,
     ReadSetFileType,
     ReadSetPartSourceType,
     ReferenceFileType,
     ResourceOwnerType,
     RunLogLevelType,
     RunRetentionModeType,
@@ -178,34 +179,37 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("OmicsClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     NotSupportedOperationException: Type[BotocoreClientError]
     RangeNotSatisfiableException: Type[BotocoreClientError]
     RequestTimeoutException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class OmicsClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/)
     """
 
     meta: ClientMeta
@@ -396,14 +400,15 @@
         *,
         name: str,
         description: str = ...,
         sseConfig: SseConfigTypeDef = ...,
         tags: Mapping[str, str] = ...,
         clientToken: str = ...,
         fallbackLocation: str = ...,
+        eTagAlgorithmFamily: ETagAlgorithmFamilyType = ...,
     ) -> CreateSequenceStoreResponseTypeDef:
         """
         Creates a sequence store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_sequence_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#create_sequence_store)
         """
```

### Comparing `mypy-boto3-omics-1.34.7/mypy_boto3_omics/literals.py` & `mypy-boto3-omics-1.34.83/mypy_boto3_omics/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "AnnotationImportJobCreatedWaiterName",
     "AnnotationStoreCreatedWaiterName",
     "AnnotationStoreDeletedWaiterName",
     "AnnotationStoreVersionCreatedWaiterName",
     "AnnotationStoreVersionDeletedWaiterName",
     "AnnotationTypeType",
     "CreationTypeType",
+    "ETagAlgorithmFamilyType",
     "ETagAlgorithmType",
     "EncryptionTypeType",
     "FileTypeType",
     "FormatToHeaderKeyType",
     "JobStatusType",
     "ListAnnotationImportJobsPaginatorName",
     "ListAnnotationStoreVersionsPaginatorName",
@@ -113,15 +114,26 @@
     "CHR_START_END_ONE_BASE",
     "CHR_START_END_REF_ALT_ONE_BASE",
     "CHR_START_END_REF_ALT_ZERO_BASE",
     "CHR_START_END_ZERO_BASE",
     "GENERIC",
 ]
 CreationTypeType = Literal["IMPORT", "UPLOAD"]
-ETagAlgorithmType = Literal["BAM_MD5up", "CRAM_MD5up", "FASTQ_MD5up"]
+ETagAlgorithmFamilyType = Literal["MD5up", "SHA256up", "SHA512up"]
+ETagAlgorithmType = Literal[
+    "BAM_MD5up",
+    "BAM_SHA256up",
+    "BAM_SHA512up",
+    "CRAM_MD5up",
+    "CRAM_SHA256up",
+    "CRAM_SHA512up",
+    "FASTQ_MD5up",
+    "FASTQ_SHA256up",
+    "FASTQ_SHA512up",
+]
 EncryptionTypeType = Literal["KMS"]
 FileTypeType = Literal["BAM", "CRAM", "FASTQ", "UBAM"]
 FormatToHeaderKeyType = Literal["ALT", "CHR", "END", "POS", "REF", "START"]
 JobStatusType = Literal[
     "CANCELLED", "COMPLETED", "COMPLETED_WITH_FAILURES", "FAILED", "IN_PROGRESS", "SUBMITTED"
 ]
 ListAnnotationImportJobsPaginatorName = Literal["list_annotation_import_jobs"]
@@ -245,14 +257,15 @@
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
@@ -263,14 +276,15 @@
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
@@ -288,14 +302,15 @@
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
@@ -308,24 +323,26 @@
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
@@ -386,15 +403,14 @@
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
@@ -568,19 +584,21 @@
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

### Comparing `mypy-boto3-omics-1.34.7/mypy_boto3_omics/literals.pyi` & `mypy-boto3-omics-1.34.83/mypy_boto3_omics/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "AnnotationImportJobCreatedWaiterName",
     "AnnotationStoreCreatedWaiterName",
     "AnnotationStoreDeletedWaiterName",
     "AnnotationStoreVersionCreatedWaiterName",
     "AnnotationStoreVersionDeletedWaiterName",
     "AnnotationTypeType",
     "CreationTypeType",
+    "ETagAlgorithmFamilyType",
     "ETagAlgorithmType",
     "EncryptionTypeType",
     "FileTypeType",
     "FormatToHeaderKeyType",
     "JobStatusType",
     "ListAnnotationImportJobsPaginatorName",
     "ListAnnotationStoreVersionsPaginatorName",
@@ -113,15 +114,26 @@
     "CHR_START_END_ONE_BASE",
     "CHR_START_END_REF_ALT_ONE_BASE",
     "CHR_START_END_REF_ALT_ZERO_BASE",
     "CHR_START_END_ZERO_BASE",
     "GENERIC",
 ]
 CreationTypeType = Literal["IMPORT", "UPLOAD"]
-ETagAlgorithmType = Literal["BAM_MD5up", "CRAM_MD5up", "FASTQ_MD5up"]
+ETagAlgorithmFamilyType = Literal["MD5up", "SHA256up", "SHA512up"]
+ETagAlgorithmType = Literal[
+    "BAM_MD5up",
+    "BAM_SHA256up",
+    "BAM_SHA512up",
+    "CRAM_MD5up",
+    "CRAM_SHA256up",
+    "CRAM_SHA512up",
+    "FASTQ_MD5up",
+    "FASTQ_SHA256up",
+    "FASTQ_SHA512up",
+]
 EncryptionTypeType = Literal["KMS"]
 FileTypeType = Literal["BAM", "CRAM", "FASTQ", "UBAM"]
 FormatToHeaderKeyType = Literal["ALT", "CHR", "END", "POS", "REF", "START"]
 JobStatusType = Literal[
     "CANCELLED", "COMPLETED", "COMPLETED_WITH_FAILURES", "FAILED", "IN_PROGRESS", "SUBMITTED"
 ]
 ListAnnotationImportJobsPaginatorName = Literal["list_annotation_import_jobs"]
@@ -245,14 +257,15 @@
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
@@ -263,14 +276,15 @@
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
@@ -288,14 +302,15 @@
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
@@ -308,24 +323,26 @@
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
@@ -386,15 +403,14 @@
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
@@ -568,19 +584,21 @@
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

### Comparing `mypy-boto3-omics-1.34.7/mypy_boto3_omics/paginator.py` & `mypy-boto3-omics-1.34.83/mypy_boto3_omics/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.34.7/mypy_boto3_omics/paginator.pyi` & `mypy-boto3-omics-1.34.83/mypy_boto3_omics/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.34.7/mypy_boto3_omics/type_defs.py` & `mypy-boto3-omics-1.34.83/mypy_boto3_omics/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AnnotationTypeType,
     CreationTypeType,
+    ETagAlgorithmFamilyType,
     ETagAlgorithmType,
     FileTypeType,
     FormatToHeaderKeyType,
     JobStatusType,
     ReadSetActivationJobItemStatusType,
     ReadSetActivationJobStatusType,
     ReadSetExportJobItemStatusType,
@@ -101,15 +102,15 @@
     "DeleteShareRequestRequestTypeDef",
     "DeleteVariantStoreRequestRequestTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "ETagTypeDef",
     "ExportReadSetDetailTypeDef",
     "ExportReadSetJobDetailTypeDef",
     "ExportReadSetTypeDef",
-    "FileInformationTypeDef",
+    "ReadSetS3AccessTypeDef",
     "FilterTypeDef",
     "VcfOptionsTypeDef",
     "WaiterConfigTypeDef",
     "GetAnnotationImportRequestRequestTypeDef",
     "GetAnnotationStoreRequestRequestTypeDef",
     "GetAnnotationStoreVersionRequestRequestTypeDef",
     "GetReadSetActivationJobRequestRequestTypeDef",
@@ -124,14 +125,15 @@
     "GetReferenceRequestRequestTypeDef",
     "GetReferenceStoreRequestRequestTypeDef",
     "GetRunGroupRequestRequestTypeDef",
     "GetRunRequestRequestTypeDef",
     "RunLogLocationTypeDef",
     "GetRunTaskRequestRequestTypeDef",
     "GetSequenceStoreRequestRequestTypeDef",
+    "SequenceStoreS3AccessTypeDef",
     "GetShareRequestRequestTypeDef",
     "ShareDetailsTypeDef",
     "GetVariantImportRequestRequestTypeDef",
     "VariantImportItemDetailTypeDef",
     "GetVariantStoreRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "ImportReadSetJobItemTypeDef",
@@ -212,31 +214,29 @@
     "AnnotationStoreItemTypeDef",
     "CreateReferenceStoreRequestRequestTypeDef",
     "CreateReferenceStoreResponseTypeDef",
     "CreateSequenceStoreRequestRequestTypeDef",
     "CreateSequenceStoreResponseTypeDef",
     "CreateVariantStoreRequestRequestTypeDef",
     "GetReferenceStoreResponseTypeDef",
-    "GetSequenceStoreResponseTypeDef",
     "GetVariantStoreResponseTypeDef",
     "ReferenceStoreDetailTypeDef",
     "SequenceStoreDetailTypeDef",
     "VariantStoreItemTypeDef",
     "ListAnnotationStoreVersionsResponseTypeDef",
     "BatchDeleteReadSetResponseTypeDef",
     "UploadReadSetPartRequestRequestTypeDef",
     "CompleteMultipartReadSetUploadRequestRequestTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
     "GetWorkflowResponseTypeDef",
     "DeleteAnnotationStoreVersionsResponseTypeDef",
     "GetReadSetExportJobResponseTypeDef",
     "ListReadSetExportJobsResponseTypeDef",
     "StartReadSetExportJobRequestRequestTypeDef",
-    "ReadSetFilesTypeDef",
-    "ReferenceFilesTypeDef",
+    "FileInformationTypeDef",
     "ListSharesRequestRequestTypeDef",
     "GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef",
     "GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef",
     "GetAnnotationStoreRequestAnnotationStoreDeletedWaitTypeDef",
     "GetAnnotationStoreVersionRequestAnnotationStoreVersionCreatedWaitTypeDef",
     "GetAnnotationStoreVersionRequestAnnotationStoreVersionDeletedWaitTypeDef",
     "GetReadSetActivationJobRequestReadSetActivationJobCompletedWaitTypeDef",
@@ -250,14 +250,15 @@
     "GetVariantImportRequestVariantImportJobCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreDeletedWaitTypeDef",
     "GetWorkflowRequestWorkflowActiveWaitTypeDef",
     "ReadSetListItemTypeDef",
     "GetReferenceImportJobResponseTypeDef",
     "GetRunResponseTypeDef",
+    "GetSequenceStoreResponseTypeDef",
     "GetShareResponseTypeDef",
     "ListSharesResponseTypeDef",
     "GetVariantImportResponseTypeDef",
     "ListReadSetImportJobsResponseTypeDef",
     "ImportReadSetSourceItemTypeDef",
     "StartReadSetImportJobSourceItemTypeDef",
     "ListReferenceImportJobsResponseTypeDef",
@@ -309,27 +310,29 @@
     "ListReferenceStoresRequestRequestTypeDef",
     "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
     "ListSequenceStoresRequestRequestTypeDef",
     "ListAnnotationStoresResponseTypeDef",
     "ListReferenceStoresResponseTypeDef",
     "ListSequenceStoresResponseTypeDef",
     "ListVariantStoresResponseTypeDef",
-    "GetReadSetMetadataResponseTypeDef",
-    "GetReferenceMetadataResponseTypeDef",
+    "ReadSetFilesTypeDef",
+    "ReferenceFilesTypeDef",
     "ListReadSetsResponseTypeDef",
     "GetReadSetImportJobResponseTypeDef",
     "StartReadSetImportJobRequestRequestTypeDef",
     "FormatOptionsTypeDef",
     "CreateAnnotationStoreRequestRequestTypeDef",
     "CreateAnnotationStoreResponseTypeDef",
     "GetAnnotationStoreResponseTypeDef",
     "UpdateAnnotationStoreResponseTypeDef",
     "CreateAnnotationStoreVersionRequestRequestTypeDef",
     "CreateAnnotationStoreVersionResponseTypeDef",
     "GetAnnotationStoreVersionResponseTypeDef",
+    "GetReadSetMetadataResponseTypeDef",
+    "GetReferenceMetadataResponseTypeDef",
     "GetAnnotationImportResponseTypeDef",
     "StartAnnotationImportRequestRequestTypeDef",
 )
 
 AbortMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
     {
@@ -343,18 +346,18 @@
         "shareId": str,
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
 TimestampTypeDef = Union[datetime, str]
 ActivateReadSetJobItemTypeDef = TypedDict(
     "ActivateReadSetJobItemTypeDef",
     {
         "id": str,
@@ -614,20 +617,18 @@
 )
 ExportReadSetTypeDef = TypedDict(
     "ExportReadSetTypeDef",
     {
         "readSetId": str,
     },
 )
-FileInformationTypeDef = TypedDict(
-    "FileInformationTypeDef",
+ReadSetS3AccessTypeDef = TypedDict(
+    "ReadSetS3AccessTypeDef",
     {
-        "totalParts": NotRequired[int],
-        "partSize": NotRequired[int],
-        "contentLength": NotRequired[int],
+        "s3Uri": NotRequired[str],
     },
 )
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "resourceArns": NotRequired[Sequence[str]],
         "status": NotRequired[Sequence[ShareStatusType]],
@@ -782,14 +783,21 @@
 )
 GetSequenceStoreRequestRequestTypeDef = TypedDict(
     "GetSequenceStoreRequestRequestTypeDef",
     {
         "id": str,
     },
 )
+SequenceStoreS3AccessTypeDef = TypedDict(
+    "SequenceStoreS3AccessTypeDef",
+    {
+        "s3Uri": NotRequired[str],
+        "s3AccessPointArn": NotRequired[str],
+    },
+)
 GetShareRequestRequestTypeDef = TypedDict(
     "GetShareRequestRequestTypeDef",
     {
         "shareId": str,
     },
 )
 ShareDetailsTypeDef = TypedDict(
@@ -1595,26 +1603,28 @@
     {
         "name": str,
         "description": NotRequired[str],
         "sseConfig": NotRequired[SseConfigTypeDef],
         "tags": NotRequired[Mapping[str, str]],
         "clientToken": NotRequired[str],
         "fallbackLocation": NotRequired[str],
+        "eTagAlgorithmFamily": NotRequired[ETagAlgorithmFamilyType],
     },
 )
 CreateSequenceStoreResponseTypeDef = TypedDict(
     "CreateSequenceStoreResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "fallbackLocation": str,
+        "eTagAlgorithmFamily": ETagAlgorithmFamilyType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateVariantStoreRequestRequestTypeDef = TypedDict(
     "CreateVariantStoreRequestRequestTypeDef",
     {
         "reference": ReferenceItemTypeDef,
@@ -1632,27 +1642,14 @@
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-GetSequenceStoreResponseTypeDef = TypedDict(
-    "GetSequenceStoreResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "description": str,
-        "sseConfig": SseConfigTypeDef,
-        "creationTime": datetime,
-        "fallbackLocation": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 GetVariantStoreResponseTypeDef = TypedDict(
     "GetVariantStoreResponseTypeDef",
     {
         "id": str,
         "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
@@ -1684,14 +1681,15 @@
         "arn": str,
         "id": str,
         "creationTime": datetime,
         "name": NotRequired[str],
         "description": NotRequired[str],
         "sseConfig": NotRequired[SseConfigTypeDef],
         "fallbackLocation": NotRequired[str],
+        "eTagAlgorithmFamily": NotRequired[ETagAlgorithmFamilyType],
     },
 )
 VariantStoreItemTypeDef = TypedDict(
     "VariantStoreItemTypeDef",
     {
         "id": str,
         "reference": ReferenceItemTypeDef,
@@ -1813,27 +1811,21 @@
         "sequenceStoreId": str,
         "destination": str,
         "roleArn": str,
         "sources": Sequence[ExportReadSetTypeDef],
         "clientToken": NotRequired[str],
     },
 )
-ReadSetFilesTypeDef = TypedDict(
-    "ReadSetFilesTypeDef",
-    {
-        "source1": NotRequired[FileInformationTypeDef],
-        "source2": NotRequired[FileInformationTypeDef],
-        "index": NotRequired[FileInformationTypeDef],
-    },
-)
-ReferenceFilesTypeDef = TypedDict(
-    "ReferenceFilesTypeDef",
+FileInformationTypeDef = TypedDict(
+    "FileInformationTypeDef",
     {
-        "source": NotRequired[FileInformationTypeDef],
-        "index": NotRequired[FileInformationTypeDef],
+        "totalParts": NotRequired[int],
+        "partSize": NotRequired[int],
+        "contentLength": NotRequired[int],
+        "s3Access": NotRequired[ReadSetS3AccessTypeDef],
     },
 )
 ListSharesRequestRequestTypeDef = TypedDict(
     "ListSharesRequestRequestTypeDef",
     {
         "resourceOwner": ResourceOwnerType,
         "filter": NotRequired[FilterTypeDef],
@@ -2037,14 +2029,29 @@
         "failureReason": str,
         "logLocation": RunLogLocationTypeDef,
         "uuid": str,
         "runOutputUri": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+GetSequenceStoreResponseTypeDef = TypedDict(
+    "GetSequenceStoreResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "description": str,
+        "sseConfig": SseConfigTypeDef,
+        "creationTime": datetime,
+        "fallbackLocation": str,
+        "s3Access": SequenceStoreS3AccessTypeDef,
+        "eTagAlgorithmFamily": ETagAlgorithmFamilyType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 GetShareResponseTypeDef = TypedDict(
     "GetShareResponseTypeDef",
     {
         "share": ShareDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2541,50 +2548,27 @@
     "ListVariantStoresResponseTypeDef",
     {
         "variantStores": List[VariantStoreItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-GetReadSetMetadataResponseTypeDef = TypedDict(
-    "GetReadSetMetadataResponseTypeDef",
+ReadSetFilesTypeDef = TypedDict(
+    "ReadSetFilesTypeDef",
     {
-        "id": str,
-        "arn": str,
-        "sequenceStoreId": str,
-        "subjectId": str,
-        "sampleId": str,
-        "status": ReadSetStatusType,
-        "name": str,
-        "description": str,
-        "fileType": FileTypeType,
-        "creationTime": datetime,
-        "sequenceInformation": SequenceInformationTypeDef,
-        "referenceArn": str,
-        "files": ReadSetFilesTypeDef,
-        "statusMessage": str,
-        "creationType": CreationTypeType,
-        "etag": ETagTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "source1": NotRequired[FileInformationTypeDef],
+        "source2": NotRequired[FileInformationTypeDef],
+        "index": NotRequired[FileInformationTypeDef],
     },
 )
-GetReferenceMetadataResponseTypeDef = TypedDict(
-    "GetReferenceMetadataResponseTypeDef",
+ReferenceFilesTypeDef = TypedDict(
+    "ReferenceFilesTypeDef",
     {
-        "id": str,
-        "arn": str,
-        "referenceStoreId": str,
-        "md5": str,
-        "status": ReferenceStatusType,
-        "name": str,
-        "description": str,
-        "creationTime": datetime,
-        "updateTime": datetime,
-        "files": ReferenceFilesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "source": NotRequired[FileInformationTypeDef],
+        "index": NotRequired[FileInformationTypeDef],
     },
 )
 ListReadSetsResponseTypeDef = TypedDict(
     "ListReadSetsResponseTypeDef",
     {
         "nextToken": str,
         "readSets": List[ReadSetListItemTypeDef],
@@ -2722,14 +2706,52 @@
         "tags": Dict[str, str],
         "versionOptions": VersionOptionsTypeDef,
         "statusMessage": str,
         "versionSizeBytes": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+GetReadSetMetadataResponseTypeDef = TypedDict(
+    "GetReadSetMetadataResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "sequenceStoreId": str,
+        "subjectId": str,
+        "sampleId": str,
+        "status": ReadSetStatusType,
+        "name": str,
+        "description": str,
+        "fileType": FileTypeType,
+        "creationTime": datetime,
+        "sequenceInformation": SequenceInformationTypeDef,
+        "referenceArn": str,
+        "files": ReadSetFilesTypeDef,
+        "statusMessage": str,
+        "creationType": CreationTypeType,
+        "etag": ETagTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetReferenceMetadataResponseTypeDef = TypedDict(
+    "GetReferenceMetadataResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "referenceStoreId": str,
+        "md5": str,
+        "status": ReferenceStatusType,
+        "name": str,
+        "description": str,
+        "creationTime": datetime,
+        "updateTime": datetime,
+        "files": ReferenceFilesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 GetAnnotationImportResponseTypeDef = TypedDict(
     "GetAnnotationImportResponseTypeDef",
     {
         "id": str,
         "destinationName": str,
         "versionName": str,
         "roleArn": str,
```

### Comparing `mypy-boto3-omics-1.34.7/mypy_boto3_omics/type_defs.pyi` & `mypy-boto3-omics-1.34.83/mypy_boto3_omics/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AnnotationTypeType,
     CreationTypeType,
+    ETagAlgorithmFamilyType,
     ETagAlgorithmType,
     FileTypeType,
     FormatToHeaderKeyType,
     JobStatusType,
     ReadSetActivationJobItemStatusType,
     ReadSetActivationJobStatusType,
     ReadSetExportJobItemStatusType,
@@ -101,15 +102,15 @@
     "DeleteShareRequestRequestTypeDef",
     "DeleteVariantStoreRequestRequestTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "ETagTypeDef",
     "ExportReadSetDetailTypeDef",
     "ExportReadSetJobDetailTypeDef",
     "ExportReadSetTypeDef",
-    "FileInformationTypeDef",
+    "ReadSetS3AccessTypeDef",
     "FilterTypeDef",
     "VcfOptionsTypeDef",
     "WaiterConfigTypeDef",
     "GetAnnotationImportRequestRequestTypeDef",
     "GetAnnotationStoreRequestRequestTypeDef",
     "GetAnnotationStoreVersionRequestRequestTypeDef",
     "GetReadSetActivationJobRequestRequestTypeDef",
@@ -124,14 +125,15 @@
     "GetReferenceRequestRequestTypeDef",
     "GetReferenceStoreRequestRequestTypeDef",
     "GetRunGroupRequestRequestTypeDef",
     "GetRunRequestRequestTypeDef",
     "RunLogLocationTypeDef",
     "GetRunTaskRequestRequestTypeDef",
     "GetSequenceStoreRequestRequestTypeDef",
+    "SequenceStoreS3AccessTypeDef",
     "GetShareRequestRequestTypeDef",
     "ShareDetailsTypeDef",
     "GetVariantImportRequestRequestTypeDef",
     "VariantImportItemDetailTypeDef",
     "GetVariantStoreRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "ImportReadSetJobItemTypeDef",
@@ -212,31 +214,29 @@
     "AnnotationStoreItemTypeDef",
     "CreateReferenceStoreRequestRequestTypeDef",
     "CreateReferenceStoreResponseTypeDef",
     "CreateSequenceStoreRequestRequestTypeDef",
     "CreateSequenceStoreResponseTypeDef",
     "CreateVariantStoreRequestRequestTypeDef",
     "GetReferenceStoreResponseTypeDef",
-    "GetSequenceStoreResponseTypeDef",
     "GetVariantStoreResponseTypeDef",
     "ReferenceStoreDetailTypeDef",
     "SequenceStoreDetailTypeDef",
     "VariantStoreItemTypeDef",
     "ListAnnotationStoreVersionsResponseTypeDef",
     "BatchDeleteReadSetResponseTypeDef",
     "UploadReadSetPartRequestRequestTypeDef",
     "CompleteMultipartReadSetUploadRequestRequestTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
     "GetWorkflowResponseTypeDef",
     "DeleteAnnotationStoreVersionsResponseTypeDef",
     "GetReadSetExportJobResponseTypeDef",
     "ListReadSetExportJobsResponseTypeDef",
     "StartReadSetExportJobRequestRequestTypeDef",
-    "ReadSetFilesTypeDef",
-    "ReferenceFilesTypeDef",
+    "FileInformationTypeDef",
     "ListSharesRequestRequestTypeDef",
     "GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef",
     "GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef",
     "GetAnnotationStoreRequestAnnotationStoreDeletedWaitTypeDef",
     "GetAnnotationStoreVersionRequestAnnotationStoreVersionCreatedWaitTypeDef",
     "GetAnnotationStoreVersionRequestAnnotationStoreVersionDeletedWaitTypeDef",
     "GetReadSetActivationJobRequestReadSetActivationJobCompletedWaitTypeDef",
@@ -250,14 +250,15 @@
     "GetVariantImportRequestVariantImportJobCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreDeletedWaitTypeDef",
     "GetWorkflowRequestWorkflowActiveWaitTypeDef",
     "ReadSetListItemTypeDef",
     "GetReferenceImportJobResponseTypeDef",
     "GetRunResponseTypeDef",
+    "GetSequenceStoreResponseTypeDef",
     "GetShareResponseTypeDef",
     "ListSharesResponseTypeDef",
     "GetVariantImportResponseTypeDef",
     "ListReadSetImportJobsResponseTypeDef",
     "ImportReadSetSourceItemTypeDef",
     "StartReadSetImportJobSourceItemTypeDef",
     "ListReferenceImportJobsResponseTypeDef",
@@ -309,27 +310,29 @@
     "ListReferenceStoresRequestRequestTypeDef",
     "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
     "ListSequenceStoresRequestRequestTypeDef",
     "ListAnnotationStoresResponseTypeDef",
     "ListReferenceStoresResponseTypeDef",
     "ListSequenceStoresResponseTypeDef",
     "ListVariantStoresResponseTypeDef",
-    "GetReadSetMetadataResponseTypeDef",
-    "GetReferenceMetadataResponseTypeDef",
+    "ReadSetFilesTypeDef",
+    "ReferenceFilesTypeDef",
     "ListReadSetsResponseTypeDef",
     "GetReadSetImportJobResponseTypeDef",
     "StartReadSetImportJobRequestRequestTypeDef",
     "FormatOptionsTypeDef",
     "CreateAnnotationStoreRequestRequestTypeDef",
     "CreateAnnotationStoreResponseTypeDef",
     "GetAnnotationStoreResponseTypeDef",
     "UpdateAnnotationStoreResponseTypeDef",
     "CreateAnnotationStoreVersionRequestRequestTypeDef",
     "CreateAnnotationStoreVersionResponseTypeDef",
     "GetAnnotationStoreVersionResponseTypeDef",
+    "GetReadSetMetadataResponseTypeDef",
+    "GetReferenceMetadataResponseTypeDef",
     "GetAnnotationImportResponseTypeDef",
     "StartAnnotationImportRequestRequestTypeDef",
 )
 
 AbortMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
     {
@@ -343,18 +346,18 @@
         "shareId": str,
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
 TimestampTypeDef = Union[datetime, str]
 ActivateReadSetJobItemTypeDef = TypedDict(
     "ActivateReadSetJobItemTypeDef",
     {
         "id": str,
@@ -614,20 +617,18 @@
 )
 ExportReadSetTypeDef = TypedDict(
     "ExportReadSetTypeDef",
     {
         "readSetId": str,
     },
 )
-FileInformationTypeDef = TypedDict(
-    "FileInformationTypeDef",
+ReadSetS3AccessTypeDef = TypedDict(
+    "ReadSetS3AccessTypeDef",
     {
-        "totalParts": NotRequired[int],
-        "partSize": NotRequired[int],
-        "contentLength": NotRequired[int],
+        "s3Uri": NotRequired[str],
     },
 )
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "resourceArns": NotRequired[Sequence[str]],
         "status": NotRequired[Sequence[ShareStatusType]],
@@ -782,14 +783,21 @@
 )
 GetSequenceStoreRequestRequestTypeDef = TypedDict(
     "GetSequenceStoreRequestRequestTypeDef",
     {
         "id": str,
     },
 )
+SequenceStoreS3AccessTypeDef = TypedDict(
+    "SequenceStoreS3AccessTypeDef",
+    {
+        "s3Uri": NotRequired[str],
+        "s3AccessPointArn": NotRequired[str],
+    },
+)
 GetShareRequestRequestTypeDef = TypedDict(
     "GetShareRequestRequestTypeDef",
     {
         "shareId": str,
     },
 )
 ShareDetailsTypeDef = TypedDict(
@@ -1595,26 +1603,28 @@
     {
         "name": str,
         "description": NotRequired[str],
         "sseConfig": NotRequired[SseConfigTypeDef],
         "tags": NotRequired[Mapping[str, str]],
         "clientToken": NotRequired[str],
         "fallbackLocation": NotRequired[str],
+        "eTagAlgorithmFamily": NotRequired[ETagAlgorithmFamilyType],
     },
 )
 CreateSequenceStoreResponseTypeDef = TypedDict(
     "CreateSequenceStoreResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "fallbackLocation": str,
+        "eTagAlgorithmFamily": ETagAlgorithmFamilyType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateVariantStoreRequestRequestTypeDef = TypedDict(
     "CreateVariantStoreRequestRequestTypeDef",
     {
         "reference": ReferenceItemTypeDef,
@@ -1632,27 +1642,14 @@
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-GetSequenceStoreResponseTypeDef = TypedDict(
-    "GetSequenceStoreResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "description": str,
-        "sseConfig": SseConfigTypeDef,
-        "creationTime": datetime,
-        "fallbackLocation": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 GetVariantStoreResponseTypeDef = TypedDict(
     "GetVariantStoreResponseTypeDef",
     {
         "id": str,
         "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
@@ -1684,14 +1681,15 @@
         "arn": str,
         "id": str,
         "creationTime": datetime,
         "name": NotRequired[str],
         "description": NotRequired[str],
         "sseConfig": NotRequired[SseConfigTypeDef],
         "fallbackLocation": NotRequired[str],
+        "eTagAlgorithmFamily": NotRequired[ETagAlgorithmFamilyType],
     },
 )
 VariantStoreItemTypeDef = TypedDict(
     "VariantStoreItemTypeDef",
     {
         "id": str,
         "reference": ReferenceItemTypeDef,
@@ -1813,27 +1811,21 @@
         "sequenceStoreId": str,
         "destination": str,
         "roleArn": str,
         "sources": Sequence[ExportReadSetTypeDef],
         "clientToken": NotRequired[str],
     },
 )
-ReadSetFilesTypeDef = TypedDict(
-    "ReadSetFilesTypeDef",
-    {
-        "source1": NotRequired[FileInformationTypeDef],
-        "source2": NotRequired[FileInformationTypeDef],
-        "index": NotRequired[FileInformationTypeDef],
-    },
-)
-ReferenceFilesTypeDef = TypedDict(
-    "ReferenceFilesTypeDef",
+FileInformationTypeDef = TypedDict(
+    "FileInformationTypeDef",
     {
-        "source": NotRequired[FileInformationTypeDef],
-        "index": NotRequired[FileInformationTypeDef],
+        "totalParts": NotRequired[int],
+        "partSize": NotRequired[int],
+        "contentLength": NotRequired[int],
+        "s3Access": NotRequired[ReadSetS3AccessTypeDef],
     },
 )
 ListSharesRequestRequestTypeDef = TypedDict(
     "ListSharesRequestRequestTypeDef",
     {
         "resourceOwner": ResourceOwnerType,
         "filter": NotRequired[FilterTypeDef],
@@ -2037,14 +2029,29 @@
         "failureReason": str,
         "logLocation": RunLogLocationTypeDef,
         "uuid": str,
         "runOutputUri": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+GetSequenceStoreResponseTypeDef = TypedDict(
+    "GetSequenceStoreResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "description": str,
+        "sseConfig": SseConfigTypeDef,
+        "creationTime": datetime,
+        "fallbackLocation": str,
+        "s3Access": SequenceStoreS3AccessTypeDef,
+        "eTagAlgorithmFamily": ETagAlgorithmFamilyType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 GetShareResponseTypeDef = TypedDict(
     "GetShareResponseTypeDef",
     {
         "share": ShareDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2541,50 +2548,27 @@
     "ListVariantStoresResponseTypeDef",
     {
         "variantStores": List[VariantStoreItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-GetReadSetMetadataResponseTypeDef = TypedDict(
-    "GetReadSetMetadataResponseTypeDef",
+ReadSetFilesTypeDef = TypedDict(
+    "ReadSetFilesTypeDef",
     {
-        "id": str,
-        "arn": str,
-        "sequenceStoreId": str,
-        "subjectId": str,
-        "sampleId": str,
-        "status": ReadSetStatusType,
-        "name": str,
-        "description": str,
-        "fileType": FileTypeType,
-        "creationTime": datetime,
-        "sequenceInformation": SequenceInformationTypeDef,
-        "referenceArn": str,
-        "files": ReadSetFilesTypeDef,
-        "statusMessage": str,
-        "creationType": CreationTypeType,
-        "etag": ETagTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "source1": NotRequired[FileInformationTypeDef],
+        "source2": NotRequired[FileInformationTypeDef],
+        "index": NotRequired[FileInformationTypeDef],
     },
 )
-GetReferenceMetadataResponseTypeDef = TypedDict(
-    "GetReferenceMetadataResponseTypeDef",
+ReferenceFilesTypeDef = TypedDict(
+    "ReferenceFilesTypeDef",
     {
-        "id": str,
-        "arn": str,
-        "referenceStoreId": str,
-        "md5": str,
-        "status": ReferenceStatusType,
-        "name": str,
-        "description": str,
-        "creationTime": datetime,
-        "updateTime": datetime,
-        "files": ReferenceFilesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "source": NotRequired[FileInformationTypeDef],
+        "index": NotRequired[FileInformationTypeDef],
     },
 )
 ListReadSetsResponseTypeDef = TypedDict(
     "ListReadSetsResponseTypeDef",
     {
         "nextToken": str,
         "readSets": List[ReadSetListItemTypeDef],
@@ -2722,14 +2706,52 @@
         "tags": Dict[str, str],
         "versionOptions": VersionOptionsTypeDef,
         "statusMessage": str,
         "versionSizeBytes": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+GetReadSetMetadataResponseTypeDef = TypedDict(
+    "GetReadSetMetadataResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "sequenceStoreId": str,
+        "subjectId": str,
+        "sampleId": str,
+        "status": ReadSetStatusType,
+        "name": str,
+        "description": str,
+        "fileType": FileTypeType,
+        "creationTime": datetime,
+        "sequenceInformation": SequenceInformationTypeDef,
+        "referenceArn": str,
+        "files": ReadSetFilesTypeDef,
+        "statusMessage": str,
+        "creationType": CreationTypeType,
+        "etag": ETagTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetReferenceMetadataResponseTypeDef = TypedDict(
+    "GetReferenceMetadataResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "referenceStoreId": str,
+        "md5": str,
+        "status": ReferenceStatusType,
+        "name": str,
+        "description": str,
+        "creationTime": datetime,
+        "updateTime": datetime,
+        "files": ReferenceFilesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 GetAnnotationImportResponseTypeDef = TypedDict(
     "GetAnnotationImportResponseTypeDef",
     {
         "id": str,
         "destinationName": str,
         "versionName": str,
         "roleArn": str,
```

### Comparing `mypy-boto3-omics-1.34.7/mypy_boto3_omics/waiter.py` & `mypy-boto3-omics-1.34.83/mypy_boto3_omics/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.34.7/mypy_boto3_omics/waiter.pyi` & `mypy-boto3-omics-1.34.83/mypy_boto3_omics/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.34.7/mypy_boto3_omics.egg-info/PKG-INFO` & `mypy-boto3-omics-1.34.83/mypy_boto3_omics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-omics
-Version: 1.34.7
-Summary: Type annotations for boto3.Omics 1.34.7 service generated with mypy-boto3-builder 7.23.0
+Version: 1.34.83
+Summary: Type annotations for boto3.Omics 1.34.83 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -25,37 +25,38 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-omics"></a>
 
 # mypy-boto3-omics
 
 [![PyPI - mypy-boto3-omics](https://img.shields.io/pypi/v/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-omics)](https://pepy.tech/project/mypy-boto3-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Omics 1.34.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[boto3.Omics 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-omics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-omics-1.34.7/mypy_boto3_omics.egg-info/SOURCES.txt` & `mypy-boto3-omics-1.34.83/mypy_boto3_omics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.34.7/setup.py` & `mypy-boto3-omics-1.34.83/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,23 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-omics",
-    version="1.34.7",
+    version="1.34.83",
     packages=["mypy_boto3_omics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.Omics 1.34.7 service generated with mypy-boto3-builder 7.23.0"
-    ),
+    description="Type annotations for boto3.Omics 1.34.83 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

