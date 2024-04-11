# Comparing `tmp/bec_lib-2.0.2.tar.gz` & `tmp/bec_lib-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_lib-2.0.2.tar", last modified: Thu Apr 11 08:36:44 2024, max compression
+gzip compressed data, was "bec_lib-2.0.3.tar", last modified: Thu Apr 11 12:57:35 2024, max compression
```

## Comparing `bec_lib-2.0.2.tar` & `bec_lib-2.0.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.524506 bec_lib-2.0.2/
--rw-r--r--   0 root         (0) root         (0)     3013 2024-04-11 08:36:44.524506 bec_lib-2.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2616 2024-04-11 01:29:15.000000 bec_lib-2.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.523506 bec_lib-2.0.2/bec_lib/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3901 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/alarm_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     3663 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/async_data.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/bec_errors.py
--rw-rw-rw-   0 root         (0) root         (0)    16590 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/bec_plotter.py
--rw-rw-rw-   0 root         (0) root         (0)    11292 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/bec_service.py
--rw-rw-rw-   0 root         (0) root         (0)     7247 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/bl_checks.py
--rw-rw-rw-   0 root         (0) root         (0)     2426 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/bl_conditions.py
--rw-rw-rw-   0 root         (0) root         (0)     5952 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/callback_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/channel_monitor.py
--rw-rw-rw-   0 root         (0) root         (0)     9024 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/client.py
--rw-r--r--   0 root         (0) root         (0)     9055 2024-04-11 08:36:34.000000 bec_lib-2.0.2/bec_lib/config_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.523506 bec_lib-2.0.2/bec_lib/configs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 08:36:34.000000 bec_lib-2.0.2/bec_lib/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    38908 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/configs/demo_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)   289604 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/configs/openapi_schema.json
--rw-rw-rw-   0 root         (0) root         (0)     4461 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/connector.py
--rw-rw-rw-   0 root         (0) root         (0)    12816 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/dap_plugin_objects.py
--rw-rw-rw-   0 root         (0) root         (0)     3935 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/dap_plugins.py
--rw-rw-rw-   0 root         (0) root         (0)    30828 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/device.py
--rw-rw-rw-   0 root         (0) root         (0)    23274 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/devicemanager.py
--rw-rw-rw-   0 root         (0) root         (0)    37595 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/endpoints.py
--rw-rw-rw-   0 root         (0) root         (0)     9233 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/file_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/lmfit_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2546 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/logbook_connector.py
--rw-r--r--   0 root         (0) root         (0)     6959 2024-04-11 08:36:34.000000 bec_lib-2.0.2/bec_lib/logger.py
--rw-rw-rw-   0 root         (0) root         (0)    20005 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/messages.py
--rw-rw-rw-   0 root         (0) root         (0)     5027 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/numpy_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)     5177 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/observer.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/pdf_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     7491 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/queue_items.py
--rw-rw-rw-   0 root         (0) root         (0)    36071 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/redis_connector.py
--rw-rw-rw-   0 root         (0) root         (0)     5664 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/request_items.py
--rw-rw-rw-   0 root         (0) root         (0)     6526 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/scan_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10892 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/scan_items.py
--rw-rw-rw-   0 root         (0) root         (0)     8573 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/scan_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     6097 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/scan_report.py
--rw-rw-rw-   0 root         (0) root         (0)    17027 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/scans.py
--rw-rw-rw-   0 root         (0) root         (0)     1147 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/scibec_validator.py
--rw-rw-rw-   0 root         (0) root         (0)    10200 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/serialization.py
--rw-rw-rw-   0 root         (0) root         (0)     3126 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/service_config.py
--rw-rw-rw-   0 root         (0) root         (0)     4688 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/signature_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.524506 bec_lib-2.0.2/bec_lib/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 08:36:34.000000 bec_lib-2.0.2/bec_lib/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8004 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/tests/end2end_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)     1594 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/tests/fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)    41009 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/tests/test_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/tests/test_service_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    23107 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/tests/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4780 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/user_scripts_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     7636 2024-04-11 01:29:15.000000 bec_lib-2.0.2/bec_lib/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.524506 bec_lib-2.0.2/bec_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3013 2024-04-11 08:36:44.000000 bec_lib-2.0.2/bec_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1531 2024-04-11 08:36:44.000000 bec_lib-2.0.2/bec_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 08:36:44.000000 bec_lib-2.0.2/bec_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      183 2024-04-11 08:36:44.000000 bec_lib-2.0.2/bec_lib.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      258 2024-04-11 08:36:44.000000 bec_lib-2.0.2/bec_lib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 08:36:44.000000 bec_lib-2.0.2/bec_lib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-11 08:36:44.525506 bec_lib-2.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1341 2024-04-11 08:36:42.000000 bec_lib-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.465441 bec_lib-2.0.3/
+-rw-r--r--   0 root         (0) root         (0)     3013 2024-04-11 12:57:35.466441 bec_lib-2.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2616 2024-04-11 12:02:54.000000 bec_lib-2.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.464441 bec_lib-2.0.3/bec_lib/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3901 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/alarm_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/async_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/bec_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    16590 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/bec_plotter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11292 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/bec_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     7247 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/bl_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2426 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/bl_conditions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5952 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/callback_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/channel_monitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     9024 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     9055 2024-04-11 12:42:13.000000 bec_lib-2.0.3/bec_lib/config_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.464441 bec_lib-2.0.3/bec_lib/configs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:57:24.000000 bec_lib-2.0.3/bec_lib/configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    38908 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/configs/demo_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)   289604 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/configs/openapi_schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     4461 2024-04-11 12:55:21.000000 bec_lib-2.0.3/bec_lib/connector.py
+-rw-rw-rw-   0 root         (0) root         (0)    12816 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/dap_plugin_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     3935 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/dap_plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)    30828 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/device.py
+-rw-rw-rw-   0 root         (0) root         (0)    23274 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/devicemanager.py
+-rw-rw-rw-   0 root         (0) root         (0)    37595 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/endpoints.py
+-rw-rw-rw-   0 root         (0) root         (0)     9233 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/file_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/lmfit_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2546 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/logbook_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)     6959 2024-04-11 12:42:13.000000 bec_lib-2.0.3/bec_lib/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    20005 2024-04-11 12:42:13.000000 bec_lib-2.0.3/bec_lib/messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     5027 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/numpy_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     5177 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/observer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/pdf_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     7491 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/queue_items.py
+-rw-rw-rw-   0 root         (0) root         (0)    36071 2024-04-11 12:55:21.000000 bec_lib-2.0.3/bec_lib/redis_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)     5664 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/request_items.py
+-rw-rw-rw-   0 root         (0) root         (0)     6526 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/scan_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10892 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/scan_items.py
+-rw-rw-rw-   0 root         (0) root         (0)     8573 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/scan_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     6097 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/scan_report.py
+-rw-rw-rw-   0 root         (0) root         (0)    17027 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/scans.py
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/scibec_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)    10200 2024-04-11 12:42:13.000000 bec_lib-2.0.3/bec_lib/serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)     3126 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/service_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     4688 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/signature_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.465441 bec_lib-2.0.3/bec_lib/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:57:24.000000 bec_lib-2.0.3/bec_lib/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8004 2024-04-11 12:42:13.000000 bec_lib-2.0.3/bec_lib/tests/end2end_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)     1594 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/tests/fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)    41009 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/tests/test_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/tests/test_service_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    23107 2024-04-11 12:55:21.000000 bec_lib-2.0.3/bec_lib/tests/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4780 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/user_scripts_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     7636 2024-04-11 12:02:54.000000 bec_lib-2.0.3/bec_lib/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.465441 bec_lib-2.0.3/bec_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3013 2024-04-11 12:57:35.000000 bec_lib-2.0.3/bec_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1531 2024-04-11 12:57:35.000000 bec_lib-2.0.3/bec_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 12:57:35.000000 bec_lib-2.0.3/bec_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      183 2024-04-11 12:57:35.000000 bec_lib-2.0.3/bec_lib.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      258 2024-04-11 12:57:35.000000 bec_lib-2.0.3/bec_lib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 12:57:35.000000 bec_lib-2.0.3/bec_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-11 12:57:35.466441 bec_lib-2.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2024-04-11 12:57:33.000000 bec_lib-2.0.3/setup.py
```

### Comparing `bec_lib-2.0.2/PKG-INFO` & `bec_lib-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bec_lib
-Version: 2.0.2
+Version: 2.0.3
 Summary: BEC library
 Home-page: https://gitlab.psi.ch/bec/bec
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
```

### Comparing `bec_lib-2.0.2/README.md` & `bec_lib-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/__init__.py` & `bec_lib-2.0.3/bec_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/alarm_handler.py` & `bec_lib-2.0.3/bec_lib/alarm_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/async_data.py` & `bec_lib-2.0.3/bec_lib/async_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/bec_plotter.py` & `bec_lib-2.0.3/bec_lib/bec_plotter.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/bec_service.py` & `bec_lib-2.0.3/bec_lib/bec_service.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/bl_checks.py` & `bec_lib-2.0.3/bec_lib/bl_checks.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/bl_conditions.py` & `bec_lib-2.0.3/bec_lib/bl_conditions.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/callback_handler.py` & `bec_lib-2.0.3/bec_lib/callback_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/channel_monitor.py` & `bec_lib-2.0.3/bec_lib/channel_monitor.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/client.py` & `bec_lib-2.0.3/bec_lib/client.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/config_helper.py` & `bec_lib-2.0.3/bec_lib/config_helper.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/configs/demo_config.yaml` & `bec_lib-2.0.3/bec_lib/configs/demo_config.yaml`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/configs/openapi_schema.json` & `bec_lib-2.0.3/bec_lib/configs/openapi_schema.json`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/connector.py` & `bec_lib-2.0.3/bec_lib/connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/dap_plugin_objects.py` & `bec_lib-2.0.3/bec_lib/dap_plugin_objects.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/dap_plugins.py` & `bec_lib-2.0.3/bec_lib/dap_plugins.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/device.py` & `bec_lib-2.0.3/bec_lib/device.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/devicemanager.py` & `bec_lib-2.0.3/bec_lib/devicemanager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/endpoints.py` & `bec_lib-2.0.3/bec_lib/endpoints.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/file_utils.py` & `bec_lib-2.0.3/bec_lib/file_utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/lmfit_serializer.py` & `bec_lib-2.0.3/bec_lib/lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/logbook_connector.py` & `bec_lib-2.0.3/bec_lib/logbook_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/logger.py` & `bec_lib-2.0.3/bec_lib/logger.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/messages.py` & `bec_lib-2.0.3/bec_lib/messages.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/numpy_encoder.py` & `bec_lib-2.0.3/bec_lib/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/observer.py` & `bec_lib-2.0.3/bec_lib/observer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/pdf_writer.py` & `bec_lib-2.0.3/bec_lib/pdf_writer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/queue_items.py` & `bec_lib-2.0.3/bec_lib/queue_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/redis_connector.py` & `bec_lib-2.0.3/bec_lib/redis_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/request_items.py` & `bec_lib-2.0.3/bec_lib/request_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/scan_data.py` & `bec_lib-2.0.3/bec_lib/scan_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/scan_items.py` & `bec_lib-2.0.3/bec_lib/scan_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/scan_manager.py` & `bec_lib-2.0.3/bec_lib/scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/scan_report.py` & `bec_lib-2.0.3/bec_lib/scan_report.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/scans.py` & `bec_lib-2.0.3/bec_lib/scans.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/scibec_validator.py` & `bec_lib-2.0.3/bec_lib/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/serialization.py` & `bec_lib-2.0.3/bec_lib/serialization.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/service_config.py` & `bec_lib-2.0.3/bec_lib/service_config.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/signature_serializer.py` & `bec_lib-2.0.3/bec_lib/signature_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/tests/end2end_fixtures.py` & `bec_lib-2.0.3/bec_lib/tests/end2end_fixtures.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/tests/fixtures.py` & `bec_lib-2.0.3/bec_lib/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/tests/test_config.yaml` & `bec_lib-2.0.3/bec_lib/tests/test_config.yaml`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/tests/utils.py` & `bec_lib-2.0.3/bec_lib/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/user_scripts_mixin.py` & `bec_lib-2.0.3/bec_lib/user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib/utils.py` & `bec_lib-2.0.3/bec_lib/utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/bec_lib.egg-info/PKG-INFO` & `bec_lib-2.0.3/bec_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bec-lib
-Version: 2.0.2
+Version: 2.0.3
 Summary: BEC library
 Home-page: https://gitlab.psi.ch/bec/bec
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
```

### Comparing `bec_lib-2.0.2/bec_lib.egg-info/SOURCES.txt` & `bec_lib-2.0.3/bec_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_lib-2.0.2/setup.py` & `bec_lib-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = "2.0.2"
+__version__ = "2.0.3"
 
 if __name__ == "__main__":
     setup(
         install_requires=[
             "hiredis",
             "louie",
             "numpy",
```

