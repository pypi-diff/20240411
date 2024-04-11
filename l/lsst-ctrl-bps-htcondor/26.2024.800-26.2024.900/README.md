# Comparing `tmp/lsst-ctrl-bps-htcondor-26.2024.800.tar.gz` & `tmp/lsst-ctrl-bps-htcondor-26.2024.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-ctrl-bps-htcondor-26.2024.800.tar", last modified: Thu Feb 22 10:42:46 2024, max compression
+gzip compressed data, was "lsst-ctrl-bps-htcondor-26.2024.900.tar", last modified: Thu Feb 29 10:20:31 2024, max compression
```

## Comparing `lsst-ctrl-bps-htcondor-26.2024.800.tar` & `lsst-ctrl-bps-htcondor-26.2024.900.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:46.743677 lsst-ctrl-bps-htcondor-26.2024.800/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-22 10:42:37.000000 lsst-ctrl-bps-htcondor-26.2024.800/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-22 10:42:37.000000 lsst-ctrl-bps-htcondor-26.2024.800/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-22 10:42:37.000000 lsst-ctrl-bps-htcondor-26.2024.800/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-22 10:42:46.743677 lsst-ctrl-bps-htcondor-26.2024.800/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-22 10:42:37.000000 lsst-ctrl-bps-htcondor-26.2024.800/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-22 10:42:37.000000 lsst-ctrl-bps-htcondor-26.2024.800/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:46.735677 lsst-ctrl-bps-htcondor-26.2024.800/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:46.739677 lsst-ctrl-bps-htcondor-26.2024.800/doc/lsst.ctrl.bps.htcondor/
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-02-22 10:42:37.000000 lsst-ctrl-bps-htcondor-26.2024.800/doc/lsst.ctrl.bps.htcondor/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-22 10:42:37.000000 lsst-ctrl-bps-htcondor-26.2024.800/doc/lsst.ctrl.bps.htcondor/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-02-22 10:42:37.000000 lsst-ctrl-bps-htcondor-26.2024.800/doc/lsst.ctrl.bps.htcondor/userguide.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-22 10:42:37.000000 lsst-ctrl-bps-htcondor-26.2024.800/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-02-22 10:42:37.000000 lsst-ctrl-bps-htcondor-26.2024.800/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:46.735677 lsst-ctrl-bps-htcondor-26.2024.800/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:46.735677 lsst-ctrl-bps-htcondor-26.2024.800/python/lsst/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:46.735677 lsst-ctrl-bps-htcondor-26.2024.800/python/lsst/ctrl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:46.735677 lsst-ctrl-bps-htcondor-26.2024.800/python/lsst/ctrl/bps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:46.739677 lsst-ctrl-bps-htcondor-26.2024.800/python/lsst/ctrl/bps/htcondor/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-22 10:42:37.000000 lsst-ctrl-bps-htcondor-26.2024.800/python/lsst/ctrl/bps/htcondor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74496 2024-02-22 10:42:37.000000 lsst-ctrl-bps-htcondor-26.2024.800/python/lsst/ctrl/bps/htcondor/htcondor_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    53700 2024-02-22 10:42:37.000000 lsst-ctrl-bps-htcondor-26.2024.800/python/lsst/ctrl/bps/htcondor/lssthtc.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 10:42:46.000000 lsst-ctrl-bps-htcondor-26.2024.800/python/lsst/ctrl/bps/htcondor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:46.743677 lsst-ctrl-bps-htcondor-26.2024.800/python/lsst_ctrl_bps_htcondor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-22 10:42:46.000000 lsst-ctrl-bps-htcondor-26.2024.800/python/lsst_ctrl_bps_htcondor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-22 10:42:46.000000 lsst-ctrl-bps-htcondor-26.2024.800/python/lsst_ctrl_bps_htcondor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:42:46.000000 lsst-ctrl-bps-htcondor-26.2024.800/python/lsst_ctrl_bps_htcondor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-22 10:42:46.000000 lsst-ctrl-bps-htcondor-26.2024.800/python/lsst_ctrl_bps_htcondor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-22 10:42:46.000000 lsst-ctrl-bps-htcondor-26.2024.800/python/lsst_ctrl_bps_htcondor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:42:46.000000 lsst-ctrl-bps-htcondor-26.2024.800/python/lsst_ctrl_bps_htcondor.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-22 10:42:46.743677 lsst-ctrl-bps-htcondor-26.2024.800/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:46.739677 lsst-ctrl-bps-htcondor-26.2024.800/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-02-22 10:42:37.000000 lsst-ctrl-bps-htcondor-26.2024.800/tests/test_htcondor_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-02-22 10:42:37.000000 lsst-ctrl-bps-htcondor-26.2024.800/tests/test_lssthtc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.059387 lsst-ctrl-bps-htcondor-26.2024.900/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-29 10:20:31.059387 lsst-ctrl-bps-htcondor-26.2024.900/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.051387 lsst-ctrl-bps-htcondor-26.2024.900/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.055387 lsst-ctrl-bps-htcondor-26.2024.900/doc/lsst.ctrl.bps.htcondor/
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/doc/lsst.ctrl.bps.htcondor/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/doc/lsst.ctrl.bps.htcondor/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/doc/lsst.ctrl.bps.htcondor/userguide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.051387 lsst-ctrl-bps-htcondor-26.2024.900/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.051387 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.051387 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.051387 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/bps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.055387 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/bps/htcondor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/bps/htcondor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74496 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/bps/htcondor/htcondor_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53700 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/bps/htcondor/lssthtc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:20:30.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/bps/htcondor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.059387 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst_ctrl_bps_htcondor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-29 10:20:31.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst_ctrl_bps_htcondor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-29 10:20:31.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst_ctrl_bps_htcondor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:31.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst_ctrl_bps_htcondor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-29 10:20:31.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst_ctrl_bps_htcondor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 10:20:31.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst_ctrl_bps_htcondor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:30.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst_ctrl_bps_htcondor.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-29 10:20:31.059387 lsst-ctrl-bps-htcondor-26.2024.900/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.059387 lsst-ctrl-bps-htcondor-26.2024.900/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/tests/test_htcondor_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/tests/test_lssthtc.py
```

### Comparing `lsst-ctrl-bps-htcondor-26.2024.800/PKG-INFO` & `lsst-ctrl-bps-htcondor-26.2024.900/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps-htcondor
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: HTCondor plugin for lsst-ctrl-bps.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps_htcondor
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-ctrl-bps-htcondor-26.2024.800/README.rst` & `lsst-ctrl-bps-htcondor-26.2024.900/README.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.800/bsd_license.txt` & `lsst-ctrl-bps-htcondor-26.2024.900/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.800/doc/lsst.ctrl.bps.htcondor/CHANGES.rst` & `lsst-ctrl-bps-htcondor-26.2024.900/doc/lsst.ctrl.bps.htcondor/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.800/doc/lsst.ctrl.bps.htcondor/index.rst` & `lsst-ctrl-bps-htcondor-26.2024.900/doc/lsst.ctrl.bps.htcondor/index.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.800/doc/lsst.ctrl.bps.htcondor/userguide.rst` & `lsst-ctrl-bps-htcondor-26.2024.900/doc/lsst.ctrl.bps.htcondor/userguide.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.800/gpl-v3.0.txt` & `lsst-ctrl-bps-htcondor-26.2024.900/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.800/pyproject.toml` & `lsst-ctrl-bps-htcondor-26.2024.900/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.800/python/lsst/ctrl/bps/htcondor/__init__.py` & `lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/bps/htcondor/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.800/python/lsst/ctrl/bps/htcondor/htcondor_service.py` & `lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/bps/htcondor/htcondor_service.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.800/python/lsst/ctrl/bps/htcondor/lssthtc.py` & `lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/bps/htcondor/lssthtc.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.800/python/lsst_ctrl_bps_htcondor.egg-info/PKG-INFO` & `lsst-ctrl-bps-htcondor-26.2024.900/python/lsst_ctrl_bps_htcondor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps-htcondor
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: HTCondor plugin for lsst-ctrl-bps.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps_htcondor
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-ctrl-bps-htcondor-26.2024.800/python/lsst_ctrl_bps_htcondor.egg-info/SOURCES.txt` & `lsst-ctrl-bps-htcondor-26.2024.900/python/lsst_ctrl_bps_htcondor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.800/tests/test_htcondor_service.py` & `lsst-ctrl-bps-htcondor-26.2024.900/tests/test_htcondor_service.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.800/tests/test_lssthtc.py` & `lsst-ctrl-bps-htcondor-26.2024.900/tests/test_lssthtc.py`

 * *Files identical despite different names*

