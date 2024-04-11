# Comparing `tmp/seam-0.2.0.tar.gz` & `tmp/seam-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seam-0.2.0.tar", max compression
+gzip compressed data, was "seam-0.3.0.tar", max compression
```

## Comparing `seam-0.2.0.tar` & `seam-0.3.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1087 2024-04-09 09:17:40.909604 seam-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     4228 2024-04-09 09:17:40.909604 seam-0.2.0/README.rst
--rw-r--r--   0        0        0      726 2024-04-09 09:17:40.909604 seam-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       97 2024-04-09 09:17:40.909604 seam-0.2.0/seam/__init__.py
--rw-r--r--   0        0        0    11938 2024-04-09 09:17:40.909604 seam-0.2.0/seam/access_codes.py
--rw-r--r--   0        0        0      903 2024-04-09 09:17:40.909604 seam-0.2.0/seam/access_codes_simulate.py
--rw-r--r--   0        0        0     3979 2024-04-09 09:17:40.909604 seam-0.2.0/seam/access_codes_unmanaged.py
--rw-r--r--   0        0        0     1746 2024-04-09 09:17:40.909604 seam-0.2.0/seam/acs.py
--rw-r--r--   0        0        0     2505 2024-04-09 09:17:40.909604 seam-0.2.0/seam/acs_access_groups.py
--rw-r--r--   0        0        0      718 2024-04-09 09:17:40.909604 seam-0.2.0/seam/acs_credential_pools.py
--rw-r--r--   0        0        0     1782 2024-04-09 09:17:40.909604 seam-0.2.0/seam/acs_credential_provisioning_automations.py
--rw-r--r--   0        0        0     4763 2024-04-09 09:17:40.909604 seam-0.2.0/seam/acs_credentials.py
--rw-r--r--   0        0        0     2172 2024-04-09 09:17:40.909604 seam-0.2.0/seam/acs_entrances.py
--rw-r--r--   0        0        0      955 2024-04-09 09:17:40.909604 seam-0.2.0/seam/acs_systems.py
--rw-r--r--   0        0        0     6476 2024-04-09 09:17:40.909604 seam-0.2.0/seam/acs_users.py
--rw-r--r--   0        0        0     3169 2024-04-09 09:17:40.909604 seam-0.2.0/seam/action_attempts.py
--rw-r--r--   0        0        0     5751 2024-04-09 09:17:40.909604 seam-0.2.0/seam/client_sessions.py
--rw-r--r--   0        0        0     3292 2024-04-09 09:17:40.909604 seam-0.2.0/seam/connect_webviews.py
--rw-r--r--   0        0        0     2520 2024-04-09 09:17:40.909604 seam-0.2.0/seam/connected_accounts.py
--rw-r--r--   0        0        0     4761 2024-04-09 09:17:40.909604 seam-0.2.0/seam/devices.py
--rw-r--r--   0        0        0      517 2024-04-09 09:17:40.909604 seam-0.2.0/seam/devices_simulate.py
--rw-r--r--   0        0        0     3323 2024-04-09 09:17:40.909604 seam-0.2.0/seam/devices_unmanaged.py
--rw-r--r--   0        0        0     2385 2024-04-09 09:17:40.909604 seam-0.2.0/seam/events.py
--rw-r--r--   0        0        0     4181 2024-04-09 09:17:40.909604 seam-0.2.0/seam/locks.py
--rw-r--r--   0        0        0      765 2024-04-09 09:17:40.909604 seam-0.2.0/seam/networks.py
--rw-r--r--   0        0        0      714 2024-04-09 09:17:40.909604 seam-0.2.0/seam/noise_sensors.py
--rw-r--r--   0        0        0     4350 2024-04-09 09:17:40.909604 seam-0.2.0/seam/noise_sensors_noise_thresholds.py
--rw-r--r--   0        0        0      594 2024-04-09 09:17:40.909604 seam-0.2.0/seam/noise_sensors_simulate.py
--rw-r--r--   0        0        0     1063 2024-04-09 09:17:40.909604 seam-0.2.0/seam/phones.py
--rw-r--r--   0        0        0     1185 2024-04-09 09:17:40.909604 seam-0.2.0/seam/phones_simulate.py
--rw-r--r--   0        0        0     1535 2024-04-09 09:17:40.909604 seam-0.2.0/seam/routes.py
--rw-r--r--   0        0        0     3175 2024-04-09 09:17:40.909604 seam-0.2.0/seam/seam.py
--rw-r--r--   0        0        0     8926 2024-04-09 09:17:40.909604 seam-0.2.0/seam/thermostats.py
--rw-r--r--   0        0        0     6930 2024-04-09 09:17:40.909604 seam-0.2.0/seam/thermostats_climate_setting_schedules.py
--rw-r--r--   0        0        0    64144 2024-04-09 09:17:40.909604 seam-0.2.0/seam/types.py
--rw-r--r--   0        0        0     6700 2024-04-09 09:17:40.909604 seam-0.2.0/seam/user_identities.py
--rw-r--r--   0        0        0     2903 2024-04-09 09:17:40.909604 seam-0.2.0/seam/user_identities_enrollment_automations.py
--rw-r--r--   0        0        0      864 2024-04-09 09:17:40.909604 seam-0.2.0/seam/utils/deep_attr_dict.py
--rw-r--r--   0        0        0     1815 2024-04-09 09:17:40.909604 seam-0.2.0/seam/webhooks.py
--rw-r--r--   0        0        0     1845 2024-04-09 09:17:40.909604 seam-0.2.0/seam/workspaces.py
--rw-r--r--   0        0        0     4978 1970-01-01 00:00:00.000000 seam-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-04-11 09:49:56.083822 seam-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     4228 2024-04-11 09:49:56.083822 seam-0.3.0/README.rst
+-rw-r--r--   0        0        0      726 2024-04-11 09:49:56.083822 seam-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       97 2024-04-11 09:49:56.083822 seam-0.3.0/seam/__init__.py
+-rw-r--r--   0        0        0    11938 2024-04-11 09:49:56.083822 seam-0.3.0/seam/access_codes.py
+-rw-r--r--   0        0        0      903 2024-04-11 09:49:56.083822 seam-0.3.0/seam/access_codes_simulate.py
+-rw-r--r--   0        0        0     3979 2024-04-11 09:49:56.083822 seam-0.3.0/seam/access_codes_unmanaged.py
+-rw-r--r--   0        0        0     1746 2024-04-11 09:49:56.083822 seam-0.3.0/seam/acs.py
+-rw-r--r--   0        0        0     2505 2024-04-11 09:49:56.083822 seam-0.3.0/seam/acs_access_groups.py
+-rw-r--r--   0        0        0      718 2024-04-11 09:49:56.083822 seam-0.3.0/seam/acs_credential_pools.py
+-rw-r--r--   0        0        0     1782 2024-04-11 09:49:56.083822 seam-0.3.0/seam/acs_credential_provisioning_automations.py
+-rw-r--r--   0        0        0     4763 2024-04-11 09:49:56.083822 seam-0.3.0/seam/acs_credentials.py
+-rw-r--r--   0        0        0     2172 2024-04-11 09:49:56.083822 seam-0.3.0/seam/acs_entrances.py
+-rw-r--r--   0        0        0      955 2024-04-11 09:49:56.083822 seam-0.3.0/seam/acs_systems.py
+-rw-r--r--   0        0        0     6476 2024-04-11 09:49:56.083822 seam-0.3.0/seam/acs_users.py
+-rw-r--r--   0        0        0     3169 2024-04-11 09:49:56.083822 seam-0.3.0/seam/action_attempts.py
+-rw-r--r--   0        0        0     5751 2024-04-11 09:49:56.083822 seam-0.3.0/seam/client_sessions.py
+-rw-r--r--   0        0        0     3292 2024-04-11 09:49:56.083822 seam-0.3.0/seam/connect_webviews.py
+-rw-r--r--   0        0        0     2520 2024-04-11 09:49:56.083822 seam-0.3.0/seam/connected_accounts.py
+-rw-r--r--   0        0        0     4761 2024-04-11 09:49:56.083822 seam-0.3.0/seam/devices.py
+-rw-r--r--   0        0        0      517 2024-04-11 09:49:56.083822 seam-0.3.0/seam/devices_simulate.py
+-rw-r--r--   0        0        0     3323 2024-04-11 09:49:56.083822 seam-0.3.0/seam/devices_unmanaged.py
+-rw-r--r--   0        0        0     2385 2024-04-11 09:49:56.083822 seam-0.3.0/seam/events.py
+-rw-r--r--   0        0        0     4181 2024-04-11 09:49:56.083822 seam-0.3.0/seam/locks.py
+-rw-r--r--   0        0        0      765 2024-04-11 09:49:56.083822 seam-0.3.0/seam/networks.py
+-rw-r--r--   0        0        0      714 2024-04-11 09:49:56.083822 seam-0.3.0/seam/noise_sensors.py
+-rw-r--r--   0        0        0     4350 2024-04-11 09:49:56.083822 seam-0.3.0/seam/noise_sensors_noise_thresholds.py
+-rw-r--r--   0        0        0      594 2024-04-11 09:49:56.083822 seam-0.3.0/seam/noise_sensors_simulate.py
+-rw-r--r--   0        0        0     1063 2024-04-11 09:49:56.083822 seam-0.3.0/seam/phones.py
+-rw-r--r--   0        0        0     1185 2024-04-11 09:49:56.083822 seam-0.3.0/seam/phones_simulate.py
+-rw-r--r--   0        0        0     1535 2024-04-11 09:49:56.083822 seam-0.3.0/seam/routes.py
+-rw-r--r--   0        0        0     3175 2024-04-11 09:49:56.083822 seam-0.3.0/seam/seam.py
+-rw-r--r--   0        0        0     8926 2024-04-11 09:49:56.083822 seam-0.3.0/seam/thermostats.py
+-rw-r--r--   0        0        0     6930 2024-04-11 09:49:56.083822 seam-0.3.0/seam/thermostats_climate_setting_schedules.py
+-rw-r--r--   0        0        0    64645 2024-04-11 09:49:56.083822 seam-0.3.0/seam/types.py
+-rw-r--r--   0        0        0     6700 2024-04-11 09:49:56.083822 seam-0.3.0/seam/user_identities.py
+-rw-r--r--   0        0        0     2903 2024-04-11 09:49:56.083822 seam-0.3.0/seam/user_identities_enrollment_automations.py
+-rw-r--r--   0        0        0      864 2024-04-11 09:49:56.083822 seam-0.3.0/seam/utils/deep_attr_dict.py
+-rw-r--r--   0        0        0     1815 2024-04-11 09:49:56.083822 seam-0.3.0/seam/webhooks.py
+-rw-r--r--   0        0        0     1845 2024-04-11 09:49:56.083822 seam-0.3.0/seam/workspaces.py
+-rw-r--r--   0        0        0     4978 1970-01-01 00:00:00.000000 seam-0.3.0/PKG-INFO
```

### Comparing `seam-0.2.0/LICENSE.txt` & `seam-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/README.rst` & `seam-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/pyproject.toml` & `seam-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seam"
-version = "0.2.0"
+version = "0.3.0"
 description = "SDK for the Seam API written in Python."
 authors = ["Seam Labs, Inc. <engineering@getseam.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/seamapi/python-next"
 repository = "https://github.com/seamapi/python-next"
```

### Comparing `seam-0.2.0/seam/access_codes.py` & `seam-0.3.0/seam/access_codes.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/access_codes_simulate.py` & `seam-0.3.0/seam/access_codes_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/access_codes_unmanaged.py` & `seam-0.3.0/seam/access_codes_unmanaged.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/acs.py` & `seam-0.3.0/seam/acs.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/acs_access_groups.py` & `seam-0.3.0/seam/acs_access_groups.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/acs_credential_pools.py` & `seam-0.3.0/seam/acs_credential_pools.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/acs_credential_provisioning_automations.py` & `seam-0.3.0/seam/acs_credential_provisioning_automations.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/acs_credentials.py` & `seam-0.3.0/seam/acs_credentials.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/acs_entrances.py` & `seam-0.3.0/seam/acs_entrances.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/acs_systems.py` & `seam-0.3.0/seam/acs_systems.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/acs_users.py` & `seam-0.3.0/seam/acs_users.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/action_attempts.py` & `seam-0.3.0/seam/action_attempts.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/client_sessions.py` & `seam-0.3.0/seam/client_sessions.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/connect_webviews.py` & `seam-0.3.0/seam/connect_webviews.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/connected_accounts.py` & `seam-0.3.0/seam/connected_accounts.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/devices.py` & `seam-0.3.0/seam/devices.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/devices_simulate.py` & `seam-0.3.0/seam/devices_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/devices_unmanaged.py` & `seam-0.3.0/seam/devices_unmanaged.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/events.py` & `seam-0.3.0/seam/events.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/locks.py` & `seam-0.3.0/seam/locks.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/networks.py` & `seam-0.3.0/seam/networks.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/noise_sensors.py` & `seam-0.3.0/seam/noise_sensors.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/noise_sensors_noise_thresholds.py` & `seam-0.3.0/seam/noise_sensors_noise_thresholds.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/noise_sensors_simulate.py` & `seam-0.3.0/seam/noise_sensors_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/phones.py` & `seam-0.3.0/seam/phones.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/phones_simulate.py` & `seam-0.3.0/seam/phones_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/routes.py` & `seam-0.3.0/seam/routes.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/seam.py` & `seam-0.3.0/seam/seam.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/thermostats.py` & `seam-0.3.0/seam/thermostats.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/thermostats_climate_setting_schedules.py` & `seam-0.3.0/seam/thermostats_climate_setting_schedules.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/types.py` & `seam-0.3.0/seam/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,14 +273,15 @@
     errors: List[Dict[str, Any]]
     warnings: List[Dict[str, Any]]
     created_at: str
     is_managed: bool
     custom_metadata: Dict[str, Any]
     can_remotely_unlock: bool
     can_remotely_lock: bool
+    can_program_offline_access_codes: bool
     can_program_online_access_codes: bool
     can_simulate_removal: bool
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
         return Device(
             device_id=d.get("device_id", None),
@@ -295,14 +296,17 @@
             errors=d.get("errors", None),
             warnings=d.get("warnings", None),
             created_at=d.get("created_at", None),
             is_managed=d.get("is_managed", None),
             custom_metadata=DeepAttrDict(d.get("custom_metadata", None)),
             can_remotely_unlock=d.get("can_remotely_unlock", None),
             can_remotely_lock=d.get("can_remotely_lock", None),
+            can_program_offline_access_codes=d.get(
+                "can_program_offline_access_codes", None
+            ),
             can_program_online_access_codes=d.get(
                 "can_program_online_access_codes", None
             ),
             can_simulate_removal=d.get("can_simulate_removal", None),
         )
 
 
@@ -316,14 +320,15 @@
     errors: List[Dict[str, Any]]
     warnings: List[Dict[str, Any]]
     created_at: str
     is_managed: bool
     properties: Dict[str, Any]
     can_remotely_unlock: bool
     can_remotely_lock: bool
+    can_program_offline_access_codes: bool
     can_program_online_access_codes: bool
     can_simulate_removal: bool
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
         return UnmanagedDevice(
             device_id=d.get("device_id", None),
@@ -334,14 +339,17 @@
             errors=d.get("errors", None),
             warnings=d.get("warnings", None),
             created_at=d.get("created_at", None),
             is_managed=d.get("is_managed", None),
             properties=DeepAttrDict(d.get("properties", None)),
             can_remotely_unlock=d.get("can_remotely_unlock", None),
             can_remotely_lock=d.get("can_remotely_lock", None),
+            can_program_offline_access_codes=d.get(
+                "can_program_offline_access_codes", None
+            ),
             can_program_online_access_codes=d.get(
                 "can_program_online_access_codes", None
             ),
             can_simulate_removal=d.get("can_simulate_removal", None),
         )
 
 
@@ -710,14 +718,15 @@
     errors: List[Dict[str, Any]]
     warnings: List[Dict[str, Any]]
     created_at: str
     is_managed: bool
     custom_metadata: Dict[str, Any]
     can_remotely_unlock: bool
     can_remotely_lock: bool
+    can_program_offline_access_codes: bool
     can_program_online_access_codes: bool
     can_simulate_removal: bool
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
         return Phone(
             device_id=d.get("device_id", None),
@@ -731,14 +740,17 @@
             errors=d.get("errors", None),
             warnings=d.get("warnings", None),
             created_at=d.get("created_at", None),
             is_managed=d.get("is_managed", None),
             custom_metadata=DeepAttrDict(d.get("custom_metadata", None)),
             can_remotely_unlock=d.get("can_remotely_unlock", None),
             can_remotely_lock=d.get("can_remotely_lock", None),
+            can_program_offline_access_codes=d.get(
+                "can_program_offline_access_codes", None
+            ),
             can_program_online_access_codes=d.get(
                 "can_program_online_access_codes", None
             ),
             can_simulate_removal=d.get("can_simulate_removal", None),
         )
 
 
@@ -1115,70 +1127,14 @@
     @abc.abstractmethod
     def reset_sandbox(
         self,
     ) -> None:
         raise NotImplementedError()
 
 
-class AbstractAccessCodesSimulate(abc.ABC):
-
-    @abc.abstractmethod
-    def create_unmanaged_access_code(
-        self, *, device_id: str, name: str, code: str
-    ) -> UnmanagedAccessCode:
-        raise NotImplementedError()
-
-
-class AbstractAccessCodesUnmanaged(abc.ABC):
-
-    @abc.abstractmethod
-    def convert_to_managed(
-        self,
-        *,
-        access_code_id: str,
-        is_external_modification_allowed: Optional[bool] = None,
-        allow_external_modification: Optional[bool] = None,
-        force: Optional[bool] = None,
-        sync: Optional[bool] = None,
-    ) -> None:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def delete(self, *, access_code_id: str, sync: Optional[bool] = None) -> None:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def get(
-        self,
-        *,
-        device_id: Optional[str] = None,
-        access_code_id: Optional[str] = None,
-        code: Optional[str] = None,
-    ) -> UnmanagedAccessCode:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def list(
-        self, *, device_id: str, user_identifier_key: Optional[str] = None
-    ) -> List[UnmanagedAccessCode]:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def update(
-        self,
-        *,
-        access_code_id: str,
-        is_managed: bool,
-        allow_external_modification: Optional[bool] = None,
-        is_external_modification_allowed: Optional[bool] = None,
-        force: Optional[bool] = None,
-    ) -> None:
-        raise NotImplementedError()
-
-
 class AbstractAcsAccessGroups(abc.ABC):
 
     @abc.abstractmethod
     def add_user(self, *, acs_access_group_id: str, acs_user_id: str) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
@@ -1384,14 +1340,70 @@
         phone_number: Optional[str] = None,
         email_address: Optional[str] = None,
         hid_acs_system_id: Optional[str] = None,
     ) -> None:
         raise NotImplementedError()
 
 
+class AbstractAccessCodesSimulate(abc.ABC):
+
+    @abc.abstractmethod
+    def create_unmanaged_access_code(
+        self, *, device_id: str, name: str, code: str
+    ) -> UnmanagedAccessCode:
+        raise NotImplementedError()
+
+
+class AbstractAccessCodesUnmanaged(abc.ABC):
+
+    @abc.abstractmethod
+    def convert_to_managed(
+        self,
+        *,
+        access_code_id: str,
+        is_external_modification_allowed: Optional[bool] = None,
+        allow_external_modification: Optional[bool] = None,
+        force: Optional[bool] = None,
+        sync: Optional[bool] = None,
+    ) -> None:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def delete(self, *, access_code_id: str, sync: Optional[bool] = None) -> None:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def get(
+        self,
+        *,
+        device_id: Optional[str] = None,
+        access_code_id: Optional[str] = None,
+        code: Optional[str] = None,
+    ) -> UnmanagedAccessCode:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def list(
+        self, *, device_id: str, user_identifier_key: Optional[str] = None
+    ) -> List[UnmanagedAccessCode]:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def update(
+        self,
+        *,
+        access_code_id: str,
+        is_managed: bool,
+        allow_external_modification: Optional[bool] = None,
+        is_external_modification_allowed: Optional[bool] = None,
+        force: Optional[bool] = None,
+    ) -> None:
+        raise NotImplementedError()
+
+
 class AbstractDevicesSimulate(abc.ABC):
 
     @abc.abstractmethod
     def remove(self, *, device_id: str) -> None:
         raise NotImplementedError()
```

### Comparing `seam-0.2.0/seam/user_identities.py` & `seam-0.3.0/seam/user_identities.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/user_identities_enrollment_automations.py` & `seam-0.3.0/seam/user_identities_enrollment_automations.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/utils/deep_attr_dict.py` & `seam-0.3.0/seam/utils/deep_attr_dict.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/webhooks.py` & `seam-0.3.0/seam/webhooks.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/seam/workspaces.py` & `seam-0.3.0/seam/workspaces.py`

 * *Files identical despite different names*

### Comparing `seam-0.2.0/PKG-INFO` & `seam-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seam
-Version: 0.2.0
+Version: 0.3.0
 Summary: SDK for the Seam API written in Python.
 Home-page: https://github.com/seamapi/python-next
 License: MIT
 Author: Seam Labs, Inc.
 Author-email: engineering@getseam.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

