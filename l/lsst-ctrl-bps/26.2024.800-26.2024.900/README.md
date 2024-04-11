# Comparing `tmp/lsst-ctrl-bps-26.2024.800.tar.gz` & `tmp/lsst-ctrl-bps-26.2024.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-ctrl-bps-26.2024.800.tar", last modified: Thu Feb 22 10:43:56 2024, max compression
+gzip compressed data, was "lsst-ctrl-bps-26.2024.900.tar", last modified: Thu Feb 29 10:21:39 2024, max compression
```

## Comparing `lsst-ctrl-bps-26.2024.800.tar` & `lsst-ctrl-bps-26.2024.900.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:56.570115 lsst-ctrl-bps-26.2024.800/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-22 10:43:56.570115 lsst-ctrl-bps-26.2024.800/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:56.558115 lsst-ctrl-bps-26.2024.800/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:56.558115 lsst-ctrl-bps-26.2024.800/doc/lsst.ctrl.bps/
--rw-r--r--   0 runner    (1001) docker     (127)    17300 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/doc/lsst.ctrl.bps/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/doc/lsst.ctrl.bps/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    44773 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/doc/lsst.ctrl.bps/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:56.558115 lsst-ctrl-bps-26.2024.800/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:56.558115 lsst-ctrl-bps-26.2024.800/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:56.562115 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:56.562115 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13097 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/bps_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/bps_draw.py
--rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/bps_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/bps_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cancel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:56.562115 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cli/bps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:56.566115 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cli/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cli/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cli/cmd/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:56.566115 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cli/opt/
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cli/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cli/opt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cli/opt/option_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cli/opt/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/clustered_quantum_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    21140 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:56.566115 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/etc/
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/etc/bps_defaults.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/etc/bps_eb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    30486 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/generic_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/pre_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/quantum_clustering_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/restart.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/submit.py
--rw-r--r--   0 runner    (1001) docker     (127)    42853 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 10:43:56.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12712 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/wms_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:56.566115 lsst-ctrl-bps-26.2024.800/python/lsst_ctrl_bps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-22 10:43:56.000000 lsst-ctrl-bps-26.2024.800/python/lsst_ctrl_bps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-02-22 10:43:56.000000 lsst-ctrl-bps-26.2024.800/python/lsst_ctrl_bps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:43:56.000000 lsst-ctrl-bps-26.2024.800/python/lsst_ctrl_bps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-22 10:43:56.000000 lsst-ctrl-bps-26.2024.800/python/lsst_ctrl_bps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-22 10:43:56.000000 lsst-ctrl-bps-26.2024.800/python/lsst_ctrl_bps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-22 10:43:56.000000 lsst-ctrl-bps-26.2024.800/python/lsst_ctrl_bps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:43:56.000000 lsst-ctrl-bps-26.2024.800/python/lsst_ctrl_bps.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-22 10:43:56.570115 lsst-ctrl-bps-26.2024.800/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:56.566115 lsst-ctrl-bps-26.2024.800/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/tests/test_bps_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/tests/test_bpsconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/tests/test_cli_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/tests/test_clustered_quantum_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/tests/test_drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/tests/test_generic_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/tests/test_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/tests/test_pre_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/tests/test_quantum_clustering_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-02-22 10:43:45.000000 lsst-ctrl-bps-26.2024.800/tests/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.637210 lsst-ctrl-bps-26.2024.900/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-29 10:21:39.637210 lsst-ctrl-bps-26.2024.900/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.625210 lsst-ctrl-bps-26.2024.900/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.629210 lsst-ctrl-bps-26.2024.900/doc/lsst.ctrl.bps/
+-rw-r--r--   0 runner    (1001) docker     (127)    17300 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/doc/lsst.ctrl.bps/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/doc/lsst.ctrl.bps/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    44773 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/doc/lsst.ctrl.bps/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.629210 lsst-ctrl-bps-26.2024.900/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.629210 lsst-ctrl-bps-26.2024.900/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.629210 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.633210 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13097 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/bps_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/bps_draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/bps_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/bps_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cancel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.633210 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/bps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.633210 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/cmd/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.633210 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/opt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/opt/option_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/opt/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/clustered_quantum_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21140 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.633210 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/etc/bps_defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/etc/bps_eb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    30486 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/generic_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/pre_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/quantum_clustering_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/submit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42853 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:21:39.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12712 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/wms_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.637210 lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-29 10:21:39.000000 lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-02-29 10:21:39.000000 lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:21:39.000000 lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-29 10:21:39.000000 lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-29 10:21:39.000000 lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 10:21:39.000000 lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:21:39.000000 lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-29 10:21:39.637210 lsst-ctrl-bps-26.2024.900/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.637210 lsst-ctrl-bps-26.2024.900/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_bps_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_bpsconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_cli_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_clustered_quantum_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_generic_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_pre_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_quantum_clustering_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_transform.py
```

### Comparing `lsst-ctrl-bps-26.2024.800/PKG-INFO` & `lsst-ctrl-bps-26.2024.900/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: Pluggable execution of workflow graphs from Rubin pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-ctrl-bps-26.2024.800/README.md` & `lsst-ctrl-bps-26.2024.900/README.md`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/bsd_license.txt` & `lsst-ctrl-bps-26.2024.900/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/doc/lsst.ctrl.bps/CHANGES.rst` & `lsst-ctrl-bps-26.2024.900/doc/lsst.ctrl.bps/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/doc/lsst.ctrl.bps/index.rst` & `lsst-ctrl-bps-26.2024.900/doc/lsst.ctrl.bps/index.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/doc/lsst.ctrl.bps/quickstart.rst` & `lsst-ctrl-bps-26.2024.900/doc/lsst.ctrl.bps/quickstart.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/gpl-v3.0.txt` & `lsst-ctrl-bps-26.2024.900/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/pyproject.toml` & `lsst-ctrl-bps-26.2024.900/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/__init__.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/__init__.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/__init__.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/bps_config.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/bps_config.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/bps_draw.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/bps_draw.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/bps_reports.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/bps_reports.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/bps_utils.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/bps_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cancel.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cancel.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cli/bps.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/bps.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cli/cmd/__init__.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cli/cmd/commands.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cli/opt/__init__.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cli/opt/arguments.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/opt/arguments.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cli/opt/option_groups.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/opt/option_groups.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/cli/opt/options.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/opt/options.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/clustered_quantum_graph.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/clustered_quantum_graph.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/constants.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/constants.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/drivers.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/drivers.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/etc/bps_defaults.yaml` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/etc/bps_defaults.yaml`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/etc/bps_eb.yaml` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/etc/bps_eb.yaml`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/generic_workflow.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/generic_workflow.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/ping.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/ping.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/pre_transform.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/pre_transform.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/prepare.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/prepare.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/quantum_clustering_funcs.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/quantum_clustering_funcs.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/report.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/report.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/restart.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/restart.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/submit.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/submit.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/transform.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/transform.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst/ctrl/bps/wms_service.py` & `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/wms_service.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst_ctrl_bps.egg-info/PKG-INFO` & `lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: Pluggable execution of workflow graphs from Rubin pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-ctrl-bps-26.2024.800/python/lsst_ctrl_bps.egg-info/SOURCES.txt` & `lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/tests/test_bps_utils.py` & `lsst-ctrl-bps-26.2024.900/tests/test_bps_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/tests/test_bpsconfig.py` & `lsst-ctrl-bps-26.2024.900/tests/test_bpsconfig.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/tests/test_cli_commands.py` & `lsst-ctrl-bps-26.2024.900/tests/test_cli_commands.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/tests/test_clustered_quantum_graph.py` & `lsst-ctrl-bps-26.2024.900/tests/test_clustered_quantum_graph.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/tests/test_drivers.py` & `lsst-ctrl-bps-26.2024.900/tests/test_drivers.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/tests/test_generic_workflow.py` & `lsst-ctrl-bps-26.2024.900/tests/test_generic_workflow.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/tests/test_ping.py` & `lsst-ctrl-bps-26.2024.900/tests/test_ping.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/tests/test_pre_transform.py` & `lsst-ctrl-bps-26.2024.900/tests/test_pre_transform.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/tests/test_quantum_clustering_funcs.py` & `lsst-ctrl-bps-26.2024.900/tests/test_quantum_clustering_funcs.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/tests/test_report.py` & `lsst-ctrl-bps-26.2024.900/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.800/tests/test_transform.py` & `lsst-ctrl-bps-26.2024.900/tests/test_transform.py`

 * *Files identical despite different names*

