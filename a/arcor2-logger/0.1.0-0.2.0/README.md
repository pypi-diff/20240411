# Comparing `tmp/arcor2_logger-0.1.0.tar.gz` & `tmp/arcor2_logger-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcor2_logger-0.1.0.tar", last modified: Mon Oct 25 07:43:51 2021, max compression
+gzip compressed data, was "arcor2_logger-0.2.0.tar", last modified: Thu Apr 11 09:47:37 2024, max compression
```

## Comparing `arcor2_logger-0.1.0.tar` & `arcor2_logger-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2021-10-25 07:43:51.569653 arcor2_logger-0.1.0/
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       12 2021-10-25 07:43:51.000000 arcor2_logger-0.1.0/MANIFEST.in
--rw-rw-r--   0 ikapinus  (1000) ikapinus  (1000)     1970 2021-10-25 07:43:51.569653 arcor2_logger-0.1.0/PKG-INFO
-drwxrwxr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2021-10-25 07:43:51.569653 arcor2_logger-0.1.0/arcor2_logger/
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        5 2021-10-25 07:43:51.000000 arcor2_logger-0.1.0/arcor2_logger/VERSION
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       96 2021-10-25 07:43:51.000000 arcor2_logger-0.1.0/arcor2_logger/__init__.py
-drwxrwxr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2021-10-25 07:43:51.569653 arcor2_logger-0.1.0/arcor2_logger/object_types/
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2021-10-25 07:43:51.000000 arcor2_logger-0.1.0/arcor2_logger/object_types/__init__.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     2580 2021-10-25 07:43:51.000000 arcor2_logger-0.1.0/arcor2_logger/object_types/logging_mixin.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2021-10-25 07:43:51.000000 arcor2_logger-0.1.0/arcor2_logger/py.typed
-drwxrwxr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2021-10-25 07:43:51.569653 arcor2_logger-0.1.0/arcor2_logger/scripts/
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2021-10-25 07:43:51.000000 arcor2_logger-0.1.0/arcor2_logger/scripts/__init__.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     3566 2021-10-25 07:43:51.000000 arcor2_logger-0.1.0/arcor2_logger/scripts/logger.py
-drwxrwxr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2021-10-25 07:43:51.569653 arcor2_logger-0.1.0/arcor2_logger.egg-info/
--rw-rw-r--   0 ikapinus  (1000) ikapinus  (1000)     1970 2021-10-25 07:43:51.000000 arcor2_logger-0.1.0/arcor2_logger.egg-info/PKG-INFO
--rw-rw-r--   0 ikapinus  (1000) ikapinus  (1000)      510 2021-10-25 07:43:51.000000 arcor2_logger-0.1.0/arcor2_logger.egg-info/SOURCES.txt
--rw-rw-r--   0 ikapinus  (1000) ikapinus  (1000)        1 2021-10-25 07:43:51.000000 arcor2_logger-0.1.0/arcor2_logger.egg-info/dependency_links.txt
--rw-rw-r--   0 ikapinus  (1000) ikapinus  (1000)       69 2021-10-25 07:43:51.000000 arcor2_logger-0.1.0/arcor2_logger.egg-info/entry_points.txt
--rw-rw-r--   0 ikapinus  (1000) ikapinus  (1000)        1 2021-10-25 07:43:51.000000 arcor2_logger-0.1.0/arcor2_logger.egg-info/namespace_packages.txt
--rw-rw-r--   0 ikapinus  (1000) ikapinus  (1000)      146 2021-10-25 07:43:51.000000 arcor2_logger-0.1.0/arcor2_logger.egg-info/requires.txt
--rw-rw-r--   0 ikapinus  (1000) ikapinus  (1000)       14 2021-10-25 07:43:51.000000 arcor2_logger-0.1.0/arcor2_logger.egg-info/top_level.txt
--rw-rw-r--   0 ikapinus  (1000) ikapinus  (1000)       38 2021-10-25 07:43:51.569653 arcor2_logger-0.1.0/setup.cfg
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     2840 2021-10-25 07:43:51.000000 arcor2_logger-0.1.0/setup.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:37.697023 arcor2_logger-0.2.0/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-04-11 09:47:36.000000 arcor2_logger-0.2.0/MANIFEST.in
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     2185 2024-04-11 09:47:37.697023 arcor2_logger-0.2.0/PKG-INFO
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:37.689023 arcor2_logger-0.2.0/arcor2_logger/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        5 2024-04-11 09:47:36.000000 arcor2_logger-0.2.0/arcor2_logger/VERSION
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       96 2024-04-11 09:47:36.000000 arcor2_logger-0.2.0/arcor2_logger/__init__.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:37.693023 arcor2_logger-0.2.0/arcor2_logger/object_types/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:36.000000 arcor2_logger-0.2.0/arcor2_logger/object_types/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2529 2024-04-11 09:47:36.000000 arcor2_logger-0.2.0/arcor2_logger/object_types/logging_mixin.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:36.000000 arcor2_logger-0.2.0/arcor2_logger/py.typed
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:37.697023 arcor2_logger-0.2.0/arcor2_logger/scripts/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:36.000000 arcor2_logger-0.2.0/arcor2_logger/scripts/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3563 2024-04-11 09:47:36.000000 arcor2_logger-0.2.0/arcor2_logger/scripts/logger.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:37.693023 arcor2_logger-0.2.0/arcor2_logger.egg-info/
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     2185 2024-04-11 09:47:37.000000 arcor2_logger-0.2.0/arcor2_logger.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      526 2024-04-11 09:47:37.000000 arcor2_logger-0.2.0/arcor2_logger.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-11 09:47:37.000000 arcor2_logger-0.2.0/arcor2_logger.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       68 2024-04-11 09:47:37.000000 arcor2_logger-0.2.0/arcor2_logger.egg-info/entry_points.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-11 09:47:37.000000 arcor2_logger-0.2.0/arcor2_logger.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      162 2024-04-11 09:47:37.000000 arcor2_logger-0.2.0/arcor2_logger.egg-info/requires.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       14 2024-04-11 09:47:37.000000 arcor2_logger-0.2.0/arcor2_logger.egg-info/top_level.txt
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      835 2024-04-11 09:47:36.000000 arcor2_logger-0.2.0/backend_shim.py
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-04-11 09:47:37.697023 arcor2_logger-0.2.0/setup.cfg
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3109 2024-04-11 09:47:36.000000 arcor2_logger-0.2.0/setup.py
```

### Comparing `arcor2_logger-0.1.0/PKG-INFO` & `arcor2_logger-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: arcor2_logger
-Version: 0.1.0
+Version: 0.2.0
 Summary: ARCOR2 Logger service.
-Home-page: UNKNOWN
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: ==3.8.*
+Requires-Python: ==3.11.*
 Description-Content-Type: text/markdown
 
 # arcor2_logger
 
 The service provides logging capabilities through the network. Logging-related methods are added to ObjectTypes using a mixin class.
 
 - Messages are sent using the websockets protocol.
@@ -49,9 +47,21 @@
 ## Environment variables
 
 - `ARCOR2_LOGGER_URL=ws://0.0.0.0:8765` - by default, the service listens on port 8765.
 - `ARCOR2_LOGGER_LEVEL=info` - by default, messages from objects with level `info` and higher are logged.
   - Other possible values are `warning`, `error` and `debug`. 
 - `ARCOR2_LOGGER_DEBUG=1` - switches logger to the `DEBUG` level.
 - `ARCOR2_LOGGER_ASYNCIO_DEBUG=1` - turns on `asyncio` debug output (helpful to debug problems related to concurrency).
+# Changelog
 
+The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [0.2.0] - 2024-04-11
+
+### Changed
+
+- Updated dependencies, switched to Python 3.11.
+
+## [0.1.0] - 2022-10-28
+
+### Changed
+- First version of the package.
```

### Comparing `arcor2_logger-0.1.0/arcor2_logger/object_types/logging_mixin.py` & `arcor2_logger-0.2.0/arcor2_logger/object_types/logging_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
-import abc
 import concurrent.futures as cf
 import logging
 import os
 from dataclasses import dataclass
-from typing import Optional, Protocol
+from typing import Protocol
 
 import websocket
 from dataclasses_jsonschema import JsonSchemaMixin
 
 from arcor2.data.common import IntEnum
 from arcor2.exceptions import Arcor2Exception
 
@@ -18,15 +17,14 @@
     INFO = logging.INFO
     WARNING = logging.WARNING
     ERROR = logging.ERROR
     DEBUG = logging.DEBUG
 
     @classmethod
     def from_string(cls, value: str) -> Level:
-
         if value == "info":
             return cls.INFO
         elif value == "warning":
             return cls.WARNING
         elif value == "error":
             return cls.ERROR
         elif value == "debug":
@@ -40,27 +38,25 @@
     id: str
     name: str
     type: str
 
 
 @dataclass
 class LogMessage(JsonSchemaMixin):
-
     message: str
     level: Level
 
 
 class Logger:
     def __init__(self, obj: GenericProtocol) -> None:
-
         self._ws = websocket.WebSocket()
         self._ws.connect(os.getenv("ARCOR2_LOGGER_URL", "ws://0.0.0.0:8765"))
         self._executor = cf.ThreadPoolExecutor(max_workers=1)
         self._executor.submit(self._ws.send, Register(obj.id, obj.name, obj.__class__.__name__).to_json())
-        self._last_task: Optional[cf.Future] = None
+        self._last_task: None | cf.Future = None
 
     def _log(self, message: str, level: Level) -> None:
         if not self._ws.connected:
             raise Arcor2Exception("Not connected to the Logger service.")
         msg = LogMessage(message, level).to_json()
         self._last_task = self._executor.submit(self._ws.send, msg)
 
@@ -73,15 +69,14 @@
     def error(self, message: str) -> None:
         self._log(message, Level.ERROR)
 
     def __del__(self) -> None:
         self.close()
 
     def close(self) -> None:
-
         if self._last_task:
             try:
                 cf.wait([self._last_task], 1.0)
             except cf.TimeoutError:
                 pass
         self._ws.close()
 
@@ -92,15 +87,15 @@
         ...
 
     @property
     def name(self) -> str:
         ...
 
 
-class LoggingMixin(metaclass=abc.ABCMeta):
+class LoggingMixin:
     """Provides logging capabilities to ObjectTypes.
 
     Calls to all log_ methods are non-blocking.
     """
 
     def get_logger(self: GenericProtocol) -> Logger:
         return Logger(self)
```

### Comparing `arcor2_logger-0.1.0/arcor2_logger/scripts/logger.py` & `arcor2_logger-0.2.0/arcor2_logger/scripts/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import argparse
 import os
 import sys
 
 import websockets
 from aiologger.levels import LogLevel
 from aiorun import run
-from arcor2_logger import version
-from arcor2_logger.object_types.logging_mixin import Level, LogMessage, Register
 from dataclasses_jsonschema import ValidationError
 from websockets.server import WebSocketServerProtocol as WsClient
 
 from arcor2 import env
 from arcor2.exceptions import Arcor2Exception
 from arcor2.helpers import port_from_url
 from arcor2.logging import get_aiologger
+from arcor2_logger import version
+from arcor2_logger.object_types.logging_mixin import Level, LogMessage, Register
 
 logger = get_aiologger("Logger")
 
 logging_level = Level.from_string(os.getenv("ARCOR2_LOGGER_LEVEL", "info"))
 
 # TODO maybe use the same machinery (arcor2/ws_server) for RPCs/Events as in ARServer/Execution?
 # ...but for now this is much more simpler and just enough
 
 
 async def handle_requests(websocket: WsClient, path: str) -> None:
-
     assert not sys.stdout.closed  # closed stdout was problem when creating and shutting down logger for each client
 
     try:
         data = await websocket.recv()
     except websockets.exceptions.ConnectionClosed:
         return
 
@@ -40,15 +39,14 @@
         logger.debug(f"Got invalid data. Expected '{Register.__name__}', received {data}. {str(e)}")
         return
 
     logger.info(f"{register.name} of type {register.type} just arrived to the party.")
 
     try:
         async for message in websocket:
-
             assert isinstance(message, str)
 
             try:
                 lm = LogMessage.from_json(message)
             except (ValidationError, Arcor2Exception) as e:
                 logger.debug(
                     f"Invalid data from {register.name}. Expected '{LogMessage.__name__}', received {message}. {str(e)}"
@@ -73,15 +71,14 @@
         logger.debug(f"Connection from {register.name} closed!")
         return
 
     logger.info(f"{register.name} of type {register.type} is leaving.")
 
 
 async def aio_main() -> None:
-
     await websockets.server.serve(
         handle_requests, "localhost", port_from_url(os.getenv("ARCOR2_LOGGER_URL", "ws://0.0.0.0:8765"))
     )
     await logger.info(f"Logger service {version()} started. Logging level is {logging_level.name}.")
 
 
 def main() -> None:
```

### Comparing `arcor2_logger-0.1.0/arcor2_logger.egg-info/PKG-INFO` & `arcor2_logger-0.2.0/arcor2_logger.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: arcor2-logger
-Version: 0.1.0
+Version: 0.2.0
 Summary: ARCOR2 Logger service.
-Home-page: UNKNOWN
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: ==3.8.*
+Requires-Python: ==3.11.*
 Description-Content-Type: text/markdown
 
 # arcor2_logger
 
 The service provides logging capabilities through the network. Logging-related methods are added to ObjectTypes using a mixin class.
 
 - Messages are sent using the websockets protocol.
@@ -49,9 +47,21 @@
 ## Environment variables
 
 - `ARCOR2_LOGGER_URL=ws://0.0.0.0:8765` - by default, the service listens on port 8765.
 - `ARCOR2_LOGGER_LEVEL=info` - by default, messages from objects with level `info` and higher are logged.
   - Other possible values are `warning`, `error` and `debug`. 
 - `ARCOR2_LOGGER_DEBUG=1` - switches logger to the `DEBUG` level.
 - `ARCOR2_LOGGER_ASYNCIO_DEBUG=1` - turns on `asyncio` debug output (helpful to debug problems related to concurrency).
+# Changelog
 
+The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [0.2.0] - 2024-04-11
+
+### Changed
+
+- Updated dependencies, switched to Python 3.11.
+
+## [0.1.0] - 2022-10-28
+
+### Changed
+- First version of the package.
```

### Comparing `arcor2_logger-0.1.0/setup.py` & `arcor2_logger-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,19 +8,32 @@
     'author': 'Robo@FIT',
     'author_email': 'imaterna@fit.vut.cz',
     'classifiers': [
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
-        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
         'Natural Language :: English',
         'Topic :: Scientific/Engineering',
     ],
     'description': 'ARCOR2 Logger service.',
+    'entry_points': {
+        'console_scripts': [
+            'arcor2_logger = arcor2_logger.scripts.logger:main',
+        ],
+    },
+    'install_requires': (
+        'aiologger~=0.7.0',
+        'aiorun~=2023.7.2',
+        'arcor2~=1.3.0',
+        'dataclasses-jsonschema[apispec,fast-dateparsing,fast-validation]~=2.16.0',
+        'websocket-client~=1.7.0',
+        'websockets~=12.0',
+    ),
     'license': 'LGPL',
     'long_description': """# arcor2_logger
 
 The service provides logging capabilities through the network. Logging-related methods are added to ObjectTypes using a mixin class.
 
 - Messages are sent using the websockets protocol.
 - Calls to `log_` methods are non-blocking.
@@ -50,39 +63,39 @@
 ## Environment variables
 
 - `ARCOR2_LOGGER_URL=ws://0.0.0.0:8765` - by default, the service listens on port 8765.
 - `ARCOR2_LOGGER_LEVEL=info` - by default, messages from objects with level `info` and higher are logged.
   - Other possible values are `warning`, `error` and `debug`. 
 - `ARCOR2_LOGGER_DEBUG=1` - switches logger to the `DEBUG` level.
 - `ARCOR2_LOGGER_ASYNCIO_DEBUG=1` - turns on `asyncio` debug output (helpful to debug problems related to concurrency).
-""",
+# Changelog
+
+The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
+
+## [0.2.0] - 2024-04-11
+
+### Changed
+
+- Updated dependencies, switched to Python 3.11.
+
+## [0.1.0] - 2022-10-28
+
+### Changed
+- First version of the package.""",
     'long_description_content_type': 'text/markdown',
     'name': 'arcor2_logger',
-    'python_requires': '==3.8.*',
-    'version': '0.1.0',
-    'packages': (
-        'arcor2_logger',
-        'arcor2_logger.object_types',
-        'arcor2_logger.scripts',
-    ),
     'namespace_packages': (
     ),
     'package_data': {
         'arcor2_logger': (
             'VERSION',
             'py.typed',
         ),
     },
-    'install_requires': (
-        'aiologger==0.6.1',
-        'aiorun==2021.8.1',
-        'arcor2~=0.22.0',
-        'dataclasses-jsonschema[apispec,fast-validation]==2.15.0',
-        'websocket-client==1.2.1',
-        'websockets==10.0',
+    'packages': (
+        'arcor2_logger',
+        'arcor2_logger.object_types',
+        'arcor2_logger.scripts',
     ),
-    'entry_points': {
-        'console_scripts': [
-            'arcor2_logger = arcor2_logger.scripts.logger:main',
-        ],
-    },
+    'python_requires': '==3.11.*',
+    'version': '0.2.0',
 })
```

