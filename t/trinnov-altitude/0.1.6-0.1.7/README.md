# Comparing `tmp/trinnov-altitude-0.1.6.tar.gz` & `tmp/trinnov-altitude-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trinnov-altitude-0.1.6.tar", last modified: Wed Apr 10 21:58:21 2024, max compression
+gzip compressed data, was "trinnov-altitude-0.1.7.tar", last modified: Wed Apr 10 23:20:23 2024, max compression
```

## Comparing `trinnov-altitude-0.1.6.tar` & `trinnov-altitude-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:58:21.407570 trinnov-altitude-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-10 21:58:21.407570 trinnov-altitude-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-10 21:58:21.407570 trinnov-altitude-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:58:21.403570 trinnov-altitude-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/tests/test_trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:58:21.403570 trinnov-altitude-0.1.6/trinnov_altitude/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/trinnov_altitude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/trinnov_altitude/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/trinnov_altitude/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/trinnov_altitude/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/trinnov_altitude/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-04-10 21:58:17.000000 trinnov-altitude-0.1.6/trinnov_altitude/trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:58:21.407570 trinnov-altitude-0.1.6/trinnov_altitude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-10 21:58:21.000000 trinnov-altitude-0.1.6/trinnov_altitude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-10 21:58:21.000000 trinnov-altitude-0.1.6/trinnov_altitude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:58:21.000000 trinnov-altitude-0.1.6/trinnov_altitude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 21:58:21.000000 trinnov-altitude-0.1.6/trinnov_altitude.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 21:58:21.000000 trinnov-altitude-0.1.6/trinnov_altitude.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:20:23.365145 trinnov-altitude-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-10 23:20:23.365145 trinnov-altitude-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-10 23:20:23.365145 trinnov-altitude-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:20:23.361145 trinnov-altitude-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/tests/test_trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:20:23.361145 trinnov-altitude-0.1.7/trinnov_altitude/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/trinnov_altitude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/trinnov_altitude/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/trinnov_altitude/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/trinnov_altitude/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/trinnov_altitude/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15916 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/trinnov_altitude/trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:20:23.365145 trinnov-altitude-0.1.7/trinnov_altitude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-10 23:20:23.000000 trinnov-altitude-0.1.7/trinnov_altitude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-10 23:20:23.000000 trinnov-altitude-0.1.7/trinnov_altitude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:20:23.000000 trinnov-altitude-0.1.7/trinnov_altitude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 23:20:23.000000 trinnov-altitude-0.1.7/trinnov_altitude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 23:20:23.000000 trinnov-altitude-0.1.7/trinnov_altitude.egg-info/top_level.txt
```

### Comparing `trinnov-altitude-0.1.6/LICENSE` & `trinnov-altitude-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.6/PKG-INFO` & `trinnov-altitude-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 0.1.6
+Version: 0.1.7
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trinnov-altitude-0.1.6/README.md` & `trinnov-altitude-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.6/setup.cfg` & `trinnov-altitude-0.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.6/tests/test_trinnov_altitude.py` & `trinnov-altitude-0.1.7/tests/test_trinnov_altitude.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.6/trinnov_altitude/const.py` & `trinnov-altitude-0.1.7/trinnov_altitude/const.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.6/trinnov_altitude/exceptions.py` & `trinnov-altitude-0.1.7/trinnov_altitude/exceptions.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.6/trinnov_altitude/messages.py` & `trinnov-altitude-0.1.7/trinnov_altitude/messages.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.6/trinnov_altitude/mocks.py` & `trinnov-altitude-0.1.7/trinnov_altitude/mocks.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.6/trinnov_altitude/trinnov_altitude.py` & `trinnov-altitude-0.1.7/trinnov_altitude/trinnov_altitude.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,17 @@
 
     # --------------------------
     # Connection
     # --------------------------
 
     async def connect(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
         """Initiates the TCP connection to the processor"""
+        if self.connected():
+            return
+
         self.logger.info("Connecting to Altitude: %s:%s", self.host, self.port)
 
         if timeout is self.USE_DEFAULT_TIMEOUT:
             timeout = self.timeout
 
         try:
             self._reader, self._writer = await asyncio.wait_for(
@@ -115,14 +118,20 @@
 
         await self._write(f"id {self.client_id}", timeout)
 
     def connected(self) -> bool:
         """Returns the connection state."""
         return self._reader is not None and self._writer is not None
 
+    def deregister_callback(self, callback: Callback):
+        """
+        Deregister a callback.
+        """
+        self._callbacks.remove(callback)
+
     async def disconnect(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
         """Closes the TCP connection to the processor"""
         if self._writer is None:
             return
 
         if timeout is self.USE_DEFAULT_TIMEOUT:
             timeout = self.timeout
@@ -137,21 +146,14 @@
 
         await self._write("bye", timeout)
         self._writer.close()
         await asyncio.wait_for(self._writer.wait_closed(), timeout)
         self._reader = None
         self._writer = None
 
-    def power_on(self):
-        """Power on the processor via WoL."""
-        if self.mac is None:
-            raise exceptions.NoMacAddressError()
-
-        send_magic_packet(self.mac)
-
     def register_callback(self, callback: Callback):
         """
         Register a callback to be fired when messages are received from
         the processor.
         """
         self._callbacks.add(callback)
 
@@ -261,19 +263,24 @@
         """
         Changes the menu page currently on the GUI. `delta` indicates the number of
         pages to change, and may be positive or negative.
         """
         await self._write("bypass 2", timeout)
 
     async def power_off(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
-        """
-        Power off.
-        """
+        """Power off."""
         await self._write("power off SECURED FHZMCH48FE", timeout)
 
+    def power_on(self):
+        """Power on."""
+        if self.mac is None:
+            raise exceptions.NoMacAddressError()
+
+        send_magic_packet(self.mac)
+
     async def preset_load(self, id: int, timeout: float | None = USE_DEFAULT_TIMEOUT):
         """
         Load the preset identified by `id`. Preset `0` is the built-in preset and
         presets >= `1` are user defined presets.
         """
         await self._write("bypass 2", timeout)
 
@@ -337,28 +344,40 @@
         self, delta: float, timeout: float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Adjust the volume by a relative dB value (float).
         """
         await self._write(f"dvolume {delta}", timeout)
 
+    async def volume_down(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
+        """
+        Lower the volume by 0.5 dB
+        """
+        await self.volume_adjust(-0.5, timeout)
+
     async def volume_set(self, db: float, timeout: float | None = USE_DEFAULT_TIMEOUT):
         """
         Set the volume to an absolute dB value (float).
         """
         await self._write(f"volume {db}", timeout)
 
     async def volume_ramp(
         self, db: float, duration: int, timeout: float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Ramp the volume to an absolute dB value (float) over a number of milliseconds (int).
         """
         await self._write(f"volume_ramp {db} {duration}", timeout)
 
+    async def volume_up(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
+        """
+        Raise the volume by 0.5 dB
+        """
+        await self.volume_adjust(0.5, timeout)
+
     # --------------------------
     # Utility
     # --------------------------
     async def _listen(self, reconnect: bool, reconnect_backoff: float):
         """
         Listen for messages and sync internal state
```

### Comparing `trinnov-altitude-0.1.6/trinnov_altitude.egg-info/PKG-INFO` & `trinnov-altitude-0.1.7/trinnov_altitude.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 0.1.6
+Version: 0.1.7
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

