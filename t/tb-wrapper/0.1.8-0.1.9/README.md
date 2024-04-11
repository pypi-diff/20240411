# Comparing `tmp/tb_wrapper-0.1.8.tar.gz` & `tmp/tb_wrapper-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tb_wrapper-0.1.8.tar", last modified: Thu Apr 11 07:42:32 2024, max compression
+gzip compressed data, was "tb_wrapper-0.1.9.tar", last modified: Thu Apr 11 08:54:46 2024, max compression
```

## Comparing `tb_wrapper-0.1.8.tar` & `tb_wrapper-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-11 07:42:32.072228 tb_wrapper-0.1.8/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    11357 2023-11-21 13:34:49.000000 tb_wrapper-0.1.8/LICENSE
--rw-r--r--   0 andrea    (1000) andrea    (1000)     1586 2024-04-11 07:42:32.072228 tb_wrapper-0.1.8/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1050 2023-12-12 14:30:11.000000 tb_wrapper-0.1.8/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      672 2024-04-11 07:42:09.000000 tb_wrapper-0.1.8/pyproject.toml
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2024-04-11 07:42:32.072228 tb_wrapper-0.1.8/setup.cfg
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-11 07:42:32.068227 tb_wrapper-0.1.8/tb_wrapper/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1517 2024-03-15 16:23:18.000000 tb_wrapper-0.1.8/tb_wrapper/AlarmController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2475 2024-04-09 14:26:35.000000 tb_wrapper-0.1.8/tb_wrapper/AssetController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5159 2024-04-11 07:41:20.000000 tb_wrapper-0.1.8/tb_wrapper/DeviceController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1821 2024-04-10 09:49:32.000000 tb_wrapper-0.1.8/tb_wrapper/MainController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3142 2024-04-09 14:26:33.000000 tb_wrapper-0.1.8/tb_wrapper/QueryController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1456 2024-04-09 14:26:31.000000 tb_wrapper-0.1.8/tb_wrapper/TelemetryController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      755 2024-04-09 14:26:28.000000 tb_wrapper-0.1.8/tb_wrapper/UserController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-12-07 10:30:45.000000 tb_wrapper-0.1.8/tb_wrapper/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1343 2023-12-07 10:30:45.000000 tb_wrapper-0.1.8/tb_wrapper/handle_exception.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-11 07:42:32.072228 tb_wrapper-0.1.8/tb_wrapper.egg-info/
--rw-r--r--   0 andrea    (1000) andrea    (1000)     1586 2024-04-11 07:42:32.000000 tb_wrapper-0.1.8/tb_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      647 2024-04-11 07:42:32.000000 tb_wrapper-0.1.8/tb_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2024-04-11 07:42:32.000000 tb_wrapper-0.1.8/tb_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       49 2024-04-11 07:42:32.000000 tb_wrapper-0.1.8/tb_wrapper.egg-info/requires.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       11 2024-04-11 07:42:32.000000 tb_wrapper-0.1.8/tb_wrapper.egg-info/top_level.txt
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-11 07:42:32.072228 tb_wrapper-0.1.8/tests/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7437 2023-12-07 10:30:45.000000 tb_wrapper-0.1.8/tests/test_AlarmController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    18776 2023-12-07 10:30:45.000000 tb_wrapper-0.1.8/tests/test_AssetController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    16871 2023-12-07 10:30:45.000000 tb_wrapper-0.1.8/tests/test_DeviceController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1301 2023-12-07 10:30:45.000000 tb_wrapper-0.1.8/tests/test_MainController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4190 2023-12-07 10:30:45.000000 tb_wrapper-0.1.8/tests/test_QueryController.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6763 2023-12-07 10:30:45.000000 tb_wrapper-0.1.8/tests/test_UserController.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-11 08:54:46.995237 tb_wrapper-0.1.9/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    11357 2023-11-21 13:34:49.000000 tb_wrapper-0.1.9/LICENSE
+-rw-r--r--   0 andrea    (1000) andrea    (1000)     1586 2024-04-11 08:54:46.995237 tb_wrapper-0.1.9/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1050 2023-12-12 14:30:11.000000 tb_wrapper-0.1.9/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      672 2024-04-11 08:53:29.000000 tb_wrapper-0.1.9/pyproject.toml
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2024-04-11 08:54:46.995237 tb_wrapper-0.1.9/setup.cfg
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-11 08:54:46.991237 tb_wrapper-0.1.9/tb_wrapper/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1517 2024-03-15 16:23:18.000000 tb_wrapper-0.1.9/tb_wrapper/AlarmController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2475 2024-04-09 14:26:35.000000 tb_wrapper-0.1.9/tb_wrapper/AssetController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5469 2024-04-11 08:52:26.000000 tb_wrapper-0.1.9/tb_wrapper/DeviceController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1821 2024-04-10 09:49:32.000000 tb_wrapper-0.1.9/tb_wrapper/MainController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3142 2024-04-09 14:26:33.000000 tb_wrapper-0.1.9/tb_wrapper/QueryController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1456 2024-04-09 14:26:31.000000 tb_wrapper-0.1.9/tb_wrapper/TelemetryController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      755 2024-04-09 14:26:28.000000 tb_wrapper-0.1.9/tb_wrapper/UserController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-12-07 10:30:45.000000 tb_wrapper-0.1.9/tb_wrapper/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1343 2023-12-07 10:30:45.000000 tb_wrapper-0.1.9/tb_wrapper/handle_exception.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-11 08:54:46.991237 tb_wrapper-0.1.9/tb_wrapper.egg-info/
+-rw-r--r--   0 andrea    (1000) andrea    (1000)     1586 2024-04-11 08:54:46.000000 tb_wrapper-0.1.9/tb_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      647 2024-04-11 08:54:46.000000 tb_wrapper-0.1.9/tb_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2024-04-11 08:54:46.000000 tb_wrapper-0.1.9/tb_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       49 2024-04-11 08:54:46.000000 tb_wrapper-0.1.9/tb_wrapper.egg-info/requires.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       11 2024-04-11 08:54:46.000000 tb_wrapper-0.1.9/tb_wrapper.egg-info/top_level.txt
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-11 08:54:46.991237 tb_wrapper-0.1.9/tests/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7437 2023-12-07 10:30:45.000000 tb_wrapper-0.1.9/tests/test_AlarmController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    18776 2023-12-07 10:30:45.000000 tb_wrapper-0.1.9/tests/test_AssetController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    16871 2023-12-07 10:30:45.000000 tb_wrapper-0.1.9/tests/test_DeviceController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1301 2023-12-07 10:30:45.000000 tb_wrapper-0.1.9/tests/test_MainController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4190 2023-12-07 10:30:45.000000 tb_wrapper-0.1.9/tests/test_QueryController.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6763 2023-12-07 10:30:45.000000 tb_wrapper-0.1.9/tests/test_UserController.py
```

### Comparing `tb_wrapper-0.1.8/LICENSE` & `tb_wrapper-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.8/PKG-INFO` & `tb_wrapper-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tb_wrapper
-Version: 0.1.8
+Version: 0.1.9
 Summary: Wrapper for Zoe Project
 Author-email: GolDAndy <author@example.com>
 Project-URL: Homepage, https://github.com/GolDandy7/tb_wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `tb_wrapper-0.1.8/README.md` & `tb_wrapper-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.8/pyproject.toml` & `tb_wrapper-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.2.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tb_wrapper"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="GolDAndy", email="author@example.com" },
 ]
 description = "Wrapper for Zoe Project"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tb_wrapper-0.1.8/tb_wrapper/AlarmController.py` & `tb_wrapper-0.1.9/tb_wrapper/AlarmController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.8/tb_wrapper/AssetController.py` & `tb_wrapper-0.1.9/tb_wrapper/AssetController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.8/tb_wrapper/DeviceController.py` & `tb_wrapper-0.1.9/tb_wrapper/DeviceController.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             page_size=10000, page=0)
         found = False
         for info in info_device.data:
             if info.name == device_profile_name:
                 found = True
         return found
 
-    def create_device_with_credentials(self, body: Dict):
+    def create_device_with_credentials(self, body: Dict) -> Device:
         return self.tb_client.save_device_with_credentials(
             body)
 
     def get_device_profile_id(self, device_profile_name: str):
         device_profile = self.tb_client.get_device_profile_infos(
             page=0, page_size=10000, text_search=device_profile_name)
 
@@ -74,29 +74,33 @@
 
     def delete_device_profile(self, device_profile_id: DeviceProfileId):
         return self.tb_client.device_profile_controller.delete_device_profile_using_delete(device_profile_id=device_profile_id, async_req=True)
 
     def delete_device(self, device_id: DeviceId):
         return self.tb_client.device_controller.delete_device_using_delete(device_id=device_id, async_req=True)
 
-    def get_tenant_devices(self, page: int, page_size: int, active: bool = None, name: str = None, sort_by: str = None, sort_order: str = None):
+    def get_tenant_devices(self, page: int, page_size: int, active: bool = None, name: str = None, sort_by: str = None, sort_order: str = None) -> PageDataDeviceInfo:
         devices = self.tb_client.get_tenant_device_infos(
             page=page, page_size=page_size, active=active, sort_property=sort_by, sort_order=sort_order, text_search=name)
-        return devices.data
+        return devices
 
-    def get_customer_devices(self, customer_id: CustomerId, page: int, page_size: int, active: bool = None, name: str = None, sort_by: str = None, sort_order: str = None):
+    def get_customer_devices(self, customer_id: CustomerId, page: int, page_size: int, active: bool = None, name: str = None, sort_by: str = None, sort_order: str = None) -> PageDataDeviceInfo:
 
         devices = self.tb_client.get_customer_device_infos(
             customer_id=customer_id, page=page, page_size=page_size, active=active, sort_property=sort_by, sort_order=sort_order, text_search=name)
-        return devices.data
+        return devices
 
-    def get_device_profile_byId(self, device_profile_id: DeviceProfileId):
+    def get_device_profile_infobyId(self, device_profile_id: DeviceProfileId) -> DeviceProfileInfo:
         return self.tb_client.get_device_profile_info_by_id(device_profile_id)
 
+    def get_device_profile_infoByName(self, device_profile_name: str) -> DeviceProfile:
+        self.tb_client.get_device_profiles(
+            page=0, page_size=1, text_search=device_profile_name).data[0]
+
     def get_device_rulechainById(self, rulechain_id: RuleChainId) -> RuleChain:
         return self.tb_client.get_rule_chain_by_id(rulechain_id)
 
-    def get_device_rulechain_infoByName(self, rulechain_name: str):
-        return self.tb_client.get_rule_chains(page=0, page_size=1000, text_search=rulechain_name).data
+    def get_device_rulechain_infoByName(self, rulechain_name: str) -> RuleChain:
+        return self.tb_client.get_rule_chains(page=0, page_size=1, text_search=rulechain_name).data[0]
 
-    def get_device_credentials(self, device_id: DeviceId):
+    def get_device_credentials(self, device_id: DeviceId) -> DeviceCredentials:
         return self.tb_client.get_device_credentials_by_device_id(device_id)
```

### Comparing `tb_wrapper-0.1.8/tb_wrapper/MainController.py` & `tb_wrapper-0.1.9/tb_wrapper/MainController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.8/tb_wrapper/QueryController.py` & `tb_wrapper-0.1.9/tb_wrapper/QueryController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.8/tb_wrapper/TelemetryController.py` & `tb_wrapper-0.1.9/tb_wrapper/TelemetryController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.8/tb_wrapper/UserController.py` & `tb_wrapper-0.1.9/tb_wrapper/UserController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.8/tb_wrapper/handle_exception.py` & `tb_wrapper-0.1.9/tb_wrapper/handle_exception.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.8/tb_wrapper.egg-info/PKG-INFO` & `tb_wrapper-0.1.9/tb_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tb_wrapper
-Version: 0.1.8
+Version: 0.1.9
 Summary: Wrapper for Zoe Project
 Author-email: GolDAndy <author@example.com>
 Project-URL: Homepage, https://github.com/GolDandy7/tb_wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `tb_wrapper-0.1.8/tb_wrapper.egg-info/SOURCES.txt` & `tb_wrapper-0.1.9/tb_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.8/tests/test_AlarmController.py` & `tb_wrapper-0.1.9/tests/test_AlarmController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.8/tests/test_AssetController.py` & `tb_wrapper-0.1.9/tests/test_AssetController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.8/tests/test_DeviceController.py` & `tb_wrapper-0.1.9/tests/test_DeviceController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.8/tests/test_MainController.py` & `tb_wrapper-0.1.9/tests/test_MainController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.8/tests/test_QueryController.py` & `tb_wrapper-0.1.9/tests/test_QueryController.py`

 * *Files identical despite different names*

### Comparing `tb_wrapper-0.1.8/tests/test_UserController.py` & `tb_wrapper-0.1.9/tests/test_UserController.py`

 * *Files identical despite different names*

