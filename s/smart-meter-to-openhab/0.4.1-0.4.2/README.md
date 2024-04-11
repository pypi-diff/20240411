# Comparing `tmp/smart_meter_to_openhab-0.4.1.tar.gz` & `tmp/smart_meter_to_openhab-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_meter_to_openhab-0.4.1.tar", max compression
+gzip compressed data, was "smart_meter_to_openhab-0.4.2.tar", max compression
```

## Comparing `smart_meter_to_openhab-0.4.1.tar` & `smart_meter_to_openhab-0.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1211 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/LICENSE
--rw-r--r--   0        0        0     4538 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/README.md
--rw-r--r--   0        0        0      793 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      543 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/.env.example
--rw-r--r--   0        0        0      154 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/__init__.py
--rw-r--r--   0        0        0     9319 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/interfaces.py
--rw-r--r--   0        0        0     7092 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/openhab.py
--rw-r--r--   0        0        0     8158 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/sml_iskra_mt175.py
--rw-r--r--   0        0        0     3531 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/sml_reader.py
--rw-r--r--   0        0        0      168 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/utils.py
--rw-r--r--   0        0        0     6448 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/smart_meter_to_openhab_scripts/main.py
--rw-r--r--   0        0        0     5211 1970-01-01 00:00:00.000000 smart_meter_to_openhab-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4580 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/README.md
+-rw-r--r--   0        0        0      793 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      543 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/.env.example
+-rw-r--r--   0        0        0      349 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/__init__.py
+-rw-r--r--   0        0        0     8849 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/interfaces.py
+-rw-r--r--   0        0        0     7314 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/openhab.py
+-rw-r--r--   0        0        0     8594 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/sml_iskra_mt175.py
+-rw-r--r--   0        0        0     3531 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/sml_reader.py
+-rw-r--r--   0        0        0      301 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/utils.py
+-rw-r--r--   0        0        0     7084 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/smart_meter_to_openhab_scripts/main.py
+-rw-r--r--   0        0        0     5253 1970-01-01 00:00:00.000000 smart_meter_to_openhab-0.4.2/PKG-INFO
```

### Comparing `smart_meter_to_openhab-0.4.1/LICENSE` & `smart_meter_to_openhab-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_meter_to_openhab-0.4.1/README.md` & `smart_meter_to_openhab-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,25 +25,26 @@
 ```
 5. Install smart-meter-to-openhab
 ```bash
 pip install smart-meter-to-openhab
 ```
 6. Provide environment variables. You can e.g. pass a .env file to smart-meter-to-openhab via the option *--dotenv_path*. Or provide them by any other means (e.g. in your ~/.profile).
 ```bash
-# Hostname incl. http(s)
+# Hostname incl. http(s) (required)
 OH_HOST='<http://your_ip:your_port'
 #openhab user (or token) for login (optional)
 OH_USER=''
 #openhab password for login (optional)
 OH_PASSWD=''
-#openhab item names. Optional, but recommended :) 
+#current consumption openhab item (required)
+OVERALL_CONSUMPTION_WATT_OH_ITEM='smart_meter_overall_consumption'
+#other openhab item names (optional)
 PHASE_1_CONSUMPTION_WATT_OH_ITEM='smart_meter_phase_1_consumption'
 PHASE_2_CONSUMPTION_WATT_OH_ITEM='smart_meter_phase_2_consumption'
 PHASE_3_CONSUMPTION_WATT_OH_ITEM='smart_meter_phase_3_consumption'
-OVERALL_CONSUMPTION_WATT_OH_ITEM='smart_meter_overall_consumption'
 OVERALL_CONSUMPTION_WH_OH_ITEM='smart_meter_overall_consumption_wh'
 ELECTRICITY_METER_KWH_OH_ITEM='smart_meter_electricity_meter'
 ```
 NOTE: certificate verification is turned off, in case *OH_HOST* refers to an https address (since most openHAB instances do probably use self-signed certificates)  
 
 7. Run smart-meter-to-openhab with e.g.
 ```bash
```

### Comparing `smart_meter_to_openhab-0.4.1/pyproject.toml` & `smart_meter_to_openhab-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smart_meter_to_openhab"
-version = "0.4.1"
+version = "0.4.2"
 description = "Pushing data of ISKRA MT175 smart meter to openhab"
 authors = ["Heiko Bauer <heiko_bauer@icloud.com>"]
 repository = "https://github.com/die-bauerei/smart-meter-to-openhab"
 readme = "README.md"
 packages = [
     {include = "smart_meter_to_openhab"},
     {include = "smart_meter_to_openhab_scripts"}
```

### Comparing `smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/.env.example` & `smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/.env.example`

 * *Files identical despite different names*

### Comparing `smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/interfaces.py` & `smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         for new_value in new_values:
             for this_value in self._oh_items_and_values:
                 if this_value.oh_item == new_value.oh_item:
                     this_value.value = new_value.value
                     break
 
     def __iter__(self) -> Iterator[OhItemAndValue]:
-        return iter(self._oh_items_and_values)                
+        return iter(self._oh_items_and_values)
     
     def is_invalid(self) -> bool:
         # consider only the values that really will be used (oh_item name not empty)
         return all(oh_item_value.value is None for oh_item_value in self._oh_items_and_values if oh_item_value.oh_item)
     
     def is_valid(self) -> bool:
         return not self.is_invalid()
@@ -75,20 +75,14 @@
         return [oh_item_value.value for oh_item_value in self._oh_items_and_values  if oh_item_value.oh_item]
     
     def __eq__(self, other) -> bool:
         if isinstance(other, OhItemAndValueContainer):
             return self.value_list() == other.value_list()
         return False
     
-    @staticmethod    
-    def create_container(values : List[OhItemAndValue], oh_item_names : Tuple[str,...]) -> OhItemAndValueContainer:
-        value_container=OhItemAndValueContainer(oh_item_names)
-        value_container.assign_values(values)
-        return value_container
-    
 # NOTE: Use a tuple (immutable type) here to prevent changing the values 
 SmartMeterOhItemNames = Tuple[str, str, str, str, str]
 def _read_smart_meter_env() -> SmartMeterOhItemNames:
     return (os.getenv('PHASE_1_CONSUMPTION_WATT_OH_ITEM', default=''),
             os.getenv('PHASE_2_CONSUMPTION_WATT_OH_ITEM', default=''),
             os.getenv('PHASE_3_CONSUMPTION_WATT_OH_ITEM', default=''),
             os.getenv('OVERALL_CONSUMPTION_WATT_OH_ITEM', default=''),
@@ -126,16 +120,17 @@
 
     @staticmethod
     def oh_item_names() -> SmartMeterOhItemNames:
         return SmartMeterValues._oh_item_names
 
     @staticmethod    
     def create(values : List[OhItemAndValue], user_specified_oh_item_names : Union[SmartMeterOhItemNames, None] = None) -> SmartMeterValues:
-        oh_items = user_specified_oh_item_names if user_specified_oh_item_names is not None else SmartMeterValues.oh_item_names()
-        return cast(SmartMeterValues, OhItemAndValueContainer.create_container(values, oh_items))
+        value=SmartMeterValues(user_specified_oh_item_names=user_specified_oh_item_names)
+        value.assign_values(values)
+        return value
     
     @staticmethod
     def create_avg(values : List[SmartMeterValues], user_specified_oh_item_names : Union[SmartMeterOhItemNames, None] = None) -> SmartMeterValues:
         smart_meter_values=SmartMeterValues(None, None, None, None, None, user_specified_oh_item_names)
         phase_1_value_list = [value.phase_1_consumption.value for value in values if value.phase_1_consumption.value is not None]
         if phase_1_value_list: 
             smart_meter_values.phase_1_consumption.value = mean(phase_1_value_list)
@@ -175,9 +170,10 @@
 
     @staticmethod
     def oh_item_names() -> ExtendedSmartMeterOhItemNames:
         return ExtendedSmartMeterValues._oh_item_names
 
     @staticmethod    
     def create(values : List[OhItemAndValue], user_specified_oh_item_names : Union[ExtendedSmartMeterOhItemNames, None] = None) -> ExtendedSmartMeterValues:
-        oh_items = user_specified_oh_item_names if user_specified_oh_item_names is not None else ExtendedSmartMeterValues.oh_item_names()
-        return cast(ExtendedSmartMeterValues, OhItemAndValueContainer.create_container(values, oh_items))
+        value=ExtendedSmartMeterValues(user_specified_oh_item_name=user_specified_oh_item_names)
+        value.assign_values(values)
+        return value
```

### Comparing `smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/openhab.py` & `smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/openhab.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 import http
 import datetime
 from logging import Logger
 from requests.auth import HTTPBasicAuth
 from requests.adapters import HTTPAdapter, Retry
-from typing import List, Tuple, Union
+from typing import List, Tuple
 from statistics import median
 from .interfaces import *
 
 # disable warnings about insecure requests because ssl verification is disabled
 import urllib3
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
@@ -19,22 +19,27 @@
     for value_index in range(len(list_values[0]) if list_values else 0):
         item_value_list : List[OhItemAndValue] = []
         for item_index, item in enumerate(valid_items):
             item_value_list.append(OhItemAndValue(item, list_values[item_index][value_index]))
         smart_meter_values.append(SmartMeterValues.create(item_value_list))
     return smart_meter_values
 
-def _check_if_updated(values : List[SmartMeterValues], default : Union[SmartMeterValues, None] = None) -> bool:
-    valid_default=default is not None and default.is_valid()
-    valid_values=[value for value in values if value.is_valid()]
-    for value in valid_values:
-        if valid_default and value == default: # consider a valid default value as updated
-            return True
-        elif value != valid_values[0]:
-            return True
+def _check_if_updated(values : List[SmartMeterValues]) -> bool:
+    valid_values : List[SmartMeterValues] = [value for value in values if value.is_valid()]
+    if len(valid_values) < 2:
+        return False
+
+    # no consumption is good and considered as updated
+    if all((value.overall_consumption.value is not None and value.overall_consumption.value == 0) for value in valid_values):
+        return True
+    
+    # for all other cases, at least one value has to be different
+    if any(value != valid_values[0] for value in valid_values):
+        return True
+    
     return False
 
 def _get_median(oh_item_names : SmartMeterOhItemNames, list_values : List[List[float]]) -> SmartMeterValues:
     smart_meter_values : List[OhItemAndValue] = []
     value_index=0
     for item in oh_item_names:
         if item:
@@ -45,15 +50,15 @@
 
 class OpenhabConnection():
     def __init__(self, oh_host : str, oh_user : str, oh_passwd : str, logger : Logger) -> None:
         self._oh_host=oh_host
         self._session=requests.Session()
         if oh_user:
             self._session.auth=HTTPBasicAuth(oh_user, oh_passwd)
-        retries=Retry(total=10,
+        retries=Retry(total=5,
                 backoff_factor=0.1,
                 status_forcelist=[ 500, 502, 503, 504 ])
         self._session.mount('http://', HTTPAdapter(max_retries=retries))
         self._session.mount('https://', HTTPAdapter(max_retries=retries))
         self._session.headers={'Content-Type': 'text/plain'}
         self._logger=logger
 
@@ -85,18 +90,16 @@
     def get_values_from_items(self, oh_item_names : SmartMeterOhItemNames) -> SmartMeterValues:
         return SmartMeterValues.create(self.get_item_value_list_from_items(oh_item_names))
     
     def get_extended_values_from_items(self, oh_item_names : ExtendedSmartMeterOhItemNames) -> ExtendedSmartMeterValues:
         return ExtendedSmartMeterValues.create(self.get_item_value_list_from_items(oh_item_names))
 
     PersistenceValuesType = List[List[float]]
-    def _get_persistence_values(self, oh_item_names : Tuple[str, ...], timedelta : datetime.timedelta) -> PersistenceValuesType:
+    def _get_persistence_values(self, oh_item_names : Tuple[str, ...], start_time : datetime.datetime, end_time : datetime.datetime) -> PersistenceValuesType:
         pers_values = []
-        end_time=datetime.datetime.now()
-        start_time=end_time-timedelta
         for item in oh_item_names:
             if item:
                 values=[]
                 try:
                     with self._session.get(
                         url=f"{self._oh_host}/rest/persistence/items/{item}", 
                         params={'starttime': start_time.isoformat(), 'endtime': end_time.isoformat()},
@@ -106,22 +109,24 @@
                         else:
                             values=[float(data['state']) for data in response.json()['data']]
                 except requests.exceptions.RequestException as e:
                     self._logger.warning("Caught Exception while getting persistence data from openHAB: " + str(e))
                 pers_values.append(values)
         return pers_values
 
-    def check_if_persistence_values_updated(self, oh_item_names : SmartMeterOhItemNames, timedelta : datetime.timedelta, 
-                         default : Union[SmartMeterValues, None] = None) -> bool:
-        pers_values=self._get_persistence_values(oh_item_names, timedelta)
+    def check_if_persistence_values_updated(self, oh_item_names : SmartMeterOhItemNames, start_time : datetime.datetime, end_time : datetime.datetime) -> bool:
+        pers_values=self._get_persistence_values(oh_item_names, start_time, end_time)
         if pers_values and any(len(values) != len(pers_values[0]) for values in pers_values):
             # return True in case the input lists are of unequal size
             # NOTE: This happens if the GET/POST requests to Openhab have not been completely successful.
+            self._logger.warning("Persistence values are of unequal size. Assuming they have been updated.")
             return True
         
         smart_meter_values=_convert_list_to_smart_meter_values(oh_item_names, pers_values)
-        return _check_if_updated(smart_meter_values, default)
+        return _check_if_updated(smart_meter_values)
 
     def get_median_from_items(self, oh_item_names : SmartMeterOhItemNames, 
                               timedelta : datetime.timedelta = datetime.timedelta(minutes=30)) -> SmartMeterValues:
-        pers_values=self._get_persistence_values(oh_item_names, timedelta)
+        end_time=datetime.datetime.now()
+        start_time=end_time-timedelta
+        pers_values=self._get_persistence_values(oh_item_names, start_time, end_time)
         return _get_median(oh_item_names, pers_values)
```

### Comparing `smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/sml_iskra_mt175.py` & `smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/sml_iskra_mt175.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import serial
 import os
+import logging
 from datetime import timedelta, datetime
 from logging import Logger
 from typing import Protocol, List, Any, Optional
 from functools import cached_property
 from pathlib import Path
 from .interfaces import SmartMeterValues
 
@@ -14,40 +15,73 @@
             return True
     return False
 
 class SmartMeterReader(Protocol):
     @cached_property
     def default(self) -> SmartMeterValues:
         ...
-
     @cached_property
     def estimated_max_read_time_in_sec(self) -> int:
         ...
     
-    # TODO: this function can already be implemented in an abstract class
+    # TODO:  this function can already be implemented in an abstract class
     def read(self, ref_values : SmartMeterValues) -> SmartMeterValues:
         ...
 
+# supporting OBIS code 1.8.0 only
+def _decode_sml_iskra_mt175_one_way(raw_data : str) -> SmartMeterValues:
+    def _convert_to_float(pos_begin : int, pos_end : int) -> Optional[float]:
+        try:
+            hex_number=raw_data[pos_begin:pos_end]
+            if hex_number.startswith('ff'):
+                # in case of negative energy the value is unspecified. returning 0 comes as close as possible to the real unknown value.
+                return 0
+            return int(hex_number, 16)
+        except Exception as e:
+            return None
+        
+    smart_meter_values=SmartMeterValues()
+
+    pos = raw_data.find('070100010800ff') # looking for OBIS Code: 1-0:1.8.0*255 - Energy kWh
+    smart_meter_values.electricity_meter.value = _convert_to_float(pos+36, pos+52) if pos != -1 else None
+    if smart_meter_values.electricity_meter.value is not None:
+        smart_meter_values.electricity_meter.value /= 1e4
+
+    pos = raw_data.find('070100100700ff') # looking for OBIS Code: 1-0:16.7.0*255 - Sum Power L1,L2,L3
+    smart_meter_values.overall_consumption.value = _convert_to_float(pos+28, pos+36) if pos != -1 else None
+
+    pos = raw_data.find('070100240700ff') # looking for OBIS Code: 1-0:36.7.0*255 - current Power L1
+    smart_meter_values.phase_1_consumption.value = _convert_to_float(pos+28, pos+36) if pos != -1 else None
+
+    pos = raw_data.find('070100380700ff') # looking for OBIS Code: 1-0:56.7.0*255 - current Power L2
+    smart_meter_values.phase_2_consumption.value = _convert_to_float(pos+28, pos+36) if pos != -1 else None
+
+    pos = raw_data.find('0701004c0700ff') # looking for OBIS Code: 1-0:76.7.0*255 - current Power L3
+    smart_meter_values.phase_3_consumption.value = _convert_to_float(pos+28, pos+36) if pos != -1 else None
+
+    return smart_meter_values
+
 # The smart meter supports consumption only. No electricity feed-in support! (German: Zweirichtungszähler)
 class SmlIskraMt175OneWay():
     # Data reading will be canceled after this time period.
     #      NOTE: Take care that this is longer then the specified transmission time of your smart meter.
     _read_raw_time_out_in_sec : int = 5
     # try n times to get a valid raw read
-    _max_read_attempts : int = 4
+    # TODO: rm this when a value of 1 works
+    _max_read_attempts : int = 1
 
     def __init__(self, serial_port : str, logger : Logger, raw_data_dump_dir : Optional[Path] = None) -> None:
         self._port=serial.Serial(baudrate=9600, bytesize=serial.EIGHTBITS, parity=serial.PARITY_NONE, stopbits=serial.STOPBITS_ONE)
         self._serial_port=serial_port
         self._logger=logger
         self._latest_raw_data=''
         self._raw_data_dump_dir=raw_data_dump_dir
         self._raw_data_dump_invalid_counter=0
         self._raw_data_dump_outlier_counter=0
-        # TODO: add a possibility to dump raw data for valid cases aswell (e.g. when logger.debug)
+        self._raw_data_dump_valid_counter=0
         if self._raw_data_dump_dir:
             os.makedirs(self._raw_data_dump_dir, exist_ok=True)
             self._logger.info(f"Using directory {self._raw_data_dump_dir} for raw data dumps.")
 
     @cached_property
     def default(self) -> SmartMeterValues:
         return SmartMeterValues(overall_consumption=0, phase_1_consumption=0, phase_2_consumption=0, phase_3_consumption=0)
@@ -91,14 +125,19 @@
             break
 
         value_list=values.value_list()
         if values.is_invalid() or _has_outlier(value_list, ref_value_list):
             self._logger.warning(f"Unable to read and validate SML data. Ignoring following values: {values}")
             values.reset()
 
+        if self._raw_data_dump_dir and self._logger.level == logging.DEBUG and values.is_valid():
+            with open(self._raw_data_dump_dir / f"raw_data_dump_valid_{self._raw_data_dump_valid_counter}.sml", 'w') as f:
+                f.write(self._latest_raw_data)
+            self._raw_data_dump_valid_counter+=1
+
         return values if values.is_valid() else self.default
 
     def _read_raw(self) -> SmartMeterValues:
         """Read raw data from the smart meter via SML
 
         Parameters
         ----------
@@ -107,22 +146,14 @@
             NOTE: Take care that this is longer then the specified transmission time of your smart meter.
         
         Returns
         -------
         SmartMeterValues
             Contains the data read from the smart meter
         """
-
-        def _convert_to_float(pos_begin : int, pos_end : int) -> Optional[float]:
-            try:
-                return int(self._latest_raw_data[pos_begin:pos_end], 16)
-            except Exception as e:
-                self._logger.info("Caught Exception in _read_raw.__convert_to_float: " + str(e))
-                return None
-
         self._latest_raw_data = ''
         smart_meter_values=SmartMeterValues()
         try:
             if not self._port.is_open:
                 self._port.port=self._serial_port
                 self._port.open()
             time_out : timedelta = timedelta(seconds=self._read_raw_time_out_in_sec)
@@ -136,32 +167,15 @@
                 if (pos != -1):
                     self._latest_raw_data = self._latest_raw_data[pos:] # cut trash before start delimiter
 
                 pos = self._latest_raw_data.find('1b1b1b1b1a')              # find end of Frame
 
                 if (pos != -1) and len(self._latest_raw_data) >= pos + 16:
                     self._latest_raw_data = self._latest_raw_data[0:pos + 16]                # cut trash after end delimiter
-                    
-                    pos = self._latest_raw_data.find('070100010800ff') # looking for OBIS Code: 1-0:1.8.0*255 - Energy kWh
-                    smart_meter_values.electricity_meter.value = _convert_to_float(pos+36, pos+52) if pos != -1 else None
-                    if smart_meter_values.electricity_meter.value is not None:
-                        smart_meter_values.electricity_meter.value /= 1e4
-
-                    pos = self._latest_raw_data.find('070100100700ff') # looking for OBIS Code: 1-0:16.7.0*255 - Sum Power L1,L2,L3
-                    smart_meter_values.overall_consumption.value = _convert_to_float(pos+28, pos+36) if pos != -1 else None
-
-                    pos = self._latest_raw_data.find('070100240700ff') # looking for OBIS Code: 1-0:36.7.0*255 - current Power L1
-                    smart_meter_values.phase_1_consumption.value = _convert_to_float(pos+28, pos+36) if pos != -1 else None
-
-                    pos = self._latest_raw_data.find('070100380700ff') # looking for OBIS Code: 1-0:56.7.0*255 - current Power L2
-                    smart_meter_values.phase_2_consumption.value = _convert_to_float(pos+28, pos+36) if pos != -1 else None
-
-                    pos = self._latest_raw_data.find('0701004c0700ff') # looking for OBIS Code: 1-0:76.7.0*255 - current Power L3
-                    smart_meter_values.phase_3_consumption.value = _convert_to_float(pos+28, pos+36) if pos != -1 else None
-
+                    smart_meter_values=_decode_sml_iskra_mt175_one_way(self._latest_raw_data)
                     break
             
             if (datetime.now() - time_start) > time_out:
                 self._logger.warning(f"Exceeded time out of {time_out} while reading from smart meter.")
         except serial.SerialException as e:
             self._logger.info("Caught Exception in _read_raw: " + str(e))
             #self._port.close() # TODO: is this needed?
```

### Comparing `smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/sml_reader.py` & `smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/sml_reader.py`

 * *Files identical despite different names*

### Comparing `smart_meter_to_openhab-0.4.1/smart_meter_to_openhab_scripts/main.py` & `smart_meter_to_openhab-0.4.2/smart_meter_to_openhab_scripts/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -47,43 +47,50 @@
 
 def _exec_process(params : List[str]) -> None:
     result = subprocess.run(params, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     rc=result.returncode
     if rc != 0:
         raise Exception("Failed to execute command "+ ' '.join(params)+". Return code was: "+str(result.returncode))
 
-def _run(process_start_time : datetime, logger : logging.Logger, read_count : int, use_uhubctl : bool, 
-         raw_data_dump_dir : Union[Path, None] = None) -> bool:
+def _run(logger : logging.Logger, read_count : int, use_uhubctl : bool, raw_data_dump_dir : Union[Path, None] = None) -> bool:
     from smart_meter_to_openhab.openhab import OpenhabConnection
     from smart_meter_to_openhab.sml_iskra_mt175 import SmlIskraMt175OneWay
     from smart_meter_to_openhab.sml_reader import SmlReader
     from smart_meter_to_openhab.interfaces import SmartMeterValues
+    from smart_meter_to_openhab.utils import add_value_to_rolling_list
 
     oh_user=os.getenv('OH_USER') if 'OH_USER' in os.environ else ''
     oh_passwd=os.getenv('OH_PASSWD') if 'OH_PASSWD' in os.environ else ''
     oh_connection = OpenhabConnection(os.getenv('OH_HOST'), oh_user, oh_passwd, logger) # type: ignore
     sml_iskra = SmlIskraMt175OneWay('/dev/ttyUSB0', logger, raw_data_dump_dir)
     sml_reader = SmlReader(logger)
     logger.info("Connections established. Starting to transfer smart meter values to openhab.")
-    ping_timedelta = timedelta(seconds=read_count*sml_iskra.estimated_max_read_time_in_sec*2.5)
+    desired_number_of_persistence_values=4
+    datetimes_before_post_to_oh=[datetime.now()]*desired_number_of_persistence_values
+    ping_timedelta = timedelta(seconds=read_count*sml_iskra.estimated_max_read_time_in_sec*desired_number_of_persistence_values)
     logger.info(f"Calculated ping_timedelta is {ping_timedelta}. Process will be reinit if no data change is detected in the openHAB DB in the given timeframe.")
+    run_start_time=datetime.now()
     ping_succeeded=False
     while True:
         logger.info("Reading SML data")
         ref_smart_meter_value=oh_connection.get_median_from_items(SmartMeterValues.oh_item_names())
         values, extended_values=sml_reader.read_avg_from_sml_and_compute_extended_values(sml_iskra, read_count, 
                                                                                          ref_values=ref_smart_meter_value)
         logger.info(f"current values: {values}")
         logger.info(f"current extended values: {extended_values}")
+        datetimes_before_post_to_oh=add_value_to_rolling_list(datetimes_before_post_to_oh, datetime.now())
         oh_connection.post_to_items(values)
         oh_connection.post_to_items(extended_values)
         logger.info("Values posted to openHAB")
-        # start pinging after process is running for the specified time
-        if (datetime.now() - process_start_time) > ping_timedelta:
-            if not oh_connection.check_if_persistence_values_updated(SmartMeterValues.oh_item_names(), ping_timedelta, default=sml_iskra.default):
+        # start pinging after running for the specified time
+        if (datetime.now() - run_start_time) > ping_timedelta:
+            # NOTE: exclude the latest values since oh sometimes has not handled the post requests from above yet.
+            if not oh_connection.check_if_persistence_values_updated(SmartMeterValues.oh_item_names(), 
+                                                                     start_time=datetimes_before_post_to_oh[0], 
+                                                                     end_time=datetimes_before_post_to_oh[-1]):
                 break
             ping_succeeded=True
             logger.info("openHAB items ping successful.")
     
     if use_uhubctl:
         logger.error("openHAB items seem to have not been updated - Power off and on usb ports and reinit process")
         # TODO: sudo reboot seems to help a lot more. But lets try this first
@@ -101,18 +108,18 @@
         load_dotenv(dotenv_path=args.dotenv_path)
     logger=create_logger(args.logfile)
     logger.setLevel(logging.INFO)
     logger.info(f"Starting smart_meter_to_openhab version {__version__}")
     logger.setLevel(log_level_from_arg(args.verbose))
     try:
         raw_data_dump_dir=args.raw_data_dump_dir if args.raw_data_dump_dir else None
-        process_start_time=datetime.now()
+        # TODO: remove the reinit thingy. Let it fail and restart by systemd or so
         unsuccessful_reinit_count=0
         while unsuccessful_reinit_count < args.max_reinit:
-            if _run(process_start_time, logger, args.smart_meter_read_count, args.uhubctl, raw_data_dump_dir):
+            if _run(logger, args.smart_meter_read_count, args.uhubctl, raw_data_dump_dir):
                 unsuccessful_reinit_count=0
             else:
                 unsuccessful_reinit_count+=1
                 logger.error("No improvement after reinit. Trying again.")
 
     except Exception as e:
         logger.exception("Caught Exception: " + str(e))
```

### Comparing `smart_meter_to_openhab-0.4.1/PKG-INFO` & `smart_meter_to_openhab-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart_meter_to_openhab
-Version: 0.4.1
+Version: 0.4.2
 Summary: Pushing data of ISKRA MT175 smart meter to openhab
 Home-page: https://github.com/die-bauerei/smart-meter-to-openhab
 Author: Heiko Bauer
 Author-email: heiko_bauer@icloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -42,25 +42,26 @@
 ```
 5. Install smart-meter-to-openhab
 ```bash
 pip install smart-meter-to-openhab
 ```
 6. Provide environment variables. You can e.g. pass a .env file to smart-meter-to-openhab via the option *--dotenv_path*. Or provide them by any other means (e.g. in your ~/.profile).
 ```bash
-# Hostname incl. http(s)
+# Hostname incl. http(s) (required)
 OH_HOST='<http://your_ip:your_port'
 #openhab user (or token) for login (optional)
 OH_USER=''
 #openhab password for login (optional)
 OH_PASSWD=''
-#openhab item names. Optional, but recommended :) 
+#current consumption openhab item (required)
+OVERALL_CONSUMPTION_WATT_OH_ITEM='smart_meter_overall_consumption'
+#other openhab item names (optional)
 PHASE_1_CONSUMPTION_WATT_OH_ITEM='smart_meter_phase_1_consumption'
 PHASE_2_CONSUMPTION_WATT_OH_ITEM='smart_meter_phase_2_consumption'
 PHASE_3_CONSUMPTION_WATT_OH_ITEM='smart_meter_phase_3_consumption'
-OVERALL_CONSUMPTION_WATT_OH_ITEM='smart_meter_overall_consumption'
 OVERALL_CONSUMPTION_WH_OH_ITEM='smart_meter_overall_consumption_wh'
 ELECTRICITY_METER_KWH_OH_ITEM='smart_meter_electricity_meter'
 ```
 NOTE: certificate verification is turned off, in case *OH_HOST* refers to an https address (since most openHAB instances do probably use self-signed certificates)  
 
 7. Run smart-meter-to-openhab with e.g.
 ```bash
```

