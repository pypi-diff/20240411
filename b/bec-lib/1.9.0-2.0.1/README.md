# Comparing `tmp/bec_lib-1.9.0.tar.gz` & `tmp/bec_lib-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_lib-1.9.0.tar", last modified: Thu Feb 22 19:50:20 2024, max compression
+gzip compressed data, was "bec_lib-2.0.1.tar", last modified: Thu Apr 11 06:21:55 2024, max compression
```

## Comparing `bec_lib-1.9.0.tar` & `bec_lib-2.0.1.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.723886 bec_lib-1.9.0/
--rw-r--r--   0 root         (0) root         (0)     3049 2024-02-22 19:50:20.723886 bec_lib-1.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2616 2024-02-22 18:57:01.000000 bec_lib-1.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.721886 bec_lib-1.9.0/bec_lib/
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3958 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/alarm_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     3509 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/async_data.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/bec_errors.py
--rw-rw-rw-   0 root         (0) root         (0)    16512 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/bec_plotter.py
--rw-rw-rw-   0 root         (0) root         (0)    10495 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/bec_service.py
--rw-rw-rw-   0 root         (0) root         (0)     7079 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/bl_checks.py
--rw-rw-rw-   0 root         (0) root         (0)     2332 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/bl_conditions.py
--rw-rw-rw-   0 root         (0) root         (0)     5703 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/callback_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/channel_monitor.py
--rw-rw-rw-   0 root         (0) root         (0)     8133 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/client.py
--rw-rw-rw-   0 root         (0) root         (0)     5809 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/config_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.721886 bec_lib-1.9.0/bec_lib/configs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 19:50:05.000000 bec_lib-1.9.0/bec_lib/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    41026 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/configs/demo_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)   289604 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/configs/openapi_schema.json
--rw-rw-rw-   0 root         (0) root         (0)     5686 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/connector.py
--rw-rw-rw-   0 root         (0) root         (0)    12425 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/dap_plugin_objects.py
--rw-rw-rw-   0 root         (0) root         (0)     3831 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/dap_plugins.py
--rw-rw-rw-   0 root         (0) root         (0)    27973 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/device.py
--rw-rw-rw-   0 root         (0) root         (0)    24298 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/devicemanager.py
--rw-rw-rw-   0 root         (0) root         (0)    28839 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/endpoints.py
--rw-rw-rw-   0 root         (0) root         (0)     2723 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/file_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1491 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/lmfit_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2472 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/logbook_connector.py
--rw-rw-rw-   0 root         (0) root         (0)     4888 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/logger.py
--rw-rw-rw-   0 root         (0) root         (0)    21506 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/messages.py
--rw-rw-rw-   0 root         (0) root         (0)     4917 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/numpy_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)     4942 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/observer.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/pdf_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     7448 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/queue_items.py
--rw-rw-rw-   0 root         (0) root         (0)    23835 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/redis_connector.py
--rw-rw-rw-   0 root         (0) root         (0)     5453 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/request_items.py
--rw-rw-rw-   0 root         (0) root         (0)     6441 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/scan_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10615 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/scan_items.py
--rw-rw-rw-   0 root         (0) root         (0)     8772 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/scan_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     5935 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/scan_report.py
--rw-rw-rw-   0 root         (0) root         (0)    14757 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/scans.py
--rw-rw-rw-   0 root         (0) root         (0)     1034 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/scibec_validator.py
--rw-rw-rw-   0 root         (0) root         (0)    10181 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/serialization.py
--rw-rw-rw-   0 root         (0) root         (0)     2778 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/service_config.py
--rw-rw-rw-   0 root         (0) root         (0)     4598 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/signature_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.722886 bec_lib-1.9.0/bec_lib/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 19:50:05.000000 bec_lib-1.9.0/bec_lib/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42385 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/tests/test_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      291 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/tests/test_service_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    23885 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/tests/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4640 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/user_scripts_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     7081 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.722886 bec_lib-1.9.0/bec_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3049 2024-02-22 19:50:20.000000 bec_lib-1.9.0/bec_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1467 2024-02-22 19:50:20.000000 bec_lib-1.9.0/bec_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 19:50:20.000000 bec_lib-1.9.0/bec_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2024-02-22 19:50:20.000000 bec_lib-1.9.0/bec_lib.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      174 2024-02-22 19:50:20.000000 bec_lib-1.9.0/bec_lib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-02-22 19:50:20.000000 bec_lib-1.9.0/bec_lib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      501 2024-02-22 19:50:20.724886 bec_lib-1.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      808 2024-02-22 19:50:16.000000 bec_lib-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.120440 bec_lib-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)     3013 2024-04-11 06:21:55.120440 bec_lib-2.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2616 2024-04-10 11:18:35.000000 bec_lib-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.119439 bec_lib-2.0.1/bec_lib/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3901 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/alarm_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/async_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/bec_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    16590 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/bec_plotter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11292 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/bec_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     7247 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/bl_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2426 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/bl_conditions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5952 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/callback_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/channel_monitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     9024 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     8854 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/config_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.119439 bec_lib-2.0.1/bec_lib/configs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 06:21:44.000000 bec_lib-2.0.1/bec_lib/configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    38908 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/configs/demo_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)   289604 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/configs/openapi_schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     4461 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/connector.py
+-rw-rw-rw-   0 root         (0) root         (0)    12816 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/dap_plugin_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     3935 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/dap_plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)    30828 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/device.py
+-rw-rw-rw-   0 root         (0) root         (0)    23274 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/devicemanager.py
+-rw-rw-rw-   0 root         (0) root         (0)    37595 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/endpoints.py
+-rw-rw-rw-   0 root         (0) root         (0)     9233 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/file_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/lmfit_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2546 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/logbook_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)     6960 2024-04-10 19:08:49.000000 bec_lib-2.0.1/bec_lib/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    20005 2024-04-10 19:08:49.000000 bec_lib-2.0.1/bec_lib/messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     5027 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/numpy_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     5177 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/observer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/pdf_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     7491 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/queue_items.py
+-rw-rw-rw-   0 root         (0) root         (0)    36071 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/redis_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)     5664 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/request_items.py
+-rw-rw-rw-   0 root         (0) root         (0)     6526 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/scan_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10892 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/scan_items.py
+-rw-rw-rw-   0 root         (0) root         (0)     8573 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/scan_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     6097 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/scan_report.py
+-rw-rw-rw-   0 root         (0) root         (0)    17027 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/scans.py
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/scibec_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)    10200 2024-04-10 19:08:49.000000 bec_lib-2.0.1/bec_lib/serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)     3126 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/service_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     4688 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/signature_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.120440 bec_lib-2.0.1/bec_lib/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 06:21:44.000000 bec_lib-2.0.1/bec_lib/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8004 2024-04-10 19:08:49.000000 bec_lib-2.0.1/bec_lib/tests/end2end_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)     1594 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/tests/fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)    41009 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/tests/test_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/tests/test_service_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    23107 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/tests/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4780 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/user_scripts_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     7636 2024-04-10 11:18:35.000000 bec_lib-2.0.1/bec_lib/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:55.120440 bec_lib-2.0.1/bec_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3013 2024-04-11 06:21:55.000000 bec_lib-2.0.1/bec_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1531 2024-04-11 06:21:55.000000 bec_lib-2.0.1/bec_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 06:21:55.000000 bec_lib-2.0.1/bec_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      183 2024-04-11 06:21:55.000000 bec_lib-2.0.1/bec_lib.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      258 2024-04-11 06:21:55.000000 bec_lib-2.0.1/bec_lib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 06:21:55.000000 bec_lib-2.0.1/bec_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-11 06:21:55.121440 bec_lib-2.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2024-04-11 06:21:52.000000 bec_lib-2.0.1/setup.py
```

### Comparing `bec_lib-1.9.0/PKG-INFO` & `bec_lib-2.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: bec_lib
-Version: 1.9.0
+Version: 2.0.1
 Summary: BEC library
 Home-page: https://gitlab.psi.ch/bec/bec
-License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # BEC Lib
 
 bec-lib is a Python library communicating with the [Beamline and Experiment Control (BEC)](https://gitlab.psi.ch/bec/bec) server. It is primarily used to build new BEC clients such as graphical user interfaces (GUIs) or command line interfaces (CLIs).
 
@@ -86,9 +84,7 @@
 
 
 Please make sure to update tests as necessary.
 
 ## License
 
 [BSD-3-Clause](https://choosealicense.com/licenses/bsd-3-clause/)
-
-
```

### Comparing `bec_lib-1.9.0/README.md` & `bec_lib-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bec_lib-1.9.0/bec_lib/alarm_handler.py` & `bec_lib-2.0.1/bec_lib/alarm_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This module provides the alarm handler class and its related functionality.
+"""
+
 from __future__ import annotations
 
 import enum
 import threading
 from collections import deque
 from typing import TYPE_CHECKING
 
@@ -44,31 +48,29 @@
             f" {self.alarm.content['msg']}"
         )
 
 
 class AlarmHandler:
     def __init__(self, connector: RedisConnector) -> None:
         self.connector = connector
-        self.alarm_consumer = None
         self.alarms_stack = deque(maxlen=100)
         self._raised_alarms = deque(maxlen=100)
         self._lock = threading.RLock()
 
     def start(self):
         """start the alarm handler and its subscriptions"""
-        self.alarm_consumer = self.connector.consumer(
+        self.connector.register(
             topics=MessageEndpoints.alarm(),
             name="AlarmHandler",
-            cb=self._alarm_consumer_callback,
+            cb=self._alarm_register_callback,
             parent=self,
         )
-        self.alarm_consumer.start()
 
     @staticmethod
-    def _alarm_consumer_callback(msg, *, parent, **_kwargs):
+    def _alarm_register_callback(msg, *, parent, **_kwargs):
         parent.add_alarm(msg.value)
 
     @threadlocked
     def add_alarm(self, msg: messages.AlarmMessage):
         """Add a new alarm message to the stack.
 
         Args:
@@ -107,15 +109,14 @@
             severity (Alarm, optional): Minimum severity. Defaults to Alarms.WARNING.
 
         Yields:
             AlarmBase: Alarm
         """
         alarms = self.get_unhandled_alarms(severity=severity)
         for alarm in alarms:
-            self.alarms_stack.remove(alarm)
             yield alarm
 
     def raise_alarms(self, severity=Alarms.MAJOR):
         """Raise unhandled alarms with specified severity.
 
         Args:
             severity (Alarm, optional): Minimum severity. Defaults to Alarms.MAJOR.
@@ -132,8 +133,8 @@
     @threadlocked
     def clear(self):
         """clear all alarms from stack"""
         self.alarms_stack.clear()
 
     def shutdown(self):
         """shutdown the alarm handler"""
-        self.alarm_consumer.shutdown()
+        self.connector.shutdown()
```

### Comparing `bec_lib-1.9.0/bec_lib/async_data.py` & `bec_lib-2.0.1/bec_lib/async_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,47 @@
+"""
+This module contains the AsyncDataHandler class which is used to receive and store async device data from the BEC.
+"""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 from bec_lib.endpoints import MessageEndpoints
 
 if TYPE_CHECKING:
     from bec_lib import messages
-    from bec_lib.redis_connector import RedisProducer
+    from bec_lib.connector import ConnectorBase
 
 
 class AsyncDataHandler:
-    def __init__(self, producer: RedisProducer):
-        self.producer = producer
+    def __init__(self, connector: ConnectorBase):
+        self.connector = connector
 
     def get_async_data_for_scan(self, scan_id: str) -> dict[list]:
         """
         Get the async data for a given scan.
 
         Args:
             scan_id(str): the scan id to get the async data for
 
         Returns:
             dict[list]: the async data for the scan sorted by device name
         """
-        async_device_keys = self.producer.keys(MessageEndpoints.device_async_readback(scan_id, "*"))
+        async_device_keys = self.connector.keys(
+            MessageEndpoints.device_async_readback(scan_id, "*")
+        )
         async_data = {}
         for device_key in async_device_keys:
             key = device_key.decode()
-            device_name = key.split(MessageEndpoints.device_async_readback(scan_id, ""))[-1].split(
-                ":"
-            )[0]
+            device_name = key.split(MessageEndpoints.device_async_readback(scan_id, "").endpoint)[
+                -1
+            ].split(":")[0]
             data = self.get_async_data_for_device(scan_id, device_name)
             if not data:
                 continue
             async_data[device_name] = data
         return async_data
 
     def get_async_data_for_device(self, scan_id: str, device_name: str) -> list:
@@ -46,15 +52,15 @@
             scan_id(str): the scan id to get the async data for
             device_name(str): the device name to get the async data for
 
         Returns:
             list: the async data for the device
         """
         key = MessageEndpoints.device_async_readback(scan_id, device_name)
-        msgs = self.producer.xrange(key, min="-", max="+")
+        msgs = self.connector.xrange(key, min="-", max="+")
         if not msgs:
             return []
         return self.process_async_data(msgs)
 
     @staticmethod
     def process_async_data(msgs: list[messages.DeviceMessage]) -> dict | list[dict]:
         """
```

### Comparing `bec_lib-1.9.0/bec_lib/bec_plotter.py` & `bec_lib-2.0.1/bec_lib/bec_plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # pylint: disable = missing-module-docstring
+"""
+This module provides the BECPlotter class and its related functionality.
+"""
 from __future__ import annotations
 
 import builtins
 import importlib
 import json
 import select
 import subprocess
@@ -50,76 +53,76 @@
     """
     A class to connect to the BEC widgets.
     """
 
     def __init__(self, gui_id: str, bec_client: BECClient = None) -> None:
         self._client = bec_client
         self.gui_id = gui_id
-        # TODO replace with a global producer
+        # TODO replace with a global connector
         if self._client is None:
             if "bec" in builtins.__dict__:
                 self._client = builtins.bec
             else:
                 self._client = BECClient()
                 self._client.start()
-        self._producer = self._client.connector.producer()
+        self._connector = self._client.connector
 
     def set_plot_config(self, plot_id: str, config: dict) -> None:
         """
         Set the plot config.
 
         Args:
             plot_id (str): The id of the plot.
             config (dict): The config to set.
         """
         msg = messages.GUIConfigMessage(config=config)
-        self._producer.set_and_publish(MessageEndpoints.gui_config(plot_id), msg)
+        self._connector.set_and_publish(MessageEndpoints.gui_config(plot_id), msg)
 
     def close(self, plot_id: str) -> None:
         """
         Close the plot.
 
         Args:
             plot_id (str): The id of the plot.
         """
         msg = messages.GUIInstructionMessage(action="close", parameter={})
-        self._producer.set_and_publish(MessageEndpoints.gui_instructions(plot_id), msg)
+        self._connector.set_and_publish(MessageEndpoints.gui_instructions(plot_id), msg)
 
     def config_dialog(self, plot_id: str) -> None:
         """
         Open the config dialog.
 
         Args:
             plot_id (str): The id of the plot.
         """
         msg = messages.GUIInstructionMessage(action="config_dialog", parameter={})
-        self._producer.set_and_publish(MessageEndpoints.gui_instructions(plot_id), msg)
+        self._connector.set_and_publish(MessageEndpoints.gui_instructions(plot_id), msg)
 
     def send_data(self, plot_id: str, data: dict) -> None:
         """
         Send data to the plot.
 
         Args:
             plot_id (str): The id of the plot.
             data (dict): The data to send.
         """
         msg = messages.GUIDataMessage(data=data)
-        self._producer.set_and_publish(topic=MessageEndpoints.gui_data(plot_id), msg=msg)
+        self._connector.set_and_publish(topic=MessageEndpoints.gui_data(plot_id), msg=msg)
         # TODO bec_dispatcher can only handle set_and_publish ATM
-        # self._producer.xadd(topic=MessageEndpoints.gui_data(plot_id),msg= {"data": msg})
+        # self._connector.xadd(topic=MessageEndpoints.gui_data(plot_id),msg= {"data": msg})
 
     def clear(self, plot_id: str) -> None:
         """
         Clear the plot.
 
         Args:
             plot_id (str): The id of the plot.
         """
         msg = messages.GUIInstructionMessage(action="clear", parameter={})
-        self._producer.set_and_publish(MessageEndpoints.gui_instructions(plot_id), msg)
+        self._connector.set_and_publish(MessageEndpoints.gui_instructions(plot_id), msg)
 
 
 class BECPlotter:
     """
     A class to plot data from the BEC. Internally, it uses redis to communicate with the plot running
     in a separate process.
     """
```

### Comparing `bec_lib-1.9.0/bec_lib/bec_service.py` & `bec_lib-2.0.1/bec_lib/bec_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This module provides the BECService class, which is the base class for all BEC services.
+"""
+
 from __future__ import annotations
 
 import getpass
 import socket
 import threading
 import time
 import uuid
@@ -37,15 +41,15 @@
     ) -> None:
         super().__init__()
         self._import_config(config)
         self._connector_cls = connector_cls
         self.connector = connector_cls(self.bootstrap_server)
         self._unique_service = unique_service
         self.wait_for_server = wait_for_server
-        self.producer = self.connector.producer()
+        self.__service_id = str(uuid.uuid4())
         self._user = getpass.getuser()
         self._hostname = socket.gethostname()
         self._service_info_thread = None
         self._service_info_event = threading.Event()
         self._metrics_emitter_thread = None
         self._metrics_emitter_event = threading.Event()
         self._services_info = {}
@@ -53,16 +57,24 @@
         self._check_services()
         self._status = BECStatus.BUSY
         self._start_update_service_info()
         self._start_metrics_emitter()
         self._wait_for_server()
 
     @property
-    def _service_id(self) -> str:
-        return str(uuid.uuid4())
+    def _service_name(self):
+        return (
+            self.__class__.__name__
+            if self._unique_service
+            else f"{self.__class__.__name__}/{self._service_id}"
+        )
+
+    @property
+    def _service_id(self):
+        return self.__service_id
 
     def _import_config(self, config: str | ServiceConfig) -> None:
         if isinstance(config, str):
             self._service_config = ServiceConfig(config_path=config)
         elif isinstance(config, ServiceConfig):
             self._service_config = config
         else:
@@ -93,40 +105,44 @@
         except RuntimeError as service_error:
             if elapsed_time > timeout_time:
                 raise RuntimeError from service_error
         return True
 
     def _initialize_logger(self) -> None:
         bec_logger.configure(
-            self.bootstrap_server, self._connector_cls, service_name=self.__class__.__name__
+            self.bootstrap_server,
+            self._connector_cls,
+            service_name=self.__class__.__name__,
+            service_config=self._service_config.config["service_config"],
         )
 
     def _update_existing_services(self):
-        service_keys = self.producer.keys(MessageEndpoints.service_status("*"))
+        service_keys = self.connector.keys(MessageEndpoints.service_status("*").endpoint)
         if not service_keys:
             return
         services = [service.decode().split(":", maxsplit=1)[0] for service in service_keys]
-        msgs = [self.producer.get(service) for service in services]
+        msgs = [self.connector.get(service) for service in services]
         self._services_info = {msg.content["name"]: msg for msg in msgs if msg is not None}
 
     def _update_service_info(self):
         while not self._service_info_event.is_set():
             logger.trace("Updating service info")
-            self._send_service_status()
+            try:
+                self._send_service_status()
+            except Exception:
+                # exception is not explicitely specified,
+                # because it depends on the underlying connector
+                pass
             self._service_info_event.wait(timeout=3)
 
     def _send_service_status(self):
-        self.producer.set_and_publish(
+        self.connector.set_and_publish(
             topic=MessageEndpoints.service_status(self._service_id),
             msg=messages.StatusMessage(
-                name=(
-                    self.__class__.__name__
-                    if self._unique_service
-                    else f"{self.__class__.__name__}/{self._service_id}"
-                ),
+                name=self._service_name,
                 status=self.status,
                 info={"user": self._user, "hostname": self._hostname, "timestamp": time.time()},
             ),
             expire=6,
         )
 
     @property
@@ -180,54 +196,59 @@
                     pid=res["pid"],
                     memory_in_mb=res["memory_info"].rss / 1024 / 1024,
                     memory_used_percent=res["memory_percent"],
                     create_time=res["create_time"],
                 )
             )
             msg = messages.ServiceMetricMessage(name=self.__class__.__name__, metrics=data)
-            self.producer.send(MessageEndpoints.metrics(self._service_id), msg)
+            try:
+                self.connector.send(MessageEndpoints.metrics(self._service_id), msg)
+            except Exception:
+                # exception is not explicitely specified,
+                # because it depends on the underlying connector
+                pass
             self._metrics_emitter_event.wait(timeout=1)
 
     def set_global_var(self, name: str, val: Any) -> None:
         """Set a global variable through Redis
 
         Args:
             name (str): Name of the variable
             val (Any): Value of the variable
 
         """
-        self.producer.set(MessageEndpoints.global_vars(name), messages.VariableMessage(value=val))
+        self.connector.set(MessageEndpoints.global_vars(name), messages.VariableMessage(value=val))
 
     def get_global_var(self, name: str) -> Any:
         """Get a global variable from Redis
 
         Args:
             name (str): Name of the variable
 
         Returns:
             Any: Value of the variable
         """
-        msg = self.producer.get(MessageEndpoints.global_vars(name))
+        msg = self.connector.get(MessageEndpoints.global_vars(name))
         if msg:
             return msg.content.get("value")
         return None
 
     def delete_global_var(self, name: str) -> None:
         """Delete a global variable from Redis
 
         Args:
             name (str): Name of the variable
 
         """
-        self.producer.delete(MessageEndpoints.global_vars(name))
+        self.connector.delete(MessageEndpoints.global_vars(name))
 
     def global_vars(self) -> str:
         """Get all available global variables"""
         # sadly, this cannot be a property as it causes side effects with IPython's tab completion
-        available_keys = self.producer.keys(MessageEndpoints.global_vars("*"))
+        available_keys = self.connector.keys(MessageEndpoints.global_vars("*"))
 
         def get_endpoint_from_topic(topic: str) -> str:
             return topic.decode().split(MessageEndpoints.global_vars(""))[-1]
 
         endpoints = [get_endpoint_from_topic(k) for k in available_keys]
 
         console = Console()
@@ -243,20 +264,24 @@
             console.print(table)
         out = capture.get()
         logger.info(out)
         print(out)
 
     def shutdown(self):
         """shutdown the BECService"""
-        self._service_info_event.set()
-        if self._service_info_thread:
-            self._service_info_thread.join()
-        self._metrics_emitter_event.set()
-        if self._metrics_emitter_thread:
-            self._metrics_emitter_thread.join()
+        try:
+            self.connector.shutdown()
+            self._service_info_event.set()
+            if self._service_info_thread:
+                self._service_info_thread.join()
+            self._metrics_emitter_event.set()
+            if self._metrics_emitter_thread:
+                self._metrics_emitter_thread.join()
+        except AttributeError:
+            print("Failed to shutdown BECService.")
 
     @property
     def service_status(self):
         """get the status of active services"""
         self._update_existing_services()
         return self._services_info
```

### Comparing `bec_lib-1.9.0/bec_lib/bl_checks.py` & `bec_lib-2.0.1/bec_lib/bl_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+This module provides the BeamlineChecks class, which is used to perform beamline checks. It also provides the bl_check
+decorator. 
+"""
+
 import builtins
 import datetime
 import functools
 import threading
 import time
 from collections import deque
 from uuid import uuid4
@@ -37,15 +42,15 @@
 def _run_with_bl_checks(bl_checks, fcn, *args, **kwargs):
     # pylint: disable=protected-access
     chk = {"id": str(uuid4()), "fcn": fcn, "args": args, "kwargs": kwargs}
     bl_checks._levels.append(chk)
     nested_call = len(bl_checks._levels) > 1
     if bl_checks._is_paused and bl_checks._beamline_checks:
         logger.warning(
-            f"Beamline checks are currently paused. Use `bec.bl_checks.resume()` to reactivate them."
+            "Beamline checks are currently paused. Use `bec.bl_checks.resume()` to reactivate them."
         )
     try:
         if nested_call:
             # check if the beam was okay so far
             if not bl_checks.beam_is_okay:
                 raise BeamlineCheckError("Beam is not okay.")
         else:
@@ -178,14 +183,15 @@
         """Start the beamline checks."""
         if self._started:
             return
         self._beam_is_okay = True
 
         self._beam_check_thread = threading.Thread(target=self._check_beam, daemon=True)
         self._beam_check_thread.start()
+        self._started = True
 
     def stop(self):
         """Stop the beamline checks"""
         if not self._started:
             return
 
         self._stop_beam_check_event.set()
```

### Comparing `bec_lib-1.9.0/bec_lib/bl_conditions.py` & `bec_lib-2.0.1/bec_lib/bl_conditions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This module contains classes for beamline checks, used to check the beamline status.
+"""
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from bec_lib.device import Device
```

### Comparing `bec_lib-1.9.0/bec_lib/callback_handler.py` & `bec_lib-2.0.1/bec_lib/callback_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""
+This module contains the CallbackHandler class to handle callbacks. 
+The CallbackHandler class is used to register and run callbacks for different 
+event types. The CallbackRegister class is used to register callbacks 
+in a with statement.
+"""
+
 import builtins
 import enum
 import threading
 import traceback
 from collections import deque
 from collections.abc import Callable
```

### Comparing `bec_lib-1.9.0/bec_lib/client.py` & `bec_lib-2.0.1/bec_lib/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,118 +1,144 @@
+"""
+BECClient class. This class is the main entry point for the BEC client and all 
+derived classes. It is used to initialize the client and start the client.
+"""
+
 from __future__ import annotations, print_function
 
 import builtins
+import getpass
 import importlib
 import inspect
-import subprocess
 from typing import TYPE_CHECKING
 
 from rich.console import Console
 from rich.table import Table
 
+from bec_lib import messages
 from bec_lib.alarm_handler import AlarmHandler, Alarms
 from bec_lib.bec_service import BECService
 from bec_lib.bl_checks import BeamlineChecks
 from bec_lib.callback_handler import CallbackHandler
-from bec_lib.config_helper import ConfigHelper
 from bec_lib.dap_plugins import DAPPlugins
 from bec_lib.devicemanager import DeviceManagerBase
 from bec_lib.endpoints import MessageEndpoints
-from bec_lib.logbook_connector import LogbookConnector
 from bec_lib.logger import bec_logger
 from bec_lib.redis_connector import RedisConnector
 from bec_lib.scan_manager import ScanManager
 from bec_lib.scans import Scans
 from bec_lib.service_config import ServiceConfig
 from bec_lib.user_scripts_mixin import UserScriptsMixin
 
 if TYPE_CHECKING:
     from bec_lib.connector import ConnectorBase
 
 logger = bec_logger.logger
 
 
 class BECClient(BECService, UserScriptsMixin):
-    def __init__(self, forced=False) -> None:
-        pass
-
-    def __new__(cls, *args, forced=False, **kwargs):
-        if not hasattr(cls, "_client") or forced or cls._client is None:
-            cls._client = super(BECClient, cls).__new__(cls)
-            cls._initialized = False
-        return cls._client
+    """
+    The BECClient class is the main entry point for the BEC client and all derived classes.
+    """
+
+    _client = None
+    _initialized = False
+    started = False
 
-    def __str__(self) -> str:
-        return "BECClient\n\nTo get a list of available commands, type `bec.show_all_commands()`"
-
-    def initialize(
+    def __init__(
         self,
         config: ServiceConfig = None,
         connector_cls: ConnectorBase = None,
         wait_for_server=False,
+        forced=False,
+        parent=None,
     ) -> None:
         """
-        Initialize the client.
+        Initialize the BECClient
 
         Args:
-            config (ServiceConfig, optional): ServiceConfig object. Defaults to None. If None, default config will be used.
-            connector_cls (ConnectorBase, optional): Connector class. Defaults to None. If None, RedisConnector will be used.
-            wait_for_server (bool, optional): Wait for BEC server to be available. Defaults to False.
+            config (ServiceConfig, optional): The configuration for the client. Defaults to None.
+            connector_cls (ConnectorBase, optional): The connector class to use. Defaults to None.
+            wait_for_server (bool, optional): Whether to wait for the server to be available before starting. Defaults to False.
+            forced (bool, optional): Whether to force the initialization of a new client. Defaults to False.
         """
-        if not config:
-            config = ServiceConfig()
-
-        if not connector_cls:
-            connector_cls = RedisConnector
-        super().__init__(config, connector_cls, wait_for_server=wait_for_server)
-        self._configure_logger()
-        # pylint: disable=attribute-defined-outside-init
+        if self._initialized:
+            return
+        self.__init_params = {
+            "config": config if config is not None else ServiceConfig(),
+            "connector_cls": connector_cls if connector_cls is not None else RedisConnector,
+            "wait_for_server": wait_for_server,
+        }
         self.device_manager = None
         self.queue = None
         self.alarm_handler = None
-        self._load_scans()
-        self._hli_funcs = {}
-        self._initialized = True
         self.config = None
-        builtins.bec = self
-        self.metadata = {}
-        # self.logbook = LogbookConnector(self.connector)
-        self._update_username()
         self.history = None
-        self.callbacks = CallbackHandler()
         self.live_updates = None
         self.dap = None
         self.bl_checks = None
+        self._hli_funcs = {}
+        self.metadata = {}
+        self.file_writer_data = {}
+        self.callbacks = None
+        self._parent = parent if parent is not None else self
+        self._initialized = True
+
+    def __new__(cls, *args, forced=False, **kwargs):
+        if forced or cls._client is None:
+            cls._client = super(BECClient, cls).__new__(cls)
+            cls._initialized = False
+        return cls._client
+
+    def __str__(self) -> str:
+        return "BECClient\n\nTo get a list of available commands, type `bec.show_all_commands()`"
+
+    @classmethod
+    def _reset_singleton(cls):
+        cls._client = None
+        cls._initialized = False
+        cls.started = False
 
     @property
     def username(self) -> str:
         """get the current username"""
         return self._username
 
     @property
     def active_account(self) -> str:
         """get the currently active target (e)account"""
-        return self.producer.get(MessageEndpoints.account())
+        msg = self.connector.get(MessageEndpoints.account())
+        if msg:
+            return msg.value
+        return ""
 
     def start(self):
         """start the client"""
-        if not self._initialized:
-            logger.warning(
-                "Client has not been initialized with 'client.initialize(config, connector_cls)'."
-                " Trying to initialize with default values."
-            )
-            self.initialize()
-
+        if self.started:
+            return
+        self.started = True
+        config = self.__init_params["config"]
+        connector_cls = self.__init_params["connector_cls"]
+        wait_for_server = self.__init_params["wait_for_server"]
+        super().__init__(config, connector_cls, wait_for_server=wait_for_server)
+        builtins.bec = self._parent
+        self._start_services()
         logger.info("Starting new client")
+
+    def _start_services(self):
+        self._configure_logger()
+        self._load_scans()
+        # self.logbook = LogbookConnector(self.connector)
+        self._update_username()
+        self.callbacks = CallbackHandler()
         self._start_device_manager()
         self._start_scan_queue()
         self._start_alarm_handler()
-
         self.load_all_user_scripts()
-        self.config = ConfigHelper(self.connector)
+        self.config = self.device_manager.config_helper
         self.history = self.queue.queue_storage.storage
         self.dap = DAPPlugins(self)
         self.bl_checks = BeamlineChecks(self)
         self.bl_checks.start()
 
     def alarms(self, severity=Alarms.WARNING):
         """get the next alarm with at least the specified severity"""
@@ -127,41 +153,38 @@
             print(alarm)
 
     def clear_all_alarms(self):
         """remove all alarms from stack"""
         self.alarm_handler.clear()
 
     @property
-    def pre_scan_hooks(self):
-        """currently stored pre-scan hooks"""
-        return self.producer.lrange(MessageEndpoints.pre_scan_macros(), 0, -1)
-
-    @pre_scan_hooks.setter
-    def pre_scan_hooks(self, hooks: list):
-        self.producer.delete(MessageEndpoints.pre_scan_macros())
+    def pre_scan_macros(self):
+        """currently stored pre-scan macros"""
+        return self.connector.lrange(MessageEndpoints.pre_scan_macros(), 0, -1)
+
+    @pre_scan_macros.setter
+    def pre_scan_macros(self, hooks: list[str]):
+        self.connector.delete(MessageEndpoints.pre_scan_macros())
         for hook in hooks:
-            self.producer.lpush(MessageEndpoints.pre_scan_macros(), hook)
+            msg = messages.VariableMessage(value=hook)
+            self.connector.lpush(MessageEndpoints.pre_scan_macros(), msg)
 
     def _load_scans(self):
-        self.scans = Scans(self)
+        self.scans = Scans(self._parent)
         builtins.scans = self.scans
 
     def load_high_level_interface(self, module_name):
         mod = importlib.import_module(f"bec_client.high_level_interfaces.{module_name}")
         members = inspect.getmembers(mod)
         funcs = {name: func for name, func in members if not name.startswith("__")}
         self._hli_funcs = funcs
         builtins.__dict__.update(funcs)
 
     def _update_username(self):
-        self._username = (
-            subprocess.run("whoami", shell=True, stdout=subprocess.PIPE)
-            .stdout.decode()
-            .split("\n")[0]
-        )
+        self._username = getpass.getuser()
 
     def _start_scan_queue(self):
         self.queue = ScanManager(self.connector)
 
     def _configure_logger(self):
         bec_logger.logger.remove()
         bec_logger.add_file_log(bec_logger.LOGLEVEL.DEBUG)
@@ -177,21 +200,26 @@
     def _start_alarm_handler(self):
         logger.info("Starting alarm listener")
         self.alarm_handler = AlarmHandler(self.connector)
         self.alarm_handler.start()
 
     def shutdown(self):
         """shutdown the client and all its components"""
-        super().shutdown()
+        if self.started:
+            super().shutdown()
         if self.device_manager:
             self.device_manager.shutdown()
         if self.queue:
             self.queue.shutdown()
         if self.alarm_handler:
             self.alarm_handler.shutdown()
+        if self.bl_checks:
+            self.bl_checks.stop()
+        bec_logger.logger.remove()
+        self.started = False
 
     def _print_available_commands(self, title: str, data: tuple) -> None:
         console = Console()
         table = Table(title=title)
         table.add_column("Name", justify="center")
         table.add_column("Description", justify="center")
         for name, descr in data:
```

### Comparing `bec_lib-1.9.0/bec_lib/configs/demo_config.yaml` & `bec_lib-2.0.1/bec_lib/tests/test_config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -18,288 +18,281 @@
 dyn_signals:
   readoutPriority: baseline
   deviceClass: sim:sim:SynDynamicComponents
   deviceConfig:
   enabled: true
   readOnly: false
 
-############################################################
-####################### User motors ########################
-############################################################
-
-hexapod:
+pseudo_signal1:
+  deviceClass: ComputedSignal
+  deviceConfig:
+    compute_method: "def compute_signals(signal1, signal2):\n    return signal1.get()*signal2.get()\n"
+    input_signals: 
+      - "bpm4i_readback"
+      - "bpm5i_readback"
+  enabled: true
+  readOnly: false
   readoutPriority: baseline
-  deviceClass: SynDeviceOPAAS
+
+failure_device:
+  deviceClass: sim:sim:SimPositionerWithCommFailure
   deviceConfig:
-  deviceTags:
-    - user motors
+    delay: 1
+    update_frequency: 400
   enabled: true
   readOnly: false
+  readoutPriority: baseline
+
+############################################################
+####################### User motors ########################
+############################################################
 
 eyefoc:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 eyex:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 eyey:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 flyer_sim:
   readoutPriority: on_request
   deviceClass: SynFlyer
   deviceConfig:
     delay: 1    
     device_access: true
-    speed: 100
     update_frequency: 400
   deviceTags:
     - flyer
   enabled: true
   readOnly: false
 hrox:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hroy:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hroz:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hy:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hz:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 mbsx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 mbsy:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 pinx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 piny:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 pinz:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 samx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 samy:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 samz:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 
@@ -309,15 +302,14 @@
 #################### Beamline monitors #####################
 ############################################################
 
 bpm3a:
   readoutPriority: monitored
   deviceClass: SimMonitor
   deviceConfig:
-  deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm3b:
   readoutPriority: monitored
   deviceClass: SimMonitor
@@ -686,1566 +678,1424 @@
 ############################################################
 
 aptrx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 aptry:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bim2x:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bim2y:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm1trx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm1try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm2trx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm2try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm3trx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm3try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm4trx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm4try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm5trx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm5try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm6trx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm6try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4r:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5r:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bs1x:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bs1y:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bs2x:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bs2y:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 burstn:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 burstr:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1a:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1b:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1c:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1d:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1e:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1f:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1g:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1h:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dettrx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 di2trx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 di2try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dtpush:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dtth:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dttrx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dttry:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dttrz:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebcsx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebcsy:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfi1:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfi2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfi3:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfi4:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfzpx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfzpy:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebtrx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebtry:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebtrz:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fi1try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fi2try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fi3try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fsh1x:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fsh2x:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ftrans:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttrx1:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttrx2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttry1:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttry2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttrz:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 idgap:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mibd:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mibd1:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mibd2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 miroll:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mith:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitrx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitry:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitry1:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitry2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitry3:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobd:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobdai:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobdbo:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobdco:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobddi:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mokev:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mopush1:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mopush2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moroll1:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moroll2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moth1:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moth1e:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moth2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moth2e:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motrx2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motry:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motry2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motrz1:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motrz1e:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moyaw2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl0ch:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl0trxi:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl0trxo:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl0wh:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1ch:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1cv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1trxi:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1trxo:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1tryb:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1tryt:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1wh:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1wv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2ch:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2cv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2trxi:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2trxo:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2tryb:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2tryt:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2wh:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2wv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3ch:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3cv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3trxi:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3trxo:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3tryb:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3tryt:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3wh:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3wv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4ch:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4cv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4trxi:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4trxo:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4tryb:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4tryt:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4wh:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4wv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5ch:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5cv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5trxi:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5trxo:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5tryb:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5tryt:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5wh:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5wv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 strox:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 stroy:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 stroz:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sttrx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sttry:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 
 ################# Beamline motors end here #################
@@ -2260,7 +2110,101 @@
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ################ Read-only signals end here ################
 
+
+############################################################
+##################### Disabled devices #####################
+############################################################
+
+motor1_disabled:
+  readoutPriority: monitored
+  deviceClass: SimPositioner
+  deviceConfig:
+    delay: 1
+    labels: motor1_disabled
+    limits:
+    - -50
+    - 50
+    name: motor1_disabled
+    tolerance: 0.01
+    update_frequency: 400
+  deviceTags:
+  - user motors
+  enabled: false
+  readOnly: false
+motor1_disabled_set:
+  readoutPriority: baseline
+  deviceClass: SimPositioner
+  deviceConfig:
+    delay: 1
+    labels: motor1_disabled_set
+    limits:
+    - -50
+    - 50
+    name: motor1_disabled_set
+    tolerance: 0.01
+    update_frequency: 400
+  deviceTags:
+  - user motors
+  enabled: true
+  readOnly: true
+motor2_disabled:
+  readoutPriority: baseline
+  deviceClass: SimPositioner
+  deviceConfig:
+    delay: 1
+    labels: motor2_disabled
+    limits:
+    - -50
+    - 50
+    name: motor2_disabled
+    tolerance: 0.01
+    update_frequency: 400
+  deviceTags:
+  - user motors
+  enabled: false
+  readOnly: false
+motor2_disabled_set:
+  readoutPriority: baseline
+  deviceClass: SimPositioner
+  deviceConfig:
+    delay: 1
+    labels: motor2_disabled_set
+    limits:
+    - -50
+    - 50
+    name: motor2_disabled_set
+    tolerance: 0.01
+    update_frequency: 400
+  deviceTags:
+  - user motors
+  enabled: true
+  readOnly: true
+######### DeviceProxy and SimCamera for delayed init tests ##########
+proxy_cam_test:
+  readoutPriority: monitored
+  deviceClass: SimCamera
+  deviceConfig:
+    device_access: true
+  deviceTags:
+    - detector
+  enabled: true
+  readOnly: false
+  softwareTrigger: false
+sim_proxy_test:
+  readoutPriority: on_request
+  deviceClass: SlitProxy
+  deviceConfig:
+    proxy_cam_test:
+      signal_name: image
+      center_offset: [0, 0] # [x,y]
+      covariance: [[1000, 500], [200, 1000]] # [[x,x],[y,y]]
+      pixel_size: 0.01
+      ref_motors: [samx, samy]
+      slit_width: [1, 1]
+      motor_dir: [0, 1] # x:0 , y:1, z:2 coordinates
+  enabled: true
+  readOnly: false
```

### Comparing `bec_lib-1.9.0/bec_lib/configs/openapi_schema.json` & `bec_lib-2.0.1/bec_lib/configs/openapi_schema.json`

 * *Files identical despite different names*

### Comparing `bec_lib-1.9.0/bec_lib/dap_plugin_objects.py` & `bec_lib-2.0.1/bec_lib/dap_plugin_objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This module contains the base classes for DAP plugin objects. These classes should be used to create custom DAP plugin objects.
+"""
+
 from __future__ import annotations
 
 import builtins
 import time
 import uuid
 from typing import TYPE_CHECKING
 
@@ -10,14 +14,15 @@
 from typeguard import typechecked
 
 from bec_lib import messages
 from bec_lib.device import DeviceBase
 from bec_lib.endpoints import MessageEndpoints
 from bec_lib.lmfit_serializer import serialize_param_object
 from bec_lib.scan_items import ScanItem
+from bec_lib.scan_report import ScanReport
 
 if TYPE_CHECKING:
     from bec_lib.client import BECClient
 
 try:
     import matplotlib.pyplot as plt
 
@@ -60,29 +65,33 @@
         # run must be an anonymous function to allow for multiple doc strings
         self._user_run = lambda *args, **kwargs: self._run(*args, **kwargs)
 
     def _run(self, *args, **kwargs):
         converted_args = []
         for arg in args:
             if isinstance(arg, ScanItem):
-                converted_args.append(arg.scanID)
+                converted_args.append(arg.scan_id)
+            elif isinstance(arg, ScanReport):
+                converted_args.append(arg.scan.scan_id)
             else:
                 converted_args.append(arg)
         args = converted_args
         converted_kwargs = {}
         for key, val in kwargs.items():
             if isinstance(val, ScanItem):
-                converted_kwargs[key] = val.scanID
+                converted_kwargs[key] = val.scan_id
+            elif isinstance(arg, ScanReport):
+                converted_kwargs[key] = arg.scan.scan_id
             elif isinstance(val, lmfit.Parameter):
                 converted_kwargs[key] = serialize_param_object(val)
             else:
                 converted_kwargs[key] = val
         kwargs = converted_kwargs
         request_id = str(uuid.uuid4())
-        self._client.producer.set_and_publish(
+        self._client.connector.set_and_publish(
             MessageEndpoints.dap_request(),
             messages.DAPRequestMessage(
                 dap_cls=self._plugin_info["class"],
                 dap_type="on_demand",
                 config={
                     "args": args,
                     "kwargs": kwargs,
@@ -106,15 +115,15 @@
 
     def _wait_for_dap_response(self, request_id: str, timeout: float = 5.0):
         start_time = time.time()
 
         while True:
             if time.time() - start_time > timeout:
                 raise TimeoutError("Timeout waiting for DAP response.")
-            response = self._client.producer.get(MessageEndpoints.dap_response(request_id))
+            response = self._client.connector.get(MessageEndpoints.dap_response(request_id))
             if not response:
                 time.sleep(0.005)
                 continue
 
             if response.metadata["RID"] != request_id:
                 time.sleep(0.005)
                 continue
@@ -124,15 +133,15 @@
             raise RuntimeError(response.content["error"])
 
     def _update_dap_config(self, request_id: str = None):
         if not self._plugin_config.get("selected_device"):
             return
         self._plugin_config["class_args"] = self._plugin_info.get("class_args")
         self._plugin_config["class_kwargs"] = self._plugin_info.get("class_kwargs")
-        self._client.producer.set_and_publish(
+        self._client.connector.set_and_publish(
             MessageEndpoints.dap_request(),
             messages.DAPRequestMessage(
                 dap_cls=self._plugin_info["class"],
                 dap_type="continuous",
                 config=self._plugin_config,
                 metadata={"RID": request_id},
             ),
@@ -145,15 +154,15 @@
     To customize a plugin, create a new class that inherits from this class and override the methods as needed.
     """
 
     def get_data(self):
         """
         Get the data from last run.
         """
-        msg = self._client.producer.get_last(MessageEndpoints.processed_data(self._service_name))
+        msg = self._client.connector.get_last(MessageEndpoints.processed_data(self._service_name))
         if not msg:
             return None
         return self._convert_result(msg)
 
 
 class DAPPluginObjectAutoRun(DAPPluginObject):
     """
```

### Comparing `bec_lib-1.9.0/bec_lib/dap_plugins.py` & `bec_lib-2.0.1/bec_lib/dap_plugins.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This module provides the DAPPlugins class, which is used to access all available DAP plugins.
+"""
+
 from __future__ import annotations
 
 import bec_lib.dap_plugin_objects as dap_plugin_objects
 from bec_lib.endpoints import MessageEndpoints
 from bec_lib.logger import bec_logger
 from bec_lib.signature_serializer import dict_to_signature
 
@@ -34,15 +38,15 @@
         if not available_services:
             # not sure how we got here...
             return
         dap_services = [
             service for service in available_services if service.startswith("DAPServer/")
         ]
         for service in dap_services:
-            available_plugins = self._parent.producer.get(
+            available_plugins = self._parent.connector.get(
                 MessageEndpoints.dap_available_plugins(service)
             )
             if available_plugins is None:
                 logger.warning("No plugins available. Are redis and the BEC server running?")
                 return
             for plugin_name, plugin_info in available_plugins.content["resource"].items():
                 try:
```

### Comparing `bec_lib-1.9.0/bec_lib/device.py` & `bec_lib-2.0.1/bec_lib/device.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,33 @@
+"""
+This module provides the DeviceBase class as well as its derived classes Signal, ComputedSignal, Positioner, and Device.
+"""
+
+from __future__ import annotations
+
 import enum
 import functools
+import inspect
+import threading
 import time
 import uuid
 from collections import namedtuple
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 from typeguard import typechecked
 
 from bec_lib import messages
 from bec_lib.endpoints import MessageEndpoints
 from bec_lib.logger import bec_logger
-from bec_lib.redis_connector import RedisProducer
 
 logger = bec_logger.logger
 
+if TYPE_CHECKING:
+    from bec_lib.redis_connector import RedisConnector
+
 
 class RPCError(Exception):
     """Exception raised when an RPC call fails."""
 
 
 class ScanRequestError(Exception):
     """Exception raised when a scan request is rejected."""
@@ -57,50 +67,68 @@
     BASELINE = "baseline"
     MONITORED = "monitored"
     ASYNC = "async"
     CONTINUOUS = "continuous"
 
 
 class Status:
-    def __init__(self, producer: RedisProducer, RID: str) -> None:
+    """
+    Status object for RPC calls
+    """
+
+    def __init__(self, connector: RedisConnector, RID: str) -> None:
         """
         Status object for RPC calls
 
         Args:
-            producer (RedisProducer): Redis producer
+            connector (RedisConnector): Redis connector
             RID (str): Request ID
         """
-        self._producer = producer
+        self._connector = connector
         self._RID = RID
+        self._event = threading.Event()
+        self._thread_event = threading.Event()
+        self._device_req_thread = None
 
     def __eq__(self, __value: object) -> bool:
         if isinstance(__value, Status):
             return self._RID == __value._RID
         return False
 
-    def wait(self, timeout=None):
-        """wait until the request is completed"""
-        sleep_time_step = 0.1
-        sleep_count = 0
-
-        def _sleep(sleep_time):
-            nonlocal sleep_count
-            nonlocal timeout
-            time.sleep(sleep_time)
-            sleep_count += sleep_time
-            if timeout is not None and sleep_count > timeout:
-                raise TimeoutError()
-
-        while True:
-            request_status = self._producer.lrange(
-                MessageEndpoints.device_req_status(self._RID), 0, -1
+    def _wait_device_req(self):
+        while self._thread_event.is_set() is False:
+            request_status = self._connector.lrange(
+                MessageEndpoints.device_req_status_container(self._RID), 0, -1
             )
             if request_status:
+                self._event.set()
                 break
-            _sleep(sleep_time_step)
+            time.sleep(0.01)
+
+    def wait(self, timeout=None):
+        """
+        Wait for the request to complete. If the request is not completed within the specified time,
+        a TimeoutError is raised.
+
+        Args:
+            timeout (float, optional): Timeout in seconds. Defaults to None. If None, the method waits indefinitely.
+        """
+        try:
+            self._device_req_thread = threading.Thread(
+                target=self._wait_device_req, daemon=True, name=f"device_req_thread_{self._RID}"
+            )
+            self._device_req_thread.start()
+
+            if not self._event.wait(timeout):
+                raise TimeoutError("The request has not been completed within the specified time.")
+        finally:
+            self._thread_event.set()
+            self._device_req_thread.join()
+            self._event.clear()
+            self._thread_event.clear()
 
 
 class DeviceBase:
     """
     The DeviceBase class is the base class for all devices that are controlled via
     the DeviceManager. It provides a simple interface to perform RPC calls on the
     device. The DeviceBase class is not meant to be used directly, but rather to be subclassed.
@@ -142,14 +170,25 @@
     def _run(self, *args, fcn=None, cached=False, **kwargs):
         device, func_call = self._get_rpc_func_name(fcn=fcn)
 
         if cached:
             return fcn(self, *args, **kwargs)
         return self._run_rpc_call(device, func_call, *args, **kwargs)
 
+    def __getattribute__(self, name: str) -> Any:
+        if name in object.__getattribute__(self, "_property_container"):
+            caller_frame = inspect.currentframe().f_back
+            while caller_frame:
+                if "jedi" in caller_frame.f_globals:
+                    # Jedi module is present, likely tab completion
+                    return object.__getattribute__(self, name)
+                caller_frame = caller_frame.f_back
+            return object.__getattribute__(self, "_run")(fcn=name, cached=False)
+        return object.__getattribute__(self, name)
+
     def __getattr__(self, name: str) -> Any:
         if name in self._property_container:
             return object.__getattribute__(self, "_run")(fcn=name, cached=False)
         return object.__getattribute__(self, name)
 
     def __setattr__(self, name: str, value: Any) -> None:
         try:
@@ -247,15 +286,15 @@
             )
         if msg.content.get("out"):
             print(msg.content.get("out"))
         return_val = msg.content.get("return_val")
         if not isinstance(return_val, dict):
             return return_val
         if return_val.get("type") == "status" and return_val.get("RID"):
-            return Status(self.root.parent.producer, return_val.get("RID"))
+            return Status(self.root.parent.connector, return_val.get("RID"))
         return return_val
 
     def _get_rpc_response(self, request_id, rpc_id) -> Any:
         queue = self.root.parent.parent.queue
         while queue.request_storage.find_request_by_ID(request_id) is None:
             time.sleep(0.01)
         scan_queue_request = queue.request_storage.find_request_by_ID(request_id)
@@ -263,15 +302,15 @@
             time.sleep(0.01)
         if not all(scan_queue_request.accepted):
             raise ScanRequestError(
                 "Function call was rejected by the server:"
                 f" {scan_queue_request.response.content['message']}"
             )
         while True:
-            msg = self.root.parent.producer.get(MessageEndpoints.device_rpc(rpc_id))
+            msg = self.root.parent.connector.get(MessageEndpoints.device_rpc(rpc_id))
             if msg:
                 break
             time.sleep(0.01)
 
         return self._handle_rpc_response(msg)
 
     def _run_rpc_call(self, device, func_call, *args, wait_for_rpc_response=True, **kwargs) -> Any:
@@ -292,15 +331,15 @@
         try:
             # prepare RPC message
             rpc_id = str(uuid.uuid4())
             request_id = str(uuid.uuid4())
             msg = self._prepare_rpc_msg(rpc_id, request_id, device, func_call, *args, **kwargs)
 
             # send RPC message
-            self.root.parent.producer.send(MessageEndpoints.scan_queue_request(), msg)
+            self.root.parent.connector.send(MessageEndpoints.scan_queue_request(), msg)
 
             # wait for RPC response
             if not wait_for_rpc_response:
                 return None
             return_val = self._get_rpc_response(request_id, rpc_id)
         except KeyboardInterrupt as exc:
             self.root.stop(wait_for_rpc_response=False)
@@ -369,14 +408,15 @@
                 if descr["type"] == "func":
                     self._custom_rpc_methods[user_access_name] = DeviceBase(
                         name=user_access_name, info=descr, parent=self
                     )
                     setattr(self, user_access_name, self._custom_rpc_methods[user_access_name].run)
                     setattr(getattr(self, user_access_name), "__doc__", descr.get("doc"))
                 else:
+                    setattr(self, user_access_name, user_access_name)
                     self._property_container.add(user_access_name)
             else:
                 self._custom_rpc_methods[user_access_name] = DeviceBase(
                     name=user_access_name,
                     info={"device_info": {"custom_user_access": descr}},
                     parent=self,
                 )
@@ -452,15 +492,15 @@
         return self.parent.config_helper.send_config_request(
             action="update", config={self.name: {"readoutPriority": val}}
         )
 
     @property
     def on_failure(self) -> OnFailure:
         """get the failure behaviour for this device"""
-        return OnFailure(self._config["onFailure"])
+        return OnFailure(self._config.get("onFailure", "retry"))
 
     @on_failure.setter
     def on_failure(self, val: OnFailure):
         """set the failure behaviour for this device"""
         if not isinstance(val, OnFailure):
             val = OnFailure(val)
         self._config["onFailure"] = val
@@ -490,50 +530,14 @@
     def software_trigger(self, value: bool):
         """Whether or not the device can be software triggered"""
         self.parent.config_helper.send_config_request(
             action="update", config={self.name: {"softwareTrigger": value}}
         )
         self._config["softwareTrigger"] = value
 
-    # def read(self, cached, filter_readback=True):
-    #     """get the last reading from a device"""
-    #     val = self.parent.producer.get(MessageEndpoints.device_read(self.name))
-    #     if not val:
-    #         return None
-    #     if filter_readback:
-    #         return messages.DeviceMessage.loads(val).content["signals"].get(self.name)
-    #     return messages.DeviceMessage.loads(val).content["signals"]
-    #
-    # def readback(self, filter_readback=True):
-    #     """get the last readback value from a device"""
-    #     val = self.parent.producer.get(MessageEndpoints.device_readback(self.name))
-    #     if not val:
-    #         return None
-    #     if filter_readback:
-    #         return DeviceMessage.loads(val).content["signals"].get(self.name)
-    #     return DeviceMessage.loads(val).content["signals"]
-
-    # @property
-    # def device_status(self):
-    #     """get the current status of the device"""
-    #     val = self.parent.producer.get(MessageEndpoints.device_status(self.name))
-    #     if val is None:
-    #         return val
-    #     val = DeviceStatusMessage.loads(val)
-    #     return val.content.get("status")
-
-    # @property
-    # def signals(self):
-    #     """get the last signals from a device"""
-    #     val = self.parent.producer.get(MessageEndpoints.device_read(self.name))
-    #     if val is None:
-    #         return None
-    #     self._signals = DeviceMessage.loads(val).content["signals"]
-    #     return self._signals
-
     @property
     def user_parameter(self) -> dict:
         """get the user parameter for this device"""
         return self._config.get("userParameter")
 
     @typechecked
     def set_user_parameter(self, val: dict):
@@ -589,19 +593,19 @@
 
         if not cached:
             signals = self._run(cached=cached, fcn=self.read)
         else:
             if is_config_signal:
                 return self.read_configuration(cached=cached)
             if use_readback:
-                val = self.root.parent.producer.get(
+                val = self.root.parent.connector.get(
                     MessageEndpoints.device_readback(self.root.name)
                 )
             else:
-                val = self.root.parent.producer.get(MessageEndpoints.device_read(self.root.name))
+                val = self.root.parent.connector.get(MessageEndpoints.device_read(self.root.name))
 
             if not val:
                 return None
             signals = val.content["signals"]
         if filter_to_hints:
             signals = {key: val for key, val in signals.items() if key in self._hints}
         return self._filter_rpc_signals(signals)
@@ -619,15 +623,15 @@
         if not cached:
             fcn = self.read_configuration if (not is_signal or is_config_signal) else self.read
             signals = self._run(cached=False, fcn=fcn)
         else:
             if is_signal and not is_config_signal:
                 return self.read(cached=True)
 
-            val = self.root.parent.producer.get(
+            val = self.root.parent.connector.get(
                 MessageEndpoints.device_read_configuration(self.root.name)
             )
             if not val:
                 return None
             signals = val.content["signals"]
 
         return self._filter_rpc_signals(signals)
@@ -645,24 +649,24 @@
             kind = self._signal_info.get("kind_str")
             if kind in ("2", "Kind.config"):
                 is_config_signal = True
             elif kind in ("0", "Kind.omitted"):
                 cached = False
         return is_signal, is_config_signal, cached
 
-    @rpc
     def describe(self):
         """
         Describes the device and yields information about the device's signals, including
         the signal's name, source, shape, data type, precision etc.
         """
+        return self._info.get("describe", {})
 
-    @rpc
     def describe_configuration(self):
         """Describes the device configuration."""
+        return self._info.get("describe_configuration", {})
 
     def get(self, cached=True):
         """
         Gets the device value.
         """
 
         is_signal = self._signal_info is not None
@@ -674,19 +678,32 @@
             return res
 
         ret = self.read()
         if ret is None:
             return None
         return ret.get(self._signal_info.get("obj_name"), {}).get("value")
 
-    @rpc
-    def put(self, value: Any):
+    def put(self, value: Any, wait=False):
         """
-        Puts the device value.
+        Puts the device value. In contrast to the set method, the put method does not
+        return a status object and does not wait for the device to settle. However,
+        the put method can be converted into a blocking call by setting the wait argument to True,
+        which will be equivalent to the set method + wait.
+
+        Use the put method if you want to update a value without waiting for the device to settle.
+        Use the set method if you want to update a value and wait for the device to settle.
+
+        Args:
+            value (Any): The value to put.
+            wait (bool, optional): If True, the method waits for the device to settle. Defaults to False.
         """
+        if wait:
+            return self.set(value).wait()
+        self._run(value, fcn=self.put)
+        return
 
 
 class Device(OphydInterfaceBase):
     """
     Device (bluesky interface):
     * trigger
     * read
@@ -751,26 +768,30 @@
                 f" {self._config.get('userParameter')}\n{separator}\nConfig:\n{config}"
             )
         return f"{type(self).__name__}(name={self.name}, enabled={self.enabled})"
 
 
 class AdjustableMixin:
     @rpc
-    def set(self, val):
+    def set(self, val: Any) -> Status:
         """
-        Sets the device value.
+        Sets the device value. This method returns a status object that can be used to wait for the device to settle.
+        In contrast to the put method, the set method can be made into a blocking call by calling the wait method on the
+        returned status object.
+
+        Args:
+            val (Any): The value to set.
         """
-        pass
 
     @property
     def limits(self):
         """
         Returns the device limits.
         """
-        limit_msg = self.root.parent.producer.get(MessageEndpoints.device_limits(self.root.name))
+        limit_msg = self.root.parent.connector.get(MessageEndpoints.device_limits(self.root.name))
         if not limit_msg:
             return [0, 0]
         limits = [
             limit_msg.content["signals"].get("low", 0),
             limit_msg.content["signals"].get("high", 0),
         ]
         return limits
@@ -804,14 +825,55 @@
         self.update_config({"deviceConfig": {"limits": limits}})
 
 
 class Signal(AdjustableMixin, OphydInterfaceBase):
     pass
 
 
+class ComputedSignal(Signal):
+
+    def set_compute_method(self, method: callable) -> None:
+        """Set the compute method for the ComputedSignal.
+
+        We allow users to use two additional packages which are imported to simplify computations:
+        - numpy as np
+        - scipy as sp
+
+        Args:
+            method (callable) : Method to execute as computation method, i.e.
+            def calculate_readback(signal):
+            ...:     return -1 * signal.get()
+
+        >>> dev.<dev_name>.set_compute_method(calculate_readback)
+
+        """
+        if not callable(method):
+            raise ValueError("The compute method must be callable.")
+
+        method = inspect.getsource(method)
+        self.update_config({"deviceConfig": {"compute_method": method}})
+
+    def set_input_signals(self, *signals) -> None:
+        """Set input signals for compute method.
+        The signals need to be valid signals and match the computation of the compute method.
+
+        Args:
+            signals : All signals to be added for the comput method
+
+        >>> dev.<dev_name>.set_input_signals(dev.bpm4i.readback, dev.bpm5i.readback)
+        """
+        if not signals:
+            self.update_config({"deviceConfig": {"input_signals": []}})
+            return
+        if not all(isinstance(signal, Signal) for signal in signals):
+            raise ValueError("All input signals must be of type Signal.")
+        signals = [signal.full_name for signal in signals]
+        self.update_config({"deviceConfig": {"input_signals": signals}})
+
+
 class Positioner(AdjustableMixin, Device):
     """
     Positioner:
     * trigger
     * read
     * set
     * stop
```

### Comparing `bec_lib-1.9.0/bec_lib/devicemanager.py` & `bec_lib-2.0.1/bec_lib/devicemanager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
+"""
+This module contains the DeviceManager class which is used to manage devices and their configuration.
+"""
+
 from __future__ import annotations
 
 import re
-import time
 import traceback
 from typing import TYPE_CHECKING
 
 from rich.console import Console
 from rich.table import Table
 from typeguard import typechecked
 
 from bec_lib import messages
 from bec_lib.bec_errors import DeviceConfigError
 from bec_lib.config_helper import ConfigHelper
-from bec_lib.device import Device, DeviceBase, Positioner, ReadoutPriority, Signal
+from bec_lib.device import ComputedSignal, Device, DeviceBase, Positioner, ReadoutPriority, Signal
 from bec_lib.endpoints import MessageEndpoints
 from bec_lib.logger import bec_logger
 from bec_lib.messages import BECStatus, DeviceConfigMessage, DeviceInfoMessage
 
 if TYPE_CHECKING:
     from bec_lib import BECService
-    from bec_lib.connector import ConnectorBase
-    from bec_lib.redis_connector import RedisProducer
 
 logger = bec_logger.logger
 
 
 class DeviceContainer(dict):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -111,15 +112,15 @@
         devices.extend(
             [self.get(dev) for dev in readout_priority_mod.get(readout_priority.name.lower(), [])]
         )
 
         excluded_readout_priority = [
             str(x.name).lower() for x in ReadoutPriority if x != readout_priority
         ]
-        excluded_devices = []
+        excluded_devices = self.disabled_devices
         for priority in excluded_readout_priority:
             excluded_devices.extend(self.get(dev) for dev in readout_priority_mod.get(priority, []))
 
         return [dev for dev in set(devices) if dev not in excluded_devices]
 
     def async_devices(self, readout_priority: dict | None = None) -> list:
         """get a list of all synchronous devices"""
@@ -272,17 +273,16 @@
         table.add_column("setpoint", justify="center")
         table.add_column("limits", justify="center")
         dev_read = {dev.name: dev.read(cached=True) for dev in device_names}
         readbacks = {}
         setpoints = {}
         limits = {}
         for dev in device_names:
-            # pylint: disable=protected-access
-            if "limits" in dev._config.get("deviceConfig", {}):
-                limits[dev.name] = str(dev._config["deviceConfig"]["limits"])
+            if hasattr(dev, "limits"):
+                limits[dev.name] = str(dev.limits)
             else:
                 limits[dev.name] = "[]"
 
         for dev, read in dev_read.items():
             if dev in read:
                 val = read[dev]["value"]
                 if not isinstance(val, str):
@@ -366,38 +366,45 @@
     devices = DeviceContainer()
     _config = {}  # valid config
     _session = {}
     _request = None  # requested config
     _request_config_parsed = None  # parsed config request
     _response = None  # response message
 
-    _connector_base_consumer = {}
-    producer = None
+    _connector_base_register = {}
     config_helper = None
     _device_cls = DeviceBase
     _status_cb = []
 
     def __init__(self, service: BECService, status_cb: list = None) -> None:
         self._service = service
         self.parent = service  # for backwards compatibility; will be removed in the future
         self.connector = self._service.connector
-        self.config_helper = ConfigHelper(self.connector)
+        self.config_helper = ConfigHelper(self.connector, self._service._service_name)
         self._status_cb = status_cb if isinstance(status_cb, list) else [status_cb]
 
+    @property
+    def producer(self):
+        # will show the deprecation warning
+        return self.connector.producer()
+
     def initialize(self, bootstrap_server) -> None:
         """
         Initialize the DeviceManager by starting all connectors.
         Args:
             bootstrap_server: Redis server address, e.g. 'localhost:6379'
 
         Returns:
 
         """
         self._start_connectors(bootstrap_server)
-        self._get_config()
+        try:
+            self._get_config()
+        except DeviceConfigError as dev_conf_error:
+            logger.error(f"Failed to initialize DeviceManager. {dev_conf_error}")
 
     def update_status(self, status: BECStatus):
         """Update the status of the device manager
         Args:
             status (BECStatus): New status
         """
         for cb in self._status_cb:
@@ -440,15 +447,14 @@
                     self.devices[dev]._config["readoutPriority"] = config[dev]["readoutPriority"]
                 if "softwareTrigger" in config[dev]:
                     self.devices[dev]._config["softwareTrigger"] = config[dev]["softwareTrigger"]
 
         elif action == "add":
             self._add_action(config)
         elif action == "reload":
-            logger.info("Reloading config.")
             self._reload_action()
         elif action == "remove":
             self._remove_action(config)
         self.update_status(BECStatus.RUNNING)
         self._acknowledge_config_request(msg)
 
     def _acknowledge_config_request(self, msg: DeviceConfigMessage) -> None:
@@ -458,55 +464,51 @@
             msg (DeviceConfigMessage): Config message
 
         Returns:
 
         """
         if not msg.metadata.get("RID"):
             return
-        self.producer.lpush(
+        self.connector.lpush(
             MessageEndpoints.service_response(msg.metadata["RID"]),
             messages.ServiceResponseMessage(
                 # pylint: disable=no-member
-                response={"accepted": True, "service": self._service.__class__.__name__}
+                response={"accepted": True, "service": self._service._service_name}
             ),
             expire=100,
         )
 
     def _add_action(self, config) -> None:
         for dev in config:
             self._add_device(dev, config)
 
     def _reload_action(self) -> None:
+        logger.info("Reloading config.")
         self.devices.flush()
         self._get_config()
 
     def _remove_action(self, config) -> None:
         for dev in config:
             self._remove_device(dev)
 
     def _start_connectors(self, bootstrap_server) -> None:
-        self._start_base_consumer()
-        self.producer = self.connector.producer()
-        self._start_custom_connectors(bootstrap_server)
+        self._start_base_register()
 
-    def _start_base_consumer(self) -> None:
+    def _start_base_register(self) -> None:
         """
         Start consuming messages for all base topics. This method will be called upon startup.
         Returns:
 
         """
-        self._connector_base_consumer["device_config_update"] = self.connector.consumer(
+        self.connector.register(
             MessageEndpoints.device_config_update(),
             cb=self._device_config_update_callback,
             parent=self,
         )
 
-        # self._connector_base_consumer["log"].start()
-        self._connector_base_consumer["device_config_update"].start()
-
     @staticmethod
     def _log_callback(msg, *, parent, **kwargs) -> None:
         """
         Consumer callback for handling log messages.
         Args:
             cls: Reference to the DeviceManager instance
             msg: log message of type LogMessage
@@ -534,56 +536,19 @@
     def _get_config(self):
         self._session["devices"] = self._get_redis_device_config()
         if not self._session["devices"]:
             logger.warning("No config available.")
         self._load_session()
 
     def _get_redis_device_config(self) -> list:
-        devices = self.producer.get(MessageEndpoints.device_config())
+        devices = self.connector.get(MessageEndpoints.device_config())
         if not devices:
             return []
         return devices.content["resource"]
 
-    def _stop_base_consumer(self):
-        """
-        Stop all base consumers by setting the corresponding event
-        Returns:
-
-        """
-        if self.connector is not None:
-            for _, con in self._connector_base_consumer.items():
-                con.signal_event.set()
-                con.join()
-
-    def _stop_consumer(self):
-        """
-        Stop all consumers
-        Returns:
-
-        """
-        self._stop_base_consumer()
-        self._stop_custom_consumer()
-
-    def _start_custom_connectors(self, bootstrap_server) -> None:
-        """
-        Override this method in a derived class to start custom connectors upon initialization.
-        Args:
-            bootstrap_server: Kafka bootstrap server
-
-        Returns:
-
-        """
-
-    def _stop_custom_consumer(self) -> None:
-        """
-        Stop all custom consumers. Override this method in a derived class.
-        Returns:
-
-        """
-
     def _add_device(self, dev: dict, msg: messages.DeviceInfoMessage):
         name = msg.content["device"]
         info = msg.content["info"]
 
         base_class = info["device_info"]["device_base_class"]
 
         if base_class == "device":
@@ -591,40 +556,41 @@
             obj = Device(name=name, info=info, parent=self)
         elif base_class == "positioner":
             logger.info(f"Adding new positioner {name}")
             obj = Positioner(name=name, info=info, parent=self)
         elif base_class == "signal":
             logger.info(f"Adding new signal {name}")
             obj = Signal(name=name, info=info, parent=self)
+        elif base_class == "computed_signal":
+            logger.info(f"Adding new computed signal {name}")
+            obj = ComputedSignal(name=name, info=info, parent=self)
         else:
             logger.error(f"Trying to add new device {name} of type {base_class}")
 
         # pylint: disable=protected-access
         obj._config = dev
         self.devices._add_device(name, obj)
 
     def _remove_device(self, dev_name):
         if dev_name in self.devices:
             self.devices.pop(dev_name)
 
-    def _load_session(self, idle_time=1, _device_cls=None):
-        time.sleep(idle_time)
+    def _load_session(self, _device_cls=None):
         if self._is_config_valid():
             for dev in self._session["devices"]:
                 # pylint: disable=broad-except
                 try:
                     msg = self._get_device_info(dev.get("name"))
                     self._add_device(dev, msg)
                 except Exception:
                     content = traceback.format_exc()
                     logger.error(f"Failed to load device {dev}: {content}")
 
     def _get_device_info(self, device_name) -> DeviceInfoMessage:
-        msg = self.producer.get(MessageEndpoints.device_info(device_name))
-        return msg
+        return self.connector.get(MessageEndpoints.device_info(device_name))
 
     def check_request_validity(self, msg: DeviceConfigMessage) -> None:
         """
         Check if the config request is valid.
 
         Args:
             msg (DeviceConfigMessage): Config message
@@ -657,14 +623,11 @@
             return False
         return True
 
     def shutdown(self):
         """
         Shutdown all connectors.
         """
-        try:
-            self.connector.shutdown()
-        except RuntimeError as runtime_error:
-            logger.error(f"Failed to shutdown connector. {runtime_error}")
+        self.connector.shutdown()
 
     def __del__(self):
         self.shutdown()
```

### Comparing `bec_lib-1.9.0/bec_lib/lmfit_serializer.py` & `bec_lib-2.0.1/bec_lib/lmfit_serializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This module contains functions for serializing and deserializing lmfit objects.
+"""
+
 from lmfit import Parameter, Parameters
 
 
 def serialize_param_object(param: Parameter) -> dict:
     """
     Serialize lmfit.Parameter object to JSON-serializable dictionary.
```

### Comparing `bec_lib-1.9.0/bec_lib/logbook_connector.py` & `bec_lib-2.0.1/bec_lib/logbook_connector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+"""
+This module provides a connector to the electronic logbook SciLog.
+"""
+
 from __future__ import annotations
 
 import sys
 import warnings
 from typing import TYPE_CHECKING
 
-import msgpack
 from requests.exceptions import HTTPError
 
 from bec_lib.endpoints import MessageEndpoints
 from bec_lib.logger import bec_logger
 
 logger = bec_logger.logger
 
@@ -20,45 +23,46 @@
 if TYPE_CHECKING:
     from bec_lib.redis_connector import RedisConnector
 
 
 class LogbookConnector:
     def __init__(self, connector: RedisConnector) -> None:
         self.connector = connector
-        self.producer = connector.producer()
         self.connected = False
         self._scilog_module = None
         self._connect()
         self.logbook = None
 
     def _connect(self):
         if "scilog" not in sys.modules:
             return
 
-        msg = self.producer.get(MessageEndpoints.logbook())
+        msg = self.connector.get(MessageEndpoints.logbook())
         if not msg:
             return
-        msg = msgpack.loads(msg)
+        scilog_creds = msg.credentials
 
-        account = self.producer.get(MessageEndpoints.account())
-        if not account:
+        account_msg = self.connector.get(MessageEndpoints.account())
+        if not account_msg:
             return
-        account = account.decode()
+        account = account_msg.value
         account = account.replace("e", "p")
 
         self._scilog_module = scilog
 
-        self.log = self._scilog_module.SciLog(msg["url"], options={"token": msg["token"]})
+        self.log = self._scilog_module.SciLog(
+            scilog_creds["url"], options={"token": scilog_creds["token"]}
+        )
         # FIXME the python sdk should not use the ownergroup
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             try:
                 logbooks = self.log.get_logbooks(readACL={"inq": [account]})
             except HTTPError:
-                self.producer.set(MessageEndpoints.logbook(), b"")
+                self.connector.set(MessageEndpoints.logbook(), b"")
                 return
         if len(logbooks) > 1:
             logger.warning("Found two logbooks. Taking the first one.")
         self.log.select_logbook(logbooks[0])
 
         # set aliases
         # pylint: disable=no-member, invalid-name
```

### Comparing `bec_lib-1.9.0/bec_lib/messages.py` & `bec_lib-2.0.1/bec_lib/messages.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,55 @@
-from __future__ import annotations
-
-import dataclasses
 import enum
 import time
 import warnings
 from copy import deepcopy
-from dataclasses import MISSING, dataclass, field, fields
-from typing import Any, Literal
+from typing import Any, ClassVar, Literal
 
 import numpy as np
+from pydantic import BaseModel, Field, field_validator, model_validator
 
 
 class BECStatus(enum.Enum):
     """BEC status enum"""
 
     RUNNING = 2
     BUSY = 1
     IDLE = 0
     ERROR = -1
 
 
-@dataclass
-class BECMessage:
-
-    def __post_init__(self):
-        # in case "metadata" is passed None as keyword arg, for example
-        for f in fields(self):
-            value = getattr(self, f.name)
-            if value is None and not f.default_factory is MISSING:
-                setattr(self, f.name, f.default_factory())
+class BECMessage(BaseModel):
+    msg_type: ClassVar[str]
+    metadata: dict | None = Field(default_factory=dict)
+
+    @field_validator("metadata")
+    @classmethod
+    def check_metadata(cls, v):
+        if v is None:
+            return {}
+        return v
 
     @property
     def content(self):
         content = self.__dict__.copy()  # dataclasses.asdict(self)
         content.pop("metadata", None)
         return content
 
-    def _is_valid(self) -> bool:
-        return True
-
     def __eq__(self, other):
         if not isinstance(other, BECMessage):
             # don't attempt to compare against unrelated types
             return False
 
         try:
-            np.testing.assert_equal(self.__dict__, other.__dict__)
+            np.testing.assert_equal(self.model_dump(), other.model_dump())
         except AssertionError:
             return False
 
-        # remove the pylint disable when we upgrade to python 3.10. dataclasses will support kw_only
-        # pylint: disable=no-member
         return self.msg_type == other.msg_type and self.metadata == other.metadata
 
-    def __str__(self):
-        return f"messages.{self.__class__.__name__}(**{self.content}, metadata={self.metadata})"
-
     def loads(self):
         warnings.warn(
             "BECMessage.loads() is deprecated and should not be used anymore. When calling Connector methods, it can be omitted. When a message needs to be deserialized call the appropriate function from bec_lib.serialization",
             FutureWarning,
         )
         return self
 
@@ -67,617 +57,565 @@
         warnings.warn(
             "BECMessage.dumps() is deprecated and should not be used anymore. When calling Connector methods, it can be omitted. When a message needs to be serialized call the appropriate function from bec_lib.serialization",
             FutureWarning,
         )
         return self
 
 
-@dataclass
 class BundleMessage(BECMessage):
     """Bundle of BECMessages"""
 
-    msg_type = "bundle_message"
-    messages: list = field(default_factory=list)
-    metadata: dict = field(default_factory=dict)
+    msg_type: ClassVar[str] = "bundle_message"
+    messages: list = Field(default_factory=list[BECMessage])
 
     def append(self, msg: BECMessage):
         """append a new BECMessage to the bundle"""
         if not isinstance(msg, BECMessage):
             raise AttributeError(f"Cannot append message of type {msg.__class__.__name__}")
-        else:
-            self.messages.append(msg)
+        self.messages.append(msg)
 
     def __len__(self):
         return len(self.messages)
 
     def __iter__(self):
         yield from self.messages
 
 
-@dataclass(eq=False)
 class ScanQueueMessage(BECMessage):
     """Message type for sending scan requests to the scan queue
     Sent by the API server / user to the scan_queue topic. It will be consumed by the scan server.
         Args:
             scan_type (str): one of the registered scan types; either rpc calls or scan types defined in the scan server
             parameter (dict): required parameters for the given scan_stype
             queue (str): either "primary" or "interception"
             metadata (dict, optional): additional metadata to describe the scan
         Examples:
             >>> ScanQueueMessage(scan_type="dscan", parameter={"motor1": "samx", "from_m1:": -5, "to_m1": 5, "steps_m1": 10, "motor2": "samy", "from_m2": -5, "to_m2": 5, "steps_m2": 10, "exp_time": 0.1})
     """
 
-    msg_type = "scan_queue_message"
+    msg_type: ClassVar[str] = "scan_queue_message"
     scan_type: str
     parameter: dict
-    queue: str = field(default="primary")
-    metadata: dict = field(default_factory=dict)
+    queue: str = Field(default="primary")
 
 
-@dataclass(eq=False)
 class ScanQueueHistoryMessage(BECMessage):
     """Sent after removal from the active queue. Contains information about the scan.
     Sent by the API server / user to the scan_queue topic. It will be consumed by the scan server.
     Args:
         status(str):  current scan status
-        queueID(str): unique queue ID
+        queue_id(str): unique queue ID
         info(dict): dictionary containing additional information about the scan
         queue (str): either "primary" or "interception"
         metadata (dict, optional): additional metadata to describe the scan
     """
 
-    msg_type = "queue_history"
+    msg_type: ClassVar[str] = "queue_history"
     status: str
-    queueID: str
+    queue_id: str
     info: dict
-    queue: str = field(default="primary")
-    metadata: dict = field(default_factory=dict)
+    queue: str = Field(default="primary")
 
 
-@dataclass(eq=False)
 class ScanStatusMessage(BECMessage):
     """Message type for sending scan status updates
     Args:
-        scanID(str): unique scan ID
-        status(dict): dictionary containing the current scan status
+        scan_id(str): unique scan ID
+        status(str): scan status ("open", "paused", "aborted", "halted", "closed")
         info(dict): dictionary containing additional information about the scan
         timestamp(float, optional): timestamp of the scan status update. If None, the current time is used.
         metadata(dict, optional): additional metadata to describe and identify the scan.
 
     Examples:
-        >>> ScanStatusMessage(scanID="1234", status={"scan_number": 1, "scan_motors": ["samx", "samy"], "scan_type": "dscan", "scan_status": "RUNNING"}, info={"positions": {"samx": 0.5, "samy": 0.5}})
+        >>> ScanStatusMessage(scan_id="1234", status="open", info={"positions": {"samx": 0.5, "samy": 0.5}})
     """
 
-    msg_type = "scan_status"
-    scanID: str
-    status: dict
+    msg_type: ClassVar[str] = "scan_status"
+    scan_id: str | None
+    status: Literal["open", "paused", "aborted", "halted", "closed"]
     info: dict
-    timestamp: float = field(default_factory=time.time)
-    metadata: dict = field(default_factory=dict)
+    timestamp: float = Field(default_factory=time.time)
 
     def __str__(self):
         content = deepcopy(self.__dict__)
         if content["info"].get("positions"):
             content["info"]["positions"] = "..."
         return f"{self.__class__.__name__}({content, self.metadata}))"
 
 
-@dataclass(eq=False)
 class ScanQueueModificationMessage(BECMessage):
     """Message type for sending scan queue modifications
     Args:
-        scanID(str): unique scan ID
+        scan_id(str): unique scan ID
         action(str): one of the actions defined in ACTIONS
                      ("pause", "deferred_pause", "continue", "abort", "clear", "restart", "halt")
         parameter(dict): additional parameters for the action
         metadata(dict, optional): additional metadata to describe and identify the scan.
     """
 
-    ACTIONS = ["pause", "deferred_pause", "continue", "abort", "clear", "restart", "halt"]
-    msg_type = "scan_queue_modification"
-    scanID: str
+    ACTIONS: ClassVar[list] = [
+        "pause",
+        "deferred_pause",
+        "continue",
+        "abort",
+        "clear",
+        "restart",
+        "halt",
+        "resume",
+    ]
+    msg_type: ClassVar[str] = "scan_queue_modification"
+    scan_id: str | list[str] | None
     action: str
     parameter: dict
-    metadata: dict = field(default_factory=dict)
 
-    def _is_valid(self) -> bool:
-        return self.action in self.ACTIONS
+    @field_validator("action")
+    @classmethod
+    def check_action(cls, v):
+        """Validate the action"""
+        if v not in cls.ACTIONS:
+            raise ValueError(f"Invalid action {v}. Must be one of {cls.ACTIONS}")
+        return v
 
 
-@dataclass(eq=False)
 class ScanQueueStatusMessage(BECMessage):
     """Message type for sending scan queue status updates
     Args:
         queue(dict): dictionary containing the current queue status
         metadata(dict, optional): additional metadata to describe and identify the scan.
     """
 
-    msg_type = "scan_queue_status"
+    msg_type: ClassVar[str] = "scan_queue_status"
     queue: dict
-    metadata: dict = field(default_factory=dict)
 
-    def _is_valid(self) -> bool:
-        if (
-            not isinstance(self.queue, dict)
-            or "primary" not in self.queue
-            or not isinstance(self.queue["primary"], dict)
-        ):
-            return False
-        return True
+    @field_validator("queue")
+    @classmethod
+    def check_queue(cls, v):
+        """Validate the queue"""
+        if not isinstance(v, dict):
+            raise ValueError(f"Invalid queue {v}. Must be a dictionary")
+        if "primary" not in v:
+            raise ValueError(f"Invalid queue {v}. Must contain a 'primary' key")
+        return v
 
 
-@dataclass(eq=False)
 class RequestResponseMessage(BECMessage):
     """Message type for sending back decisions on the acceptance of requests
     Args:
         accepted (bool): True if the request was accepted
         message (str): String describing the decision, e.g. "Invalid request"
         metadata (dict, optional): additional metadata to describe and identify the request / response
     """
 
-    msg_type = "request_response"
+    msg_type: ClassVar[str] = "request_response"
     accepted: bool
-    message: str
-    metadata: dict = field(default_factory=dict)
+    message: str | dict | None = Field(default=None)
 
 
-@dataclass(eq=False)
 class DeviceInstructionMessage(BECMessage):
     """Message type for sending device instructions to the device server
     Args:
         device (str): device name
         action (str): device action, e.g. method call
         parameter (dict): device action parameter
         metadata (dict, optional): metadata to describe the conditions of the device instruction
     """
 
-    msg_type = "device_instruction"
-    device: str
+    msg_type: ClassVar[str] = "device_instruction"
+    device: str | list[str] | None
     action: str
     parameter: dict
-    metadata: dict = field(default_factory=dict)
 
 
-@dataclass(eq=False)
 class DeviceMessage(BECMessage):
     """Message type for sending device readings from the device server
     Args:
         signals (dict): dictionary of device signals
         metadata (dict, optional): metadata to describe the conditions of the device reading
     Examples:
-        >>> BECMessage.DeviceMessage(signals={'samx': {'value': 14.999033949016491, 'timestamp': 1686385306.0265112}, 'samx_setpoint': {'value': 15.0, 'timestamp': 1686385306.016806}, 'samx_motor_is_moving': {'value': 0, 'timestamp': 1686385306.026888}}}, metadata={'stream': 'primary', 'DIID': 353, 'RID': 'd3471acc-309d-43b7-8ff8-f986c3fdecf1', 'pointID': 49, 'scanID': '8e234698-358e-402d-a272-73e168a72f66', 'queueID': '7a232746-6c90-44f5-81f5-74ab0ea22d4a'})
+        >>> BECMessage.DeviceMessage(signals={'samx': {'value': 14.999033949016491, 'timestamp': 1686385306.0265112}, 'samx_setpoint': {'value': 15.0, 'timestamp': 1686385306.016806}, 'samx_motor_is_moving': {'value': 0, 'timestamp': 1686385306.026888}}}, metadata={'stream': 'primary', 'DIID': 353, 'RID': 'd3471acc-309d-43b7-8ff8-f986c3fdecf1', 'point_id': 49, 'scan_id': '8e234698-358e-402d-a272-73e168a72f66', 'queue_id': '7a232746-6c90-44f5-81f5-74ab0ea22d4a'})
     """
 
-    msg_type = "device_message"
-    signals: dict
-    metadata: dict = field(default_factory=dict)
+    msg_type: ClassVar[str] = "device_message"
+    signals: dict = Field(default_factory=dict)
 
-    def _is_valid(self) -> bool:
-        return isinstance(self.signals, dict)
 
-
-@dataclass(eq=False)
 class DeviceRPCMessage(BECMessage):
     """Message type for sending device RPC return values from the device server
     Args:
         device (str): device name
         return_val (Any): return value of the RPC call
         out (str): output of the RPC call
         success (bool, optional): True if the RPC call was successful
         metadata (dict, optional): metadata to describe the conditions of the device RPC call
     """
 
-    msg_type = "device_rpc_message"
+    msg_type: ClassVar[str] = "device_rpc_message"
     device: str
     return_val: Any
-    out: str
-    success: bool = field(default=True)
-    metadata: dict = field(default_factory=dict)
-
-    def _is_valid(self) -> bool:
-        return isinstance(self.device, str)
+    out: str | dict
+    success: bool = Field(default=True)
 
 
-@dataclass(eq=False)
 class DeviceStatusMessage(BECMessage):
     """Message type for sending device status updates from the device server
     Args:
         device (str): device name
         status (int): device status
         metadata (dict, optional): additional metadata to describe the conditions of the device status
     """
 
-    msg_type = "device_status_message"
+    msg_type: ClassVar[str] = "device_status_message"
     device: str
     status: int
-    metadata: dict = field(default_factory=dict)
 
 
-@dataclass(eq=False)
 class DeviceReqStatusMessage(BECMessage):
     """Message type for sending device request status updates from the device server
     Args:
         device (str): device name
         success (bool): True if the request was successful
         metadata (dict, optional): additional metadata to describe the conditions of the device request status
     """
 
-    msg_type = "device_req_status_message"
+    msg_type: ClassVar[str] = "device_req_status_message"
     device: str
     success: bool
-    metadata: dict = field(default_factory=dict)
 
 
-@dataclass(eq=False)
 class DeviceInfoMessage(BECMessage):
     """Message type for sending device info updates from the device server
     Args:
         device (str): device name
         info (dict): device info as dictionary
         metadata (dict, optional): additional metadata to describe the conditions of the device info
     """
 
-    msg_type = "device_info_message"
+    msg_type: ClassVar[str] = "device_info_message"
     device: str
     info: dict
-    metadata: dict = field(default_factory=dict)
 
 
-@dataclass(eq=False)
 class DeviceMonitorMessage(BECMessage):
     """Message type for sending device monitor updates from the device server
     Args:
         device (str): device name
         data (list): dictionary with device monitor data, #TODO should this be a list or better dictionary?
         metadata (dict, optional): additional metadata to describe the conditions of the device monitor
     """
 
-    msg_type = "device_monitor_message"
+    msg_type: ClassVar[str] = "device_monitor_message"
     device: str
     data: np.ndarray
-    metadata: dict = field(default_factory=dict)
+
+    class Config:
+        arbitrary_types_allowed = True
 
 
-@dataclass(eq=False)
 class ScanMessage(BECMessage):
     """Message type for sending scan segment data from the scan bundler
     Args:
         point_id (int): point ID from scan segment
-        scanID (int): scan ID
+        scan_id (str): scan ID
         data (dict): scan segment data
         metadata (dict, optional): additional metadata to describe the conditions of the scan segment
     """
 
-    msg_type = "scan_message"
+    msg_type: ClassVar[str] = "scan_message"
     point_id: int
-    scanID: int
+    scan_id: str
     data: dict
-    metadata: dict = field(default_factory=dict)
 
 
-@dataclass(eq=False)
 class ScanBaselineMessage(BECMessage):
     """Message type for sending scan baseline data from the scan bundler
     Args:
-        scanID (int): scan ID
+        scan_id (str): scan ID
         data (dict): scan baseline data
         metadata (dict, optional): additional metadata to describe the conditions of the scan baseline
     """
 
-    msg_type = "scan_baseline_message"
-    scanID: int
+    msg_type: ClassVar[str] = "scan_baseline_message"
+    scan_id: str
     data: dict
-    metadata: dict = field(default_factory=dict)
 
 
-@dataclass(eq=False)
 class DeviceConfigMessage(BECMessage):
     """Message type for sending device config updates
     Args:
         action (str): set, update or reload
         config (dict): device config (add, set, update) or None (reload)
         metadata (dict, optional): additional metadata to describe the conditions of the device config
     """
 
-    ACTIONS = ["add", "set", "update", "reload"]
-    msg_type = "device_config_message"
-    action: str
-    config: dict
-    metadata: dict = field(default_factory=dict)
-
-    def _is_valid(self) -> bool:
-        return self.action in self.ACTIONS
+    msg_type: ClassVar[str] = "device_config_message"
+    action: Literal["add", "set", "update", "reload", "remove"] = Field(
+        default=None, validate_default=True
+    )
+    config: dict | None = Field(default=None)
+
+    @model_validator(mode="after")
+    @classmethod
+    def check_config(cls, values):
+        """Validate the config"""
+        if values.action in ["add", "set", "update"] and not values.config:
+            raise ValueError(f"Invalid config {values.config}. Must be a dictionary")
+        return values
 
 
-@dataclass(eq=False)
 class LogMessage(BECMessage):
     """Log message
     Args:
         log_type (str): log, warning or error
         log_msg (dict or str): log message
         metadata (dict, optional):
     """
 
-    msg_type = "log_message"
+    msg_type: ClassVar[str] = "log_message"
     log_type: str
     log_msg: dict | str
-    metadata: dict = field(default_factory=dict)
 
 
-@dataclass(eq=False)
 class AlarmMessage(BECMessage):
     """Alarm message
     Severity 1: Minor alarm, no user interaction needed. The system can continue.
     Severity 2: Major alarm, user interaction needed. If the alarm was raised during the execution of a request, the request will be paused until the alarm is resolved.
     Severity 3: Major alarm, user interaction needed. The system cannot recover by itself.
 
     Args:
         severity (int): severity level (1-3)
         source (str): source of the problem (where did it occur?)
         msg (str): problem description (what happened?)
         metadata (dict, optional): Additional metadata.
     """
 
-    msg_type = "alarm_message"
+    msg_type: ClassVar[str] = "alarm_message"
     severity: int
     alarm_type: str
-    source: str
+    source: dict
     msg: str
-    metadata: dict = field(default_factory=dict)
 
 
-@dataclass(eq=False)
 class StatusMessage(BECMessage):
     """Status message
     Args:
         name (str): name of the status
         status (BECStatus): value of the BECStatus enum
         (RUNNING = 2
         BUSY = 1
         IDLE = 0
         ERROR = -1))
         info (dict): status info
         metadata (dict, optional): additional metadata
     """
 
-    msg_type = "status_message"
+    msg_type: ClassVar[str] = "status_message"
     name: str
     status: BECStatus
     info: dict
-    metadata: dict = field(default_factory=dict)
 
 
-@dataclass(eq=False)
 class FileMessage(BECMessage):
     """File message to inform about the status of a file writing operation
     Args:
         file_path (str): path to the file
         done (bool, optional): True if the file writing operation is done. Defaults to True.
         successful (bool, optional): True if the file writing operation was successful. Defaults to True.
         metadata (dict, optional): status metadata. Defaults to None.
     """
 
-    msg_type = "file_message"
+    msg_type: ClassVar[str] = "file_message"
     file_path: str
-    done: bool = field(default=True)
-    successful: bool = field(default=True)
-    metadata: dict = field(default_factory=dict)
+    done: bool = Field(default=True)
+    successful: bool = Field(default=True)
 
 
-@dataclass(eq=False)
 class FileContentMessage(BECMessage):
     """File content message to inform about the content of a file
     Args:
         file_path (str): path to the file
         data (str): content of the file
         metadata (dict, optional): status metadata. Defaults to None.
     """
 
-    msg_type = "file_content_message"
+    msg_type: ClassVar[str] = "file_content_message"
     file_path: str
     data: dict
-    metadata: dict = field(default_factory=dict)
 
 
-@dataclass(eq=False)
 class VariableMessage(BECMessage):
     """Message to inform about a global variable
     Args:
-        value (str): name of the global variable
+        value (any): Variable value
         metadata (dict, optional): additional metadata
     """
 
-    msg_type = "var_message"
-    value: str
-    metadata: dict = field(default_factory=dict)
+    msg_type: ClassVar[str] = "var_message"
+    value: Any
 
 
-@dataclass(eq=False)
 class ObserverMessage(BECMessage):
     """Message for observer updates
     Args:
         observer (list[dict]): list of observer descriptions (dictionaries)
         metadata (dict, optional): additional metadata
     """
 
-    msg_type = "observer_message"
+    msg_type: ClassVar[str] = "observer_message"
     observer: list[dict]
-    metadata: dict = field(default_factory=dict)
 
 
-@dataclass(eq=False)
 class ServiceMetricMessage(BECMessage):
     """Message for service metrics
     Args:
         name (str): name of the service
         metrics (dict): dictionary with service metrics
         metadata (dict, optional): additional metadata
     """
 
-    msg_type = "service_metric_message"
+    msg_type: ClassVar[str] = "service_metric_message"
     name: str
     metrics: dict
-    metadata: dict = field(default_factory=dict)
 
 
-@dataclass(eq=False)
 class ProcessedDataMessage(BECMessage):
     """Message for processed data
     Args:
         data (str): processed data
         metadata (dict, optional): metadata. Defaults to None.
     """
 
-    msg_type = "processed_data_message"
-    data: str
-    metadata: dict = field(default_factory=dict)
+    msg_type: ClassVar[str] = "processed_data_message"
+    data: dict | list[dict]
 
 
-@dataclass(eq=False)
 class DAPConfigMessage(BECMessage):
     """Message for DAP configuration
     Args:
         config (dict): DAP configuration
         metadata (dict, optional): metadata. Defaults to None.
     """
 
-    msg_type = "dap_config_message"
+    msg_type: ClassVar[str] = "dap_config_message"
     config: dict
-    metadata: dict = field(default_factory=dict)
 
 
-@dataclass(eq=False)
 class DAPRequestMessage(BECMessage):
     """Message for DAP requests
     Args:
         dap_cls (str): DAP class name
         dap_type (Literal["continuous", "on_demand"]): DAP type. Either "continuous" or "on_demand"
         config (dict): DAP configuration
         metadata (dict, optional): metadata. Defaults to None.
     """
 
-    msg_type = "dap_request_message"
+    msg_type: ClassVar[str] = "dap_request_message"
     dap_cls: str
     dap_type: Literal["continuous", "on_demand"]
     config: dict
-    metadata: dict = field(default_factory=dict)
 
-    def _is_valid(self) -> bool:
-        if self.dap_type not in ["continuous", "on_demand"]:
-            return False
-        return True
+    @field_validator("dap_type")
+    @classmethod
+    def check_dap_type(cls, v):
+        """Validate the dap_type"""
+        if v not in ["continuous", "on_demand"]:
+            raise ValueError(f"Invalid dap_type {v}. Must be one of ['continuous', 'on_demand']")
+        return v
 
 
-@dataclass(eq=False)
 class DAPResponseMessage(BECMessage):
     """
     Message for DAP responses
     Args:
         success (bool): True if the request was successful
-        data (dict, optional): DAP data. Defaults to None.
+        data (tuple, optional): DAP data (tuple of data and metadata). Defaults to None.
         error (dict, optional): DAP error. Defaults to None.
         dap_request (dict, optional): DAP request. Defaults to None.
         metadata (dict, optional): metadata. Defaults to None.
     """
 
-    msg_type = "dap_response_message"
+    msg_type: ClassVar[str] = "dap_response_message"
     success: bool
-    data: dict = field(default_factory=dict)
-    error: dict = field(default_factory=dict)
-    dap_request: dict = field(default_factory=dict)
-    metadata: dict = field(default_factory=dict)
+    data: tuple | None = Field(default_factory=lambda: ({}, None))
+    error: str | None = None
+    dap_request: BECMessage | None = Field(default=None)
 
 
-@dataclass(eq=False)
 class AvailableResourceMessage(BECMessage):
     """Message for available resources such as scans, data processing plugins etc
     Args:
         resource (dict): resource description
         metadata (dict, optional): metadata. Defaults to None.
     """
 
-    msg_type = "available_resource_message"
-    resource: dict
-    metadata: dict = field(default_factory=dict)
+    msg_type: ClassVar[str] = "available_resource_message"
+    resource: dict | list[dict]
 
 
-@dataclass(eq=False)
 class ProgressMessage(BECMessage):
     """Message for communicating the progress of a long running task
     Args:
         value (float): current progress value
         max_value (float): maximum progress value
         done (bool): True if the task is done
         metadata (dict, optional): metadata. Defaults to None.
     """
 
-    msg_type = "progress_message"
+    msg_type: ClassVar[str] = "progress_message"
     value: float
     max_value: float
     done: bool
-    metadata: dict = field(default_factory=dict)
 
 
-@dataclass(eq=False)
 class GUIConfigMessage(BECMessage):
     """Message for GUI configuration
     Args:
         config (dict): GUI configuration
         metadata (dict, optional): metadata. Defaults to None.
     """
 
-    msg_type = "gui_config_message"
+    msg_type: ClassVar[str] = "gui_config_message"
     config: dict
-    metadata: dict = field(default_factory=dict)
 
 
-@dataclass(eq=False)
 class GUIDataMessage(BECMessage):
     """Message for GUI data
     Args:
         data (dict): GUI data
         metadata (dict, optional): metadata. Defaults to None.
     """
 
-    msg_type = "gui_data_message"
+    msg_type: ClassVar[str] = "gui_data_message"
     data: dict
-    metadata: dict = field(default_factory=dict)
 
 
-@dataclass(eq=False)
 class GUIInstructionMessage(BECMessage):
     """Message for GUI instructions
     Args:
         instruction (str): GUI instruction
         metadata (dict, optional): metadata. Defaults to None.
     """
 
-    msg_type = "gui_instruction_message"
+    msg_type: ClassVar[str] = "gui_instruction_message"
     action: str
     parameter: dict
-    metadata: dict = field(default_factory=dict)
 
 
-@dataclass(eq=False)
 class ServiceResponseMessage(BECMessage):
     """Message for service responses
     Args:
         response (dict): service response
         metadata (dict, optional): metadata. Defaults to None.
     """
 
-    msg_type = "service_response_message"
+    msg_type: ClassVar[str] = "service_response_message"
     response: dict
-    metadata: dict = field(default_factory=dict)
 
 
-@dataclass(eq=False)
 class CredentialsMessage(BECMessage):
     """Message for credentials
     Args:
         credentials (dict): credentials
         metadata (dict, optional): metadata. Defaults to None.
     """
 
-    msg_type = "credentials_message"
+    msg_type: ClassVar[str] = "credentials_message"
     credentials: dict
-    metadata: dict = field(default_factory=dict)
```

### Comparing `bec_lib-1.9.0/bec_lib/numpy_encoder.py` & `bec_lib-2.0.1/bec_lib/numpy_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """
+This module contains the numpy encoder and decoder functions for serializing and deserializing numpy objects.
 Modified from https://github.com/lebedov/msgpack-numpy
 """
 
 import pickle
 import sys
 
 import numpy as np
```

### Comparing `bec_lib-1.9.0/bec_lib/observer.py` & `bec_lib-2.0.1/bec_lib/observer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+"""
+This module provides the Observer class and the ObserverManager class. The Observer class is used
+to define an observer object, which is used to monitor a device for a specific condition. The
+ObserverManager class is used to manage the observer objects.
+"""
+
 from __future__ import annotations
 
 import enum
 from typing import TYPE_CHECKING
 
 from typeguard import typechecked
 
-from bec_lib import messages
 from bec_lib.device import Device
 from bec_lib.endpoints import MessageEndpoints
 
 if TYPE_CHECKING:
     from bec_lib.devicemanager import DeviceManagerBase
 
 
@@ -148,15 +153,15 @@
         self.update_observer()
 
     def _is_device_observed(self, device: str) -> bool:
         return any(obs.device == device for obs in self._observer)
 
     def _get_installed_observer(self):
         # get current observer list from Redis
-        observer_msg = self.device_manager.producer.get(MessageEndpoints.observer())
+        observer_msg = self.device_manager.connector.get(MessageEndpoints.observer())
         if observer_msg is None:
             return []
         return [Observer.from_dict(obs) for obs in observer_msg.content["observer"]]
 
     def update_observer(self):
         # send the current observer list to MongoDB and Redis
         pass
```

### Comparing `bec_lib-1.9.0/bec_lib/pdf_writer.py` & `bec_lib-2.0.1/bec_lib/pdf_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+"""
+This module contains a class for writing pdfs.
+"""
+
 import datetime
 
 from fpdf import FPDF
 
 
 class BECPDF(FPDF):
+    """Custom PDF class for BEC."""
+
     def header(self):
         if not hasattr(self, "title"):
             return
         # Arial bold 15
         self.set_font("Courier", "", 8)
         # Calculate width of title and position
         w = self.get_string_width(self.title) + 6
@@ -27,14 +33,16 @@
         # date
         self.cell(0, 10, f"BEC, {str(datetime.datetime.now())}", 0, 0, "L")
         # Page number
         self.cell(0, 10, "Page " + str(self.page_no()), 0, 0, "R")
 
 
 class PDFWriter:
+    """Class for writing pdfs."""
+
     LEFT_MARGIN = 25
     TOP_MARGIN = 20
     RIGHT_MARGIN = 20
     FONT_SIZE = 10
 
     def __init__(self, file: str, title: str = None, font="Courier") -> None:
         """Filer writer for pdfs.
```

### Comparing `bec_lib-1.9.0/bec_lib/queue_items.py` & `bec_lib-2.0.1/bec_lib/queue_items.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This module contains the QueueItem and QueueStorage classes.
+"""
+
 from __future__ import annotations
 
 import functools
 import threading
 from collections import deque
 from typing import TYPE_CHECKING
 
@@ -30,33 +34,35 @@
 
 
 class QueueItem:
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         scan_manager: ScanManager,
-        queueID: str,
+        queue_id: str,
         request_blocks: list,
         status: str,
         active_request_block: dict,
-        scanID: list(str),
+        scan_id: list[str],
         **_kwargs,
     ) -> None:
         self.scan_manager = scan_manager
-        self.queueID = queueID
+        self.queue_id = queue_id
         self.request_blocks = request_blocks
         self._status = status
         self.active_request_block = active_request_block
-        self.scanIDs = scanID
+        self.scan_ids = scan_id
 
     @property
     @update_queue
     def scans(self) -> list[ScanItem]:
         """get the scans items assigned to the current queue item"""
-        return [self.scan_manager.scan_storage.find_scan_by_ID(scanID) for scanID in self.scanIDs]
+        return [
+            self.scan_manager.scan_storage.find_scan_by_ID(scan_id) for scan_id in self.scan_ids
+        ]
 
     @property
     @update_queue
     def requestIDs(self):
         return [request_block["RID"] for request_block in self.request_blocks]
 
     @property
@@ -73,131 +79,129 @@
     def status(self):
         return self._status
 
     def _update_with_buffer(self):
         current_queue = self.scan_manager.queue_storage.current_scan_queue
         queue_info = current_queue["primary"].get("info")
         for queue_item in queue_info:
-            if queue_item["queueID"] == self.queueID:
+            if queue_item["queue_id"] == self.queue_id:
                 self.update_queue_item(queue_item)
                 return
-        history = self.scan_manager.queue_storage.queue_history()
+        history = self.scan_manager.queue_storage.queue_history
         for queue_item in history:
-            if queue_item.content["queueID"] == self.queueID:
+            if queue_item.content["queue_id"] == self.queue_id:
                 self.update_queue_item(queue_item.content["info"])
                 return
 
     def update_queue_item(self, queue_item):
         """update the queue item"""
         self.request_blocks = queue_item.get("request_blocks")
         self._status = queue_item.get("status")
         self.active_request_block = queue_item.get("active_request_block")
-        self.scanIDs = queue_item.get("scanID")
+        self.scan_ids = queue_item.get("scan_id")
 
     @property
     def queue_position(self) -> int | None:
         """get the current queue position"""
         current_queue = self.scan_manager.queue_storage.current_scan_queue
         for queue_group in current_queue.values():
             if not isinstance(queue_group, dict):
                 continue
             for queue_position, queue in enumerate(queue_group["info"]):
-                if self.queueID == queue["queueID"]:
+                if self.queue_id == queue["queue_id"]:
                     return queue_position
         return None
 
 
 class QueueStorage:
     """stores queue items"""
 
     def __init__(self, scan_manager: ScanManager, maxlen=50) -> None:
         self.storage: deque[QueueItem] = deque(maxlen=maxlen)
         self._lock = threading.RLock()
         self.scan_manager = scan_manager
-        self._current_scan_queue = None
+        self.current_scan_queue = None
+        self.queue_history = None
 
-    def queue_history(self, history=5):
-        """get the queue history of length 'history'"""
-        if not history:
-            raise ValueError("History length cannot be 0.")
-        if history < 0:
-            history *= -1
+    def _update_queue_history(self):
+        """get the queue history from redis"""
+        self.queue_history = self.scan_manager.connector.lrange(
+            MessageEndpoints.scan_queue_history(), 0, 5
+        )
 
-        return self.scan_manager.producer.lrange(MessageEndpoints.scan_queue_history(), 0, history)
-
-    @property
-    def current_scan_queue(self) -> dict:
+    def _update_current_scan_queue(self):
         """get the current scan queue from redis"""
-        msg = self.scan_manager.producer.get(MessageEndpoints.scan_queue_status())
+        msg = self.scan_manager.connector.get(MessageEndpoints.scan_queue_status())
         if msg:
-            self._current_scan_queue = msg.content["queue"]
-        return self._current_scan_queue
+            self.current_scan_queue = msg.content["queue"]
 
-    @current_scan_queue.setter
-    def current_scan_queue(self, val: dict):
-        self._current_scan_queue = val
+    def _update_queue(self):
+        self._update_current_scan_queue()
+        self._update_queue_history()
 
     def describe_queue(self):
         """create a rich.table description of the current scan queue"""
         queue_tables = []
+        self._update_queue()
         console = Console()
         for queue_name, scan_queue in self.current_scan_queue.items():
             table = Table(title=f"{queue_name} queue / {scan_queue.get('status')}")
-            table.add_column("queueID", justify="center")
-            table.add_column("scanID", justify="center")
+            table.add_column("queue_id", justify="center")
+            table.add_column("scan_id", justify="center")
             table.add_column("is_scan", justify="center")
             table.add_column("type", justify="center")
             table.add_column("scan_number", justify="center")
             table.add_column("IQ status", justify="center")
 
             for instruction_queue in scan_queue.get("info"):
                 scan_msgs = [
                     msg.get("content") for msg in instruction_queue.get("request_blocks", [])
                 ]
                 table.add_row(
-                    instruction_queue.get("queueID"),
-                    ", ".join([str(s) for s in instruction_queue.get("scanID")]),
+                    instruction_queue.get("queue_id"),
+                    ", ".join([str(s) for s in instruction_queue.get("scan_id")]),
                     ", ".join([str(s) for s in instruction_queue.get("is_scan")]),
                     ", ".join([msg["scan_type"] for msg in scan_msgs]),
                     ", ".join([str(s) for s in instruction_queue.get("scan_number")]),
                     instruction_queue.get("status"),
                 )
             with console.capture() as capture:
                 console.print(table)
             queue_tables.append(capture.get())
         return queue_tables
 
     @threadlocked
     def update_with_status(self, queue_msg: messages.ScanQueueStatusMessage) -> None:
         """update a queue item with a new ScanQueueStatusMessage / queue message"""
         self.current_scan_queue = queue_msg.content["queue"]
+        self._update_queue_history()
         queue_info = queue_msg.content["queue"]["primary"].get("info")
         for queue_item in queue_info:
-            queue = self.find_queue_item_by_ID(queueID=queue_item["queueID"])
+            queue = self.find_queue_item_by_ID(queue_id=queue_item["queue_id"])
             if queue:
                 queue.update_queue_item(queue_item)
                 continue
             self.storage.append(QueueItem(scan_manager=self.scan_manager, **queue_item))
 
     @threadlocked
-    def find_queue_item_by_ID(self, queueID: str) -> QueueItem | None:
-        """find a queue item based on its queueID"""
+    def find_queue_item_by_ID(self, queue_id: str) -> QueueItem | None:
+        """find a queue item based on its queue_id"""
         for queue_item in self.storage:
-            if queue_item.queueID == queueID:
+            if queue_item.queue_id == queue_id:
                 return queue_item
         return None
 
     @threadlocked
     def find_queue_item_by_requestID(self, requestID: str) -> QueueItem | None:
         """find a queue item based on its requestID"""
         for queue_item in self.storage:
             if requestID in queue_item.requestIDs:
                 return queue_item
         return None
 
     @threadlocked
-    def find_queue_item_by_scanID(self, scanID: str) -> QueueItem | None:
-        """find a queue item based on its scanID"""
+    def find_queue_item_by_scan_id(self, scan_id: str) -> QueueItem | None:
+        """find a queue item based on its scan_id"""
         for queue_item in self.storage:
-            if scanID in queue_item.scans:
+            if scan_id in queue_item.scans:
                 return queue_item
         return None
```

### Comparing `bec_lib-1.9.0/bec_lib/redis_connector.py` & `bec_lib-2.0.1/bec_lib/redis_connector.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,218 +1,674 @@
+"""
+This module provides a connector to a redis server. It is a wrapper around the
+redis library providing a simple interface to send and receive messages from a
+redis server.
+"""
+
 from __future__ import annotations
 
+import collections
+import inspect
+import queue
+import sys
+import threading
 import time
 import warnings
+from dataclasses import dataclass
 from functools import wraps
 from typing import TYPE_CHECKING
 
+import louie
 import redis
+import redis.client
+import redis.exceptions
 
-from bec_lib.connector import (
-    ConnectorBase,
-    ConsumerConnector,
-    ConsumerConnectorThreaded,
-    MessageObject,
-    ProducerConnector,
-)
-from bec_lib.endpoints import MessageEndpoints
+from bec_lib.connector import ConnectorBase, MessageObject
+from bec_lib.endpoints import EndpointInfo, MessageEndpoints
+from bec_lib.logger import bec_logger
 from bec_lib.messages import AlarmMessage, BECMessage, LogMessage
 from bec_lib.serialization import MsgpackSerialization
 
 if TYPE_CHECKING:
     from bec_lib.alarm_handler import Alarms
 
 
-def catch_connection_error(func):
-    """catch connection errors"""
+def validate_endpoint(endpoint_arg):
+    def decorator(func):
+        argspec = inspect.getfullargspec(func)
+        argument_index = argspec.args.index(endpoint_arg)
 
-    @wraps(func)
-    def wrapper(*args, **kwargs):
-        try:
-            return func(*args, **kwargs)
-        except redis.exceptions.ConnectionError:
-            warnings.warn("Failed to connect to redis. Is the server running?")
-            time.sleep(0.1)
-            return None
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            try:
+                endpoint = args[argument_index]
+                arg = list(args)
+            except IndexError:
+                endpoint = kwargs[endpoint_arg]
+                arg = kwargs
+            if isinstance(endpoint, str):
+                warnings.warn(
+                    "RedisConnector methods with a string topic are deprecated and should not be used anymore. Use RedisConnector methods with an EndpointInfo instead.",
+                    DeprecationWarning,
+                )
+                return func(*args, **kwargs)
+            elif isinstance(endpoint, EndpointInfo):
+                if func.__name__ not in endpoint.message_op:
+                    raise ValueError(
+                        f"Endpoint {endpoint} is not compatible with {func.__name__} method"
+                    )
+                if isinstance(arg, list):
+                    arg[argument_index] = endpoint.endpoint
+                    return func(*arg, **kwargs)
+                else:
+                    arg[endpoint_arg] = endpoint.endpoint
+                    return func(*args, **arg)
+            else:
+                raise TypeError(f"Endpoint {endpoint} is not EndpointInfo")
 
-    return wrapper
+        return wrapper
 
+    return decorator
 
-class RedisConnector(ConnectorBase):
-    def __init__(self, bootstrap: list, redis_cls=None):
-        super().__init__(bootstrap)
-        self.redis_cls = redis_cls
-        self.host, self.port = (
-            bootstrap[0].split(":") if isinstance(bootstrap, list) else bootstrap.split(":")
-        )
-        self._notifications_producer = RedisProducer(
-            host=self.host, port=self.port, redis_cls=self.redis_cls
-        )
 
-    def producer(self, **kwargs):
-        return RedisProducer(host=self.host, port=self.port, redis_cls=self.redis_cls)
+@dataclass
+class StreamTopicInfo:
+    topic: str | list[str]
+    stream_id: int
+    id: str
+    newest_only: bool
+    from_start: bool
+    cb: callable
+    kwargs: dict
+
+
+class StreamRegisterMixin:
+    """
+    Mixin to add stream registration capabilities to a connector
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._stream_topics_cb = collections.defaultdict(list)
+        self._stream_events_listener_thread = None
+        self._stream_events_dispatcher_thread = None
+        self._stream_messages_queue = queue.Queue()
+        self._stop_stream_events_listener_thread = threading.Event()
+        self._custom_stream_listeners = {}
+        self.__stream_counter = 0
+
+    def _stream_counter(self):
+        self.__stream_counter += 1
+        return self.__stream_counter
 
-    # pylint: disable=too-many-arguments
-    def consumer(
+    def register_stream(
         self,
-        topics=None,
-        pattern=None,
-        group_id=None,
-        event=None,
-        cb=None,
-        threaded=True,
-        name=None,
+        topics: str | list[str] | EndpointInfo | list[EndpointInfo] = None,
+        patterns: str | list[str] | EndpointInfo | list[EndpointInfo] = None,
+        cb: callable = None,
+        from_start: bool = False,
+        newest_only: bool = False,
+        start_thread: bool = True,
         **kwargs,
-    ):
-        if cb is None:
-            raise ValueError("The callback function must be specified.")
+    ) -> int:
+        """
+        Register a callback for a stream topic or pattern
+
+        Args:
+            topic (str, optional): Topic. This should be a valid message endpoint in BEC and can be a string or an EndpointInfo object. Defaults to None. Either topic or pattern should be provided.
+            pattern (str, optional): Pattern of topics. In contrast to topics, patterns may contain "*" wildcards. The evaluated patterns should be a valid message endpoint in BEC and can be a string or an EndpointInfo object. Defaults to None. Either topic or pattern should be provided.
+            cb (callable, optional): callback. Defaults to None.
+            from_start (bool, optional): read from start. Defaults to False.
+            newest_only (bool, optional): read newest only. Defaults to False.
+            start_thread (bool, optional): start the dispatcher thread. Defaults to True.
+            **kwargs: additional keyword arguments to be transmitted to the callback
+
+        Returns:
+            int: stream id
+
+        Examples:
+            >>> def my_callback(msg, **kwargs):
+            ...     print(msg)
+            ...
+            >>> connector.register_stream("test", my_callback)
+            >>> connector.register_stream(topic="test", cb=my_callback)
+            >>> connector.register_stream(pattern="test:*", cb=my_callback)
+            >>> connector.register_stream(pattern="test:*", cb=my_callback, start_thread=False)
+            >>> connector.register_stream(pattern="test:*", cb=my_callback, start_thread=False, my_arg="test")
+        """
+
+        if topics is None and patterns is None:
+            raise ValueError("topics and pattern cannot be both None")
+
+        if newest_only and from_start:
+            raise ValueError("newest_only and from_start cannot be both True")
+
+        if not cb:
+            raise ValueError("Callback cb cannot be None")
+
+        # make a weakref from the callable, using louie;
+        # it can create safe refs for simple functions as well as methods
+        cb_ref = louie.saferef.safe_ref(cb)
+
+        if patterns is not None:
+            stream_topics = self._convert_endpointinfo_to_str(patterns)
+        else:
+            stream_topics = self._convert_endpointinfo_to_str(topics)
+
+        if newest_only:
+            # if newest_only is True, we need to provide a separate callback for each topic,
+            # directly calling the callback. This is because we need to have a backpressure
+            # mechanism in place, and we cannot rely on the dispatcher thread to handle it.
+            if isinstance(stream_topics, list):
+                out = []
+                for topic in stream_topics:
+                    out.append(self._add_direct_stream_listener(topic, cb_ref, **kwargs))
+                return out
+            return self._add_direct_stream_listener(stream_topics, cb_ref, **kwargs)
+
+        if self._stream_events_listener_thread is None:
+            # create the thread that will get all messages for this connector;
+            self._stream_events_listener_thread = threading.Thread(
+                target=self._get_stream_messages_loop, daemon=True
+            )
+            self._stream_events_listener_thread.start()
+        if isinstance(stream_topics, list):
+            stream_id = []
+            for topic in stream_topics:
+                stream_id.append(self._stream_counter())
+                self._stream_topics_cb[topic].append(
+                    StreamTopicInfo(
+                        id="0-0",
+                        topic=topic,
+                        stream_id=stream_id,
+                        newest_only=newest_only,
+                        from_start=from_start,
+                        cb=cb_ref,
+                        kwargs=kwargs,
+                    )
+                )
+        else:
+            stream_id = self._stream_counter()
+            self._stream_topics_cb[stream_topics].append(
+                StreamTopicInfo(
+                    id="0-0",
+                    topic=stream_topics,
+                    stream_id=stream_id,
+                    newest_only=newest_only,
+                    from_start=from_start,
+                    cb=cb_ref,
+                    kwargs=kwargs,
+                )
+            )
 
-        if threaded:
-            if topics is None and pattern is None:
-                raise ValueError("Topics must be set for threaded consumer")
-            listener = RedisConsumerThreaded(
-                self.host,
-                self.port,
-                topics,
-                pattern,
-                group_id,
-                event,
-                cb,
-                redis_cls=self.redis_cls,
-                name=name,
-                **kwargs,
+        if start_thread and self._stream_events_dispatcher_thread is None:
+            # start dispatcher thread
+            self._stream_events_dispatcher_thread = threading.Thread(
+                target=self._dispatch_stream_events, daemon=True
             )
-            self._threads.append(listener)
-            return listener
-        return RedisConsumer(
-            self.host,
-            self.port,
-            topics,
-            pattern,
-            group_id,
-            event,
-            cb,
-            redis_cls=self.redis_cls,
-            **kwargs,
+            self._stream_events_dispatcher_thread.start()
+        return stream_id
+
+    def unregister_stream(self, stream_id: int) -> bool:
+        """
+        Unregister a stream listener.
+
+        Args:
+            stream_id (int): stream id
+
+        Returns:
+            bool: True if the stream listener has been removed, False otherwise
+        """
+
+        if stream_id in self._custom_stream_listeners:
+            listener = self._custom_stream_listeners.pop(stream_id)
+            event = listener["stop_event"]
+            thread = listener["thread"]
+            event.set()
+            thread.join()
+            return True
+        if stream_id in self._stream_topics_cb:
+            self._stream_topics_cb.pop(stream_id)
+            return True
+        return False
+
+    def _add_direct_stream_listener(self, topic, cb, **kwargs) -> int:
+        """
+        Add a direct listener for a topic. This is used when newest_only is True.
+
+        Args:
+            topic (str): topic
+            cb (callable): callback
+            kwargs (dict): additional keyword arguments to be transmitted to the callback
+
+        Returns:
+            int: stream id
+        """
+        stream_id = self._stream_counter()
+        info = StreamTopicInfo(
+            id="0-0",
+            topic=topic,
+            stream_id=stream_id,
+            newest_only=True,
+            from_start=False,
+            cb=cb,
+            kwargs=kwargs,
         )
+        event = threading.Event()
+        thread = threading.Thread(
+            target=self._direct_stream_listener, args=(info, event), daemon=True
+        )
+        self._custom_stream_listeners[stream_id] = {
+            "info": info,
+            "thread": thread,
+            "stop_event": event,
+        }
+        thread.start()
+
+        return stream_id
+
+    def _direct_stream_listener(self, info: StreamTopicInfo, stop_event: threading.Event):
+        while not stop_event.is_set():
+            msg = self.xread(info.topic, count=1, block=1000)
+            if not msg:
+                time.sleep(0.1)
+                continue
+            cb = info.cb()
+            if not cb:
+                return
+            try:
+                cb(msg[0], **info.kwargs)
+            # pylint: disable=broad-except
+            except Exception:
+                sys.excepthook(*sys.exc_info())
+
+    def _dispatch_stream_events(self):
+        while self.poll_stream_messages():
+            ...
+
+    def _get_stream_topics(self) -> dict:
+        stream_topics = {}
+        for topic, subscriber in self._stream_topics_cb.items():
+            for info in subscriber:
+                stream_topics[topic] = info.id
+        return stream_topics
 
-    def stream_consumer(
-        self,
-        topics=None,
-        pattern=None,
-        group_id=None,
-        event=None,
-        cb=None,
-        from_start=False,
-        newest_only=False,
-        **kwargs,
-    ):
+    def _get_stream_messages_loop(self) -> None:
+        """
+        Get stream messages loop. This method is run in a separate thread and listens
+        for messages from the redis server.
+        """
+        error = False
+        while not self._stop_stream_events_listener_thread.is_set():
+            try:
+                stream_topics = self._get_stream_topics()
+                if not stream_topics:
+                    continue
+                msg = self._redis_conn.xread(streams=stream_topics, block=1000)
+                print(stream_topics)
+
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
+                if msg is not None:
+                    self._stream_messages_queue.put(msg)
+
+    def poll_stream_messages(self, timeout=None) -> None:
         """
-        Threaded stream consumer for redis streams.
+        Poll for new messages, receive them and execute callbacks
 
         Args:
-            topics (str, list): topics to subscribe to
-            pattern (str, list): pattern to subscribe to
-            group_id (str): group id
-            event (threading.Event): event to stop the consumer
-            cb (function): callback function
-            from_start (bool): read from start. Defaults to False.
-            newest_only (bool): read only the newest message. Defaults to False.
+            timeout ([type], optional): timeout in seconds. Defaults to None.
         """
-        if cb is None:
-            raise ValueError("The callback function must be specified.")
+        while True:
+            try:
+                msg = self._stream_messages_queue.get(timeout=timeout)
+            except queue.Empty as exc:
+                raise TimeoutError(
+                    f"{self}: poll_stream_messages: did not receive a message within {timeout} seconds"
+                ) from exc
+            if msg is StopIteration:
+                return False
+            if self._handle_stream_message(msg):
+                return True
+
+    def _handle_stream_message(self, msg):
+        if not msg:
+            return False
+        for topic, msgs in msg:
+            callbacks = self._stream_topics_cb[topic.decode()]
+            for index, record in msgs:
+                msg_dict = {
+                    k.decode(): MsgpackSerialization.loads(msg) for k, msg in record.items()
+                }
+                for info in callbacks:
+                    info.id = index
+                    cb = info.cb()
+                    if cb:
+                        try:
+                            cb(msg_dict, **info.kwargs)
+                        # pylint: disable=broad-except
+                        except Exception:
+                            sys.excepthook(*sys.exc_info())
+        return True
+
+    def shutdown(self):
+        """
+        Shutdown the connector
+        """
+        super().shutdown()
+        if self._stream_events_listener_thread:
+            self._stop_stream_events_listener_thread.set()
+            self._stream_events_listener_thread.join()
+            self._stream_events_listener_thread = None
+        if self._stream_events_dispatcher_thread:
+            self._stream_messages_queue.put(StopIteration)
+            self._stream_events_dispatcher_thread.join()
+            self._stream_events_dispatcher_thread = None
 
-        if pattern:
-            raise ValueError("Pattern is currently not supported for stream consumer.")
 
-        if topics is None and pattern is None:
-            raise ValueError("Topics must be set for stream consumer.")
-        listener = RedisStreamConsumerThreaded(
-            self.host,
-            self.port,
-            topics,
-            pattern,
-            group_id,
-            event,
-            cb,
-            redis_cls=self.redis_cls,
-            from_start=from_start,
-            newest_only=newest_only,
-            **kwargs,
+class RedisConnector(StreamRegisterMixin, ConnectorBase):
+    """
+    Redis connector class. This class is a wrapper around the redis library providing
+    a simple interface to send and receive messages from a redis server.
+    """
+
+    def __init__(self, bootstrap: list, redis_cls=None):
+        """
+        Initialize the connector
+
+        Args:
+            bootstrap (list): list of strings in the form "host:port"
+            redis_cls (redis.client, optional): redis client class. Defaults to None.
+        """
+        super().__init__(bootstrap)
+        self.host, self.port = (
+            bootstrap[0].split(":") if isinstance(bootstrap, list) else bootstrap.split(":")
         )
-        self._threads.append(listener)
-        return listener
 
-    @catch_connection_error
+        if redis_cls:
+            self._redis_conn = redis_cls(host=self.host, port=self.port)
+        else:
+            self._redis_conn = redis.Redis(host=self.host, port=self.port)
+
+        # main pubsub connection
+        self._pubsub_conn = self._redis_conn.pubsub()
+        self._pubsub_conn.ignore_subscribe_messages = True
+        # keep track of topics and callbacks
+        self._topics_cb = collections.defaultdict(list)
+
+        self._events_listener_thread = None
+        self._events_dispatcher_thread = None
+        self._messages_queue = queue.Queue()
+        self._stop_events_listener_thread = threading.Event()
+        self.stream_keys = {}
+
+    def shutdown(self):
+        """
+        Shutdown the connector
+        """
+        super().shutdown()
+        if self._events_listener_thread:
+            self._stop_events_listener_thread.set()
+            self._events_listener_thread.join()
+            self._events_listener_thread = None
+        if self._events_dispatcher_thread:
+            self._messages_queue.put(StopIteration)
+            self._events_dispatcher_thread.join()
+            self._events_dispatcher_thread = None
+
+        # release all connections
+        self._pubsub_conn.close()
+        self._redis_conn.close()
+
     def log_warning(self, msg):
-        """send a warning"""
-        self._notifications_producer.send(
-            MessageEndpoints.log(), LogMessage(log_type="warning", log_msg=msg)
-        )
+        """
+        send a warning
+
+        Args:
+            msg (str): warning message
+        """
+        self.set_and_publish(MessageEndpoints.log(), LogMessage(log_type="warning", log_msg=msg))
 
-    @catch_connection_error
     def log_message(self, msg):
-        """send a log message"""
-        self._notifications_producer.send(
-            MessageEndpoints.log(), LogMessage(log_type="log", log_msg=msg)
-        )
+        """
+        send a message as log
+
+        Args:
+            msg (str): message
+        """
+        self.set_and_publish(MessageEndpoints.log(), LogMessage(log_type="log", log_msg=msg))
 
-    @catch_connection_error
     def log_error(self, msg):
-        """send an error as log"""
-        self._notifications_producer.send(
-            MessageEndpoints.log(), LogMessage(log_type="error", log_msg=msg)
-        )
+        """
+        send an error as log
+
+        Args:
+            msg (str): error message
+        """
+        self.set_and_publish(MessageEndpoints.log(), LogMessage(log_type="error", log_msg=msg))
 
-    @catch_connection_error
     def raise_alarm(self, severity: Alarms, alarm_type: str, source: str, msg: str, metadata: dict):
-        """raise an alarm"""
-        self._notifications_producer.set_and_publish(
-            MessageEndpoints.alarm(),
-            AlarmMessage(
-                severity=severity, alarm_type=alarm_type, source=source, msg=msg, metadata=metadata
-            ),
+        """
+        Raise an alarm
+
+        Args:
+            severity (Alarms): alarm severity
+            alarm_type (str): alarm type
+            source (str): source
+            msg (str): message
+            metadata (dict): metadata
+        """
+        alarm_msg = AlarmMessage(
+            severity=severity, alarm_type=alarm_type, source=source, msg=msg, metadata=metadata
         )
+        self.set_and_publish(MessageEndpoints.alarm(), alarm_msg)
 
+    def pipeline(self) -> redis.client.Pipeline:
+        """Create a new pipeline"""
+        return self._redis_conn.pipeline()
 
-class RedisProducer(ProducerConnector):
-    def __init__(self, host: str, port: int, redis_cls=None) -> None:
-        # pylint: disable=invalid-name
-        if redis_cls:
-            self.r = redis_cls(host=host, port=port)
-            return
-        self.r = redis.Redis(host=host, port=port)
-        self.stream_keys = {}
+    def execute_pipeline(self, pipeline) -> list:
+        """
+        Execute a pipeline and return the results
+
+        Args:
+            pipeline (Pipeline): redis pipeline
 
-    def execute_pipeline(self, pipeline):
-        """Execute the pipeline and returns the results with decoded BECMessages"""
+        Returns:
+            list: list of results
+        """
+        if not isinstance(pipeline, redis.client.Pipeline):
+            raise TypeError(f"Expected a redis Pipeline, got {type(pipeline)}")
         ret = []
         results = pipeline.execute()
         for res in results:
             try:
                 ret.append(MsgpackSerialization.loads(res))
             except RuntimeError:
                 ret.append(res)
         return ret
 
-    @catch_connection_error
     def raw_send(self, topic: str, msg: bytes, pipe=None):
-        """send to redis without any check on message type"""
-        client = pipe if pipe is not None else self.r
+        """
+        Send a message to a topic. This is the raw version of send, it does not
+        check the message type. Use this method if you want to send a message
+        that is not a BECMessage.
+
+        Args:
+            topic (str): topic
+            msg (bytes): message
+            pipe (Pipeline, optional): redis pipe. Defaults to None.
+        """
+        client = pipe if pipe is not None else self._redis_conn
         client.publish(topic, msg)
 
-    def send(self, topic: str, msg: BECMessage, pipe=None) -> None:
-        """send to redis"""
+    @validate_endpoint("topic")
+    def send(self, topic: EndpointInfo, msg: BECMessage, pipe=None) -> None:
+        """
+        Send a message to a topic
+
+        Args:
+            topic (str): topic
+            msg (BECMessage): message
+            pipe (Pipeline, optional): redis pipe. Defaults to None.
+        """
         if not isinstance(msg, BECMessage):
             raise TypeError(f"Message {msg} is not a BECMessage")
         self.raw_send(topic, MsgpackSerialization.dumps(msg), pipe)
 
-    @catch_connection_error
+    def register(
+        self,
+        topics: str | list[str] | EndpointInfo | list[EndpointInfo] = None,
+        patterns: str | list[str] | EndpointInfo | list[EndpointInfo] = None,
+        cb: callable = None,
+        start_thread: bool = True,
+        **kwargs,
+    ):
+        """
+        Register a callback for a topic or a pattern
+
+        Args:
+            topics (str, list, EndpointInfo, list[EndpointInfo], optional): topic or list of topics. Defaults to None. The topic should be a valid message endpoint in BEC and can be a string or an EndpointInfo object.
+            patterns (str, list, optional): pattern or list of patterns. Defaults to None. In contrast to topics, patterns may contain "*" wildcards. The evaluated patterns should be a valid message endpoint in BEC and can be a string or an EndpointInfo object.
+            cb (callable, optional): callback. Defaults to None.
+            start_thread (bool, optional): start the dispatcher thread. Defaults to True.
+            **kwargs: additional keyword arguments to be transmitted to the callback
+
+        Examples:
+            >>> def my_callback(msg, **kwargs):
+            ...     print(msg)
+            ...
+            >>> connector.register("test", my_callback)
+            >>> connector.register(topics="test", cb=my_callback)
+            >>> connector.register(patterns="test:*", cb=my_callback)
+            >>> connector.register(patterns="test:*", cb=my_callback, start_thread=False)
+            >>> connector.register(patterns="test:*", cb=my_callback, start_thread=False, my_arg="test")
+        """
+        if self._events_listener_thread is None:
+            # create the thread that will get all messages for this connector;
+            self._events_listener_thread = threading.Thread(
+                target=self._get_messages_loop, args=(self._pubsub_conn,), daemon=True
+            )
+            self._events_listener_thread.start()
+
+        if cb is None:
+            raise ValueError("Callback cb cannot be None")
+        # make a weakref from the callable, using louie;
+        # it can create safe refs for simple functions as well as methods
+        cb_ref = louie.saferef.safe_ref(cb)
+
+        if topics is None and patterns is None:
+            raise ValueError("topics and patterns cannot be both None")
+
+        if patterns is not None:
+            patterns = self._convert_endpointinfo_to_str(patterns)
+            if not isinstance(patterns, list):
+                patterns = [patterns]
+
+            self._pubsub_conn.psubscribe(patterns)
+            for pattern in patterns:
+                self._topics_cb[pattern].append((cb_ref, kwargs))
+        else:
+            topics = self._convert_endpointinfo_to_str(topics)
+            if not isinstance(topics, list):
+                topics = [topics]
+
+            self._pubsub_conn.subscribe(topics)
+            for topic in topics:
+                self._topics_cb[topic].append((cb_ref, kwargs))
+
+        if start_thread and self._events_dispatcher_thread is None:
+            # start dispatcher thread
+            self._events_dispatcher_thread = threading.Thread(
+                target=self._dispatch_events, daemon=True
+            )
+            self._events_dispatcher_thread.start()
+
+    def _convert_endpointinfo_to_str(self, endpoint):
+        if isinstance(endpoint, EndpointInfo):
+            return endpoint.endpoint
+        if isinstance(endpoint, str):
+            return endpoint
+        if isinstance(endpoint, list):
+            return [self._convert_endpointinfo_to_str(e) for e in endpoint]
+        raise ValueError(f"Invalid endpoint {endpoint}")
+
+    def _get_messages_loop(self, pubsub: redis.client.PubSub) -> None:
+        """
+        Get messages loop. This method is run in a separate thread and listens
+        for messages from the redis server.
+
+        Args:
+            pubsub (redis.client.PubSub): pubsub object
+        """
+        error = False
+        while not self._stop_events_listener_thread.is_set():
+            try:
+                msg = pubsub.get_message(timeout=1)
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
+                if msg is not None:
+                    self._messages_queue.put(msg)
+
+    def _handle_message(self, msg):
+        if msg["type"].endswith("subscribe"):
+            # ignore subscribe messages
+            return False
+        channel = msg["channel"].decode()
+        if msg["pattern"] is not None:
+            callbacks = self._topics_cb[msg["pattern"].decode()]
+        else:
+            callbacks = self._topics_cb[channel]
+        msg = MessageObject(topic=channel, value=MsgpackSerialization.loads(msg["data"]))
+        for cb_ref, kwargs in callbacks:
+            cb = cb_ref()
+            if cb:
+                try:
+                    cb(msg, **kwargs)
+                # pylint: disable=broad-except
+                except Exception:
+                    sys.excepthook(*sys.exc_info())
+        return True
+
+    def poll_messages(self, timeout=None) -> None:
+        while True:
+            try:
+                msg = self._messages_queue.get(timeout=timeout)
+            except queue.Empty as exc:
+                raise TimeoutError(
+                    f"{self}: poll_messages: did not receive a message within {timeout} seconds"
+                ) from exc
+            if msg is StopIteration:
+                return False
+            if self._handle_message(msg):
+                return True
+
+    def _dispatch_events(self):
+        while self.poll_messages():
+            ...
+
+    @validate_endpoint("topic")
     def lpush(
-        self, topic: str, msg: str, pipe=None, max_size: int = None, expire: int = None
+        self, topic: EndpointInfo, msg: str, pipe=None, max_size: int = None, expire: int = None
     ) -> None:
         """Time complexity: O(1) for each element added, so O(N) to
         add N elements when the command is called with multiple arguments.
         Insert all the specified values at the head of the list stored at key.
         If key does not exist, it is created as empty list before
         performing the push operations. When key holds a value that
         is not a list, an error is returned."""
@@ -223,107 +679,103 @@
         if max_size:
             client.ltrim(topic, 0, max_size)
         if expire:
             client.expire(topic, expire)
         if not pipe:
             client.execute()
 
-    @catch_connection_error
-    def lset(self, topic: str, index: int, msg: str, pipe=None) -> None:
-        client = pipe if pipe is not None else self.r
+    @validate_endpoint("topic")
+    def lset(self, topic: EndpointInfo, index: int, msg: str, pipe=None) -> None:
+        client = pipe if pipe is not None else self._redis_conn
         if isinstance(msg, BECMessage):
             msg = MsgpackSerialization.dumps(msg)
         return client.lset(topic, index, msg)
 
-    @catch_connection_error
-    def rpush(self, topic: str, msg: str, pipe=None) -> int:
+    @validate_endpoint("topic")
+    def rpush(self, topic: EndpointInfo, msg: str, pipe=None) -> int:
         """O(1) for each element added, so O(N) to add N elements when the
         command is called with multiple arguments. Insert all the specified
         values at the tail of the list stored at key. If key does not exist,
         it is created as empty list before performing the push operation. When
         key holds a value that is not a list, an error is returned."""
-        client = pipe if pipe is not None else self.r
+        client = pipe if pipe is not None else self._redis_conn
         if isinstance(msg, BECMessage):
             msg = MsgpackSerialization.dumps(msg)
         return client.rpush(topic, msg)
 
-    @catch_connection_error
-    def lrange(self, topic: str, start: int, end: int, pipe=None):
+    @validate_endpoint("topic")
+    def lrange(self, topic: EndpointInfo, start: int, end: int, pipe=None):
         """O(S+N) where S is the distance of start offset from HEAD for small
         lists, from nearest end (HEAD or TAIL) for large lists; and N is the
         number of elements in the specified range. Returns the specified elements
         of the list stored at key. The offsets start and stop are zero-based indexes,
         with 0 being the first element of the list (the head of the list), 1 being
         the next element and so on."""
-        client = pipe if pipe is not None else self.r
+        client = pipe if pipe is not None else self._redis_conn
         cmd_result = client.lrange(topic, start, end)
         if pipe:
             return cmd_result
-        else:
-            # in case of command executed in a pipe, use 'execute_pipeline' method
-            ret = []
-            for msg in cmd_result:
-                try:
-                    ret.append(MsgpackSerialization.loads(msg))
-                except RuntimeError:
-                    ret.append(msg)
-            return ret
 
-    @catch_connection_error
-    def set_and_publish(self, topic: str, msg, pipe=None, expire: int = None) -> None:
+        # in case of command executed in a pipe, use 'execute_pipeline' method
+        ret = []
+        for msg in cmd_result:
+            try:
+                ret.append(MsgpackSerialization.loads(msg))
+            except RuntimeError:
+                ret.append(msg)
+        return ret
+
+    @validate_endpoint("topic")
+    def set_and_publish(self, topic: EndpointInfo, msg, pipe=None, expire: int = None) -> None:
         """piped combination of self.publish and self.set"""
         client = pipe if pipe is not None else self.pipeline()
-        if isinstance(msg, BECMessage):
-            msg = MsgpackSerialization.dumps(msg)
-        client.publish(topic, msg)
-        client.set(topic, msg)
-        if expire:
-            client.expire(topic, expire)
+        if not isinstance(msg, BECMessage):
+            raise TypeError(f"Message {msg} is not a BECMessage")
+        msg = MsgpackSerialization.dumps(msg)
+        self.set(topic, msg, pipe=client, expire=expire)
+        self.raw_send(topic, msg, pipe=client)
         if not pipe:
             client.execute()
 
-    @catch_connection_error
-    def set(self, topic: str, msg, pipe=None, expire: int = None) -> None:
+    @validate_endpoint("topic")
+    def set(self, topic: EndpointInfo, msg, pipe=None, expire: int = None) -> None:
         """set redis value"""
-        client = pipe if pipe is not None else self.r
+        client = pipe if pipe is not None else self._redis_conn
         if isinstance(msg, BECMessage):
             msg = MsgpackSerialization.dumps(msg)
         client.set(topic, msg, ex=expire)
 
-    @catch_connection_error
-    def keys(self, pattern: str) -> list:
+    @validate_endpoint("pattern")
+    def keys(self, pattern: EndpointInfo) -> list:
         """returns all keys matching a pattern"""
-        return self.r.keys(pattern)
-
-    @catch_connection_error
-    def pipeline(self):
-        """create a new pipeline"""
-        return self.r.pipeline()
+        return self._redis_conn.keys(pattern)
 
-    @catch_connection_error
-    def delete(self, topic, pipe=None):
+    @validate_endpoint("topic")
+    def delete(self, topic: EndpointInfo, pipe=None):
         """delete topic"""
-        client = pipe if pipe is not None else self.r
+        client = pipe if pipe is not None else self._redis_conn
         client.delete(topic)
 
-    @catch_connection_error
-    def get(self, topic: str, pipe=None):
+    @validate_endpoint("topic")
+    def get(self, topic: EndpointInfo, pipe=None):
         """retrieve entry, either via hgetall or get"""
-        client = pipe if pipe is not None else self.r
+        client = pipe if pipe is not None else self._redis_conn
         data = client.get(topic)
         if pipe:
             return data
         else:
             try:
                 return MsgpackSerialization.loads(data)
             except RuntimeError:
                 return data
 
-    @catch_connection_error
-    def xadd(self, topic: str, msg_dict: dict, max_size=None, pipe=None, expire: int = None):
+    @validate_endpoint("topic")
+    def xadd(
+        self, topic: EndpointInfo, msg_dict: dict, max_size=None, pipe=None, expire: int = None
+    ):
         """
         add to stream
 
         Args:
             topic (str): redis topic
             msg_dict (dict): message to add
             max_size (int, optional): max size of stream. Defaults to None.
@@ -335,54 +787,76 @@
             >>> redis.xadd("test", {"test": "test"}, max_size=10)
         """
         if pipe:
             client = pipe
         elif expire:
             client = self.pipeline()
         else:
-            client = self.r
+            client = self._redis_conn
 
-        for key, msg in msg_dict.items():
-            msg_dict[key] = MsgpackSerialization.dumps(msg)
+        msg_dict = {key: MsgpackSerialization.dumps(val) for key, val in msg_dict.items()}
 
         if max_size:
             client.xadd(topic, msg_dict, maxlen=max_size)
         else:
             client.xadd(topic, msg_dict)
         if expire:
             client.expire(topic, expire)
         if not pipe and expire:
             client.execute()
 
-    @catch_connection_error
-    def get_last(self, topic: str, key="data"):
-        """retrieve last entry from stream"""
-        client = self.r
+    @validate_endpoint("topic")
+    def get_last(self, topic: EndpointInfo, key=None, count=1):
+        """
+        Get last message from stream. Repeated calls will return
+        the same message until a new message is added to the stream.
+
+        Args:
+            topic (str): redis topic
+            key (str, optional): key to retrieve. Defaults to None. If None, the whole message is returned.
+            count (int, optional): number of last elements to retrieve
+        """
+        if count <= 0:
+            return None
+        ret = []
+        client = self._redis_conn
         try:
-            _, msg_dict = client.xrevrange(topic, "+", "-", count=1)[0]
+            res = client.xrevrange(topic, "+", "-", count=count)
+            if not res:
+                return None
+            for _, msg_dict in reversed(res):
+                ret.append(
+                    {k.decode(): MsgpackSerialization.loads(msg) for k, msg in msg_dict.items()}
+                    if key is None
+                    else MsgpackSerialization.loads(msg_dict[key.encode()])
+                )
         except TypeError:
             return None
-        else:
-            msg_dict = {k.decode(): MsgpackSerialization.loads(msg) for k, msg in msg_dict.items()}
 
-            if key is None:
-                return msg_dict
-            return msg_dict.get(key)
+        if count > 1:
+            return ret
+        else:
+            return ret[0]
 
-    @catch_connection_error
+    @validate_endpoint("topic")
     def xread(
-        self, topic: str, id: str = None, count: int = None, block: int = None, from_start=False
+        self,
+        topic: EndpointInfo,
+        id: str = None,
+        count: int = None,
+        block: int = None,
+        from_start=False,
     ) -> list:
         """
         read from stream
 
         Args:
             topic (str): redis topic
             id (str, optional): id to read from. Defaults to None.
-            count (int, optional): number of messages to read. Defaults to None.
+            count (int, optional): number of messages to read. Defaults to None, which means all.
             block (int, optional): block for x milliseconds. Defaults to None.
             from_start (bool, optional): read from start. Defaults to False.
 
         Returns:
             [list]: list of messages
 
         Examples:
@@ -391,23 +865,23 @@
 
             # read one message at a time
             >>> key = 0
             >>> msg = redis.xread("test", key, count=1)
             >>> key = msg[0][1][0][0]
             >>> next_msg = redis.xread("test", key, count=1)
         """
-        client = self.r
+        client = self._redis_conn
         if from_start:
             self.stream_keys[topic] = "0-0"
         if topic not in self.stream_keys:
             if id is None:
                 try:
-                    msg = self.r.xrevrange(topic, "+", "-", count=1)
+                    msg = client.xrevrange(topic, "+", "-", count=1)
                     if msg:
-                        self.stream_keys[topic] = msg[0][0]
+                        self.stream_keys[topic] = msg[0][0].decode()
                         out = {}
                         for key, val in msg[0][1].items():
                             out[key.decode()] = MsgpackSerialization.loads(val)
                         return [out]
                     self.stream_keys[topic] = "0-0"
                 except redis.exceptions.ResponseError:
                     self.stream_keys[topic] = "0-0"
@@ -420,296 +894,69 @@
     def _decode_stream_messages_xread(self, msg):
         out = []
         for topic, msgs in msg:
             for index, record in msgs:
                 out.append(
                     {k.decode(): MsgpackSerialization.loads(msg) for k, msg in record.items()}
                 )
-                self.stream_keys[topic] = index
+                self.stream_keys[topic.decode()] = index
         return out if out else None
 
-    @catch_connection_error
-    def xrange(self, topic: str, min: str, max: str, count: int = None):
+    @validate_endpoint("topic")
+    def xrange(self, topic: EndpointInfo, min: str, max: str, count: int = None):
         """
         read a range from stream
 
         Args:
             topic (str): redis topic
             min (str): min id. Use "-" to read from start
             max (str): max id. Use "+" to read to end
             count (int, optional): number of messages to read. Defaults to None.
+
+        Returns:
+            [list]: list of messages or None
         """
-        client = self.r
+        client = self._redis_conn
         msgs = []
         for reading in client.xrange(topic, min, max, count=count):
-            index, msg_dict = reading
+            _, msg_dict = reading
             msgs.append(
                 {k.decode(): MsgpackSerialization.loads(msg) for k, msg in msg_dict.items()}
             )
-        return msgs
-
-
-class RedisConsumerMixin:
-    def _init_topics_and_pattern(self, topics, pattern):
-        if topics:
-            if not isinstance(topics, list):
-                topics = [topics]
-        if pattern:
-            if not isinstance(pattern, list):
-                pattern = [pattern]
-        return topics, pattern
-
-    def _init_redis_cls(self, redis_cls):
-        # pylint: disable=invalid-name
-        if redis_cls:
-            self.r = redis_cls(host=self.host, port=self.port)
-        else:
-            self.r = redis.Redis(host=self.host, port=self.port)
-
-    @catch_connection_error
-    def initialize_connector(self) -> None:
-        if self.pattern is not None:
-            self.pubsub.psubscribe(self.pattern)
-        else:
-            self.pubsub.subscribe(self.topics)
-
-
-class RedisConsumer(RedisConsumerMixin, ConsumerConnector):
-    # pylint: disable=too-many-arguments
-    def __init__(
-        self,
-        host,
-        port,
-        topics=None,
-        pattern=None,
-        group_id=None,
-        event=None,
-        cb=None,
-        redis_cls=None,
-        **kwargs,
-    ):
-        self.host = host
-        self.port = port
-
-        bootstrap_server = "".join([host, ":", port])
-        topics, pattern = self._init_topics_and_pattern(topics, pattern)
-        super().__init__(
-            bootstrap_server=bootstrap_server,
-            topics=topics,
-            pattern=pattern,
-            group_id=group_id,
-            event=event,
-            cb=cb,
-            **kwargs,
-        )
-        self.error_message_sent = False
-        self._init_redis_cls(redis_cls)
-        self.pubsub = self.r.pubsub()
-        self.initialize_connector()
-
-    @catch_connection_error
-    def poll_messages(self) -> None:
-        """
-        Poll messages from self.connector and call the callback function self.cb
-        """
-        message = self.pubsub.get_message(ignore_subscribe_messages=True)
-        if message is not None:
-            msg = MessageObject(
-                topic=message["channel"], value=MsgpackSerialization.loads(message["data"])
-            )
-            return self.cb(msg, **self.kwargs)
-
-        time.sleep(0.01)
-        return None
-
-    def shutdown(self):
-        """shutdown the consumer"""
-        self.pubsub.close()
-
+        return msgs if msgs else None
 
-class RedisStreamConsumerThreaded(RedisConsumerMixin, ConsumerConnectorThreaded):
-    # pylint: disable=too-many-arguments
-    def __init__(
-        self,
-        host,
-        port,
-        topics=None,
-        pattern=None,
-        group_id=None,
-        event=None,
-        cb=None,
-        redis_cls=None,
-        from_start=False,
-        newest_only=False,
-        **kwargs,
-    ):
-        self.host = host
-        self.port = port
-        self.from_start = from_start
-        self.newest_only = newest_only
-
-        bootstrap_server = "".join([host, ":", port])
-        topics, pattern = self._init_topics_and_pattern(topics, pattern)
-        super().__init__(
-            bootstrap_server=bootstrap_server,
-            topics=topics,
-            pattern=pattern,
-            group_id=group_id,
-            event=event,
-            cb=cb,
-            **kwargs,
+    def producer(self):
+        """Return itself as a producer, to be compatible with old code"""
+        warnings.warn(
+            "RedisConnector.producer() is deprecated and should not be used anymore. A Connector is a producer now, just use the connector object.",
+            FutureWarning,
         )
+        return self
 
-        self._init_redis_cls(redis_cls)
-
-        self.sleep_times = [0.005, 0.1]
-        self.last_received_msg = 0
-        self.idle_time = 30
-        self.error_message_sent = False
-        self.stream_keys = {}
-
-    def initialize_connector(self) -> None:
-        pass
-
-    def _init_topics_and_pattern(self, topics, pattern):
-        if topics:
-            if not isinstance(topics, list):
-                topics = [topics]
-        if pattern:
-            if not isinstance(pattern, list):
-                pattern = [pattern]
-        return topics, pattern
-
-    def get_id(self, topic: str) -> str:
-        """
-        Get the stream key for the given topic.
-
-        Args:
-            topic (str): topic to get the stream key for
-        """
-        if topic not in self.stream_keys:
-            return "0-0"
-        return self.stream_keys.get(topic)
-
-    def get_newest_message(self, container: list, append=True) -> None:
-        """
-        Get the newest message from the stream and update the stream key. If
-        append is True, append the message to the container.
-
-        Args:
-            container (list): container to append the message to
-            append (bool, optional): append to container. Defaults to True.
-        """
-        for topic in self.topics:
-            msg = self.r.xrevrange(topic, "+", "-", count=1)
-            if msg:
-                if append:
-                    container.append((topic, msg[0][1]))
-                self.stream_keys[topic] = msg[0][0]
-            else:
-                self.stream_keys[topic] = "0-0"
-
-    @catch_connection_error
-    def poll_messages(self) -> None:
-        """
-        Poll messages from self.connector and call the callback function self.cb
-
-        """
-        if self.pattern is not None:
-            topics = [key.decode() for key in self.r.scan_iter(match=self.pattern, _type="stream")]
-        else:
-            topics = self.topics
-        messages = []
-        if self.newest_only:
-            self.get_newest_message(messages)
-        elif not self.from_start and not self.stream_keys:
-            self.get_newest_message(messages, append=False)
-        else:
-            streams = {topic: self.get_id(topic) for topic in topics}
-            read_msgs = self.r.xread(streams, count=1)
-            if read_msgs:
-                for msg in read_msgs:
-                    topic = msg[0].decode()
-                    messages.append((topic, msg[1][0][1]))
-                    self.stream_keys[topic] = msg[1][-1][0]
-
-        if messages:
-            if MessageEndpoints.log() not in topics:
-                # no need to update the update frequency just for logs
-                self.last_received_msg = time.time()
-            for topic, msg in messages:
-                try:
-                    msg = MsgpackSerialization.loads(msg[b"data"])
-                except RuntimeError:
-                    msg = msg[b"data"]
-                msg_obj = MessageObject(topic=topic, value=msg)
-                self.cb(msg_obj, **self.kwargs)
-        else:
-            sleep_time = int(bool(time.time() - self.last_received_msg > self.idle_time))
-            if self.sleep_times[sleep_time]:
-                time.sleep(self.sleep_times[sleep_time])
-
-
-class RedisConsumerThreaded(RedisConsumerMixin, ConsumerConnectorThreaded):
-    # pylint: disable=too-many-arguments
-    def __init__(
+    def consumer(
         self,
-        host,
-        port,
         topics=None,
-        pattern=None,
+        patterns=None,
         group_id=None,
         event=None,
         cb=None,
-        redis_cls=None,
+        threaded=True,
         name=None,
         **kwargs,
     ):
-        self.host = host
-        self.port = port
+        """Return a fake thread object to be compatible with old code
 
-        bootstrap_server = "".join([host, ":", port])
-        topics, pattern = self._init_topics_and_pattern(topics, pattern)
-        super().__init__(
-            bootstrap_server=bootstrap_server,
-            topics=topics,
-            pattern=pattern,
-            group_id=group_id,
-            event=event,
-            cb=cb,
-            name=name,
-            **kwargs,
+        In order to keep this fail-safe and simple it uses 'mock'...
+        """
+        from unittest.mock import (  # import is done here, to not pollute the file with something normally in tests
+            Mock,
         )
 
-        self._init_redis_cls(redis_cls)
-        self.pubsub = self.r.pubsub()
-
-        self.sleep_times = [0.005, 0.1]
-        self.last_received_msg = 0
-        self.idle_time = 30
-        self.error_message_sent = False
-
-    @catch_connection_error
-    def poll_messages(self) -> None:
-        """
-        Poll messages from self.connector and call the callback function self.cb
-
-        Note: pubsub messages are supposed to be BECMessage objects only
-        """
-        messages = self.pubsub.get_message(ignore_subscribe_messages=True)
-        if messages is not None:
-            if f"{MessageEndpoints.log()}".encode() not in messages["channel"]:
-                # no need to update the update frequency just for logs
-                self.last_received_msg = time.time()
-            msg = MessageObject(
-                topic=messages["channel"].decode(),
-                value=MsgpackSerialization.loads(messages["data"]),
-            )
-            self.cb(msg, **self.kwargs)
-        else:
-            sleep_time = int(bool(time.time() - self.last_received_msg > self.idle_time))
-            if self.sleep_times[sleep_time]:
-                time.sleep(self.sleep_times[sleep_time])
-
-    def shutdown(self):
-        super().shutdown()
-        self.pubsub.close()
+        warnings.warn(
+            "RedisConnector.consumer() is deprecated and should not be used anymore. Use RedisConnector.register() with 'topics', 'patterns', 'cb' or 'start_thread' instead. Additional keyword args are transmitted to the callback. For the caller, the main difference with RedisConnector.register() is that it does not return a new thread.",
+            FutureWarning,
+        )
+        dummy_thread = Mock(spec=threading.Thread)
+        dummy_thread.start.side_effet = lambda: self.register(
+            topics, patterns, cb, threaded, **kwargs
+        )
+        return dummy_thread
```

### Comparing `bec_lib-1.9.0/bec_lib/request_items.py` & `bec_lib-2.0.1/bec_lib/request_items.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+This module contains the RequestItem class and RequestStorage class. The RequestItem class is used to store information
+about a scan request. The RequestStorage class is used to store request items.
+"""
+
 from __future__ import annotations
 
 import threading
 from collections import deque
 from typing import TYPE_CHECKING
 
 from bec_lib import messages
@@ -21,27 +26,27 @@
 class RequestItem:
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         scan_manager: ScanManager,
         requestID: str,
         decision_pending: bool = True,
-        scanID: str = None,
+        scan_id: str = None,
         request=None,
         response=None,
         accepted: bool = None,
         **_kwargs,
     ) -> None:
         self.scan_manager = scan_manager
         self.requestID = requestID
         self.request = request
         self.response = response
         self.accepted = accepted
         self._decision_pending = decision_pending
-        self._scanID = scanID
+        self._scan_id = scan_id
         self.callbacks = CallbackHandler()
 
     def update_with_response(self, response: messages.RequestResponseMessage):
         """update the current request item with a RequestResponseMessage / response message"""
         self.response = response
         self._decision_pending = False
         self.requestID = response.metadata["RID"]
```

### Comparing `bec_lib-1.9.0/bec_lib/scan_data.py` & `bec_lib-2.0.1/bec_lib/scan_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This module contains the classes for storing scan data from scan_segments. 
+"""
+
 import collections
 from typing import Any
 
 from _collections_abc import dict_items, dict_keys, dict_values
 
 from bec_lib import messages
```

### Comparing `bec_lib-1.9.0/bec_lib/scan_items.py` & `bec_lib-2.0.1/bec_lib/scan_items.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+This module contains the ScanItem and ScanStorage classes. The ScanItem class is used to store
+information about a scan. The ScanStorage class is used to store scan items.
+"""
+
 from __future__ import annotations
 
 import builtins
 import datetime
 import sys
 import threading
 import time
@@ -28,42 +33,42 @@
 class ScanItem:
     status: dict
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         scan_manager: ScanManager,
-        queueID: str,
+        queue_id: str,
         scan_number: list,
-        scanID: list,
+        scan_id: list,
         status: str,
         **_kwargs,
     ) -> None:
         self.scan_manager = scan_manager
-        self._queueID = queueID
+        self._queue_id = queue_id
         self.scan_number = scan_number
-        self.scanID = scanID
+        self.scan_id = scan_id
         self.status = status
         self.data = ScanData()
         self.async_data = {}
         self.baseline = ScanData()
-        self._async_data_handler = AsyncDataHandler(scan_manager.producer)
+        self._async_data_handler = AsyncDataHandler(scan_manager.connector)
         self.open_scan_defs = set()
         self.open_queue_group = None
         self.num_points = None
         self.start_time = None
         self.end_time = None
         self.scan_report_instructions = []
         self.callbacks = []
         self.bec = builtins.__dict__.get("bec")
 
     @property
     def queue(self):
         """get the queue item for the current scan item"""
-        return self.scan_manager.queue_storage.find_queue_item_by_ID(self._queueID)
+        return self.scan_manager.queue_storage.find_queue_item_by_ID(self._queue_id)
 
     def emit_data(self, scan_msg: messages.ScanMessage) -> None:
         self.bec.callbacks.run("scan_segment", scan_msg.content, scan_msg.metadata)
         self._run_request_callbacks("scan_segment", scan_msg.content, scan_msg.metadata)
 
     def emit_status(self, scan_status: messages.ScanStatusMessage) -> None:
         self.bec.callbacks.run("scan_status", scan_status.content, scan_status.metadata)
@@ -94,20 +99,20 @@
             for dev, dev_data in scan_msg_data.items():
                 for signal, signal_data in dev_data.items():
                     for key, value in signal_data.items():
                         tmp[(dev, signal, key)].append(value)
         return pd.DataFrame(tmp)
 
     def _update_async_data(self):
-        self.async_data = self._async_data_handler.get_async_data_for_scan(self.scanID)
-        # msg = messages.ScanMessage(point_id=0, scanID=self.scanID, data=data)
+        self.async_data = self._async_data_handler.get_async_data_for_scan(self.scan_id)
+        # msg = messages.ScanMessage(point_id=0, scan_id=self.scan_id, data=data)
         # self.async_data.set(0, msg)
 
     def __eq__(self, other):
-        return self.scanID == other.scanID
+        return self.scan_id == other.scan_id
 
     def describe(self) -> str:
         """describe the scan item"""
         start_time = (
             f"\tStart time: {datetime.datetime.fromtimestamp(self.start_time).strftime('%c')}\n"
             if self.start_time
             else ""
@@ -118,18 +123,18 @@
             else ""
         )
         elapsed_time = (
             f"\tElapsed time: {(self.end_time-self.start_time):.1f} s\n"
             if self.end_time and self.start_time
             else ""
         )
-        scanID = f"\tScan ID: {self.scanID}\n" if self.scanID else ""
+        scan_id = f"\tScan ID: {self.scan_id}\n" if self.scan_id else ""
         scan_number = f"\tScan number: {self.scan_number}\n" if self.scan_number else ""
         num_points = f"\tNumber of points: {self.num_points}\n" if self.num_points else ""
-        details = start_time + end_time + elapsed_time + scanID + scan_number + num_points
+        details = start_time + end_time + elapsed_time + scan_id + scan_number + num_points
         return details
 
     def __str__(self) -> str:
         return f"ScanItem:\n {self.describe()}"
 
 
 class ScanStorage:
@@ -148,58 +153,59 @@
         if not scan_queue or not scan_queue["primary"].get("info"):
             return None
         return scan_queue["primary"].get("info")[0]
 
     @property
     def current_scan(self) -> ScanItem | None:
         """get the current scan item"""
-        if not self.current_scanID:
+        if not self.current_scan_id:
             return None
-        return self.find_scan_by_ID(scanID=self.current_scanID[0])
+        return self.find_scan_by_ID(scan_id=self.current_scan_id[0])
 
     @property
-    def current_scanID(self) -> str | None:
-        """get the current scanID"""
+    def current_scan_id(self) -> str | None:
+        """get the current scan_id"""
         if self.current_scan_info is None:
             return None
-        return self.current_scan_info.get("scanID")
+        return self.current_scan_info.get("scan_id")
 
     @threadlocked
-    def find_scan_by_ID(self, scanID: str) -> ScanItem | None:
-        """find a scan item based on its scanID"""
+    def find_scan_by_ID(self, scan_id: str) -> ScanItem | None:
+        """find a scan item based on its scan_id"""
         for scan in self.storage:
-            if scanID == scan.scanID:
+            if scan_id == scan.scan_id:
                 return scan
         return None
 
     def update_with_scan_status(self, scan_status: messages.ScanStatusMessage) -> None:
         """update scan item in storage with a new ScanStatusMessage"""
 
-        scanID = scan_status.content["scanID"]
-        if not scanID:
+        scan_id = scan_status.content["scan_id"]
+        if not scan_id:
             return
 
         scan_number = scan_status.content["info"].get("scan_number")
         if scan_number:
             self.last_scan_number = scan_number
 
         while True:
-            scan_item = self.find_scan_by_ID(scanID=scan_status.content["scanID"])
+            scan_item = self.find_scan_by_ID(scan_id=scan_status.content["scan_id"])
             if scan_item:
                 break
             time.sleep(0.1)
 
         # update timestamps
         if scan_status.content.get("status") == "open":
             scan_item.start_time = scan_status.content.get("timestamp")
         elif scan_status.content.get("status") == "closed":
             scan_item.end_time = scan_status.content.get("timestamp")
 
         # update status message
         scan_item.status = scan_status.content.get("status")
+        scan_item.status_message = scan_status
 
         # update total number of points
         if scan_status.content["info"].get("num_points"):
             scan_item.num_points = scan_status.content["info"].get("num_points")
 
         # update scan number
         if scan_item.scan_number is None:
@@ -229,58 +235,58 @@
         # run status callbacks
         scan_item.emit_status(scan_status)
 
     def add_scan_segment(self, scan_msg: messages.ScanMessage) -> None:
         """update a scan item with a new scan segment"""
         logger.info(
             f"Received scan segment {scan_msg.content['point_id']} for scan"
-            f" {scan_msg.metadata['scanID']}: "
+            f" {scan_msg.metadata['scan_id']}: "
         )
         while True:
             with self._lock:
                 for scan_item in self.storage:
-                    if scan_item.scanID == scan_msg.metadata["scanID"]:
+                    if scan_item.scan_id == scan_msg.metadata["scan_id"]:
                         scan_item.data.set(scan_msg.content["point_id"], scan_msg)
                         scan_item.emit_data(scan_msg)
                         return
             time.sleep(0.01)
 
     def add_scan_baseline(self, scan_msg: messages.ScanBaselineMessage) -> None:
         """update a scan item with a new scan baseline"""
-        logger.info(f"Received scan baseline for scan {scan_msg.metadata['scanID']}: ")
+        logger.info(f"Received scan baseline for scan {scan_msg.metadata['scan_id']}: ")
         while True:
             with self._lock:
                 for scan_item in self.storage:
-                    if scan_item.scanID == scan_msg.metadata["scanID"]:
+                    if scan_item.scan_id == scan_msg.metadata["scan_id"]:
                         point = len(scan_item.baseline)
                         scan_item.baseline.set(point, scan_msg)
                         return
             time.sleep(0.01)
 
     @threadlocked
-    def add_scan_item(self, queueID: str, scan_number: list, scanID: list, status: str):
+    def add_scan_item(self, queue_id: str, scan_number: list, scan_id: list, status: str):
         """append new scan item to scan storage"""
-        self.storage.append(ScanItem(self.scan_manager, queueID, scan_number, scanID, status))
+        self.storage.append(ScanItem(self.scan_manager, queue_id, scan_number, scan_id, status))
 
     @threadlocked
     def update_with_queue_status(self, queue_msg: messages.ScanQueueStatusMessage):
         """create new scan items based on their existence in the queue info"""
         queue_info = queue_msg.content["queue"]["primary"].get("info")
         for queue_item in queue_info:
             # append = True
             # for scan_obj in self.storage:
-            #     if len(set(scan_obj.scanID) & set(queue_item["scanID"])) > 0:
+            #     if len(set(scan_obj.scan_id) & set(queue_item["scan_id"])) > 0:
             #         append = False
             if not any(queue_item["is_scan"]):
                 continue
 
-            for ii, scan in enumerate(queue_item["scanID"]):
+            for ii, scan in enumerate(queue_item["scan_id"]):
                 if self.find_scan_by_ID(scan):
                     continue
 
                 logger.debug(f"Appending new scan: {queue_item}")
                 self.add_scan_item(
-                    queueID=queue_item["queueID"],
+                    queue_id=queue_item["queue_id"],
                     scan_number=queue_item["scan_number"][ii],
-                    scanID=queue_item["scanID"][ii],
+                    scan_id=queue_item["scan_id"][ii],
                     status=queue_item["status"],
                 )
```

### Comparing `bec_lib-1.9.0/bec_lib/scan_manager.py` & `bec_lib-2.0.1/bec_lib/scan_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+This module provides a class that provides a convenient way to interact with the scan queue as well
+as the requests and scans that are currently running or have been completed.
+"""
+
 from __future__ import annotations
 
 import uuid
 
 from typeguard import typechecked
 
 from bec_lib import messages
@@ -21,214 +26,206 @@
         as the requests and scans that are currently running or have been completed.
         It also contains storage container for the queue, requests and scans.
 
         Args:
             connector (BECConnector): BECConnector instance
         """
         self.connector = connector
-        self.producer = self.connector.producer()
         self.queue_storage = QueueStorage(scan_manager=self)
         self.request_storage = RequestStorage(scan_manager=self)
         self.scan_storage = ScanStorage(scan_manager=self)
 
-        self._scan_queue_consumer = self.connector.consumer(
-            topics=MessageEndpoints.scan_queue_status(),
-            cb=self._scan_queue_status_callback,
-            parent=self,
-        )
-        self._scan_queue_request_consumer = self.connector.consumer(
-            topics=MessageEndpoints.scan_queue_request(),
-            cb=self._scan_queue_request_callback,
-            parent=self,
+        self.connector.register(
+            topics=MessageEndpoints.scan_queue_status(), cb=self._scan_queue_status_callback
+        )
+        self.connector.register(
+            topics=MessageEndpoints.scan_queue_request(), cb=self._scan_queue_request_callback
         )
-        self._scan_queue_request_response_consumer = self.connector.consumer(
+        self.connector.register(
             topics=MessageEndpoints.scan_queue_request_response(),
             cb=self._scan_queue_request_response_callback,
-            parent=self,
         )
-        self._scan_status_consumer = self.connector.consumer(
-            topics=MessageEndpoints.scan_status(), cb=self._scan_status_callback, parent=self
+        self.connector.register(
+            topics=MessageEndpoints.scan_status(), cb=self._scan_status_callback
         )
 
-        self._scan_segment_consumer = self.connector.consumer(
-            topics=MessageEndpoints.scan_segment(), cb=self._scan_segment_callback, parent=self
+        self.connector.register(
+            topics=MessageEndpoints.scan_segment(), cb=self._scan_segment_callback
         )
 
-        self._baseline_consumer = self.connector.consumer(
-            topics=MessageEndpoints.scan_baseline(), cb=self._baseline_callback, parent=self
-        )
-
-        self._scan_queue_consumer.start()
-        self._scan_queue_request_consumer.start()
-        self._scan_queue_request_response_consumer.start()
-        self._scan_status_consumer.start()
-        self._scan_segment_consumer.start()
-        self._baseline_consumer.start()
+        self.connector.register(topics=MessageEndpoints.scan_baseline(), cb=self._baseline_callback)
 
     def update_with_queue_status(self, queue: messages.ScanQueueStatusMessage) -> None:
         """update storage with a new queue status message"""
         self.queue_storage.update_with_status(queue)
         self.scan_storage.update_with_queue_status(queue)
 
-    def request_scan_interruption(self, deferred_pause=True, scanID: str = None) -> None:
+    def request_scan_interruption(self, deferred_pause=True, scan_id: str = None) -> None:
         """request a scan interruption
 
         Args:
             deferred_pause (bool, optional): Request a deferred pause. If False, a pause will be requested. Defaults to True.
-            scanID (str, optional): ScanID. Defaults to None.
+            scan_id (str, optional): ScanID. Defaults to None.
 
         """
-        if scanID is None:
-            scanID = self.scan_storage.current_scanID
-        if not any(scanID):
+        if scan_id is None:
+            scan_id = self.scan_storage.current_scan_id
+        if not any(scan_id):
             return self.request_scan_abortion()
 
         action = "deferred_pause" if deferred_pause else "pause"
         logger.info(f"Requesting {action}")
-        return self.producer.send(
+        return self.connector.send(
             MessageEndpoints.scan_queue_modification_request(),
-            messages.ScanQueueModificationMessage(scanID=scanID, action=action, parameter={}),
+            messages.ScanQueueModificationMessage(scan_id=scan_id, action=action, parameter={}),
         )
 
-    def request_scan_abortion(self, scanID=None):
+    def request_scan_abortion(self, scan_id=None):
         """request a scan abortion
 
         Args:
-            scanID (str, optional): ScanID. Defaults to None.
+            scan_id (str, optional): ScanID. Defaults to None.
 
         """
-        if scanID is None:
-            scanID = self.scan_storage.current_scanID
+        if scan_id is None:
+            scan_id = self.scan_storage.current_scan_id
         logger.info("Requesting scan abortion")
-        self.producer.send(
+        self.connector.send(
             MessageEndpoints.scan_queue_modification_request(),
-            messages.ScanQueueModificationMessage(scanID=scanID, action="abort", parameter={}),
+            messages.ScanQueueModificationMessage(scan_id=scan_id, action="abort", parameter={}),
         )
 
-    def request_scan_halt(self, scanID=None):
+    def request_scan_halt(self, scan_id=None):
         """request a scan halt
 
         Args:
-            scanID (str, optional): ScanID. Defaults to None.
+            scan_id (str, optional): ScanID. Defaults to None.
 
         """
-        if scanID is None:
-            scanID = self.scan_storage.current_scanID
+        if scan_id is None:
+            scan_id = self.scan_storage.current_scan_id
         logger.info("Requesting scan halt")
-        self.producer.send(
+        self.connector.send(
             MessageEndpoints.scan_queue_modification_request(),
-            messages.ScanQueueModificationMessage(scanID=scanID, action="halt", parameter={}),
+            messages.ScanQueueModificationMessage(scan_id=scan_id, action="halt", parameter={}),
         )
 
-    def request_scan_continuation(self, scanID=None):
+    def request_scan_continuation(self, scan_id=None):
         """request a scan continuation
 
         Args:
-            scanID (str, optional): ScanID. Defaults to None.
+            scan_id (str, optional): ScanID. Defaults to None.
 
         """
-        if scanID is None:
-            scanID = self.scan_storage.current_scanID
+        if scan_id is None:
+            scan_id = self.scan_storage.current_scan_id
         logger.info("Requesting scan continuation")
-        self.producer.send(
+        self.connector.send(
             MessageEndpoints.scan_queue_modification_request(),
-            messages.ScanQueueModificationMessage(scanID=scanID, action="continue", parameter={}),
+            messages.ScanQueueModificationMessage(scan_id=scan_id, action="continue", parameter={}),
         )
 
     def request_queue_reset(self):
         """request a scan queue reset"""
         logger.info("Requesting a queue reset")
-        self.producer.send(
+        self.connector.send(
             MessageEndpoints.scan_queue_modification_request(),
-            messages.ScanQueueModificationMessage(scanID=None, action="clear", parameter={}),
+            messages.ScanQueueModificationMessage(scan_id=None, action="clear", parameter={}),
         )
 
-    def request_scan_restart(self, scanID=None, requestID=None, replace=True) -> str:
+    def request_scan_restart(self, scan_id=None, requestID=None, replace=True) -> str:
         """request to restart a scan"""
-        if scanID is None:
-            scanID = self.scan_storage.current_scanID
+        if scan_id is None:
+            scan_id = self.scan_storage.current_scan_id
         if requestID is None:
             requestID = str(uuid.uuid4())
         logger.info("Requesting to abort and repeat a scan")
         position = "replace" if replace else "append"
 
-        self.producer.send(
+        self.connector.send(
             MessageEndpoints.scan_queue_modification_request(),
             messages.ScanQueueModificationMessage(
-                scanID=scanID, action="restart", parameter={"position": position, "RID": requestID}
+                scan_id=scan_id,
+                action="restart",
+                parameter={"position": position, "RID": requestID},
             ),
         )
         return requestID
 
     @property
     def next_scan_number(self):
         """get the next scan number from redis"""
-        num = self.producer.get(MessageEndpoints.scan_number())
-        if num is None:
+        msg = self.connector.get(MessageEndpoints.scan_number())
+        if msg is None:
             logger.warning("Failed to retrieve scan number from redis.")
             return -1
-        return int(num)
+        if not isinstance(msg, messages.VariableMessage):
+            # this is a temporary fix for providing backwards compatibility
+            return int(msg)
+        return int(msg.value)
 
     @next_scan_number.setter
     @typechecked
     def next_scan_number(self, val: int):
         """set the next scan number in redis"""
-        return self.producer.set(MessageEndpoints.scan_number(), val)
+        msg = messages.VariableMessage(value=val)
+        return self.connector.set(MessageEndpoints.scan_number(), msg)
 
     @property
     def next_dataset_number(self):
         """get the next dataset number from redis"""
-        return int(self.producer.get(MessageEndpoints.dataset_number()))
+        msg = self.connector.get(MessageEndpoints.dataset_number())
+        if msg is None:
+            logger.warning("Failed to retrieve dataset number from redis.")
+            return -1
+        if not isinstance(msg, messages.VariableMessage):
+            # this is a temporary fix for providing backwards compatibility
+            return int(msg)
+        return int(msg.value)
 
     @next_dataset_number.setter
     @typechecked
     def next_dataset_number(self, val: int):
         """set the next dataset number in redis"""
-        return self.producer.set(MessageEndpoints.dataset_number(), val)
+        msg = messages.VariableMessage(value=val)
+        return self.connector.set(MessageEndpoints.dataset_number(), msg)
 
-    @staticmethod
-    def _scan_queue_status_callback(msg, *, parent: ScanManager, **_kwargs) -> None:
+    def _scan_queue_status_callback(self, msg, **_kwargs) -> None:
         queue_status = msg.value
         if not queue_status:
             return
-        parent.update_with_queue_status(queue_status)
+        self.update_with_queue_status(queue_status)
 
-    @staticmethod
-    def _scan_queue_request_callback(msg, *, parent: ScanManager, **_kwargs) -> None:
+    def _scan_queue_request_callback(self, msg, **_kwargs) -> None:
         request = msg.value
-        parent.request_storage.update_with_request(request)
+        self.request_storage.update_with_request(request)
 
-    @staticmethod
-    def _scan_queue_request_response_callback(msg, *, parent: ScanManager, **_kwargs) -> None:
+    def _scan_queue_request_response_callback(self, msg, **_kwargs) -> None:
         response = msg.value
         logger.debug(response)
-        parent.request_storage.update_with_response(response)
+        self.request_storage.update_with_response(response)
 
-    @staticmethod
-    def _scan_status_callback(msg, *, parent: ScanManager, **_kwargs) -> None:
+    def _scan_status_callback(self, msg, **_kwargs) -> None:
         scan = msg.value
-        parent.scan_storage.update_with_scan_status(scan)
+        self.scan_storage.update_with_scan_status(scan)
 
-    @staticmethod
-    def _scan_segment_callback(msg, *, parent: ScanManager, **_kwargs) -> None:
+    def _scan_segment_callback(self, msg, **_kwargs) -> None:
         scan_msgs = msg.value
         if not isinstance(scan_msgs, list):
             scan_msgs = [scan_msgs]
         for scan_msg in scan_msgs:
-            parent.scan_storage.add_scan_segment(scan_msg)
+            self.scan_storage.add_scan_segment(scan_msg)
 
-    @staticmethod
-    def _baseline_callback(msg, *, parent: ScanManager, **_kwargs) -> None:
+    def _baseline_callback(self, msg, **_kwargs) -> None:
         msg = msg.value
-        parent.scan_storage.add_scan_baseline(msg)
+        self.scan_storage.add_scan_baseline(msg)
 
     def __str__(self) -> str:
-        return "\n".join(self.queue_storage.describe_queue())
+        try:
+            return "\n".join(self.queue_storage.describe_queue())
+        except Exception:
+            # queue_storage.describe_queue() can fail,
+            # for example if there is no current scan queue (None)
+            return super().__str__()
 
     def shutdown(self):
-        """stop the scan manager's threads"""
-        self._scan_queue_consumer.shutdown()
-        self._scan_queue_request_consumer.shutdown()
-        self._scan_queue_request_response_consumer.shutdown()
-        self._scan_status_consumer.shutdown()
-        self._scan_segment_consumer.shutdown()
-        self._baseline_consumer.shutdown()
+        pass
```

### Comparing `bec_lib-1.9.0/bec_lib/scan_report.py` & `bec_lib-2.0.1/bec_lib/scan_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+Scan Report class that provides a convenient way to access the status of a scan request. It is typically
+the return value of a scan request. 
+"""
+
 from __future__ import annotations
 
 import time
 from math import inf
 from typing import TYPE_CHECKING
 
 from bec_lib import messages
@@ -85,16 +90,16 @@
             if elapsed_time > timeout:
                 raise TimeoutError
         return queue_item
 
     def _get_mv_status(self) -> bool:
         """get the status of a move request"""
         motors = list(self.request.request.content["parameter"]["args"].keys())
-        request_status = self._client.device_manager.producer.lrange(
-            MessageEndpoints.device_req_status(self.request.requestID), 0, -1
+        request_status = self._client.device_manager.connector.lrange(
+            MessageEndpoints.device_req_status_container(self.request.requestID), 0, -1
         )
         if len(request_status) == len(motors):
             return True
         return False
 
     def wait(self, timeout: float = None) -> ScanReport:
         """
```

### Comparing `bec_lib-1.9.0/bec_lib/scans.py` & `bec_lib-2.0.1/bec_lib/scans.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+"""
+This module contains the Scans class and related classes for defining and running scans in BEC 
+from the client side.
+"""
+
 from __future__ import annotations
 
 import builtins
 import uuid
 from collections.abc import Callable
 from contextlib import ContextDecorator
+from copy import deepcopy
 from typing import TYPE_CHECKING
 
 from toolz import partition
 from typeguard import typechecked
 
 from bec_lib import messages
 from bec_lib.device import DeviceBase
@@ -42,29 +48,40 @@
         scans = self.client.scans
 
         # handle reserved kwargs:
         hide_report_kwarg = kwargs.get("hide_report", False)
         # pylint: disable=protected-access
         hide_report = hide_report_kwarg or scans._hide_report
 
-        metadata = self.client.metadata.copy()
-        if not "sample_name" in metadata:
+        metadata = deepcopy(self.client.metadata)
+        if "sample_name" not in metadata:
             sample_name = self.client.get_global_var("sample_name")
             if sample_name is not None:
                 metadata["sample_name"] = sample_name
 
+        file_writer_data = deepcopy(self.client.file_writer_data)
+
         if "md" in kwargs:
             metadata.update(kwargs["md"])
 
         if "file_suffix" in kwargs:
-            # ensure that file_suffix is only containing alphanumeric characters
             suffix = kwargs.pop("file_suffix")
-            if not suffix.isalnum() or not suffix.isascii():
+            # to check if suffix is alphanumeric and ascii, however we allow in addition - and _
+            check_suffix = suffix.replace("_", "").replace("-", "")
+            if not check_suffix.isalnum() or not check_suffix.isascii():
+                raise ValueError("file_suffix must only contain alphanumeric ASCII characters.")
+            file_writer_data["file_suffix"] = suffix
+        if "file_directory" in kwargs:
+            directory = kwargs.pop("file_directory")
+            check_directory = directory.replace("/", "").replace("_", "").replace("-", "")
+            if not check_directory.isalnum() or not check_directory.isascii():
                 raise ValueError("file_suffix must only contain alphanumeric ASCII characters.")
-            metadata["file_suffix"] = suffix
+            file_writer_data["file_directory"] = directory.strip("/")
+
+        metadata["file_writer_data"] = file_writer_data
 
         # pylint: disable=protected-access
         if scans._scan_group:
             metadata["queue_group"] = scans._scan_group
         if scans._scan_def_id:
             metadata["scan_def_id"] = scans._scan_def_id
         if scans._dataset_id_on_hold:
@@ -96,29 +113,29 @@
 
     def _get_scan_report_type(self, hide_report) -> str:
         """get the scan report type"""
         if hide_report:
             return None
         return self.scan_info.get("scan_report_hint")
 
-    def _start_consumer(self, request: messages.ScanQueueMessage) -> ConsumerConnector:
-        """Start a consumer for the given request"""
-        consumer = self.client.device_manager.connector.consumer(
+    def _start_register(self, request: messages.ScanQueueMessage) -> ConsumerConnector:
+        """Start a register for the given request"""
+        register = self.client.device_manager.connector.register(
             [
                 MessageEndpoints.device_readback(dev)
                 for dev in request.content["parameter"]["args"].keys()
             ],
             threaded=False,
             cb=(lambda msg: msg),
         )
-        return consumer
+        return register
 
     def _send_scan_request(self, request: messages.ScanQueueMessage) -> None:
         """Send a scan request to the scan server"""
-        self.client.device_manager.producer.send(MessageEndpoints.scan_queue_request(), request)
+        self.client.device_manager.connector.send(MessageEndpoints.scan_queue_request(), request)
 
 
 class Scans:
     """Scans is a class for available scans in BEC"""
 
     def __init__(self, parent):
         self.parent = parent
@@ -132,15 +149,15 @@
         self._hide_report_ctx = HideReport(parent=self)
         self._dataset_id_on_hold = None
         self._dataset_id_on_hold_ctx = DatasetIdOnHold(parent=self)
         self._scan_export = None
 
     def _import_scans(self):
         """Import scans from the scan server"""
-        available_scans = self.parent.producer.get(MessageEndpoints.available_scans())
+        available_scans = self.parent.connector.get(MessageEndpoints.available_scans())
         if available_scans is None:
             logger.warning("No scans available. Are redis and the BEC server running?")
             return
         for scan_name, scan_info in available_scans.resource.items():
             self._available_scans[scan_name] = ScanObject(scan_name, scan_info, client=self.parent)
             setattr(self, scan_name, self._available_scans[scan_name].run)
             setattr(getattr(self, scan_name), "__doc__", scan_info.get("doc"))
@@ -182,15 +199,15 @@
 
         Raises:
             TypeError: Raised if not all required keyword arguments have been specified.
             TypeError: Raised if the number of args do fit into the required bundling pattern.
             TypeError: Raised if an argument is not of the required type as specified in scan_info.
 
         Returns:
-            messages.ScanQueueMessage: _description_
+            messages.ScanQueueMessage: scan request message
         """
         arg_input = list(scan_info.get("arg_input", {}).values())
 
         arg_bundle_size = scan_info.get("arg_bundle_size", {})
         bundle_size = arg_bundle_size.get("bundle")
         if len(arg_input) > 0:
             if len(args) % len(arg_input) != 0:
@@ -199,14 +216,25 @@
                     f" {len(arg_input)} arguments ({len(args)} given)."
                 )
             if not all(req_kwarg in kwargs for req_kwarg in scan_info.get("required_kwargs")):
                 raise TypeError(
                     f"{scan_info.get('doc')}\n Not all required keyword arguments have been"
                     f" specified. The required arguments are: {scan_info.get('required_kwargs')}"
                 )
+            # check that all specified devices in args are different objects
+            for arg in args:
+                if not isinstance(arg, DeviceBase):
+                    continue
+                if args.count(arg) > 1:
+                    raise TypeError(
+                        f"{scan_info.get('doc')}\n All specified devices must be different"
+                        f" objects."
+                    )
+
+            # check that all arguments are of the correct type
             for ii, arg in enumerate(args):
                 if not isinstance(arg, Scans.get_arg_type(arg_input[ii % len(arg_input)])):
                     raise TypeError(
                         f"{scan_info.get('doc')}\n Argument {ii} must be of type"
                         f" {arg_input[ii%len(arg_input)]}, not {type(arg).__name__}."
                     )
 
@@ -348,35 +376,65 @@
         if self._call_count:
             return
         self.parent._dataset_id_on_hold = None
         queue = self.parent.parent.queue
         queue.next_dataset_number += 1
 
 
+class FileWriterData:
+    @typechecked
+    def __init__(self, file_writer_data: dict) -> None:
+        """Context manager for updating metadata
+
+        Args:
+            metadata (dict): Metadata dictionary
+        """
+        self.client = self._get_client()
+        self._file_writer_data = file_writer_data
+        self._orig_file_writer_data = None
+
+    def _get_client(self):
+        """Get BEC client"""
+        return builtins.__dict__["bec"]
+
+    def __enter__(self):
+        """Enter the context manager"""
+        self._orig_file_writer_data = deepcopy(self.client.file_writer_data)
+        self.client.file_writer_data.update(self._file_writer_data)
+        return self
+
+    def exit(self, *exc):
+        """Exit the context manager"""
+        self.client.file_writer_data = self._orig_file_writer_data
+
+
 class Metadata:
     @typechecked
     def __init__(self, metadata: dict) -> None:
         """Context manager for updating metadata
 
         Args:
             metadata (dict): Metadata dictionary
         """
         self.client = self._get_client()
         self._metadata = metadata
         self._orig_metadata = None
 
     def _get_client(self):
+        """Get BEC client"""
         return builtins.__dict__["bec"]
 
     def __enter__(self):
-        self._orig_metadata = self.client.metadata.copy()
+        """Enter the context manager"""
+        self._orig_metadata = deepcopy(self.client.metadata)
         self.client.metadata.update(self._metadata)
         return self
 
     def __exit__(self, *exc):
+        """Exit the context manager"""
         self.client.metadata = self._orig_metadata
 
 
 class ScanExport:
     def __init__(self, output_file: str) -> None:
         """Context manager for exporting scans
 
@@ -412,9 +470,9 @@
         try:
             for scan in self.scans:
                 scan.wait()
         finally:
             try:
                 self._export_to_csv()
                 self.scans = None
-            except:
-                logger.warning("Could not export scans to csv file.")
+            except Exception as exc:
+                logger.warning(f"Could not export scans to csv file, due to exception {exc}")
```

### Comparing `bec_lib-1.9.0/bec_lib/scibec_validator.py` & `bec_lib-2.0.1/bec_lib/scibec_validator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This module provides a class to validate the device configuration against the openapi schema of SciBec.
+"""
+
 import json
 import os
 
 import fastjsonschema
 
 import bec_lib
```

### Comparing `bec_lib-1.9.0/bec_lib/serialization.py` & `bec_lib-2.0.1/bec_lib/serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Serialization module for BEC messages
+"""
+
 from __future__ import annotations
 
 import contextlib
 import gc
 import inspect
 import json
 from abc import abstractmethod
@@ -48,16 +52,15 @@
         msg_body = msgpack.loads(body)
         msg_class = get_message_class(header.pop("msg_type"))
         msg = msg_class(**header, **msg_body)
     except Exception as exception:
         raise RuntimeError("Failed to decode BECMessage") from exception
 
     # shouldn't this be checked when the msg is used? or when the message is created?
-    if msg._is_valid():
-        return msg
+    return msg
 
 
 def encode_bec_status(status):
     if not isinstance(status, BECStatus):
         return status
     return status.value.to_bytes(1, "big")  # int.to_bytes
```

### Comparing `bec_lib-1.9.0/bec_lib/service_config.py` & `bec_lib-2.0.1/bec_lib/service_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,39 @@
+"""
+This module provides a class to handle the service configuration.
+"""
+
 import json
 import os
+from pathlib import Path
 
 import yaml
 
 from bec_lib.logger import bec_logger
 
 try:
     from bec_plugins.utils import load_service_config as plugin_load_service_config
 except ImportError:
     plugin_load_service_config = None
 
 logger = bec_logger.logger
 
+DEFAULT_BASE_PATH = (
+    str(Path(__file__).resolve().parent.parent.parent) if "site-packages" not in __file__ else "./"
+)
+
 DEFAULT_SERVICE_CONFIG = {
-    "redis": {"host": "localhost", "port": 6379},
-    "service_config": {"file_writer": {"plugin": "default_NeXus_format", "base_path": "./"}},
+    "redis": {"host": os.environ.get("BEC_REDIS_HOST", "localhost"), "port": 6379},
+    "service_config": {
+        "file_writer": {
+            "plugin": "default_NeXus_format",
+            "base_path": DEFAULT_BASE_PATH,
+        },
+        "log_writer": {"base_path": DEFAULT_BASE_PATH},
+    },
 }
 
 
 class ServiceConfig:
     def __init__(
         self, config_path: str = None, redis: dict = None, config: dict = None, **kwargs
     ) -> None:
@@ -28,15 +43,15 @@
         if self.config:
             self._load_urls("redis", required=True)
             self._load_urls("mongodb", required=False)
 
         self._update_config(service_config=config, redis=redis)
 
         self.service_config = self.config.get(
-            "service_config", {"file_writer": {"plugin": "default_NeXus_format", "base_path": "./"}}
+            "service_config", DEFAULT_SERVICE_CONFIG["service_config"]
         )
 
     def _update_config(self, **kwargs):
         for key, val in kwargs.items():
             if not val:
                 continue
             self.config[key] = val
```

### Comparing `bec_lib-1.9.0/bec_lib/signature_serializer.py` & `bec_lib-2.0.1/bec_lib/signature_serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This module contains functions to serialize and deserialize function signatures.
+"""
+
 from __future__ import annotations
 
 import ast
 import builtins
 import inspect
 import operator
 import sys
```

### Comparing `bec_lib-1.9.0/bec_lib/tests/test_config.yaml` & `bec_lib-2.0.1/bec_lib/configs/demo_config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -18,279 +18,281 @@
 dyn_signals:
   readoutPriority: baseline
   deviceClass: sim:sim:SynDynamicComponents
   deviceConfig:
   enabled: true
   readOnly: false
 
+pseudo_signal1:
+  deviceClass: ComputedSignal
+  deviceConfig:
+    compute_method: "def compute_signals(signal1, signal2):\n    return signal1.get()*signal2.get()\n"
+    input_signals: 
+      - "bpm4i_readback"
+      - "bpm5i_readback"
+  enabled: true
+  readOnly: false
+  readoutPriority: baseline
+
 ############################################################
 ####################### User motors ########################
 ############################################################
 
+hexapod:
+  readoutPriority: baseline
+  deviceClass: SynDeviceOPAAS
+  deviceConfig:
+  deviceTags:
+    - user motors
+  enabled: true
+  readOnly: false
+
 eyefoc:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 eyex:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 eyey:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 flyer_sim:
   readoutPriority: on_request
   deviceClass: SynFlyer
   deviceConfig:
     delay: 1    
     device_access: true
-    speed: 100
     update_frequency: 400
   deviceTags:
     - flyer
   enabled: true
   readOnly: false
 hrox:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hroy:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hroz:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hy:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hz:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 mbsx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 mbsy:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 pinx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 piny:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 pinz:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 samx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 samy:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 samz:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
-    speed: 100
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 
@@ -676,1566 +678,1424 @@
 ############################################################
 
 aptrx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 aptry:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bim2x:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bim2y:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm1trx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm1try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm2trx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm2try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm3trx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm3try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm4trx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm4try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm5trx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm5try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm6trx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm6try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4r:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5r:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bs1x:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bs1y:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bs2x:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bs2y:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 burstn:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 burstr:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1a:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1b:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1c:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1d:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1e:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1f:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1g:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1h:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dettrx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 di2trx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 di2try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dtpush:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dtth:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dttrx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dttry:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dttrz:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebcsx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebcsy:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfi1:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfi2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfi3:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfi4:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfzpx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfzpy:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebtrx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebtry:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebtrz:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fi1try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fi2try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fi3try:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fsh1x:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fsh2x:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ftrans:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttrx1:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttrx2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttry1:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttry2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttrz:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 idgap:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mibd:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mibd1:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mibd2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 miroll:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mith:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitrx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitry:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitry1:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitry2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitry3:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobd:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobdai:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobdbo:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobdco:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobddi:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mokev:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mopush1:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mopush2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moroll1:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moroll2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moth1:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moth1e:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moth2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moth2e:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motrx2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motry:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motry2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motrz1:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motrz1e:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moyaw2:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl0ch:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl0trxi:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl0trxo:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl0wh:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1ch:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1cv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1trxi:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1trxo:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1tryb:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1tryt:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1wh:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1wv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2ch:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2cv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2trxi:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2trxo:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2tryb:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2tryt:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2wh:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2wv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3ch:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3cv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3trxi:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3trxo:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3tryb:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3tryt:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3wh:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3wv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4ch:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4cv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4trxi:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4trxo:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4tryb:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4tryt:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4wh:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4wv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5ch:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5cv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5trxi:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5trxo:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5tryb:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5tryt:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5wh:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5wv:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 strox:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 stroy:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 stroz:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sttrx:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sttry:
   readoutPriority: baseline
   deviceClass: SimPositioner
   deviceConfig:
     delay: 1
-    speed: 100
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 
 ################# Beamline motors end here #################
@@ -2250,84 +2110,7 @@
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ################ Read-only signals end here ################
 
-
-############################################################
-##################### Disabled devices #####################
-############################################################
-
-motor1_disabled:
-  readoutPriority: baseline
-  deviceClass: SimPositioner
-  deviceConfig:
-    delay: 1
-    labels: motor1_disabled
-    limits:
-    - -50
-    - 50
-    name: motor1_disabled
-    speed: 100
-    tolerance: 0.01
-    update_frequency: 400
-  deviceTags:
-  - user motors
-  enabled: false
-  readOnly: false
-motor1_disabled_set:
-  readoutPriority: baseline
-  deviceClass: SimPositioner
-  deviceConfig:
-    delay: 1
-    labels: motor1_disabled_set
-    limits:
-    - -50
-    - 50
-    name: motor1_disabled_set
-    speed: 100
-    tolerance: 0.01
-    update_frequency: 400
-  deviceTags:
-  - user motors
-  enabled: true
-  readOnly: true
-motor2_disabled:
-  readoutPriority: baseline
-  deviceClass: SimPositioner
-  deviceConfig:
-    delay: 1
-    labels: motor2_disabled
-    limits:
-    - -50
-    - 50
-    name: motor2_disabled
-    speed: 100
-    tolerance: 0.01
-    update_frequency: 400
-  deviceTags:
-  - user motors
-  enabled: false
-  readOnly: false
-motor2_disabled_set:
-  readoutPriority: baseline
-  deviceClass: SimPositioner
-  deviceConfig:
-    delay: 1
-    labels: motor2_disabled_set
-    limits:
-    - -50
-    - 50
-    name: motor2_disabled_set
-    speed: 100
-    tolerance: 0.01
-    update_frequency: 400
-  deviceTags:
-  - user motors
-  enabled: true
-  readOnly: true
-
-
-################ Disabled devices end here #################
-
```

### Comparing `bec_lib-1.9.0/bec_lib/tests/utils.py` & `bec_lib-2.0.1/bec_lib/tests/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,66 +1,49 @@
 from __future__ import annotations
 
 import builtins
+import functools
 import os
 import time
 import uuid
 from typing import TYPE_CHECKING
-from unittest import mock
 
-import bec_lib
-import pytest
 import yaml
+
+import bec_lib
 from bec_lib import BECClient, messages
 from bec_lib.connector import ConnectorBase
 from bec_lib.devicemanager import DeviceManagerBase
-from bec_lib.endpoints import MessageEndpoints
+from bec_lib.endpoints import EndpointInfo, MessageEndpoints
 from bec_lib.logger import bec_logger
 from bec_lib.scans import Scans
-from bec_lib.service_config import ServiceConfig
 
 if TYPE_CHECKING:
     from bec_lib.alarm_handler import Alarms
 
 dir_path = os.path.dirname(bec_lib.__file__)
 
 logger = bec_logger.logger
 
 # pylint: disable=no-member
 # pylint: disable=missing-function-docstring
 # pylint: disable=redefined-outer-name
 # pylint: disable=protected-access
 
 
-@pytest.fixture
-def dm():
-    service_mock = mock.MagicMock()
-    service_mock.connector = ConnectorMock("")
-    dev_manager = DMClientMock(service_mock)
-    yield dev_manager
-
-
-@pytest.fixture
-def dm_with_devices(dm):
-    with open(f"{dir_path}/tests/test_config.yaml", "r") as f:
-        dm._session = create_session_from_config(yaml.safe_load(f))
-    dm._load_session()
-    yield dm
-
-
 def queue_is_empty(queue) -> bool:  # pragma: no cover
     if not queue:
         return True
     if not queue["primary"].get("info"):
         return True
     return False
 
 
 def get_queue(bec):  # pragma: no cover
-    return bec.queue.producer.get(MessageEndpoints.scan_queue_status())
+    return bec.queue.connector.get(MessageEndpoints.scan_queue_status())
 
 
 def wait_for_empty_queue(bec):  # pragma: no cover
     while not get_queue(bec):
         time.sleep(1)
     while not queue_is_empty(get_queue(bec).content["queue"]):
         time.sleep(1)
@@ -88,17 +71,16 @@
 
 
 class ClientMock(BECClient):
     def _load_scans(self):
         self.scans = ScansMock(self)
         builtins.scans = self.scans
 
-    def start(self):
-        self._start_scan_queue()
-        self._start_alarm_handler()
+    # def _start_services(self):
+    #     pass
 
     def _start_metrics_emitter(self):
         pass
 
     def _start_update_service_info(self):
         pass
 
@@ -468,108 +450,89 @@
 
     def get_device(self, device_name):
         for dev in self._session["devices"]:
             if dev["name"] == device_name:
                 return dev
 
 
-@pytest.fixture()
-def bec_client():
-    client = ClientMock()
-    client.initialize(
-        ServiceConfig(redis={"host": "host", "port": 123}, scibec={"host": "host", "port": 123}),
-        ConnectorMock,
-    )
-    device_manager = DMClientMock(client)
-    if "test_session" not in builtins.__dict__:
-        with open(f"{dir_path}/tests/test_config.yaml", "r", encoding="utf-8") as f:
-            builtins.__dict__["test_session"] = create_session_from_config(yaml.safe_load(f))
-    device_manager._session = builtins.__dict__["test_session"]
-    device_manager.producer = device_manager.connector.producer()
-    client.wait_for_service = lambda service_name: None
-    device_manager._load_session(idle_time=0)
-    for name, dev in device_manager.devices.items():
-        dev._info["hints"] = {"fields": [name]}
-    client.device_manager = device_manager
-    yield client
-    ClientMock._client = None
-    device_manager.devices.flush()
-
-
 class PipelineMock:  # pragma: no cover
     _pipe_buffer = []
-    _producer = None
+    _connector = None
 
-    def __init__(self, producer) -> None:
-        self._producer = producer
+    def __init__(self, connector) -> None:
+        self._connector = connector
 
     def execute(self):
-        if not self._producer.store_data:
+        if not self._connector.store_data:
             self._pipe_buffer = []
             return []
         res = [
-            getattr(self._producer, method)(*args, **kwargs)
+            getattr(self._connector, method)(*args, **kwargs)
             for method, args, kwargs in self._pipe_buffer
         ]
         self._pipe_buffer = []
         return res
 
 
-class ConsumerMock:  # pragma: no cover
-    def __init__(self) -> None:
-        self.signal_event = SignalMock()
-
-    def start(self):
-        pass
-
-    def join(self):
-        pass
-
-    def shutdown(self):
-        pass
-
-
 class SignalMock:  # pragma: no cover
     def __init__(self) -> None:
         self.is_set = False
 
     def set(self):
         self.is_set = True
 
 
-class ProducerMock:  # pragma: no cover
-    def __init__(self, store_data=True) -> None:
+class ConnectorMock(ConnectorBase):  # pragma: no cover
+    def __init__(self, bootstrap_server="localhost:0000", store_data=True):
+        super().__init__(bootstrap_server)
         self.message_sent = []
         self._get_buffer = {}
         self.store_data = store_data
 
+    def raise_alarm(
+        self, severity: Alarms, alarm_type: str, source: str, msg: dict, metadata: dict
+    ):
+        pass
+
+    def log_error(self, *args, **kwargs):
+        pass
+
+    def shutdown(self):
+        pass
+
+    def register(self, *args, **kwargs):
+        pass
+
+    def keys(self, *args, **kwargs):
+        return []
+
     def set(self, topic, msg, pipe=None, expire: int = None):
         if pipe:
-            pipe._pipe_buffer.append(("set", (topic, msg), {"expire": expire}))
+            pipe._pipe_buffer.append(("set", (topic.endpoint, msg), {"expire": expire}))
             return
         self.message_sent.append({"queue": topic, "msg": msg, "expire": expire})
 
     def raw_send(self, topic, msg, pipe=None):
         if pipe:
-            pipe._pipe_buffer.append(("send", (topic, msg), {}))
+            pipe._pipe_buffer.append(("send", (topic.endpoint, msg), {}))
             return
         self.message_sent.append({"queue": topic, "msg": msg})
 
     def send(self, topic, msg, pipe=None):
         if not isinstance(msg, messages.BECMessage):
             raise TypeError("Message must be a BECMessage")
         return self.raw_send(topic, msg, pipe)
 
     def set_and_publish(self, topic, msg, pipe=None, expire: int = None):
         if pipe:
-            pipe._pipe_buffer.append(("set_and_publish", (topic, msg), {"expire": expire}))
+            pipe._pipe_buffer.append(("set_and_publish", (topic.endpoint, msg), {"expire": expire}))
             return
         self.message_sent.append({"queue": topic, "msg": msg, "expire": expire})
 
-    def lpush(self, topic, msg, pipe=None):
+    def lpush(self, topic, msg, pipe=None, max_size=None):
         if pipe:
             pipe._pipe_buffer.append(("lpush", (topic, msg), {}))
             return
 
     def rpush(self, topic, msg, pipe=None):
         if pipe:
             pipe._pipe_buffer.append(("rpush", (topic, msg), {}))
@@ -579,61 +542,63 @@
     def lrange(self, topic, start, stop, pipe=None):
         if pipe:
             pipe._pipe_buffer.append(("lrange", (topic, start, stop), {}))
             return
         return []
 
     def get(self, topic, pipe=None):
+        if isinstance(topic, EndpointInfo):
+            topic = topic.endpoint
         if pipe:
             pipe._pipe_buffer.append(("get", (topic,), {}))
             return
         val = self._get_buffer.get(topic)
         if isinstance(val, list):
             return val.pop(0)
         self._get_buffer.pop(topic, None)
         return val
 
-    def keys(self, pattern: str) -> list:
-        return []
-
     def pipeline(self):
         return PipelineMock(self)
 
     def delete(self, topic, pipe=None):
         if pipe:
             pipe._pipe_buffer.append(("delete", (topic,), {}))
             return
 
     def lset(self, topic: str, index: int, msgs: str, pipe=None) -> None:
         if pipe:
             pipe._pipe_buffer.append(("lrange", (topic, index, msgs), {}))
             return
 
+    def producer(self):
+        return self
 
-class ConnectorMock(ConnectorBase):  # pragma: no cover
-    def __init__(self, bootstrap_server: list, store_data=True):
-        super().__init__(bootstrap_server)
-        self.store_data = store_data
-
-    def consumer(self, *args, **kwargs) -> ConsumerMock:
-        return ConsumerMock()
+    def execute_pipeline(self, pipeline):
+        pipeline.execute()
 
-    def producer(self, *args, **kwargs):
-        return ProducerMock(self.store_data)
-
-    def raise_alarm(
-        self, severity: Alarms, alarm_type: str, source: str, msg: dict, metadata: dict
-    ):
+    def xadd(self, topic, msg_dict, max_size=None, pipe=None, expire: int = None):
+        if pipe:
+            pipe._pipe_buffer.append(("xadd", (topic, msg_dict), {"expire": expire}))
+            return
         pass
 
-    def log_error(self, *args, **kwargs):
-        pass
+    def xread(self, topic, id=None, count=None, block=None, pipe=None, from_start=False):
+        if pipe:
+            pipe._pipe_buffer.append(
+                ("xread", (topic, id, count, block), {"from_start": from_start})
+            )
+            return
+        return []
 
-    def shutdown(self):
-        pass
+    def xrange(self, topic, min="-", max="+", pipe=None):
+        if pipe:
+            pipe._pipe_buffer.append(("xrange", (topic, min, max), {}))
+            return
+        return []
 
 
 def create_session_from_config(config: dict) -> dict:
     device_configs = []
     session_id = str(uuid.uuid4())
     for name, conf in config.items():
         dev_conf = {
@@ -644,7 +609,13 @@
             "enabled": conf["enabled"],
             "read_only": conf["readOnly"],
         }
         dev_conf.update(conf)
         device_configs.append(dev_conf)
     session = {"accessGroups": "customer", "devices": device_configs}
     return session
+
+
+@functools.lru_cache
+def load_test_config():
+    with open(f"{dir_path}/tests/test_config.yaml", "r", encoding="utf-8") as f:
+        return create_session_from_config(yaml.safe_load(f))
```

### Comparing `bec_lib-1.9.0/bec_lib/user_scripts_mixin.py` & `bec_lib-2.0.1/bec_lib/user_scripts_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This module provides a mixin class for the BEC class that allows the user to load and unload scripts from the `scripts` directory.
+"""
+
 from __future__ import annotations
 
 import builtins
 import glob
 import importlib
 import inspect
 import os
@@ -79,15 +83,15 @@
             if name in self._scripts:
                 logger.warning(f"Conflicting definitions for {name}.")
             logger.info(f"Importing {name}")
             self._scripts[name] = {"cls": cls, "fname": file}
 
     def forget_user_script(self, name: str) -> None:
         """unload / remove a user scripts. The file will remain on disk."""
-        if not name in self._scripts:
+        if name not in self._scripts:
             logger.error(f"{name} is not a known user script.")
             return
         builtins.__dict__.pop(name)
         self._scripts.pop(name)
 
     def list_user_scripts(self):
         """display all currently loaded user functions"""
```

### Comparing `bec_lib-1.9.0/bec_lib/utils.py` & `bec_lib-2.0.1/bec_lib/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+"""
+Utility functions for the bec_lib package.
+"""
+
 from __future__ import annotations
 
 import csv
+import datetime
 import functools
 from collections import defaultdict
 from typing import TYPE_CHECKING
 
 from typeguard import typechecked
 
 if TYPE_CHECKING:
-    from bec_lib.scan_report import ScanReport
     from bec_lib.scan_items import ScanItem
+    from bec_lib.scan_report import ScanReport
 
 
 class user_access:
 
     def __init__(self, meth):
         """
         Decorator to mark <device_class> methods to be accessible from the bec client
@@ -80,15 +85,15 @@
     header_out = []
     body_out = []
     data_output = []
 
     for ii, scan_rep in enumerate(scan_report):
         if hasattr(scan_rep, "scan"):
             scan_rep = scan_rep.scan
-        header_out.append([f"#{ii}"])
+        header_out.append(["#ScanNumber", f"{scan_rep.scan_number}"])
         header_tmp, body_tmp = _extract_scan_data(
             scan_item=scan_rep, header=header, write_metadata=write_metadata
         )
         header_out.extend(header_tmp[:-1])
         body_out.extend(body_tmp)
     header_out.append(header_tmp[-1])  # To only append the header keys once
     data_output.extend(header_out)
@@ -126,17 +131,30 @@
         write_metadata (bool, optional): If True, the metadata of the scan will be written to the header of csv file. Defaults to True.
 
     Returns:
         (tuple): Tuple of header and body of the csv file.
     """
     scan_dict = scan_to_dict(scan_item, flat=True)
 
-    header_tmp = [["#" + entry.replace("\t", "")] for entry in str(scan_item).split("\n")]
-    header_tmp.insert(1, ["#ScanStatus", scan_item.status])
-    scan_metadata = scan_item.data.messages[list(scan_item.data.messages.keys())[-1]].metadata
+    header_tmp = []
+    header_tmp.append(["#scan_id", f"{scan_item.scan_id}"])
+    header_tmp.append(["#ScanStatus", f"{scan_item.status}"])
+
+    start_time = f"{datetime.datetime.fromtimestamp(scan_item.start_time).strftime('%c')}"
+    header_tmp.append(["#StartTime", start_time])
+    end_time = f"{datetime.datetime.fromtimestamp(scan_item.start_time).strftime('%c')}"
+    header_tmp.append(["#EndTime", end_time])
+    elapsed_time = (
+        f"\tElapsed time: {(scan_item.end_time-scan_item.start_time):.1f} s\n"
+        if scan_item.end_time and scan_item.start_time
+        else ""
+    )
+    header_tmp.append(["#ElapsedTime", elapsed_time])
+
+    scan_metadata = scan_item.status_message.info
     if write_metadata:
         header_tmp.append(["#ScanMetadata"])
         for key, value in scan_metadata.items():
             header_tmp.append(["".join(["#", key]), value])
     if header:
         header_keys = header
     else:
```

### Comparing `bec_lib-1.9.0/bec_lib.egg-info/PKG-INFO` & `bec_lib-2.0.1/bec_lib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: bec-lib
-Version: 1.9.0
+Version: 2.0.1
 Summary: BEC library
 Home-page: https://gitlab.psi.ch/bec/bec
-License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # BEC Lib
 
 bec-lib is a Python library communicating with the [Beamline and Experiment Control (BEC)](https://gitlab.psi.ch/bec/bec) server. It is primarily used to build new BEC clients such as graphical user interfaces (GUIs) or command line interfaces (CLIs).
 
@@ -86,9 +84,7 @@
 
 
 Please make sure to update tests as necessary.
 
 ## License
 
 [BSD-3-Clause](https://choosealicense.com/licenses/bsd-3-clause/)
-
-
```

### Comparing `bec_lib-1.9.0/bec_lib.egg-info/SOURCES.txt` & `bec_lib-2.0.1/bec_lib.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 ./bec_lib/signature_serializer.py
 ./bec_lib/user_scripts_mixin.py
 ./bec_lib/utils.py
 ./bec_lib/configs/__init__.py
 ./bec_lib/configs/demo_config.yaml
 ./bec_lib/configs/openapi_schema.json
 ./bec_lib/tests/__init__.py
+./bec_lib/tests/end2end_fixtures.py
+./bec_lib/tests/fixtures.py
 ./bec_lib/tests/test_config.yaml
 ./bec_lib/tests/test_service_config.yaml
 ./bec_lib/tests/utils.py
 bec_lib.egg-info/PKG-INFO
 bec_lib.egg-info/SOURCES.txt
 bec_lib.egg-info/dependency_links.txt
 bec_lib.egg-info/entry_points.txt
```

