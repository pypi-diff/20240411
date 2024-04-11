# Comparing `tmp/elkoep-mqtt-0.2.26.tar.gz` & `tmp/elkoep-mqtt-0.2.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elkoep-mqtt-0.2.26.tar", last modified: Wed Jan 31 13:49:36 2024, max compression
+gzip compressed data, was "elkoep-mqtt-0.2.27.tar", last modified: Thu Apr 11 12:02:37 2024, max compression
```

## Comparing `elkoep-mqtt-0.2.26.tar` & `elkoep-mqtt-0.2.27.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:49:36.219316 elkoep-mqtt-0.2.26/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-01-31 13:49:36.219316 elkoep-mqtt-0.2.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:49:36.219316 elkoep-mqtt-0.2.26/elkoep_mqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-01-31 13:49:36.000000 elkoep-mqtt-0.2.26/elkoep_mqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-01-31 13:49:36.000000 elkoep-mqtt-0.2.26/elkoep_mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 13:49:36.000000 elkoep-mqtt-0.2.26/elkoep_mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 13:49:36.000000 elkoep-mqtt-0.2.26/elkoep_mqtt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-31 13:49:36.000000 elkoep-mqtt-0.2.26/elkoep_mqtt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:49:36.215316 elkoep-mqtt-0.2.26/inelsmqtt/
--rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/inelsmqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/inelsmqtt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    22395 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/inelsmqtt/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:49:36.215316 elkoep-mqtt-0.2.26/inelsmqtt/devices/
--rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/inelsmqtt/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/inelsmqtt/devices/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/inelsmqtt/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/inelsmqtt/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   103241 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/inelsmqtt/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-01-31 13:49:36.219316 elkoep-mqtt-0.2.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:49:36.215316 elkoep-mqtt-0.2.26/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/tests/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:49:36.219316 elkoep-mqtt-0.2.26/tests/devices/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/tests/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16688 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/tests/devices/device_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/tests/discovery_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/tests/inels_mqtt_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-01-31 13:49:22.000000 elkoep-mqtt-0.2.26/tests/online_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:02:37.241004 elkoep-mqtt-0.2.27/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-11 12:02:37.241004 elkoep-mqtt-0.2.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:02:37.241004 elkoep-mqtt-0.2.27/elkoep_mqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-11 12:02:37.000000 elkoep-mqtt-0.2.27/elkoep_mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-11 12:02:37.000000 elkoep-mqtt-0.2.27/elkoep_mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:02:37.000000 elkoep-mqtt-0.2.27/elkoep_mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:02:37.000000 elkoep-mqtt-0.2.27/elkoep_mqtt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 12:02:37.000000 elkoep-mqtt-0.2.27/elkoep_mqtt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:02:37.237004 elkoep-mqtt-0.2.27/inelsmqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)    18091 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/inelsmqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/inelsmqtt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22709 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/inelsmqtt/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:02:37.237004 elkoep-mqtt-0.2.27/inelsmqtt/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)    10869 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/inelsmqtt/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/inelsmqtt/devices/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/inelsmqtt/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/inelsmqtt/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105922 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/inelsmqtt/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-11 12:02:37.241004 elkoep-mqtt-0.2.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:02:37.237004 elkoep-mqtt-0.2.27/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/tests/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:02:37.237004 elkoep-mqtt-0.2.27/tests/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/tests/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16688 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/tests/devices/device_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/tests/discovery_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/tests/inels_mqtt_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/tests/online_test.py
```

### Comparing `elkoep-mqtt-0.2.26/LICENSE` & `elkoep-mqtt-0.2.27/LICENSE`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.26/PKG-INFO` & `elkoep-mqtt-0.2.27/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elkoep-mqtt
-Version: 0.2.26
+Version: 0.2.27
 Summary: Python library for iNELS mqtt protocol
 Home-page: https://github.com/epdevlab/elkoep-mqtt
 Author: Elko EP s.r.o.
 Author-email: epdevlab@gmail.com
 License: MIT
 Keywords: iNels,Elko EP,Home assistant integration
 Classifier: License :: OSI Approved :: MIT License
@@ -98,7 +98,11 @@
 - TI3-10B (157)
 - TI3-40B (158)
 - TI3-60M (159)
 - IDRT3-1 (160)
 - JA3-018M (163)
 - Virtual heating regulator (167)
 - Virtual cooling regulator (168)
+- SA3_014M (169)
+- JA3_014M (170)
+- BITS (bits)
+- INTEGETS (integers)
```

### Comparing `elkoep-mqtt-0.2.26/README.md` & `elkoep-mqtt-0.2.27/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -83,7 +83,11 @@
 - TI3-10B (157)
 - TI3-40B (158)
 - TI3-60M (159)
 - IDRT3-1 (160)
 - JA3-018M (163)
 - Virtual heating regulator (167)
 - Virtual cooling regulator (168)
+- SA3_014M (169)
+- JA3_014M (170)
+- BITS (bits)
+- INTEGETS (integers)
```

### Comparing `elkoep-mqtt-0.2.26/elkoep_mqtt.egg-info/PKG-INFO` & `elkoep-mqtt-0.2.27/elkoep_mqtt.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elkoep-mqtt
-Version: 0.2.26
+Version: 0.2.27
 Summary: Python library for iNELS mqtt protocol
 Home-page: https://github.com/epdevlab/elkoep-mqtt
 Author: Elko EP s.r.o.
 Author-email: epdevlab@gmail.com
 License: MIT
 Keywords: iNels,Elko EP,Home assistant integration
 Classifier: License :: OSI Approved :: MIT License
@@ -98,7 +98,11 @@
 - TI3-10B (157)
 - TI3-40B (158)
 - TI3-60M (159)
 - IDRT3-1 (160)
 - JA3-018M (163)
 - Virtual heating regulator (167)
 - Virtual cooling regulator (168)
+- SA3_014M (169)
+- JA3_014M (170)
+- BITS (bits)
+- INTEGETS (integers)
```

### Comparing `elkoep-mqtt-0.2.26/elkoep_mqtt.egg-info/SOURCES.txt` & `elkoep-mqtt-0.2.27/elkoep_mqtt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.26/inelsmqtt/__init__.py` & `elkoep-mqtt-0.2.27/inelsmqtt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -407,29 +407,37 @@
         _LOGGER.info("Found device from topic %s\n", msg.topic)
 
         # pass only those who belong to known device types
         fragments = msg.topic.split("/")
         device_type = fragments[TOPIC_FRAGMENTS[FRAGMENT_DEVICE_TYPE]]
         action = fragments[TOPIC_FRAGMENTS[FRAGMENT_STATE]]
 
-        if device_type in DEVICE_TYPE_DICT:
-            topic = msg.topic.split("/")[2:]
-            topic = "/".join(topic)
+        topic = msg.topic.split("/")[2:]
+        topic = "/".join(topic)
 
+        if device_type in DEVICE_TYPE_DICT:
             if action == "status":
                 self.__discovered[topic] = msg.payload
                 self.__last_values[msg.topic] = msg.payload
                 self.__is_subscribed_list[msg.topic] = True
                 _LOGGER.info("Device of type %s found [status].\n", device_type)
             elif action == "connected":
                 if topic not in self.__discovered:
                     self.__discovered[topic] = None#msg.payload
                     self.__last_values[msg.topic] = msg.payload
                     self.__is_subscribed_list[msg.topic] = True
                 _LOGGER.info("Device of type %s found [connected].\n", device_type)
+        else:
+            if device_type == "gw" and action == "connected":
+                if msg.topic not in self.__is_subscribed_list:
+                    client.subscribe(msg.topic, 0, None, None)
+                    self.__messages[msg.topic] = msg.payload
+                    self.__last_values[msg.topic] = copy.copy(msg.topic)
+                    self.__is_subscribed_list[msg.topic] = True
+                    _LOGGER.info("Device of type %s found [gw].\n", device_type)
             
     def __on_message(
         self,
         client: mqtt.Client,  # pylint: disable=unused-argument
         userdata,  # pylint: disable=unused-argument
         msg,
     ) -> None:
@@ -442,15 +450,15 @@
         """
         self.__message_readed = True
         message_parts = msg.topic.split("/")
         device_type = message_parts[TOPIC_FRAGMENTS[FRAGMENT_DEVICE_TYPE]]
 
         message_type = message_parts[TOPIC_FRAGMENTS[FRAGMENT_STATE]]
 
-        if device_type in DEVICE_TYPE_DICT:
+        if device_type in DEVICE_TYPE_DICT or device_type == "gw":
             # keep last value
             self.__last_values[msg.topic] = (
                 copy.copy(self.__messages[msg.topic])
                 if msg.topic in self.__messages
                 else msg.payload
             )
             self.__messages[msg.topic] = msg.payload
```

### Comparing `elkoep-mqtt-0.2.26/inelsmqtt/config.py` & `elkoep-mqtt-0.2.27/inelsmqtt/config.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.26/inelsmqtt/const.py` & `elkoep-mqtt-0.2.27/inelsmqtt/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 SWITCH = "switch"
 SENSOR = "sensor"
 LIGHT = "light"
 COVER = "cover"
 CLIMATE = "climate"
 BUTTON = "button"
 BINARY_SENSOR = "binary_sensor"
+NUMBER = "number"
 
 # RF
 RF_SINGLE_SWITCH = "Single switching unit"  # 01
 RF_SWITCHING_UNIT = "Switching unit" #02
 RF_SHUTTERS = "Shutters" #3
 RF_SINGLE_DIMMER = "Single dimmer"  # 04
 RF_DIMMER = "Dimmer" #05
@@ -84,14 +85,16 @@
 WSB3_40 = "WSB3-40"
 WSB3_40H = "WSB3-40H"
 RC3_610DALI = "RC3-610DALI"
 JA3_018M = "JA3-018M"
 JA3_014M = "JA3-014M"
 DALI_DMX_UNIT = "DALI-DMX-Unit"
 DALI_DMX_UNIT_2 = "DALI-DMX-Unit-2"
+INTEGERS = "INTEGERS"
+BITS = "BITS"
 
 #Virtual bus
 VIRT_CONTR = "Virtual controller"
 VIRT_HEAT_REG = "Heat virtual regulator"
 VIRT_COOL_REG = "Cool virtual regulator"
 
 
@@ -173,14 +176,17 @@
     "164": DALI_DMX_UNIT,
     "165": DALI_DMX_UNIT_2,
     "166": VIRT_CONTR,
     "167": VIRT_HEAT_REG,
     "168": VIRT_COOL_REG,
 
     "170": JA3_014M,
+
+    "bits": BITS,
+    "integers": INTEGERS,
 }
 
 #TODO retire this system
 # device types
 DEVICE_TYPE_DICT = {
     # RF
     "01": SWITCH, # RF_SINGLE_SWITCH
@@ -253,14 +259,17 @@
     "164": LIGHT, # DALI_DMX_UNIT
     "165": LIGHT, # DALI_DMX_UNIT_2
     "166": CLIMATE, # VIRT_CONTR
     "167": CLIMATE, # VIRT_HEAT_REG
     "168": CLIMATE, # VIRT_COOL_REG
 
     "170": COVER, # JA3_014M
+
+    "bits": SWITCH,
+    "integers": NUMBER,
 }
 
 
 BATTERY = "battery"
 TEMP_IN = "temp_in"
 TEMP_OUT = "temp_out"
 TEMPERATURE = "temperature"
@@ -839,17 +848,24 @@
     FRAGMENT_DOMAIN: 0,
     FRAGMENT_STATE: 1,
     FRAGMENT_SERIAL_NUMBER: 2,
     FRAGMENT_DEVICE_TYPE: 3,
     FRAGMENT_UNIQUE_ID: 4,
 }
 
+GW_CONNECTED = {
+    b"{\"status\": true}": True,
+    b"{\"status\": false}": False,
+}
+
 DEVICE_CONNECTED = {
     "on\n": True,
     "off\n": False,
+    "{\"status\": true}": True,
+    "{\"status\": false}": False,
 }
 
 # SWITCH CONSTANTS
 SWITCH_ON_STATE = "02\n01\n"
 SWITCH_OFF_STATE = "02\n00\n"
 
 SWITCH_ON_SET = "01\n00\n00\n"
```

### Comparing `elkoep-mqtt-0.2.26/inelsmqtt/devices/__init__.py` & `elkoep-mqtt-0.2.27/inelsmqtt/devices/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     MANUFACTURER,
     SENSOR,
     BUTTON,
     TOPIC_FRAGMENTS,
     FRAGMENT_DEVICE_TYPE,
     FRAGMENT_SERIAL_NUMBER,
     FRAGMENT_UNIQUE_ID,
+    GW_CONNECTED,
     DEVICE_CONNECTED,
     VERSION,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -62,14 +63,15 @@
         self.__state_topic = state_topic
         self.__set_topic = None
 
         if self.__device_type is not SENSOR and self.__device_type is not BUTTON:
             self.__set_topic = f"{fragments[TOPIC_FRAGMENTS[FRAGMENT_DOMAIN]]}/set/{fragments[TOPIC_FRAGMENTS[FRAGMENT_SERIAL_NUMBER]]}/{fragments[TOPIC_FRAGMENTS[FRAGMENT_DEVICE_TYPE]]}/{fragments[TOPIC_FRAGMENTS[FRAGMENT_UNIQUE_ID]]}"  # noqa: E501
 
         self.__connected_topic = f"{fragments[TOPIC_FRAGMENTS[FRAGMENT_DOMAIN]]}/connected/{fragments[TOPIC_FRAGMENTS[FRAGMENT_SERIAL_NUMBER]]}/{fragments[TOPIC_FRAGMENTS[FRAGMENT_DEVICE_TYPE]]}/{fragments[TOPIC_FRAGMENTS[FRAGMENT_UNIQUE_ID]]}"  # noqa: E501
+        self.__gw_connected_topic = f"{fragments[TOPIC_FRAGMENTS[FRAGMENT_DOMAIN]]}/connected/{fragments[TOPIC_FRAGMENTS[FRAGMENT_SERIAL_NUMBER]]}/gw"  # noqa: E501
         self.__title = title if title is not None else self.__unique_id
         self.__domain = fragments[TOPIC_FRAGMENTS[FRAGMENT_DOMAIN]]
         self.__state: Any = None
         self.__values: DeviceValue = None
     
         self.__entity_callbacks: dict[tuple[str, int], Callable[[Any], Any]] = None
         # subscribe availability
@@ -133,15 +135,19 @@
     @property
     def is_available(self) -> bool:
         """Get info about availability of device
 
         Returns:
             bool: True/False
         """
-        val = self.__mqtt.messages()[self._Device__connected_topic]
+        gw = self.__mqtt.messages().get(self._Device__gw_connected_topic)
+        if not GW_CONNECTED.get(gw):
+            return False
+
+        val = self.__mqtt.messages().get(self._Device__connected_topic)
         if isinstance(val, (bytes, bytearray)):
             val = val.decode()
 
         return DEVICE_CONNECTED.get(val) and self.__values is not None and self.__values._DeviceValue__ha_value is not None
 
     @property
     def set_topic(self) -> str:
```

### Comparing `elkoep-mqtt-0.2.26/inelsmqtt/devices/switch.py` & `elkoep-mqtt-0.2.27/inelsmqtt/devices/switch.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.26/inelsmqtt/discovery.py` & `elkoep-mqtt-0.2.27/inelsmqtt/discovery.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.26/inelsmqtt/mqtt_client.py` & `elkoep-mqtt-0.2.27/inelsmqtt/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.26/inelsmqtt/util.py` & `elkoep-mqtt-0.2.27/inelsmqtt/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Utility classes."""
 from dataclasses import dataclass
 import logging
+import json
+import re
 
 from operator import itemgetter
 from typing import Any, Dict, Optional
 
 from inelsmqtt.mqtt_client import GetMessageType
 
 from .const import (
@@ -201,16 +203,32 @@
     
     INELS_DEVICE_TYPE_DATA_STRUCT_DATA,
 
     DEVICE_TYPE_07_COMM_TEST,
     Shutter_state,
     Climate_action,
     Climate_modes,
+
+    BITS,
+    INTEGERS,
+    NUMBER,
 )
 
+#bit
+@dataclass
+class Bit():
+    is_on: bool
+    addr: str
+
+#number
+@dataclass
+class Number():
+    value: int
+    addr: str
+
 #relay
 @dataclass
 class SimpleRelay():
     """Create simple relay"""
     is_on: bool
 
 @dataclass
@@ -274,14 +292,37 @@
     return type("Object", (), kwargs)
 
 def break_into_bytes(line: str):
     if len(line)%2 == 0:
         return [line[i:i+2] for i in range(0, len(line), 2)]
     return []
 
+def xparse_formated_json(data):
+    regex = r"state\":\{(.*)\}\}"
+    match = re.search(regex, data)
+    addr_val_list = []
+    if match != None:
+        states = match.group(1)
+        addr_value_pair_list = states.split(',')
+        for item in addr_value_pair_list:
+            addr, val = item.split(':')
+            addr_val_list.append(
+                (addr, int(val))
+            )
+    return addr_val_list
+
+def parse_formated_json(data):
+    addr_val_list = []
+    data = json.loads(data)
+    for addr, val in data['state'].items():
+        addr_val_list.append(
+            (addr, val)
+        )
+    return addr_val_list
+
 class DeviceValue(object):
     """Device value interpretation object."""
 
     def __init__(
         self,
         device_type: str,
         inels_type: str,
@@ -838,14 +879,50 @@
                     self.__ha_value = new_object(
                         simple_relay=simple_relay,
                         interface=interface,
                         temp_in=temp_in,
                         card_present=card_present,
                         card_id=card_id,
                     )
+                elif self.__inels_type is BITS:
+                    bit: list[Bit] = []
+                    for addr, val in parse_formated_json(self.__inels_status_value):
+                        bit.append(
+                            Bit(
+                                is_on=val, addr=addr
+                            )
+                        )
+
+                    self.__ha_value = new_object(
+                        bit=bit,
+                    )
+
+                    set_val = {}
+                    for bit in self.ha_value.bit:
+                        set_val[bit.addr] = bit.is_on
+
+                    self.__inels_set_value = json.dumps({"cmd": set_val})
+            elif self.__device_type is NUMBER:
+                number: list[Number] = []
+                for addr, val in parse_formated_json(self.__inels_status_value):
+                    number.append(
+                        Number(
+                            value=val, addr=addr
+                        )
+                    )
+
+                self.__ha_value = new_object(
+                    number=number,
+                )
+
+                set_val = {}
+                for number in self.ha_value.number:
+                    set_val[number.addr] = number.value
+
+                self.__inels_set_value = json.dumps({"cmd": set_val})
             elif self.__device_type is SENSOR:  # temperature sensor
                 if self.__inels_type is RF_TEMPERATURE_INPUT:
                     battery = int(self.__trim_inels_status_values(DEVICE_TYPE_10_DATA, BATTERY, ""), 16)
                     temp_in = self.__trim_inels_status_values(DEVICE_TYPE_10_DATA, TEMP_IN, "")
                     temp_out = self.__trim_inels_status_values(DEVICE_TYPE_10_DATA, TEMP_OUT, "")
 
                     self.__ha_value = new_object(
@@ -1189,27 +1266,27 @@
                         )
                 elif self.__inels_type is RF_LIGHT_BULB:
                     if self.inels_status_value is None:
                         _LOGGER.info("inels_status_value was None for %s", RF_LIGHT_BULB)
                         self.__inels_set_value = DEVICE_TYPE_13_COMM_TEST
                         self.__ha_value = None
                     else:
-                        simple_light = []
-                        simple_light.append(
+                        warm_light = []
+                        warm_light.append(
                             WarmLight(
                                     brightness=round(
                                         int(self.__trim_inels_status_values(DEVICE_TYPE_13_DATA, OUT, ""), 16) * 100.0/255.0
                                     ),
                                     relative_ct=round(
                                         int(self.__trim_inels_status_values(DEVICE_TYPE_13_DATA, WHITE, ""), 16) * 100.0/255.0
                                     )
                                 ),
                             )
 
-                        self.__ha_value=new_object(simple_light=simple_light)
+                        self.__ha_value=new_object(warm_light=warm_light)
                 elif self.__inels_type is DA3_22M:
                     temp = self.__trim_inels_status_values(DA3_22M_DATA, TEMP_IN, "")
 
                     state = self.__trim_inels_status_values(
                         DA3_22M_DATA, DA3_22M, "")
                     state_hex_str = f"0x{state}"
                     state_bin_str = f"{int(state_hex_str, 16):0>8b}"
@@ -2177,15 +2254,27 @@
                         set_val += fan_val
                         set_val += f"{original_status[15]}\n"
                         
                         self.__inels_set_value = set_val
                     elif self.__inels_type in [GCR3_11, GCH3_31]:
                         set_val = "04\n" if self.ha_value.simple_relay[0].is_on else "00\n"
                         set_val += "00\n" * 9
-                        self.__inels_set_value = set_val 
+                        self.__inels_set_value = set_val
+                    elif self.__inels_type is BITS:
+                        set_val = {}
+                        for bit in self.ha_value.bit:
+                            set_val[bit.addr] = int(bit.is_on)
+
+                        self.__inels_set_value = json.dumps({"cmd": set_val})
+                elif self.__device_type is NUMBER:
+                    set_val = {}
+                    for number in self.ha_value.number:
+                        set_val[number.addr] = int(number.value)
+
+                    self.__inels_set_value = json.dumps({"cmd": set_val})
                 elif self.__device_type is LIGHT:
                     if self.__inels_type in [RF_SINGLE_DIMMER, RF_DIMMER]:
                         if self.__ha_value is None:
                             self.__inels_set_value = DEVICE_TYPE_05_COMM_TEST
                         else:
                             out = round(self.__ha_value.simple_light[0].brightness, -1)
                             out = out if out < 100 else 100
@@ -2200,15 +2289,15 @@
                         else:
                             rgb = self.__ha_value.rgb[0]
                             self.__inels_set_value = f"01\n{rgb.r:02X}\n{rgb.g:02X}\n{rgb.b:02X}\n{int(rgb.brightness*2.55):02X}\n00\n"
                     elif self.__inels_type is RF_LIGHT_BULB:
                         if self.__ha_value is None:
                             self.__inels_set_value = DEVICE_TYPE_13_COMM_TEST
                         else:
-                            self.__inels_set_value = f"0F\n00\n00\n00\n{round(self.ha_value.simple_light[0].brightness*2.55):02X}\n{round(self.ha_value.simple_light[0].relative_ct*2.55):02X}\n"
+                            self.__inels_set_value = f"0F\n00\n00\n00\n{round(self.ha_value.warm_light[0].brightness*2.55):02X}\n{round(self.ha_value.warm_light[0].relative_ct*2.55):02X}\n"
                     elif self.__inels_type is DA3_22M:
                         # correct the values
                         out1 = round(self.__ha_value.light_coa_toa[0].brightness, -1)
                         out1 = out1 if out1 < 100 else 100
 
                         out2 = round(self.__ha_value.light_coa_toa[1].brightness, -1)
                         out2 = out2 if out2 < 100 else 100
```

### Comparing `elkoep-mqtt-0.2.26/setup.py` & `elkoep-mqtt-0.2.27/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup script for elkoep-mqtt package."""
 from setuptools import setup, find_packages
 
 setup(
     name="elkoep-mqtt",
-    version="0.2.26",
+    version="0.2.27",
     url="https://github.com/epdevlab/elkoep-mqtt",
     license="MIT",
     author="Elko EP s.r.o.",
     author_email="epdevlab@gmail.com",
     description="Python library for iNELS mqtt protocol",
     keywords=["iNels", "Elko EP", "Home assistant integration"],
     long_description_content_type="text/markdown",
```

### Comparing `elkoep-mqtt-0.2.26/tests/const.py` & `elkoep-mqtt-0.2.27/tests/const.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.26/tests/devices/device_test.py` & `elkoep-mqtt-0.2.27/tests/devices/device_test.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.26/tests/discovery_test.py` & `elkoep-mqtt-0.2.27/tests/discovery_test.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.26/tests/inels_mqtt_test.py` & `elkoep-mqtt-0.2.27/tests/inels_mqtt_test.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.26/tests/online_test.py` & `elkoep-mqtt-0.2.27/tests/online_test.py`

 * *Files identical despite different names*

