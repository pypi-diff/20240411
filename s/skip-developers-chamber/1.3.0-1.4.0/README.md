# Comparing `tmp/skip-developers-chamber-1.3.0.tar.gz` & `tmp/skip-developers-chamber-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-developers-chamber-1.3.0.tar", last modified: Thu Mar  7 13:58:02 2024, max compression
+gzip compressed data, was "skip-developers-chamber-1.4.0.tar", last modified: Thu Apr 11 09:36:00 2024, max compression
```

## Comparing `skip-developers-chamber-1.3.0.tar` & `skip-developers-chamber-1.4.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:58:02.497466 skip-developers-chamber-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-07 13:58:02.497466 skip-developers-chamber-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15303 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:58:02.489466 skip-developers-chamber-1.3.0/developers_chamber/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:58:02.489466 skip-developers-chamber-1.3.0/developers_chamber/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/bin/pydev.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/bitbucket_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:58:02.489466 skip-developers-chamber-1.3.0/developers_chamber/click/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/click/options.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    27455 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/ecs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/gitlab_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/jira_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/project_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:58:02.493466 skip-developers-chamber-1.3.0/developers_chamber/qa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/qa/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/qa/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:58:02.493466 skip-developers-chamber-1.3.0/developers_chamber/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/scripts/bitbucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/scripts/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15433 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/scripts/ecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/scripts/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/scripts/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/scripts/init_aliasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/scripts/jira.py
--rw-r--r--   0 runner    (1001) docker     (127)    18907 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/scripts/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/scripts/qa.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/scripts/sh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/scripts/slack.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/scripts/toggle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/scripts/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/slack_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/toggle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/developers_chamber/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 13:58:02.497466 skip-developers-chamber-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-07 13:57:51.000000 skip-developers-chamber-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:58:02.493466 skip-developers-chamber-1.3.0/skip_developers_chamber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-07 13:58:02.000000 skip-developers-chamber-1.3.0/skip_developers_chamber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-07 13:58:02.000000 skip-developers-chamber-1.3.0/skip_developers_chamber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 13:58:02.000000 skip-developers-chamber-1.3.0/skip_developers_chamber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-07 13:58:02.000000 skip-developers-chamber-1.3.0/skip_developers_chamber.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 13:58:02.000000 skip-developers-chamber-1.3.0/skip_developers_chamber.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-07 13:58:02.000000 skip-developers-chamber-1.3.0/skip_developers_chamber.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-07 13:58:02.000000 skip-developers-chamber-1.3.0/skip_developers_chamber.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:36:00.276886 skip-developers-chamber-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-11 09:36:00.276886 skip-developers-chamber-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15303 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:36:00.268886 skip-developers-chamber-1.4.0/developers_chamber/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:36:00.268886 skip-developers-chamber-1.4.0/developers_chamber/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/bin/pydev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/bitbucket_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:36:00.272886 skip-developers-chamber-1.4.0/developers_chamber/click/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/click/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27455 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/ecs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/gitlab_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/jira_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/project_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:36:00.272886 skip-developers-chamber-1.4.0/developers_chamber/qa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/qa/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/qa/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:36:00.272886 skip-developers-chamber-1.4.0/developers_chamber/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/bitbucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15433 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/init_aliasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/jira.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18907 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/sh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/toggle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/slack_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/toggle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:36:00.276886 skip-developers-chamber-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:36:00.276886 skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-11 09:36:00.000000 skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-11 09:36:00.000000 skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:36:00.000000 skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-11 09:36:00.000000 skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:36:00.000000 skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-11 09:36:00.000000 skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 09:36:00.000000 skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/top_level.txt
```

### Comparing `skip-developers-chamber-1.3.0/LICENSE` & `skip-developers-chamber-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/PKG-INFO` & `skip-developers-chamber-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-developers-chamber
-Version: 1.3.0
+Version: 1.4.0
 Summary: A small plugin which help with development, deployment, git
 Home-page: https://github.com/skip-pay/developers-chamber
 Author: Druids team
 Author-email: matllubos@gmail.com
 License: MIT
 Keywords: django,skripts,easy live,git,bitbucket,Jira
 License-File: LICENSE
```

### Comparing `skip-developers-chamber-1.3.0/README.md` & `skip-developers-chamber-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/bin/pydev.py` & `skip-developers-chamber-1.4.0/developers_chamber/bin/pydev.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/bitbucket_utils.py` & `skip-developers-chamber-1.4.0/developers_chamber/bitbucket_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/click/options.py` & `skip-developers-chamber-1.4.0/developers_chamber/click/options.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/ecs_utils.py` & `skip-developers-chamber-1.4.0/developers_chamber/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/git_utils.py` & `skip-developers-chamber-1.4.0/developers_chamber/git_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,39 +2,45 @@
 import re
 
 import git
 from click import BadParameter, UsageError
 from git import GitCommandError
 
 from .types import ReleaseType
-from .version_utils import bump_version
+from .version_utils import bump_version, get_next_version
 
 LATEST_TAG = "latest"
 DEFAULT_TARGET_BRANCH = os.environ.get('GITLAB_TARGET_BRANCH', 'next')
 DEPLOYMENT_COMMIT_PATTERN = r'^Deployment of "(?P<branch_name>.+)"$'
 RELEASE_BRANCH_PATTERN = r'^(?P<release_type>(release|patch))-(?P<version>[0-9]+\.[0-9]+\.[0-9]+)$'
 
 
-def create_release_branch(version, release_type, remote_name=None, branch_name=None):
+def create_release_branch(version_file, release_type, remote_name=None, branch_name=None):
     repo = git.Repo('.')
     g = repo.git
 
+    if remote_name:
+        # Ensures that all tags are up to date.
+        g.fetch(remote_name, "--tags", force=True)
+
     if branch_name:
         g.checkout(branch_name)
-    if remote_name:
-        g.pull(remote_name, branch_name)
+        if remote_name and branch_name != LATEST_TAG:
+            g.pull(remote_name, branch_name)
+
+    version = get_next_version(release_type, None, version_file)
 
-    current_branch = repo.active_branch.name
+    current_branch = branch_name or repo.active_branch.name
     if release_type in {ReleaseType.minor, ReleaseType.major}:
         if current_branch != DEFAULT_TARGET_BRANCH:
             raise UsageError(f'New release should be created from {DEFAULT_TARGET_BRANCH} branch')
         release_branch_name = 'release-{}'.format(version)
     elif release_type == ReleaseType.patch:
-        if not re.match(RELEASE_BRANCH_PATTERN, current_branch):
-            raise UsageError('New patch release should be created from either release or patch branch')
+        if current_branch != LATEST_TAG and not re.match(RELEASE_BRANCH_PATTERN, current_branch):
+            raise UsageError('New patch release should be created from either release or patch branch or latest tag')
         release_branch_name = 'patch-{}'.format(version)
     else:
         raise BadParameter('build is not allowed for release')
     g.checkout(branch_name or 'HEAD', b=release_branch_name)
 
     if remote_name:
         g.push(remote_name, release_branch_name, force=True)
```

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/gitlab_utils.py` & `skip-developers-chamber-1.4.0/developers_chamber/gitlab_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/jira_utils.py` & `skip-developers-chamber-1.4.0/developers_chamber/jira_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/project_utils.py` & `skip-developers-chamber-1.4.0/developers_chamber/project_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/qa/base.py` & `skip-developers-chamber-1.4.0/developers_chamber/qa/base.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/qa/checks.py` & `skip-developers-chamber-1.4.0/developers_chamber/qa/checks.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/scripts/bitbucket.py` & `skip-developers-chamber-1.4.0/developers_chamber/scripts/bitbucket.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/scripts/docker.py` & `skip-developers-chamber-1.4.0/developers_chamber/scripts/docker.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/scripts/ecs.py` & `skip-developers-chamber-1.4.0/developers_chamber/scripts/ecs.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/scripts/git.py` & `skip-developers-chamber-1.4.0/developers_chamber/scripts/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,15 @@
     """
     Create a release branch and push it to the remote repository if the remote name is specified.
     """
     if release_type == ReleaseType.build:
         raise click.BadParameter('build is not allowed for release')
     click.echo(
         'New release branch "{}" was created'.format(
-            create_release_branch_func(
-                get_next_version(release_type, None, file), release_type, remote_name, branch_name
-            )
+            create_release_branch_func(file, release_type, remote_name, branch_name)
         )
     )
 
 
 @git.command()
 @click.option('--environment', '-e', help='deployment environment', type=str, required=True)
 @click.option('--remote-name', '-r', help='remote repository name if you want to push the new branch', type=str,
```

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/scripts/gitlab.py` & `skip-developers-chamber-1.4.0/developers_chamber/scripts/gitlab.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/scripts/init_aliasses.py` & `skip-developers-chamber-1.4.0/developers_chamber/scripts/init_aliasses.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/scripts/jira.py` & `skip-developers-chamber-1.4.0/developers_chamber/scripts/jira.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/scripts/project.py` & `skip-developers-chamber-1.4.0/developers_chamber/scripts/project.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/scripts/qa.py` & `skip-developers-chamber-1.4.0/developers_chamber/scripts/qa.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/scripts/slack.py` & `skip-developers-chamber-1.4.0/developers_chamber/scripts/slack.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/scripts/toggle.py` & `skip-developers-chamber-1.4.0/developers_chamber/scripts/toggle.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/scripts/version.py` & `skip-developers-chamber-1.4.0/developers_chamber/scripts/version.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/slack_utils.py` & `skip-developers-chamber-1.4.0/developers_chamber/slack_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/toggle_utils.py` & `skip-developers-chamber-1.4.0/developers_chamber/toggle_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/types.py` & `skip-developers-chamber-1.4.0/developers_chamber/types.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/utils.py` & `skip-developers-chamber-1.4.0/developers_chamber/utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/developers_chamber/version_utils.py` & `skip-developers-chamber-1.4.0/developers_chamber/version_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.3.0/setup.py` & `skip-developers-chamber-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='skip-developers-chamber',
-    version='1.3.0',
+    version='1.4.0',
     description='A small plugin which help with development, deployment, git',
     keywords='django, skripts, easy live, git, bitbucket, Jira',
     author='Druids team',
     author_email='matllubos@gmail.com',
     url='https://github.com/skip-pay/developers-chamber',
     license='MIT',
     package_dir={'developers_chamber': 'developers_chamber'},
```

### Comparing `skip-developers-chamber-1.3.0/skip_developers_chamber.egg-info/PKG-INFO` & `skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-developers-chamber
-Version: 1.3.0
+Version: 1.4.0
 Summary: A small plugin which help with development, deployment, git
 Home-page: https://github.com/skip-pay/developers-chamber
 Author: Druids team
 Author-email: matllubos@gmail.com
 License: MIT
 Keywords: django,skripts,easy live,git,bitbucket,Jira
 License-File: LICENSE
```

### Comparing `skip-developers-chamber-1.3.0/skip_developers_chamber.egg-info/SOURCES.txt` & `skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

