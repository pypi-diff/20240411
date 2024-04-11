# Comparing `tmp/sciexp2-expdef-2.1.2.tar.gz` & `tmp/sciexp2-expdef-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sciexp2-expdef-2.1.2.tar", last modified: Wed Mar 13 17:58:09 2024, max compression
+gzip compressed data, was "dist/sciexp2-expdef-2.1.3.tar", last modified: Thu Apr 11 15:33:26 2024, max compression
```

## Comparing `sciexp2-expdef-2.1.2.tar` & `sciexp2-expdef-2.1.3.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:58:09.000000 sciexp2-expdef-2.1.2/
--rw-r--r--   0 root         (0) root         (0)     1473 2024-03-13 17:58:09.000000 sciexp2-expdef-2.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    35147 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/.requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1682 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:58:09.000000 sciexp2-expdef-2.1.2/sciexp2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:58:09.000000 sciexp2-expdef-2.1.2/sciexp2/expdef/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:58:09.000000 sciexp2-expdef-2.1.2/sciexp2/expdef/system/
--rw-rw-rw-   0 root         (0) root         (0)     2224 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/expdef/system/shell.py
--rw-rw-rw-   0 root         (0) root         (0)     9636 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/expdef/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4277 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/expdef/system/gridengine.py
--rw-rw-rw-   0 root         (0) root         (0)    52094 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/expdef/experiments.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:58:09.000000 sciexp2-expdef-2.1.2/sciexp2/expdef/templates/
--rwxrwxrwx   0 root         (0) root         (0)     5070 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/expdef/templates/gridengine.tpl
--rw-rw-rw-   0 root         (0) root         (0)      527 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/expdef/templates/gridengine.dsc
--rwxrwxrwx   0 root         (0) root         (0)     2687 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/expdef/templates/shell.tpl
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/expdef/templates/shell.dsc
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/expdef/templates/dacupc-gridengine.dsc
--rw-rw-rw-   0 root         (0) root         (0)      347 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/expdef/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11349 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/expdef/launcher.py
--rw-rw-rw-   0 root         (0) root         (0)    12015 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/expdef/templates.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/expdef/env.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:58:09.000000 sciexp2-expdef-2.1.2/sciexp2/common/
--rw-rw-rw-   0 root         (0) root         (0)    14817 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/common/text.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16385 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/common/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    13877 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/common/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     4835 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/common/filter.py
--rw-rw-rw-   0 root         (0) root         (0)      927 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/common/pp.py
--rw-rw-rw-   0 root         (0) root         (0)    24868 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/common/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     9931 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/sciexp2/common/parallel.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 17:58:09.000000 sciexp2-expdef-2.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:58:09.000000 sciexp2-expdef-2.1.2/sciexp2_expdef.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1473 2024-03-13 17:58:08.000000 sciexp2-expdef-2.1.2/sciexp2_expdef.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      907 2024-03-13 17:58:08.000000 sciexp2-expdef-2.1.2/sciexp2_expdef.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 17:58:08.000000 sciexp2-expdef-2.1.2/sciexp2_expdef.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-13 17:58:08.000000 sciexp2-expdef-2.1.2/sciexp2_expdef.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-03-13 17:58:08.000000 sciexp2-expdef-2.1.2/sciexp2_expdef.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)    12314 2024-03-13 17:57:50.000000 sciexp2-expdef-2.1.2/launcher
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/.requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/system/
+-rw-rw-rw-   0 root         (0) root         (0)     2356 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/system/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)     9636 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4277 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/system/gridengine.py
+-rw-rw-rw-   0 root         (0) root         (0)    53040 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/experiments.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/templates/
+-rwxrwxrwx   0 root         (0) root         (0)     5070 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/templates/gridengine.tpl
+-rw-rw-rw-   0 root         (0) root         (0)      527 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/templates/gridengine.dsc
+-rwxrwxrwx   0 root         (0) root         (0)     2687 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/templates/shell.tpl
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/templates/shell.dsc
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/templates/dacupc-gridengine.dsc
+-rw-rw-rw-   0 root         (0) root         (0)      347 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11349 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/launcher.py
+-rw-rw-rw-   0 root         (0) root         (0)    12015 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/templates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/expdef/env.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2/common/
+-rw-rw-rw-   0 root         (0) root         (0)    14817 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/common/text.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16498 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/common/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14779 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/common/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     4835 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/common/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      927 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/common/pp.py
+-rw-rw-rw-   0 root         (0) root         (0)    24868 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/sciexp2/common/instance.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2_expdef.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2_expdef.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      880 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2_expdef.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2_expdef.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2_expdef.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-11 15:33:26.000000 sciexp2-expdef-2.1.3/sciexp2_expdef.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)    12314 2024-04-11 15:33:08.000000 sciexp2-expdef-2.1.3/launcher
```

### Comparing `sciexp2-expdef-2.1.2/PKG-INFO` & `sciexp2-expdef-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciexp2-expdef
-Version: 2.1.2
+Version: 2.1.3
 Summary: Experiment definition framework for SciExp²
 Home-page: https://sciexp2-expdef.readthedocs.io/
 Author: Lluís Vilanova
 Author-email: llvilanovag@gmail.com
 License: GNU General Public License (GPL) version 3 or later
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sciexp2-expdef-2.1.2/LICENSE` & `sciexp2-expdef-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.2/setup.py` & `sciexp2-expdef-2.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.2/README.md` & `sciexp2-expdef-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.2/sciexp2/expdef/system/shell.py` & `sciexp2-expdef-2.1.3/sciexp2/expdef/system/shell.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """Launch and monitor local shell jobs."""
 
 __author__ = "Lluís Vilanova"
-__copyright__ = "Copyright 2009-2023, Lluís Vilanova"
+__copyright__ = "Copyright 2009-2024, Lluís Vilanova"
 __license__ = "GPL version 3 or later"
 
 
 import os
 import subprocess
+import sys
 
 import sciexp2.expdef.system
 import sciexp2.common.instance
 from sciexp2.common import progress
 from sciexp2.common.utils import execute_with_sigint
 
 
@@ -52,19 +53,20 @@
 
     def submit(self, *args):
         launcher = os.sep.join([self._system._base, self["LAUNCHER"]])
         assert os.path.isfile(launcher)
 
         cmd = ["bash"] + self._submit_args(args) + [launcher]
         progress.verbose(" %s", " ".join(cmd))
-        if progress.level() < progress.LVL_DEBUG:
-            kwargs = dict(stdout=sciexp2.expdef.system._DEVNULL,
-                          stderr=subprocess.STDOUT)
-        else:
-            kwargs = dict(stderr=subprocess.STDOUT)
+        kwargs = dict(stdout=sciexp2.expdef.system._DEVNULL,
+                      stderr=sciexp2.expdef.system._DEVNULL)
+        if progress.level() > progress.LVL_PROGRESS:
+            kwargs["stderr"] = progress.get_writer(sys.stderr)
+        if progress.level() >= progress.LVL_VERBOSE:
+            kwargs["stdout"] = progress.get_writer(sys.stdout)
 
         res = execute_with_sigint(cmd, **kwargs)
         if res != 0:
             raise subprocess.CalledProcessError(res, cmd)
 
     def kill(self, *args):
         raise Exception("Cannot kill local shell script jobs")
```

### Comparing `sciexp2-expdef-2.1.2/sciexp2/expdef/system/__init__.py` & `sciexp2-expdef-2.1.3/sciexp2/expdef/system/__init__.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.2/sciexp2/expdef/system/gridengine.py` & `sciexp2-expdef-2.1.3/sciexp2/expdef/system/gridengine.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.2/sciexp2/expdef/experiments.py` & `sciexp2-expdef-2.1.3/sciexp2/expdef/experiments.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 __author__ = "Lluís Vilanova"
 __copyright__ = "Copyright 2008-2024, Lluís Vilanova"
 __license__ = "GPL version 3 or later"
 
 
 import collections
 import contextlib
+import concurrent
 import functools
 import itertools
 import operator
 import os
 import shutil
 import six
+import sys
+import threading
 import warnings
 
-from sciexp2.common import parallel as parallel_pkg
 from sciexp2.common import progress
 from sciexp2.common import utils
 from sciexp2.common.instance import InstanceGroup, Instance
 from sciexp2.common.filter import *
 from sciexp2.common.utils import execute_with_sigint
 from sciexp2.common import pp
 from sciexp2.common import text
@@ -35,14 +37,23 @@
     def __init__(self, object):
         self._object = object
     def __repr__(self):
         keys = sorted(self._object.keys())
         return "{%s}" % ", ".join("%r: %r" % (key, self._object[key])
                                   for key in keys)
 
+def get_executor_workers(parallel):
+    if not parallel:
+        return 1
+    elif parallel is True:
+        return os.cpu_count()
+    else:
+        return parallel
+
+
 ######################################################################
 # Experiments
 
 def _is_dummy(experiments):
     if isinstance(experiments, Experiments):
         return (len(experiments._experiments) == 1 and
                 len(experiments._experiments.get_index(0)) == 0)
@@ -116,15 +127,15 @@
     cmd_flat = cmd_arg_sep.join(cmd)
     def get_cmd(cmd):
         return cmd.split(cmd_arg_sep)
 
     translator = text.Translator(cmd_flat)
     exp_cmds = translator.translate_many(experiments_list, with_envs=True)
 
-    def execute(exp_cmd):
+    def execute(exp_cmd, progr):
         cmd = get_cmd(exp_cmd[0])
         exp = exp_cmd[1][0]
         exp_rest = exp_cmd[1][1:]
 
         progress.verbose(" ".join(cmd))
         if len(exp_rest) > 0:
             if repeat == "warn":
@@ -137,16 +148,21 @@
                         exp, exp_rest[0]))
 
 
         def get_stdfile(name, env):
             @contextlib.contextmanager
             def as_context(arg):
                 yield arg
+
             translator = std_translator[name]
-            if translator is None:
+            if translator is None and name == "stdout":
+                return progress.get_writer(sys.stdout)
+            elif translator is None and name == "stderr":
+                return progress.get_writer(sys.stderr)
+            elif translator is None:
                 return as_context(std_args[name])
             else:
                 with env.auto_translate():
                     path = translator.translate(env)
                 return open(path, "w")
 
         with get_stdfile("stdin",  exp) as stdin,\
@@ -162,26 +178,22 @@
             raise Exception("Command did not finish correctly: "
                             "%s -> %d" % (" ".join(cmd), res))
 
         return len(exp_cmd[1])
 
     # use progr() explicitly to ensure progress is made after each command
     with progress.get(experiments_list, msg="Executing commands...") as progr:
-        if parallel is False:
-            for exp in exp_cmds:
-                exp_cmd = exp[0]
-                exps = exp[1]
-                count = execute(exp)
-                progr(count)
-        else:
-            if parallel is True:
-                parallel = None
-            for count in parallel_pkg.t_imap_unordered(
-                    exp_cmds, execute, parallelism=parallel):
-                progr(count)
+        max_workers = get_executor_workers(parallel)
+
+        def execute_with_progress(exp):
+            count = execute(exp, progr)
+            progr(count)
+
+        with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
+            list(executor.map(execute_with_progress, exp_cmds))
 
 
 def _do_recombine(experiments, exp_filters, variables, var_filters, append):
     exp_filters = and_filters(*exp_filters)
     var_filters = and_filters(*var_filters)
 
     # normalize variable value types
@@ -430,29 +442,32 @@
                               for template in parsed_templates]
                 add(translated, exp)
 
     return list(result())
 
 
 def _do_generate(experiments, template_from, template_to,
-                 pre_exp_fun, post_exp_fun):
+                 pre_exp_fun, post_exp_fun, parallel):
+    out = os.path.abspath(utils.get_path(experiments.out))
     translate_from = text.Translator(template_from)
     translate_to = text.Translator(template_to)
 
     done_first = {}
     done_exp = {}
+
     with progress.get(len(experiments), msg="generating files...") as progr:
-        for exp in experiments:
+
+        def generate_with_progress(exp):
             with exp.auto_translate():
                 _WithExp._EXPERIMENT = exp
                 _WithExpTpl._EXPERIMENT = exp
 
                 path_from = utils.get_path(translate_from.translate(exp))
                 path_to = utils.get_path(translate_to.translate(exp))
-                path_to = os.path.join(experiments.out, path_to)
+                path_to = os.path.join(out, path_to)
 
                 done_idx = path_from + "+" + path_to
                 if done_idx in done_first:
                     if done_first[done_idx]:
                         done_first[done_idx] = False
                         progress.info(
                             "Skipping already generated file: %s -> %s",
@@ -474,32 +489,39 @@
                             contents_to_old = f.read()
                     else:
                         contents_to_old = ""
 
                     if contents_to != contents_to_old:
                         with open(path_to, "w") as f:
                             f.write(contents_to)
+                    elif not os.path.isfile(path_to):
+                        utils.get_file(path_to, "w")
                     shutil.copymode(path_from, path_to)
 
                     post_exp_fun(exp, path_to)
 
-                progr()
+            progr()
 
-def _do_generate_user(experiments, template_from, template_to):
+        max_workers = get_executor_workers(parallel)
+        with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
+            list(executor.map(generate_with_progress, experiments))
+
+
+def _do_generate_user(experiments, template_from, template_to, parallel):
     def pre_exp_fun(exp, path_from, path_to):
         with open(path_from, "r") as f:
             contents_to = f.read()
         return exp, text.translate(contents_to, exp)
     def post_exp_fun(exp, path_to):
         pass
     _do_generate(experiments, template_from, template_to,
-                 pre_exp_fun, post_exp_fun)
+                 pre_exp_fun, post_exp_fun, parallel)
 
 def _do_generate_jobs(experiments, system, template_to, export, depends,
-                      submit_args, job_desc):
+                      submit_args, job_desc, parallel):
     template = templates.get(system)
 
     depends = set(depends) | set(["{{LAUNCHER}}"])
 
     # export all variables in depends
     export = set(export)
     for elem in depends:
@@ -565,15 +587,15 @@
             val = exp[var]
             if not _val_is_translate(val):
                 continue
             exp[var] = text.translate(val, exp)
         experiments_generated.add(Instance(exp))
 
     _do_generate(experiments, template.template_path, template_to,
-                 pre_exp_fun, post_exp_fun)
+                 pre_exp_fun, post_exp_fun, parallel)
 
     launcher.save(job_desc, job_desc_base,
                   template.system, experiments_generated,
                   export, depends, submit_args)
 
 
 class Experiments(pp.Pretty):
@@ -801,16 +823,15 @@
         repeat : str, optional
             What to do when more than one experiment is translated into the same
             command. Can be ``"ignore"``, ``"warn"`` (default), or ``"error"``.
         stdin, stdout, stderr : file or str, optional
             Paths for the standard input/output/error for the command (defaults
             to None).
         parallel : optional
-            Whether to execute commands in parallel using separate processes
-            (default is `False`).
+            Whether to execute commands in parallel (default is `False`).
 
         Notes
         -----
         Command execution is internally handled by `subproces.Popen` and thus
         the `stdin`, `stdout` and `stderr` arguments can also have any value
         accepted by it.
 
@@ -941,37 +962,40 @@
         There can be cases where multiple source files correspond to a single
         destination file (after translating the templates). Such cases are
         logged by a message.
 
         """
         _do_pack(self, template_from, template_to, dereference)
 
-    def generate(self, template_from, template_to):
+    def generate(self, template_from, template_to, parallel=True):
         """Generate files from other templated files.
 
         Like `pack`, the paths to source and destination files are
         templates. Every source file is, in addition, considered a template that
         will be translated with each of the experiments.
 
         Parameters
         ----------
         template_from, template_to : str
             Templates for Source/destination file paths.
+        parallel : optional
+            Whether to generate files in parallel (default is `True`).
 
         Notes
         -----
         Like `pack`, if multiple source files correspond to a single destination
         file (after translating the templates), the case is logged by a message
         and only the first generated file is kept.
 
         """
-        return _do_generate_user(self, template_from, template_to)
+        return _do_generate_user(self, template_from, template_to, parallel)
 
     def generate_jobs(self, system, template_to, export=[], depends=[],
-                      submit_args=[], job_desc="jobs.jd"):
+                      submit_args=[], job_desc="jobs.jd",
+                      parallel=True):
         """Generate job files for given job system.
 
         Works similar to `generate`, but takes a predefined source file template
         that is identified by `system`. It also creates a job descriptor file
         that can be later used by the `launcher` program.
 
         Parameters
@@ -984,14 +1008,16 @@
             List of variable names to export into the job descriptor file.
         depends : list of str, optional
             File path templates for job dependencies.
         submit_args : list of str, optional
             Templates for additional arguments to the job submission command.
         job_desc : str, optional
             Name of the output job descriptor file.
+        parallel : optional
+            Whether to generate files in parallel (default is `True`).
 
         All job systems implicitly define the *LAUNCHER* variable, which has the
         path of the to the generated script to run that. All job systems also
         define *DONE* and *FAIL* as file paths to identify the state of each
         job.
 
         The variables selected by `export` will be later available when using
@@ -1021,15 +1047,15 @@
         None of the experiments can define the *LAUNCHER* variable. Some job
         systems also define their own set of reserved variables and default
         values to others (in case your experiments don't specify them); see the
         job system's documentation for more information.
 
         """
         _do_generate_jobs(self, system, template_to, export, depends,
-                          submit_args, job_desc)
+                          submit_args, job_desc, parallel)
 
 
     def translate(self, template, with_exps=False, with_unique=True):
         """Translate the given templates with each experiment.
 
         Parameters
         ----------
```

### Comparing `sciexp2-expdef-2.1.2/sciexp2/expdef/templates/gridengine.tpl` & `sciexp2-expdef-2.1.3/sciexp2/expdef/templates/gridengine.tpl`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.2/sciexp2/expdef/templates/gridengine.dsc` & `sciexp2-expdef-2.1.3/sciexp2/expdef/templates/gridengine.dsc`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.2/sciexp2/expdef/templates/shell.tpl` & `sciexp2-expdef-2.1.3/sciexp2/expdef/templates/shell.tpl`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.2/sciexp2/expdef/templates/dacupc-gridengine.dsc` & `sciexp2-expdef-2.1.3/sciexp2/expdef/templates/dacupc-gridengine.dsc`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.2/sciexp2/expdef/launcher.py` & `sciexp2-expdef-2.1.3/sciexp2/expdef/launcher.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.2/sciexp2/expdef/templates.py` & `sciexp2-expdef-2.1.3/sciexp2/expdef/templates.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.2/sciexp2/expdef/env.py` & `sciexp2-expdef-2.1.3/sciexp2/expdef/env.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.2/sciexp2/common/text.py` & `sciexp2-expdef-2.1.3/sciexp2/common/text.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.2/sciexp2/common/utils.py` & `sciexp2-expdef-2.1.3/sciexp2/common/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,19 @@
                                                        ", ".join(kwargs)))
 
 # -----------------------------
 
 def assert_dir(path):
     """Check that given directory exists, otherwise create it."""
     if path != "" and not os.path.exists(path):
-        os.makedirs(path)
+        try:
+            os.makedirs(path)
+        except FileExistsError:
+            # might be due to concurrent mkdir
+            pass
 
 
 def assert_path(path):
     """Check that given path exists, otherwise create directories."""
     if not path.endswith(os.sep):
         path = os.path.dirname(path)
     assert_dir(path)
```

### Comparing `sciexp2-expdef-2.1.2/sciexp2/common/progress.py` & `sciexp2-expdef-2.1.3/sciexp2/common/progress.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 __copyright__ = "Copyright 2008-2024, Lluís Vilanova"
 __license__ = "GPL version 3 or later"
 
 
 import collections
 import itertools
 import numbers
+import os
 import sys
 import threading
 import types
 
 import six
 import tqdm
 
@@ -48,14 +49,32 @@
     #pylint: disable=bare-except
     except:
         _CLS = tqdm.tqdm
 else:
     _CLS = tqdm.tqdm
 
 
+def get_writer(file):
+    read_fd, write_fd = os.pipe()
+
+    write_wrapper = os.fdopen(write_fd, "w")
+    read_wrapper = os.fdopen(read_fd, "r")
+
+    def reader():
+        while True:
+            data = read_wrapper.readline()
+            if len(data) == 0:
+                return
+            tqdm.tqdm.write(data, end="", file=file)
+    reader_thread = threading.Thread(target=reader, daemon=True)
+    reader_thread.start()
+
+    return write_wrapper
+
+
 def level(level_=None):
     """Get/set the current progress indication level."""
     if level_ is not None:
         if level_ < LVL_NONE or LVL_DEBUG < level_:
             raise ValueError(f"Invalid progress level {level_}")
         # pylint: disable=global-statement
         global _LEVEL
@@ -134,14 +153,22 @@
     def __exit__(self, *args, **kwargs):
         self._cleanup()
 
     def __del__(self):
         """Delete the progress indicator from screen."""
         self._cleanup()
 
+    def write(self, s, file=None, end="\n", nolock=False):
+        if self._obj is not None:
+            return self._obj.write(s, file=file, end=end, nolock=nolock)
+        else:
+            if file is None:
+                file = sys.stdout
+            return file.write(s, end=end)
+
 
 class Null:
     """A "null" progress indicator.
 
     """
 
     def __init__(self, *args, **kwargs):
@@ -161,14 +188,19 @@
 
     def __exit__(self, *args, **kwargs):
         pass
 
     def __del__(self):
         pass
 
+    def write(self, s, file=None, end="\n", nolock=False):
+        if file is None:
+            file = sys.stdout
+        return file.write(s, end=end)
+
 
 def _progressable_get_func_wrapper(func, other, progr):
     """Update progress every time `func` is called."""
     # pylint: disable=unused-argument
     def wrapper(self, *args, **kwargs):
         res = func(other, *args, **kwargs)
         progr()
```

### Comparing `sciexp2-expdef-2.1.2/sciexp2/common/filter.py` & `sciexp2-expdef-2.1.3/sciexp2/common/filter.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.2/sciexp2/common/pp.py` & `sciexp2-expdef-2.1.3/sciexp2/common/pp.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.2/sciexp2/common/instance.py` & `sciexp2-expdef-2.1.3/sciexp2/common/instance.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.2/sciexp2_expdef.egg-info/PKG-INFO` & `sciexp2-expdef-2.1.3/sciexp2_expdef.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciexp2-expdef
-Version: 2.1.2
+Version: 2.1.3
 Summary: Experiment definition framework for SciExp²
 Home-page: https://sciexp2-expdef.readthedocs.io/
 Author: Lluís Vilanova
 Author-email: llvilanovag@gmail.com
 License: GNU General Public License (GPL) version 3 or later
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sciexp2-expdef-2.1.2/sciexp2_expdef.egg-info/SOURCES.txt` & `sciexp2-expdef-2.1.3/sciexp2_expdef.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 README.md
 launcher
 setup.py
 sciexp2/__init__.py
 sciexp2/common/__init__.py
 sciexp2/common/filter.py
 sciexp2/common/instance.py
-sciexp2/common/parallel.py
 sciexp2/common/pp.py
 sciexp2/common/progress.py
 sciexp2/common/text.py
 sciexp2/common/utils.py
 sciexp2/expdef/__init__.py
 sciexp2/expdef/env.py
 sciexp2/expdef/experiments.py
```

### Comparing `sciexp2-expdef-2.1.2/launcher` & `sciexp2-expdef-2.1.3/launcher`

 * *Files identical despite different names*

