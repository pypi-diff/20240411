# Comparing `tmp/pulumi_gitea-0.0.2.tar.gz` & `tmp/pulumi_gitea-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_gitea-0.0.2.tar", last modified: Wed Mar 20 20:20:24 2024, max compression
+gzip compressed data, was "pulumi_gitea-0.0.3.tar", last modified: Wed Apr 10 23:30:34 2024, max compression
```

## Comparing `pulumi_gitea-0.0.2.tar` & `pulumi_gitea-0.0.3.tar`

### file list

```diff
@@ -1,42 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:20:24.101648 pulumi_gitea-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-20 20:20:24.101648 pulumi_gitea-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:20:24.097648 pulumi_gitea-0.0.2/pulumi_gitea/
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/access_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:20:24.097648 pulumi_gitea-0.0.2/pulumi_gitea/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    10591 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/fork.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/get_org.py
--rw-r--r--   0 runner    (1001) docker     (127)    11048 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/get_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/get_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:20:24.097648 pulumi_gitea-0.0.2/pulumi_gitea/git/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/git/hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:20:24.101648 pulumi_gitea-0.0.2/pulumi_gitea/oauth2/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/oauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/oauth2/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    18905 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/org.py
--rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:20:24.101648 pulumi_gitea-0.0.2/pulumi_gitea/publickey/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/publickey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14101 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/publickey/deployment_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:20:24.101648 pulumi_gitea-0.0.2/pulumi_gitea/repositories/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11134 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/repositories/deployment_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    81731 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    26018 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    39380 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/pulumi_gitea/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:20:24.097648 pulumi_gitea-0.0.2/pulumi_gitea.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-20 20:20:24.000000 pulumi_gitea-0.0.2/pulumi_gitea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-20 20:20:24.000000 pulumi_gitea-0.0.2/pulumi_gitea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 20:20:24.000000 pulumi_gitea-0.0.2/pulumi_gitea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 20:20:24.000000 pulumi_gitea-0.0.2/pulumi_gitea.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-20 20:20:24.000000 pulumi_gitea-0.0.2/pulumi_gitea.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-20 20:20:24.000000 pulumi_gitea-0.0.2/pulumi_gitea.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 20:20:24.101648 pulumi_gitea-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-20 20:20:23.000000 pulumi_gitea-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:30:34.874997 pulumi_gitea-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-10 23:30:34.874997 pulumi_gitea-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:30:34.870997 pulumi_gitea-0.0.3/pulumi_gitea/
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/access_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:30:34.874997 pulumi_gitea-0.0.3/pulumi_gitea/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10591 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/fork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/get_org.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11048 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/get_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/git_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/oauth2_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18905 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/org.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13958 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/public_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    81731 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/repository_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26018 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39380 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:30:34.874997 pulumi_gitea-0.0.3/pulumi_gitea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/pulumi_gitea.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 23:30:34.874997 pulumi_gitea-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-10 23:30:34.000000 pulumi_gitea-0.0.3/setup.py
```

### Comparing `pulumi_gitea-0.0.2/PKG-INFO` & `pulumi_gitea-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_gitea
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Pulumi package for creating and managing Gitea resources
 Home-page: https://github.com/MaienM/pulumi-gitea
 License: Apache-2.0
 Project-URL: Repository, https://github.com/MaienM/pulumi-gitea
 Keywords: pulumi gitea category/infrastructure
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_gitea-0.0.2/README.md` & `pulumi_gitea-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_gitea-0.0.2/pulumi_gitea/_utilities.py` & `pulumi_gitea-0.0.3/pulumi_gitea/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitea-0.0.2/pulumi_gitea/access_token.py` & `pulumi_gitea-0.0.3/pulumi_gitea/access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitea-0.0.2/pulumi_gitea/config/vars.py` & `pulumi_gitea-0.0.3/pulumi_gitea/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitea-0.0.2/pulumi_gitea/fork.py` & `pulumi_gitea-0.0.3/pulumi_gitea/fork.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitea-0.0.2/pulumi_gitea/get_org.py` & `pulumi_gitea-0.0.3/pulumi_gitea/get_org.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitea-0.0.2/pulumi_gitea/get_repo.py` & `pulumi_gitea-0.0.3/pulumi_gitea/get_repo.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitea-0.0.2/pulumi_gitea/get_user.py` & `pulumi_gitea-0.0.3/pulumi_gitea/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitea-0.0.2/pulumi_gitea/git/hook.py` & `pulumi_gitea-0.0.3/pulumi_gitea/git_hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 
-__all__ = ['HookArgs', 'Hook']
+__all__ = ['GitHookArgs', 'GitHook']
 
 @pulumi.input_type
-class HookArgs:
+class GitHookArgs:
     def __init__(__self__, *,
                  content: pulumi.Input[str],
                  repo: pulumi.Input[str],
                  user: pulumi.Input[str],
                  name: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a Hook resource.
+        The set of arguments for constructing a GitHook resource.
         :param pulumi.Input[str] content: Content of the git hook
         :param pulumi.Input[str] repo: The repository that this hook belongs too.
         :param pulumi.Input[str] user: The user (or organisation) owning the repo this hook belongs too
         :param pulumi.Input[str] name: Name of the git hook to configure
         """
         pulumi.set(__self__, "content", content)
         pulumi.set(__self__, "repo", repo)
@@ -77,22 +77,22 @@
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
-class _HookState:
+class _GitHookState:
     def __init__(__self__, *,
                  content: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  repo: Optional[pulumi.Input[str]] = None,
                  user: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering Hook resources.
+        Input properties used for looking up and filtering GitHook resources.
         :param pulumi.Input[str] content: Content of the git hook
         :param pulumi.Input[str] name: Name of the git hook to configure
         :param pulumi.Input[str] repo: The repository that this hook belongs too.
         :param pulumi.Input[str] user: The user (or organisation) owning the repo this hook belongs too
         """
         if content is not None:
             pulumi.set(__self__, "content", content)
@@ -148,41 +148,41 @@
         return pulumi.get(self, "user")
 
     @user.setter
     def user(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user", value)
 
 
-class Hook(pulumi.CustomResource):
+class GitHook(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  content: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  repo: Optional[pulumi.Input[str]] = None,
                  user: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        `Git.Hook` manages git hooks on a repository.
+        `GitHook` manages git hooks on a repository.
         import is currently not supported
 
         WARNING: using this resource requires to enable server side hookswhich are known to cause [security issues](https://github.com/go-gitea/gitea/pull/13058)!
 
         if you want to procede, you need to enable server side hooks as stated [here](https://docs.gitea.io/en-us/config-cheat-sheet/#security-security)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitea as gitea
 
         test_org = gitea.Org("testOrg")
         org_repo = gitea.Repository("orgRepo", username=test_org.name)
-        org_repo_post_receive = gitea.git.Hook("orgRepoPostReceive",
+        org_repo_post_receive = gitea.GitHook("orgRepoPostReceive",
             user=test_org.name,
             repo=org_repo.name,
             content=(lambda path: open(path).read())(f"{path['module']}/post-receive.sh"))
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -191,45 +191,45 @@
         :param pulumi.Input[str] repo: The repository that this hook belongs too.
         :param pulumi.Input[str] user: The user (or organisation) owning the repo this hook belongs too
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: HookArgs,
+                 args: GitHookArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        `Git.Hook` manages git hooks on a repository.
+        `GitHook` manages git hooks on a repository.
         import is currently not supported
 
         WARNING: using this resource requires to enable server side hookswhich are known to cause [security issues](https://github.com/go-gitea/gitea/pull/13058)!
 
         if you want to procede, you need to enable server side hooks as stated [here](https://docs.gitea.io/en-us/config-cheat-sheet/#security-security)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitea as gitea
 
         test_org = gitea.Org("testOrg")
         org_repo = gitea.Repository("orgRepo", username=test_org.name)
-        org_repo_post_receive = gitea.git.Hook("orgRepoPostReceive",
+        org_repo_post_receive = gitea.GitHook("orgRepoPostReceive",
             user=test_org.name,
             repo=org_repo.name,
             content=(lambda path: open(path).read())(f"{path['module']}/post-receive.sh"))
         ```
 
         :param str resource_name: The name of the resource.
-        :param HookArgs args: The arguments to use to populate this resource's properties.
+        :param GitHookArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(HookArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(GitHookArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -241,61 +241,61 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = HookArgs.__new__(HookArgs)
+            __props__ = GitHookArgs.__new__(GitHookArgs)
 
             if content is None and not opts.urn:
                 raise TypeError("Missing required property 'content'")
             __props__.__dict__["content"] = content
             __props__.__dict__["name"] = name
             if repo is None and not opts.urn:
                 raise TypeError("Missing required property 'repo'")
             __props__.__dict__["repo"] = repo
             if user is None and not opts.urn:
                 raise TypeError("Missing required property 'user'")
             __props__.__dict__["user"] = user
-        super(Hook, __self__).__init__(
-            'gitea:Git/hook:Hook',
+        super(GitHook, __self__).__init__(
+            'gitea:index/gitHook:GitHook',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             content: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             repo: Optional[pulumi.Input[str]] = None,
-            user: Optional[pulumi.Input[str]] = None) -> 'Hook':
+            user: Optional[pulumi.Input[str]] = None) -> 'GitHook':
         """
-        Get an existing Hook resource's state with the given name, id, and optional extra
+        Get an existing GitHook resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] content: Content of the git hook
         :param pulumi.Input[str] name: Name of the git hook to configure
         :param pulumi.Input[str] repo: The repository that this hook belongs too.
         :param pulumi.Input[str] user: The user (or organisation) owning the repo this hook belongs too
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _HookState.__new__(_HookState)
+        __props__ = _GitHookState.__new__(_GitHookState)
 
         __props__.__dict__["content"] = content
         __props__.__dict__["name"] = name
         __props__.__dict__["repo"] = repo
         __props__.__dict__["user"] = user
-        return Hook(resource_name, opts=opts, __props__=__props__)
+        return GitHook(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def content(self) -> pulumi.Output[str]:
         """
         Content of the git hook
         """
```

### Comparing `pulumi_gitea-0.0.2/pulumi_gitea/oauth2/app.py` & `pulumi_gitea-0.0.3/pulumi_gitea/oauth2_app.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 
-__all__ = ['AppArgs', 'App']
+__all__ = ['Oauth2AppArgs', 'Oauth2App']
 
 @pulumi.input_type
-class AppArgs:
+class Oauth2AppArgs:
     def __init__(__self__, *,
                  redirect_uris: pulumi.Input[Sequence[pulumi.Input[str]]],
                  confidential_client: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a App resource.
+        The set of arguments for constructing a Oauth2App resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] redirect_uris: Accepted redirect URIs
         :param pulumi.Input[bool] confidential_client: If set to false, it will be a public client (PKCE will be required)
         :param pulumi.Input[str] name: OAuth Application name
         """
         pulumi.set(__self__, "redirect_uris", redirect_uris)
         if confidential_client is not None:
             pulumi.set(__self__, "confidential_client", confidential_client)
@@ -63,23 +63,23 @@
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
-class _AppState:
+class _Oauth2AppState:
     def __init__(__self__, *,
                  client_id: Optional[pulumi.Input[str]] = None,
                  client_secret: Optional[pulumi.Input[str]] = None,
                  confidential_client: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  redirect_uris: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        Input properties used for looking up and filtering App resources.
+        Input properties used for looking up and filtering Oauth2App resources.
         :param pulumi.Input[str] client_id: OAuth2 Application client id
         :param pulumi.Input[str] client_secret: Oauth2 Application client secret
         :param pulumi.Input[bool] confidential_client: If set to false, it will be a public client (PKCE will be required)
         :param pulumi.Input[str] name: OAuth Application name
         :param pulumi.Input[Sequence[pulumi.Input[str]]] redirect_uris: Accepted redirect URIs
         """
         if client_id is not None:
@@ -150,15 +150,15 @@
         return pulumi.get(self, "redirect_uris")
 
     @redirect_uris.setter
     def redirect_uris(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "redirect_uris", value)
 
 
-class App(pulumi.CustomResource):
+class Oauth2App(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  confidential_client: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  redirect_uris: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
@@ -172,26 +172,26 @@
         :param pulumi.Input[str] name: OAuth Application name
         :param pulumi.Input[Sequence[pulumi.Input[str]]] redirect_uris: Accepted redirect URIs
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: AppArgs,
+                 args: Oauth2AppArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Handling [gitea oauth application](https://docs.gitea.io/en-us/oauth2-provider/) resources
 
         :param str resource_name: The name of the resource.
-        :param AppArgs args: The arguments to use to populate this resource's properties.
+        :param Oauth2AppArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(AppArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(Oauth2AppArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -202,63 +202,63 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = AppArgs.__new__(AppArgs)
+            __props__ = Oauth2AppArgs.__new__(Oauth2AppArgs)
 
             __props__.__dict__["confidential_client"] = confidential_client
             __props__.__dict__["name"] = name
             if redirect_uris is None and not opts.urn:
                 raise TypeError("Missing required property 'redirect_uris'")
             __props__.__dict__["redirect_uris"] = redirect_uris
             __props__.__dict__["client_id"] = None
             __props__.__dict__["client_secret"] = None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["clientSecret"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(App, __self__).__init__(
-            'gitea:Oauth2/app:App',
+        super(Oauth2App, __self__).__init__(
+            'gitea:index/oauth2App:Oauth2App',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             client_id: Optional[pulumi.Input[str]] = None,
             client_secret: Optional[pulumi.Input[str]] = None,
             confidential_client: Optional[pulumi.Input[bool]] = None,
             name: Optional[pulumi.Input[str]] = None,
-            redirect_uris: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'App':
+            redirect_uris: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'Oauth2App':
         """
-        Get an existing App resource's state with the given name, id, and optional extra
+        Get an existing Oauth2App resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] client_id: OAuth2 Application client id
         :param pulumi.Input[str] client_secret: Oauth2 Application client secret
         :param pulumi.Input[bool] confidential_client: If set to false, it will be a public client (PKCE will be required)
         :param pulumi.Input[str] name: OAuth Application name
         :param pulumi.Input[Sequence[pulumi.Input[str]]] redirect_uris: Accepted redirect URIs
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _AppState.__new__(_AppState)
+        __props__ = _Oauth2AppState.__new__(_Oauth2AppState)
 
         __props__.__dict__["client_id"] = client_id
         __props__.__dict__["client_secret"] = client_secret
         __props__.__dict__["confidential_client"] = confidential_client
         __props__.__dict__["name"] = name
         __props__.__dict__["redirect_uris"] = redirect_uris
-        return App(resource_name, opts=opts, __props__=__props__)
+        return Oauth2App(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="clientId")
     def client_id(self) -> pulumi.Output[str]:
         """
         OAuth2 Application client id
         """
```

### Comparing `pulumi_gitea-0.0.2/pulumi_gitea/org.py` & `pulumi_gitea-0.0.3/pulumi_gitea/org.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitea-0.0.2/pulumi_gitea/provider.py` & `pulumi_gitea-0.0.3/pulumi_gitea/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitea-0.0.2/pulumi_gitea/publickey/deployment_key.py` & `pulumi_gitea-0.0.3/pulumi_gitea/public_key.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 
-__all__ = ['DeploymentKeyArgs', 'DeploymentKey']
+__all__ = ['PublicKeyArgs', 'PublicKey']
 
 @pulumi.input_type
-class DeploymentKeyArgs:
+class PublicKeyArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  title: pulumi.Input[str],
                  username: pulumi.Input[str],
                  read_only: Optional[pulumi.Input[bool]] = None):
         """
-        The set of arguments for constructing a DeploymentKey resource.
+        The set of arguments for constructing a PublicKey resource.
         :param pulumi.Input[str] key: An armored SSH key to add
         :param pulumi.Input[str] title: Title of the key to add
         :param pulumi.Input[str] username: User to associate with the added key
         :param pulumi.Input[bool] read_only: Describe if the key has only read access or read/write
         """
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "title", title)
@@ -77,25 +77,25 @@
 
     @read_only.setter
     def read_only(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "read_only", value)
 
 
 @pulumi.input_type
-class _DeploymentKeyState:
+class _PublicKeyState:
     def __init__(__self__, *,
                  created: Optional[pulumi.Input[str]] = None,
                  fingerprint: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  read_only: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering DeploymentKey resources.
+        Input properties used for looking up and filtering PublicKey resources.
         :param pulumi.Input[str] key: An armored SSH key to add
         :param pulumi.Input[bool] read_only: Describe if the key has only read access or read/write
         :param pulumi.Input[str] title: Title of the key to add
         :param pulumi.Input[str] username: User to associate with the added key
         """
         if created is not None:
             pulumi.set(__self__, "created", created)
@@ -184,40 +184,40 @@
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
 
-class DeploymentKey(pulumi.CustomResource):
+class PublicKey(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  read_only: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        `PublicKey.DeploymentKey` manages ssh key that are associated with users.
+        `PublicKey` manages ssh key that are associated with users.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitea as gitea
 
         test = gitea.User("test",
             username="test",
             login_name="test",
             password="Geheim1!",
             email="test@user.dev",
             must_change_password=False)
-        test_user_key = gitea.public_key.DeploymentKey("testUserKey",
+        test_user_key = gitea.PublicKey("testUserKey",
             title="test",
             key=(lambda path: open(path).read())(f"{path['module']}/id_ed25519.pub"),
             username=test.username)
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -226,44 +226,44 @@
         :param pulumi.Input[str] title: Title of the key to add
         :param pulumi.Input[str] username: User to associate with the added key
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: DeploymentKeyArgs,
+                 args: PublicKeyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        `PublicKey.DeploymentKey` manages ssh key that are associated with users.
+        `PublicKey` manages ssh key that are associated with users.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitea as gitea
 
         test = gitea.User("test",
             username="test",
             login_name="test",
             password="Geheim1!",
             email="test@user.dev",
             must_change_password=False)
-        test_user_key = gitea.public_key.DeploymentKey("testUserKey",
+        test_user_key = gitea.PublicKey("testUserKey",
             title="test",
             key=(lambda path: open(path).read())(f"{path['module']}/id_ed25519.pub"),
             username=test.username)
         ```
 
         :param str resource_name: The name of the resource.
-        :param DeploymentKeyArgs args: The arguments to use to populate this resource's properties.
+        :param PublicKeyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(DeploymentKeyArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(PublicKeyArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -275,15 +275,15 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = DeploymentKeyArgs.__new__(DeploymentKeyArgs)
+            __props__ = PublicKeyArgs.__new__(PublicKeyArgs)
 
             if key is None and not opts.urn:
                 raise TypeError("Missing required property 'key'")
             __props__.__dict__["key"] = None if key is None else pulumi.Output.secret(key)
             __props__.__dict__["read_only"] = read_only
             if title is None and not opts.urn:
                 raise TypeError("Missing required property 'title'")
@@ -292,55 +292,55 @@
                 raise TypeError("Missing required property 'username'")
             __props__.__dict__["username"] = username
             __props__.__dict__["created"] = None
             __props__.__dict__["fingerprint"] = None
             __props__.__dict__["type"] = None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["key"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(DeploymentKey, __self__).__init__(
-            'gitea:PublicKey/deploymentKey:DeploymentKey',
+        super(PublicKey, __self__).__init__(
+            'gitea:index/publicKey:PublicKey',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             created: Optional[pulumi.Input[str]] = None,
             fingerprint: Optional[pulumi.Input[str]] = None,
             key: Optional[pulumi.Input[str]] = None,
             read_only: Optional[pulumi.Input[bool]] = None,
             title: Optional[pulumi.Input[str]] = None,
             type: Optional[pulumi.Input[str]] = None,
-            username: Optional[pulumi.Input[str]] = None) -> 'DeploymentKey':
+            username: Optional[pulumi.Input[str]] = None) -> 'PublicKey':
         """
-        Get an existing DeploymentKey resource's state with the given name, id, and optional extra
+        Get an existing PublicKey resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] key: An armored SSH key to add
         :param pulumi.Input[bool] read_only: Describe if the key has only read access or read/write
         :param pulumi.Input[str] title: Title of the key to add
         :param pulumi.Input[str] username: User to associate with the added key
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _DeploymentKeyState.__new__(_DeploymentKeyState)
+        __props__ = _PublicKeyState.__new__(_PublicKeyState)
 
         __props__.__dict__["created"] = created
         __props__.__dict__["fingerprint"] = fingerprint
         __props__.__dict__["key"] = key
         __props__.__dict__["read_only"] = read_only
         __props__.__dict__["title"] = title
         __props__.__dict__["type"] = type
         __props__.__dict__["username"] = username
-        return DeploymentKey(resource_name, opts=opts, __props__=__props__)
+        return PublicKey(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def created(self) -> pulumi.Output[str]:
         return pulumi.get(self, "created")
 
     @property
```

### Comparing `pulumi_gitea-0.0.2/pulumi_gitea/repositories/deployment_key.py` & `pulumi_gitea-0.0.3/pulumi_gitea/repository_key.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 
-__all__ = ['DeploymentKeyArgs', 'DeploymentKey']
+__all__ = ['RepositoryKeyArgs', 'RepositoryKey']
 
 @pulumi.input_type
-class DeploymentKeyArgs:
+class RepositoryKeyArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  repository: pulumi.Input[int],
                  title: pulumi.Input[str],
                  read_only: Optional[pulumi.Input[bool]] = None):
         """
-        The set of arguments for constructing a DeploymentKey resource.
+        The set of arguments for constructing a RepositoryKey resource.
         :param pulumi.Input[str] key: Armored SSH key to add
         :param pulumi.Input[int] repository: The ID of the repository where the deploy key belongs to
         :param pulumi.Input[str] title: Name of the deploy key
         :param pulumi.Input[bool] read_only: Whether this key has read or read/write access
         """
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "repository", repository)
@@ -77,22 +77,22 @@
 
     @read_only.setter
     def read_only(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "read_only", value)
 
 
 @pulumi.input_type
-class _DeploymentKeyState:
+class _RepositoryKeyState:
     def __init__(__self__, *,
                  key: Optional[pulumi.Input[str]] = None,
                  read_only: Optional[pulumi.Input[bool]] = None,
                  repository: Optional[pulumi.Input[int]] = None,
                  title: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering DeploymentKey resources.
+        Input properties used for looking up and filtering RepositoryKey resources.
         :param pulumi.Input[str] key: Armored SSH key to add
         :param pulumi.Input[bool] read_only: Whether this key has read or read/write access
         :param pulumi.Input[int] repository: The ID of the repository where the deploy key belongs to
         :param pulumi.Input[str] title: Name of the deploy key
         """
         if key is not None:
             pulumi.set(__self__, "key", key)
@@ -148,54 +148,54 @@
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
 
-class DeploymentKey(pulumi.CustomResource):
+class RepositoryKey(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  read_only: Optional[pulumi.Input[bool]] = None,
                  repository: Optional[pulumi.Input[int]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        `Repositories.DeploymentKey` manages a deploy key for a single gitea_repository.
+        `RepositoryKey` manages a deploy key for a single gitea_repository.
 
         Every key needs a unique name and unique key, i.e. no key can be added twice to the same repo
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] key: Armored SSH key to add
         :param pulumi.Input[bool] read_only: Whether this key has read or read/write access
         :param pulumi.Input[int] repository: The ID of the repository where the deploy key belongs to
         :param pulumi.Input[str] title: Name of the deploy key
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: DeploymentKeyArgs,
+                 args: RepositoryKeyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        `Repositories.DeploymentKey` manages a deploy key for a single gitea_repository.
+        `RepositoryKey` manages a deploy key for a single gitea_repository.
 
         Every key needs a unique name and unique key, i.e. no key can be added twice to the same repo
 
         :param str resource_name: The name of the resource.
-        :param DeploymentKeyArgs args: The arguments to use to populate this resource's properties.
+        :param RepositoryKeyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(DeploymentKeyArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(RepositoryKeyArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -207,61 +207,61 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = DeploymentKeyArgs.__new__(DeploymentKeyArgs)
+            __props__ = RepositoryKeyArgs.__new__(RepositoryKeyArgs)
 
             if key is None and not opts.urn:
                 raise TypeError("Missing required property 'key'")
             __props__.__dict__["key"] = key
             __props__.__dict__["read_only"] = read_only
             if repository is None and not opts.urn:
                 raise TypeError("Missing required property 'repository'")
             __props__.__dict__["repository"] = repository
             if title is None and not opts.urn:
                 raise TypeError("Missing required property 'title'")
             __props__.__dict__["title"] = title
-        super(DeploymentKey, __self__).__init__(
-            'gitea:Repositories/deploymentKey:DeploymentKey',
+        super(RepositoryKey, __self__).__init__(
+            'gitea:index/repositoryKey:RepositoryKey',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             key: Optional[pulumi.Input[str]] = None,
             read_only: Optional[pulumi.Input[bool]] = None,
             repository: Optional[pulumi.Input[int]] = None,
-            title: Optional[pulumi.Input[str]] = None) -> 'DeploymentKey':
+            title: Optional[pulumi.Input[str]] = None) -> 'RepositoryKey':
         """
-        Get an existing DeploymentKey resource's state with the given name, id, and optional extra
+        Get an existing RepositoryKey resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] key: Armored SSH key to add
         :param pulumi.Input[bool] read_only: Whether this key has read or read/write access
         :param pulumi.Input[int] repository: The ID of the repository where the deploy key belongs to
         :param pulumi.Input[str] title: Name of the deploy key
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _DeploymentKeyState.__new__(_DeploymentKeyState)
+        __props__ = _RepositoryKeyState.__new__(_RepositoryKeyState)
 
         __props__.__dict__["key"] = key
         __props__.__dict__["read_only"] = read_only
         __props__.__dict__["repository"] = repository
         __props__.__dict__["title"] = title
-        return DeploymentKey(resource_name, opts=opts, __props__=__props__)
+        return RepositoryKey(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def key(self) -> pulumi.Output[str]:
         """
         Armored SSH key to add
         """
```

### Comparing `pulumi_gitea-0.0.2/pulumi_gitea/repository.py` & `pulumi_gitea-0.0.3/pulumi_gitea/repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitea-0.0.2/pulumi_gitea/team.py` & `pulumi_gitea-0.0.3/pulumi_gitea/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitea-0.0.2/pulumi_gitea/user.py` & `pulumi_gitea-0.0.3/pulumi_gitea/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitea-0.0.2/pulumi_gitea.egg-info/PKG-INFO` & `pulumi_gitea-0.0.3/pulumi_gitea.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-gitea
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Pulumi package for creating and managing Gitea resources
 Home-page: https://github.com/MaienM/pulumi-gitea
 License: Apache-2.0
 Project-URL: Repository, https://github.com/MaienM/pulumi-gitea
 Keywords: pulumi gitea category/infrastructure
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_gitea-0.0.2/pulumi_gitea.egg-info/SOURCES.txt` & `pulumi_gitea-0.0.3/pulumi_gitea.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,30 +3,26 @@
 pulumi_gitea/__init__.py
 pulumi_gitea/_utilities.py
 pulumi_gitea/access_token.py
 pulumi_gitea/fork.py
 pulumi_gitea/get_org.py
 pulumi_gitea/get_repo.py
 pulumi_gitea/get_user.py
+pulumi_gitea/git_hook.py
+pulumi_gitea/oauth2_app.py
 pulumi_gitea/org.py
 pulumi_gitea/provider.py
+pulumi_gitea/public_key.py
 pulumi_gitea/pulumi-plugin.json
 pulumi_gitea/py.typed
 pulumi_gitea/repository.py
+pulumi_gitea/repository_key.py
 pulumi_gitea/team.py
 pulumi_gitea/user.py
 pulumi_gitea.egg-info/PKG-INFO
 pulumi_gitea.egg-info/SOURCES.txt
 pulumi_gitea.egg-info/dependency_links.txt
 pulumi_gitea.egg-info/not-zip-safe
 pulumi_gitea.egg-info/requires.txt
 pulumi_gitea.egg-info/top_level.txt
 pulumi_gitea/config/__init__.py
-pulumi_gitea/config/vars.py
-pulumi_gitea/git/__init__.py
-pulumi_gitea/git/hook.py
-pulumi_gitea/oauth2/__init__.py
-pulumi_gitea/oauth2/app.py
-pulumi_gitea/publickey/__init__.py
-pulumi_gitea/publickey/deployment_key.py
-pulumi_gitea/repositories/__init__.py
-pulumi_gitea/repositories/deployment_key.py
+pulumi_gitea/config/vars.py
```

### Comparing `pulumi_gitea-0.0.2/setup.py` & `pulumi_gitea-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import errno
 import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "gitea Pulumi Package - Development Version"
```

