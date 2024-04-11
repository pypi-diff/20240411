# Comparing `tmp/smarter_client-0.1.7.tar.gz` & `tmp/smarter_client-0.1.9.tar.gz`

## Comparing `smarter_client-0.1.7.tar` & `smarter_client-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,33 @@
--rw-r--r--   0        0        0    22281 2020-02-02 00:00:00.000000 smarter_client-0.1.7/.pylintrc
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 smarter_client-0.1.7/conftest.py
--rw-r--r--   0        0        0    52843 2020-02-02 00:00:00.000000 smarter_client-0.1.7/pdm.lock
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 smarter_client-0.1.7/requirements.txt
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 smarter_client-0.1.7/setup.cfg
--rw-r--r--   0        0        0     8685 2020-02-02 00:00:00.000000 smarter_client-0.1.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 smarter_client-0.1.7/.vscode/launch.json
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 smarter_client-0.1.7/.vscode/settings.json
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 smarter_client-0.1.7/smarter_client/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 smarter_client-0.1.7/smarter_client/_consts.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 smarter_client-0.1.7/smarter_client/dict_util.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 smarter_client-0.1.7/smarter_client/version.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 smarter_client-0.1.7/smarter_client/domain/__init__.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 smarter_client-0.1.7/smarter_client/domain/identity_toolkit_client.py
--rw-r--r--   0        0        0    11533 2020-02-02 00:00:00.000000 smarter_client-0.1.7/smarter_client/domain/models.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 smarter_client-0.1.7/smarter_client/domain/smarter_client.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 smarter_client-0.1.7/smarter_client/domain/decorators/session.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 smarter_client-0.1.7/smarter_client/managed_devices/__init__.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 smarter_client-0.1.7/smarter_client/managed_devices/base.py
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 smarter_client-0.1.7/smarter_client/managed_devices/kettle_v3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smarter_client-0.1.7/src/smarter_kettle_client/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smarter_client-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 smarter_client-0.1.7/tests/dict_util_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smarter_client-0.1.7/tests/domain/__init__.py
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 smarter_client-0.1.7/tests/domain/models_test.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 smarter_client-0.1.7/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 smarter_client-0.1.7/LICENSE
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 smarter_client-0.1.7/README.md
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 smarter_client-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 smarter_client-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    22281 2020-02-02 00:00:00.000000 smarter_client-0.1.9/.pylintrc
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 smarter_client-0.1.9/conftest.py
+-rw-r--r--   0        0        0    55699 2020-02-02 00:00:00.000000 smarter_client-0.1.9/pdm.lock
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 smarter_client-0.1.9/requirements.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 smarter_client-0.1.9/setup.cfg
+-rw-r--r--   0        0        0     8685 2020-02-02 00:00:00.000000 smarter_client-0.1.9/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 smarter_client-0.1.9/.github/workflows/upload-previews.yml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 smarter_client-0.1.9/.vscode/launch.json
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 smarter_client-0.1.9/.vscode/settings.json
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/_consts.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/dict_util.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/version.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/domain/__init__.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/domain/identity_toolkit_client.py
+-rw-r--r--   0        0        0    11690 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/domain/models.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/domain/smarter_client.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/domain/decorators/session.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/managed_devices/__init__.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/managed_devices/base.py
+-rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 smarter_client-0.1.9/smarter_client/managed_devices/kettle_v3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smarter_client-0.1.9/src/smarter_kettle_client/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smarter_client-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 smarter_client-0.1.9/tests/dict_util_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smarter_client-0.1.9/tests/domain/__init__.py
+-rw-r--r--   0        0        0    10825 2020-02-02 00:00:00.000000 smarter_client-0.1.9/tests/domain/models_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smarter_client-0.1.9/tests/domain/decoorators/__init__.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 smarter_client-0.1.9/tests/domain/decoorators/session_test.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 smarter_client-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 smarter_client-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 smarter_client-0.1.9/README.md
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 smarter_client-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 smarter_client-0.1.9/PKG-INFO
```

### Comparing `smarter_client-0.1.7/.pylintrc` & `smarter_client-0.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.7/conftest.py` & `smarter_client-0.1.9/conftest.py`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.7/pdm.lock` & `smarter_client-0.1.9/pdm.lock`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is @generated by PDM.
 # It is not intended for manual editing.
 
 [metadata]
 groups = ["default", "testing", "build"]
 strategy = ["cross_platform", "inherit_metadata"]
 lock_version = "4.4.1"
-content_hash = "sha256:a2914acd0993ef8bbdbd4532d5bf0fa1fb8f71f59a38800c84a4d5a5b4b21dd9"
+content_hash = "sha256:783180abd8b5c4b2ca727fc9d895f4bff07d9fcf8f63eac865b010b229b29bef"
 
 [[package]]
 name = "aiohttp"
 version = "3.9.3"
 requires_python = ">=3.8"
 summary = "Async http client/server framework (asyncio)"
 groups = ["default"]
@@ -707,14 +707,28 @@
 ]
 files = [
     {file = "pytest-mock-3.14.0.tar.gz", hash = "sha256:2719255a1efeceadbc056d6bf3df3d1c5015530fb40cf347c0f9afac88410bd0"},
     {file = "pytest_mock-3.14.0-py3-none-any.whl", hash = "sha256:0b72c38033392a5f4621342fe11e9219ac11ec9d375f8e2a0c164539e0d70f6f"},
 ]
 
 [[package]]
+name = "python-dateutil"
+version = "2.9.0.post0"
+requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,>=2.7"
+summary = "Extensions to the standard Python datetime module"
+groups = ["testing"]
+dependencies = [
+    "six>=1.5",
+]
+files = [
+    {file = "python-dateutil-2.9.0.post0.tar.gz", hash = "sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3"},
+    {file = "python_dateutil-2.9.0.post0-py2.py3-none-any.whl", hash = "sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427"},
+]
+
+[[package]]
 name = "python-jwt"
 version = "4.1.0"
 requires_python = ">=3.6"
 summary = "Module for generating and verifying JSON Web Tokens"
 groups = ["default"]
 dependencies = [
     "jwcrypto>=1.4.2",
@@ -781,21 +795,46 @@
 ]
 
 [[package]]
 name = "six"
 version = "1.16.0"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"
 summary = "Python 2 and 3 compatibility utilities"
-groups = ["default"]
+groups = ["default", "testing"]
 files = [
     {file = "six-1.16.0-py2.py3-none-any.whl", hash = "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"},
     {file = "six-1.16.0.tar.gz", hash = "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926"},
 ]
 
 [[package]]
+name = "time-machine"
+version = "2.14.1"
+requires_python = ">=3.8"
+summary = "Travel through time in your tests."
+groups = ["testing"]
+dependencies = [
+    "python-dateutil",
+]
+files = [
+    {file = "time-machine-2.14.1.tar.gz", hash = "sha256:57dc7efc1dde4331902d1bdefd34e8ee890a5c28533157e3b14a429c86b39533"},
+    {file = "time_machine-2.14.1-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:30a4a18357fa6cf089eeefcb37e9549b42523aebb5933894770a8919e6c398e1"},
+    {file = "time_machine-2.14.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:d45bd60bea85869615b117667f10a821e3b0d3603c47bfd105b45d1f67156fc8"},
+    {file = "time_machine-2.14.1-cp312-cp312-macosx_14_0_arm64.whl", hash = "sha256:39de6d37a14ff8882d4f1cbd50c53268b54e1cf4ef9be2bfe590d10a51ccd314"},
+    {file = "time_machine-2.14.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7fd7d188b4f9d358c6bd477daf93b460d9b244a4c296ddd065945f2b6193c2bd"},
+    {file = "time_machine-2.14.1-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:99e6f013e67c4f74a9d8f57e34173b2047f2ad48f764e44c38f3ee5344a38c01"},
+    {file = "time_machine-2.14.1-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a927d87501da8b053a27e80f5d0e1e58fbde4b50d70df2d3853ed67e89a731cf"},
+    {file = "time_machine-2.14.1-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:c77a616561dd4c7c442e9eee8cbb915750496e9a5a7fca6bcb11a9860226d2d0"},
+    {file = "time_machine-2.14.1-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:e7fa70a6bdca40cc4a8386fd85bc1bae0a23ab11e49604ef853ab3ce92be127f"},
+    {file = "time_machine-2.14.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:d63ef00d389fa6d2c76c863af580b3e4a8f0ccc6a9aea8e64590588e37f13c00"},
+    {file = "time_machine-2.14.1-cp312-cp312-win32.whl", hash = "sha256:6706eb06487354a5e219cacea709fb3ec44dec3842c6218237d5069fa5f1ad64"},
+    {file = "time_machine-2.14.1-cp312-cp312-win_amd64.whl", hash = "sha256:36aa4f17adcd73a6064bf4991a29126cac93521f0690805edb91db837c4e1453"},
+    {file = "time_machine-2.14.1-cp312-cp312-win_arm64.whl", hash = "sha256:edea570f3835a036e8860bb8d6eb8d08473c59313db86e36e3b207f796fd7b14"},
+]
+
+[[package]]
 name = "tomlkit"
 version = "0.12.4"
 requires_python = ">=3.7"
 summary = "Style preserving TOML library"
 groups = ["default"]
 files = [
     {file = "tomlkit-0.12.4-py3-none-any.whl", hash = "sha256:5cd82d48a3dd89dee1f9d64420aa20ae65cfbd00668d6f094d7578a78efbb77b"},
```

### Comparing `smarter_client-0.1.7/.github/workflows/ci.yml` & `smarter_client-0.1.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.7/smarter_client/dict_util.py` & `smarter_client-0.1.9/smarter_client/dict_util.py`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.7/smarter_client/version.py` & `smarter_client-0.1.9/smarter_client/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 """The `version` module holds the version information for Smarter Kettle Client."""
 from __future__ import annotations as _annotations
 
 __all__ = 'VERSION', 'version_info'
 
-VERSION = '0.1.7'
+VERSION = '0.1.9'
 """The version of Smarter Kettle Client."""
 
 
 def version_short() -> str:
     """Return the `major.minor` part of version.
 
     It returns '2.1' if version is '2.1.1'.
```

### Comparing `smarter_client-0.1.7/smarter_client/domain/identity_toolkit_client.py` & `smarter_client-0.1.9/smarter_client/domain/identity_toolkit_client.py`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.7/smarter_client/domain/models.py` & `smarter_client-0.1.9/smarter_client/domain/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from abc import ABCMeta
 from abc import abstractmethod
-from typing import Any, Self
+from typing import Any, Callable, Self
 from pprint import pprint
 
 import datetime
 from smarter_client.dict_util import delete_dict, patch_dict, put_dict
 from . import smarter_client
 
 
@@ -122,15 +122,15 @@
         super().clear()
         super().update({
             key: Command.from_data(self.client, value, key, self.device)
             for key, value
             in self._data.items()
         })
 
-    def _fetch(self) -> dict:
+    def _fetch(self) -> dict:  # pragma: no cover
         raise NotImplementedError()
 
 
 # </Commands>
 
 
 class CommandInstance(BaseEntity):
@@ -147,15 +147,15 @@
 
     def _init_data(self) -> None:
         self.user_id = self._data.get('user_id')
         self.value = self._data.get('value')
         self.state = self._data.get('state')
         self.response = self._data.get('response')
 
-    def _fetch(self) -> dict:
+    def _fetch(self) -> dict:  # pragma: no cover
         raise NotImplementedError()
 
     @classmethod
     def from_data(cls,
                   client: smarter_client.SmarterClient,
                   data: dict,
                   identifier: str,
@@ -185,62 +185,66 @@
                   client: smarter_client.SmarterClient,
                   data: dict,
                   name: str,
                   device: Device) -> Self:
         self = Command(client)
         self._data = data
         self.identifier = name
-        self.name = name
         self.device = device
+        self._init_data()
 
         return self
 
     def __init__(self, client: smarter_client.SmarterClient):
         super().__init__(client)
 
     def execute(self, user_id: str, value: any):
         return self.client.send_command(self.device.identifier, self.name, {"user_id": user_id, "value": value})
 
     def _init_data(self) -> None:
-        self.identifier = self._data.get('name')
         self.name = self.identifier
         self.example = self._data.get('example')
         self.instances = {
             key: CommandInstance.from_data(
                 self.client, value, key, self, self.device)
             for key, value
             in self._data.items()
             if key != 'example'
         }
 
-    def _fetch(self) -> dict:
+    def _fetch(self) -> dict:  # pragma: no cover
         raise NotImplementedError()
-
-    def create_child(self, path: list[str], data: dict):
-        child = CommandInstance.from_data(
-            self.client, data, path[0], self, self.device)
-        self.instances.append(child)
-        return child
 # </Command>
 
 
 class Device(BaseEntity):
     commands: Commands = None
     settings: Settings = None
     status: Status = None
+    _stream_close: Callable = None
 
     def __init__(self, client: smarter_client.SmarterClient):
         super().__init__(client)
 
     # Public methods
-    def watch(self, callback):
+    def watch(self, callback=lambda: None):
+        if self._stream_close is not None:
+            raise RuntimeError(
+                'Already watching device. Call unwatch() first. Support for multiple callbacks may be implemented in a later version')
+
         def on_data(event):
             self._on_event(event)
             callback(event)
-        self.client.watch_device_attribute(self.identifier, on_data)
+        self._stream_close = self.client.watch_device_attribute(
+            self.identifier, on_data)
+
+    def unwatch(self):
+        if self._stream_close is not None:
+            self._stream_close()
+            self._stream_close = None
 
     # Private methods
     def _init_data(self):
         self.commands = Commands.from_data(
             self.client, self._data.get('commands'), self)
 
         self.settings = Settings.from_data(
@@ -273,36 +277,37 @@
         self.email = data.get('email')
         self.display_name = data.get('displayName')
         self.id_token = data.get('idToken')
         self.registered = data.get('registered')
         self.refresh_token = data.get('refreshToken')
         self.session_duration = data.get('expiresIn')
 
-        self.expires_at = datetime.datetime.now() + datetime.timedelta(0,
-                                                                       int(self.session_duration))
+        self.expires_at = self._get_expiration_datetime(data)
+
+    def _get_expiration_datetime(self, data: dict):
+        return datetime.datetime.now() + datetime.timedelta(0, int(data.get('expiresIn')))
 
     def is_expired(self) -> bool:
         """
         Returns True if the session has expired.
         """
-        return self.expires_at > datetime.datetime.now()
+        return self.expires_at <= datetime.datetime.now()
 
     @property
     def expires_in(self) -> int:
         """
         Returns the number of seconds until the session expires.
         """
         return (self.expires_at - datetime.datetime.now()).total_seconds()
 
     def update(self, data: dict):
         self.id_token = data.get('idToken')
         self.refresh_token = data.get('refreshToken')
         self.local_id = data.get('userId')
-        self.expires_at = datetime.datetime.now() + datetime.timedelta(0,
-                                                                       int(data.get('expires_in')))
+        self.expires_at = self._get_expiration_datetime(data)
 
 
 # </LoginSession>
 
 class Network(BaseEntity):
     access_tokens_fcm: dict[str, str] = None
     associated_devices: list[Device] = None
```

### Comparing `smarter_client-0.1.7/smarter_client/domain/smarter_client.py` & `smarter_client-0.1.9/smarter_client/domain/smarter_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Module contains implementation of Smarter Firebase API
 """
 from __future__ import annotations
+from typing import Callable
 from pyrebase.pyrebase import Stream
 import pyrebase
 
 from smarter_client.domain.decorators.session import refreshsession
 from .models import LoginSession
 from .._consts import API_KEY
 
 
-class SmarterClient:
+class SmarterClient:  # pragma: no cover
     """
     A client for interacting with the Smarter API.
     """
     session: LoginSession
 
     def __init__(self):
         config = {
@@ -75,10 +76,12 @@
             .child('devices') \
             .child(device_id) \
             .child('commands') \
             .child(command) \
             .push(data, self.token)
 
     @refreshsession
-    def watch_device_attribute(self, device_id: str, callback) -> Stream:
+    def watch_device_attribute(self, device_id: str, callback) -> Callable:
         database = self.app.database()
-        return database.child('devices').child(device_id).stream(callback, self.token)
+        stream = database.child('devices').child(
+            device_id).stream(callback, self.token)
+        return lambda: stream.close()
```

### Comparing `smarter_client-0.1.7/smarter_client/managed_devices/__init__.py` & `smarter_client-0.1.9/smarter_client/managed_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.7/smarter_client/managed_devices/base.py` & `smarter_client-0.1.9/smarter_client/managed_devices/base.py`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.7/smarter_client/managed_devices/kettle_v3.py` & `smarter_client-0.1.9/smarter_client/managed_devices/kettle_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import Any, Dict
+from typing import Any, Callable, Dict
 
 from smarter_client.domain import Device, SmarterClient
 from smarter_client.managed_devices.base import BaseDevice
 
 
 class SmarterKettleV3(BaseDevice):
     device: Device = None
@@ -38,18 +38,21 @@
     def status(self):
         return self.device.status
 
     @property
     def settings(self):
         return self.device.settings
 
-    def watch_status(self, handler: Any):
+    def watch_status(self, handler: Callable):
         self._status_handler = handler
         self.device.watch(self._on_event)
 
+    def dispose(self):
+        self.device.unwatch()
+
     def add_alarm(self, value: int):
         self._send_command('add_alarm', value)
 
     def calibrate_weight_sensor(self, value: int):
         self._send_command('calibrate_weight_sensor', value)
 
     def change_alarm(self, value: int):
```

### Comparing `smarter_client-0.1.7/tests/dict_util_test.py` & `smarter_client-0.1.9/tests/dict_util_test.py`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.7/.gitignore` & `smarter_client-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.7/LICENSE` & `smarter_client-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.7/README.md` & `smarter_client-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `smarter_client-0.1.7/pyproject.toml` & `smarter_client-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 [tool.pdm.dev-dependencies]
 testing = [
     "pytest>=6.2.0",
     "pytest-cov>=2.4.0",
     "pytest-localserver>=0.4.1",
     "pytest-asyncio>=0.16.0",
     "pytest-mock>=3.6.1",
+    "time-machine>=2.14.1",
 ]
 
 
 build = ["build"]
 
 [project.urls]
 Homepage = "https://www.github.com/kbirger/smarter-kettle-client"
```

### Comparing `smarter_client-0.1.7/PKG-INFO` & `smarter_client-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: smarter-client
-Version: 0.1.7
+Version: 0.1.9
 Summary: Smarter Kettle client library
 Project-URL: Homepage, https://www.github.com/kbirger/smarter-kettle-client
 Project-URL: Release Notes, https://www.github.com/kbirger/smarter-kettle-client
 Project-URL: Source, https://www.github.com/kbirger/smarter-kettle-client
 Author: @kbirger
 Author-email: Kirill Birger <kbirger@gmail.com>
 License: MIT
```

