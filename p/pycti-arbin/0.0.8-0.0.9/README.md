# Comparing `tmp/pycti-arbin-0.0.8.tar.gz` & `tmp/pycti-arbin-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-arbin-0.0.8.tar", last modified: Mon Oct 23 21:47:06 2023, max compression
+gzip compressed data, was "pycti-arbin-0.0.9.tar", last modified: Thu Nov  9 19:34:38 2023, max compression
```

## Comparing `pycti-arbin-0.0.8.tar` & `pycti-arbin-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-10-23 21:47:06.813320 pycti-arbin-0.0.8/
--rw-r--r--   0 Benjamin   (502) staff       (20)     1072 2023-07-10 18:08:25.000000 pycti-arbin-0.0.8/LICENSE
--rw-r--r--   0 Benjamin   (502) staff       (20)    10650 2023-10-23 21:47:06.812646 pycti-arbin-0.0.8/PKG-INFO
--rw-r--r--   0 Benjamin   (502) staff       (20)    10143 2023-10-11 23:06:30.000000 pycti-arbin-0.0.8/README.md
-drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-10-23 21:47:06.806062 pycti-arbin-0.0.8/pycti_arbin.egg-info/
--rw-r--r--   0 Benjamin   (502) staff       (20)    10650 2023-10-23 21:47:06.000000 pycti-arbin-0.0.8/pycti_arbin.egg-info/PKG-INFO
--rw-r--r--   0 Benjamin   (502) staff       (20)      386 2023-10-23 21:47:06.000000 pycti-arbin-0.0.8/pycti_arbin.egg-info/SOURCES.txt
--rw-r--r--   0 Benjamin   (502) staff       (20)        1 2023-10-23 21:47:06.000000 pycti-arbin-0.0.8/pycti_arbin.egg-info/dependency_links.txt
--rw-r--r--   0 Benjamin   (502) staff       (20)       37 2023-10-23 21:47:06.000000 pycti-arbin-0.0.8/pycti_arbin.egg-info/requires.txt
--rw-r--r--   0 Benjamin   (502) staff       (20)       11 2023-10-23 21:47:06.000000 pycti-arbin-0.0.8/pycti_arbin.egg-info/top_level.txt
-drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-10-23 21:47:06.808980 pycti-arbin-0.0.8/pyctiarbin/
--rw-r--r--   0 Benjamin   (502) staff       (20)      152 2023-10-11 23:06:30.000000 pycti-arbin-0.0.8/pyctiarbin/__init__.py
-drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-10-23 21:47:06.811279 pycti-arbin-0.0.8/pyctiarbin/arbinspoofer/
--rw-r--r--   0 Benjamin   (502) staff       (20)       39 2023-10-11 23:06:30.000000 pycti-arbin-0.0.8/pyctiarbin/arbinspoofer/__init__.py
--rw-r--r--   0 Benjamin   (502) staff       (20)    11549 2023-10-11 23:06:30.000000 pycti-arbin-0.0.8/pyctiarbin/arbinspoofer/arbin_spoofer.py
--rw-r--r--   0 Benjamin   (502) staff       (20)     9304 2023-10-17 20:59:18.000000 pycti-arbin-0.0.8/pyctiarbin/channel_interface.py
--rw-r--r--   0 Benjamin   (502) staff       (20)     9350 2023-10-23 21:43:44.000000 pycti-arbin-0.0.8/pyctiarbin/cycler_interface.py
--rw-r--r--   0 Benjamin   (502) staff       (20)    42396 2023-10-11 23:06:30.000000 pycti-arbin-0.0.8/pyctiarbin/messages.py
--rw-r--r--   0 Benjamin   (502) staff       (20)       38 2023-10-23 21:47:06.813446 pycti-arbin-0.0.8/setup.cfg
--rw-r--r--   0 Benjamin   (502) staff       (20)      836 2023-10-23 21:43:44.000000 pycti-arbin-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-09 19:34:38.512479 pycti-arbin-0.0.9/
+-rw-rw-rw-   0        0        0     1072 2023-10-27 05:50:25.000000 pycti-arbin-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0    10922 2023-11-09 19:34:38.511083 pycti-arbin-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10143 2023-10-27 05:50:25.000000 pycti-arbin-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-11-09 19:34:38.504447 pycti-arbin-0.0.9/pycti_arbin.egg-info/
+-rw-rw-rw-   0        0        0    10922 2023-11-09 19:34:38.000000 pycti-arbin-0.0.9/pycti_arbin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2023-11-09 19:34:38.000000 pycti-arbin-0.0.9/pycti_arbin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-09 19:34:38.000000 pycti-arbin-0.0.9/pycti_arbin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-11-09 19:34:38.000000 pycti-arbin-0.0.9/pycti_arbin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-11-09 19:34:38.000000 pycti-arbin-0.0.9/pycti_arbin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-11-09 19:34:38.507573 pycti-arbin-0.0.9/pyctiarbin/
+-rw-rw-rw-   0        0        0      152 2023-10-27 05:50:25.000000 pycti-arbin-0.0.9/pyctiarbin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-09 19:34:38.509075 pycti-arbin-0.0.9/pyctiarbin/arbinspoofer/
+-rw-rw-rw-   0        0        0       39 2023-10-27 05:50:25.000000 pycti-arbin-0.0.9/pyctiarbin/arbinspoofer/__init__.py
+-rw-rw-rw-   0        0        0    11549 2023-10-27 05:50:25.000000 pycti-arbin-0.0.9/pyctiarbin/arbinspoofer/arbin_spoofer.py
+-rw-rw-rw-   0        0        0     9304 2023-10-27 05:50:25.000000 pycti-arbin-0.0.9/pyctiarbin/channel_interface.py
+-rw-rw-rw-   0        0        0     9350 2023-10-27 05:50:25.000000 pycti-arbin-0.0.9/pyctiarbin/cycler_interface.py
+-rw-rw-rw-   0        0        0    42723 2023-11-09 19:32:42.000000 pycti-arbin-0.0.9/pyctiarbin/messages.py
+-rw-rw-rw-   0        0        0       42 2023-11-09 19:34:38.512479 pycti-arbin-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-11-09 19:32:42.000000 pycti-arbin-0.0.9/setup.py
```

### Comparing `pycti-arbin-0.0.8/LICENSE` & `pycti-arbin-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-arbin-0.0.8/PKG-INFO` & `pycti-arbin-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: pycti-arbin
-Version: 0.0.8
-Summary: A class based Python interface for communication and control of Arbin cyclers over CTI.
-Home-page: https://github.com/BattGenie/pycti.git
-Author: Zander Nevitt, Bing Syuan Wang
-Author-email: info@battgenie.life
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyCTI-Arbin
 
 `pycti-arbin` is a Python module that provides cycler and channel level interfaces for communication and control of [Arbin cyclers](https://arbin.com/) via their Console TCP/IP Interface (CTI).
 
 ## Overview
 
 - [Motivation](#motivation)
```

### Comparing `pycti-arbin-0.0.8/README.md` & `pycti-arbin-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,258 +1,272 @@
-# PyCTI-Arbin
-
-`pycti-arbin` is a Python module that provides cycler and channel level interfaces for communication and control of [Arbin cyclers](https://arbin.com/) via their Console TCP/IP Interface (CTI).
-
-## Overview
-
-- [Motivation](#motivation)
-- [Installation](#installation)
-  - [Source Installation](#source-installation)
-- [Getting Started](#getting-started)
-  - [Configuration](#configuration)
-    - [CyclerInterface Configuration](#cyclerinterface-configuration)
-    - [ChannelInterface Configuration](#channelinterface-configuration)
-  - [Env](#env)
-- [Getting Channel Readings](#getting-channel-readings)
-- [Development](#development)
-  - [Contributing](#contributing)
-  - [Testing](#testing)
-    - [ArbinSpoofer](#arbinspoofer)
-  - [Documentation](#documentation)
-- [License](#license)
-
-## Motivation
-
-Why did we create `pycti-arbin`? This package enables a wide variety of applications such as:
-
-- Real-time data logging, monitoring and alerting
-
-`pycti-arbin` can be used to passively monitor running tests and log readings directly to a database, bypassing the need to manually export data. Moreover, it's possible to create automated alerts based on incoming real-time data. For example, if a test were to fault or temperature were to exceed a set threshold. While Arbin already has a built-in notification system with MacNotify, `pycti-arbin` provides a more flexible and customizable solution without having to directly modify test procedures.
-
-- Automated test management
-
-The GUI provided by Arbin for test management is straight-forward and easy to use, but requires significant manual work. With `pycti-arbin` it is possible to write programs to automatically start tests simultaneously across many channels (or even many cyclers) at once.
-
-- Testing of next generation closed-loop charging methods
-
-While conventional constant-current followed by constant-voltage (CCCV) charging has been the industry standard for many years and is well supported by cyclers, there is movement towards advanced [closed-loop control charging techniques that provide improved battery life and decreased charge times](https://battgenie.life/technology/). `pycti-arbin` enables testing of closed-loop battery charging methods by providing an interface between software hosting battery charging algorithms and active Arbin tests, allowing the charge current to be dynamically set.
-
-- Well tested, easy to use, community supported interface in the most popular programming language.
-
-It is entirely possible to write one's own CTI wrapper, but `pycti-arbin` provides a well-tested ready to use package that takes care of lower level communication, providing a simple yet powerful interface in the most popular programming language.
-
-## Installation
-
-### Using pip
-
-`pycti-arbin` can be installed using pip:
-
-```bash
-pip install pycti-arbin
-```
-
-### Source Installation
-
-To install from source, type the following into the command line:
-
-```bash
-git clone https://github.com/BattGenie/pycti.git
-cd pycti
-pip install -r requirements.txt
-pip install .
-```
-
-## Getting Started
-
-`pycti-arbin` provides two distinct classes for interacting with Arbin cyclers:
-
-- `CyclerInterface` : A cycler-level interface for reading channel status of any channel on the cycler. This class is capable of read only operations on the cycler.
-
-- `ChannelInterface` : A channel-level interface for reading status of a specific channel, starting/stopping tests on that channel, and assigning meta variables during active tests on the channel. This class is capable of read and write operations on a single channel.
-
-### Configuration
-
-Both `CyclerInterface` and `ChannelInterface` require configuration dictionaries upon initialization. The fields of these configuration dictionaries are detailed in the following sections.
-
-#### CyclerInterface Configuration
-
-An example `CyclerInterface` configuration dictionary is shown below:
-
-```python
-CYCLER_INTERFACE_CONFIG = {
-    "ip_address": 127.0.0.1,
-    "port": 1234,
-    "timeout_s": 3,
-    "msg_buffer_size": 4096
-}
-```
-
-Where the fields are as follows:
-
-- `ip_address` : str
-    The IP address of the Arbin host computer.
-- `port` : int
-    The TCP port to communicate through. This is generally going to be 9031
-- `timeout_s` : *optional* : float
-    How long to wait before timing out on TCP communication. Defaults to 3 seconds.
-- `msg_buffer_size` : *optional* : int
-    How big of a message buffer to use for sending/receiving messages.
-    A minimum of 1024 bytes is recommended. Defaults to 4096 bytes.
-
-#### ChannelInterface Configuration
-
-An example `ChannelInterface` configuration dictionary is shown below:
-
-```python
-CHANNEL_INTERFACE_CONFIG = {
-  "channel": 1,
-  "test_name": "fake_test_name",
-  "schedule_name": "Rest+207855.sdx",
-  "ip_address": 127.0.0.1,
-  "port": 1234,
-  "timeout_s": 3,
-  "msg_buffer_size": 4096
-}
-```
-
-Where the fields are as follows:
-
-- `channel` : int
-    The channel to target with the ChannelInterface class instance.
-- `test_name` : *optional* : str
-    The test name to use if using the ChannelInterface to start a test.
-- `schedule_name` : *optional* : str
-    The name of the schedule file to use if using the ChannelInterface to start a test.
-- `ip_address` : str
-    The IP address of the Arbin host computer.
-- `port` : int
-    The TCP port to communicate through. This is generally going to be 7031
-- `timeout_s` : *optional* : float
-    How long to wait before timing out on TCP communication. Defaults to 3 seconds.
-- `msg_buffer_size` : *optional* : int
-    How big of a message buffer to use for sending/receiving messages.
-    A minimum of 1024 bytes is recommended. Defaults to 4096 bytes.
-
-### Env
-
-In addition to a configuration dictionary, both interfaces require a `.env` file containing the Arbin CTI username and password to use for communication. The `.env` file path can be passed as a constructor argument. If it is not specified, the the program looks in the working directly for a `.env` file.
-
-The `.env` file must contain the following fields:
-
-```bash
-ARBIN_CTI_USERNAME='your_username'
-ARBIN_CTI_PASSWORD='your_password'
-```
-
-Where `your_username` and `your_password` should be replaced with your username and password.
-
-### Getting Channel Readings
-
-To get channel readings with a `CyclerInterface` you must specify which channel you want to read from:
-
-```python
-from pyctiarbin import CyclerInterface
-
-CYCLER_INTERFACE_CONFIG = {
-    "ip_address": "127.0.0.1"
-    "port": 1234,
-    "timeout_s": 3,
-    "msg_buffer_size": 4096
-}
-
-cycler_interface = CyclerInterface(CYCLER_INTERFACE_CONFIG)
-cycler_interface.read_channel_status(channel=1)
-```
-
-For a `ChannelInterface` there is no need to specify the channel since we define it in the config:
-
-```python
-from pyctiarbin import ChannelInterface
-
-CHANNEL_INTERFACE_CONFIG = {
-  "channel": 1,
-  "test_name": "fake_test_name",
-  "schedule_name": "Rest+207855.sdx",
-  "ip_address": "127.0.0.1"
-  "port": 1234,
-  "timeout_s": 3,
-  "msg_buffer_size": 4096
-}
-
-channel_interface = ChannelInterface(CHANNEL_INTERFACE_CONFIG)
-channel_interface.read_channel_status()
-```
-
-For more examples of how to use the `CyclerInterface` and `ChannelInterface` class see the `demo_notebook.ipynb` and documentation.
-
-## Tested MITS Pro Version
-
-| Version         | Build      | pycti-arbin |
-|-----------------|------------|-------------|
-| Mits8 PV.202110 | Oct 4 2021 | 0.0.4       |
-|                 |            |             |
-
-## Development
-
-This section contains various information to help developers further extend and test `pycti-arbin`
-
-## Contributing
-
-As it exists now `pycti-arbin` only implements a fraction of the messages supported by CTI. Further work can be done to expand `pycti-arbin` to include more of the messages detailed in the CTI documentation `docs/ArbinCTI_Protocol v1.1.pdf`.
-
-We welcome your help in expanding `pycti-arbin`! Please see the [CONTRIBUTING.md](https://github.com/BattGenie/pycti/blob/main/CONTRIBUTING.md) file in this repository for contribution guidelines.
-
-## Testing
-
-To run the tests navigate to the "tests" directory and type the following:
-
-```bash
-pytest .
-```
-
-To run tests and generate a coverage report:
-
-```bash
-coverage run -m pytest
-```
-
-To view the generated coverage report:
-
-```bash
-coverage report -m 
-```
-
-### ArbinSpoofer
-
-Testing software on a real cycler is dangerous so we've created a submodule `arbinspoofer` to emulate some of the behavior of the Arbin software with a class `ArbinSpoofer`. This class creates a local TCP server and that accepts connections from n number of clients. The `ArbinSpoofer` does not perfectly emulate a Arbin cycler (for example, it does not track if a test is already running on a channel) and merely checks that the message format is correct and responds with standard messages.
-
-## Documentation
-
-All documentation was generated with [pydoc](https://docs.python.org/3/library/pydoc.html). To re-generate the documentation type the following command from the top level directory of the repository:
-
-```bash
-pydoc --html .
-```
-
-## License
-
-MIT License
-
-Copyright (c) 2023 BattGenie Inc.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE
+Metadata-Version: 2.1
+Name: pycti-arbin
+Version: 0.0.9
+Summary: A class based Python interface for communication and control of Arbin cyclers over CTI.
+Home-page: https://github.com/BattGenie/pycti.git
+Author: Zander Nevitt, Bing Syuan Wang
+Author-email: info@battgenie.life
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PyCTI-Arbin
+
+`pycti-arbin` is a Python module that provides cycler and channel level interfaces for communication and control of [Arbin cyclers](https://arbin.com/) via their Console TCP/IP Interface (CTI).
+
+## Overview
+
+- [Motivation](#motivation)
+- [Installation](#installation)
+  - [Source Installation](#source-installation)
+- [Getting Started](#getting-started)
+  - [Configuration](#configuration)
+    - [CyclerInterface Configuration](#cyclerinterface-configuration)
+    - [ChannelInterface Configuration](#channelinterface-configuration)
+  - [Env](#env)
+- [Getting Channel Readings](#getting-channel-readings)
+- [Development](#development)
+  - [Contributing](#contributing)
+  - [Testing](#testing)
+    - [ArbinSpoofer](#arbinspoofer)
+  - [Documentation](#documentation)
+- [License](#license)
+
+## Motivation
+
+Why did we create `pycti-arbin`? This package enables a wide variety of applications such as:
+
+- Real-time data logging, monitoring and alerting
+
+`pycti-arbin` can be used to passively monitor running tests and log readings directly to a database, bypassing the need to manually export data. Moreover, it's possible to create automated alerts based on incoming real-time data. For example, if a test were to fault or temperature were to exceed a set threshold. While Arbin already has a built-in notification system with MacNotify, `pycti-arbin` provides a more flexible and customizable solution without having to directly modify test procedures.
+
+- Automated test management
+
+The GUI provided by Arbin for test management is straight-forward and easy to use, but requires significant manual work. With `pycti-arbin` it is possible to write programs to automatically start tests simultaneously across many channels (or even many cyclers) at once.
+
+- Testing of next generation closed-loop charging methods
+
+While conventional constant-current followed by constant-voltage (CCCV) charging has been the industry standard for many years and is well supported by cyclers, there is movement towards advanced [closed-loop control charging techniques that provide improved battery life and decreased charge times](https://battgenie.life/technology/). `pycti-arbin` enables testing of closed-loop battery charging methods by providing an interface between software hosting battery charging algorithms and active Arbin tests, allowing the charge current to be dynamically set.
+
+- Well tested, easy to use, community supported interface in the most popular programming language.
+
+It is entirely possible to write one's own CTI wrapper, but `pycti-arbin` provides a well-tested ready to use package that takes care of lower level communication, providing a simple yet powerful interface in the most popular programming language.
+
+## Installation
+
+### Using pip
+
+`pycti-arbin` can be installed using pip:
+
+```bash
+pip install pycti-arbin
+```
+
+### Source Installation
+
+To install from source, type the following into the command line:
+
+```bash
+git clone https://github.com/BattGenie/pycti.git
+cd pycti
+pip install -r requirements.txt
+pip install .
+```
+
+## Getting Started
+
+`pycti-arbin` provides two distinct classes for interacting with Arbin cyclers:
+
+- `CyclerInterface` : A cycler-level interface for reading channel status of any channel on the cycler. This class is capable of read only operations on the cycler.
+
+- `ChannelInterface` : A channel-level interface for reading status of a specific channel, starting/stopping tests on that channel, and assigning meta variables during active tests on the channel. This class is capable of read and write operations on a single channel.
+
+### Configuration
+
+Both `CyclerInterface` and `ChannelInterface` require configuration dictionaries upon initialization. The fields of these configuration dictionaries are detailed in the following sections.
+
+#### CyclerInterface Configuration
+
+An example `CyclerInterface` configuration dictionary is shown below:
+
+```python
+CYCLER_INTERFACE_CONFIG = {
+    "ip_address": 127.0.0.1,
+    "port": 1234,
+    "timeout_s": 3,
+    "msg_buffer_size": 4096
+}
+```
+
+Where the fields are as follows:
+
+- `ip_address` : str
+    The IP address of the Arbin host computer.
+- `port` : int
+    The TCP port to communicate through. This is generally going to be 9031
+- `timeout_s` : *optional* : float
+    How long to wait before timing out on TCP communication. Defaults to 3 seconds.
+- `msg_buffer_size` : *optional* : int
+    How big of a message buffer to use for sending/receiving messages.
+    A minimum of 1024 bytes is recommended. Defaults to 4096 bytes.
+
+#### ChannelInterface Configuration
+
+An example `ChannelInterface` configuration dictionary is shown below:
+
+```python
+CHANNEL_INTERFACE_CONFIG = {
+  "channel": 1,
+  "test_name": "fake_test_name",
+  "schedule_name": "Rest+207855.sdx",
+  "ip_address": 127.0.0.1,
+  "port": 1234,
+  "timeout_s": 3,
+  "msg_buffer_size": 4096
+}
+```
+
+Where the fields are as follows:
+
+- `channel` : int
+    The channel to target with the ChannelInterface class instance.
+- `test_name` : *optional* : str
+    The test name to use if using the ChannelInterface to start a test.
+- `schedule_name` : *optional* : str
+    The name of the schedule file to use if using the ChannelInterface to start a test.
+- `ip_address` : str
+    The IP address of the Arbin host computer.
+- `port` : int
+    The TCP port to communicate through. This is generally going to be 7031
+- `timeout_s` : *optional* : float
+    How long to wait before timing out on TCP communication. Defaults to 3 seconds.
+- `msg_buffer_size` : *optional* : int
+    How big of a message buffer to use for sending/receiving messages.
+    A minimum of 1024 bytes is recommended. Defaults to 4096 bytes.
+
+### Env
+
+In addition to a configuration dictionary, both interfaces require a `.env` file containing the Arbin CTI username and password to use for communication. The `.env` file path can be passed as a constructor argument. If it is not specified, the the program looks in the working directly for a `.env` file.
+
+The `.env` file must contain the following fields:
+
+```bash
+ARBIN_CTI_USERNAME='your_username'
+ARBIN_CTI_PASSWORD='your_password'
+```
+
+Where `your_username` and `your_password` should be replaced with your username and password.
+
+### Getting Channel Readings
+
+To get channel readings with a `CyclerInterface` you must specify which channel you want to read from:
+
+```python
+from pyctiarbin import CyclerInterface
+
+CYCLER_INTERFACE_CONFIG = {
+    "ip_address": "127.0.0.1"
+    "port": 1234,
+    "timeout_s": 3,
+    "msg_buffer_size": 4096
+}
+
+cycler_interface = CyclerInterface(CYCLER_INTERFACE_CONFIG)
+cycler_interface.read_channel_status(channel=1)
+```
+
+For a `ChannelInterface` there is no need to specify the channel since we define it in the config:
+
+```python
+from pyctiarbin import ChannelInterface
+
+CHANNEL_INTERFACE_CONFIG = {
+  "channel": 1,
+  "test_name": "fake_test_name",
+  "schedule_name": "Rest+207855.sdx",
+  "ip_address": "127.0.0.1"
+  "port": 1234,
+  "timeout_s": 3,
+  "msg_buffer_size": 4096
+}
+
+channel_interface = ChannelInterface(CHANNEL_INTERFACE_CONFIG)
+channel_interface.read_channel_status()
+```
+
+For more examples of how to use the `CyclerInterface` and `ChannelInterface` class see the `demo_notebook.ipynb` and documentation.
+
+## Tested MITS Pro Version
+
+| Version         | Build      | pycti-arbin |
+|-----------------|------------|-------------|
+| Mits8 PV.202110 | Oct 4 2021 | 0.0.4       |
+|                 |            |             |
+
+## Development
+
+This section contains various information to help developers further extend and test `pycti-arbin`
+
+## Contributing
+
+As it exists now `pycti-arbin` only implements a fraction of the messages supported by CTI. Further work can be done to expand `pycti-arbin` to include more of the messages detailed in the CTI documentation `docs/ArbinCTI_Protocol v1.1.pdf`.
+
+We welcome your help in expanding `pycti-arbin`! Please see the [CONTRIBUTING.md](https://github.com/BattGenie/pycti/blob/main/CONTRIBUTING.md) file in this repository for contribution guidelines.
+
+## Testing
+
+To run the tests navigate to the "tests" directory and type the following:
+
+```bash
+pytest .
+```
+
+To run tests and generate a coverage report:
+
+```bash
+coverage run -m pytest
+```
+
+To view the generated coverage report:
+
+```bash
+coverage report -m 
+```
+
+### ArbinSpoofer
+
+Testing software on a real cycler is dangerous so we've created a submodule `arbinspoofer` to emulate some of the behavior of the Arbin software with a class `ArbinSpoofer`. This class creates a local TCP server and that accepts connections from n number of clients. The `ArbinSpoofer` does not perfectly emulate a Arbin cycler (for example, it does not track if a test is already running on a channel) and merely checks that the message format is correct and responds with standard messages.
+
+## Documentation
+
+All documentation was generated with [pydoc](https://docs.python.org/3/library/pydoc.html). To re-generate the documentation type the following command from the top level directory of the repository:
+
+```bash
+pydoc --html .
+```
+
+## License
+
+MIT License
+
+Copyright (c) 2023 BattGenie Inc.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE
```

### Comparing `pycti-arbin-0.0.8/pycti_arbin.egg-info/PKG-INFO` & `pycti-arbin-0.0.9/pycti_arbin.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,272 +1,272 @@
-Metadata-Version: 2.1
-Name: pycti-arbin
-Version: 0.0.8
-Summary: A class based Python interface for communication and control of Arbin cyclers over CTI.
-Home-page: https://github.com/BattGenie/pycti.git
-Author: Zander Nevitt, Bing Syuan Wang
-Author-email: info@battgenie.life
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PyCTI-Arbin
-
-`pycti-arbin` is a Python module that provides cycler and channel level interfaces for communication and control of [Arbin cyclers](https://arbin.com/) via their Console TCP/IP Interface (CTI).
-
-## Overview
-
-- [Motivation](#motivation)
-- [Installation](#installation)
-  - [Source Installation](#source-installation)
-- [Getting Started](#getting-started)
-  - [Configuration](#configuration)
-    - [CyclerInterface Configuration](#cyclerinterface-configuration)
-    - [ChannelInterface Configuration](#channelinterface-configuration)
-  - [Env](#env)
-- [Getting Channel Readings](#getting-channel-readings)
-- [Development](#development)
-  - [Contributing](#contributing)
-  - [Testing](#testing)
-    - [ArbinSpoofer](#arbinspoofer)
-  - [Documentation](#documentation)
-- [License](#license)
-
-## Motivation
-
-Why did we create `pycti-arbin`? This package enables a wide variety of applications such as:
-
-- Real-time data logging, monitoring and alerting
-
-`pycti-arbin` can be used to passively monitor running tests and log readings directly to a database, bypassing the need to manually export data. Moreover, it's possible to create automated alerts based on incoming real-time data. For example, if a test were to fault or temperature were to exceed a set threshold. While Arbin already has a built-in notification system with MacNotify, `pycti-arbin` provides a more flexible and customizable solution without having to directly modify test procedures.
-
-- Automated test management
-
-The GUI provided by Arbin for test management is straight-forward and easy to use, but requires significant manual work. With `pycti-arbin` it is possible to write programs to automatically start tests simultaneously across many channels (or even many cyclers) at once.
-
-- Testing of next generation closed-loop charging methods
-
-While conventional constant-current followed by constant-voltage (CCCV) charging has been the industry standard for many years and is well supported by cyclers, there is movement towards advanced [closed-loop control charging techniques that provide improved battery life and decreased charge times](https://battgenie.life/technology/). `pycti-arbin` enables testing of closed-loop battery charging methods by providing an interface between software hosting battery charging algorithms and active Arbin tests, allowing the charge current to be dynamically set.
-
-- Well tested, easy to use, community supported interface in the most popular programming language.
-
-It is entirely possible to write one's own CTI wrapper, but `pycti-arbin` provides a well-tested ready to use package that takes care of lower level communication, providing a simple yet powerful interface in the most popular programming language.
-
-## Installation
-
-### Using pip
-
-`pycti-arbin` can be installed using pip:
-
-```bash
-pip install pycti-arbin
-```
-
-### Source Installation
-
-To install from source, type the following into the command line:
-
-```bash
-git clone https://github.com/BattGenie/pycti.git
-cd pycti
-pip install -r requirements.txt
-pip install .
-```
-
-## Getting Started
-
-`pycti-arbin` provides two distinct classes for interacting with Arbin cyclers:
-
-- `CyclerInterface` : A cycler-level interface for reading channel status of any channel on the cycler. This class is capable of read only operations on the cycler.
-
-- `ChannelInterface` : A channel-level interface for reading status of a specific channel, starting/stopping tests on that channel, and assigning meta variables during active tests on the channel. This class is capable of read and write operations on a single channel.
-
-### Configuration
-
-Both `CyclerInterface` and `ChannelInterface` require configuration dictionaries upon initialization. The fields of these configuration dictionaries are detailed in the following sections.
-
-#### CyclerInterface Configuration
-
-An example `CyclerInterface` configuration dictionary is shown below:
-
-```python
-CYCLER_INTERFACE_CONFIG = {
-    "ip_address": 127.0.0.1,
-    "port": 1234,
-    "timeout_s": 3,
-    "msg_buffer_size": 4096
-}
-```
-
-Where the fields are as follows:
-
-- `ip_address` : str
-    The IP address of the Arbin host computer.
-- `port` : int
-    The TCP port to communicate through. This is generally going to be 9031
-- `timeout_s` : *optional* : float
-    How long to wait before timing out on TCP communication. Defaults to 3 seconds.
-- `msg_buffer_size` : *optional* : int
-    How big of a message buffer to use for sending/receiving messages.
-    A minimum of 1024 bytes is recommended. Defaults to 4096 bytes.
-
-#### ChannelInterface Configuration
-
-An example `ChannelInterface` configuration dictionary is shown below:
-
-```python
-CHANNEL_INTERFACE_CONFIG = {
-  "channel": 1,
-  "test_name": "fake_test_name",
-  "schedule_name": "Rest+207855.sdx",
-  "ip_address": 127.0.0.1,
-  "port": 1234,
-  "timeout_s": 3,
-  "msg_buffer_size": 4096
-}
-```
-
-Where the fields are as follows:
-
-- `channel` : int
-    The channel to target with the ChannelInterface class instance.
-- `test_name` : *optional* : str
-    The test name to use if using the ChannelInterface to start a test.
-- `schedule_name` : *optional* : str
-    The name of the schedule file to use if using the ChannelInterface to start a test.
-- `ip_address` : str
-    The IP address of the Arbin host computer.
-- `port` : int
-    The TCP port to communicate through. This is generally going to be 7031
-- `timeout_s` : *optional* : float
-    How long to wait before timing out on TCP communication. Defaults to 3 seconds.
-- `msg_buffer_size` : *optional* : int
-    How big of a message buffer to use for sending/receiving messages.
-    A minimum of 1024 bytes is recommended. Defaults to 4096 bytes.
-
-### Env
-
-In addition to a configuration dictionary, both interfaces require a `.env` file containing the Arbin CTI username and password to use for communication. The `.env` file path can be passed as a constructor argument. If it is not specified, the the program looks in the working directly for a `.env` file.
-
-The `.env` file must contain the following fields:
-
-```bash
-ARBIN_CTI_USERNAME='your_username'
-ARBIN_CTI_PASSWORD='your_password'
-```
-
-Where `your_username` and `your_password` should be replaced with your username and password.
-
-### Getting Channel Readings
-
-To get channel readings with a `CyclerInterface` you must specify which channel you want to read from:
-
-```python
-from pyctiarbin import CyclerInterface
-
-CYCLER_INTERFACE_CONFIG = {
-    "ip_address": "127.0.0.1"
-    "port": 1234,
-    "timeout_s": 3,
-    "msg_buffer_size": 4096
-}
-
-cycler_interface = CyclerInterface(CYCLER_INTERFACE_CONFIG)
-cycler_interface.read_channel_status(channel=1)
-```
-
-For a `ChannelInterface` there is no need to specify the channel since we define it in the config:
-
-```python
-from pyctiarbin import ChannelInterface
-
-CHANNEL_INTERFACE_CONFIG = {
-  "channel": 1,
-  "test_name": "fake_test_name",
-  "schedule_name": "Rest+207855.sdx",
-  "ip_address": "127.0.0.1"
-  "port": 1234,
-  "timeout_s": 3,
-  "msg_buffer_size": 4096
-}
-
-channel_interface = ChannelInterface(CHANNEL_INTERFACE_CONFIG)
-channel_interface.read_channel_status()
-```
-
-For more examples of how to use the `CyclerInterface` and `ChannelInterface` class see the `demo_notebook.ipynb` and documentation.
-
-## Tested MITS Pro Version
-
-| Version         | Build      | pycti-arbin |
-|-----------------|------------|-------------|
-| Mits8 PV.202110 | Oct 4 2021 | 0.0.4       |
-|                 |            |             |
-
-## Development
-
-This section contains various information to help developers further extend and test `pycti-arbin`
-
-## Contributing
-
-As it exists now `pycti-arbin` only implements a fraction of the messages supported by CTI. Further work can be done to expand `pycti-arbin` to include more of the messages detailed in the CTI documentation `docs/ArbinCTI_Protocol v1.1.pdf`.
-
-We welcome your help in expanding `pycti-arbin`! Please see the [CONTRIBUTING.md](https://github.com/BattGenie/pycti/blob/main/CONTRIBUTING.md) file in this repository for contribution guidelines.
-
-## Testing
-
-To run the tests navigate to the "tests" directory and type the following:
-
-```bash
-pytest .
-```
-
-To run tests and generate a coverage report:
-
-```bash
-coverage run -m pytest
-```
-
-To view the generated coverage report:
-
-```bash
-coverage report -m 
-```
-
-### ArbinSpoofer
-
-Testing software on a real cycler is dangerous so we've created a submodule `arbinspoofer` to emulate some of the behavior of the Arbin software with a class `ArbinSpoofer`. This class creates a local TCP server and that accepts connections from n number of clients. The `ArbinSpoofer` does not perfectly emulate a Arbin cycler (for example, it does not track if a test is already running on a channel) and merely checks that the message format is correct and responds with standard messages.
-
-## Documentation
-
-All documentation was generated with [pydoc](https://docs.python.org/3/library/pydoc.html). To re-generate the documentation type the following command from the top level directory of the repository:
-
-```bash
-pydoc --html .
-```
-
-## License
-
-MIT License
-
-Copyright (c) 2023 BattGenie Inc.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE
+Metadata-Version: 2.1
+Name: pycti-arbin
+Version: 0.0.9
+Summary: A class based Python interface for communication and control of Arbin cyclers over CTI.
+Home-page: https://github.com/BattGenie/pycti.git
+Author: Zander Nevitt, Bing Syuan Wang
+Author-email: info@battgenie.life
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PyCTI-Arbin
+
+`pycti-arbin` is a Python module that provides cycler and channel level interfaces for communication and control of [Arbin cyclers](https://arbin.com/) via their Console TCP/IP Interface (CTI).
+
+## Overview
+
+- [Motivation](#motivation)
+- [Installation](#installation)
+  - [Source Installation](#source-installation)
+- [Getting Started](#getting-started)
+  - [Configuration](#configuration)
+    - [CyclerInterface Configuration](#cyclerinterface-configuration)
+    - [ChannelInterface Configuration](#channelinterface-configuration)
+  - [Env](#env)
+- [Getting Channel Readings](#getting-channel-readings)
+- [Development](#development)
+  - [Contributing](#contributing)
+  - [Testing](#testing)
+    - [ArbinSpoofer](#arbinspoofer)
+  - [Documentation](#documentation)
+- [License](#license)
+
+## Motivation
+
+Why did we create `pycti-arbin`? This package enables a wide variety of applications such as:
+
+- Real-time data logging, monitoring and alerting
+
+`pycti-arbin` can be used to passively monitor running tests and log readings directly to a database, bypassing the need to manually export data. Moreover, it's possible to create automated alerts based on incoming real-time data. For example, if a test were to fault or temperature were to exceed a set threshold. While Arbin already has a built-in notification system with MacNotify, `pycti-arbin` provides a more flexible and customizable solution without having to directly modify test procedures.
+
+- Automated test management
+
+The GUI provided by Arbin for test management is straight-forward and easy to use, but requires significant manual work. With `pycti-arbin` it is possible to write programs to automatically start tests simultaneously across many channels (or even many cyclers) at once.
+
+- Testing of next generation closed-loop charging methods
+
+While conventional constant-current followed by constant-voltage (CCCV) charging has been the industry standard for many years and is well supported by cyclers, there is movement towards advanced [closed-loop control charging techniques that provide improved battery life and decreased charge times](https://battgenie.life/technology/). `pycti-arbin` enables testing of closed-loop battery charging methods by providing an interface between software hosting battery charging algorithms and active Arbin tests, allowing the charge current to be dynamically set.
+
+- Well tested, easy to use, community supported interface in the most popular programming language.
+
+It is entirely possible to write one's own CTI wrapper, but `pycti-arbin` provides a well-tested ready to use package that takes care of lower level communication, providing a simple yet powerful interface in the most popular programming language.
+
+## Installation
+
+### Using pip
+
+`pycti-arbin` can be installed using pip:
+
+```bash
+pip install pycti-arbin
+```
+
+### Source Installation
+
+To install from source, type the following into the command line:
+
+```bash
+git clone https://github.com/BattGenie/pycti.git
+cd pycti
+pip install -r requirements.txt
+pip install .
+```
+
+## Getting Started
+
+`pycti-arbin` provides two distinct classes for interacting with Arbin cyclers:
+
+- `CyclerInterface` : A cycler-level interface for reading channel status of any channel on the cycler. This class is capable of read only operations on the cycler.
+
+- `ChannelInterface` : A channel-level interface for reading status of a specific channel, starting/stopping tests on that channel, and assigning meta variables during active tests on the channel. This class is capable of read and write operations on a single channel.
+
+### Configuration
+
+Both `CyclerInterface` and `ChannelInterface` require configuration dictionaries upon initialization. The fields of these configuration dictionaries are detailed in the following sections.
+
+#### CyclerInterface Configuration
+
+An example `CyclerInterface` configuration dictionary is shown below:
+
+```python
+CYCLER_INTERFACE_CONFIG = {
+    "ip_address": 127.0.0.1,
+    "port": 1234,
+    "timeout_s": 3,
+    "msg_buffer_size": 4096
+}
+```
+
+Where the fields are as follows:
+
+- `ip_address` : str
+    The IP address of the Arbin host computer.
+- `port` : int
+    The TCP port to communicate through. This is generally going to be 9031
+- `timeout_s` : *optional* : float
+    How long to wait before timing out on TCP communication. Defaults to 3 seconds.
+- `msg_buffer_size` : *optional* : int
+    How big of a message buffer to use for sending/receiving messages.
+    A minimum of 1024 bytes is recommended. Defaults to 4096 bytes.
+
+#### ChannelInterface Configuration
+
+An example `ChannelInterface` configuration dictionary is shown below:
+
+```python
+CHANNEL_INTERFACE_CONFIG = {
+  "channel": 1,
+  "test_name": "fake_test_name",
+  "schedule_name": "Rest+207855.sdx",
+  "ip_address": 127.0.0.1,
+  "port": 1234,
+  "timeout_s": 3,
+  "msg_buffer_size": 4096
+}
+```
+
+Where the fields are as follows:
+
+- `channel` : int
+    The channel to target with the ChannelInterface class instance.
+- `test_name` : *optional* : str
+    The test name to use if using the ChannelInterface to start a test.
+- `schedule_name` : *optional* : str
+    The name of the schedule file to use if using the ChannelInterface to start a test.
+- `ip_address` : str
+    The IP address of the Arbin host computer.
+- `port` : int
+    The TCP port to communicate through. This is generally going to be 7031
+- `timeout_s` : *optional* : float
+    How long to wait before timing out on TCP communication. Defaults to 3 seconds.
+- `msg_buffer_size` : *optional* : int
+    How big of a message buffer to use for sending/receiving messages.
+    A minimum of 1024 bytes is recommended. Defaults to 4096 bytes.
+
+### Env
+
+In addition to a configuration dictionary, both interfaces require a `.env` file containing the Arbin CTI username and password to use for communication. The `.env` file path can be passed as a constructor argument. If it is not specified, the the program looks in the working directly for a `.env` file.
+
+The `.env` file must contain the following fields:
+
+```bash
+ARBIN_CTI_USERNAME='your_username'
+ARBIN_CTI_PASSWORD='your_password'
+```
+
+Where `your_username` and `your_password` should be replaced with your username and password.
+
+### Getting Channel Readings
+
+To get channel readings with a `CyclerInterface` you must specify which channel you want to read from:
+
+```python
+from pyctiarbin import CyclerInterface
+
+CYCLER_INTERFACE_CONFIG = {
+    "ip_address": "127.0.0.1"
+    "port": 1234,
+    "timeout_s": 3,
+    "msg_buffer_size": 4096
+}
+
+cycler_interface = CyclerInterface(CYCLER_INTERFACE_CONFIG)
+cycler_interface.read_channel_status(channel=1)
+```
+
+For a `ChannelInterface` there is no need to specify the channel since we define it in the config:
+
+```python
+from pyctiarbin import ChannelInterface
+
+CHANNEL_INTERFACE_CONFIG = {
+  "channel": 1,
+  "test_name": "fake_test_name",
+  "schedule_name": "Rest+207855.sdx",
+  "ip_address": "127.0.0.1"
+  "port": 1234,
+  "timeout_s": 3,
+  "msg_buffer_size": 4096
+}
+
+channel_interface = ChannelInterface(CHANNEL_INTERFACE_CONFIG)
+channel_interface.read_channel_status()
+```
+
+For more examples of how to use the `CyclerInterface` and `ChannelInterface` class see the `demo_notebook.ipynb` and documentation.
+
+## Tested MITS Pro Version
+
+| Version         | Build      | pycti-arbin |
+|-----------------|------------|-------------|
+| Mits8 PV.202110 | Oct 4 2021 | 0.0.4       |
+|                 |            |             |
+
+## Development
+
+This section contains various information to help developers further extend and test `pycti-arbin`
+
+## Contributing
+
+As it exists now `pycti-arbin` only implements a fraction of the messages supported by CTI. Further work can be done to expand `pycti-arbin` to include more of the messages detailed in the CTI documentation `docs/ArbinCTI_Protocol v1.1.pdf`.
+
+We welcome your help in expanding `pycti-arbin`! Please see the [CONTRIBUTING.md](https://github.com/BattGenie/pycti/blob/main/CONTRIBUTING.md) file in this repository for contribution guidelines.
+
+## Testing
+
+To run the tests navigate to the "tests" directory and type the following:
+
+```bash
+pytest .
+```
+
+To run tests and generate a coverage report:
+
+```bash
+coverage run -m pytest
+```
+
+To view the generated coverage report:
+
+```bash
+coverage report -m 
+```
+
+### ArbinSpoofer
+
+Testing software on a real cycler is dangerous so we've created a submodule `arbinspoofer` to emulate some of the behavior of the Arbin software with a class `ArbinSpoofer`. This class creates a local TCP server and that accepts connections from n number of clients. The `ArbinSpoofer` does not perfectly emulate a Arbin cycler (for example, it does not track if a test is already running on a channel) and merely checks that the message format is correct and responds with standard messages.
+
+## Documentation
+
+All documentation was generated with [pydoc](https://docs.python.org/3/library/pydoc.html). To re-generate the documentation type the following command from the top level directory of the repository:
+
+```bash
+pydoc --html .
+```
+
+## License
+
+MIT License
+
+Copyright (c) 2023 BattGenie Inc.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE
```

### Comparing `pycti-arbin-0.0.8/pyctiarbin/arbinspoofer/arbin_spoofer.py` & `pycti-arbin-0.0.9/pyctiarbin/arbinspoofer/arbin_spoofer.py`

 * *Files identical despite different names*

### Comparing `pycti-arbin-0.0.8/pyctiarbin/channel_interface.py` & `pycti-arbin-0.0.9/pyctiarbin/channel_interface.py`

 * *Files identical despite different names*

### Comparing `pycti-arbin-0.0.8/pyctiarbin/cycler_interface.py` & `pycti-arbin-0.0.9/pyctiarbin/cycler_interface.py`

 * *Files identical despite different names*

### Comparing `pycti-arbin-0.0.8/pyctiarbin/messages.py` & `pycti-arbin-0.0.9/pyctiarbin/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1201,11 +1201,17 @@
                 Returns
                 -------
                 msg_dict : dict
                     The message with items decoded into a dictionary
                 """
                 msg_dict = super().unpack(msg_bin)
 
-                msg_dict['result'] = cls.mv_result_decoder[
-                    ord(msg_dict['result'])]
+                # Convert the result code to a string
+                result = ord(msg_dict['result'])
+                if result not in cls.mv_result_decoder.keys():
+                    logger.warning(
+                        f'Unknown result code {result} for SetMetaVariable message!')
+                    msg_dict['result'] = 'Unknown'
+                else:
+                    msg_dict['result'] = cls.mv_result_decoder[result]
 
                 return msg_dict
```

### Comparing `pycti-arbin-0.0.8/setup.py` & `pycti-arbin-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pycti-arbin",
-    version="0.0.8",
+    version="0.0.9",
     author="Zander Nevitt, Bing Syuan Wang",
     author_email="info@battgenie.life",
     description="A class based Python interface for communication and control of Arbin cyclers over CTI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BattGenie/pycti.git",
     packages=setuptools.find_packages(),
```

