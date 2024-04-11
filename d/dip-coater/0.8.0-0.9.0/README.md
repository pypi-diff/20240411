# Comparing `tmp/dip-coater-0.8.0.tar.gz` & `tmp/dip-coater-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dip-coater-0.8.0.tar", last modified: Mon Apr  8 16:35:41 2024, max compression
+gzip compressed data, was "dip-coater-0.9.0.tar", last modified: Tue Apr  9 07:55:17 2024, max compression
```

## Comparing `dip-coater-0.8.0.tar` & `dip-coater-0.9.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 16:35:41.123197 dip-coater-0.8.0/
--rw-r--r--   0 rik      (459800007) staff       (20)      100 2024-04-05 10:30:51.000000 dip-coater-0.8.0/MANIFEST.in
--rw-r--r--   0 rik      (459800007) staff       (20)     1994 2024-04-08 16:35:41.122976 dip-coater-0.8.0/PKG-INFO
--rw-r--r--   0 rik      (459800007) staff       (20)     1292 2024-04-08 07:44:49.000000 dip-coater-0.8.0/README.md
--rw-r--r--   0 rik      (459800007) staff       (20)     1008 2024-04-08 16:31:27.000000 dip-coater-0.8.0/pyproject.toml
--rw-r--r--   0 rik      (459800007) staff       (20)       38 2024-04-08 16:35:41.123268 dip-coater-0.8.0/setup.cfg
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 16:35:41.118648 dip-coater-0.8.0/src/
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 16:35:41.119623 dip-coater-0.8.0/src/MyRPi/
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 16:35:41.119797 dip-coater-0.8.0/src/MyRPi/GPIO/
--rw-r--r--   0 rik      (459800007) staff       (20)       26 2024-04-05 10:42:43.000000 dip-coater-0.8.0/src/MyRPi/GPIO/__init__.py
--rw-r--r--   0 rik      (459800007) staff       (20)      220 2024-04-04 11:42:49.000000 dip-coater-0.8.0/src/MyRPi/_GPIO.py
--rw-r--r--   0 rik      (459800007) staff       (20)        0 2024-04-04 11:31:25.000000 dip-coater-0.8.0/src/MyRPi/__init__.py
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 16:35:41.120778 dip-coater-0.8.0/src/MyTMC_2209/
--rw-r--r--   0 rik      (459800007) staff       (20)      707 2024-04-08 16:31:27.000000 dip-coater-0.8.0/src/MyTMC_2209/TMC_2209_StepperDriver.py
--rw-r--r--   0 rik      (459800007) staff       (20)      362 2024-04-08 16:31:27.000000 dip-coater-0.8.0/src/MyTMC_2209/_TMC_2209_comm.py
--rw-r--r--   0 rik      (459800007) staff       (20)      307 2024-04-08 16:31:27.000000 dip-coater-0.8.0/src/MyTMC_2209/_TMC_2209_logger.py
--rw-r--r--   0 rik      (459800007) staff       (20)        0 2024-04-08 16:31:27.000000 dip-coater-0.8.0/src/MyTMC_2209/__init__.py
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 16:35:41.121598 dip-coater-0.8.0/src/dip_coater/
--rw-r--r--   0 rik      (459800007) staff       (20)        0 2024-04-05 10:07:42.000000 dip-coater-0.8.0/src/dip_coater/__init__.py
--rw-r--r--   0 rik      (459800007) staff       (20)      926 2024-04-08 16:31:27.000000 dip-coater-0.8.0/src/dip_coater/help.md
--rw-r--r--   0 rik      (459800007) staff       (20)     4606 2024-04-08 16:31:27.000000 dip-coater-0.8.0/src/dip_coater/motor.py
--rw-r--r--   0 rik      (459800007) staff       (20)    14262 2024-04-08 16:31:27.000000 dip-coater-0.8.0/src/dip_coater/tui.py
--rw-r--r--   0 rik      (459800007) staff       (20)     2318 2024-04-08 16:31:27.000000 dip-coater-0.8.0/src/dip_coater/tui.tcss
-drwxr-xr-x   0 rik      (459800007) staff       (20)        0 2024-04-08 16:35:41.122588 dip-coater-0.8.0/src/dip_coater.egg-info/
--rw-r--r--   0 rik      (459800007) staff       (20)     1994 2024-04-08 16:35:41.000000 dip-coater-0.8.0/src/dip_coater.egg-info/PKG-INFO
--rw-r--r--   0 rik      (459800007) staff       (20)      590 2024-04-08 16:35:41.000000 dip-coater-0.8.0/src/dip_coater.egg-info/SOURCES.txt
--rw-r--r--   0 rik      (459800007) staff       (20)        1 2024-04-08 16:35:41.000000 dip-coater-0.8.0/src/dip_coater.egg-info/dependency_links.txt
--rw-r--r--   0 rik      (459800007) staff       (20)       51 2024-04-08 16:35:41.000000 dip-coater-0.8.0/src/dip_coater.egg-info/entry_points.txt
--rw-r--r--   0 rik      (459800007) staff       (20)       58 2024-04-08 16:35:41.000000 dip-coater-0.8.0/src/dip_coater.egg-info/requires.txt
--rw-r--r--   0 rik      (459800007) staff       (20)       28 2024-04-08 16:35:41.000000 dip-coater-0.8.0/src/dip_coater.egg-info/top_level.txt
+drwxr-xr-x   0 sibo     (459882621) sibo     (459882621)        0 2024-04-09 07:55:17.622025 dip-coater-0.9.0/
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)      100 2024-04-08 17:03:07.000000 dip-coater-0.9.0/MANIFEST.in
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)     2205 2024-04-09 07:55:17.621836 dip-coater-0.9.0/PKG-INFO
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)     1480 2024-04-09 07:53:04.000000 dip-coater-0.9.0/README.md
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)     1012 2024-04-09 07:53:04.000000 dip-coater-0.9.0/pyproject.toml
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)       38 2024-04-09 07:55:17.622066 dip-coater-0.9.0/setup.cfg
+drwxr-xr-x   0 sibo     (459882621) sibo     (459882621)        0 2024-04-09 07:55:17.618247 dip-coater-0.9.0/src/
+drwxr-xr-x   0 sibo     (459882621) sibo     (459882621)        0 2024-04-09 07:55:17.619227 dip-coater-0.9.0/src/MyRPi/
+drwxr-xr-x   0 sibo     (459882621) sibo     (459882621)        0 2024-04-09 07:55:17.619345 dip-coater-0.9.0/src/MyRPi/GPIO/
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)       26 2024-04-08 17:03:07.000000 dip-coater-0.9.0/src/MyRPi/GPIO/__init__.py
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)      220 2024-04-08 17:03:07.000000 dip-coater-0.9.0/src/MyRPi/_GPIO.py
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)        0 2024-04-08 17:03:07.000000 dip-coater-0.9.0/src/MyRPi/__init__.py
+drwxr-xr-x   0 sibo     (459882621) sibo     (459882621)        0 2024-04-09 07:55:17.619993 dip-coater-0.9.0/src/MyTMC_2209/
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)      774 2024-04-09 07:53:04.000000 dip-coater-0.9.0/src/MyTMC_2209/TMC_2209_StepperDriver.py
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)      362 2024-04-08 17:03:07.000000 dip-coater-0.9.0/src/MyTMC_2209/_TMC_2209_comm.py
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)      307 2024-04-08 17:03:07.000000 dip-coater-0.9.0/src/MyTMC_2209/_TMC_2209_logger.py
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)        0 2024-04-08 17:03:07.000000 dip-coater-0.9.0/src/MyTMC_2209/__init__.py
+drwxr-xr-x   0 sibo     (459882621) sibo     (459882621)        0 2024-04-09 07:55:17.620638 dip-coater-0.9.0/src/dip_coater/
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)        0 2024-04-08 17:03:07.000000 dip-coater-0.9.0/src/dip_coater/__init__.py
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)      926 2024-04-08 17:03:07.000000 dip-coater-0.9.0/src/dip_coater/help.md
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)     4745 2024-04-09 07:53:04.000000 dip-coater-0.9.0/src/dip_coater/motor.py
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)    14251 2024-04-09 07:53:04.000000 dip-coater-0.9.0/src/dip_coater/tui.py
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)     2318 2024-04-08 17:03:07.000000 dip-coater-0.9.0/src/dip_coater/tui.tcss
+drwxr-xr-x   0 sibo     (459882621) sibo     (459882621)        0 2024-04-09 07:55:17.621491 dip-coater-0.9.0/src/dip_coater.egg-info/
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)     2205 2024-04-09 07:55:17.000000 dip-coater-0.9.0/src/dip_coater.egg-info/PKG-INFO
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)      590 2024-04-09 07:55:17.000000 dip-coater-0.9.0/src/dip_coater.egg-info/SOURCES.txt
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)        1 2024-04-09 07:55:17.000000 dip-coater-0.9.0/src/dip_coater.egg-info/dependency_links.txt
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)       51 2024-04-09 07:55:17.000000 dip-coater-0.9.0/src/dip_coater.egg-info/entry_points.txt
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)       65 2024-04-09 07:55:17.000000 dip-coater-0.9.0/src/dip_coater.egg-info/requires.txt
+-rw-r--r--   0 sibo     (459882621) sibo     (459882621)       28 2024-04-09 07:55:17.000000 dip-coater-0.9.0/src/dip_coater.egg-info/top_level.txt
```

### Comparing `dip-coater-0.8.0/PKG-INFO` & `dip-coater-0.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,61 @@
 Metadata-Version: 2.1
 Name: dip-coater
-Version: 0.8.0
+Version: 0.9.0
 Author-email: Rik Huygen <rik.huygen@kuleuven.be>, Sibo Van Gool <sibo.vangool@kuleuven.be>
 License: MIT License
 Project-URL: repository, https://github.com/IvS-KULeuven/dip_coater
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: textual
 Requires-Dist: textual-dev
-Requires-Dist: TMC-2209-Raspberry-Pi
 Provides-Extra: rpi
 Requires-Dist: RPi.GPIO; extra == "rpi"
+Requires-Dist: TMC-2209-Raspberry-Pi>=0.4.3; extra == "rpi"
 
 # The Dip Coater App
 
 This small App is developed for IvS to drive the motor for the dip coater. The motor is connected to a Raspberry Pi through the GPIO bus.
 
-This App is develop with [Textual](https://www.textualize.io).
+This App is developed with [Textual](https://www.textualize.io).
 
 ## Installation
 
 Always install in a dedicated virtual environment!
 
+```bash
+$ cd </path/to/dip-coater>
+$ python3 -m venv venv --prompt=dip-coater
+$ source venv/bin/activate
+$ pip install --upgrade pip setuptools wheel
+$ pip install -e .
+```
+
 On a Raspberry Pi, install the project together with the RPi package:
 
-```
+```bash
 $ pip install dip-coater[rpi] 
 ```
 
 When you want to develop and test on a macOS or Linux system, install without the RPi package. The App will mock the imports and functions.
 
-```
+```bash
 $ pip install dip-coater
 ```
 
 ## Usage
 
 Start the App from the command line in a terminal. You can start it also from a remote ssh session in a terminal, e.g. if you have the installation on the Raspberry Pi and you have a remote connection to your RPi.
 
-```
+```bash
 $ dip-coater
 ```
 
 This will show the following App in your terminal:
 
 ![](https://raw.githubusercontent.com/IvS-KULeuven/dip_coater/develop/images/dip-coater-dark.png)
```

### Comparing `dip-coater-0.8.0/README.md` & `dip-coater-0.9.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 # The Dip Coater App
 
 This small App is developed for IvS to drive the motor for the dip coater. The motor is connected to a Raspberry Pi through the GPIO bus.
 
-This App is develop with [Textual](https://www.textualize.io).
+This App is developed with [Textual](https://www.textualize.io).
 
 ## Installation
 
 Always install in a dedicated virtual environment!
 
+```bash
+$ cd </path/to/dip-coater>
+$ python3 -m venv venv --prompt=dip-coater
+$ source venv/bin/activate
+$ pip install --upgrade pip setuptools wheel
+$ pip install -e .
+```
+
 On a Raspberry Pi, install the project together with the RPi package:
 
-```
+```bash
 $ pip install dip-coater[rpi] 
 ```
 
 When you want to develop and test on a macOS or Linux system, install without the RPi package. The App will mock the imports and functions.
 
-```
+```bash
 $ pip install dip-coater
 ```
 
 ## Usage
 
 Start the App from the command line in a terminal. You can start it also from a remote ssh session in a terminal, e.g. if you have the installation on the Raspberry Pi and you have a remote connection to your RPi.
 
-```
+```bash
 $ dip-coater
 ```
 
 This will show the following App in your terminal:
 
 ![](https://raw.githubusercontent.com/IvS-KULeuven/dip_coater/develop/images/dip-coater-dark.png)
```

### Comparing `dip-coater-0.8.0/pyproject.toml` & `dip-coater-0.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dip-coater"
-version = "0.8.0"
+version = "0.9.0"
 authors = [
     {name="Rik Huygen", email="rik.huygen@kuleuven.be"},
     {name="Sibo Van Gool", email="sibo.vangool@kuleuven.be"}
 ]
 license = { text = "MIT License" }
 readme = "README.md"
 classifiers = [
@@ -19,22 +19,21 @@
     "License :: OSI Approved :: MIT License",
 ]
 requires-python = ">=3.8, <4.0"
 
 dependencies = [
     "textual",
     "textual-dev",
-    "TMC-2209-Raspberry-Pi"
 ]
 
 [project.urls]
 repository = "https://github.com/IvS-KULeuven/dip_coater"
 
 [project.optional-dependencies]
-rpi = ["RPi.GPIO"]
+rpi = ["RPi.GPIO", "TMC-2209-Raspberry-Pi>=0.4.3"]
 
 [project.scripts]
 dip-coater = "dip_coater.tui:main"
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `dip-coater-0.8.0/src/MyTMC_2209/TMC_2209_StepperDriver.py` & `dip-coater-0.9.0/src/MyTMC_2209/TMC_2209_StepperDriver.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,18 @@
     from ._TMC_2209_comm import (set_direction_reg, set_current, set_interpolation, set_spreadcycle,
                                  set_microstepping_resolution, set_internal_rsense)
 
     def __init__(self, pin_en, pin_step=-1, pin_dir=-1, baudrate=115200, serialport="/dev/serial0",
                  driver_address=0, gpio_mode=None, loglevel=None, skip_uart_init=False):
         self.tmc_logger = TMC_logger(loglevel, f"TMC2209 {driver_address}")
 
-    def set_stepmode(self, ):
+    def set_stepmode(self, _stepmode: int):
         pass
 
     def set_motor_enabled(self, en):
         pass
 
+    def set_vactual(self, flag: bool):
+        pass
+
     def set_vactual_rps(self, rps, duration=0, revolutions=0, acceleration=0):
         pass
```

### Comparing `dip-coater-0.8.0/src/dip_coater/help.md` & `dip-coater-0.9.0/src/dip_coater/help.md`

 * *Files identical despite different names*

### Comparing `dip-coater-0.8.0/src/dip_coater/motor.py` & `dip-coater-0.9.0/src/dip_coater/motor.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,20 +23,22 @@
         self.tmc = TMC_2209(en_pin, step_pin, dir_pin, loglevel=_loglevel)
 
         self.tmc.tmc_logger.set_loglevel(_loglevel)  # NONE, ERROR, INFO, DEBUG, MOVEMENT, ALL
 
         # Set motor driver settings
         self.tmc.set_vactual(True)      # Motor is controlled by UART
         self.tmc.set_direction_reg(False)
-        self.tmc.set_current(1500)
+        self.tmc.set_current(1500, pdn_disable=True)    # mA (also disable PDN, otherwise UART can't be used)
         self.tmc.set_interpolation(True)
         self.tmc.set_spreadcycle(False)  # True: spreadcycle, False: stealthchop
         self.tmc.set_microstepping_resolution(_stepmode)  # 1, 2, 4, 8, 16, 32, 64, 128, 256
         self.tmc.set_internal_rsense(False)
 
+        self.tmc.set_movement_abs_rel(MovementAbsRel.ABSOLUTE)
+
     def set_stepmode(self, _stepmode=4):
         """ Set the step mode of the motor driver
 
         :param stepmode: The step mode to set (1, 2, 4, 8, 16, 32, 64, 128, 256)
         """
         self.tmc.set_microstepping_resolution(_stepmode)
```

### Comparing `dip-coater-0.8.0/src/dip_coater/tui.py` & `dip-coater-0.9.0/src/dip_coater/tui.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,24 +28,24 @@
 # Mock the import of RPi when the package is not available
 try:
     import RPi
 except ModuleNotFoundError:
     import sys
     import MyRPi
     sys.modules["RPi"] = MyRPi
+
 try:
     import TMC_2209
 except ModuleNotFoundError:
     import sys
-    import MyTMC_2209
-    sys.modules["TMC_2209"] = MyTMC_2209
+    import MyTMC_2209 as TMC_2209
+    sys.modules["TMC_2209"] = TMC_2209
 
 from TMC_2209._TMC_2209_logger import Loglevel
-import dip_coater.motor as motor
-from motor import TMC2209_MotorDriver
+from dip_coater.motor import TMC2209_MotorDriver
 
 # Logging settings
 STEP_MODE_WRITE_TO_LOG = False
 LOGGING_LEVEL = Loglevel.ERROR  # NONE, ERROR, INFO, DEBUG, MOVEMENT, ALL
 
 # Speed settings (mm/s)
 DEFAULT_SPEED = 10
```

### Comparing `dip-coater-0.8.0/src/dip_coater/tui.tcss` & `dip-coater-0.9.0/src/dip_coater/tui.tcss`

 * *Files identical despite different names*

### Comparing `dip-coater-0.8.0/src/dip_coater.egg-info/PKG-INFO` & `dip-coater-0.9.0/src/dip_coater.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,61 @@
 Metadata-Version: 2.1
 Name: dip-coater
-Version: 0.8.0
+Version: 0.9.0
 Author-email: Rik Huygen <rik.huygen@kuleuven.be>, Sibo Van Gool <sibo.vangool@kuleuven.be>
 License: MIT License
 Project-URL: repository, https://github.com/IvS-KULeuven/dip_coater
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: textual
 Requires-Dist: textual-dev
-Requires-Dist: TMC-2209-Raspberry-Pi
 Provides-Extra: rpi
 Requires-Dist: RPi.GPIO; extra == "rpi"
+Requires-Dist: TMC-2209-Raspberry-Pi>=0.4.3; extra == "rpi"
 
 # The Dip Coater App
 
 This small App is developed for IvS to drive the motor for the dip coater. The motor is connected to a Raspberry Pi through the GPIO bus.
 
-This App is develop with [Textual](https://www.textualize.io).
+This App is developed with [Textual](https://www.textualize.io).
 
 ## Installation
 
 Always install in a dedicated virtual environment!
 
+```bash
+$ cd </path/to/dip-coater>
+$ python3 -m venv venv --prompt=dip-coater
+$ source venv/bin/activate
+$ pip install --upgrade pip setuptools wheel
+$ pip install -e .
+```
+
 On a Raspberry Pi, install the project together with the RPi package:
 
-```
+```bash
 $ pip install dip-coater[rpi] 
 ```
 
 When you want to develop and test on a macOS or Linux system, install without the RPi package. The App will mock the imports and functions.
 
-```
+```bash
 $ pip install dip-coater
 ```
 
 ## Usage
 
 Start the App from the command line in a terminal. You can start it also from a remote ssh session in a terminal, e.g. if you have the installation on the Raspberry Pi and you have a remote connection to your RPi.
 
-```
+```bash
 $ dip-coater
 ```
 
 This will show the following App in your terminal:
 
 ![](https://raw.githubusercontent.com/IvS-KULeuven/dip_coater/develop/images/dip-coater-dark.png)
```

### Comparing `dip-coater-0.8.0/src/dip_coater.egg-info/SOURCES.txt` & `dip-coater-0.9.0/src/dip_coater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

