# Comparing `tmp/bec_lib-2.0.3.tar.gz` & `tmp/bec_lib-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_lib-2.0.3.tar", last modified: Thu Apr 11 12:57:35 2024, max compression
+gzip compressed data, was "bec_lib-2.1.0.tar", last modified: Thu Apr 11 16:31:31 2024, max compression
```

## Comparing `bec_lib-2.0.3.tar` & `bec_lib-2.1.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.465441 bec_lib-2.0.3/
--rw-r--r--   0 root         (0) root         (0)     3013 2024-04-11 12:57:35.466441 bec_lib-2.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2616 2024-04-11 12:02:54.000000 bec_lib-2.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.464441 bec_lib-2.0.3/bec_lib/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3901 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/alarm_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     3663 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/async_data.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/bec_errors.py
--rw-rw-rw-   0 root         (0) root         (0)    16590 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/bec_plotter.py
--rw-rw-rw-   0 root         (0) root         (0)    11292 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/bec_service.py
--rw-rw-rw-   0 root         (0) root         (0)     7247 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/bl_checks.py
--rw-rw-rw-   0 root         (0) root         (0)     2426 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/bl_conditions.py
--rw-rw-rw-   0 root         (0) root         (0)     5952 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/callback_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/channel_monitor.py
--rw-rw-rw-   0 root         (0) root         (0)     9024 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/client.py
--rw-rw-rw-   0 root         (0) root         (0)     9055 2024-04-11 12:42:13.000000 bec_lib-2.0.3/bec_lib/config_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.464441 bec_lib-2.0.3/bec_lib/configs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:57:24.000000 bec_lib-2.0.3/bec_lib/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    38908 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/configs/demo_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)   289604 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/configs/openapi_schema.json
--rw-rw-rw-   0 root         (0) root         (0)     4461 2024-04-11 12:55:21.000000 bec_lib-2.0.3/bec_lib/connector.py
--rw-rw-rw-   0 root         (0) root         (0)    12816 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/dap_plugin_objects.py
--rw-rw-rw-   0 root         (0) root         (0)     3935 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/dap_plugins.py
--rw-rw-rw-   0 root         (0) root         (0)    30828 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/device.py
--rw-rw-rw-   0 root         (0) root         (0)    23274 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/devicemanager.py
--rw-rw-rw-   0 root         (0) root         (0)    37595 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/endpoints.py
--rw-rw-rw-   0 root         (0) root         (0)     9233 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/file_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/lmfit_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2546 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/logbook_connector.py
--rw-rw-rw-   0 root         (0) root         (0)     6959 2024-04-11 12:42:13.000000 bec_lib-2.0.3/bec_lib/logger.py
--rw-rw-rw-   0 root         (0) root         (0)    20005 2024-04-11 12:42:13.000000 bec_lib-2.0.3/bec_lib/messages.py
--rw-rw-rw-   0 root         (0) root         (0)     5027 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/numpy_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)     5177 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/observer.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/pdf_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     7491 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/queue_items.py
--rw-rw-rw-   0 root         (0) root         (0)    36071 2024-04-11 12:55:21.000000 bec_lib-2.0.3/bec_lib/redis_connector.py
--rw-rw-rw-   0 root         (0) root         (0)     5664 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/request_items.py
--rw-rw-rw-   0 root         (0) root         (0)     6526 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/scan_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10892 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/scan_items.py
--rw-rw-rw-   0 root         (0) root         (0)     8573 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/scan_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     6097 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/scan_report.py
--rw-rw-rw-   0 root         (0) root         (0)    17027 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/scans.py
--rw-rw-rw-   0 root         (0) root         (0)     1147 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/scibec_validator.py
--rw-rw-rw-   0 root         (0) root         (0)    10200 2024-04-11 12:42:13.000000 bec_lib-2.0.3/bec_lib/serialization.py
--rw-rw-rw-   0 root         (0) root         (0)     3126 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/service_config.py
--rw-rw-rw-   0 root         (0) root         (0)     4688 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/signature_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.465441 bec_lib-2.0.3/bec_lib/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:57:24.000000 bec_lib-2.0.3/bec_lib/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8004 2024-04-11 12:42:13.000000 bec_lib-2.0.3/bec_lib/tests/end2end_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)     1594 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/tests/fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)    41009 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/tests/test_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/tests/test_service_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    23107 2024-04-11 12:55:21.000000 bec_lib-2.0.3/bec_lib/tests/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4780 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/user_scripts_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     7636 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.465441 bec_lib-2.0.3/bec_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3013 2024-04-11 12:57:35.000000 bec_lib-2.0.3/bec_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1531 2024-04-11 12:57:35.000000 bec_lib-2.0.3/bec_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 12:57:35.000000 bec_lib-2.0.3/bec_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      183 2024-04-11 12:57:35.000000 bec_lib-2.0.3/bec_lib.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      258 2024-04-11 12:57:35.000000 bec_lib-2.0.3/bec_lib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 12:57:35.000000 bec_lib-2.0.3/bec_lib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-11 12:57:35.466441 bec_lib-2.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1341 2024-04-11 12:57:33.000000 bec_lib-2.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:31:31.368960 bec_lib-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)     3013 2024-04-11 16:31:31.369960 bec_lib-2.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2616 2024-04-11 09:28:21.000000 bec_lib-2.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:31:31.367960 bec_lib-2.1.0/bec_lib/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3901 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/alarm_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/async_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/bec_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    16590 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/bec_plotter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11292 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/bec_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     7247 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/bl_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2426 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/bl_conditions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5952 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/callback_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/channel_monitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     9024 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     9055 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/config_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:31:31.367960 bec_lib-2.1.0/bec_lib/configs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 16:31:20.000000 bec_lib-2.1.0/bec_lib/configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    38908 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/configs/demo_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)   289604 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/configs/openapi_schema.json
+-rw-r--r--   0 root         (0) root         (0)     4747 2024-04-11 16:31:21.000000 bec_lib-2.1.0/bec_lib/connector.py
+-rw-rw-rw-   0 root         (0) root         (0)    12816 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/dap_plugin_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     3935 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/dap_plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)    30828 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/device.py
+-rw-rw-rw-   0 root         (0) root         (0)    23274 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/devicemanager.py
+-rw-rw-rw-   0 root         (0) root         (0)    37595 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/endpoints.py
+-rw-rw-rw-   0 root         (0) root         (0)     9233 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/file_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/lmfit_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2546 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/logbook_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)     6959 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    20005 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     5027 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/numpy_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     5177 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/observer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/pdf_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     7491 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/queue_items.py
+-rw-r--r--   0 root         (0) root         (0)    39020 2024-04-11 16:31:21.000000 bec_lib-2.1.0/bec_lib/redis_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)     5664 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/request_items.py
+-rw-rw-rw-   0 root         (0) root         (0)     6526 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/scan_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10892 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/scan_items.py
+-rw-rw-rw-   0 root         (0) root         (0)     8573 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/scan_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     6097 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/scan_report.py
+-rw-rw-rw-   0 root         (0) root         (0)    17027 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/scans.py
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/scibec_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)    10200 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)     3126 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/service_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     4688 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/signature_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:31:31.368960 bec_lib-2.1.0/bec_lib/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 16:31:20.000000 bec_lib-2.1.0/bec_lib/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8004 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/tests/end2end_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)     1594 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/tests/fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)    41009 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/tests/test_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/tests/test_service_config.yaml
+-rw-r--r--   0 root         (0) root         (0)    23224 2024-04-11 16:31:21.000000 bec_lib-2.1.0/bec_lib/tests/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4780 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/user_scripts_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     7636 2024-04-11 09:28:21.000000 bec_lib-2.1.0/bec_lib/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:31:31.368960 bec_lib-2.1.0/bec_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3013 2024-04-11 16:31:31.000000 bec_lib-2.1.0/bec_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1531 2024-04-11 16:31:31.000000 bec_lib-2.1.0/bec_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 16:31:31.000000 bec_lib-2.1.0/bec_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      183 2024-04-11 16:31:31.000000 bec_lib-2.1.0/bec_lib.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      258 2024-04-11 16:31:31.000000 bec_lib-2.1.0/bec_lib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 16:31:31.000000 bec_lib-2.1.0/bec_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-11 16:31:31.370960 bec_lib-2.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2024-04-11 16:31:29.000000 bec_lib-2.1.0/setup.py
```

### Comparing `bec_lib-2.0.3/PKG-INFO` & `bec_lib-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bec_lib
-Version: 2.0.3
+Version: 2.1.0
 Summary: BEC library
 Home-page: https://gitlab.psi.ch/bec/bec
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
```

### Comparing `bec_lib-2.0.3/README.md` & `bec_lib-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/__init__.py` & `bec_lib-2.1.0/bec_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/alarm_handler.py` & `bec_lib-2.1.0/bec_lib/alarm_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/async_data.py` & `bec_lib-2.1.0/bec_lib/async_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/bec_plotter.py` & `bec_lib-2.1.0/bec_lib/bec_plotter.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/bec_service.py` & `bec_lib-2.1.0/bec_lib/bec_service.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/bl_checks.py` & `bec_lib-2.1.0/bec_lib/bl_checks.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/bl_conditions.py` & `bec_lib-2.1.0/bec_lib/bl_conditions.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/callback_handler.py` & `bec_lib-2.1.0/bec_lib/callback_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/channel_monitor.py` & `bec_lib-2.1.0/bec_lib/channel_monitor.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/client.py` & `bec_lib-2.1.0/bec_lib/client.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/config_helper.py` & `bec_lib-2.1.0/bec_lib/config_helper.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/configs/demo_config.yaml` & `bec_lib-2.1.0/bec_lib/configs/demo_config.yaml`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/configs/openapi_schema.json` & `bec_lib-2.1.0/bec_lib/configs/openapi_schema.json`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/connector.py` & `bec_lib-2.1.0/bec_lib/connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,16 +124,21 @@
     def send(self, topic: str, msg: BECMessage) -> None:
         """Send a message"""
 
     @abc.abstractmethod
     def register(self, topics=None, patterns=None, cb=None, start_thread=True, **kwargs):
         """Register a callback for a topic or pattern"""
 
-    def shutdown(self):
-        """Shutdown the connector"""
+    @abc.abstractmethod
+    def unregister(self, topics=None, pattern=None, cb=None):
+        """Unregister a callback for a topic or pattern"""
+
+    @abc.abstractmethod
+    def poll_messages(self, timeout=None):
+        """Poll for new messages, receive them and execute callbacks"""
 
 
 class ConnectorBase(PubSubInterface, StoreInterface):
     """ConnectorBase defines the interface for a connector"""
 
     def raise_warning(self, msg):
         """Raise a warning"""
@@ -150,7 +155,10 @@
     def log_error(self, msg):
         """send an error as log"""
         self.set_and_publish(MessageEndpoints.log(), LogMessage(log_type="error", log_msg=msg))
 
     def set_and_publish(self, topic: str, msg, pipe=None, expire: int = None) -> None:
         """Set a value and publish it"""
         raise NotImplementedError
+
+    def shutdown(self):
+        """Shutdown the connector"""
```

### Comparing `bec_lib-2.0.3/bec_lib/dap_plugin_objects.py` & `bec_lib-2.1.0/bec_lib/dap_plugin_objects.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/dap_plugins.py` & `bec_lib-2.1.0/bec_lib/dap_plugins.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/device.py` & `bec_lib-2.1.0/bec_lib/device.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/devicemanager.py` & `bec_lib-2.1.0/bec_lib/devicemanager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/endpoints.py` & `bec_lib-2.1.0/bec_lib/endpoints.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/file_utils.py` & `bec_lib-2.1.0/bec_lib/file_utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/lmfit_serializer.py` & `bec_lib-2.1.0/bec_lib/lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/logbook_connector.py` & `bec_lib-2.1.0/bec_lib/logbook_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/logger.py` & `bec_lib-2.1.0/bec_lib/logger.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/messages.py` & `bec_lib-2.1.0/bec_lib/messages.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/numpy_encoder.py` & `bec_lib-2.1.0/bec_lib/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/observer.py` & `bec_lib-2.1.0/bec_lib/observer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/pdf_writer.py` & `bec_lib-2.1.0/bec_lib/pdf_writer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/queue_items.py` & `bec_lib-2.1.0/bec_lib/queue_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/redis_connector.py` & `bec_lib-2.1.0/bec_lib/redis_connector.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 redis server.
 """
 
 from __future__ import annotations
 
 import collections
 import inspect
+import itertools
 import queue
 import sys
 import threading
 import time
 import warnings
+from collections.abc import MutableMapping, Sequence
 from dataclasses import dataclass
 from functools import wraps
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 import louie
 import redis
 import redis.client
 import redis.exceptions
 
 from bec_lib.connector import ConnectorBase, MessageObject
@@ -67,317 +69,41 @@
 
         return wrapper
 
     return decorator
 
 
 @dataclass
-class StreamTopicInfo:
-    topic: str | list[str]
-    stream_id: int
+class StreamSubscriptionInfo:
     id: str
+    topic: str
     newest_only: bool
     from_start: bool
-    cb: callable
+    cb_ref: callable
     kwargs: dict
 
+    def __eq__(self, other):
+        if not isinstance(other, StreamSubscriptionInfo):
+            return False
+        return self.topic == other.topic and self.cb_ref == other.cb_ref
 
-class StreamRegisterMixin:
-    """
-    Mixin to add stream registration capabilities to a connector
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._stream_topics_cb = collections.defaultdict(list)
-        self._stream_events_listener_thread = None
-        self._stream_events_dispatcher_thread = None
-        self._stream_messages_queue = queue.Queue()
-        self._stop_stream_events_listener_thread = threading.Event()
-        self._custom_stream_listeners = {}
-        self.__stream_counter = 0
-
-    def _stream_counter(self):
-        self.__stream_counter += 1
-        return self.__stream_counter
-
-    def register_stream(
-        self,
-        topics: str | list[str] | EndpointInfo | list[EndpointInfo] = None,
-        patterns: str | list[str] | EndpointInfo | list[EndpointInfo] = None,
-        cb: callable = None,
-        from_start: bool = False,
-        newest_only: bool = False,
-        start_thread: bool = True,
-        **kwargs,
-    ) -> int:
-        """
-        Register a callback for a stream topic or pattern
-
-        Args:
-            topic (str, optional): Topic. This should be a valid message endpoint in BEC and can be a string or an EndpointInfo object. Defaults to None. Either topic or pattern should be provided.
-            pattern (str, optional): Pattern of topics. In contrast to topics, patterns may contain "*" wildcards. The evaluated patterns should be a valid message endpoint in BEC and can be a string or an EndpointInfo object. Defaults to None. Either topic or pattern should be provided.
-            cb (callable, optional): callback. Defaults to None.
-            from_start (bool, optional): read from start. Defaults to False.
-            newest_only (bool, optional): read newest only. Defaults to False.
-            start_thread (bool, optional): start the dispatcher thread. Defaults to True.
-            **kwargs: additional keyword arguments to be transmitted to the callback
-
-        Returns:
-            int: stream id
-
-        Examples:
-            >>> def my_callback(msg, **kwargs):
-            ...     print(msg)
-            ...
-            >>> connector.register_stream("test", my_callback)
-            >>> connector.register_stream(topic="test", cb=my_callback)
-            >>> connector.register_stream(pattern="test:*", cb=my_callback)
-            >>> connector.register_stream(pattern="test:*", cb=my_callback, start_thread=False)
-            >>> connector.register_stream(pattern="test:*", cb=my_callback, start_thread=False, my_arg="test")
-        """
-
-        if topics is None and patterns is None:
-            raise ValueError("topics and pattern cannot be both None")
-
-        if newest_only and from_start:
-            raise ValueError("newest_only and from_start cannot be both True")
-
-        if not cb:
-            raise ValueError("Callback cb cannot be None")
-
-        # make a weakref from the callable, using louie;
-        # it can create safe refs for simple functions as well as methods
-        cb_ref = louie.saferef.safe_ref(cb)
-
-        if patterns is not None:
-            stream_topics = self._convert_endpointinfo_to_str(patterns)
-        else:
-            stream_topics = self._convert_endpointinfo_to_str(topics)
-
-        if newest_only:
-            # if newest_only is True, we need to provide a separate callback for each topic,
-            # directly calling the callback. This is because we need to have a backpressure
-            # mechanism in place, and we cannot rely on the dispatcher thread to handle it.
-            if isinstance(stream_topics, list):
-                out = []
-                for topic in stream_topics:
-                    out.append(self._add_direct_stream_listener(topic, cb_ref, **kwargs))
-                return out
-            return self._add_direct_stream_listener(stream_topics, cb_ref, **kwargs)
-
-        if self._stream_events_listener_thread is None:
-            # create the thread that will get all messages for this connector;
-            self._stream_events_listener_thread = threading.Thread(
-                target=self._get_stream_messages_loop, daemon=True
-            )
-            self._stream_events_listener_thread.start()
-        if isinstance(stream_topics, list):
-            stream_id = []
-            for topic in stream_topics:
-                stream_id.append(self._stream_counter())
-                self._stream_topics_cb[topic].append(
-                    StreamTopicInfo(
-                        id="0-0",
-                        topic=topic,
-                        stream_id=stream_id,
-                        newest_only=newest_only,
-                        from_start=from_start,
-                        cb=cb_ref,
-                        kwargs=kwargs,
-                    )
-                )
-        else:
-            stream_id = self._stream_counter()
-            self._stream_topics_cb[stream_topics].append(
-                StreamTopicInfo(
-                    id="0-0",
-                    topic=stream_topics,
-                    stream_id=stream_id,
-                    newest_only=newest_only,
-                    from_start=from_start,
-                    cb=cb_ref,
-                    kwargs=kwargs,
-                )
-            )
-
-        if start_thread and self._stream_events_dispatcher_thread is None:
-            # start dispatcher thread
-            self._stream_events_dispatcher_thread = threading.Thread(
-                target=self._dispatch_stream_events, daemon=True
-            )
-            self._stream_events_dispatcher_thread.start()
-        return stream_id
-
-    def unregister_stream(self, stream_id: int) -> bool:
-        """
-        Unregister a stream listener.
-
-        Args:
-            stream_id (int): stream id
-
-        Returns:
-            bool: True if the stream listener has been removed, False otherwise
-        """
-
-        if stream_id in self._custom_stream_listeners:
-            listener = self._custom_stream_listeners.pop(stream_id)
-            event = listener["stop_event"]
-            thread = listener["thread"]
-            event.set()
-            thread.join()
-            return True
-        if stream_id in self._stream_topics_cb:
-            self._stream_topics_cb.pop(stream_id)
-            return True
-        return False
-
-    def _add_direct_stream_listener(self, topic, cb, **kwargs) -> int:
-        """
-        Add a direct listener for a topic. This is used when newest_only is True.
-
-        Args:
-            topic (str): topic
-            cb (callable): callback
-            kwargs (dict): additional keyword arguments to be transmitted to the callback
-
-        Returns:
-            int: stream id
-        """
-        stream_id = self._stream_counter()
-        info = StreamTopicInfo(
-            id="0-0",
-            topic=topic,
-            stream_id=stream_id,
-            newest_only=True,
-            from_start=False,
-            cb=cb,
-            kwargs=kwargs,
-        )
-        event = threading.Event()
-        thread = threading.Thread(
-            target=self._direct_stream_listener, args=(info, event), daemon=True
-        )
-        self._custom_stream_listeners[stream_id] = {
-            "info": info,
-            "thread": thread,
-            "stop_event": event,
-        }
-        thread.start()
-
-        return stream_id
-
-    def _direct_stream_listener(self, info: StreamTopicInfo, stop_event: threading.Event):
-        while not stop_event.is_set():
-            msg = self.xread(info.topic, count=1, block=1000)
-            if not msg:
-                time.sleep(0.1)
-                continue
-            cb = info.cb()
-            if not cb:
-                return
-            try:
-                cb(msg[0], **info.kwargs)
-            # pylint: disable=broad-except
-            except Exception:
-                sys.excepthook(*sys.exc_info())
-
-    def _dispatch_stream_events(self):
-        while self.poll_stream_messages():
-            ...
-
-    def _get_stream_topics(self) -> dict:
-        stream_topics = {}
-        for topic, subscriber in self._stream_topics_cb.items():
-            for info in subscriber:
-                stream_topics[topic] = info.id
-        return stream_topics
-
-    def _get_stream_messages_loop(self) -> None:
-        """
-        Get stream messages loop. This method is run in a separate thread and listens
-        for messages from the redis server.
-        """
-        error = False
-        while not self._stop_stream_events_listener_thread.is_set():
-            try:
-                stream_topics = self._get_stream_topics()
-                if not stream_topics:
-                    continue
-                msg = self._redis_conn.xread(streams=stream_topics, block=1000)
-                print(stream_topics)
-
-            except redis.exceptions.ConnectionError:
-                if not error:
-                    error = True
-                    bec_logger.logger.error("Failed to connect to redis. Is the server running?")
-                time.sleep(1)
-            # pylint: disable=broad-except
-            except Exception:
-                sys.excepthook(*sys.exc_info())
-            else:
-                error = False
-                if msg is not None:
-                    self._stream_messages_queue.put(msg)
-
-    def poll_stream_messages(self, timeout=None) -> None:
-        """
-        Poll for new messages, receive them and execute callbacks
 
-        Args:
-            timeout ([type], optional): timeout in seconds. Defaults to None.
-        """
-        while True:
-            try:
-                msg = self._stream_messages_queue.get(timeout=timeout)
-            except queue.Empty as exc:
-                raise TimeoutError(
-                    f"{self}: poll_stream_messages: did not receive a message within {timeout} seconds"
-                ) from exc
-            if msg is StopIteration:
-                return False
-            if self._handle_stream_message(msg):
-                return True
+@dataclass
+class DirectReadingStreamSubscriptionInfo(StreamSubscriptionInfo):
+    thread = None
+    stop_event = None
 
-    def _handle_stream_message(self, msg):
-        if not msg:
-            return False
-        for topic, msgs in msg:
-            callbacks = self._stream_topics_cb[topic.decode()]
-            for index, record in msgs:
-                msg_dict = {
-                    k.decode(): MsgpackSerialization.loads(msg) for k, msg in record.items()
-                }
-                for info in callbacks:
-                    info.id = index
-                    cb = info.cb()
-                    if cb:
-                        try:
-                            cb(msg_dict, **info.kwargs)
-                        # pylint: disable=broad-except
-                        except Exception:
-                            sys.excepthook(*sys.exc_info())
-        return True
 
-    def shutdown(self):
-        """
-        Shutdown the connector
-        """
-        super().shutdown()
-        if self._stream_events_listener_thread:
-            self._stop_stream_events_listener_thread.set()
-            self._stream_events_listener_thread.join()
-            self._stream_events_listener_thread = None
-        if self._stream_events_dispatcher_thread:
-            self._stream_messages_queue.put(StopIteration)
-            self._stream_events_dispatcher_thread.join()
-            self._stream_events_dispatcher_thread = None
+@dataclass
+class StreamMessage:
+    msg: dict
+    callbacks: list
 
 
-class RedisConnector(StreamRegisterMixin, ConnectorBase):
+class RedisConnector(ConnectorBase):
     """
     Redis connector class. This class is a wrapper around the redis library providing
     a simple interface to send and receive messages from a redis server.
     """
 
     def __init__(self, bootstrap: list, redis_cls=None):
         """
@@ -398,30 +124,42 @@
             self._redis_conn = redis.Redis(host=self.host, port=self.port)
 
         # main pubsub connection
         self._pubsub_conn = self._redis_conn.pubsub()
         self._pubsub_conn.ignore_subscribe_messages = True
         # keep track of topics and callbacks
         self._topics_cb = collections.defaultdict(list)
+        self._topics_cb_lock = threading.Lock()
+        self._stream_topics_subscription = collections.defaultdict(list)
+        self._stream_topics_subscription_lock = threading.Lock()
 
         self._events_listener_thread = None
+        self._stream_events_listener_thread = None
         self._events_dispatcher_thread = None
         self._messages_queue = queue.Queue()
         self._stop_events_listener_thread = threading.Event()
+        self._stop_stream_events_listener_thread = threading.Event()
         self.stream_keys = {}
 
     def shutdown(self):
         """
         Shutdown the connector
         """
         super().shutdown()
+        # this will take care of shutting down direct listening threads
+        self._unregister_stream(self._stream_topics_subscription)
+
         if self._events_listener_thread:
             self._stop_events_listener_thread.set()
             self._events_listener_thread.join()
             self._events_listener_thread = None
+        if self._stream_events_listener_thread:
+            self._stop_stream_events_listener_thread.set()
+            self._stream_events_listener_thread.join()
+            self._stream_events_listener_thread = None
         if self._events_dispatcher_thread:
             self._messages_queue.put(StopIteration)
             self._events_dispatcher_thread.join()
             self._events_dispatcher_thread = None
 
         # release all connections
         self._pubsub_conn.close()
@@ -519,90 +257,370 @@
             msg (BECMessage): message
             pipe (Pipeline, optional): redis pipe. Defaults to None.
         """
         if not isinstance(msg, BECMessage):
             raise TypeError(f"Message {msg} is not a BECMessage")
         self.raw_send(topic, MsgpackSerialization.dumps(msg), pipe)
 
+    def _start_events_dispatcher_thread(self, start_thread):
+        if start_thread and self._events_dispatcher_thread is None:
+            # start dispatcher thread
+            started_event = threading.Event()
+            self._events_dispatcher_thread = threading.Thread(
+                target=self._dispatch_events, args=(started_event,)
+            )
+            self._events_dispatcher_thread.start()
+            started_event.wait()  # synchronization of thread start
+
+    def _convert_endpointinfo(self, endpoint, check_message_op=True):
+        if isinstance(endpoint, EndpointInfo):
+            return [endpoint.endpoint], endpoint.message_op.name
+        if isinstance(endpoint, str):
+            return [endpoint], ""
+        # Support list of endpoints or dict with endpoints as keys
+        if isinstance(endpoint, (Sequence, MutableMapping)):
+            endpoints_str = []
+            ref_message_op = None
+            for e in endpoint:
+                e_str, message_op = self._convert_endpointinfo(e, check_message_op=check_message_op)
+                if check_message_op:
+                    if ref_message_op is None:
+                        ref_message_op = message_op
+                    else:
+                        if message_op != ref_message_op:
+                            raise ValueError(
+                                f"All endpoints do not have the same type: {ref_message_op}"
+                            )
+                endpoints_str.append(e_str)
+            return list(itertools.chain(*endpoints_str)), ref_message_op or ""
+        raise ValueError(f"Invalid endpoint {endpoint}")
+
+    def _normalize_patterns(self, patterns):
+        patterns, _ = self._convert_endpointinfo(patterns)
+        if isinstance(patterns, str):
+            return [patterns]
+        elif isinstance(patterns, list):
+            if not all(isinstance(p, str) for p in patterns):
+                raise ValueError("register: patterns must be a string or a list of strings")
+        else:
+            raise ValueError("register: patterns must be a string or a list of strings")
+        return patterns
+
     def register(
         self,
         topics: str | list[str] | EndpointInfo | list[EndpointInfo] = None,
-        patterns: str | list[str] | EndpointInfo | list[EndpointInfo] = None,
+        patterns: str | list[str] = None,
         cb: callable = None,
         start_thread: bool = True,
+        from_start: bool = False,
+        newest_only: bool = False,
         **kwargs,
     ):
         """
         Register a callback for a topic or a pattern
 
         Args:
             topics (str, list, EndpointInfo, list[EndpointInfo], optional): topic or list of topics. Defaults to None. The topic should be a valid message endpoint in BEC and can be a string or an EndpointInfo object.
-            patterns (str, list, optional): pattern or list of patterns. Defaults to None. In contrast to topics, patterns may contain "*" wildcards. The evaluated patterns should be a valid message endpoint in BEC and can be a string or an EndpointInfo object.
+            patterns (str, list, optional): pattern or list of patterns. Defaults to None. In contrast to topics, patterns may contain "*" wildcards. The evaluated patterns should be a valid pub/sub message endpoint in BEC
             cb (callable, optional): callback. Defaults to None.
             start_thread (bool, optional): start the dispatcher thread. Defaults to True.
+            from_start (bool, optional): for streams only: return data from start on first reading. Defaults to False.
+            newest_only (bool, optional): for streams only: return newest data only. Defaults to False.
             **kwargs: additional keyword arguments to be transmitted to the callback
 
         Examples:
             >>> def my_callback(msg, **kwargs):
             ...     print(msg)
             ...
             >>> connector.register("test", my_callback)
             >>> connector.register(topics="test", cb=my_callback)
             >>> connector.register(patterns="test:*", cb=my_callback)
             >>> connector.register(patterns="test:*", cb=my_callback, start_thread=False)
             >>> connector.register(patterns="test:*", cb=my_callback, start_thread=False, my_arg="test")
         """
+        if cb is None:
+            raise ValueError("Callback cb cannot be None")
+
+        if topics is None and patterns is None:
+            raise ValueError("topics and patterns cannot be both None")
+
+        # make a weakref from the callable, using louie;
+        # it can create safe refs for simple functions as well as methods
+        cb_ref = louie.saferef.safe_ref(cb)
+        item = (cb_ref, kwargs)
+
         if self._events_listener_thread is None:
             # create the thread that will get all messages for this connector;
             self._events_listener_thread = threading.Thread(
-                target=self._get_messages_loop, args=(self._pubsub_conn,), daemon=True
+                target=self._get_messages_loop, args=(self._pubsub_conn,)
             )
             self._events_listener_thread.start()
 
-        if cb is None:
-            raise ValueError("Callback cb cannot be None")
+        if patterns is not None:
+            patterns = self._normalize_patterns(patterns)
+
+            self._pubsub_conn.psubscribe(patterns)
+            with self._topics_cb_lock:
+                for pattern in patterns:
+                    if item not in self._topics_cb[pattern]:
+                        self._topics_cb[pattern].append(item)
+        else:
+            topics, message_op = self._convert_endpointinfo(topics)
+            if message_op == "STREAM":
+                return self._register_stream(
+                    topics=topics,
+                    cb=cb,
+                    from_start=from_start,
+                    newest_only=newest_only,
+                    start_thread=start_thread,
+                    **kwargs,
+                )
+
+            self._pubsub_conn.subscribe(topics)
+            with self._topics_cb_lock:
+                for topic in topics:
+                    if item not in self._topics_cb[topic]:
+                        self._topics_cb[topic].append(item)
+        self._start_events_dispatcher_thread(start_thread)
+
+    def _add_direct_stream_listener(self, topic, cb_ref, **kwargs) -> int:
+        """
+        Add a direct listener for a topic. This is used when newest_only is True.
+
+        Args:
+            topic (str): topic
+            cb (callable): weakref to callback
+            kwargs (dict): additional keyword arguments to be transmitted to the callback
+
+        Returns:
+            int: stream id
+        """
+        info = DirectReadingStreamSubscriptionInfo(
+            id="-",
+            topic=topic,
+            newest_only=True,
+            from_start=False,
+            cb_ref=cb_ref,
+            kwargs=kwargs,
+        )
+        if info in self._stream_topics_subscription[topic]:
+            raise RuntimeError("Already registered stream topic with the same callback")
+
+        info.stop_event = threading.Event()
+        info.thread = threading.Thread(target=self._direct_stream_listener, args=(info,))
+        with self._stream_topics_subscription_lock:
+            self._stream_topics_subscription[topic].append(info)
+        info.thread.start()
+
+    def _direct_stream_listener(self, info: DirectReadingStreamSubscriptionInfo):
+        stop_event = info.stop_event
+        cb_ref = info.cb_ref
+        kwargs = info.kwargs
+        topic = info.topic
+        while not stop_event.is_set():
+            ret = self._redis_conn.xrevrange(topic, "+", info.id, count=1)
+            if not ret:
+                time.sleep(0.1)
+                continue
+            redis_id, msg_dict = ret[0]
+            timestamp, _, ind = redis_id.partition(b"-")
+            info.id = f"{timestamp.decode()}-{int(ind.decode())+1}"
+            stream_msg = StreamMessage(
+                {key.decode(): MsgpackSerialization.loads(val) for key, val in msg_dict.items()},
+                ((cb_ref, kwargs),),
+            )
+            self._messages_queue.put(stream_msg)
+
+    def _get_stream_topics_id(self) -> dict:
+        stream_topics_id = {}
+        for topic, subscriber_info_list in self._stream_topics_subscription.items():
+            for info in subscriber_info_list:
+                if isinstance(info, DirectReadingStreamSubscriptionInfo):
+                    continue
+                stream_topics_id[topic] = info.id
+        return stream_topics_id
+
+    def _get_stream_messages_loop(self) -> None:
+        """
+        Get stream messages loop. This method is run in a separate thread and listens
+        for messages from the redis server.
+        """
+        error = False
+
+        while not self._stop_stream_events_listener_thread.is_set():
+            try:
+                stream_topics_id = self._get_stream_topics_id()
+                if not stream_topics_id:
+                    time.sleep(0.1)
+                    continue
+                msg_list = self._redis_conn.xread(streams=stream_topics_id, block=1000)
+            except redis.exceptions.ConnectionError:
+                if not error:
+                    error = True
+                    bec_logger.logger.error("Failed to connect to redis. Is the server running?")
+                time.sleep(1)
+            # pylint: disable=broad-except
+            except Exception:
+                sys.excepthook(*sys.exc_info())
+            else:
+                error = False
+                if msg_list is not None:
+                    for topic, msgs in msg_list:
+                        subscription_infos = self._stream_topics_subscription[topic.decode()]
+                        for index, record in msgs:
+                            msg_dict = {
+                                k.decode(): MsgpackSerialization.loads(msg)
+                                for k, msg in record.items()
+                            }
+                            callbacks = []
+                            for info in subscription_infos:
+                                info.id = index
+                                callbacks.append((info.cb_ref, info.kwargs))
+                            msg = StreamMessage(msg_dict, callbacks)
+                            self._messages_queue.put(msg)
+        return True
+
+    def _register_stream(
+        self,
+        topics: list[str] = None,
+        cb: callable = None,
+        from_start: bool = False,
+        newest_only: bool = False,
+        start_thread: bool = True,
+        **kwargs,
+    ) -> None:
+        """
+        Register a callback for a stream topic or pattern
+
+        Args:
+            topic (str, optional): Topic. This should be a valid message endpoint string.
+            cb (callable, optional): callback. Defaults to None.
+            from_start (bool, optional): read from start. Defaults to False.
+            newest_only (bool, optional): read newest only. Defaults to False.
+            start_thread (bool, optional): start the dispatcher thread. Defaults to True.
+            **kwargs: additional keyword arguments to be transmitted to the callback
+
+        """
+        if newest_only and from_start:
+            raise ValueError("newest_only and from_start cannot be both True")
+
         # make a weakref from the callable, using louie;
         # it can create safe refs for simple functions as well as methods
         cb_ref = louie.saferef.safe_ref(cb)
 
-        if topics is None and patterns is None:
-            raise ValueError("topics and patterns cannot be both None")
+        self._start_events_dispatcher_thread(start_thread)
 
-        if patterns is not None:
-            patterns = self._convert_endpointinfo_to_str(patterns)
-            if not isinstance(patterns, list):
-                patterns = [patterns]
+        if newest_only:
+            # if newest_only is True, we need to provide a separate callback for each topic,
+            # directly calling the callback. This is because we need to have a backpressure
+            # mechanism in place, and we cannot rely on the dispatcher thread to handle it.
+            for topic in topics:
+                self._add_direct_stream_listener(topic, cb_ref, **kwargs)
+        else:
+            with self._stream_topics_subscription_lock:
+                for topic in topics:
+                    new_subscription = StreamSubscriptionInfo(
+                        id="0-0",
+                        topic=topic,
+                        newest_only=newest_only,
+                        from_start=from_start,
+                        cb_ref=cb_ref,
+                        kwargs=kwargs,
+                    )
+                    subscriptions = self._stream_topics_subscription[topic]
+                    if new_subscription in subscriptions:
+                        # raise an error if attempted to register a stream with the same callback,
+                        # whereas it has already been registered as a 'direct reading' stream with
+                        # newest_only=True ; it is clearly an error case that would produce weird results
+                        index = subscriptions.index(new_subscription)
+                        if isinstance(subscriptions[index], DirectReadingStreamSubscriptionInfo):
+                            raise RuntimeError(
+                                "Already registered stream topic with the same callback with 'newest_only=True'"
+                            )
+                    else:
+                        subscriptions.append(new_subscription)
+
+            if self._stream_events_listener_thread is None:
+                # create the thread that will get all messages for this connector
+                self._stream_events_listener_thread = threading.Thread(
+                    target=self._get_stream_messages_loop
+                )
+                self._stream_events_listener_thread.start()
 
-            self._pubsub_conn.psubscribe(patterns)
+    def _filter_topics_cb(self, topics: list, cb: Union[callable, None]):
+        unsubscribe_list = []
+        with self._topics_cb_lock:
+            for topic in topics:
+                topics_cb = self._topics_cb[topic]
+                # remove callback from list
+                self._topics_cb[topic] = list(
+                    filter(lambda item: cb and item[0]() is not cb, topics_cb)
+                )
+                if not self._topics_cb[topic]:
+                    # no callbacks left, unsubscribe
+                    unsubscribe_list.append(topic)
+            # clean the topics that have been unsubscribed
+            for topic in unsubscribe_list:
+                del self._topics_cb[topic]
+        return unsubscribe_list
+
+    def unregister(self, topics=None, patterns=None, cb=None):
+        if self._events_listener_thread is None:
+            return
+
+        if patterns is not None:
+            patterns = self._normalize_patterns(patterns)
+            # see if registered streams can be unregistered
             for pattern in patterns:
-                self._topics_cb[pattern].append((cb_ref, kwargs))
+                self._unregister_stream(
+                    fnmatch.filter(self._stream_topics_subscription, pattern), cb
+                )
+            pubsub_unsubscribe_list = self._filter_topics_cb(patterns, cb)
+            self._pubsub_conn.punsubscribe(pubsub_unsubscribe_list)
         else:
-            topics = self._convert_endpointinfo_to_str(topics)
-            if not isinstance(topics, list):
-                topics = [topics]
+            topics, _ = self._convert_endpointinfo(topics, check_message_op=False)
+            if not self._unregister_stream(topics, cb):
+                unsubscribe_list = self._filter_topics_cb(topics, cb)
+                self._pubsub_conn.unsubscribe(unsubscribe_list)
 
-            self._pubsub_conn.subscribe(topics)
-            for topic in topics:
-                self._topics_cb[topic].append((cb_ref, kwargs))
+    def _unregister_stream(self, topics: list[str], cb: callable = None) -> bool:
+        """
+        Unregister a stream listener.
 
-        if start_thread and self._events_dispatcher_thread is None:
-            # start dispatcher thread
-            self._events_dispatcher_thread = threading.Thread(
-                target=self._dispatch_events, daemon=True
-            )
-            self._events_dispatcher_thread.start()
+        Args:
+            topics (list[str]): list of stream topics
 
-    def _convert_endpointinfo_to_str(self, endpoint):
-        if isinstance(endpoint, EndpointInfo):
-            return endpoint.endpoint
-        if isinstance(endpoint, str):
-            return endpoint
-        if isinstance(endpoint, list):
-            return [self._convert_endpointinfo_to_str(e) for e in endpoint]
-        raise ValueError(f"Invalid endpoint {endpoint}")
+        Returns:
+            bool: True if the stream listener has been removed, False otherwise
+        """
+        unsubscribe_list = []
+        with self._stream_topics_subscription_lock:
+            for topic in topics:
+                subscription_infos = self._stream_topics_subscription[topic]
+                # remove from list if callback corresponds
+                self._stream_topics_subscription[topic] = list(
+                    filter(lambda sub_info: cb and sub_info.cb_ref() is not cb, subscription_infos)
+                )
+                if not self._stream_topics_subscription[topic]:
+                    # no callbacks left, unsubscribe
+                    unsubscribe_list += subscription_infos
+            # clean the topics that have been unsubscribed
+            for subscription_info in unsubscribe_list:
+                if isinstance(subscription_info, DirectReadingStreamSubscriptionInfo):
+                    subscription_info.stop_event.set()
+                    subscription_info.thread.join()
+                # it is possible to register the same stream multiple times with different
+                # callbacks, in this case when unregistering with cb=None (unregister all)
+                # the topic can be deleted multiple times, hence try...except in code below
+                try:
+                    del self._stream_topics_subscription[subscription_info.topic]
+                except KeyError:
+                    pass
+
+        return len(unsubscribe_list) > 0
 
     def _get_messages_loop(self, pubsub: redis.client.PubSub) -> None:
         """
         Get messages loop. This method is run in a separate thread and listens
         for messages from the redis server.
 
         Args:
@@ -621,32 +639,42 @@
             except Exception:
                 sys.excepthook(*sys.exc_info())
             else:
                 error = False
                 if msg is not None:
                     self._messages_queue.put(msg)
 
+    def _execute_callback(self, cb, msg, kwargs):
+        try:
+            cb(msg, **kwargs)
+        # pylint: disable=broad-except
+        except Exception:
+            sys.excepthook(*sys.exc_info())
+
+    def _handle_stream_message(self, stream_msg):
+        for cb_ref, kwargs in stream_msg.callbacks:
+            cb = cb_ref()
+            if cb:
+                self._execute_callback(cb, stream_msg.msg, kwargs)
+        return True
+
     def _handle_message(self, msg):
-        if msg["type"].endswith("subscribe"):
-            # ignore subscribe messages
-            return False
+        if isinstance(msg, StreamMessage):
+            return self._handle_stream_message(msg)
         channel = msg["channel"].decode()
-        if msg["pattern"] is not None:
-            callbacks = self._topics_cb[msg["pattern"].decode()]
-        else:
-            callbacks = self._topics_cb[channel]
+        with self._topics_cb_lock:
+            if msg["pattern"] is not None:
+                callbacks = self._topics_cb[msg["pattern"].decode()]
+            else:
+                callbacks = self._topics_cb[channel]
         msg = MessageObject(topic=channel, value=MsgpackSerialization.loads(msg["data"]))
         for cb_ref, kwargs in callbacks:
             cb = cb_ref()
             if cb:
-                try:
-                    cb(msg, **kwargs)
-                # pylint: disable=broad-except
-                except Exception:
-                    sys.excepthook(*sys.exc_info())
+                self._execute_callback(cb, msg, kwargs)
         return True
 
     def poll_messages(self, timeout=None) -> None:
         while True:
             try:
                 msg = self._messages_queue.get(timeout=timeout)
             except queue.Empty as exc:
@@ -654,15 +682,16 @@
                     f"{self}: poll_messages: did not receive a message within {timeout} seconds"
                 ) from exc
             if msg is StopIteration:
                 return False
             if self._handle_message(msg):
                 return True
 
-    def _dispatch_events(self):
+    def _dispatch_events(self, started_event):
+        started_event.set()
         while self.poll_messages():
             ...
 
     @validate_endpoint("topic")
     def lpush(
         self, topic: EndpointInfo, msg: str, pipe=None, max_size: int = None, expire: int = None
     ) -> None:
```

### Comparing `bec_lib-2.0.3/bec_lib/request_items.py` & `bec_lib-2.1.0/bec_lib/request_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/scan_data.py` & `bec_lib-2.1.0/bec_lib/scan_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/scan_items.py` & `bec_lib-2.1.0/bec_lib/scan_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/scan_manager.py` & `bec_lib-2.1.0/bec_lib/scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/scan_report.py` & `bec_lib-2.1.0/bec_lib/scan_report.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/scans.py` & `bec_lib-2.1.0/bec_lib/scans.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/scibec_validator.py` & `bec_lib-2.1.0/bec_lib/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/serialization.py` & `bec_lib-2.1.0/bec_lib/serialization.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/service_config.py` & `bec_lib-2.1.0/bec_lib/service_config.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/signature_serializer.py` & `bec_lib-2.1.0/bec_lib/signature_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/tests/end2end_fixtures.py` & `bec_lib-2.1.0/bec_lib/tests/end2end_fixtures.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/tests/fixtures.py` & `bec_lib-2.1.0/bec_lib/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/tests/test_config.yaml` & `bec_lib-2.1.0/bec_lib/tests/test_config.yaml`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/tests/utils.py` & `bec_lib-2.1.0/bec_lib/tests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -498,14 +498,20 @@
 
     def shutdown(self):
         pass
 
     def register(self, *args, **kwargs):
         pass
 
+    def unregister(self, *args, **kwargs):
+        pass
+
+    def poll_messages(self, *args, **kwargs):
+        pass
+
     def keys(self, *args, **kwargs):
         return []
 
     def set(self, topic, msg, pipe=None, expire: int = None):
         if pipe:
             pipe._pipe_buffer.append(("set", (topic.endpoint, msg), {"expire": expire}))
             return
```

### Comparing `bec_lib-2.0.3/bec_lib/user_scripts_mixin.py` & `bec_lib-2.1.0/bec_lib/user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib/utils.py` & `bec_lib-2.1.0/bec_lib/utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/bec_lib.egg-info/PKG-INFO` & `bec_lib-2.1.0/bec_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bec-lib
-Version: 2.0.3
+Version: 2.1.0
 Summary: BEC library
 Home-page: https://gitlab.psi.ch/bec/bec
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
```

### Comparing `bec_lib-2.0.3/bec_lib.egg-info/SOURCES.txt` & `bec_lib-2.1.0/bec_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.3/setup.py` & `bec_lib-2.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = "2.0.3"
+__version__ = "2.1.0"
 
 if __name__ == "__main__":
     setup(
         install_requires=[
             "hiredis",
             "louie",
             "numpy",
```

