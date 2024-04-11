# Comparing `tmp/fidelius-0.6.0.tar.gz` & `tmp/fidelius-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fidelius-0.6.0.tar", last modified: Fri Apr  5 16:56:16 2024, max compression
+gzip compressed data, was "fidelius-1.0.0b1.tar", last modified: Thu Apr 11 15:52:23 2024, max compression
```

## Comparing `fidelius-0.6.0.tar` & `fidelius-1.0.0b1.tar`

### file list

```diff
@@ -1,28 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:56:16.104496 fidelius-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 16:56:05.000000 fidelius-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-04-05 16:56:16.104496 fidelius-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14208 2024-04-05 16:56:05.000000 fidelius-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:56:16.104496 fidelius-0.6.0/fidelius/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:56:16.104496 fidelius-0.6.0/fidelius/fideliusapi/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/fideliusapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:56:16.104496 fidelius-0.6.0/fidelius/gateway/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/gateway/paramadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/gateway/paramstore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:56:16.104496 fidelius-0.6.0/fidelius/structs/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/structs/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/structs/_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:56:16.104496 fidelius-0.6.0/fidelius/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-05 16:56:05.000000 fidelius-0.6.0/fidelius/utils/replacer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:56:16.104496 fidelius-0.6.0/fidelius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-04-05 16:56:16.000000 fidelius-0.6.0/fidelius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-05 16:56:16.000000 fidelius-0.6.0/fidelius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:56:16.000000 fidelius-0.6.0/fidelius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-05 16:56:16.000000 fidelius-0.6.0/fidelius.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 16:56:16.000000 fidelius-0.6.0/fidelius.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-05 16:56:05.000000 fidelius-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:56:16.104496 fidelius-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-05 16:56:05.000000 fidelius-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:52:23.417746 fidelius-1.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17001 2024-04-11 15:52:23.417746 fidelius-1.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14314 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:52:23.413746 fidelius-1.0.0b1/fidelius/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:52:23.413746 fidelius-1.0.0b1/fidelius/fideliusapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/fideliusapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:52:23.413746 fidelius-1.0.0b1/fidelius/gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16395 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:52:23.413746 fidelius-1.0.0b1/fidelius/gateway/mock/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/mock/_inmemcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/mock/_mockadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/mock/_mockrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/mock/_std.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:52:23.413746 fidelius-1.0.0b1/fidelius/gateway/paramstore/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/paramstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/paramstore/_paramstoreadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/paramstore/_paramstorerepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/paramstore/_std.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:52:23.417746 fidelius-1.0.0b1/fidelius/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/structs/_appprops.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/structs/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/structs/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/structs/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/structs/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:52:23.417746 fidelius-1.0.0b1/fidelius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17001 2024-04-11 15:52:23.000000 fidelius-1.0.0b1/fidelius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-11 15:52:23.000000 fidelius-1.0.0b1/fidelius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:52:23.000000 fidelius-1.0.0b1/fidelius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 15:52:23.000000 fidelius-1.0.0b1/fidelius.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 15:52:23.000000 fidelius-1.0.0b1/fidelius.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:52:23.417746 fidelius-1.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/setup.py
```

### Comparing `fidelius-0.6.0/LICENSE` & `fidelius-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fidelius-0.6.0/PKG-INFO` & `fidelius-1.0.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fidelius
-Version: 0.6.0
+Version: 1.0.0b1
 Summary: The Fidelius Charm! (keeping things secret)
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>, Kristin Fjola Tomasdottir <kristinf@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2022-2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,28 +43,32 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ccptools<2,>=1.1
 Requires-Dist: boto3<2,>=1.20
 
 # The Fidelius Charm - Keeping Things Secret
 
 Fidelius is a package for fetching (and managing) secrets and other 
 parameters from AWS' Parameter Store.
 
 This is designed with CCP Borg Application Framework and the Alviss config 
 package in mind but should work for other cases as well.
 
 **IMPORTANT:** This has been migrated more-or-less _"as-is"_ from CCP Tool's 
 internal repo and hasn't yet been given the love it needs to be properly 
 open-sourced and user friendly for other people _(unless you read though the 
-code and find it perfectly fits your use case)_. 
+code and find it perfectly fits your use case)_.
+
+**ALSO IMPORTANT:** This README hasn't been updated to reflect changes in 
+version 1.0.0 yet. Sowwie! :-/
 
 ## What should be stored with Fidelius
 
 All secrets, always, as Secret Parameters (they are stored as encrypted)!
 
 This includes (but is not limited to):
```

### Comparing `fidelius-0.6.0/README.md` & `fidelius-1.0.0b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 
 This is designed with CCP Borg Application Framework and the Alviss config 
 package in mind but should work for other cases as well.
 
 **IMPORTANT:** This has been migrated more-or-less _"as-is"_ from CCP Tool's 
 internal repo and hasn't yet been given the love it needs to be properly 
 open-sourced and user friendly for other people _(unless you read though the 
-code and find it perfectly fits your use case)_. 
+code and find it perfectly fits your use case)_.
+
+**ALSO IMPORTANT:** This README hasn't been updated to reflect changes in 
+version 1.0.0 yet. Sowwie! :-/
 
 ## What should be stored with Fidelius
 
 All secrets, always, as Secret Parameters (they are stored as encrypted)!
 
 This includes (but is not limited to):
```

### Comparing `fidelius-0.6.0/fidelius/gateway/paramadmin.py` & `fidelius-1.0.0b1/fidelius/gateway/paramstore/_paramstoreadmin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,161 @@
 __all__ = [
-    'ParameterStoreAdmin',
+    'AwsParameterStoreAdmin',
 ]
-from .paramstore import *
+
 from fidelius.structs import *
+from fidelius.gateway._abstract import *
+from ._paramstorerepo import *
 
 import logging
 log = logging.getLogger(__name__)
 
 
-class ParameterStoreAdmin(ParameterStore):
-    def __init__(self, app: str, group: str, env: str, owner: str, finance: str = 'COST', **extra_tags):
-        super().__init__(app, group, env)
-        self._tags = Tags(application=self._app, owner=owner, tier=env, finance=finance, **extra_tags)
-
-    def set_env(self, env: str):
-        self._env = env
-        self._tags.tier = env
+class AwsParameterStoreAdmin(_BaseFideliusAdminRepo, AwsParamStoreRepo):
+    def __init__(self, app_props: FideliusAppProps, tags: Optional[FideliusTags] = None, **kwargs):
+        log.debug('AwsParameterStoreAdmin.__init__')
+        super().__init__(app_props, tags, **kwargs)
+
+    def create_param(self, name: str, value: str,
+                     description: Optional[str] = None, env: Optional[str] = None) -> (str, str):
+        path = self.get_full_path(name, env=env)
+        res = self._set_parameter(full_name=path,
+                                  value=value,
+                                  description=description,
+                                  overwrite=False,
+                                  encrypted=False)
+        return path, self.get_expression_string(name)
+
+    def update_param(self, name: str, value: str,
+                     description: Optional[str] = None, env: Optional[str] = None) -> (str, str):
+        path = self.get_full_path(name, env=env)
+        if self.get_app_param(name, env=env) is None:
+            raise FideliusParameterNotFound(f'parameter not found: {path}')
 
-    def _set_parameter(self,
-                       full_name: str,
-                       value: str,
-                       encrypted: bool = False,
-                       overwrite: bool = False,
-                       description: Optional[str] = None) -> Dict:
-        kwargs = dict(Name=full_name,
-                      Description=description or full_name,
-                      Value=value,
-                      Type='SecureString' if encrypted else 'String',
-                      Overwrite=overwrite,
-                      Tags=self._tags.to_aws_format(),
-                      Tier='Standard')
-        if encrypted:
-            kwargs['KeyId'] = self._KEY_ID
-
-        response = self._ssm.put_parameter(**kwargs)
-        return response
-
-    def create_param(self, name: str, value: str, description: Optional[str] = None):
-        self._set_parameter(full_name=self._full_path(name),
+        self._set_parameter(full_name=path,
                             value=value,
                             description=description,
-                            overwrite=False,
+                            overwrite=True,
                             encrypted=False)
+        return path, self.get_expression_string(name)
 
-    def update_param(self, name: str, value: str, description: Optional[str] = None):
-        if self.get(name=name, no_default=True):
-            self._set_parameter(full_name=self._full_path(name),
-                                value=value,
-                                description=description,
-                                overwrite=True,
-                                encrypted=False)
-        else:
-            raise ValueError('that parameter does not exists yet, use create_param')
+    def delete_param(self, name: str, env: Optional[str] = None):
+        self._delete_parameter(full_name=self.get_full_path(name, env=env))
 
-    def create_shared_param(self, name: str, folder: str, value: str, description: Optional[str] = None):
-        self._set_parameter(full_name=self._full_path(name, folder),
+    def create_shared_param(self, name: str, folder: str, value: str,
+                            description: Optional[str] = None, env: Optional[str] = None) -> (str, str):
+        path = self.get_full_path(name, folder=folder, env=env)
+        self._set_parameter(full_name=path,
                             value=value,
                             description=description,
                             overwrite=False,
                             encrypted=False)
+        return path, self.get_expression_string(name, folder=folder)
 
-    def update_shared_param(self, name: str, folder: str, value: str, description: Optional[str] = None):
-        self._set_parameter(full_name=self._full_path(name, folder),
+    def update_shared_param(self, name: str, folder: str, value: str,
+                            description: Optional[str] = None, env: Optional[str] = None) -> (str, str):
+        path = self.get_full_path(name, folder=folder, env=env)
+        if self.get_shared_param(name, folder=folder, env=env) is None:
+            raise FideliusParameterNotFound(f'parameter not found: {path}')
+
+        self._set_parameter(full_name=path,
                             value=value,
                             description=description,
                             overwrite=True,
                             encrypted=False)
+        return path, self.get_expression_string(name, folder=folder)
+
+    def delete_shared_param(self, name: str, folder: str, env: Optional[str] = None):
+        self._delete_parameter(full_name=self.get_full_path(name, folder=folder, env=env))
 
-    def create_secret(self, name: str, value: str, description: Optional[str] = None):
-        self._set_parameter(full_name=self._full_path(name),
+    def create_secret(self, name: str, value: str,
+                      description: Optional[str] = None, env: Optional[str] = None) -> (str, str):
+        path = self.get_full_path(name, env=env)
+        self._set_parameter(full_name=path,
                             value=value,
                             description=description,
                             overwrite=False,
                             encrypted=True)
+        return path, self.get_expression_string(name)
 
-    def update_secret(self, name: str, value: str, description: Optional[str] = None):
-        if self.get(name=name, no_default=True):
-            self._set_parameter(full_name=self._full_path(name),
-                                value=value,
-                                description=description,
-                                overwrite=True,
-                                encrypted=True)
-        else:
-            raise ValueError('that secret does not exists yet, use create_secret')
+    def update_secret(self, name: str, value: str,
+                      description: Optional[str] = None, env: Optional[str] = None) -> (str, str):
+        path = self.get_full_path(name, env=env)
+        if self.get_app_param(name, env=env) is None:
+            raise FideliusParameterNotFound(f'parameter not found: {path}')
 
-    def create_shared_secret(self, name: str, folder: str, value: str, description: Optional[str] = None):
-        self._set_parameter(full_name=self._full_path(name, folder),
+        self._set_parameter(full_name=path,
+                            value=value,
+                            description=description,
+                            overwrite=True,
+                            encrypted=True)
+        return path, self.get_expression_string(name)
+
+    def delete_secret(self, name: str, env: Optional[str] = None):
+        self._delete_parameter(full_name=self.get_full_path(name, env=env))
+
+    def create_shared_secret(self, name: str, folder: str, value: str,
+                             description: Optional[str] = None, env: Optional[str] = None) -> (str, str):
+        path = self.get_full_path(name, folder=folder, env=env)
+        self._set_parameter(full_name=path,
                             value=value,
                             description=description,
                             overwrite=False,
                             encrypted=True)
+        return path, self.get_expression_string(name, folder=folder)
 
-    def update_shared_secret(self, name: str, folder: str, value: str, description: Optional[str] = None):
-        self._set_parameter(full_name=self._full_path(name, folder),
+    def update_shared_secret(self, name: str, folder: str, value: str,
+                             description: Optional[str] = None, env: Optional[str] = None) -> (str, str):
+        path = self.get_full_path(name, folder=folder, env=env)
+        if self.get_shared_param(name, folder=folder, env=env) is None:
+            raise FideliusParameterNotFound(f'parameter not found: {path}')
+
+        self._set_parameter(full_name=path,
                             value=value,
                             description=description,
                             overwrite=True,
                             encrypted=True)
+        return path, self.get_expression_string(name, folder=folder)
+
+    def delete_shared_secret(self, name: str, folder: str, env: Optional[str] = None):
+        self._delete_parameter(full_name=self.get_full_path(name, folder=folder, env=env))
+
+    def _tags_to_aws_format(self) -> Optional[List[Dict[str, str]]]:
+        if self.tags:
+            return [{'Key': k, 'Value': v} for k, v in self.tags.to_dict().items()]
+        return None
+
+    def _set_parameter(self,
+                       full_name: str,
+                       value: str,
+                       encrypted: bool = False,
+                       overwrite: bool = False,
+                       description: Optional[str] = None) -> Dict:
+        kwargs = dict(Name=full_name,
+                      Description=description or full_name,
+                      Value=value,
+                      Type='SecureString' if encrypted else 'String',
+                      Overwrite=overwrite,
+                      Tier='Standard')
+        if not overwrite:
+            tags = self._tags_to_aws_format()
+            if tags:
+                kwargs['Tags'] = tags
+
+        if encrypted:
+            kwargs['KeyId'] = self._aws_key_arn
+
+        try:
+            response = self._ssm.put_parameter(**kwargs)
+            return response
+        except self._ssm.exceptions.ParameterAlreadyExists:
+            raise FideliusParameterAlreadyExists(f'parameter already exists: {full_name}')
+
+        except self._ssm.exceptions.ParameterNotFound:
+            raise FideliusParameterNotFound(f'parameter not found: {full_name}')
+
+    def _delete_parameter(self, full_name: str) -> Dict:
+        try:
+            response = self._ssm.delete_parameter(Name=full_name)
+            return response
+        except self._ssm.exceptions.ParameterNotFound:
+            raise FideliusParameterNotFound(f'parameter not found: {full_name}')
```

### Comparing `fidelius-0.6.0/fidelius.egg-info/PKG-INFO` & `fidelius-1.0.0b1/fidelius.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fidelius
-Version: 0.6.0
+Version: 1.0.0b1
 Summary: The Fidelius Charm! (keeping things secret)
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>, Kristin Fjola Tomasdottir <kristinf@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2022-2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,28 +43,32 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ccptools<2,>=1.1
 Requires-Dist: boto3<2,>=1.20
 
 # The Fidelius Charm - Keeping Things Secret
 
 Fidelius is a package for fetching (and managing) secrets and other 
 parameters from AWS' Parameter Store.
 
 This is designed with CCP Borg Application Framework and the Alviss config 
 package in mind but should work for other cases as well.
 
 **IMPORTANT:** This has been migrated more-or-less _"as-is"_ from CCP Tool's 
 internal repo and hasn't yet been given the love it needs to be properly 
 open-sourced and user friendly for other people _(unless you read though the 
-code and find it perfectly fits your use case)_. 
+code and find it perfectly fits your use case)_.
+
+**ALSO IMPORTANT:** This README hasn't been updated to reflect changes in 
+version 1.0.0 yet. Sowwie! :-/
 
 ## What should be stored with Fidelius
 
 All secrets, always, as Secret Parameters (they are stored as encrypted)!
 
 This includes (but is not limited to):
```

### Comparing `fidelius-0.6.0/pyproject.toml` & `fidelius-1.0.0b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities"
 ]
 dependencies = [
-  "boto3 >=1.20, <2"
+    "ccptools >=1.1, <2",
+    "boto3 >=1.20, <2"
 ]
 
 [project.urls]
 Homepage = "https://github.com/ccpgames/fidelius"
 Documentation = "https://github.com/ccpgames/fidelius/blob/main/README.md"
 Repository = "https://github.com/ccpgames/fidelius.git"
 Issues = "https://github.com/ccpgames/fidelius/issues"
```

