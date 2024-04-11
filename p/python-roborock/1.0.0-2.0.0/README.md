# Comparing `tmp/python_roborock-1.0.0.tar.gz` & `tmp/python_roborock-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-1.0.0.tar", max compression
+gzip compressed data, was "python_roborock-2.0.0.tar", max compression
```

## Comparing `python_roborock-1.0.0.tar` & `python_roborock-2.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2024-04-09 15:49:07.233429 python_roborock-1.0.0/LICENSE
--rw-r--r--   0        0        0     1220 2024-04-09 15:49:07.233429 python_roborock-1.0.0/README.md
--rw-r--r--   0        0        0     1677 2024-04-09 15:49:08.057433 python_roborock-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      165 2024-04-09 15:49:07.233429 python_roborock-1.0.0/roborock/__init__.py
--rw-r--r--   0        0        0     4392 2024-04-09 15:49:07.233429 python_roborock-1.0.0/roborock/api.py
--rw-r--r--   0        0        0     6826 2024-04-09 15:49:07.233429 python_roborock-1.0.0/roborock/cli.py
--rw-r--r--   0        0        0     7144 2024-04-09 15:49:07.233429 python_roborock-1.0.0/roborock/cloud_api.py
--rw-r--r--   0        0        0    11343 2024-04-09 15:49:07.233429 python_roborock-1.0.0/roborock/code_mappings.py
--rw-r--r--   0        0        0     7912 2024-04-09 15:49:07.233429 python_roborock-1.0.0/roborock/command_cache.py
--rw-r--r--   0        0        0     2339 2024-04-09 15:49:07.233429 python_roborock-1.0.0/roborock/const.py
--rw-r--r--   0        0        0    27590 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/containers.py
--rw-r--r--   0        0        0     1962 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/exceptions.py
--rw-r--r--   0        0        0     4367 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/local_api.py
--rw-r--r--   0        0        0    12331 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/protocol.py
--rw-r--r--   0        0        0        0 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/py.typed
--rw-r--r--   0        0        0      834 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/roborock_future.py
--rw-r--r--   0        0        0     4381 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/roborock_message.py
--rw-r--r--   0        0        0    21816 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/roborock_typing.py
--rw-r--r--   0        0        0     3465 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/util.py
--rw-r--r--   0        0        0      183 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/version_1_apis/__init__.py
--rw-r--r--   0        0        0    19949 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/version_1_apis/roborock_client_v1.py
--rw-r--r--   0        0        0     3477 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/version_1_apis/roborock_local_client_v1.py
--rw-r--r--   0        0        0     3342 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/version_1_apis/roborock_mqtt_client_v1.py
--rw-r--r--   0        0        0      111 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/version_a01_apis/__init__.py
--rw-r--r--   0        0        0     5046 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/version_a01_apis/roborock_client_a01.py
--rw-r--r--   0        0        0     2482 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/version_a01_apis/roborock_mqtt_client_a01.py
--rw-r--r--   0        0        0    13040 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/web_api.py
--rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 python_roborock-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-11 14:48:23.714890 python_roborock-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1220 2024-04-11 14:48:23.714890 python_roborock-2.0.0/README.md
+-rw-r--r--   0        0        0     1677 2024-04-11 14:48:24.430890 python_roborock-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      165 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/__init__.py
+-rw-r--r--   0        0        0     4107 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/api.py
+-rw-r--r--   0        0        0     6826 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/cli.py
+-rw-r--r--   0        0        0     7144 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/cloud_api.py
+-rw-r--r--   0        0        0    13571 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/code_mappings.py
+-rw-r--r--   0        0        0     7912 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/command_cache.py
+-rw-r--r--   0        0        0     2339 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/const.py
+-rw-r--r--   0        0        0    27590 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/containers.py
+-rw-r--r--   0        0        0     1962 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/exceptions.py
+-rw-r--r--   0        0        0     4367 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/local_api.py
+-rw-r--r--   0        0        0    12315 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/protocol.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/py.typed
+-rw-r--r--   0        0        0      834 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/roborock_future.py
+-rw-r--r--   0        0        0     5464 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/roborock_message.py
+-rw-r--r--   0        0        0    21816 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/roborock_typing.py
+-rw-r--r--   0        0        0     3465 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/util.py
+-rw-r--r--   0        0        0      183 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/version_1_apis/__init__.py
+-rw-r--r--   0        0        0    19949 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/version_1_apis/roborock_client_v1.py
+-rw-r--r--   0        0        0     3477 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/version_1_apis/roborock_local_client_v1.py
+-rw-r--r--   0        0        0     3342 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/version_1_apis/roborock_mqtt_client_v1.py
+-rw-r--r--   0        0        0      111 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/version_a01_apis/__init__.py
+-rw-r--r--   0        0        0     7342 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/version_a01_apis/roborock_client_a01.py
+-rw-r--r--   0        0        0     2961 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/version_a01_apis/roborock_mqtt_client_a01.py
+-rw-r--r--   0        0        0    13040 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/web_api.py
+-rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 python_roborock-2.0.0/PKG-INFO
```

### Comparing `python_roborock-1.0.0/LICENSE` & `python_roborock-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-1.0.0/README.md` & `python_roborock-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-1.0.0/pyproject.toml` & `python_roborock-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "1.0.0"
+version = "2.0.0"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 documentation = "https://python-roborock.readthedocs.io/"
 classifiers = [
```

### Comparing `python_roborock-1.0.0/roborock/api.py` & `python_roborock-2.0.0/roborock/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 import secrets
 import time
 from collections.abc import Callable, Coroutine
 from typing import Any
 
 from .containers import (
     DeviceData,
-    ModelStatus,
-    S7MaxVStatus,
-    Status,
 )
 from .exceptions import (
     RoborockTimeout,
     UnknownMethodError,
     VacuumError,
 )
 from .roborock_future import RoborockFuture
@@ -44,24 +41,18 @@
         self.keep_alive = KEEPALIVE
         self._diagnostic_data: dict[str, dict[str, Any]] = {
             "misc_info": {"Nonce": base64.b64encode(self._nonce).decode("utf-8")}
         }
         self._logger = RoborockLoggerAdapter(device_info.device.name, _LOGGER)
         self.is_available: bool = True
         self.queue_timeout = queue_timeout
-        self._status_type: type[Status] = ModelStatus.get(self.device_info.model, S7MaxVStatus)
 
     def __del__(self) -> None:
         self.release()
 
-    @property
-    def status_type(self) -> type[Status]:
-        """Gets the status type for this device"""
-        return self._status_type
-
     def release(self):
         self.sync_disconnect()
 
     async def async_release(self):
         await self.async_disconnect()
 
     @property
```

### Comparing `python_roborock-1.0.0/roborock/cli.py` & `python_roborock-2.0.0/roborock/cli.py`

 * *Files identical despite different names*

### Comparing `python_roborock-1.0.0/roborock/cloud_api.py` & `python_roborock-2.0.0/roborock/cloud_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-1.0.0/roborock/code_mappings.py` & `python_roborock-2.0.0/roborock/code_mappings.py`

 * *Files 21% similar despite different names*

```diff
@@ -446,7 +446,142 @@
         20007  # Battery temperature protection. Wait for the temperature to return to a normal range.
     )
     battery_temperature_protection_2 = 20008
     power_adapter_error = 20009  # Check if the power adapter is working properly.
     dirty_charging_contacts = 10007  # Disconnection between the device and dock. Wipe charging contacts.
     low_battery = 20017  # Low battery level. Charge before starting self-cleaning.
     battery_under_10 = 20018  # Charge until the battery level exceeds 10% before manually starting self-cleaning.
+
+
+class ZeoMode(RoborockEnum):
+    wash = 1
+    wash_and_dry = 2
+    dry = 3
+
+
+class ZeoState(RoborockEnum):
+    standby = 1
+    weighing = 2
+    soaking = 3
+    washing = 4
+    rinsing = 5
+    spinning = 6
+    drying = 7
+    cooling = 8
+    under_delay_start = 9
+    done = 10
+
+
+class ZeoProgram(RoborockEnum):
+    standard = 1
+    quick = 2
+    sanitize = 3
+    wool = 4
+    air_refresh = 5
+    custom = 6
+    bedding = 7
+    down = 8
+    silk = 9
+    rinse_and_spin = 10
+    spin = 11
+    down_clean = 12
+    baby_care = 13
+    anti_allergen = 14
+    sportswear = 15
+    night = 16
+    new_clothes = 17
+    shirts = 18
+    synthetics = 19
+    underwear = 20
+    gentle = 21
+    intensive = 22
+    cotton_linen = 23
+    season = 24
+    warming = 25
+    bra = 26
+    panties = 27
+    boiling_wash = 28
+    socks = 30
+    towels = 31
+    anti_mite = 32
+    exo_40_60 = 33
+    twenty_c = 34
+    t_shirts = 35
+    stain_removal = 36
+
+
+class ZeoSoak(RoborockEnum):
+    normal = 0
+    low = 1
+    medium = 2
+    high = 3
+    max = 4
+
+
+class ZeoTemperature(RoborockEnum):
+    normal = 1
+    low = 2
+    medium = 3
+    high = 4
+    max = 5
+    twenty_c = 6
+
+
+class ZeoRinse(RoborockEnum):
+    none = 0
+    min = 1
+    low = 2
+    mid = 3
+    high = 4
+    max = 5
+
+
+class ZeoSpin(RoborockEnum):
+    none = 1
+    very_low = 2
+    low = 3
+    mid = 4
+    high = 5
+    very_high = 6
+    max = 7
+
+
+class ZeoDryingMode(RoborockEnum):
+    none = 0
+    quick = 1
+    iron = 2
+    store = 3
+
+
+class ZeoDetergentType(RoborockEnum):
+    empty = 0
+    low = 1
+    medium = 2
+    high = 3
+
+
+class ZeoSoftenerType(RoborockEnum):
+    empty = 0
+    low = 1
+    medium = 2
+    high = 3
+
+
+class ZeoError(RoborockEnum):
+    none = 0
+    refill_error = 1
+    drain_error = 2
+    door_lock_error = 3
+    water_level_error = 4
+    inverter_error = 5
+    heating_error = 6
+    temperature_error = 7
+    communication_error = 10
+    drying_error = 11
+    drying_error_e_12 = 12
+    drying_error_e_13 = 13
+    drying_error_e_14 = 14
+    drying_error_e_15 = 15
+    drying_error_e_16 = 16
+    drying_error_water_flow = 17  # Check for normal water flow
+    drying_error_restart = 18  # Restart the washer and try again
+    spin_error = 19  # re-arrange clothes
```

### Comparing `python_roborock-1.0.0/roborock/command_cache.py` & `python_roborock-2.0.0/roborock/command_cache.py`

 * *Files identical despite different names*

### Comparing `python_roborock-1.0.0/roborock/const.py` & `python_roborock-2.0.0/roborock/const.py`

 * *Files identical despite different names*

### Comparing `python_roborock-1.0.0/roborock/containers.py` & `python_roborock-2.0.0/roborock/containers.py`

 * *Files identical despite different names*

### Comparing `python_roborock-1.0.0/roborock/exceptions.py` & `python_roborock-2.0.0/roborock/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_roborock-1.0.0/roborock/local_api.py` & `python_roborock-2.0.0/roborock/local_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-1.0.0/roborock/protocol.py` & `python_roborock-2.0.0/roborock/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
 from roborock import BroadcastMessage, RoborockException
 from roborock.roborock_message import RoborockMessage
 
 _LOGGER = logging.getLogger(__name__)
 SALT = b"TXdfu$jyZ#TZHsg4"
 A01_HASH = "726f626f726f636b2d67a6d6da"
-A01_AES_DECIPHER = "ELSYN0wTI4AUm7C4"
 BROADCAST_TOKEN = b"qWKYcdQWrbm9hPqe"
 AP_CONFIG = 1
 SOCK_DISCOVERY = 2
 
 
 def md5hex(message: str) -> str:
     md5 = hashlib.md5()
@@ -204,26 +203,26 @@
     def _encode(self, obj, context, _):
         """Encrypt the given payload with the token stored in the context.
 
         :param obj: JSON object to encrypt
         """
         if context.version == b"A01":
             iv = md5hex(format(context.random, "08x") + A01_HASH)[8:24]
-            decipher = AES.new(bytes(A01_AES_DECIPHER, "utf-8"), AES.MODE_CBC, bytes(iv, "utf-8"))
+            decipher = AES.new(bytes(context.search("local_key"), "utf-8"), AES.MODE_CBC, bytes(iv, "utf-8"))
             f = decipher.encrypt(obj)
             return f
         token = self.token_func(context)
         encrypted = Utils.encrypt_ecb(obj, token)
         return encrypted
 
     def _decode(self, obj, context, _):
         """Decrypts the given payload with the token stored in the context."""
         if context.version == b"A01":
             iv = md5hex(format(context.random, "08x") + A01_HASH)[8:24]
-            decipher = AES.new(bytes(A01_AES_DECIPHER, "utf-8"), AES.MODE_CBC, bytes(iv, "utf-8"))
+            decipher = AES.new(bytes(context.search("local_key"), "utf-8"), AES.MODE_CBC, bytes(iv, "utf-8"))
             f = decipher.decrypt(obj)
             return f
         token = self.token_func(context)
         decrypted = Utils.decrypt_ecb(obj, token)
         return decrypted
```

### Comparing `python_roborock-1.0.0/roborock/roborock_future.py` & `python_roborock-2.0.0/roborock/roborock_future.py`

 * *Files identical despite different names*

### Comparing `python_roborock-1.0.0/roborock/roborock_message.py` & `python_roborock-2.0.0/roborock/roborock_message.py`

 * *Files 20% similar despite different names*

```diff
@@ -83,14 +83,56 @@
     PRODUCT_INFO = 10005
     PRIVACY_INFO = 10006
     OTA_NFO = 10007
     RPC_REQUEST = 10101
     RPC_RESPONSE = 10102
 
 
+class RoborockZeoProtocol(RoborockEnum):
+    START = 200  # rw
+    PAUSE = 201  # rw
+    SHUTDOWN = 202  # rw
+    STATE = 203  # ro
+    MODE = 204  # rw
+    PROGRAM = 205  # rw
+    CHILD_LOCK = 206  # rw
+    TEMP = 207  # rw
+    RINSE_TIMES = 208  # rw
+    SPIN_LEVEL = 209  # rw
+    DRYING_MODE = 210  # rw
+    DETERGENT_SET = 211  # rw
+    SOFTENER_SET = 212  # rw
+    DETERGENT_TYPE = 213  # rw
+    SOFTENER_TYPE = 214  # rw
+    COUNTDOWN = 217  # rw
+    WASHING_LEFT = 218  # ro
+    DOORLOCK_STATE = 219  # ro
+    ERROR = 220  # ro
+    CUSTOM_PARAM_SAVE = 221  # rw
+    CUSTOM_PARAM_GET = 222  # ro
+    SOUND_SET = 223  # rw
+    TIMES_AFTER_CLEAN = 224  # ro
+    DEFAULT_SETTING = 225  # rw
+    DETERGENT_EMPTY = 226  # ro
+    SOFTENER_EMPTY = 227  # ro
+    LIGHT_SETTING = 229  # rw
+    DETERGENT_VOLUME = 230  # rw
+    SOFTENER_VOLUME = 231  # rw
+    APP_AUTHORIZATION = 232  # rw
+    ID_QUERY = 10000
+    F_C = 10001
+    SND_STATE = 10004
+    PRODUCT_INFO = 10005
+    PRIVACY_INFO = 10006
+    OTA_NFO = 10007
+    WASHING_LOG = 10008
+    RPC_REQ = 10101
+    RPC_RESp = 10102
+
+
 ROBOROCK_DATA_STATUS_PROTOCOL = [
     RoborockDataProtocol.ERROR_CODE,
     RoborockDataProtocol.STATE,
     RoborockDataProtocol.BATTERY,
     RoborockDataProtocol.FAN_POWER,
     RoborockDataProtocol.WATER_BOX_MODE,
     RoborockDataProtocol.CHARGE_STATUS,
```

### Comparing `python_roborock-1.0.0/roborock/roborock_typing.py` & `python_roborock-2.0.0/roborock/roborock_typing.py`

 * *Files identical despite different names*

### Comparing `python_roborock-1.0.0/roborock/util.py` & `python_roborock-2.0.0/roborock/util.py`

 * *Files identical despite different names*

### Comparing `python_roborock-1.0.0/roborock/version_1_apis/roborock_client_v1.py` & `python_roborock-2.0.0/roborock/version_1_apis/roborock_client_v1.py`

 * *Files identical despite different names*

### Comparing `python_roborock-1.0.0/roborock/version_1_apis/roborock_local_client_v1.py` & `python_roborock-2.0.0/roborock/version_1_apis/roborock_local_client_v1.py`

 * *Files identical despite different names*

### Comparing `python_roborock-1.0.0/roborock/version_1_apis/roborock_mqtt_client_v1.py` & `python_roborock-2.0.0/roborock/version_1_apis/roborock_mqtt_client_v1.py`

 * *Files identical despite different names*

### Comparing `python_roborock-1.0.0/roborock/version_a01_apis/roborock_mqtt_client_a01.py` & `python_roborock-2.0.0/roborock/version_a01_apis/roborock_mqtt_client_a01.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,67 @@
 import asyncio
 import base64
 import json
+import typing
 
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad, unpad
 
 from roborock.cloud_api import RoborockMqttClient
-from roborock.containers import DeviceData, UserData
+from roborock.containers import DeviceData, RoborockCategory, UserData
 from roborock.exceptions import RoborockException
 from roborock.protocol import MessageParser, Utils
-from roborock.roborock_message import RoborockDyadDataProtocol, RoborockMessage, RoborockMessageProtocol
+from roborock.roborock_message import (
+    RoborockDyadDataProtocol,
+    RoborockMessage,
+    RoborockMessageProtocol,
+    RoborockZeoProtocol,
+)
 
 from .roborock_client_a01 import RoborockClientA01
 
 
 class RoborockMqttClientA01(RoborockMqttClient, RoborockClientA01):
-    def __init__(self, user_data: UserData, device_info: DeviceData, queue_timeout: int = 10) -> None:
+    def __init__(
+        self, user_data: UserData, device_info: DeviceData, category: RoborockCategory, queue_timeout: int = 10
+    ) -> None:
         rriot = user_data.rriot
         if rriot is None:
             raise RoborockException("Got no rriot data from user_data")
         endpoint = base64.b64encode(Utils.md5(rriot.k.encode())[8:14]).decode()
 
         RoborockMqttClient.__init__(self, user_data, device_info, queue_timeout)
-        RoborockClientA01.__init__(self, endpoint, device_info)
+        RoborockClientA01.__init__(self, endpoint, device_info, category, queue_timeout)
 
     async def send_message(self, roborock_message: RoborockMessage):
         await self.validate_connection()
         response_protocol = RoborockMessageProtocol.RPC_RESPONSE
 
         local_key = self.device_info.device.local_key
         m = MessageParser.build(roborock_message, local_key, prefixed=False)
         # self._logger.debug(f"id={request_id} Requesting method {method} with {params}")
         payload = json.loads(unpad(roborock_message.payload, AES.block_size))
         futures = []
         if "10000" in payload["dps"]:
             for dps in json.loads(payload["dps"]["10000"]):
                 futures.append(asyncio.ensure_future(self._async_response(dps, response_protocol)))
         self._send_msg_raw(m)
-        responses = await asyncio.gather(*futures)
-        dps_responses = {}
+        responses = await asyncio.gather(*futures, return_exceptions=True)
+        dps_responses: dict[int, typing.Any] = {}
         if "10000" in payload["dps"]:
             for i, dps in enumerate(json.loads(payload["dps"]["10000"])):
-                dps_responses[dps] = responses[i][0]
+                response = responses[i]
+                if isinstance(response, BaseException):
+                    self._logger.warning("Timed out get req for %s after %s s", dps, self.queue_timeout)
+                    dps_responses[dps] = None
+                else:
+                    dps_responses[dps] = response[0]
         return dps_responses
 
-    async def update_values(self, dyad_data_protocols: list[RoborockDyadDataProtocol]):
+    async def update_values(self, dyad_data_protocols: list[RoborockDyadDataProtocol | RoborockZeoProtocol]):
         payload = {"dps": {RoborockDyadDataProtocol.ID_QUERY: str([int(protocol) for protocol in dyad_data_protocols])}}
         return await self.send_message(
             RoborockMessage(
                 protocol=RoborockMessageProtocol.RPC_REQUEST,
                 version=b"A01",
                 payload=pad(json.dumps(payload).encode("utf-8"), AES.block_size),
             )
```

### Comparing `python_roborock-1.0.0/roborock/web_api.py` & `python_roborock-2.0.0/roborock/web_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-1.0.0/PKG-INFO` & `python_roborock-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 1.0.0
+Version: 2.0.0
 Summary: A package to control Roborock vacuums.
 Home-page: https://github.com/humbertogontijo/python-roborock
 License: GPL-3.0-only
 Keywords: roborock,vacuum,homeassistant
 Author: humbertogontijo
 Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-roborock Version: 1.0.0 Summary: A package
+Metadata-Version: 2.1 Name: python-roborock Version: 2.0.0 Summary: A package
 to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
 python-roborock License: GPL-3.0-only Keywords: roborock,vacuum,homeassistant
 Author: humbertogontijo Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.10,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
```

