# Comparing `tmp/bec-server-2.0.2.tar.gz` & `tmp/bec-server-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec-server-2.0.2.tar", last modified: Thu Apr 11 08:36:44 2024, max compression
+gzip compressed data, was "bec-server-2.0.3.tar", last modified: Thu Apr 11 12:57:35 2024, max compression
```

## Comparing `bec-server-2.0.2.tar` & `bec-server-2.0.3.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.980550 bec-server-2.0.2/
--rw-r--r--   0 root         (0) root         (0)      398 2024-04-11 08:36:44.980550 bec-server-2.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 08:36:34.000000 bec-server-2.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.974549 bec-server-2.0.2/bec_server/
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.975549 bec-server-2.0.2/bec_server/bec_server_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 08:36:34.000000 bec-server-2.0.2/bec_server/bec_server_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1856 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/bec_server_utils/launch.py
--rw-rw-rw-   0 root         (0) root         (0)     3445 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/bec_server_utils/service_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1043 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/bec_server_utils/subprocess_launch.py
--rw-rw-rw-   0 root         (0) root         (0)     2845 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/bec_server_utils/tmux_launch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.975549 bec-server-2.0.2/bec_server/data_processing/
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/data_processing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.975549 bec-server-2.0.2/bec_server/data_processing/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 08:36:34.000000 bec-server-2.0.2/bec_server/data_processing/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1086 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/data_processing/cli/launch.py
--rw-rw-rw-   0 root         (0) root         (0)     1371 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/data_processing/dap_server.py
--rw-rw-rw-   0 root         (0) root         (0)     4891 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/data_processing/dap_service.py
--rw-rw-rw-   0 root         (0) root         (0)     9648 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/data_processing/dap_service_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    12174 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/data_processing/lmfit1d_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.975549 bec-server-2.0.2/bec_server/device_server/
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/device_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.976549 bec-server-2.0.2/bec_server/device_server/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 08:36:34.000000 bec-server-2.0.2/bec_server/device_server/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1149 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/device_server/cli/launch.py
--rw-rw-rw-   0 root         (0) root         (0)    18964 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/device_server/device_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.976549 bec-server-2.0.2/bec_server/device_server/devices/
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/device_server/devices/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/device_server/devices/config_update_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     5026 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/device_server/devices/device_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)    23444 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/device_server/devices/devicemanager.py
--rw-rw-rw-   0 root         (0) root         (0)     7707 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/device_server/rpc_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.976549 bec-server-2.0.2/bec_server/file_writer/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/file_writer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.976549 bec-server-2.0.2/bec_server/file_writer/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 08:36:34.000000 bec-server-2.0.2/bec_server/file_writer/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      926 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/file_writer/cli/launch.py
--rw-rw-rw-   0 root         (0) root         (0)    11717 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/file_writer/file_writer.py
--rw-rw-rw-   0 root         (0) root         (0)    11359 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/file_writer/file_writer_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1531 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/file_writer/merged_dicts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.976549 bec-server-2.0.2/bec_server/file_writer_plugins/
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/file_writer_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22190 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/file_writer_plugins/cSAXS.py
--rw-rw-rw-   0 root         (0) root         (0)     3016 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/file_writer_plugins/default_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.977549 bec-server-2.0.2/bec_server/scan_bundler/
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_bundler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1889 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_bundler/bec_emitter.py
--rw-rw-rw-   0 root         (0) root         (0)     5049 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_bundler/bluesky_emitter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.977549 bec-server-2.0.2/bec_server/scan_bundler/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 08:36:34.000000 bec-server-2.0.2/bec_server/scan_bundler/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      764 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_bundler/cli/launch.py
--rw-rw-rw-   0 root         (0) root         (0)     2144 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_bundler/emitter.py
--rw-rw-rw-   0 root         (0) root         (0)    15950 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_bundler/scan_bundler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.978550 bec-server-2.0.2/bec_server/scan_server/
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.978550 bec-server-2.0.2/bec_server/scan_server/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 08:36:34.000000 bec-server-2.0.2/bec_server/scan_server/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      880 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/cli/launch.py
--rw-rw-rw-   0 root         (0) root         (0)     6531 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/device_validation.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     3489 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/path_optimization.py
--rw-rw-rw-   0 root         (0) root         (0)     2075 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/scan_assembler.py
--rw-rw-rw-   0 root         (0) root         (0)     6354 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/scan_guard.py
--rw-rw-rw-   0 root         (0) root         (0)     4114 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/scan_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.978550 bec-server-2.0.2/bec_server/scan_server/scan_plugins/
--rw-rw-rw-   0 root         (0) root         (0)    21424 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/scan_plugins/LamNIFermatScan.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/scan_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13216 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/scan_plugins/flomni_fermat_scan.py
--rw-rw-rw-   0 root         (0) root         (0)     6379 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/scan_plugins/otf_scan.py
--rw-rw-rw-   0 root         (0) root         (0)    13056 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/scan_plugins/owis_grid.py
--rw-rw-rw-   0 root         (0) root         (0)     9086 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/scan_plugins/sgalil_grid.py
--rw-rw-rw-   0 root         (0) root         (0)    34791 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/scan_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     4173 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/scan_server.py
--rw-rw-rw-   0 root         (0) root         (0)    18416 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/scan_stubs.py
--rw-rw-rw-   0 root         (0) root         (0)    35666 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/scan_worker.py
--rw-rw-rw-   0 root         (0) root         (0)    52578 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scan_server/scans.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.979550 bec-server-2.0.2/bec_server/scihub/
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scihub/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.979550 bec-server-2.0.2/bec_server/scihub/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 08:36:34.000000 bec-server-2.0.2/bec_server/scihub/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      757 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scihub/cli/launch.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scihub/repeated_timer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.979550 bec-server-2.0.2/bec_server/scihub/scibec/
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scihub/scibec/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8519 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scihub/scibec/config_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     7549 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scihub/scibec/scibec_connector.py
--rw-rw-rw-   0 root         (0) root         (0)    10557 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scihub/scibec/scibec_metadata_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1086 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scihub/scihub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.979550 bec-server-2.0.2/bec_server/scihub/scilog/
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scihub/scilog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2698 2024-04-11 01:29:15.000000 bec-server-2.0.2/bec_server/scihub/scilog/scilog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.980550 bec-server-2.0.2/bec_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      398 2024-04-11 08:36:44.000000 bec-server-2.0.2/bec_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3204 2024-04-11 08:36:44.000000 bec-server-2.0.2/bec_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 08:36:44.000000 bec-server-2.0.2/bec_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      315 2024-04-11 08:36:44.000000 bec-server-2.0.2/bec_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      201 2024-04-11 08:36:44.000000 bec-server-2.0.2/bec_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-11 08:36:44.000000 bec-server-2.0.2/bec_server.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      504 2024-04-11 08:36:44.981550 bec-server-2.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1371 2024-04-11 08:36:42.000000 bec-server-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.888479 bec-server-2.0.3/
+-rw-r--r--   0 root         (0) root         (0)      398 2024-04-11 12:57:35.888479 bec-server-2.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:57:24.000000 bec-server-2.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.883479 bec-server-2.0.3/bec_server/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.883479 bec-server-2.0.3/bec_server/bec_server_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:57:24.000000 bec-server-2.0.3/bec_server/bec_server_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1856 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/bec_server_utils/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)     3445 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/bec_server_utils/service_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/bec_server_utils/subprocess_launch.py
+-rw-rw-rw-   0 root         (0) root         (0)     2845 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/bec_server_utils/tmux_launch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.884479 bec-server-2.0.3/bec_server/data_processing/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/data_processing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.884479 bec-server-2.0.3/bec_server/data_processing/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:57:24.000000 bec-server-2.0.3/bec_server/data_processing/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2024-04-11 12:55:21.000000 bec-server-2.0.3/bec_server/data_processing/cli/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/data_processing/dap_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     4891 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/data_processing/dap_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     9648 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/data_processing/dap_service_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    12174 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/data_processing/lmfit1d_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.884479 bec-server-2.0.3/bec_server/device_server/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/device_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.884479 bec-server-2.0.3/bec_server/device_server/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:57:24.000000 bec-server-2.0.3/bec_server/device_server/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2024-04-11 12:55:21.000000 bec-server-2.0.3/bec_server/device_server/cli/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)    18964 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/device_server/device_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.884479 bec-server-2.0.3/bec_server/device_server/devices/
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/device_server/devices/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/device_server/devices/config_update_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     5026 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/device_server/devices/device_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)    23444 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/device_server/devices/devicemanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     7707 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/device_server/rpc_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.885479 bec-server-2.0.3/bec_server/file_writer/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/file_writer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.885479 bec-server-2.0.3/bec_server/file_writer/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:57:24.000000 bec-server-2.0.3/bec_server/file_writer/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2024-04-11 12:55:21.000000 bec-server-2.0.3/bec_server/file_writer/cli/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)    11717 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/file_writer/file_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)    11359 2024-04-11 12:55:21.000000 bec-server-2.0.3/bec_server/file_writer/file_writer_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/file_writer/merged_dicts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.885479 bec-server-2.0.3/bec_server/file_writer_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/file_writer_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22190 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/file_writer_plugins/cSAXS.py
+-rw-rw-rw-   0 root         (0) root         (0)     3016 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/file_writer_plugins/default_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.885479 bec-server-2.0.3/bec_server/scan_bundler/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_bundler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_bundler/bec_emitter.py
+-rw-rw-rw-   0 root         (0) root         (0)     5049 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_bundler/bluesky_emitter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.885479 bec-server-2.0.3/bec_server/scan_bundler/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:57:24.000000 bec-server-2.0.3/bec_server/scan_bundler/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      992 2024-04-11 12:55:21.000000 bec-server-2.0.3/bec_server/scan_bundler/cli/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)     2144 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_bundler/emitter.py
+-rw-rw-rw-   0 root         (0) root         (0)    15950 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_bundler/scan_bundler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.887479 bec-server-2.0.3/bec_server/scan_server/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.887479 bec-server-2.0.3/bec_server/scan_server/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:57:24.000000 bec-server-2.0.3/bec_server/scan_server/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-04-11 12:55:21.000000 bec-server-2.0.3/bec_server/scan_server/cli/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)     6531 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_server/device_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_server/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3489 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_server/path_optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)     2075 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_server/scan_assembler.py
+-rw-rw-rw-   0 root         (0) root         (0)     6354 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_server/scan_guard.py
+-rw-rw-rw-   0 root         (0) root         (0)     4114 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_server/scan_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.887479 bec-server-2.0.3/bec_server/scan_server/scan_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)    21424 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_server/scan_plugins/LamNIFermatScan.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_server/scan_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13216 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_server/scan_plugins/flomni_fermat_scan.py
+-rw-rw-rw-   0 root         (0) root         (0)     6379 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_server/scan_plugins/otf_scan.py
+-rw-rw-rw-   0 root         (0) root         (0)    13056 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_server/scan_plugins/owis_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)     9086 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_server/scan_plugins/sgalil_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)    34791 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_server/scan_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     4173 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_server/scan_server.py
+-rw-rw-rw-   0 root         (0) root         (0)    18416 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_server/scan_stubs.py
+-rw-rw-rw-   0 root         (0) root         (0)    35666 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_server/scan_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)    52578 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scan_server/scans.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.887479 bec-server-2.0.3/bec_server/scihub/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scihub/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.888479 bec-server-2.0.3/bec_server/scihub/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:57:24.000000 bec-server-2.0.3/bec_server/scihub/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2024-04-11 12:55:21.000000 bec-server-2.0.3/bec_server/scihub/cli/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scihub/repeated_timer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.888479 bec-server-2.0.3/bec_server/scihub/scibec/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scihub/scibec/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8519 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scihub/scibec/config_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7549 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scihub/scibec/scibec_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)    10557 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scihub/scibec/scibec_metadata_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scihub/scihub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.888479 bec-server-2.0.3/bec_server/scihub/scilog/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scihub/scilog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2698 2024-04-11 12:42:13.000000 bec-server-2.0.3/bec_server/scihub/scilog/scilog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.888479 bec-server-2.0.3/bec_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      398 2024-04-11 12:57:35.000000 bec-server-2.0.3/bec_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3204 2024-04-11 12:57:35.000000 bec-server-2.0.3/bec_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 12:57:35.000000 bec-server-2.0.3/bec_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      315 2024-04-11 12:57:35.000000 bec-server-2.0.3/bec_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      201 2024-04-11 12:57:35.000000 bec-server-2.0.3/bec_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-11 12:57:35.000000 bec-server-2.0.3/bec_server.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      504 2024-04-11 12:57:35.892480 bec-server-2.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2024-04-11 12:57:33.000000 bec-server-2.0.3/setup.py
```

### Comparing `bec-server-2.0.2/bec_server/bec_server_utils/launch.py` & `bec-server-2.0.3/bec_server/bec_server_utils/launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/bec_server_utils/service_handler.py` & `bec-server-2.0.3/bec_server/bec_server_utils/service_handler.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/bec_server_utils/subprocess_launch.py` & `bec-server-2.0.3/bec_server/bec_server_utils/subprocess_launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/bec_server_utils/tmux_launch.py` & `bec-server-2.0.3/bec_server/bec_server_utils/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/data_processing/dap_server.py` & `bec-server-2.0.3/bec_server/data_processing/dap_server.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/data_processing/dap_service.py` & `bec-server-2.0.3/bec_server/data_processing/dap_service.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/data_processing/dap_service_manager.py` & `bec-server-2.0.3/bec_server/data_processing/dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/data_processing/lmfit1d_service.py` & `bec-server-2.0.3/bec_server/data_processing/lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/device_server/cli/launch.py` & `bec-server-2.0.3/bec_server/device_server/cli/launch.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# This file is the entry point for the BEC device server. It is responsible for
+# launching the device server and handling command line arguments.
+# It is called either by the bec-device-server entry point or directly from the command line.
+
 # pylint: disable=wrong-import-position
 # pylint: disable=wrong-import-order
 # we need to run the startup script before we import anything else. This is
 # to ensure that the epics environment variables are set correctly.
 
 try:
     from bec_plugins.device_server import startup
@@ -37,7 +41,11 @@
     try:
         event = threading.Event()
         s.start()
         logger.success("Started DeviceServer")
         event.wait()
     except KeyboardInterrupt:
         s.shutdown()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `bec-server-2.0.2/bec_server/device_server/device_server.py` & `bec-server-2.0.3/bec_server/device_server/device_server.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/device_server/devices/config_update_handler.py` & `bec-server-2.0.3/bec_server/device_server/devices/config_update_handler.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/device_server/devices/device_serializer.py` & `bec-server-2.0.3/bec_server/device_server/devices/device_serializer.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/device_server/devices/devicemanager.py` & `bec-server-2.0.3/bec_server/device_server/devices/devicemanager.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/device_server/rpc_mixin.py` & `bec-server-2.0.3/bec_server/device_server/rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/file_writer/file_writer.py` & `bec-server-2.0.3/bec_server/file_writer/file_writer.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/file_writer/file_writer_manager.py` & `bec-server-2.0.3/bec_server/file_writer/file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/file_writer/merged_dicts.py` & `bec-server-2.0.3/bec_server/file_writer/merged_dicts.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/file_writer_plugins/cSAXS.py` & `bec-server-2.0.3/bec_server/file_writer_plugins/cSAXS.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/file_writer_plugins/default_writer.py` & `bec-server-2.0.3/bec_server/file_writer_plugins/default_writer.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_bundler/bec_emitter.py` & `bec-server-2.0.3/bec_server/scan_bundler/bec_emitter.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_bundler/bluesky_emitter.py` & `bec-server-2.0.3/bec_server/scan_bundler/bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_bundler/cli/launch.py` & `bec-server-2.0.3/bec_server/scan_bundler/cli/launch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Description: Launch the scan bundler.
+# This script is the entry point for the Scan Bundler. It is called either
+# by the bec-scan-bundler entry point or directly from the command line.
 import argparse
 import threading
 
 from bec_lib import RedisConnector, ServiceConfig, bec_logger
 from bec_server import scan_bundler
 
 logger = bec_logger.logger
@@ -23,7 +26,11 @@
 
     try:
         event = threading.Event()
         logger.success("Started ScanBundler")
         event.wait()
     except KeyboardInterrupt:
         sb.shutdown()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `bec-server-2.0.2/bec_server/scan_bundler/emitter.py` & `bec-server-2.0.3/bec_server/scan_bundler/emitter.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_bundler/scan_bundler.py` & `bec-server-2.0.3/bec_server/scan_bundler/scan_bundler.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_server/cli/launch.py` & `bec-server-2.0.3/bec_server/scan_server/cli/launch.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# This file is the entry point for the Scan Server.
+# It is called either by the bec-scan-server entry point or directly from the command line.
+
 import argparse
 import threading
 
 from bec_lib import RedisConnector, ServiceConfig, bec_logger
 from bec_server import scan_server
 
 logger = bec_logger.logger
@@ -25,7 +28,11 @@
         # pylint: disable=E1102
         logger.success("Started ScanServer")
         event.wait()
     except KeyboardInterrupt as e:
         bec_server.shutdown()
         event.set()
         raise e
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `bec-server-2.0.2/bec_server/scan_server/device_validation.py` & `bec-server-2.0.3/bec_server/scan_server/device_validation.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_server/path_optimization.py` & `bec-server-2.0.3/bec_server/scan_server/path_optimization.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_server/scan_assembler.py` & `bec-server-2.0.3/bec_server/scan_server/scan_assembler.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_server/scan_guard.py` & `bec-server-2.0.3/bec_server/scan_server/scan_guard.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_server/scan_manager.py` & `bec-server-2.0.3/bec_server/scan_server/scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_server/scan_plugins/LamNIFermatScan.py` & `bec-server-2.0.3/bec_server/scan_server/scan_plugins/LamNIFermatScan.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_server/scan_plugins/flomni_fermat_scan.py` & `bec-server-2.0.3/bec_server/scan_server/scan_plugins/flomni_fermat_scan.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_server/scan_plugins/otf_scan.py` & `bec-server-2.0.3/bec_server/scan_server/scan_plugins/otf_scan.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_server/scan_plugins/owis_grid.py` & `bec-server-2.0.3/bec_server/scan_server/scan_plugins/owis_grid.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_server/scan_plugins/sgalil_grid.py` & `bec-server-2.0.3/bec_server/scan_server/scan_plugins/sgalil_grid.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_server/scan_queue.py` & `bec-server-2.0.3/bec_server/scan_server/scan_queue.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_server/scan_server.py` & `bec-server-2.0.3/bec_server/scan_server/scan_server.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_server/scan_stubs.py` & `bec-server-2.0.3/bec_server/scan_server/scan_stubs.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_server/scan_worker.py` & `bec-server-2.0.3/bec_server/scan_server/scan_worker.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scan_server/scans.py` & `bec-server-2.0.3/bec_server/scan_server/scans.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scihub/repeated_timer.py` & `bec-server-2.0.3/bec_server/scihub/repeated_timer.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scihub/scibec/config_handler.py` & `bec-server-2.0.3/bec_server/scihub/scibec/config_handler.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scihub/scibec/scibec_connector.py` & `bec-server-2.0.3/bec_server/scihub/scibec/scibec_connector.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scihub/scibec/scibec_metadata_handler.py` & `bec-server-2.0.3/bec_server/scihub/scibec/scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scihub/scihub.py` & `bec-server-2.0.3/bec_server/scihub/scihub.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server/scihub/scilog/scilog.py` & `bec-server-2.0.3/bec_server/scihub/scilog/scilog.py`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/bec_server.egg-info/SOURCES.txt` & `bec-server-2.0.3/bec_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec-server-2.0.2/setup.py` & `bec-server-2.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
-__version__ = "2.0.2"
+__version__ = "2.0.3"
 
 
 if __name__ == "__main__":
     setup(
         install_requires=[
             "bec-lib",
             "cytoolz",
```

