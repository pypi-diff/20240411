# Comparing `tmp/lsst-ctrl-mpexec-26.2024.800.tar.gz` & `tmp/lsst-ctrl-mpexec-26.2024.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-ctrl-mpexec-26.2024.800.tar", last modified: Thu Feb 22 10:45:09 2024, max compression
+gzip compressed data, was "lsst-ctrl-mpexec-26.2024.900.tar", last modified: Thu Feb 29 10:22:41 2024, max compression
```

## Comparing `lsst-ctrl-mpexec-26.2024.800.tar` & `lsst-ctrl-mpexec-26.2024.900.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:45:09.608163 lsst-ctrl-mpexec-26.2024.800/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-02-22 10:45:09.608163 lsst-ctrl-mpexec-26.2024.800/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:45:09.596164 lsst-ctrl-mpexec-26.2024.800/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:45:09.596164 lsst-ctrl-mpexec-26.2024.800/doc/lsst.ctrl.mpexec/
--rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/doc/lsst.ctrl.mpexec/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)    19001 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/doc/lsst.ctrl.mpexec/configuring-pipetask-tasks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/doc/lsst.ctrl.mpexec/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/doc/lsst.ctrl.mpexec/pipetask.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:45:09.596164 lsst-ctrl-mpexec-26.2024.800/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:45:09.596164 lsst-ctrl-mpexec-26.2024.800/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:45:09.596164 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:45:09.600164 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:45:09.600164 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:45:09.600164 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/cmd/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:45:09.600164 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/opt/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/opt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/opt/optionGroups.py
--rw-r--r--   0 runner    (1001) docker     (127)    18341 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/opt/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/pipetask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:45:09.604164 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/confirmable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/pre_exec_init_qbb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/purge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/qgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/run_qbb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/update_graph_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    41298 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cmdLineFwk.py
--rw-r--r--   0 runner    (1001) docker     (127)    13673 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/dotTools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/execFixupDataId.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/executionGraphFixup.py
--rw-r--r--   0 runner    (1001) docker     (127)     9238 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/log_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)    27702 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/mpGraphExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)    21671 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/preExecInit.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/quantumGraphExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/separablePipelineExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16001 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/showInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    14665 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/simple_pipeline_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    23338 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/singleQuantumExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/taskFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 10:45:09.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:45:09.608163 lsst-ctrl-mpexec-26.2024.800/python/lsst_ctrl_mpexec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-02-22 10:45:09.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst_ctrl_mpexec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-02-22 10:45:09.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst_ctrl_mpexec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:45:09.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst_ctrl_mpexec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-22 10:45:09.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst_ctrl_mpexec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-22 10:45:09.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst_ctrl_mpexec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-22 10:45:09.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst_ctrl_mpexec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:45:09.000000 lsst-ctrl-mpexec-26.2024.800/python/lsst_ctrl_mpexec.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-22 10:45:09.608163 lsst-ctrl-mpexec-26.2024.800/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:45:09.608163 lsst-ctrl-mpexec-26.2024.800/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/tests/test_cliCmdCleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/tests/test_cliCmdPurge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/tests/test_cliCmdReport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/tests/test_cliCmdUpdateGraphRun.py
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/tests/test_cliScript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/tests/test_cliUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    46275 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/tests/test_cmdLineFwk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/tests/test_dotTools.py
--rw-r--r--   0 runner    (1001) docker     (127)    30387 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/tests/test_executors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/tests/test_preExecInit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    27390 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/tests/test_separablePipelineExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15981 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/tests/test_simple_pipeline_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-02-22 10:44:59.000000 lsst-ctrl-mpexec-26.2024.800/tests/test_taskFactory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.155057 lsst-ctrl-mpexec-26.2024.900/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-02-29 10:22:41.155057 lsst-ctrl-mpexec-26.2024.900/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.139056 lsst-ctrl-mpexec-26.2024.900/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.139056 lsst-ctrl-mpexec-26.2024.900/doc/lsst.ctrl.mpexec/
+-rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/doc/lsst.ctrl.mpexec/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19001 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/doc/lsst.ctrl.mpexec/configuring-pipetask-tasks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/doc/lsst.ctrl.mpexec/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/doc/lsst.ctrl.mpexec/pipetask.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.139056 lsst-ctrl-mpexec-26.2024.900/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.143056 lsst-ctrl-mpexec-26.2024.900/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.143056 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.143056 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.147056 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.147056 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/cmd/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.147056 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/opt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/opt/optionGroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18341 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/opt/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/pipetask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.147056 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/confirmable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/pre_exec_init_qbb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/purge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/qgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/run_qbb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/update_graph_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41298 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cmdLineFwk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13673 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/dotTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/execFixupDataId.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/executionGraphFixup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9238 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/log_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27702 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/mpGraphExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21671 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/preExecInit.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/quantumGraphExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/separablePipelineExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16001 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/showInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14665 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/simple_pipeline_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23338 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/singleQuantumExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/taskFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:22:40.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.151056 lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-02-29 10:22:41.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-02-29 10:22:41.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:22:41.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-29 10:22:41.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-29 10:22:41.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 10:22:41.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:22:40.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-29 10:22:41.155057 lsst-ctrl-mpexec-26.2024.900/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.151056 lsst-ctrl-mpexec-26.2024.900/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_cliCmdCleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_cliCmdPurge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_cliCmdReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_cliCmdUpdateGraphRun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_cliScript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_cliUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46275 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_cmdLineFwk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_dotTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30387 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_executors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_preExecInit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27390 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_separablePipelineExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15981 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_simple_pipeline_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_taskFactory.py
```

### Comparing `lsst-ctrl-mpexec-26.2024.800/PKG-INFO` & `lsst-ctrl-mpexec-26.2024.900/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-mpexec
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: Pipeline execution infrastructure for the Rubin Observatory LSST Science Pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_mpexec
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-ctrl-mpexec-26.2024.800/README.rst` & `lsst-ctrl-mpexec-26.2024.900/README.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/bsd_license.txt` & `lsst-ctrl-mpexec-26.2024.900/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/doc/lsst.ctrl.mpexec/CHANGES.rst` & `lsst-ctrl-mpexec-26.2024.900/doc/lsst.ctrl.mpexec/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/doc/lsst.ctrl.mpexec/configuring-pipetask-tasks.rst` & `lsst-ctrl-mpexec-26.2024.900/doc/lsst.ctrl.mpexec/configuring-pipetask-tasks.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/doc/lsst.ctrl.mpexec/index.rst` & `lsst-ctrl-mpexec-26.2024.900/doc/lsst.ctrl.mpexec/index.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/gpl-v3.0.txt` & `lsst-ctrl-mpexec-26.2024.900/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/pyproject.toml` & `lsst-ctrl-mpexec-26.2024.900/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/__init__.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/__init__.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/__init__.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/__init__.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/cmd/__init__.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/cmd/commands.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/opt/__init__.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/opt/arguments.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/opt/arguments.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/opt/optionGroups.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/opt/optionGroups.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/opt/options.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/opt/options.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/pipetask.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/pipetask.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/__init__.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/build.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/build.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/cleanup.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/cleanup.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/confirmable.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/confirmable.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/pre_exec_init_qbb.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/pre_exec_init_qbb.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/purge.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/purge.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/qgraph.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/qgraph.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/report.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/report.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/run.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/run.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/run_qbb.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/run_qbb.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/script/update_graph_run.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/update_graph_run.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cli/utils.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/utils.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/cmdLineFwk.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cmdLineFwk.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/dotTools.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/dotTools.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/execFixupDataId.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/execFixupDataId.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/executionGraphFixup.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/executionGraphFixup.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/log_capture.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/log_capture.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/mpGraphExecutor.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/mpGraphExecutor.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/preExecInit.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/preExecInit.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/quantumGraphExecutor.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/quantumGraphExecutor.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/reports.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/reports.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/separablePipelineExecutor.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/separablePipelineExecutor.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/showInfo.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/showInfo.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/simple_pipeline_executor.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/simple_pipeline_executor.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/singleQuantumExecutor.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/singleQuantumExecutor.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/taskFactory.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/taskFactory.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst/ctrl/mpexec/util.py` & `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/util.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst_ctrl_mpexec.egg-info/PKG-INFO` & `lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-mpexec
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: Pipeline execution infrastructure for the Rubin Observatory LSST Science Pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_mpexec
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-ctrl-mpexec-26.2024.800/python/lsst_ctrl_mpexec.egg-info/SOURCES.txt` & `lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/tests/test_cliCmdCleanup.py` & `lsst-ctrl-mpexec-26.2024.900/tests/test_cliCmdCleanup.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/tests/test_cliCmdPurge.py` & `lsst-ctrl-mpexec-26.2024.900/tests/test_cliCmdPurge.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/tests/test_cliCmdReport.py` & `lsst-ctrl-mpexec-26.2024.900/tests/test_cliCmdReport.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/tests/test_cliCmdUpdateGraphRun.py` & `lsst-ctrl-mpexec-26.2024.900/tests/test_cliCmdUpdateGraphRun.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/tests/test_cliScript.py` & `lsst-ctrl-mpexec-26.2024.900/tests/test_cliScript.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/tests/test_cliUtils.py` & `lsst-ctrl-mpexec-26.2024.900/tests/test_cliUtils.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/tests/test_cmdLineFwk.py` & `lsst-ctrl-mpexec-26.2024.900/tests/test_cmdLineFwk.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/tests/test_dotTools.py` & `lsst-ctrl-mpexec-26.2024.900/tests/test_dotTools.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/tests/test_executors.py` & `lsst-ctrl-mpexec-26.2024.900/tests/test_executors.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/tests/test_preExecInit.py` & `lsst-ctrl-mpexec-26.2024.900/tests/test_preExecInit.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/tests/test_reports.py` & `lsst-ctrl-mpexec-26.2024.900/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/tests/test_separablePipelineExecutor.py` & `lsst-ctrl-mpexec-26.2024.900/tests/test_separablePipelineExecutor.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/tests/test_simple_pipeline_executor.py` & `lsst-ctrl-mpexec-26.2024.900/tests/test_simple_pipeline_executor.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.800/tests/test_taskFactory.py` & `lsst-ctrl-mpexec-26.2024.900/tests/test_taskFactory.py`

 * *Files identical despite different names*

