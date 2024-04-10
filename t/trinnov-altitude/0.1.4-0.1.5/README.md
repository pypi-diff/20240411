# Comparing `tmp/trinnov-altitude-0.1.4.tar.gz` & `tmp/trinnov-altitude-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trinnov-altitude-0.1.4.tar", last modified: Wed Apr 10 00:58:01 2024, max compression
+gzip compressed data, was "trinnov-altitude-0.1.5.tar", last modified: Wed Apr 10 16:16:24 2024, max compression
```

## Comparing `trinnov-altitude-0.1.4.tar` & `trinnov-altitude-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:58:01.872435 trinnov-altitude-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-10 00:58:01.872435 trinnov-altitude-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-10 00:58:01.872435 trinnov-altitude-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:58:01.868435 trinnov-altitude-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/tests/test_trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:58:01.872435 trinnov-altitude-0.1.4/trinnov_altitude/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/trinnov_altitude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/trinnov_altitude/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/trinnov_altitude/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/trinnov_altitude/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/trinnov_altitude/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-04-10 00:57:54.000000 trinnov-altitude-0.1.4/trinnov_altitude/trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:58:01.872435 trinnov-altitude-0.1.4/trinnov_altitude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-10 00:58:01.000000 trinnov-altitude-0.1.4/trinnov_altitude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-10 00:58:01.000000 trinnov-altitude-0.1.4/trinnov_altitude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 00:58:01.000000 trinnov-altitude-0.1.4/trinnov_altitude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 00:58:01.000000 trinnov-altitude-0.1.4/trinnov_altitude.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:16:24.148434 trinnov-altitude-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-10 16:16:24.148434 trinnov-altitude-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-10 16:16:24.148434 trinnov-altitude-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:16:24.144434 trinnov-altitude-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/tests/test_trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:16:24.144434 trinnov-altitude-0.1.5/trinnov_altitude/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/trinnov_altitude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/trinnov_altitude/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/trinnov_altitude/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/trinnov_altitude/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/trinnov_altitude/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-04-10 16:16:17.000000 trinnov-altitude-0.1.5/trinnov_altitude/trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:16:24.148434 trinnov-altitude-0.1.5/trinnov_altitude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-10 16:16:24.000000 trinnov-altitude-0.1.5/trinnov_altitude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-10 16:16:24.000000 trinnov-altitude-0.1.5/trinnov_altitude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:16:24.000000 trinnov-altitude-0.1.5/trinnov_altitude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 16:16:24.000000 trinnov-altitude-0.1.5/trinnov_altitude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 16:16:24.000000 trinnov-altitude-0.1.5/trinnov_altitude.egg-info/top_level.txt
```

### Comparing `trinnov-altitude-0.1.4/LICENSE` & `trinnov-altitude-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.4/PKG-INFO` & `trinnov-altitude-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 0.1.4
+Version: 0.1.5
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Home Automation
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: wakeonlan>=3.1
 
 # Trinnov Altitude Python Library
 
 A Python library for interacting with the [Trinnov Altitude processor](https://www.trinnov.com/en/products/altitude32/) via the
 [TCP/IP automation protocol](docs/Alititude%20Protocol.pdf) provided by the Trinnov Altitude.
 
 ## Overview
```

### Comparing `trinnov-altitude-0.1.4/README.md` & `trinnov-altitude-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.4/setup.cfg` & `trinnov-altitude-0.1.5/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -12,11 +12,16 @@
 	Intended Audience :: Developers
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Topic :: Software Development :: Libraries
 	Topic :: Home Automation
 
+[options]
+packages = find:
+install_requires = 
+	wakeonlan>=3.1
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `trinnov-altitude-0.1.4/tests/test_trinnov_altitude.py` & `trinnov-altitude-0.1.5/tests/test_trinnov_altitude.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,42 @@
 import asyncio
 import pytest
 import pytest_asyncio
 
-from trinnov_altitude.exceptions import ConnectionFailedError, ConnectionTimeoutError
+from trinnov_altitude.exceptions import (
+    ConnectionFailedError,
+    ConnectionTimeoutError,
+    InvalidMacAddressOUIError,
+    MalformedMacAddressError,
+)
 from trinnov_altitude.messages import Message, OKMessage
 from trinnov_altitude.mocks import MockTrinnovAltitudeServer
 from trinnov_altitude.trinnov_altitude import TrinnovAltitude
 
 
 @pytest_asyncio.fixture
 async def mock_server():
     server = MockTrinnovAltitudeServer()
     await server.start_server()
     yield server
     await server.stop_server()
 
 
 @pytest.mark.asyncio
+async def test_validate_mac():
+    with pytest.raises(MalformedMacAddressError):
+        TrinnovAltitude.validate_mac("malformed")
+
+    with pytest.raises(InvalidMacAddressOUIError):
+        TrinnovAltitude.validate_mac("c9:7f:32:2b:ea:f4")
+
+    assert TrinnovAltitude.validate_mac("c8:7f:54:7a:eb:c2")
+
+
+@pytest.mark.asyncio
 async def test_connect_failed(mock_server):
     client = TrinnovAltitude(host="invalid")
     with pytest.raises(ConnectionFailedError):
         await client.connect()
 
 
 @pytest.mark.asyncio
```

### Comparing `trinnov-altitude-0.1.4/trinnov_altitude/const.py` & `trinnov-altitude-0.1.5/trinnov_altitude/const.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.4/trinnov_altitude/messages.py` & `trinnov-altitude-0.1.5/trinnov_altitude/messages.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.4/trinnov_altitude/mocks.py` & `trinnov-altitude-0.1.5/trinnov_altitude/mocks.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.4/trinnov_altitude/trinnov_altitude.py` & `trinnov-altitude-0.1.5/trinnov_altitude/trinnov_altitude.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,67 @@
 """
 Implements the Trinnov Altitude processor automation protocol over TCP/IP
 """
 
 import asyncio
 from collections.abc import Callable
 import logging
+import re
+from wakeonlan import send_magic_packet
+
 from trinnov_altitude import const, exceptions, messages
 
 
 class TrinnovAltitude:
     """
     Trinnov Altitude
 
     A class for interfacing with the Trinnov Altitude processor via the TCP/IP protocol.
     """
 
     DEFAULT_CLIENT_ID = "py-trinnov-altitude"
     DEFAULT_PORT = 44100
     DEFAULT_TIMEOUT = 2.0
     ENCODING = "ascii"
+    VALID_OUIS = [
+        "c8:7f:54",  # ASUSTek OUI (components inside Altitudes)
+        "64:98:9e",  # Trinnov's OUI
+    ]
 
     # Use a sentinel value to signal that the DEFAULT_TIMEOUT should be used.
     # This allows users to pass None and disable the timeout to wait indefinitely.
     USE_DEFAULT_TIMEOUT = -1.0
 
+    @classmethod
+    def validate_mac(cls, mac_address):
+        """
+        Validate, to the best of our abilities, that the Mac address is a
+        valid Trinnov Altitude Mac address.
+        ."""
+
+        normalized_mac_address = mac_address.lower()
+
+        # Verify the format
+        pattern = re.compile(r"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$")
+        if pattern.match(normalized_mac_address) is None:
+            raise exceptions.MalformedMacAddressError(mac_address)
+
+        # Verify it starts with Trinnov associates OUIs
+        mac_oui = normalized_mac_address[:8]
+        if not any(mac_oui == oui for oui in cls.VALID_OUIS):
+            raise exceptions.InvalidMacAddressOUIError(mac_oui, cls.VALID_OUIS)
+
+        return True
+
+    @classmethod
+    def wake_on_lan(cls, mac_address):
+        """Wake the processor via WoL."""
+        cls.validate_mac(mac_address)
+        send_magic_packet(mac_address)
+
     def __init__(
         self,
         host: str,
         port: int = DEFAULT_PORT,
         client_id: str = DEFAULT_CLIENT_ID,
         timeout: float = DEFAULT_TIMEOUT,
         logger: logging.Logger = logging.getLogger(__name__),
```

### Comparing `trinnov-altitude-0.1.4/trinnov_altitude.egg-info/PKG-INFO` & `trinnov-altitude-0.1.5/trinnov_altitude.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 0.1.4
+Version: 0.1.5
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Home Automation
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: wakeonlan>=3.1
 
 # Trinnov Altitude Python Library
 
 A Python library for interacting with the [Trinnov Altitude processor](https://www.trinnov.com/en/products/altitude32/) via the
 [TCP/IP automation protocol](docs/Alititude%20Protocol.pdf) provided by the Trinnov Altitude.
 
 ## Overview
```

