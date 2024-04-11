# Comparing `tmp/mypy-boto3-iam-1.34.8.tar.gz` & `tmp/mypy-boto3-iam-1.34.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iam-1.34.8.tar", last modified: Tue Dec 26 20:32:09 2023, max compression
+gzip compressed data, was "mypy-boto3-iam-1.34.83.tar", last modified: Thu Apr 11 19:18:07 2024, max compression
```

## Comparing `mypy-boto3-iam-1.34.8.tar` & `mypy-boto3-iam-1.34.83.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 20:32:09.760571 mypy-boto3-iam-1.34.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-26 20:31:53.000000 mypy-boto3-iam-1.34.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22358 2023-12-26 20:32:09.760571 mypy-boto3-iam-1.34.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20886 2023-12-26 20:31:53.000000 mypy-boto3-iam-1.34.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 20:32:09.760571 mypy-boto3-iam-1.34.8/mypy_boto3_iam/
--rw-r--r--   0 runner    (1001) docker     (127)     8784 2023-12-26 20:31:53.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8784 2023-12-26 20:31:53.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-26 20:31:53.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   113574 2023-12-26 20:31:55.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   113571 2023-12-26 20:31:54.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16134 2023-12-26 20:31:56.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16134 2023-12-26 20:31:56.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    38443 2023-12-26 20:31:56.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    38408 2023-12-26 20:31:56.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-26 20:31:53.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   142074 2023-12-26 20:31:55.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)   142003 2023-12-26 20:31:55.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   112203 2023-12-26 20:31:58.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   112203 2023-12-26 20:31:57.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-26 20:31:53.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2023-12-26 20:31:56.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2023-12-26 20:31:56.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 20:32:09.760571 mypy-boto3-iam-1.34.8/mypy_boto3_iam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22358 2023-12-26 20:32:09.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      726 2023-12-26 20:32:09.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-26 20:32:09.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-26 20:32:09.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-26 20:32:09.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-26 20:32:09.000000 mypy-boto3-iam-1.34.8/mypy_boto3_iam.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-26 20:32:09.760571 mypy-boto3-iam-1.34.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2023-12-26 20:31:53.000000 mypy-boto3-iam-1.34.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:07.043377 mypy-boto3-iam-1.34.83/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 19:17:21.000000 mypy-boto3-iam-1.34.83/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22426 2024-04-11 19:18:07.043377 mypy-boto3-iam-1.34.83/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20887 2024-04-11 19:17:21.000000 mypy-boto3-iam-1.34.83/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:07.043377 mypy-boto3-iam-1.34.83/mypy_boto3_iam/
+-rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-04-11 19:17:21.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-04-11 19:17:21.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-11 19:17:21.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113655 2024-04-11 19:17:22.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113652 2024-04-11 19:17:22.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16250 2024-04-11 19:17:24.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16250 2024-04-11 19:17:24.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    38443 2024-04-11 19:17:24.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38408 2024-04-11 19:17:23.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:17:21.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   142645 2024-04-11 19:17:23.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)   142574 2024-04-11 19:17:23.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   112202 2024-04-11 19:17:26.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112202 2024-04-11 19:17:25.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 19:17:21.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-11 19:17:24.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-11 19:17:24.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:07.043377 mypy-boto3-iam-1.34.83/mypy_boto3_iam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22426 2024-04-11 19:18:07.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-11 19:18:07.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:07.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:07.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 19:18:07.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 19:18:07.000000 mypy-boto3-iam-1.34.83/mypy_boto3_iam.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:18:07.043377 mypy-boto3-iam-1.34.83/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-11 19:17:21.000000 mypy-boto3-iam-1.34.83/setup.py
```

### Comparing `mypy-boto3-iam-1.34.8/LICENSE` & `mypy-boto3-iam-1.34.83/LICENSE`

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

### Comparing `mypy-boto3-iam-1.34.8/PKG-INFO` & `mypy-boto3-iam-1.34.83/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iam
-Version: 1.34.8
-Summary: Type annotations for boto3.IAM 1.34.8 service generated with mypy-boto3-builder 7.23.0
+Version: 1.34.83
+Summary: Type annotations for boto3.IAM 1.34.83 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/
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
 
 <a id="mypy-boto3-iam"></a>
 
 # mypy-boto3-iam
 
 [![PyPI - mypy-boto3-iam](https://img.shields.io/pypi/v/mypy-boto3-iam.svg?color=blue)](https://pypi.org/project/mypy-boto3-iam)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iam.svg?color=blue)](https://pypi.org/project/mypy-boto3-iam)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iam)](https://pepy.tech/project/mypy-boto3-iam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAM 1.34.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
+[boto3.IAM 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
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
 [mypy-boto3-iam docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iam-1.34.8/README.md` & `mypy-boto3-iam-1.34.83/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iam.svg?color=blue)](https://pypi.org/project/mypy-boto3-iam)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iam)](https://pepy.tech/project/mypy-boto3-iam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAM 1.34.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
+[boto3.IAM 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
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
 [mypy-boto3-iam docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iam-1.34.8/mypy_boto3_iam/__init__.py` & `mypy-boto3-iam-1.34.83/mypy_boto3_iam/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.34.8/mypy_boto3_iam/__init__.pyi` & `mypy-boto3-iam-1.34.83/mypy_boto3_iam/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.34.8/mypy_boto3_iam/__main__.py` & `mypy-boto3-iam-1.34.83/mypy_boto3_iam/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IAM 1.34.8\nVersion:         1.34.8\nBuilder version:"
-        " 7.23.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.IAM 1.34.83\n"
+        "Version:         1.34.83\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.8")
+    print("1.34.83")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-iam-1.34.8/mypy_boto3_iam/client.py` & `mypy-boto3-iam-1.34.83/mypy_boto3_iam/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,14 +194,15 @@
     InvalidPublicKeyException: Type[BotocoreClientError]
     InvalidUserTypeException: Type[BotocoreClientError]
     KeyPairMismatchException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     MalformedCertificateException: Type[BotocoreClientError]
     MalformedPolicyDocumentException: Type[BotocoreClientError]
     NoSuchEntityException: Type[BotocoreClientError]
+    OpenIdIdpCommunicationErrorException: Type[BotocoreClientError]
     PasswordPolicyViolationException: Type[BotocoreClientError]
     PolicyEvaluationException: Type[BotocoreClientError]
     PolicyNotAttachableException: Type[BotocoreClientError]
     ReportGenerationLimitExceededException: Type[BotocoreClientError]
     ServiceFailureException: Type[BotocoreClientError]
     ServiceNotSupportedException: Type[BotocoreClientError]
     UnmodifiableEntityException: Type[BotocoreClientError]
@@ -353,16 +354,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_login_profile)
         """
 
     def create_open_id_connect_provider(
         self,
         *,
         Url: str,
-        ThumbprintList: Sequence[str],
         ClientIDList: Sequence[str] = ...,
+        ThumbprintList: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateOpenIDConnectProviderResponseTypeDef:
         """
         Creates an IAM entity to describe an identity provider (IdP) that supports
         `OpenID Connect (OIDC)
         <http://openid.net/connect/>`__.
 
@@ -1498,15 +1499,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#remove_client_id_from_open_id_connect_provider)
         """
 
     def remove_role_from_instance_profile(
         self, *, InstanceProfileName: str, RoleName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Removes the specified IAM role from the specified EC2 instance profile.
+        Removes the specified IAM role from the specified Amazon EC2 instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.remove_role_from_instance_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#remove_role_from_instance_profile)
         """
 
     def remove_user_from_group(
         self, *, GroupName: str, UserName: str
```

### Comparing `mypy-boto3-iam-1.34.8/mypy_boto3_iam/client.pyi` & `mypy-boto3-iam-1.34.83/mypy_boto3_iam/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -192,14 +192,15 @@
     InvalidPublicKeyException: Type[BotocoreClientError]
     InvalidUserTypeException: Type[BotocoreClientError]
     KeyPairMismatchException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     MalformedCertificateException: Type[BotocoreClientError]
     MalformedPolicyDocumentException: Type[BotocoreClientError]
     NoSuchEntityException: Type[BotocoreClientError]
+    OpenIdIdpCommunicationErrorException: Type[BotocoreClientError]
     PasswordPolicyViolationException: Type[BotocoreClientError]
     PolicyEvaluationException: Type[BotocoreClientError]
     PolicyNotAttachableException: Type[BotocoreClientError]
     ReportGenerationLimitExceededException: Type[BotocoreClientError]
     ServiceFailureException: Type[BotocoreClientError]
     ServiceNotSupportedException: Type[BotocoreClientError]
     UnmodifiableEntityException: Type[BotocoreClientError]
@@ -350,16 +351,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_login_profile)
         """
 
     def create_open_id_connect_provider(
         self,
         *,
         Url: str,
-        ThumbprintList: Sequence[str],
         ClientIDList: Sequence[str] = ...,
+        ThumbprintList: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateOpenIDConnectProviderResponseTypeDef:
         """
         Creates an IAM entity to describe an identity provider (IdP) that supports
         `OpenID Connect (OIDC)
         <http://openid.net/connect/>`__.
 
@@ -1495,15 +1496,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#remove_client_id_from_open_id_connect_provider)
         """
 
     def remove_role_from_instance_profile(
         self, *, InstanceProfileName: str, RoleName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Removes the specified IAM role from the specified EC2 instance profile.
+        Removes the specified IAM role from the specified Amazon EC2 instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.remove_role_from_instance_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#remove_role_from_instance_profile)
         """
 
     def remove_user_from_group(
         self, *, GroupName: str, UserName: str
```

### Comparing `mypy-boto3-iam-1.34.8/mypy_boto3_iam/literals.py` & `mypy-boto3-iam-1.34.83/mypy_boto3_iam/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,14 +213,15 @@
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
@@ -231,14 +232,15 @@
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
@@ -256,14 +258,15 @@
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
@@ -276,24 +279,26 @@
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
@@ -354,15 +359,14 @@
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
@@ -536,19 +540,21 @@
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

### Comparing `mypy-boto3-iam-1.34.8/mypy_boto3_iam/literals.pyi` & `mypy-boto3-iam-1.34.83/mypy_boto3_iam/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -213,14 +213,15 @@
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
@@ -231,14 +232,15 @@
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
@@ -256,14 +258,15 @@
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
@@ -276,24 +279,26 @@
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
@@ -354,15 +359,14 @@
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
@@ -536,19 +540,21 @@
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

### Comparing `mypy-boto3-iam-1.34.8/mypy_boto3_iam/paginator.py` & `mypy-boto3-iam-1.34.83/mypy_boto3_iam/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.34.8/mypy_boto3_iam/paginator.pyi` & `mypy-boto3-iam-1.34.83/mypy_boto3_iam/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.34.8/mypy_boto3_iam/service_resource.py` & `mypy-boto3-iam-1.34.83/mypy_boto3_iam/service_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     assignmentStatusTypeType,
     policyScopeTypeType,
     statusTypeType,
     summaryKeyTypeType,
 )
 from .type_defs import (
     AttachedPermissionsBoundaryResponseTypeDef,
-    AttachedPermissionsBoundaryTypeDef,
     PolicyDocumentTypeDef,
     RoleLastUsedResponseTypeDef,
     RoleTypeDef,
     ServerCertificateMetadataResponseTypeDef,
     TagTypeDef,
     UpdateSAMLProviderResponseTypeDef,
     UserResponseTypeDef,
@@ -1256,14 +1255,15 @@
     access_key_id: str
     status: statusTypeType
     secret_access_key: str
     create_date: datetime
     user_name: str
     id: str
     secret: str
+    meta: "IAMResourceMeta"
 
     def activate(self, *, Status: statusTypeType = "Active") -> None:
         """
         Changes the status of the specified access key from Active to Inactive, or vice
         versa.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccessKeyPair.activate)
@@ -1311,14 +1311,15 @@
     require_uppercase_characters: bool
     require_lowercase_characters: bool
     allow_users_to_change_password: bool
     expire_passwords: bool
     max_password_age: int
     password_reuse_prevention: int
     hard_expiry: bool
+    meta: "IAMResourceMeta"
 
     def delete(self) -> None:
         """
         Deletes the password policy for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccountPasswordPolicy.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#accountpasswordpolicydelete-method)
@@ -1379,14 +1380,15 @@
 class AccountSummary(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccountSummary)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#accountsummary)
     """
 
     summary_map: Dict[summaryKeyTypeType, int]
+    meta: "IAMResourceMeta"
 
     def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccountSummary.get_available_subresources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#accountsummaryget_available_subresources-method)
@@ -1424,20 +1426,21 @@
 
     path: str
     user_name: str
     user_id: str
     arn: str
     create_date: datetime
     password_last_used: datetime
-    permissions_boundary: AttachedPermissionsBoundaryTypeDef
+    permissions_boundary: AttachedPermissionsBoundaryResponseTypeDef
     tags: List[TagTypeDef]
     user: "User"
     access_keys: CurrentUserAccessKeysCollection
     mfa_devices: CurrentUserMfaDevicesCollection
     signing_certificates: CurrentUserSigningCertificatesCollection
+    meta: "IAMResourceMeta"
 
     def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.CurrentUser.get_available_subresources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#currentuserget_available_subresources-method)
@@ -1478,14 +1481,15 @@
     instance_profile_id: str
     arn: str
     create_date: datetime
     roles_attribute: List[RoleTypeDef]
     tags: List[TagTypeDef]
     name: str
     roles: List["Role"]
+    meta: "IAMResourceMeta"
 
     def add_role(self, *, RoleName: str) -> None:
         """
         Adds the specified IAM role to the specified instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.InstanceProfile.add_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#instanceprofileadd_role-method)
@@ -1525,15 +1529,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.InstanceProfile.reload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#instanceprofilereload-method)
         """
 
     def remove_role(self, *, RoleName: str) -> None:
         """
-        Removes the specified IAM role from the specified EC2 instance profile.
+        Removes the specified IAM role from the specified Amazon EC2 instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.InstanceProfile.remove_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#instanceprofileremove_role-method)
         """
 
 
 _InstanceProfile = InstanceProfile
@@ -1546,14 +1550,15 @@
     """
 
     document: PolicyDocumentTypeDef
     is_default_version: bool
     create_date: datetime
     arn: str
     version_id: str
+    meta: "IAMResourceMeta"
 
     def delete(self) -> None:
         """
         Deletes the specified version from the specified managed policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.PolicyVersion.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#policyversiondelete-method)
@@ -1608,14 +1613,15 @@
     """
 
     saml_metadata_document: str
     create_date: datetime
     valid_until: datetime
     tags: List[TagTypeDef]
     arn: str
+    meta: "IAMResourceMeta"
 
     def delete(self) -> None:
         """
         Deletes a SAML provider resource in IAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#samlproviderdelete-method)
@@ -1670,14 +1676,15 @@
     base32_string_seed: bytes
     qr_code_png: bytes
     user_attribute: UserResponseTypeDef
     enable_date: datetime
     tags: List[TagTypeDef]
     serial_number: str
     user: "User"
+    meta: "IAMResourceMeta"
 
     def delete(self) -> None:
         """
         Deletes a virtual MFA device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.VirtualMfaDevice.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#virtualmfadevicedelete-method)
@@ -1702,14 +1709,15 @@
     """
 
     access_key_id: str
     status: statusTypeType
     create_date: datetime
     user_name: str
     id: str
+    meta: "IAMResourceMeta"
 
     def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccessKey.User)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#accesskeyuser-method)
@@ -1756,14 +1764,15 @@
 class AssumeRolePolicy(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AssumeRolePolicy)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#assumerolepolicy)
     """
 
     role_name: str
+    meta: "IAMResourceMeta"
 
     def Role(self) -> "_Role":
         """
         Creates a Role resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AssumeRolePolicy.Role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#assumerolepolicyrole-method)
@@ -1795,14 +1804,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#grouppolicy)
     """
 
     policy_name: str
     policy_document: PolicyDocumentTypeDef
     group_name: str
     name: str
+    meta: "IAMResourceMeta"
 
     def Group(self) -> "_Group":
         """
         Creates a Group resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.GroupPolicy.Group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#grouppolicygroup-method)
@@ -1862,14 +1872,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.MfaDevice)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#mfadevice)
     """
 
     enable_date: datetime
     user_name: str
     serial_number: str
+    meta: "IAMResourceMeta"
 
     def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.MfaDevice.User)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#mfadeviceuser-method)
@@ -1934,14 +1945,15 @@
     tags: List[TagTypeDef]
     arn: str
     default_version: "PolicyVersion"
     attached_groups: PolicyAttachedGroupsCollection
     attached_roles: PolicyAttachedRolesCollection
     attached_users: PolicyAttachedUsersCollection
     versions: PolicyVersionsCollection
+    meta: "IAMResourceMeta"
 
     def attach_group(self, *, GroupName: str) -> None:
         """
         Attaches the specified managed policy to the specified IAM group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.attach_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#policyattach_group-method)
@@ -2039,14 +2051,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#rolepolicy)
     """
 
     policy_name: str
     policy_document: PolicyDocumentTypeDef
     role_name: str
     name: str
+    meta: "IAMResourceMeta"
 
     def Role(self) -> "_Role":
         """
         Creates a Role resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.RolePolicy.Role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#rolepolicyrole-method)
@@ -2108,14 +2121,15 @@
     """
 
     server_certificate_metadata: ServerCertificateMetadataResponseTypeDef
     certificate_body: str
     certificate_chain: str
     tags: List[TagTypeDef]
     name: str
+    meta: "IAMResourceMeta"
 
     def delete(self) -> None:
         """
         Deletes the specified server certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServerCertificate.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#servercertificatedelete-method)
@@ -2172,14 +2186,15 @@
 
     certificate_id: str
     certificate_body: str
     status: statusTypeType
     upload_date: datetime
     user_name: str
     id: str
+    meta: "IAMResourceMeta"
 
     def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SigningCertificate.User)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#signingcertificateuser-method)
@@ -2231,14 +2246,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#userpolicy)
     """
 
     policy_name: str
     policy_document: PolicyDocumentTypeDef
     user_name: str
     name: str
+    meta: "IAMResourceMeta"
 
     def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.UserPolicy.User)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#userpolicyuser-method)
@@ -2304,14 +2320,15 @@
     group_id: str
     arn: str
     create_date: datetime
     name: str
     attached_policies: GroupAttachedPoliciesCollection
     policies: GroupPoliciesCollection
     users: GroupUsersCollection
+    meta: "IAMResourceMeta"
 
     def Policy(self, name: str) -> "_GroupPolicy":
         """
         Creates a GroupPolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.Policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#grouppolicy-method)
@@ -2417,14 +2434,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.LoginProfile)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#loginprofile)
     """
 
     create_date: datetime
     password_reset_required: bool
     user_name: str
+    meta: "IAMResourceMeta"
 
     def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.LoginProfile.User)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#loginprofileuser-method)
@@ -2498,21 +2516,22 @@
     role_name: str
     role_id: str
     arn: str
     create_date: datetime
     assume_role_policy_document: PolicyDocumentTypeDef
     description: str
     max_session_duration: int
-    permissions_boundary: AttachedPermissionsBoundaryTypeDef
+    permissions_boundary: AttachedPermissionsBoundaryResponseTypeDef
     tags: List[TagTypeDef]
     role_last_used: RoleLastUsedResponseTypeDef
     name: str
     attached_policies: RoleAttachedPoliciesCollection
     instance_profiles: RoleInstanceProfilesCollection
     policies: RolePoliciesCollection
+    meta: "IAMResourceMeta"
 
     def AssumeRolePolicy(self) -> "_AssumeRolePolicy":
         """
         Creates a AssumeRolePolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Role.AssumeRolePolicy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#roleassumerolepolicy-method)
@@ -2597,14 +2616,15 @@
     name: str
     access_keys: UserAccessKeysCollection
     attached_policies: UserAttachedPoliciesCollection
     groups: UserGroupsCollection
     mfa_devices: UserMfaDevicesCollection
     policies: UserPoliciesCollection
     signing_certificates: UserSigningCertificatesCollection
+    meta: "IAMResourceMeta"
 
     def AccessKey(self, id: str) -> "_AccessKey":
         """
         Creates a AccessKey resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.AccessKey)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#useraccesskey-method)
```

### Comparing `mypy-boto3-iam-1.34.8/mypy_boto3_iam/service_resource.pyi` & `mypy-boto3-iam-1.34.83/mypy_boto3_iam/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     assignmentStatusTypeType,
     policyScopeTypeType,
     statusTypeType,
     summaryKeyTypeType,
 )
 from .type_defs import (
     AttachedPermissionsBoundaryResponseTypeDef,
-    AttachedPermissionsBoundaryTypeDef,
     PolicyDocumentTypeDef,
     RoleLastUsedResponseTypeDef,
     RoleTypeDef,
     ServerCertificateMetadataResponseTypeDef,
     TagTypeDef,
     UpdateSAMLProviderResponseTypeDef,
     UserResponseTypeDef,
@@ -1228,14 +1227,15 @@
     access_key_id: str
     status: statusTypeType
     secret_access_key: str
     create_date: datetime
     user_name: str
     id: str
     secret: str
+    meta: "IAMResourceMeta"
 
     def activate(self, *, Status: statusTypeType = "Active") -> None:
         """
         Changes the status of the specified access key from Active to Inactive, or vice
         versa.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccessKeyPair.activate)
@@ -1281,14 +1281,15 @@
     require_uppercase_characters: bool
     require_lowercase_characters: bool
     allow_users_to_change_password: bool
     expire_passwords: bool
     max_password_age: int
     password_reuse_prevention: int
     hard_expiry: bool
+    meta: "IAMResourceMeta"
 
     def delete(self) -> None:
         """
         Deletes the password policy for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccountPasswordPolicy.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#accountpasswordpolicydelete-method)
@@ -1347,14 +1348,15 @@
 class AccountSummary(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AccountSummary)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#accountsummary)
     """
 
     summary_map: Dict[summaryKeyTypeType, int]
+    meta: "IAMResourceMeta"
 
     def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccountSummary.get_available_subresources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#accountsummaryget_available_subresources-method)
@@ -1390,20 +1392,21 @@
 
     path: str
     user_name: str
     user_id: str
     arn: str
     create_date: datetime
     password_last_used: datetime
-    permissions_boundary: AttachedPermissionsBoundaryTypeDef
+    permissions_boundary: AttachedPermissionsBoundaryResponseTypeDef
     tags: List[TagTypeDef]
     user: "User"
     access_keys: CurrentUserAccessKeysCollection
     mfa_devices: CurrentUserMfaDevicesCollection
     signing_certificates: CurrentUserSigningCertificatesCollection
+    meta: "IAMResourceMeta"
 
     def get_available_subresources(self) -> Sequence[str]:
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.CurrentUser.get_available_subresources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#currentuserget_available_subresources-method)
@@ -1442,14 +1445,15 @@
     instance_profile_id: str
     arn: str
     create_date: datetime
     roles_attribute: List[RoleTypeDef]
     tags: List[TagTypeDef]
     name: str
     roles: List["Role"]
+    meta: "IAMResourceMeta"
 
     def add_role(self, *, RoleName: str) -> None:
         """
         Adds the specified IAM role to the specified instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.InstanceProfile.add_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#instanceprofileadd_role-method)
@@ -1489,15 +1493,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.InstanceProfile.reload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#instanceprofilereload-method)
         """
 
     def remove_role(self, *, RoleName: str) -> None:
         """
-        Removes the specified IAM role from the specified EC2 instance profile.
+        Removes the specified IAM role from the specified Amazon EC2 instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.InstanceProfile.remove_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#instanceprofileremove_role-method)
         """
 
 _InstanceProfile = InstanceProfile
 
@@ -1508,14 +1512,15 @@
     """
 
     document: PolicyDocumentTypeDef
     is_default_version: bool
     create_date: datetime
     arn: str
     version_id: str
+    meta: "IAMResourceMeta"
 
     def delete(self) -> None:
         """
         Deletes the specified version from the specified managed policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.PolicyVersion.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#policyversiondelete-method)
@@ -1568,14 +1573,15 @@
     """
 
     saml_metadata_document: str
     create_date: datetime
     valid_until: datetime
     tags: List[TagTypeDef]
     arn: str
+    meta: "IAMResourceMeta"
 
     def delete(self) -> None:
         """
         Deletes a SAML provider resource in IAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#samlproviderdelete-method)
@@ -1628,14 +1634,15 @@
     base32_string_seed: bytes
     qr_code_png: bytes
     user_attribute: UserResponseTypeDef
     enable_date: datetime
     tags: List[TagTypeDef]
     serial_number: str
     user: "User"
+    meta: "IAMResourceMeta"
 
     def delete(self) -> None:
         """
         Deletes a virtual MFA device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.VirtualMfaDevice.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#virtualmfadevicedelete-method)
@@ -1658,14 +1665,15 @@
     """
 
     access_key_id: str
     status: statusTypeType
     create_date: datetime
     user_name: str
     id: str
+    meta: "IAMResourceMeta"
 
     def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AccessKey.User)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#accesskeyuser-method)
@@ -1710,14 +1718,15 @@
 class AssumeRolePolicy(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.AssumeRolePolicy)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#assumerolepolicy)
     """
 
     role_name: str
+    meta: "IAMResourceMeta"
 
     def Role(self) -> "_Role":
         """
         Creates a Role resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.AssumeRolePolicy.Role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#assumerolepolicyrole-method)
@@ -1747,14 +1756,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#grouppolicy)
     """
 
     policy_name: str
     policy_document: PolicyDocumentTypeDef
     group_name: str
     name: str
+    meta: "IAMResourceMeta"
 
     def Group(self) -> "_Group":
         """
         Creates a Group resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.GroupPolicy.Group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#grouppolicygroup-method)
@@ -1812,14 +1822,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.MfaDevice)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#mfadevice)
     """
 
     enable_date: datetime
     user_name: str
     serial_number: str
+    meta: "IAMResourceMeta"
 
     def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.MfaDevice.User)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#mfadeviceuser-method)
@@ -1882,14 +1893,15 @@
     tags: List[TagTypeDef]
     arn: str
     default_version: "PolicyVersion"
     attached_groups: PolicyAttachedGroupsCollection
     attached_roles: PolicyAttachedRolesCollection
     attached_users: PolicyAttachedUsersCollection
     versions: PolicyVersionsCollection
+    meta: "IAMResourceMeta"
 
     def attach_group(self, *, GroupName: str) -> None:
         """
         Attaches the specified managed policy to the specified IAM group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Policy.attach_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#policyattach_group-method)
@@ -1985,14 +1997,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#rolepolicy)
     """
 
     policy_name: str
     policy_document: PolicyDocumentTypeDef
     role_name: str
     name: str
+    meta: "IAMResourceMeta"
 
     def Role(self) -> "_Role":
         """
         Creates a Role resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.RolePolicy.Role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#rolepolicyrole-method)
@@ -2052,14 +2065,15 @@
     """
 
     server_certificate_metadata: ServerCertificateMetadataResponseTypeDef
     certificate_body: str
     certificate_chain: str
     tags: List[TagTypeDef]
     name: str
+    meta: "IAMResourceMeta"
 
     def delete(self) -> None:
         """
         Deletes the specified server certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServerCertificate.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#servercertificatedelete-method)
@@ -2114,14 +2128,15 @@
 
     certificate_id: str
     certificate_body: str
     status: statusTypeType
     upload_date: datetime
     user_name: str
     id: str
+    meta: "IAMResourceMeta"
 
     def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SigningCertificate.User)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#signingcertificateuser-method)
@@ -2171,14 +2186,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#userpolicy)
     """
 
     policy_name: str
     policy_document: PolicyDocumentTypeDef
     user_name: str
     name: str
+    meta: "IAMResourceMeta"
 
     def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.UserPolicy.User)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#userpolicyuser-method)
@@ -2242,14 +2258,15 @@
     group_id: str
     arn: str
     create_date: datetime
     name: str
     attached_policies: GroupAttachedPoliciesCollection
     policies: GroupPoliciesCollection
     users: GroupUsersCollection
+    meta: "IAMResourceMeta"
 
     def Policy(self, name: str) -> "_GroupPolicy":
         """
         Creates a GroupPolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Group.Policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#grouppolicy-method)
@@ -2353,14 +2370,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.LoginProfile)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#loginprofile)
     """
 
     create_date: datetime
     password_reset_required: bool
     user_name: str
+    meta: "IAMResourceMeta"
 
     def User(self) -> "_User":
         """
         Creates a User resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.LoginProfile.User)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#loginprofileuser-method)
@@ -2432,21 +2450,22 @@
     role_name: str
     role_id: str
     arn: str
     create_date: datetime
     assume_role_policy_document: PolicyDocumentTypeDef
     description: str
     max_session_duration: int
-    permissions_boundary: AttachedPermissionsBoundaryTypeDef
+    permissions_boundary: AttachedPermissionsBoundaryResponseTypeDef
     tags: List[TagTypeDef]
     role_last_used: RoleLastUsedResponseTypeDef
     name: str
     attached_policies: RoleAttachedPoliciesCollection
     instance_profiles: RoleInstanceProfilesCollection
     policies: RolePoliciesCollection
+    meta: "IAMResourceMeta"
 
     def AssumeRolePolicy(self) -> "_AssumeRolePolicy":
         """
         Creates a AssumeRolePolicy resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Role.AssumeRolePolicy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#roleassumerolepolicy-method)
@@ -2529,14 +2548,15 @@
     name: str
     access_keys: UserAccessKeysCollection
     attached_policies: UserAttachedPoliciesCollection
     groups: UserGroupsCollection
     mfa_devices: UserMfaDevicesCollection
     policies: UserPoliciesCollection
     signing_certificates: UserSigningCertificatesCollection
+    meta: "IAMResourceMeta"
 
     def AccessKey(self, id: str) -> "_AccessKey":
         """
         Creates a AccessKey resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.User.AccessKey)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#useraccesskey-method)
```

### Comparing `mypy-boto3-iam-1.34.8/mypy_boto3_iam/type_defs.py` & `mypy-boto3-iam-1.34.83/mypy_boto3_iam/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     "AttachRolePolicyRequestPolicyAttachRoleTypeDef",
     "AttachRolePolicyRequestRequestTypeDef",
     "AttachRolePolicyRequestRoleAttachPolicyTypeDef",
     "AttachUserPolicyRequestPolicyAttachUserTypeDef",
     "AttachUserPolicyRequestRequestTypeDef",
     "AttachUserPolicyRequestUserAttachPolicyTypeDef",
     "ResponseMetadataTypeDef",
+    "AttachedPermissionsBoundaryTypeDef",
     "AttachedPolicyTypeDef",
     "ChangePasswordRequestRequestTypeDef",
     "ChangePasswordRequestServiceResourceChangePasswordTypeDef",
     "ContextEntryTypeDef",
     "CreateAccessKeyRequestRequestTypeDef",
     "CreateAccountAliasRequestRequestTypeDef",
     "CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef",
@@ -265,15 +266,14 @@
     "UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UpdateUserRequestUserUpdateTypeDef",
     "UploadSSHPublicKeyRequestRequestTypeDef",
     "UploadSigningCertificateRequestRequestTypeDef",
     "UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef",
     "AttachedPermissionsBoundaryResponseTypeDef",
-    "AttachedPermissionsBoundaryTypeDef",
     "CreateAccessKeyResponseTypeDef",
     "DeleteServiceLinkedRoleResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GenerateCredentialReportResponseTypeDef",
     "GenerateOrganizationsAccessReportResponseTypeDef",
     "GenerateServiceLastAccessedDetailsResponseTypeDef",
     "GetAccessKeyLastUsedResponseTypeDef",
@@ -330,14 +330,16 @@
     "TagPolicyRequestRequestTypeDef",
     "TagRoleRequestRequestTypeDef",
     "TagSAMLProviderRequestRequestTypeDef",
     "TagServerCertificateRequestRequestTypeDef",
     "TagUserRequestRequestTypeDef",
     "UploadServerCertificateRequestRequestTypeDef",
     "UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef",
+    "UserResponseTypeDef",
+    "UserTypeDef",
     "CreateLoginProfileResponseTypeDef",
     "GetLoginProfileResponseTypeDef",
     "CreateServiceSpecificCredentialResponseTypeDef",
     "ResetServiceSpecificCredentialResponseTypeDef",
     "DeletionTaskFailureReasonTypeTypeDef",
     "EntityDetailsTypeDef",
     "GetOrganizationsAccessReportResponseTypeDef",
@@ -393,40 +395,38 @@
     "UploadServerCertificateResponseTypeDef",
     "ListServiceSpecificCredentialsResponseTypeDef",
     "ListSigningCertificatesResponseTypeDef",
     "UploadSigningCertificateResponseTypeDef",
     "PolicyDocumentDictTypeDef",
     "StatementTypeDef",
     "ServiceLastAccessedTypeDef",
-    "UserResponseTypeDef",
-    "UserTypeDef",
     "CreatePolicyResponseTypeDef",
     "GetPolicyResponseTypeDef",
     "ListPoliciesResponseTypeDef",
+    "CreateUserResponseTypeDef",
+    "GetGroupResponseTypeDef",
+    "GetUserResponseTypeDef",
+    "ListUsersResponseTypeDef",
+    "VirtualMFADeviceTypeDef",
     "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
     "GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef",
     "ListPoliciesGrantingServiceAccessResponseTypeDef",
     "GetServerCertificateResponseTypeDef",
     "PolicyDocumentTypeDef",
     "ResourceSpecificResultTypeDef",
     "GetServiceLastAccessedDetailsResponseTypeDef",
-    "CreateUserResponseTypeDef",
-    "GetGroupResponseTypeDef",
-    "GetUserResponseTypeDef",
-    "ListUsersResponseTypeDef",
-    "VirtualMFADeviceTypeDef",
+    "CreateVirtualMFADeviceResponseTypeDef",
+    "ListVirtualMFADevicesResponseTypeDef",
     "GetGroupPolicyResponseTypeDef",
     "GetRolePolicyResponseTypeDef",
     "GetUserPolicyResponseTypeDef",
     "PolicyDetailTypeDef",
     "PolicyVersionTypeDef",
     "RoleTypeDef",
     "EvaluationResultTypeDef",
-    "CreateVirtualMFADeviceResponseTypeDef",
-    "ListVirtualMFADevicesResponseTypeDef",
     "GroupDetailTypeDef",
     "UserDetailTypeDef",
     "CreatePolicyVersionResponseTypeDef",
     "GetPolicyVersionResponseTypeDef",
     "ListPolicyVersionsResponseTypeDef",
     "ManagedPolicyDetailTypeDef",
     "CreateRoleResponseTypeDef",
@@ -578,18 +578,25 @@
         "PolicyArn": str,
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
+    },
+)
+AttachedPermissionsBoundaryTypeDef = TypedDict(
+    "AttachedPermissionsBoundaryTypeDef",
+    {
+        "PermissionsBoundaryType": NotRequired[Literal["PermissionsBoundaryPolicy"]],
+        "PermissionsBoundaryArn": NotRequired[str],
     },
 )
 AttachedPolicyTypeDef = TypedDict(
     "AttachedPolicyTypeDef",
     {
         "PolicyName": NotRequired[str],
         "PolicyArn": NotRequired[str],
@@ -2054,22 +2061,14 @@
     "AttachedPermissionsBoundaryResponseTypeDef",
     {
         "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
         "PermissionsBoundaryArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-AttachedPermissionsBoundaryTypeDef = TypedDict(
-    "AttachedPermissionsBoundaryTypeDef",
-    {
-        "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
-        "PermissionsBoundaryArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 CreateAccessKeyResponseTypeDef = TypedDict(
     "CreateAccessKeyResponseTypeDef",
     {
         "AccessKey": AccessKeyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2322,16 +2321,16 @@
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 CreateOpenIDConnectProviderRequestRequestTypeDef = TypedDict(
     "CreateOpenIDConnectProviderRequestRequestTypeDef",
     {
         "Url": str,
-        "ThumbprintList": Sequence[str],
         "ClientIDList": NotRequired[Sequence[str]],
+        "ThumbprintList": NotRequired[Sequence[str]],
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 CreateOpenIDConnectProviderResponseTypeDef = TypedDict(
     "CreateOpenIDConnectProviderResponseTypeDef",
     {
         "OpenIDConnectProviderArn": str,
@@ -2633,14 +2632,41 @@
         "CertificateBody": str,
         "PrivateKey": str,
         "Path": NotRequired[str],
         "CertificateChain": NotRequired[str],
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
+UserResponseTypeDef = TypedDict(
+    "UserResponseTypeDef",
+    {
+        "Path": str,
+        "UserName": str,
+        "UserId": str,
+        "Arn": str,
+        "CreateDate": datetime,
+        "PasswordLastUsed": datetime,
+        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UserTypeDef = TypedDict(
+    "UserTypeDef",
+    {
+        "Path": str,
+        "UserName": str,
+        "UserId": str,
+        "Arn": str,
+        "CreateDate": datetime,
+        "PasswordLastUsed": NotRequired[datetime],
+        "PermissionsBoundary": NotRequired[AttachedPermissionsBoundaryTypeDef],
+        "Tags": NotRequired[List[TagTypeDef]],
+    },
+)
 CreateLoginProfileResponseTypeDef = TypedDict(
     "CreateLoginProfileResponseTypeDef",
     {
         "LoginProfile": LoginProfileTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3129,41 +3155,14 @@
         "LastAuthenticated": NotRequired[datetime],
         "LastAuthenticatedEntity": NotRequired[str],
         "LastAuthenticatedRegion": NotRequired[str],
         "TotalAuthenticatedEntities": NotRequired[int],
         "TrackedActionsLastAccessed": NotRequired[List[TrackedActionLastAccessedTypeDef]],
     },
 )
-UserResponseTypeDef = TypedDict(
-    "UserResponseTypeDef",
-    {
-        "Path": str,
-        "UserName": str,
-        "UserId": str,
-        "Arn": str,
-        "CreateDate": datetime,
-        "PasswordLastUsed": datetime,
-        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UserTypeDef = TypedDict(
-    "UserTypeDef",
-    {
-        "Path": str,
-        "UserName": str,
-        "UserId": str,
-        "Arn": str,
-        "CreateDate": datetime,
-        "PasswordLastUsed": NotRequired[datetime],
-        "PermissionsBoundary": NotRequired[AttachedPermissionsBoundaryTypeDef],
-        "Tags": NotRequired[List[TagTypeDef]],
-    },
-)
 CreatePolicyResponseTypeDef = TypedDict(
     "CreatePolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3179,14 +3178,58 @@
     {
         "Policies": List[PolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
+    {
+        "User": UserTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetGroupResponseTypeDef = TypedDict(
+    "GetGroupResponseTypeDef",
+    {
+        "Group": GroupTypeDef,
+        "Users": List[UserTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetUserResponseTypeDef = TypedDict(
+    "GetUserResponseTypeDef",
+    {
+        "User": UserTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListUsersResponseTypeDef = TypedDict(
+    "ListUsersResponseTypeDef",
+    {
+        "Users": List[UserTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+VirtualMFADeviceTypeDef = TypedDict(
+    "VirtualMFADeviceTypeDef",
+    {
+        "SerialNumber": str,
+        "Base32StringSeed": NotRequired[bytes],
+        "QRCodePNG": NotRequired[bytes],
+        "User": NotRequired[UserTypeDef],
+        "EnableDate": NotRequired[datetime],
+        "Tags": NotRequired[List[TagTypeDef]],
+    },
+)
 GetServiceLinkedRoleDeletionStatusResponseTypeDef = TypedDict(
     "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
     {
         "Status": DeletionTaskStatusTypeType,
         "Reason": DeletionTaskFailureReasonTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3242,58 +3285,30 @@
         "JobCompletionDate": datetime,
         "IsTruncated": bool,
         "Marker": str,
         "Error": ErrorDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
-    {
-        "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-GetGroupResponseTypeDef = TypedDict(
-    "GetGroupResponseTypeDef",
-    {
-        "Group": GroupTypeDef,
-        "Users": List[UserTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-GetUserResponseTypeDef = TypedDict(
-    "GetUserResponseTypeDef",
+CreateVirtualMFADeviceResponseTypeDef = TypedDict(
+    "CreateVirtualMFADeviceResponseTypeDef",
     {
-        "User": UserTypeDef,
+        "VirtualMFADevice": VirtualMFADeviceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListUsersResponseTypeDef = TypedDict(
-    "ListUsersResponseTypeDef",
+ListVirtualMFADevicesResponseTypeDef = TypedDict(
+    "ListVirtualMFADevicesResponseTypeDef",
     {
-        "Users": List[UserTypeDef],
+        "VirtualMFADevices": List[VirtualMFADeviceTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-VirtualMFADeviceTypeDef = TypedDict(
-    "VirtualMFADeviceTypeDef",
-    {
-        "SerialNumber": str,
-        "Base32StringSeed": NotRequired[bytes],
-        "QRCodePNG": NotRequired[bytes],
-        "User": NotRequired[UserTypeDef],
-        "EnableDate": NotRequired[datetime],
-        "Tags": NotRequired[List[TagTypeDef]],
-    },
-)
 GetGroupPolicyResponseTypeDef = TypedDict(
     "GetGroupPolicyResponseTypeDef",
     {
         "GroupName": str,
         "PolicyName": str,
         "PolicyDocument": PolicyDocumentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3359,30 +3374,14 @@
         "MissingContextValues": NotRequired[List[str]],
         "OrganizationsDecisionDetail": NotRequired[OrganizationsDecisionDetailTypeDef],
         "PermissionsBoundaryDecisionDetail": NotRequired[PermissionsBoundaryDecisionDetailTypeDef],
         "EvalDecisionDetails": NotRequired[Dict[str, PolicyEvaluationDecisionTypeType]],
         "ResourceSpecificResults": NotRequired[List[ResourceSpecificResultTypeDef]],
     },
 )
-CreateVirtualMFADeviceResponseTypeDef = TypedDict(
-    "CreateVirtualMFADeviceResponseTypeDef",
-    {
-        "VirtualMFADevice": VirtualMFADeviceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-ListVirtualMFADevicesResponseTypeDef = TypedDict(
-    "ListVirtualMFADevicesResponseTypeDef",
-    {
-        "VirtualMFADevices": List[VirtualMFADeviceTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 GroupDetailTypeDef = TypedDict(
     "GroupDetailTypeDef",
     {
         "Path": NotRequired[str],
         "GroupName": NotRequired[str],
         "GroupId": NotRequired[str],
         "Arn": NotRequired[str],
```

### Comparing `mypy-boto3-iam-1.34.8/mypy_boto3_iam/type_defs.pyi` & `mypy-boto3-iam-1.34.83/mypy_boto3_iam/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     "AttachRolePolicyRequestPolicyAttachRoleTypeDef",
     "AttachRolePolicyRequestRequestTypeDef",
     "AttachRolePolicyRequestRoleAttachPolicyTypeDef",
     "AttachUserPolicyRequestPolicyAttachUserTypeDef",
     "AttachUserPolicyRequestRequestTypeDef",
     "AttachUserPolicyRequestUserAttachPolicyTypeDef",
     "ResponseMetadataTypeDef",
+    "AttachedPermissionsBoundaryTypeDef",
     "AttachedPolicyTypeDef",
     "ChangePasswordRequestRequestTypeDef",
     "ChangePasswordRequestServiceResourceChangePasswordTypeDef",
     "ContextEntryTypeDef",
     "CreateAccessKeyRequestRequestTypeDef",
     "CreateAccountAliasRequestRequestTypeDef",
     "CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef",
@@ -265,15 +266,14 @@
     "UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UpdateUserRequestUserUpdateTypeDef",
     "UploadSSHPublicKeyRequestRequestTypeDef",
     "UploadSigningCertificateRequestRequestTypeDef",
     "UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef",
     "AttachedPermissionsBoundaryResponseTypeDef",
-    "AttachedPermissionsBoundaryTypeDef",
     "CreateAccessKeyResponseTypeDef",
     "DeleteServiceLinkedRoleResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GenerateCredentialReportResponseTypeDef",
     "GenerateOrganizationsAccessReportResponseTypeDef",
     "GenerateServiceLastAccessedDetailsResponseTypeDef",
     "GetAccessKeyLastUsedResponseTypeDef",
@@ -330,14 +330,16 @@
     "TagPolicyRequestRequestTypeDef",
     "TagRoleRequestRequestTypeDef",
     "TagSAMLProviderRequestRequestTypeDef",
     "TagServerCertificateRequestRequestTypeDef",
     "TagUserRequestRequestTypeDef",
     "UploadServerCertificateRequestRequestTypeDef",
     "UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef",
+    "UserResponseTypeDef",
+    "UserTypeDef",
     "CreateLoginProfileResponseTypeDef",
     "GetLoginProfileResponseTypeDef",
     "CreateServiceSpecificCredentialResponseTypeDef",
     "ResetServiceSpecificCredentialResponseTypeDef",
     "DeletionTaskFailureReasonTypeTypeDef",
     "EntityDetailsTypeDef",
     "GetOrganizationsAccessReportResponseTypeDef",
@@ -393,40 +395,38 @@
     "UploadServerCertificateResponseTypeDef",
     "ListServiceSpecificCredentialsResponseTypeDef",
     "ListSigningCertificatesResponseTypeDef",
     "UploadSigningCertificateResponseTypeDef",
     "PolicyDocumentDictTypeDef",
     "StatementTypeDef",
     "ServiceLastAccessedTypeDef",
-    "UserResponseTypeDef",
-    "UserTypeDef",
     "CreatePolicyResponseTypeDef",
     "GetPolicyResponseTypeDef",
     "ListPoliciesResponseTypeDef",
+    "CreateUserResponseTypeDef",
+    "GetGroupResponseTypeDef",
+    "GetUserResponseTypeDef",
+    "ListUsersResponseTypeDef",
+    "VirtualMFADeviceTypeDef",
     "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
     "GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef",
     "ListPoliciesGrantingServiceAccessResponseTypeDef",
     "GetServerCertificateResponseTypeDef",
     "PolicyDocumentTypeDef",
     "ResourceSpecificResultTypeDef",
     "GetServiceLastAccessedDetailsResponseTypeDef",
-    "CreateUserResponseTypeDef",
-    "GetGroupResponseTypeDef",
-    "GetUserResponseTypeDef",
-    "ListUsersResponseTypeDef",
-    "VirtualMFADeviceTypeDef",
+    "CreateVirtualMFADeviceResponseTypeDef",
+    "ListVirtualMFADevicesResponseTypeDef",
     "GetGroupPolicyResponseTypeDef",
     "GetRolePolicyResponseTypeDef",
     "GetUserPolicyResponseTypeDef",
     "PolicyDetailTypeDef",
     "PolicyVersionTypeDef",
     "RoleTypeDef",
     "EvaluationResultTypeDef",
-    "CreateVirtualMFADeviceResponseTypeDef",
-    "ListVirtualMFADevicesResponseTypeDef",
     "GroupDetailTypeDef",
     "UserDetailTypeDef",
     "CreatePolicyVersionResponseTypeDef",
     "GetPolicyVersionResponseTypeDef",
     "ListPolicyVersionsResponseTypeDef",
     "ManagedPolicyDetailTypeDef",
     "CreateRoleResponseTypeDef",
@@ -578,18 +578,25 @@
         "PolicyArn": str,
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
+    },
+)
+AttachedPermissionsBoundaryTypeDef = TypedDict(
+    "AttachedPermissionsBoundaryTypeDef",
+    {
+        "PermissionsBoundaryType": NotRequired[Literal["PermissionsBoundaryPolicy"]],
+        "PermissionsBoundaryArn": NotRequired[str],
     },
 )
 AttachedPolicyTypeDef = TypedDict(
     "AttachedPolicyTypeDef",
     {
         "PolicyName": NotRequired[str],
         "PolicyArn": NotRequired[str],
@@ -2054,22 +2061,14 @@
     "AttachedPermissionsBoundaryResponseTypeDef",
     {
         "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
         "PermissionsBoundaryArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-AttachedPermissionsBoundaryTypeDef = TypedDict(
-    "AttachedPermissionsBoundaryTypeDef",
-    {
-        "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
-        "PermissionsBoundaryArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 CreateAccessKeyResponseTypeDef = TypedDict(
     "CreateAccessKeyResponseTypeDef",
     {
         "AccessKey": AccessKeyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2322,16 +2321,16 @@
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 CreateOpenIDConnectProviderRequestRequestTypeDef = TypedDict(
     "CreateOpenIDConnectProviderRequestRequestTypeDef",
     {
         "Url": str,
-        "ThumbprintList": Sequence[str],
         "ClientIDList": NotRequired[Sequence[str]],
+        "ThumbprintList": NotRequired[Sequence[str]],
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 CreateOpenIDConnectProviderResponseTypeDef = TypedDict(
     "CreateOpenIDConnectProviderResponseTypeDef",
     {
         "OpenIDConnectProviderArn": str,
@@ -2633,14 +2632,41 @@
         "CertificateBody": str,
         "PrivateKey": str,
         "Path": NotRequired[str],
         "CertificateChain": NotRequired[str],
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
+UserResponseTypeDef = TypedDict(
+    "UserResponseTypeDef",
+    {
+        "Path": str,
+        "UserName": str,
+        "UserId": str,
+        "Arn": str,
+        "CreateDate": datetime,
+        "PasswordLastUsed": datetime,
+        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UserTypeDef = TypedDict(
+    "UserTypeDef",
+    {
+        "Path": str,
+        "UserName": str,
+        "UserId": str,
+        "Arn": str,
+        "CreateDate": datetime,
+        "PasswordLastUsed": NotRequired[datetime],
+        "PermissionsBoundary": NotRequired[AttachedPermissionsBoundaryTypeDef],
+        "Tags": NotRequired[List[TagTypeDef]],
+    },
+)
 CreateLoginProfileResponseTypeDef = TypedDict(
     "CreateLoginProfileResponseTypeDef",
     {
         "LoginProfile": LoginProfileTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3129,41 +3155,14 @@
         "LastAuthenticated": NotRequired[datetime],
         "LastAuthenticatedEntity": NotRequired[str],
         "LastAuthenticatedRegion": NotRequired[str],
         "TotalAuthenticatedEntities": NotRequired[int],
         "TrackedActionsLastAccessed": NotRequired[List[TrackedActionLastAccessedTypeDef]],
     },
 )
-UserResponseTypeDef = TypedDict(
-    "UserResponseTypeDef",
-    {
-        "Path": str,
-        "UserName": str,
-        "UserId": str,
-        "Arn": str,
-        "CreateDate": datetime,
-        "PasswordLastUsed": datetime,
-        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UserTypeDef = TypedDict(
-    "UserTypeDef",
-    {
-        "Path": str,
-        "UserName": str,
-        "UserId": str,
-        "Arn": str,
-        "CreateDate": datetime,
-        "PasswordLastUsed": NotRequired[datetime],
-        "PermissionsBoundary": NotRequired[AttachedPermissionsBoundaryTypeDef],
-        "Tags": NotRequired[List[TagTypeDef]],
-    },
-)
 CreatePolicyResponseTypeDef = TypedDict(
     "CreatePolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3179,14 +3178,58 @@
     {
         "Policies": List[PolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
+    {
+        "User": UserTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetGroupResponseTypeDef = TypedDict(
+    "GetGroupResponseTypeDef",
+    {
+        "Group": GroupTypeDef,
+        "Users": List[UserTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetUserResponseTypeDef = TypedDict(
+    "GetUserResponseTypeDef",
+    {
+        "User": UserTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListUsersResponseTypeDef = TypedDict(
+    "ListUsersResponseTypeDef",
+    {
+        "Users": List[UserTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+VirtualMFADeviceTypeDef = TypedDict(
+    "VirtualMFADeviceTypeDef",
+    {
+        "SerialNumber": str,
+        "Base32StringSeed": NotRequired[bytes],
+        "QRCodePNG": NotRequired[bytes],
+        "User": NotRequired[UserTypeDef],
+        "EnableDate": NotRequired[datetime],
+        "Tags": NotRequired[List[TagTypeDef]],
+    },
+)
 GetServiceLinkedRoleDeletionStatusResponseTypeDef = TypedDict(
     "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
     {
         "Status": DeletionTaskStatusTypeType,
         "Reason": DeletionTaskFailureReasonTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3242,58 +3285,30 @@
         "JobCompletionDate": datetime,
         "IsTruncated": bool,
         "Marker": str,
         "Error": ErrorDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
-    {
-        "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-GetGroupResponseTypeDef = TypedDict(
-    "GetGroupResponseTypeDef",
-    {
-        "Group": GroupTypeDef,
-        "Users": List[UserTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-GetUserResponseTypeDef = TypedDict(
-    "GetUserResponseTypeDef",
+CreateVirtualMFADeviceResponseTypeDef = TypedDict(
+    "CreateVirtualMFADeviceResponseTypeDef",
     {
-        "User": UserTypeDef,
+        "VirtualMFADevice": VirtualMFADeviceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListUsersResponseTypeDef = TypedDict(
-    "ListUsersResponseTypeDef",
+ListVirtualMFADevicesResponseTypeDef = TypedDict(
+    "ListVirtualMFADevicesResponseTypeDef",
     {
-        "Users": List[UserTypeDef],
+        "VirtualMFADevices": List[VirtualMFADeviceTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-VirtualMFADeviceTypeDef = TypedDict(
-    "VirtualMFADeviceTypeDef",
-    {
-        "SerialNumber": str,
-        "Base32StringSeed": NotRequired[bytes],
-        "QRCodePNG": NotRequired[bytes],
-        "User": NotRequired[UserTypeDef],
-        "EnableDate": NotRequired[datetime],
-        "Tags": NotRequired[List[TagTypeDef]],
-    },
-)
 GetGroupPolicyResponseTypeDef = TypedDict(
     "GetGroupPolicyResponseTypeDef",
     {
         "GroupName": str,
         "PolicyName": str,
         "PolicyDocument": PolicyDocumentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3359,30 +3374,14 @@
         "MissingContextValues": NotRequired[List[str]],
         "OrganizationsDecisionDetail": NotRequired[OrganizationsDecisionDetailTypeDef],
         "PermissionsBoundaryDecisionDetail": NotRequired[PermissionsBoundaryDecisionDetailTypeDef],
         "EvalDecisionDetails": NotRequired[Dict[str, PolicyEvaluationDecisionTypeType]],
         "ResourceSpecificResults": NotRequired[List[ResourceSpecificResultTypeDef]],
     },
 )
-CreateVirtualMFADeviceResponseTypeDef = TypedDict(
-    "CreateVirtualMFADeviceResponseTypeDef",
-    {
-        "VirtualMFADevice": VirtualMFADeviceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-ListVirtualMFADevicesResponseTypeDef = TypedDict(
-    "ListVirtualMFADevicesResponseTypeDef",
-    {
-        "VirtualMFADevices": List[VirtualMFADeviceTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 GroupDetailTypeDef = TypedDict(
     "GroupDetailTypeDef",
     {
         "Path": NotRequired[str],
         "GroupName": NotRequired[str],
         "GroupId": NotRequired[str],
         "Arn": NotRequired[str],
```

### Comparing `mypy-boto3-iam-1.34.8/mypy_boto3_iam/waiter.py` & `mypy-boto3-iam-1.34.83/mypy_boto3_iam/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.34.8/mypy_boto3_iam/waiter.pyi` & `mypy-boto3-iam-1.34.83/mypy_boto3_iam/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.34.8/mypy_boto3_iam.egg-info/PKG-INFO` & `mypy-boto3-iam-1.34.83/mypy_boto3_iam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iam
-Version: 1.34.8
-Summary: Type annotations for boto3.IAM 1.34.8 service generated with mypy-boto3-builder 7.23.0
+Version: 1.34.83
+Summary: Type annotations for boto3.IAM 1.34.83 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/
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
 
 <a id="mypy-boto3-iam"></a>
 
 # mypy-boto3-iam
 
 [![PyPI - mypy-boto3-iam](https://img.shields.io/pypi/v/mypy-boto3-iam.svg?color=blue)](https://pypi.org/project/mypy-boto3-iam)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iam.svg?color=blue)](https://pypi.org/project/mypy-boto3-iam)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iam)](https://pepy.tech/project/mypy-boto3-iam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAM 1.34.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
+[boto3.IAM 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
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
 [mypy-boto3-iam docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iam-1.34.8/mypy_boto3_iam.egg-info/SOURCES.txt` & `mypy-boto3-iam-1.34.83/mypy_boto3_iam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.34.8/setup.py` & `mypy-boto3-iam-1.34.83/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,23 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iam",
-    version="1.34.8",
+    version="1.34.83",
     packages=["mypy_boto3_iam"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.IAM 1.34.8 service generated with mypy-boto3-builder 7.23.0"
-    ),
+    description="Type annotations for boto3.IAM 1.34.83 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

