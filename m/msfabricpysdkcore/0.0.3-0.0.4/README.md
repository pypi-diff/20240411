# Comparing `tmp/msfabricpysdkcore-0.0.3.tar.gz` & `tmp/msfabricpysdkcore-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msfabricpysdkcore-0.0.3.tar", last modified: Wed Apr 10 07:50:21 2024, max compression
+gzip compressed data, was "msfabricpysdkcore-0.0.4.tar", last modified: Thu Apr 11 10:29:49 2024, max compression
```

## Comparing `msfabricpysdkcore-0.0.3.tar` & `msfabricpysdkcore-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 07:50:21.701844 msfabricpysdkcore-0.0.3/
--rw-rw-rw-   0        0        0     1156 2024-04-10 07:49:21.000000 msfabricpysdkcore-0.0.3/LICENSE
--rw-rw-rw-   0        0        0    12511 2024-04-10 07:50:21.699851 msfabricpysdkcore-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    11991 2024-04-10 05:54:29.000000 msfabricpysdkcore-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 07:50:21.607255 msfabricpysdkcore-0.0.3/msfabricpysdkcore/
--rw-rw-rw-   0        0        0       36 2024-04-03 05:52:03.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/__init__.py
--rw-rw-rw-   0        0        0     1929 2024-04-02 10:11:53.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/auth.py
--rw-rw-rw-   0        0        0     1696 2024-04-09 16:57:48.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/capacity.py
--rw-rw-rw-   0        0        0    15047 2024-04-10 05:29:31.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/client.py
--rw-rw-rw-   0        0        0    11086 2024-04-10 05:11:49.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/item.py
--rw-rw-rw-   0        0        0     2759 2024-04-02 13:32:39.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/job_instance.py
--rw-rw-rw-   0        0        0     4011 2024-04-09 16:58:34.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/lakehouse.py
--rw-rw-rw-   0        0        0     3021 2024-04-02 12:46:53.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/long_running_operation.py
--rw-rw-rw-   0        0        0     2033 2024-03-28 05:21:57.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/onelakeshortcut.py
-drwxrwxrwx   0        0        0        0 2024-04-10 07:50:21.692327 msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/
--rw-rw-rw-   0        0        0        0 2024-03-22 16:16:45.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/__init__.py
--rw-rw-rw-   0        0        0     2397 2024-04-02 10:23:19.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/test_git.py
--rw-rw-rw-   0        0        0     2940 2024-04-10 05:26:30.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/test_items_incl_lakehouse.py
--rw-rw-rw-   0        0        0     1643 2024-04-02 13:24:07.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/test_jobs.py
--rw-rw-rw-   0        0        0     2389 2024-03-28 05:22:31.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/test_shortcuts.py
--rw-rw-rw-   0        0        0     6562 2024-04-10 05:15:10.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/test_workspaces_capacities.py
--rw-rw-rw-   0        0        0    21475 2024-04-10 05:31:51.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/workspace.py
-drwxrwxrwx   0        0        0        0 2024-04-10 07:50:21.696841 msfabricpysdkcore-0.0.3/msfabricpysdkcore.egg-info/
--rw-rw-rw-   0        0        0    12511 2024-04-10 07:50:21.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      820 2024-04-10 07:50:21.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 07:50:21.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-10 07:50:21.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-10 07:50:21.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      564 2024-04-04 12:17:39.000000 msfabricpysdkcore-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 07:50:21.701844 msfabricpysdkcore-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      235 2024-04-10 07:48:09.000000 msfabricpysdkcore-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 10:29:49.043453 msfabricpysdkcore-0.0.4/
+-rw-rw-rw-   0        0        0     1156 2024-04-10 07:49:21.000000 msfabricpysdkcore-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0    16184 2024-04-11 10:29:49.041303 msfabricpysdkcore-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    15666 2024-04-11 09:50:11.000000 msfabricpysdkcore-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 10:29:48.944992 msfabricpysdkcore-0.0.4/msfabricpysdkcore/
+-rw-rw-rw-   0        0        0       78 2024-04-10 09:59:59.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/__init__.py
+-rw-rw-rw-   0        0        0     3778 2024-04-11 09:28:32.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/admin_item.py
+-rw-rw-rw-   0        0        0     4248 2024-04-11 07:13:04.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/admin_workspace.py
+-rw-rw-rw-   0        0        0    21039 2024-04-11 09:11:00.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/adminapi.py
+-rw-rw-rw-   0        0        0     1929 2024-04-02 10:11:53.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/auth.py
+-rw-rw-rw-   0        0        0     1761 2024-04-10 09:00:53.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/capacity.py
+-rw-rw-rw-   0        0        0     1060 2024-04-10 09:50:03.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/client.py
+-rw-rw-rw-   0        0        0    14367 2024-04-10 09:55:03.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/coreapi.py
+-rw-rw-rw-   0        0        0    14722 2024-04-10 15:15:40.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/domain.py
+-rw-rw-rw-   0        0        0    11155 2024-04-10 09:00:37.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/item.py
+-rw-rw-rw-   0        0        0     2828 2024-04-10 09:01:04.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/job_instance.py
+-rw-rw-rw-   0        0        0     4011 2024-04-09 16:58:34.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/lakehouse.py
+-rw-rw-rw-   0        0        0     3021 2024-04-02 12:46:53.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/long_running_operation.py
+-rw-rw-rw-   0        0        0     2102 2024-04-10 09:00:15.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/onelakeshortcut.py
+drwxrwxrwx   0        0        0        0 2024-04-11 10:29:49.028252 msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-22 16:16:45.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/__init__.py
+-rw-rw-rw-   0        0        0     2062 2024-04-11 09:34:12.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_admin_apis.py
+-rw-rw-rw-   0        0        0     4649 2024-04-10 15:12:58.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_domains.py
+-rw-rw-rw-   0        0        0     2398 2024-04-10 09:53:02.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_git.py
+-rw-rw-rw-   0        0        0     2941 2024-04-10 09:52:48.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_items_incl_lakehouse.py
+-rw-rw-rw-   0        0        0     1581 2024-04-10 09:53:00.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_jobs.py
+-rw-rw-rw-   0        0        0     2390 2024-04-10 09:53:04.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_shortcuts.py
+-rw-rw-rw-   0        0        0     6563 2024-04-10 09:53:06.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_workspaces_capacities.py
+-rw-rw-rw-   0        0        0    21544 2024-04-10 09:00:03.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore/workspace.py
+drwxrwxrwx   0        0        0        0 2024-04-11 10:29:49.037223 msfabricpysdkcore-0.0.4/msfabricpysdkcore.egg-info/
+-rw-rw-rw-   0        0        0    16184 2024-04-11 10:29:48.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1059 2024-04-11 10:29:48.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 10:29:48.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-11 10:29:48.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-11 10:29:48.000000 msfabricpysdkcore-0.0.4/msfabricpysdkcore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      564 2024-04-11 10:22:43.000000 msfabricpysdkcore-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 10:29:49.043453 msfabricpysdkcore-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      235 2024-04-11 10:22:49.000000 msfabricpysdkcore-0.0.4/setup.py
```

### Comparing `msfabricpysdkcore-0.0.3/LICENSE` & `msfabricpysdkcore-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.3/PKG-INFO` & `msfabricpysdkcore-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: msfabricpysdkcore
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python SDK for Microsoft Fabric
 Author: Andreas Rederer
 Project-URL: Homepage, https://github.com/DaSenf1860/ms-fabric-sdk-core
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.30.0
 Requires-Dist: azure-identity>=1.15.0
 
-# A Python SDK for Microsoft Fabric
+# Python SDK for Microsoft Fabric
 
 This is a Python SDK for Microsoft Fabric. It is a wrapper around the REST APIs (v1) of Fabric*.
 
 ![Python hugging a F](assets/fabricpythontransparent.png)
 
 The Microsoft Fabric REST APIs are documented [here](https://docs.microsoft.com/en-us/rest/api/fabric/).
 They are designed to automate your Fabric processes.
@@ -30,25 +30,34 @@
 - Referencing objects by name instead of ID
 - More granular objects, e.g. a Workspace and Item object instead of referencing IDs all the time
 - Do bulk operations (see [Usage Patterns](usage_patterns.md))
 - Pagination support
 
 See the latest release notes [here](releasenotes/release_notes.md).
 
-Currently it supports all Core APIs and Lakehouse APIs, i.e.:
-- [Capacities](#working-with-capacities)
-- [Git](#working-with-git)
-- [Items](#working-with-items)
-- [Job Scheduler](#working-with-job-scheduler)
-- Long Running Operations
-- [OneLakeShortcuts](#working-with-one-lake-shortcuts)
-- [Workspaces](#working-with-workspaces)
-- [Lakehouse APIs](#lakehouse-apis)
+Currently it supports all Core APIs, Admin APIs and Lakehouse APIs, i.e.:
+- Core APIs
+  - [Capacities](#working-with-capacities)
+  - [Git](#working-with-git)
+  - [Items](#working-with-items)
+  - [Job Scheduler](#working-with-job-scheduler)
+  - Long Running Operations
+  - [OneLakeShortcuts](#working-with-one-lake-shortcuts)
+  - [Workspaces](#working-with-workspaces)
+- Lakehouse APIs
+  - [Tables](#tables)
+- Admin APIs
+  - [Domains](#admin-api-for-domains)
+  - [Items](#admin-api-for-items)
+  - [Tenants](#admin-api-for-tenants)
+  - [Users](#admin-api-for-users)
+  - [Workspaces](#admin-api-for-workspaces)
 
-It is planned to support also the Admin APIs and new APIs which are not released yet.
+It is planned to support also the APIs of the user experiences and new APIs which are not released yet.
+Also we have plans to support APIs to interact with Fabric capacities on the Azure Side.
 Eventually Power BI APIs like the Scanner API will be covered as well.
 
 *Because this SDK uses the API in the background, all limitations and restrictions of the API apply to this SDK as well. This includes rate limits, permissions, etc.
 
 
 
 
@@ -362,19 +371,21 @@
 # or
 ws.cancel_item_job_instance(item_id="item_id", job_instance_id="job_instance_id")
 # or 
 item.cancel_item_job_instance(job_instance_id="job_instance_id")
 
 ```
 
-## Lakehouse APIs
+### Tables
+
 
-# List tables in a Lakehouse
 
 ```python
+# List tables in a Lakehouse
+
 from msfabricpysdkcore import FabricClientCore
 
 fc = FabricClientCore()
 ws = fc.get_workspace_by_name("testworkspace")
 lakehouse = ws.get_item_by_name(item_name="lakehouse1", item_type="Lakehouse")
 table_list = lakehouse.list_tables()
 # or
@@ -391,9 +402,146 @@
               path_type= "File", relative_path="Files/folder1/titanic.csv")
 # or
 fc.load_table(workspace_id = "someworkspaceid", item_id = "someitemid", table_name="testtable",
               path_type= "File", relative_path="Files/folder1/titanic.csv")
 
 ```
 
+### Admin API for Workspaces
+
+```python
+from msfabricpysdkcore import FabricClientAdmin
+
+fca = FabricClientAdmin()
+
+
+# List workspaces
+ws = fca.list_workspaces(name="testworkspace")[0]
+
+# Get workspace
+ws = fca.get_workspace(workspace_id="workspace_id")
+
+# Get workspace access details
+
+ws_access = fca.get_workspace_access_details("workspace_id")
+# or
+ws_access = ws.get_access_details()
+```
+
+### Admin API for Users
+
+```python
+from msfabricpysdkcore import FabricClientAdmin
+
+fca = FabricClientAdmin()
+
+# Get access entities
+
+user_id = 'b4fuhaidc2'
+access_entities = fca.get_access_entities(user_id, type="Notebook")
+
+```
+
+### Admin API for Tenants
+
+```python
+from msfabricpysdkcore import FabricClientAdmin
+
+fca = FabricClientAdmin()
+
+# Get tenant settings
+
+tenant_settings = fca.get_tenant_settings()
+
+# Get capacity tenant settings overrides
+
+overrides = fca.get_capacities_tenant_settings_overrides()
+
+```
+
+### Admin API for Items
+
+```python
+from msfabricpysdkcore import FabricClientAdmin
+
+fca = FabricClientAdmin()
+
+# List items
+
+item_list = fca.list_items(workspace_id="wsid")
+
+# Get item
+
+item = fca.get_item(workspace_id="wsid", item_id=item_list[0].id)
+# or
+item = ws.get_item(item_id=item_list[0].id)
+
+# Get item access details
+
+item_access = fca.get_item_access_details(workspace_id="wsid", item_id=item_list[0].id)
+#or
+item_access = ws.get_item_access_details(item_id=item_list[0].id)
+# or
+item_access = item.get_access_details()
+
+```
+
+### Admin API for Domains
+
+```python
+from msfabricpysdkcore import FabricClientAdmin
+
+fca = FabricClientAdmin()
+
+# Create domain
+domain_name = "sdktestdomains"
+domain = fca.create_domain(display_name=domain_name)
+
+# Get domain by name
+domain_clone = fca.get_domain_by_name(domain_name)
+
+# Get domain by id
+domain_clone = fca.get_domain_by_id(domain.id)
+
+# List domains
+domains = fca.list_domains()
+
+# Update domain
+domain_new_name = "sdktestdomains2"
+domain_clone = fca.update_domain(domain.id, display_name=domain_new_name)
+
+# Assign domain workspaces by Ids
+fca.assign_domain_workspaces_by_ids(domain.id, ["workspace_id_1", "workspace_id_2"])
+
+# List domain workspaces
+workspaces = fca.list_domain_workspaces(domain.id, workspace_objects=True)
+
+# Unassign domain workspaces by ids
+status_code = fca.unassign_domain_workspaces_by_ids(domain.id, ["workspace_id_1", "workspace_id_2"])
+
+# Assign domain workspaces by capacities
+status_code = fca.assign_domain_workspaces_by_capacities(domain.id, ["cap_id1", "cap_id2"])
+
+# Unassign all domain workspaces
+status_code = fca.unassign_all_domain_workspaces(domain.id)
+
+# Assign domain workspaces by principals
+principal1 = {'id': '6edbsdfbfdgdf656', 'type': 'User'}
+principal2 = {'id': '6eyxcbyyxc57', 'type': 'User'}
+
+status_code = fca.assign_domains_workspaces_by_principals(domain.id, [principal1, principal2], wait_for_completion=True)
+
+# Role assignments bulk assign
+
+principals = [principal, principal_2]
+status_code = fca.role_assignments_bulk_assign(domain.id, "Contributors", principals)
+
+# Role assignments bulk unassign
+status_code = fca.role_assignments_bulk_unassign(domain.id, "Contributors", [principal_2])
+
+# Delete domain
+status_code = fca.delete_domain(domain.id)
+```
+
+
 Note: This SDK is not an official SDK from Microsoft. It is a community project and not supported by Microsoft. Use it at your own risk.
 Also the API is still in preview and might change. This SDK is not yet feature complete and might not cover all APIs yet. Feel free to contribute to this project to make it better.
```

### Comparing `msfabricpysdkcore-0.0.3/msfabricpysdkcore/auth.py` & `msfabricpysdkcore-0.0.4/msfabricpysdkcore/auth.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.3/msfabricpysdkcore/capacity.py` & `msfabricpysdkcore-0.0.4/msfabricpysdkcore/capacity.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,14 +34,17 @@
             'display_name': self.display_name,
             'sku': self.sku,
             'region': self.region,
             'state': self.state
         }
         return json.dumps(dic, indent=2)
 
+    def __repr__(self) -> str:
+        return self.__str__()
+
     def from_dict(dic):
         """Method to create a Capacity object from a dictionary
         
         Args:
             dic (dict): The dictionary containing the capacity information
         Returns:
             Capacity: The Capacity object created from the dictionary
```

### Comparing `msfabricpysdkcore-0.0.3/msfabricpysdkcore/client.py` & `msfabricpysdkcore-0.0.4/msfabricpysdkcore/coreapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,21 @@
 import requests
 import json
-import os
 from time import sleep
 
 from msfabricpysdkcore.capacity import Capacity
+from msfabricpysdkcore.client import FabricClient
 from msfabricpysdkcore.workspace import Workspace
-from msfabricpysdkcore.auth import FabricAuthClient, FabricServicePrincipal
 
-class FabricClientCore():
-    """FabricClientCore class to interact with Fabric API"""
+class FabricClientCore(FabricClient):
+    """FabricClientCore class to interact with Fabric Core APIs"""
 
     def __init__(self, tenant_id = None, client_id = None, client_secret = None) -> None:
         """Initialize FabricClientCore object"""
-        self.tenant_id = tenant_id if tenant_id else os.getenv("FABRIC_TENANT_ID")
-        self.client_id = client_id if client_id else os.getenv("FABRIC_CLIENT_ID")
-        self.client_secret = client_secret if client_secret else os.getenv("FABRIC_CLIENT_SECRET")
-
-        if self.client_id is None or self.client_secret is None or self.tenant_id is None:
-            self.auth = FabricAuthClient()
-        else:
-            self.auth = FabricServicePrincipal(tenant_id = self.tenant_id,
-                                               client_id = self.client_id, 
-                                               client_secret = self.client_secret)
-
-        self.scope = "https://api.fabric.microsoft.com/.default"
+        super().__init__(tenant_id, client_id, client_secret)
 
 
     def list_workspaces(self, continuationToken = None):
         """List all workspaces in the tenant"""
 
         url = "https://api.fabric.microsoft.com/v1/workspaces"
         if continuationToken:
@@ -329,8 +317,8 @@
     
     def load_table(self, workspace_id, item_id, table_name, path_type, relative_path,
                     file_extension = None, format_options = None,
                     mode = None, recursive = None, wait_for_completion = True):
         ws = self.get_workspace_by_id(workspace_id)
         return ws.load_table(item_id, table_name, path_type, relative_path,
                     file_extension, format_options,
-                    mode, recursive, wait_for_completion)
+                    mode, recursive, wait_for_completion)
```

### Comparing `msfabricpysdkcore-0.0.3/msfabricpysdkcore/item.py` & `msfabricpysdkcore-0.0.4/msfabricpysdkcore/item.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,17 @@
             'type': self.type,
             'definition': self.definition,
             'workspace_id': self.workspace_id,
             'properties': self.properties
         }
         return json.dumps(dict_, indent=2)
     
+    def __repr__(self) -> str:
+        return self.__str__()
+    
     def from_dict(item_dict, auth):
         """Create Item object from dictionary"""
         
         if item_dict['type'] == "Lakehouse":
             from msfabricpysdkcore.lakehouse import Lakehouse
             return Lakehouse(id=item_dict['id'], display_name=item_dict['displayName'], type=item_dict['type'], workspace_id=item_dict['workspaceId'],
                     properties=item_dict.get('properties', None),
```

### Comparing `msfabricpysdkcore-0.0.3/msfabricpysdkcore/job_instance.py` & `msfabricpysdkcore-0.0.4/msfabricpysdkcore/job_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,17 @@
             'root_activity_id': self.root_activity_id,
             'start_time_utc': self.start_time_utc,
             'end_time_utc': self.end_time_utc,
             'failureReason': self.failureReason
         }
         return json.dumps(dict_, indent=2)
     
+    def __repr__(self) -> str:
+        return self.__str__()
+    
     def from_dict(job_dict, auth):
         """Create JobInstance object from dictionary"""
         return JobInstance(id=job_dict['id'], item_id=job_dict['itemId'], workspace_id=job_dict['workspaceId'],
                            job_type=job_dict['jobType'], invoke_type=job_dict['invokeType'], status=job_dict['status'],
                            root_activity_id=job_dict['rootActivityId'], start_time_utc=job_dict['startTimeUtc'],
                            end_time_utc=job_dict['endTimeUtc'], failureReason=job_dict['failureReason'], auth=auth)
```

### Comparing `msfabricpysdkcore-0.0.3/msfabricpysdkcore/lakehouse.py` & `msfabricpysdkcore-0.0.4/msfabricpysdkcore/lakehouse.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.3/msfabricpysdkcore/long_running_operation.py` & `msfabricpysdkcore-0.0.4/msfabricpysdkcore/long_running_operation.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.3/msfabricpysdkcore/onelakeshortcut.py` & `msfabricpysdkcore-0.0.4/msfabricpysdkcore/onelakeshortcut.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,17 @@
             'path': self.path,
             'target': self.target,
             'item_id': self.item_id,
             'workspace_id': self.workspace_id,
         }
         return json.dumps(dict_, indent=2)
     
+    def __repr__(self) -> str:
+        return self.__str__()
+    
     def from_dict(short_dict, auth):
         """Create OneLakeShortCut object from dictionary"""
         return OneLakeShortcut(name=short_dict['name'],
                                path=short_dict['path'], 
                                target=short_dict['target'], 
                                item_id=short_dict['itemId'], 
                                workspace_id=short_dict['workspaceId'],
```

### Comparing `msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/test_git.py` & `msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_git.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from msfabricpysdkcore.client import FabricClientCore
+from msfabricpysdkcore.coreapi import FabricClientCore
 from datetime import datetime
 from dotenv import load_dotenv
 
 class TestFabricClientCore(unittest.TestCase):
 
     def __init__(self, *args, **kwargs):
         super(TestFabricClientCore, self).__init__(*args, **kwargs)
```

### Comparing `msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/test_items_incl_lakehouse.py` & `msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_items_incl_lakehouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 from datetime import datetime
 from dotenv import load_dotenv
 from time import sleep
-from msfabricpysdkcore.client import FabricClientCore
+from msfabricpysdkcore.coreapi import FabricClientCore
 
 class TestFabricClientCore(unittest.TestCase):
 
     def __init__(self, *args, **kwargs):
         super(TestFabricClientCore, self).__init__(*args, **kwargs)
         #load_dotenv()
         self.fc = FabricClientCore()
```

### Comparing `msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/test_jobs.py` & `msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_jobs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import unittest
-from msfabricpysdkcore.client import FabricClientCore
-from datetime import datetime
-from dotenv import load_dotenv
+from msfabricpysdkcore.coreapi import FabricClientCore
 
 class TestFabricClientCore(unittest.TestCase):
 
     def __init__(self, *args, **kwargs):
         super(TestFabricClientCore, self).__init__(*args, **kwargs)
         #load_dotenv()
         self.fc = FabricClientCore()
```

### Comparing `msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/test_shortcuts.py` & `msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_shortcuts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from msfabricpysdkcore.client import FabricClientCore
+from msfabricpysdkcore.coreapi import FabricClientCore
 from datetime import datetime
 from dotenv import load_dotenv
 
 class TestFabricClientCore(unittest.TestCase):
 
     def __init__(self, *args, **kwargs):
         super(TestFabricClientCore, self).__init__(*args, **kwargs)
```

### Comparing `msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/test_workspaces_capacities.py` & `msfabricpysdkcore-0.0.4/msfabricpysdkcore/tests/test_workspaces_capacities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from dotenv import load_dotenv
 from datetime import datetime
-from msfabricpysdkcore.client import FabricClientCore
+from msfabricpysdkcore.coreapi import FabricClientCore
 
 load_dotenv()
 
 class TestFabricClientCore(unittest.TestCase):
 
     def __init__(self, *args, **kwargs):
         super(TestFabricClientCore, self).__init__(*args, **kwargs)
```

### Comparing `msfabricpysdkcore-0.0.3/msfabricpysdkcore/workspace.py` & `msfabricpysdkcore-0.0.4/msfabricpysdkcore/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,17 @@
             'display_name': self.display_name,
             'description': self.description,
             'type': self.type,
             'capacity_id': self.capacity_id
         }
         return json.dumps(dict_, indent=2)
     
+    def __repr__(self) -> str:
+        return self.__str__()
+    
     def get_role_assignments(self):
         """Get role assignments for the workspace"""
         url = f"https://api.fabric.microsoft.com/v1/workspaces/{self.id}/roleAssignments"
 
         for _ in range(10):
             response = requests.get(url=url, headers=self.auth.get_headers())
             if response.status_code == 429:
```

### Comparing `msfabricpysdkcore-0.0.3/msfabricpysdkcore.egg-info/PKG-INFO` & `msfabricpysdkcore-0.0.4/msfabricpysdkcore.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: msfabricpysdkcore
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python SDK for Microsoft Fabric
 Author: Andreas Rederer
 Project-URL: Homepage, https://github.com/DaSenf1860/ms-fabric-sdk-core
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.30.0
 Requires-Dist: azure-identity>=1.15.0
 
-# A Python SDK for Microsoft Fabric
+# Python SDK for Microsoft Fabric
 
 This is a Python SDK for Microsoft Fabric. It is a wrapper around the REST APIs (v1) of Fabric*.
 
 ![Python hugging a F](assets/fabricpythontransparent.png)
 
 The Microsoft Fabric REST APIs are documented [here](https://docs.microsoft.com/en-us/rest/api/fabric/).
 They are designed to automate your Fabric processes.
@@ -30,25 +30,34 @@
 - Referencing objects by name instead of ID
 - More granular objects, e.g. a Workspace and Item object instead of referencing IDs all the time
 - Do bulk operations (see [Usage Patterns](usage_patterns.md))
 - Pagination support
 
 See the latest release notes [here](releasenotes/release_notes.md).
 
-Currently it supports all Core APIs and Lakehouse APIs, i.e.:
-- [Capacities](#working-with-capacities)
-- [Git](#working-with-git)
-- [Items](#working-with-items)
-- [Job Scheduler](#working-with-job-scheduler)
-- Long Running Operations
-- [OneLakeShortcuts](#working-with-one-lake-shortcuts)
-- [Workspaces](#working-with-workspaces)
-- [Lakehouse APIs](#lakehouse-apis)
+Currently it supports all Core APIs, Admin APIs and Lakehouse APIs, i.e.:
+- Core APIs
+  - [Capacities](#working-with-capacities)
+  - [Git](#working-with-git)
+  - [Items](#working-with-items)
+  - [Job Scheduler](#working-with-job-scheduler)
+  - Long Running Operations
+  - [OneLakeShortcuts](#working-with-one-lake-shortcuts)
+  - [Workspaces](#working-with-workspaces)
+- Lakehouse APIs
+  - [Tables](#tables)
+- Admin APIs
+  - [Domains](#admin-api-for-domains)
+  - [Items](#admin-api-for-items)
+  - [Tenants](#admin-api-for-tenants)
+  - [Users](#admin-api-for-users)
+  - [Workspaces](#admin-api-for-workspaces)
 
-It is planned to support also the Admin APIs and new APIs which are not released yet.
+It is planned to support also the APIs of the user experiences and new APIs which are not released yet.
+Also we have plans to support APIs to interact with Fabric capacities on the Azure Side.
 Eventually Power BI APIs like the Scanner API will be covered as well.
 
 *Because this SDK uses the API in the background, all limitations and restrictions of the API apply to this SDK as well. This includes rate limits, permissions, etc.
 
 
 
 
@@ -362,19 +371,21 @@
 # or
 ws.cancel_item_job_instance(item_id="item_id", job_instance_id="job_instance_id")
 # or 
 item.cancel_item_job_instance(job_instance_id="job_instance_id")
 
 ```
 
-## Lakehouse APIs
+### Tables
+
 
-# List tables in a Lakehouse
 
 ```python
+# List tables in a Lakehouse
+
 from msfabricpysdkcore import FabricClientCore
 
 fc = FabricClientCore()
 ws = fc.get_workspace_by_name("testworkspace")
 lakehouse = ws.get_item_by_name(item_name="lakehouse1", item_type="Lakehouse")
 table_list = lakehouse.list_tables()
 # or
@@ -391,9 +402,146 @@
               path_type= "File", relative_path="Files/folder1/titanic.csv")
 # or
 fc.load_table(workspace_id = "someworkspaceid", item_id = "someitemid", table_name="testtable",
               path_type= "File", relative_path="Files/folder1/titanic.csv")
 
 ```
 
+### Admin API for Workspaces
+
+```python
+from msfabricpysdkcore import FabricClientAdmin
+
+fca = FabricClientAdmin()
+
+
+# List workspaces
+ws = fca.list_workspaces(name="testworkspace")[0]
+
+# Get workspace
+ws = fca.get_workspace(workspace_id="workspace_id")
+
+# Get workspace access details
+
+ws_access = fca.get_workspace_access_details("workspace_id")
+# or
+ws_access = ws.get_access_details()
+```
+
+### Admin API for Users
+
+```python
+from msfabricpysdkcore import FabricClientAdmin
+
+fca = FabricClientAdmin()
+
+# Get access entities
+
+user_id = 'b4fuhaidc2'
+access_entities = fca.get_access_entities(user_id, type="Notebook")
+
+```
+
+### Admin API for Tenants
+
+```python
+from msfabricpysdkcore import FabricClientAdmin
+
+fca = FabricClientAdmin()
+
+# Get tenant settings
+
+tenant_settings = fca.get_tenant_settings()
+
+# Get capacity tenant settings overrides
+
+overrides = fca.get_capacities_tenant_settings_overrides()
+
+```
+
+### Admin API for Items
+
+```python
+from msfabricpysdkcore import FabricClientAdmin
+
+fca = FabricClientAdmin()
+
+# List items
+
+item_list = fca.list_items(workspace_id="wsid")
+
+# Get item
+
+item = fca.get_item(workspace_id="wsid", item_id=item_list[0].id)
+# or
+item = ws.get_item(item_id=item_list[0].id)
+
+# Get item access details
+
+item_access = fca.get_item_access_details(workspace_id="wsid", item_id=item_list[0].id)
+#or
+item_access = ws.get_item_access_details(item_id=item_list[0].id)
+# or
+item_access = item.get_access_details()
+
+```
+
+### Admin API for Domains
+
+```python
+from msfabricpysdkcore import FabricClientAdmin
+
+fca = FabricClientAdmin()
+
+# Create domain
+domain_name = "sdktestdomains"
+domain = fca.create_domain(display_name=domain_name)
+
+# Get domain by name
+domain_clone = fca.get_domain_by_name(domain_name)
+
+# Get domain by id
+domain_clone = fca.get_domain_by_id(domain.id)
+
+# List domains
+domains = fca.list_domains()
+
+# Update domain
+domain_new_name = "sdktestdomains2"
+domain_clone = fca.update_domain(domain.id, display_name=domain_new_name)
+
+# Assign domain workspaces by Ids
+fca.assign_domain_workspaces_by_ids(domain.id, ["workspace_id_1", "workspace_id_2"])
+
+# List domain workspaces
+workspaces = fca.list_domain_workspaces(domain.id, workspace_objects=True)
+
+# Unassign domain workspaces by ids
+status_code = fca.unassign_domain_workspaces_by_ids(domain.id, ["workspace_id_1", "workspace_id_2"])
+
+# Assign domain workspaces by capacities
+status_code = fca.assign_domain_workspaces_by_capacities(domain.id, ["cap_id1", "cap_id2"])
+
+# Unassign all domain workspaces
+status_code = fca.unassign_all_domain_workspaces(domain.id)
+
+# Assign domain workspaces by principals
+principal1 = {'id': '6edbsdfbfdgdf656', 'type': 'User'}
+principal2 = {'id': '6eyxcbyyxc57', 'type': 'User'}
+
+status_code = fca.assign_domains_workspaces_by_principals(domain.id, [principal1, principal2], wait_for_completion=True)
+
+# Role assignments bulk assign
+
+principals = [principal, principal_2]
+status_code = fca.role_assignments_bulk_assign(domain.id, "Contributors", principals)
+
+# Role assignments bulk unassign
+status_code = fca.role_assignments_bulk_unassign(domain.id, "Contributors", [principal_2])
+
+# Delete domain
+status_code = fca.delete_domain(domain.id)
+```
+
+
 Note: This SDK is not an official SDK from Microsoft. It is a community project and not supported by Microsoft. Use it at your own risk.
 Also the API is still in preview and might change. This SDK is not yet feature complete and might not cover all APIs yet. Feel free to contribute to this project to make it better.
```

### Comparing `msfabricpysdkcore-0.0.3/msfabricpysdkcore.egg-info/SOURCES.txt` & `msfabricpysdkcore-0.0.4/msfabricpysdkcore.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 msfabricpysdkcore/__init__.py
+msfabricpysdkcore/admin_item.py
+msfabricpysdkcore/admin_workspace.py
+msfabricpysdkcore/adminapi.py
 msfabricpysdkcore/auth.py
 msfabricpysdkcore/capacity.py
 msfabricpysdkcore/client.py
+msfabricpysdkcore/coreapi.py
+msfabricpysdkcore/domain.py
 msfabricpysdkcore/item.py
 msfabricpysdkcore/job_instance.py
 msfabricpysdkcore/lakehouse.py
 msfabricpysdkcore/long_running_operation.py
 msfabricpysdkcore/onelakeshortcut.py
 msfabricpysdkcore/workspace.py
 msfabricpysdkcore.egg-info/PKG-INFO
 msfabricpysdkcore.egg-info/SOURCES.txt
 msfabricpysdkcore.egg-info/dependency_links.txt
 msfabricpysdkcore.egg-info/requires.txt
 msfabricpysdkcore.egg-info/top_level.txt
 msfabricpysdkcore/tests/__init__.py
+msfabricpysdkcore/tests/test_admin_apis.py
+msfabricpysdkcore/tests/test_domains.py
 msfabricpysdkcore/tests/test_git.py
 msfabricpysdkcore/tests/test_items_incl_lakehouse.py
 msfabricpysdkcore/tests/test_jobs.py
 msfabricpysdkcore/tests/test_shortcuts.py
 msfabricpysdkcore/tests/test_workspaces_capacities.py
```

### Comparing `msfabricpysdkcore-0.0.3/pyproject.toml` & `msfabricpysdkcore-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 65.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msfabricpysdkcore"
-version = "0.0.3"
+version = "0.0.4"
 dynamic = ["dependencies"]
 authors = [
   { name="Andreas Rederer"},
 ]
 description = "A Python SDK for Microsoft Fabric"
 readme = "README.md"
 requires-python = ">=3.11"
```

