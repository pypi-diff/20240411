# Comparing `tmp/Eryn-1.1.6.tar.gz` & `tmp/Eryn-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Eryn-1.1.6.tar", last modified: Fri Mar 15 23:29:20 2024, max compression
+gzip compressed data, was "Eryn-1.1.7.tar", last modified: Thu Apr 11 01:55:12 2024, max compression
```

## Comparing `Eryn-1.1.6.tar` & `Eryn-1.1.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-03-15 23:29:20.925566 Eryn-1.1.6/
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-03-15 23:29:20.923128 Eryn-1.1.6/Eryn.egg-info/
--rw-r--r--   0 mlkatz1    (502) staff       (20)     4938 2024-03-15 23:29:20.000000 Eryn-1.1.6/Eryn.egg-info/PKG-INFO
--rw-r--r--   0 mlkatz1    (502) staff       (20)      857 2024-03-15 23:29:20.000000 Eryn-1.1.6/Eryn.egg-info/SOURCES.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)        1 2024-03-15 23:29:20.000000 Eryn-1.1.6/Eryn.egg-info/dependency_links.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)        5 2024-03-15 23:29:20.000000 Eryn-1.1.6/Eryn.egg-info/top_level.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)     4938 2024-03-15 23:29:20.923988 Eryn-1.1.6/PKG-INFO
--rw-r--r--   0 mlkatz1    (502) staff       (20)     4623 2024-03-15 23:27:25.000000 Eryn-1.1.6/README.md
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-03-15 23:29:20.908254 Eryn-1.1.6/eryn/
--rw-r--r--   0 mlkatz1    (502) staff       (20)       38 2023-05-16 15:38:51.000000 Eryn-1.1.6/eryn/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)       21 2024-03-15 23:29:20.000000 Eryn-1.1.6/eryn/_version.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-03-15 23:29:20.909918 Eryn-1.1.6/eryn/backends/
--rw-r--r--   0 mlkatz1    (502) staff       (20)      380 2023-05-16 15:38:51.000000 Eryn-1.1.6/eryn/backends/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    43826 2024-03-15 23:26:44.000000 Eryn-1.1.6/eryn/backends/backend.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    28148 2024-03-15 23:26:44.000000 Eryn-1.1.6/eryn/backends/hdfbackend.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    68508 2024-03-15 23:26:44.000000 Eryn-1.1.6/eryn/ensemble.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)      284 2023-05-16 15:38:51.000000 Eryn-1.1.6/eryn/model.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-03-15 23:29:20.919131 Eryn-1.1.6/eryn/moves/
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1081 2023-05-16 15:38:51.000000 Eryn-1.1.6/eryn/moves/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     4547 2023-05-16 15:38:51.000000 Eryn-1.1.6/eryn/moves/combine.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     7670 2023-05-16 15:38:51.000000 Eryn-1.1.6/eryn/moves/delayedrejection.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     3935 2023-05-16 22:44:45.000000 Eryn-1.1.6/eryn/moves/distgen.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     9133 2023-05-16 15:38:51.000000 Eryn-1.1.6/eryn/moves/distgenrj.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     6723 2023-08-05 00:53:53.000000 Eryn-1.1.6/eryn/moves/gaussian.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     8987 2024-03-15 23:26:44.000000 Eryn-1.1.6/eryn/moves/group.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     3493 2023-05-16 15:38:51.000000 Eryn-1.1.6/eryn/moves/groupstretch.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     6425 2023-05-16 15:38:51.000000 Eryn-1.1.6/eryn/moves/mh.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    28550 2024-03-15 23:26:44.000000 Eryn-1.1.6/eryn/moves/move.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     5347 2023-05-16 15:38:51.000000 Eryn-1.1.6/eryn/moves/mtdistgen.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     8102 2023-05-16 15:38:51.000000 Eryn-1.1.6/eryn/moves/mtdistgenrj.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    29921 2024-03-15 23:26:44.000000 Eryn-1.1.6/eryn/moves/multipletry.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    13091 2024-03-15 23:26:44.000000 Eryn-1.1.6/eryn/moves/red_blue.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    15915 2023-06-07 23:55:44.000000 Eryn-1.1.6/eryn/moves/rj.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     8242 2024-03-15 23:26:44.000000 Eryn-1.1.6/eryn/moves/stretch.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    23812 2023-05-16 15:38:51.000000 Eryn-1.1.6/eryn/moves/tempering.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1330 2023-05-16 15:38:51.000000 Eryn-1.1.6/eryn/pbar.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    12643 2024-03-15 23:26:44.000000 Eryn-1.1.6/eryn/prior.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    31096 2024-03-15 23:26:44.000000 Eryn-1.1.6/eryn/state.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-03-15 23:29:20.922243 Eryn-1.1.6/eryn/utils/
--rw-r--r--   0 mlkatz1    (502) staff       (20)      250 2023-05-16 15:38:51.000000 Eryn-1.1.6/eryn/utils/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     3983 2023-05-16 15:38:51.000000 Eryn-1.1.6/eryn/utils/periodic.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     5095 2023-05-16 15:38:51.000000 Eryn-1.1.6/eryn/utils/stopping.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     8895 2023-05-16 15:38:51.000000 Eryn-1.1.6/eryn/utils/transform.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     2137 2023-05-16 15:38:51.000000 Eryn-1.1.6/eryn/utils/updates.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    11173 2023-08-05 00:53:53.000000 Eryn-1.1.6/eryn/utils/utility.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)       72 2023-05-16 15:38:51.000000 Eryn-1.1.6/pyproject.toml
--rw-r--r--   0 mlkatz1    (502) staff       (20)       38 2024-03-15 23:29:20.925824 Eryn-1.1.6/setup.cfg
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1037 2023-05-16 15:38:51.000000 Eryn-1.1.6/setup.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-11 01:55:12.666208 Eryn-1.1.7/
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-11 01:55:12.663773 Eryn-1.1.7/Eryn.egg-info/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     4938 2024-04-11 01:55:12.000000 Eryn-1.1.7/Eryn.egg-info/PKG-INFO
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      857 2024-04-11 01:55:12.000000 Eryn-1.1.7/Eryn.egg-info/SOURCES.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        1 2024-04-11 01:55:12.000000 Eryn-1.1.7/Eryn.egg-info/dependency_links.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        5 2024-04-11 01:55:12.000000 Eryn-1.1.7/Eryn.egg-info/top_level.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     4938 2024-04-11 01:55:12.665140 Eryn-1.1.7/PKG-INFO
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     4623 2024-04-11 01:25:29.000000 Eryn-1.1.7/README.md
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-11 01:55:12.630287 Eryn-1.1.7/eryn/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       38 2023-05-16 15:38:51.000000 Eryn-1.1.7/eryn/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       21 2024-04-11 01:55:12.000000 Eryn-1.1.7/eryn/_version.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-11 01:55:12.632836 Eryn-1.1.7/eryn/backends/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      380 2023-05-16 15:38:51.000000 Eryn-1.1.7/eryn/backends/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    44843 2024-04-11 01:39:25.000000 Eryn-1.1.7/eryn/backends/backend.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    28148 2024-03-15 23:26:44.000000 Eryn-1.1.7/eryn/backends/hdfbackend.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    68265 2024-04-11 01:35:33.000000 Eryn-1.1.7/eryn/ensemble.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      284 2023-05-16 15:38:51.000000 Eryn-1.1.7/eryn/model.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-11 01:55:12.654111 Eryn-1.1.7/eryn/moves/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1081 2023-05-16 15:38:51.000000 Eryn-1.1.7/eryn/moves/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     4547 2023-05-16 15:38:51.000000 Eryn-1.1.7/eryn/moves/combine.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     7670 2023-05-16 15:38:51.000000 Eryn-1.1.7/eryn/moves/delayedrejection.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     3935 2023-05-16 22:44:45.000000 Eryn-1.1.7/eryn/moves/distgen.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     9133 2023-05-16 15:38:51.000000 Eryn-1.1.7/eryn/moves/distgenrj.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     6853 2024-04-11 01:22:24.000000 Eryn-1.1.7/eryn/moves/gaussian.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     9013 2024-04-11 01:51:52.000000 Eryn-1.1.7/eryn/moves/group.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     3493 2023-05-16 15:38:51.000000 Eryn-1.1.7/eryn/moves/groupstretch.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     6425 2023-05-16 15:38:51.000000 Eryn-1.1.7/eryn/moves/mh.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    28550 2024-03-15 23:26:44.000000 Eryn-1.1.7/eryn/moves/move.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     5347 2023-05-16 15:38:51.000000 Eryn-1.1.7/eryn/moves/mtdistgen.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     8102 2023-05-16 15:38:51.000000 Eryn-1.1.7/eryn/moves/mtdistgenrj.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    30156 2024-04-11 01:44:57.000000 Eryn-1.1.7/eryn/moves/multipletry.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    13091 2024-03-15 23:26:44.000000 Eryn-1.1.7/eryn/moves/red_blue.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    15915 2023-06-07 23:55:44.000000 Eryn-1.1.7/eryn/moves/rj.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     8242 2024-03-15 23:26:44.000000 Eryn-1.1.7/eryn/moves/stretch.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    23812 2023-05-16 15:38:51.000000 Eryn-1.1.7/eryn/moves/tempering.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1330 2023-05-16 15:38:51.000000 Eryn-1.1.7/eryn/pbar.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    12643 2024-03-15 23:26:44.000000 Eryn-1.1.7/eryn/prior.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    31096 2024-03-15 23:26:44.000000 Eryn-1.1.7/eryn/state.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-11 01:55:12.662141 Eryn-1.1.7/eryn/utils/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      250 2023-05-16 15:38:51.000000 Eryn-1.1.7/eryn/utils/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     4135 2024-04-11 01:25:16.000000 Eryn-1.1.7/eryn/utils/periodic.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     5095 2023-05-16 15:38:51.000000 Eryn-1.1.7/eryn/utils/stopping.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     8895 2023-05-16 15:38:51.000000 Eryn-1.1.7/eryn/utils/transform.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     2137 2023-05-16 15:38:51.000000 Eryn-1.1.7/eryn/utils/updates.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    11173 2023-08-05 00:53:53.000000 Eryn-1.1.7/eryn/utils/utility.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       72 2023-05-16 15:38:51.000000 Eryn-1.1.7/pyproject.toml
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       38 2024-04-11 01:55:12.666441 Eryn-1.1.7/setup.cfg
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1037 2024-04-11 01:53:15.000000 Eryn-1.1.7/setup.py
```

### Comparing `Eryn-1.1.6/Eryn.egg-info/PKG-INFO` & `Eryn-1.1.7/Eryn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Eryn
-Version: 1.1.6
+Version: 1.1.7
 Summary: An all purpose MCMC sampler
 Home-page: https://github.com/mikekatz04/Eryn
 Author: Michael Katz, Nikos Karnesis
 Author-email: mikekatz04@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -55,15 +55,15 @@
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms/tags).
 
-Current Version: 1.1.6
+Current Version: 1.1.7
 
 ## Citation
 
 When using this package, please cite at minimum the following sources:
 
 ```
 @article{Karnesis:2023ras,
```

### Comparing `Eryn-1.1.6/Eryn.egg-info/SOURCES.txt` & `Eryn-1.1.7/Eryn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/PKG-INFO` & `Eryn-1.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Eryn
-Version: 1.1.6
+Version: 1.1.7
 Summary: An all purpose MCMC sampler
 Home-page: https://github.com/mikekatz04/Eryn
 Author: Michael Katz, Nikos Karnesis
 Author-email: mikekatz04@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -55,15 +55,15 @@
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms/tags).
 
-Current Version: 1.1.6
+Current Version: 1.1.7
 
 ## Citation
 
 When using this package, please cite at minimum the following sources:
 
 ```
 @article{Karnesis:2023ras,
```

### Comparing `Eryn-1.1.6/README.md` & `Eryn-1.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms/tags).
 
-Current Version: 1.1.6
+Current Version: 1.1.7
 
 ## Citation
 
 When using this package, please cite at minimum the following sources:
 
 ```
 @article{Karnesis:2023ras,
```

### Comparing `Eryn-1.1.6/eryn/backends/backend.py` & `Eryn-1.1.7/eryn/backends/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
 
-from ..utils.utility import get_integrated_act, thermodynamic_integration_log_evidence, stepping_stone_log_evidence, psrf
+from ..utils.utility import (
+    get_integrated_act,
+    thermodynamic_integration_log_evidence,
+    stepping_stone_log_evidence,
+    psrf,
+)
 from ..state import State
 
 __all__ = ["Backend"]
 
 
 class Backend(object):
     """A simple default backend that stores the chain in memory
@@ -36,19 +41,19 @@
         initiailized (bool): If ``True``, backend object has been initialized.
         iteration (int): Current index within the data storage arrays.
         log_prior (3D double np.ndarray): Log of the prior values. Shape is
             (nsteps, nwalkers, ntemps).
         log_like (3D double np.ndarray): Log of the likelihood values. Shape is
             (nsteps, nwalkers, ntemps).
         move_info (dict): Dictionary containing move info.
-        move_keys (list): List of keys for ``move_info``. 
+        move_keys (list): List of keys for ``move_info``.
         nbranches (int): Number of branches.
         ndims (dict): Dimensionality of each branch.
         nleaves_max (dict): Maximum allowable leaves for each branch.
-        nwalkers (int): The size of the ensemble (per temperature). 
+        nwalkers (int): The size of the ensemble (per temperature).
         ntemps (int): Number of rungs in the temperature ladder.
         reset_args (tuple): Arguments to reset backend.
         reset_kwargs (dict): Keyword arguments to reset backend.
         rj (bool): If True, reversible-jump techniques are used.
         rj_accepted (2D int np.ndarray): Number of accepted steps for between-model moves.
             The shape is (ntemps, nwalkers).
         store_missing_leaves (double): Number to store for leaves that are not
@@ -82,16 +87,16 @@
     ):
         """Clear the state of the chain and empty the backend
 
         Args:
             nwalkers (int): The size of the ensemble (per temperature).
             ndims (int, list of ints, or dict): The number of dimensions for each branch. If
                 ``dict``, keys should be the branch names and values the associated dimensionality.
-            nleaves_max (int, list of ints, or dict, optional): Maximum allowable leaf count for each branch. 
-                It should have the same length as the number of branches. 
+            nleaves_max (int, list of ints, or dict, optional): Maximum allowable leaf count for each branch.
+                It should have the same length as the number of branches.
                 If ``dict``, keys should be the branch names and values the associated maximal leaf value.
                 (default: ``1``)
             ntemps (int, optional): Number of rungs in the temperature ladder.
                 (default: ``1``)
             branch_names (str or list of str, optional): Names of the branches used. If not given,
                 branches will be names ``model_0``, ..., ``model_n`` for ``n`` branches.
                 (default: ``None``)
@@ -146,15 +151,17 @@
             assert len(branch_names) == len(ndims)
             ndims = {bn: nd for bn, nd in zip(branch_names, ndims)}
 
         elif isinstance(ndims, dict):
             assert len(list(ndims.keys())) == len(branch_names)
             for key in ndims:
                 if key not in branch_names:
-                    raise ValueError(f"{key} is in ndims but does not appear in branch_names: {branch_names}.")
+                    raise ValueError(
+                        f"{key} is in ndims but does not appear in branch_names: {branch_names}."
+                    )
         else:
             raise ValueError("ndims is to be a scalar int, list or dict.")
 
         if isinstance(nleaves_max, int):
             assert len(branch_names) == 1
             nleaves_max = {branch_names[0]: nleaves_max}
 
@@ -162,15 +169,17 @@
             assert len(branch_names) == len(nleaves_max)
             nleaves_max = {bn: nl for bn, nl in zip(branch_names, nleaves_max)}
 
         elif isinstance(nleaves_max, dict):
             assert len(list(nleaves_max.keys())) == len(branch_names)
             for key in nleaves_max:
                 if key not in branch_names:
-                    raise ValueError(f"{key} is in nleaves_max but does not appear in branch_names: {branch_names}.")
+                    raise ValueError(
+                        f"{key} is in nleaves_max but does not appear in branch_names: {branch_names}."
+                    )
         else:
             raise ValueError("nleaves_max is to be a scalar int, list, or dict.")
 
         self.nbranches = len(branch_names)
 
         self.branch_names = branch_names
         self.ndims = ndims
@@ -186,22 +195,31 @@
 
         else:
             self.rj_accepted = None
 
         # chains are stored in dictionaries
         self.chain = {
             name: np.empty(
-                (0, self.ntemps, self.nwalkers, self.nleaves_max[name], self.ndims[name]), dtype=self.dtype
+                (
+                    0,
+                    self.ntemps,
+                    self.nwalkers,
+                    self.nleaves_max[name],
+                    self.ndims[name],
+                ),
+                dtype=self.dtype,
             )
             for name in self.branch_names
         }
 
         # inds correspond to leaves used or not
         self.inds = {
-            name: np.empty((0, self.ntemps, self.nwalkers, self.nleaves_max[name]), dtype=bool)
+            name: np.empty(
+                (0, self.ntemps, self.nwalkers, self.nleaves_max[name]), dtype=bool
+            )
             for name in self.branch_names
         }
 
         # log likelihood and prior
         self.log_like = np.empty((0, self.ntemps, self.nwalkers), dtype=self.dtype)
         self.log_prior = np.empty((0, self.ntemps, self.nwalkers), dtype=self.dtype)
 
@@ -294,17 +312,17 @@
 
         Args:
             thin (int, optional): Take only every ``thin`` steps from the
                 chain. (default: ``1``)
             discard (int, optional): Discard the first ``discard`` steps in
                 the chain as burn-in. (default: ``0``)
             slice_vals (indexing np.ndarray or slice, optional): This is only available in :class:`eryn.backends.hdfbackend`.
-                If provided, slice the array directly from the HDF5 file with slice = ``slice_vals``. 
-                ``thin`` and ``discard`` will be ignored if slice_vals is not ``None``. 
-                This is particularly useful if files are very large and the user only wants a 
+                If provided, slice the array directly from the HDF5 file with slice = ``slice_vals``.
+                ``thin`` and ``discard`` will be ignored if slice_vals is not ``None``.
+                This is particularly useful if files are very large and the user only wants a
                 small subset of the overall array. (default: ``None``)
 
         Returns:
             dict: MCMC samples
                 The dictionary contains np.ndarrays of samples
                 across the branches.
 
@@ -348,17 +366,17 @@
 
         Args:
             thin (int, optional): Take only every ``thin`` steps from the
                 chain. (default: ``1``)
             discard (int, optional): Discard the first ``discard`` steps in
                 the chain as burn-in. (default: ``0``)
             slice_vals (indexing np.ndarray or slice, optional): This is only available in :class:`eryn.backends.hdfbackend`.
-                If provided, slice the array directly from the HDF5 file with slice = ``slice_vals``. 
-                ``thin`` and ``discard`` will be ignored if slice_vals is not ``None``. 
-                This is particularly useful if files are very large and the user only wants a 
+                If provided, slice the array directly from the HDF5 file with slice = ``slice_vals``.
+                ``thin`` and ``discard`` will be ignored if slice_vals is not ``None``.
+                This is particularly useful if files are very large and the user only wants a
                 small subset of the overall array. (default: ``None``)
 
         Returns:
             dict: The ``inds`` associated with the MCMC samples.
                   The dictionary contains np.ndarrays of ``inds``
                   across the branches indicated which leaves were used at each step.
 
@@ -370,17 +388,17 @@
 
         Args:
             thin (int, optional): Take only every ``thin`` steps from the
                 chain. (default: ``1``)
             discard (int, optional): Discard the first ``discard`` steps in
                 the chain as burn-in. (default: ``0``)
             slice_vals (indexing np.ndarray or slice, optional): This is only available in :class:`eryn.backends.hdfbackend`.
-                If provided, slice the array directly from the HDF5 file with slice = ``slice_vals``. 
-                ``thin`` and ``discard`` will be ignored if slice_vals is not ``None``. 
-                This is particularly useful if files are very large and the user only wants a 
+                If provided, slice the array directly from the HDF5 file with slice = ``slice_vals``.
+                ``thin`` and ``discard`` will be ignored if slice_vals is not ``None``.
+                This is particularly useful if files are very large and the user only wants a
                 small subset of the overall array. (default: ``None``)
 
         Returns:
             dict: nleaves on each branch.
                 The number of leaves on each branch associated with the MCMC samples
                   within each branch.
 
@@ -394,17 +412,17 @@
 
         Args:
             thin (int, optional): Take only every ``thin`` steps from the
                 chain. (default: ``1``)
             discard (int, optional): Discard the first ``discard`` steps in
                 the chain as burn-in. (default: ``0``)
             slice_vals (indexing np.ndarray or slice, optional): This is only available in :class:`eryn.backends.hdfbackend`.
-                If provided, slice the array directly from the HDF5 file with slice = ``slice_vals``. 
-                ``thin`` and ``discard`` will be ignored if slice_vals is not ``None``. 
-                This is particularly useful if files are very large and the user only wants a 
+                If provided, slice the array directly from the HDF5 file with slice = ``slice_vals``.
+                ``thin`` and ``discard`` will be ignored if slice_vals is not ``None``.
+                This is particularly useful if files are very large and the user only wants a
                 small subset of the overall array. (default: ``None``)
 
         Returns:
             double np.ndarray[nsteps, ntemps, nwalkers, nblobs]: The chain of blobs.
 
         """
         return self.get_value("blobs", **kwargs)
@@ -414,17 +432,17 @@
 
         Args:
             thin (int, optional): Take only every ``thin`` steps from the
                 chain. (default: ``1``)
             discard (int, optional): Discard the first ``discard`` steps in
                 the chain as burn-in. (default: ``0``)
             slice_vals (indexing np.ndarray or slice, optional): This is only available in :class:`eryn.backends.hdfbackend`.
-                If provided, slice the array directly from the HDF5 file with slice = ``slice_vals``. 
-                ``thin`` and ``discard`` will be ignored if slice_vals is not ``None``. 
-                This is particularly useful if files are very large and the user only wants a 
+                If provided, slice the array directly from the HDF5 file with slice = ``slice_vals``.
+                ``thin`` and ``discard`` will be ignored if slice_vals is not ``None``.
+                This is particularly useful if files are very large and the user only wants a
                 small subset of the overall array. (default: ``None``)
 
         Returns:
             double np.ndarray[nsteps, ntemps, nwalkers]: The chain of log likelihood values.
 
         """
         return self.get_value("log_like", **kwargs)
@@ -434,17 +452,17 @@
 
         Args:
             thin (int, optional): Take only every ``thin`` steps from the
                 chain. (default: ``1``)
             discard (int, optional): Discard the first ``discard`` steps in
                 the chain as burn-in. (default: ``0``)
             slice_vals (indexing np.ndarray or slice, optional): This is only available in :class:`eryn.backends.hdfbackend`.
-                If provided, slice the array directly from the HDF5 file with slice = ``slice_vals``. 
-                ``thin`` and ``discard`` will be ignored if slice_vals is not ``None``. 
-                This is particularly useful if files are very large and the user only wants a 
+                If provided, slice the array directly from the HDF5 file with slice = ``slice_vals``.
+                ``thin`` and ``discard`` will be ignored if slice_vals is not ``None``.
+                This is particularly useful if files are very large and the user only wants a
                 small subset of the overall array. (default: ``None``)
 
         Returns:
             double np.ndarray[nsteps, ntemps, nwalkers]: The chain of log prior values.
 
         """
         return self.get_value("log_prior", **kwargs)
@@ -456,17 +474,17 @@
             temper (bool, optional): Apply tempering to the posterior values.
                 (default: ``False``)
             thin (int, optional): Take only every ``thin`` steps from the
                 chain. (default: ``1``)
             discard (int, optional): Discard the first ``discard`` steps in
                 the chain as burn-in. (default: ``0``)
             slice_vals (indexing np.ndarray or slice, optional): This is only available in :class:`eryn.backends.hdfbackend`.
-                If provided, slice the array directly from the HDF5 file with slice = ``slice_vals``. 
-                ``thin`` and ``discard`` will be ignored if slice_vals is not ``None``. 
-                This is particularly useful if files are very large and the user only wants a 
+                If provided, slice the array directly from the HDF5 file with slice = ``slice_vals``.
+                ``thin`` and ``discard`` will be ignored if slice_vals is not ``None``.
+                This is particularly useful if files are very large and the user only wants a
                 small subset of the overall array. (default: ``None``)
 
         Returns:
             double np.ndarray[nsteps, ntemps, nwalkers]: The chain of log prior values.
 
         """
         if temper:
@@ -485,17 +503,17 @@
 
         Args:
             thin (int, optional): Take only every ``thin`` steps from the
                 chain. (default: ``1``)
             discard (int, optional): Discard the first ``discard`` steps in
                 the chain as burn-in. (default: ``0``)
             slice_vals (indexing np.ndarray or slice, optional): This is only available in :class:`eryn.backends.hdfbackend`.
-                If provided, slice the array directly from the HDF5 file with slice = ``slice_vals``. 
-                ``thin`` and ``discard`` will be ignored if slice_vals is not ``None``. 
-                This is particularly useful if files are very large and the user only wants a 
+                If provided, slice the array directly from the HDF5 file with slice = ``slice_vals``.
+                ``thin`` and ``discard`` will be ignored if slice_vals is not ``None``.
+                This is particularly useful if files are very large and the user only wants a
                 small subset of the overall array. (default: ``None``)
 
         Returns:
             double np.ndarray[nsteps, ntemps]: The chain of temperatures.
 
 
         """
@@ -587,30 +605,37 @@
                 as 1D double np.ndarrays as values with associated ``branch_names`` as
                 keys.
 
         """
         # stopping index into temperatures
         ind = self.ntemps if all_temps else 1
 
+        if self.ntemps > 1 or self.rj:
+            raise ValueError(
+                "get_autocorr_time is not well-defined for number of temperatures > 1 or when using reversible jump."
+            )
+
         # get chain
         x = self.get_chain(discard=discard, thin=thin)
         x = {name: value[:, :ind] for name, value in x.items()}
 
         out = get_integrated_act(x, **kwargs)
 
         # apply thinning factor if desired
         thin_factor = thin if multiply_thin else 1
 
         return {name: values * thin_factor for name, values in out.items()}
 
-    def get_evidence_estimate(self, discard=0, thin=1, return_error=True, method="therodynamic", **ss_kwargs):
+    def get_evidence_estimate(
+        self, discard=0, thin=1, return_error=True, method="therodynamic", **ss_kwargs
+    ):
         """Get an estimate of the evidence
 
-        This function gets the sample information and uses 
-        :func:`thermodynamic_integration_log_evidence` or 
+        This function gets the sample information and uses
+        :func:`thermodynamic_integration_log_evidence` or
         :func:`stepping_stone_log_evidence` to compute the evidence estimate.
 
         Args:
             discard (int, optional): Discard the first ``discard`` steps in
                 the chain as burn-in. (default: ``0``)
             thin (int, optional): Use only every ``thin`` steps from the
                 chain. The returned estimate is multiplied by ``thin`` so the
@@ -638,95 +663,120 @@
                 kwarg in temperature settings."""
             )
 
         # setup information
         betas = betas_all[0]
 
         # get log evidence and error
-        if method.lower() in ["therodynamic", "thermodynamic integration", "thermo", "ti"]:
+        if method.lower() in [
+            "therodynamic",
+            "thermodynamic integration",
+            "thermo",
+            "ti",
+        ]:
             logls = np.mean(logls_all, axis=(0, -1))
             logZ, dlogZ = thermodynamic_integration_log_evidence(betas, logls)
-        elif method.lower() in ["stepping stone", "ss", "step", "stone", "stepping-stone"]:
+        elif method.lower() in [
+            "stepping stone",
+            "ss",
+            "step",
+            "stone",
+            "stepping-stone",
+        ]:
             logZ, dlogZ = stepping_stone_log_evidence(betas, logls_all, **ss_kwargs)
         else:
             raise ValueError(
-                """Please choose only between 'thermodynamic' and 'stepping-stone' methods.""")
-            
+                """Please choose only between 'thermodynamic' and 'stepping-stone' methods."""
+            )
+
         if return_error:
             return (logZ, dlogZ)
         else:
             return logZ
-        
-    def get_gelman_rubin_convergence_diagnostic(self, discard=0, thin=1, doprint=True, **psrf_kwargs):
+
+    def get_gelman_rubin_convergence_diagnostic(
+        self, discard=0, thin=1, doprint=True, **psrf_kwargs
+    ):
         """
-        The Gelman - Rubin convergence diagnostic. 
-        A general approach to monitoring convergence of MCMC output of multiple walkers. 
-        The function makes a comparison of within-chain and between-chain variances. 
-        A large deviation between these two variances indicates non-convergence, and 
+        The Gelman - Rubin convergence diagnostic.
+        A general approach to monitoring convergence of MCMC output of multiple walkers.
+        The function makes a comparison of within-chain and between-chain variances.
+        A large deviation between these two variances indicates non-convergence, and
         the output [Rhat] deviates from unity.
-        
-        Based on 
-        a. Brooks, SP. and Gelman, A. (1998) General methods for monitoring convergence 
+
+        Based on
+        a. Brooks, SP. and Gelman, A. (1998) General methods for monitoring convergence
         of iterative simulations. Journal of Computational and Graphical Statistics, 7, 434-455
-        b. Gelman, A and Rubin, DB (1992) Inference from iterative simulation using multiple sequences, 
+        b. Gelman, A and Rubin, DB (1992) Inference from iterative simulation using multiple sequences,
         Statistical Science, 7, 457-511.
-        
+
         Args:
-            C (np.ndarray[nwalkers, nsamples, ndim]): The parameter traces. The MCMC chains. 
+            C (np.ndarray[nwalkers, nsamples, ndim]): The parameter traces. The MCMC chains.
             doprint (bool, optional): Flag to print the results on screen.
         discard (int, optional): Discard the first ``discard`` steps in
                 the chain as burn-in. (default: ``0``)
         thin (int, optional): Use only every ``thin`` steps from the
                 chain. The returned estimate is multiplied by ``thin`` so the
                 estimated time is in units of steps, not thinned steps.
                 (default: ``1``)
         doprint (bool, optional): Flag to print a table with the results, per temperature.
 
         Returns
-            dict:   ``Rhat_all_branches``: 
+            dict:   ``Rhat_all_branches``:
                 Returns an estimate of the Gelman-Rubin convergence diagnostic ``Rhat``,
                 per temperature, stored in a dictionary, per branch name.
-        
+
         """
         Rhat_all_branches = dict()
         # Loop over the different models
         for branch in self.branch_names:
-            
-            Rhat = dict() # Initialize
+
+            Rhat = dict()  # Initialize
             # Loop over the temperatures
             for temp in range(self.ntemps):
-                
+
                 # Get all the chains per branch
                 chains = self.get_chain(discard=discard, thin=thin)[branch][:, temp]
-                
+
                 # Handle the cases of multiple leaves on a given branch
                 if chains.shape[2] == 1:
-                    # If no multiple leaves, we squeeze and transpose to the 
+                    # If no multiple leaves, we squeeze and transpose to the
                     # right shape to pass to the psrf function, which is  (nwalkers, nsamples, ndim)
                     chains_in = chains.squeeze().transpose((1, 0, 2))
                 else:
                     # Project onto the model dim all chains [in case of RJ and multiple leaves per branch]
-                    inds = self.get_inds(discard=discard, thin=thin)[branch][:, temp] # [t, w, nleavesmax, dim]
-                    min_leaves = inds.sum(axis=(0,2)).min()
+                    inds = self.get_inds(discard=discard, thin=thin)[branch][
+                        :, temp
+                    ]  # [t, w, nleavesmax, dim]
+                    min_leaves = inds.sum(axis=(0, 2)).min()
                     tmp = [inds[:, w].flatten() for w in range(self.nwalkers)]
-                    keep = [np.where( tmp[w] )[0][:min_leaves] for w in range(len(tmp)) ]
-                    chains_in = np.asarray([chains[:,w].reshape(-1, self.ndims[branch])[keep[w]] for w in range(self.nwalkers)])
-                                
+                    keep = [np.where(tmp[w])[0][:min_leaves] for w in range(len(tmp))]
+                    chains_in = np.asarray(
+                        [
+                            chains[:, w].reshape(-1, self.ndims[branch])[keep[w]]
+                            for w in range(self.nwalkers)
+                        ]
+                    )
+
                 Rhat[temp] = psrf(chains_in, self.ndims[branch], **psrf_kwargs)
-            Rhat_all_branches[branch] = Rhat # Store the Rhat per branch
+            Rhat_all_branches[branch] = Rhat  # Store the Rhat per branch
 
-        if doprint: # Print table of results
+        if doprint:  # Print table of results
             print("  Gelman-Rubin diagnostic \n  <R̂>: Mean value for all parameters\n")
             print("  --------------")
             for branch in self.branch_names:
                 print(" Model: {}".format(branch))
                 print("   T \t <R̂>")
                 print("  --------------")
                 for temp in range(self.ntemps):
-                    print("   {:01d}\t{:3.2f}".format(temp, np.mean(Rhat_all_branches[branch][temp])))
+                    print(
+                        "   {:01d}\t{:3.2f}".format(
+                            temp, np.mean(Rhat_all_branches[branch][temp])
+                        )
+                    )
                 print("\n")
 
         return Rhat_all_branches
 
     @property
     def shape(self):
         """The dimensions of the ensemble
@@ -774,26 +824,29 @@
             key: (self.ntemps, self.nwalkers, self.nleaves_max[key], self.ndims[key])
             for key in self.branch_names
         }
 
         # temperary addition to chains
         a = {
             key: np.empty(
-                (i, self.ntemps, self.nwalkers, self.nleaves_max[key], self.ndims[key]), dtype=self.dtype
+                (i, self.ntemps, self.nwalkers, self.nleaves_max[key], self.ndims[key]),
+                dtype=self.dtype,
             )
             for key in self.branch_names
         }
         # combine with original chain
         self.chain = {
             key: np.concatenate((self.chain[key], a[key]), axis=0) for key in a
         }
 
         # temperorary addition to inds
         a = {
-            key: np.empty((i, self.ntemps, self.nwalkers, self.nleaves_max[key]), dtype=bool)
+            key: np.empty(
+                (i, self.ntemps, self.nwalkers, self.nleaves_max[key]), dtype=bool
+            )
             for key in self.branch_names
         }
         # combine with original inds
         self.inds = {key: np.concatenate((self.inds[key], a[key]), axis=0) for key in a}
 
         # temperorary addition for log likelihood
         a = np.empty((i, self.ntemps, self.nwalkers), dtype=self.dtype)
@@ -817,15 +870,19 @@
             # combine with original blobs
             if self.blobs is None:
                 self.blobs = a
             else:
                 self.blobs = np.concatenate((self.blobs, a), axis=0)
 
     def _check(
-        self, state, accepted, rj_accepted=None, swaps_accepted=None,
+        self,
+        state,
+        accepted,
+        rj_accepted=None,
+        swaps_accepted=None,
     ):
         """Check all the information going in is okay."""
         self._check_blobs(state.blobs)
         self._check_rj_accepted(rj_accepted)
 
         shapes = self.shape
         has_blobs = self.has_blobs()
@@ -854,56 +911,68 @@
                         (ntemp1, nwalker1, nleaves1),
                         key,
                         state.branches[key].inds.shape,
                     )
                 )
 
         # make sure log likelihood, log prior, blobs, accepted, rj_accepted, betas are okay
-        if state.log_like.shape != (ntemps, nwalkers,):
+        if state.log_like.shape != (
+            ntemps,
+            nwalkers,
+        ):
             raise ValueError(
                 "invalid log probability size; expected {0}".format((ntemps, nwalkers))
             )
-        if state.log_prior.shape != (ntemps, nwalkers,):
+        if state.log_prior.shape != (
+            ntemps,
+            nwalkers,
+        ):
             raise ValueError(
                 "invalid log prior size; expected {0}".format((ntemps, nwalkers))
             )
         if state.blobs is not None and not has_blobs:
             raise ValueError("unexpected blobs")
         if state.blobs is None and has_blobs:
             raise ValueError("expected blobs, but none were given")
         if state.blobs is not None and state.blobs.shape[:2] != (ntemps, nwalkers):
             raise ValueError(
                 "invalid blobs size; expected {0}".format((ntemps, nwalkers))
             )
-        if accepted.shape != (ntemps, nwalkers,):
+        if accepted.shape != (
+            ntemps,
+            nwalkers,
+        ):
             raise ValueError(
                 "invalid acceptance size; expected {0}".format((ntemps, nwalkers))
             )
 
         if swaps_accepted is not None and swaps_accepted.shape != (ntemps - 1,):
             raise ValueError(
                 "invalid swaps_accepted size; expected {0}".format(ntemps - 1)
             )
         if self.rj:
-            if rj_accepted.shape != (ntemps, nwalkers,):
+            if rj_accepted.shape != (
+                ntemps,
+                nwalkers,
+            ):
                 raise ValueError(
                     "invalid rj acceptance size; expected {0}".format(
                         (ntemps, nwalkers)
                     )
                 )
 
         if state.betas is not None and state.betas.shape != (ntemps,):
             raise ValueError("invalid beta size; expected {0}".format(ntemps))
 
     def get_move_info(self):
         """Get move information.
-        
+
         Returns:
             dict: Keys are move names and values are dictionaries with information on the moves.
-        
+
         """
         return self.move_info
 
     def save_step(
         self,
         state,
         accepted,
@@ -920,22 +989,25 @@
             rj_accepted (ndarray, optional): An array of the number of accepted steps
                 for the reversible jump proposal for each walker.
                 If :code:`self.rj` is True, then rj_accepted must be an array with
                 :code:`rj_accepted.shape == accepted.shape`. If :code:`self.rj`
                 is False, then rj_accepted must be None, which is the default.
             swaps_accepted (ndarray, optional): 1D array with number of swaps accepted
                 for the in-model step. (default: ``None``)
-            moves_accepted_fraction (dict, optional): Dict of acceptance fraction arrays for all of the 
+            moves_accepted_fraction (dict, optional): Dict of acceptance fraction arrays for all of the
                 moves in the sampler. This dict must have the same keys as ``self.move_keys``.
                 (default: ``None``)
 
         """
         # check to make sure all information in the state is okay
         self._check(
-            state, accepted, rj_accepted=rj_accepted, swaps_accepted=swaps_accepted,
+            state,
+            accepted,
+            rj_accepted=rj_accepted,
+            swaps_accepted=swaps_accepted,
         )
 
         # save the coordinates and inds
         for key, model in state.branches.items():
             self.inds[key][self.iteration] = model.inds
             # use self.store_missing_leaves to set value for missing leaves
             # state retains old coordinates
@@ -968,17 +1040,17 @@
                 raise ValueError(
                     """moves_accepted_fraction was passed, but moves_info was not initialized. Use the moves kwarg 
                     in the reset function."""
                 )
 
             # update acceptance fractions
             for move_key in self.move_keys:
-                self.move_info[move_key]["acceptance_fraction"][
-                    :
-                ] = moves_accepted_fraction[move_key]
+                self.move_info[move_key]["acceptance_fraction"][:] = (
+                    moves_accepted_fraction[move_key]
+                )
 
         self.random_state = state.random_state
         self.iteration += 1
 
     def get_info(self, discard=0, thin=1):
         """Get an output info dictionary
```

### Comparing `Eryn-1.1.6/eryn/backends/hdfbackend.py` & `Eryn-1.1.7/eryn/backends/hdfbackend.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/ensemble.py` & `Eryn-1.1.7/eryn/ensemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,15 +480,17 @@
             self.backend = HDFBackend(backend)
         else:
             self.backend = backend
 
         self.info = info
 
         all_moves_tmp = list(
-            tuple(self.moves) if not self.has_reversible_jump else tuple(self.moves) + tuple(self.rj_moves)
+            tuple(self.moves)
+            if not self.has_reversible_jump
+            else tuple(self.moves) + tuple(self.rj_moves)
         )
 
         self.all_moves = {}
         if self.track_moves:
             current_indices_move_keys = {}
             for move in all_moves_tmp:
                 # get out of tuple if weights are given
@@ -786,15 +788,19 @@
         if iterations is None and store:
             raise ValueError("'store' must be False when 'iterations' is None")
 
         # Interpret the input as a walker state and check the dimensions.
 
         # initial_state.__class__ rather than State in case it is a subclass
         # of State
-        if hasattr(initial_state, "__class__") and issubclass(initial_state.__class__, State) and not isinstance(initial_state.__class__, State):
+        if (
+            hasattr(initial_state, "__class__")
+            and issubclass(initial_state.__class__, State)
+            and not isinstance(initial_state.__class__, State)
+        ):
             state = initial_state.__class__(initial_state, copy=True)
         else:
             state = State(initial_state, copy=True)
 
         # Check the backend shape
         for i, (name, branch) in enumerate(state.branches.items()):
             ntemps_, nwalkers_, nleaves_, ndim_ = branch.shape
@@ -839,15 +845,17 @@
                 raise ValueError(
                     "Input state has inverse temperatures (betas), but not the correct number of temperatures according to sampler inputs."
                 )
 
             self.temperature_control.betas = state.betas.copy()
 
         else:
-            if hasattr(self, "temperature_control") and hasattr(self.temperature_control, "betas"):
+            if hasattr(self, "temperature_control") and hasattr(
+                self.temperature_control, "betas"
+            ):
                 state.betas = self.temperature_control.betas.copy()
 
         if np.shape(state.log_like) != (self.ntemps, self.nwalkers):
             raise ValueError("incompatible input dimensions")
         if np.shape(state.log_prior) != (self.ntemps, self.nwalkers):
             raise ValueError("incompatible input dimensions")
 
@@ -1043,15 +1051,15 @@
             ):
                 stop = self.stopping_fn(i, results, self)
 
                 if stop:
                     break
 
             i += 1
-            
+
         # Store so that the ``initial_state=None`` case will work
         self._previous_state = results
 
         return results
 
     def compute_log_prior(self, coords, inds=None, supps=None, branch_supps=None):
         """Calculate the vector of log-prior for the walkers
@@ -1083,15 +1091,17 @@
             }
 
         # take information out of dict and spread to x1..xn
         x_in = {}
 
         # for completely customizable priors
         if "all_models_together" in self.priors:
-            prior_out = self.priors["all_models_together"].logpdf(coords, inds, supps=supps, branch_supps=branch_supps)
+            prior_out = self.priors["all_models_together"].logpdf(
+                coords, inds, supps=supps, branch_supps=branch_supps
+            )
             assert prior_out.shape == (ntemps, nwalkers)
 
         elif self.provide_groups:
             # get group information from the inds dict
             groups = groups_from_inds(inds)
 
             # get the coordinates that are used
@@ -1184,15 +1194,17 @@
                 raise ValueError("At least one parameter value was infinite")
             if np.any(np.isnan(ptemp[inds[name]])):
                 raise ValueError("At least one parameter value was NaN")
 
         # if no prior values are added, compute_prior
         # this is necessary to ensure Likelihood is not evaluated outside of the prior
         if logp is None:
-            logp = self.compute_log_prior(coords, inds=inds, supps=supps, branch_supps=branch_supps)
+            logp = self.compute_log_prior(
+                coords, inds=inds, supps=supps, branch_supps=branch_supps
+            )
 
         # if all points are outside the prior
         if np.all(np.isinf(logp)):
             warnings.warn(
                 "All points input for the Likelihood have a log prior of -inf."
             )
             return np.full_like(logp, -1e300), None
@@ -1373,17 +1385,17 @@
                                 # make sure there is a dictionary ready in this kwarg dictionary
                                 if "branch_supps" not in kwarg_i:
                                     kwarg_i["branch_supps"] = {}
 
                                 # fill these branch supplimentals for the specific group
                                 if branch_supps_in[branch_name_i] is not None:
                                     # get list of branch_supps values
-                                    kwarg_i["branch_supps"][
-                                        branch_name_i
-                                    ] = branch_supps_in[branch_name_i][inds_keep]
+                                    kwarg_i["branch_supps"][branch_name_i] = (
+                                        branch_supps_in[branch_name_i][inds_keep]
+                                    )
                                 else:
                                     kwarg_i["branch_supps"][branch_name_i] = None
 
                 # if only one model type, will take out of groups
                 add_term = arg_i[0] if len(groups_in) == 1 else arg_i
 
                 # based on how this is dealth with in the _FunctionWrapper
@@ -1473,26 +1485,18 @@
         if self.has_reversible_jump:
             return self.backend.rj_accepted / float(self.backend.iteration)
         else:
             return None
 
     @property
     def swap_acceptance_fraction(self):
-        """The fraction of proposed steps that were accepted"""
-        # print(self.backend.iteration) # np.sum(self.backend.accepted)
-        return self.backend.swaps_accepted / float(self.backend.iteration)
-
-    @property
-    def rj_swap_acceptance_fraction(self):
-        """The fraction of proposed reversible jump steps that were accepted"""
-        if self.has_reversible_jump:
-            # print(self.backend.iteration, np.sum(self.backend.rj_accepted))
-            return self.backend.rj_swaps_accepted / float(self.backend.iteration)
-        else:
-            return None
+        """The fraction of proposed temperature swaps that were accepted"""
+        return self.backend.swaps_accepted / float(
+            self.backend.iteration * self.nwalkers
+        )
 
     def get_chain(self, **kwargs):
         return self.get_value("chain", **kwargs)
 
     get_chain.__doc__ = Backend.get_chain.__doc__
 
     def get_blobs(self, **kwargs):
```

### Comparing `Eryn-1.1.6/eryn/moves/__init__.py` & `Eryn-1.1.7/eryn/moves/__init__.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/moves/combine.py` & `Eryn-1.1.7/eryn/moves/combine.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/moves/delayedrejection.py` & `Eryn-1.1.7/eryn/moves/delayedrejection.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/moves/distgen.py` & `Eryn-1.1.7/eryn/moves/distgen.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/moves/distgenrj.py` & `Eryn-1.1.7/eryn/moves/distgenrj.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/moves/gaussian.py` & `Eryn-1.1.7/eryn/moves/gaussian.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,22 +107,28 @@
             # put into coords in proper location
             q[name][inds_here] = new_coords.copy()
 
         # handle periodic parameters
         if self.periodic is not None:
             q = self.periodic.wrap(
                 {
-                    name: tmp.reshape(ntemps * nwalkers, nleaves_max, ndim)
+                    name: tmp.reshape((ntemps * nwalkers,) + tmp.shape[-2:])
                     for name, tmp in q.items()
                 },
                 xp=self.xp,
             )
 
             q = {
-                name: tmp.reshape(ntemps, nwalkers, nleaves_max, ndim)
+                name: tmp.reshape(
+                    (
+                        ntemps,
+                        nwalkers,
+                    )
+                    + tmp.shape[-2:]
+                )
                 for name, tmp in q.items()
             }
 
         return q, np.zeros((ntemps, nwalkers))
 
 
 class _isotropic_proposal(object):
```

### Comparing `Eryn-1.1.6/eryn/moves/group.py` & `Eryn-1.1.7/eryn/moves/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,79 +11,75 @@
 __all__ = ["GroupMove"]
 
 
 class GroupMove(Move, ABC):
     """
     A "group" ensemble move based on the :class:`eryn.moves.RedBlueMove`.
 
-    In moves like the :class:`eryn.moves.StretchMove`, the complimentary 
-    group for which the proposal is used is chosen from the current points in 
+    In moves like the :class:`eryn.moves.StretchMove`, the complimentary
+    group for which the proposal is used is chosen from the current points in
     the ensemble. In "group" moves the complimentary group is a stationary group
-    that is updated every `n_iter_update` iterations. This update is performed with the 
+    that is updated every `n_iter_update` iterations. This update is performed with the
     last set of coordinates to maintain detailed balance.
 
     Args:
         nfriends (int, optional): The number of friends to draw from as the complimentary
-            ensemble. This group is determined from the stationary group. If ``None``, it will  
+            ensemble. This group is determined from the stationary group. If ``None``, it will
             be set to the number of walkers. (default: ``None``)
-        n_iter_update (int, optional): Number of iterations to run before updating the 
-            stationary distribution. (default: 100). 
+        n_iter_update (int, optional): Number of iterations to run before updating the
+            stationary distribution. (default: 100).
         live_dangerously (bool, optional): If ``True``, allow for ``n_iter_update == 1``.
             (deafault: ``False``)
 
     ``kwargs`` are passed to :class:`Move` class.
 
     """
 
     def __init__(
-        self,
-        nfriends=None,
-        n_iter_update=100,
-        live_dangerously=False,
-        **kwargs
+        self, nfriends=None, n_iter_update=100, live_dangerously=False, **kwargs
     ):
 
         Move.__init__(self, **kwargs)
         self.nfriends = int(nfriends)
         self.n_iter_update = n_iter_update
 
         if self.n_iter_update <= 1 and not live_dangerously:
             raise ValueError("n_iter_update must be greather than or equal to 2.")
 
         self.iter = 0
 
     def find_friends(self, name, s, s_inds=None):
         """Function for finding friends.
-        
+
         Args:
             name (str): Branch name for proposal coordinates.
             s (np.ndarray): Coordinates array for the points to be moved.
             s_inds (np.ndarray, optional): ``inds`` arrays that represent which leaves are present.
                 (default: ``None``)
 
         Return:
-            np.ndarray: Complimentary values. 
-        
+            np.ndarray: Complimentary values.
+
         """
         raise NotImplementedError
 
     def choose_c_vals(self, name, s, s_inds=None):
         """Get the complimentary values."""
         return self.find_friends(name, s, s_inds=s_inds)
 
     def setup(self, branches):
         """Any setup necessary for the proposal"""
         pass
 
     def setup_friends(self, branches):
         """Setup anything for finding friends.
-        
+
         Args:
             branches (dict): Dictionary with all the current branches in the sampler.
-        
+
         """
         raise NotImplementedError
 
     @classmethod
     def get_proposal(self, s_all, random, gibbs_ndim=None, s_inds_all=None, **kwargs):
         """Generate group stretch proposal coordinates
 
@@ -91,15 +87,15 @@
             s_all (dict): Keys are ``branch_names`` and values are coordinates
                 for which a proposal is to be generated.
             random (object): Random state object.
             gibbs_ndim (int or np.ndarray, optional): If Gibbs sampling, this indicates
                 the true dimension. If given as an array, must have shape ``(ntemps, nwalkers)``.
                 See the tutorial for more information.
                 (default: ``None``)
-            s_inds_all (dict, optional): Keys are ``branch_names`` and values are 
+            s_inds_all (dict, optional): Keys are ``branch_names`` and values are
                 ``inds`` arrays indicating which leaves are currently used. (default: ``None``)
 
         Returns:
             tuple: First entry is new positions. Second entry is detailed balance factors.
 
         Raises:
             ValueError: Issues with dimensionality.
@@ -143,15 +139,15 @@
 
         # Split the ensemble in half and iterate over these two halves.
         accepted = np.zeros((ntemps, nwalkers), dtype=bool)
 
         all_branch_names = list(state.branches.keys())
 
         # get gibbs sampling information
-        for (branch_names_run, inds_run) in self.gibbs_sampling_setup_iterator(
+        for branch_names_run, inds_run in self.gibbs_sampling_setup_iterator(
             all_branch_names
         ):
 
             if not np.all(
                 np.asarray(list(state.branches_supplimental.values())) == None
             ):
                 new_branch_supps = deepcopy(state.branches_supplimental)
@@ -185,19 +181,24 @@
                     # nleaves * ndim
                     gibbs_ndim += np.prod(state.branches[brn].shape[-2:])
 
             self.current_model = model
             self.current_state = state
             # Get the move-specific proposal.
             q, factors = self.get_proposal(
-                coords_going_for_proposal, model.random, gibbs_ndim=gibbs_ndim, s_inds_all=inds_going_for_proposal
+                coords_going_for_proposal,
+                model.random,
+                gibbs_ndim=gibbs_ndim,
+                s_inds_all=inds_going_for_proposal,
             )
 
             # account for gibbs sampling
-            self.cleanup_proposals_gibbs(branch_names_run, inds_run, q, state.branches_coords)
+            self.cleanup_proposals_gibbs(
+                branch_names_run, inds_run, q, state.branches_coords
+            )
 
             # Compute prior of the proposed position
             # new_inds_prior is adjusted if product-space is used
             logp = model.compute_log_prior_fn(q, inds=state.branches_inds)
 
             self.fix_logp_gibbs(branch_names_run, inds_run, logp, state.branches_inds)
 
@@ -247,9 +248,9 @@
             state = self.temperature_control.temper_comps(state)
 
         if self.iter != 0 and self.iter % self.n_iter_update == 0:
             # use old values to maintain detailed balance when updating
             # nfriends
             self.setup_friends(old_branches)
 
+        self.iter += 1
         return state, accepted
-
```

### Comparing `Eryn-1.1.6/eryn/moves/groupstretch.py` & `Eryn-1.1.7/eryn/moves/groupstretch.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/moves/mh.py` & `Eryn-1.1.7/eryn/moves/mh.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/moves/move.py` & `Eryn-1.1.7/eryn/moves/move.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/moves/mtdistgen.py` & `Eryn-1.1.7/eryn/moves/mtdistgen.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/moves/mtdistgenrj.py` & `Eryn-1.1.7/eryn/moves/mtdistgenrj.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/moves/multipletry.py` & `Eryn-1.1.7/eryn/moves/multipletry.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import warnings
 from copy import deepcopy
 from abc import ABC
 
 # from scipy.special import logsumexp
 
 try:
-    import cupy as xp
+    import cupy as cp
 
     gpu_available = True
 except (ModuleNotFoundError, ImportError):
-    import numpy as xp
+    import numpy as cp
 
     gpu_available = False
 
 from .rj import ReversibleJumpMove
 from ..prior import ProbDistContainer
 from ..utils.utility import groups_from_inds
 
@@ -28,14 +28,15 @@
 
     max = xp.max(a, axis=axis)
     ds = a - max[:, None]
 
     sum_of_exp = xp.exp(ds).sum(axis=axis)
     return max + xp.log(sum_of_exp)
 
+
 def get_mt_computations(logP, log_proposal_pdf, symmetric=False, xp=None):
 
     if xp is None:
         xp = np
 
         # set weights based on if symmetric
     if symmetric:
@@ -49,157 +50,162 @@
     # probs = wi / sum(wi)
     log_of_probs = log_importance_weights - log_sum_weights[:, None]
 
     # probabilities to choose try
     probs = xp.exp(log_of_probs)
 
     # draw based on likelihood
-    inds_keep = (
-        probs.cumsum(1) > xp.random.rand(probs.shape[0])[:, None]
-    ).argmax(1)
+    inds_keep = (probs.cumsum(1) > xp.random.rand(probs.shape[0])[:, None]).argmax(1)
 
     return log_importance_weights, log_sum_weights, inds_keep
 
 
 class MultipleTryMove(ABC):
     """Generate multiple proposal tries.
 
-    This class should be inherited by another proposal class 
+    This class should be inherited by another proposal class
     with the ``@classmethods`` overwritten. See :class:`eryn.moves.MTDistGenMove`
     and :class:`MTDistGenRJ` for examples.
 
     Args:
         num_try (int, optional): Number of tries. (default: 1)
-        independent (bool, optional): Set to ``True`` if the proposal is independent of the current points. 
-            (default: ``False``). 
-        symmetric (bool, optional): Set to ``True`` if the proposal is symmetric. 
-            (default: ``False``). 
-        rj (bool, optional): Set to ``True`` if this is a nested reversible jump proposal. 
-            (default: ``False``). 
+        independent (bool, optional): Set to ``True`` if the proposal is independent of the current points.
+            (default: ``False``).
+        symmetric (bool, optional): Set to ``True`` if the proposal is symmetric.
+            (default: ``False``).
+        rj (bool, optional): Set to ``True`` if this is a nested reversible jump proposal.
+            (default: ``False``).
         **kwargs (dict, optional): for compatibility with other proposals.
 
         Raises:
-            ValueError: Input issues. 
-        
+            ValueError: Input issues.
+
     """
 
     def __init__(
-        self, num_try=1, independent=False, symmetric=False, rj=False, xp=None, **kwargs
+        self,
+        num_try=1,
+        independent=False,
+        symmetric=False,
+        rj=False,
+        use_gpu=None,
+        **kwargs
     ):
-        # TODO: add in xp
         self.num_try = num_try
 
         self.independent = independent
         self.symmetric = symmetric
         self.rj = rj
 
         if self.rj:
             if self.symmetric or self.independent:
                 raise ValueError(
                     "If rj==True, symmetric and independt must both be False."
                 )
 
-        if xp is None:
-            xp = np
+        self.use_gpu = use_gpu
 
-        self.xp = xp
+    @property
+    def xp(self):
+        xp = cp if self.use_gpu else np
+        return xp
 
     @classmethod
     def special_like_func(self, generated_coords, *args, inds_leaves_rj=None, **kwargs):
         """Calculate the Likelihood for sampled points.
-        
+
         Args:
-            generated_coords (np.ndarray): Generated coordinates with shape ``(number of independent walkers, num_try)``. 
-            *args (tuple, optional): additional arguments passed by overwriting the 
+            generated_coords (np.ndarray): Generated coordinates with shape ``(number of independent walkers, num_try)``.
+            *args (tuple, optional): additional arguments passed by overwriting the
                 ``get_proposal`` function and passing ``args_like`` keyword argument.
             inds_leaves_rj (np.ndarray): Index into each individual walker giving the
                 leaf index associated with this proposal. Should only be used if ``self.rj is True``. (default: ``None``)
-            **kwargs (tuple, optional): additional keyword arguments passed by overwriting the 
+            **kwargs (tuple, optional): additional keyword arguments passed by overwriting the
                 ``get_proposal`` function and passing ``kwargs_like`` keyword argument.
 
         Returns:
             np.ndarray: Likelihood values with shape ``(generated_coords.shape[0], num_try).``
 
         Raises:
-            NotImplementedError: Function not included. 
-        
+            NotImplementedError: Function not included.
+
         """
         raise NotImplementedError
 
     @classmethod
     def special_prior_func(self, generated_coords, *args, **kwargs):
         """Calculate the Prior for sampled points.
-        
+
         Args:
-            generated_coords (np.ndarray): Generated coordinates with shape ``(number of independent walkers, num_try)``. 
-            *args (tuple, optional): additional arguments passed by overwriting the 
+            generated_coords (np.ndarray): Generated coordinates with shape ``(number of independent walkers, num_try)``.
+            *args (tuple, optional): additional arguments passed by overwriting the
                 ``get_proposal`` function and passing ``args_prior`` keyword argument.
             inds_leaves_rj (np.ndarray): Index into each individual walker giving the
                 leaf index associated with this proposal. Should only be used if ``self.rj is True``. (default: ``None``)
-            **kwargs (tuple, optional): additional keyword arguments passed by overwriting the 
+            **kwargs (tuple, optional): additional keyword arguments passed by overwriting the
                 ``get_proposal`` function and passing ``kwargs_prior`` keyword argument.
 
         Returns:
             np.ndarray: Prior values with shape ``(generated_coords.shape[0], num_try).``
 
         Raises:
-            NotImplementedError: Function not included. 
-        
+            NotImplementedError: Function not included.
+
         """
         raise NotImplementedError
 
     @classmethod
     def special_generate_func(
         coords, random, size=1, *args, fill_tuple=None, fill_values=None, **kwargs
     ):
         """Generate samples and calculate the logpdf of their proposal function.
-        
+
         Args:
-            coords (np.ndarray): Current coordinates of walkers. 
+            coords (np.ndarray): Current coordinates of walkers.
             random (obj): Random generator.
-            *args (tuple, optional): additional arguments passed by overwriting the 
+            *args (tuple, optional): additional arguments passed by overwriting the
                 ``get_proposal`` function and passing ``args_generate`` keyword argument.
-            size (int, optional): Number of tries to generate. 
+            size (int, optional): Number of tries to generate.
             fill_tuple (tuple, optional): Length 2 tuple with the indexing of which values to fill
-                when generating. Can be used for auxillary proposals or reverse RJ proposals. First index is the index into walkers and the second index is 
+                when generating. Can be used for auxillary proposals or reverse RJ proposals. First index is the index into walkers and the second index is
                 the index into the number of tries. (default: ``None``)
-            fill_values (np.ndarray): values to fill associated with ``fill_tuple``. Should 
+            fill_values (np.ndarray): values to fill associated with ``fill_tuple``. Should
                 have size ``(len(fill_tuple[0]), ndim)``. (default: ``None``).
-            **kwargs (tuple, optional): additional keyword arguments passed by overwriting the 
+            **kwargs (tuple, optional): additional keyword arguments passed by overwriting the
                 ``get_proposal`` function and passing ``kwargs_generate`` keyword argument.
 
         Returns:
             tuple: (generated points, logpdf of generated points).
 
         Raises:
-            NotImplementedError: Function not included. 
-        
+            NotImplementedError: Function not included.
+
         """
         raise NotImplementedError
 
     @classmethod
     def special_generate_logpdf(self, coords):
         """Get logpdf of generated coordinates.
-        
+
         Args:
-            coords (np.ndarray): Current coordinates of walkers. 
-            
+            coords (np.ndarray): Current coordinates of walkers.
+
         Returns:
             np.ndarray: logpdf of generated points.
-        
+
         Raises:
-            NotImplementedError: Function not included. 
+            NotImplementedError: Function not included.
         """
         raise NotImplementedError
 
     def get_mt_log_posterior(self, ll, lp, betas=None):
         """Calculate the log of the posterior for all tries.
 
         Args:
-            ll (np.ndarray): Log Likelihood values with shape ``(nwalkers, num_tries)``. 
+            ll (np.ndarray): Log Likelihood values with shape ``(nwalkers, num_tries)``.
             lp (np.ndarray): Log Prior values with shape ``(nwalkers, num_tries)``.
             betas (np.ndarray, optional): Inverse temperatures to include in log Posterior computation.
                 (default: ``None``)
 
         Returns:
             np.ndarray: Log of the Posterior with shape ``(nwalkers, num_tries)``.
 
@@ -214,22 +220,22 @@
                 betas_tmp = betas
             ll_temp = betas_tmp * ll
 
         return ll_temp + lp
 
     def readout_adjustment(self, out_vals, all_vals_prop, aux_all_vals):
         """Read out values from the proposal.
-        
-        Allows the user to read out any values from the proposal that may be needed elsewhere. This function must be overwritten. 
-        
+
+        Allows the user to read out any values from the proposal that may be needed elsewhere. This function must be overwritten.
+
         Args:
-            out_vals (list): ``[logP_out, ll_out, lp_out, log_proposal_pdf_out, log_sum_weights]``. 
+            out_vals (list): ``[logP_out, ll_out, lp_out, log_proposal_pdf_out, log_sum_weights]``.
             all_vals_prop (list): ``[logP, ll, lp, log_proposal_pdf, log_sum_weights]``.
             aux_all_vals (list): ``[aux_logP, aux_ll, aux_lp, aux_log_proposal_pdf, aux_log_sum_weights]``.
-        
+
         """
         pass
 
     def get_mt_proposal(
         self,
         coords,
         random,
@@ -247,56 +253,56 @@
     ):
         """Make a multiple-try proposal
 
         Here, ``nwalkers`` refers to all independent walkers which generally
         will mean ``nwalkers * ntemps`` in terms of the rest of the sampler.
 
         Args:
-            coords (np.ndarray): Current coordinates of walkers. 
+            coords (np.ndarray): Current coordinates of walkers.
             random (obj): Random generator.
-            args_generate (tuple, optional): Additional ``*args`` to pass to generate function. 
-                Must overwrite ``get_proposal`` function to use these. 
+            args_generate (tuple, optional): Additional ``*args`` to pass to generate function.
+                Must overwrite ``get_proposal`` function to use these.
                 (default: ``()``)
-            kwargs_generate (dict, optional): Additional ``**kwargs`` to pass to generate function. 
+            kwargs_generate (dict, optional): Additional ``**kwargs`` to pass to generate function.
                 (default: ``{}``)
                 Must overwrite ``get_proposal`` function to use these.
-            args_like (tuple, optional): Additional ``*args`` to pass to Likelihood function. 
-                Must overwrite ``get_proposal`` function to use these. 
+            args_like (tuple, optional): Additional ``*args`` to pass to Likelihood function.
+                Must overwrite ``get_proposal`` function to use these.
                 (default: ``()``)
-            kwargs_like (dict, optional): Additional ``**kwargs`` to pass to Likelihood function. 
-                Must overwrite ``get_proposal`` function to use these. 
+            kwargs_like (dict, optional): Additional ``**kwargs`` to pass to Likelihood function.
+                Must overwrite ``get_proposal`` function to use these.
                 (default: ``{}``)
-            args_prior (tuple, optional): Additional ``*args`` to pass to Prior function. 
-                Must overwrite ``get_proposal`` function to use these. 
+            args_prior (tuple, optional): Additional ``*args`` to pass to Prior function.
+                Must overwrite ``get_proposal`` function to use these.
                 (default: ``()``)
-            kwargs_prior (dict, optional): Additional ``**kwargs`` to pass to Prior function. 
-                Must overwrite ``get_proposal`` function to use these. 
+            kwargs_prior (dict, optional): Additional ``**kwargs`` to pass to Prior function.
+                Must overwrite ``get_proposal`` function to use these.
                 (default: ``{}``)
-            betas (np.ndarray, optional): Inverse temperatures passes to the proposal with shape ``(nwalkers,)``. 
-            ll_in (np.ndarray, optional): Log Likelihood values coming in for current coordinates. Must be provided 
-                if ``self.rj is True``. If ``self.rj is True``, must be nested. 
-                Also, for all proposed removals, this value must be the Likelihood with the binary 
+            betas (np.ndarray, optional): Inverse temperatures passes to the proposal with shape ``(nwalkers,)``.
+            ll_in (np.ndarray, optional): Log Likelihood values coming in for current coordinates. Must be provided
+                if ``self.rj is True``. If ``self.rj is True``, must be nested.
+                Also, for all proposed removals, this value must be the Likelihood with the binary
                 removed so all proposals are pretending to add a binary.
                 Useful if ``self.independent is True``. (default: ``None``)
-            lp_in (np.ndarray, optional): Log Prior values coming in for current coordinates. Must be provided 
-                if ``self.rj is True``. If ``self.rj is True``, must be nested. 
-                Also, for all proposed removals, this value must be the Likelihood with the binary 
+            lp_in (np.ndarray, optional): Log Prior values coming in for current coordinates. Must be provided
+                if ``self.rj is True``. If ``self.rj is True``, must be nested.
+                Also, for all proposed removals, this value must be the Likelihood with the binary
                 removed so all proposals are pretending to add a binary.
                 Useful if ``self.independent is True``. (default: ``None``)
-            inds_leaves_rj (np.ndarray, optional): Array giving the leaf index of each incoming walker. 
+            inds_leaves_rj (np.ndarray, optional): Array giving the leaf index of each incoming walker.
                 Must be provided if ``self.rj is True``. (default: ``None``)
-            inds_reverse_rj (np.ndarray, optional): Array giving the walker index for which proposals are 
-                reverse proposal removing a leaf. 
+            inds_reverse_rj (np.ndarray, optional): Array giving the walker index for which proposals are
+                reverse proposal removing a leaf.
                 Must be provided if ``self.rj is True``. (default: ``None``)
 
         Returns:
             tuple: (generated points, factors).
 
         Raises:
-            ValueError: Inputs are incorrect. 
+            ValueError: Inputs are incorrect.
 
         """
 
         # check if rj and make sure we have all the information in that case
         if self.rj:
             try:
                 assert ll_in is not None and lp_in is not None
@@ -343,15 +349,17 @@
         # this will properly cancel the prior with the proposal for leaves that already exists
         if self.rj:
             log_proposal_pdf += lp_in[:, None]
 
         # get posterior distribution including tempering
         logP = self.get_mt_log_posterior(ll, lp, betas=betas)
 
-        log_importance_weights, log_sum_weights, inds_keep = get_mt_computations(logP, log_proposal_pdf, symmetric=self.symmetric, xp=self.xp)
+        log_importance_weights, log_sum_weights, inds_keep = get_mt_computations(
+            logP, log_proposal_pdf, symmetric=self.symmetric, xp=self.xp
+        )
 
         # tuple of index arrays of which try chosen per walker
         inds_tuple = (self.xp.arange(len(inds_keep)), inds_keep)
 
         if self.rj:
             # this just ensures the cancellation of logP and aux_logP outside of proposal
             inds_tuple[1][inds_reverse_rj] = 0
@@ -584,29 +592,35 @@
             {key_in: generated_points.reshape(ntemps, nwalkers, 1, -1)},
             factors.reshape(ntemps, nwalkers),
         )
 
 
 class MultipleTryMoveRJ(MultipleTryMove):
     def get_proposal(
-        self, branches_coords, branches_inds, nleaves_min_all, nleaves_max_all, random, **kwargs
+        self,
+        branches_coords,
+        branches_inds,
+        nleaves_min_all,
+        nleaves_max_all,
+        random,
+        **kwargs
     ):
         """Make a proposal
 
         Args:
             all_coords (dict): Keys are ``branch_names``. Values are
                 np.ndarray[ntemps, nwalkers, nleaves_max, ndim]. These are the curent
                 coordinates for all the walkers.
             all_inds (dict): Keys are ``branch_names``. Values are
                 np.ndarray[ntemps, nwalkers, nleaves_max]. These are the boolean
                 arrays marking which leaves are currently used within each walker.
-            nleaves_min_all (list): Minimum values of leaf ount for each model. Must have same order as ``all_cords``. 
-            nleaves_max_all (list): Maximum values of leaf ount for each model. Must have same order as ``all_cords``. 
+            nleaves_min_all (list): Minimum values of leaf ount for each model. Must have same order as ``all_cords``.
+            nleaves_max_all (list): Maximum values of leaf ount for each model. Must have same order as ``all_cords``.
             random (object): Current random state of the sampler.
-            **kwargs (ignored): For modularity. 
+            **kwargs (ignored): For modularity.
 
         Returns:
             tuple: Tuple containing proposal information.
                 First entry is the new coordinates as a dictionary with keys
                 as ``branch_names`` and values as
                 ``double `` np.ndarray[ntemps, nwalkers, nleaves_max, ndim] containing
                 proposed coordinates. Second entry is the new ``inds`` array with
@@ -683,54 +697,59 @@
             # adjust indices
             new_inds[key_in][(temp_inds, walker_inds, leaf_inds)] = new_val
 
             if change == "-1":
                 # which walkers are removing
                 inds_reverse_rj = temp_inds * nwalkers + walker_inds
 
-        # setup reversal coords and inds
-        # need to determine Likelihood and prior of removed binaries.
-        # this goes into the multiple try proposal as previous ll and lp
-        temp_reverse_coords = {}
-        temp_reverse_inds = {}
-
-        for key in self.current_state.branches:
-            (
-                ntemps_tmp,
-                nwalkers_tmp,
-                nleaves_max_tmp,
-                ndim_tmp,
-            ) = self.current_state.branches[key].shape
-
-            # coords from reversal
-            temp_reverse_coords[key] = self.current_state.branches[key].coords.reshape(
-                ntemps_tmp * nwalkers_tmp, nleaves_max_tmp, ndim_tmp
-            )[inds_reverse_rj][None, :]
-
-            # which inds array to use
-            inds_tmp_here = (
-                new_inds[key]
-                if key == key_in
-                else self.current_state.branches[key].inds
-            )
-            temp_reverse_inds[key] = inds_tmp_here.reshape(
-                ntemps * nwalkers, nleaves_max_tmp
-            )[inds_reverse_rj][None, :]
-
-        # calculate information for the reverse
-        lp_reverse_here = self.current_model.compute_log_prior_fn(
-            temp_reverse_coords, inds=temp_reverse_inds
-        )[0]
-        ll_reverse_here = self.current_model.compute_log_like_fn(
-            temp_reverse_coords, inds=temp_reverse_inds, logp=lp_here
-        )[0]
-
-        # fill the here values
-        ll_here[inds_reverse_rj] = ll_reverse_here
-        lp_here[inds_reverse_rj] = lp_reverse_here
+        if inds_reverse_rj is not None:
+            # setup reversal coords and inds
+            # need to determine Likelihood and prior of removed binaries.
+            # this goes into the multiple try proposal as previous ll and lp
+            temp_reverse_coords = {}
+            temp_reverse_inds = {}
+
+            for key in self.current_state.branches:
+                (
+                    ntemps_tmp,
+                    nwalkers_tmp,
+                    nleaves_max_tmp,
+                    ndim_tmp,
+                ) = self.current_state.branches[key].shape
+
+                # coords from reversal
+                temp_reverse_coords[key] = self.current_state.branches[
+                    key
+                ].coords.reshape(ntemps_tmp * nwalkers_tmp, nleaves_max_tmp, ndim_tmp)[
+                    inds_reverse_rj
+                ][
+                    None, :
+                ]
+
+                # which inds array to use
+                inds_tmp_here = (
+                    new_inds[key]
+                    if key == key_in
+                    else self.current_state.branches[key].inds
+                )
+                temp_reverse_inds[key] = inds_tmp_here.reshape(
+                    ntemps * nwalkers, nleaves_max_tmp
+                )[inds_reverse_rj][None, :]
+
+            # calculate information for the reverse
+            lp_reverse_here = self.current_model.compute_log_prior_fn(
+                temp_reverse_coords, inds=temp_reverse_inds
+            )[0]
+            ll_reverse_here = self.current_model.compute_log_like_fn(
+                temp_reverse_coords, inds=temp_reverse_inds, logp=lp_here
+            )[0]
+
+            # fill the here values
+            ll_here[inds_reverse_rj] = ll_reverse_here
+            lp_here[inds_reverse_rj] = lp_reverse_here
 
         # get mt proposal
         generated_points, factors = self.get_mt_proposal(
             coords_in,
             random,
             betas=betas_here,
             ll_in=ll_here,
```

### Comparing `Eryn-1.1.6/eryn/moves/red_blue.py` & `Eryn-1.1.7/eryn/moves/red_blue.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/moves/rj.py` & `Eryn-1.1.7/eryn/moves/rj.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/moves/stretch.py` & `Eryn-1.1.7/eryn/moves/stretch.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/moves/tempering.py` & `Eryn-1.1.7/eryn/moves/tempering.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/pbar.py` & `Eryn-1.1.7/eryn/pbar.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/prior.py` & `Eryn-1.1.7/eryn/prior.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/state.py` & `Eryn-1.1.7/eryn/state.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/utils/periodic.py` & `Eryn-1.1.7/eryn/utils/periodic.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
         Args:
             p1 (dict): If dict, keys are ``branch_names``
                 and values are positions with parameters along the final dimension.
             p2 (dict): If dict, keys are ``branch_names``
                 and values are positions with parameters along the final dimension.
             xp (object, optional): ``numpy`` or ``cupy``. If ``None``, use ``numpy``.
-                (default: ``None``) 
+                (default: ``None``)
 
         Returns:
             dict: Distances accounting for periodicity.
                     Keys are branch names and values are distance arrays.
 
         """
 
@@ -54,21 +54,27 @@
         assert list(p1.keys()) == list(p2.keys())
 
         names = list(p1.keys())
 
         # prepare output
         out_diff = {}
         for key in names:
-            # get period info
-            periods = xp.asarray(self.periods[key])
-            inds_periodic = xp.asarray(self.inds_periodic[key])
 
             # get basic distance
             diff = p2[key] - p1[key]
 
+            # no periodic parameters for this key
+            if key not in self.periods:
+                out_diff[key] = diff
+                continue
+
+            # get period info
+            periods = xp.asarray(self.periods[key])
+            inds_periodic = xp.asarray(self.inds_periodic[key])
+
             if len(self.periods[key]) > 0:
                 # get specific periodic parameterss
                 diff_periodic = diff[:, :, inds_periodic]
 
                 # fix when the distance is over 1/2 period away
                 inds_fix = (
                     xp.abs(diff_periodic) > periods[xp.newaxis, xp.newaxis, :] / 2.0
@@ -96,15 +102,15 @@
     def wrap(self, p, xp=None):
         """Wrap p with periodic distance control
 
         Args:
             p (dict): If dict, keys are ``branch_names``
                 and values are positions with parameters along the final dimension.
             xp (object, optional): ``numpy`` or ``cupy``. If ``None``, use ``numpy``.
-                (default: ``None``) 
+                (default: ``None``)
 
         """
 
         # cupy or numpy
         if xp is None:
             xp = np
```

### Comparing `Eryn-1.1.6/eryn/utils/stopping.py` & `Eryn-1.1.7/eryn/utils/stopping.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/utils/transform.py` & `Eryn-1.1.7/eryn/utils/transform.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/utils/updates.py` & `Eryn-1.1.7/eryn/utils/updates.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/eryn/utils/utility.py` & `Eryn-1.1.7/eryn/utils/utility.py`

 * *Files identical despite different names*

### Comparing `Eryn-1.1.6/setup.py` & `Eryn-1.1.7/setup.py`

 * *Files identical despite different names*

