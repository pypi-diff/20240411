# Comparing `tmp/akips-0.1.5.tar.gz` & `tmp/akips-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akips-0.1.5.tar", max compression
+gzip compressed data, was "akips-0.2.0.tar", max compression
```

## Comparing `akips-0.1.5.tar` & `akips-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1081 2023-09-21 01:11:03.608768 akips-0.1.5/LICENSE
--rw-r--r--   0        0        0     1458 2023-09-25 15:32:31.817902 akips-0.1.5/README.md
--rw-r--r--   0        0        0    10514 2023-10-11 14:22:49.428767 akips-0.1.5/akips/__init__.py
--rw-r--r--   0        0        0      254 2023-09-22 19:01:52.560879 akips-0.1.5/akips/exceptions.py
--rw-r--r--   0        0        0      508 2023-09-26 11:21:29.589483 akips-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2099 1970-01-01 00:00:00.000000 akips-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-09-21 01:11:03.608768 akips-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1458 2023-09-25 15:32:31.817902 akips-0.2.0/README.md
+-rw-r--r--   0        0        0    11909 2024-04-11 13:35:55.005243 akips-0.2.0/akips/__init__.py
+-rw-r--r--   0        0        0      254 2023-09-22 19:01:52.560879 akips-0.2.0/akips/exceptions.py
+-rw-r--r--   0        0        0      508 2024-04-11 12:39:29.825381 akips-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2099 1970-01-01 00:00:00.000000 akips-0.2.0/PKG-INFO
```

### Comparing `akips-0.1.5/LICENSE` & `akips-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `akips-0.1.5/README.md` & `akips-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `akips-0.1.5/akips/__init__.py` & `akips-0.2.0/akips/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 ''' Base module '''
 __version__ = '0.1.5'
 
+import io
 import re
 import logging
 from datetime import datetime
 import requests
 import pytz
+import csv
 
 from akips.exceptions import AkipsError
 
 # Logging configuration
 logger = logging.getLogger(__name__)
 
 
@@ -24,26 +26,30 @@
         self.password = password
         self.verify = verify
         self.session = requests.Session()
 
         if not verify:
             requests.packages.urllib3.disable_warnings()    # pylint: disable=no-member
 
-    def get_devices(self):
+    def get_devices(self, group_filter='any', groups=[]):
         ''' Pull a list of key attributes for all devices in akips '''
         attributes = [
             'ip4addr',
             'SNMPv2-MIB.sysName',
             'SNMPv2-MIB.sysDescr',
             'SNMPv2-MIB.sysLocation'
         ]
         cmd_attributes = "|".join(attributes)
         params = {
             'cmds': f'mget text * sys /{cmd_attributes}/',
         }
+        if groups:
+            ''' [any|all|not group {group name} ...] '''
+            group_list = " ".join(groups)
+            params['cmds'] += f" {group_filter} group {group_list}"
         text = self._get(params=params)
         if text:
             data = {}
             # Data comes back as 'plain/text' type so we have to parse it
             lines = text.split('\n')
             for line in lines:
                 match = re.match(r'^(\S+)\s(\S+)\s(\S+)\s=\s(.*)$', line)
@@ -69,24 +75,24 @@
             lines = text.split('\n')
             for line in lines:
                 match = re.match(r'^(\S+)\s(\S+)\s(\S+)\s=(\s(.*))?$', line)
                 if match:
                     name = match.group(1)
                     if match.group(2) not in data:
                         # initialize the dict of attributes
-                        data[ match.group(2) ] = {}
+                        data[match.group(2)] = {}
                     if match.group(5):
                         # Save this attribute value to data
-                        data[ match.group(2) ][ match.group(3) ] = match.group(5)
+                        data[match.group(2)][match.group(3)] = match.group(5)
                     else:
                         # save a blank string if there was nothing after equals
-                        data[ match.group(2) ][ match.group(3) ] = ''
+                        data[match.group(2)][match.group(3)] = ''
             if name:
                 data['name'] = name
-            logger.debug("Found device {} in akips".format( data ))
+            logger.debug("Found device {} in akips".format(data))
             return data
         return None
 
     def get_device_by_ip(self, ipaddr, use_cache=True):
         ''' Search for a device by an alternate IP address
         This makes use of a special site script and not the normal api '''
         # params = {
@@ -107,40 +113,40 @@
             lines = text.split('\n')
             for line in lines:
                 match = re.match(r'^(\S+)\s(\S+)\s(\S+)\s=\s(\S+),(\S+),(\S+),(\S+),(\S+)?$', line)
                 if match:
                     # epoch fields are in the server's timezone
                     name = match.group(1)
                     attribute = match.group(3)
-                    event_start = datetime.fromtimestamp(int( match.group(7) ), tz=pytz.timezone(self.server_timezone))
+                    event_start = datetime.fromtimestamp(int(match.group(7)), tz=pytz.timezone(self.server_timezone))
                     if name not in data:
                         # populate a starting point for this device
                         data[name] = {
                             'name': name,
                             'ping_state': 'n/a',
                             'snmp_state': 'n/a',
                             'event_start': event_start  # epoch in local timezone
                         }
                     if attribute == 'PING.icmpState':
                         data[name]['child'] = match.group(2),
-                        data[name]['ping_state'] =  match.group(5)
+                        data[name]['ping_state'] = match.group(5)
                         data[name]['index'] = match.group(4)
-                        data[name]['device_added'] = datetime.fromtimestamp(int( match.group(6) ), tz=pytz.timezone(self.server_timezone))
-                        data[name]['event_start'] = datetime.fromtimestamp(int( match.group(7) ), tz=pytz.timezone(self.server_timezone))
+                        data[name]['device_added'] = datetime.fromtimestamp(int(match.group(6)), tz=pytz.timezone(self.server_timezone))
+                        data[name]['event_start'] = datetime.fromtimestamp(int(match.group(7)), tz=pytz.timezone(self.server_timezone))
                         data[name]['ip4addr'] = match.group(8)
                     elif attribute == 'SNMP.snmpState':
                         data[name]['child'] = match.group(2),
-                        data[name]['snmp_state'] =  match.group(5)
+                        data[name]['snmp_state'] = match.group(5)
                         data[name]['index'] = match.group(4)
-                        data[name]['device_added'] = datetime.fromtimestamp(int( match.group(6) ), tz=pytz.timezone(self.server_timezone))
-                        data[name]['event_start'] = datetime.fromtimestamp(int( match.group(7) ), tz=pytz.timezone(self.server_timezone))
+                        data[name]['device_added'] = datetime.fromtimestamp(int(match.group(6)), tz=pytz.timezone(self.server_timezone))
+                        data[name]['event_start'] = datetime.fromtimestamp(int(match.group(7)), tz=pytz.timezone(self.server_timezone))
                         data[name]['ip4addr'] = None
                     if event_start < data[name]['event_start']:
                         data[name]['event_start'] = event_start
-            logger.debug("Found {} devices in akips".format( len( data )))
+            logger.debug("Found {} devices in akips".format(len(data)))
             logger.debug("data: {}".format(data))
 
         # for name in data:
         #     # Fill in the unreported gaps so we have ping4 and snmp up/down data
         #     if data[name]['ping_state'] == 'n/a':
         #         ping_status = self.get_status(device=name, child='ping4', attribute='PING.icmpState')
 
@@ -163,16 +169,16 @@
             # Data comes back as 'plain/text' type so we have to parse it
             lines = text.split('\n')
             for line in lines:
                 match = re.match(r'^(\S+)\s=\s(.*)$', line)
                 if match:
                     if match.group(1) not in data:
                         # Populate a default entry for all desired fields
-                        data[ match.group(1) ] = match.group(2).split(',')
-            logger.debug("Found {} device and group mappings in akips".format( len( data.keys() )))
+                        data[match.group(1)] = match.group(2).split(',')
+            logger.debug("Found {} device and group mappings in akips".format(len(data.keys())))
             return data
         return None
 
     def get_maintenance_mode(self):
         ''' Pull a list of devices in maintenance mode '''
         # params = {
         #     'cmds': 'mget * * any group maintenance_mode',
@@ -220,14 +226,44 @@
                         'details': match.group(7),
                     }
                     data.append(entry)
             logger.debug("Found {} events of type {} in akips".format(len(data), type))
             return data
         return None
 
+    ### Time-series commands
+
+    def get_series(self, period='last1h', device='*', attribute='*', group_filter='any', groups=[], get_dict=True):
+        ''' Pull a series of values.  Command syntax:
+            cseries avg 
+            time {time filter] type parent child attribute
+            [any|all|not group {group name} ...] '''
+        params = {
+            'cmds': f'cseries avg time {period} * {device} * {attribute}'
+        }
+        if groups:
+            group_list = " ".join(groups)
+            params['cmds'] += f" {group_filter} group {group_list}"
+        text = self._get(params=params)
+        if text:
+            # Parse output in CSV format
+            buff = io.StringIO(text)
+            if get_dict:
+                # parse each row as a dictionary, key will be column header
+                reader = csv.DictReader(buff)
+            else:
+                # parse each row as a list, will have a column header row
+                reader = csv.reader(buff)
+            csv_to_list = [row for row in reader]
+            logger.debug("Found {} series entries".format(len(csv_to_list)))
+            return csv_to_list
+        return None
+
+    ### Base operations
+
     def _get(self, section='/api-db/', params=None, timeout=30):
         ''' Call HTTP GET against the AKiPS server '''
         server_url = 'https://' + self.server + section
         params['username'] = self.username
         params['password'] = self.password
 
         try:
```

### Comparing `akips-0.1.5/PKG-INFO` & `akips-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akips
-Version: 0.1.5
+Version: 0.2.0
 Summary: Module to interact with the AKiPS Network Monitoring Software API interface
 Home-page: https://github.com/wwhitaker/akips
 License: MIT
 Author: William E Whitaker
 Author-email: will.whitaker@unc.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

