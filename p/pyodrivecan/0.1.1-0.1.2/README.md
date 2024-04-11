# Comparing `tmp/pyodrivecan-0.1.1.tar.gz` & `tmp/pyodrivecan-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodrivecan-0.1.1.tar", last modified: Fri Apr  5 00:33:18 2024, max compression
+gzip compressed data, was "pyodrivecan-0.1.2.tar", last modified: Wed Apr 10 18:46:51 2024, max compression
```

## Comparing `pyodrivecan-0.1.1.tar` & `pyodrivecan-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:33:18.437115 pyodrivecan-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 00:33:12.000000 pyodrivecan-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-05 00:33:18.437115 pyodrivecan-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-05 00:33:18.437115 pyodrivecan-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 00:33:12.000000 pyodrivecan-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:33:18.433115 pyodrivecan-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:33:18.437115 pyodrivecan-0.1.1/src/pyodrivecan/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-05 00:33:12.000000 pyodrivecan-0.1.1/src/pyodrivecan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-04-05 00:33:12.000000 pyodrivecan-0.1.1/src/pyodrivecan/odrivedatabase.py
--rw-r--r--   0 runner    (1001) docker     (127)    48375 2024-04-05 00:33:12.000000 pyodrivecan-0.1.1/src/pyodrivecan/pyodrivecan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:33:18.437115 pyodrivecan-0.1.1/src/pyodrivecan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-05 00:33:18.000000 pyodrivecan-0.1.1/src/pyodrivecan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-05 00:33:18.000000 pyodrivecan-0.1.1/src/pyodrivecan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:33:18.000000 pyodrivecan-0.1.1/src/pyodrivecan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 00:33:18.000000 pyodrivecan-0.1.1/src/pyodrivecan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 00:33:18.000000 pyodrivecan-0.1.1/src/pyodrivecan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:46:51.399137 pyodrivecan-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-10 18:46:47.000000 pyodrivecan-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-10 18:46:51.399137 pyodrivecan-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-10 18:46:51.399137 pyodrivecan-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-10 18:46:47.000000 pyodrivecan-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:46:51.395137 pyodrivecan-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:46:51.399137 pyodrivecan-0.1.2/src/pyodrivecan/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-10 18:46:47.000000 pyodrivecan-0.1.2/src/pyodrivecan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-04-10 18:46:47.000000 pyodrivecan-0.1.2/src/pyodrivecan/odrivedatabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48997 2024-04-10 18:46:47.000000 pyodrivecan-0.1.2/src/pyodrivecan/pyodrivecan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:46:51.399137 pyodrivecan-0.1.2/src/pyodrivecan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-10 18:46:51.000000 pyodrivecan-0.1.2/src/pyodrivecan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-10 18:46:51.000000 pyodrivecan-0.1.2/src/pyodrivecan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 18:46:51.000000 pyodrivecan-0.1.2/src/pyodrivecan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 18:46:51.000000 pyodrivecan-0.1.2/src/pyodrivecan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 18:46:51.000000 pyodrivecan-0.1.2/src/pyodrivecan.egg-info/top_level.txt
```

### Comparing `pyodrivecan-0.1.1/LICENSE` & `pyodrivecan-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodrivecan-0.1.1/PKG-INFO` & `pyodrivecan-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodrivecan
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for controlling O-Drive Motor Controller using can with Python.
 Home-page: https://github.com/dylanballback/ODriveCan
 Author: Dylan Ballback
 Author-email: dylanballback19@gmail.com
 License: mit
 Keywords: O-Drive,CAN,Python
 Classifier: Topic :: Printing
```

### Comparing `pyodrivecan-0.1.1/setup.cfg` & `pyodrivecan-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyodrivecan-0.1.1/src/pyodrivecan/odrivedatabase.py` & `pyodrivecan-0.1.2/src/pyodrivecan/odrivedatabase.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,17 @@
             torque_target REAL,
             torque_estimate REAL,
             bus_voltage REAL,
             bus_current REAL,
             iq_setpoint REAL,
             iq_measured REAL,
             electrical_power REAL,
-            mechanical_power REAL
+            mechanical_power REAL, 
+            fet_temp REAL, 
+            motor_temp REAL
         );
         """
         self.execute(sql)
 
 
 
     def create_user_defined_table(self, table_name, columns):
@@ -232,43 +234,43 @@
                 return 1  # If table is empty, start with 1
         except Error as e:
             print(e)
             return 1  # Default to 1 if there's an issue
 
 
 
-    def add_odrive_data(self, trial_id, node_ID, time, position, velocity, torque_target, torque_estimate, bus_voltage, bus_current, iq_setpoint, iq_measured, electrical_power, mechanical_power):
+    def add_odrive_data(self, trial_id, node_ID, time, position, velocity, torque_target, torque_estimate, bus_voltage, bus_current, iq_setpoint, iq_measured, electrical_power, mechanical_power, fet_temp, motor_temp):
         """
         Inserts data into the ODriveData table.
 
         Para:
             trial_id, node_ID, time, position, velocity, torque_target, torque_estimate, bus_voltage, bus_current, iq_setpoint, iq_measured, electrical_power, mechanical_power - Fields representing the data to be inserted into the ODriveData table.
 
         Returns:
             The row ID of the last row this INSERT modified, or None on failure.
 
         Example:
             >>> database.add_odrive_data(1, 'node_1', '2024-02-09 10:00:00', 123.45, 67.89, 2.34, 2.30, 48.0, 1.5, 3.33, 3.30, 120, 110)
             ...
             ... 1
         """
-        sql = '''INSERT INTO ODriveData(trial_id, node_ID, time, position, velocity, torque_target, torque_estimate, bus_voltage, bus_current, iq_setpoint, iq_measured, electrical_power, mechanical_power)
-                 VALUES(?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?);'''
-        return self.execute(sql, (trial_id, node_ID, time, position, velocity, torque_target, torque_estimate, bus_voltage, bus_current, iq_setpoint, iq_measured, electrical_power, mechanical_power))
+        sql = '''INSERT INTO ODriveData(trial_id, node_ID, time, position, velocity, torque_target, torque_estimate, bus_voltage, bus_current, iq_setpoint, iq_measured, electrical_power, mechanical_power, fet_temp, motor_temp)
+                 VALUES(?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?);'''
+        return self.execute(sql, (trial_id, node_ID, time, position, velocity, torque_target, torque_estimate, bus_voltage, bus_current, iq_setpoint, iq_measured, electrical_power, mechanical_power, fet_temp, motor_temp))
 
 
     def bulk_insert_odrive_data(self, data_list):
         """Inserts multiple data records into the database."""
         conn = self.create_connection()  # Create a new connection
         try:
             c = conn.cursor()
             for data in data_list:
-                sql = '''INSERT INTO ODriveData(trial_id, node_ID, time, position, velocity, torque_target, torque_estimate, bus_voltage, bus_current, iq_setpoint, iq_measured, electrical_power, mechanical_power)
+                sql = '''INSERT INTO ODriveData(trial_id, node_ID, time, position, velocity, torque_target, torque_estimate, bus_voltage, bus_current, iq_setpoint, iq_measured, electrical_power, mechanical_power, fet_temp, motor_temp )
                          VALUES(?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?);'''
-                params = (data['trial_id'], data['node_ID'], data['time'], data['position'], data['velocity'], data['torque_target'], data['torque_estimate'], data['bus_voltage'], data['bus_current'], data['iq_setpoint'], data['iq_measured'], data['electrical_power'], data['mechanical_power'])
+                params = (data['trial_id'], data['node_ID'], data['time'], data['position'], data['velocity'], data['torque_target'], data['torque_estimate'], data['bus_voltage'], data['bus_current'], data['iq_setpoint'], data['iq_measured'], data['electrical_power'], data['mechanical_power'], data['fet_temp'], data['motor_temp'])
                 c.execute(sql, params)
             conn.commit()
         except Error as e:
             print(e)
         finally:
             conn.close()
```

### Comparing `pyodrivecan-0.1.1/src/pyodrivecan/pyodrivecan.py` & `pyodrivecan-0.1.2/src/pyodrivecan/pyodrivecan.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
         nodeID             (int): The node ID of the O-Drive controller on the CAN network.
         position           (float, optional): The current position of the motor in revolutions. Defaults to None.
         velocity           (float, optional): The current velocity of the motor in revolutions per second. Defaults to None.
         torque_target      (float, optional): The target torque for the motor. Defaults to None.
         torque_estimate    (float, optional): The estimated torque of the motor. Defaults to None.
         bus_voltage        (float, optional): The current bus voltage of the O-Drive. Defaults to None.
         bus_current        (float, optional): The current bus current of the O-Drive. Defaults to None.
+        fet_temp           (float, optional): The O-Drive measured FET temperature. Defaults to None.
+        motor_temp         (float, optional): The O-Drive measured Motor temperature. Defaults to None.
         iq_setpoint        (float, optional): The setpoint current in the q-axis of the motor's dq frame. Defaults to None.
         iq_measured        (float, optional): The measured current in the q-axis of the motor's dq frame. Defaults to None.
         electrical_power   (float, optional): The calculated electrical power being delivered to the motor. Defaults to None.
         mechanical_power   (float, optional): The calculated mechanical power being produced by the motor. Defaults to None.
         error_messages     (str, optional): Any error messages that are generated by the O-Drive. Defaults to None.
         database           (str): The path to the database file used for storing O-Drive data. Defaults to 'odrive_data.db'.
         running            (bool): A flag indicating if the main event loop is running.
@@ -102,14 +104,16 @@
             velocity=None,
             torque_target=None,
             torque_estimate=None,
             bus_voltage=None,
             bus_current=None,
             iq_setpoint=None,
             iq_measured=None,
+            fet_temp=None,
+            motor_temp=None,
             electrical_power=None,
             mechanical_power=None,
             error_messages = None,
             database='odrive_data.db',
             active_error = None,
             disarm_reason = None
             ):
@@ -904,14 +908,19 @@
             self.iq_measured = iq_measured
             #print(f"IQ Setpoint and Measured - Setpoint: {iq_setpoint:.3f} A, Measured: {iq_measured:.3f} A")
         elif arbitration_id == (self.nodeID << 5 | 0x1D):  # Powers
             electrical_power, mechanical_power = struct.unpack('<ff', data)
             self.electrical_power = electrical_power
             self.mechanical_power = mechanical_power
             #print(f"Powers - Electrical: {electrical_power:.3f} W, Mechanical: {mechanical_power:.3f} W")
+        elif arbitration_id == (self.nodeID << 5 | 0x15): # Get_Temperature
+            fet_temp, motor_temp = struct.unpack('<ff', data)
+            self.fet_temp = fet_temp
+            self.motor_temp = motor_temp
+            #print(f"Temps - FET: {fet_temp:.3f} C, Motor: {motor_temp:.3f} C")
         elif arbitration_id == (self.nodeID << 5 | 0x03):  # Get_Error message
             active_errors, disarm_reason = struct.unpack('<II', data)
             # Decode and print active errors
             if active_errors != 0:  # Check if there are any active errors
                 errors = [description for code, description in self.ERROR_CODES.items() if active_errors & code]
                 self.active_error = ', '.join(errors)
                 print(f"ODrive {self.nodeID} Active Errors: {self.active_error}")
@@ -960,15 +969,17 @@
                 self.torque_target,
                 self.torque_estimate,
                 self.bus_voltage,
                 self.bus_current,
                 self.iq_setpoint,
                 self.iq_measured,
                 self.electrical_power,
-                self.mechanical_power
+                self.mechanical_power,
+                self.fet_temp,
+                self.motor_temp
             )
 
 
     async def get_velocity(self):
         """
         This function makes sure that the returned velocity is not 'None'
         """
```

### Comparing `pyodrivecan-0.1.1/src/pyodrivecan.egg-info/PKG-INFO` & `pyodrivecan-0.1.2/src/pyodrivecan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodrivecan
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for controlling O-Drive Motor Controller using can with Python.
 Home-page: https://github.com/dylanballback/ODriveCan
 Author: Dylan Ballback
 Author-email: dylanballback19@gmail.com
 License: mit
 Keywords: O-Drive,CAN,Python
 Classifier: Topic :: Printing
```

