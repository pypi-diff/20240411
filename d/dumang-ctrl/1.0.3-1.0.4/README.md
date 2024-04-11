# Comparing `tmp/dumang_ctrl-1.0.3.tar.gz` & `tmp/dumang_ctrl-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumang_ctrl-1.0.3.tar", max compression
+gzip compressed data, was "dumang_ctrl-1.0.4.tar", max compression
```

## Comparing `dumang_ctrl-1.0.3.tar` & `dumang_ctrl-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2024-03-12 02:51:43.568173 dumang_ctrl-1.0.3/LICENSE
--rw-r--r--   0        0        0     1690 2024-03-23 05:53:52.430096 dumang_ctrl-1.0.3/README.md
--rw-r--r--   0        0        0      269 2024-03-15 21:49:22.464021 dumang_ctrl-1.0.3/dumang_ctrl/__init__.py
--rw-r--r--   0        0        0        0 2024-03-12 02:51:43.568173 dumang_ctrl-1.0.3/dumang_ctrl/dumang/__init__.py
--rw-r--r--   0        0        0      179 2024-03-14 22:10:35.047067 dumang_ctrl-1.0.3/dumang_ctrl/dumang/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    51833 2024-03-23 05:21:18.516887 dumang_ctrl-1.0.3/dumang_ctrl/dumang/__pycache__/common.cpython-311.pyc
--rw-r--r--   0        0        0    36428 2024-03-26 05:08:34.556195 dumang_ctrl-1.0.3/dumang_ctrl/dumang/common.py
--rw-r--r--   0        0        0     6409 2024-03-26 05:08:34.556195 dumang_ctrl-1.0.3/dumang_ctrl/dumang/gui.py
--rw-r--r--   0        0        0        0 2024-03-12 02:51:43.571506 dumang_ctrl-1.0.3/dumang_ctrl/tools/__init__.py
--rw-r--r--   0        0        0      178 2024-03-14 22:10:35.020400 dumang_ctrl-1.0.3/dumang_ctrl/tools/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    12982 2024-03-14 23:08:11.492925 dumang_ctrl-1.0.3/dumang_ctrl/tools/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     8610 2024-03-23 04:36:08.668325 dumang_ctrl-1.0.3/dumang_ctrl/tools/__pycache__/sync.cpython-311.pyc
--rw-r--r--   0        0        0     9902 2024-03-26 05:08:34.556195 dumang_ctrl-1.0.3/dumang_ctrl/tools/config.py
--rw-r--r--   0        0        0     5146 2024-03-26 05:08:34.556195 dumang_ctrl-1.0.3/dumang_ctrl/tools/sync.py
--rw-r--r--   0        0        0     1860 2024-03-26 05:08:06.481562 dumang_ctrl-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2430 1970-01-01 00:00:00.000000 dumang_ctrl-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-12 02:51:43.000000 dumang_ctrl-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1690 2024-03-23 05:53:52.000000 dumang_ctrl-1.0.4/README.md
+-rw-r--r--   0        0        0      269 2024-03-15 21:49:22.000000 dumang_ctrl-1.0.4/dumang_ctrl/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-12 02:51:43.000000 dumang_ctrl-1.0.4/dumang_ctrl/dumang/__init__.py
+-rw-r--r--   0        0        0      179 2024-03-14 22:10:35.000000 dumang_ctrl-1.0.4/dumang_ctrl/dumang/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    51833 2024-03-23 05:21:18.000000 dumang_ctrl-1.0.4/dumang_ctrl/dumang/__pycache__/common.cpython-311.pyc
+-rw-r--r--   0        0        0    36432 2024-03-26 22:21:14.000000 dumang_ctrl-1.0.4/dumang_ctrl/dumang/common.py
+-rw-r--r--   0        0        0     6409 2024-03-26 05:08:34.000000 dumang_ctrl-1.0.4/dumang_ctrl/dumang/gui.py
+-rw-r--r--   0        0        0        0 2024-03-12 02:51:43.000000 dumang_ctrl-1.0.4/dumang_ctrl/tools/__init__.py
+-rw-r--r--   0        0        0      178 2024-03-14 22:10:35.000000 dumang_ctrl-1.0.4/dumang_ctrl/tools/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    12982 2024-03-14 23:08:11.000000 dumang_ctrl-1.0.4/dumang_ctrl/tools/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     8610 2024-03-23 04:36:08.000000 dumang_ctrl-1.0.4/dumang_ctrl/tools/__pycache__/sync.cpython-311.pyc
+-rw-r--r--   0        0        0     9902 2024-03-26 05:08:34.000000 dumang_ctrl-1.0.4/dumang_ctrl/tools/config.py
+-rw-r--r--   0        0        0     4828 2024-03-26 22:19:33.000000 dumang_ctrl-1.0.4/dumang_ctrl/tools/sync.py
+-rw-r--r--   0        0        0     1860 2024-04-11 04:11:32.769369 dumang_ctrl-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2430 1970-01-01 00:00:00.000000 dumang_ctrl-1.0.4/PKG-INFO
```

### Comparing `dumang_ctrl-1.0.3/LICENSE` & `dumang_ctrl-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dumang_ctrl-1.0.3/README.md` & `dumang_ctrl-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dumang_ctrl-1.0.3/dumang_ctrl/dumang/__pycache__/common.cpython-311.pyc` & `dumang_ctrl-1.0.4/dumang_ctrl/dumang/__pycache__/common.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dumang_ctrl-1.0.3/dumang_ctrl/dumang/common.py` & `dumang_ctrl-1.0.4/dumang_ctrl/dumang/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 logger = logging.getLogger(__name__)
 
 BOARD_INFO_REQUEST_CMD = 0x30
 BOARD_INFO_RESPONSE_CMD = 0x31
 DKM_INFO_REQUEST_CMD = 0x06
 DKM_INFO_RESPONSE_CMD = 0x07
 BOARD_SYNC_CMD = 0x46
-LAYER_PRESS_CMD = 0x3E
-LAYER_DEPRESS_CMD = 0x3C
+KEY_UP_CMD = 0x3E
+KEY_DOWN_CMD = 0x3C
 LIGHT_PULSE_CMD = 0x2A
 DKM_REPORT_REQUEST_CMD = 0x04
 DKM_REPORT_RESPONSE_CMD = 0x05
 DKM_ADDED_CMD = 0x18
 DKM_REMOVED_CMD = 0x1A
 DKM_CONFIGURE_CMD = 0x09
 MACRO_REPORT_REQUEST_CMD = 0x42
@@ -713,18 +713,18 @@
 
     @classmethod
     def parse(cls, rawbytes):
         c = None
         if rawbytes:
             cmd = rawbytes[0]
 
-            if cmd == LAYER_PRESS_CMD:
-                c = LayerPressPacket.fromrawbytes(rawbytes)
-            elif cmd == LAYER_DEPRESS_CMD:
-                c = LayerDepressPacket.fromrawbytes(rawbytes)
+            if cmd == KEY_UP_CMD:
+                c = KeyDownPacket.fromrawbytes(rawbytes)
+            elif cmd == KEY_DOWN_CMD:
+                c = KeyUpPacket.fromrawbytes(rawbytes)
             elif cmd == BOARD_INFO_RESPONSE_CMD:
                 c = BoardInfoResponsePacket.fromrawbytes(rawbytes)
             elif cmd == DKM_INFO_RESPONSE_CMD:
                 c = DKMInfoResponsePacket.fromrawbytes(rawbytes)
             elif cmd == DKM_COLOR_RESPONSE_CMD:
                 c = DKMColorResponsePacket.fromrawbytes(rawbytes)
             elif cmd == LIGHT_PULSE_CMD:
@@ -808,36 +808,36 @@
         return cls((rawbytes[3], rawbytes[4]))
 
     def __repr__(self):
         return "{} - CMD:{:02X} Version:{}".format(self.__class__.__name__,
                                                    self.cmd, self.version)
 
 
-class LayerPressPacket(DuMangPacket):
+class KeyDownPacket(DuMangPacket):
 
     def __init__(self, ID, flag, layer_info):
-        super().__init__(LAYER_PRESS_CMD, None)
+        super().__init__(KEY_UP_CMD, None)
         self.ID = ID
         self.flag = flag
         self.layer_info = layer_info
 
     @classmethod
     def fromrawbytes(cls, rawbytes):
         return cls(rawbytes[1], rawbytes[2], rawbytes[3])
 
     def __repr__(self):
         return "{} - CMD:{:02X} ID:{:02X} Flag:{:02X} LayerInfo:{:02X}".format(
             self.__class__.__name__, self.cmd, self.ID, self.flag,
             self.layer_info)
 
 
-class LayerDepressPacket(DuMangPacket):
+class KeyUpPacket(DuMangPacket):
 
     def __init__(self, ID, flag, layer_info):
-        super().__init__(LAYER_DEPRESS_CMD, None)
+        super().__init__(KEY_DOWN_CMD, None)
         self.ID = ID
         self.flag = flag
         self.layer_info = layer_info
 
     @classmethod
     def fromrawbytes(cls, rawbytes):
         return cls(rawbytes[1], rawbytes[2], rawbytes[3])
@@ -846,23 +846,23 @@
         return "{} - CMD:{:02X} ID:{:02X} Flag:{:02X} LayerInfo:{:02X}".format(
             self.__class__.__name__, self.cmd, self.ID, self.flag,
             self.layer_info)
 
 
 class BoardSyncPacket(DuMangPacket):
 
-    def __init__(self, ID, press, layer_info):
+    def __init__(self, ID, layer_active, layer_info):
         super().__init__(BOARD_SYNC_CMD, None)
         self.ID = ID
-        self.press = press
+        self.layer_active = 0x03 if layer_active == True else 0x02
         self.layer_info = layer_info
 
     def encode(self):
         return [
-            self.cmd, 0x01, self.press, 0x00, self.ID, self.layer_info,
+            self.cmd, 0x01, self.layer_active, 0x00, self.ID, self.layer_info,
             self.layer_info & 0x03, 0x00
         ]
 
 
 class LightPulsePacket(DuMangPacket):
 
     def __init__(self, onoff, key):
```

### Comparing `dumang_ctrl-1.0.3/dumang_ctrl/dumang/gui.py` & `dumang_ctrl-1.0.4/dumang_ctrl/dumang/gui.py`

 * *Files identical despite different names*

### Comparing `dumang_ctrl-1.0.3/dumang_ctrl/tools/__pycache__/config.cpython-311.pyc` & `dumang_ctrl-1.0.4/dumang_ctrl/tools/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dumang_ctrl-1.0.3/dumang_ctrl/tools/__pycache__/sync.cpython-311.pyc` & `dumang_ctrl-1.0.4/dumang_ctrl/tools/__pycache__/sync.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `dumang_ctrl-1.0.3/dumang_ctrl/tools/config.py` & `dumang_ctrl-1.0.4/dumang_ctrl/tools/config.py`

 * *Files identical despite different names*

### Comparing `dumang_ctrl-1.0.3/dumang_ctrl/tools/sync.py` & `dumang_ctrl-1.0.4/dumang_ctrl/tools/sync.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,29 +7,26 @@
 from dumang_ctrl.dumang.common import *
 
 logger = logging.getLogger("DuMang Sync")
 logger.setLevel(logging.INFO)
 
 
 def layer_toggle_process(p):
-    press = 0
+    if isinstance(p, KeyUpPacket):
+        layer_active = False
+    elif isinstance(p, KeyDownPacket):
+        layer_active = True
 
-    if p.cmd == LAYER_PRESS_CMD:
-        press = 0x03
-    elif p.cmd == LAYER_DEPRESS_CMD:
-        press = 0x02
-
-    if press > 0:
-        return BoardSyncPacket(p.ID, press, p.layer_info)
+    return BoardSyncPacket(p.ID, layer_active, p.layer_info)
 
 
 def send_response(p, q):
     response = None
 
-    if isinstance(p, (LayerPressPacket, LayerDepressPacket)):
+    if isinstance(p, (KeyDownPacket, KeyUpPacket)):
         response = layer_toggle_process(p)
 
     if response:
         q.put(response)
 
 
 def sync_thread(kbd1, kbd2):
@@ -69,14 +66,34 @@
 
 def init_receive_threads(kbd1, kbd2):
     r1 = Job(target=kbd1.receive_thread, daemon=True)
     r2 = Job(target=kbd2.receive_thread, daemon=True)
     return [r1, r2]
 
 
+def kill_and_join_threads(kbd1, kbd2, threads):
+    if kbd1:
+        kbd1.kill_threads()
+    if kbd2:
+        kbd2.kill_threads()
+
+    for t in threads:
+        t.stop()
+
+    for t in threads:
+        t.join()
+
+    threads = []
+
+    if kbd1:
+        kbd1.close()
+    if kbd2:
+        kbd2.close()
+
+
 def device_init_thread(monitor):
     threads = []
     kbd1 = None
     kbd2 = None
 
     while True:
         status = monitor.get_status()
@@ -103,62 +120,30 @@
                 t.start()
 
         elif status == NOTIFY_STATUS_WAIT:
             logger.debug("Keyboard Disconnected!")
             logger.debug("Stopping sync threads...")
 
             # NOTE: Kill threads and wait for devices to be reconnected.
-            if kbd1:
-                kbd1.kill_threads()
-            if kbd2:
-                kbd2.kill_threads()
-
-            for t in threads:
-                t.stop()
-
-            for t in threads:
-                t.join()
-
-            threads = []
-
-            if kbd1:
-                kbd1.close()
-            if kbd2:
-                kbd2.close()
+            kill_and_join_threads(kbd1, kbd2, threads)
 
             kbd1 = None
             kbd2 = None
         elif status == NOTIFY_STATUS_STOP:
             logger.debug("Stopping sync threads...")
 
             if not (kbd1 or kbd2):
                 logger.info(
                     "Could not find devices. Make sure you've setup udev rules!"
                 )
                 return
 
             # NOTE: Same as the NOTIFY_STATUS_WAIT case above. However,
             # here we want to return from the loop.
-            if kbd1:
-                kbd1.kill_threads()
-            if kbd2:
-                kbd2.kill_threads()
-
-            for t in threads:
-                t.stop()
-
-            for t in threads:
-                t.join()
-
-            threads = []
-
-            if kbd1:
-                kbd1.close()
-            if kbd2:
-                kbd2.close()
+            kill_and_join_threads(kbd1, kbd2, threads)
 
             kbd1 = None
             kbd2 = None
 
             return
```

### Comparing `dumang_ctrl-1.0.3/pyproject.toml` & `dumang_ctrl-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dumang-ctrl"
-version = "1.0.3"
+version = "1.0.4"
 description = "Dumang DK6 Tools"
 authors = ["Miguel A. Arroyo <email@arroyo.me>"]
 repository = "https://github.com/mayanez/dumang-keyboard-ctrl"
 documentation = "https://mayanez.github.io/dumang-keyboard-ctrl/"
 readme = "README.md"
 license = "LICENSE"
 packages = [
```

### Comparing `dumang_ctrl-1.0.3/PKG-INFO` & `dumang_ctrl-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dumang-ctrl
-Version: 1.0.3
+Version: 1.0.4
 Summary: Dumang DK6 Tools
 Home-page: https://github.com/mayanez/dumang-keyboard-ctrl
 License: LICENSE
 Author: Miguel A. Arroyo
 Author-email: email@arroyo.me
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```

