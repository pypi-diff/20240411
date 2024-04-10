# Comparing `tmp/ledsc-1.0.2.tar.gz` & `tmp/ledsc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledsc-1.0.2.tar", last modified: Wed Apr 10 21:31:14 2024, max compression
+gzip compressed data, was "ledsc-1.0.3.tar", last modified: Wed Apr 10 21:48:38 2024, max compression
```

## Comparing `ledsc-1.0.2.tar` & `ledsc-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-10 21:31:14.465274 ledsc-1.0.2/
--rw-r--r--   0 hell      (1000) hell      (1000)      985 2024-04-10 21:31:14.465274 ledsc-1.0.2/PKG-INFO
--rw-r--r--   0 hell      (1000) hell      (1000)      558 2024-03-14 21:51:08.000000 ledsc-1.0.2/README.md
-drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-10 21:31:14.465274 ledsc-1.0.2/ledsc/
--rw-r--r--   0 hell      (1000) hell      (1000)       43 2024-03-15 08:08:09.000000 ledsc-1.0.2/ledsc/__init__.py
--rw-r--r--   0 hell      (1000) hell      (1000)     7257 2024-04-10 21:30:26.000000 ledsc-1.0.2/ledsc/ledsc.py
-drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-10 21:31:14.465274 ledsc-1.0.2/ledsc.egg-info/
--rw-r--r--   0 hell      (1000) hell      (1000)      985 2024-04-10 21:31:14.000000 ledsc-1.0.2/ledsc.egg-info/PKG-INFO
--rw-rw-r--   0 hell      (1000) hell      (1000)      201 2024-04-10 21:31:14.000000 ledsc-1.0.2/ledsc.egg-info/SOURCES.txt
--rw-rw-r--   0 hell      (1000) hell      (1000)        1 2024-04-10 21:31:14.000000 ledsc-1.0.2/ledsc.egg-info/dependency_links.txt
--rw-rw-r--   0 hell      (1000) hell      (1000)       30 2024-04-10 21:31:14.000000 ledsc-1.0.2/ledsc.egg-info/requires.txt
--rw-rw-r--   0 hell      (1000) hell      (1000)        6 2024-04-10 21:31:14.000000 ledsc-1.0.2/ledsc.egg-info/top_level.txt
--rw-r--r--   0 hell      (1000) hell      (1000)      437 2024-04-10 21:30:26.000000 ledsc-1.0.2/pyproject.toml
--rw-rw-r--   0 hell      (1000) hell      (1000)       38 2024-04-10 21:31:14.465274 ledsc-1.0.2/setup.cfg
+drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-10 21:48:38.757357 ledsc-1.0.3/
+-rw-r--r--   0 hell      (1000) hell      (1000)      985 2024-04-10 21:48:38.757357 ledsc-1.0.3/PKG-INFO
+-rw-r--r--   0 hell      (1000) hell      (1000)      558 2024-03-14 21:51:08.000000 ledsc-1.0.3/README.md
+drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-10 21:48:38.753357 ledsc-1.0.3/ledsc/
+-rw-r--r--   0 hell      (1000) hell      (1000)       43 2024-04-10 21:45:20.000000 ledsc-1.0.3/ledsc/__init__.py
+-rw-r--r--   0 hell      (1000) hell      (1000)     7487 2024-04-10 21:47:03.000000 ledsc-1.0.3/ledsc/ledsc.py
+drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-04-10 21:48:38.757357 ledsc-1.0.3/ledsc.egg-info/
+-rw-r--r--   0 hell      (1000) hell      (1000)      985 2024-04-10 21:48:38.000000 ledsc-1.0.3/ledsc.egg-info/PKG-INFO
+-rw-rw-r--   0 hell      (1000) hell      (1000)      201 2024-04-10 21:48:38.000000 ledsc-1.0.3/ledsc.egg-info/SOURCES.txt
+-rw-rw-r--   0 hell      (1000) hell      (1000)        1 2024-04-10 21:48:38.000000 ledsc-1.0.3/ledsc.egg-info/dependency_links.txt
+-rw-rw-r--   0 hell      (1000) hell      (1000)       30 2024-04-10 21:48:38.000000 ledsc-1.0.3/ledsc.egg-info/requires.txt
+-rw-rw-r--   0 hell      (1000) hell      (1000)        6 2024-04-10 21:48:38.000000 ledsc-1.0.3/ledsc.egg-info/top_level.txt
+-rw-r--r--   0 hell      (1000) hell      (1000)      437 2024-04-10 21:45:20.000000 ledsc-1.0.3/pyproject.toml
+-rw-rw-r--   0 hell      (1000) hell      (1000)       38 2024-04-10 21:48:38.757357 ledsc-1.0.3/setup.cfg
```

### Comparing `ledsc-1.0.2/PKG-INFO` & `ledsc-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledsc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for communicate with led string controller
 Author-email: Patrik Kratochvil <info@ledsc.eu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ledsc-1.0.2/README.md` & `ledsc-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ledsc-1.0.2/ledsc/ledsc.py` & `ledsc-1.0.3/ledsc/ledsc.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     EE_LDF_R = 1008  # LED controller default color R
     EE_LDF_G = 1009  # LED controller default color G
     EE_LDF_B = 1010  # LED controller default color B
     EE_LDF_W = 1011  # LED controller default color W
     EE_GR = 1012  # Greeting enable
     EE_PXEN = 1013  # proximity sensor enable
     EE_PWMC = 1014  # PWM cycle
+    EE_LOS = 1015  # Light on start
 
 
 class LedSC:
     def __init__(self, modbus_client: ModbusSerialClient, slave_id: int):
         self.client = modbus_client
         self.slave_id = slave_id
         if self.slave_id == 0:
@@ -180,14 +181,17 @@
 
     def set_default_rgbw(self, red: int, green: int, blue: int, white: int):
         self.write_registers(REG.EE_LDF_R.value, [red, green, blue, white])
 
     def set_default_transition_time(self, value: int):
         self.write_register(REG.EE_LDF_TR.value, value)
 
+    def set_light_on_start(self, value: int):
+        self.write_register(REG.EE_LOS.value, value)
+
     def get_mb_slave_id(self) -> int:
         return self.read_register(REG.EE_MBADDR.value)
 
     def get_serial_baudrate(self) -> int:
         return self.read_register(REG.EE_SBAUD.value)
 
     def get_serial_parity(self) -> int:
@@ -206,7 +210,10 @@
         return self.read_register(REG.EE_PWMC.value)
 
     def get_default_rgbw(self) -> List[int]:
         return self.read_register(REG.EE_LDF_R.value, count=4)
 
     def get_default_transition_time(self) -> int:
         return self.read_register(REG.EE_LDF_TR.value)
+
+    def get_light_on_start(self) -> int:
+        return self.read_register(REG.EE_LOS.value)
```

### Comparing `ledsc-1.0.2/ledsc.egg-info/PKG-INFO` & `ledsc-1.0.3/ledsc.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledsc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for communicate with led string controller
 Author-email: Patrik Kratochvil <info@ledsc.eu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

