# Comparing `tmp/sensirion_i2c_sht4x-1.0.0.tar.gz` & `tmp/sensirion_i2c_sht4x-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensirion_i2c_sht4x-1.0.0.tar", last modified: Tue Oct 31 09:24:22 2023, max compression
+gzip compressed data, was "sensirion_i2c_sht4x-1.1.0.tar", last modified: Thu Apr 11 14:35:04 2024, max compression
```

## Comparing `sensirion_i2c_sht4x-1.0.0.tar` & `sensirion_i2c_sht4x-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 09:24:22.361698 sensirion_i2c_sht4x-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-10-31 09:23:09.000000 sensirion_i2c_sht4x-1.0.0/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-10-19 13:30:53.000000 sensirion_i2c_sht4x-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4203 2023-10-31 09:24:22.361698 sensirion_i2c_sht4x-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-10-19 13:30:53.000000 sensirion_i2c_sht4x-1.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 09:24:22.361698 sensirion_i2c_sht4x-1.0.0/sensirion_i2c_sht4x/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-10-19 13:30:53.000000 sensirion_i2c_sht4x-1.0.0/sensirion_i2c_sht4x/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4278 2023-10-19 13:30:53.000000 sensirion_i2c_sht4x-1.0.0/sensirion_i2c_sht4x/commands.py
--rw-rw-rw-   0 root         (0) root         (0)    12760 2023-10-19 13:30:53.000000 sensirion_i2c_sht4x-1.0.0/sensirion_i2c_sht4x/device.py
--rw-rw-rw-   0 root         (0) root         (0)      374 2023-10-19 13:30:53.000000 sensirion_i2c_sht4x-1.0.0/sensirion_i2c_sht4x/response_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1363 2023-10-19 13:30:53.000000 sensirion_i2c_sht4x-1.0.0/sensirion_i2c_sht4x/result_types.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-10-31 09:24:09.000000 sensirion_i2c_sht4x-1.0.0/sensirion_i2c_sht4x/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 09:24:22.361698 sensirion_i2c_sht4x-1.0.0/sensirion_i2c_sht4x.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4203 2023-10-31 09:24:22.000000 sensirion_i2c_sht4x-1.0.0/sensirion_i2c_sht4x.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      471 2023-10-31 09:24:22.000000 sensirion_i2c_sht4x-1.0.0/sensirion_i2c_sht4x.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-31 09:24:22.000000 sensirion_i2c_sht4x-1.0.0/sensirion_i2c_sht4x.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      272 2023-10-31 09:24:22.000000 sensirion_i2c_sht4x-1.0.0/sensirion_i2c_sht4x.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-10-31 09:24:22.000000 sensirion_i2c_sht4x-1.0.0/sensirion_i2c_sht4x.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      367 2023-10-31 09:24:22.365698 sensirion_i2c_sht4x-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2344 2023-10-19 13:30:53.000000 sensirion_i2c_sht4x-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:35:04.055151 sensirion_i2c_sht4x-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-10-19 13:30:53.000000 sensirion_i2c_sht4x-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4218 2024-04-11 14:35:04.055151 sensirion_i2c_sht4x-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-10-19 13:30:53.000000 sensirion_i2c_sht4x-1.1.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:35:04.055151 sensirion_i2c_sht4x-1.1.0/sensirion_i2c_sht4x/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-10-19 13:30:53.000000 sensirion_i2c_sht4x-1.1.0/sensirion_i2c_sht4x/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4278 2024-04-11 14:11:32.000000 sensirion_i2c_sht4x-1.1.0/sensirion_i2c_sht4x/commands.py
+-rw-rw-rw-   0 root         (0) root         (0)    12760 2024-04-11 14:11:32.000000 sensirion_i2c_sht4x-1.1.0/sensirion_i2c_sht4x/device.py
+-rw-rw-rw-   0 root         (0) root         (0)      374 2023-10-19 13:30:53.000000 sensirion_i2c_sht4x-1.1.0/sensirion_i2c_sht4x/response_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1363 2024-04-11 14:11:32.000000 sensirion_i2c_sht4x-1.1.0/sensirion_i2c_sht4x/result_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-11 14:11:32.000000 sensirion_i2c_sht4x-1.1.0/sensirion_i2c_sht4x/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:35:04.055151 sensirion_i2c_sht4x-1.1.0/sensirion_i2c_sht4x.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4218 2024-04-11 14:35:03.000000 sensirion_i2c_sht4x-1.1.0/sensirion_i2c_sht4x.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      457 2024-04-11 14:35:04.000000 sensirion_i2c_sht4x-1.1.0/sensirion_i2c_sht4x.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 14:35:03.000000 sensirion_i2c_sht4x-1.1.0/sensirion_i2c_sht4x.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2024-04-11 14:35:03.000000 sensirion_i2c_sht4x-1.1.0/sensirion_i2c_sht4x.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-11 14:35:03.000000 sensirion_i2c_sht4x-1.1.0/sensirion_i2c_sht4x.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      367 2024-04-11 14:35:04.059151 sensirion_i2c_sht4x-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2269 2024-04-11 14:11:32.000000 sensirion_i2c_sht4x-1.1.0/setup.py
```

### Comparing `sensirion_i2c_sht4x-1.0.0/PKG-INFO` & `sensirion_i2c_sht4x-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: sensirion_i2c_sht4x
-Version: 1.0.0
+Version: 1.1.0
 Summary: I2C driver for the Sensirion SHT4X sensor family
 Home-page: UNKNOWN
 Author: Sensirion
 Author-email: info@sensirion.com
 License: BSD
 Project-URL: Documentation, https://sensirion.github.io/python-i2c-sht4x
 Project-URL: Repository, https://github.com/Sensirion/python-i2c-sht4x
-Project-URL: Changelog, https://github.com/Sensirion/python-i2c-sht4x/blob/master/CHANGELOG.rst
+Project-URL: Changelog, https://github.com/Sensirion/python-i2c-sht4x/blob/master/CHANGELOG.md
 Description: # Python I2C Driver for Sensirion SHT4X
         
-        This repository contains the Python driver to communicate with a Sensirion sensor of the SHT4X family over I2C. 
+        This repository contains the Python driver to communicate with a Sensirion sensor of the SHT4X family over I2C.
         
         <img src="https://raw.githubusercontent.com/Sensirion/python-i2c-sht4x/master/images/SHT4x.png"
             width="300px" alt="SHT4X picture">
         
         
         Click [here](https://sensirion.com/products/catalog/SEK-SHT40/) to learn more about the Sensirion SHT4X sensor family.
         
@@ -41,27 +41,27 @@
         <details><summary>Sensor pinout</summary>
         <p>
         <img src="https://raw.githubusercontent.com/Sensirion/python-i2c-sht4x/master/images/SHT40_pinout.png"
              width="300px" alt="sensor wiring picture">
         
         | *Pin* | *Cable Color* | *Name* | *Description*  | *Comments* |
         |-------|---------------|:------:|----------------|------------|
-        | 1 | green | SDA | I2C: Serial data input / output | 
-        | 2 | black | GND | Ground | 
-        | 3 | yellow | SCL | I2C: Serial clock input | 
+        | 1 | green | SDA | I2C: Serial data input / output |
+        | 2 | black | GND | Ground |
+        | 3 | yellow | SCL | I2C: Serial clock input |
         | 4 | red | VDD | Supply Voltage | 1.1V to 3.6V
         
         
         </p>
         </details>
         
         
         ## Documentation & Quickstart
         
-        See the [documentation page](https://sensirion.github.io/python-i2c-sht4x) for an API description and a 
+        See the [documentation page](https://sensirion.github.io/python-i2c-sht4x) for an API description and a
         [quickstart](https://sensirion.github.io/python-i2c-sht4x/execute-measurements.html) example.
         
         
         ## Contributing
         
         We develop and test this driver using our company internal tools (version
         control, continuous integration, code review etc.) and automatically
@@ -85,23 +85,22 @@
         pip install editorconfig-checker==2.0.3   # Install requirements
         editorconfig-checker                      # Run check
         ```
         
         ## License
         
         See [LICENSE](LICENSE).
-        
 Keywords: Sensirion SHT4X
         I2C
         SHT40
         SHT41
         SHT45
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
-Provides-Extra: docs
 Provides-Extra: test
```

### Comparing `sensirion_i2c_sht4x-1.0.0/sensirion_i2c_sht4x/commands.py` & `sensirion_i2c_sht4x-1.1.0/sensirion_i2c_sht4x/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# (c) Copyright 2023 Sensirion AG, Switzerland
+# (c) Copyright 2024 Sensirion AG, Switzerland
 #
 #     THIS FILE IS AUTOMATICALLY GENERATED!
 #
-# Generator:     sensirion-driver-generator 0.32.0
+# Generator:     sensirion-driver-generator 0.40.0
 # Product:       sht4x
-# Model-Version: 2.0.0
+# Model-Version: 2.1.1
 #
 """
 The transfer classes specify the data that is transferred between host and sensor. The generated transfer classes
 are used by the driver class and not intended for direct use.
 """
 
 from sensirion_driver_adapters.transfer import Transfer
```

### Comparing `sensirion_i2c_sht4x-1.0.0/sensirion_i2c_sht4x/device.py` & `sensirion_i2c_sht4x-1.1.0/sensirion_i2c_sht4x/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# (c) Copyright 2023 Sensirion AG, Switzerland
+# (c) Copyright 2024 Sensirion AG, Switzerland
 #
 #     THIS FILE IS AUTOMATICALLY GENERATED!
 #
-# Generator:     sensirion-driver-generator 0.32.0
+# Generator:     sensirion-driver-generator 0.40.0
 # Product:       sht4x
-# Model-Version: 2.0.0
+# Model-Version: 2.1.1
 #
 """
 The class Sht4xDeviceBase implements the low level interface of the sensor.
 The class Sht4xDevice extends the Sht4xDeviceBase. It provides additional functions to ease the use of the
 sensor.
 """
```

### Comparing `sensirion_i2c_sht4x-1.0.0/sensirion_i2c_sht4x/result_types.py` & `sensirion_i2c_sht4x-1.1.0/sensirion_i2c_sht4x/result_types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# (c) Copyright 2023 Sensirion AG, Switzerland
+# (c) Copyright 2024 Sensirion AG, Switzerland
 #
 #     THIS FILE IS AUTOMATICALLY GENERATED!
 #
-# Generator:     sensirion-driver-generator 0.32.0
+# Generator:     sensirion-driver-generator 0.40.0
 # Product:       sht4x
-# Model-Version: 2.0.0
+# Model-Version: 2.1.1
 #
 """
 The signal classes specify transformations of the raw sensor signals into a meaningful units.
 The generated signal types are used by the driver class and not intended for direct use.
 """
 
 from sensirion_driver_support_types.signals import AbstractSignal
```

### Comparing `sensirion_i2c_sht4x-1.0.0/sensirion_i2c_sht4x.egg-info/PKG-INFO` & `sensirion_i2c_sht4x-1.1.0/sensirion_i2c_sht4x.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: sensirion-i2c-sht4x
-Version: 1.0.0
+Version: 1.1.0
 Summary: I2C driver for the Sensirion SHT4X sensor family
 Home-page: UNKNOWN
 Author: Sensirion
 Author-email: info@sensirion.com
 License: BSD
 Project-URL: Documentation, https://sensirion.github.io/python-i2c-sht4x
 Project-URL: Repository, https://github.com/Sensirion/python-i2c-sht4x
-Project-URL: Changelog, https://github.com/Sensirion/python-i2c-sht4x/blob/master/CHANGELOG.rst
+Project-URL: Changelog, https://github.com/Sensirion/python-i2c-sht4x/blob/master/CHANGELOG.md
 Description: # Python I2C Driver for Sensirion SHT4X
         
-        This repository contains the Python driver to communicate with a Sensirion sensor of the SHT4X family over I2C. 
+        This repository contains the Python driver to communicate with a Sensirion sensor of the SHT4X family over I2C.
         
         <img src="https://raw.githubusercontent.com/Sensirion/python-i2c-sht4x/master/images/SHT4x.png"
             width="300px" alt="SHT4X picture">
         
         
         Click [here](https://sensirion.com/products/catalog/SEK-SHT40/) to learn more about the Sensirion SHT4X sensor family.
         
@@ -41,27 +41,27 @@
         <details><summary>Sensor pinout</summary>
         <p>
         <img src="https://raw.githubusercontent.com/Sensirion/python-i2c-sht4x/master/images/SHT40_pinout.png"
              width="300px" alt="sensor wiring picture">
         
         | *Pin* | *Cable Color* | *Name* | *Description*  | *Comments* |
         |-------|---------------|:------:|----------------|------------|
-        | 1 | green | SDA | I2C: Serial data input / output | 
-        | 2 | black | GND | Ground | 
-        | 3 | yellow | SCL | I2C: Serial clock input | 
+        | 1 | green | SDA | I2C: Serial data input / output |
+        | 2 | black | GND | Ground |
+        | 3 | yellow | SCL | I2C: Serial clock input |
         | 4 | red | VDD | Supply Voltage | 1.1V to 3.6V
         
         
         </p>
         </details>
         
         
         ## Documentation & Quickstart
         
-        See the [documentation page](https://sensirion.github.io/python-i2c-sht4x) for an API description and a 
+        See the [documentation page](https://sensirion.github.io/python-i2c-sht4x) for an API description and a
         [quickstart](https://sensirion.github.io/python-i2c-sht4x/execute-measurements.html) example.
         
         
         ## Contributing
         
         We develop and test this driver using our company internal tools (version
         control, continuous integration, code review etc.) and automatically
@@ -85,23 +85,22 @@
         pip install editorconfig-checker==2.0.3   # Install requirements
         editorconfig-checker                      # Run check
         ```
         
         ## License
         
         See [LICENSE](LICENSE).
-        
 Keywords: Sensirion SHT4X
         I2C
         SHT40
         SHT41
         SHT45
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
-Provides-Extra: docs
 Provides-Extra: test
```

### Comparing `sensirion_i2c_sht4x-1.0.0/setup.py` & `sensirion_i2c_sht4x-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,43 +8,37 @@
 
 # Python versions this package is compatible with
 python_requires = '>=3.6, <4'
 
 # Packages that this package imports. List everything apart from standard lib packages.
 install_requires = [
     'sensirion-i2c-driver>=1.0.0,<2.0',
-    'sensirion-driver-adapters>=2.1.8,<3.0',
+    'sensirion-driver-adapters>=2.1.9,<3.0',
     'sensirion-driver-support-types~=0.2.0',
-    'sensirion-shdlc-sensorbridge~=0.1.1'
+    'sensirion-shdlc-sensorbridge>=0.1.0,<0.3.0'
 ]
 
 # Packages required for tests and docs
 extras_require = {
     'test': [
         'flake8~=3.7.8',
         'pytest~=6.2.5',
         'pytest-cov~=3.0.0',
-    ],
-    'docs': [
-        'click==8.0.4',
-        'jinja2==3.0.1',
-        'sphinx~=4.2.0',
-        'sphinx-rtd-theme~=0.5.2',
     ]
 }
 
 # Read version number from version.py
 version_line = open("sensirion_i2c_sht4x/version.py", "rt").read()
 result = re.search(r"^version = ['\"]([^'\"]*)['\"]", version_line, re.M)
 if result:
     version_string = result.group(1)
 else:
     raise RuntimeError("Unable to find version string")
 
-# Use README.rst and CHANGELOG.rst as package description
+# Use README.rst and CHANGELOG.md as package description
 root_path = os.path.dirname(__file__)
 long_description = open(os.path.join(root_path, 'README.md')).read()
 
 setup(
     name='sensirion_i2c_sht4x',
     version=version_string,
     author='Sensirion',
@@ -55,23 +49,24 @@
         I2C
         SHT40
         SHT41
         SHT45""",
     project_urls={
         "Documentation": "https://sensirion.github.io/python-i2c-sht4x",
         "Repository": "https://github.com/Sensirion/python-i2c-sht4x",
-        "Changelog": "https://github.com/Sensirion/python-i2c-sht4x/blob/master/CHANGELOG.rst",
+        "Changelog": "https://github.com/Sensirion/python-i2c-sht4x/blob/master/CHANGELOG.md",
     },
     packages=find_packages(exclude=['tests', 'tests.*']),
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires=python_requires,
     install_requires=install_requires,
     extras_require=extras_require,
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ]
 )
```

