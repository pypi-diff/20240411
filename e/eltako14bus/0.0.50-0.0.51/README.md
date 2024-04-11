# Comparing `tmp/eltako14bus-0.0.50.tar.gz` & `tmp/eltako14bus-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eltako14bus-0.0.50.tar", last modified: Tue Apr  2 13:48:50 2024, max compression
+gzip compressed data, was "eltako14bus-0.0.51.tar", last modified: Wed Apr 10 20:09:38 2024, max compression
```

## Comparing `eltako14bus-0.0.50.tar` & `eltako14bus-0.0.51.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:48:50.064133 eltako14bus-0.0.50/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-02 13:48:50.064133 eltako14bus-0.0.50/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:48:50.064133 eltako14bus-0.0.50/eltako14bus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-02 13:48:50.000000 eltako14bus-0.0.50/eltako14bus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-02 13:48:50.000000 eltako14bus-0.0.50/eltako14bus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:48:50.000000 eltako14bus-0.0.50/eltako14bus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 13:48:50.000000 eltako14bus-0.0.50/eltako14bus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 13:48:50.000000 eltako14bus-0.0.50/eltako14bus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:48:50.064133 eltako14bus-0.0.50/eltakobus/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/coap.py
--rw-r--r--   0 runner    (1001) docker     (127)    44440 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    39509 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/eep.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/locking.py
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/eltakobus/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:48:50.064133 eltako14bus-0.0.50/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1108 2024-04-02 13:48:45.000000 eltako14bus-0.0.50/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:38.962202 eltako14bus-0.0.51/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 20:09:33.000000 eltako14bus-0.0.51/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-10 20:09:38.962202 eltako14bus-0.0.51/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-10 20:09:33.000000 eltako14bus-0.0.51/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:38.958202 eltako14bus-0.0.51/eltako14bus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-10 20:09:38.000000 eltako14bus-0.0.51/eltako14bus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-10 20:09:38.000000 eltako14bus-0.0.51/eltako14bus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:09:38.000000 eltako14bus-0.0.51/eltako14bus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-10 20:09:38.000000 eltako14bus-0.0.51/eltako14bus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 20:09:38.000000 eltako14bus-0.0.51/eltako14bus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:38.958202 eltako14bus-0.0.51/eltakobus/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-10 20:09:33.000000 eltako14bus-0.0.51/eltakobus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-10 20:09:33.000000 eltako14bus-0.0.51/eltakobus/bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-10 20:09:33.000000 eltako14bus-0.0.51/eltakobus/coap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44440 2024-04-10 20:09:33.000000 eltako14bus-0.0.51/eltakobus/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43169 2024-04-10 20:09:33.000000 eltako14bus-0.0.51/eltakobus/eep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-10 20:09:33.000000 eltako14bus-0.0.51/eltakobus/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-10 20:09:33.000000 eltako14bus-0.0.51/eltakobus/locking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-10 20:09:33.000000 eltako14bus-0.0.51/eltakobus/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-04-10 20:09:33.000000 eltako14bus-0.0.51/eltakobus/serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-10 20:09:33.000000 eltako14bus-0.0.51/eltakobus/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:09:38.962202 eltako14bus-0.0.51/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1108 2024-04-10 20:09:33.000000 eltako14bus-0.0.51/setup.py
```

### Comparing `eltako14bus-0.0.50/LICENSE` & `eltako14bus-0.0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.50/PKG-INFO` & `eltako14bus-0.0.51/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eltako14bus
-Version: 0.0.50
+Version: 0.0.51
 Summary: Library for participating in the Eltako Series 14 RS485 bus
 Home-page: https://github.com/grimmpp/eltako14bus
 Author: chrysn, grimmpp
 Author-email: chrysn@fsfe.org, grimmpp14@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Description-Content-Type: text/markdown
```

### Comparing `eltako14bus-0.0.50/README.md` & `eltako14bus-0.0.51/README.md`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.50/eltako14bus.egg-info/PKG-INFO` & `eltako14bus-0.0.51/eltako14bus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eltako14bus
-Version: 0.0.50
+Version: 0.0.51
 Summary: Library for participating in the Eltako Series 14 RS485 bus
 Home-page: https://github.com/grimmpp/eltako14bus
 Author: chrysn, grimmpp
 Author-email: chrysn@fsfe.org, grimmpp14@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Description-Content-Type: text/markdown
```

### Comparing `eltako14bus-0.0.50/eltakobus/bus.py` & `eltako14bus-0.0.51/eltakobus/bus.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.50/eltakobus/coap.py` & `eltako14bus-0.0.51/eltakobus/coap.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.50/eltakobus/device.py` & `eltako14bus-0.0.51/eltakobus/device.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.50/eltakobus/eep.py` & `eltako14bus-0.0.51/eltakobus/eep.py`

 * *Files 3% similar despite different names*

```diff
@@ -1307,8 +1307,134 @@
 
     def __init__(self, twilight, day_light, illumination):
         self._twilight = twilight
         self._day_light = day_light
         self._illumination = illumination
 
 class A5_06_01(_BrightnessTwilightSensor):
-    """Brightness Twilight Sensor"""
+    """Brightness Twilight Sensor"""
+
+class _DigitalInputAndBattery(EEP):
+    """Digital Input regarding A5-30-01"""
+
+    @classmethod
+    def decode_message(cls, msg):
+        if msg.org != 0x07:
+            raise WrongOrgError
+        
+        battery_status = msg.data[1]
+        contact_status = msg.data[2]
+        learn_button = (msg.data[3] & 0x08) >> 3
+
+        return cls(battery_status, contact_status, learn_button)
+
+    def encode_message(self, address):
+        data = bytearray([0, 0, 0, 0])
+        
+        data[0] = 0
+        data[1] = self.battery_status
+        data[2] = self.contact_status
+        data[3] = self.learn_button
+
+        status = 0x00
+        
+        return Regular4BSMessage(address, status, data, True)
+    
+    @property
+    def low_battery(self):
+        return self._low_battery
+
+    @property
+    def contact_closed(self):
+        return self._contact_closed
+
+    @property
+    def battery_status(self):
+        return self._battery_status
+    
+    @property
+    def contact_status(self):
+        return self._contact_status
+    
+    @property
+    def learn_button(self):
+        return self._learn_button
+
+    def __init__(self, battery_status, contact_status, learn_button):
+        self._battery_status = battery_status
+        self._contact_status = contact_status
+        self._low_battery = self._battery_status < 121
+        self._contact_closed = self._contact_status < 196
+        self._learn_button = learn_button
+
+class A5_30_01(_DigitalInputAndBattery):
+    """Digital Input with battery status"""
+
+class _DigitalInputsAndTemperature(EEP):
+    """4 Digital Inputs and Temperature"""
+
+    @classmethod
+    def decode_message(cls, msg):
+        if msg.org != 0x07:
+            raise WrongOrgError
+        
+        temperature = msg.data[1] / 255 * 40
+        
+        digital_input_0 = msg.data[2] & 0x01
+        digital_input_1 = (msg.data[2] & 0x02) >> 1
+        digital_input_2 = (msg.data[2] & 0x04) >> 2
+        digital_input_3 = (msg.data[2] & 0x08) >> 3
+        status_of_wake = (msg.data[2] & 0x10) >> 4
+
+        learn_button = (msg.data[3] & 0x08) >> 3
+
+        return cls(temperature, digital_input_0, digital_input_1, digital_input_2, digital_input_3, status_of_wake, learn_button)
+    
+
+    def encode_message(self, address):
+        data = bytearray([0, 0, 0, 0])
+        
+        data[1] = self._temperature / 40 * 255
+
+        data[2] += self.digital_input_0
+        data[2] += self.digital_input_1 << 1
+        data[2] += self.digital_input_2 << 2
+        data[2] += self.digital_input_3 << 3
+        data[2] += self.status_of_wake << 4
+
+        data[3] = self.learn_button
+
+        status = 0x00
+        
+        return Regular4BSMessage(address, status, data, True)
+    
+    @property
+    def digital_input_0(self):
+        return self._digital_input_0
+    
+    @property
+    def digital_input_1(self):
+        return self._digital_input_1
+    
+    @property
+    def digital_input_2(self):
+        return self._digital_input_2
+    
+    @property
+    def digital_input_3(self):
+        return self._digital_input_3
+    
+    @property
+    def status_of_wake(self):
+        return self._status_of_wake
+
+    def __init__(self, temperature, digital_input_0, digital_input_1, digital_input_2, digital_input_3, status_of_wake, learn_button):
+        self._temperature = temperature
+        self._digital_input_0 = digital_input_0
+        self._digital_input_1 = digital_input_1
+        self._digital_input_2 = digital_input_2
+        self._digital_input_3 = digital_input_3
+        self._status_of_wake = status_of_wake
+        self._learn_button = learn_button
+
+class A5_30_03(_DigitalInputsAndTemperature):
+    """Digital Inputs"""
```

### Comparing `eltako14bus-0.0.50/eltakobus/error.py` & `eltako14bus-0.0.51/eltakobus/error.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.50/eltakobus/locking.py` & `eltako14bus-0.0.51/eltakobus/locking.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.50/eltakobus/message.py` & `eltako14bus-0.0.51/eltakobus/message.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.50/eltakobus/serial.py` & `eltako14bus-0.0.51/eltakobus/serial.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.50/eltakobus/util.py` & `eltako14bus-0.0.51/eltakobus/util.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.50/setup.py` & `eltako14bus-0.0.51/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 }
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="eltako14bus",
-    version="0.0.50",
+    version="0.0.51",
     author="chrysn, grimmpp",
     author_email="chrysn@fsfe.org, grimmpp14@gmail.com",
     description="Library for participating in the Eltako Series 14 RS485 bus",
     url="https://github.com/grimmpp/eltako14bus",
     packages=setuptools.find_packages(),
     extras_require=extras_require,
     # Not that there'd be tests, but at least it fetches the right dependencies and syntax checks everything
```

