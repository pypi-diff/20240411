# Comparing `tmp/lsst-ctrl-bps-parsl-26.2024.800.tar.gz` & `tmp/lsst-ctrl-bps-parsl-26.2024.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-ctrl-bps-parsl-26.2024.800.tar", last modified: Thu Feb 22 10:42:47 2024, max compression
+gzip compressed data, was "lsst-ctrl-bps-parsl-26.2024.900.tar", last modified: Thu Feb 29 10:20:45 2024, max compression
```

## Comparing `lsst-ctrl-bps-parsl-26.2024.800.tar` & `lsst-ctrl-bps-parsl-26.2024.900.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:47.822222 lsst-ctrl-bps-parsl-26.2024.800/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-02-22 10:42:47.822222 lsst-ctrl-bps-parsl-26.2024.800/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/bsd_license.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:47.814221 lsst-ctrl-bps-parsl-26.2024.800/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:47.814221 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:47.814221 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:47.814221 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:47.818221 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11724 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/site.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:47.818221 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/sites/
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/sites/ccin2p3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/sites/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/sites/nersc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/sites/princeton.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/sites/slac.py
--rw-r--r--   0 runner    (1001) docker     (127)    12665 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/sites/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/sites/work_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 10:42:47.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11434 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:47.822222 lsst-ctrl-bps-parsl-26.2024.800/python/lsst_ctrl_bps_parsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-02-22 10:42:47.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst_ctrl_bps_parsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-02-22 10:42:47.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst_ctrl_bps_parsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:42:47.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst_ctrl_bps_parsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-22 10:42:47.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst_ctrl_bps_parsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-22 10:42:47.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst_ctrl_bps_parsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:42:47.000000 lsst-ctrl-bps-parsl-26.2024.800/python/lsst_ctrl_bps_parsl.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-22 10:42:47.822222 lsst-ctrl-bps-parsl-26.2024.800/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:47.822222 lsst-ctrl-bps-parsl-26.2024.800/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-02-22 10:42:37.000000 lsst-ctrl-bps-parsl-26.2024.800/tests/test_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:45.693358 lsst-ctrl-bps-parsl-26.2024.900/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-02-29 10:20:45.693358 lsst-ctrl-bps-parsl-26.2024.900/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/bsd_license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:45.685358 lsst-ctrl-bps-parsl-26.2024.900/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:45.685358 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:45.685358 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:45.685358 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:45.689358 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11724 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/site.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:45.689358 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/sites/
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/sites/ccin2p3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/sites/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/sites/nersc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/sites/princeton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/sites/slac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12665 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/sites/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/sites/work_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:20:45.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11434 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:45.693358 lsst-ctrl-bps-parsl-26.2024.900/python/lsst_ctrl_bps_parsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-02-29 10:20:45.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst_ctrl_bps_parsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-02-29 10:20:45.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst_ctrl_bps_parsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:45.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst_ctrl_bps_parsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-29 10:20:45.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst_ctrl_bps_parsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 10:20:45.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst_ctrl_bps_parsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:45.000000 lsst-ctrl-bps-parsl-26.2024.900/python/lsst_ctrl_bps_parsl.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-29 10:20:45.693358 lsst-ctrl-bps-parsl-26.2024.900/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:45.693358 lsst-ctrl-bps-parsl-26.2024.900/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-02-29 10:20:22.000000 lsst-ctrl-bps-parsl-26.2024.900/tests/test_job.py
```

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/PKG-INFO` & `lsst-ctrl-bps-parsl-26.2024.900/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps-parsl
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: Parsl-based plugin for lsst-ctrl-bps.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps_parsl
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/README.md` & `lsst-ctrl-bps-parsl-26.2024.900/README.md`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/bsd_license.txt` & `lsst-ctrl-bps-parsl-26.2024.900/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/gpl-v3.0.txt` & `lsst-ctrl-bps-parsl-26.2024.900/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/pyproject.toml` & `lsst-ctrl-bps-parsl-26.2024.900/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/__init__.py` & `lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/configuration.py` & `lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/configuration.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/environment.py` & `lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/environment.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/job.py` & `lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/job.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/service.py` & `lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/service.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/site.py` & `lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/site.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/sites/__init__.py` & `lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/sites/ccin2p3.py` & `lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/sites/ccin2p3.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/sites/local.py` & `lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/sites/local.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/sites/nersc.py` & `lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/sites/nersc.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/sites/princeton.py` & `lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/sites/princeton.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/sites/slac.py` & `lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/sites/slac.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/sites/slurm.py` & `lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/sites/slurm.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/sites/work_queue.py` & `lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/sites/work_queue.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/python/lsst/ctrl/bps/parsl/workflow.py` & `lsst-ctrl-bps-parsl-26.2024.900/python/lsst/ctrl/bps/parsl/workflow.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/python/lsst_ctrl_bps_parsl.egg-info/PKG-INFO` & `lsst-ctrl-bps-parsl-26.2024.900/python/lsst_ctrl_bps_parsl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps-parsl
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: Parsl-based plugin for lsst-ctrl-bps.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps_parsl
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/python/lsst_ctrl_bps_parsl.egg-info/SOURCES.txt` & `lsst-ctrl-bps-parsl-26.2024.900/python/lsst_ctrl_bps_parsl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/tests/test_config.py` & `lsst-ctrl-bps-parsl-26.2024.900/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/tests/test_import.py` & `lsst-ctrl-bps-parsl-26.2024.900/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-parsl-26.2024.800/tests/test_job.py` & `lsst-ctrl-bps-parsl-26.2024.900/tests/test_job.py`

 * *Files identical despite different names*

