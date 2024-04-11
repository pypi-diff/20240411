# Comparing `tmp/lsst-ctrl-bps-panda-26.2024.800.tar.gz` & `tmp/lsst-ctrl-bps-panda-26.2024.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-ctrl-bps-panda-26.2024.800.tar", last modified: Thu Feb 22 10:43:05 2024, max compression
+gzip compressed data, was "lsst-ctrl-bps-panda-26.2024.900.tar", last modified: Thu Feb 29 10:20:28 2024, max compression
```

## Comparing `lsst-ctrl-bps-panda-26.2024.800.tar` & `lsst-ctrl-bps-panda-26.2024.900.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:05.724572 lsst-ctrl-bps-panda-26.2024.800/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-02-22 10:43:05.724572 lsst-ctrl-bps-panda-26.2024.800/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/bsd_license.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:05.720572 lsst-ctrl-bps-panda-26.2024.800/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:05.720572 lsst-ctrl-bps-panda-26.2024.800/python/lsst/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:05.720572 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:05.720572 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:05.720572 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:05.724572 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:05.724572 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/cli/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/cli/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/cli/cmd/panda_auth_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/cli/panda_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/cmd_line_embedder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:05.724572 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/conf_example/
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/conf_example/example_panda_SLAC.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/conf_example/pipelines_check_idf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/conf_example/test_idf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/conf_example/test_sdf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/conf_example/test_usdf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:05.724572 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/edgenode/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/edgenode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/edgenode/cmd_line_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/panda_auth_drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/panda_auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15176 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/panda_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    23468 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 10:43:05.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:05.724572 lsst-ctrl-bps-panda-26.2024.800/python/lsst_ctrl_bps_panda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-02-22 10:43:05.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst_ctrl_bps_panda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-02-22 10:43:05.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst_ctrl_bps_panda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:43:05.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst_ctrl_bps_panda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-22 10:43:05.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst_ctrl_bps_panda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-22 10:43:05.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst_ctrl_bps_panda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:43:05.000000 lsst-ctrl-bps-panda-26.2024.800/python/lsst_ctrl_bps_panda.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-22 10:43:05.728572 lsst-ctrl-bps-panda-26.2024.800/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:05.724572 lsst-ctrl-bps-panda-26.2024.800/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/tests/test_cmd_line_embedder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/tests/test_panda_auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-02-22 10:42:53.000000 lsst-ctrl-bps-panda-26.2024.800/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.417526 lsst-ctrl-bps-panda-26.2024.900/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-02-29 10:20:28.417526 lsst-ctrl-bps-panda-26.2024.900/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/bsd_license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.409526 lsst-ctrl-bps-panda-26.2024.900/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.409526 lsst-ctrl-bps-panda-26.2024.900/python/lsst/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.409526 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.409526 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.413526 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.413526 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.413526 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cli/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cli/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cli/cmd/panda_auth_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cli/panda_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cmd_line_embedder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.413526 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/conf_example/
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/conf_example/example_panda_SLAC.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/conf_example/pipelines_check_idf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/conf_example/test_idf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/conf_example/test_sdf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/conf_example/test_usdf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.413526 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/edgenode/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/edgenode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/edgenode/cmd_line_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/panda_auth_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/panda_auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15176 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/panda_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23468 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:20:28.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.417526 lsst-ctrl-bps-panda-26.2024.900/python/lsst_ctrl_bps_panda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-02-29 10:20:28.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst_ctrl_bps_panda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-02-29 10:20:28.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst_ctrl_bps_panda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:28.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst_ctrl_bps_panda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-29 10:20:28.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst_ctrl_bps_panda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 10:20:28.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst_ctrl_bps_panda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:28.000000 lsst-ctrl-bps-panda-26.2024.900/python/lsst_ctrl_bps_panda.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-29 10:20:28.417526 lsst-ctrl-bps-panda-26.2024.900/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:28.413526 lsst-ctrl-bps-panda-26.2024.900/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/tests/test_cmd_line_embedder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/tests/test_panda_auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-02-29 10:20:19.000000 lsst-ctrl-bps-panda-26.2024.900/tests/test_utils.py
```

### Comparing `lsst-ctrl-bps-panda-26.2024.800/PKG-INFO` & `lsst-ctrl-bps-panda-26.2024.900/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps-panda
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: PanDA plugin for lsst-ctrl-bps.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps_panda
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-ctrl-bps-panda-26.2024.800/README.rst` & `lsst-ctrl-bps-panda-26.2024.900/README.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/bsd_license.txt` & `lsst-ctrl-bps-panda-26.2024.900/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/gpl-v3.0.txt` & `lsst-ctrl-bps-panda-26.2024.900/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/pyproject.toml` & `lsst-ctrl-bps-panda-26.2024.900/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/__init__.py` & `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/cli/cmd/__init__.py` & `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cli/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/cli/cmd/panda_auth_commands.py` & `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cli/cmd/panda_auth_commands.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/cli/panda_auth.py` & `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cli/panda_auth.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/cmd_line_embedder.py` & `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/cmd_line_embedder.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/conf_example/example_panda_SLAC.yaml` & `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/conf_example/example_panda_SLAC.yaml`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/conf_example/pipelines_check_idf.yaml` & `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/conf_example/pipelines_check_idf.yaml`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/constants.py` & `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/constants.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/edgenode/cmd_line_decoder.py` & `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/edgenode/cmd_line_decoder.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/panda_auth_drivers.py` & `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/panda_auth_drivers.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/panda_auth_utils.py` & `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/panda_auth_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/panda_service.py` & `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/panda_service.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/python/lsst/ctrl/bps/panda/utils.py` & `lsst-ctrl-bps-panda-26.2024.900/python/lsst/ctrl/bps/panda/utils.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/python/lsst_ctrl_bps_panda.egg-info/PKG-INFO` & `lsst-ctrl-bps-panda-26.2024.900/python/lsst_ctrl_bps_panda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps-panda
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: PanDA plugin for lsst-ctrl-bps.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps_panda
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-ctrl-bps-panda-26.2024.800/python/lsst_ctrl_bps_panda.egg-info/SOURCES.txt` & `lsst-ctrl-bps-panda-26.2024.900/python/lsst_ctrl_bps_panda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/tests/test_cmd_line_embedder.py` & `lsst-ctrl-bps-panda-26.2024.900/tests/test_cmd_line_embedder.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/tests/test_panda_auth_utils.py` & `lsst-ctrl-bps-panda-26.2024.900/tests/test_panda_auth_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-panda-26.2024.800/tests/test_utils.py` & `lsst-ctrl-bps-panda-26.2024.900/tests/test_utils.py`

 * *Files identical despite different names*

