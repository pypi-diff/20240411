# Comparing `tmp/rpcclient-4.6.0.tar.gz` & `tmp/rpcclient-4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpcclient-4.6.0.tar", last modified: Thu Apr  4 06:08:05 2024, max compression
+gzip compressed data, was "rpcclient-4.6.1.tar", last modified: Thu Apr 11 10:51:39 2024, max compression
```

## Comparing `rpcclient-4.6.0.tar` & `rpcclient-4.6.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.354661 rpcclient-4.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-04 06:07:41.000000 rpcclient-4.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-04 06:07:41.000000 rpcclient-4.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-04 06:07:41.000000 rpcclient-4.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-04 06:08:05.350661 rpcclient-4.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-04 06:07:41.000000 rpcclient-4.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-04 06:07:41.000000 rpcclient-4.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-04 06:07:41.000000 rpcclient-4.6.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.338661 rpcclient-4.6.0/rpcclient/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 06:08:05.000000 rpcclient-4.6.0/rpcclient/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/allocated.py
--rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/client_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.346661 rpcclient-4.6.0/rpcclient/darwin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/cfpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    42645 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/core_graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/crash_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/darwin_lief.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/ioregistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/keychain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/objc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7665 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/power.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)    44670 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/scpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)    30236 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)    12094 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/syslog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/xpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23947 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.346661 rpcclient-4.6.0/rpcclient/ios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/amfi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/backlight.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/mobile_gestalt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/screen_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/sprinboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/telephony.py
--rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/wifi.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/lief.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.346661 rpcclient-4.6.0/rpcclient/linux/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/linux/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/linux/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.346661 rpcclient-4.6.0/rpcclient/macos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/macos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/macos/apple_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/macos/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/processes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.346661 rpcclient-4.6.0/rpcclient/protos/
--rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-04-04 06:07:52.000000 rpcclient-4.6.0/rpcclient/protos/rpc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    30372 2024-04-04 06:07:52.000000 rpcclient-4.6.0/rpcclient/protos/rpc_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/protosocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.350661 rpcclient-4.6.0/rpcclient/structs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/structs/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/structs/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/symbols_jar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (127)    25827 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/xonshrc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.350661 rpcclient-4.6.0/rpcclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-04 06:08:05.000000 rpcclient-4.6.0/rpcclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-04 06:08:05.000000 rpcclient-4.6.0/rpcclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 06:08:05.000000 rpcclient-4.6.0/rpcclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-04 06:08:05.000000 rpcclient-4.6.0/rpcclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-04 06:08:05.000000 rpcclient-4.6.0/rpcclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 06:08:05.000000 rpcclient-4.6.0/rpcclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 06:08:05.354661 rpcclient-4.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.350661 rpcclient-4.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_allocation_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_core_foundation_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_darwin_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_keychain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_objc_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_power.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_spawn.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_thread_safe.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_worker_processes.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_xpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.441916 rpcclient-4.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-11 10:51:21.000000 rpcclient-4.6.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-11 10:51:21.000000 rpcclient-4.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-11 10:51:21.000000 rpcclient-4.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-11 10:51:39.441916 rpcclient-4.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-11 10:51:21.000000 rpcclient-4.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-11 10:51:21.000000 rpcclient-4.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-11 10:51:21.000000 rpcclient-4.6.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.425916 rpcclient-4.6.1/rpcclient/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-11 10:51:39.000000 rpcclient-4.6.1/rpcclient/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/allocated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19781 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/client_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.433916 rpcclient-4.6.1/rpcclient/darwin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/cfpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42645 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/core_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/crash_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/darwin_lief.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/ioregistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/keychain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/objc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7665 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/power.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44670 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/scpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30236 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12094 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/darwin/xpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23947 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.433916 rpcclient-4.6.1/rpcclient/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/amfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/backlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/mobile_gestalt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/screen_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/sprinboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/telephony.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/ios/wifi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/lief.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.433916 rpcclient-4.6.1/rpcclient/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/linux/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/linux/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.437916 rpcclient-4.6.1/rpcclient/macos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/macos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/macos/apple_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/macos/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/processes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.437916 rpcclient-4.6.1/rpcclient/protos/
+-rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-04-11 10:51:28.000000 rpcclient-4.6.1/rpcclient/protos/rpc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30372 2024-04-11 10:51:28.000000 rpcclient-4.6.1/rpcclient/protos/rpc_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/protosocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.437916 rpcclient-4.6.1/rpcclient/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/structs/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/structs/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/symbols_jar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25827 2024-04-11 10:51:21.000000 rpcclient-4.6.1/rpcclient/xonshrc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.437916 rpcclient-4.6.1/rpcclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-11 10:51:39.000000 rpcclient-4.6.1/rpcclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-11 10:51:39.000000 rpcclient-4.6.1/rpcclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 10:51:39.000000 rpcclient-4.6.1/rpcclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-11 10:51:39.000000 rpcclient-4.6.1/rpcclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-11 10:51:39.000000 rpcclient-4.6.1/rpcclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 10:51:39.000000 rpcclient-4.6.1/rpcclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 10:51:39.441916 rpcclient-4.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:51:39.437916 rpcclient-4.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_allocation_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_core_foundation_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_darwin_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_keychain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_objc_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_power.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_thread_safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_worker_processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-11 10:51:21.000000 rpcclient-4.6.1/tests/test_xpc.py
```

### Comparing `rpcclient-4.6.0/CODE_OF_CONDUCT.md` & `rpcclient-4.6.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/LICENSE` & `rpcclient-4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/PKG-INFO` & `rpcclient-4.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpcclient
-Version: 4.6.0
+Version: 4.6.1
 Summary: rpcclient for connecting with the rpcserver
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanelc305 <netanelc305@pm.me>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanelc305 <netanelc305@pm.me>
 License: GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007
 Project-URL: Homepage, https://github.com/doronz88/rpc-project
 Project-URL: Bug Reports, https://github.com/doronz88/rpc-project/issues
 Keywords: ios,macos,linux,automation,remote-shell,remote-control,ipython
```

### Comparing `rpcclient-4.6.0/pyproject.toml` & `rpcclient-4.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/__main__.py` & `rpcclient-4.6.1/rpcclient/__main__.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/client.py` & `rpcclient-4.6.1/rpcclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,17 +365,19 @@
 
     def interactive(self, additional_namespace: typing.Mapping = None):
         """ Start an interactive shell """
         sys.argv = ['a']
         c = Config()
         c.IPCompleter.use_jedi = False
         c.InteractiveShellApp.exec_lines = [
-            '''IPython.get_ipython().events.register('pre_run_cell', p._ipython_run_cell_hook)'''
+            '''IPython.get_ipython().events.register('pre_run_cell', p._ipython_run_cell_hook)''',
+            '''logging.getLogger('asyncio').disabled = True'''
         ]
         c.TerminalInteractiveShell.autoformatter = None
+        c.BaseIPythonApplication.profile = 'rpcclient'
         namespace = globals()
         namespace.update({'p': self, 'symbols': self.symbols})
         if additional_namespace is not None:
             namespace.update(additional_namespace)
         print(USAGE)
         IPython.start_ipython(config=c, user_ns=namespace)
```

### Comparing `rpcclient-4.6.0/rpcclient/client_factory.py` & `rpcclient-4.6.1/rpcclient/client_factory.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/bluetooth.py` & `rpcclient-4.6.1/rpcclient/darwin/bluetooth.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/cfpreferences.py` & `rpcclient-4.6.1/rpcclient/darwin/cfpreferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/client.py` & `rpcclient-4.6.1/rpcclient/darwin/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/consts.py` & `rpcclient-4.6.1/rpcclient/darwin/consts.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/core_graphics.py` & `rpcclient-4.6.1/rpcclient/darwin/core_graphics.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/crash_reports.py` & `rpcclient-4.6.1/rpcclient/darwin/crash_reports.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/darwin_lief.py` & `rpcclient-4.6.1/rpcclient/darwin/darwin_lief.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/fs.py` & `rpcclient-4.6.1/rpcclient/darwin/fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/hid.py` & `rpcclient-4.6.1/rpcclient/darwin/hid.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/ioregistry.py` & `rpcclient-4.6.1/rpcclient/darwin/ioregistry.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/keychain.py` & `rpcclient-4.6.1/rpcclient/darwin/keychain.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/location.py` & `rpcclient-4.6.1/rpcclient/darwin/location.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/media.py` & `rpcclient-4.6.1/rpcclient/darwin/media.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/network.py` & `rpcclient-4.6.1/rpcclient/darwin/network.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/objc.py` & `rpcclient-4.6.1/rpcclient/darwin/objc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/objective_c_class.py` & `rpcclient-4.6.1/rpcclient/darwin/objective_c_class.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/objective_c_symbol.py` & `rpcclient-4.6.1/rpcclient/darwin/objective_c_symbol.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,7 +233,10 @@
         try:
             self._set_ivar(key, value)
         except SettingIvarError:
             super(ObjectiveCSymbol, self).__setattr__(key, value)
 
     def __str__(self):
         return self._to_str(False)
+
+    def __repr__(self):
+        return f'<{self.__class__.__name__} 0x{int(self):x} Class: {self.class_.name}>'
```

### Comparing `rpcclient-4.6.0/rpcclient/darwin/power.py` & `rpcclient-4.6.1/rpcclient/darwin/power.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/processes.py` & `rpcclient-4.6.1/rpcclient/darwin/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/reports.py` & `rpcclient-4.6.1/rpcclient/darwin/reports.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/scpreferences.py` & `rpcclient-4.6.1/rpcclient/darwin/scpreferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/structs.py` & `rpcclient-4.6.1/rpcclient/darwin/structs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/symbol.py` & `rpcclient-4.6.1/rpcclient/darwin/symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/syslog.py` & `rpcclient-4.6.1/rpcclient/darwin/syslog.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/time.py` & `rpcclient-4.6.1/rpcclient/darwin/time.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/darwin/xpc.py` & `rpcclient-4.6.1/rpcclient/darwin/xpc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/exceptions.py` & `rpcclient-4.6.1/rpcclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/fs.py` & `rpcclient-4.6.1/rpcclient/fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/ios/accessibility.py` & `rpcclient-4.6.1/rpcclient/ios/accessibility.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/ios/amfi.py` & `rpcclient-4.6.1/rpcclient/ios/amfi.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/ios/backlight.py` & `rpcclient-4.6.1/rpcclient/ios/backlight.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/ios/client.py` & `rpcclient-4.6.1/rpcclient/ios/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/ios/lockdown.py` & `rpcclient-4.6.1/rpcclient/ios/lockdown.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/ios/mobile_gestalt.py` & `rpcclient-4.6.1/rpcclient/ios/mobile_gestalt.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/ios/processes.py` & `rpcclient-4.6.1/rpcclient/ios/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/ios/screen_capture.py` & `rpcclient-4.6.1/rpcclient/ios/screen_capture.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/ios/sprinboard.py` & `rpcclient-4.6.1/rpcclient/ios/sprinboard.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/ios/telephony.py` & `rpcclient-4.6.1/rpcclient/ios/telephony.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/ios/wifi.py` & `rpcclient-4.6.1/rpcclient/ios/wifi.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/lief.py` & `rpcclient-4.6.1/rpcclient/lief.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/linux/client.py` & `rpcclient-4.6.1/rpcclient/linux/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/linux/structs.py` & `rpcclient-4.6.1/rpcclient/linux/structs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/macos/apple_script.py` & `rpcclient-4.6.1/rpcclient/macos/apple_script.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/macos/client.py` & `rpcclient-4.6.1/rpcclient/macos/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/network.py` & `rpcclient-4.6.1/rpcclient/network.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/processes.py` & `rpcclient-4.6.1/rpcclient/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/protos/rpc_pb2.py` & `rpcclient-4.6.1/rpcclient/protos/rpc_pb2.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/protos/rpc_pb2.pyi` & `rpcclient-4.6.1/rpcclient/protos/rpc_pb2.pyi`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/protosocket.py` & `rpcclient-4.6.1/rpcclient/protosocket.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/structs/consts.py` & `rpcclient-4.6.1/rpcclient/structs/consts.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/structs/generic.py` & `rpcclient-4.6.1/rpcclient/structs/generic.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/symbol.py` & `rpcclient-4.6.1/rpcclient/symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/symbols_jar.py` & `rpcclient-4.6.1/rpcclient/symbols_jar.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/sysctl.py` & `rpcclient-4.6.1/rpcclient/sysctl.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient/xonshrc.py` & `rpcclient-4.6.1/rpcclient/xonshrc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/rpcclient.egg-info/PKG-INFO` & `rpcclient-4.6.1/rpcclient.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpcclient
-Version: 4.6.0
+Version: 4.6.1
 Summary: rpcclient for connecting with the rpcserver
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanelc305 <netanelc305@pm.me>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanelc305 <netanelc305@pm.me>
 License: GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007
 Project-URL: Homepage, https://github.com/doronz88/rpc-project
 Project-URL: Bug Reports, https://github.com/doronz88/rpc-project/issues
 Keywords: ios,macos,linux,automation,remote-shell,remote-control,ipython
```

### Comparing `rpcclient-4.6.0/rpcclient.egg-info/SOURCES.txt` & `rpcclient-4.6.1/rpcclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/tests/conftest.py` & `rpcclient-4.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/tests/test_allocation_cleanup.py` & `rpcclient-4.6.1/tests/test_allocation_cleanup.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/tests/test_client.py` & `rpcclient-4.6.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/tests/test_darwin_client.py` & `rpcclient-4.6.1/tests/test_darwin_client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/tests/test_fs.py` & `rpcclient-4.6.1/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/tests/test_objc_symbol.py` & `rpcclient-4.6.1/tests/test_objc_symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/tests/test_power.py` & `rpcclient-4.6.1/tests/test_power.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/tests/test_preferences.py` & `rpcclient-4.6.1/tests/test_preferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/tests/test_processes.py` & `rpcclient-4.6.1/tests/test_processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/tests/test_socket.py` & `rpcclient-4.6.1/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/tests/test_spawn.py` & `rpcclient-4.6.1/tests/test_spawn.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/tests/test_thread_safe.py` & `rpcclient-4.6.1/tests/test_thread_safe.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/tests/test_time.py` & `rpcclient-4.6.1/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.6.0/tests/test_xpc.py` & `rpcclient-4.6.1/tests/test_xpc.py`

 * *Files identical despite different names*

