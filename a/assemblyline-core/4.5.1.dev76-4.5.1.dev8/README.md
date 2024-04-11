# Comparing `tmp/assemblyline-core-4.5.1.dev76.tar.gz` & `tmp/assemblyline-core-4.5.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyline-core-4.5.1.dev76.tar", last modified: Thu Apr 11 13:59:52 2024, max compression
+gzip compressed data, was "assemblyline-core-4.5.1.dev8.tar", last modified: Thu Feb 22 20:16:23 2024, max compression
```

## Comparing `assemblyline-core-4.5.1.dev76.tar` & `assemblyline-core-4.5.1.dev8.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.321322 assemblyline-core-4.5.1.dev76/
--rw-r--r--   0 vsts      (1001) docker     (127)     1396 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/LICENCE.md
--rw-r--r--   0 vsts      (1001) docker     (127)     1814 2024-04-11 13:59:52.321322 assemblyline-core-4.5.1.dev76/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      860 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.269322 assemblyline-core-4.5.1.dev76/assemblyline_core/
--rw-r--r--   0 vsts      (1001) docker     (127)       12 2024-04-11 13:59:48.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/VERSION
--rw-r--r--   0 vsts      (1001) docker     (127)       49 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.277322 assemblyline-core-4.5.1.dev76/assemblyline_core/alerter/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/alerter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15813 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/alerter/processing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4964 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/alerter/run_alerter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.277322 assemblyline-core-4.5.1.dev76/assemblyline_core/archiver/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/archiver/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9179 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/archiver/run_archiver.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10237 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/badlist_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.277322 assemblyline-core-4.5.1.dev76/assemblyline_core/dispatching/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/dispatching/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      122 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/dispatching/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17216 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/dispatching/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    94587 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/dispatching/dispatcher.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7403 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/dispatching/schedules.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2050 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/dispatching/timeout.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.277322 assemblyline-core-4.5.1.dev76/assemblyline_core/expiry/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/expiry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14062 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/expiry/run_expiry.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.281322 assemblyline-core-4.5.1.dev76/assemblyline_core/ingester/
--rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/ingester/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/ingester/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      190 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/ingester/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39214 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/ingester/ingester.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.289322 assemblyline-core-4.5.1.dev76/assemblyline_core/metrics/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/metrics/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30865 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/metrics/es_metrics.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15986 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/metrics/heartbeat_formatter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7559 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/metrics/helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19852 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/metrics/metrics_server.py
--rw-r--r--   0 vsts      (1001) docker     (127)      256 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/metrics/run_heartbeat_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)      250 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/metrics/run_metrics_aggregator.py
--rw-r--r--   0 vsts      (1001) docker     (127)      274 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/metrics/run_statistics_aggregator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.289322 assemblyline-core-4.5.1.dev76/assemblyline_core/plumber/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/plumber/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9534 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/plumber/run_plumber.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.289322 assemblyline-core-4.5.1.dev76/assemblyline_core/replay/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/replay/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18908 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/replay/client.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.289322 assemblyline-core-4.5.1.dev76/assemblyline_core/replay/creator/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/replay/creator/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2899 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/replay/creator/run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7790 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/replay/creator/run_worker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.293322 assemblyline-core-4.5.1.dev76/assemblyline_core/replay/loader/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/replay/loader/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3564 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/replay/loader/run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3183 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/replay/loader/run_worker.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2577 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/replay/replay.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10914 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/safelist_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.297322 assemblyline-core-4.5.1.dev76/assemblyline_core/scaler/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/scaler/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1858 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/scaler/collection.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.297322 assemblyline-core-4.5.1.dev76/assemblyline_core/scaler/controllers/
--rw-r--r--   0 vsts      (1001) docker     (127)       90 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/scaler/controllers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24747 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/scaler/controllers/docker_ctl.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2462 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/scaler/controllers/interface.py
--rw-r--r--   0 vsts      (1001) docker     (127)    65957 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/scaler/controllers/kubernetes_ctl.py
--rw-r--r--   0 vsts      (1001) docker     (127)      160 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/scaler/run_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49873 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/scaler/scaler_server.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12219 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/server_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10044 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/signature_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10982 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/submission_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23620 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/tasking_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.297322 assemblyline-core-4.5.1.dev76/assemblyline_core/updater/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/updater/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9906 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/updater/helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34206 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/updater/run_updater.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.309322 assemblyline-core-4.5.1.dev76/assemblyline_core/vacuum/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/vacuum/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5628 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/vacuum/crawler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/vacuum/department_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3478 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/vacuum/safelist.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3136 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/vacuum/stream_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29885 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/vacuum/worker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.317322 assemblyline-core-4.5.1.dev76/assemblyline_core/workflow/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10391 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/assemblyline_core/workflow/run_workflow.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.277322 assemblyline-core-4.5.1.dev76/assemblyline_core.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1814 2024-04-11 13:59:52.000000 assemblyline-core-4.5.1.dev76/assemblyline_core.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     3136 2024-04-11 13:59:52.000000 assemblyline-core-4.5.1.dev76/assemblyline_core.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-11 13:59:52.000000 assemblyline-core-4.5.1.dev76/assemblyline_core.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-04-11 13:59:52.000000 assemblyline-core-4.5.1.dev76/assemblyline_core.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-04-11 13:59:52.000000 assemblyline-core-4.5.1.dev76/assemblyline_core.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-04-11 13:59:52.329322 assemblyline-core-4.5.1.dev76/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     2020 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-11 13:59:52.321322 assemblyline-core-4.5.1.dev76/test/
--rw-r--r--   0 vsts      (1001) docker     (127)     5768 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/test/test_alerter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8754 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/test/test_badlist_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15228 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/test/test_dispatcher.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2043 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/test/test_expiry.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/test/test_plumber.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10842 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/test/test_replay.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9751 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/test/test_safelist_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2006 2024-04-11 13:59:26.000000 assemblyline-core-4.5.1.dev76/test/test_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5380 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/test/test_scheduler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3563 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/test/test_signature_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    46102 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/test/test_simulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4419 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/test/test_vacuum.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6792 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/test/test_worker_ingest.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4780 2024-04-11 13:59:28.000000 assemblyline-core-4.5.1.dev76/test/test_worker_submit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.592267 assemblyline-core-4.5.1.dev8/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1396 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/LICENCE.md
+-rw-r--r--   0 vsts      (1001) docker     (127)     1813 2024-02-22 20:16:23.592267 assemblyline-core-4.5.1.dev8/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      860 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.548266 assemblyline-core-4.5.1.dev8/assemblyline_core/
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-02-22 20:16:21.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/VERSION
+-rw-r--r--   0 vsts      (1001) docker     (127)       49 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.552266 assemblyline-core-4.5.1.dev8/assemblyline_core/alerter/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/alerter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15813 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/alerter/processing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4964 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/alerter/run_alerter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.552266 assemblyline-core-4.5.1.dev8/assemblyline_core/archiver/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/archiver/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8318 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/archiver/run_archiver.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10237 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/badlist_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.556266 assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      122 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17216 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    94587 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/dispatcher.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7403 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/schedules.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2050 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/timeout.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.556266 assemblyline-core-4.5.1.dev8/assemblyline_core/expiry/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/expiry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14062 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/expiry/run_expiry.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.560266 assemblyline-core-4.5.1.dev8/assemblyline_core/ingester/
+-rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/ingester/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/ingester/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      190 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/ingester/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39214 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/ingester/ingester.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.564266 assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30865 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/es_metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13587 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/heartbeat_formatter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7559 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17322 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/metrics_server.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      256 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/run_heartbeat_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      250 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/run_metrics_aggregator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      274 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/run_statistics_aggregator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.568266 assemblyline-core-4.5.1.dev8/assemblyline_core/plumber/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/plumber/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9534 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/plumber/run_plumber.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.568266 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18884 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/client.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.572266 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/creator/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/creator/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2899 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/creator/run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7790 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/creator/run_worker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.572266 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/loader/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/loader/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3564 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/loader/run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3183 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/loader/run_worker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2577 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/replay/replay.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10914 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/safelist_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.572266 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1858 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/collection.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.576267 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/controllers/
+-rw-r--r--   0 vsts      (1001) docker     (127)       90 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/controllers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24170 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/controllers/docker_ctl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2462 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/controllers/interface.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    66066 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/controllers/kubernetes_ctl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      160 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/run_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49926 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/scaler_server.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12219 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/server_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10044 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/signature_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10982 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/submission_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23620 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/tasking_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.576267 assemblyline-core-4.5.1.dev8/assemblyline_core/updater/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/updater/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9293 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/updater/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34234 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/updater/run_updater.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.580267 assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5628 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/crawler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/department_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3478 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/safelist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3136 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/stream_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29284 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/worker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.584267 assemblyline-core-4.5.1.dev8/assemblyline_core/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10391 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/assemblyline_core/workflow/run_workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.552266 assemblyline-core-4.5.1.dev8/assemblyline_core.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1813 2024-02-22 20:16:23.000000 assemblyline-core-4.5.1.dev8/assemblyline_core.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     3136 2024-02-22 20:16:23.000000 assemblyline-core-4.5.1.dev8/assemblyline_core.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-22 20:16:23.000000 assemblyline-core-4.5.1.dev8/assemblyline_core.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-02-22 20:16:23.000000 assemblyline-core-4.5.1.dev8/assemblyline_core.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-02-22 20:16:23.000000 assemblyline-core-4.5.1.dev8/assemblyline_core.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-02-22 20:16:23.592267 assemblyline-core-4.5.1.dev8/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     2020 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-22 20:16:23.592267 assemblyline-core-4.5.1.dev8/test/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5768 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/test/test_alerter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8754 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_badlist_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15228 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_dispatcher.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2043 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_expiry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_plumber.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10842 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_replay.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9751 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_safelist_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2006 2024-02-22 20:16:06.000000 assemblyline-core-4.5.1.dev8/test/test_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5380 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_scheduler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3563 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_signature_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    46102 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_simulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4419 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_vacuum.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6792 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_worker_ingest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4780 2024-02-22 20:16:08.000000 assemblyline-core-4.5.1.dev8/test/test_worker_submit.py
```

### Comparing `assemblyline-core-4.5.1.dev76/LICENCE.md` & `assemblyline-core-4.5.1.dev8/LICENCE.md`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/PKG-INFO` & `assemblyline-core-4.5.1.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline-core
-Version: 4.5.1.dev76
+Version: 4.5.1.dev8
 Summary: Assemblyline 4 - Core components
 Home-page: https://github.com/CybercentreCanada/assemblyline-core/
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `assemblyline-core-4.5.1.dev76/README.md` & `assemblyline-core-4.5.1.dev8/README.md`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/alerter/processing.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/alerter/processing.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/alerter/run_alerter.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/alerter/run_alerter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/archiver/run_archiver.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/archiver/run_archiver.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import os
 import tempfile
 
 from assemblyline.common import forge
 from assemblyline.common.archiving import ARCHIVE_QUEUE_NAME
 from assemblyline.common.metrics import MetricsFactory
 from assemblyline.datastore.collection import ESCollection, Index
-from assemblyline.datastore.exceptions import VersionConflictException
 from assemblyline.odm.messages.archive_heartbeat import Metrics
+from assemblyline.odm.models.submission import Submission
 from assemblyline.remote.datatypes import get_client
 from assemblyline.remote.datatypes.queues.named import NamedQueue
 
 from assemblyline_core.server_base import ServerBase
 
 
 class SubmissionNotFound(Exception):
@@ -58,46 +58,29 @@
         message = self.archive_queue.pop(timeout=1)
 
         # If there is no alert bail out
         if not message:
             return
         else:
             try:
-                if len(message) == 3:
-                    archive_type, type_id, delete_after = message
-                    metadata = None
-                else:
-                    archive_type, type_id, delete_after, metadata = message
-
+                archive_type, type_id, delete_after = message
                 self.counter.increment('received')
             except Exception:
                 self.log.error(f"Invalid message received: {message}")
                 return
 
         # Start of process alert transaction
         if self.apm_client:
             self.apm_client.begin_transaction('Process archive message')
 
         try:
             if archive_type == "submission":
                 self.counter.increment('submission')
                 # Load submission
-                while True:
-                    try:
-                        submission, version = self.datastore.submission.get_if_exists(type_id, version=True)
-
-                        # If we have metadata passed in the message, we need to apply it before archiving the submission
-                        if metadata and self.config.core.archiver.use_metadata:
-                            submission.metadata.update({f"archive.{k}": v for k, v in metadata.items()})
-                            self.datastore.submission.save(type_id, submission, version=version)
-
-                        break
-                    except VersionConflictException as vce:
-                        self.log.info(f"Retrying saving metadata due to version conflict: {str(vce)}")
-
+                submission: Submission = self.datastore.submission.get_if_exists(type_id)
                 if not submission:
                     raise SubmissionNotFound(type_id)
 
                 self.datastore.submission.archive(type_id, delete_after=delete_after)
                 if not delete_after:
                     self.datastore.submission.update(type_id, [(ESCollection.UPDATE_SET, 'archived', True)],
                                                      index_type=Index.HOT)
```

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/badlist_client.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/badlist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/dispatching/client.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/dispatching/dispatcher.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/dispatcher.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/dispatching/schedules.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/schedules.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/dispatching/timeout.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/dispatching/timeout.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/expiry/run_expiry.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/expiry/run_expiry.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/ingester/ingester.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/ingester/ingester.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/metrics/es_metrics.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/es_metrics.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import json
 import tempfile
-import time
-import sys
-from os import environ, path
-from urllib.parse import urlparse
 
 import elasticapm
-import elasticsearch
-from packaging import version
+import sys
 
-from assemblyline.common import forge
-from assemblyline.common.isotime import now_as_iso
+import elasticsearch
+import time
 
 from assemblyline_core.metrics.helper import with_retries, ensure_indexes
 from assemblyline_core.server_base import ServerBase
 
+from assemblyline.common import forge
+from assemblyline.common.isotime import now_as_iso
+
+from os import environ, path
+from packaging import version
+from urllib.parse import urlparse
 
 METRICSTORE_ROOT_CA_PATH = environ.get('METRICSTORE_ROOT_CA_PATH', '/etc/assemblyline/ssl/al_root-ca.crt')
 METRICSTORE_VERIFY_CERTS = environ.get('METRICSTORE_VERIFY_CERTS', 'true').lower() == "true"
 
-
 class ESMetricsServer(ServerBase):
     """
     There can only be one of these type of metrics server running because it gathers elasticsearch metrics for
     the whole cluster.
     """
 
     def __init__(self, config=None):
```

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/metrics/heartbeat_formatter.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/heartbeat_formatter.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,24 +3,22 @@
 from apscheduler.schedulers.background import BackgroundScheduler
 
 from assemblyline.common import forge, metrics
 from assemblyline.common.archiving import ARCHIVE_QUEUE_NAME
 from assemblyline.common.constants import DISPATCH_TASK_HASH, SUBMISSION_QUEUE, \
     SERVICE_STATE_HASH, ServiceStatus
 from assemblyline.datastore.exceptions import SearchException
-from assemblyline.odm.messages.retrohunt_heartbeat import RetrohuntMessage
 from assemblyline.odm.messages.scaler_heartbeat import ScalerMessage
 from assemblyline.odm.messages.scaler_status_heartbeat import ScalerStatusMessage
 from assemblyline.odm.messages.alerter_heartbeat import AlerterMessage
 from assemblyline.odm.messages.archive_heartbeat import ArchiveMessage
 from assemblyline.odm.messages.dispatcher_heartbeat import DispatcherMessage
 from assemblyline.odm.messages.expiry_heartbeat import ExpiryMessage
 from assemblyline.odm.messages.ingest_heartbeat import IngestMessage
 from assemblyline.odm.messages.service_heartbeat import ServiceMessage
-from assemblyline.odm.messages.shard_heartbeat import ShardMessage
 from assemblyline.odm.messages.vacuum_heartbeat import VacuumMessage
 from assemblyline.remote.datatypes import get_client
 from assemblyline.remote.datatypes.hash import Hash, ExpiringHash
 from assemblyline.remote.datatypes.queues.comms import CommsQueue
 from assemblyline.remote.datatypes.queues.named import NamedQueue
 from assemblyline.remote.datatypes.queues.priority import PriorityQueue
 
@@ -287,55 +285,9 @@
                     }
                 }
                 self.status_queue.publish(VacuumMessage(msg).as_primitives())
                 self.log.info(f"Sent vacuum heartbeat: {msg['msg']}")
             except Exception:
                 self.log.exception("An exception occurred while generating VacuumMessage")
 
-        elif m_type == "elastic_shards":
-            try:
-                msg = {
-                    "sender": self.sender,
-                    "msg": {
-                        "instances": instances,
-                        "request_time": m_data['request_time'],
-                        "shard_sizes": m_data['shard_sizes'],
-                    }
-                }
-                self.status_queue.publish(ShardMessage(msg).as_primitives())
-                self.log.info(f"Sent elastic shard heartbeat: {msg['msg']}")
-            except Exception:
-                self.log.exception("An exception occurred while generating ShardMessage")
-
-        elif m_type == "retrohunt":
-            try:
-
-                status = m_data.get('status', {})
-                fetcher = status.get('fetcher', {})
-                resources = status.get('resources', {})
-                storage = status.get('storage', {})
-                last_minute_cpu = sum(report.get('cpu_load_1m', 0) for report in resources.values())
-                memory = sum(report.get('memory', 0) for report in resources.values())
-                free_storage = [report.get('high_water', 0) - report.get('used', 0)
-                                for report in storage.values()]
-
-                msg = {
-                    "sender": self.sender,
-                    "msg": {
-                        'instances': instances,
-                        'request_time': m_data['request_time'],
-                        'pending_files': fetcher.get('pending_files'),
-                        'ingested_last_minute': fetcher.get('last_minute_throughput'),
-                        'worker_storage_available': min(free_storage),
-                        'total_storage_available': sum(free_storage),
-                        'active_searches': status.get('active_searches'),
-                        'last_minute_cpu': last_minute_cpu,
-                        'total_memory_used': memory,
-                    }
-                }
-                self.status_queue.publish(RetrohuntMessage(msg).as_primitives())
-                self.log.info(f"Sent retrohunt heartbeat: {msg['msg']}")
-            except Exception:
-                self.log.exception("An exception occurred while generating RetrohuntMessage")
-
         else:
             self.log.warning(f"Skipping unknown counter: {m_name} [{m_type}] ==> {m_data}")
```

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/metrics/helper.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/helper.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/metrics/metrics_server.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/metrics/metrics_server.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 #!/usr/bin/env python
 
 import tempfile
 import sys
 import time
-import threading
 from collections import Counter
-from threading import Lock, Thread
-from os import environ, path
-from urllib.parse import urlparse
+from threading import Lock
 
 import elasticapm
 import elasticsearch
-import requests
-from packaging import version
 
 from apscheduler.schedulers.background import BackgroundScheduler
 from assemblyline_core.metrics.heartbeat_formatter import HeartbeatFormatter
 from assemblyline_core.metrics.helper import ensure_indexes, with_retries
 from assemblyline_core.server_base import ServerBase
 from assemblyline.common.isotime import now_as_iso
 from assemblyline.common import forge
 from assemblyline.remote.datatypes.queues.comms import CommsQueue
+from os import environ, path
+from packaging import version
+from urllib.parse import urlparse
 
 METRICS_QUEUE = "assemblyline_metrics"
 NON_AGGREGATED = ['scaler', 'scaler_status']
 NON_AGGREGATED_COUNTERS = {'dispatcher': {'save_queue', 'error_queue'}}
 
 METRICSTORE_ROOT_CA_PATH = environ.get('METRICSTORE_ROOT_CA_PATH', '/etc/assemblyline/ssl/al_root-ca.crt')
 METRICSTORE_VERIFY_CERTS = environ.get('METRICSTORE_VERIFY_CERTS', 'true').lower() == "true"
@@ -256,15 +254,14 @@
     def __init__(self, config=None):
         super().__init__('assemblyline.heartbeat_manager')
         self.config = config or forge.get_config()
         self.datastore = forge.get_datastore()
         self.metrics_queue = CommsQueue(METRICS_QUEUE)
         self.scheduler = BackgroundScheduler(daemon=True)
         self.hm = HeartbeatFormatter("heartbeat_manager", self.log, config=self.config)
-        self.hauntedhouse_client = forge.get_hauntedhouse_client(self.config)
 
         self.counters_lock = Lock()
         self.counters = {}
         self.rolling_window = {}
         self.window_ttl = {}
         self.ttl = self.config.core.metrics.export_interval * 2
         self.window_size = int(60 / self.config.core.metrics.export_interval)
@@ -279,18 +276,14 @@
         else:
             self.apm_client = None
 
     def try_run(self):
         self.scheduler.add_job(self._export_hearbeats, 'interval', seconds=self.config.core.metrics.export_interval)
         self.scheduler.start()
 
-        threading.Thread(target=self._call_interval, args=('es_shards', self._fetch_shards), daemon=True).start()
-        if self.config.retrohunt.enabled:
-            threading.Thread(target=self._call_interval, args=('retrohunt', self._fetch_retrohunt), daemon=True).start()
-
         while self.running:
             for msg in self.metrics_queue.listen():
                 # APM Transaction start
                 if self.apm_client:
                     self.apm_client.begin_transaction('heartbeat')
 
                 m_name = msg.pop('name', None)
@@ -318,72 +311,14 @@
                         for k, v in non_agg_values.items():
                             self.counters[c_key][k] = v
 
                 # APM Transaction end
                 if self.apm_client:
                     self.apm_client.end_transaction('process_message', 'success')
 
-    def _call_interval(self, name, method):
-        while self.running:
-            # Run the heartbeat
-            send_time = time.time()
-            try:
-                method()
-            except Exception:
-                self.log.exception('Error running metric fetcher %s', name)
-
-            # Wait until we are inline with the heartbeat interval
-            elapsed = time.time() - send_time
-            remaining = self.config.core.metrics.export_interval - elapsed
-            if remaining > 0:
-                self.sleep(remaining)     
-
-    def _fetch_shards(self):
-        request_time = None
-        sizes = {}
-        nodes = []
-        try:
-            # Pull shard data from elastisearch
-            start_time = time.time()
-            response = self.datastore.ds.client.cat.shards(bytes='b', format='json', master_timeout='5s')
-            for shard in response.body:
-                index = shard['index']
-                sizes.setdefault(index, 0)
-                sizes[index] = max(sizes[index], int(shard['store']))
-                nodes.append(shard['node'])
-            request_time = time.time() - start_time
-
-        finally:
-            # Export metrics heartbeat, send None and empty if an error occurs while getting the data
-            # the error will be logged in the outer function
-            metrics = {
-                'shard_sizes': sizes,
-                'request_time': request_time,
-            }
-            self.hm.send_heartbeat('elastic_shards', 'datastore', metrics, len(set(nodes)))
-
-    def _fetch_retrohunt(self):
-        status = {}
-        request_time = None
-        try:
-            # Pull status message from retrohunt
-            start_time = time.time()
-            status = self.hauntedhouse_client.status()
-            request_time = time.time() - start_time
-
-        finally:    
-            metrics = {
-                'request_time': request_time,
-                'status': status,
-            }
-            instances = len(status.get('storage', {}))
-
-            # Export heartbeat
-            self.hm.send_heartbeat('retrohount', 'hauntedhouse', metrics, instances)
-
     def _export_hearbeats(self):
         try:
             self.heartbeat()
             self.log.info("Expiring unused counters...")
             # APM Transaction start
             if self.apm_client:
                 self.apm_client.begin_transaction('heartbeat')
```

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/plumber/run_plumber.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/plumber/run_plumber.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/replay/client.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/replay/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,25 +367,25 @@
         }
         self.checkpoint_hash = Hash('replay_checkpoints', redis_persist)
 
         super().__init__(log, **kwargs)
 
     def _query(self, collection, query, filter_queries=[], rows=None, track_total_hits=False):
         return getattr(self.datastore, collection).search(
-            query, filters=filter_queries, rows=rows, track_total_hits=track_total_hits, as_obj=False
+            query, filters=filter_queries, rows=rows, track_total_hits=track_total_hits
         )
 
     def _put_checkpoint(self, collection, checkpoint):
         self.checkpoint_hash.set(collection, checkpoint)
 
     def _get_checkpoint(self, collection) -> str:
         return self.checkpoint_hash.get(collection) or "*"
 
     def _get_next_object_ids(self, collection, query, filter_queries, fl, sort):
-        return getattr(self.datastore, collection).search(query, fl=fl, sort=sort, rows=100, filters=filter_queries, as_obj=False)
+        return getattr(self.datastore, collection).search(query, fl=fl, sort=sort, rows=100, filters=filter_queries)
 
     def _set_bulk_object_pending(self, collection, query, filter_queries, max_docs):
         ds_collection = getattr(self.datastore, collection)
         operations = [(ds_collection.UPDATE_SET, 'metadata.replay', REPLAY_PENDING)]
         ds_collection.update_by_query(query, operations, filters=filter_queries, max_docs=max_docs)
 
     def _stream_objects(self, collection, query, fl="*", filter_queries=[]):
@@ -427,15 +427,15 @@
                         data['enabled'] = obj["enabled"]
                     es_collection.save(id, BadlistClient._merge_hashes(data, obj))
                 elif collection == "safelist":
                     if obj:
                         # Preserve the system's enabled state of the item
                         data['enabled'] = obj["enabled"]
                     es_collection.save(id, SafelistClient._merge_hashes(data, obj))
-            es_collection.commit()
+                es_collection.commit()
 
     def set_single_object_complete(self, collection, id):
         ds_collection = getattr(self.datastore, collection)
         operations = [(ds_collection.UPDATE_SET, 'metadata.replay', REPLAY_DONE)]
         ds_collection.update(id, operations)
 
     def get_next_message(self, message_type):
```

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/replay/creator/run.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/replay/creator/run.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/replay/creator/run_worker.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/replay/creator/run_worker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/replay/loader/run.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/replay/loader/run.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/replay/loader/run_worker.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/replay/loader/run_worker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/replay/replay.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/replay/replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/safelist_client.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/safelist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/scaler/collection.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/collection.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/scaler/controllers/docker_ctl.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/controllers/docker_ctl.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,18 +117,15 @@
                 for service_name in self.networks:
                     network = self._get_network(service_name)
                     if self.service_server.name not in {c.name for c in network.containers}:
                         self._connect_to_network(self.service_server, self.networks[service_name],
                                                  aliases=['service-server'])
 
                 # As long as the current service server is still running, just block its exit code in this thread
-                try:
-                    self.service_server.wait()
-                except docker.errors.NotFound:
-                    pass
+                self.service_server.wait()
 
                 # If it does return, find the new service server
                 self.service_server = self.find_service_server()
             except Exception:
                 self.log.exception("An error occurred while watching the service server.")
 
     def stop(self):
@@ -157,32 +154,23 @@
             aliases = [container.name]
         try:
             network.connect(container, aliases=aliases)
         except docker.errors.APIError as e:
             if 'already exists' in str(e):
                 return
             raise e
-        except docker.errors.NotFound as e:
-            if aliases == ['service-server']:
-                # We've lost our service-server container, time to find another
-                self.service_server = self.find_service_server()
-                network.connect(self.service_server, aliases=aliases)
-                return
-            raise e
-
 
     def _start(self, service_name):
         """Launch a docker container in a manner suitable for Assemblyline."""
         container_name, container_index = self._name_container(service_name)
         prof = self._profiles[service_name]
         cfg = prof.container_config
 
         # Set the list of labels
-        labels = {_v.name: _v.value for _v in cfg.labels}
-        labels.update(self._labels)
+        labels = dict(self._labels)
         labels.update({
             'component': service_name,
             'com.docker.compose.service': service_name.lower(),
             'com.docker.compose.container-number': str(container_index)
         })
 
         # Prepare the volumes and folders
@@ -490,16 +478,15 @@
         if instance_key is None:
             instance_key = uuid.uuid4().hex
 
         volumes = {_n: {'bind': _v.mount_path, 'mode': 'rw'} for _n, _v in spec.volumes.items()}
         if spec.run_as_core:
             volumes.update({row[0]: {'bind': row[1], 'mode': 'ro'} for row in self.core_mounts})
 
-        all_labels = {_v.name: _v.value for _v in spec.container.labels}
-        all_labels.update(self._labels)
+        all_labels = dict(self._labels)
         all_labels.update({
             'component': service_name,
             CHANGE_KEY_NAME: change_check,
             'com.docker.compose.service': deployment_name.lower()
         })
         all_labels.update(labels)
```

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/scaler/controllers/interface.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/controllers/interface.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/scaler/controllers/kubernetes_ctl.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/controllers/kubernetes_ctl.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from dateutil.tz import tzlocal
 from typing import List, Optional, Tuple
 from time import sleep
 from assemblyline.odm.models.config import Selector
 
 from kubernetes import client, config, watch
 from kubernetes.client import V1Deployment, V1DeploymentSpec, V1PodTemplateSpec, V1DeploymentStrategy, \
-    V1PodSpec, V1ObjectMeta, V1Volume, V1Container, V1VolumeMount, V1EnvVar, V1ConfigMapVolumeSource, \
+    V1PodSpec, V1PodOS, V1ObjectMeta, V1Volume, V1Container, V1VolumeMount, V1EnvVar, V1ConfigMapVolumeSource, \
     V1PersistentVolumeClaimVolumeSource, V1LabelSelector, V1ResourceRequirements, V1PersistentVolumeClaim, \
     V1PersistentVolumeClaimSpec, V1NetworkPolicy, V1NetworkPolicySpec, V1NetworkPolicyEgressRule, V1NetworkPolicyPeer, \
     V1NetworkPolicyIngressRule, V1Secret, V1SecretVolumeSource, V1LocalObjectReference, V1Service, \
     V1ServiceSpec, V1ServicePort, V1PodSecurityContext, V1Probe, V1ExecAction, V1SecurityContext, \
     V1Affinity, V1NodeAffinity, V1NodeSelector, V1NodeSelectorTerm, V1NodeSelectorRequirement, CoreV1Event
 from kubernetes.client.rest import ApiException
 from assemblyline.odm.models.service import DependencyConfig, DockerConfig, PersistentVolume
@@ -729,20 +729,18 @@
                            volumes: list[V1Volume] = None, mounts: list[V1VolumeMount] = None,
                            core_mounts: bool = False, change_key: str = '', high_priority: bool = False,
                            deployment_strategy: V1DeploymentStrategy = V1DeploymentStrategy()):
         # Build a cache key to check for changes, just trying to only patch what changed
         # will still potentially result in a lot of restarts due to different kubernetes
         # systems returning differently formatted data
         field_selector, label_selector = selector_to_list_filters(self.linux_node_selector)
-        key_labels = sorted((labels or {}).items())
+        lbls = sorted((labels or {}).items())
         svc_env = sorted(self._service_limited_env[service_name].items())
-        deployment_labels = {_v.name: _v.value for _v in docker_config.labels}
-        key_labels += sorted(deployment_labels.items())
         change_key = str(f"n={deployment_name}{change_key}dc={docker_config}ss={shutdown_seconds}"
-                         f"l={key_labels}v={volumes}m={mounts}cm={core_mounts}senv={svc_env}"
+                         f"l={lbls}v={volumes}m={mounts}cm={core_mounts}senv={svc_env}"
                          f"nodes={field_selector or ''}{label_selector or ''}")
         self.logger.debug(f"{deployment_name} actual change_key: {change_key}")
         change_key = str(hash(change_key))
 
         # Check if a deployment already exists, and if it does check if it has the same change key set
         replace = None
         try:
@@ -790,16 +788,15 @@
                                                  _request_timeout=API_TIMEOUT)
             else:
                 self.api.create_namespaced_secret(namespace=self.namespace, body=new_pull_secret,
                                                   _request_timeout=API_TIMEOUT)
         elif current_pull_secret:
             self.api.delete_namespaced_secret(pull_secret_name, self.namespace, _request_timeout=API_TIMEOUT)
 
-        all_labels = deployment_labels
-        all_labels.update(self._labels)
+        all_labels = dict(self._labels)
         all_labels['component'] = service_name
         if core_mounts:
             all_labels['privilege'] = 'core'
         all_labels.update(labels or {})
 
         # Build set of volumes, first the global mounts, then the core specific ones,
         # then the ones specific to this container only
@@ -835,22 +832,33 @@
                 name="chown-mounts",
                 image=docker_config.image,
                 command=['chown', '-R', '1000:1000'] + [m.mount_path for m in chown_mounts],
                 security_context=V1SecurityContext(run_as_user=0),
                 volume_mounts=chown_mounts
             ))
 
+        pod_os = None
+        security_context = V1PodSecurityContext(fs_group=1000)
+        if docker_config.operating_system:
+            #  Allow Kubernetes to schedule the pod to a compatible node
+            pod_os = V1PodOS(name=docker_config.operating_system)
+
+        if docker_config.operating_system == 'windows':
+            security_context = None
+
+
         pod = V1PodSpec(
             init_containers=init_containers,
             volumes=all_volumes,
             containers=self._create_containers(service_name, deployment_name, docker_config,
                                                all_mounts, core_container=core_mounts),
+            os=pod_os,
             priority_class_name=self.dependency_priority if high_priority else self.priority,
             termination_grace_period_seconds=shutdown_seconds,
-            security_context=V1PodSecurityContext(fs_group=1000),
+            security_context=security_context,
             service_account_name=service_account,
             affinity=selector_to_node_affinity(self.linux_node_selector),
         )
 
         if use_pull_secret:
             pod.image_pull_secrets = [V1LocalObjectReference(name=pull_secret_name)]
 
@@ -1047,15 +1055,14 @@
         if not container_key:
             # No existing instance found
             return
 
         # Generate the expected change key
         senv = sorted(self._service_limited_env[service_name].items())
         labels = [('container', container_name), ('dependency_for', service_name)]
-        labels += sorted([(_v.name, _v.value) for _v in spec.container.labels])
         temp_spec = DependencyConfig(spec.as_primitives())
         volumes, mounts, _ = self._get_volumes_mounts_strategy(deployment_name, container_name, temp_spec)
         temp_spec.container.environment.append(dict(name='AL_INSTANCE_KEY', value=container_key))
         change_key = str(f"n={deployment_name}{change_key}dc={temp_spec.container}ss={30}"
                          f"l={labels}v={volumes}m={mounts}cm={True}senv={senv}")
 
         self.logger.debug(f"{deployment_name} expected change_key: {change_key}")
```

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/scaler/scaler_server.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/scaler/scaler_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,22 +181,22 @@
     def max_instances(self) -> int:
         # Adjust the max_instances based on the number that is already requested
         # this keeps the scaler from running way ahead with its demands when resource caps are reached
         if self._max_instances == 0:
             return self.target_instances + MAX_CONTAINER_ALLOCATION
         return min(self._max_instances, self.target_instances + MAX_CONTAINER_ALLOCATION)
 
-    @max_instances.setter
-    def max_instances(self, value: int):
-        self._max_instances = max(0, value)
-
     @property
     def min_instances(self) -> int:
         return self._min_instances
 
+    @max_instances.setter
+    def max_instances(self, value: int):
+        self._max_instances = max(0, value)
+
     @min_instances.setter
     def min_instances(self, value: int):
         self._min_instances = max(0, value)
 
     def update(self, delta: float, instances: int, backlog: int, duty_cycle: float):
         self.last_update = time.time()
         self.running_instances = instances
@@ -597,16 +597,17 @@
                 # Add the service to the list of services being scaled
                 with self.profiles_lock:
                     min_instances = default_settings.min_instances
                     if service.min_instances is not None:
                         # Use service-specific value if present
                         min_instances = service.min_instances
                     if name not in self.profiles:
-                        self.log.info("Adding %s%s to scaling",
-                                      'privileged ' if service.privileged else '', service.name)
+                        self.log.info(f"Adding "
+                                      f"{f'privileged {service.name}' if service.privileged else service.name}"
+                                      " to scaling")
                         self.add_service(ServiceProfile(
                             name=name,
                             min_instances=min_instances,
                             growth=default_settings.growth,
                             shrink=default_settings.shrink,
                             config_blob=config_blob,
                             dependency_blobs=dependency_blobs,
```

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/server_base.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/server_base.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/signature_client.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/signature_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/submission_client.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/submission_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/tasking_client.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/tasking_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/updater/helper.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/updater/helper.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,103 +8,122 @@
 from assemblyline.odm.models.config import Config as SystemConfig
 from assemblyline.odm.models.service import Service as ServiceConfig
 
 from base64 import b64encode
 from collections import defaultdict
 from logging import Logger
 from packaging.version import parse, Version
+from typing import Any, Dict, List, Tuple
 
 DEFAULT_DOCKER_REGISTRY = "registry.hub.docker.com"
 
 
 class ContainerRegistry():
+    def __init__(self, server, headers: Dict[str, str] = None, verify: bool = True,
+                 proxies: Dict[str, str] = None, *args, **kwargs):
+        self.server = server
+        self.session = requests.Session()
+        self.session.headers = headers
+        self.session.verify = verify
+        self.session.proxies = proxies
+
+    def _make_request(self, path: str) -> Dict[str, Any]:
+        request_path = f"{self.server}{path}"
+        resp = None
+        try:
+            resp = self.session.get(f"https://{request_path}")
+        except requests.exceptions.SSLError:
+            # Connect to insecure registry over HTTP (development only)
+            if not self.session.verify:
+                resp = self.session.get(f"http://{request_path}")
+        # Test for valid response
+        if resp and resp.ok:
+            return resp.json()
+        return None
+
     # Provide a means of obtaining a list of tags from a container registry
-    def _get_proprietary_registry_tags(self, server, image_name, auth, verify, proxies=None, token_server=None):
+    def get_image_tags(self, image_name) -> List[str]:
+        raise NotImplementedError()
+
+    # Provide a means of obtaining the compatible operating system for the container image
+    def get_image_os(self, image_name, image_tag) -> str:
         raise NotImplementedError()
 
 
+class DockerHub(ContainerRegistry):
+    def __init__(self, update_channel, proxies: Dict[str, str] = None, *args, **kwargs):
+        super().__init__(DEFAULT_DOCKER_REGISTRY, None, True, proxies)
+        self.update_channel = update_channel
+
+    def get_image_tags(self, image_name) -> List[str]:
+        resp = self._make_request(f"/v2/repositories/{image_name}/tags?page_size=5&page=1&name={self.update_channel}")
+        if resp:
+            return [x['name'] for x in resp['results']]
+        return []
+
+    def get_image_os(self, image_name, image_tag) -> str:
+        resp = self._make_request(f"/v2/repositories/{image_name}/tags/{image_tag}")
+        if resp:
+            return resp['images'][0]['os']
+        return None
+
+
+# Ref: https://docs.docker.com/registry/spec/api/#detail
 class DockerRegistry(ContainerRegistry):
-    def _get_proprietary_registry_tags(self, server, image_name, auth, verify, proxies=None, token_server=None):
+    def get_image_tags(self, image_name) -> List[str]:
         # Find latest tag for each types
-        url = f"https://{server}/v2/{image_name}/tags/list"
+        resp = self._make_request(f"/v2/{image_name}/tags/list")
+        if resp:
+            return resp['tags'] or []
+        return []
 
-        # Get tag list
-        headers = {}
-        if auth:
-            headers["Authorization"] = auth
-        else:
-            # Retrieve token for authentication: https://distribution.github.io/distribution/spec/auth/token/
+    def get_image_os(self, image_name, image_tag) -> str:
+        resp = self._make_request(f"/v2/{image_name}/manifests/{image_tag}")
+        if resp:
+            # Retrieve OS compatibilty from historical record
+            return json.loads(resp['history'][0]['v1Compatibility'])['os']
 
-            # Assume the token server is the same as the container image registry host if not explicitly set
-            token_server = token_server if token_server else server
-            token_url = f"https://{token_server}/token?scope=repository:{image_name}:pull"
-            resp = requests.get(token_url)
-            if resp.ok:
-                # Request to obtain token was successful, set Authorization header for registry API
-                token = resp.json().get('token')
-                headers["Authorization"] = f"Bearer {token}"
+        # Unable to determine the OS compatibility
+        return None
 
-        resp = None
-        try:
-            resp = requests.get(url, headers=headers, verify=verify, proxies=proxies)
-        except requests.exceptions.SSLError:
-            # Connect to insecure registry over HTTP (development only)
-            if not verify:
-                url = f"http://{server}/v2/{image_name}/tags/list"
-                resp = requests.get(url, headers=headers, verify=verify, proxies=proxies)
-        # Test for valid response
-        if resp and resp.ok:
-            # Test for positive list of tags
-            resp_data = resp.json()
-            return resp_data['tags'] or []
-        return []
 
+# Ref: https://github.com/goharbor/harbor/blob/main/api/v2.0/swagger.yaml
 class HarborRegistry(ContainerRegistry):
-    def _get_proprietary_registry_tags(self, server, image_name, auth, verify, proxies=None, token_server=None):
+    def _get_project_repo_ids(self, image_name) -> Tuple[str, str]:
         # Determine project/repo IDs from image name
         project_id, repo_id = image_name.split('/', 1)
         repo_id = repo_id.replace('/', "%2F")
-        url = f"https://{server}/api/v2.0/projects/{project_id}/repositories/{repo_id}/artifacts?page_size=0"
+        return project_id, repo_id
 
-        headers = {}
-        if auth:
-            headers["Authorization"] = auth
-        else:
-            # Retrieve token for authentication: https://github.com/goharbor/harbor/wiki/Harbor-FAQs#api
+    def get_image_tags(self, image_name) -> List[str]:
+        project_id, repo_id = self._get_project_repo_ids(image_name)
+        resp = self._make_request(f"/api/v2.0/projects/{project_id}/repositories/{repo_id}/artifacts?page_size=0")
+        if resp:
+            return [tag['name'] for image in resp if image['tags'] for tag in image['tags']]
+        return []
 
-            # Assume the token server is the same as the container image registry host if not explicitly set
-            token_server = token_server if token_server else server
-            token_url = f"https://{server}/service/token?scope=repository:{image_name}:pull"
-            resp = requests.get(token_url)
-            if resp.ok:
-                # Request to obtain token was successful, set Authorization header for registry API
-                token = resp.json().get('token')
-                headers["Authorization"] = f"Bearer {token}"
-        resp = None
-        try:
-            resp = requests.get(url, headers=headers, verify=verify, proxies=proxies)
-        except requests.exceptions.SSLError:
-            # Connect to insecure registry over HTTP (development only)
-            if not verify:
-                url = f"http://{server}/api/v2.0/projects/{project_id}/repositories/{repo_id}/artifacts"
-                resp = requests.get(url, headers=headers, verify=verify, proxies=proxies)
+    def get_image_os(self, image_name, image_tag) -> str:
+        project_id, repo_id = self._get_project_repo_ids(image_name)
+        resp = self._make_request(f"/api/v2.0/projects/{project_id}/repositories/{repo_id}/artifacts/{image_tag}")
+        if resp:
+            # Retrieve OS compatibilty from reference
+            return resp['references'][0]['platform']['os']
 
-        if resp and resp.ok:
-            return [tag['name'] for image in resp.json() if image['tags'] for tag in image['tags']]
-        return []
+        # Unable to determine the OS compatibility
+        return None
 
 
 REGISTRY_TYPE_MAPPING = {
-    'docker': DockerRegistry(),
-    'harbor': HarborRegistry()
+    'dockerhub': DockerHub,
+    'docker': DockerRegistry,
+    'harbor': HarborRegistry
 }
 
 
-def get_latest_tag_for_service(
-        service_config: ServiceConfig, system_config: SystemConfig, logger: Logger, prefix: str = ""):
+def get_latest_tag_for_service(service_config: ServiceConfig, system_config: SystemConfig, logger: Logger, prefix: str = ""):
     def process_image(image):
         # Find which server to search in
         server = image.split("/")[0]
         if server != "cccs":
             if ":" in server:
                 image_name = image[len(server) + 1:]
             else:
@@ -146,42 +165,40 @@
                 # Apply the credentials that the system is configured to use with the registry
                 service_config.docker_config.registry_username = registry['username']
                 service_config.docker_config.registry_password = registry['password']
                 service_config.docker_config.registry_type = registry['type']
                 break
 
     if service_config.docker_config.registry_username and service_config.docker_config.registry_password:
-        # We're authenticating using Basic Auth
         auth_config = {
             'username': service_config.docker_config.registry_username,
             'password': service_config.docker_config.registry_password
         }
         upass = f"{service_config.docker_config.registry_username}:{service_config.docker_config.registry_password}"
         auth = f"Basic {b64encode(upass.encode()).decode()}"
-    elif service_config.docker_config.registry_password:
-        # We're assuming that if only a password is given, then this is a token
-        auth = f"Bearer {service_config.docker_config.registry_password}"
 
-    registry = REGISTRY_TYPE_MAPPING[service_config.docker_config.registry_type]
-    token_server = None
     proxies = None
     for reg_conf in system_config.core.updater.registry_configs:
         if reg_conf.name == server:
             proxies = reg_conf.proxies or None
-            token_server = reg_conf.token_server or None
             break
 
-    if server == DEFAULT_DOCKER_REGISTRY:
-        tags = _get_dockerhub_tags(image_name, update_channel, proxies)
-    else:
-        tags = registry._get_proprietary_registry_tags(server, image_name, auth,
-                                                       not system_config.services.allow_insecure_registry,
-                                                       proxies, token_server)
-    tag_name = None
+    registry_type = 'dockerhub' if server == DEFAULT_DOCKER_REGISTRY else service_config.docker_config.registry_type
+    registry_args = {
+        'server': server,
+        'headers': {'Authorization': auth},
+        'verify': not system_config.services.allow_insecure_registry,
+        'proxies': proxies,
+        'update_channel': update_channel
+    }
 
+    registry: ContainerRegistry = REGISTRY_TYPE_MAPPING[registry_type](**registry_args)
+    tags = registry.get_image_tags(image_name)
+
+    tag_name = None
     # Pre-filter tags to only consider 'compatible' tags relative to the running system
     tags = [t for t in tags
             if re.match(f"({FRAMEWORK_VERSION})[.]({SYSTEM_VERSION})[.]\\d+[.]({update_channel})\\d+", t)]
 
     if not tags:
         logger.warning(f"{prefix}Cannot fetch latest tag for service {service_name} - {image_name}"
                        f" => [server: {server}, repo_name: {image_name}, channel: {update_channel}]")
@@ -197,32 +214,14 @@
 
         logger.info(f"{prefix}Latest {service_name} tag on {update_channel.upper()} channel is: {tag_name}")
 
     # Fix service image for use in Kubernetes
     image_variables = defaultdict(str)
     image_variables.update(system_config.services.image_variables)
     image = string.Template(image).safe_substitute(image_variables)
-    server, image_name = process_image(image)
+    os = registry.get_image_os(image_name, tag_name)
 
     # Append server to image if not the default server
-    if server != "registry.hub.docker.com":
+    if server != DEFAULT_DOCKER_REGISTRY:
         image_name = "/".join([server, image_name])
 
-    return image_name, tag_name, auth_config
-
-
-# Default for obtaining tags from DockerHub
-def _get_dockerhub_tags(image_name, update_channel, proxies=None):
-    # Find latest tag for each types
-    url = f"https://{DEFAULT_DOCKER_REGISTRY}/v2/repositories/{image_name}/tags" \
-        f"?page_size=5&page=1&name={update_channel}"
-
-    # Get tag list
-    resp = requests.get(url, proxies=proxies)
-
-    # Test for valid response
-    if resp.ok:
-        # Test for positive list of tags
-        resp_data = resp.json()
-        return [x['name'] for x in resp_data['results']]
-
-    return []
+    return image_name, tag_name, auth_config, os
```

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/updater/run_updater.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/updater/run_updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,18 +472,18 @@
                 try:
                     service = Service(
                         {'name': service_name,
                          'update_channel': self.config.services.preferred_update_channel,
                          'version': tag,
                          'docker_config': {'image': install_data.get('image')}})
 
-                    image_name, tag_name, auth = get_latest_tag_for_service(
+                    image_name, tag_name, auth, os = get_latest_tag_for_service(
                         service,  self.config, self.log, prefix="[CI] ")
 
-                    docker_config = dict(image=f"{image_name}:{tag_name}")
+                    docker_config = dict(image=f"{image_name}:{tag_name}", operating_system=os)
                     if auth:
                         docker_config.update(dict(registry_username=auth['username'],
                                                   registry_password=auth['password']))
 
                     # Apply any container configuration changes specifically for jobs
                     docker_config.update(self.job_dockerconfig)
 
@@ -671,15 +671,15 @@
         while self.running:
             self.log.info("[CV] Checking for new versions of all service containers...")
             existing_services = set(self.container_update.keys()) | set(self.latest_service_tags.keys())
             discovered_services: list[str] = []
 
             for service in self.datastore.list_all_services(full=True):
                 discovered_services.append(service.name)
-                image_name, tag_name, auth = get_latest_tag_for_service(service, self.config, self.log, prefix="[CV] ")
+                image_name, tag_name, auth, _ = get_latest_tag_for_service(service, self.config, self.log, prefix="[CV] ")
                 self.latest_service_tags.set(service.name,
                                              {'auth': auth, 'image': image_name, service.update_channel: tag_name})
 
             # Remove services we have locally or in redis that have been deleted from the database
             for stray_service in existing_services - set(discovered_services):
                 self.log.info(f"[CV] Service updates disabled for {stray_service}")
                 self._service_stage_hash.pop(stray_service)
```

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/vacuum/crawler.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/crawler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/vacuum/department_map.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/department_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/vacuum/safelist.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/safelist.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/vacuum/stream_map.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/stream_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/vacuum/worker.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/vacuum/worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from assemblyline.common.forge import CachedObject, get_classification, get_config, get_datastore, get_filestore, \
     get_apm_client
 from assemblyline.common.codec import decode_file
 from assemblyline.common.dict_utils import flatten
 from assemblyline.common.log import init_logging
 from assemblyline.common.metrics import MetricsFactory
-from assemblyline.datastore.helper import AssemblylineDatastore, MetadataValidator
+from assemblyline.datastore.helper import AssemblylineDatastore
 from assemblyline.common import identify
 from assemblyline.common.isotime import now_as_iso
 from assemblyline.common.uid import get_random_id
 from assemblyline.odm.models import user
 from assemblyline.odm.models.config import Config
 from assemblyline.odm.models.submission import DEFAULT_SRV_SEL
 from assemblyline.odm.models.user_settings import UserSettings
@@ -160,15 +160,14 @@
                  identifier, apm_client=None):
         # Start these worker processes in daemon mode so the OS makes sure they exit when the vacuum process exits.
         super().__init__(daemon=True)
         # Things initialized here will be copied into the new process when it starts.
         # Anything that can't be copied easily should be initialized in 'run'.
         self.config: Config = config
         self.datastore = datastore
-        self.metadata_check = MetadataValidator(datastore)
         self.counter = counter
         self.minimum_classification = self.config.core.vacuum.minimum_classification
         logger.info("Connect to work queue")
         self.queue = NamedQueue(VACUUM_BUFFER_NAME, redis)
         self.worker_id = worker_id
         self.filestore: FileStore = get_filestore()
         self.engine = get_classification()
@@ -266,15 +265,14 @@
 
         # Ignore external sources
         settings.pop('default_external_sources', None)
 
         # Remove UI specific params
         settings.pop('default_zip_password', None)
         settings.pop('download_encoding', None)
-        settings.pop('executive_summary', None)
         settings.pop('expand_min_score', None)
         settings.pop('submission_view', None)
         settings.pop('ui4', None)
         settings.pop('ui4_ask', None)
         return settings
 
     def timed(self, name):
@@ -492,34 +490,24 @@
 
                 # Set ingest type
                 s_params['type'] = self.config.core.vacuum.ingest_type
 
                 # Extract email body strings or similar password settings
                 password_strings = metadata.pop("email_strings", [])
                 if not isinstance(password_strings, list):
-                    logger.warning("Unsupported password list format: %s", password_strings)
+                    logger.warning("Unsupported password list format: " + str(password_strings))
                     password_strings = []
 
                 if password_strings:
                     init_data = json.dumps(dict(passwords=password_strings))
                     s_params['initial_data'] = init_data
 
                 # Set description if it does not exists
                 s_params['description'] = f"[{s_params['type']}] Inspection of file: {file_sha256}"
 
-                # Validate the metadata
-                while metadata:
-                    metadata_error = self.metadata_check.check_metadata(metadata)
-                    if metadata_error:
-                        logger.error("Could not accept metadata %s on %s: %s", metadata_error[0],
-                                     file_sha256, metadata_error[1])
-                        metadata.pop(metadata_error[0], None)
-                    else:
-                        break
-
                 # Create submission object
                 try:
                     submission_obj = Submission({
                         "sid": ingest_id,
                         "files": [{
                             'name': metadata.get('filename', file_sha256),
                             'sha256': file_sha256,
```

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core/workflow/run_workflow.py` & `assemblyline-core-4.5.1.dev8/assemblyline_core/workflow/run_workflow.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core.egg-info/PKG-INFO` & `assemblyline-core-4.5.1.dev8/assemblyline_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline-core
-Version: 4.5.1.dev76
+Version: 4.5.1.dev8
 Summary: Assemblyline 4 - Core components
 Home-page: https://github.com/CybercentreCanada/assemblyline-core/
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `assemblyline-core-4.5.1.dev76/assemblyline_core.egg-info/SOURCES.txt` & `assemblyline-core-4.5.1.dev8/assemblyline_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/setup.py` & `assemblyline-core-4.5.1.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/test/test_alerter.py` & `assemblyline-core-4.5.1.dev8/test/test_alerter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/test/test_badlist_client.py` & `assemblyline-core-4.5.1.dev8/test/test_badlist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/test/test_dispatcher.py` & `assemblyline-core-4.5.1.dev8/test/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/test/test_expiry.py` & `assemblyline-core-4.5.1.dev8/test/test_expiry.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/test/test_plumber.py` & `assemblyline-core-4.5.1.dev8/test/test_plumber.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/test/test_replay.py` & `assemblyline-core-4.5.1.dev8/test/test_replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/test/test_safelist_client.py` & `assemblyline-core-4.5.1.dev8/test/test_safelist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/test/test_scaler.py` & `assemblyline-core-4.5.1.dev8/test/test_scaler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/test/test_scheduler.py` & `assemblyline-core-4.5.1.dev8/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/test/test_signature_client.py` & `assemblyline-core-4.5.1.dev8/test/test_signature_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/test/test_simulation.py` & `assemblyline-core-4.5.1.dev8/test/test_simulation.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/test/test_vacuum.py` & `assemblyline-core-4.5.1.dev8/test/test_vacuum.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/test/test_worker_ingest.py` & `assemblyline-core-4.5.1.dev8/test/test_worker_ingest.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev76/test/test_worker_submit.py` & `assemblyline-core-4.5.1.dev8/test/test_worker_submit.py`

 * *Files identical despite different names*

