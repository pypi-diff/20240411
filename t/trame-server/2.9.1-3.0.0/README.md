# Comparing `tmp/trame-server-2.9.1.tar.gz` & `tmp/trame-server-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-server-2.9.1.tar", last modified: Wed Feb 15 18:48:29 2023, max compression
+gzip compressed data, was "trame-server-3.0.0.tar", last modified: Wed Apr 10 22:56:44 2024, max compression
```

## Comparing `trame-server-2.9.1.tar` & `trame-server-3.0.0.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 18:48:29.024079 trame-server-2.9.1/
--rw-r--r--   0 root         (0) root         (0)      552 2023-02-15 18:48:25.000000 trame-server-2.9.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-15 18:48:25.000000 trame-server-2.9.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4318 2023-02-15 18:48:29.024079 trame-server-2.9.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3585 2023-02-15 18:48:25.000000 trame-server-2.9.1/README.rst
--rw-r--r--   0 root         (0) root         (0)      888 2023-02-15 18:48:29.024079 trame-server-2.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-15 18:48:25.000000 trame-server-2.9.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 18:48:29.020079 trame-server-2.9.1/trame_server/
--rw-r--r--   0 root         (0) root         (0)      552 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/LICENSE
--rw-r--r--   0 root         (0) root         (0)      170 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10511 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/controller.py
--rw-r--r--   0 root         (0) root         (0)    20952 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/core.py
--rw-r--r--   0 root         (0) root         (0)     7223 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/protocol.py
--rw-r--r--   0 root         (0) root         (0)     6754 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/state.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 18:48:29.024079 trame-server-2.9.1/trame_server/utils/
--rw-r--r--   0 root         (0) root         (0)     2636 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5396 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/utils/asynchronous.py
--rw-r--r--   0 root         (0) root         (0)      455 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/utils/browser.py
--rw-r--r--   0 root         (0) root         (0)     2208 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/utils/desktop.py
--rw-r--r--   0 root         (0) root         (0)     9859 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/utils/hot_reload.py
--rw-r--r--   0 root         (0) root         (0)     1966 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/utils/server.py
--rw-r--r--   0 root         (0) root         (0)      552 2023-02-15 18:48:25.000000 trame-server-2.9.1/trame_server/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 18:48:29.020079 trame-server-2.9.1/trame_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4318 2023-02-15 18:48:29.000000 trame-server-2.9.1/trame_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      635 2023-02-15 18:48:29.000000 trame-server-2.9.1/trame_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-15 18:48:29.000000 trame-server-2.9.1/trame_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-02-15 18:48:29.000000 trame-server-2.9.1/trame_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-02-15 18:48:29.000000 trame-server-2.9.1/trame_server.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:56:44.695624 trame-server-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)      552 2024-04-10 22:56:42.000000 trame-server-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 22:56:42.000000 trame-server-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4414 2024-04-10 22:56:44.695624 trame-server-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3681 2024-04-10 22:56:42.000000 trame-server-3.0.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)      903 2024-04-10 22:56:44.695624 trame-server-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 22:56:42.000000 trame-server-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:56:44.695624 trame-server-3.0.0/trame_server/
+-rw-r--r--   0 root         (0) root         (0)      552 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      211 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10337 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/client.py
+-rw-r--r--   0 root         (0) root         (0)    12544 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/controller.py
+-rw-r--r--   0 root         (0) root         (0)    25206 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/core.py
+-rw-r--r--   0 root         (0) root         (0)     7658 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/protocol.py
+-rw-r--r--   0 root         (0) root         (0)     9229 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/state.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:56:44.695624 trame-server-3.0.0/trame_server/utils/
+-rw-r--r--   0 root         (0) root         (0)     2785 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3075 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/argument_parser.py
+-rw-r--r--   0 root         (0) root         (0)     5396 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/asynchronous.py
+-rw-r--r--   0 root         (0) root         (0)      455 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/browser.py
+-rw-r--r--   0 root         (0) root         (0)     4884 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/desktop.py
+-rw-r--r--   0 root         (0) root         (0)    10103 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/hot_reload.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2767 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/namespace.py
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/server.py
+-rw-r--r--   0 root         (0) root         (0)      552 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:56:44.695624 trame-server-3.0.0/trame_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4414 2024-04-10 22:56:44.000000 trame-server-3.0.0/trame_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      728 2024-04-10 22:56:44.000000 trame-server-3.0.0/trame_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 22:56:44.000000 trame-server-3.0.0/trame_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 22:56:44.000000 trame-server-3.0.0/trame_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-10 22:56:44.000000 trame-server-3.0.0/trame_server.egg-info/top_level.txt
```

### Comparing `trame-server-2.9.1/LICENSE` & `trame-server-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.1/PKG-INFO` & `trame-server-3.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-server
-Version: 2.9.1
+Version: 3.0.0
 Summary: Internal server side implementation of trame
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
@@ -51,14 +51,15 @@
 
 **Environments variables**
 
 * **TRAME_LOG_NETWORK**     : Path to log file for capturing network exchange. (default: None)
 * **TRAME_WS_MAX_MSG_SIZE** : Maximum size in bytes of any ws message. (default: 10MB)
 * **TRAME_WS_HEART_BEAT**   : Time in second before assuming the server is non-responsive. (default: 30s)
 * **TRAME_DESKTOP_DEBUG**   : If defined it will allow user to inspect the web content in desktop mode
+* **TRAME_SERVER**          : If set to true, this will prevent browser from opening by default
 
 
 **Life cycle callbacks**
 
 Life cycle events are directly managed on the application controller
 and are prefixed with `on_*`.
```

### Comparing `trame-server-2.9.1/README.rst` & `trame-server-3.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 **Environments variables**
 
 * **TRAME_LOG_NETWORK**     : Path to log file for capturing network exchange. (default: None)
 * **TRAME_WS_MAX_MSG_SIZE** : Maximum size in bytes of any ws message. (default: 10MB)
 * **TRAME_WS_HEART_BEAT**   : Time in second before assuming the server is non-responsive. (default: 30s)
 * **TRAME_DESKTOP_DEBUG**   : If defined it will allow user to inspect the web content in desktop mode
+* **TRAME_SERVER**          : If set to true, this will prevent browser from opening by default
 
 
 **Life cycle callbacks**
 
 Life cycle events are directly managed on the application controller
 and are prefixed with `on_*`.
```

### Comparing `trame-server-2.9.1/setup.cfg` & `trame-server-3.0.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-server
-version = 2.9.1
+version = 3.0.0
 description = Internal server side implementation of trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache License 2.0
 classifiers = 
 	Development Status :: 5 - Production/Stable
@@ -22,15 +22,16 @@
 	Application
 	Framework
 
 [options]
 packages = find:
 include_package_data = True
 install_requires = 
-	wslink>=1.9.0
+	wslink>=2,<3
+	more-itertools
 
 [semantic_release]
 version_pattern = setup.cfg:version = (\d+\.\d+\.\d+)
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `trame-server-2.9.1/trame_server/LICENSE` & `trame-server-3.0.0/trame_server/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.1/trame_server/controller.py` & `trame-server-3.0.0/trame_server/controller.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,22 @@
-from .utils import is_dunder, asynchronous
+import logging
+from .utils import is_dunder, asynchronous, share
 from .utils.hot_reload import reload
+from .utils.namespace import Translator
+
+logger = logging.getLogger(__name__)
+
+
+class TriggerCounter:
+    def __init__(self, init=0):
+        self._count = init
+
+    def next(self):
+        self._count += 1
+        return self._count
 
 
 class Controller:
     """Controller acts as a container for function proxies
 
     It allows functions to be passed around that are not yet defined,
     and can be defined or re-defined later. For example:
@@ -26,40 +39,79 @@
     >>> ctrl.on_data_change()
     "Update pipeline!"
     "Wow that is pretty cool!"
     "Update view!"
     >>> ctrl.on_data_change.clear(set_only=True) # add, remove, discard, clear
     """
 
-    def __init__(self, server):
-        super().__setattr__("_server", server)
-        super().__setattr__("_func_dict", {})
-
-    @property
-    def trigger(self):
-        return self._server.trigger
-
-    @property
-    def trigger_name(self):
-        return self._server.trigger_name
-
-    @property
-    def __trame_hot_reload__(self):
-        return self._server.hot_reload
+    def __init__(self, translator=None, internal=None, hot_reload=False):
+        super().__setattr__("__trame_hot_reload__", hot_reload)
+        super().__setattr__("_translator", translator if translator else Translator())
+        super().__setattr__("_triggers", share(internal, "_triggers", {}))
+        super().__setattr__(
+            "_triggers_fn2name", share(internal, "_triggers_fn2name", {})
+        )
+        super().__setattr__(
+            "_triggers_name_id", share(internal, "_triggers_name_id", TriggerCounter())
+        )
+        super().__setattr__("_func_dict", share(internal, "_func_dict", {}))
+
+    def trigger(self, name):
+        """
+        Use as decorator `@server.trigger(name)` so the decorated function
+        will be able to be called from the client by doing `click="trigger(name)"`.
+
+        :param name: A name to use for that trigger
+        :type name: str
+        """
+        name = self._translator.translate_key(name)
+
+        def register_trigger(func):
+            logger.info("trigger(%s)", name)
+            self._triggers[name] = func
+            self._triggers_fn2name[func] = name
+            return func
+
+        return register_trigger
+
+    def trigger_name(self, fn):
+        """
+        Given a function this method will register a trigger and returned its name.
+        If manually registered, the given name at the time will be returned.
+
+        :return: The trigger name for that function
+        :rtype: str
+        """
+        if fn in self._triggers_fn2name:
+            return self._triggers_fn2name[fn]
+
+        name = f"trigger__{self._triggers_name_id.next()}"
+        self.trigger(name)(fn)
+        return name
+
+    def trigger_fn(self, name):
+        """
+        Given a trigger name get its attached function/method.
+
+        :return: The trigger function for that name
+        :rtype: function
+        """
+        return self._triggers.get(name)
 
     def __getitem__(self, name):
         return self.__getattr__(name)
 
     def __setitem__(self, name, value):
         self.__setattr__(name, value)
 
     def __getattr__(self, name):
         if is_dunder(name):
             return super().__getattr__(name)
 
+        name = self._translator.translate_key(name)
         if name not in self._func_dict:
             self._func_dict[name] = ControllerFunction(self, name)
 
         return self._func_dict[name]
 
     def __setattr__(self, name, func):
         # Do not allow pre-existing attributes, such as `trigger`, to be
@@ -67,14 +119,15 @@
         if name in self.__dict__ or name in Controller.__dict__:
             msg = (
                 f"'{name}' is a special attribute on Controller that cannot "
                 "be re-assigned"
             )
             raise Exception(msg)
 
+        name = self._translator.translate_key(name)
         if name in self._func_dict:
             self._func_dict[name].func = func
         else:
             self._func_dict[name] = ControllerFunction(self, name, func)
 
     def add(self, name, clear=False):
         """
@@ -107,14 +160,15 @@
                 pass
 
             # or
             ctrl.on_server_ready.clear()
             ctrl.on_server_ready.add(on_ready)
 
         """
+        name = self._translator.translate_key(name)
 
         def register_ctrl_method(func):
             if clear:
                 self[name].clear()
 
             self[name].add(func)
             return func
@@ -137,14 +191,15 @@
             def on_ready(**state):
                 pass
 
             # or
             ctrl.on_server_ready.once(on_ready)
 
         """
+        name = self._translator.translate_key(name)
 
         def register_ctrl_method(func):
             self[name].once(func)
             return func
 
         return register_ctrl_method
 
@@ -179,14 +234,15 @@
                 pass
 
             # or
             ctrl.on_server_ready.clear()
             ctrl.on_server_ready.add_task(on_ready)
 
         """
+        name = self._translator.translate_key(name)
 
         def register_ctrl_method(func):
             if clear:
                 self[name].clear()
 
             self[name].add_task(func)
             return func
@@ -224,14 +280,15 @@
                 pass
 
             # or
             ctrl.on_server_ready.clear()
             ctrl.on_server_ready = on_ready
 
         """
+        name = self._translator.translate_key(name)
 
         def register_ctrl_method(func):
             if clear:
                 self[name].clear()
 
             self[name] = func
             return func
@@ -280,17 +337,14 @@
             copy_list = list(map(reload, copy_list))
 
         # Exec added fn after
         results = list(map(lambda f: f(*args, **kwargs), copy_list))
 
         # Schedule any task
         for task_fn in list(self.task_funcs):
-            if self.hot_reload:
-                task_fn = reload(task_fn)
-
             results.append(asynchronous.create_task(task_fn(*args, **kwargs)))
 
         # Figure out return
         if self.func is None:
             return results
         elif len(copy_list):
             return [result, *results]
```

### Comparing `trame-server-2.9.1/trame_server/core.py` & `trame-server-3.0.0/trame_server/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,33 @@
-import argparse
 import asyncio
 import inspect
 import logging
 import os
 import sys
+from typing import Optional
+
 
 from . import utils
 
 from .state import State
 from .controller import Controller
 from .ui import VirtualNodeManager
 from .protocol import CoreServer
+from .utils.argument_parser import ArgumentParser
+from .utils.namespace import Translator
+from .utils import share
+
+logger = logging.getLogger(__name__)
+
+DEFAULT_CLIENT_TYPE = "vue3"
+
+
+def set_default_client_type(value):
+    global DEFAULT_CLIENT_TYPE
+    DEFAULT_CLIENT_TYPE = value
 
 
 class Server:
     """
     Server implementation for trame.
     This is the core object that manage client/server communication but also
     holds a state and controller instance.
@@ -29,81 +42,106 @@
     :param name: A name identifier for a given server
     :type name: str, optional (default: trame)
 
     :param **options: Gather any keyword arguments into options
     :type options: Dict
     """
 
-    def __init__(self, name="trame", vn_constructor=None, **options):
+    def __init__(
+        self,
+        name="trame",
+        vn_constructor=None,
+        translator=None,
+        parent_server=None,
+        **options,
+    ):
         # Core internal variables
+        self._parent_server = parent_server
+        self._translator = translator if translator else Translator()
+        self._name = share(parent_server, "_name", name)
+        self._options = share(parent_server, "_options", options)
+        self._client_type = share(parent_server, "_client_type", None)
+
+        # use parent_server instead of local version
         self._server = None
-        self._running_port = 0
         self._running_stage = 0  # 0: off / 1: pending / 2: running
+        self._running_port = 0
         self._running_future = None
-        self._name = name
         self._www = None
-        self._options = options
-        self._client_type = None
-
-        # Controller
-        self._controller = Controller(self)
-
-        # UI
-        self._ui = VirtualNodeManager(self, vn_constructor)
-
-        # HTTP server
-        self.serve = {}
-
-        # @change
-        self._change_callbacks = {}
-
-        # @trigger
-        self._triggers = {}
-        self._triggers_fn2name = {}
-        self._triggers_name_id = 0
-
-        # CLI argument handling
-        self._cli_parser = None
-
-        # modules
+        self.serve = {}  # HTTP static endpoints
         self._loaded_modules = set()
-
-        # protocols to register
+        self._cli_parser = None
         self._root_protocol = None
         self._protocols_to_configure = []
 
-        # Shared state + reserve internal keys
-        self._state = State(self)
-        for key in ["scripts", "module_scripts", "styles", "vue_use", "mousetrap"]:
-            self._state[f"trame__{key}"] = []
-        self._state.trame__client_only = ["trame__busy"]
-        self._state.trame__busy = 1
-        self._state.trame__favicon = None
-        self._state.trame__title = "Trame"
-
         # ENV variable mapping settings
-        self._options["log_network"] = self._options.get(
-            "log_network", os.environ.get("TRAME_LOG_NETWORK", False)
-        )
-        self._options["ws_max_msg_size"] = self._options.get(
-            "ws_max_msg_size", os.environ.get("TRAME_WS_MAX_MSG_SIZE", 10000000)
-        )
-        self._options["ws_heart_beat"] = self._options.get(
-            "ws_heart_beat", os.environ.get("TRAME_WS_HEART_BEAT", 30)
-        )
-        self._options["desktop_debug"] = self._options.get(
-            "desktop_debug", os.environ.get("TRAME_DESKTOP_DEBUG", False)
-        )
-        # reset default wslink startup message
-        os.environ["WSLINK_READY_MSG"] = ""
-
-        # Initialize hot reload
         self.hot_reload = "--hot-reload" in sys.argv or bool(
             os.getenv("TRAME_HOT_RELOAD", False)
         )
+        if parent_server is None:
+            self._options["log_network"] = self._options.get(
+                "log_network", os.environ.get("TRAME_LOG_NETWORK", False)
+            )
+            self._options["ws_max_msg_size"] = self._options.get(
+                "ws_max_msg_size", os.environ.get("TRAME_WS_MAX_MSG_SIZE", 10000000)
+            )
+            self._options["ws_heart_beat"] = self._options.get(
+                "ws_heart_beat", os.environ.get("TRAME_WS_HEART_BEAT", 30)
+            )
+            self._options["desktop_debug"] = self._options.get(
+                "desktop_debug", os.environ.get("TRAME_DESKTOP_DEBUG", False)
+            )
+            # reset default wslink startup message
+            os.environ["WSLINK_READY_MSG"] = ""
+
+        # Shared state + reserve internal keys
+        if parent_server is None:
+            self._state = State(
+                self.translator, commit_fn=self._push_state, hot_reload=self.hot_reload
+            )
+            for key in ["scripts", "module_scripts", "styles", "vue_use", "mousetrap"]:
+                self._state[f"trame__{key}"] = []
+            self._state.trame__client_only = ["trame__busy"]
+            self._state.trame__busy = 1
+            self._state.trame__favicon = None
+            self._state.trame__title = "Trame"
+        else:
+            self._state = State(
+                self.translator,
+                internal=parent_server._state,
+                commit_fn=self._push_state,
+                hot_reload=self.hot_reload,
+            )
+
+        # Controller
+        if parent_server is None:
+            self._controller = Controller(self.translator, hot_reload=self.hot_reload)
+        else:
+            self._controller = Controller(
+                self.translator,
+                internal=parent_server._controller,
+                hot_reload=self.hot_reload,
+            )
+
+        # Server only context
+        if parent_server is None:
+            self._context = State(self.translator, hot_reload=self.hot_reload)
+        else:
+            self._context = State(
+                self.translator,
+                internal=parent_server._context,
+                hot_reload=self.hot_reload,
+            )
+
+        # UI (FIXME): use for translator
+        self._ui = share(parent_server, "_ui", VirtualNodeManager(self, vn_constructor))
+
+    def create_child_server(self, translator=None, prefix=None):
+        translator = translator if translator else Translator(prefix=prefix)
+        return Server(translator=translator, parent_server=self)
 
     # -------------------------------------------------------------------------
     # State management helpers
     # -------------------------------------------------------------------------
 
     def _push_state(self, state):
         if self.protocol:
@@ -130,14 +168,18 @@
           - state = {}             : Set of variable to add to state
           - server = { data: '/path/on/fs' }: Set of endpoints to server static content
           - www = '/path/on/fs'    : Path served as main web content
 
         :param module: A module to enable or a dict()
         :param kwargs: Any optional parameters needed for your module setup() function.
         """
+        if self.root_server != self:
+            self.root_server.enable_module(module, **kwargs)
+            return
+
         # Make sure definitions is a dict while skipping already loaded module
         definitions = module
         if isinstance(definitions, dict):
             definitions = module
         elif definitions in self._loaded_modules:
             return
         else:
@@ -191,91 +233,85 @@
                 ]
             )
 
     # -------------------------------------------------------------------------
     # Annotations
     # -------------------------------------------------------------------------
 
-    def change(self, *_args, **_kwargs):
+    @property
+    def change(self):
         """
         Use as decorator `@server.change(key1, key2, ...)` so the decorated function
         will be called like so `_fn(**state)` when any of the listed key name
         is getting modified from either client or server.
 
         :param *_args: A list of variable name to monitor
         :type *_args: str
         """
-
-        def register_change_callback(func):
-            for name in _args:
-                if name not in self._change_callbacks:
-                    self._change_callbacks[name] = []
-
-                self._change_callbacks[name].append(func)
-            return func
-
-        return register_change_callback
+        return self._state.change
 
     # -------------------------------------------------------------------------
 
-    def trigger(self, name):
+    @property
+    def trigger(self):
         """
         Use as decorator `@server.trigger(name)` so the decorated function
         will be able to be called from the client by doing `click="trigger(name)"`.
 
         :param name: A name to use for that trigger
         :type name: str
         """
-
-        def register_trigger(func):
-            self._triggers[name] = func
-            self._triggers_fn2name[func] = name
-            return func
-
-        return register_trigger
+        return self._controller.trigger
 
     # -------------------------------------------------------------------------
     # From a function get its trigger name and register it if need be
     # -------------------------------------------------------------------------
 
-    def trigger_name(self, fn):
+    @property
+    def trigger_name(self):
         """
         Given a function this method will register a trigger and returned its name.
         If manually registered, the given name at the time will be returned.
 
         :return: The trigger name for that function
         :rtype: str
         """
-        if fn in self._triggers_fn2name:
-            return self._triggers_fn2name[fn]
-
-        self._triggers_name_id += 1
-        name = f"trigger__{self._triggers_name_id}"
-        self.trigger(name)(fn)
-        return name
+        return self._controller.trigger_name
 
     # -------------------------------------------------------------------------
     # App properties
     # -------------------------------------------------------------------------
 
     @property
     def name(self):
         """Name of server"""
         return self._name
 
     @property
+    def root_server(self):
+        """Root server to start"""
+        if self._parent_server:
+            return self._parent_server.root_server
+        return self
+
+    @property
+    def translator(self):
+        """Translator of the server"""
+        return self._translator
+
+    @property
     def options(self):
         """Server options provided at instantiation time"""
         return self._options
 
     @property
     def client_type(self):
         """Specify the client type. Either 'vue2' or 'vue3' for now."""
         if self._client_type is None:
-            return "vue2"  # default
+            return DEFAULT_CLIENT_TYPE  # default
         return self._client_type
 
     @client_type.setter
     def client_type(self, value):
         """Should only be called once before any widget initialization"""
         if self._client_type is None:
             self._client_type = value
@@ -287,18 +323,21 @@
                 The client_type can only be set once.
             """
             )
 
     @property
     def cli(self):
         """argparse parser"""
+        if self.root_server != self:
+            return self.root_server.cli
+
         if self._cli_parser:
             return self._cli_parser
 
-        self._cli_parser = argparse.ArgumentParser(description="Kitware trame")
+        self._cli_parser = ArgumentParser(description="Kitware trame")
 
         # Trame specific args
         self._cli_parser.add_argument(
             "--server",
             help="Prevent your browser from opening at startup",
             action="store_true",
         )
@@ -322,28 +361,45 @@
         self._cli_parser.add_argument(
             "--hot-reload",
             help="""Automatically reload state/controller callback functions for every
                     function call. This allows live editing of the functions. Functions
                     located in the site-packages directories are skipped.""",
             action="store_true",
         )
+        self._cli_parser.add_argument(
+            "--trame-args",
+            help="""If specified, trame will ignore all other arguments, and only the contents
+                    of the `--trame-args` will be used. For example:
+                    `--trame-args="-p 8081 --server"`. Alternatively, the environment variable
+                    `TRAME_ARGS` may be set instead.""",
+        )
 
         CoreServer.add_arguments(self._cli_parser)
 
         return self._cli_parser
 
     @property
     def state(self):
         """
         :return: The server shared state
         :rtype: trame_server.state.State
         """
         return self._state
 
     @property
+    def context(self):
+        """
+        The server-only context (not shared with the client).
+
+        :return: The server context state
+        :rtype: trame_server.state.State
+        """
+        return self._context
+
+    @property
     def controller(self):
         """
         :return: The server controller
         :rtype: trame_server.controller.Controller
         """
         return self._controller
 
@@ -354,19 +410,25 @@
         :rtype: trame_server.ui.VirtualNodeManager
         """
         return self._ui
 
     @property
     def running(self):
         """Return True if the server is currently starting or running."""
+        if self.root_server != self:
+            return self.root_server.running
+
         return self._running_stage > 1
 
     @property
     def ready(self):
         """Return a future that will resolve once the server is ready"""
+        if self.root_server != self:
+            return self.root_server.ready
+
         if self._running_future is None:
             self._running_future = asyncio.get_running_loop().create_future()
 
         return self._running_future
 
     # -------------------------------------------------------------------------
     # API for network handling
@@ -386,19 +448,26 @@
         """
         Register function that will be called with a wslink.ServerProtocol
         when the server start and is ready for registering new wslink.Protocol.
 
         :param configure_protocol_fn: A function to be called later with a
                                       wslink.ServerProtocol as argument.
         """
+        if self.root_server != self:
+            self.root_server.add_protocol_to_configure(configure_protocol_fn)
+            return
+
         self._protocols_to_configure.append(configure_protocol_fn)
 
     @property
     def protocol(self):
         """Return the server root protocol"""
+        if self.root_server != self:
+            return self.root_server.protocol
+
         return self._root_protocol
 
     # -------------------------------------------------------------------------
 
     def protocol_call(self, method, *args, **kwargs):
         """
         Call a registered protocol method
@@ -411,26 +480,36 @@
         """
         if self.protocol:
             pair = self.protocol.getRPCMethod(method)
             if pair:
                 obj, func = pair
                 return func(obj, *args, **kwargs)
 
+    def force_state_push(self, *key_names):
+        """
+        Should only be needed when client corrupted its data and need the server need to send it again.
+
+        :param *args: Set of key names to be send again to the client.
+        """
+        self.protocol_call(
+            "trame.force.push", *[self._translator.translate_key(k) for k in key_names]
+        )
+
     # -------------------------------------------------------------------------
     # Server handling (start/stop/port)
     # -------------------------------------------------------------------------
 
     def start(
         self,
         port: int = None,
         thread: bool = False,
-        open_browser: bool = True,
+        open_browser: Optional[bool] = None,
         show_connection_info: bool = True,
         disable_logging: bool = False,
-        backend: str = "aiohttp",
+        backend: str = None,
         exec_mode: str = "main",
         timeout: int = None,
         host: str = None,
         **kwargs,
     ):
         """
         Start the server by listening to the provided port or using the
@@ -447,41 +526,65 @@
         :param thread: If the server run in a thread which means
                        we should disable interuption listeners
         :param open_browser: Should we open the system browser with app url.
                              Using the `--server` command line argument is
                              similar to setting it to False.
         :param show_connection_info: Should we print connection URL at startup?
         :param disable_logging: Ask wslink to disable logging
+        :param backend: aiohttp by default but could be generic or tornado.
+                        This can also be set with the environment variable ``TRAME_BACKEND``.
+                        Defaults to ``'aiohttp'``.
         :param exec_mode: main/desktop/task/coroutine
                           specify how the start function should work
         :param timeout: How much second should we wait before automatically
                         stopping the server when no client is connected.
                         Setting it to 0 will disable such auto-shutdown.
         :param host: The hostname used to bind the server. This can also be
                      set with the environment variable ``TRAME_DEFAULT_HOST``.
                      Defaults to ``'localhost'``.
         :param **kwargs: Keyword arguments for capturing optional parameters
                          for wslink server and/or desktop browser
         """
+        if self.root_server != self:
+            self.root_server.start(
+                port=port,
+                thread=thread,
+                open_browser=open_browser,
+                show_connection_info=show_connection_info,
+                disable_logging=disable_logging,
+                backend=backend,
+                exec_mode=exec_mode,
+                timeout=timeout,
+                host=host,
+                **kwargs,
+            )
+            return
+
         if self._running_stage:
             return
 
         # Try to bind client if none were added
         if self._www is None:
             from trame_client import module
 
             self.enable_module(module)
 
+        if open_browser is None:
+            open_browser = not os.environ.get("TRAME_SERVER", False)
+
         # Trigger on_server_start life cycle callback
         if self.controller.on_server_start.exists():
             self.controller.on_server_start(self)
 
         CoreServer.bind_server(self)
         options = self.cli.parse_known_args()[0]
 
+        if backend is None:
+            backend = os.environ.get("TRAME_BACKEND", "aiohttp")
+
         if options.host == "localhost":
             if host is None:
                 host = os.environ.get("TRAME_DEFAULT_HOST", "localhost")
             options.host = host
 
         if timeout is not None:
             options.timeout = timeout
@@ -539,14 +642,15 @@
             options.fsEndpoints = "|".join(endpoints)
 
         # Reset http delivery
         if options.no_http:
             options.content = ""
             options.fsEndpoints = ""
 
+        self._server_options = options
         CoreServer.configure(options)
 
         self._running_stage = 1
         task = CoreServer.server_start(
             options,
             **{  # Do a proper merging/override
                 **kwargs,
@@ -585,15 +689,25 @@
 
             task.add_done_callback(on_done)
 
         return task
 
     async def stop(self):
         """Coroutine for stopping the server"""
-        if self._running_stage:
+        if self.root_server != self:
+            await self.root_server.stop()
+        elif self._running_stage:
             await self._server.stop()
             self._running_future = None
 
     @property
     def port(self):
         """Once started, you can retrieve the port used"""
+        if self.root_server != self:
+            return self.root_server.port
+
         return self._running_port
+
+    @property
+    def server_options(self):
+        """Once started, you can retrieve the server options used"""
+        return self._server_options
```

### Comparing `trame-server-2.9.1/trame_server/protocol.py` & `trame-server-3.0.0/trame_server/protocol.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,15 +86,16 @@
             self.server.controller.on_server_bind(_server)
             server_routes.extend(wslink_routes)
 
     def port_callback(self, port_used):
         self.server._running_port = port_used
         if self.server._running_stage < 2:
             self.server._running_stage = 2
-            self.server.state.server_ready()
+            self.server.state.ready()
+            self.server.context.ready()
             if self.server.controller.on_server_ready.exists():
                 self.server.controller.on_server_ready(**self.server.state.to_dict())
 
             # Mark the server as ready
             if not self.server.ready.done():
                 self.server.ready.set_result(True)
 
@@ -150,14 +151,26 @@
         logger.action_s2c(actions)
         self.publish("trame.actions.topic", actions)
 
     # ---------------------------------------------------------------
     # RPCs
     # ---------------------------------------------------------------
 
+    @exportRpc("trame.force.push")
+    def force_push_state(self, *keys):
+        state_to_send = {key: self.server.state[key] for key in keys}
+        if state_to_send:
+            self.publish(
+                "trame.state.topic",
+                state_to_send,
+                skip_last_active_client=False,
+            )
+
+    # ---------------------------------------------------------------
+
     @exportRpc("trame.lifecycle.update")
     def life_cycle_update(self, name):
         _fn = self.server.controller[f"on_{name}"]
         if _fn.exists():
             _fn()
 
     # ---------------------------------------------------------------
@@ -178,16 +191,17 @@
 
     # ---------------------------------------------------------------
 
     @exportRpc("trame.trigger")
     async def trigger(self, name, args, kwargs):
         logger.action_c2s({"name": name, "args": args, "kwargs": kwargs})
         with self.server.state:
-            if name in self.server._triggers:
-                result = self.server._triggers[name](*args, **kwargs)
+            fn = self.server.controller.trigger_fn(name)
+            if fn:
+                result = fn(*args, **kwargs)
                 if inspect.isawaitable(result):
                     result = await result
                 return result
             else:
                 print(f"Trigger {name} seems to be missing")
 
     # ---------------------------------------------------------------
```

### Comparing `trame-server-2.9.1/trame_server/ui.py` & `trame-server-3.0.0/trame_server/ui.py`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.1/trame_server/utils/__init__.py` & `trame-server-3.0.0/trame_server/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 import json
 import sys
 
 from . import logger
 
 
+def share(obj, attr_name, default_value):
+    if obj and hasattr(obj, attr_name):
+        return getattr(obj, attr_name)
+
+    return default_value
+
+
 def _isascii_36(s):
     # For Python < 3.7, we have to use our own isascii() function.
     # This works for both bytes and strings.
     try:
         if isinstance(s, str):
             s.encode("ascii")
         else:
```

### Comparing `trame-server-2.9.1/trame_server/utils/asynchronous.py` & `trame-server-3.0.0/trame_server/utils/asynchronous.py`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.1/trame_server/utils/hot_reload.py` & `trame-server-3.0.0/trame_server/utils/hot_reload.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     # Skip any methods whose classes inherit from these
     SKIP_CLASSES = [AbstractElement, AbstractLayout]
 except ImportError:
     SKIP_CLASSES = []
 
 
 # Strip any decorators with these names
-STRIP_DECORATORS = ["ctrl", "state"]
+STRIP_DECORATORS = ["ctrl", "state", "life_cycle"]
 
 
 # We don't actually have logic right now to reload lambdas anyways
 SKIP_LAMBDA_FUNCS = True
 
 # If this is True, then skip any functions that are located under any
 # site packages directories.
@@ -220,18 +220,25 @@
     print(f"Edit '{func.__qualname__}' in '{fpath}' and press return to continue")
     sys.stdin.readline()
 
 
 def _get_decorator_name(dec_node):
     if hasattr(dec_node, "id"):
         return dec_node.id
-    elif hasattr(dec_node.func, "id"):
-        return dec_node.func.id
 
-    return dec_node.func.value.id
+    if hasattr(dec_node, "func"):
+        if hasattr(dec_node.func, "id"):
+            return dec_node.func.id
+        elif hasattr(dec_node.func, "value"):
+            return dec_node.func.value.id
+
+    if hasattr(dec_node, "value"):
+        return dec_node.value.id
+
+    raise Exception(f"Failed to find decorator name: {dec_node}")
 
 
 def _strip_hot_reload_decorator(func):
     """Remove the 'hot_reload' decorator and all decorators before it"""
     decorator_names = [_get_decorator_name(dec) for dec in func.decorator_list]
     hot_reload_idx = decorator_names.index("hot_reload")
     func.decorator_list = func.decorator_list[hot_reload_idx + 1 :]
```

### Comparing `trame-server-2.9.1/trame_server/utils/logger.py` & `trame-server-3.0.0/trame_server/utils/logger.py`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.1/trame_server/utils/server.py` & `trame-server-3.0.0/trame_server/utils/server.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+import sys
 import socket
 
 
 def print_informations(server):
-    args = server.cli.parse_known_args()[0]
-    local_url = f"http://{args.host}:{args.port}/"
+    options = server.server_options
+    local_url = f"http://{options.host}:{server.port}/"
     print()
     print("App running at:")
     print(f" - Local:   {local_url}")
 
     try:
-        host_name = socket.gethostname()
-        host_ip = socket.gethostbyname(host_name)
+        try:
+            host_ip = socket.gethostbyname(options.host)
+        except Exception:
+            host_name = socket.gethostname()
+            host_ip = socket.gethostbyname(host_name)
         print(f" - Network: http://{host_ip}:{server.port}/")
     except socket.gaierror:
+        print(f" - Network: http://{options.host}:{server.port}/")
         pass
 
     print()
     print(
         "Note that for multi-users you need to use and configure a launcher.",
         flush=True,
     )
+    sys.stdout.flush()
```

### Comparing `trame-server-2.9.1/trame_server/utils/version.py` & `trame-server-3.0.0/trame_server/utils/version.py`

 * *Files identical despite different names*

### Comparing `trame-server-2.9.1/trame_server.egg-info/PKG-INFO` & `trame-server-3.0.0/trame_server.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-server
-Version: 2.9.1
+Version: 3.0.0
 Summary: Internal server side implementation of trame
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
@@ -51,14 +51,15 @@
 
 **Environments variables**
 
 * **TRAME_LOG_NETWORK**     : Path to log file for capturing network exchange. (default: None)
 * **TRAME_WS_MAX_MSG_SIZE** : Maximum size in bytes of any ws message. (default: 10MB)
 * **TRAME_WS_HEART_BEAT**   : Time in second before assuming the server is non-responsive. (default: 30s)
 * **TRAME_DESKTOP_DEBUG**   : If defined it will allow user to inspect the web content in desktop mode
+* **TRAME_SERVER**          : If set to true, this will prevent browser from opening by default
 
 
 **Life cycle callbacks**
 
 Life cycle events are directly managed on the application controller
 and are prefixed with `on_*`.
```

### Comparing `trame-server-2.9.1/trame_server.egg-info/SOURCES.txt` & `trame-server-3.0.0/trame_server.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 trame_server/LICENSE
 trame_server/__init__.py
+trame_server/client.py
 trame_server/controller.py
 trame_server/core.py
 trame_server/protocol.py
 trame_server/state.py
 trame_server/ui.py
 trame_server.egg-info/PKG-INFO
 trame_server.egg-info/SOURCES.txt
 trame_server.egg-info/dependency_links.txt
 trame_server.egg-info/requires.txt
 trame_server.egg-info/top_level.txt
 trame_server/utils/__init__.py
+trame_server/utils/argument_parser.py
 trame_server/utils/asynchronous.py
 trame_server/utils/browser.py
 trame_server/utils/desktop.py
 trame_server/utils/hot_reload.py
 trame_server/utils/logger.py
+trame_server/utils/namespace.py
 trame_server/utils/server.py
 trame_server/utils/version.py
```

