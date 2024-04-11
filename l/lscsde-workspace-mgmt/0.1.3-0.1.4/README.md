# Comparing `tmp/lscsde_workspace_mgmt-0.1.3.tar.gz` & `tmp/lscsde_workspace_mgmt-0.1.4.tar.gz`

## Comparing `lscsde_workspace_mgmt-0.1.3.tar` & `lscsde_workspace_mgmt-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/.git
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/_version.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/exceptions.py
--rw-r--r--   0        0        0    17365 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/k8sio.py
--rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/managers.py
--rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/models.py
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/objects.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/.gitignore
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/LICENSE
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/README.md
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/.git
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/_version.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/exceptions.py
+-rw-r--r--   0        0        0    22688 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/k8sio.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/managers.py
+-rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/models.py
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/objects.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/LICENSE
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/README.md
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/PKG-INFO
```

### Comparing `lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/exceptions.py` & `lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/exceptions.py`

 * *Files identical despite different names*

### Comparing `lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/k8sio.py` & `lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/k8sio.py`

 * *Files 27% similar despite different names*

```diff
@@ -22,14 +22,105 @@
     V1Volume,
     V1VolumeMount,
     V1PersistentVolumeClaim,
     V1PersistentVolumeClaimSpec,
     V1PersistentVolumeClaimVolumeSource,
     V1PersistentVolumeClaimList
 )
+from os import getenv
+from datetime import datetime
+from uuid import uuid4
+from pytz import utc
+
+class EventClient:
+    def __init__(self, api_client : client.ApiClient, log : Logger, reporting_controller : str = "xlscsde.nhs.uk/undefined-controller", reporting_user = "Unknown User"):
+        self.api = client.EventsV1Api(api_client)
+        self.log = log
+        self.reporting_controller = reporting_controller
+        self.reporting_instance = getenv("HOSTNAME", getenv("COMPUTERNAME", "unknown"))
+        self.reporting_user = reporting_user
+
+    async def RegisterWorkspaceEvent(self, workspace : AnalyticsWorkspace, reason : str, note : str):
+        event_time = datetime.now(utc)
+        body = client.EventsV1Event(
+            action=reason,
+            metadata = V1ObjectMeta(
+                namespace = workspace.metadata.namespace,
+                name = f"ws-{uuid4().hex}-{workspace.metadata.resource_version}-evt"
+            ),
+            event_time = event_time,
+            reason = reason,
+            note = note,
+            reporting_controller = self.reporting_controller,
+            reporting_instance = self.reporting_instance,
+            regarding=client.V1ObjectReference(
+                api_version = workspace.api_version,
+                kind = workspace.kind,
+                namespace = workspace.metadata.namespace,
+                name = workspace.metadata.name
+            ),
+            type = "Normal"
+        )
+        await self.api.create_namespaced_event(namespace = workspace.metadata.namespace, body = body)
+    
+    async def RegisterWorkspaceBindingEvent(self, binding : AnalyticsWorkspaceBinding, reason : str, note : str):
+        event_time = datetime.now(utc)
+        body = client.EventsV1Event(
+            action=reason,
+            metadata = V1ObjectMeta(
+                namespace = binding.metadata.namespace,
+                name = f"wsb-{uuid4().hex}-{binding.metadata.resource_version}-evt"
+            ),
+            event_time = event_time,
+            reason = reason,
+            note = note,
+            reporting_controller = self.reporting_controller,
+            reporting_instance = self.reporting_instance,
+            regarding=client.V1ObjectReference(
+                api_version = binding.api_version,
+                kind = binding.kind,
+                namespace = binding.metadata.namespace,
+                name = binding.metadata.name
+            ),
+            type = "Normal"
+        )
+        await self.api.create_namespaced_event(namespace = binding.metadata.namespace, body = body)
+    
+    async def WorkspaceCreated(self, workspace : AnalyticsWorkspace, note : str = None):
+        if not note:
+            note = f"Workspace Created by {self.reporting_user}"
+
+        await self.RegisterWorkspaceEvent(workspace, "WorkspaceCreated", note)
+
+    async def WorkspaceUpdated(self, workspace : AnalyticsWorkspace, note : str = None):
+        if not note:
+            note = f"Workspace Updated by {self.reporting_user}"
+
+        await self.RegisterWorkspaceEvent(workspace, "WorkspaceUpdated", note)
+
+    async def WorkspaceDeleted(self, workspace : AnalyticsWorkspace, note : str = None):
+        if not note:
+            note = f"Workspace Deleted by {self.reporting_user}"
+
+        await self.RegisterWorkspaceEvent(workspace, "WorkspaceDeleted", note)
+
+    async def WorkspaceBindingCreated(self, binding : AnalyticsWorkspaceBinding, note : str = None):
+        if not note:
+            note = f"Workspace Binding Created by {self.reporting_user}"
+        await self.RegisterWorkspaceBindingEvent(binding, "WorkspaceBindingCreated", note)
+
+    async def WorkspaceBindingUpdated(self, binding : AnalyticsWorkspaceBinding, note : str = None):
+        if not note:
+            note = f"Workspace Binding Updated by {self.reporting_user}"
+        await self.RegisterWorkspaceBindingEvent(binding, "WorkspaceBindingUpdated", note)
+
+    async def WorkspaceBindingDeleted(self, binding : AnalyticsWorkspaceBinding, note : str = None):
+        if not note:
+            note = f"Workspace Binding Deleted by {self.reporting_user}"
+        await self.RegisterWorkspaceBindingEvent(binding, "WorkspaceBindingDeleted", note)
 
 class KubernetesNamespacedCustomClient:
     def __init__(self, k8s_api : client.CustomObjectsApi, log : Logger, group : str, version : str, plural : str, kind : str):
         self.group = group
         self.version = version
         self.plural = plural
         self.kind = kind
@@ -100,38 +191,37 @@
         return await self.api.delete_namespaced_custom_object(
             group = self.group,
             version = self.version,
             namespace = namespace,
             plural = self.plural,
             name = name
         )
+        
 
 class AnalyticsWorkspaceBindingClient(KubernetesNamespacedCustomClient):
     adaptor = TypeAdapter(AnalyticsWorkspaceBinding)
-    def __init__(self, k8s_api: client.CustomObjectsApi, log: Logger):
+    def __init__(self, k8s_api: client.CustomObjectsApi, log: Logger, event_client : EventClient):
         super().__init__(
             k8s_api = k8s_api, 
             log = log, 
             group = "xlscsde.nhs.uk",
             version = "v1",
             plural = "analyticsworkspacebindings",
             kind = "AnalyticsWorkspaceBinding"
         )
+        self.event_client = event_client
 
     async def get(self, namespace, name):
         result = await super().get(namespace, name)
-        print(result)
         return self.adaptor.validate_python(result)
     
     async def list(self, namespace, **kwargs):
         result = await super().list(namespace, **kwargs)
         return [self.adaptor.validate_python(item) for item in result["items"]]
 
-    
-
     async def list_by_username(self, namespace, username):
         helper = KubernetesHelper() 
         formatted_username = helper.format_as_label(username)
         no_label = await self.list(namespace = namespace, label_selector = f"!xlscsde.nhs.uk/username")
         for item in no_label:
             if item.spec.username:
                 try:
@@ -156,15 +246,18 @@
         if append_label:
             contents["metadata"]["labels"]["xlscsde.nhs.uk/username"] = body.spec.username_as_label()
 
         result = await super().create(
             namespace = body.metadata.namespace,
             body = contents
         )
-        return self.adaptor.validate_python(result)
+        
+        created_binding : AnalyticsWorkspaceBinding = self.adaptor.validate_python(result)
+        await self.event_client.WorkspaceBindingUpdated(created_binding)
+        return created_binding
 
     async def patch(self, namespace : str = None, name : str = None, patch_body : dict = None, body : AnalyticsWorkspaceBinding = None):
         if not patch_body:
             if not body:
                 raise InvalidParameterException("Either namespace, name and patch_body or body must be provided")
             
             spec_adapter = TypeAdapter(AnalyticsWorkspaceBindingSpec)
@@ -185,15 +278,18 @@
             name = body.metadata.name
             
         result = await super().patch(
             namespace = namespace,
             name = name,
             body = patch_body
         )
-        return self.adaptor.validate_python(result)
+        
+        updated_binding : AnalyticsWorkspaceBinding = self.adaptor.validate_python(result)
+        await self.event_client.WorkspaceBindingUpdated(updated_binding)
+        return updated_binding
 
     async def patch_status(self, namespace : str, name : str, status : AnalyticsWorkspaceBindingStatus):
         status_adapter = TypeAdapter(AnalyticsWorkspaceBindingStatus)
         body = [{"op": "replace", "path": "/status", "value": status_adapter.dump_python(status, by_alias=True)}] 
         result = await super().patch_status(
             namespace = namespace,
             name = name,
@@ -207,15 +303,17 @@
             contents["metadata"]["labels"]["xlscsde.nhs.uk/username"] = body.spec.username_as_label()
 
         result = await super().replace(
             namespace = body.metadata.namespace,
             name = body.metadata.name,
             body = contents
         )
-        return self.adaptor.validate_python(result)
+        updated_binding : AnalyticsWorkspaceBinding = self.adaptor.validate_python(result)
+        await self.event_client.WorkspaceBindingUpdated(updated_binding)
+        return updated_binding
     
     async def delete(self, body : AnalyticsWorkspaceBinding = None, namespace : str = None, name : str = None):
         if body:
             if not namespace:
                 namespace = body.metadata.namespace
             if not name:
                 name = body.metadata.name
@@ -227,31 +325,36 @@
             patch_body = [{"op": "add", "path": "/status", "value": { "statusText" : "Deleting" }}] 
             
         await super().patch_status(
             namespace = body.metadata.namespace,
             name = body.metadata.name,
             body = patch_body
         )
+
+        if body:
+            await self.event_client.WorkspaceBindingDeleted(body)
+
         return await super().delete(
             namespace = body.metadata.namespace,
             name = body.metadata.name
         )
 
 class AnalyticsWorkspaceClient(KubernetesNamespacedCustomClient):
     adaptor = TypeAdapter(AnalyticsWorkspace)
 
-    def __init__(self, k8s_api: client.CustomObjectsApi, log: Logger):
+    def __init__(self, k8s_api: client.CustomObjectsApi, log: Logger, event_client : EventClient):
         super().__init__(
             k8s_api = k8s_api, 
             log = log, 
             group = "xlscsde.nhs.uk",
             version = "v1",
             plural = "analyticsworkspaces",
             kind = "AnalyticsWorkspace"
         )
+        self.event_client = event_client
         
     async def get(self, namespace, name):
         result = await super().get(namespace, name)
         return self.adaptor.validate_python(result)
     
     async def list(self, namespace, **kwargs):
         result = await super().list(namespace, **kwargs)
@@ -278,15 +381,17 @@
         return workspaces     
             
     async def create(self, body : AnalyticsWorkspace):
         result = await super().create(
             namespace = body.metadata.namespace,
             body = self.adaptor.dump_python(body, by_alias=True)
         )
-        return self.adaptor.validate_python(result)
+        created_workspace : AnalyticsWorkspace = self.adaptor.validate_python(result)
+        await self.event_client.WorkspaceCreated(created_workspace)
+        return created_workspace
 
     async def patch(self, namespace : str = None, name : str = None, patch_body : dict = None, body : AnalyticsWorkspace = None):
         if not patch_body:
             if not body:
                 raise InvalidParameterException("Either namespace, name and patch_body or body must be provided")
             
             spec_adapter = TypeAdapter(AnalyticsWorkspaceSpec)
@@ -309,15 +414,17 @@
             
         result = await super().patch(
             namespace = namespace,
             name = name,
             body = patch_body
         )        
         
-        return self.adaptor.validate_python(result)
+        updated_workspace : AnalyticsWorkspace = self.adaptor.validate_python(result)
+        await self.event_client.WorkspaceUpdated(updated_workspace)
+        return updated_workspace
 
     async def patch_status(self, namespace : str, name : str, status : AnalyticsWorkspaceStatus):
         status_adapter = TypeAdapter(AnalyticsWorkspaceStatus)
         body = [{"op": "replace", "path": "/status", "value": status_adapter.dump_python(status, by_alias=True)}] 
         result = await super().patch_status(
             namespace = namespace,
             name = name,
@@ -350,19 +457,23 @@
             patch_body = [{"op": "add", "path": "/status", "value": { "statusText" : "Deleting" }}] 
 
         await super().patch_status(
             namespace = body.metadata.namespace,
             name = body.metadata.name,
             body = patch_body
         )
+
+        if body:
+            await self.event_client.WorkspaceDeleted(body)
+        
         return await super().delete(
             namespace = body.metadata.namespace,
             name = body.metadata.name
         )
-    
+
 class PersistentVolumeClaimClient:
     def __init__(self, api_client : client.ApiClient, log : Logger):
         self.api = client.CoreV1Api(api_client)
         self.log = log
         
     async def get(self, name: str, namespace: str) -> V1PersistentVolumeClaim:
         self.log.info(f"Searching for PVC {name} on {namespace} exists")
```

### Comparing `lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/managers.py` & `lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/managers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .k8sio import (
     AnalyticsWorkspaceClient,
     AnalyticsWorkspaceBindingClient,
+    EventClient,
     PersistentVolumeClaimClient,
     V1ObjectMeta,
     V1Pod
 )
 
 from .objects import (
     AnalyticsWorkspace,
@@ -19,18 +20,19 @@
 from kubernetes_asyncio.client import (
     CustomObjectsApi,
     ApiClient
 )
 from logging import Logger
 
 class AnalyticsWorkspaceManager:
-    def __init__(self, api_client : ApiClient, log : Logger):
+    def __init__(self, api_client : ApiClient, log : Logger, reporting_controller : str = "xlscsde.nhs.uk/unspecified-controller", reporting_user = "Unknown User"):
         custom_objects_api = CustomObjectsApi(api_client=api_client)
-        self.workspace_client = AnalyticsWorkspaceClient(custom_objects_api, log)
-        self.binding_client = AnalyticsWorkspaceBindingClient(custom_objects_api, log)
+        self.event_client = EventClient(api_client=api_client,log = log, reporting_controller = reporting_controller, reporting_user=reporting_user)
+        self.workspace_client = AnalyticsWorkspaceClient(custom_objects_api, log, event_client=self.event_client)
+        self.binding_client = AnalyticsWorkspaceBindingClient(custom_objects_api, log, event_client=self.event_client)
         self.pvc_client = PersistentVolumeClaimClient(api_client, log)
         self.log = log
 
     async def get_workspaces_for_user(self, namespace : str, username : str):
         workspaces = await self.workspace_client.list_by_username(self.binding_client, namespace, username)
         permitted_workspaces : dict[str, AnalyticsWorkspace] = {}
         for workspace in workspaces:
```

### Comparing `lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/models.py` & `lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/models.py`

 * *Files identical despite different names*

### Comparing `lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/objects.py` & `lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/objects.py`

 * *Files identical despite different names*

### Comparing `lscsde_workspace_mgmt-0.1.3/.gitignore` & `lscsde_workspace_mgmt-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lscsde_workspace_mgmt-0.1.3/LICENSE` & `lscsde_workspace_mgmt-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lscsde_workspace_mgmt-0.1.3/pyproject.toml` & `lscsde_workspace_mgmt-0.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 ]
 description = "LSCSDE Workspace Management" 
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
   "pydantic",
   "kubernetes-asyncio",
+  "pytz",
   'importlib-metadata; python_version<"3.10"',
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `lscsde_workspace_mgmt-0.1.3/PKG-INFO` & `lscsde_workspace_mgmt-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.3
 Name: lscsde_workspace_mgmt
-Version: 0.1.3
+Version: 0.1.4
 Summary: LSCSDE Workspace Management
 Project-URL: Homepage, https://github.com/lsc-sde/py-lscsde-workspace-mgmt
 Project-URL: Issues, https://github.com/lsc-sde/py-lscsde-workspace-mgmt/issues
 Author-email: Shaun Turner <shaun.turner1@nhs.net>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: importlib-metadata; python_version < '3.10'
 Requires-Dist: kubernetes-asyncio
 Requires-Dist: pydantic
+Requires-Dist: pytz
 Description-Content-Type: text/markdown
 
 # py-lscsde-workspace-mgmt
 Python Module for LSCSDE Workspace Management
 
 ## Developer Instructions
 ### Incrementing the version
```

