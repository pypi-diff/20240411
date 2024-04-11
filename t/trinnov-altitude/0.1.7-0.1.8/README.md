# Comparing `tmp/trinnov-altitude-0.1.7.tar.gz` & `tmp/trinnov-altitude-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trinnov-altitude-0.1.7.tar", last modified: Wed Apr 10 23:20:23 2024, max compression
+gzip compressed data, was "trinnov-altitude-0.1.8.tar", last modified: Thu Apr 11 00:23:32 2024, max compression
```

## Comparing `trinnov-altitude-0.1.7.tar` & `trinnov-altitude-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:20:23.365145 trinnov-altitude-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-10 23:20:23.365145 trinnov-altitude-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-10 23:20:23.365145 trinnov-altitude-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:20:23.361145 trinnov-altitude-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/tests/test_trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:20:23.361145 trinnov-altitude-0.1.7/trinnov_altitude/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/trinnov_altitude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/trinnov_altitude/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/trinnov_altitude/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/trinnov_altitude/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/trinnov_altitude/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    15916 2024-04-10 23:20:19.000000 trinnov-altitude-0.1.7/trinnov_altitude/trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:20:23.365145 trinnov-altitude-0.1.7/trinnov_altitude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-10 23:20:23.000000 trinnov-altitude-0.1.7/trinnov_altitude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-10 23:20:23.000000 trinnov-altitude-0.1.7/trinnov_altitude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:20:23.000000 trinnov-altitude-0.1.7/trinnov_altitude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 23:20:23.000000 trinnov-altitude-0.1.7/trinnov_altitude.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 23:20:23.000000 trinnov-altitude-0.1.7/trinnov_altitude.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:23:32.540726 trinnov-altitude-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-04-11 00:23:32.540726 trinnov-altitude-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-11 00:23:32.540726 trinnov-altitude-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:23:32.540726 trinnov-altitude-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/tests/test_trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:23:32.540726 trinnov-altitude-0.1.8/trinnov_altitude/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/trinnov_altitude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/trinnov_altitude/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/trinnov_altitude/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/trinnov_altitude/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/trinnov_altitude/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19361 2024-04-11 00:23:28.000000 trinnov-altitude-0.1.8/trinnov_altitude/trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:23:32.540726 trinnov-altitude-0.1.8/trinnov_altitude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-04-11 00:23:32.000000 trinnov-altitude-0.1.8/trinnov_altitude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-11 00:23:32.000000 trinnov-altitude-0.1.8/trinnov_altitude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:23:32.000000 trinnov-altitude-0.1.8/trinnov_altitude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 00:23:32.000000 trinnov-altitude-0.1.8/trinnov_altitude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 00:23:32.000000 trinnov-altitude-0.1.8/trinnov_altitude.egg-info/top_level.txt
```

### Comparing `trinnov-altitude-0.1.7/LICENSE` & `trinnov-altitude-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.7/setup.cfg` & `trinnov-altitude-0.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.7/tests/test_trinnov_altitude.py` & `trinnov-altitude-0.1.8/tests/test_trinnov_altitude.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.7/trinnov_altitude/const.py` & `trinnov-altitude-0.1.8/trinnov_altitude/const.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.7/trinnov_altitude/exceptions.py` & `trinnov-altitude-0.1.8/trinnov_altitude/exceptions.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.7/trinnov_altitude/messages.py` & `trinnov-altitude-0.1.8/trinnov_altitude/messages.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.7/trinnov_altitude/mocks.py` & `trinnov-altitude-0.1.8/trinnov_altitude/mocks.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.7/trinnov_altitude/trinnov_altitude.py` & `trinnov-altitude-0.1.8/trinnov_altitude/trinnov_altitude.py`

 * *Files 27% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         self._response_handler_task: asyncio.Task | None = None
         self._writer: asyncio.StreamWriter | None = None
 
     # --------------------------
     # Connection
     # --------------------------
 
-    async def connect(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
+    async def connect(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
         """Initiates the TCP connection to the processor"""
         if self.connected():
             return
 
         self.logger.info("Connecting to Altitude: %s:%s", self.host, self.port)
 
         if timeout is self.USE_DEFAULT_TIMEOUT:
@@ -124,15 +124,15 @@
 
     def deregister_callback(self, callback: Callback):
         """
         Deregister a callback.
         """
         self._callbacks.remove(callback)
 
-    async def disconnect(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
+    async def disconnect(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
         """Closes the TCP connection to the processor"""
         if self._writer is None:
             return
 
         if timeout is self.USE_DEFAULT_TIMEOUT:
             timeout = self.timeout
 
@@ -155,224 +155,357 @@
         Register a callback to be fired when messages are received from
         the processor.
         """
         self._callbacks.add(callback)
 
     def start_listening(
         self,
-        callback: Callback = None,
+        callback: Callback | None = None,
         reconnect: bool = True,
         reconnect_backoff: int = 2,
     ):
         if callback:
             self.register_callback(callback)
 
         self._response_handler_task = asyncio.create_task(
             self._listen(reconnect, reconnect_backoff)
         )
 
     # --------------------------
     # Commands
     # --------------------------
+    async def acoustic_correction_off(
+        self, timeout: int | float | None = USE_DEFAULT_TIMEOUT
+    ):
+        """
+        Turn the acoustic correction off.
+        """
+        await self.acoustic_correction_set(False)
+
+    async def acoustic_correction_on(
+        self, timeout: int | float | None = USE_DEFAULT_TIMEOUT
+    ):
+        """
+        Turn the acoustic correction on.
+        """
+        await self.acoustic_correction_set(True)
+
     async def acoustic_correction_set(
-        self, state: bool, timeout: float | None = USE_DEFAULT_TIMEOUT
+        self, state: bool, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Set the acoustic correction to On (True) or Off (False)
         """
         await self._write(f"use_acoustic_correct {int(state)}", timeout)
 
     async def acoustic_correction_toggle(
-        self, timeout: float | None = USE_DEFAULT_TIMEOUT
+        self, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Toggle the acoustic correction state.
         """
         await self._write("use_acoustic_correct 2", timeout)
 
+    async def bypass_off(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
+        """
+        Turn the bypass off
+        """
+        await self.bypass_set(False)
+
+    async def bypass_on(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
+        """
+        Turn the bypass on
+        """
+        await self.bypass_set(True)
+
     async def bypass_set(
-        self, state: bool, timeout: float | None = USE_DEFAULT_TIMEOUT
+        self, state: bool, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Set the bypass state to On (True) or Off (False)
         """
         await self._write(f"bypass {int(state)}", timeout)
 
-    async def bypass_toggle(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
+    async def bypass_toggle(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
         """
         Toggle the bypass state.
         """
         await self._write("bypass 2", timeout)
 
-    async def dim_set(self, state: bool, timeout: float | None = USE_DEFAULT_TIMEOUT):
+    async def dim_off(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
+        """
+        Turn the dim off.
+        """
+        await self.dim_set(False)
+
+    async def dim_on(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
+        """
+        Turn the dim on.
+        """
+        await self.dim_set(True)
+
+    async def dim_set(
+        self, state: bool, timeout: int | float | None = USE_DEFAULT_TIMEOUT
+    ):
         """
         Set the dim state to On (True) or Off (False)
         """
         await self._write(f"dim {int(state)}", timeout)
 
-    async def dim_toggle(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
+    async def dim_toggle(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
         """
         Toggle the dim state.
         """
         await self._write("dim 2", timeout)
 
+    async def front_display_off(
+        self, timeout: int | float | None = USE_DEFAULT_TIMEOUT
+    ):
+        """
+        Turn the front display off.
+        """
+        await self.front_display_set(False)
+
+    async def front_display_on(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
+        """
+        Turn the front display on.
+        """
+        await self.front_display_set(True)
+
     async def front_display_set(
-        self, state: bool, timeout: float | None = USE_DEFAULT_TIMEOUT
+        self, state: bool, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Set the front display of the processor to On (True) or Off (False).
         """
         await self._write(f"fav_light {int(state)}", timeout)
 
-    async def front_display_toggle(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
+    async def front_display_toggle(
+        self, timeout: int | float | None = USE_DEFAULT_TIMEOUT
+    ):
         """
         Toggle the front display of the processor.
         """
         await self._write("dim 2", timeout)
 
+    async def level_alignment_off(
+        self, timeout: int | float | None = USE_DEFAULT_TIMEOUT
+    ):
+        """
+        Turn the level alignment off.
+        """
+        await self.level_alignment_set(False)
+
+    async def level_alignment_on(
+        self, timeout: int | float | None = USE_DEFAULT_TIMEOUT
+    ):
+        """
+        Turn the level alignment on.
+        """
+        await self.level_alignment_set(True)
+
     async def level_alignment_set(
-        self, state: bool, timeout: float | None = USE_DEFAULT_TIMEOUT
+        self, state: bool, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Set the level alignment state to On (True) or Off (False)
         """
         await self._write(f"use_level_alignment {int(state)}", timeout)
 
     async def level_alignment_toggle(
-        self, state, timeout: float | None = USE_DEFAULT_TIMEOUT
+        self, state, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Toggle the level alignment state.
         """
         await self._write("use_level_alignment 2", timeout)
 
-    async def mute_set(self, state: bool, timeout: float | None = USE_DEFAULT_TIMEOUT):
+    async def mute_off(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
+        """
+        Turn the mute off.
+        """
+        await self.mute_set(False)
+
+    async def mute_on(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
+        """
+        Turn the mute on.
+        """
+        await self.mute_set(True)
+
+    async def mute_set(
+        self, state: bool, timeout: int | float | None = USE_DEFAULT_TIMEOUT
+    ):
         """
         Set the mute state to On (True) or Off (False)
         """
         await self._write(f"mute {int(state)}", timeout)
 
-    async def mute_toggle(self, state, timeout: float | None = USE_DEFAULT_TIMEOUT):
+    async def mute_toggle(
+        self, state, timeout: int | float | None = USE_DEFAULT_TIMEOUT
+    ):
         """
         Toggle the mute state.
         """
         await self._write("mute 2", timeout)
 
     async def page_adjust(
-        self, delta: int, timeout: float | None = USE_DEFAULT_TIMEOUT
+        self, delta: int, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Changes the menu page currently on the GUI. `delta` indicates the number of
         pages to change, and may be positive or negative.
         """
         await self._write("bypass 2", timeout)
 
-    async def power_off(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
+    async def power_off(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
         """Power off."""
         await self._write("power off SECURED FHZMCH48FE", timeout)
 
     def power_on(self):
         """Power on."""
         if self.mac is None:
             raise exceptions.NoMacAddressError()
 
         send_magic_packet(self.mac)
 
-    async def preset_load(self, id: int, timeout: float | None = USE_DEFAULT_TIMEOUT):
+    async def preset_load(
+        self, id: int, timeout: int | float | None = USE_DEFAULT_TIMEOUT
+    ):
         """
         Load the preset identified by `id`. Preset `0` is the built-in preset and
         presets >= `1` are user defined presets.
         """
         await self._write("bypass 2", timeout)
 
+    async def quick_optimized_off(
+        self, timeout: int | float | None = USE_DEFAULT_TIMEOUT
+    ):
+        """
+        Turn quick optimized off.
+        """
+        await self.quick_optimized_set(False)
+
+    async def quick_optimized_on(
+        self, timeout: int | float | None = USE_DEFAULT_TIMEOUT
+    ):
+        """
+        Turn quick optimized on.
+        """
+        await self.quick_optimized_set(True)
+
     async def quick_optimized_set(
-        self, state: bool, timeout: float | None = USE_DEFAULT_TIMEOUT
+        self, state: bool, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Set the quick optimized state to On (True) or Off (False)
         """
         await self._write(f"quick_optimized {int(state)}", timeout)
 
     async def quick_optimized_toggle(
-        self, state, timeout: float | None = USE_DEFAULT_TIMEOUT
+        self, state, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Toggle the quick optimized state.
         """
         await self._write("quick_optimized 2", timeout)
 
     async def remapping_mode_set(
-        self, mode: const.RemappingMode, timeout: float | None = USE_DEFAULT_TIMEOUT
+        self,
+        mode: const.RemappingMode,
+        timeout: int | float | None = USE_DEFAULT_TIMEOUT,
     ):
         """
         Set the remapping mode. See `const.RemappingMode` for available options
         and descriptions.
         """
         await self._write(f"remapping_mode {mode.value}", timeout)
 
-    async def source_set(self, id: int, timeout: float | None = USE_DEFAULT_TIMEOUT):
+    async def source_set(
+        self, id: int, timeout: int | float | None = USE_DEFAULT_TIMEOUT
+    ):
         """
         Set the source identified by `id`, where `0` is the first source.
         """
         await self._write(f"profile {id}", timeout)
 
+    async def time_alignment_off(
+        self, timeout: int | float | None = USE_DEFAULT_TIMEOUT
+    ):
+        """
+        Turn time alignment off.
+        """
+        await self.time_alignment_set(False)
+
+    async def time_alignment_on(
+        self, timeout: int | float | None = USE_DEFAULT_TIMEOUT
+    ):
+        """
+        Turn time alignment on.
+        """
+        await self.time_alignment_set(True)
+
     async def time_alignment_set(
-        self, state: bool, timeout: float | None = USE_DEFAULT_TIMEOUT
+        self, state: bool, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Set the time alignment state to On (True) or Off (False)
         """
         await self._write(f"use_time_alignment {int(state)}", timeout)
 
     async def time_alignment_toggle(
-        self, state, timeout: float | None = USE_DEFAULT_TIMEOUT
+        self, state, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Toggle the time alignment state.
         """
         await self._write("use_time_alignment 2", timeout)
 
     async def upmixer_set(
-        self, mode: const.UpmixerMode, timeout: float | None = USE_DEFAULT_TIMEOUT
+        self, mode: const.UpmixerMode, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Set the upmixer mode. See `const.UpmixerMode` for available options
         and descriptions.
         """
         await self._write(f"remapping_mode {mode.value}", timeout)
 
     async def volume_adjust(
-        self, delta: float, timeout: float | None = USE_DEFAULT_TIMEOUT
+        self, delta: int | float, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Adjust the volume by a relative dB value (float).
         """
         await self._write(f"dvolume {delta}", timeout)
 
-    async def volume_down(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
+    async def volume_down(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
         """
         Lower the volume by 0.5 dB
         """
         await self.volume_adjust(-0.5, timeout)
 
-    async def volume_set(self, db: float, timeout: float | None = USE_DEFAULT_TIMEOUT):
+    async def volume_set(
+        self, db: int | float, timeout: int | float | None = USE_DEFAULT_TIMEOUT
+    ):
         """
-        Set the volume to an absolute dB value (float).
+        Set the volume to an absolute dB value.
         """
         await self._write(f"volume {db}", timeout)
 
     async def volume_ramp(
-        self, db: float, duration: int, timeout: float | None = USE_DEFAULT_TIMEOUT
+        self,
+        db: int | float,
+        duration: int,
+        timeout: int | float | None = USE_DEFAULT_TIMEOUT,
     ):
         """
         Ramp the volume to an absolute dB value (float) over a number of milliseconds (int).
         """
         await self._write(f"volume_ramp {db} {duration}", timeout)
 
-    async def volume_up(self, timeout: float | None = USE_DEFAULT_TIMEOUT):
+    async def volume_up(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
         """
         Raise the volume by 0.5 dB
         """
         await self.volume_adjust(0.5, timeout)
 
     # --------------------------
     # Utility
```

