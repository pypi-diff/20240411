# Comparing `tmp/dirigera-1.1.0.tar.gz` & `tmp/dirigera-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirigera-1.1.0.tar", last modified: Fri Apr  5 16:38:49 2024, max compression
+gzip compressed data, was "dirigera-1.1.1.tar", last modified: Thu Apr 11 12:45:37 2024, max compression
```

## Comparing `dirigera-1.1.0.tar` & `dirigera-1.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:49.585303 dirigera-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-05 16:38:42.000000 dirigera-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-04-05 16:38:49.585303 dirigera-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-04-05 16:38:42.000000 dirigera-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-05 16:38:42.000000 dirigera-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:38:49.585303 dirigera-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 16:38:42.000000 dirigera-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:49.577303 dirigera-1.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:49.577303 dirigera-1.1.0/src/dirigera/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:49.581303 dirigera-1.1.0/src/dirigera/devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/air_purifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/base_ikea_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/blinds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/motion_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/open_close_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/outlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/devices/scene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:49.581303 dirigera-1.1.0/src/dirigera/hub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/hub/abstract_smart_home_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/hub/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-05 16:38:42.000000 dirigera-1.1.0/src/dirigera/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:49.585303 dirigera-1.1.0/src/dirigera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-04-05 16:38:49.000000 dirigera-1.1.0/src/dirigera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-05 16:38:49.000000 dirigera-1.1.0/src/dirigera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:38:49.000000 dirigera-1.1.0/src/dirigera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 16:38:49.000000 dirigera-1.1.0/src/dirigera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 16:38:49.000000 dirigera-1.1.0/src/dirigera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 16:38:49.000000 dirigera-1.1.0/src/dirigera.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:38:49.585303 dirigera-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_air_purifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_blinds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_motion_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_open_close_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_outlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_scenes.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-05 16:38:42.000000 dirigera-1.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:37.453992 dirigera-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-11 12:45:33.000000 dirigera-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-04-11 12:45:37.453992 dirigera-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-04-11 12:45:33.000000 dirigera-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-11 12:45:33.000000 dirigera-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:45:37.453992 dirigera-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-11 12:45:33.000000 dirigera-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:37.445992 dirigera-1.1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:37.449992 dirigera-1.1.1/src/dirigera/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:37.449992 dirigera-1.1.1/src/dirigera/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/air_purifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/base_ikea_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/blinds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/motion_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/outlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/scene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:37.453992 dirigera-1.1.1/src/dirigera/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/hub/abstract_smart_home_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14937 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/hub/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:37.453992 dirigera-1.1.1/src/dirigera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-04-11 12:45:37.000000 dirigera-1.1.1/src/dirigera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-11 12:45:37.000000 dirigera-1.1.1/src/dirigera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:45:37.000000 dirigera-1.1.1/src/dirigera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-11 12:45:37.000000 dirigera-1.1.1/src/dirigera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-11 12:45:37.000000 dirigera-1.1.1/src/dirigera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 12:45:37.000000 dirigera-1.1.1/src/dirigera.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:37.453992 dirigera-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_air_purifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_blinds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_motion_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_outlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_scenes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_utils.py
```

### Comparing `dirigera-1.1.0/LICENSE` & `dirigera-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/PKG-INFO` & `dirigera-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 1.1.0
+Version: 1.1.1
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dirigera-1.1.0/README.md` & `dirigera-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/pyproject.toml` & `dirigera-1.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dirigera"
-version = "1.1.0"
+version = "1.1.1"
 description = "An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub"
 readme = "README.md"
 authors = [{ name = "Leggin", email = "legginsun@gmail.com" }]
 license = { file = "LICENSE" }
 keywords = [
     "python",
     "iot",
```

### Comparing `dirigera-1.1.0/src/dirigera/devices/air_purifier.py` & `dirigera-1.1.1/src/dirigera/devices/air_purifier.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/src/dirigera/devices/blinds.py` & `dirigera-1.1.1/src/dirigera/devices/blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/src/dirigera/devices/controller.py` & `dirigera-1.1.1/src/dirigera/devices/controller.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/src/dirigera/devices/device.py` & `dirigera-1.1.1/src/dirigera/devices/device.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/src/dirigera/devices/environment_sensor.py` & `dirigera-1.1.1/src/dirigera/devices/environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/src/dirigera/devices/light.py` & `dirigera-1.1.1/src/dirigera/devices/light.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/src/dirigera/devices/motion_sensor.py` & `dirigera-1.1.1/src/dirigera/devices/motion_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/src/dirigera/devices/open_close_sensor.py` & `dirigera-1.1.1/src/dirigera/devices/open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/src/dirigera/devices/outlet.py` & `dirigera-1.1.1/src/dirigera/devices/outlet.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/src/dirigera/devices/scene.py` & `dirigera-1.1.1/src/dirigera/devices/scene.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/src/dirigera/hub/abstract_smart_home_hub.py` & `dirigera-1.1.1/src/dirigera/hub/abstract_smart_home_hub.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/src/dirigera/hub/auth.py` & `dirigera-1.1.1/src/dirigera/hub/auth.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/src/dirigera/hub/hub.py` & `dirigera-1.1.1/src/dirigera/hub/hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
             ip_address (str): The IP address of the hub.
             port (str, optional): The port number for the hub API. Defaults to "8443".
             api_version (str, optional): The version of the API to use. Defaults to "v1".
         """
         self.api_base_url = f"https://{ip_address}:{port}/{api_version}"
         self.websocket_base_url = f"wss://{ip_address}:{port}/{api_version}"
         self.token = token
+        self.wsapp : Any = None
 
     def headers(self) -> Dict[str, Any]:
         return {"Authorization": f"Bearer {self.token}"}
 
     def create_event_listener(
         self,
         on_open: Any = None,
@@ -69,31 +70,36 @@
             on_close (Any, optional)
             on_ping (Any, optional)
             on_pong (Any, optional)
             on_data (Any, optional)
             on_cont_message (Any, optional)
             ping_intervall (int, optional): Ping interval in Seconds. Defaults to 60.
         """
-        wsapp = websocket.WebSocketApp(
+        self.wsapp = websocket.WebSocketApp(
             self.websocket_base_url,
             header={"Authorization": f"Bearer {self.token}"},
             on_open=on_open,
             on_message=on_message,
             on_error=on_error,
             on_close=on_close,
             on_ping=on_ping,
             on_pong=on_pong,
             on_data=on_data,
             on_cont_message=on_cont_message,
         )
 
-        wsapp.run_forever(
+        self.wsapp.run_forever(
             sslopt={"cert_reqs": ssl.CERT_NONE}, ping_interval=ping_intervall
         )
 
+    def stop_event_listener(self) -> None:
+        if self.wsapp is not None:
+            self.wsapp.close()
+            self.wsapp = None
+
     def patch(self, route: str, data: List[Dict[str, Any]]) -> Any:
         response = requests.patch(
             f"{self.api_base_url}{route}",
             headers=self.headers(),
             json=data,
             timeout=10,
             verify=False,
```

### Comparing `dirigera-1.1.0/src/dirigera.egg-info/PKG-INFO` & `dirigera-1.1.1/src/dirigera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 1.1.0
+Version: 1.1.1
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dirigera-1.1.0/src/dirigera.egg-info/SOURCES.txt` & `dirigera-1.1.1/src/dirigera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/tests/test_air_purifier.py` & `dirigera-1.1.1/tests/test_air_purifier.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/tests/test_blinds.py` & `dirigera-1.1.1/tests/test_blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/tests/test_controller.py` & `dirigera-1.1.1/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/tests/test_environment_sensor.py` & `dirigera-1.1.1/tests/test_environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/tests/test_light.py` & `dirigera-1.1.1/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/tests/test_motion_sensor.py` & `dirigera-1.1.1/tests/test_motion_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/tests/test_open_close_sensor.py` & `dirigera-1.1.1/tests/test_open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/tests/test_outlet.py` & `dirigera-1.1.1/tests/test_outlet.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/tests/test_scenes.py` & `dirigera-1.1.1/tests/test_scenes.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.0/tests/test_utils.py` & `dirigera-1.1.1/tests/test_utils.py`

 * *Files identical despite different names*

