# Comparing `tmp/trinnov-altitude-0.1.5.tar.gz` & `tmp/trinnov-altitude-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trinnov-altitude-0.1.5.tar", last modified: Wed Apr 10 16:16:24 2024, max compression
+gzip compressed data, was "trinnov-altitude-0.1.6.tar", last modified: Wed Apr 10 21:58:21 2024, max compression
```

## Comparing `trinnov-altitude-0.1.5.tar` & `trinnov-altitude-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:16:24.148434 trinnov-altitude-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-10 16:16:24.148434 trinnov-altitude-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-10 16:16:24.148434 trinnov-altitude-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:16:24.144434 trinnov-altitude-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/tests/test_trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:16:24.144434 trinnov-altitude-0.1.5/trinnov_altitude/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/trinnov_altitude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/trinnov_altitude/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/trinnov_altitude/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/trinnov_altitude/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/trinnov_altitude/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/trinnov_altitude/trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:16:24.148434 trinnov-altitude-0.1.5/trinnov_altitude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-10 16:16:24.000000 trinnov-altitude-0.1.5/trinnov_altitude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-10 16:16:24.000000 trinnov-altitude-0.1.5/trinnov_altitude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:16:24.000000 trinnov-altitude-0.1.5/trinnov_altitude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 16:16:24.000000 trinnov-altitude-0.1.5/trinnov_altitude.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 16:16:24.000000 trinnov-altitude-0.1.5/trinnov_altitude.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:58:21.407570 trinnov-altitude-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-10 21:58:21.407570 trinnov-altitude-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-10 21:58:21.407570 trinnov-altitude-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:58:21.403570 trinnov-altitude-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/tests/test_trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:58:21.403570 trinnov-altitude-0.1.6/trinnov_altitude/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/trinnov_altitude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/trinnov_altitude/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/trinnov_altitude/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/trinnov_altitude/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/trinnov_altitude/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/trinnov_altitude/trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:58:21.407570 trinnov-altitude-0.1.6/trinnov_altitude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-10 21:58:21.000000 trinnov-altitude-0.1.6/trinnov_altitude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-10 21:58:21.000000 trinnov-altitude-0.1.6/trinnov_altitude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:58:21.000000 trinnov-altitude-0.1.6/trinnov_altitude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 21:58:21.000000 trinnov-altitude-0.1.6/trinnov_altitude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 21:58:21.000000 trinnov-altitude-0.1.6/trinnov_altitude.egg-info/top_level.txt
```

### Comparing `trinnov-altitude-0.1.5/LICENSE` & `trinnov-altitude-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.5/PKG-INFO` & `trinnov-altitude-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 0.1.5
+Version: 0.1.6
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -38,47 +38,62 @@
 
 ## Installation
 
 `pip install trinnov-altitude`
 
 ## Setup
 
-### Connect
+### Power on
+
+Powers the processor on via Wake on Lan. The process must be powered on
+before you can connect.
 
 ```python
 from trinnov_altitude.trinnov_altitude import TrinnovAltitude
 
-# Instantiate the Trinnov Altitude client. Adjust the `host` and `client_id`
-# accordingly.
-altitude = TrinnovAltitude(host = "192.168.1.90", client_id = "my_altitude_integration")
+altitude = TrinnovAltitude(host = "192.168.1.90", mac = "c8:7f:54:2d:ce:f2")
+await altitude.power_on()
+```
+
+### Connect
 
-# Connect to the Trinnov Altitude processor
-await altitude.connect()
+Connect to the processor via TCP/IP. Note that you must power on the device
+before connecting. The Trinnov Altitude does not have a standby mode that will
+accept connections.
 
-# Disconnect
-await altitude.disconnect()
+```python
+from trinnov_altitude.trinnov_altitude import TrinnovAltitude
+
+altitude = TrinnovAltitude(host = "192.168.1.90")
+
+try:
+    await altitude.connect()
+finally:
+    # Always disconnect and cleanup
+    await altitude.disconnect()
 ```
 
-### Subscribe to updates
+### Listen for updates
+
+The processor will broadcast state changes to all connected clients. You must
+explicitly start listening to receive the messages and sync the internal state
+of your object.
 
 ```python
 from trinnov_altitude.trinnov_altitude import TrinnovAltitude
 
-altitude = TrinnovAltitude(host = "192.168.1.90", client_id = "my_altitude_integration")
+altitude = TrinnovAltitude(host = "192.168.1.90")
 
-# Define your callback
+# Optionally define a callback to be fired on each individual update
 def callback(message):
     # react to the change here
     pass
 
-# Register the callback. It will be called each time a message is received
-# from the processor.
-altitude.register_callback(callback)
-
-await altitude.connect()
+# Start listening for updates in an async.io Task
+altitude.start_listening(callback: callback)
 ```
 
 ## Commands
 
 All commands assume you have [setup](#setup) your Trinnov Altitude client.
 
 ### Change the volume
```

### Comparing `trinnov-altitude-0.1.5/README.md` & `trinnov-altitude-0.1.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -21,47 +21,62 @@
 
 ## Installation
 
 `pip install trinnov-altitude`
 
 ## Setup
 
-### Connect
+### Power on
+
+Powers the processor on via Wake on Lan. The process must be powered on
+before you can connect.
 
 ```python
 from trinnov_altitude.trinnov_altitude import TrinnovAltitude
 
-# Instantiate the Trinnov Altitude client. Adjust the `host` and `client_id`
-# accordingly.
-altitude = TrinnovAltitude(host = "192.168.1.90", client_id = "my_altitude_integration")
+altitude = TrinnovAltitude(host = "192.168.1.90", mac = "c8:7f:54:2d:ce:f2")
+await altitude.power_on()
+```
+
+### Connect
 
-# Connect to the Trinnov Altitude processor
-await altitude.connect()
+Connect to the processor via TCP/IP. Note that you must power on the device
+before connecting. The Trinnov Altitude does not have a standby mode that will
+accept connections.
 
-# Disconnect
-await altitude.disconnect()
+```python
+from trinnov_altitude.trinnov_altitude import TrinnovAltitude
+
+altitude = TrinnovAltitude(host = "192.168.1.90")
+
+try:
+    await altitude.connect()
+finally:
+    # Always disconnect and cleanup
+    await altitude.disconnect()
 ```
 
-### Subscribe to updates
+### Listen for updates
+
+The processor will broadcast state changes to all connected clients. You must
+explicitly start listening to receive the messages and sync the internal state
+of your object.
 
 ```python
 from trinnov_altitude.trinnov_altitude import TrinnovAltitude
 
-altitude = TrinnovAltitude(host = "192.168.1.90", client_id = "my_altitude_integration")
+altitude = TrinnovAltitude(host = "192.168.1.90")
 
-# Define your callback
+# Optionally define a callback to be fired on each individual update
 def callback(message):
     # react to the change here
     pass
 
-# Register the callback. It will be called each time a message is received
-# from the processor.
-altitude.register_callback(callback)
-
-await altitude.connect()
+# Start listening for updates in an async.io Task
+altitude.start_listening(callback: callback)
 ```
 
 ## Commands
 
 All commands assume you have [setup](#setup) your Trinnov Altitude client.
 
 ### Change the volume
```

### Comparing `trinnov-altitude-0.1.5/setup.cfg` & `trinnov-altitude-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.5/tests/test_trinnov_altitude.py` & `trinnov-altitude-0.1.6/tests/test_trinnov_altitude.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,40 +58,42 @@
 async def test_callback(mock_server):
     client = TrinnovAltitude(host="localhost", port=mock_server.port)
 
     def _update(message: Message):
         client._last_message = message  # type: ignore
 
     client.register_callback(_update)
-    await client.connect()
+    client.start_listening()
 
-    # Wait for sync task
+    # Wait for listen task to process all messages
     await asyncio.sleep(2)
     await client.disconnect()
 
     assert isinstance(client._last_message, OKMessage)  # type: ignore
 
 
 @pytest.mark.asyncio
 async def test_volume_adjust(mock_server):
     client = TrinnovAltitude(host="localhost", port=mock_server.port)
     await client.connect()
     await client.volume_adjust(2)
 
     # Wait for sync task
+    client.start_listening()
     await asyncio.sleep(0.5)
 
     assert client.volume == -38.0
     await client.disconnect()
 
 
 @pytest.mark.asyncio
 async def test_volume_set(mock_server):
     client = TrinnovAltitude(host="localhost", port=mock_server.port)
     await client.connect()
     await client.volume_set(-46)
 
     # Wait for sync task
+    client.start_listening()
     await asyncio.sleep(0.5)
 
     assert client.volume == -46.0
     await client.disconnect()
```

### Comparing `trinnov-altitude-0.1.5/trinnov_altitude/const.py` & `trinnov-altitude-0.1.6/trinnov_altitude/const.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.5/trinnov_altitude/messages.py` & `trinnov-altitude-0.1.6/trinnov_altitude/messages.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.5/trinnov_altitude/mocks.py` & `trinnov-altitude-0.1.6/trinnov_altitude/mocks.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.5/trinnov_altitude/trinnov_altitude.py` & `trinnov-altitude-0.1.6/trinnov_altitude/trinnov_altitude.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 Implements the Trinnov Altitude processor automation protocol over TCP/IP
 """
 
 import asyncio
-from collections.abc import Callable
+from collections.abc import Callable, Set
 import logging
 import re
+from typing import TypeAlias
 from wakeonlan import send_magic_packet
 
 from trinnov_altitude import const, exceptions, messages
 
+Callback: TypeAlias = Callable[[messages.Message], None]
+
 
 class TrinnovAltitude:
     """
     Trinnov Altitude
 
     A class for interfacing with the Trinnov Altitude processor via the TCP/IP protocol.
     """
@@ -48,31 +51,30 @@
         # Verify it starts with Trinnov associates OUIs
         mac_oui = normalized_mac_address[:8]
         if not any(mac_oui == oui for oui in cls.VALID_OUIS):
             raise exceptions.InvalidMacAddressOUIError(mac_oui, cls.VALID_OUIS)
 
         return True
 
-    @classmethod
-    def wake_on_lan(cls, mac_address):
-        """Wake the processor via WoL."""
-        cls.validate_mac(mac_address)
-        send_magic_packet(mac_address)
-
     def __init__(
         self,
         host: str,
         port: int = DEFAULT_PORT,
+        mac: str | None = None,
         client_id: str = DEFAULT_CLIENT_ID,
         timeout: float = DEFAULT_TIMEOUT,
         logger: logging.Logger = logging.getLogger(__name__),
     ):
+        if mac is not None:
+            self.__class__.validate_mac(mac)
+
         # Settings
         self.host = host
         self.port = port
+        self.mac = mac
         self.client_id = client_id
         self.timeout = timeout
         self.logger = logger
 
         # State
         self.audiosync: bool | None = None
         self.bypass: bool | None = None
@@ -82,320 +84,367 @@
         self.presets: dict = {}
         self.source: str | None = None
         self.sources: dict = {}
         self.version: str | None = None
         self.volume: float | None = None
 
         # Utility
-        self._callback: Callable[[messages.Message], None] | None = None
+        self._callbacks: Set[Callback] = set()
         self._reader: asyncio.StreamReader | None = None
         self._response_handler_task: asyncio.Task | None = None
         self._writer: asyncio.StreamWriter | None = None
 
     # --------------------------
     # Connection
     # --------------------------
 
-    async def connect(self, timeout=USE_DEFAULT_TIMEOUT):
-        """Initiates connection to the processor"""
+    async def connect(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
+        """Initiates the TCP connection to the processor"""
         self.logger.info("Connecting to Altitude: %s:%s", self.host, self.port)
 
         if timeout is self.USE_DEFAULT_TIMEOUT:
             timeout = self.timeout
 
         try:
             self._reader, self._writer = await asyncio.wait_for(
                 asyncio.open_connection(self.host, self.port), timeout
             )
         except asyncio.TimeoutError:
             raise exceptions.ConnectionTimeoutError
         except Exception as e:
             raise exceptions.ConnectionFailedError(e)
 
-        self._response_handler_task = asyncio.create_task(self._sync())
-
-        await self._send(f"id {self.client_id}", timeout)
+        await self._write(f"id {self.client_id}", timeout)
 
-    def connected(self):
+    def connected(self) -> bool:
+        """Returns the connection state."""
         return self._reader is not None and self._writer is not None
 
-    async def disconnect(self, timeout=USE_DEFAULT_TIMEOUT):
-        """Closes the connection to the processor"""
+    async def disconnect(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
+        """Closes the TCP connection to the processor"""
         if self._writer is None:
             return
 
         if timeout is self.USE_DEFAULT_TIMEOUT:
             timeout = self.timeout
 
         if self._response_handler_task:
             self._response_handler_task.cancel()
             try:
                 await self._response_handler_task
             except asyncio.CancelledError:
                 pass
             self._response_handler_task = None
 
-        await self._send("bye", timeout)
+        await self._write("bye", timeout)
         self._writer.close()
         await asyncio.wait_for(self._writer.wait_closed(), timeout)
         self._reader = None
         self._writer = None
 
-    def register_callback(self, callback: Callable[[messages.Message], None]):
-        self._callback = callback
+    def power_on(self):
+        """Power on the processor via WoL."""
+        if self.mac is None:
+            raise exceptions.NoMacAddressError()
+
+        send_magic_packet(self.mac)
+
+    def register_callback(self, callback: Callback):
+        """
+        Register a callback to be fired when messages are received from
+        the processor.
+        """
+        self._callbacks.add(callback)
+
+    def start_listening(
+        self,
+        callback: Callback = None,
+        reconnect: bool = True,
+        reconnect_backoff: int = 2,
+    ):
+        if callback:
+            self.register_callback(callback)
+
+        self._response_handler_task = asyncio.create_task(
+            self._listen(reconnect, reconnect_backoff)
+        )
 
     # --------------------------
     # Commands
     # --------------------------
     async def acoustic_correction_set(
-        self, state: bool, timeout: float = USE_DEFAULT_TIMEOUT
+        self, state: bool, timeout: float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Set the acoustic correction to On (True) or Off (False)
         """
-        await self._send(f"use_acoustic_correct {int(state)}", timeout)
+        await self._write(f"use_acoustic_correct {int(state)}", timeout)
 
-    async def acoustic_correction_toggle(self, timeout: float = USE_DEFAULT_TIMEOUT):
+    async def acoustic_correction_toggle(
+        self, timeout: float | None = USE_DEFAULT_TIMEOUT
+    ):
         """
         Toggle the acoustic correction state.
         """
-        await self._send("use_acoustic_correct 2", timeout)
+        await self._write("use_acoustic_correct 2", timeout)
 
-    async def bypass_set(self, state: bool, timeout: float = USE_DEFAULT_TIMEOUT):
+    async def bypass_set(
+        self, state: bool, timeout: float | None = USE_DEFAULT_TIMEOUT
+    ):
         """
         Set the bypass state to On (True) or Off (False)
         """
-        await self._send(f"bypass {int(state)}", timeout)
+        await self._write(f"bypass {int(state)}", timeout)
 
-    async def bypass_toggle(self, timeout: float = USE_DEFAULT_TIMEOUT):
+    async def bypass_toggle(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
         """
         Toggle the bypass state.
         """
-        await self._send("bypass 2", timeout)
+        await self._write("bypass 2", timeout)
 
-    async def dim_set(self, state: bool, timeout: float = USE_DEFAULT_TIMEOUT):
+    async def dim_set(self, state: bool, timeout: float | None = USE_DEFAULT_TIMEOUT):
         """
         Set the dim state to On (True) or Off (False)
         """
-        await self._send(f"dim {int(state)}", timeout)
+        await self._write(f"dim {int(state)}", timeout)
 
-    async def dim_toggle(self, timeout=USE_DEFAULT_TIMEOUT):
+    async def dim_toggle(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
         """
         Toggle the dim state.
         """
-        await self._send("dim 2", timeout)
+        await self._write("dim 2", timeout)
 
     async def front_display_set(
-        self, state: bool, timeout: float = USE_DEFAULT_TIMEOUT
+        self, state: bool, timeout: float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Set the front display of the processor to On (True) or Off (False).
         """
-        await self._send(f"fav_light {int(state)}", timeout)
+        await self._write(f"fav_light {int(state)}", timeout)
 
-    async def front_display_toggle(self, timeout=USE_DEFAULT_TIMEOUT):
+    async def front_display_toggle(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
         """
         Toggle the front display of the processor.
         """
-        await self._send("dim 2", timeout)
+        await self._write("dim 2", timeout)
 
     async def level_alignment_set(
-        self, state: bool, timeout: float = USE_DEFAULT_TIMEOUT
+        self, state: bool, timeout: float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Set the level alignment state to On (True) or Off (False)
         """
-        await self._send(f"use_level_alignment {int(state)}", timeout)
+        await self._write(f"use_level_alignment {int(state)}", timeout)
 
-    async def level_alignment_toggle(self, state, timeout=USE_DEFAULT_TIMEOUT):
+    async def level_alignment_toggle(
+        self, state, timeout: float | None = USE_DEFAULT_TIMEOUT
+    ):
         """
         Toggle the level alignment state.
         """
-        await self._send("use_level_alignment 2", timeout)
+        await self._write("use_level_alignment 2", timeout)
 
-    async def mute_set(self, state: bool, timeout: float = USE_DEFAULT_TIMEOUT):
+    async def mute_set(self, state: bool, timeout: float | None = USE_DEFAULT_TIMEOUT):
         """
         Set the mute state to On (True) or Off (False)
         """
-        await self._send(f"mute {int(state)}", timeout)
+        await self._write(f"mute {int(state)}", timeout)
 
-    async def mute_toggle(self, state, timeout=USE_DEFAULT_TIMEOUT):
+    async def mute_toggle(self, state, timeout: float | None = USE_DEFAULT_TIMEOUT):
         """
         Toggle the mute state.
         """
-        await self._send("mute 2", timeout)
+        await self._write("mute 2", timeout)
 
-    async def page_adjust(self, delta: int, timeout: float = USE_DEFAULT_TIMEOUT):
+    async def page_adjust(
+        self, delta: int, timeout: float | None = USE_DEFAULT_TIMEOUT
+    ):
         """
         Changes the menu page currently on the GUI. `delta` indicates the number of
         pages to change, and may be positive or negative.
         """
-        await self._send("bypass 2", timeout)
+        await self._write("bypass 2", timeout)
 
-    async def power_off(self, timeout=USE_DEFAULT_TIMEOUT):
+    async def power_off(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
         """
         Power off.
         """
-        await self._send("power off SECURED FHZMCH48FE", timeout)
+        await self._write("power off SECURED FHZMCH48FE", timeout)
 
-    async def preset_load(self, id: int, timeout: float = USE_DEFAULT_TIMEOUT):
+    async def preset_load(self, id: int, timeout: float | None = USE_DEFAULT_TIMEOUT):
         """
         Load the preset identified by `id`. Preset `0` is the built-in preset and
         presets >= `1` are user defined presets.
         """
-        await self._send("bypass 2", timeout)
+        await self._write("bypass 2", timeout)
 
     async def quick_optimized_set(
-        self, state: bool, timeout: float = USE_DEFAULT_TIMEOUT
+        self, state: bool, timeout: float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Set the quick optimized state to On (True) or Off (False)
         """
-        await self._send(f"quick_optimized {int(state)}", timeout)
+        await self._write(f"quick_optimized {int(state)}", timeout)
 
-    async def quick_optimized_toggle(self, state, timeout=USE_DEFAULT_TIMEOUT):
+    async def quick_optimized_toggle(
+        self, state, timeout: float | None = USE_DEFAULT_TIMEOUT
+    ):
         """
         Toggle the quick optimized state.
         """
-        await self._send("quick_optimized 2", timeout)
+        await self._write("quick_optimized 2", timeout)
 
     async def remapping_mode_set(
-        self, mode: const.RemappingMode, timeout: float = USE_DEFAULT_TIMEOUT
+        self, mode: const.RemappingMode, timeout: float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Set the remapping mode. See `const.RemappingMode` for available options
         and descriptions.
         """
-        await self._send(f"remapping_mode {mode.value}", timeout)
+        await self._write(f"remapping_mode {mode.value}", timeout)
 
-    async def source_set(self, id: int, timeout: float = USE_DEFAULT_TIMEOUT):
+    async def source_set(self, id: int, timeout: float | None = USE_DEFAULT_TIMEOUT):
         """
         Set the source identified by `id`, where `0` is the first source.
         """
-        await self._send(f"profile {id}", timeout)
+        await self._write(f"profile {id}", timeout)
 
     async def time_alignment_set(
-        self, state: bool, timeout: float = USE_DEFAULT_TIMEOUT
+        self, state: bool, timeout: float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Set the time alignment state to On (True) or Off (False)
         """
-        await self._send(f"use_time_alignment {int(state)}", timeout)
+        await self._write(f"use_time_alignment {int(state)}", timeout)
 
-    async def time_alignment_toggle(self, state, timeout=USE_DEFAULT_TIMEOUT):
+    async def time_alignment_toggle(
+        self, state, timeout: float | None = USE_DEFAULT_TIMEOUT
+    ):
         """
         Toggle the time alignment state.
         """
-        await self._send("use_time_alignment 2", timeout)
+        await self._write("use_time_alignment 2", timeout)
 
     async def upmixer_set(
-        self, mode: const.UpmixerMode, timeout: float = USE_DEFAULT_TIMEOUT
+        self, mode: const.UpmixerMode, timeout: float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Set the upmixer mode. See `const.UpmixerMode` for available options
         and descriptions.
         """
-        await self._send(f"remapping_mode {mode.value}", timeout)
+        await self._write(f"remapping_mode {mode.value}", timeout)
 
-    async def volume_adjust(self, delta: float, timeout=USE_DEFAULT_TIMEOUT):
+    async def volume_adjust(
+        self, delta: float, timeout: float | None = USE_DEFAULT_TIMEOUT
+    ):
         """
         Adjust the volume by a relative dB value (float).
         """
-        await self._send(f"dvolume {delta}", timeout)
+        await self._write(f"dvolume {delta}", timeout)
 
-    async def volume_set(self, db: float, timeout=USE_DEFAULT_TIMEOUT):
+    async def volume_set(self, db: float, timeout: float | None = USE_DEFAULT_TIMEOUT):
         """
         Set the volume to an absolute dB value (float).
         """
-        await self._send(f"volume {db}", timeout)
+        await self._write(f"volume {db}", timeout)
 
-    async def volume_ramp(self, db: float, duration: int, timeout=USE_DEFAULT_TIMEOUT):
+    async def volume_ramp(
+        self, db: float, duration: int, timeout: float | None = USE_DEFAULT_TIMEOUT
+    ):
         """
         Ramp the volume to an absolute dB value (float) over a number of milliseconds (int).
         """
-        await self._send(f"volume_ramp {db} {duration}", timeout)
+        await self._write(f"volume_ramp {db} {duration}", timeout)
 
     # --------------------------
     # Utility
     # --------------------------
+    async def _listen(self, reconnect: bool, reconnect_backoff: float):
+        """
+        Listen for messages and sync internal state
 
-    async def _receive(self, timeout):
-        """Receives a single message from the processor"""
+        This method will automatically reconnect when necessary if `reconnect`
+        is set to `True`.
+        """
+        while True:
+            try:
+                raw_message = await self._read(timeout=None)
+            except (EOFError, OSError, Exception) as e:
+                if reconnect:
+                    self.logger.error(
+                        f"Unable to read message from Trinnov Altitude, reconnecting...: {e}"
+                    )
+
+                    try:
+                        await self.connect(timeout=1)
+                    except Exception as err:  # pylint: disable=broad-except
+                        self.logger.exception(
+                            "Unhandled exception %s('%s')", type(err).__name__, err
+                        )
+                        await asyncio.sleep(reconnect_backoff)
+                else:
+                    raise e
+            else:
+                self._process_message(raw_message)
+
+    async def _read(self, timeout: float | None) -> str:
+        """Read a single raw message off of the socket"""
         if self._reader is None:
             raise exceptions.NotConnectedError()
 
         if timeout is self.USE_DEFAULT_TIMEOUT:
             timeout = self.timeout
 
-        try:
-            message = await asyncio.wait_for(self._reader.readline(), timeout)
-            message = message.decode().rstrip()
-
-            if message == "":
-                await self.disconnect(timeout)
-                return None
-
-            self.logger.debug(f"Received from Altitude: {message}")
-            return message
-        except asyncio.TimeoutError:
-            return None
+        message = await asyncio.wait_for(self._reader.readline(), timeout)
+        message = message.decode().rstrip()
+        self.logger.debug(f"Received from Altitude: {message}")
+        return message
+
+    def _process_message(self, raw_message: str):  # noqa: C901
+        """Receive a single message off of the socket and process it."""
+        message = messages.message_factory(raw_message)
+
+        if isinstance(message, messages.AudiosyncMessage):
+            self.audiosync = message.state
+        elif isinstance(message, messages.BypassMessage):
+            self.bypass = message.state
+        elif isinstance(message, messages.DimMessage):
+            self.dim = message.state
+        elif isinstance(message, messages.ErrorMessage):
+            self.logger.error(f"Trinnov Altitude responsed with error: {message.error}")
+        elif isinstance(message, messages.PresetMessage):
+            self.presets[message.index] = message.name
+        elif isinstance(message, messages.PresetsClearMessage):
+            self.presets = {}
+        elif isinstance(message, messages.MuteMessage):
+            self.mute = message.state
+        elif isinstance(message, messages.SourceMessage):
+            self.sources[message.index] = message.name
+        elif isinstance(message, messages.SourcesClearMessage):
+            self.sources = {}
+        elif isinstance(message, messages.SamplingRateMessage):
+            self.sampling_rate = message.rate
+        elif isinstance(message, messages.VolumeMessage):
+            self.volume = message.volume
+        elif isinstance(message, messages.WelcomeMessage):
+            self.version = message.version
+            self.id = message.id
+
+        if message is not None:
+            for callback in self._callbacks:
+                callback(message)
 
-    async def _send(self, message: str, timeout):
-        """Sends a message to the processor"""
+    async def _write(self, message: str, timeout: float | None):
+        """Write a single message to the socket"""
         if self._writer is None:
             raise exceptions.NotConnectedError()
 
         if timeout is self.USE_DEFAULT_TIMEOUT:
             timeout = self.timeout
 
         if not message.endswith("\n"):
             message += "\n"
 
         message_bytes = message.encode(self.ENCODING)
         self._writer.write(message_bytes)
         await asyncio.wait_for(self._writer.drain(), timeout=timeout)
         self.logger.debug(f"Sent to Altitude: {message.rstrip()}")
-
-    async def _sync(self):  # noqa: C901
-        """
-        Sync internal state
-
-        Receives all broadcasted messages from the proessor and syncs the
-        internal state.
-        """
-        while True:
-            raw_message = await self._receive(None)
-            if raw_message is None:
-                break
-
-            message = messages.message_factory(raw_message)
-
-            if isinstance(message, messages.AudiosyncMessage):
-                self.audiosync = message.state
-            elif isinstance(message, messages.BypassMessage):
-                self.bypass = message.state
-            elif isinstance(message, messages.DimMessage):
-                self.dim = message.state
-            elif isinstance(message, messages.ErrorMessage):
-                self.logger.error(
-                    f"Trinnov Altitude responsed with error: {message.error}"
-                )
-            elif isinstance(message, messages.PresetMessage):
-                self.presets[message.index] = message.name
-            elif isinstance(message, messages.PresetsClearMessage):
-                self.presets = {}
-            elif isinstance(message, messages.MuteMessage):
-                self.mute = message.state
-            elif isinstance(message, messages.SourceMessage):
-                self.sources[message.index] = message.name
-            elif isinstance(message, messages.SourcesClearMessage):
-                self.sources = {}
-            elif isinstance(message, messages.SamplingRateMessage):
-                self.sampling_rate = message.rate
-            elif isinstance(message, messages.VolumeMessage):
-                self.volume = message.volume
-            elif isinstance(message, messages.WelcomeMessage):
-                self.version = message.version
-                self.id = message.id
-
-            if self._callback is not None and message is not None:
-                self._callback(message)
```

### Comparing `trinnov-altitude-0.1.5/trinnov_altitude.egg-info/PKG-INFO` & `trinnov-altitude-0.1.6/trinnov_altitude.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 0.1.5
+Version: 0.1.6
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -38,47 +38,62 @@
 
 ## Installation
 
 `pip install trinnov-altitude`
 
 ## Setup
 
-### Connect
+### Power on
+
+Powers the processor on via Wake on Lan. The process must be powered on
+before you can connect.
 
 ```python
 from trinnov_altitude.trinnov_altitude import TrinnovAltitude
 
-# Instantiate the Trinnov Altitude client. Adjust the `host` and `client_id`
-# accordingly.
-altitude = TrinnovAltitude(host = "192.168.1.90", client_id = "my_altitude_integration")
+altitude = TrinnovAltitude(host = "192.168.1.90", mac = "c8:7f:54:2d:ce:f2")
+await altitude.power_on()
+```
+
+### Connect
 
-# Connect to the Trinnov Altitude processor
-await altitude.connect()
+Connect to the processor via TCP/IP. Note that you must power on the device
+before connecting. The Trinnov Altitude does not have a standby mode that will
+accept connections.
 
-# Disconnect
-await altitude.disconnect()
+```python
+from trinnov_altitude.trinnov_altitude import TrinnovAltitude
+
+altitude = TrinnovAltitude(host = "192.168.1.90")
+
+try:
+    await altitude.connect()
+finally:
+    # Always disconnect and cleanup
+    await altitude.disconnect()
 ```
 
-### Subscribe to updates
+### Listen for updates
+
+The processor will broadcast state changes to all connected clients. You must
+explicitly start listening to receive the messages and sync the internal state
+of your object.
 
 ```python
 from trinnov_altitude.trinnov_altitude import TrinnovAltitude
 
-altitude = TrinnovAltitude(host = "192.168.1.90", client_id = "my_altitude_integration")
+altitude = TrinnovAltitude(host = "192.168.1.90")
 
-# Define your callback
+# Optionally define a callback to be fired on each individual update
 def callback(message):
     # react to the change here
     pass
 
-# Register the callback. It will be called each time a message is received
-# from the processor.
-altitude.register_callback(callback)
-
-await altitude.connect()
+# Start listening for updates in an async.io Task
+altitude.start_listening(callback: callback)
 ```
 
 ## Commands
 
 All commands assume you have [setup](#setup) your Trinnov Altitude client.
 
 ### Change the volume
```

