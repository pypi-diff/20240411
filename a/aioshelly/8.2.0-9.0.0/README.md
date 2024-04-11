# Comparing `tmp/aioshelly-8.2.0.tar.gz` & `tmp/aioshelly-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioshelly-8.2.0.tar", last modified: Thu Mar 14 22:37:30 2024, max compression
+gzip compressed data, was "aioshelly-9.0.0.tar", last modified: Thu Apr 11 13:52:37 2024, max compression
```

## Comparing `aioshelly-8.2.0.tar` & `aioshelly-9.0.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:37:30.402824 aioshelly-8.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-03-14 22:37:22.000000 aioshelly-8.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-14 22:37:22.000000 aioshelly-8.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-03-14 22:37:30.402824 aioshelly-8.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-03-14 22:37:22.000000 aioshelly-8.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:37:30.398824 aioshelly-8.2.0/aioshelly/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-14 22:37:22.000000 aioshelly-8.2.0/aioshelly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:37:30.398824 aioshelly-8.2.0/aioshelly/ble/
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-03-14 22:37:22.000000 aioshelly-8.2.0/aioshelly/ble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:37:30.402824 aioshelly-8.2.0/aioshelly/ble/backend/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-14 22:37:22.000000 aioshelly-8.2.0/aioshelly/ble/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-14 22:37:22.000000 aioshelly-8.2.0/aioshelly/ble/backend/scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-03-14 22:37:22.000000 aioshelly-8.2.0/aioshelly/ble/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-14 22:37:22.000000 aioshelly-8.2.0/aioshelly/ble/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:37:30.402824 aioshelly-8.2.0/aioshelly/block_device/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-14 22:37:22.000000 aioshelly-8.2.0/aioshelly/block_device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8896 2024-03-14 22:37:22.000000 aioshelly-8.2.0/aioshelly/block_device/coap.py
--rw-r--r--   0 runner    (1001) docker     (127)    18512 2024-03-14 22:37:22.000000 aioshelly-8.2.0/aioshelly/block_device/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-03-14 22:37:22.000000 aioshelly-8.2.0/aioshelly/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-03-14 22:37:22.000000 aioshelly-8.2.0/aioshelly/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-14 22:37:22.000000 aioshelly-8.2.0/aioshelly/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-14 22:37:22.000000 aioshelly-8.2.0/aioshelly/json.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 22:37:22.000000 aioshelly-8.2.0/aioshelly/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:37:30.402824 aioshelly-8.2.0/aioshelly/rpc_device/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-14 22:37:22.000000 aioshelly-8.2.0/aioshelly/rpc_device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14386 2024-03-14 22:37:22.000000 aioshelly-8.2.0/aioshelly/rpc_device/device.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-14 22:37:22.000000 aioshelly-8.2.0/aioshelly/rpc_device/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    18608 2024-03-14 22:37:22.000000 aioshelly-8.2.0/aioshelly/rpc_device/wsrpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:37:30.402824 aioshelly-8.2.0/aioshelly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-03-14 22:37:30.000000 aioshelly-8.2.0/aioshelly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-14 22:37:30.000000 aioshelly-8.2.0/aioshelly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 22:37:30.000000 aioshelly-8.2.0/aioshelly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-14 22:37:30.000000 aioshelly-8.2.0/aioshelly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-14 22:37:30.000000 aioshelly-8.2.0/aioshelly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 22:37:30.000000 aioshelly-8.2.0/aioshelly.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-14 22:37:22.000000 aioshelly-8.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 22:37:30.402824 aioshelly-8.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-14 22:37:22.000000 aioshelly-8.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:37:30.402824 aioshelly-8.2.0/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-14 22:37:22.000000 aioshelly-8.2.0/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:37:30.402824 aioshelly-8.2.0/tools/common/
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-03-14 22:37:22.000000 aioshelly-8.2.0/tools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-03-14 22:37:22.000000 aioshelly-8.2.0/tools/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    11798 2024-03-14 22:37:22.000000 aioshelly-8.2.0/tools/fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-03-14 22:37:22.000000 aioshelly-8.2.0/tools/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:52:37.099065 aioshelly-9.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-04-11 13:52:25.000000 aioshelly-9.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-11 13:52:25.000000 aioshelly-9.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-11 13:52:37.099065 aioshelly-9.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-11 13:52:25.000000 aioshelly-9.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:52:37.095065 aioshelly-9.0.0/aioshelly/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 13:52:25.000000 aioshelly-9.0.0/aioshelly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:52:37.095065 aioshelly-9.0.0/aioshelly/ble/
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-11 13:52:25.000000 aioshelly-9.0.0/aioshelly/ble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:52:37.095065 aioshelly-9.0.0/aioshelly/ble/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 13:52:25.000000 aioshelly-9.0.0/aioshelly/ble/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-11 13:52:25.000000 aioshelly-9.0.0/aioshelly/ble/backend/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-11 13:52:25.000000 aioshelly-9.0.0/aioshelly/ble/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-11 13:52:25.000000 aioshelly-9.0.0/aioshelly/ble/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:52:37.099065 aioshelly-9.0.0/aioshelly/block_device/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-11 13:52:25.000000 aioshelly-9.0.0/aioshelly/block_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-11 13:52:25.000000 aioshelly-9.0.0/aioshelly/block_device/coap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19012 2024-04-11 13:52:25.000000 aioshelly-9.0.0/aioshelly/block_device/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-11 13:52:25.000000 aioshelly-9.0.0/aioshelly/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-11 13:52:25.000000 aioshelly-9.0.0/aioshelly/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-11 13:52:25.000000 aioshelly-9.0.0/aioshelly/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-11 13:52:25.000000 aioshelly-9.0.0/aioshelly/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:52:25.000000 aioshelly-9.0.0/aioshelly/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:52:37.099065 aioshelly-9.0.0/aioshelly/rpc_device/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-11 13:52:25.000000 aioshelly-9.0.0/aioshelly/rpc_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14125 2024-04-11 13:52:25.000000 aioshelly-9.0.0/aioshelly/rpc_device/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-11 13:52:25.000000 aioshelly-9.0.0/aioshelly/rpc_device/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18590 2024-04-11 13:52:25.000000 aioshelly-9.0.0/aioshelly/rpc_device/wsrpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:52:37.099065 aioshelly-9.0.0/aioshelly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-11 13:52:37.000000 aioshelly-9.0.0/aioshelly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-11 13:52:37.000000 aioshelly-9.0.0/aioshelly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:52:37.000000 aioshelly-9.0.0/aioshelly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-11 13:52:37.000000 aioshelly-9.0.0/aioshelly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 13:52:37.000000 aioshelly-9.0.0/aioshelly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:52:37.000000 aioshelly-9.0.0/aioshelly.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-11 13:52:25.000000 aioshelly-9.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:52:37.099065 aioshelly-9.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-11 13:52:25.000000 aioshelly-9.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:52:37.099065 aioshelly-9.0.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 13:52:25.000000 aioshelly-9.0.0/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:52:37.099065 aioshelly-9.0.0/tools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-11 13:52:25.000000 aioshelly-9.0.0/tools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-04-11 13:52:25.000000 aioshelly-9.0.0/tools/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11058 2024-04-11 13:52:25.000000 aioshelly-9.0.0/tools/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-11 13:52:25.000000 aioshelly-9.0.0/tools/verify.py
```

### Comparing `aioshelly-8.2.0/LICENSE` & `aioshelly-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioshelly-8.2.0/PKG-INFO` & `aioshelly-9.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: aioshelly
-Version: 8.2.0
+Version: 9.0.0
 Summary: Asynchronous library to control Shelly devices.
 Home-page: https://github.com/home-assistant-libs/aioshelly
 Author: Paulus Schoutsen
 Author-email: paulus@home-assistant.io
 License: Apache License 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bluetooth-data-tools>=1.19.0
 Requires-Dist: aiohttp
 Requires-Dist: habluetooth>=2.1.0
 Requires-Dist: yarl
 Requires-Dist: orjson>=3.8.1
@@ -28,15 +27,15 @@
 
 Asynchronous library to control Shelly devices
 
 **This library is under development**
 
 ## Requirements
 
-- Python >= 3.10
+- Python >= 3.11
 - bluetooth-data-tools
 - aiohttp
 - orjson
 
 ## Install
 ```bash
 pip install aioshelly
@@ -55,31 +54,24 @@
 import asyncio
 from pprint import pprint
 
 import aiohttp
 
 from aioshelly.block_device import COAP, BlockDevice
 from aioshelly.common import ConnectionOptions
-from aioshelly.exceptions import (
-    DeviceConnectionError,
-    FirmwareUnsupported,
-    InvalidAuthError,
-)
+from aioshelly.exceptions import DeviceConnectionError, InvalidAuthError
 
 
 async def test_block_device():
     """Test Gen1 Block (CoAP) based device."""
     options = ConnectionOptions("192.168.1.165", "username", "password")
 
     async with aiohttp.ClientSession() as aiohttp_session, COAP() as coap_context:
         try:
             device = await BlockDevice.create(aiohttp_session, coap_context, options)
-        except FirmwareUnsupported as err:
-            print(f"Device firmware not supported, error: {repr(err)}")
-            return
         except InvalidAuthError as err:
             print(f"Invalid or missing authorization, error: {repr(err)}")
             return
         except DeviceConnectionError as err:
             print(f"Error connecting to {options.ip_address}, error: {repr(err)}")
             return
 
@@ -98,34 +90,27 @@
 ```python
 import asyncio
 from pprint import pprint
 
 import aiohttp
 
 from aioshelly.common import ConnectionOptions
-from aioshelly.exceptions import (
-    DeviceConnectionError,
-    FirmwareUnsupported,
-    InvalidAuthError,
-)
+from aioshelly.exceptions import DeviceConnectionError, InvalidAuthError
 from aioshelly.rpc_device import RpcDevice, WsServer
 
 
 async def test_rpc_device():
     """Test Gen2/Gen3 RPC (WebSocket) based device."""
     options = ConnectionOptions("192.168.1.188", "username", "password")
     ws_context = WsServer()
     await ws_context.initialize(8123)
 
     async with aiohttp.ClientSession() as aiohttp_session:
         try:
             device = await RpcDevice.create(aiohttp_session, ws_context, options)
-        except FirmwareUnsupported as err:
-            print(f"Device firmware not supported, error: {repr(err)}")
-            return
         except InvalidAuthError as err:
             print(f"Invalid or missing authorization, error: {repr(err)}")
             return
         except DeviceConnectionError as err:
             print(f"Error connecting to {options.ip_address}, error: {repr(err)}")
             return
```

### Comparing `aioshelly-8.2.0/README.md` & `aioshelly-9.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Asynchronous library to control Shelly devices
 
 **This library is under development**
 
 ## Requirements
 
-- Python >= 3.10
+- Python >= 3.11
 - bluetooth-data-tools
 - aiohttp
 - orjson
 
 ## Install
 ```bash
 pip install aioshelly
@@ -29,31 +29,24 @@
 import asyncio
 from pprint import pprint
 
 import aiohttp
 
 from aioshelly.block_device import COAP, BlockDevice
 from aioshelly.common import ConnectionOptions
-from aioshelly.exceptions import (
-    DeviceConnectionError,
-    FirmwareUnsupported,
-    InvalidAuthError,
-)
+from aioshelly.exceptions import DeviceConnectionError, InvalidAuthError
 
 
 async def test_block_device():
     """Test Gen1 Block (CoAP) based device."""
     options = ConnectionOptions("192.168.1.165", "username", "password")
 
     async with aiohttp.ClientSession() as aiohttp_session, COAP() as coap_context:
         try:
             device = await BlockDevice.create(aiohttp_session, coap_context, options)
-        except FirmwareUnsupported as err:
-            print(f"Device firmware not supported, error: {repr(err)}")
-            return
         except InvalidAuthError as err:
             print(f"Invalid or missing authorization, error: {repr(err)}")
             return
         except DeviceConnectionError as err:
             print(f"Error connecting to {options.ip_address}, error: {repr(err)}")
             return
 
@@ -72,34 +65,27 @@
 ```python
 import asyncio
 from pprint import pprint
 
 import aiohttp
 
 from aioshelly.common import ConnectionOptions
-from aioshelly.exceptions import (
-    DeviceConnectionError,
-    FirmwareUnsupported,
-    InvalidAuthError,
-)
+from aioshelly.exceptions import DeviceConnectionError, InvalidAuthError
 from aioshelly.rpc_device import RpcDevice, WsServer
 
 
 async def test_rpc_device():
     """Test Gen2/Gen3 RPC (WebSocket) based device."""
     options = ConnectionOptions("192.168.1.188", "username", "password")
     ws_context = WsServer()
     await ws_context.initialize(8123)
 
     async with aiohttp.ClientSession() as aiohttp_session:
         try:
             device = await RpcDevice.create(aiohttp_session, ws_context, options)
-        except FirmwareUnsupported as err:
-            print(f"Device firmware not supported, error: {repr(err)}")
-            return
         except InvalidAuthError as err:
             print(f"Invalid or missing authorization, error: {repr(err)}")
             return
         except DeviceConnectionError as err:
             print(f"Error connecting to {options.ip_address}, error: {repr(err)}")
             return
```

### Comparing `aioshelly-8.2.0/aioshelly/ble/__init__.py` & `aioshelly-9.0.0/aioshelly/ble/__init__.py`

 * *Files identical despite different names*

### Comparing `aioshelly-8.2.0/aioshelly/ble/backend/scanner.py` & `aioshelly-9.0.0/aioshelly/ble/backend/scanner.py`

 * *Files identical despite different names*

### Comparing `aioshelly-8.2.0/aioshelly/ble/const.py` & `aioshelly-9.0.0/aioshelly/ble/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 DEFAULT_INTERVAL_MS = 320
 DEFAULT_WINDOW_MS = 30
 DEFAULT_DURATION_MS = -1
 
 BLE_CODE = """
 // aioshelly BLE script 2.0
+// Script automatically installed by Home Assistant for Bluetooth proxy support
+// https://www.home-assistant.io/integrations/bluetooth/#remote-adapters-bluetooth-proxies
 const queueServeTimer = 100; // in ms, timer for events emitting
 const burstSendCount =  5; // number if events, emitted on timer event
 const maxQueue =  32; // if the queue exceeds the limit, all new events are ignored until it empties
 const packetsInSingleEvent = 16; // max number of packets in single event
 
 let queue = [];
 let timerHandler = null;
```

### Comparing `aioshelly-8.2.0/aioshelly/ble/parser.py` & `aioshelly-9.0.0/aioshelly/ble/parser.py`

 * *Files identical despite different names*

### Comparing `aioshelly-8.2.0/aioshelly/block_device/coap.py` & `aioshelly-9.0.0/aioshelly/block_device/coap.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 import logging
 import socket
 import struct
 from collections.abc import Callable
 from enum import Enum, auto
 from ipaddress import IPv4Address
 from types import TracebackType
-from typing import TYPE_CHECKING, cast
-
-from typing_extensions import Self
+from typing import TYPE_CHECKING, Self, cast
 
 from ..const import DEFAULT_COAP_PORT, END_OF_OPTIONS_MARKER, PERIODIC_COAP_TYPE_CODE
 from ..json import JSONDecodeError, json_loads
 
 COAP_OPTION_DEVICE_ID = 3332
 
 _LOGGER = logging.getLogger(__name__)
```

### Comparing `aioshelly-8.2.0/aioshelly/block_device/device.py` & `aioshelly-9.0.0/aioshelly/block_device/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 import asyncio
 import logging
 from collections.abc import Callable
 from enum import Enum, auto
 from http import HTTPStatus
 from typing import Any, ClassVar, cast
 
-import aiohttp
-import async_timeout
-from aiohttp import ClientResponseError
-from aiohttp.client import ClientResponse
+from aiohttp import ClientResponse, ClientResponseError, ClientSession
 from yarl import URL
 
 from ..common import ConnectionOptions, IpOrOptionsType, get_info, process_ip_or_options
 from ..const import (
     CONNECT_ERRORS,
     DEFAULT_HTTP_PORT,
     DEVICE_IO_TIMEOUT,
+    FIRMWARE_PATTERN,
+    GEN1_LIGHT_TRANSITION_MIN_FIRMWARE_DATE,
+    GEN1_MIN_FIRMWARE_DATE,
+    GEN1_MODELS_SUPPORTING_LIGHT_TRANSITION,
+    GEN1_MODELS_UNSUPPORTED,
     HTTP_CALL_TIMEOUT,
     MODEL_RGBW2,
 )
 from ..exceptions import (
     CustomPortNotSupported,
     DeviceConnectionError,
-    FirmwareUnsupported,
     InvalidAuthError,
     MacAddressMismatchError,
     NotInitialized,
     ShellyError,
     WrongShellyGen,
 )
 from ..json import json_loads
@@ -59,73 +60,70 @@
 
 class BlockUpdateType(Enum):
     """Block Update type."""
 
     COAP_PERIODIC = auto()
     COAP_REPLY = auto()
     INITIALIZED = auto()
+    ONLINE = auto()
 
 
 class BlockDevice:
     """Shelly block device representation."""
 
     def __init__(
         self,
         coap_context: COAP,
-        aiohttp_session: aiohttp.ClientSession,
+        aiohttp_session: ClientSession,
         options: ConnectionOptions,
     ) -> None:
         """Device init."""
         self.coap_context: COAP = coap_context
-        self.aiohttp_session: aiohttp.ClientSession = aiohttp_session
+        self.aiohttp_session: ClientSession = aiohttp_session
         self.options: ConnectionOptions = options
         self.coap_d: dict[str, Any] | None = None
-        self.blocks: list | None = None
+        self.blocks: list[Block] = []
         self.coap_s: dict[str, Any] | None = None
         self._settings: dict[str, Any] | None = None
         self._shelly: dict[str, Any] | None = None
         self._status: dict[str, Any] | None = None
         sub_id = options.ip_address
         if options.device_mac:
             sub_id = options.device_mac[-6:]
         self._unsub_coap: Callable | None = coap_context.subscribe_updates(
             sub_id, self._coap_message_received
         )
         self._update_listener: Callable | None = None
-        self._coap_response_events: dict = {}
+        self._coap_response_events: dict[str, asyncio.Event] = {}
         self.initialized = False
         self._initializing = False
         self._last_error: ShellyError | None = None
-        self._init_task: asyncio.Task[None] | None = None
 
     @classmethod
     async def create(
         cls: type[BlockDevice],
-        aiohttp_session: aiohttp.ClientSession,
+        aiohttp_session: ClientSession,
         coap_context: COAP,
         ip_or_options: IpOrOptionsType,
-        initialize: bool = True,
     ) -> BlockDevice:
         """Device creation."""
         options = await process_ip_or_options(ip_or_options)
-        instance = cls(coap_context, aiohttp_session, options)
-
-        if initialize:
-            await instance.initialize()
-        else:
-            await instance._coap_request("s")  # noqa: SLF001
-
-        return instance
+        # Try sending cit/s request to trigger a sleeping device
+        try:
+            await coap_context.request(options.ip_address, "s")
+        except OSError as err:
+            _LOGGER.debug("host %s: error: %r", options.ip_address, err)
+        return cls(coap_context, aiohttp_session, options)
 
     @property
     def ip_address(self) -> str:
         """Device ip address."""
         return self.options.ip_address
 
-    async def initialize(self, async_init: bool = False) -> None:
+    async def initialize(self) -> None:
         """Device initialization."""
         if self._initializing:
             raise RuntimeError("Already initializing")
 
         # GEN1 cannot be configured behind a range extender as CoAP port cannot be
         # natted
         if self.options.port != DEFAULT_HTTP_PORT:
@@ -138,80 +136,72 @@
             self._shelly = await get_info(
                 self.aiohttp_session, self.options.ip_address, self.options.device_mac
             )
 
             if self.requires_auth and not self.options.auth:
                 raise InvalidAuthError("auth missing and required")
 
-            async with async_timeout.timeout(DEVICE_IO_TIMEOUT):
+            async with asyncio.timeout(DEVICE_IO_TIMEOUT):
                 await self.update_settings()
                 await self.update_status()
 
-                event_d: asyncio.Event = await self._coap_request("d")
-                # We need to wait for D to come in before we request S
-                # Or else we might miss the answer to D
-                await event_d.wait()
-
-                if not async_init:
-                    event_s = await self._coap_request("s")
-                    await event_s.wait()
+                # Older devices has incompatible CoAP protocol (v1)
+                # Skip CoAP to avoid parsing errors
+                if self.firmware_supported:
+                    event_d = await self._coap_request("d")
+                    # We need to wait for D to come in before we request S
+                    # Or else we might miss the answer to D
+                    await event_d.wait()
+
+                    if self.coap_s is None:
+                        event_s = await self._coap_request("s")
+                        await event_s.wait()
 
             self.initialized = True
         except ClientResponseError as err:
             if err.status == HTTPStatus.UNAUTHORIZED:
                 self._last_error = InvalidAuthError(err)
-                # Auth error during async init, used by sleeping devices
-                # Will raise 'invalidAuthError; on next property read
-                self.initialized = True
             else:
                 self._last_error = DeviceConnectionError(err)
             _LOGGER.debug("host %s: error: %r", ip, self._last_error)
-            if not async_init:
-                self.shutdown()
-                raise self._last_error from err
-        except (MacAddressMismatchError, FirmwareUnsupported) as err:
+            self.shutdown()
+            raise self._last_error from err
+        except MacAddressMismatchError as err:
             self._last_error = err
             _LOGGER.debug("host %s: error: %r", ip, err)
-            if not async_init:
-                self.shutdown()
-                raise
+            self.shutdown()
+            raise
         except CONNECT_ERRORS as err:
             self._last_error = DeviceConnectionError(err)
             _LOGGER.debug("host %s: error: %r", ip, self._last_error)
-            if not async_init:
-                self.shutdown()
-                raise DeviceConnectionError(err) from err
+            self.shutdown()
+            raise DeviceConnectionError(err) from err
         finally:
             self._initializing = False
 
         if self._update_listener:
             self._update_listener(self, BlockUpdateType.INITIALIZED)
 
     def shutdown(self) -> None:
         """Shutdown device."""
         self._update_listener = None
 
         if self._unsub_coap:
-            self._unsub_coap()
+            try:
+                self._unsub_coap()
+            except KeyError as err:
+                _LOGGER.error(
+                    "host %s: error during shutdown: %r", self.options.ip_address, err
+                )
             self._unsub_coap = None
 
-    async def _async_init(self) -> None:
-        """Async init upon CoAP message event."""
-        await self.initialize(True)
-
     def _coap_message_received(self, msg: CoapMessage) -> None:
         """COAP message received."""
-        if not self._initializing and not self.initialized:
-            loop = asyncio.get_running_loop()
-            self._init_task = loop.create_task(self._async_init())
-
-            def _clear_init_task(_: Any) -> None:
-                self._init_task = None
-
-            self._init_task.add_done_callback(_clear_init_task)
+        if not self._initializing and not self.initialized and self._update_listener:
+            self._update_listener(self, BlockUpdateType.ONLINE)
 
         if not msg.payload:
             return
         if "G" in msg.payload:
             self._update_s(msg.payload, msg.coap_type)
             path = "s"
         elif "blk" in msg.payload:
@@ -224,15 +214,15 @@
         event = self._coap_response_events.pop(path, None)
         if event is not None:
             event.set()
 
     async def update(self) -> None:
         """Device update."""
         try:
-            async with async_timeout.timeout(DEVICE_IO_TIMEOUT):
+            async with asyncio.timeout(DEVICE_IO_TIMEOUT):
                 event = await self._coap_request("s")
                 await event.wait()
         except CONNECT_ERRORS as err:
             self._last_error = DeviceConnectionError(err)
             raise DeviceConnectionError from err
 
     def _update_d(self, data: dict[str, Any]) -> None:
@@ -442,14 +432,34 @@
         return cast(str, self.settings["name"] or self.hostname)
 
     @property
     def last_error(self) -> ShellyError | None:
         """Return the last error during async device init."""
         return self._last_error
 
+    @property
+    def firmware_supported(self) -> bool:
+        """Return True if device firmware version is supported."""
+        if self.model in GEN1_MODELS_UNSUPPORTED:
+            return False
+
+        if self.model in GEN1_MODELS_SUPPORTING_LIGHT_TRANSITION:
+            fw_ver = GEN1_LIGHT_TRANSITION_MIN_FIRMWARE_DATE
+        else:
+            fw_ver = GEN1_MIN_FIRMWARE_DATE
+
+        match = FIRMWARE_PATTERN.search(self.firmware_version)
+
+        if match is None:
+            return False
+
+        # We compare firmware release dates because Shelly version numbering is
+        # inconsistent, sometimes the word is used as the version number.
+        return int(match[0]) >= fw_ver
+
 
 class Block:
     """Shelly CoAP block."""
 
     TYPES: ClassVar[dict] = {}
     type = None
```

### Comparing `aioshelly-8.2.0/aioshelly/const.py` & `aioshelly-9.0.0/aioshelly/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Constants for aioshelly."""
 
 import asyncio
+import re
 
 import aiohttp
 
 from .exceptions import DeviceConnectionError
 
 CONNECT_ERRORS = (
     aiohttp.ClientError,
@@ -63,26 +64,29 @@
 MODEL_PLUS_1_UL = "SNSW-001X15UL"
 MODEL_PLUS_10V = "SNGW-0A11WW010"  # pre-release of SNDM-00100WW
 MODEL_PLUS_10V_DIMMER = "SNDM-00100WW"
 MODEL_PLUS_1PM = "SNSW-001P16EU"
 MODEL_PLUS_1PM_MINI = "SNSW-001P8EU"
 MODEL_PLUS_1PM_UL = "SNSW-001P15UL"
 MODEL_PLUS_2PM = "SNSW-002P16EU"
+MODEL_PLUS_2PM_UL = "SNSW-002P15UL"
 MODEL_PLUS_2PM_V2 = "SNSW-102P16EU"
 MODEL_PLUS_HT = "SNSN-0013A"
-MODEL_PLUS_I4 = "SNSW-0024X"
+MODEL_PLUS_I4 = "SNSN-0024X"
 MODEL_PLUS_I4DC = "SNSN-0D24X"
 MODEL_PLUS_PLUG_IT = "SNPL-00110IT"
 MODEL_PLUS_PLUG_S = "SNPL-00112EU"
+MODEL_PLUS_PLUG_S_V2 = "SNPL-10112EU"  # hw v2
 MODEL_PLUS_PLUG_UK = "SNPL-00112UK"
 MODEL_PLUS_PLUG_US = "SNPL-00116US"
 MODEL_PLUS_PM_MINI = "SNPM-001PCEU16"
 MODEL_PLUS_RGBW_PM = "SNDC-0D4P10WW"
 MODEL_PLUS_SMOKE = "SNSN-0031Z"
 MODEL_PLUS_UNI = "SNSN-0043X"
+MODEL_PLUS_WALL_DIMMER = "SNDM-0013US"
 MODEL_PRO_1 = "SPSW-001XE16EU"
 MODEL_PRO_1_V2 = "SPSW-101XE16EU"
 MODEL_PRO_1_V3 = "SPSW-201XE16EU"
 MODEL_PRO_1PM = "SPSW-001PE16EU"
 MODEL_PRO_1PM_V2 = "SPSW-101PE16EU"
 MODEL_PRO_1PM_V3 = "SPSW-201PE16EU"
 MODEL_PRO_2 = "SPSW-002XE16EU"
@@ -95,14 +99,15 @@
 MODEL_PRO_4PM = "SPSW-004PE16EU"
 MODEL_PRO_4PM_V2 = "SPSW-104PE16EU"
 MODEL_PRO_DIMMER_1PM = "SPDM-001PE01EU"
 MODEL_PRO_DIMMER_2PM = "SPDM-002PE01EU"
 MODEL_PRO_DUAL_COVER = "SPSH-002PE16EU"
 MODEL_PRO_EM = "SPEM-002CEBEU50"
 MODEL_PRO_EM3 = "SPEM-003CEBEU"
+MODEL_PRO_EM3_120 = "SPEM-003CEBEU120"
 MODEL_PRO_EM3_400 = "SPEM-003CEBEU400"
 MODEL_WALL_DISPLAY = "SAWD-0A1XX10EU1"
 # Gen3 RPC based models
 MODEL_1_MINI_G3 = "S3SW-001X8EU"
 MODEL_1PM_MINI_G3 = "S3SW-001P8EU"
 MODEL_HT_G3 = "S3SN-0U12A"
 MODEL_PM_MINI_G3 = "S3PM-001PCEU16"
@@ -158,26 +163,29 @@
     MODEL_PLUS_1_UL: "Shelly Plus 1 UL",
     MODEL_PLUS_10V: "Shelly Plus 10V",
     MODEL_PLUS_10V_DIMMER: "Shelly Plus 0-10V Dimmer",
     MODEL_PLUS_1PM: "Shelly Plus 1PM",
     MODEL_PLUS_1PM_MINI: "Shelly Plus 1PM Mini",
     MODEL_PLUS_1PM_UL: "Shelly Plus 1PM UL",
     MODEL_PLUS_2PM: "Shelly Plus 2PM",
+    MODEL_PLUS_2PM_UL: "Shelly Plus 2PM UL",
     MODEL_PLUS_2PM_V2: "Shelly Plus 2PM",
     MODEL_PLUS_HT: "Shelly Plus H&T",
     MODEL_PLUS_I4: "Shelly Plus I4",
     MODEL_PLUS_I4DC: "Shelly Plus I4DC",
     MODEL_PLUS_PLUG_IT: "Shelly Plus Plug IT",
     MODEL_PLUS_PLUG_S: "Shelly Plus Plug S",
+    MODEL_PLUS_PLUG_S_V2: "Shelly Plus Plug S",
     MODEL_PLUS_PLUG_UK: "Shelly Plus Plug UK",
     MODEL_PLUS_PLUG_US: "Shelly Plus Plug US",
     MODEL_PLUS_PM_MINI: "Shelly Plus PM Mini",
     MODEL_PLUS_RGBW_PM: "Shelly Plus RGBW PM",
     MODEL_PLUS_SMOKE: "Shelly Plus Smoke",
     MODEL_PLUS_UNI: "Shelly Plus Uni",
+    MODEL_PLUS_WALL_DIMMER: "Shelly Plus Wall Dimmer",
     MODEL_PRO_1: "Shelly Pro 1",
     MODEL_PRO_1_V2: "Shelly Pro 1",
     MODEL_PRO_1_V3: "Shelly Pro 1",
     MODEL_PRO_1PM: "Shelly Pro 1PM",
     MODEL_PRO_1PM_V2: "Shelly Pro 1PM",
     MODEL_PRO_1PM_V3: "Shelly Pro 1PM",
     MODEL_PRO_2: "Shelly Pro 2",
@@ -189,14 +197,15 @@
     MODEL_PRO_4PM: "Shelly Pro 4PM",
     MODEL_PRO_4PM_V2: "Shelly Pro 4PM",
     MODEL_PRO_DIMMER_1PM: "Shelly Pro Dimmer 1PM",
     MODEL_PRO_DIMMER_2PM: "Shelly Pro Dimmer 2PM",
     MODEL_PRO_DUAL_COVER: "Shelly Pro Dual Cover PM",
     MODEL_PRO_EM: "Shelly Pro EM",
     MODEL_PRO_EM3: "Shelly Pro 3EM",
+    MODEL_PRO_EM3_120: "Shelly Pro 3EM",
     MODEL_PRO_EM3_400: "Shelly Pro 3EM-400",
     MODEL_WALL_DISPLAY: "Shelly Wall Display",
     # Gen3 RPC based models
     MODEL_1_MINI_G3: "Shelly 1 Mini Gen3",
     MODEL_1PM_MINI_G3: "Shelly 1PM Mini Gen3",
     MODEL_HT_G3: "Shelly H&T Gen3",
     MODEL_PM_MINI_G3: "Shelly PM Mini Gen3",
@@ -252,7 +261,9 @@
 
 BLOCK_GENERATIONS = (GEN1,)
 RPC_GENERATIONS = (GEN2, GEN3)
 
 DEFAULT_HTTP_PORT = 80
 PERIODIC_COAP_TYPE_CODE = 30
 END_OF_OPTIONS_MARKER = 0xFF
+
+FIRMWARE_PATTERN = re.compile(r"^(\d{8})")
```

### Comparing `aioshelly-8.2.0/aioshelly/exceptions.py` & `aioshelly-9.0.0/aioshelly/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,18 +31,14 @@
 #    Errors that are expected to happen and should be handled by the caller.
 
 
 class DeviceConnectionError(ShellyError):
     """Exception indicates device connection errors."""
 
 
-class FirmwareUnsupported(ShellyError):
-    """Raised if device firmware version is unsupported."""
-
-
 class InvalidAuthError(ShellyError):
     """Raised to indicate invalid or missing authentication error."""
 
 
 class MacAddressMismatchError(ShellyError):
     """Raised if input MAC address does not match the device MAC address."""
```

### Comparing `aioshelly-8.2.0/aioshelly/rpc_device/device.py` & `aioshelly-9.0.0/aioshelly/rpc_device/device.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,28 @@
 
 import asyncio
 import logging
 from collections.abc import Callable
 from enum import Enum, auto
 from typing import Any, cast
 
-import aiohttp
-import async_timeout
-from aiohttp.client import ClientSession
+from aiohttp import ClientSession
 
 from ..common import ConnectionOptions, IpOrOptionsType, get_info, process_ip_or_options
-from ..const import CONNECT_ERRORS, DEVICE_IO_TIMEOUT, NOTIFY_WS_CLOSED
+from ..const import (
+    CONNECT_ERRORS,
+    DEVICE_IO_TIMEOUT,
+    FIRMWARE_PATTERN,
+    GEN2,
+    GEN2_MIN_FIRMWARE_DATE,
+    GEN3_MIN_FIRMWARE_DATE,
+    NOTIFY_WS_CLOSED,
+)
 from ..exceptions import (
     DeviceConnectionError,
-    FirmwareUnsupported,
     InvalidAuthError,
     MacAddressMismatchError,
     NotInitialized,
     RpcCallError,
     ShellyError,
     WrongShellyGen,
 )
@@ -51,23 +56,24 @@
     """RPC Update type."""
 
     EVENT = auto()
     STATUS = auto()
     INITIALIZED = auto()
     DISCONNECTED = auto()
     UNKNOWN = auto()
+    ONLINE = auto()
 
 
 class RpcDevice:
     """Shelly RPC device representation."""
 
     def __init__(
         self,
         ws_context: WsServer,
-        aiohttp_session: aiohttp.ClientSession,
+        aiohttp_session: ClientSession,
         options: ConnectionOptions,
     ) -> None:
         """Device init."""
         self.aiohttp_session: ClientSession = aiohttp_session
         self.options: ConnectionOptions = options
         self._shelly: dict[str, Any] | None = None
         self._status: dict[str, Any] | None = None
@@ -82,37 +88,25 @@
         self._unsub_ws: Callable | None = ws_context.subscribe_updates(
             sub_id, self._wsrpc.handle_frame
         )
         self._update_listener: Callable | None = None
         self.initialized: bool = False
         self._initializing: bool = False
         self._last_error: ShellyError | None = None
-        self._init_task: asyncio.Task[None] | None = None
 
     @classmethod
     async def create(
         cls: type[RpcDevice],
-        aiohttp_session: aiohttp.ClientSession,
+        aiohttp_session: ClientSession,
         ws_context: WsServer,
         ip_or_options: IpOrOptionsType,
-        initialize: bool = True,
     ) -> RpcDevice:
         """Device creation."""
         options = await process_ip_or_options(ip_or_options)
-        instance = cls(ws_context, aiohttp_session, options)
-
-        if initialize:
-            await instance.initialize()
-
-        return instance
-
-    async def _async_init(self) -> None:
-        """Async init upon WsRPC message event."""
-        await self.initialize(True)
-        await self._wsrpc.disconnect()
+        return cls(ws_context, aiohttp_session, options)
 
     def _on_notification(
         self, method: str, params: dict[str, Any] | None = None
     ) -> None:
         """Received status notification from device."""
         update_type = RpcUpdateType.UNKNOWN
         if params is not None:
@@ -124,38 +118,34 @@
                 update_type = RpcUpdateType.STATUS
             elif method == "NotifyEvent":
                 self._event = params
                 update_type = RpcUpdateType.EVENT
         elif method == NOTIFY_WS_CLOSED:
             update_type = RpcUpdateType.DISCONNECTED
 
-        if not self._initializing and not self.initialized:
-            loop = asyncio.get_running_loop()
-            self._init_task = loop.create_task(self._async_init())
-
-            def _clear_init_task(_: Any) -> None:
-                self._init_task = None
+        if not self._update_listener or self._initializing:
+            return
 
-            self._init_task.add_done_callback(_clear_init_task)
+        if not self.initialized:
+            self._update_listener(self, RpcUpdateType.ONLINE)
             return
 
-        if self._update_listener and self.initialized:
-            self._update_listener(self, update_type)
+        self._update_listener(self, update_type)
 
     @property
     def ip_address(self) -> str:
         """Device ip address."""
         return self.options.ip_address
 
     @property
     def port(self) -> int:
         """Device port."""
         return self.options.port
 
-    async def initialize(self, async_init: bool = False) -> None:
+    async def initialize(self) -> None:
         """Device initialization."""
         if self._initializing:
             raise RuntimeError("Already initializing")
 
         self._initializing = True
         self.initialized = False
         ip = self.options.ip_address
@@ -174,63 +164,61 @@
 
                 self._wsrpc.set_auth_data(
                     self.shelly["auth_domain"],
                     self.options.username,
                     self.options.password,
                 )
 
-            async with async_timeout.timeout(DEVICE_IO_TIMEOUT):
+            async with asyncio.timeout(DEVICE_IO_TIMEOUT):
                 await self._wsrpc.connect(self.aiohttp_session)
                 await self.update_config()
 
-                if not async_init or self._status is None:
+                if self._status is None:
                     await self.update_status()
 
             self.initialized = True
         except InvalidAuthError as err:
             self._last_error = InvalidAuthError(err)
             _LOGGER.debug("host %s:%s: error: %r", ip, port, self._last_error)
-            # Auth error during async init, used by sleeping devices
-            # Will raise 'InvalidAuthError' on next property read
-            if not async_init:
-                await self._disconnect_websocket()
-                raise
-            self.initialized = True
-        except (MacAddressMismatchError, FirmwareUnsupported) as err:
+            await self._disconnect_websocket()
+            raise
+        except MacAddressMismatchError as err:
             self._last_error = err
             _LOGGER.debug("host %s:%s: error: %r", ip, port, err)
-            if not async_init:
-                await self._disconnect_websocket()
-                raise
+            await self._disconnect_websocket()
+            raise
         except (*CONNECT_ERRORS, RpcCallError) as err:
             self._last_error = DeviceConnectionError(err)
             _LOGGER.debug("host %s:%s: error: %r", ip, port, self._last_error)
-            if not async_init:
-                await self._disconnect_websocket()
-                raise DeviceConnectionError(err) from err
+            await self._disconnect_websocket()
+            raise DeviceConnectionError(err) from err
         finally:
             self._initializing = False
 
         if self._update_listener and self.initialized:
             self._update_listener(self, RpcUpdateType.INITIALIZED)
 
     async def shutdown(self) -> None:
         """Shutdown device and remove the listener.
 
         This method will unsubscribe the update listener and disconnect the websocket.
 
-        To fully reverse a shutdown, call initialize() and subscribe_updates() again.
         """
         self._update_listener = None
         await self._disconnect_websocket()
 
     async def _disconnect_websocket(self) -> None:
         """Disconnect websocket."""
         if self._unsub_ws:
-            self._unsub_ws()
+            try:
+                self._unsub_ws()
+            except KeyError as err:
+                _LOGGER.error(
+                    "host %s: error during shutdown: %r", self.options.ip_address, err
+                )
             self._unsub_ws = None
 
         await self._wsrpc.disconnect()
 
     def subscribe_updates(self, update_listener: Callable) -> None:
         """Subscribe to device status updates."""
         self._update_listener = update_listener
@@ -338,15 +326,15 @@
         return bool(self.shelly["auth_en"])
 
     async def call_rpc(
         self, method: str, params: dict[str, Any] | None = None
     ) -> dict[str, Any]:
         """Call RPC method."""
         try:
-            async with async_timeout.timeout(DEVICE_IO_TIMEOUT):
+            async with asyncio.timeout(DEVICE_IO_TIMEOUT):
                 return await self._wsrpc.call(method, params)
         except (InvalidAuthError, RpcCallError) as err:
             self._last_error = err
             raise
         except CONNECT_ERRORS as err:
             self._last_error = DeviceConnectionError(err)
             raise DeviceConnectionError from err
@@ -427,7 +415,21 @@
         """Return true if device is connected."""
         return self._wsrpc.connected
 
     @property
     def last_error(self) -> ShellyError | None:
         """Return the last error during async device init."""
         return self._last_error
+
+    @property
+    def firmware_supported(self) -> bool:
+        """Return True if device firmware version is supported."""
+        fw_ver = GEN2_MIN_FIRMWARE_DATE if self.gen == GEN2 else GEN3_MIN_FIRMWARE_DATE
+
+        match = FIRMWARE_PATTERN.search(self.firmware_version)
+
+        if match is None:
+            return False
+
+        # We compare firmware release dates because Shelly version numbering is
+        # inconsistent, sometimes the word is used as the version number.
+        return int(match[0]) >= fw_ver
```

### Comparing `aioshelly-8.2.0/aioshelly/rpc_device/models.py` & `aioshelly-9.0.0/aioshelly/rpc_device/models.py`

 * *Files identical despite different names*

### Comparing `aioshelly-8.2.0/aioshelly/rpc_device/wsrpc.py` & `aioshelly-9.0.0/aioshelly/rpc_device/wsrpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,21 @@
 import time
 from asyncio import Task, tasks
 from collections.abc import Callable, Coroutine
 from dataclasses import dataclass
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Any, cast
 
-import aiohttp
-import async_timeout
-from aiohttp import ClientWebSocketResponse, WSMessage, WSMsgType, client_exceptions
+from aiohttp import (
+    ClientSession,
+    ClientWebSocketResponse,
+    WSMessage,
+    WSMsgType,
+    client_exceptions,
+)
 from aiohttp.web import (
     Application,
     AppRunner,
     BaseRequest,
     TCPSite,
     WebSocketResponse,
     get,
@@ -170,15 +174,15 @@
         self._background_tasks: set[Task] = set()
 
     @property
     def _next_id(self) -> int:
         self._call_id += 1
         return self._call_id
 
-    async def connect(self, aiohttp_session: aiohttp.ClientSession) -> None:
+    async def connect(self, aiohttp_session: ClientSession) -> None:
         """Connect to device."""
         if self.connected:
             raise RuntimeError("Already connected")
 
         _LOGGER.debug("Trying to connect to device at %s", self._ip_address)
         try:
             self._client = await aiohttp_session.ws_connect(
@@ -441,18 +445,18 @@
             raise RuntimeError("Not connected")
 
         future: asyncio.Future[dict[str, Any]] = self._loop.create_future()
         call = RPCCall(self._next_id, method, params, self._session, future)
         self._calls[call.call_id] = call
 
         try:
-            async with async_timeout.timeout(timeout):
+            async with asyncio.timeout(timeout):
                 await self._send_json(call.request_frame)
                 resp = await future
-        except asyncio.TimeoutError as exc:
+        except TimeoutError as exc:
             with contextlib.suppress(asyncio.CancelledError):
                 future.cancel()
                 await future
             raise DeviceConnectionError(call) from exc
 
         _LOGGER.debug("%s(%s) -> %s", call.method, call.params, resp)
         return resp
```

### Comparing `aioshelly-8.2.0/aioshelly.egg-info/PKG-INFO` & `aioshelly-9.0.0/aioshelly.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: aioshelly
-Version: 8.2.0
+Version: 9.0.0
 Summary: Asynchronous library to control Shelly devices.
 Home-page: https://github.com/home-assistant-libs/aioshelly
 Author: Paulus Schoutsen
 Author-email: paulus@home-assistant.io
 License: Apache License 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bluetooth-data-tools>=1.19.0
 Requires-Dist: aiohttp
 Requires-Dist: habluetooth>=2.1.0
 Requires-Dist: yarl
 Requires-Dist: orjson>=3.8.1
@@ -28,15 +27,15 @@
 
 Asynchronous library to control Shelly devices
 
 **This library is under development**
 
 ## Requirements
 
-- Python >= 3.10
+- Python >= 3.11
 - bluetooth-data-tools
 - aiohttp
 - orjson
 
 ## Install
 ```bash
 pip install aioshelly
@@ -55,31 +54,24 @@
 import asyncio
 from pprint import pprint
 
 import aiohttp
 
 from aioshelly.block_device import COAP, BlockDevice
 from aioshelly.common import ConnectionOptions
-from aioshelly.exceptions import (
-    DeviceConnectionError,
-    FirmwareUnsupported,
-    InvalidAuthError,
-)
+from aioshelly.exceptions import DeviceConnectionError, InvalidAuthError
 
 
 async def test_block_device():
     """Test Gen1 Block (CoAP) based device."""
     options = ConnectionOptions("192.168.1.165", "username", "password")
 
     async with aiohttp.ClientSession() as aiohttp_session, COAP() as coap_context:
         try:
             device = await BlockDevice.create(aiohttp_session, coap_context, options)
-        except FirmwareUnsupported as err:
-            print(f"Device firmware not supported, error: {repr(err)}")
-            return
         except InvalidAuthError as err:
             print(f"Invalid or missing authorization, error: {repr(err)}")
             return
         except DeviceConnectionError as err:
             print(f"Error connecting to {options.ip_address}, error: {repr(err)}")
             return
 
@@ -98,34 +90,27 @@
 ```python
 import asyncio
 from pprint import pprint
 
 import aiohttp
 
 from aioshelly.common import ConnectionOptions
-from aioshelly.exceptions import (
-    DeviceConnectionError,
-    FirmwareUnsupported,
-    InvalidAuthError,
-)
+from aioshelly.exceptions import DeviceConnectionError, InvalidAuthError
 from aioshelly.rpc_device import RpcDevice, WsServer
 
 
 async def test_rpc_device():
     """Test Gen2/Gen3 RPC (WebSocket) based device."""
     options = ConnectionOptions("192.168.1.188", "username", "password")
     ws_context = WsServer()
     await ws_context.initialize(8123)
 
     async with aiohttp.ClientSession() as aiohttp_session:
         try:
             device = await RpcDevice.create(aiohttp_session, ws_context, options)
-        except FirmwareUnsupported as err:
-            print(f"Device firmware not supported, error: {repr(err)}")
-            return
         except InvalidAuthError as err:
             print(f"Invalid or missing authorization, error: {repr(err)}")
             return
         except DeviceConnectionError as err:
             print(f"Error connecting to {options.ip_address}, error: {repr(err)}")
             return
```

### Comparing `aioshelly-8.2.0/aioshelly.egg-info/SOURCES.txt` & `aioshelly-9.0.0/aioshelly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioshelly-8.2.0/setup.py` & `aioshelly-9.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "8.2.0"
+VERSION = "9.0.0"
 
 with open("requirements.txt", encoding="utf-8") as file:  # noqa: PTH123
     requirements = file.read().splitlines()
 
 setup(
     name="aioshelly",
     version=VERSION,
@@ -18,23 +18,22 @@
     url="https://github.com/home-assistant-libs/aioshelly",
     author="Paulus Schoutsen",
     author_email="paulus@home-assistant.io",
     description="Asynchronous library to control Shelly devices.",
     long_description=README_FILE.read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    python_requires=">=3.10",
+    python_requires=">=3.11",
     package_data={"aioshelly": ["py.typed"]},
     zip_safe=True,
     platforms="any",
     install_requires=requirements,
     classifiers=[
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

### Comparing `aioshelly-8.2.0/tools/common/__init__.py` & `aioshelly-9.0.0/tools/common/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,86 +1,126 @@
 # Common tools methods
 """Methods for aioshelly cmdline tools."""
 
 from __future__ import annotations
 
+import asyncio
 import sys
 from collections.abc import Callable
-from datetime import datetime, timezone
+from datetime import UTC, datetime
 from functools import partial
 from typing import TYPE_CHECKING, Any, cast
 
-import aiohttp
+from aiohttp import ClientSession
 
 from aioshelly.block_device import BLOCK_VALUE_UNIT, COAP, BlockDevice, BlockUpdateType
 from aioshelly.common import ConnectionOptions, get_info
 from aioshelly.const import (
     BLOCK_GENERATIONS,
     DEFAULT_HTTP_PORT,
     MODEL_NAMES,
     RPC_GENERATIONS,
 )
-from aioshelly.exceptions import InvalidAuthError, ShellyError
+from aioshelly.exceptions import (
+    CustomPortNotSupported,
+    DeviceConnectionError,
+    InvalidAuthError,
+    MacAddressMismatchError,
+    ShellyError,
+    WrongShellyGen,
+)
 from aioshelly.rpc_device import RpcDevice, RpcUpdateType, WsServer
 
 coap_context = COAP()
 ws_context = WsServer()
+init_tasks_ref = set()
 
 
 async def create_device(
-    aiohttp_session: aiohttp.ClientSession,
+    aiohttp_session: ClientSession,
     options: ConnectionOptions,
-    init: bool,
     gen: int | None,
 ) -> Any:
     """Create a Gen1/Gen2/Gen3 device."""
     if gen is None:
         if info := await get_info(
             aiohttp_session, options.ip_address, port=options.port
         ):
             gen = info.get("gen", 1)
         else:
             raise ShellyError("Unknown Gen")
 
     if gen in BLOCK_GENERATIONS:
-        return await BlockDevice.create(aiohttp_session, coap_context, options, init)
+        return await BlockDevice.create(aiohttp_session, coap_context, options)
 
     if gen in RPC_GENERATIONS:
-        return await RpcDevice.create(aiohttp_session, ws_context, options, init)
+        return await RpcDevice.create(aiohttp_session, ws_context, options)
 
     raise ShellyError("Unknown Gen")
 
 
+async def init_device(device: BlockDevice | RpcDevice) -> bool:
+    """Initialize Shelly device."""
+    port = getattr(device, "port", DEFAULT_HTTP_PORT)
+    try:
+        await device.initialize()
+    except InvalidAuthError as err:
+        print(f"Invalid or missing authorization, error: {err!r}")
+    except DeviceConnectionError as err:
+        print(f"Error connecting to {device.ip_address}:{port}, " f"error: {err!r}")
+    except MacAddressMismatchError as err:
+        print(f"MAC address mismatch, error: {err!r}")
+    except WrongShellyGen:
+        print(f"Wrong Shelly generation for device {device.ip_address}:{port}")
+    except CustomPortNotSupported:
+        print("Custom port not supported for Gen1")
+    else:
+        return True
+
+    return False
+
+
 async def connect_and_print_device(
-    aiohttp_session: aiohttp.ClientSession,
+    aiohttp_session: ClientSession,
     options: ConnectionOptions,
     init: bool,
     gen: int | None,
-) -> None:
+) -> bool:
     """Connect and print device data."""
-    device = await create_device(aiohttp_session, options, init, gen)
+    device = await create_device(aiohttp_session, options, gen)
+
+    if init and not await init_device(device):
+        return False
+
     print_device(device)
     device.subscribe_updates(partial(device_updated, action=print_device))
 
+    return True
+
 
 def device_updated(
     cb_device: BlockDevice | RpcDevice,
     update_type: BlockUpdateType | RpcUpdateType,
     action: Callable[[BlockDevice | RpcDevice], None],
 ) -> None:
     """Device updated callback."""
     print()
     print(
-        f"{datetime.now(tz=timezone.utc).strftime('%H:%M:%S')} "
+        f"{datetime.now(tz=UTC).strftime('%H:%M:%S')} "
         f"Device updated! ({update_type})"
     )
-    try:
-        action(cb_device)
-    except InvalidAuthError:
-        print("Invalid or missing authorization (from async init)")
+
+    if update_type in (BlockUpdateType.ONLINE, RpcUpdateType.ONLINE):
+        loop = asyncio.get_running_loop()
+        init_task = loop.create_task(init_device(cb_device))
+        init_tasks_ref.add(init_task)
+        init_task.add_done_callback(init_tasks_ref.remove)
+        return
+
+    action(cb_device)
 
 
 def print_device(device: BlockDevice | RpcDevice) -> None:
     """Print device data."""
     port = getattr(device, "port", DEFAULT_HTTP_PORT)
     if not device.initialized:
         print()
@@ -88,14 +128,17 @@
         print()
         return
 
     model_name = MODEL_NAMES.get(device.model) or f"Unknown ({device.model})"
     print(f"** {device.name} - {model_name}  @ {device.ip_address}:{port} **")
     print()
 
+    if not device.firmware_supported:
+        print(f"Device firmware not supported: {device.firmware_version}")
+
     if device.gen in BLOCK_GENERATIONS:
         print_block_device(cast(BlockDevice, device))
     elif device.gen in RPC_GENERATIONS:
         print_rpc_device(cast(RpcDevice, device))
 
 
 def print_block_device(device: BlockDevice) -> None:
@@ -130,11 +173,11 @@
     sys.exit(_exit_code)
 
 
 async def update_outbound_ws(
     options: ConnectionOptions, init: bool, ws_url: str
 ) -> None:
     """Update outbound WebSocket URL (Gen2/3)."""
-    async with aiohttp.ClientSession() as aiohttp_session:
+    async with ClientSession() as aiohttp_session:
         device: RpcDevice = await create_device(aiohttp_session, options, init, 2)
         print(f"Updating outbound weboskcet URL to {ws_url}")
         print(f"Restart required: {await device.update_outbound_websocket(ws_url)}")
```

### Comparing `aioshelly-8.2.0/tools/example.py` & `aioshelly-9.0.0/tools/example.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,63 +9,37 @@
 import logging
 import signal
 import traceback
 from functools import partial
 from pathlib import Path
 from types import FrameType
 
-import aiohttp
+from aiohttp import ClientSession
 from common import (
     close_connections,
     coap_context,
     connect_and_print_device,
     create_device,
     device_updated,
+    init_device,
     print_device,
     update_outbound_ws,
     ws_context,
 )
 
 from aioshelly.common import ConnectionOptions
 from aioshelly.const import DEFAULT_HTTP_PORT, WS_API_URL
-from aioshelly.exceptions import (
-    CustomPortNotSupported,
-    DeviceConnectionError,
-    FirmwareUnsupported,
-    InvalidAuthError,
-    MacAddressMismatchError,
-    WrongShellyGen,
-)
 
 
 async def test_single(options: ConnectionOptions, init: bool, gen: int | None) -> None:
     """Test single device."""
-    async with aiohttp.ClientSession() as aiohttp_session:
-        try:
-            device = await create_device(aiohttp_session, options, init, gen)
-        except FirmwareUnsupported as err:
-            print(f"Device firmware not supported, error: {err!r}")
-            return
-        except InvalidAuthError as err:
-            print(f"Invalid or missing authorization, error: {err!r}")
-            return
-        except DeviceConnectionError as err:
-            print(
-                f"Error connecting to {options.ip_address}:{options.port}, "
-                f"error: {err!r}"
-            )
-            return
-        except MacAddressMismatchError as err:
-            print(f"MAC address mismatch, error: {err!r}")
-            return
-        except WrongShellyGen:
-            print(f"Wrong Shelly generation {gen}, device gen: {2 if gen==1 else 1}")
-            return
-        except CustomPortNotSupported:
-            print(f"Custom port ({options.port}) not supported for Gen1")
+    async with ClientSession() as aiohttp_session:
+        device = await create_device(aiohttp_session, options, gen)
+
+        if init and not await init_device(device):
             return
 
         print_device(device)
 
         device.subscribe_updates(partial(device_updated, action=print_device))
 
         while True:
@@ -75,43 +49,29 @@
 async def test_devices(init: bool, gen: int | None) -> None:
     """Test multiple devices."""
     options: ConnectionOptions
 
     with Path.open("devices.json", encoding="utf8") as fp:
         device_options = [ConnectionOptions(**json.loads(line)) for line in fp]
 
-    async with aiohttp.ClientSession() as aiohttp_session:
+    async with ClientSession() as aiohttp_session:
         results = await asyncio.gather(
             *[
                 asyncio.gather(
                     connect_and_print_device(aiohttp_session, options, init, gen),
                 )
                 for options in device_options
             ],
             return_exceptions=True,
         )
 
         for options, result in zip(device_options, results, strict=False):
-            if not isinstance(result, Exception):
-                continue
-
-            print()
-            print(f"Error printing device @ {options.ip_address}:{options.port}")
-
-            if isinstance(result, FirmwareUnsupported):
-                print("Device firmware not supported")
-            elif isinstance(result, InvalidAuthError):
-                print("Invalid or missing authorization")
-            elif isinstance(result, DeviceConnectionError):
-                print("Error connecting to device")
-            elif isinstance(result, MacAddressMismatchError):
-                print("MAC address mismatch error")
-            elif isinstance(result, WrongShellyGen):
-                print("Wrong Shelly generation")
-            else:
+            if isinstance(result, bool) and not result:
+                print(f"Error printing device @ {options.ip_address}:{options.port}")
+            elif isinstance(result, Exception):
                 print()
                 traceback.print_tb(result.__traceback__)
                 print(result)
 
         while True:
             await asyncio.sleep(0.1)
```

### Comparing `aioshelly-8.2.0/tools/fixture.py` & `aioshelly-9.0.0/tools/fixture.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,58 +9,43 @@
 import signal
 import sys
 from functools import partial
 from pathlib import Path
 from types import FrameType
 from typing import Any
 
-import aiohttp
 import orjson
-from common import close_connections, create_device, device_updated
+from aiohttp import ClientSession
+from common import (
+    close_connections,
+    coap_context,
+    create_device,
+    device_updated,
+    init_device,
+    ws_context,
+)
 
-from aioshelly.block_device import COAP, BlockDevice
+from aioshelly.block_device import BlockDevice
 from aioshelly.common import ConnectionOptions
 from aioshelly.const import BLOCK_GENERATIONS, MODEL_NAMES, WS_API_URL
-from aioshelly.exceptions import (
-    DeviceConnectionError,
-    FirmwareUnsupported,
-    InvalidAuthError,
-    MacAddressMismatchError,
-    WrongShellyGen,
-)
-from aioshelly.rpc_device import RpcDevice, WsServer
-
-coap_context = COAP()
-ws_context = WsServer()
+from aioshelly.rpc_device import RpcDevice
 
 
 async def connect_and_save(
     options: ConnectionOptions, init: bool, gen: int | None
 ) -> None:
     """Save fixture single device."""
-    async with aiohttp.ClientSession() as aiohttp_session:
-        try:
-            device = await create_device(aiohttp_session, options, init, gen)
-        except FirmwareUnsupported as err:
-            print(f"Device firmware not supported, error: {err!r}")
-            return
-        except InvalidAuthError as err:
-            print(f"Invalid or missing authorization, error: {err!r}")
-            return
-        except DeviceConnectionError as err:
-            print(f"Error connecting to {options.ip_address}, error: {err!r}")
-            return
-        except MacAddressMismatchError as err:
-            print(f"MAC address mismatch, error: {err!r}")
-            return
-        except WrongShellyGen:
-            print(f"Wrong Shelly generation {gen}, device gen: {2 if gen==1 else 1}")
-            return
+    async with ClientSession() as aiohttp_session:
+        device = await create_device(aiohttp_session, options, gen)
+
+        if init:
+            if not await init_device(device):
+                return
 
-        save_endpoints(device)
+            save_endpoints(device)
 
         device.subscribe_updates(partial(device_updated, action=save_endpoints))
 
         while True:
             await asyncio.sleep(0.1)
```

### Comparing `aioshelly-8.2.0/tools/verify.py` & `aioshelly-9.0.0/tools/verify.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
 def run() -> None:
     """Run coiot_examples and print errors."""
     errors = []
     for example in coiot_examples():
         try:
             print_example(example)
-        except Exception as err:  # noqa: BLE001 PERF203
+        except Exception as err:  # noqa: BLE001
             errors.append((example, err))
             break
 
     for example, err in errors:
         print("Error fetching", example.name)
         print(example.url)
         print()
```

