# Comparing `tmp/pybricks-3.5.0b1.tar.gz` & `tmp/pybricks-3.5.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybricks-3.5.0b1.tar", max compression
+gzip compressed data, was "pybricks-3.5.0b2.tar", max compression
```

## Comparing `pybricks-3.5.0b1.tar` & `pybricks-3.5.0b2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      213 2024-03-21 18:18:23.553122 pybricks-3.5.0b1/AUTHORS.md
--rw-r--r--   0        0        0     1082 2024-03-21 18:18:23.553122 pybricks-3.5.0b1/LICENSE
--rw-r--r--   0        0        0     1185 2024-03-21 18:18:23.553122 pybricks-3.5.0b1/README.rst
--rw-r--r--   0        0        0     1360 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/pyproject.toml
--rw-r--r--   0        0        0     4264 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/micropython/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/micropython/py.typed
--rw-r--r--   0        0        0      122 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/__init__.py
--rw-r--r--   0        0        0    45572 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/_common.py
--rw-r--r--   0        0        0     4511 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/ev3dev/_speaker.py
--rw-r--r--   0        0        0     6619 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/ev3devices.py
--rw-r--r--   0        0        0     8556 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/hubs.py
--rw-r--r--   0        0        0    12138 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/iodevices.py
--rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/media/__init__.py
--rw-r--r--   0        0        0    20861 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/media/ev3dev.py
--rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/media/py.typed
--rw-r--r--   0        0        0     6524 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/messaging.py
--rw-r--r--   0        0        0     6671 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/nxtdevices.py
--rw-r--r--   0        0        0    12635 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/parameters.py
--rw-r--r--   0        0        0    13076 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/pupdevices.py
--rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/py.typed
--rw-r--r--   0        0        0    10716 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/robotics.py
--rw-r--r--   0        0        0     7920 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/pybricks/tools.py
--rw-r--r--   0        0        0     1409 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/uerrno/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/uerrno/py.typed
--rw-r--r--   0        0        0     2523 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/uio/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/uio/py.typed
--rw-r--r--   0        0        0     2007 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/ujson/__init__.py
--rw-r--r--   0        0        0     6378 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/umath/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/umath/py.typed
--rw-r--r--   0        0        0     3153 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/urandom/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/urandom/py.typed
--rw-r--r--   0        0        0     4952 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/uselect/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/uselect/py.typed
--rw-r--r--   0        0        0     2280 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/ustruct/__init__.py
--rw-r--r--   0        0        0     1402 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/usys/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 18:18:23.681122 pybricks-3.5.0b1/src/usys/py.typed
--rw-r--r--   0        0        0     2091 1970-01-01 00:00:00.000000 pybricks-3.5.0b1/PKG-INFO
+-rw-r--r--   0        0        0      213 2024-04-05 09:00:22.318943 pybricks-3.5.0b2/AUTHORS.md
+-rw-r--r--   0        0        0     1082 2024-04-05 09:00:22.318943 pybricks-3.5.0b2/LICENSE
+-rw-r--r--   0        0        0     1185 2024-04-05 09:00:22.318943 pybricks-3.5.0b2/README.rst
+-rw-r--r--   0        0        0     1359 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/pyproject.toml
+-rw-r--r--   0        0        0     4264 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/micropython/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/micropython/py.typed
+-rw-r--r--   0        0        0      122 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/pybricks/__init__.py
+-rw-r--r--   0        0        0    45572 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/pybricks/_common.py
+-rw-r--r--   0        0        0     4511 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/pybricks/ev3dev/_speaker.py
+-rw-r--r--   0        0        0     6619 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/pybricks/ev3devices.py
+-rw-r--r--   0        0        0     8556 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/pybricks/hubs.py
+-rw-r--r--   0        0        0    12286 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/pybricks/iodevices.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/pybricks/media/__init__.py
+-rw-r--r--   0        0        0    20861 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/pybricks/media/ev3dev.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/pybricks/media/py.typed
+-rw-r--r--   0        0        0     6524 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/pybricks/messaging.py
+-rw-r--r--   0        0        0     6671 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/pybricks/nxtdevices.py
+-rw-r--r--   0        0        0    12635 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/pybricks/parameters.py
+-rw-r--r--   0        0        0    13203 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/pybricks/pupdevices.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/pybricks/py.typed
+-rw-r--r--   0        0        0    10716 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/pybricks/robotics.py
+-rw-r--r--   0        0        0     8478 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/pybricks/tools.py
+-rw-r--r--   0        0        0     1409 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/uerrno/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/uerrno/py.typed
+-rw-r--r--   0        0        0     2523 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/uio/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:00:22.446945 pybricks-3.5.0b2/src/uio/py.typed
+-rw-r--r--   0        0        0     2007 2024-04-05 09:00:22.450945 pybricks-3.5.0b2/src/ujson/__init__.py
+-rw-r--r--   0        0        0     6378 2024-04-05 09:00:22.450945 pybricks-3.5.0b2/src/umath/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:00:22.450945 pybricks-3.5.0b2/src/umath/py.typed
+-rw-r--r--   0        0        0     3153 2024-04-05 09:00:22.450945 pybricks-3.5.0b2/src/urandom/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:00:22.450945 pybricks-3.5.0b2/src/urandom/py.typed
+-rw-r--r--   0        0        0     4952 2024-04-05 09:00:22.450945 pybricks-3.5.0b2/src/uselect/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:00:22.450945 pybricks-3.5.0b2/src/uselect/py.typed
+-rw-r--r--   0        0        0     2280 2024-04-05 09:00:22.450945 pybricks-3.5.0b2/src/ustruct/__init__.py
+-rw-r--r--   0        0        0     1402 2024-04-05 09:00:22.450945 pybricks-3.5.0b2/src/usys/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:00:22.450945 pybricks-3.5.0b2/src/usys/py.typed
+-rw-r--r--   0        0        0     2091 1970-01-01 00:00:00.000000 pybricks-3.5.0b2/PKG-INFO
```

### Comparing `pybricks-3.5.0b1/LICENSE` & `pybricks-3.5.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/README.rst` & `pybricks-3.5.0b2/README.rst`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/pyproject.toml` & `pybricks-3.5.0b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybricks"
-version = "v3.5.0b1"
+version = "3.5.0b2"
 description = "Documentation and user-API stubs for Pybricks MicroPython"
 authors = ["The Pybricks Authors <team@pybricks.com>"]
 maintainers = ["Laurens Valk <laurens@pybricks.com>", "David Lechner <david@pybricks.com>" ]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://pybricks.com"
 repository = "https://github.com/pybricks/pybricks-api"
```

### Comparing `pybricks-3.5.0b1/src/micropython/__init__.py` & `pybricks-3.5.0b2/src/micropython/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/src/pybricks/_common.py` & `pybricks-3.5.0b2/src/pybricks/_common.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/src/pybricks/ev3dev/_speaker.py` & `pybricks-3.5.0b2/src/pybricks/ev3dev/_speaker.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/src/pybricks/ev3devices.py` & `pybricks-3.5.0b2/src/pybricks/ev3devices.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/src/pybricks/hubs.py` & `pybricks-3.5.0b2/src/pybricks/hubs.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/src/pybricks/iodevices.py` & `pybricks-3.5.0b2/src/pybricks/iodevices.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
 
 
         .. _`hub type identifier`:
             https://github.com/pybricks/technical-info/blob/master/assigned-numbers.md#hub-type-ids
         """
 
     @overload
-    def name(self, name: str) -> None: ...
+    def name(self, name: str) -> MaybeAwaitable: ...
 
     @overload
     def name(self) -> str: ...
 
     def name(self, *args):
         """name(name)
         name() -> str
@@ -332,14 +332,20 @@
         If a message has not been received since the last read, the method will
         block until a message is received.
 
         Returns:
             The raw binary message.
         """
 
+    def disconnect(self) -> MaybeAwaitable:
+        """disconnect()
+
+        Disconnects the remote LWP3Device from the hub.
+        """
+
 
 class XboxController:
     """Use the Microsoft® Xbox® controller as a sensor in your projects to
     control them remotely.
 
     The hub will scan for the controller and connect to it. It will disconnect
     when the program ends.
```

### Comparing `pybricks-3.5.0b1/src/pybricks/media/ev3dev.py` & `pybricks-3.5.0b2/src/pybricks/media/ev3dev.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/src/pybricks/messaging.py` & `pybricks-3.5.0b2/src/pybricks/messaging.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/src/pybricks/nxtdevices.py` & `pybricks-3.5.0b2/src/pybricks/nxtdevices.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/src/pybricks/parameters.py` & `pybricks-3.5.0b2/src/pybricks/parameters.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/src/pybricks/pupdevices.py` & `pybricks-3.5.0b2/src/pybricks/pupdevices.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,20 @@
         Sets or gets the Bluetooth name of the remote.
 
         Arguments:
             name (str): New Bluetooth name of the remote. If no name is given,
                 this method returns the current name.
         """
 
+    def disconnect(self) -> MaybeAwaitable:
+        """disconnect()
+
+        Disconnects the remote from the hub.
+        """
+
 
 class TiltSensor:
     """LEGO® Powered Up Tilt Sensor."""
 
     def __init__(self, port: Port):
         """TiltSensor(port)
```

### Comparing `pybricks-3.5.0b1/src/pybricks/robotics.py` & `pybricks-3.5.0b2/src/pybricks/robotics.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/src/pybricks/tools.py` & `pybricks-3.5.0b2/src/pybricks/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -207,22 +207,31 @@
         b (Matrix): A three-dimensional vector.
 
     Returns:
         The cross product, also a three-dimensional vector.
     """
 
 
-def read_input_byte() -> Optional[int]:
+def read_input_byte(last: bool = False, chr: bool = False) -> Optional[int | str]:
     """
-    read_input_byte() -> int | None
+    read_input_byte() -> int | str | None
 
-    Reads one byte from standard input without blocking.
+    Reads one byte from standard input without blocking and removes it from the
+    input buffer.
+
+    Arguments:
+        last (bool): Choose ``True`` to read the last (most recent) byte in the buffer and discard the rest.
+                     Choose ``False`` to read only the first (oldest) byte.
+        chr (bool): Choose ``True`` to convert the result to a one-character string.
 
     Returns:
-        The numeric value of the byte read or ``None`` if no data is available.
+        The byte that was read, as a numeric value (``0`` to ``255``) or
+        string (e.g. ``"B"``). Returns ``None`` if no data is available. If
+        ``chr=True``, it also return ``None`` if the byte that was read is not
+        printable as a character.
     """
 
 
 def hub_menu(*symbols: int | str) -> int | str:
     """
     hub_menu(symbol1, symbol2, ...) -> int | str
```

### Comparing `pybricks-3.5.0b1/src/uerrno/__init__.py` & `pybricks-3.5.0b2/src/uerrno/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/src/uio/__init__.py` & `pybricks-3.5.0b2/src/uio/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/src/ujson/__init__.py` & `pybricks-3.5.0b2/src/ujson/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/src/umath/__init__.py` & `pybricks-3.5.0b2/src/umath/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/src/urandom/__init__.py` & `pybricks-3.5.0b2/src/urandom/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/src/uselect/__init__.py` & `pybricks-3.5.0b2/src/uselect/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/src/ustruct/__init__.py` & `pybricks-3.5.0b2/src/ustruct/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/src/usys/__init__.py` & `pybricks-3.5.0b2/src/usys/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks-3.5.0b1/PKG-INFO` & `pybricks-3.5.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybricks
-Version: 3.5.0b1
+Version: 3.5.0b2
 Summary: Documentation and user-API stubs for Pybricks MicroPython
 Home-page: https://pybricks.com
 License: MIT
 Author: The Pybricks Authors
 Author-email: team@pybricks.com
 Maintainer: Laurens Valk
 Maintainer-email: laurens@pybricks.com
```

