# Comparing `tmp/msfabricpysdkcore-0.0.4.tar.gz` & `tmp/msfabricpysdkcore-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msfabricpysdkcore-0.0.4.tar", last modified: Thu Apr 11 10:29:49 2024, max compression
+gzip compressed data, was "msfabricpysdkcore-0.0.5.tar", last modified: Thu Apr 11 17:35:20 2024, max compression
```

## Comparing `msfabricpysdkcore-0.0.4.tar` & `msfabricpysdkcore-0.0.5.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 10:29:49.043453 msfabricpysdkcore-0.0.4/
--rw-rw-rw-   0        0        0     1156 2024-04-10 07:49:21.000000 msfabricpysdkcore-0.0.4/LICENSE
--rw-rw-rw-   0        0        0    16184 2024-04-11 10:29:49.041303 msfabricpysdkcore-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    15666 2024-04-11 09:50:11.000000 msfabricpysdkcore-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 10:29:48.944992 msfabricpysdkcore-0.0.4/msfabricpysdkcore/
--rw-rw-rw-   0        0        0       78 2024-04-10 09:59:59.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/__init__.py
--rw-rw-rw-   0        0        0     3778 2024-04-11 09:28:32.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/admin_item.py
--rw-rw-rw-   0        0        0     4248 2024-04-11 07:13:04.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/admin_workspace.py
--rw-rw-rw-   0        0        0    21039 2024-04-11 09:11:00.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/adminapi.py
--rw-rw-rw-   0        0        0     1929 2024-04-02 10:11:53.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/auth.py
--rw-rw-rw-   0        0        0     1761 2024-04-10 09:00:53.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/capacity.py
--rw-rw-rw-   0        0        0     1060 2024-04-10 09:50:03.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/client.py
--rw-rw-rw-   0        0        0    14367 2024-04-10 09:55:03.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/coreapi.py
--rw-rw-rw-   0        0        0    14722 2024-04-10 15:15:40.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/domain.py
--rw-rw-rw-   0        0        0    11155 2024-04-10 09:00:37.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/item.py
--rw-rw-rw-   0        0        0     2828 2024-04-10 09:01:04.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/job_instance.py
--rw-rw-rw-   0        0        0     4011 2024-04-09 16:58:34.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/lakehouse.py
--rw-rw-rw-   0        0        0     3021 2024-04-02 12:46:53.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/long_running_operation.py
--rw-rw-rw-   0        0        0     2102 2024-04-10 09:00:15.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/onelakeshortcut.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:29:49.028252 msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/
--rw-rw-rw-   0        0        0        0 2024-03-22 16:16:45.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/__init__.py
--rw-rw-rw-   0        0        0     2062 2024-04-11 09:34:12.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_admin_apis.py
--rw-rw-rw-   0        0        0     4649 2024-04-10 15:12:58.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_domains.py
--rw-rw-rw-   0        0        0     2398 2024-04-10 09:53:02.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_git.py
--rw-rw-rw-   0        0        0     2941 2024-04-10 09:52:48.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_items_incl_lakehouse.py
--rw-rw-rw-   0        0        0     1581 2024-04-10 09:53:00.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_jobs.py
--rw-rw-rw-   0        0        0     2390 2024-04-10 09:53:04.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_shortcuts.py
--rw-rw-rw-   0        0        0     6563 2024-04-10 09:53:06.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_workspaces_capacities.py
--rw-rw-rw-   0        0        0    21544 2024-04-10 09:00:03.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/workspace.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:29:49.037223 msfabricpysdkcore-0.0.4/msfabricpysdkcore.egg-info/
--rw-rw-rw-   0        0        0    16184 2024-04-11 10:29:48.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1059 2024-04-11 10:29:48.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 10:29:48.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-11 10:29:48.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-11 10:29:48.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      564 2024-04-11 10:22:43.000000 msfabricpysdkcore-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-11 10:29:49.043453 msfabricpysdkcore-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      235 2024-04-11 10:22:49.000000 msfabricpysdkcore-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:35:20.495555 msfabricpysdkcore-0.0.5/
+-rw-rw-rw-   0        0        0     1156 2024-04-10 07:49:21.000000 msfabricpysdkcore-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0    16184 2024-04-11 17:35:20.483603 msfabricpysdkcore-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    15666 2024-04-11 09:50:11.000000 msfabricpysdkcore-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 17:35:20.381876 msfabricpysdkcore-0.0.5/msfabricpysdkcore/
+-rw-rw-rw-   0        0        0       78 2024-04-10 09:59:59.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/__init__.py
+-rw-rw-rw-   0        0        0     3778 2024-04-11 09:28:32.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/admin_item.py
+-rw-rw-rw-   0        0        0     4248 2024-04-11 07:13:04.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/admin_workspace.py
+-rw-rw-rw-   0        0        0    21039 2024-04-11 09:11:00.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/adminapi.py
+-rw-rw-rw-   0        0        0     1929 2024-04-02 10:11:53.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/auth.py
+-rw-rw-rw-   0        0        0     1761 2024-04-10 09:00:53.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/capacity.py
+-rw-rw-rw-   0        0        0     1060 2024-04-10 09:50:03.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/client.py
+-rw-rw-rw-   0        0        0    14423 2024-04-11 14:22:24.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/coreapi.py
+-rw-rw-rw-   0        0        0    14722 2024-04-10 15:15:40.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/domain.py
+-rw-rw-rw-   0        0        0    11296 2024-04-11 14:34:03.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/item.py
+-rw-rw-rw-   0        0        0     2745 2024-04-11 11:55:54.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/job_instance.py
+-rw-rw-rw-   0        0        0     3928 2024-04-11 11:55:24.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/lakehouse.py
+-rw-rw-rw-   0        0        0     2848 2024-04-11 16:24:05.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/long_running_operation.py
+-rw-rw-rw-   0        0        0     2102 2024-04-10 09:00:15.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/onelakeshortcut.py
+-rw-rw-rw-   0        0        0      737 2024-04-11 13:45:47.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/otheritems.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:35:20.465140 msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-22 16:16:45.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/__init__.py
+-rw-rw-rw-   0        0        0     2062 2024-04-11 09:34:12.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_admin_apis.py
+-rw-rw-rw-   0        0        0     4649 2024-04-10 15:12:58.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_domains.py
+-rw-rw-rw-   0        0        0     2398 2024-04-10 09:53:02.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_git.py
+-rw-rw-rw-   0        0        0     4627 2024-04-11 15:34:34.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_items_incl_lakehouse.py
+-rw-rw-rw-   0        0        0     1581 2024-04-10 09:53:00.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_jobs.py
+-rw-rw-rw-   0        0        0     2390 2024-04-10 09:53:04.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_shortcuts.py
+-rw-rw-rw-   0        0        0     6563 2024-04-10 09:53:06.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_workspaces_capacities.py
+-rw-rw-rw-   0        0        0    26160 2024-04-11 14:25:12.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/workspace.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:35:20.483603 msfabricpysdkcore-0.0.5/msfabricpysdkcore.egg-info/
+-rw-rw-rw-   0        0        0    16184 2024-04-11 17:35:20.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2024-04-11 17:35:20.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 17:35:20.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-11 17:35:20.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-11 17:35:20.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      564 2024-04-11 10:42:03.000000 msfabricpysdkcore-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 17:35:20.496556 msfabricpysdkcore-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      235 2024-04-11 10:41:58.000000 msfabricpysdkcore-0.0.5/setup.py
```

### Comparing `msfabricpysdkcore-0.0.4/LICENSE` & `msfabricpysdkcore-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.4/PKG-INFO` & `msfabricpysdkcore-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msfabricpysdkcore
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python SDK for Microsoft Fabric
 Author: Andreas Rederer
 Project-URL: Homepage, https://github.com/DaSenf1860/ms-fabric-sdk-core
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `msfabricpysdkcore-0.0.4/README.md` & `msfabricpysdkcore-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/admin_item.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/admin_item.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/admin_workspace.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/admin_workspace.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/adminapi.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/adminapi.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/auth.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/auth.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/capacity.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/capacity.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/client.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/client.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/coreapi.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/coreapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,18 +199,18 @@
         return ws.get_item(item_id = item_id, item_name = item_name, item_type = item_type)
 
     def delete_item(self, workspace_id, item_id):
         """Delete an item from a workspace"""
         ws = self.get_workspace_by_id(workspace_id)
         return ws.delete_item(item_id)
 
-    def list_items(self, workspace_id):
+    def list_items(self, workspace_id, with_properties = False):
         """List items in a workspace"""
         ws = self.get_workspace_by_id(workspace_id)
-        return ws.list_items()
+        return ws.list_items(with_properties=with_properties)
     
     def get_item_definition(self, workspace_id, item_id):
         """Get the definition of an item"""
         ws = self.get_workspace_by_id(workspace_id)
         return ws.get_item_definition(item_id)
     
     def update_item(self, workspace_id, item_id, display_name = None, description = None):
```

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/domain.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/domain.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/item.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/item.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,25 +76,27 @@
         for _ in range(10):
             response = requests.post(url=url, headers=self.auth.get_headers())
             if response.status_code == 429:
                 print("Too many requests, waiting 10 seconds")
                 sleep(10)
                 continue
             if response.status_code == 202:
-                check_long_running_operation( response.headers, self.auth)
+                operation_result = check_long_running_operation( response.headers, self.auth)
+                self.definition = operation_result['definition']
+                return operation_result
                 
             if response.status_code not in (200, 202, 429):
                 print(response.status_code)
                 print(response.text)
                 raise Exception(f"Error getting item definition: {response.text}")
             break
         
-        print(response.text)
-        print(response.status_code)
-        return json.loads(response.text)
+        resp_dict = json.loads(response.text)
+        self.definition = resp_dict['definition']
+        return resp_dict
     
     def update(self, display_name = None, description = None):
         """Update the item"""
         url = f"https://api.fabric.microsoft.com/v1/workspaces/{self.workspace_id}/items/{self.id}"
 
         payload = dict()
         if display_name:
```

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/job_instance.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/job_instance.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json 
 import requests
 from time import sleep
-from msfabricpysdkcore.long_running_operation import check_long_running_operation
 
 class JobInstance:
     """Class to represent a job instance in Microsoft Fabric"""
 
     def __init__(self, id, item_id, workspace_id, auth, job_type, invoke_type, status, root_activity_id,
                  start_time_utc, end_time_utc, failureReason):
```

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/lakehouse.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/lakehouse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json 
 import requests
 from time import sleep
 
-from msfabricpysdkcore.long_running_operation import check_long_running_operation
 from msfabricpysdkcore.item import Item
 
 class Lakehouse(Item):
     """Class to represent a item in Microsoft Fabric"""
 
     def __init__(self, id, display_name, type, workspace_id, auth, properties = None, definition=None, description=""):
         super().__init__(id, display_name, type, workspace_id, auth, properties, definition, description)
```

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/long_running_operation.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/long_running_operation.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,21 +18,22 @@
 
         for _ in range(10):
             response = requests.get(url=url, headers=self.auth.get_headers())
             if response.status_code == 429:
                 print("Too many requests, waiting 10 seconds")
                 sleep(10)
                 continue
+            if response.status_code == 400:
+                return None
             if response.status_code not in (200, 429):
                 print(response.status_code)
                 print(response.text)
                 raise Exception(f"Error getting operation results: {response.text}")
             break
 
-        print(json.loads(response.text))
         return json.loads(response.text)
     
     def get_operation_state(self):
         """Get the state of an operation"""
         url = f"https://api.fabric.microsoft.com/v1/operations/{self.operation_id}"
 
         for _ in range(10):
@@ -43,15 +44,14 @@
                 continue
             if response.status_code not in (200, 429):
                 print(response.status_code)
                 print(response.text)
                 raise Exception(f"Error getting operation state: {response.text}")
             break
 
-        print(json.loads(response.text))
         return json.loads(response.text)    
     
     def wait_for_completion(self):
         """Wait for the operation to complete"""
         max_iter = 20
         while self.state not in ('Succeeded', 'Failed'):
             self.state = self.get_operation_state()["status"]
@@ -68,14 +68,11 @@
     operation_id = headers.get('x-ms-operation-id', None)
     if location:
         operation_id = location.split("/")[-1]
     
     if not operation_id:
         print("Operation initiated, no operation id found")
         return None
-    else:
-        print("Operation initiated, waiting for completion")
-        lro = LongRunningOperation(operation_id=operation_id, auth=auth)
-        lro.wait_for_completion()
-        print("Operation completed")
-    lro = LongRunningOperation(operation_id, auth)
-    return lro.wait_for_completion()
+    lro = LongRunningOperation(operation_id=operation_id, auth=auth)
+    lro.wait_for_completion()
+    
+    return lro.get_operation_results()
```

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/onelakeshortcut.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/onelakeshortcut.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_admin_apis.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_admin_apis.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_domains.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_domains.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_git.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_items_incl_lakehouse.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_shortcuts.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,53 @@
 import unittest
+from msfabricpysdkcore.coreapi import FabricClientCore
 from datetime import datetime
 from dotenv import load_dotenv
-from time import sleep
-from msfabricpysdkcore.coreapi import FabricClientCore
 
 class TestFabricClientCore(unittest.TestCase):
 
     def __init__(self, *args, **kwargs):
         super(TestFabricClientCore, self).__init__(*args, **kwargs)
         #load_dotenv()
         self.fc = FabricClientCore()
         self.workspace_id = "c3352d34-0b54-40f0-b204-cc964b1beb8d"
 
-        datetime_str = datetime.now().strftime("%Y%m%d%H%M%S")
-        self.item_name = "testitem" + datetime_str
-        self.item_type = "Notebook"
-    
-    def test_item_end_to_end(self):
-
-        item = self.fc.create_item(display_name=self.item_name, type=self.item_type, workspace_id=self.workspace_id) 
-        self.assertEqual(item.display_name, self.item_name)
-        self.assertEqual(item.type, self.item_type)
-        self.assertEqual(item.workspace_id, self.workspace_id)
-        self.assertEqual(item.description, "")
-
-        item = self.fc.get_item(workspace_id=self.workspace_id, item_id=item.id)
-        item_ = self.fc.get_item(workspace_id=self.workspace_id,
-                                  item_name=self.item_name, item_type=self.item_type)
-        self.assertEqual(item.id, item_.id)
-        self.assertEqual(item.display_name, self.item_name)
-        self.assertEqual(item.type, self.item_type)
-        self.assertEqual(item.workspace_id, self.workspace_id)
-        self.assertEqual(item.description, "")
-
-        item_list = self.fc.list_items(workspace_id=self.workspace_id)
-        self.assertTrue(len(item_list) > 0)
-
-        item_ids = [item_.id for item_ in item_list]
-        self.assertIn(item.id, item_ids)
-
-        self.fc.update_item(workspace_id=self.workspace_id, item_id=item.id, display_name=f"u{self.item_name}")
-        item = self.fc.get_item(workspace_id=self.workspace_id, item_id=item.id)
-        self.assertEqual(item.display_name, f"u{self.item_name}")
-
-        status_code = self.fc.delete_item(workspace_id=self.workspace_id, item_id=item.id)
+        self.lakehouse_target = "cb4ca0b5-b53b-4879-b206-a53c35cbff55"
+        self.lakehouse_shortcut = "e2c09c89-bf97-4f71-bdeb-36338795ec36"
 
+        datetime_str = datetime.now().strftime("%Y%m%d%H%M%S")
+        self.shortcutname = "shortcut" + datetime_str
+        self.path_target = "Files/folder1"
+        self.path_shortcut = "Files/shortcutfolder"
+
+        self.target = {'oneLake': {'itemId': self.lakehouse_target,
+                                   'path': self.path_target,        
+                                   'workspaceId': self.workspace_id}}
+
+    def test_shortcut_end_to_end(self):
+
+        item = self.fc.create_shortcut(workspace_id=self.workspace_id,
+                                       item_id=self.lakehouse_shortcut,
+                                       path=self.path_shortcut,
+                                       name=self.shortcutname,
+                                       target=self.target)
+        self.assertEqual(item.name, self.shortcutname)
+        self.assertEqual(item.path, self.path_shortcut)
+        self.assertEqual(item.target, self.target)
+
+        item = self.fc.get_shortcut(workspace_id=self.workspace_id,
+                                    item_id=self.lakehouse_shortcut,
+                                    path=self.path_shortcut,
+                                    name=self.shortcutname)
+        self.assertEqual(item.name, self.shortcutname)
+        self.assertEqual(item.path, self.path_shortcut)
+        self.assertEqual(item.target, self.target)
+
+        status_code = self.fc.delete_shortcut(workspace_id=self.workspace_id,
+                                             item_id=self.lakehouse_shortcut,
+                                             path=self.path_shortcut,
+                                             name=self.shortcutname)
+        
         self.assertAlmostEqual(status_code, 200)
 
-    def test_lakehouse(self):
-
-        lakehouse = self.fc.get_item(workspace_id=self.workspace_id, item_name="lakehouse1", item_type="Lakehouse")
-        item_id = lakehouse.id
-        date_str = datetime.now().strftime("%Y%m%d%H%M%S")
-        table_name = f"table{date_str}"
-
-
-        status_code = self.fc.load_table(workspace_id=self.workspace_id, item_id=item_id, table_name=table_name, 
-                                         path_type="File", relative_path="Files/folder1/titanic.csv")
-
-        self.assertEqual(status_code, 202)
-
-        table_list = self.fc.list_tables(workspace_id=self.workspace_id, item_id=item_id)
-        table_names = [table["name"] for table in table_list]
-
-        self.assertIn(table_name, table_names)
-
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_jobs.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_workspaces_capacities.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_workspaces_capacities.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore/workspace.py` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore/workspace.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import json 
 import requests
 from time import sleep
 from msfabricpysdkcore.item import Item
+from msfabricpysdkcore.lakehouse import Lakehouse
 from msfabricpysdkcore.long_running_operation import check_long_running_operation
+from msfabricpysdkcore.otheritems import SparkJobDefinition
+from msfabricpysdkcore.otheritems import Warehouse
 
 class Workspace:
     """Class to represent a workspace in Microsoft Fabric"""
 
     def __init__(self, id, display_name, description, type, auth, capacity_id = None) -> None:
         self.id = id
         self.display_name = display_name
@@ -243,56 +246,148 @@
                 print(response.text)
                 raise Exception(f"Error creating item: {response.text}")
             break
 
         item_dict = json.loads(response.text)
         if item_dict is None:
             print("Item not returned by API, trying to get it by name")
-            return self.get_item_by_name(display_name, type)        
-        return Item.from_dict(item_dict, auth=self.auth)
+            return self.get_item_by_name(display_name, type)    
+
+        if item_dict["type"] == "Lakehouse":
+            return self.get_lakehouse(item_dict["id"])
+        if item_dict["type"] == "Warehouse":
+            return self.get_warehouse(item_dict["id"])
+        if item_dict["type"] == "SparkJobDefinition":
+            return self.get_spark_job_definition(item_dict["id"])
         
+        item_obj = Item.from_dict(item_dict, auth=self.auth)
+        if item_obj.type in ["Notebook", "Report", "SemanticModel"]:
+            item_obj.get_definition()
+        return item_obj
 
     def get_item_by_name(self, item_name, item_type):
         """Get an item from a workspace by name"""
-        ws_items = self.list_items()
+        ws_items = self.list_items(with_properties=False)
         for item in ws_items:
             if item.display_name == item_name and item.type == item_type:
-                return item    
+                return self.get_item(item.id, item_type)    
 
-    def get_item(self, item_id = None, item_name = None, item_type = None):
-        # GET https://api.fabric.microsoft.com/v1/workspaces/{workspaceId}/items/{itemId}
-        """Get an item from a workspace"""
-        if item_id is None and item_name is not None and item_type is not None:
-            return self.get_item_by_name(item_name, item_type)
-        elif item_id is None:
-            raise Exception("item_id or the combination item_name + item_type is required")
-        
-        url = f"https://api.fabric.microsoft.com/v1/workspaces/{self.id}/items/{item_id}"
+
+    def get_item_internal(self, url):
 
         for _ in range(10):
             response = requests.get(url=url, headers=self.auth.get_headers())
             if response.status_code == 429:
                 print("Too many requests, waiting 10 seconds")
                 sleep(10)
                 continue
             if response.status_code not in (200, 429):
                 print(response.status_code)
                 print(response.text)
                 raise Exception(f"Error getting item: {response.text}")
             break
         
         item_dict = json.loads(response.text)
-        return Item.from_dict(item_dict, auth=self.auth)
+        return item_dict
+
+    def get_lakehouse(self, lakehouse_id = None, lakehouse_name = None):
+        """Get a lakehouse from a workspace"""
+
+        if lakehouse_id is None and lakehouse_name is not None:
+            return self.get_item_by_name(lakehouse_name, "Lakehouse")
+        elif lakehouse_id is None:
+            raise Exception("lakehouse_id or the lakehouse_name is required")
+        
+        url = f"https://api.fabric.microsoft.com/v1/workspaces/{self.id}/lakehouses/{lakehouse_id}"
+
+        item_dict = self.get_item_internal(url)
+        return Lakehouse.from_dict(item_dict, auth=self.auth)
+    
+    def get_warehouse(self, warehouse_id = None, warehouse_name = None):
+        """Get a warehouse from a workspace"""
+        if warehouse_id is None and warehouse_name is not None:
+            return self.get_item_by_name(warehouse_name, "Warehouse")
+        elif warehouse_id is None:
+            raise Exception("warehouse_id or the warehouse_name is required")
+        
+        url = f"https://api.fabric.microsoft.com/v1/workspaces/{self.id}/warehouses/{warehouse_id}"
+
+        item_dict = self.get_item_internal(url)
+        return Warehouse.from_dict(item_dict, auth=self.auth)
+
+    def get_spark_job_definition(self, spark_job_definition_id = None, spark_job_definition_name = None):
+        """Get a spark job definition from a workspace"""
+        if spark_job_definition_id is None and spark_job_definition_name is not None:
+            return self.get_item_by_name(spark_job_definition_name, "SparkJobDefinition")
+        elif spark_job_definition_id is None:
+            raise Exception("spark_job_definition_id or the spark_job_definition_name is required")
+        
+        url = f"https://api.fabric.microsoft.com/v1/workspaces/{self.id}/sparkjobdefinitions/{spark_job_definition_id}"
+
+        item_dict = self.get_item_internal(url)
+        sjd_obj =  SparkJobDefinition.from_dict(item_dict, auth=self.auth)
+        sjd_obj.get_definition()
+        return sjd_obj
+
+    def get_item(self, item_id = None, item_name = None, item_type = None):
+        # GET https://api.fabric.microsoft.com/v1/workspaces/{workspaceId}/items/{itemId}
+        """Get an item from a workspace"""
+        if item_type:
+            if item_type.lower() == "lakehouse":
+                return self.get_lakehouse(item_id, item_name)
+            if item_type.lower() == "warehouse":
+                return self.get_warehouse(item_id, item_name)
+            if item_type.lower() == "sparkjobdefinition":
+                return self.get_spark_job_definition(item_id, item_name)
+                
+        if item_id is None and item_name is not None and item_type is not None:
+            return self.get_item_by_name(item_name, item_type)
+        elif item_id is None:
+            raise Exception("item_id or the combination item_name + item_type is required")
+        
+        url = f"https://api.fabric.microsoft.com/v1/workspaces/{self.id}/items/{item_id}"
+
+        item_dict = self.get_item_internal(url)
+        if item_dict["type"] == "Lakehouse":
+            return self.get_lakehouse(item_dict["id"])
+        if item_dict["type"] == "Warehouse":
+            return self.get_warehouse(item_dict["id"])
+        if item_dict["type"] == "SparkJobDefinition":
+            return self.get_spark_job_definition(item_dict["id"])
+        
+
+        item_obj = Item.from_dict(item_dict, auth=self.auth)
+        if item_obj.type in ["Notebook", "Report", "SemanticModel"]:
+            item_obj.get_definition()
+        return item_obj
+
 
     def delete_item(self, item_id):
         """Delete an item from a workspace"""
         return self.get_item(item_id).delete()
   
 
-    def list_items(self, continuationToken = None):
+    def get_item_object_w_properties(self, item_list):
+
+        new_item_list = []
+        for item in item_list:
+            if item["type"] == "Lakehouse":
+                item = self.get_lakehouse(item["id"])
+            elif item["type"] == "Warehouse":
+                item = self.get_warehouse(item["id"])
+            elif item["type"] == "SparkJobDefinition":
+                item = self.get_spark_job_definition(item["id"])
+            else:
+                item = Item.from_dict(item, auth=self.auth)
+                if item.type in ["Notebook", "Report", "SemanticModel"]:
+                    item.get_definition()
+            new_item_list.append(item)
+        return new_item_list
+
+    def list_items(self, with_properties = False, continuationToken = None):
         """List items in a workspace"""
         url = f"https://api.fabric.microsoft.com/v1/workspaces/{self.id}/items"
 
         if continuationToken:
             url = f"{url}?continuationToken={continuationToken}"
 
         for _ in range(10):
@@ -305,18 +400,22 @@
                 print(response.status_code)
                 print(response.text)
                 raise Exception(f"Error listing items: {response.text}")
             break
         
         resp_dict = json.loads(response.text)
         items = resp_dict["value"]
-        items = [Item.from_dict(item, auth=self.auth) for item in items]
+        if with_properties:
+            items = self.get_item_object_w_properties(items)
+        else:
+            items = [Item.from_dict(item, auth=self.auth) for item in items]
 
         if "continuationToken" in resp_dict:
-            item_list_next = self.list_items(continuationToken=resp_dict["continuationToken"])
+            item_list_next = self.list_items(with_properties=with_properties, 
+                                             continuationToken=resp_dict["continuationToken"])
             items.extend(item_list_next)
 
         return items
     
     def get_item_definition(self, item_id):
         """Get the definition of an item from a workspace"""
         return self.get_item(item_id).get_definition()
```

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore.egg-info/PKG-INFO` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msfabricpysdkcore
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python SDK for Microsoft Fabric
 Author: Andreas Rederer
 Project-URL: Homepage, https://github.com/DaSenf1860/ms-fabric-sdk-core
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `msfabricpysdkcore-0.0.4/msfabricpysdkcore.egg-info/SOURCES.txt` & `msfabricpysdkcore-0.0.5/msfabricpysdkcore.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 msfabricpysdkcore/coreapi.py
 msfabricpysdkcore/domain.py
 msfabricpysdkcore/item.py
 msfabricpysdkcore/job_instance.py
 msfabricpysdkcore/lakehouse.py
 msfabricpysdkcore/long_running_operation.py
 msfabricpysdkcore/onelakeshortcut.py
+msfabricpysdkcore/otheritems.py
 msfabricpysdkcore/workspace.py
 msfabricpysdkcore.egg-info/PKG-INFO
 msfabricpysdkcore.egg-info/SOURCES.txt
 msfabricpysdkcore.egg-info/dependency_links.txt
 msfabricpysdkcore.egg-info/requires.txt
 msfabricpysdkcore.egg-info/top_level.txt
 msfabricpysdkcore/tests/__init__.py
```

### Comparing `msfabricpysdkcore-0.0.4/pyproject.toml` & `msfabricpysdkcore-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 65.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msfabricpysdkcore"
-version = "0.0.4"
+version = "0.0.5"
 dynamic = ["dependencies"]
 authors = [
   { name="Andreas Rederer"},
 ]
 description = "A Python SDK for Microsoft Fabric"
 readme = "README.md"
 requires-python = ">=3.11"
```

