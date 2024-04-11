# Comparing `tmp/bec-server-1.9.0.tar.gz` & `tmp/bec-server-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec-server-1.9.0.tar", last modified: Thu Feb 22 19:50:23 2024, max compression
+gzip compressed data, was "bec-server-2.0.1.tar", last modified: Thu Apr 11 06:21:55 2024, max compression
```

## Comparing `bec-server-1.9.0.tar` & `bec-server-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,100 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:23.031110 bec-server-1.9.0/
--rw-r--r--   0 root         (0) root         (0)      442 2024-02-22 19:50:23.031110 bec-server-1.9.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:23.031110 bec-server-1.9.0/bec_server/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-02-22 18:57:01.000000 bec-server-1.9.0/bec_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2024-02-22 18:57:01.000000 bec-server-1.9.0/bec_server/launch.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2024-02-22 18:57:01.000000 bec-server-1.9.0/bec_server/service_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     2845 2024-02-22 18:57:01.000000 bec-server-1.9.0/bec_server/tmux_launch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:23.031110 bec-server-1.9.0/bec_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      442 2024-02-22 19:50:23.000000 bec-server-1.9.0/bec_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      332 2024-02-22 19:50:23.000000 bec-server-1.9.0/bec_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 19:50:23.000000 bec-server-1.9.0/bec_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-02-22 19:50:23.000000 bec-server-1.9.0/bec_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      192 2024-02-22 19:50:23.000000 bec-server-1.9.0/bec_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-02-22 19:50:23.000000 bec-server-1.9.0/bec_server.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      503 2024-02-22 19:50:23.035110 bec-server-1.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2184 2024-02-22 19:50:16.000000 bec-server-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.544478 bec-server-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)      398 2024-04-11 06:21:55.544478 bec-server-2.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 06:21:44.000000 bec-server-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.538478 bec-server-2.0.1/bec_server/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.539478 bec-server-2.0.1/bec_server/bec_server_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 06:21:44.000000 bec-server-2.0.1/bec_server/bec_server_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1856 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/bec_server_utils/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)     3445 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/bec_server_utils/service_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/bec_server_utils/subprocess_launch.py
+-rw-rw-rw-   0 root         (0) root         (0)     2845 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/bec_server_utils/tmux_launch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.539478 bec-server-2.0.1/bec_server/data_processing/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/data_processing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.539478 bec-server-2.0.1/bec_server/data_processing/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 06:21:44.000000 bec-server-2.0.1/bec_server/data_processing/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/data_processing/cli/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/data_processing/dap_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     4891 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/data_processing/dap_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     9648 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/data_processing/dap_service_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    12174 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/data_processing/lmfit1d_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.539478 bec-server-2.0.1/bec_server/device_server/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/device_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.540478 bec-server-2.0.1/bec_server/device_server/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 06:21:44.000000 bec-server-2.0.1/bec_server/device_server/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1149 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/device_server/cli/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)    18964 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/device_server/device_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.540478 bec-server-2.0.1/bec_server/device_server/devices/
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/device_server/devices/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/device_server/devices/config_update_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     5026 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/device_server/devices/device_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)    23444 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/device_server/devices/devicemanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     7707 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/device_server/rpc_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.540478 bec-server-2.0.1/bec_server/file_writer/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/file_writer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.540478 bec-server-2.0.1/bec_server/file_writer/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 06:21:44.000000 bec-server-2.0.1/bec_server/file_writer/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      926 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/file_writer/cli/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)    11717 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/file_writer/file_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)    11359 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/file_writer/file_writer_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/file_writer/merged_dicts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.541478 bec-server-2.0.1/bec_server/file_writer_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/file_writer_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22190 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/file_writer_plugins/cSAXS.py
+-rw-rw-rw-   0 root         (0) root         (0)     3016 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/file_writer_plugins/default_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.541478 bec-server-2.0.1/bec_server/scan_bundler/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_bundler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_bundler/bec_emitter.py
+-rw-rw-rw-   0 root         (0) root         (0)     5049 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_bundler/bluesky_emitter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.541478 bec-server-2.0.1/bec_server/scan_bundler/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 06:21:44.000000 bec-server-2.0.1/bec_server/scan_bundler/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      764 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_bundler/cli/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)     2144 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_bundler/emitter.py
+-rw-rw-rw-   0 root         (0) root         (0)    15950 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_bundler/scan_bundler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.542478 bec-server-2.0.1/bec_server/scan_server/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.542478 bec-server-2.0.1/bec_server/scan_server/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 06:21:44.000000 bec-server-2.0.1/bec_server/scan_server/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      880 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_server/cli/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)     6531 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_server/device_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_server/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3489 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_server/path_optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)     2075 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_server/scan_assembler.py
+-rw-rw-rw-   0 root         (0) root         (0)     6354 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_server/scan_guard.py
+-rw-rw-rw-   0 root         (0) root         (0)     4114 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_server/scan_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.543478 bec-server-2.0.1/bec_server/scan_server/scan_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)    21424 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_server/scan_plugins/LamNIFermatScan.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_server/scan_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13216 2024-04-11 01:23:09.000000 bec-server-2.0.1/bec_server/scan_server/scan_plugins/flomni_fermat_scan.py
+-rw-rw-rw-   0 root         (0) root         (0)     6379 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_server/scan_plugins/otf_scan.py
+-rw-rw-rw-   0 root         (0) root         (0)    13056 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_server/scan_plugins/owis_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)     9086 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_server/scan_plugins/sgalil_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)    34791 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_server/scan_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     4173 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_server/scan_server.py
+-rw-rw-rw-   0 root         (0) root         (0)    18416 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_server/scan_stubs.py
+-rw-rw-rw-   0 root         (0) root         (0)    35666 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_server/scan_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)    52578 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scan_server/scans.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.543478 bec-server-2.0.1/bec_server/scihub/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scihub/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.543478 bec-server-2.0.1/bec_server/scihub/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 06:21:44.000000 bec-server-2.0.1/bec_server/scihub/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      757 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scihub/cli/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scihub/repeated_timer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.543478 bec-server-2.0.1/bec_server/scihub/scibec/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scihub/scibec/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8519 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scihub/scibec/config_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7549 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scihub/scibec/scibec_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)    10557 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scihub/scibec/scibec_metadata_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scihub/scihub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.543478 bec-server-2.0.1/bec_server/scihub/scilog/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scihub/scilog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2698 2024-04-10 19:08:49.000000 bec-server-2.0.1/bec_server/scihub/scilog/scilog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.544478 bec-server-2.0.1/bec_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      398 2024-04-11 06:21:55.000000 bec-server-2.0.1/bec_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3204 2024-04-11 06:21:55.000000 bec-server-2.0.1/bec_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 06:21:55.000000 bec-server-2.0.1/bec_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      315 2024-04-11 06:21:55.000000 bec-server-2.0.1/bec_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      201 2024-04-11 06:21:55.000000 bec-server-2.0.1/bec_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-11 06:21:55.000000 bec-server-2.0.1/bec_server.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      504 2024-04-11 06:21:55.545478 bec-server-2.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2024-04-11 06:21:52.000000 bec-server-2.0.1/setup.py
```

### Comparing `bec-server-1.9.0/bec_server/service_handler.py` & `bec-server-2.0.1/bec_server/bec_server_utils/service_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 from string import Template
 
-from bec_server.tmux_launch import tmux_start, tmux_stop
+from bec_server.bec_server_utils.subprocess_launch import subprocess_start, subprocess_stop
+from bec_server.bec_server_utils.tmux_launch import tmux_start, tmux_stop
 
 
 class bcolors:
     """
     Colors for the terminal output.
     """
 
@@ -23,45 +24,46 @@
 class ServiceHandler:
     """
     Service handler for the BEC server. This class is used to start, stop and restart the BEC server.
     Depending on the platform, the server is launched in a tmux session or in an iTerm2 session.
     """
 
     SERVICES = {
-        "scan_server": {
-            "path": Template("$base_path/scan_server"),
-            "command": "bec-scan-server",
-        },
+        "scan_server": {"path": Template("$base_path/scan_server"), "command": "bec-scan-server"},
         "scan_bundler": {
             "path": Template("$base_path/scan_bundler"),
             "command": "bec-scan-bundler",
         },
         "device_server": {
             "path": Template("$base_path/device_server"),
             "command": "bec-device-server",
         },
         "file_writer": {"path": Template("$base_path/file_writer"), "command": "bec-file-writer"},
         "scihub": {"path": Template("$base_path/scihub"), "command": "bec-scihub"},
         "data_processing": {"path": Template("$base_path/data_processing"), "command": "bec-dap"},
     }
 
-    def __init__(self, bec_path: str, config_path: str):
+    def __init__(self, bec_path: str, config_path: str, no_tmux: bool = False):
         """
 
         Args:
             bec_path (str): Path to the BEC source code
             config_path (str): Path to the config file
 
         """
         self.bec_path = bec_path
         self.config_path = config_path
+        self.no_tmux = no_tmux
 
         self._detect_available_interfaces()
 
     def _detect_available_interfaces(self):
+        if self.no_tmux:
+            self.interface = None
+            return
         # check if we are on MacOS and if so, check if we have iTerm2 installed
         if sys.platform == "darwin":
             try:
                 import iterm2
             except ImportError:
                 self.interface = "tmux"
             else:
@@ -79,24 +81,29 @@
             print("Starting BEC server using tmux...")
             tmux_start(self.bec_path, self.config_path, self.SERVICES)
             print(
                 f"{bcolors.OKCYAN}{bcolors.BOLD}Use `tmux attach -t bec` to attach to the BEC server. Once connected, use `ctrl+b d` to detach again."
             )
         elif self.interface == "iterm2":
             pass
+        else:
+            # no tmux
+            return subprocess_start(self.bec_path, self.config_path, self.SERVICES)
 
     def stop(self):
         """
         Stop the BEC server using the available interface.
         """
         print("Stopping BEC server...")
         if self.interface == "tmux":
             tmux_stop()
         elif self.interface == "iterm2":
             pass
+        else:
+            subprocess_stop()
 
     def restart(self):
         """
         Restart the BEC server using the available interface.
         """
         print("Restarting BEC server...")
         self.stop()
```

### Comparing `bec-server-1.9.0/bec_server/tmux_launch.py` & `bec-server-2.0.1/bec_server/bec_server_utils/tmux_launch.py`

 * *Files identical despite different names*

