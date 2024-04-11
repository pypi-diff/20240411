# Comparing `tmp/bttc-0.0.73.8.tar.gz` & `tmp/bttc-0.0.73.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bttc-0.0.73.8.tar", last modified: Wed Apr 10 06:02:37 2024, max compression
+gzip compressed data, was "bttc-0.0.73.9.tar", last modified: Wed Apr 10 07:52:08 2024, max compression
```

## Comparing `bttc-0.0.73.8.tar` & `bttc-0.0.73.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.634044 bttc-0.0.73.8/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.73.8/LICENSE
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-10 06:02:37.634044 bttc-0.0.73.8/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1347 2024-04-08 13:33:17.000000 bttc-0.0.73.8/README.md
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.630044 bttc-0.0.73.8/bttc/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5005 2024-04-10 06:02:27.000000 bttc-0.0.73.8/bttc/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-09 04:28:05.000000 bttc-0.0.73.8/bttc/apk_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/ble_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.73.8/bttc/ble_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/bt_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    16265 2024-04-10 05:57:16.000000 bttc-0.0.73.8/bttc/bt_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.630044 bttc-0.0.73.8/bttc/cli/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.73.8/bttc/cli/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/cli/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    22454 2024-04-10 02:58:23.000000 bttc-0.0.73.8/bttc/cli/main.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/common_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3816 2024-04-08 13:33:17.000000 bttc-0.0.73.8/bttc/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    30210 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/general_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.630044 bttc-0.0.73.8/bttc/mobly_android_device_lib/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/mobly_android_device_lib/jsonrpc_client_base.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.630044 bttc-0.0.73.8/bttc/mobly_android_device_lib/services/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/mobly_android_device_lib/services/sl4a_client.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/mobly_android_device_lib/services/sl4a_service.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/mobly_android_device_lib/tl4a_snippet_client.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.626044 bttc-0.0.73.8/bttc/profiles/
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.630044 bttc-0.0.73.8/bttc/profiles/avrcp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/avrcp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/avrcp/avrcp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/avrcp/avrcp_target_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/avrcp/errors.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.630044 bttc-0.0.73.8/bttc/profiles/hfp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/hfp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/hfp/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/hfp/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/hfp/hfp_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/hfp/hfp_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/hfp/hfp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/profiles/hfp/hfp_strategy.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/strategy.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.634044 bttc-0.0.73.8/bttc/utils/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/utils/ad_checker.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3197 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/utils/device_factory.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.634044 bttc-0.0.73.8/bttc/utils/iperf/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/utils/iperf/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/utils/iperf/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4643 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/utils/key_events_handler.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/utils/log_parser.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/utils/logcat.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/utils/retry.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/utils/typing_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2915 2024-04-08 13:33:17.000000 bttc-0.0.73.8/bttc/utils_loader.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.73.8/bttc/wifi_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 06:02:37.630044 bttc-0.0.73.8/bttc.egg-info/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-10 06:02:37.000000 bttc-0.0.73.8/bttc.egg-info/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1284 2024-04-10 06:02:37.000000 bttc-0.0.73.8/bttc.egg-info/SOURCES.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-04-10 06:02:37.000000 bttc-0.0.73.8/bttc.egg-info/dependency_links.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-04-10 06:02:37.000000 bttc-0.0.73.8/bttc.egg-info/requires.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-04-10 06:02:37.000000 bttc-0.0.73.8/bttc.egg-info/top_level.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-04-10 06:02:37.634044 bttc-0.0.73.8/setup.cfg
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1714 2024-04-10 00:48:38.000000 bttc-0.0.73.8/setup.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.955250 bttc-0.0.73.9/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.73.9/LICENSE
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-10 07:52:08.955250 bttc-0.0.73.9/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1347 2024-04-08 13:33:17.000000 bttc-0.0.73.9/README.md
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.951250 bttc-0.0.73.9/bttc/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5315 2024-04-10 07:51:36.000000 bttc-0.0.73.9/bttc/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-09 04:28:05.000000 bttc-0.0.73.9/bttc/apk_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/ble_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.73.9/bttc/ble_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/bt_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    16265 2024-04-10 05:57:16.000000 bttc-0.0.73.9/bttc/bt_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.951250 bttc-0.0.73.9/bttc/cli/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.73.9/bttc/cli/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/cli/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    22487 2024-04-10 07:45:43.000000 bttc-0.0.73.9/bttc/cli/main.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/common_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3816 2024-04-08 13:33:17.000000 bttc-0.0.73.9/bttc/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    30210 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/general_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.951250 bttc-0.0.73.9/bttc/mobly_android_device_lib/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/mobly_android_device_lib/jsonrpc_client_base.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.951250 bttc-0.0.73.9/bttc/mobly_android_device_lib/services/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/mobly_android_device_lib/services/sl4a_client.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/mobly_android_device_lib/services/sl4a_service.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/mobly_android_device_lib/tl4a_snippet_client.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.947250 bttc-0.0.73.9/bttc/profiles/
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.951250 bttc-0.0.73.9/bttc/profiles/avrcp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/avrcp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/avrcp/avrcp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/avrcp/avrcp_target_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/avrcp/errors.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.955250 bttc-0.0.73.9/bttc/profiles/hfp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/hfp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/hfp/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/hfp/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/hfp/hfp_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/hfp/hfp_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/hfp/hfp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/hfp/hfp_strategy.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/strategy.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.955250 bttc-0.0.73.9/bttc/utils/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/utils/ad_checker.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3909 2024-04-10 07:48:22.000000 bttc-0.0.73.9/bttc/utils/device_factory.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.955250 bttc-0.0.73.9/bttc/utils/iperf/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/utils/iperf/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/utils/iperf/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4643 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/utils/key_events_handler.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/utils/log_parser.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/utils/logcat.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/utils/retry.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/utils/typing_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2915 2024-04-08 13:33:17.000000 bttc-0.0.73.9/bttc/utils_loader.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/wifi_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.951250 bttc-0.0.73.9/bttc.egg-info/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-10 07:52:08.000000 bttc-0.0.73.9/bttc.egg-info/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1284 2024-04-10 07:52:08.000000 bttc-0.0.73.9/bttc.egg-info/SOURCES.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-04-10 07:52:08.000000 bttc-0.0.73.9/bttc.egg-info/dependency_links.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-04-10 07:52:08.000000 bttc-0.0.73.9/bttc.egg-info/requires.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-04-10 07:52:08.000000 bttc-0.0.73.9/bttc.egg-info/top_level.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-04-10 07:52:08.955250 bttc-0.0.73.9/setup.cfg
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1714 2024-04-10 00:48:38.000000 bttc-0.0.73.9/setup.py
```

### Comparing `bttc-0.0.73.8/LICENSE` & `bttc-0.0.73.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/PKG-INFO` & `bttc-0.0.73.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.73.8
+Version: 0.0.73.9
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bttc-0.0.73.8/README.md` & `bttc-0.0.73.9/README.md`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/__init__.py` & `bttc-0.0.73.9/bttc/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,41 +24,43 @@
 from bttc import errors
 from bttc import utils_loader
 from bttc.utils import device_factory
 from ppadb import client
 from typing import TypeAlias
 
 
-__version__ = '0.0.73.8'
+__version__ = '0.0.73.9'
 __author__ = 'John Lee/Yuan Long Luo/Denny Chai'
 __credits__ = 'Google Pixel PQM'
 
 
 GeneralDevice: TypeAlias = android_device.AndroidDevice
 
 
 def get(
     serial_number: str | None = None,
     required_utility_names: set[str] | None = None,
     init_mbs: bool = False,
     init_sl4a: bool = False,
     init_snippet_uiautomator: bool = False,
-    init_tl4a: bool = False):
+    init_tl4a: bool = False,
+    depress_init_error: bool = False):
   """Retrieves an Android device instance based on the provided serial number.
 
   Args:
     serial_number: Serial number of the device to retrieve.
         If not provided, automatically selects the first available device.
     required_utility_names: Set of function module names to bind to the
         device.
     init_mbs: If True, initializes the MBS service on the device.
     init_sl4a: If True, initializes the SL4A service on the device.
     init_snippet_uiautomator: If True, initializes the Snippet UiAutomator
         service.
     init_tl4a: If True, initializes the TL4A service.
+    depress_init_error: True to ignore error caused by initialization.
 
 Returns:
     An initialized Android device instance.
 
 Raises:
     AdbDeviceError: If no devices are found, or multiple devices are found
         without providing a specific serial number.
@@ -85,54 +87,58 @@
   ]
   if not_supported_utility_names:
     raise errors.UnknownUtilityNameError(not_supported_utility_names)
 
   device = device_factory.get(
       serial_number, init_mbs=init_mbs, init_sl4a=init_sl4a,
       init_snippet_uiautomator=init_snippet_uiautomator,
-      init_tl4a=init_tl4a)
+      init_tl4a=init_tl4a,
+      depress_init_error=depress_init_error)
   atexit.register(device.services.stop_all)
   for module_name, module_info in func_module_info.items():
     if module_name in required_utility_names or module_info.auto_load:
       module_info.module.bind(device)
 
   return device
 
 
 def get_all(
     required_utility_names: set[str] | None = None,
     init_mbs: bool = False,
     init_sl4a: bool = False,
     init_snippet_uiautomator: bool = False,
-    init_tl4a: bool = False):
+    init_tl4a: bool = False,
+    depress_init_error: bool = False):
   """Retrieves instances of all connected Android devices.
 
   Args:
     required_utility_names: Set of function module names to bind to each
         device.
     init_mbs: If True, initializes the MBS service on each device.
     init_sl4a: If True, initializes the SL4A service on each device.
     init_snippet_uiautomator: If True, initializes the Snippet UiAutomator
         service.
     init_tl4a: If True, initializes the TL4A service.
+    depress_init_error: True to ignore error caused by initialization.
 
 Returns:
     A dictionary where keys are device serial numbers and values are initialized
     Device instances.
   """
   device_info = {}
   adb_client = client.Client(host='localhost', port=5037)
   for device in adb_client.devices():
     device_info[device.serial] = get(
         device.serial,
         required_utility_names=required_utility_names,
         init_mbs=init_mbs,
         init_sl4a=init_sl4a,
         init_snippet_uiautomator=init_snippet_uiautomator,
-        init_tl4a=init_tl4a)
+        init_tl4a=init_tl4a,
+        depress_init_error=depress_init_error)
 
   return device_info
 
 
 def list_utils(dut: GeneralDevice) -> list[core.UtilBase]:
   """Gets loaded utilities from the given DUT.
```

### Comparing `bttc-0.0.73.8/bttc/apk_utils.py` & `bttc-0.0.73.9/bttc/apk_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/ble_data.py` & `bttc-0.0.73.9/bttc/ble_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/ble_utils.py` & `bttc-0.0.73.9/bttc/ble_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/bt_data.py` & `bttc-0.0.73.9/bttc/bt_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/bt_utils.py` & `bttc-0.0.73.9/bttc/bt_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/cli/__init__.py` & `bttc-0.0.73.9/bttc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/cli/constants.py` & `bttc-0.0.73.9/bttc/cli/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/cli/main.py` & `bttc-0.0.73.9/bttc/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -486,15 +486,16 @@
   def dut(self) -> Any:
     return self._dut
 
   def _init_dut(self, serial: str):
     self._dut = bttc.get(
         serial,
         init_snippet_uiautomator=self.dut_init_snippet_uiautomator,
-        init_sl4a=self.dut_init_sl4a)
+        init_sl4a=self.dut_init_sl4a,
+        depress_init_error=True)
     self.prompt = BttcCmdApp.DEVICE_PROMPT_PROMPT.format(serial=serial)
 
   @dec_require_dut
   def do_device_time(self, args):
     self.poutput(f'{self._dut.gm.device_datetime}\n')
 
   @cmd2.with_argparser(load_cmd2_commandset_parser)
```

### Comparing `bttc-0.0.73.8/bttc/common_data.py` & `bttc-0.0.73.9/bttc/common_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/constants.py` & `bttc-0.0.73.9/bttc/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/core.py` & `bttc-0.0.73.9/bttc/core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/errors.py` & `bttc-0.0.73.9/bttc/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/general_utils.py` & `bttc-0.0.73.9/bttc/general_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/mobly_android_device_lib/jsonrpc_client_base.py` & `bttc-0.0.73.9/bttc/mobly_android_device_lib/jsonrpc_client_base.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/mobly_android_device_lib/services/sl4a_client.py` & `bttc-0.0.73.9/bttc/mobly_android_device_lib/services/sl4a_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/mobly_android_device_lib/services/sl4a_service.py` & `bttc-0.0.73.9/bttc/mobly_android_device_lib/services/sl4a_service.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/mobly_android_device_lib/tl4a_snippet_client.py` & `bttc-0.0.73.9/bttc/mobly_android_device_lib/tl4a_snippet_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/profiles/avrcp/__init__.py` & `bttc-0.0.73.9/bttc/profiles/avrcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/profiles/avrcp/avrcp_facade.py` & `bttc-0.0.73.9/bttc/profiles/avrcp/avrcp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/profiles/avrcp/avrcp_target_devices.py` & `bttc-0.0.73.9/bttc/profiles/avrcp/avrcp_target_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/profiles/avrcp/errors.py` & `bttc-0.0.73.9/bttc/profiles/avrcp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/profiles/hfp/__init__.py` & `bttc-0.0.73.9/bttc/profiles/hfp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/profiles/hfp/constants.py` & `bttc-0.0.73.9/bttc/profiles/hfp/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/profiles/hfp/errors.py` & `bttc-0.0.73.9/bttc/profiles/hfp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/profiles/hfp/hfp_data.py` & `bttc-0.0.73.9/bttc/profiles/hfp/hfp_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/profiles/hfp/hfp_devices.py` & `bttc-0.0.73.9/bttc/profiles/hfp/hfp_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/profiles/hfp/hfp_facade.py` & `bttc-0.0.73.9/bttc/profiles/hfp/hfp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/profiles/hfp/hfp_strategy.py` & `bttc-0.0.73.9/bttc/profiles/hfp/hfp_strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/strategy.py` & `bttc-0.0.73.9/bttc/strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/utils/ad_checker.py` & `bttc-0.0.73.9/bttc/utils/ad_checker.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/utils/device_factory.py` & `bttc-0.0.73.9/bttc/utils/device_factory.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,20 +16,35 @@
 import logging
 
 from mobly.controllers import android_device
 from bttc.mobly_android_device_lib import tl4a_snippet_client
 from bttc.mobly_android_device_lib.services import sl4a_service
 
 from snippet_uiautomator import uiautomator
-from typing import TypeAlias, Union
+from typing import Any, Callable, TypeAlias, Union
 
 
 GeneralDevice: TypeAlias = android_device.AndroidDevice
 
 
+def dec_depress_ex(do_depress: bool = False) -> Callable[Any, ...]:
+  def inner(func: Callable[Any, ...]) -> Callable[Any, ...]:
+    def wrapper(*args, **kwargs):
+      try:
+        func(*args, **kwargs)
+      except Exception as ex:
+        if do_depress:
+          logging.warning('%s', ex)
+        else:
+          raise ex
+    return wrapper
+
+  return inner
+
+
 def load_sl4a(device: GeneralDevice):
   """Loads SL4A service in given device."""
   if device.services.has_service_by_name('sl4a'):
     logging.info('SL4A is already loaded in device=%s!', device)
     return
 
   logging.info('Registering service "sl4a" in device=%s...', device)
@@ -37,63 +52,70 @@
 
 
 def get(
     ad: Union[GeneralDevice, str],
     init_mbs: bool = False,
     init_sl4a: bool = False,
     init_snippet_uiautomator: bool = False,
-    init_tl4a: bool = False) -> GeneralDevice:
+    init_tl4a: bool = False,
+    depress_init_error: bool = False) -> GeneralDevice:
   """Produces desired device.
 
   Args:
     init_mbs: True to register service `snippets` in provided device.
     init_sl4a: True to register service `sl4a` in provided device.
     init_snippet_uiautomator: True to register service `uiautomator` in provided
         device.
     init_tl4a: True to register service `tl4a` in provided device.
+    depress_init_error: True to ignore error caused by initialization.
 
   Returns:
     The produced device object.
   """
   device: GeneralDevice | None = None
   if isinstance(ad, str):
     device = android_device.create([{'serial': ad}])[0]
   else:
     device = ad
 
   if all([
       (init_mbs or init_snippet_uiautomator),
       'snippets' not in device.services.list_live_services()]):
     logging.info('Register service "mbs" in device=%s...', device)
-    device.load_snippet(
+    dec_depress_ex(depress_init_error)(
+        device.load_snippet)(
         'mbs',
         'com.google.android.mobly.snippet.bundled')
 
   if init_sl4a:
-    load_sl4a(device)
+    dec_depress_ex(depress_init_error)(
+        load_sl4a)(device)
 
   if init_tl4a:
-    tl4a_snippet_client.load_system_snippet(device)
+    dec_depress_ex(depress_init_error)(
+        tl4a_snippet_client.load_system_snippet)(device)
 
   if all([
       init_snippet_uiautomator,
       'uiautomator' not in device.services.list_live_services()]):
     if 'ui_dump' in device.services.list_live_services():
       device.log.info(
           '`ui_dump` is detected and it will conflict with snippet uiautomator!'
           ' Unloading it so to register snippet uiautomator next...')
       device.services.unregister('ui_dump')
 
-    device.services.register(
+    dec_depress_ex(depress_init_error)(
+        device.services.register)(
         'uiautomator', uiautomator.UiAutomatorService)
 
   if all([
       init_snippet_uiautomator,
       'uiautomator' not in device.services.list_live_services()]):
-    device.services.register(
+    dec_depress_ex(depress_init_error)(
+        device.services.register)(
         'uiautomator', uiautomator.UiAutomatorService)
 
   logging.info(
       '%s has registered service(s): %s',
       device, device.services.list_live_services())
 
   return device
```

### Comparing `bttc-0.0.73.8/bttc/utils/iperf/__init__.py` & `bttc-0.0.73.9/bttc/utils/iperf/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/utils/iperf/errors.py` & `bttc-0.0.73.9/bttc/utils/iperf/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/utils/key_events_handler.py` & `bttc-0.0.73.9/bttc/utils/key_events_handler.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/utils/log_parser.py` & `bttc-0.0.73.9/bttc/utils/log_parser.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/utils/logcat.py` & `bttc-0.0.73.9/bttc/utils/logcat.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/utils/retry.py` & `bttc-0.0.73.9/bttc/utils/retry.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/utils/typing_utils.py` & `bttc-0.0.73.9/bttc/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/utils_loader.py` & `bttc-0.0.73.9/bttc/utils_loader.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc/wifi_utils.py` & `bttc-0.0.73.9/bttc/wifi_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/bttc.egg-info/PKG-INFO` & `bttc-0.0.73.9/bttc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.73.8
+Version: 0.0.73.9
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bttc-0.0.73.8/bttc.egg-info/SOURCES.txt` & `bttc-0.0.73.9/bttc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.8/setup.py` & `bttc-0.0.73.9/setup.py`

 * *Files identical despite different names*

