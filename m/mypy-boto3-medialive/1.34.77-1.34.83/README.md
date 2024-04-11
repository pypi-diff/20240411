# Comparing `tmp/mypy-boto3-medialive-1.34.77.tar.gz` & `tmp/mypy-boto3-medialive-1.34.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-medialive-1.34.77.tar", last modified: Wed Apr  3 19:32:40 2024, max compression
+gzip compressed data, was "mypy-boto3-medialive-1.34.83.tar", last modified: Thu Apr 11 19:18:07 2024, max compression
```

## Comparing `mypy-boto3-medialive-1.34.77.tar` & `mypy-boto3-medialive-1.34.83.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:40.200160 mypy-boto3-medialive-1.34.77/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 19:32:19.000000 mypy-boto3-medialive-1.34.77/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15740 2024-04-03 19:32:40.200160 mypy-boto3-medialive-1.34.77/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14177 2024-04-03 19:32:19.000000 mypy-boto3-medialive-1.34.77/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:40.200160 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-03 19:32:19.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-03 19:32:19.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-03 19:32:19.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54614 2024-04-03 19:32:20.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    54611 2024-04-03 19:32:19.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    43209 2024-04-03 19:32:20.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    43209 2024-04-03 19:32:20.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-04-03 19:32:20.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12116 2024-04-03 19:32:20.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:19.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   156623 2024-04-03 19:32:23.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   156623 2024-04-03 19:32:23.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 19:32:19.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-04-03 19:32:20.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-03 19:32:20.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:40.200160 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15740 2024-04-03 19:32:40.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-03 19:32:40.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:40.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:40.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 19:32:40.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 19:32:40.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:32:40.200160 mypy-boto3-medialive-1.34.77/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-03 19:32:19.000000 mypy-boto3-medialive-1.34.77/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:07.415372 mypy-boto3-medialive-1.34.83/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 19:17:30.000000 mypy-boto3-medialive-1.34.83/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17232 2024-04-11 19:18:07.415372 mypy-boto3-medialive-1.34.83/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15669 2024-04-11 19:17:30.000000 mypy-boto3-medialive-1.34.83/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:07.415372 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-11 19:17:30.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-11 19:17:30.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-11 19:17:30.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77865 2024-04-11 19:17:31.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77862 2024-04-11 19:17:30.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    46713 2024-04-11 19:17:32.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46713 2024-04-11 19:17:31.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18536 2024-04-11 19:17:31.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18520 2024-04-11 19:17:31.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:17:30.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   186555 2024-04-11 19:17:35.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   186555 2024-04-11 19:17:34.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 19:17:30.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-04-11 19:17:31.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-04-11 19:17:31.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:07.415372 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17232 2024-04-11 19:18:07.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-11 19:18:07.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:07.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:07.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 19:18:07.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-11 19:18:07.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:18:07.415372 mypy-boto3-medialive-1.34.83/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-11 19:17:30.000000 mypy-boto3-medialive-1.34.83/setup.py
```

### Comparing `mypy-boto3-medialive-1.34.77/LICENSE` & `mypy-boto3-medialive-1.34.83/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.34.77/PKG-INFO` & `mypy-boto3-medialive-1.34.83/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medialive
-Version: 1.34.77
-Summary: Type annotations for boto3.MediaLive 1.34.77 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.83
+Summary: Type annotations for boto3.MediaLive 1.34.83 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -283,44 +283,62 @@
 ```python
 from boto3.session import Session
 
 from mypy_boto3_medialive import MediaLiveClient
 from mypy_boto3_medialive.paginator import (
     DescribeSchedulePaginator,
     ListChannelsPaginator,
+    ListCloudWatchAlarmTemplateGroupsPaginator,
+    ListCloudWatchAlarmTemplatesPaginator,
+    ListEventBridgeRuleTemplateGroupsPaginator,
+    ListEventBridgeRuleTemplatesPaginator,
     ListInputDeviceTransfersPaginator,
     ListInputDevicesPaginator,
     ListInputSecurityGroupsPaginator,
     ListInputsPaginator,
     ListMultiplexProgramsPaginator,
     ListMultiplexesPaginator,
     ListOfferingsPaginator,
     ListReservationsPaginator,
+    ListSignalMapsPaginator,
 )
 
 client: MediaLiveClient = Session().client("medialive")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_schedule_paginator: DescribeSchedulePaginator = client.get_paginator("describe_schedule")
 list_channels_paginator: ListChannelsPaginator = client.get_paginator("list_channels")
+list_cloud_watch_alarm_template_groups_paginator: ListCloudWatchAlarmTemplateGroupsPaginator = (
+    client.get_paginator("list_cloud_watch_alarm_template_groups")
+)
+list_cloud_watch_alarm_templates_paginator: ListCloudWatchAlarmTemplatesPaginator = (
+    client.get_paginator("list_cloud_watch_alarm_templates")
+)
+list_event_bridge_rule_template_groups_paginator: ListEventBridgeRuleTemplateGroupsPaginator = (
+    client.get_paginator("list_event_bridge_rule_template_groups")
+)
+list_event_bridge_rule_templates_paginator: ListEventBridgeRuleTemplatesPaginator = (
+    client.get_paginator("list_event_bridge_rule_templates")
+)
 list_input_device_transfers_paginator: ListInputDeviceTransfersPaginator = client.get_paginator(
     "list_input_device_transfers"
 )
 list_input_devices_paginator: ListInputDevicesPaginator = client.get_paginator("list_input_devices")
 list_input_security_groups_paginator: ListInputSecurityGroupsPaginator = client.get_paginator(
     "list_input_security_groups"
 )
 list_inputs_paginator: ListInputsPaginator = client.get_paginator("list_inputs")
 list_multiplex_programs_paginator: ListMultiplexProgramsPaginator = client.get_paginator(
     "list_multiplex_programs"
 )
 list_multiplexes_paginator: ListMultiplexesPaginator = client.get_paginator("list_multiplexes")
 list_offerings_paginator: ListOfferingsPaginator = client.get_paginator("list_offerings")
 list_reservations_paginator: ListReservationsPaginator = client.get_paginator("list_reservations")
+list_signal_maps_paginator: ListSignalMapsPaginator = client.get_paginator("list_signal_maps")
 ```
 
 <a id="waiters-annotations"></a>
 
 ### Waiters annotations
 
 `mypy_boto3_medialive.waiter` module contains type annotations for all waiters.
@@ -337,14 +355,18 @@
     InputAttachedWaiter,
     InputDeletedWaiter,
     InputDetachedWaiter,
     MultiplexCreatedWaiter,
     MultiplexDeletedWaiter,
     MultiplexRunningWaiter,
     MultiplexStoppedWaiter,
+    SignalMapCreatedWaiter,
+    SignalMapMonitorDeletedWaiter,
+    SignalMapMonitorDeployedWaiter,
+    SignalMapUpdatedWaiter,
 )
 
 client: MediaLiveClient = Session().client("medialive")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 channel_created_waiter: ChannelCreatedWaiter = client.get_waiter("channel_created")
@@ -354,14 +376,22 @@
 input_attached_waiter: InputAttachedWaiter = client.get_waiter("input_attached")
 input_deleted_waiter: InputDeletedWaiter = client.get_waiter("input_deleted")
 input_detached_waiter: InputDetachedWaiter = client.get_waiter("input_detached")
 multiplex_created_waiter: MultiplexCreatedWaiter = client.get_waiter("multiplex_created")
 multiplex_deleted_waiter: MultiplexDeletedWaiter = client.get_waiter("multiplex_deleted")
 multiplex_running_waiter: MultiplexRunningWaiter = client.get_waiter("multiplex_running")
 multiplex_stopped_waiter: MultiplexStoppedWaiter = client.get_waiter("multiplex_stopped")
+signal_map_created_waiter: SignalMapCreatedWaiter = client.get_waiter("signal_map_created")
+signal_map_monitor_deleted_waiter: SignalMapMonitorDeletedWaiter = client.get_waiter(
+    "signal_map_monitor_deleted"
+)
+signal_map_monitor_deployed_waiter: SignalMapMonitorDeployedWaiter = client.get_waiter(
+    "signal_map_monitor_deployed"
+)
+signal_map_updated_waiter: SignalMapUpdatedWaiter = client.get_waiter("signal_map_updated")
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_medialive.literals` module contains literals extracted from shapes
```

### Comparing `mypy-boto3-medialive-1.34.77/README.md` & `mypy-boto3-medialive-1.34.83/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -250,44 +250,62 @@
 ```python
 from boto3.session import Session
 
 from mypy_boto3_medialive import MediaLiveClient
 from mypy_boto3_medialive.paginator import (
     DescribeSchedulePaginator,
     ListChannelsPaginator,
+    ListCloudWatchAlarmTemplateGroupsPaginator,
+    ListCloudWatchAlarmTemplatesPaginator,
+    ListEventBridgeRuleTemplateGroupsPaginator,
+    ListEventBridgeRuleTemplatesPaginator,
     ListInputDeviceTransfersPaginator,
     ListInputDevicesPaginator,
     ListInputSecurityGroupsPaginator,
     ListInputsPaginator,
     ListMultiplexProgramsPaginator,
     ListMultiplexesPaginator,
     ListOfferingsPaginator,
     ListReservationsPaginator,
+    ListSignalMapsPaginator,
 )
 
 client: MediaLiveClient = Session().client("medialive")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_schedule_paginator: DescribeSchedulePaginator = client.get_paginator("describe_schedule")
 list_channels_paginator: ListChannelsPaginator = client.get_paginator("list_channels")
+list_cloud_watch_alarm_template_groups_paginator: ListCloudWatchAlarmTemplateGroupsPaginator = (
+    client.get_paginator("list_cloud_watch_alarm_template_groups")
+)
+list_cloud_watch_alarm_templates_paginator: ListCloudWatchAlarmTemplatesPaginator = (
+    client.get_paginator("list_cloud_watch_alarm_templates")
+)
+list_event_bridge_rule_template_groups_paginator: ListEventBridgeRuleTemplateGroupsPaginator = (
+    client.get_paginator("list_event_bridge_rule_template_groups")
+)
+list_event_bridge_rule_templates_paginator: ListEventBridgeRuleTemplatesPaginator = (
+    client.get_paginator("list_event_bridge_rule_templates")
+)
 list_input_device_transfers_paginator: ListInputDeviceTransfersPaginator = client.get_paginator(
     "list_input_device_transfers"
 )
 list_input_devices_paginator: ListInputDevicesPaginator = client.get_paginator("list_input_devices")
 list_input_security_groups_paginator: ListInputSecurityGroupsPaginator = client.get_paginator(
     "list_input_security_groups"
 )
 list_inputs_paginator: ListInputsPaginator = client.get_paginator("list_inputs")
 list_multiplex_programs_paginator: ListMultiplexProgramsPaginator = client.get_paginator(
     "list_multiplex_programs"
 )
 list_multiplexes_paginator: ListMultiplexesPaginator = client.get_paginator("list_multiplexes")
 list_offerings_paginator: ListOfferingsPaginator = client.get_paginator("list_offerings")
 list_reservations_paginator: ListReservationsPaginator = client.get_paginator("list_reservations")
+list_signal_maps_paginator: ListSignalMapsPaginator = client.get_paginator("list_signal_maps")
 ```
 
 <a id="waiters-annotations"></a>
 
 ### Waiters annotations
 
 `mypy_boto3_medialive.waiter` module contains type annotations for all waiters.
@@ -304,14 +322,18 @@
     InputAttachedWaiter,
     InputDeletedWaiter,
     InputDetachedWaiter,
     MultiplexCreatedWaiter,
     MultiplexDeletedWaiter,
     MultiplexRunningWaiter,
     MultiplexStoppedWaiter,
+    SignalMapCreatedWaiter,
+    SignalMapMonitorDeletedWaiter,
+    SignalMapMonitorDeployedWaiter,
+    SignalMapUpdatedWaiter,
 )
 
 client: MediaLiveClient = Session().client("medialive")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 channel_created_waiter: ChannelCreatedWaiter = client.get_waiter("channel_created")
@@ -321,14 +343,22 @@
 input_attached_waiter: InputAttachedWaiter = client.get_waiter("input_attached")
 input_deleted_waiter: InputDeletedWaiter = client.get_waiter("input_deleted")
 input_detached_waiter: InputDetachedWaiter = client.get_waiter("input_detached")
 multiplex_created_waiter: MultiplexCreatedWaiter = client.get_waiter("multiplex_created")
 multiplex_deleted_waiter: MultiplexDeletedWaiter = client.get_waiter("multiplex_deleted")
 multiplex_running_waiter: MultiplexRunningWaiter = client.get_waiter("multiplex_running")
 multiplex_stopped_waiter: MultiplexStoppedWaiter = client.get_waiter("multiplex_stopped")
+signal_map_created_waiter: SignalMapCreatedWaiter = client.get_waiter("signal_map_created")
+signal_map_monitor_deleted_waiter: SignalMapMonitorDeletedWaiter = client.get_waiter(
+    "signal_map_monitor_deleted"
+)
+signal_map_monitor_deployed_waiter: SignalMapMonitorDeployedWaiter = client.get_waiter(
+    "signal_map_monitor_deployed"
+)
+signal_map_updated_waiter: SignalMapUpdatedWaiter = client.get_waiter("signal_map_updated")
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_medialive.literals` module contains literals extracted from shapes
```

### Comparing `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/__init__.py` & `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,27 +12,36 @@
         ChannelStoppedWaiter,
         Client,
         DescribeSchedulePaginator,
         InputAttachedWaiter,
         InputDeletedWaiter,
         InputDetachedWaiter,
         ListChannelsPaginator,
+        ListCloudWatchAlarmTemplateGroupsPaginator,
+        ListCloudWatchAlarmTemplatesPaginator,
+        ListEventBridgeRuleTemplateGroupsPaginator,
+        ListEventBridgeRuleTemplatesPaginator,
         ListInputDeviceTransfersPaginator,
         ListInputDevicesPaginator,
         ListInputSecurityGroupsPaginator,
         ListInputsPaginator,
         ListMultiplexProgramsPaginator,
         ListMultiplexesPaginator,
         ListOfferingsPaginator,
         ListReservationsPaginator,
+        ListSignalMapsPaginator,
         MediaLiveClient,
         MultiplexCreatedWaiter,
         MultiplexDeletedWaiter,
         MultiplexRunningWaiter,
         MultiplexStoppedWaiter,
+        SignalMapCreatedWaiter,
+        SignalMapMonitorDeletedWaiter,
+        SignalMapMonitorDeployedWaiter,
+        SignalMapUpdatedWaiter,
     )
 
     session = Session()
     client: MediaLiveClient = session.client("medialive")
 
     channel_created_waiter: ChannelCreatedWaiter = client.get_waiter("channel_created")
     channel_deleted_waiter: ChannelDeletedWaiter = client.get_waiter("channel_deleted")
@@ -41,53 +50,71 @@
     input_attached_waiter: InputAttachedWaiter = client.get_waiter("input_attached")
     input_deleted_waiter: InputDeletedWaiter = client.get_waiter("input_deleted")
     input_detached_waiter: InputDetachedWaiter = client.get_waiter("input_detached")
     multiplex_created_waiter: MultiplexCreatedWaiter = client.get_waiter("multiplex_created")
     multiplex_deleted_waiter: MultiplexDeletedWaiter = client.get_waiter("multiplex_deleted")
     multiplex_running_waiter: MultiplexRunningWaiter = client.get_waiter("multiplex_running")
     multiplex_stopped_waiter: MultiplexStoppedWaiter = client.get_waiter("multiplex_stopped")
+    signal_map_created_waiter: SignalMapCreatedWaiter = client.get_waiter("signal_map_created")
+    signal_map_monitor_deleted_waiter: SignalMapMonitorDeletedWaiter = client.get_waiter("signal_map_monitor_deleted")
+    signal_map_monitor_deployed_waiter: SignalMapMonitorDeployedWaiter = client.get_waiter("signal_map_monitor_deployed")
+    signal_map_updated_waiter: SignalMapUpdatedWaiter = client.get_waiter("signal_map_updated")
 
     describe_schedule_paginator: DescribeSchedulePaginator = client.get_paginator("describe_schedule")
     list_channels_paginator: ListChannelsPaginator = client.get_paginator("list_channels")
+    list_cloud_watch_alarm_template_groups_paginator: ListCloudWatchAlarmTemplateGroupsPaginator = client.get_paginator("list_cloud_watch_alarm_template_groups")
+    list_cloud_watch_alarm_templates_paginator: ListCloudWatchAlarmTemplatesPaginator = client.get_paginator("list_cloud_watch_alarm_templates")
+    list_event_bridge_rule_template_groups_paginator: ListEventBridgeRuleTemplateGroupsPaginator = client.get_paginator("list_event_bridge_rule_template_groups")
+    list_event_bridge_rule_templates_paginator: ListEventBridgeRuleTemplatesPaginator = client.get_paginator("list_event_bridge_rule_templates")
     list_input_device_transfers_paginator: ListInputDeviceTransfersPaginator = client.get_paginator("list_input_device_transfers")
     list_input_devices_paginator: ListInputDevicesPaginator = client.get_paginator("list_input_devices")
     list_input_security_groups_paginator: ListInputSecurityGroupsPaginator = client.get_paginator("list_input_security_groups")
     list_inputs_paginator: ListInputsPaginator = client.get_paginator("list_inputs")
     list_multiplex_programs_paginator: ListMultiplexProgramsPaginator = client.get_paginator("list_multiplex_programs")
     list_multiplexes_paginator: ListMultiplexesPaginator = client.get_paginator("list_multiplexes")
     list_offerings_paginator: ListOfferingsPaginator = client.get_paginator("list_offerings")
     list_reservations_paginator: ListReservationsPaginator = client.get_paginator("list_reservations")
+    list_signal_maps_paginator: ListSignalMapsPaginator = client.get_paginator("list_signal_maps")
     ```
 """
 
 from .client import MediaLiveClient
 from .paginator import (
     DescribeSchedulePaginator,
     ListChannelsPaginator,
+    ListCloudWatchAlarmTemplateGroupsPaginator,
+    ListCloudWatchAlarmTemplatesPaginator,
+    ListEventBridgeRuleTemplateGroupsPaginator,
+    ListEventBridgeRuleTemplatesPaginator,
     ListInputDevicesPaginator,
     ListInputDeviceTransfersPaginator,
     ListInputSecurityGroupsPaginator,
     ListInputsPaginator,
     ListMultiplexesPaginator,
     ListMultiplexProgramsPaginator,
     ListOfferingsPaginator,
     ListReservationsPaginator,
+    ListSignalMapsPaginator,
 )
 from .waiter import (
     ChannelCreatedWaiter,
     ChannelDeletedWaiter,
     ChannelRunningWaiter,
     ChannelStoppedWaiter,
     InputAttachedWaiter,
     InputDeletedWaiter,
     InputDetachedWaiter,
     MultiplexCreatedWaiter,
     MultiplexDeletedWaiter,
     MultiplexRunningWaiter,
     MultiplexStoppedWaiter,
+    SignalMapCreatedWaiter,
+    SignalMapMonitorDeletedWaiter,
+    SignalMapMonitorDeployedWaiter,
+    SignalMapUpdatedWaiter,
 )
 
 Client = MediaLiveClient
 
 __all__ = (
     "ChannelCreatedWaiter",
     "ChannelDeletedWaiter",
@@ -95,21 +122,30 @@
     "ChannelStoppedWaiter",
     "Client",
     "DescribeSchedulePaginator",
     "InputAttachedWaiter",
     "InputDeletedWaiter",
     "InputDetachedWaiter",
     "ListChannelsPaginator",
+    "ListCloudWatchAlarmTemplateGroupsPaginator",
+    "ListCloudWatchAlarmTemplatesPaginator",
+    "ListEventBridgeRuleTemplateGroupsPaginator",
+    "ListEventBridgeRuleTemplatesPaginator",
     "ListInputDeviceTransfersPaginator",
     "ListInputDevicesPaginator",
     "ListInputSecurityGroupsPaginator",
     "ListInputsPaginator",
     "ListMultiplexProgramsPaginator",
     "ListMultiplexesPaginator",
     "ListOfferingsPaginator",
     "ListReservationsPaginator",
+    "ListSignalMapsPaginator",
     "MediaLiveClient",
     "MultiplexCreatedWaiter",
     "MultiplexDeletedWaiter",
     "MultiplexRunningWaiter",
     "MultiplexStoppedWaiter",
+    "SignalMapCreatedWaiter",
+    "SignalMapMonitorDeletedWaiter",
+    "SignalMapMonitorDeployedWaiter",
+    "SignalMapUpdatedWaiter",
 )
```

### Comparing `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/__init__.pyi` & `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/__init__.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -12,27 +12,36 @@
         ChannelStoppedWaiter,
         Client,
         DescribeSchedulePaginator,
         InputAttachedWaiter,
         InputDeletedWaiter,
         InputDetachedWaiter,
         ListChannelsPaginator,
+        ListCloudWatchAlarmTemplateGroupsPaginator,
+        ListCloudWatchAlarmTemplatesPaginator,
+        ListEventBridgeRuleTemplateGroupsPaginator,
+        ListEventBridgeRuleTemplatesPaginator,
         ListInputDeviceTransfersPaginator,
         ListInputDevicesPaginator,
         ListInputSecurityGroupsPaginator,
         ListInputsPaginator,
         ListMultiplexProgramsPaginator,
         ListMultiplexesPaginator,
         ListOfferingsPaginator,
         ListReservationsPaginator,
+        ListSignalMapsPaginator,
         MediaLiveClient,
         MultiplexCreatedWaiter,
         MultiplexDeletedWaiter,
         MultiplexRunningWaiter,
         MultiplexStoppedWaiter,
+        SignalMapCreatedWaiter,
+        SignalMapMonitorDeletedWaiter,
+        SignalMapMonitorDeployedWaiter,
+        SignalMapUpdatedWaiter,
     )
 
     session = Session()
     client: MediaLiveClient = session.client("medialive")
 
     channel_created_waiter: ChannelCreatedWaiter = client.get_waiter("channel_created")
     channel_deleted_waiter: ChannelDeletedWaiter = client.get_waiter("channel_deleted")
@@ -41,53 +50,71 @@
     input_attached_waiter: InputAttachedWaiter = client.get_waiter("input_attached")
     input_deleted_waiter: InputDeletedWaiter = client.get_waiter("input_deleted")
     input_detached_waiter: InputDetachedWaiter = client.get_waiter("input_detached")
     multiplex_created_waiter: MultiplexCreatedWaiter = client.get_waiter("multiplex_created")
     multiplex_deleted_waiter: MultiplexDeletedWaiter = client.get_waiter("multiplex_deleted")
     multiplex_running_waiter: MultiplexRunningWaiter = client.get_waiter("multiplex_running")
     multiplex_stopped_waiter: MultiplexStoppedWaiter = client.get_waiter("multiplex_stopped")
+    signal_map_created_waiter: SignalMapCreatedWaiter = client.get_waiter("signal_map_created")
+    signal_map_monitor_deleted_waiter: SignalMapMonitorDeletedWaiter = client.get_waiter("signal_map_monitor_deleted")
+    signal_map_monitor_deployed_waiter: SignalMapMonitorDeployedWaiter = client.get_waiter("signal_map_monitor_deployed")
+    signal_map_updated_waiter: SignalMapUpdatedWaiter = client.get_waiter("signal_map_updated")
 
     describe_schedule_paginator: DescribeSchedulePaginator = client.get_paginator("describe_schedule")
     list_channels_paginator: ListChannelsPaginator = client.get_paginator("list_channels")
+    list_cloud_watch_alarm_template_groups_paginator: ListCloudWatchAlarmTemplateGroupsPaginator = client.get_paginator("list_cloud_watch_alarm_template_groups")
+    list_cloud_watch_alarm_templates_paginator: ListCloudWatchAlarmTemplatesPaginator = client.get_paginator("list_cloud_watch_alarm_templates")
+    list_event_bridge_rule_template_groups_paginator: ListEventBridgeRuleTemplateGroupsPaginator = client.get_paginator("list_event_bridge_rule_template_groups")
+    list_event_bridge_rule_templates_paginator: ListEventBridgeRuleTemplatesPaginator = client.get_paginator("list_event_bridge_rule_templates")
     list_input_device_transfers_paginator: ListInputDeviceTransfersPaginator = client.get_paginator("list_input_device_transfers")
     list_input_devices_paginator: ListInputDevicesPaginator = client.get_paginator("list_input_devices")
     list_input_security_groups_paginator: ListInputSecurityGroupsPaginator = client.get_paginator("list_input_security_groups")
     list_inputs_paginator: ListInputsPaginator = client.get_paginator("list_inputs")
     list_multiplex_programs_paginator: ListMultiplexProgramsPaginator = client.get_paginator("list_multiplex_programs")
     list_multiplexes_paginator: ListMultiplexesPaginator = client.get_paginator("list_multiplexes")
     list_offerings_paginator: ListOfferingsPaginator = client.get_paginator("list_offerings")
     list_reservations_paginator: ListReservationsPaginator = client.get_paginator("list_reservations")
+    list_signal_maps_paginator: ListSignalMapsPaginator = client.get_paginator("list_signal_maps")
     ```
 """
 
 from .client import MediaLiveClient
 from .paginator import (
     DescribeSchedulePaginator,
     ListChannelsPaginator,
+    ListCloudWatchAlarmTemplateGroupsPaginator,
+    ListCloudWatchAlarmTemplatesPaginator,
+    ListEventBridgeRuleTemplateGroupsPaginator,
+    ListEventBridgeRuleTemplatesPaginator,
     ListInputDevicesPaginator,
     ListInputDeviceTransfersPaginator,
     ListInputSecurityGroupsPaginator,
     ListInputsPaginator,
     ListMultiplexesPaginator,
     ListMultiplexProgramsPaginator,
     ListOfferingsPaginator,
     ListReservationsPaginator,
+    ListSignalMapsPaginator,
 )
 from .waiter import (
     ChannelCreatedWaiter,
     ChannelDeletedWaiter,
     ChannelRunningWaiter,
     ChannelStoppedWaiter,
     InputAttachedWaiter,
     InputDeletedWaiter,
     InputDetachedWaiter,
     MultiplexCreatedWaiter,
     MultiplexDeletedWaiter,
     MultiplexRunningWaiter,
     MultiplexStoppedWaiter,
+    SignalMapCreatedWaiter,
+    SignalMapMonitorDeletedWaiter,
+    SignalMapMonitorDeployedWaiter,
+    SignalMapUpdatedWaiter,
 )
 
 Client = MediaLiveClient
 
 __all__ = (
     "ChannelCreatedWaiter",
     "ChannelDeletedWaiter",
@@ -95,21 +122,30 @@
     "ChannelStoppedWaiter",
     "Client",
     "DescribeSchedulePaginator",
     "InputAttachedWaiter",
     "InputDeletedWaiter",
     "InputDetachedWaiter",
     "ListChannelsPaginator",
+    "ListCloudWatchAlarmTemplateGroupsPaginator",
+    "ListCloudWatchAlarmTemplatesPaginator",
+    "ListEventBridgeRuleTemplateGroupsPaginator",
+    "ListEventBridgeRuleTemplatesPaginator",
     "ListInputDeviceTransfersPaginator",
     "ListInputDevicesPaginator",
     "ListInputSecurityGroupsPaginator",
     "ListInputsPaginator",
     "ListMultiplexProgramsPaginator",
     "ListMultiplexesPaginator",
     "ListOfferingsPaginator",
     "ListReservationsPaginator",
+    "ListSignalMapsPaginator",
     "MediaLiveClient",
     "MultiplexCreatedWaiter",
     "MultiplexDeletedWaiter",
     "MultiplexRunningWaiter",
     "MultiplexStoppedWaiter",
+    "SignalMapCreatedWaiter",
+    "SignalMapMonitorDeletedWaiter",
+    "SignalMapMonitorDeployedWaiter",
+    "SignalMapUpdatedWaiter",
 )
```

### Comparing `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/__main__.py` & `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaLive 1.34.77\n"
-        "Version:         1.34.77\n"
+        "Type annotations for boto3.MediaLive 1.34.83\n"
+        "Version:         1.34.83\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.77")
+    print("1.34.83")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/client.py` & `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,45 +18,60 @@
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ChannelClassType,
     ChannelPipelineIdToRestartType,
+    CloudWatchAlarmTemplateComparisonOperatorType,
+    CloudWatchAlarmTemplateStatisticType,
+    CloudWatchAlarmTemplateTargetResourceTypeType,
+    CloudWatchAlarmTemplateTreatMissingDataType,
+    EventBridgeRuleTemplateEventTypeType,
     InputTypeType,
     LogLevelType,
     RebootInputDeviceForceType,
 )
 from .paginator import (
     DescribeSchedulePaginator,
     ListChannelsPaginator,
+    ListCloudWatchAlarmTemplateGroupsPaginator,
+    ListCloudWatchAlarmTemplatesPaginator,
+    ListEventBridgeRuleTemplateGroupsPaginator,
+    ListEventBridgeRuleTemplatesPaginator,
     ListInputDevicesPaginator,
     ListInputDeviceTransfersPaginator,
     ListInputSecurityGroupsPaginator,
     ListInputsPaginator,
     ListMultiplexesPaginator,
     ListMultiplexProgramsPaginator,
     ListOfferingsPaginator,
     ListReservationsPaginator,
+    ListSignalMapsPaginator,
 )
 from .type_defs import (
     AccountConfigurationTypeDef,
     BatchDeleteResponseTypeDef,
     BatchScheduleActionCreateRequestTypeDef,
     BatchScheduleActionDeleteRequestTypeDef,
     BatchStartResponseTypeDef,
     BatchStopResponseTypeDef,
     BatchUpdateScheduleResponseTypeDef,
     CdiInputSpecificationTypeDef,
     CreateChannelResponseTypeDef,
+    CreateCloudWatchAlarmTemplateGroupResponseTypeDef,
+    CreateCloudWatchAlarmTemplateResponseTypeDef,
+    CreateEventBridgeRuleTemplateGroupResponseTypeDef,
+    CreateEventBridgeRuleTemplateResponseTypeDef,
     CreateInputResponseTypeDef,
     CreateInputSecurityGroupResponseTypeDef,
     CreateMultiplexProgramResponseTypeDef,
     CreateMultiplexResponseTypeDef,
     CreatePartnerInputResponseTypeDef,
+    CreateSignalMapResponseTypeDef,
     DeleteChannelResponseTypeDef,
     DeleteMultiplexProgramResponseTypeDef,
     DeleteMultiplexResponseTypeDef,
     DeleteReservationResponseTypeDef,
     DescribeAccountConfigurationResponseTypeDef,
     DescribeChannelResponseTypeDef,
     DescribeInputDeviceResponseTypeDef,
@@ -67,49 +82,67 @@
     DescribeMultiplexResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     DescribeReservationResponseTypeDef,
     DescribeScheduleResponseTypeDef,
     DescribeThumbnailsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EncoderSettingsTypeDef,
+    EventBridgeRuleTemplateTargetTypeDef,
+    GetCloudWatchAlarmTemplateGroupResponseTypeDef,
+    GetCloudWatchAlarmTemplateResponseTypeDef,
+    GetEventBridgeRuleTemplateGroupResponseTypeDef,
+    GetEventBridgeRuleTemplateResponseTypeDef,
+    GetSignalMapResponseTypeDef,
     InputAttachmentTypeDef,
     InputDestinationRequestTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
     InputDeviceSettingsTypeDef,
     InputSourceRequestTypeDef,
     InputSpecificationTypeDef,
     InputVpcRequestTypeDef,
     InputWhitelistRuleCidrTypeDef,
     ListChannelsResponseTypeDef,
+    ListCloudWatchAlarmTemplateGroupsResponseTypeDef,
+    ListCloudWatchAlarmTemplatesResponseTypeDef,
+    ListEventBridgeRuleTemplateGroupsResponseTypeDef,
+    ListEventBridgeRuleTemplatesResponseTypeDef,
     ListInputDevicesResponseTypeDef,
     ListInputDeviceTransfersResponseTypeDef,
     ListInputSecurityGroupsResponseTypeDef,
     ListInputsResponseTypeDef,
     ListMultiplexesResponseTypeDef,
     ListMultiplexProgramsResponseTypeDef,
     ListOfferingsResponseTypeDef,
     ListReservationsResponseTypeDef,
+    ListSignalMapsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaintenanceCreateSettingsTypeDef,
     MaintenanceUpdateSettingsTypeDef,
     MediaConnectFlowRequestTypeDef,
     MultiplexProgramSettingsTypeDef,
     MultiplexSettingsTypeDef,
     OutputDestinationTypeDef,
     PurchaseOfferingResponseTypeDef,
     RenewalSettingsTypeDef,
     RestartChannelPipelinesResponseTypeDef,
     StartChannelResponseTypeDef,
+    StartDeleteMonitorDeploymentResponseTypeDef,
+    StartMonitorDeploymentResponseTypeDef,
     StartMultiplexResponseTypeDef,
+    StartUpdateSignalMapResponseTypeDef,
     StopChannelResponseTypeDef,
     StopMultiplexResponseTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
     UpdateChannelClassResponseTypeDef,
     UpdateChannelResponseTypeDef,
+    UpdateCloudWatchAlarmTemplateGroupResponseTypeDef,
+    UpdateCloudWatchAlarmTemplateResponseTypeDef,
+    UpdateEventBridgeRuleTemplateGroupResponseTypeDef,
+    UpdateEventBridgeRuleTemplateResponseTypeDef,
     UpdateInputDeviceResponseTypeDef,
     UpdateInputResponseTypeDef,
     UpdateInputSecurityGroupResponseTypeDef,
     UpdateMultiplexProgramResponseTypeDef,
     UpdateMultiplexResponseTypeDef,
     UpdateReservationResponseTypeDef,
     VpcOutputSettingsTypeDef,
@@ -122,14 +155,18 @@
     InputAttachedWaiter,
     InputDeletedWaiter,
     InputDetachedWaiter,
     MultiplexCreatedWaiter,
     MultiplexDeletedWaiter,
     MultiplexRunningWaiter,
     MultiplexStoppedWaiter,
+    SignalMapCreatedWaiter,
+    SignalMapMonitorDeletedWaiter,
+    SignalMapMonitorDeployedWaiter,
+    SignalMapUpdatedWaiter,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -290,14 +327,83 @@
         Creates a new channel See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreateChannel).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_channel)
         """
 
+    def create_cloud_watch_alarm_template(
+        self,
+        *,
+        ComparisonOperator: CloudWatchAlarmTemplateComparisonOperatorType,
+        EvaluationPeriods: int,
+        GroupIdentifier: str,
+        MetricName: str,
+        Name: str,
+        Period: int,
+        Statistic: CloudWatchAlarmTemplateStatisticType,
+        TargetResourceType: CloudWatchAlarmTemplateTargetResourceTypeType,
+        Threshold: float,
+        TreatMissingData: CloudWatchAlarmTemplateTreatMissingDataType,
+        DatapointsToAlarm: int = ...,
+        Description: str = ...,
+        Tags: Mapping[str, str] = ...,
+    ) -> CreateCloudWatchAlarmTemplateResponseTypeDef:
+        """
+        Creates a cloudwatch alarm template to dynamically generate cloudwatch metric
+        alarms on targeted resource
+        types.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_cloud_watch_alarm_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_cloud_watch_alarm_template)
+        """
+
+    def create_cloud_watch_alarm_template_group(
+        self, *, Name: str, Description: str = ..., Tags: Mapping[str, str] = ...
+    ) -> CreateCloudWatchAlarmTemplateGroupResponseTypeDef:
+        """
+        Creates a cloudwatch alarm template group to group your cloudwatch alarm
+        templates and to attach to signal maps for dynamically creating
+        alarms.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_cloud_watch_alarm_template_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_cloud_watch_alarm_template_group)
+        """
+
+    def create_event_bridge_rule_template(
+        self,
+        *,
+        EventType: EventBridgeRuleTemplateEventTypeType,
+        GroupIdentifier: str,
+        Name: str,
+        Description: str = ...,
+        EventTargets: Sequence[EventBridgeRuleTemplateTargetTypeDef] = ...,
+        Tags: Mapping[str, str] = ...,
+    ) -> CreateEventBridgeRuleTemplateResponseTypeDef:
+        """
+        Creates an eventbridge rule template to monitor events and send notifications
+        to your targeted
+        resources.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_event_bridge_rule_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_event_bridge_rule_template)
+        """
+
+    def create_event_bridge_rule_template_group(
+        self, *, Name: str, Description: str = ..., Tags: Mapping[str, str] = ...
+    ) -> CreateEventBridgeRuleTemplateGroupResponseTypeDef:
+        """
+        Creates an eventbridge rule template group to group your eventbridge rule
+        templates and to attach to signal maps for dynamically creating notification
+        rules.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_event_bridge_rule_template_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_event_bridge_rule_template_group)
+        """
+
     def create_input(
         self,
         *,
         Destinations: Sequence[InputDestinationRequestTypeDef] = ...,
         InputDevices: Sequence[InputDeviceSettingsTypeDef] = ...,
         InputSecurityGroups: Sequence[str] = ...,
         MediaConnectFlows: Sequence[MediaConnectFlowRequestTypeDef] = ...,
@@ -369,14 +475,31 @@
         Create a partner input See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreatePartnerInput).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_partner_input)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_partner_input)
         """
 
+    def create_signal_map(
+        self,
+        *,
+        DiscoveryEntryPointArn: str,
+        Name: str,
+        CloudWatchAlarmTemplateGroupIdentifiers: Sequence[str] = ...,
+        Description: str = ...,
+        EventBridgeRuleTemplateGroupIdentifiers: Sequence[str] = ...,
+        Tags: Mapping[str, str] = ...,
+    ) -> CreateSignalMapResponseTypeDef:
+        """
+        Initiates the creation of a new signal map.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_signal_map)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_signal_map)
+        """
+
     def create_tags(
         self, *, ResourceArn: str, Tags: Mapping[str, str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Create tags for a resource See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreateTags).
 
@@ -388,14 +511,50 @@
         """
         Starts deletion of channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_channel)
         """
 
+    def delete_cloud_watch_alarm_template(self, *, Identifier: str) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes a cloudwatch alarm template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_cloud_watch_alarm_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_cloud_watch_alarm_template)
+        """
+
+    def delete_cloud_watch_alarm_template_group(
+        self, *, Identifier: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes a cloudwatch alarm template group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_cloud_watch_alarm_template_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_cloud_watch_alarm_template_group)
+        """
+
+    def delete_event_bridge_rule_template(self, *, Identifier: str) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes an eventbridge rule template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_event_bridge_rule_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_event_bridge_rule_template)
+        """
+
+    def delete_event_bridge_rule_template_group(
+        self, *, Identifier: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes an eventbridge rule template group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_event_bridge_rule_template_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_event_bridge_rule_template_group)
+        """
+
     def delete_input(self, *, InputId: str) -> Dict[str, Any]:
         """
         Deletes the input end point See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DeleteInput).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_input)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_input)
@@ -440,14 +599,22 @@
         """
         Delete all schedule actions on a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_schedule)
         """
 
+    def delete_signal_map(self, *, Identifier: str) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes the specified signal map.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_signal_map)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_signal_map)
+        """
+
     def delete_tags(
         self, *, ResourceArn: str, TagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes tags for a resource See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DeleteTags).
 
@@ -577,25 +744,129 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#generate_presigned_url)
         """
 
+    def get_cloud_watch_alarm_template(
+        self, *, Identifier: str
+    ) -> GetCloudWatchAlarmTemplateResponseTypeDef:
+        """
+        Retrieves the specified cloudwatch alarm template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_cloud_watch_alarm_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_cloud_watch_alarm_template)
+        """
+
+    def get_cloud_watch_alarm_template_group(
+        self, *, Identifier: str
+    ) -> GetCloudWatchAlarmTemplateGroupResponseTypeDef:
+        """
+        Retrieves the specified cloudwatch alarm template group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_cloud_watch_alarm_template_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_cloud_watch_alarm_template_group)
+        """
+
+    def get_event_bridge_rule_template(
+        self, *, Identifier: str
+    ) -> GetEventBridgeRuleTemplateResponseTypeDef:
+        """
+        Retrieves the specified eventbridge rule template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_event_bridge_rule_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_event_bridge_rule_template)
+        """
+
+    def get_event_bridge_rule_template_group(
+        self, *, Identifier: str
+    ) -> GetEventBridgeRuleTemplateGroupResponseTypeDef:
+        """
+        Retrieves the specified eventbridge rule template group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_event_bridge_rule_template_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_event_bridge_rule_template_group)
+        """
+
+    def get_signal_map(self, *, Identifier: str) -> GetSignalMapResponseTypeDef:
+        """
+        Retrieves the specified signal map.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_signal_map)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_signal_map)
+        """
+
     def list_channels(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChannelsResponseTypeDef:
         """
         Produces list of channels that have been created See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/ListChannels).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_channels)
         """
 
+    def list_cloud_watch_alarm_template_groups(
+        self,
+        *,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        Scope: str = ...,
+        SignalMapIdentifier: str = ...,
+    ) -> ListCloudWatchAlarmTemplateGroupsResponseTypeDef:
+        """
+        Lists cloudwatch alarm template groups.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_cloud_watch_alarm_template_groups)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_cloud_watch_alarm_template_groups)
+        """
+
+    def list_cloud_watch_alarm_templates(
+        self,
+        *,
+        GroupIdentifier: str = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        Scope: str = ...,
+        SignalMapIdentifier: str = ...,
+    ) -> ListCloudWatchAlarmTemplatesResponseTypeDef:
+        """
+        Lists cloudwatch alarm templates.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_cloud_watch_alarm_templates)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_cloud_watch_alarm_templates)
+        """
+
+    def list_event_bridge_rule_template_groups(
+        self, *, MaxResults: int = ..., NextToken: str = ..., SignalMapIdentifier: str = ...
+    ) -> ListEventBridgeRuleTemplateGroupsResponseTypeDef:
+        """
+        Lists eventbridge rule template groups.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_event_bridge_rule_template_groups)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_event_bridge_rule_template_groups)
+        """
+
+    def list_event_bridge_rule_templates(
+        self,
+        *,
+        GroupIdentifier: str = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        SignalMapIdentifier: str = ...,
+    ) -> ListEventBridgeRuleTemplatesResponseTypeDef:
+        """
+        Lists eventbridge rule templates.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_event_bridge_rule_templates)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_event_bridge_rule_templates)
+        """
+
     def list_input_device_transfers(
         self, *, TransferType: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListInputDeviceTransfersResponseTypeDef:
         """
         List input devices that are currently being transferred.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_input_device_transfers)
@@ -695,14 +966,29 @@
         """
         List purchased reservations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_reservations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_reservations)
         """
 
+    def list_signal_maps(
+        self,
+        *,
+        CloudWatchAlarmTemplateGroupIdentifier: str = ...,
+        EventBridgeRuleTemplateGroupIdentifier: str = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+    ) -> ListSignalMapsResponseTypeDef:
+        """
+        Lists signal maps.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_signal_maps)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_signal_maps)
+        """
+
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Produces list of tags that have been created for a resource See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/ListTagsForResource).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_tags_for_resource)
@@ -759,14 +1045,24 @@
         Starts an existing channel See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/StartChannel).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_channel)
         """
 
+    def start_delete_monitor_deployment(
+        self, *, Identifier: str
+    ) -> StartDeleteMonitorDeploymentResponseTypeDef:
+        """
+        Initiates a deployment to delete the monitor of the specified signal map.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_delete_monitor_deployment)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_delete_monitor_deployment)
+        """
+
     def start_input_device(self, *, InputDeviceId: str) -> Dict[str, Any]:
         """
         Start an input device that is attached to a MediaConnect flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_input_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_input_device)
         """
@@ -775,22 +1071,50 @@
         """
         Start a maintenance window for the specified input device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_input_device_maintenance_window)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_input_device_maintenance_window)
         """
 
+    def start_monitor_deployment(
+        self, *, Identifier: str, DryRun: bool = ...
+    ) -> StartMonitorDeploymentResponseTypeDef:
+        """
+        Initiates a deployment to deploy the latest monitor of the specified signal map.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_monitor_deployment)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_monitor_deployment)
+        """
+
     def start_multiplex(self, *, MultiplexId: str) -> StartMultiplexResponseTypeDef:
         """
         Start (run) the multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_multiplex)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_multiplex)
         """
 
+    def start_update_signal_map(
+        self,
+        *,
+        Identifier: str,
+        CloudWatchAlarmTemplateGroupIdentifiers: Sequence[str] = ...,
+        Description: str = ...,
+        DiscoveryEntryPointArn: str = ...,
+        EventBridgeRuleTemplateGroupIdentifiers: Sequence[str] = ...,
+        ForceRediscovery: bool = ...,
+        Name: str = ...,
+    ) -> StartUpdateSignalMapResponseTypeDef:
+        """
+        Initiates an update for the specified signal map.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_update_signal_map)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_update_signal_map)
+        """
+
     def stop_channel(self, *, ChannelId: str) -> StopChannelResponseTypeDef:
         """
         Stops a running channel See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/StopChannel).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.stop_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#stop_channel)
@@ -869,14 +1193,75 @@
         """
         Changes the class of the channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_channel_class)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_channel_class)
         """
 
+    def update_cloud_watch_alarm_template(
+        self,
+        *,
+        Identifier: str,
+        ComparisonOperator: CloudWatchAlarmTemplateComparisonOperatorType = ...,
+        DatapointsToAlarm: int = ...,
+        Description: str = ...,
+        EvaluationPeriods: int = ...,
+        GroupIdentifier: str = ...,
+        MetricName: str = ...,
+        Name: str = ...,
+        Period: int = ...,
+        Statistic: CloudWatchAlarmTemplateStatisticType = ...,
+        TargetResourceType: CloudWatchAlarmTemplateTargetResourceTypeType = ...,
+        Threshold: float = ...,
+        TreatMissingData: CloudWatchAlarmTemplateTreatMissingDataType = ...,
+    ) -> UpdateCloudWatchAlarmTemplateResponseTypeDef:
+        """
+        Updates the specified cloudwatch alarm template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_cloud_watch_alarm_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_cloud_watch_alarm_template)
+        """
+
+    def update_cloud_watch_alarm_template_group(
+        self, *, Identifier: str, Description: str = ...
+    ) -> UpdateCloudWatchAlarmTemplateGroupResponseTypeDef:
+        """
+        Updates the specified cloudwatch alarm template group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_cloud_watch_alarm_template_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_cloud_watch_alarm_template_group)
+        """
+
+    def update_event_bridge_rule_template(
+        self,
+        *,
+        Identifier: str,
+        Description: str = ...,
+        EventTargets: Sequence[EventBridgeRuleTemplateTargetTypeDef] = ...,
+        EventType: EventBridgeRuleTemplateEventTypeType = ...,
+        GroupIdentifier: str = ...,
+        Name: str = ...,
+    ) -> UpdateEventBridgeRuleTemplateResponseTypeDef:
+        """
+        Updates the specified eventbridge rule template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_event_bridge_rule_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_event_bridge_rule_template)
+        """
+
+    def update_event_bridge_rule_template_group(
+        self, *, Identifier: str, Description: str = ...
+    ) -> UpdateEventBridgeRuleTemplateGroupResponseTypeDef:
+        """
+        Updates the specified eventbridge rule template group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_event_bridge_rule_template_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_event_bridge_rule_template_group)
+        """
+
     def update_input(
         self,
         *,
         InputId: str,
         Destinations: Sequence[InputDestinationRequestTypeDef] = ...,
         InputDevices: Sequence[InputDeviceRequestTypeDef] = ...,
         InputSecurityGroups: Sequence[str] = ...,
@@ -974,14 +1359,50 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_cloud_watch_alarm_template_groups"]
+    ) -> ListCloudWatchAlarmTemplateGroupsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_cloud_watch_alarm_templates"]
+    ) -> ListCloudWatchAlarmTemplatesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_event_bridge_rule_template_groups"]
+    ) -> ListEventBridgeRuleTemplateGroupsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_event_bridge_rule_templates"]
+    ) -> ListEventBridgeRuleTemplatesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_input_device_transfers"]
     ) -> ListInputDeviceTransfersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
 
@@ -1041,14 +1462,21 @@
     ) -> ListReservationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(self, operation_name: Literal["list_signal_maps"]) -> ListSignalMapsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
+        """
+
+    @overload
     def get_waiter(self, waiter_name: Literal["channel_created"]) -> ChannelCreatedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
 
     @overload
@@ -1116,7 +1544,39 @@
 
     @overload
     def get_waiter(self, waiter_name: Literal["multiplex_stopped"]) -> MultiplexStoppedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
+
+    @overload
+    def get_waiter(self, waiter_name: Literal["signal_map_created"]) -> SignalMapCreatedWaiter:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
+        """
+
+    @overload
+    def get_waiter(
+        self, waiter_name: Literal["signal_map_monitor_deleted"]
+    ) -> SignalMapMonitorDeletedWaiter:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
+        """
+
+    @overload
+    def get_waiter(
+        self, waiter_name: Literal["signal_map_monitor_deployed"]
+    ) -> SignalMapMonitorDeployedWaiter:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
+        """
+
+    @overload
+    def get_waiter(self, waiter_name: Literal["signal_map_updated"]) -> SignalMapUpdatedWaiter:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
+        """
```

### Comparing `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/client.pyi` & `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/client.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -18,45 +18,60 @@
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ChannelClassType,
     ChannelPipelineIdToRestartType,
+    CloudWatchAlarmTemplateComparisonOperatorType,
+    CloudWatchAlarmTemplateStatisticType,
+    CloudWatchAlarmTemplateTargetResourceTypeType,
+    CloudWatchAlarmTemplateTreatMissingDataType,
+    EventBridgeRuleTemplateEventTypeType,
     InputTypeType,
     LogLevelType,
     RebootInputDeviceForceType,
 )
 from .paginator import (
     DescribeSchedulePaginator,
     ListChannelsPaginator,
+    ListCloudWatchAlarmTemplateGroupsPaginator,
+    ListCloudWatchAlarmTemplatesPaginator,
+    ListEventBridgeRuleTemplateGroupsPaginator,
+    ListEventBridgeRuleTemplatesPaginator,
     ListInputDevicesPaginator,
     ListInputDeviceTransfersPaginator,
     ListInputSecurityGroupsPaginator,
     ListInputsPaginator,
     ListMultiplexesPaginator,
     ListMultiplexProgramsPaginator,
     ListOfferingsPaginator,
     ListReservationsPaginator,
+    ListSignalMapsPaginator,
 )
 from .type_defs import (
     AccountConfigurationTypeDef,
     BatchDeleteResponseTypeDef,
     BatchScheduleActionCreateRequestTypeDef,
     BatchScheduleActionDeleteRequestTypeDef,
     BatchStartResponseTypeDef,
     BatchStopResponseTypeDef,
     BatchUpdateScheduleResponseTypeDef,
     CdiInputSpecificationTypeDef,
     CreateChannelResponseTypeDef,
+    CreateCloudWatchAlarmTemplateGroupResponseTypeDef,
+    CreateCloudWatchAlarmTemplateResponseTypeDef,
+    CreateEventBridgeRuleTemplateGroupResponseTypeDef,
+    CreateEventBridgeRuleTemplateResponseTypeDef,
     CreateInputResponseTypeDef,
     CreateInputSecurityGroupResponseTypeDef,
     CreateMultiplexProgramResponseTypeDef,
     CreateMultiplexResponseTypeDef,
     CreatePartnerInputResponseTypeDef,
+    CreateSignalMapResponseTypeDef,
     DeleteChannelResponseTypeDef,
     DeleteMultiplexProgramResponseTypeDef,
     DeleteMultiplexResponseTypeDef,
     DeleteReservationResponseTypeDef,
     DescribeAccountConfigurationResponseTypeDef,
     DescribeChannelResponseTypeDef,
     DescribeInputDeviceResponseTypeDef,
@@ -67,49 +82,67 @@
     DescribeMultiplexResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     DescribeReservationResponseTypeDef,
     DescribeScheduleResponseTypeDef,
     DescribeThumbnailsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EncoderSettingsTypeDef,
+    EventBridgeRuleTemplateTargetTypeDef,
+    GetCloudWatchAlarmTemplateGroupResponseTypeDef,
+    GetCloudWatchAlarmTemplateResponseTypeDef,
+    GetEventBridgeRuleTemplateGroupResponseTypeDef,
+    GetEventBridgeRuleTemplateResponseTypeDef,
+    GetSignalMapResponseTypeDef,
     InputAttachmentTypeDef,
     InputDestinationRequestTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
     InputDeviceSettingsTypeDef,
     InputSourceRequestTypeDef,
     InputSpecificationTypeDef,
     InputVpcRequestTypeDef,
     InputWhitelistRuleCidrTypeDef,
     ListChannelsResponseTypeDef,
+    ListCloudWatchAlarmTemplateGroupsResponseTypeDef,
+    ListCloudWatchAlarmTemplatesResponseTypeDef,
+    ListEventBridgeRuleTemplateGroupsResponseTypeDef,
+    ListEventBridgeRuleTemplatesResponseTypeDef,
     ListInputDevicesResponseTypeDef,
     ListInputDeviceTransfersResponseTypeDef,
     ListInputSecurityGroupsResponseTypeDef,
     ListInputsResponseTypeDef,
     ListMultiplexesResponseTypeDef,
     ListMultiplexProgramsResponseTypeDef,
     ListOfferingsResponseTypeDef,
     ListReservationsResponseTypeDef,
+    ListSignalMapsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaintenanceCreateSettingsTypeDef,
     MaintenanceUpdateSettingsTypeDef,
     MediaConnectFlowRequestTypeDef,
     MultiplexProgramSettingsTypeDef,
     MultiplexSettingsTypeDef,
     OutputDestinationTypeDef,
     PurchaseOfferingResponseTypeDef,
     RenewalSettingsTypeDef,
     RestartChannelPipelinesResponseTypeDef,
     StartChannelResponseTypeDef,
+    StartDeleteMonitorDeploymentResponseTypeDef,
+    StartMonitorDeploymentResponseTypeDef,
     StartMultiplexResponseTypeDef,
+    StartUpdateSignalMapResponseTypeDef,
     StopChannelResponseTypeDef,
     StopMultiplexResponseTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
     UpdateChannelClassResponseTypeDef,
     UpdateChannelResponseTypeDef,
+    UpdateCloudWatchAlarmTemplateGroupResponseTypeDef,
+    UpdateCloudWatchAlarmTemplateResponseTypeDef,
+    UpdateEventBridgeRuleTemplateGroupResponseTypeDef,
+    UpdateEventBridgeRuleTemplateResponseTypeDef,
     UpdateInputDeviceResponseTypeDef,
     UpdateInputResponseTypeDef,
     UpdateInputSecurityGroupResponseTypeDef,
     UpdateMultiplexProgramResponseTypeDef,
     UpdateMultiplexResponseTypeDef,
     UpdateReservationResponseTypeDef,
     VpcOutputSettingsTypeDef,
@@ -122,14 +155,18 @@
     InputAttachedWaiter,
     InputDeletedWaiter,
     InputDetachedWaiter,
     MultiplexCreatedWaiter,
     MultiplexDeletedWaiter,
     MultiplexRunningWaiter,
     MultiplexStoppedWaiter,
+    SignalMapCreatedWaiter,
+    SignalMapMonitorDeletedWaiter,
+    SignalMapMonitorDeployedWaiter,
+    SignalMapUpdatedWaiter,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -287,14 +324,83 @@
         Creates a new channel See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreateChannel).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_channel)
         """
 
+    def create_cloud_watch_alarm_template(
+        self,
+        *,
+        ComparisonOperator: CloudWatchAlarmTemplateComparisonOperatorType,
+        EvaluationPeriods: int,
+        GroupIdentifier: str,
+        MetricName: str,
+        Name: str,
+        Period: int,
+        Statistic: CloudWatchAlarmTemplateStatisticType,
+        TargetResourceType: CloudWatchAlarmTemplateTargetResourceTypeType,
+        Threshold: float,
+        TreatMissingData: CloudWatchAlarmTemplateTreatMissingDataType,
+        DatapointsToAlarm: int = ...,
+        Description: str = ...,
+        Tags: Mapping[str, str] = ...,
+    ) -> CreateCloudWatchAlarmTemplateResponseTypeDef:
+        """
+        Creates a cloudwatch alarm template to dynamically generate cloudwatch metric
+        alarms on targeted resource
+        types.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_cloud_watch_alarm_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_cloud_watch_alarm_template)
+        """
+
+    def create_cloud_watch_alarm_template_group(
+        self, *, Name: str, Description: str = ..., Tags: Mapping[str, str] = ...
+    ) -> CreateCloudWatchAlarmTemplateGroupResponseTypeDef:
+        """
+        Creates a cloudwatch alarm template group to group your cloudwatch alarm
+        templates and to attach to signal maps for dynamically creating
+        alarms.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_cloud_watch_alarm_template_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_cloud_watch_alarm_template_group)
+        """
+
+    def create_event_bridge_rule_template(
+        self,
+        *,
+        EventType: EventBridgeRuleTemplateEventTypeType,
+        GroupIdentifier: str,
+        Name: str,
+        Description: str = ...,
+        EventTargets: Sequence[EventBridgeRuleTemplateTargetTypeDef] = ...,
+        Tags: Mapping[str, str] = ...,
+    ) -> CreateEventBridgeRuleTemplateResponseTypeDef:
+        """
+        Creates an eventbridge rule template to monitor events and send notifications
+        to your targeted
+        resources.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_event_bridge_rule_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_event_bridge_rule_template)
+        """
+
+    def create_event_bridge_rule_template_group(
+        self, *, Name: str, Description: str = ..., Tags: Mapping[str, str] = ...
+    ) -> CreateEventBridgeRuleTemplateGroupResponseTypeDef:
+        """
+        Creates an eventbridge rule template group to group your eventbridge rule
+        templates and to attach to signal maps for dynamically creating notification
+        rules.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_event_bridge_rule_template_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_event_bridge_rule_template_group)
+        """
+
     def create_input(
         self,
         *,
         Destinations: Sequence[InputDestinationRequestTypeDef] = ...,
         InputDevices: Sequence[InputDeviceSettingsTypeDef] = ...,
         InputSecurityGroups: Sequence[str] = ...,
         MediaConnectFlows: Sequence[MediaConnectFlowRequestTypeDef] = ...,
@@ -366,14 +472,31 @@
         Create a partner input See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreatePartnerInput).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_partner_input)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_partner_input)
         """
 
+    def create_signal_map(
+        self,
+        *,
+        DiscoveryEntryPointArn: str,
+        Name: str,
+        CloudWatchAlarmTemplateGroupIdentifiers: Sequence[str] = ...,
+        Description: str = ...,
+        EventBridgeRuleTemplateGroupIdentifiers: Sequence[str] = ...,
+        Tags: Mapping[str, str] = ...,
+    ) -> CreateSignalMapResponseTypeDef:
+        """
+        Initiates the creation of a new signal map.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.create_signal_map)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#create_signal_map)
+        """
+
     def create_tags(
         self, *, ResourceArn: str, Tags: Mapping[str, str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Create tags for a resource See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/CreateTags).
 
@@ -385,14 +508,50 @@
         """
         Starts deletion of channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_channel)
         """
 
+    def delete_cloud_watch_alarm_template(self, *, Identifier: str) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes a cloudwatch alarm template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_cloud_watch_alarm_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_cloud_watch_alarm_template)
+        """
+
+    def delete_cloud_watch_alarm_template_group(
+        self, *, Identifier: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes a cloudwatch alarm template group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_cloud_watch_alarm_template_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_cloud_watch_alarm_template_group)
+        """
+
+    def delete_event_bridge_rule_template(self, *, Identifier: str) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes an eventbridge rule template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_event_bridge_rule_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_event_bridge_rule_template)
+        """
+
+    def delete_event_bridge_rule_template_group(
+        self, *, Identifier: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes an eventbridge rule template group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_event_bridge_rule_template_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_event_bridge_rule_template_group)
+        """
+
     def delete_input(self, *, InputId: str) -> Dict[str, Any]:
         """
         Deletes the input end point See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DeleteInput).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_input)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_input)
@@ -437,14 +596,22 @@
         """
         Delete all schedule actions on a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_schedule)
         """
 
+    def delete_signal_map(self, *, Identifier: str) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes the specified signal map.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_signal_map)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#delete_signal_map)
+        """
+
     def delete_tags(
         self, *, ResourceArn: str, TagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes tags for a resource See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DeleteTags).
 
@@ -574,25 +741,129 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#generate_presigned_url)
         """
 
+    def get_cloud_watch_alarm_template(
+        self, *, Identifier: str
+    ) -> GetCloudWatchAlarmTemplateResponseTypeDef:
+        """
+        Retrieves the specified cloudwatch alarm template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_cloud_watch_alarm_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_cloud_watch_alarm_template)
+        """
+
+    def get_cloud_watch_alarm_template_group(
+        self, *, Identifier: str
+    ) -> GetCloudWatchAlarmTemplateGroupResponseTypeDef:
+        """
+        Retrieves the specified cloudwatch alarm template group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_cloud_watch_alarm_template_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_cloud_watch_alarm_template_group)
+        """
+
+    def get_event_bridge_rule_template(
+        self, *, Identifier: str
+    ) -> GetEventBridgeRuleTemplateResponseTypeDef:
+        """
+        Retrieves the specified eventbridge rule template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_event_bridge_rule_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_event_bridge_rule_template)
+        """
+
+    def get_event_bridge_rule_template_group(
+        self, *, Identifier: str
+    ) -> GetEventBridgeRuleTemplateGroupResponseTypeDef:
+        """
+        Retrieves the specified eventbridge rule template group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_event_bridge_rule_template_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_event_bridge_rule_template_group)
+        """
+
+    def get_signal_map(self, *, Identifier: str) -> GetSignalMapResponseTypeDef:
+        """
+        Retrieves the specified signal map.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_signal_map)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_signal_map)
+        """
+
     def list_channels(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChannelsResponseTypeDef:
         """
         Produces list of channels that have been created See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/ListChannels).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_channels)
         """
 
+    def list_cloud_watch_alarm_template_groups(
+        self,
+        *,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        Scope: str = ...,
+        SignalMapIdentifier: str = ...,
+    ) -> ListCloudWatchAlarmTemplateGroupsResponseTypeDef:
+        """
+        Lists cloudwatch alarm template groups.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_cloud_watch_alarm_template_groups)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_cloud_watch_alarm_template_groups)
+        """
+
+    def list_cloud_watch_alarm_templates(
+        self,
+        *,
+        GroupIdentifier: str = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        Scope: str = ...,
+        SignalMapIdentifier: str = ...,
+    ) -> ListCloudWatchAlarmTemplatesResponseTypeDef:
+        """
+        Lists cloudwatch alarm templates.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_cloud_watch_alarm_templates)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_cloud_watch_alarm_templates)
+        """
+
+    def list_event_bridge_rule_template_groups(
+        self, *, MaxResults: int = ..., NextToken: str = ..., SignalMapIdentifier: str = ...
+    ) -> ListEventBridgeRuleTemplateGroupsResponseTypeDef:
+        """
+        Lists eventbridge rule template groups.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_event_bridge_rule_template_groups)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_event_bridge_rule_template_groups)
+        """
+
+    def list_event_bridge_rule_templates(
+        self,
+        *,
+        GroupIdentifier: str = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        SignalMapIdentifier: str = ...,
+    ) -> ListEventBridgeRuleTemplatesResponseTypeDef:
+        """
+        Lists eventbridge rule templates.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_event_bridge_rule_templates)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_event_bridge_rule_templates)
+        """
+
     def list_input_device_transfers(
         self, *, TransferType: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListInputDeviceTransfersResponseTypeDef:
         """
         List input devices that are currently being transferred.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_input_device_transfers)
@@ -692,14 +963,29 @@
         """
         List purchased reservations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_reservations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_reservations)
         """
 
+    def list_signal_maps(
+        self,
+        *,
+        CloudWatchAlarmTemplateGroupIdentifier: str = ...,
+        EventBridgeRuleTemplateGroupIdentifier: str = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+    ) -> ListSignalMapsResponseTypeDef:
+        """
+        Lists signal maps.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_signal_maps)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_signal_maps)
+        """
+
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Produces list of tags that have been created for a resource See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/ListTagsForResource).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#list_tags_for_resource)
@@ -756,14 +1042,24 @@
         Starts an existing channel See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/StartChannel).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_channel)
         """
 
+    def start_delete_monitor_deployment(
+        self, *, Identifier: str
+    ) -> StartDeleteMonitorDeploymentResponseTypeDef:
+        """
+        Initiates a deployment to delete the monitor of the specified signal map.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_delete_monitor_deployment)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_delete_monitor_deployment)
+        """
+
     def start_input_device(self, *, InputDeviceId: str) -> Dict[str, Any]:
         """
         Start an input device that is attached to a MediaConnect flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_input_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_input_device)
         """
@@ -772,22 +1068,50 @@
         """
         Start a maintenance window for the specified input device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_input_device_maintenance_window)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_input_device_maintenance_window)
         """
 
+    def start_monitor_deployment(
+        self, *, Identifier: str, DryRun: bool = ...
+    ) -> StartMonitorDeploymentResponseTypeDef:
+        """
+        Initiates a deployment to deploy the latest monitor of the specified signal map.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_monitor_deployment)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_monitor_deployment)
+        """
+
     def start_multiplex(self, *, MultiplexId: str) -> StartMultiplexResponseTypeDef:
         """
         Start (run) the multiplex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_multiplex)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_multiplex)
         """
 
+    def start_update_signal_map(
+        self,
+        *,
+        Identifier: str,
+        CloudWatchAlarmTemplateGroupIdentifiers: Sequence[str] = ...,
+        Description: str = ...,
+        DiscoveryEntryPointArn: str = ...,
+        EventBridgeRuleTemplateGroupIdentifiers: Sequence[str] = ...,
+        ForceRediscovery: bool = ...,
+        Name: str = ...,
+    ) -> StartUpdateSignalMapResponseTypeDef:
+        """
+        Initiates an update for the specified signal map.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.start_update_signal_map)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#start_update_signal_map)
+        """
+
     def stop_channel(self, *, ChannelId: str) -> StopChannelResponseTypeDef:
         """
         Stops a running channel See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/StopChannel).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.stop_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#stop_channel)
@@ -866,14 +1190,75 @@
         """
         Changes the class of the channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_channel_class)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_channel_class)
         """
 
+    def update_cloud_watch_alarm_template(
+        self,
+        *,
+        Identifier: str,
+        ComparisonOperator: CloudWatchAlarmTemplateComparisonOperatorType = ...,
+        DatapointsToAlarm: int = ...,
+        Description: str = ...,
+        EvaluationPeriods: int = ...,
+        GroupIdentifier: str = ...,
+        MetricName: str = ...,
+        Name: str = ...,
+        Period: int = ...,
+        Statistic: CloudWatchAlarmTemplateStatisticType = ...,
+        TargetResourceType: CloudWatchAlarmTemplateTargetResourceTypeType = ...,
+        Threshold: float = ...,
+        TreatMissingData: CloudWatchAlarmTemplateTreatMissingDataType = ...,
+    ) -> UpdateCloudWatchAlarmTemplateResponseTypeDef:
+        """
+        Updates the specified cloudwatch alarm template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_cloud_watch_alarm_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_cloud_watch_alarm_template)
+        """
+
+    def update_cloud_watch_alarm_template_group(
+        self, *, Identifier: str, Description: str = ...
+    ) -> UpdateCloudWatchAlarmTemplateGroupResponseTypeDef:
+        """
+        Updates the specified cloudwatch alarm template group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_cloud_watch_alarm_template_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_cloud_watch_alarm_template_group)
+        """
+
+    def update_event_bridge_rule_template(
+        self,
+        *,
+        Identifier: str,
+        Description: str = ...,
+        EventTargets: Sequence[EventBridgeRuleTemplateTargetTypeDef] = ...,
+        EventType: EventBridgeRuleTemplateEventTypeType = ...,
+        GroupIdentifier: str = ...,
+        Name: str = ...,
+    ) -> UpdateEventBridgeRuleTemplateResponseTypeDef:
+        """
+        Updates the specified eventbridge rule template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_event_bridge_rule_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_event_bridge_rule_template)
+        """
+
+    def update_event_bridge_rule_template_group(
+        self, *, Identifier: str, Description: str = ...
+    ) -> UpdateEventBridgeRuleTemplateGroupResponseTypeDef:
+        """
+        Updates the specified eventbridge rule template group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_event_bridge_rule_template_group)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_event_bridge_rule_template_group)
+        """
+
     def update_input(
         self,
         *,
         InputId: str,
         Destinations: Sequence[InputDestinationRequestTypeDef] = ...,
         InputDevices: Sequence[InputDeviceRequestTypeDef] = ...,
         InputSecurityGroups: Sequence[str] = ...,
@@ -971,14 +1356,50 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_cloud_watch_alarm_template_groups"]
+    ) -> ListCloudWatchAlarmTemplateGroupsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_cloud_watch_alarm_templates"]
+    ) -> ListCloudWatchAlarmTemplatesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_event_bridge_rule_template_groups"]
+    ) -> ListEventBridgeRuleTemplateGroupsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_event_bridge_rule_templates"]
+    ) -> ListEventBridgeRuleTemplatesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_input_device_transfers"]
     ) -> ListInputDeviceTransfersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
 
@@ -1038,14 +1459,21 @@
     ) -> ListReservationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(self, operation_name: Literal["list_signal_maps"]) -> ListSignalMapsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_paginator)
+        """
+
+    @overload
     def get_waiter(self, waiter_name: Literal["channel_created"]) -> ChannelCreatedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
 
     @overload
@@ -1113,7 +1541,39 @@
 
     @overload
     def get_waiter(self, waiter_name: Literal["multiplex_stopped"]) -> MultiplexStoppedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
         """
+
+    @overload
+    def get_waiter(self, waiter_name: Literal["signal_map_created"]) -> SignalMapCreatedWaiter:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
+        """
+
+    @overload
+    def get_waiter(
+        self, waiter_name: Literal["signal_map_monitor_deleted"]
+    ) -> SignalMapMonitorDeletedWaiter:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
+        """
+
+    @overload
+    def get_waiter(
+        self, waiter_name: Literal["signal_map_monitor_deployed"]
+    ) -> SignalMapMonitorDeployedWaiter:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
+        """
+
+    @overload
+    def get_waiter(self, waiter_name: Literal["signal_map_updated"]) -> SignalMapUpdatedWaiter:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.get_waiter)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#get_waiter)
+        """
```

### Comparing `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/literals.py` & `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,18 @@
     "ChannelClassType",
     "ChannelCreatedWaiterName",
     "ChannelDeletedWaiterName",
     "ChannelPipelineIdToRestartType",
     "ChannelRunningWaiterName",
     "ChannelStateType",
     "ChannelStoppedWaiterName",
+    "CloudWatchAlarmTemplateComparisonOperatorType",
+    "CloudWatchAlarmTemplateStatisticType",
+    "CloudWatchAlarmTemplateTargetResourceTypeType",
+    "CloudWatchAlarmTemplateTreatMissingDataType",
     "CmafIngestSegmentLengthUnitsType",
     "CmafNielsenId3BehaviorType",
     "ColorSpaceType",
     "ContentTypeType",
     "DashRoleAudioType",
     "DashRoleCaptionType",
     "DescribeSchedulePaginatorName",
@@ -98,14 +102,15 @@
     "Eac3StereoDownmixType",
     "Eac3SurroundExModeType",
     "Eac3SurroundModeType",
     "EbuTtDDestinationStyleControlType",
     "EbuTtDFillLineGapControlType",
     "EmbeddedConvert608To708Type",
     "EmbeddedScte20DetectionType",
+    "EventBridgeRuleTemplateEventTypeType",
     "FeatureActivationsInputPrepareScheduleActionsType",
     "FeatureActivationsOutputStaticImageOverlayScheduleActionsType",
     "FecOutputIncludeFecType",
     "FixedAfdType",
     "Fmp4NielsenId3BehaviorType",
     "Fmp4TimedMetadataBehaviorType",
     "FollowPointType",
@@ -213,22 +218,27 @@
     "InputSourceEndBehaviorType",
     "InputSourceTypeType",
     "InputStateType",
     "InputTimecodeSourceType",
     "InputTypeType",
     "LastFrameClippingBehaviorType",
     "ListChannelsPaginatorName",
+    "ListCloudWatchAlarmTemplateGroupsPaginatorName",
+    "ListCloudWatchAlarmTemplatesPaginatorName",
+    "ListEventBridgeRuleTemplateGroupsPaginatorName",
+    "ListEventBridgeRuleTemplatesPaginatorName",
     "ListInputDeviceTransfersPaginatorName",
     "ListInputDevicesPaginatorName",
     "ListInputSecurityGroupsPaginatorName",
     "ListInputsPaginatorName",
     "ListMultiplexProgramsPaginatorName",
     "ListMultiplexesPaginatorName",
     "ListOfferingsPaginatorName",
     "ListReservationsPaginatorName",
+    "ListSignalMapsPaginatorName",
     "LogLevelType",
     "M2tsAbsentInputAudioBehaviorType",
     "M2tsAribCaptionsPidControlType",
     "M2tsAribType",
     "M2tsAudioBufferModelType",
     "M2tsAudioIntervalType",
     "M2tsAudioStreamTypeType",
@@ -300,14 +310,20 @@
     "Scte35InputModeType",
     "Scte35NoRegionalBlackoutFlagType",
     "Scte35SegmentationCancelIndicatorType",
     "Scte35SpliceInsertNoRegionalBlackoutBehaviorType",
     "Scte35SpliceInsertWebDeliveryAllowedBehaviorType",
     "Scte35TypeType",
     "Scte35WebDeliveryAllowedFlagType",
+    "SignalMapCreatedWaiterName",
+    "SignalMapMonitorDeletedWaiterName",
+    "SignalMapMonitorDeployedWaiterName",
+    "SignalMapMonitorDeploymentStatusType",
+    "SignalMapStatusType",
+    "SignalMapUpdatedWaiterName",
     "SmoothGroupAudioOnlyTimecodeControlType",
     "SmoothGroupCertificateModeType",
     "SmoothGroupEventIdModeType",
     "SmoothGroupEventStopBehaviorType",
     "SmoothGroupSegmentationModeType",
     "SmoothGroupSparseTrackTypeType",
     "SmoothGroupStreamManifestBehaviorType",
@@ -408,14 +424,36 @@
     "RUNNING",
     "STARTING",
     "STOPPING",
     "UPDATE_FAILED",
     "UPDATING",
 ]
 ChannelStoppedWaiterName = Literal["channel_stopped"]
+CloudWatchAlarmTemplateComparisonOperatorType = Literal[
+    "GreaterThanOrEqualToThreshold",
+    "GreaterThanThreshold",
+    "LessThanOrEqualToThreshold",
+    "LessThanThreshold",
+]
+CloudWatchAlarmTemplateStatisticType = Literal[
+    "Average", "Maximum", "Minimum", "SampleCount", "Sum"
+]
+CloudWatchAlarmTemplateTargetResourceTypeType = Literal[
+    "CLOUDFRONT_DISTRIBUTION",
+    "MEDIACONNECT_FLOW",
+    "MEDIALIVE_CHANNEL",
+    "MEDIALIVE_INPUT_DEVICE",
+    "MEDIALIVE_MULTIPLEX",
+    "MEDIAPACKAGE_CHANNEL",
+    "MEDIAPACKAGE_ORIGIN_ENDPOINT",
+    "S3_BUCKET",
+]
+CloudWatchAlarmTemplateTreatMissingDataType = Literal[
+    "breaching", "ignore", "missing", "notBreaching"
+]
 CmafIngestSegmentLengthUnitsType = Literal["MILLISECONDS", "SECONDS"]
 CmafNielsenId3BehaviorType = Literal["NO_PASSTHROUGH", "PASSTHROUGH"]
 ColorSpaceType = Literal["HDR10", "HLG_2020", "REC_601", "REC_709"]
 ContentTypeType = Literal["image/jpeg"]
 DashRoleAudioType = Literal[
     "ALTERNATE",
     "COMMENTARY",
@@ -500,14 +538,29 @@
 Eac3StereoDownmixType = Literal["DPL2", "LO_RO", "LT_RT", "NOT_INDICATED"]
 Eac3SurroundExModeType = Literal["DISABLED", "ENABLED", "NOT_INDICATED"]
 Eac3SurroundModeType = Literal["DISABLED", "ENABLED", "NOT_INDICATED"]
 EbuTtDDestinationStyleControlType = Literal["EXCLUDE", "INCLUDE"]
 EbuTtDFillLineGapControlType = Literal["DISABLED", "ENABLED"]
 EmbeddedConvert608To708Type = Literal["DISABLED", "UPCONVERT"]
 EmbeddedScte20DetectionType = Literal["AUTO", "OFF"]
+EventBridgeRuleTemplateEventTypeType = Literal[
+    "MEDIACONNECT_ALERT",
+    "MEDIACONNECT_FLOW_STATUS_CHANGE",
+    "MEDIACONNECT_OUTPUT_HEALTH",
+    "MEDIACONNECT_SOURCE_HEALTH",
+    "MEDIALIVE_CHANNEL_ALERT",
+    "MEDIALIVE_CHANNEL_INPUT_CHANGE",
+    "MEDIALIVE_CHANNEL_STATE_CHANGE",
+    "MEDIALIVE_MULTIPLEX_ALERT",
+    "MEDIALIVE_MULTIPLEX_STATE_CHANGE",
+    "MEDIAPACKAGE_HARVEST_JOB_NOTIFICATION",
+    "MEDIAPACKAGE_INPUT_NOTIFICATION",
+    "MEDIAPACKAGE_KEY_PROVIDER_NOTIFICATION",
+    "SIGNAL_MAP_ACTIVE_ALARM",
+]
 FeatureActivationsInputPrepareScheduleActionsType = Literal["DISABLED", "ENABLED"]
 FeatureActivationsOutputStaticImageOverlayScheduleActionsType = Literal["DISABLED", "ENABLED"]
 FecOutputIncludeFecType = Literal["COLUMN", "COLUMN_AND_ROW"]
 FixedAfdType = Literal[
     "AFD_0000",
     "AFD_0010",
     "AFD_0011",
@@ -691,22 +744,27 @@
     "RTP_PUSH",
     "TS_FILE",
     "UDP_PUSH",
     "URL_PULL",
 ]
 LastFrameClippingBehaviorType = Literal["EXCLUDE_LAST_FRAME", "INCLUDE_LAST_FRAME"]
 ListChannelsPaginatorName = Literal["list_channels"]
+ListCloudWatchAlarmTemplateGroupsPaginatorName = Literal["list_cloud_watch_alarm_template_groups"]
+ListCloudWatchAlarmTemplatesPaginatorName = Literal["list_cloud_watch_alarm_templates"]
+ListEventBridgeRuleTemplateGroupsPaginatorName = Literal["list_event_bridge_rule_template_groups"]
+ListEventBridgeRuleTemplatesPaginatorName = Literal["list_event_bridge_rule_templates"]
 ListInputDeviceTransfersPaginatorName = Literal["list_input_device_transfers"]
 ListInputDevicesPaginatorName = Literal["list_input_devices"]
 ListInputSecurityGroupsPaginatorName = Literal["list_input_security_groups"]
 ListInputsPaginatorName = Literal["list_inputs"]
 ListMultiplexProgramsPaginatorName = Literal["list_multiplex_programs"]
 ListMultiplexesPaginatorName = Literal["list_multiplexes"]
 ListOfferingsPaginatorName = Literal["list_offerings"]
 ListReservationsPaginatorName = Literal["list_reservations"]
+ListSignalMapsPaginatorName = Literal["list_signal_maps"]
 LogLevelType = Literal["DEBUG", "DISABLED", "ERROR", "INFO", "WARNING"]
 M2tsAbsentInputAudioBehaviorType = Literal["DROP", "ENCODE_SILENCE"]
 M2tsAribCaptionsPidControlType = Literal["AUTO", "USE_CONFIGURED"]
 M2tsAribType = Literal["DISABLED", "ENABLED"]
 M2tsAudioBufferModelType = Literal["ATSC", "DVB"]
 M2tsAudioIntervalType = Literal["VIDEO_AND_FIXED_INTERVALS", "VIDEO_INTERVAL"]
 M2tsAudioStreamTypeType = Literal["ATSC", "DVB"]
@@ -811,14 +869,41 @@
 Scte35SegmentationCancelIndicatorType = Literal[
     "SEGMENTATION_EVENT_CANCELED", "SEGMENTATION_EVENT_NOT_CANCELED"
 ]
 Scte35SpliceInsertNoRegionalBlackoutBehaviorType = Literal["FOLLOW", "IGNORE"]
 Scte35SpliceInsertWebDeliveryAllowedBehaviorType = Literal["FOLLOW", "IGNORE"]
 Scte35TypeType = Literal["NONE", "SCTE_35_WITHOUT_SEGMENTATION"]
 Scte35WebDeliveryAllowedFlagType = Literal["WEB_DELIVERY_ALLOWED", "WEB_DELIVERY_NOT_ALLOWED"]
+SignalMapCreatedWaiterName = Literal["signal_map_created"]
+SignalMapMonitorDeletedWaiterName = Literal["signal_map_monitor_deleted"]
+SignalMapMonitorDeployedWaiterName = Literal["signal_map_monitor_deployed"]
+SignalMapMonitorDeploymentStatusType = Literal[
+    "DELETE_COMPLETE",
+    "DELETE_FAILED",
+    "DELETE_IN_PROGRESS",
+    "DEPLOYMENT_COMPLETE",
+    "DEPLOYMENT_FAILED",
+    "DEPLOYMENT_IN_PROGRESS",
+    "DRY_RUN_DEPLOYMENT_COMPLETE",
+    "DRY_RUN_DEPLOYMENT_FAILED",
+    "DRY_RUN_DEPLOYMENT_IN_PROGRESS",
+    "NOT_DEPLOYED",
+]
+SignalMapStatusType = Literal[
+    "CREATE_COMPLETE",
+    "CREATE_FAILED",
+    "CREATE_IN_PROGRESS",
+    "NOT_READY",
+    "READY",
+    "UPDATE_COMPLETE",
+    "UPDATE_FAILED",
+    "UPDATE_IN_PROGRESS",
+    "UPDATE_REVERTED",
+]
+SignalMapUpdatedWaiterName = Literal["signal_map_updated"]
 SmoothGroupAudioOnlyTimecodeControlType = Literal["PASSTHROUGH", "USE_CONFIGURED_CLOCK"]
 SmoothGroupCertificateModeType = Literal["SELF_SIGNED", "VERIFY_AUTHENTICITY"]
 SmoothGroupEventIdModeType = Literal["NO_EVENT_ID", "USE_CONFIGURED", "USE_TIMESTAMP"]
 SmoothGroupEventStopBehaviorType = Literal["NONE", "SEND_EOS"]
 SmoothGroupSegmentationModeType = Literal["USE_INPUT_SEGMENTATION", "USE_SEGMENT_DURATION"]
 SmoothGroupSparseTrackTypeType = Literal["NONE", "SCTE_35", "SCTE_35_WITHOUT_SEGMENTATION"]
 SmoothGroupStreamManifestBehaviorType = Literal["DO_NOT_SEND", "SEND"]
@@ -958,14 +1043,15 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
@@ -1264,35 +1350,44 @@
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "describe_schedule",
     "list_channels",
+    "list_cloud_watch_alarm_template_groups",
+    "list_cloud_watch_alarm_templates",
+    "list_event_bridge_rule_template_groups",
+    "list_event_bridge_rule_templates",
     "list_input_device_transfers",
     "list_input_devices",
     "list_input_security_groups",
     "list_inputs",
     "list_multiplex_programs",
     "list_multiplexes",
     "list_offerings",
     "list_reservations",
+    "list_signal_maps",
 ]
 WaiterName = Literal[
     "channel_created",
     "channel_deleted",
     "channel_running",
     "channel_stopped",
     "input_attached",
     "input_deleted",
     "input_detached",
     "multiplex_created",
     "multiplex_deleted",
     "multiplex_running",
     "multiplex_stopped",
+    "signal_map_created",
+    "signal_map_monitor_deleted",
+    "signal_map_monitor_deployed",
+    "signal_map_updated",
 ]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
```

### Comparing `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/literals.pyi` & `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,18 @@
     "ChannelClassType",
     "ChannelCreatedWaiterName",
     "ChannelDeletedWaiterName",
     "ChannelPipelineIdToRestartType",
     "ChannelRunningWaiterName",
     "ChannelStateType",
     "ChannelStoppedWaiterName",
+    "CloudWatchAlarmTemplateComparisonOperatorType",
+    "CloudWatchAlarmTemplateStatisticType",
+    "CloudWatchAlarmTemplateTargetResourceTypeType",
+    "CloudWatchAlarmTemplateTreatMissingDataType",
     "CmafIngestSegmentLengthUnitsType",
     "CmafNielsenId3BehaviorType",
     "ColorSpaceType",
     "ContentTypeType",
     "DashRoleAudioType",
     "DashRoleCaptionType",
     "DescribeSchedulePaginatorName",
@@ -98,14 +102,15 @@
     "Eac3StereoDownmixType",
     "Eac3SurroundExModeType",
     "Eac3SurroundModeType",
     "EbuTtDDestinationStyleControlType",
     "EbuTtDFillLineGapControlType",
     "EmbeddedConvert608To708Type",
     "EmbeddedScte20DetectionType",
+    "EventBridgeRuleTemplateEventTypeType",
     "FeatureActivationsInputPrepareScheduleActionsType",
     "FeatureActivationsOutputStaticImageOverlayScheduleActionsType",
     "FecOutputIncludeFecType",
     "FixedAfdType",
     "Fmp4NielsenId3BehaviorType",
     "Fmp4TimedMetadataBehaviorType",
     "FollowPointType",
@@ -213,22 +218,27 @@
     "InputSourceEndBehaviorType",
     "InputSourceTypeType",
     "InputStateType",
     "InputTimecodeSourceType",
     "InputTypeType",
     "LastFrameClippingBehaviorType",
     "ListChannelsPaginatorName",
+    "ListCloudWatchAlarmTemplateGroupsPaginatorName",
+    "ListCloudWatchAlarmTemplatesPaginatorName",
+    "ListEventBridgeRuleTemplateGroupsPaginatorName",
+    "ListEventBridgeRuleTemplatesPaginatorName",
     "ListInputDeviceTransfersPaginatorName",
     "ListInputDevicesPaginatorName",
     "ListInputSecurityGroupsPaginatorName",
     "ListInputsPaginatorName",
     "ListMultiplexProgramsPaginatorName",
     "ListMultiplexesPaginatorName",
     "ListOfferingsPaginatorName",
     "ListReservationsPaginatorName",
+    "ListSignalMapsPaginatorName",
     "LogLevelType",
     "M2tsAbsentInputAudioBehaviorType",
     "M2tsAribCaptionsPidControlType",
     "M2tsAribType",
     "M2tsAudioBufferModelType",
     "M2tsAudioIntervalType",
     "M2tsAudioStreamTypeType",
@@ -300,14 +310,20 @@
     "Scte35InputModeType",
     "Scte35NoRegionalBlackoutFlagType",
     "Scte35SegmentationCancelIndicatorType",
     "Scte35SpliceInsertNoRegionalBlackoutBehaviorType",
     "Scte35SpliceInsertWebDeliveryAllowedBehaviorType",
     "Scte35TypeType",
     "Scte35WebDeliveryAllowedFlagType",
+    "SignalMapCreatedWaiterName",
+    "SignalMapMonitorDeletedWaiterName",
+    "SignalMapMonitorDeployedWaiterName",
+    "SignalMapMonitorDeploymentStatusType",
+    "SignalMapStatusType",
+    "SignalMapUpdatedWaiterName",
     "SmoothGroupAudioOnlyTimecodeControlType",
     "SmoothGroupCertificateModeType",
     "SmoothGroupEventIdModeType",
     "SmoothGroupEventStopBehaviorType",
     "SmoothGroupSegmentationModeType",
     "SmoothGroupSparseTrackTypeType",
     "SmoothGroupStreamManifestBehaviorType",
@@ -408,14 +424,36 @@
     "RUNNING",
     "STARTING",
     "STOPPING",
     "UPDATE_FAILED",
     "UPDATING",
 ]
 ChannelStoppedWaiterName = Literal["channel_stopped"]
+CloudWatchAlarmTemplateComparisonOperatorType = Literal[
+    "GreaterThanOrEqualToThreshold",
+    "GreaterThanThreshold",
+    "LessThanOrEqualToThreshold",
+    "LessThanThreshold",
+]
+CloudWatchAlarmTemplateStatisticType = Literal[
+    "Average", "Maximum", "Minimum", "SampleCount", "Sum"
+]
+CloudWatchAlarmTemplateTargetResourceTypeType = Literal[
+    "CLOUDFRONT_DISTRIBUTION",
+    "MEDIACONNECT_FLOW",
+    "MEDIALIVE_CHANNEL",
+    "MEDIALIVE_INPUT_DEVICE",
+    "MEDIALIVE_MULTIPLEX",
+    "MEDIAPACKAGE_CHANNEL",
+    "MEDIAPACKAGE_ORIGIN_ENDPOINT",
+    "S3_BUCKET",
+]
+CloudWatchAlarmTemplateTreatMissingDataType = Literal[
+    "breaching", "ignore", "missing", "notBreaching"
+]
 CmafIngestSegmentLengthUnitsType = Literal["MILLISECONDS", "SECONDS"]
 CmafNielsenId3BehaviorType = Literal["NO_PASSTHROUGH", "PASSTHROUGH"]
 ColorSpaceType = Literal["HDR10", "HLG_2020", "REC_601", "REC_709"]
 ContentTypeType = Literal["image/jpeg"]
 DashRoleAudioType = Literal[
     "ALTERNATE",
     "COMMENTARY",
@@ -500,14 +538,29 @@
 Eac3StereoDownmixType = Literal["DPL2", "LO_RO", "LT_RT", "NOT_INDICATED"]
 Eac3SurroundExModeType = Literal["DISABLED", "ENABLED", "NOT_INDICATED"]
 Eac3SurroundModeType = Literal["DISABLED", "ENABLED", "NOT_INDICATED"]
 EbuTtDDestinationStyleControlType = Literal["EXCLUDE", "INCLUDE"]
 EbuTtDFillLineGapControlType = Literal["DISABLED", "ENABLED"]
 EmbeddedConvert608To708Type = Literal["DISABLED", "UPCONVERT"]
 EmbeddedScte20DetectionType = Literal["AUTO", "OFF"]
+EventBridgeRuleTemplateEventTypeType = Literal[
+    "MEDIACONNECT_ALERT",
+    "MEDIACONNECT_FLOW_STATUS_CHANGE",
+    "MEDIACONNECT_OUTPUT_HEALTH",
+    "MEDIACONNECT_SOURCE_HEALTH",
+    "MEDIALIVE_CHANNEL_ALERT",
+    "MEDIALIVE_CHANNEL_INPUT_CHANGE",
+    "MEDIALIVE_CHANNEL_STATE_CHANGE",
+    "MEDIALIVE_MULTIPLEX_ALERT",
+    "MEDIALIVE_MULTIPLEX_STATE_CHANGE",
+    "MEDIAPACKAGE_HARVEST_JOB_NOTIFICATION",
+    "MEDIAPACKAGE_INPUT_NOTIFICATION",
+    "MEDIAPACKAGE_KEY_PROVIDER_NOTIFICATION",
+    "SIGNAL_MAP_ACTIVE_ALARM",
+]
 FeatureActivationsInputPrepareScheduleActionsType = Literal["DISABLED", "ENABLED"]
 FeatureActivationsOutputStaticImageOverlayScheduleActionsType = Literal["DISABLED", "ENABLED"]
 FecOutputIncludeFecType = Literal["COLUMN", "COLUMN_AND_ROW"]
 FixedAfdType = Literal[
     "AFD_0000",
     "AFD_0010",
     "AFD_0011",
@@ -691,22 +744,27 @@
     "RTP_PUSH",
     "TS_FILE",
     "UDP_PUSH",
     "URL_PULL",
 ]
 LastFrameClippingBehaviorType = Literal["EXCLUDE_LAST_FRAME", "INCLUDE_LAST_FRAME"]
 ListChannelsPaginatorName = Literal["list_channels"]
+ListCloudWatchAlarmTemplateGroupsPaginatorName = Literal["list_cloud_watch_alarm_template_groups"]
+ListCloudWatchAlarmTemplatesPaginatorName = Literal["list_cloud_watch_alarm_templates"]
+ListEventBridgeRuleTemplateGroupsPaginatorName = Literal["list_event_bridge_rule_template_groups"]
+ListEventBridgeRuleTemplatesPaginatorName = Literal["list_event_bridge_rule_templates"]
 ListInputDeviceTransfersPaginatorName = Literal["list_input_device_transfers"]
 ListInputDevicesPaginatorName = Literal["list_input_devices"]
 ListInputSecurityGroupsPaginatorName = Literal["list_input_security_groups"]
 ListInputsPaginatorName = Literal["list_inputs"]
 ListMultiplexProgramsPaginatorName = Literal["list_multiplex_programs"]
 ListMultiplexesPaginatorName = Literal["list_multiplexes"]
 ListOfferingsPaginatorName = Literal["list_offerings"]
 ListReservationsPaginatorName = Literal["list_reservations"]
+ListSignalMapsPaginatorName = Literal["list_signal_maps"]
 LogLevelType = Literal["DEBUG", "DISABLED", "ERROR", "INFO", "WARNING"]
 M2tsAbsentInputAudioBehaviorType = Literal["DROP", "ENCODE_SILENCE"]
 M2tsAribCaptionsPidControlType = Literal["AUTO", "USE_CONFIGURED"]
 M2tsAribType = Literal["DISABLED", "ENABLED"]
 M2tsAudioBufferModelType = Literal["ATSC", "DVB"]
 M2tsAudioIntervalType = Literal["VIDEO_AND_FIXED_INTERVALS", "VIDEO_INTERVAL"]
 M2tsAudioStreamTypeType = Literal["ATSC", "DVB"]
@@ -811,14 +869,41 @@
 Scte35SegmentationCancelIndicatorType = Literal[
     "SEGMENTATION_EVENT_CANCELED", "SEGMENTATION_EVENT_NOT_CANCELED"
 ]
 Scte35SpliceInsertNoRegionalBlackoutBehaviorType = Literal["FOLLOW", "IGNORE"]
 Scte35SpliceInsertWebDeliveryAllowedBehaviorType = Literal["FOLLOW", "IGNORE"]
 Scte35TypeType = Literal["NONE", "SCTE_35_WITHOUT_SEGMENTATION"]
 Scte35WebDeliveryAllowedFlagType = Literal["WEB_DELIVERY_ALLOWED", "WEB_DELIVERY_NOT_ALLOWED"]
+SignalMapCreatedWaiterName = Literal["signal_map_created"]
+SignalMapMonitorDeletedWaiterName = Literal["signal_map_monitor_deleted"]
+SignalMapMonitorDeployedWaiterName = Literal["signal_map_monitor_deployed"]
+SignalMapMonitorDeploymentStatusType = Literal[
+    "DELETE_COMPLETE",
+    "DELETE_FAILED",
+    "DELETE_IN_PROGRESS",
+    "DEPLOYMENT_COMPLETE",
+    "DEPLOYMENT_FAILED",
+    "DEPLOYMENT_IN_PROGRESS",
+    "DRY_RUN_DEPLOYMENT_COMPLETE",
+    "DRY_RUN_DEPLOYMENT_FAILED",
+    "DRY_RUN_DEPLOYMENT_IN_PROGRESS",
+    "NOT_DEPLOYED",
+]
+SignalMapStatusType = Literal[
+    "CREATE_COMPLETE",
+    "CREATE_FAILED",
+    "CREATE_IN_PROGRESS",
+    "NOT_READY",
+    "READY",
+    "UPDATE_COMPLETE",
+    "UPDATE_FAILED",
+    "UPDATE_IN_PROGRESS",
+    "UPDATE_REVERTED",
+]
+SignalMapUpdatedWaiterName = Literal["signal_map_updated"]
 SmoothGroupAudioOnlyTimecodeControlType = Literal["PASSTHROUGH", "USE_CONFIGURED_CLOCK"]
 SmoothGroupCertificateModeType = Literal["SELF_SIGNED", "VERIFY_AUTHENTICITY"]
 SmoothGroupEventIdModeType = Literal["NO_EVENT_ID", "USE_CONFIGURED", "USE_TIMESTAMP"]
 SmoothGroupEventStopBehaviorType = Literal["NONE", "SEND_EOS"]
 SmoothGroupSegmentationModeType = Literal["USE_INPUT_SEGMENTATION", "USE_SEGMENT_DURATION"]
 SmoothGroupSparseTrackTypeType = Literal["NONE", "SCTE_35", "SCTE_35_WITHOUT_SEGMENTATION"]
 SmoothGroupStreamManifestBehaviorType = Literal["DO_NOT_SEND", "SEND"]
@@ -958,14 +1043,15 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
@@ -1264,35 +1350,44 @@
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "describe_schedule",
     "list_channels",
+    "list_cloud_watch_alarm_template_groups",
+    "list_cloud_watch_alarm_templates",
+    "list_event_bridge_rule_template_groups",
+    "list_event_bridge_rule_templates",
     "list_input_device_transfers",
     "list_input_devices",
     "list_input_security_groups",
     "list_inputs",
     "list_multiplex_programs",
     "list_multiplexes",
     "list_offerings",
     "list_reservations",
+    "list_signal_maps",
 ]
 WaiterName = Literal[
     "channel_created",
     "channel_deleted",
     "channel_running",
     "channel_stopped",
     "input_attached",
     "input_deleted",
     "input_detached",
     "multiplex_created",
     "multiplex_deleted",
     "multiplex_running",
     "multiplex_stopped",
+    "signal_map_created",
+    "signal_map_monitor_deleted",
+    "signal_map_monitor_deployed",
+    "signal_map_updated",
 ]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
```

### Comparing `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/paginator.py` & `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/paginator.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -8,110 +8,195 @@
     ```python
     from boto3.session import Session
 
     from mypy_boto3_medialive.client import MediaLiveClient
     from mypy_boto3_medialive.paginator import (
         DescribeSchedulePaginator,
         ListChannelsPaginator,
+        ListCloudWatchAlarmTemplateGroupsPaginator,
+        ListCloudWatchAlarmTemplatesPaginator,
+        ListEventBridgeRuleTemplateGroupsPaginator,
+        ListEventBridgeRuleTemplatesPaginator,
         ListInputDeviceTransfersPaginator,
         ListInputDevicesPaginator,
         ListInputSecurityGroupsPaginator,
         ListInputsPaginator,
         ListMultiplexProgramsPaginator,
         ListMultiplexesPaginator,
         ListOfferingsPaginator,
         ListReservationsPaginator,
+        ListSignalMapsPaginator,
     )
 
     session = Session()
     client: MediaLiveClient = session.client("medialive")
 
     describe_schedule_paginator: DescribeSchedulePaginator = client.get_paginator("describe_schedule")
     list_channels_paginator: ListChannelsPaginator = client.get_paginator("list_channels")
+    list_cloud_watch_alarm_template_groups_paginator: ListCloudWatchAlarmTemplateGroupsPaginator = client.get_paginator("list_cloud_watch_alarm_template_groups")
+    list_cloud_watch_alarm_templates_paginator: ListCloudWatchAlarmTemplatesPaginator = client.get_paginator("list_cloud_watch_alarm_templates")
+    list_event_bridge_rule_template_groups_paginator: ListEventBridgeRuleTemplateGroupsPaginator = client.get_paginator("list_event_bridge_rule_template_groups")
+    list_event_bridge_rule_templates_paginator: ListEventBridgeRuleTemplatesPaginator = client.get_paginator("list_event_bridge_rule_templates")
     list_input_device_transfers_paginator: ListInputDeviceTransfersPaginator = client.get_paginator("list_input_device_transfers")
     list_input_devices_paginator: ListInputDevicesPaginator = client.get_paginator("list_input_devices")
     list_input_security_groups_paginator: ListInputSecurityGroupsPaginator = client.get_paginator("list_input_security_groups")
     list_inputs_paginator: ListInputsPaginator = client.get_paginator("list_inputs")
     list_multiplex_programs_paginator: ListMultiplexProgramsPaginator = client.get_paginator("list_multiplex_programs")
     list_multiplexes_paginator: ListMultiplexesPaginator = client.get_paginator("list_multiplexes")
     list_offerings_paginator: ListOfferingsPaginator = client.get_paginator("list_offerings")
     list_reservations_paginator: ListReservationsPaginator = client.get_paginator("list_reservations")
+    list_signal_maps_paginator: ListSignalMapsPaginator = client.get_paginator("list_signal_maps")
     ```
 """
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     DescribeScheduleResponsePaginatorTypeDef,
     ListChannelsResponsePaginatorTypeDef,
+    ListCloudWatchAlarmTemplateGroupsResponseTypeDef,
+    ListCloudWatchAlarmTemplatesResponseTypeDef,
+    ListEventBridgeRuleTemplateGroupsResponseTypeDef,
+    ListEventBridgeRuleTemplatesResponseTypeDef,
     ListInputDevicesResponseTypeDef,
     ListInputDeviceTransfersResponseTypeDef,
     ListInputSecurityGroupsResponseTypeDef,
     ListInputsResponseTypeDef,
     ListMultiplexesResponseTypeDef,
     ListMultiplexProgramsResponseTypeDef,
     ListOfferingsResponseTypeDef,
     ListReservationsResponseTypeDef,
+    ListSignalMapsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "DescribeSchedulePaginator",
     "ListChannelsPaginator",
+    "ListCloudWatchAlarmTemplateGroupsPaginator",
+    "ListCloudWatchAlarmTemplatesPaginator",
+    "ListEventBridgeRuleTemplateGroupsPaginator",
+    "ListEventBridgeRuleTemplatesPaginator",
     "ListInputDeviceTransfersPaginator",
     "ListInputDevicesPaginator",
     "ListInputSecurityGroupsPaginator",
     "ListInputsPaginator",
     "ListMultiplexProgramsPaginator",
     "ListMultiplexesPaginator",
     "ListOfferingsPaginator",
     "ListReservationsPaginator",
+    "ListSignalMapsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeSchedulePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
     """
 
     def paginate(
         self, *, ChannelId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeScheduleResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
         """
 
-
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChannelsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
         """
 
+class ListCloudWatchAlarmTemplateGroupsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListCloudWatchAlarmTemplateGroups)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listcloudwatchalarmtemplategroupspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        Scope: str = ...,
+        SignalMapIdentifier: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListCloudWatchAlarmTemplateGroupsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListCloudWatchAlarmTemplateGroups.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listcloudwatchalarmtemplategroupspaginator)
+        """
+
+class ListCloudWatchAlarmTemplatesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListCloudWatchAlarmTemplates)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listcloudwatchalarmtemplatespaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        GroupIdentifier: str = ...,
+        Scope: str = ...,
+        SignalMapIdentifier: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListCloudWatchAlarmTemplatesResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListCloudWatchAlarmTemplates.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listcloudwatchalarmtemplatespaginator)
+        """
+
+class ListEventBridgeRuleTemplateGroupsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListEventBridgeRuleTemplateGroups)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listeventbridgeruletemplategroupspaginator)
+    """
+
+    def paginate(
+        self, *, SignalMapIdentifier: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[ListEventBridgeRuleTemplateGroupsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListEventBridgeRuleTemplateGroups.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listeventbridgeruletemplategroupspaginator)
+        """
+
+class ListEventBridgeRuleTemplatesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListEventBridgeRuleTemplates)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listeventbridgeruletemplatespaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        GroupIdentifier: str = ...,
+        SignalMapIdentifier: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListEventBridgeRuleTemplatesResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListEventBridgeRuleTemplates.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listeventbridgeruletemplatespaginator)
+        """
 
 class ListInputDeviceTransfersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDeviceTransfers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicetransferspaginator)
     """
 
@@ -119,90 +204,84 @@
         self, *, TransferType: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInputDeviceTransfersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDeviceTransfers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicetransferspaginator)
         """
 
-
 class ListInputDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInputDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicespaginator)
         """
 
-
 class ListInputSecurityGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputSecurityGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputsecuritygroupspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInputSecurityGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputSecurityGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputsecuritygroupspaginator)
         """
 
-
 class ListInputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInputsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputspaginator)
         """
 
-
 class ListMultiplexProgramsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexPrograms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexprogramspaginator)
     """
 
     def paginate(
         self, *, MultiplexId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMultiplexProgramsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexPrograms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexprogramspaginator)
         """
 
-
 class ListMultiplexesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMultiplexesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexespaginator)
         """
 
-
 class ListOfferingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListOfferings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listofferingspaginator)
     """
 
     def paginate(
@@ -221,15 +300,14 @@
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listofferingspaginator)
         """
 
-
 class ListReservationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListReservations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listreservationspaginator)
     """
 
     def paginate(
@@ -245,7 +323,25 @@
         VideoQuality: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListReservationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListReservations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listreservationspaginator)
         """
+
+class ListSignalMapsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListSignalMaps)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listsignalmapspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        CloudWatchAlarmTemplateGroupIdentifier: str = ...,
+        EventBridgeRuleTemplateGroupIdentifier: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListSignalMapsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListSignalMaps.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listsignalmapspaginator)
+        """
```

### Comparing `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/paginator.pyi` & `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/waiter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,240 +1,266 @@
 """
-Type annotations for medialive service client paginators.
+Type annotations for medialive service client waiters.
 
-[Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/)
+[Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/)
 
 Usage::
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_medialive.client import MediaLiveClient
-    from mypy_boto3_medialive.paginator import (
-        DescribeSchedulePaginator,
-        ListChannelsPaginator,
-        ListInputDeviceTransfersPaginator,
-        ListInputDevicesPaginator,
-        ListInputSecurityGroupsPaginator,
-        ListInputsPaginator,
-        ListMultiplexProgramsPaginator,
-        ListMultiplexesPaginator,
-        ListOfferingsPaginator,
-        ListReservationsPaginator,
+    from mypy_boto3_medialive.waiter import (
+        ChannelCreatedWaiter,
+        ChannelDeletedWaiter,
+        ChannelRunningWaiter,
+        ChannelStoppedWaiter,
+        InputAttachedWaiter,
+        InputDeletedWaiter,
+        InputDetachedWaiter,
+        MultiplexCreatedWaiter,
+        MultiplexDeletedWaiter,
+        MultiplexRunningWaiter,
+        MultiplexStoppedWaiter,
+        SignalMapCreatedWaiter,
+        SignalMapMonitorDeletedWaiter,
+        SignalMapMonitorDeployedWaiter,
+        SignalMapUpdatedWaiter,
     )
 
     session = Session()
     client: MediaLiveClient = session.client("medialive")
 
-    describe_schedule_paginator: DescribeSchedulePaginator = client.get_paginator("describe_schedule")
-    list_channels_paginator: ListChannelsPaginator = client.get_paginator("list_channels")
-    list_input_device_transfers_paginator: ListInputDeviceTransfersPaginator = client.get_paginator("list_input_device_transfers")
-    list_input_devices_paginator: ListInputDevicesPaginator = client.get_paginator("list_input_devices")
-    list_input_security_groups_paginator: ListInputSecurityGroupsPaginator = client.get_paginator("list_input_security_groups")
-    list_inputs_paginator: ListInputsPaginator = client.get_paginator("list_inputs")
-    list_multiplex_programs_paginator: ListMultiplexProgramsPaginator = client.get_paginator("list_multiplex_programs")
-    list_multiplexes_paginator: ListMultiplexesPaginator = client.get_paginator("list_multiplexes")
-    list_offerings_paginator: ListOfferingsPaginator = client.get_paginator("list_offerings")
-    list_reservations_paginator: ListReservationsPaginator = client.get_paginator("list_reservations")
+    channel_created_waiter: ChannelCreatedWaiter = client.get_waiter("channel_created")
+    channel_deleted_waiter: ChannelDeletedWaiter = client.get_waiter("channel_deleted")
+    channel_running_waiter: ChannelRunningWaiter = client.get_waiter("channel_running")
+    channel_stopped_waiter: ChannelStoppedWaiter = client.get_waiter("channel_stopped")
+    input_attached_waiter: InputAttachedWaiter = client.get_waiter("input_attached")
+    input_deleted_waiter: InputDeletedWaiter = client.get_waiter("input_deleted")
+    input_detached_waiter: InputDetachedWaiter = client.get_waiter("input_detached")
+    multiplex_created_waiter: MultiplexCreatedWaiter = client.get_waiter("multiplex_created")
+    multiplex_deleted_waiter: MultiplexDeletedWaiter = client.get_waiter("multiplex_deleted")
+    multiplex_running_waiter: MultiplexRunningWaiter = client.get_waiter("multiplex_running")
+    multiplex_stopped_waiter: MultiplexStoppedWaiter = client.get_waiter("multiplex_stopped")
+    signal_map_created_waiter: SignalMapCreatedWaiter = client.get_waiter("signal_map_created")
+    signal_map_monitor_deleted_waiter: SignalMapMonitorDeletedWaiter = client.get_waiter("signal_map_monitor_deleted")
+    signal_map_monitor_deployed_waiter: SignalMapMonitorDeployedWaiter = client.get_waiter("signal_map_monitor_deployed")
+    signal_map_updated_waiter: SignalMapUpdatedWaiter = client.get_waiter("signal_map_updated")
     ```
 """
 
-from typing import Generic, Iterator, TypeVar
+from botocore.waiter import Waiter
 
-from botocore.paginate import PageIterator, Paginator
-
-from .type_defs import (
-    DescribeScheduleResponsePaginatorTypeDef,
-    ListChannelsResponsePaginatorTypeDef,
-    ListInputDevicesResponseTypeDef,
-    ListInputDeviceTransfersResponseTypeDef,
-    ListInputSecurityGroupsResponseTypeDef,
-    ListInputsResponseTypeDef,
-    ListMultiplexesResponseTypeDef,
-    ListMultiplexProgramsResponseTypeDef,
-    ListOfferingsResponseTypeDef,
-    ListReservationsResponseTypeDef,
-    PaginatorConfigTypeDef,
-)
+from .type_defs import WaiterConfigTypeDef
 
 __all__ = (
-    "DescribeSchedulePaginator",
-    "ListChannelsPaginator",
-    "ListInputDeviceTransfersPaginator",
-    "ListInputDevicesPaginator",
-    "ListInputSecurityGroupsPaginator",
-    "ListInputsPaginator",
-    "ListMultiplexProgramsPaginator",
-    "ListMultiplexesPaginator",
-    "ListOfferingsPaginator",
-    "ListReservationsPaginator",
+    "ChannelCreatedWaiter",
+    "ChannelDeletedWaiter",
+    "ChannelRunningWaiter",
+    "ChannelStoppedWaiter",
+    "InputAttachedWaiter",
+    "InputDeletedWaiter",
+    "InputDetachedWaiter",
+    "MultiplexCreatedWaiter",
+    "MultiplexDeletedWaiter",
+    "MultiplexRunningWaiter",
+    "MultiplexStoppedWaiter",
+    "SignalMapCreatedWaiter",
+    "SignalMapMonitorDeletedWaiter",
+    "SignalMapMonitorDeployedWaiter",
+    "SignalMapUpdatedWaiter",
 )
 
-_ItemTypeDef = TypeVar("_ItemTypeDef")
 
-class _PageIterator(Generic[_ItemTypeDef], PageIterator):
-    def __iter__(self) -> Iterator[_ItemTypeDef]:
+class ChannelCreatedWaiter(Waiter):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.ChannelCreated)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#channelcreatedwaiter)
+    """
+
+    def wait(self, *, ChannelId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.ChannelCreated.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#channelcreatedwaiter)
+        """
+
+
+class ChannelDeletedWaiter(Waiter):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.ChannelDeleted)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#channeldeletedwaiter)
+    """
+
+    def wait(self, *, ChannelId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
-        Proxy method to specify iterator item type.
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.ChannelDeleted.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#channeldeletedwaiter)
         """
 
-class DescribeSchedulePaginator(Paginator):
+
+class ChannelRunningWaiter(Waiter):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.ChannelRunning)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#channelrunningwaiter)
     """
 
-    def paginate(
-        self, *, ChannelId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[DescribeScheduleResponsePaginatorTypeDef]:
+    def wait(self, *, ChannelId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.ChannelRunning.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#channelrunningwaiter)
         """
 
-class ListChannelsPaginator(Paginator):
+
+class ChannelStoppedWaiter(Waiter):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.ChannelStopped)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#channelstoppedwaiter)
     """
 
-    def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListChannelsResponsePaginatorTypeDef]:
+    def wait(self, *, ChannelId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.ChannelStopped.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#channelstoppedwaiter)
         """
 
-class ListInputDeviceTransfersPaginator(Paginator):
+
+class InputAttachedWaiter(Waiter):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDeviceTransfers)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicetransferspaginator)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.InputAttached)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#inputattachedwaiter)
     """
 
-    def paginate(
-        self, *, TransferType: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListInputDeviceTransfersResponseTypeDef]:
+    def wait(self, *, InputId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDeviceTransfers.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicetransferspaginator)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.InputAttached.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#inputattachedwaiter)
         """
 
-class ListInputDevicesPaginator(Paginator):
+
+class InputDeletedWaiter(Waiter):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDevices)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicespaginator)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.InputDeleted)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#inputdeletedwaiter)
     """
 
-    def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListInputDevicesResponseTypeDef]:
+    def wait(self, *, InputId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDevices.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicespaginator)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.InputDeleted.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#inputdeletedwaiter)
         """
 
-class ListInputSecurityGroupsPaginator(Paginator):
+
+class InputDetachedWaiter(Waiter):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputSecurityGroups)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputsecuritygroupspaginator)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.InputDetached)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#inputdetachedwaiter)
     """
 
-    def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListInputSecurityGroupsResponseTypeDef]:
+    def wait(self, *, InputId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputSecurityGroups.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputsecuritygroupspaginator)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.InputDetached.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#inputdetachedwaiter)
         """
 
-class ListInputsPaginator(Paginator):
+
+class MultiplexCreatedWaiter(Waiter):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputs)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputspaginator)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.MultiplexCreated)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#multiplexcreatedwaiter)
     """
 
-    def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListInputsResponseTypeDef]:
+    def wait(self, *, MultiplexId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputs.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputspaginator)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.MultiplexCreated.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#multiplexcreatedwaiter)
         """
 
-class ListMultiplexProgramsPaginator(Paginator):
+
+class MultiplexDeletedWaiter(Waiter):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexPrograms)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexprogramspaginator)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.MultiplexDeleted)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#multiplexdeletedwaiter)
     """
 
-    def paginate(
-        self, *, MultiplexId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListMultiplexProgramsResponseTypeDef]:
+    def wait(self, *, MultiplexId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexPrograms.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexprogramspaginator)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.MultiplexDeleted.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#multiplexdeletedwaiter)
         """
 
-class ListMultiplexesPaginator(Paginator):
+
+class MultiplexRunningWaiter(Waiter):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexes)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexespaginator)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.MultiplexRunning)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#multiplexrunningwaiter)
     """
 
-    def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListMultiplexesResponseTypeDef]:
+    def wait(self, *, MultiplexId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexes.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexespaginator)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.MultiplexRunning.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#multiplexrunningwaiter)
         """
 
-class ListOfferingsPaginator(Paginator):
+
+class MultiplexStoppedWaiter(Waiter):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListOfferings)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listofferingspaginator)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.MultiplexStopped)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#multiplexstoppedwaiter)
     """
 
-    def paginate(
-        self,
-        *,
-        ChannelClass: str = ...,
-        ChannelConfiguration: str = ...,
-        Codec: str = ...,
-        Duration: str = ...,
-        MaximumBitrate: str = ...,
-        MaximumFramerate: str = ...,
-        Resolution: str = ...,
-        ResourceType: str = ...,
-        SpecialFeature: str = ...,
-        VideoQuality: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListOfferingsResponseTypeDef]:
+    def wait(self, *, MultiplexId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListOfferings.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listofferingspaginator)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.MultiplexStopped.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#multiplexstoppedwaiter)
         """
 
-class ListReservationsPaginator(Paginator):
+
+class SignalMapCreatedWaiter(Waiter):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.SignalMapCreated)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#signalmapcreatedwaiter)
+    """
+
+    def wait(self, *, Identifier: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.SignalMapCreated.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#signalmapcreatedwaiter)
+        """
+
+
+class SignalMapMonitorDeletedWaiter(Waiter):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.SignalMapMonitorDeleted)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#signalmapmonitordeletedwaiter)
+    """
+
+    def wait(self, *, Identifier: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.SignalMapMonitorDeleted.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#signalmapmonitordeletedwaiter)
+        """
+
+
+class SignalMapMonitorDeployedWaiter(Waiter):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.SignalMapMonitorDeployed)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#signalmapmonitordeployedwaiter)
+    """
+
+    def wait(self, *, Identifier: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.SignalMapMonitorDeployed.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#signalmapmonitordeployedwaiter)
+        """
+
+
+class SignalMapUpdatedWaiter(Waiter):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListReservations)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listreservationspaginator)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.SignalMapUpdated)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#signalmapupdatedwaiter)
     """
 
-    def paginate(
-        self,
-        *,
-        ChannelClass: str = ...,
-        Codec: str = ...,
-        MaximumBitrate: str = ...,
-        MaximumFramerate: str = ...,
-        Resolution: str = ...,
-        ResourceType: str = ...,
-        SpecialFeature: str = ...,
-        VideoQuality: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListReservationsResponseTypeDef]:
+    def wait(self, *, Identifier: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListReservations.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listreservationspaginator)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.SignalMapUpdated.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#signalmapupdatedwaiter)
         """
```

### Comparing `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/type_defs.py` & `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/type_defs.py`

 * *Files 25% similar despite different names*

```diff
@@ -51,14 +51,18 @@
     BurnInOutlineColorType,
     BurnInShadowColorType,
     BurnInTeletextGridControlType,
     CdiInputResolutionType,
     ChannelClassType,
     ChannelPipelineIdToRestartType,
     ChannelStateType,
+    CloudWatchAlarmTemplateComparisonOperatorType,
+    CloudWatchAlarmTemplateStatisticType,
+    CloudWatchAlarmTemplateTargetResourceTypeType,
+    CloudWatchAlarmTemplateTreatMissingDataType,
     CmafIngestSegmentLengthUnitsType,
     CmafNielsenId3BehaviorType,
     ColorSpaceType,
     DashRoleAudioType,
     DashRoleCaptionType,
     DeviceSettingsSyncStateType,
     DeviceUpdateStatusType,
@@ -89,14 +93,15 @@
     Eac3StereoDownmixType,
     Eac3SurroundExModeType,
     Eac3SurroundModeType,
     EbuTtDDestinationStyleControlType,
     EbuTtDFillLineGapControlType,
     EmbeddedConvert608To708Type,
     EmbeddedScte20DetectionType,
+    EventBridgeRuleTemplateEventTypeType,
     FeatureActivationsInputPrepareScheduleActionsType,
     FeatureActivationsOutputStaticImageOverlayScheduleActionsType,
     FecOutputIncludeFecType,
     FixedAfdType,
     Fmp4NielsenId3BehaviorType,
     Fmp4TimedMetadataBehaviorType,
     FollowPointType,
@@ -271,14 +276,16 @@
     Scte35InputModeType,
     Scte35NoRegionalBlackoutFlagType,
     Scte35SegmentationCancelIndicatorType,
     Scte35SpliceInsertNoRegionalBlackoutBehaviorType,
     Scte35SpliceInsertWebDeliveryAllowedBehaviorType,
     Scte35TypeType,
     Scte35WebDeliveryAllowedFlagType,
+    SignalMapMonitorDeploymentStatusType,
+    SignalMapStatusType,
     SmoothGroupAudioOnlyTimecodeControlType,
     SmoothGroupCertificateModeType,
     SmoothGroupEventIdModeType,
     SmoothGroupEventStopBehaviorType,
     SmoothGroupSegmentationModeType,
     SmoothGroupSparseTrackTypeType,
     SmoothGroupStreamManifestBehaviorType,
@@ -358,38 +365,52 @@
     "CdiInputSpecificationTypeDef",
     "ChannelEgressEndpointTypeDef",
     "InputSpecificationTypeDef",
     "MaintenanceStatusTypeDef",
     "VpcOutputSettingsDescriptionTypeDef",
     "PipelineDetailTypeDef",
     "ClaimDeviceRequestRequestTypeDef",
+    "CloudWatchAlarmTemplateGroupSummaryTypeDef",
+    "CloudWatchAlarmTemplateSummaryTypeDef",
     "CmafIngestOutputSettingsTypeDef",
     "ColorCorrectionTypeDef",
     "MaintenanceCreateSettingsTypeDef",
     "VpcOutputSettingsTypeDef",
+    "CreateCloudWatchAlarmTemplateGroupRequestRequestTypeDef",
+    "CreateCloudWatchAlarmTemplateRequestRequestTypeDef",
+    "CreateEventBridgeRuleTemplateGroupRequestRequestTypeDef",
+    "EventBridgeRuleTemplateTargetTypeDef",
     "InputDestinationRequestTypeDef",
     "InputDeviceSettingsTypeDef",
     "InputSourceRequestTypeDef",
     "InputVpcRequestTypeDef",
     "MediaConnectFlowRequestTypeDef",
     "InputWhitelistRuleCidrTypeDef",
     "MultiplexSettingsTypeDef",
     "CreatePartnerInputRequestRequestTypeDef",
+    "CreateSignalMapRequestRequestTypeDef",
+    "MonitorDeploymentTypeDef",
+    "SuccessfulMonitorDeploymentTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
+    "DeleteCloudWatchAlarmTemplateGroupRequestRequestTypeDef",
+    "DeleteCloudWatchAlarmTemplateRequestRequestTypeDef",
+    "DeleteEventBridgeRuleTemplateGroupRequestRequestTypeDef",
+    "DeleteEventBridgeRuleTemplateRequestRequestTypeDef",
     "DeleteInputRequestRequestTypeDef",
     "DeleteInputSecurityGroupRequestRequestTypeDef",
     "DeleteMultiplexProgramRequestRequestTypeDef",
     "MultiplexProgramPacketIdentifiersMapTypeDef",
     "MultiplexProgramPipelineDetailTypeDef",
     "DeleteMultiplexRequestRequestTypeDef",
     "DeleteReservationRequestRequestTypeDef",
     "RenewalSettingsTypeDef",
     "ReservationResourceSpecificationTypeDef",
     "DeleteScheduleRequestRequestTypeDef",
+    "DeleteSignalMapRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeInputDeviceRequestRequestTypeDef",
     "InputDeviceHdSettingsTypeDef",
     "InputDeviceNetworkSettingsTypeDef",
     "DescribeInputDeviceThumbnailRequestRequestTypeDef",
@@ -409,23 +430,30 @@
     "DvbSdtSettingsTypeDef",
     "DvbTdtSettingsTypeDef",
     "FeatureActivationsTypeDef",
     "NielsenConfigurationTypeDef",
     "ThumbnailConfigurationTypeDef",
     "TimecodeConfigTypeDef",
     "EpochLockingSettingsTypeDef",
+    "EventBridgeRuleTemplateGroupSummaryTypeDef",
+    "EventBridgeRuleTemplateSummaryTypeDef",
     "InputLossFailoverSettingsTypeDef",
     "VideoBlackFailoverSettingsTypeDef",
     "FecOutputSettingsTypeDef",
     "FixedModeScheduleActionStartSettingsTypeDef",
     "Fmp4HlsSettingsTypeDef",
     "FollowModeScheduleActionStartSettingsTypeDef",
     "FrameCaptureS3SettingsTypeDef",
     "FrameCaptureOutputSettingsTypeDef",
     "TimecodeBurninSettingsTypeDef",
+    "GetCloudWatchAlarmTemplateGroupRequestRequestTypeDef",
+    "GetCloudWatchAlarmTemplateRequestRequestTypeDef",
+    "GetEventBridgeRuleTemplateGroupRequestRequestTypeDef",
+    "GetEventBridgeRuleTemplateRequestRequestTypeDef",
+    "GetSignalMapRequestRequestTypeDef",
     "H264ColorSpaceSettingsTypeDef",
     "TemporalFilterSettingsTypeDef",
     "Hdr10SettingsTypeDef",
     "HlsAkamaiSettingsTypeDef",
     "HlsBasicPutSettingsTypeDef",
     "HlsMediaStoreSettingsTypeDef",
     "HlsS3SettingsTypeDef",
@@ -438,28 +466,35 @@
     "InputDestinationVpcTypeDef",
     "InputDeviceConfigurableAudioChannelPairConfigTypeDef",
     "InputDeviceMediaConnectConfigurableSettingsTypeDef",
     "InputDeviceMediaConnectSettingsTypeDef",
     "InputDeviceRequestTypeDef",
     "InputDeviceUhdAudioChannelPairConfigTypeDef",
     "ListChannelsRequestRequestTypeDef",
+    "ListCloudWatchAlarmTemplateGroupsRequestRequestTypeDef",
+    "ListCloudWatchAlarmTemplatesRequestRequestTypeDef",
+    "ListEventBridgeRuleTemplateGroupsRequestRequestTypeDef",
+    "ListEventBridgeRuleTemplatesRequestRequestTypeDef",
     "ListInputDeviceTransfersRequestRequestTypeDef",
     "TransferringInputDeviceSummaryTypeDef",
     "ListInputDevicesRequestRequestTypeDef",
     "ListInputSecurityGroupsRequestRequestTypeDef",
     "ListInputsRequestRequestTypeDef",
     "ListMultiplexProgramsRequestRequestTypeDef",
     "MultiplexProgramSummaryTypeDef",
     "ListMultiplexesRequestRequestTypeDef",
     "ListOfferingsRequestRequestTypeDef",
     "ListReservationsRequestRequestTypeDef",
+    "ListSignalMapsRequestRequestTypeDef",
+    "SignalMapSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "M3u8SettingsTypeDef",
     "MaintenanceUpdateSettingsTypeDef",
     "MediaPackageOutputDestinationSettingsTypeDef",
+    "MediaResourceNeighborTypeDef",
     "MotionGraphicsActivateScheduleActionSettingsTypeDef",
     "MotionGraphicsSettingsTypeDef",
     "MsSmoothOutputSettingsTypeDef",
     "MultiplexMediaConnectOutputDestinationSettingsTypeDef",
     "MultiplexProgramChannelDestinationSettingsTypeDef",
     "MultiplexProgramServiceDescriptorTypeDef",
     "MultiplexSettingsSummaryTypeDef",
@@ -477,22 +512,28 @@
     "Scte35ReturnToNetworkScheduleActionSettingsTypeDef",
     "Scte35SpliceInsertScheduleActionSettingsTypeDef",
     "StaticImageDeactivateScheduleActionSettingsTypeDef",
     "StaticImageOutputDeactivateScheduleActionSettingsPaginatorTypeDef",
     "StaticImageOutputDeactivateScheduleActionSettingsTypeDef",
     "Scte35DeliveryRestrictionsTypeDef",
     "StartChannelRequestRequestTypeDef",
+    "StartDeleteMonitorDeploymentRequestRequestTypeDef",
     "StartInputDeviceMaintenanceWindowRequestRequestTypeDef",
     "StartInputDeviceRequestRequestTypeDef",
+    "StartMonitorDeploymentRequestRequestTypeDef",
     "StartMultiplexRequestRequestTypeDef",
+    "StartUpdateSignalMapRequestRequestTypeDef",
     "StopChannelRequestRequestTypeDef",
     "StopInputDeviceRequestRequestTypeDef",
     "StopMultiplexRequestRequestTypeDef",
     "ThumbnailTypeDef",
     "TransferInputDeviceRequestRequestTypeDef",
+    "UpdateCloudWatchAlarmTemplateGroupRequestRequestTypeDef",
+    "UpdateCloudWatchAlarmTemplateRequestRequestTypeDef",
+    "UpdateEventBridgeRuleTemplateGroupRequestRequestTypeDef",
     "VideoSelectorPidTypeDef",
     "VideoSelectorProgramIdTypeDef",
     "UpdateAccountConfigurationRequestRequestTypeDef",
     "ArchiveCdnSettingsTypeDef",
     "CmafIngestGroupSettingsTypeDef",
     "MediaPackageGroupSettingsTypeDef",
     "MsSmoothGroupSettingsTypeDef",
@@ -512,21 +553,37 @@
     "StaticKeySettingsTypeDef",
     "AudioTrackSelectionPaginatorTypeDef",
     "AudioTrackSelectionTypeDef",
     "AvailSettingsTypeDef",
     "BatchDeleteResponseTypeDef",
     "BatchStartResponseTypeDef",
     "BatchStopResponseTypeDef",
+    "CreateCloudWatchAlarmTemplateGroupResponseTypeDef",
+    "CreateCloudWatchAlarmTemplateResponseTypeDef",
+    "CreateEventBridgeRuleTemplateGroupResponseTypeDef",
     "DescribeAccountConfigurationResponseTypeDef",
     "DescribeInputDeviceThumbnailResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "GetCloudWatchAlarmTemplateGroupResponseTypeDef",
+    "GetCloudWatchAlarmTemplateResponseTypeDef",
+    "GetEventBridgeRuleTemplateGroupResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateAccountConfigurationResponseTypeDef",
+    "UpdateCloudWatchAlarmTemplateGroupResponseTypeDef",
+    "UpdateCloudWatchAlarmTemplateResponseTypeDef",
+    "UpdateEventBridgeRuleTemplateGroupResponseTypeDef",
     "TeletextSourceSettingsTypeDef",
+    "ListCloudWatchAlarmTemplateGroupsResponseTypeDef",
+    "ListCloudWatchAlarmTemplatesResponseTypeDef",
     "ColorCorrectionSettingsTypeDef",
+    "CreateEventBridgeRuleTemplateRequestRequestTypeDef",
+    "CreateEventBridgeRuleTemplateResponseTypeDef",
+    "GetEventBridgeRuleTemplateResponseTypeDef",
+    "UpdateEventBridgeRuleTemplateRequestRequestTypeDef",
+    "UpdateEventBridgeRuleTemplateResponseTypeDef",
     "CreateInputRequestRequestTypeDef",
     "CreateInputSecurityGroupRequestRequestTypeDef",
     "UpdateInputSecurityGroupRequestRequestTypeDef",
     "CreateMultiplexRequestRequestTypeDef",
     "UpdateMultiplexRequestRequestTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
     "UpdateReservationRequestRequestTypeDef",
@@ -542,28 +599,39 @@
     "DescribeInputRequestInputAttachedWaitTypeDef",
     "DescribeInputRequestInputDeletedWaitTypeDef",
     "DescribeInputRequestInputDetachedWaitTypeDef",
     "DescribeMultiplexRequestMultiplexCreatedWaitTypeDef",
     "DescribeMultiplexRequestMultiplexDeletedWaitTypeDef",
     "DescribeMultiplexRequestMultiplexRunningWaitTypeDef",
     "DescribeMultiplexRequestMultiplexStoppedWaitTypeDef",
+    "GetSignalMapRequestSignalMapCreatedWaitTypeDef",
+    "GetSignalMapRequestSignalMapMonitorDeletedWaitTypeDef",
+    "GetSignalMapRequestSignalMapMonitorDeployedWaitTypeDef",
+    "GetSignalMapRequestSignalMapUpdatedWaitTypeDef",
     "DescribeInputSecurityGroupResponseTypeDef",
     "InputSecurityGroupTypeDef",
     "DescribeScheduleRequestDescribeSchedulePaginateTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
+    "ListCloudWatchAlarmTemplateGroupsRequestListCloudWatchAlarmTemplateGroupsPaginateTypeDef",
+    "ListCloudWatchAlarmTemplatesRequestListCloudWatchAlarmTemplatesPaginateTypeDef",
+    "ListEventBridgeRuleTemplateGroupsRequestListEventBridgeRuleTemplateGroupsPaginateTypeDef",
+    "ListEventBridgeRuleTemplatesRequestListEventBridgeRuleTemplatesPaginateTypeDef",
     "ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
     "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
     "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
     "ListInputsRequestListInputsPaginateTypeDef",
     "ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
     "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
     "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListReservationsRequestListReservationsPaginateTypeDef",
+    "ListSignalMapsRequestListSignalMapsPaginateTypeDef",
     "M2tsSettingsTypeDef",
     "OutputLockingSettingsTypeDef",
+    "ListEventBridgeRuleTemplateGroupsResponseTypeDef",
+    "ListEventBridgeRuleTemplatesResponseTypeDef",
     "FailoverConditionSettingsTypeDef",
     "ScheduleActionStartSettingsPaginatorTypeDef",
     "ScheduleActionStartSettingsTypeDef",
     "FrameCaptureCdnSettingsTypeDef",
     "FrameCaptureSettingsTypeDef",
     "H264FilterSettingsTypeDef",
     "H265FilterSettingsTypeDef",
@@ -575,15 +643,17 @@
     "InputClippingSettingsTypeDef",
     "InputDestinationTypeDef",
     "InputDeviceConfigurableSettingsTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "InputDeviceUhdSettingsTypeDef",
     "ListInputDeviceTransfersResponseTypeDef",
     "ListMultiplexProgramsResponseTypeDef",
+    "ListSignalMapsResponseTypeDef",
     "StandardHlsSettingsTypeDef",
+    "MediaResourceTypeDef",
     "MotionGraphicsConfigurationTypeDef",
     "MultiplexOutputDestinationTypeDef",
     "MultiplexSummaryTypeDef",
     "MultiplexVideoSettingsTypeDef",
     "NielsenWatermarksSettingsTypeDef",
     "OutputDestinationPaginatorTypeDef",
     "OutputDestinationTypeDef",
@@ -623,14 +693,19 @@
     "DescribeInputResponseTypeDef",
     "InputTypeDef",
     "UpdateInputDeviceRequestRequestTypeDef",
     "DescribeInputDeviceResponseTypeDef",
     "InputDeviceSummaryTypeDef",
     "UpdateInputDeviceResponseTypeDef",
     "HlsSettingsTypeDef",
+    "CreateSignalMapResponseTypeDef",
+    "GetSignalMapResponseTypeDef",
+    "StartDeleteMonitorDeploymentResponseTypeDef",
+    "StartMonitorDeploymentResponseTypeDef",
+    "StartUpdateSignalMapResponseTypeDef",
     "DeleteMultiplexResponseTypeDef",
     "DescribeMultiplexResponseTypeDef",
     "MultiplexTypeDef",
     "StartMultiplexResponseTypeDef",
     "StopMultiplexResponseTypeDef",
     "ListMultiplexesResponseTypeDef",
     "MultiplexProgramSettingsTypeDef",
@@ -1086,14 +1161,49 @@
 )
 ClaimDeviceRequestRequestTypeDef = TypedDict(
     "ClaimDeviceRequestRequestTypeDef",
     {
         "Id": NotRequired[str],
     },
 )
+CloudWatchAlarmTemplateGroupSummaryTypeDef = TypedDict(
+    "CloudWatchAlarmTemplateGroupSummaryTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Id": str,
+        "Name": str,
+        "TemplateCount": int,
+        "Description": NotRequired[str],
+        "ModifiedAt": NotRequired[datetime],
+        "Tags": NotRequired[Dict[str, str]],
+    },
+)
+CloudWatchAlarmTemplateSummaryTypeDef = TypedDict(
+    "CloudWatchAlarmTemplateSummaryTypeDef",
+    {
+        "Arn": str,
+        "ComparisonOperator": CloudWatchAlarmTemplateComparisonOperatorType,
+        "CreatedAt": datetime,
+        "EvaluationPeriods": int,
+        "GroupId": str,
+        "Id": str,
+        "MetricName": str,
+        "Name": str,
+        "Period": int,
+        "Statistic": CloudWatchAlarmTemplateStatisticType,
+        "TargetResourceType": CloudWatchAlarmTemplateTargetResourceTypeType,
+        "Threshold": float,
+        "TreatMissingData": CloudWatchAlarmTemplateTreatMissingDataType,
+        "DatapointsToAlarm": NotRequired[int],
+        "Description": NotRequired[str],
+        "ModifiedAt": NotRequired[datetime],
+        "Tags": NotRequired[Dict[str, str]],
+    },
+)
 CmafIngestOutputSettingsTypeDef = TypedDict(
     "CmafIngestOutputSettingsTypeDef",
     {
         "NameModifier": NotRequired[str],
     },
 )
 ColorCorrectionTypeDef = TypedDict(
@@ -1115,14 +1225,54 @@
     "VpcOutputSettingsTypeDef",
     {
         "SubnetIds": Sequence[str],
         "PublicAddressAllocationIds": NotRequired[Sequence[str]],
         "SecurityGroupIds": NotRequired[Sequence[str]],
     },
 )
+CreateCloudWatchAlarmTemplateGroupRequestRequestTypeDef = TypedDict(
+    "CreateCloudWatchAlarmTemplateGroupRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Description": NotRequired[str],
+        "Tags": NotRequired[Mapping[str, str]],
+    },
+)
+CreateCloudWatchAlarmTemplateRequestRequestTypeDef = TypedDict(
+    "CreateCloudWatchAlarmTemplateRequestRequestTypeDef",
+    {
+        "ComparisonOperator": CloudWatchAlarmTemplateComparisonOperatorType,
+        "EvaluationPeriods": int,
+        "GroupIdentifier": str,
+        "MetricName": str,
+        "Name": str,
+        "Period": int,
+        "Statistic": CloudWatchAlarmTemplateStatisticType,
+        "TargetResourceType": CloudWatchAlarmTemplateTargetResourceTypeType,
+        "Threshold": float,
+        "TreatMissingData": CloudWatchAlarmTemplateTreatMissingDataType,
+        "DatapointsToAlarm": NotRequired[int],
+        "Description": NotRequired[str],
+        "Tags": NotRequired[Mapping[str, str]],
+    },
+)
+CreateEventBridgeRuleTemplateGroupRequestRequestTypeDef = TypedDict(
+    "CreateEventBridgeRuleTemplateGroupRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Description": NotRequired[str],
+        "Tags": NotRequired[Mapping[str, str]],
+    },
+)
+EventBridgeRuleTemplateTargetTypeDef = TypedDict(
+    "EventBridgeRuleTemplateTargetTypeDef",
+    {
+        "Arn": str,
+    },
+)
 InputDestinationRequestTypeDef = TypedDict(
     "InputDestinationRequestTypeDef",
     {
         "StreamName": NotRequired[str],
     },
 )
 InputDeviceSettingsTypeDef = TypedDict(
@@ -1171,27 +1321,77 @@
     "CreatePartnerInputRequestRequestTypeDef",
     {
         "InputId": str,
         "RequestId": NotRequired[str],
         "Tags": NotRequired[Mapping[str, str]],
     },
 )
+CreateSignalMapRequestRequestTypeDef = TypedDict(
+    "CreateSignalMapRequestRequestTypeDef",
+    {
+        "DiscoveryEntryPointArn": str,
+        "Name": str,
+        "CloudWatchAlarmTemplateGroupIdentifiers": NotRequired[Sequence[str]],
+        "Description": NotRequired[str],
+        "EventBridgeRuleTemplateGroupIdentifiers": NotRequired[Sequence[str]],
+        "Tags": NotRequired[Mapping[str, str]],
+    },
+)
+MonitorDeploymentTypeDef = TypedDict(
+    "MonitorDeploymentTypeDef",
+    {
+        "Status": SignalMapMonitorDeploymentStatusType,
+        "DetailsUri": NotRequired[str],
+        "ErrorMessage": NotRequired[str],
+    },
+)
+SuccessfulMonitorDeploymentTypeDef = TypedDict(
+    "SuccessfulMonitorDeploymentTypeDef",
+    {
+        "DetailsUri": str,
+        "Status": SignalMapMonitorDeploymentStatusType,
+    },
+)
 CreateTagsRequestRequestTypeDef = TypedDict(
     "CreateTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": NotRequired[Mapping[str, str]],
     },
 )
 DeleteChannelRequestRequestTypeDef = TypedDict(
     "DeleteChannelRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
+DeleteCloudWatchAlarmTemplateGroupRequestRequestTypeDef = TypedDict(
+    "DeleteCloudWatchAlarmTemplateGroupRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+DeleteCloudWatchAlarmTemplateRequestRequestTypeDef = TypedDict(
+    "DeleteCloudWatchAlarmTemplateRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+DeleteEventBridgeRuleTemplateGroupRequestRequestTypeDef = TypedDict(
+    "DeleteEventBridgeRuleTemplateGroupRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+DeleteEventBridgeRuleTemplateRequestRequestTypeDef = TypedDict(
+    "DeleteEventBridgeRuleTemplateRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
 DeleteInputRequestRequestTypeDef = TypedDict(
     "DeleteInputRequestRequestTypeDef",
     {
         "InputId": str,
     },
 )
 DeleteInputSecurityGroupRequestRequestTypeDef = TypedDict(
@@ -1266,14 +1466,20 @@
 )
 DeleteScheduleRequestRequestTypeDef = TypedDict(
     "DeleteScheduleRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
+DeleteSignalMapRequestRequestTypeDef = TypedDict(
+    "DeleteSignalMapRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
 DeleteTagsRequestRequestTypeDef = TypedDict(
     "DeleteTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1465,14 +1671,42 @@
 EpochLockingSettingsTypeDef = TypedDict(
     "EpochLockingSettingsTypeDef",
     {
         "CustomEpoch": NotRequired[str],
         "JamSyncTime": NotRequired[str],
     },
 )
+EventBridgeRuleTemplateGroupSummaryTypeDef = TypedDict(
+    "EventBridgeRuleTemplateGroupSummaryTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Id": str,
+        "Name": str,
+        "TemplateCount": int,
+        "Description": NotRequired[str],
+        "ModifiedAt": NotRequired[datetime],
+        "Tags": NotRequired[Dict[str, str]],
+    },
+)
+EventBridgeRuleTemplateSummaryTypeDef = TypedDict(
+    "EventBridgeRuleTemplateSummaryTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "EventTargetCount": int,
+        "EventType": EventBridgeRuleTemplateEventTypeType,
+        "GroupId": str,
+        "Id": str,
+        "Name": str,
+        "Description": NotRequired[str],
+        "ModifiedAt": NotRequired[datetime],
+        "Tags": NotRequired[Dict[str, str]],
+    },
+)
 InputLossFailoverSettingsTypeDef = TypedDict(
     "InputLossFailoverSettingsTypeDef",
     {
         "InputLossThresholdMsec": NotRequired[int],
     },
 )
 VideoBlackFailoverSettingsTypeDef = TypedDict(
@@ -1527,14 +1761,44 @@
     "TimecodeBurninSettingsTypeDef",
     {
         "FontSize": TimecodeBurninFontSizeType,
         "Position": TimecodeBurninPositionType,
         "Prefix": NotRequired[str],
     },
 )
+GetCloudWatchAlarmTemplateGroupRequestRequestTypeDef = TypedDict(
+    "GetCloudWatchAlarmTemplateGroupRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+GetCloudWatchAlarmTemplateRequestRequestTypeDef = TypedDict(
+    "GetCloudWatchAlarmTemplateRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+GetEventBridgeRuleTemplateGroupRequestRequestTypeDef = TypedDict(
+    "GetEventBridgeRuleTemplateGroupRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+GetEventBridgeRuleTemplateRequestRequestTypeDef = TypedDict(
+    "GetEventBridgeRuleTemplateRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+GetSignalMapRequestRequestTypeDef = TypedDict(
+    "GetSignalMapRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
 H264ColorSpaceSettingsTypeDef = TypedDict(
     "H264ColorSpaceSettingsTypeDef",
     {
         "ColorSpacePassthroughSettings": NotRequired[Mapping[str, Any]],
         "Rec601Settings": NotRequired[Mapping[str, Any]],
         "Rec709Settings": NotRequired[Mapping[str, Any]],
     },
@@ -1684,14 +1948,50 @@
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
     },
 )
+ListCloudWatchAlarmTemplateGroupsRequestRequestTypeDef = TypedDict(
+    "ListCloudWatchAlarmTemplateGroupsRequestRequestTypeDef",
+    {
+        "MaxResults": NotRequired[int],
+        "NextToken": NotRequired[str],
+        "Scope": NotRequired[str],
+        "SignalMapIdentifier": NotRequired[str],
+    },
+)
+ListCloudWatchAlarmTemplatesRequestRequestTypeDef = TypedDict(
+    "ListCloudWatchAlarmTemplatesRequestRequestTypeDef",
+    {
+        "GroupIdentifier": NotRequired[str],
+        "MaxResults": NotRequired[int],
+        "NextToken": NotRequired[str],
+        "Scope": NotRequired[str],
+        "SignalMapIdentifier": NotRequired[str],
+    },
+)
+ListEventBridgeRuleTemplateGroupsRequestRequestTypeDef = TypedDict(
+    "ListEventBridgeRuleTemplateGroupsRequestRequestTypeDef",
+    {
+        "MaxResults": NotRequired[int],
+        "NextToken": NotRequired[str],
+        "SignalMapIdentifier": NotRequired[str],
+    },
+)
+ListEventBridgeRuleTemplatesRequestRequestTypeDef = TypedDict(
+    "ListEventBridgeRuleTemplatesRequestRequestTypeDef",
+    {
+        "GroupIdentifier": NotRequired[str],
+        "MaxResults": NotRequired[int],
+        "NextToken": NotRequired[str],
+        "SignalMapIdentifier": NotRequired[str],
+    },
+)
 ListInputDeviceTransfersRequestRequestTypeDef = TypedDict(
     "ListInputDeviceTransfersRequestRequestTypeDef",
     {
         "TransferType": str,
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
     },
@@ -1776,14 +2076,37 @@
         "NextToken": NotRequired[str],
         "Resolution": NotRequired[str],
         "ResourceType": NotRequired[str],
         "SpecialFeature": NotRequired[str],
         "VideoQuality": NotRequired[str],
     },
 )
+ListSignalMapsRequestRequestTypeDef = TypedDict(
+    "ListSignalMapsRequestRequestTypeDef",
+    {
+        "CloudWatchAlarmTemplateGroupIdentifier": NotRequired[str],
+        "EventBridgeRuleTemplateGroupIdentifier": NotRequired[str],
+        "MaxResults": NotRequired[int],
+        "NextToken": NotRequired[str],
+    },
+)
+SignalMapSummaryTypeDef = TypedDict(
+    "SignalMapSummaryTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Id": str,
+        "MonitorDeploymentStatus": SignalMapMonitorDeploymentStatusType,
+        "Name": str,
+        "Status": SignalMapStatusType,
+        "Description": NotRequired[str],
+        "ModifiedAt": NotRequired[datetime],
+        "Tags": NotRequired[Dict[str, str]],
+    },
+)
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 M3u8SettingsTypeDef = TypedDict(
@@ -1820,14 +2143,21 @@
 )
 MediaPackageOutputDestinationSettingsTypeDef = TypedDict(
     "MediaPackageOutputDestinationSettingsTypeDef",
     {
         "ChannelId": NotRequired[str],
     },
 )
+MediaResourceNeighborTypeDef = TypedDict(
+    "MediaResourceNeighborTypeDef",
+    {
+        "Arn": str,
+        "Name": NotRequired[str],
+    },
+)
 MotionGraphicsActivateScheduleActionSettingsTypeDef = TypedDict(
     "MotionGraphicsActivateScheduleActionSettingsTypeDef",
     {
         "Duration": NotRequired[int],
         "PasswordParam": NotRequired[str],
         "Url": NotRequired[str],
         "Username": NotRequired[str],
@@ -2006,32 +2336,57 @@
 )
 StartChannelRequestRequestTypeDef = TypedDict(
     "StartChannelRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
+StartDeleteMonitorDeploymentRequestRequestTypeDef = TypedDict(
+    "StartDeleteMonitorDeploymentRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
 StartInputDeviceMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "StartInputDeviceMaintenanceWindowRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
 StartInputDeviceRequestRequestTypeDef = TypedDict(
     "StartInputDeviceRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
+StartMonitorDeploymentRequestRequestTypeDef = TypedDict(
+    "StartMonitorDeploymentRequestRequestTypeDef",
+    {
+        "Identifier": str,
+        "DryRun": NotRequired[bool],
+    },
+)
 StartMultiplexRequestRequestTypeDef = TypedDict(
     "StartMultiplexRequestRequestTypeDef",
     {
         "MultiplexId": str,
     },
 )
+StartUpdateSignalMapRequestRequestTypeDef = TypedDict(
+    "StartUpdateSignalMapRequestRequestTypeDef",
+    {
+        "Identifier": str,
+        "CloudWatchAlarmTemplateGroupIdentifiers": NotRequired[Sequence[str]],
+        "Description": NotRequired[str],
+        "DiscoveryEntryPointArn": NotRequired[str],
+        "EventBridgeRuleTemplateGroupIdentifiers": NotRequired[Sequence[str]],
+        "ForceRediscovery": NotRequired[bool],
+        "Name": NotRequired[str],
+    },
+)
 StopChannelRequestRequestTypeDef = TypedDict(
     "StopChannelRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 StopInputDeviceRequestRequestTypeDef = TypedDict(
@@ -2060,14 +2415,46 @@
     {
         "InputDeviceId": str,
         "TargetCustomerId": NotRequired[str],
         "TargetRegion": NotRequired[str],
         "TransferMessage": NotRequired[str],
     },
 )
+UpdateCloudWatchAlarmTemplateGroupRequestRequestTypeDef = TypedDict(
+    "UpdateCloudWatchAlarmTemplateGroupRequestRequestTypeDef",
+    {
+        "Identifier": str,
+        "Description": NotRequired[str],
+    },
+)
+UpdateCloudWatchAlarmTemplateRequestRequestTypeDef = TypedDict(
+    "UpdateCloudWatchAlarmTemplateRequestRequestTypeDef",
+    {
+        "Identifier": str,
+        "ComparisonOperator": NotRequired[CloudWatchAlarmTemplateComparisonOperatorType],
+        "DatapointsToAlarm": NotRequired[int],
+        "Description": NotRequired[str],
+        "EvaluationPeriods": NotRequired[int],
+        "GroupIdentifier": NotRequired[str],
+        "MetricName": NotRequired[str],
+        "Name": NotRequired[str],
+        "Period": NotRequired[int],
+        "Statistic": NotRequired[CloudWatchAlarmTemplateStatisticType],
+        "TargetResourceType": NotRequired[CloudWatchAlarmTemplateTargetResourceTypeType],
+        "Threshold": NotRequired[float],
+        "TreatMissingData": NotRequired[CloudWatchAlarmTemplateTreatMissingDataType],
+    },
+)
+UpdateEventBridgeRuleTemplateGroupRequestRequestTypeDef = TypedDict(
+    "UpdateEventBridgeRuleTemplateGroupRequestRequestTypeDef",
+    {
+        "Identifier": str,
+        "Description": NotRequired[str],
+    },
+)
 VideoSelectorPidTypeDef = TypedDict(
     "VideoSelectorPidTypeDef",
     {
         "Pid": NotRequired[int],
     },
 )
 VideoSelectorProgramIdTypeDef = TypedDict(
@@ -2339,14 +2726,63 @@
     "BatchStopResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateCloudWatchAlarmTemplateGroupResponseTypeDef = TypedDict(
+    "CreateCloudWatchAlarmTemplateGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "Id": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CreateCloudWatchAlarmTemplateResponseTypeDef = TypedDict(
+    "CreateCloudWatchAlarmTemplateResponseTypeDef",
+    {
+        "Arn": str,
+        "ComparisonOperator": CloudWatchAlarmTemplateComparisonOperatorType,
+        "CreatedAt": datetime,
+        "DatapointsToAlarm": int,
+        "Description": str,
+        "EvaluationPeriods": int,
+        "GroupId": str,
+        "Id": str,
+        "MetricName": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Period": int,
+        "Statistic": CloudWatchAlarmTemplateStatisticType,
+        "Tags": Dict[str, str],
+        "TargetResourceType": CloudWatchAlarmTemplateTargetResourceTypeType,
+        "Threshold": float,
+        "TreatMissingData": CloudWatchAlarmTemplateTreatMissingDataType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CreateEventBridgeRuleTemplateGroupResponseTypeDef = TypedDict(
+    "CreateEventBridgeRuleTemplateGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "Id": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DescribeAccountConfigurationResponseTypeDef = TypedDict(
     "DescribeAccountConfigurationResponseTypeDef",
     {
         "AccountConfiguration": AccountConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2363,41 +2799,225 @@
 )
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+GetCloudWatchAlarmTemplateGroupResponseTypeDef = TypedDict(
+    "GetCloudWatchAlarmTemplateGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "Id": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetCloudWatchAlarmTemplateResponseTypeDef = TypedDict(
+    "GetCloudWatchAlarmTemplateResponseTypeDef",
+    {
+        "Arn": str,
+        "ComparisonOperator": CloudWatchAlarmTemplateComparisonOperatorType,
+        "CreatedAt": datetime,
+        "DatapointsToAlarm": int,
+        "Description": str,
+        "EvaluationPeriods": int,
+        "GroupId": str,
+        "Id": str,
+        "MetricName": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Period": int,
+        "Statistic": CloudWatchAlarmTemplateStatisticType,
+        "Tags": Dict[str, str],
+        "TargetResourceType": CloudWatchAlarmTemplateTargetResourceTypeType,
+        "Threshold": float,
+        "TreatMissingData": CloudWatchAlarmTemplateTreatMissingDataType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetEventBridgeRuleTemplateGroupResponseTypeDef = TypedDict(
+    "GetEventBridgeRuleTemplateGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "Id": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 UpdateAccountConfigurationResponseTypeDef = TypedDict(
     "UpdateAccountConfigurationResponseTypeDef",
     {
         "AccountConfiguration": AccountConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateCloudWatchAlarmTemplateGroupResponseTypeDef = TypedDict(
+    "UpdateCloudWatchAlarmTemplateGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "Id": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateCloudWatchAlarmTemplateResponseTypeDef = TypedDict(
+    "UpdateCloudWatchAlarmTemplateResponseTypeDef",
+    {
+        "Arn": str,
+        "ComparisonOperator": CloudWatchAlarmTemplateComparisonOperatorType,
+        "CreatedAt": datetime,
+        "DatapointsToAlarm": int,
+        "Description": str,
+        "EvaluationPeriods": int,
+        "GroupId": str,
+        "Id": str,
+        "MetricName": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Period": int,
+        "Statistic": CloudWatchAlarmTemplateStatisticType,
+        "Tags": Dict[str, str],
+        "TargetResourceType": CloudWatchAlarmTemplateTargetResourceTypeType,
+        "Threshold": float,
+        "TreatMissingData": CloudWatchAlarmTemplateTreatMissingDataType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateEventBridgeRuleTemplateGroupResponseTypeDef = TypedDict(
+    "UpdateEventBridgeRuleTemplateGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "Id": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 TeletextSourceSettingsTypeDef = TypedDict(
     "TeletextSourceSettingsTypeDef",
     {
         "OutputRectangle": NotRequired[CaptionRectangleTypeDef],
         "PageNumber": NotRequired[str],
     },
 )
+ListCloudWatchAlarmTemplateGroupsResponseTypeDef = TypedDict(
+    "ListCloudWatchAlarmTemplateGroupsResponseTypeDef",
+    {
+        "CloudWatchAlarmTemplateGroups": List[CloudWatchAlarmTemplateGroupSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListCloudWatchAlarmTemplatesResponseTypeDef = TypedDict(
+    "ListCloudWatchAlarmTemplatesResponseTypeDef",
+    {
+        "CloudWatchAlarmTemplates": List[CloudWatchAlarmTemplateSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ColorCorrectionSettingsTypeDef = TypedDict(
     "ColorCorrectionSettingsTypeDef",
     {
         "GlobalColorCorrections": Sequence[ColorCorrectionTypeDef],
     },
 )
+CreateEventBridgeRuleTemplateRequestRequestTypeDef = TypedDict(
+    "CreateEventBridgeRuleTemplateRequestRequestTypeDef",
+    {
+        "EventType": EventBridgeRuleTemplateEventTypeType,
+        "GroupIdentifier": str,
+        "Name": str,
+        "Description": NotRequired[str],
+        "EventTargets": NotRequired[Sequence[EventBridgeRuleTemplateTargetTypeDef]],
+        "Tags": NotRequired[Mapping[str, str]],
+    },
+)
+CreateEventBridgeRuleTemplateResponseTypeDef = TypedDict(
+    "CreateEventBridgeRuleTemplateResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "EventTargets": List[EventBridgeRuleTemplateTargetTypeDef],
+        "EventType": EventBridgeRuleTemplateEventTypeType,
+        "GroupId": str,
+        "Id": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetEventBridgeRuleTemplateResponseTypeDef = TypedDict(
+    "GetEventBridgeRuleTemplateResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "EventTargets": List[EventBridgeRuleTemplateTargetTypeDef],
+        "EventType": EventBridgeRuleTemplateEventTypeType,
+        "GroupId": str,
+        "Id": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateEventBridgeRuleTemplateRequestRequestTypeDef = TypedDict(
+    "UpdateEventBridgeRuleTemplateRequestRequestTypeDef",
+    {
+        "Identifier": str,
+        "Description": NotRequired[str],
+        "EventTargets": NotRequired[Sequence[EventBridgeRuleTemplateTargetTypeDef]],
+        "EventType": NotRequired[EventBridgeRuleTemplateEventTypeType],
+        "GroupIdentifier": NotRequired[str],
+        "Name": NotRequired[str],
+    },
+)
+UpdateEventBridgeRuleTemplateResponseTypeDef = TypedDict(
+    "UpdateEventBridgeRuleTemplateResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "EventTargets": List[EventBridgeRuleTemplateTargetTypeDef],
+        "EventType": EventBridgeRuleTemplateEventTypeType,
+        "GroupId": str,
+        "Id": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreateInputRequestRequestTypeDef = TypedDict(
     "CreateInputRequestRequestTypeDef",
     {
         "Destinations": NotRequired[Sequence[InputDestinationRequestTypeDef]],
         "InputDevices": NotRequired[Sequence[InputDeviceSettingsTypeDef]],
         "InputSecurityGroups": NotRequired[Sequence[str]],
         "MediaConnectFlows": NotRequired[Sequence[MediaConnectFlowRequestTypeDef]],
@@ -2643,14 +3263,42 @@
 DescribeMultiplexRequestMultiplexStoppedWaitTypeDef = TypedDict(
     "DescribeMultiplexRequestMultiplexStoppedWaitTypeDef",
     {
         "MultiplexId": str,
         "WaiterConfig": NotRequired[WaiterConfigTypeDef],
     },
 )
+GetSignalMapRequestSignalMapCreatedWaitTypeDef = TypedDict(
+    "GetSignalMapRequestSignalMapCreatedWaitTypeDef",
+    {
+        "Identifier": str,
+        "WaiterConfig": NotRequired[WaiterConfigTypeDef],
+    },
+)
+GetSignalMapRequestSignalMapMonitorDeletedWaitTypeDef = TypedDict(
+    "GetSignalMapRequestSignalMapMonitorDeletedWaitTypeDef",
+    {
+        "Identifier": str,
+        "WaiterConfig": NotRequired[WaiterConfigTypeDef],
+    },
+)
+GetSignalMapRequestSignalMapMonitorDeployedWaitTypeDef = TypedDict(
+    "GetSignalMapRequestSignalMapMonitorDeployedWaitTypeDef",
+    {
+        "Identifier": str,
+        "WaiterConfig": NotRequired[WaiterConfigTypeDef],
+    },
+)
+GetSignalMapRequestSignalMapUpdatedWaitTypeDef = TypedDict(
+    "GetSignalMapRequestSignalMapUpdatedWaitTypeDef",
+    {
+        "Identifier": str,
+        "WaiterConfig": NotRequired[WaiterConfigTypeDef],
+    },
+)
 DescribeInputSecurityGroupResponseTypeDef = TypedDict(
     "DescribeInputSecurityGroupResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Inputs": List[str],
         "State": InputSecurityGroupStateType,
@@ -2679,14 +3327,50 @@
 )
 ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
     "ListChannelsRequestListChannelsPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListCloudWatchAlarmTemplateGroupsRequestListCloudWatchAlarmTemplateGroupsPaginateTypeDef = (
+    TypedDict(
+        "ListCloudWatchAlarmTemplateGroupsRequestListCloudWatchAlarmTemplateGroupsPaginateTypeDef",
+        {
+            "Scope": NotRequired[str],
+            "SignalMapIdentifier": NotRequired[str],
+            "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+        },
+    )
+)
+ListCloudWatchAlarmTemplatesRequestListCloudWatchAlarmTemplatesPaginateTypeDef = TypedDict(
+    "ListCloudWatchAlarmTemplatesRequestListCloudWatchAlarmTemplatesPaginateTypeDef",
+    {
+        "GroupIdentifier": NotRequired[str],
+        "Scope": NotRequired[str],
+        "SignalMapIdentifier": NotRequired[str],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
+ListEventBridgeRuleTemplateGroupsRequestListEventBridgeRuleTemplateGroupsPaginateTypeDef = (
+    TypedDict(
+        "ListEventBridgeRuleTemplateGroupsRequestListEventBridgeRuleTemplateGroupsPaginateTypeDef",
+        {
+            "SignalMapIdentifier": NotRequired[str],
+            "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+        },
+    )
+)
+ListEventBridgeRuleTemplatesRequestListEventBridgeRuleTemplatesPaginateTypeDef = TypedDict(
+    "ListEventBridgeRuleTemplatesRequestListEventBridgeRuleTemplatesPaginateTypeDef",
+    {
+        "GroupIdentifier": NotRequired[str],
+        "SignalMapIdentifier": NotRequired[str],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
     "ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
     {
         "TransferType": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
@@ -2747,14 +3431,22 @@
         "Resolution": NotRequired[str],
         "ResourceType": NotRequired[str],
         "SpecialFeature": NotRequired[str],
         "VideoQuality": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListSignalMapsRequestListSignalMapsPaginateTypeDef = TypedDict(
+    "ListSignalMapsRequestListSignalMapsPaginateTypeDef",
+    {
+        "CloudWatchAlarmTemplateGroupIdentifier": NotRequired[str],
+        "EventBridgeRuleTemplateGroupIdentifier": NotRequired[str],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 M2tsSettingsTypeDef = TypedDict(
     "M2tsSettingsTypeDef",
     {
         "AbsentInputAudioBehavior": NotRequired[M2tsAbsentInputAudioBehaviorType],
         "Arib": NotRequired[M2tsAribType],
         "AribCaptionsPid": NotRequired[str],
         "AribCaptionsPidControl": NotRequired[M2tsAribCaptionsPidControlType],
@@ -2807,14 +3499,30 @@
 OutputLockingSettingsTypeDef = TypedDict(
     "OutputLockingSettingsTypeDef",
     {
         "EpochLockingSettings": NotRequired[EpochLockingSettingsTypeDef],
         "PipelineLockingSettings": NotRequired[Mapping[str, Any]],
     },
 )
+ListEventBridgeRuleTemplateGroupsResponseTypeDef = TypedDict(
+    "ListEventBridgeRuleTemplateGroupsResponseTypeDef",
+    {
+        "EventBridgeRuleTemplateGroups": List[EventBridgeRuleTemplateGroupSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListEventBridgeRuleTemplatesResponseTypeDef = TypedDict(
+    "ListEventBridgeRuleTemplatesResponseTypeDef",
+    {
+        "EventBridgeRuleTemplates": List[EventBridgeRuleTemplateSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 FailoverConditionSettingsTypeDef = TypedDict(
     "FailoverConditionSettingsTypeDef",
     {
         "AudioSilenceSettings": NotRequired[AudioSilenceFailoverSettingsTypeDef],
         "InputLossSettings": NotRequired[InputLossFailoverSettingsTypeDef],
         "VideoBlackSettings": NotRequired[VideoBlackFailoverSettingsTypeDef],
     },
@@ -2980,21 +3688,37 @@
     "ListMultiplexProgramsResponseTypeDef",
     {
         "MultiplexPrograms": List[MultiplexProgramSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListSignalMapsResponseTypeDef = TypedDict(
+    "ListSignalMapsResponseTypeDef",
+    {
+        "NextToken": str,
+        "SignalMaps": List[SignalMapSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 StandardHlsSettingsTypeDef = TypedDict(
     "StandardHlsSettingsTypeDef",
     {
         "M3u8Settings": M3u8SettingsTypeDef,
         "AudioRenditionSets": NotRequired[str],
     },
 )
+MediaResourceTypeDef = TypedDict(
+    "MediaResourceTypeDef",
+    {
+        "Destinations": NotRequired[List[MediaResourceNeighborTypeDef]],
+        "Name": NotRequired[str],
+        "Sources": NotRequired[List[MediaResourceNeighborTypeDef]],
+    },
+)
 MotionGraphicsConfigurationTypeDef = TypedDict(
     "MotionGraphicsConfigurationTypeDef",
     {
         "MotionGraphicsSettings": MotionGraphicsSettingsTypeDef,
         "MotionGraphicsInsertion": NotRequired[MotionGraphicsInsertionType],
     },
 )
@@ -3536,14 +4260,134 @@
     {
         "AudioOnlyHlsSettings": NotRequired[AudioOnlyHlsSettingsTypeDef],
         "Fmp4HlsSettings": NotRequired[Fmp4HlsSettingsTypeDef],
         "FrameCaptureHlsSettings": NotRequired[Mapping[str, Any]],
         "StandardHlsSettings": NotRequired[StandardHlsSettingsTypeDef],
     },
 )
+CreateSignalMapResponseTypeDef = TypedDict(
+    "CreateSignalMapResponseTypeDef",
+    {
+        "Arn": str,
+        "CloudWatchAlarmTemplateGroupIds": List[str],
+        "CreatedAt": datetime,
+        "Description": str,
+        "DiscoveryEntryPointArn": str,
+        "ErrorMessage": str,
+        "EventBridgeRuleTemplateGroupIds": List[str],
+        "FailedMediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "Id": str,
+        "LastDiscoveredAt": datetime,
+        "LastSuccessfulMonitorDeployment": SuccessfulMonitorDeploymentTypeDef,
+        "MediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "ModifiedAt": datetime,
+        "MonitorChangesPendingDeployment": bool,
+        "MonitorDeployment": MonitorDeploymentTypeDef,
+        "Name": str,
+        "Status": SignalMapStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetSignalMapResponseTypeDef = TypedDict(
+    "GetSignalMapResponseTypeDef",
+    {
+        "Arn": str,
+        "CloudWatchAlarmTemplateGroupIds": List[str],
+        "CreatedAt": datetime,
+        "Description": str,
+        "DiscoveryEntryPointArn": str,
+        "ErrorMessage": str,
+        "EventBridgeRuleTemplateGroupIds": List[str],
+        "FailedMediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "Id": str,
+        "LastDiscoveredAt": datetime,
+        "LastSuccessfulMonitorDeployment": SuccessfulMonitorDeploymentTypeDef,
+        "MediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "ModifiedAt": datetime,
+        "MonitorChangesPendingDeployment": bool,
+        "MonitorDeployment": MonitorDeploymentTypeDef,
+        "Name": str,
+        "Status": SignalMapStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+StartDeleteMonitorDeploymentResponseTypeDef = TypedDict(
+    "StartDeleteMonitorDeploymentResponseTypeDef",
+    {
+        "Arn": str,
+        "CloudWatchAlarmTemplateGroupIds": List[str],
+        "CreatedAt": datetime,
+        "Description": str,
+        "DiscoveryEntryPointArn": str,
+        "ErrorMessage": str,
+        "EventBridgeRuleTemplateGroupIds": List[str],
+        "FailedMediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "Id": str,
+        "LastDiscoveredAt": datetime,
+        "LastSuccessfulMonitorDeployment": SuccessfulMonitorDeploymentTypeDef,
+        "MediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "ModifiedAt": datetime,
+        "MonitorChangesPendingDeployment": bool,
+        "MonitorDeployment": MonitorDeploymentTypeDef,
+        "Name": str,
+        "Status": SignalMapStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+StartMonitorDeploymentResponseTypeDef = TypedDict(
+    "StartMonitorDeploymentResponseTypeDef",
+    {
+        "Arn": str,
+        "CloudWatchAlarmTemplateGroupIds": List[str],
+        "CreatedAt": datetime,
+        "Description": str,
+        "DiscoveryEntryPointArn": str,
+        "ErrorMessage": str,
+        "EventBridgeRuleTemplateGroupIds": List[str],
+        "FailedMediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "Id": str,
+        "LastDiscoveredAt": datetime,
+        "LastSuccessfulMonitorDeployment": SuccessfulMonitorDeploymentTypeDef,
+        "MediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "ModifiedAt": datetime,
+        "MonitorChangesPendingDeployment": bool,
+        "MonitorDeployment": MonitorDeploymentTypeDef,
+        "Name": str,
+        "Status": SignalMapStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+StartUpdateSignalMapResponseTypeDef = TypedDict(
+    "StartUpdateSignalMapResponseTypeDef",
+    {
+        "Arn": str,
+        "CloudWatchAlarmTemplateGroupIds": List[str],
+        "CreatedAt": datetime,
+        "Description": str,
+        "DiscoveryEntryPointArn": str,
+        "ErrorMessage": str,
+        "EventBridgeRuleTemplateGroupIds": List[str],
+        "FailedMediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "Id": str,
+        "LastDiscoveredAt": datetime,
+        "LastSuccessfulMonitorDeployment": SuccessfulMonitorDeploymentTypeDef,
+        "MediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "ModifiedAt": datetime,
+        "MonitorChangesPendingDeployment": bool,
+        "MonitorDeployment": MonitorDeploymentTypeDef,
+        "Name": str,
+        "Status": SignalMapStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DeleteMultiplexResponseTypeDef = TypedDict(
     "DeleteMultiplexResponseTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
```

### Comparing `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/type_defs.pyi` & `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/type_defs.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -51,14 +51,18 @@
     BurnInOutlineColorType,
     BurnInShadowColorType,
     BurnInTeletextGridControlType,
     CdiInputResolutionType,
     ChannelClassType,
     ChannelPipelineIdToRestartType,
     ChannelStateType,
+    CloudWatchAlarmTemplateComparisonOperatorType,
+    CloudWatchAlarmTemplateStatisticType,
+    CloudWatchAlarmTemplateTargetResourceTypeType,
+    CloudWatchAlarmTemplateTreatMissingDataType,
     CmafIngestSegmentLengthUnitsType,
     CmafNielsenId3BehaviorType,
     ColorSpaceType,
     DashRoleAudioType,
     DashRoleCaptionType,
     DeviceSettingsSyncStateType,
     DeviceUpdateStatusType,
@@ -89,14 +93,15 @@
     Eac3StereoDownmixType,
     Eac3SurroundExModeType,
     Eac3SurroundModeType,
     EbuTtDDestinationStyleControlType,
     EbuTtDFillLineGapControlType,
     EmbeddedConvert608To708Type,
     EmbeddedScte20DetectionType,
+    EventBridgeRuleTemplateEventTypeType,
     FeatureActivationsInputPrepareScheduleActionsType,
     FeatureActivationsOutputStaticImageOverlayScheduleActionsType,
     FecOutputIncludeFecType,
     FixedAfdType,
     Fmp4NielsenId3BehaviorType,
     Fmp4TimedMetadataBehaviorType,
     FollowPointType,
@@ -271,14 +276,16 @@
     Scte35InputModeType,
     Scte35NoRegionalBlackoutFlagType,
     Scte35SegmentationCancelIndicatorType,
     Scte35SpliceInsertNoRegionalBlackoutBehaviorType,
     Scte35SpliceInsertWebDeliveryAllowedBehaviorType,
     Scte35TypeType,
     Scte35WebDeliveryAllowedFlagType,
+    SignalMapMonitorDeploymentStatusType,
+    SignalMapStatusType,
     SmoothGroupAudioOnlyTimecodeControlType,
     SmoothGroupCertificateModeType,
     SmoothGroupEventIdModeType,
     SmoothGroupEventStopBehaviorType,
     SmoothGroupSegmentationModeType,
     SmoothGroupSparseTrackTypeType,
     SmoothGroupStreamManifestBehaviorType,
@@ -358,38 +365,52 @@
     "CdiInputSpecificationTypeDef",
     "ChannelEgressEndpointTypeDef",
     "InputSpecificationTypeDef",
     "MaintenanceStatusTypeDef",
     "VpcOutputSettingsDescriptionTypeDef",
     "PipelineDetailTypeDef",
     "ClaimDeviceRequestRequestTypeDef",
+    "CloudWatchAlarmTemplateGroupSummaryTypeDef",
+    "CloudWatchAlarmTemplateSummaryTypeDef",
     "CmafIngestOutputSettingsTypeDef",
     "ColorCorrectionTypeDef",
     "MaintenanceCreateSettingsTypeDef",
     "VpcOutputSettingsTypeDef",
+    "CreateCloudWatchAlarmTemplateGroupRequestRequestTypeDef",
+    "CreateCloudWatchAlarmTemplateRequestRequestTypeDef",
+    "CreateEventBridgeRuleTemplateGroupRequestRequestTypeDef",
+    "EventBridgeRuleTemplateTargetTypeDef",
     "InputDestinationRequestTypeDef",
     "InputDeviceSettingsTypeDef",
     "InputSourceRequestTypeDef",
     "InputVpcRequestTypeDef",
     "MediaConnectFlowRequestTypeDef",
     "InputWhitelistRuleCidrTypeDef",
     "MultiplexSettingsTypeDef",
     "CreatePartnerInputRequestRequestTypeDef",
+    "CreateSignalMapRequestRequestTypeDef",
+    "MonitorDeploymentTypeDef",
+    "SuccessfulMonitorDeploymentTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
+    "DeleteCloudWatchAlarmTemplateGroupRequestRequestTypeDef",
+    "DeleteCloudWatchAlarmTemplateRequestRequestTypeDef",
+    "DeleteEventBridgeRuleTemplateGroupRequestRequestTypeDef",
+    "DeleteEventBridgeRuleTemplateRequestRequestTypeDef",
     "DeleteInputRequestRequestTypeDef",
     "DeleteInputSecurityGroupRequestRequestTypeDef",
     "DeleteMultiplexProgramRequestRequestTypeDef",
     "MultiplexProgramPacketIdentifiersMapTypeDef",
     "MultiplexProgramPipelineDetailTypeDef",
     "DeleteMultiplexRequestRequestTypeDef",
     "DeleteReservationRequestRequestTypeDef",
     "RenewalSettingsTypeDef",
     "ReservationResourceSpecificationTypeDef",
     "DeleteScheduleRequestRequestTypeDef",
+    "DeleteSignalMapRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeInputDeviceRequestRequestTypeDef",
     "InputDeviceHdSettingsTypeDef",
     "InputDeviceNetworkSettingsTypeDef",
     "DescribeInputDeviceThumbnailRequestRequestTypeDef",
@@ -409,23 +430,30 @@
     "DvbSdtSettingsTypeDef",
     "DvbTdtSettingsTypeDef",
     "FeatureActivationsTypeDef",
     "NielsenConfigurationTypeDef",
     "ThumbnailConfigurationTypeDef",
     "TimecodeConfigTypeDef",
     "EpochLockingSettingsTypeDef",
+    "EventBridgeRuleTemplateGroupSummaryTypeDef",
+    "EventBridgeRuleTemplateSummaryTypeDef",
     "InputLossFailoverSettingsTypeDef",
     "VideoBlackFailoverSettingsTypeDef",
     "FecOutputSettingsTypeDef",
     "FixedModeScheduleActionStartSettingsTypeDef",
     "Fmp4HlsSettingsTypeDef",
     "FollowModeScheduleActionStartSettingsTypeDef",
     "FrameCaptureS3SettingsTypeDef",
     "FrameCaptureOutputSettingsTypeDef",
     "TimecodeBurninSettingsTypeDef",
+    "GetCloudWatchAlarmTemplateGroupRequestRequestTypeDef",
+    "GetCloudWatchAlarmTemplateRequestRequestTypeDef",
+    "GetEventBridgeRuleTemplateGroupRequestRequestTypeDef",
+    "GetEventBridgeRuleTemplateRequestRequestTypeDef",
+    "GetSignalMapRequestRequestTypeDef",
     "H264ColorSpaceSettingsTypeDef",
     "TemporalFilterSettingsTypeDef",
     "Hdr10SettingsTypeDef",
     "HlsAkamaiSettingsTypeDef",
     "HlsBasicPutSettingsTypeDef",
     "HlsMediaStoreSettingsTypeDef",
     "HlsS3SettingsTypeDef",
@@ -438,28 +466,35 @@
     "InputDestinationVpcTypeDef",
     "InputDeviceConfigurableAudioChannelPairConfigTypeDef",
     "InputDeviceMediaConnectConfigurableSettingsTypeDef",
     "InputDeviceMediaConnectSettingsTypeDef",
     "InputDeviceRequestTypeDef",
     "InputDeviceUhdAudioChannelPairConfigTypeDef",
     "ListChannelsRequestRequestTypeDef",
+    "ListCloudWatchAlarmTemplateGroupsRequestRequestTypeDef",
+    "ListCloudWatchAlarmTemplatesRequestRequestTypeDef",
+    "ListEventBridgeRuleTemplateGroupsRequestRequestTypeDef",
+    "ListEventBridgeRuleTemplatesRequestRequestTypeDef",
     "ListInputDeviceTransfersRequestRequestTypeDef",
     "TransferringInputDeviceSummaryTypeDef",
     "ListInputDevicesRequestRequestTypeDef",
     "ListInputSecurityGroupsRequestRequestTypeDef",
     "ListInputsRequestRequestTypeDef",
     "ListMultiplexProgramsRequestRequestTypeDef",
     "MultiplexProgramSummaryTypeDef",
     "ListMultiplexesRequestRequestTypeDef",
     "ListOfferingsRequestRequestTypeDef",
     "ListReservationsRequestRequestTypeDef",
+    "ListSignalMapsRequestRequestTypeDef",
+    "SignalMapSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "M3u8SettingsTypeDef",
     "MaintenanceUpdateSettingsTypeDef",
     "MediaPackageOutputDestinationSettingsTypeDef",
+    "MediaResourceNeighborTypeDef",
     "MotionGraphicsActivateScheduleActionSettingsTypeDef",
     "MotionGraphicsSettingsTypeDef",
     "MsSmoothOutputSettingsTypeDef",
     "MultiplexMediaConnectOutputDestinationSettingsTypeDef",
     "MultiplexProgramChannelDestinationSettingsTypeDef",
     "MultiplexProgramServiceDescriptorTypeDef",
     "MultiplexSettingsSummaryTypeDef",
@@ -477,22 +512,28 @@
     "Scte35ReturnToNetworkScheduleActionSettingsTypeDef",
     "Scte35SpliceInsertScheduleActionSettingsTypeDef",
     "StaticImageDeactivateScheduleActionSettingsTypeDef",
     "StaticImageOutputDeactivateScheduleActionSettingsPaginatorTypeDef",
     "StaticImageOutputDeactivateScheduleActionSettingsTypeDef",
     "Scte35DeliveryRestrictionsTypeDef",
     "StartChannelRequestRequestTypeDef",
+    "StartDeleteMonitorDeploymentRequestRequestTypeDef",
     "StartInputDeviceMaintenanceWindowRequestRequestTypeDef",
     "StartInputDeviceRequestRequestTypeDef",
+    "StartMonitorDeploymentRequestRequestTypeDef",
     "StartMultiplexRequestRequestTypeDef",
+    "StartUpdateSignalMapRequestRequestTypeDef",
     "StopChannelRequestRequestTypeDef",
     "StopInputDeviceRequestRequestTypeDef",
     "StopMultiplexRequestRequestTypeDef",
     "ThumbnailTypeDef",
     "TransferInputDeviceRequestRequestTypeDef",
+    "UpdateCloudWatchAlarmTemplateGroupRequestRequestTypeDef",
+    "UpdateCloudWatchAlarmTemplateRequestRequestTypeDef",
+    "UpdateEventBridgeRuleTemplateGroupRequestRequestTypeDef",
     "VideoSelectorPidTypeDef",
     "VideoSelectorProgramIdTypeDef",
     "UpdateAccountConfigurationRequestRequestTypeDef",
     "ArchiveCdnSettingsTypeDef",
     "CmafIngestGroupSettingsTypeDef",
     "MediaPackageGroupSettingsTypeDef",
     "MsSmoothGroupSettingsTypeDef",
@@ -512,21 +553,37 @@
     "StaticKeySettingsTypeDef",
     "AudioTrackSelectionPaginatorTypeDef",
     "AudioTrackSelectionTypeDef",
     "AvailSettingsTypeDef",
     "BatchDeleteResponseTypeDef",
     "BatchStartResponseTypeDef",
     "BatchStopResponseTypeDef",
+    "CreateCloudWatchAlarmTemplateGroupResponseTypeDef",
+    "CreateCloudWatchAlarmTemplateResponseTypeDef",
+    "CreateEventBridgeRuleTemplateGroupResponseTypeDef",
     "DescribeAccountConfigurationResponseTypeDef",
     "DescribeInputDeviceThumbnailResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "GetCloudWatchAlarmTemplateGroupResponseTypeDef",
+    "GetCloudWatchAlarmTemplateResponseTypeDef",
+    "GetEventBridgeRuleTemplateGroupResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateAccountConfigurationResponseTypeDef",
+    "UpdateCloudWatchAlarmTemplateGroupResponseTypeDef",
+    "UpdateCloudWatchAlarmTemplateResponseTypeDef",
+    "UpdateEventBridgeRuleTemplateGroupResponseTypeDef",
     "TeletextSourceSettingsTypeDef",
+    "ListCloudWatchAlarmTemplateGroupsResponseTypeDef",
+    "ListCloudWatchAlarmTemplatesResponseTypeDef",
     "ColorCorrectionSettingsTypeDef",
+    "CreateEventBridgeRuleTemplateRequestRequestTypeDef",
+    "CreateEventBridgeRuleTemplateResponseTypeDef",
+    "GetEventBridgeRuleTemplateResponseTypeDef",
+    "UpdateEventBridgeRuleTemplateRequestRequestTypeDef",
+    "UpdateEventBridgeRuleTemplateResponseTypeDef",
     "CreateInputRequestRequestTypeDef",
     "CreateInputSecurityGroupRequestRequestTypeDef",
     "UpdateInputSecurityGroupRequestRequestTypeDef",
     "CreateMultiplexRequestRequestTypeDef",
     "UpdateMultiplexRequestRequestTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
     "UpdateReservationRequestRequestTypeDef",
@@ -542,28 +599,39 @@
     "DescribeInputRequestInputAttachedWaitTypeDef",
     "DescribeInputRequestInputDeletedWaitTypeDef",
     "DescribeInputRequestInputDetachedWaitTypeDef",
     "DescribeMultiplexRequestMultiplexCreatedWaitTypeDef",
     "DescribeMultiplexRequestMultiplexDeletedWaitTypeDef",
     "DescribeMultiplexRequestMultiplexRunningWaitTypeDef",
     "DescribeMultiplexRequestMultiplexStoppedWaitTypeDef",
+    "GetSignalMapRequestSignalMapCreatedWaitTypeDef",
+    "GetSignalMapRequestSignalMapMonitorDeletedWaitTypeDef",
+    "GetSignalMapRequestSignalMapMonitorDeployedWaitTypeDef",
+    "GetSignalMapRequestSignalMapUpdatedWaitTypeDef",
     "DescribeInputSecurityGroupResponseTypeDef",
     "InputSecurityGroupTypeDef",
     "DescribeScheduleRequestDescribeSchedulePaginateTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
+    "ListCloudWatchAlarmTemplateGroupsRequestListCloudWatchAlarmTemplateGroupsPaginateTypeDef",
+    "ListCloudWatchAlarmTemplatesRequestListCloudWatchAlarmTemplatesPaginateTypeDef",
+    "ListEventBridgeRuleTemplateGroupsRequestListEventBridgeRuleTemplateGroupsPaginateTypeDef",
+    "ListEventBridgeRuleTemplatesRequestListEventBridgeRuleTemplatesPaginateTypeDef",
     "ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
     "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
     "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
     "ListInputsRequestListInputsPaginateTypeDef",
     "ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
     "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
     "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListReservationsRequestListReservationsPaginateTypeDef",
+    "ListSignalMapsRequestListSignalMapsPaginateTypeDef",
     "M2tsSettingsTypeDef",
     "OutputLockingSettingsTypeDef",
+    "ListEventBridgeRuleTemplateGroupsResponseTypeDef",
+    "ListEventBridgeRuleTemplatesResponseTypeDef",
     "FailoverConditionSettingsTypeDef",
     "ScheduleActionStartSettingsPaginatorTypeDef",
     "ScheduleActionStartSettingsTypeDef",
     "FrameCaptureCdnSettingsTypeDef",
     "FrameCaptureSettingsTypeDef",
     "H264FilterSettingsTypeDef",
     "H265FilterSettingsTypeDef",
@@ -575,15 +643,17 @@
     "InputClippingSettingsTypeDef",
     "InputDestinationTypeDef",
     "InputDeviceConfigurableSettingsTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "InputDeviceUhdSettingsTypeDef",
     "ListInputDeviceTransfersResponseTypeDef",
     "ListMultiplexProgramsResponseTypeDef",
+    "ListSignalMapsResponseTypeDef",
     "StandardHlsSettingsTypeDef",
+    "MediaResourceTypeDef",
     "MotionGraphicsConfigurationTypeDef",
     "MultiplexOutputDestinationTypeDef",
     "MultiplexSummaryTypeDef",
     "MultiplexVideoSettingsTypeDef",
     "NielsenWatermarksSettingsTypeDef",
     "OutputDestinationPaginatorTypeDef",
     "OutputDestinationTypeDef",
@@ -623,14 +693,19 @@
     "DescribeInputResponseTypeDef",
     "InputTypeDef",
     "UpdateInputDeviceRequestRequestTypeDef",
     "DescribeInputDeviceResponseTypeDef",
     "InputDeviceSummaryTypeDef",
     "UpdateInputDeviceResponseTypeDef",
     "HlsSettingsTypeDef",
+    "CreateSignalMapResponseTypeDef",
+    "GetSignalMapResponseTypeDef",
+    "StartDeleteMonitorDeploymentResponseTypeDef",
+    "StartMonitorDeploymentResponseTypeDef",
+    "StartUpdateSignalMapResponseTypeDef",
     "DeleteMultiplexResponseTypeDef",
     "DescribeMultiplexResponseTypeDef",
     "MultiplexTypeDef",
     "StartMultiplexResponseTypeDef",
     "StopMultiplexResponseTypeDef",
     "ListMultiplexesResponseTypeDef",
     "MultiplexProgramSettingsTypeDef",
@@ -1086,14 +1161,49 @@
 )
 ClaimDeviceRequestRequestTypeDef = TypedDict(
     "ClaimDeviceRequestRequestTypeDef",
     {
         "Id": NotRequired[str],
     },
 )
+CloudWatchAlarmTemplateGroupSummaryTypeDef = TypedDict(
+    "CloudWatchAlarmTemplateGroupSummaryTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Id": str,
+        "Name": str,
+        "TemplateCount": int,
+        "Description": NotRequired[str],
+        "ModifiedAt": NotRequired[datetime],
+        "Tags": NotRequired[Dict[str, str]],
+    },
+)
+CloudWatchAlarmTemplateSummaryTypeDef = TypedDict(
+    "CloudWatchAlarmTemplateSummaryTypeDef",
+    {
+        "Arn": str,
+        "ComparisonOperator": CloudWatchAlarmTemplateComparisonOperatorType,
+        "CreatedAt": datetime,
+        "EvaluationPeriods": int,
+        "GroupId": str,
+        "Id": str,
+        "MetricName": str,
+        "Name": str,
+        "Period": int,
+        "Statistic": CloudWatchAlarmTemplateStatisticType,
+        "TargetResourceType": CloudWatchAlarmTemplateTargetResourceTypeType,
+        "Threshold": float,
+        "TreatMissingData": CloudWatchAlarmTemplateTreatMissingDataType,
+        "DatapointsToAlarm": NotRequired[int],
+        "Description": NotRequired[str],
+        "ModifiedAt": NotRequired[datetime],
+        "Tags": NotRequired[Dict[str, str]],
+    },
+)
 CmafIngestOutputSettingsTypeDef = TypedDict(
     "CmafIngestOutputSettingsTypeDef",
     {
         "NameModifier": NotRequired[str],
     },
 )
 ColorCorrectionTypeDef = TypedDict(
@@ -1115,14 +1225,54 @@
     "VpcOutputSettingsTypeDef",
     {
         "SubnetIds": Sequence[str],
         "PublicAddressAllocationIds": NotRequired[Sequence[str]],
         "SecurityGroupIds": NotRequired[Sequence[str]],
     },
 )
+CreateCloudWatchAlarmTemplateGroupRequestRequestTypeDef = TypedDict(
+    "CreateCloudWatchAlarmTemplateGroupRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Description": NotRequired[str],
+        "Tags": NotRequired[Mapping[str, str]],
+    },
+)
+CreateCloudWatchAlarmTemplateRequestRequestTypeDef = TypedDict(
+    "CreateCloudWatchAlarmTemplateRequestRequestTypeDef",
+    {
+        "ComparisonOperator": CloudWatchAlarmTemplateComparisonOperatorType,
+        "EvaluationPeriods": int,
+        "GroupIdentifier": str,
+        "MetricName": str,
+        "Name": str,
+        "Period": int,
+        "Statistic": CloudWatchAlarmTemplateStatisticType,
+        "TargetResourceType": CloudWatchAlarmTemplateTargetResourceTypeType,
+        "Threshold": float,
+        "TreatMissingData": CloudWatchAlarmTemplateTreatMissingDataType,
+        "DatapointsToAlarm": NotRequired[int],
+        "Description": NotRequired[str],
+        "Tags": NotRequired[Mapping[str, str]],
+    },
+)
+CreateEventBridgeRuleTemplateGroupRequestRequestTypeDef = TypedDict(
+    "CreateEventBridgeRuleTemplateGroupRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Description": NotRequired[str],
+        "Tags": NotRequired[Mapping[str, str]],
+    },
+)
+EventBridgeRuleTemplateTargetTypeDef = TypedDict(
+    "EventBridgeRuleTemplateTargetTypeDef",
+    {
+        "Arn": str,
+    },
+)
 InputDestinationRequestTypeDef = TypedDict(
     "InputDestinationRequestTypeDef",
     {
         "StreamName": NotRequired[str],
     },
 )
 InputDeviceSettingsTypeDef = TypedDict(
@@ -1171,27 +1321,77 @@
     "CreatePartnerInputRequestRequestTypeDef",
     {
         "InputId": str,
         "RequestId": NotRequired[str],
         "Tags": NotRequired[Mapping[str, str]],
     },
 )
+CreateSignalMapRequestRequestTypeDef = TypedDict(
+    "CreateSignalMapRequestRequestTypeDef",
+    {
+        "DiscoveryEntryPointArn": str,
+        "Name": str,
+        "CloudWatchAlarmTemplateGroupIdentifiers": NotRequired[Sequence[str]],
+        "Description": NotRequired[str],
+        "EventBridgeRuleTemplateGroupIdentifiers": NotRequired[Sequence[str]],
+        "Tags": NotRequired[Mapping[str, str]],
+    },
+)
+MonitorDeploymentTypeDef = TypedDict(
+    "MonitorDeploymentTypeDef",
+    {
+        "Status": SignalMapMonitorDeploymentStatusType,
+        "DetailsUri": NotRequired[str],
+        "ErrorMessage": NotRequired[str],
+    },
+)
+SuccessfulMonitorDeploymentTypeDef = TypedDict(
+    "SuccessfulMonitorDeploymentTypeDef",
+    {
+        "DetailsUri": str,
+        "Status": SignalMapMonitorDeploymentStatusType,
+    },
+)
 CreateTagsRequestRequestTypeDef = TypedDict(
     "CreateTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": NotRequired[Mapping[str, str]],
     },
 )
 DeleteChannelRequestRequestTypeDef = TypedDict(
     "DeleteChannelRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
+DeleteCloudWatchAlarmTemplateGroupRequestRequestTypeDef = TypedDict(
+    "DeleteCloudWatchAlarmTemplateGroupRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+DeleteCloudWatchAlarmTemplateRequestRequestTypeDef = TypedDict(
+    "DeleteCloudWatchAlarmTemplateRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+DeleteEventBridgeRuleTemplateGroupRequestRequestTypeDef = TypedDict(
+    "DeleteEventBridgeRuleTemplateGroupRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+DeleteEventBridgeRuleTemplateRequestRequestTypeDef = TypedDict(
+    "DeleteEventBridgeRuleTemplateRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
 DeleteInputRequestRequestTypeDef = TypedDict(
     "DeleteInputRequestRequestTypeDef",
     {
         "InputId": str,
     },
 )
 DeleteInputSecurityGroupRequestRequestTypeDef = TypedDict(
@@ -1266,14 +1466,20 @@
 )
 DeleteScheduleRequestRequestTypeDef = TypedDict(
     "DeleteScheduleRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
+DeleteSignalMapRequestRequestTypeDef = TypedDict(
+    "DeleteSignalMapRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
 DeleteTagsRequestRequestTypeDef = TypedDict(
     "DeleteTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1465,14 +1671,42 @@
 EpochLockingSettingsTypeDef = TypedDict(
     "EpochLockingSettingsTypeDef",
     {
         "CustomEpoch": NotRequired[str],
         "JamSyncTime": NotRequired[str],
     },
 )
+EventBridgeRuleTemplateGroupSummaryTypeDef = TypedDict(
+    "EventBridgeRuleTemplateGroupSummaryTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Id": str,
+        "Name": str,
+        "TemplateCount": int,
+        "Description": NotRequired[str],
+        "ModifiedAt": NotRequired[datetime],
+        "Tags": NotRequired[Dict[str, str]],
+    },
+)
+EventBridgeRuleTemplateSummaryTypeDef = TypedDict(
+    "EventBridgeRuleTemplateSummaryTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "EventTargetCount": int,
+        "EventType": EventBridgeRuleTemplateEventTypeType,
+        "GroupId": str,
+        "Id": str,
+        "Name": str,
+        "Description": NotRequired[str],
+        "ModifiedAt": NotRequired[datetime],
+        "Tags": NotRequired[Dict[str, str]],
+    },
+)
 InputLossFailoverSettingsTypeDef = TypedDict(
     "InputLossFailoverSettingsTypeDef",
     {
         "InputLossThresholdMsec": NotRequired[int],
     },
 )
 VideoBlackFailoverSettingsTypeDef = TypedDict(
@@ -1527,14 +1761,44 @@
     "TimecodeBurninSettingsTypeDef",
     {
         "FontSize": TimecodeBurninFontSizeType,
         "Position": TimecodeBurninPositionType,
         "Prefix": NotRequired[str],
     },
 )
+GetCloudWatchAlarmTemplateGroupRequestRequestTypeDef = TypedDict(
+    "GetCloudWatchAlarmTemplateGroupRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+GetCloudWatchAlarmTemplateRequestRequestTypeDef = TypedDict(
+    "GetCloudWatchAlarmTemplateRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+GetEventBridgeRuleTemplateGroupRequestRequestTypeDef = TypedDict(
+    "GetEventBridgeRuleTemplateGroupRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+GetEventBridgeRuleTemplateRequestRequestTypeDef = TypedDict(
+    "GetEventBridgeRuleTemplateRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
+GetSignalMapRequestRequestTypeDef = TypedDict(
+    "GetSignalMapRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
 H264ColorSpaceSettingsTypeDef = TypedDict(
     "H264ColorSpaceSettingsTypeDef",
     {
         "ColorSpacePassthroughSettings": NotRequired[Mapping[str, Any]],
         "Rec601Settings": NotRequired[Mapping[str, Any]],
         "Rec709Settings": NotRequired[Mapping[str, Any]],
     },
@@ -1684,14 +1948,50 @@
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
     },
 )
+ListCloudWatchAlarmTemplateGroupsRequestRequestTypeDef = TypedDict(
+    "ListCloudWatchAlarmTemplateGroupsRequestRequestTypeDef",
+    {
+        "MaxResults": NotRequired[int],
+        "NextToken": NotRequired[str],
+        "Scope": NotRequired[str],
+        "SignalMapIdentifier": NotRequired[str],
+    },
+)
+ListCloudWatchAlarmTemplatesRequestRequestTypeDef = TypedDict(
+    "ListCloudWatchAlarmTemplatesRequestRequestTypeDef",
+    {
+        "GroupIdentifier": NotRequired[str],
+        "MaxResults": NotRequired[int],
+        "NextToken": NotRequired[str],
+        "Scope": NotRequired[str],
+        "SignalMapIdentifier": NotRequired[str],
+    },
+)
+ListEventBridgeRuleTemplateGroupsRequestRequestTypeDef = TypedDict(
+    "ListEventBridgeRuleTemplateGroupsRequestRequestTypeDef",
+    {
+        "MaxResults": NotRequired[int],
+        "NextToken": NotRequired[str],
+        "SignalMapIdentifier": NotRequired[str],
+    },
+)
+ListEventBridgeRuleTemplatesRequestRequestTypeDef = TypedDict(
+    "ListEventBridgeRuleTemplatesRequestRequestTypeDef",
+    {
+        "GroupIdentifier": NotRequired[str],
+        "MaxResults": NotRequired[int],
+        "NextToken": NotRequired[str],
+        "SignalMapIdentifier": NotRequired[str],
+    },
+)
 ListInputDeviceTransfersRequestRequestTypeDef = TypedDict(
     "ListInputDeviceTransfersRequestRequestTypeDef",
     {
         "TransferType": str,
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
     },
@@ -1776,14 +2076,37 @@
         "NextToken": NotRequired[str],
         "Resolution": NotRequired[str],
         "ResourceType": NotRequired[str],
         "SpecialFeature": NotRequired[str],
         "VideoQuality": NotRequired[str],
     },
 )
+ListSignalMapsRequestRequestTypeDef = TypedDict(
+    "ListSignalMapsRequestRequestTypeDef",
+    {
+        "CloudWatchAlarmTemplateGroupIdentifier": NotRequired[str],
+        "EventBridgeRuleTemplateGroupIdentifier": NotRequired[str],
+        "MaxResults": NotRequired[int],
+        "NextToken": NotRequired[str],
+    },
+)
+SignalMapSummaryTypeDef = TypedDict(
+    "SignalMapSummaryTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Id": str,
+        "MonitorDeploymentStatus": SignalMapMonitorDeploymentStatusType,
+        "Name": str,
+        "Status": SignalMapStatusType,
+        "Description": NotRequired[str],
+        "ModifiedAt": NotRequired[datetime],
+        "Tags": NotRequired[Dict[str, str]],
+    },
+)
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 M3u8SettingsTypeDef = TypedDict(
@@ -1820,14 +2143,21 @@
 )
 MediaPackageOutputDestinationSettingsTypeDef = TypedDict(
     "MediaPackageOutputDestinationSettingsTypeDef",
     {
         "ChannelId": NotRequired[str],
     },
 )
+MediaResourceNeighborTypeDef = TypedDict(
+    "MediaResourceNeighborTypeDef",
+    {
+        "Arn": str,
+        "Name": NotRequired[str],
+    },
+)
 MotionGraphicsActivateScheduleActionSettingsTypeDef = TypedDict(
     "MotionGraphicsActivateScheduleActionSettingsTypeDef",
     {
         "Duration": NotRequired[int],
         "PasswordParam": NotRequired[str],
         "Url": NotRequired[str],
         "Username": NotRequired[str],
@@ -2006,32 +2336,57 @@
 )
 StartChannelRequestRequestTypeDef = TypedDict(
     "StartChannelRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
+StartDeleteMonitorDeploymentRequestRequestTypeDef = TypedDict(
+    "StartDeleteMonitorDeploymentRequestRequestTypeDef",
+    {
+        "Identifier": str,
+    },
+)
 StartInputDeviceMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "StartInputDeviceMaintenanceWindowRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
 StartInputDeviceRequestRequestTypeDef = TypedDict(
     "StartInputDeviceRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
+StartMonitorDeploymentRequestRequestTypeDef = TypedDict(
+    "StartMonitorDeploymentRequestRequestTypeDef",
+    {
+        "Identifier": str,
+        "DryRun": NotRequired[bool],
+    },
+)
 StartMultiplexRequestRequestTypeDef = TypedDict(
     "StartMultiplexRequestRequestTypeDef",
     {
         "MultiplexId": str,
     },
 )
+StartUpdateSignalMapRequestRequestTypeDef = TypedDict(
+    "StartUpdateSignalMapRequestRequestTypeDef",
+    {
+        "Identifier": str,
+        "CloudWatchAlarmTemplateGroupIdentifiers": NotRequired[Sequence[str]],
+        "Description": NotRequired[str],
+        "DiscoveryEntryPointArn": NotRequired[str],
+        "EventBridgeRuleTemplateGroupIdentifiers": NotRequired[Sequence[str]],
+        "ForceRediscovery": NotRequired[bool],
+        "Name": NotRequired[str],
+    },
+)
 StopChannelRequestRequestTypeDef = TypedDict(
     "StopChannelRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 StopInputDeviceRequestRequestTypeDef = TypedDict(
@@ -2060,14 +2415,46 @@
     {
         "InputDeviceId": str,
         "TargetCustomerId": NotRequired[str],
         "TargetRegion": NotRequired[str],
         "TransferMessage": NotRequired[str],
     },
 )
+UpdateCloudWatchAlarmTemplateGroupRequestRequestTypeDef = TypedDict(
+    "UpdateCloudWatchAlarmTemplateGroupRequestRequestTypeDef",
+    {
+        "Identifier": str,
+        "Description": NotRequired[str],
+    },
+)
+UpdateCloudWatchAlarmTemplateRequestRequestTypeDef = TypedDict(
+    "UpdateCloudWatchAlarmTemplateRequestRequestTypeDef",
+    {
+        "Identifier": str,
+        "ComparisonOperator": NotRequired[CloudWatchAlarmTemplateComparisonOperatorType],
+        "DatapointsToAlarm": NotRequired[int],
+        "Description": NotRequired[str],
+        "EvaluationPeriods": NotRequired[int],
+        "GroupIdentifier": NotRequired[str],
+        "MetricName": NotRequired[str],
+        "Name": NotRequired[str],
+        "Period": NotRequired[int],
+        "Statistic": NotRequired[CloudWatchAlarmTemplateStatisticType],
+        "TargetResourceType": NotRequired[CloudWatchAlarmTemplateTargetResourceTypeType],
+        "Threshold": NotRequired[float],
+        "TreatMissingData": NotRequired[CloudWatchAlarmTemplateTreatMissingDataType],
+    },
+)
+UpdateEventBridgeRuleTemplateGroupRequestRequestTypeDef = TypedDict(
+    "UpdateEventBridgeRuleTemplateGroupRequestRequestTypeDef",
+    {
+        "Identifier": str,
+        "Description": NotRequired[str],
+    },
+)
 VideoSelectorPidTypeDef = TypedDict(
     "VideoSelectorPidTypeDef",
     {
         "Pid": NotRequired[int],
     },
 )
 VideoSelectorProgramIdTypeDef = TypedDict(
@@ -2339,14 +2726,63 @@
     "BatchStopResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateCloudWatchAlarmTemplateGroupResponseTypeDef = TypedDict(
+    "CreateCloudWatchAlarmTemplateGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "Id": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CreateCloudWatchAlarmTemplateResponseTypeDef = TypedDict(
+    "CreateCloudWatchAlarmTemplateResponseTypeDef",
+    {
+        "Arn": str,
+        "ComparisonOperator": CloudWatchAlarmTemplateComparisonOperatorType,
+        "CreatedAt": datetime,
+        "DatapointsToAlarm": int,
+        "Description": str,
+        "EvaluationPeriods": int,
+        "GroupId": str,
+        "Id": str,
+        "MetricName": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Period": int,
+        "Statistic": CloudWatchAlarmTemplateStatisticType,
+        "Tags": Dict[str, str],
+        "TargetResourceType": CloudWatchAlarmTemplateTargetResourceTypeType,
+        "Threshold": float,
+        "TreatMissingData": CloudWatchAlarmTemplateTreatMissingDataType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CreateEventBridgeRuleTemplateGroupResponseTypeDef = TypedDict(
+    "CreateEventBridgeRuleTemplateGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "Id": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DescribeAccountConfigurationResponseTypeDef = TypedDict(
     "DescribeAccountConfigurationResponseTypeDef",
     {
         "AccountConfiguration": AccountConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2363,41 +2799,225 @@
 )
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+GetCloudWatchAlarmTemplateGroupResponseTypeDef = TypedDict(
+    "GetCloudWatchAlarmTemplateGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "Id": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetCloudWatchAlarmTemplateResponseTypeDef = TypedDict(
+    "GetCloudWatchAlarmTemplateResponseTypeDef",
+    {
+        "Arn": str,
+        "ComparisonOperator": CloudWatchAlarmTemplateComparisonOperatorType,
+        "CreatedAt": datetime,
+        "DatapointsToAlarm": int,
+        "Description": str,
+        "EvaluationPeriods": int,
+        "GroupId": str,
+        "Id": str,
+        "MetricName": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Period": int,
+        "Statistic": CloudWatchAlarmTemplateStatisticType,
+        "Tags": Dict[str, str],
+        "TargetResourceType": CloudWatchAlarmTemplateTargetResourceTypeType,
+        "Threshold": float,
+        "TreatMissingData": CloudWatchAlarmTemplateTreatMissingDataType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetEventBridgeRuleTemplateGroupResponseTypeDef = TypedDict(
+    "GetEventBridgeRuleTemplateGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "Id": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 UpdateAccountConfigurationResponseTypeDef = TypedDict(
     "UpdateAccountConfigurationResponseTypeDef",
     {
         "AccountConfiguration": AccountConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateCloudWatchAlarmTemplateGroupResponseTypeDef = TypedDict(
+    "UpdateCloudWatchAlarmTemplateGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "Id": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateCloudWatchAlarmTemplateResponseTypeDef = TypedDict(
+    "UpdateCloudWatchAlarmTemplateResponseTypeDef",
+    {
+        "Arn": str,
+        "ComparisonOperator": CloudWatchAlarmTemplateComparisonOperatorType,
+        "CreatedAt": datetime,
+        "DatapointsToAlarm": int,
+        "Description": str,
+        "EvaluationPeriods": int,
+        "GroupId": str,
+        "Id": str,
+        "MetricName": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Period": int,
+        "Statistic": CloudWatchAlarmTemplateStatisticType,
+        "Tags": Dict[str, str],
+        "TargetResourceType": CloudWatchAlarmTemplateTargetResourceTypeType,
+        "Threshold": float,
+        "TreatMissingData": CloudWatchAlarmTemplateTreatMissingDataType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateEventBridgeRuleTemplateGroupResponseTypeDef = TypedDict(
+    "UpdateEventBridgeRuleTemplateGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "Id": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 TeletextSourceSettingsTypeDef = TypedDict(
     "TeletextSourceSettingsTypeDef",
     {
         "OutputRectangle": NotRequired[CaptionRectangleTypeDef],
         "PageNumber": NotRequired[str],
     },
 )
+ListCloudWatchAlarmTemplateGroupsResponseTypeDef = TypedDict(
+    "ListCloudWatchAlarmTemplateGroupsResponseTypeDef",
+    {
+        "CloudWatchAlarmTemplateGroups": List[CloudWatchAlarmTemplateGroupSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListCloudWatchAlarmTemplatesResponseTypeDef = TypedDict(
+    "ListCloudWatchAlarmTemplatesResponseTypeDef",
+    {
+        "CloudWatchAlarmTemplates": List[CloudWatchAlarmTemplateSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ColorCorrectionSettingsTypeDef = TypedDict(
     "ColorCorrectionSettingsTypeDef",
     {
         "GlobalColorCorrections": Sequence[ColorCorrectionTypeDef],
     },
 )
+CreateEventBridgeRuleTemplateRequestRequestTypeDef = TypedDict(
+    "CreateEventBridgeRuleTemplateRequestRequestTypeDef",
+    {
+        "EventType": EventBridgeRuleTemplateEventTypeType,
+        "GroupIdentifier": str,
+        "Name": str,
+        "Description": NotRequired[str],
+        "EventTargets": NotRequired[Sequence[EventBridgeRuleTemplateTargetTypeDef]],
+        "Tags": NotRequired[Mapping[str, str]],
+    },
+)
+CreateEventBridgeRuleTemplateResponseTypeDef = TypedDict(
+    "CreateEventBridgeRuleTemplateResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "EventTargets": List[EventBridgeRuleTemplateTargetTypeDef],
+        "EventType": EventBridgeRuleTemplateEventTypeType,
+        "GroupId": str,
+        "Id": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetEventBridgeRuleTemplateResponseTypeDef = TypedDict(
+    "GetEventBridgeRuleTemplateResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "EventTargets": List[EventBridgeRuleTemplateTargetTypeDef],
+        "EventType": EventBridgeRuleTemplateEventTypeType,
+        "GroupId": str,
+        "Id": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateEventBridgeRuleTemplateRequestRequestTypeDef = TypedDict(
+    "UpdateEventBridgeRuleTemplateRequestRequestTypeDef",
+    {
+        "Identifier": str,
+        "Description": NotRequired[str],
+        "EventTargets": NotRequired[Sequence[EventBridgeRuleTemplateTargetTypeDef]],
+        "EventType": NotRequired[EventBridgeRuleTemplateEventTypeType],
+        "GroupIdentifier": NotRequired[str],
+        "Name": NotRequired[str],
+    },
+)
+UpdateEventBridgeRuleTemplateResponseTypeDef = TypedDict(
+    "UpdateEventBridgeRuleTemplateResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "EventTargets": List[EventBridgeRuleTemplateTargetTypeDef],
+        "EventType": EventBridgeRuleTemplateEventTypeType,
+        "GroupId": str,
+        "Id": str,
+        "ModifiedAt": datetime,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreateInputRequestRequestTypeDef = TypedDict(
     "CreateInputRequestRequestTypeDef",
     {
         "Destinations": NotRequired[Sequence[InputDestinationRequestTypeDef]],
         "InputDevices": NotRequired[Sequence[InputDeviceSettingsTypeDef]],
         "InputSecurityGroups": NotRequired[Sequence[str]],
         "MediaConnectFlows": NotRequired[Sequence[MediaConnectFlowRequestTypeDef]],
@@ -2643,14 +3263,42 @@
 DescribeMultiplexRequestMultiplexStoppedWaitTypeDef = TypedDict(
     "DescribeMultiplexRequestMultiplexStoppedWaitTypeDef",
     {
         "MultiplexId": str,
         "WaiterConfig": NotRequired[WaiterConfigTypeDef],
     },
 )
+GetSignalMapRequestSignalMapCreatedWaitTypeDef = TypedDict(
+    "GetSignalMapRequestSignalMapCreatedWaitTypeDef",
+    {
+        "Identifier": str,
+        "WaiterConfig": NotRequired[WaiterConfigTypeDef],
+    },
+)
+GetSignalMapRequestSignalMapMonitorDeletedWaitTypeDef = TypedDict(
+    "GetSignalMapRequestSignalMapMonitorDeletedWaitTypeDef",
+    {
+        "Identifier": str,
+        "WaiterConfig": NotRequired[WaiterConfigTypeDef],
+    },
+)
+GetSignalMapRequestSignalMapMonitorDeployedWaitTypeDef = TypedDict(
+    "GetSignalMapRequestSignalMapMonitorDeployedWaitTypeDef",
+    {
+        "Identifier": str,
+        "WaiterConfig": NotRequired[WaiterConfigTypeDef],
+    },
+)
+GetSignalMapRequestSignalMapUpdatedWaitTypeDef = TypedDict(
+    "GetSignalMapRequestSignalMapUpdatedWaitTypeDef",
+    {
+        "Identifier": str,
+        "WaiterConfig": NotRequired[WaiterConfigTypeDef],
+    },
+)
 DescribeInputSecurityGroupResponseTypeDef = TypedDict(
     "DescribeInputSecurityGroupResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Inputs": List[str],
         "State": InputSecurityGroupStateType,
@@ -2679,14 +3327,50 @@
 )
 ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
     "ListChannelsRequestListChannelsPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListCloudWatchAlarmTemplateGroupsRequestListCloudWatchAlarmTemplateGroupsPaginateTypeDef = (
+    TypedDict(
+        "ListCloudWatchAlarmTemplateGroupsRequestListCloudWatchAlarmTemplateGroupsPaginateTypeDef",
+        {
+            "Scope": NotRequired[str],
+            "SignalMapIdentifier": NotRequired[str],
+            "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+        },
+    )
+)
+ListCloudWatchAlarmTemplatesRequestListCloudWatchAlarmTemplatesPaginateTypeDef = TypedDict(
+    "ListCloudWatchAlarmTemplatesRequestListCloudWatchAlarmTemplatesPaginateTypeDef",
+    {
+        "GroupIdentifier": NotRequired[str],
+        "Scope": NotRequired[str],
+        "SignalMapIdentifier": NotRequired[str],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
+ListEventBridgeRuleTemplateGroupsRequestListEventBridgeRuleTemplateGroupsPaginateTypeDef = (
+    TypedDict(
+        "ListEventBridgeRuleTemplateGroupsRequestListEventBridgeRuleTemplateGroupsPaginateTypeDef",
+        {
+            "SignalMapIdentifier": NotRequired[str],
+            "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+        },
+    )
+)
+ListEventBridgeRuleTemplatesRequestListEventBridgeRuleTemplatesPaginateTypeDef = TypedDict(
+    "ListEventBridgeRuleTemplatesRequestListEventBridgeRuleTemplatesPaginateTypeDef",
+    {
+        "GroupIdentifier": NotRequired[str],
+        "SignalMapIdentifier": NotRequired[str],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
     "ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
     {
         "TransferType": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
@@ -2747,14 +3431,22 @@
         "Resolution": NotRequired[str],
         "ResourceType": NotRequired[str],
         "SpecialFeature": NotRequired[str],
         "VideoQuality": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListSignalMapsRequestListSignalMapsPaginateTypeDef = TypedDict(
+    "ListSignalMapsRequestListSignalMapsPaginateTypeDef",
+    {
+        "CloudWatchAlarmTemplateGroupIdentifier": NotRequired[str],
+        "EventBridgeRuleTemplateGroupIdentifier": NotRequired[str],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 M2tsSettingsTypeDef = TypedDict(
     "M2tsSettingsTypeDef",
     {
         "AbsentInputAudioBehavior": NotRequired[M2tsAbsentInputAudioBehaviorType],
         "Arib": NotRequired[M2tsAribType],
         "AribCaptionsPid": NotRequired[str],
         "AribCaptionsPidControl": NotRequired[M2tsAribCaptionsPidControlType],
@@ -2807,14 +3499,30 @@
 OutputLockingSettingsTypeDef = TypedDict(
     "OutputLockingSettingsTypeDef",
     {
         "EpochLockingSettings": NotRequired[EpochLockingSettingsTypeDef],
         "PipelineLockingSettings": NotRequired[Mapping[str, Any]],
     },
 )
+ListEventBridgeRuleTemplateGroupsResponseTypeDef = TypedDict(
+    "ListEventBridgeRuleTemplateGroupsResponseTypeDef",
+    {
+        "EventBridgeRuleTemplateGroups": List[EventBridgeRuleTemplateGroupSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListEventBridgeRuleTemplatesResponseTypeDef = TypedDict(
+    "ListEventBridgeRuleTemplatesResponseTypeDef",
+    {
+        "EventBridgeRuleTemplates": List[EventBridgeRuleTemplateSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 FailoverConditionSettingsTypeDef = TypedDict(
     "FailoverConditionSettingsTypeDef",
     {
         "AudioSilenceSettings": NotRequired[AudioSilenceFailoverSettingsTypeDef],
         "InputLossSettings": NotRequired[InputLossFailoverSettingsTypeDef],
         "VideoBlackSettings": NotRequired[VideoBlackFailoverSettingsTypeDef],
     },
@@ -2980,21 +3688,37 @@
     "ListMultiplexProgramsResponseTypeDef",
     {
         "MultiplexPrograms": List[MultiplexProgramSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListSignalMapsResponseTypeDef = TypedDict(
+    "ListSignalMapsResponseTypeDef",
+    {
+        "NextToken": str,
+        "SignalMaps": List[SignalMapSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 StandardHlsSettingsTypeDef = TypedDict(
     "StandardHlsSettingsTypeDef",
     {
         "M3u8Settings": M3u8SettingsTypeDef,
         "AudioRenditionSets": NotRequired[str],
     },
 )
+MediaResourceTypeDef = TypedDict(
+    "MediaResourceTypeDef",
+    {
+        "Destinations": NotRequired[List[MediaResourceNeighborTypeDef]],
+        "Name": NotRequired[str],
+        "Sources": NotRequired[List[MediaResourceNeighborTypeDef]],
+    },
+)
 MotionGraphicsConfigurationTypeDef = TypedDict(
     "MotionGraphicsConfigurationTypeDef",
     {
         "MotionGraphicsSettings": MotionGraphicsSettingsTypeDef,
         "MotionGraphicsInsertion": NotRequired[MotionGraphicsInsertionType],
     },
 )
@@ -3536,14 +4260,134 @@
     {
         "AudioOnlyHlsSettings": NotRequired[AudioOnlyHlsSettingsTypeDef],
         "Fmp4HlsSettings": NotRequired[Fmp4HlsSettingsTypeDef],
         "FrameCaptureHlsSettings": NotRequired[Mapping[str, Any]],
         "StandardHlsSettings": NotRequired[StandardHlsSettingsTypeDef],
     },
 )
+CreateSignalMapResponseTypeDef = TypedDict(
+    "CreateSignalMapResponseTypeDef",
+    {
+        "Arn": str,
+        "CloudWatchAlarmTemplateGroupIds": List[str],
+        "CreatedAt": datetime,
+        "Description": str,
+        "DiscoveryEntryPointArn": str,
+        "ErrorMessage": str,
+        "EventBridgeRuleTemplateGroupIds": List[str],
+        "FailedMediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "Id": str,
+        "LastDiscoveredAt": datetime,
+        "LastSuccessfulMonitorDeployment": SuccessfulMonitorDeploymentTypeDef,
+        "MediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "ModifiedAt": datetime,
+        "MonitorChangesPendingDeployment": bool,
+        "MonitorDeployment": MonitorDeploymentTypeDef,
+        "Name": str,
+        "Status": SignalMapStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetSignalMapResponseTypeDef = TypedDict(
+    "GetSignalMapResponseTypeDef",
+    {
+        "Arn": str,
+        "CloudWatchAlarmTemplateGroupIds": List[str],
+        "CreatedAt": datetime,
+        "Description": str,
+        "DiscoveryEntryPointArn": str,
+        "ErrorMessage": str,
+        "EventBridgeRuleTemplateGroupIds": List[str],
+        "FailedMediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "Id": str,
+        "LastDiscoveredAt": datetime,
+        "LastSuccessfulMonitorDeployment": SuccessfulMonitorDeploymentTypeDef,
+        "MediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "ModifiedAt": datetime,
+        "MonitorChangesPendingDeployment": bool,
+        "MonitorDeployment": MonitorDeploymentTypeDef,
+        "Name": str,
+        "Status": SignalMapStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+StartDeleteMonitorDeploymentResponseTypeDef = TypedDict(
+    "StartDeleteMonitorDeploymentResponseTypeDef",
+    {
+        "Arn": str,
+        "CloudWatchAlarmTemplateGroupIds": List[str],
+        "CreatedAt": datetime,
+        "Description": str,
+        "DiscoveryEntryPointArn": str,
+        "ErrorMessage": str,
+        "EventBridgeRuleTemplateGroupIds": List[str],
+        "FailedMediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "Id": str,
+        "LastDiscoveredAt": datetime,
+        "LastSuccessfulMonitorDeployment": SuccessfulMonitorDeploymentTypeDef,
+        "MediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "ModifiedAt": datetime,
+        "MonitorChangesPendingDeployment": bool,
+        "MonitorDeployment": MonitorDeploymentTypeDef,
+        "Name": str,
+        "Status": SignalMapStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+StartMonitorDeploymentResponseTypeDef = TypedDict(
+    "StartMonitorDeploymentResponseTypeDef",
+    {
+        "Arn": str,
+        "CloudWatchAlarmTemplateGroupIds": List[str],
+        "CreatedAt": datetime,
+        "Description": str,
+        "DiscoveryEntryPointArn": str,
+        "ErrorMessage": str,
+        "EventBridgeRuleTemplateGroupIds": List[str],
+        "FailedMediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "Id": str,
+        "LastDiscoveredAt": datetime,
+        "LastSuccessfulMonitorDeployment": SuccessfulMonitorDeploymentTypeDef,
+        "MediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "ModifiedAt": datetime,
+        "MonitorChangesPendingDeployment": bool,
+        "MonitorDeployment": MonitorDeploymentTypeDef,
+        "Name": str,
+        "Status": SignalMapStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+StartUpdateSignalMapResponseTypeDef = TypedDict(
+    "StartUpdateSignalMapResponseTypeDef",
+    {
+        "Arn": str,
+        "CloudWatchAlarmTemplateGroupIds": List[str],
+        "CreatedAt": datetime,
+        "Description": str,
+        "DiscoveryEntryPointArn": str,
+        "ErrorMessage": str,
+        "EventBridgeRuleTemplateGroupIds": List[str],
+        "FailedMediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "Id": str,
+        "LastDiscoveredAt": datetime,
+        "LastSuccessfulMonitorDeployment": SuccessfulMonitorDeploymentTypeDef,
+        "MediaResourceMap": Dict[str, MediaResourceTypeDef],
+        "ModifiedAt": datetime,
+        "MonitorChangesPendingDeployment": bool,
+        "MonitorDeployment": MonitorDeploymentTypeDef,
+        "Name": str,
+        "Status": SignalMapStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DeleteMultiplexResponseTypeDef = TypedDict(
     "DeleteMultiplexResponseTypeDef",
     {
         "Arn": str,
         "AvailabilityZones": List[str],
         "Destinations": List[MultiplexOutputDestinationTypeDef],
         "Id": str,
```

### Comparing `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/waiter.py` & `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/waiter.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,18 @@
         InputAttachedWaiter,
         InputDeletedWaiter,
         InputDetachedWaiter,
         MultiplexCreatedWaiter,
         MultiplexDeletedWaiter,
         MultiplexRunningWaiter,
         MultiplexStoppedWaiter,
+        SignalMapCreatedWaiter,
+        SignalMapMonitorDeletedWaiter,
+        SignalMapMonitorDeployedWaiter,
+        SignalMapUpdatedWaiter,
     )
 
     session = Session()
     client: MediaLiveClient = session.client("medialive")
 
     channel_created_waiter: ChannelCreatedWaiter = client.get_waiter("channel_created")
     channel_deleted_waiter: ChannelDeletedWaiter = client.get_waiter("channel_deleted")
@@ -33,14 +37,18 @@
     input_attached_waiter: InputAttachedWaiter = client.get_waiter("input_attached")
     input_deleted_waiter: InputDeletedWaiter = client.get_waiter("input_deleted")
     input_detached_waiter: InputDetachedWaiter = client.get_waiter("input_detached")
     multiplex_created_waiter: MultiplexCreatedWaiter = client.get_waiter("multiplex_created")
     multiplex_deleted_waiter: MultiplexDeletedWaiter = client.get_waiter("multiplex_deleted")
     multiplex_running_waiter: MultiplexRunningWaiter = client.get_waiter("multiplex_running")
     multiplex_stopped_waiter: MultiplexStoppedWaiter = client.get_waiter("multiplex_stopped")
+    signal_map_created_waiter: SignalMapCreatedWaiter = client.get_waiter("signal_map_created")
+    signal_map_monitor_deleted_waiter: SignalMapMonitorDeletedWaiter = client.get_waiter("signal_map_monitor_deleted")
+    signal_map_monitor_deployed_waiter: SignalMapMonitorDeployedWaiter = client.get_waiter("signal_map_monitor_deployed")
+    signal_map_updated_waiter: SignalMapUpdatedWaiter = client.get_waiter("signal_map_updated")
     ```
 """
 
 from botocore.waiter import Waiter
 
 from .type_defs import WaiterConfigTypeDef
 
@@ -52,151 +60,192 @@
     "InputAttachedWaiter",
     "InputDeletedWaiter",
     "InputDetachedWaiter",
     "MultiplexCreatedWaiter",
     "MultiplexDeletedWaiter",
     "MultiplexRunningWaiter",
     "MultiplexStoppedWaiter",
+    "SignalMapCreatedWaiter",
+    "SignalMapMonitorDeletedWaiter",
+    "SignalMapMonitorDeployedWaiter",
+    "SignalMapUpdatedWaiter",
 )
 
-
 class ChannelCreatedWaiter(Waiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.ChannelCreated)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#channelcreatedwaiter)
     """
 
     def wait(self, *, ChannelId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.ChannelCreated.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#channelcreatedwaiter)
         """
 
-
 class ChannelDeletedWaiter(Waiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.ChannelDeleted)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#channeldeletedwaiter)
     """
 
     def wait(self, *, ChannelId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.ChannelDeleted.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#channeldeletedwaiter)
         """
 
-
 class ChannelRunningWaiter(Waiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.ChannelRunning)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#channelrunningwaiter)
     """
 
     def wait(self, *, ChannelId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.ChannelRunning.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#channelrunningwaiter)
         """
 
-
 class ChannelStoppedWaiter(Waiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.ChannelStopped)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#channelstoppedwaiter)
     """
 
     def wait(self, *, ChannelId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.ChannelStopped.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#channelstoppedwaiter)
         """
 
-
 class InputAttachedWaiter(Waiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.InputAttached)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#inputattachedwaiter)
     """
 
     def wait(self, *, InputId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.InputAttached.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#inputattachedwaiter)
         """
 
-
 class InputDeletedWaiter(Waiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.InputDeleted)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#inputdeletedwaiter)
     """
 
     def wait(self, *, InputId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.InputDeleted.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#inputdeletedwaiter)
         """
 
-
 class InputDetachedWaiter(Waiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.InputDetached)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#inputdetachedwaiter)
     """
 
     def wait(self, *, InputId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.InputDetached.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#inputdetachedwaiter)
         """
 
-
 class MultiplexCreatedWaiter(Waiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.MultiplexCreated)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#multiplexcreatedwaiter)
     """
 
     def wait(self, *, MultiplexId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.MultiplexCreated.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#multiplexcreatedwaiter)
         """
 
-
 class MultiplexDeletedWaiter(Waiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.MultiplexDeleted)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#multiplexdeletedwaiter)
     """
 
     def wait(self, *, MultiplexId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.MultiplexDeleted.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#multiplexdeletedwaiter)
         """
 
-
 class MultiplexRunningWaiter(Waiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.MultiplexRunning)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#multiplexrunningwaiter)
     """
 
     def wait(self, *, MultiplexId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.MultiplexRunning.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#multiplexrunningwaiter)
         """
 
-
 class MultiplexStoppedWaiter(Waiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.MultiplexStopped)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#multiplexstoppedwaiter)
     """
 
     def wait(self, *, MultiplexId: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.MultiplexStopped.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#multiplexstoppedwaiter)
         """
+
+class SignalMapCreatedWaiter(Waiter):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.SignalMapCreated)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#signalmapcreatedwaiter)
+    """
+
+    def wait(self, *, Identifier: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.SignalMapCreated.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#signalmapcreatedwaiter)
+        """
+
+class SignalMapMonitorDeletedWaiter(Waiter):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.SignalMapMonitorDeleted)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#signalmapmonitordeletedwaiter)
+    """
+
+    def wait(self, *, Identifier: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.SignalMapMonitorDeleted.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#signalmapmonitordeletedwaiter)
+        """
+
+class SignalMapMonitorDeployedWaiter(Waiter):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.SignalMapMonitorDeployed)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#signalmapmonitordeployedwaiter)
+    """
+
+    def wait(self, *, Identifier: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.SignalMapMonitorDeployed.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#signalmapmonitordeployedwaiter)
+        """
+
+class SignalMapUpdatedWaiter(Waiter):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.SignalMapUpdated)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#signalmapupdatedwaiter)
+    """
+
+    def wait(self, *, Identifier: str, WaiterConfig: WaiterConfigTypeDef = ...) -> None:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Waiter.SignalMapUpdated.wait)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/waiters/#signalmapupdatedwaiter)
+        """
```

### Comparing `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive.egg-info/PKG-INFO` & `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medialive
-Version: 1.34.77
-Summary: Type annotations for boto3.MediaLive 1.34.77 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.83
+Summary: Type annotations for boto3.MediaLive 1.34.83 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -283,44 +283,62 @@
 ```python
 from boto3.session import Session
 
 from mypy_boto3_medialive import MediaLiveClient
 from mypy_boto3_medialive.paginator import (
     DescribeSchedulePaginator,
     ListChannelsPaginator,
+    ListCloudWatchAlarmTemplateGroupsPaginator,
+    ListCloudWatchAlarmTemplatesPaginator,
+    ListEventBridgeRuleTemplateGroupsPaginator,
+    ListEventBridgeRuleTemplatesPaginator,
     ListInputDeviceTransfersPaginator,
     ListInputDevicesPaginator,
     ListInputSecurityGroupsPaginator,
     ListInputsPaginator,
     ListMultiplexProgramsPaginator,
     ListMultiplexesPaginator,
     ListOfferingsPaginator,
     ListReservationsPaginator,
+    ListSignalMapsPaginator,
 )
 
 client: MediaLiveClient = Session().client("medialive")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_schedule_paginator: DescribeSchedulePaginator = client.get_paginator("describe_schedule")
 list_channels_paginator: ListChannelsPaginator = client.get_paginator("list_channels")
+list_cloud_watch_alarm_template_groups_paginator: ListCloudWatchAlarmTemplateGroupsPaginator = (
+    client.get_paginator("list_cloud_watch_alarm_template_groups")
+)
+list_cloud_watch_alarm_templates_paginator: ListCloudWatchAlarmTemplatesPaginator = (
+    client.get_paginator("list_cloud_watch_alarm_templates")
+)
+list_event_bridge_rule_template_groups_paginator: ListEventBridgeRuleTemplateGroupsPaginator = (
+    client.get_paginator("list_event_bridge_rule_template_groups")
+)
+list_event_bridge_rule_templates_paginator: ListEventBridgeRuleTemplatesPaginator = (
+    client.get_paginator("list_event_bridge_rule_templates")
+)
 list_input_device_transfers_paginator: ListInputDeviceTransfersPaginator = client.get_paginator(
     "list_input_device_transfers"
 )
 list_input_devices_paginator: ListInputDevicesPaginator = client.get_paginator("list_input_devices")
 list_input_security_groups_paginator: ListInputSecurityGroupsPaginator = client.get_paginator(
     "list_input_security_groups"
 )
 list_inputs_paginator: ListInputsPaginator = client.get_paginator("list_inputs")
 list_multiplex_programs_paginator: ListMultiplexProgramsPaginator = client.get_paginator(
     "list_multiplex_programs"
 )
 list_multiplexes_paginator: ListMultiplexesPaginator = client.get_paginator("list_multiplexes")
 list_offerings_paginator: ListOfferingsPaginator = client.get_paginator("list_offerings")
 list_reservations_paginator: ListReservationsPaginator = client.get_paginator("list_reservations")
+list_signal_maps_paginator: ListSignalMapsPaginator = client.get_paginator("list_signal_maps")
 ```
 
 <a id="waiters-annotations"></a>
 
 ### Waiters annotations
 
 `mypy_boto3_medialive.waiter` module contains type annotations for all waiters.
@@ -337,14 +355,18 @@
     InputAttachedWaiter,
     InputDeletedWaiter,
     InputDetachedWaiter,
     MultiplexCreatedWaiter,
     MultiplexDeletedWaiter,
     MultiplexRunningWaiter,
     MultiplexStoppedWaiter,
+    SignalMapCreatedWaiter,
+    SignalMapMonitorDeletedWaiter,
+    SignalMapMonitorDeployedWaiter,
+    SignalMapUpdatedWaiter,
 )
 
 client: MediaLiveClient = Session().client("medialive")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 channel_created_waiter: ChannelCreatedWaiter = client.get_waiter("channel_created")
@@ -354,14 +376,22 @@
 input_attached_waiter: InputAttachedWaiter = client.get_waiter("input_attached")
 input_deleted_waiter: InputDeletedWaiter = client.get_waiter("input_deleted")
 input_detached_waiter: InputDetachedWaiter = client.get_waiter("input_detached")
 multiplex_created_waiter: MultiplexCreatedWaiter = client.get_waiter("multiplex_created")
 multiplex_deleted_waiter: MultiplexDeletedWaiter = client.get_waiter("multiplex_deleted")
 multiplex_running_waiter: MultiplexRunningWaiter = client.get_waiter("multiplex_running")
 multiplex_stopped_waiter: MultiplexStoppedWaiter = client.get_waiter("multiplex_stopped")
+signal_map_created_waiter: SignalMapCreatedWaiter = client.get_waiter("signal_map_created")
+signal_map_monitor_deleted_waiter: SignalMapMonitorDeletedWaiter = client.get_waiter(
+    "signal_map_monitor_deleted"
+)
+signal_map_monitor_deployed_waiter: SignalMapMonitorDeployedWaiter = client.get_waiter(
+    "signal_map_monitor_deployed"
+)
+signal_map_updated_waiter: SignalMapUpdatedWaiter = client.get_waiter("signal_map_updated")
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_medialive.literals` module contains literals extracted from shapes
```

### Comparing `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive.egg-info/SOURCES.txt` & `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.34.77/setup.py` & `mypy-boto3-medialive-1.34.83/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-medialive",
-    version="1.34.77",
+    version="1.34.83",
     packages=["mypy_boto3_medialive"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.MediaLive 1.34.77 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.MediaLive 1.34.83 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

