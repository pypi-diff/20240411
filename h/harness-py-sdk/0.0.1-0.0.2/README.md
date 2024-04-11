# Comparing `tmp/harness_py_sdk-0.0.1.tar.gz` & `tmp/harness_py_sdk-0.0.2.tar.gz`

## Comparing `harness_py_sdk-0.0.1.tar` & `harness_py_sdk-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,24 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.1/requirements.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.1/src/harness_py_sdk/ __init__.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.1/src/harness_py_sdk/harness_base_service.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.1/src/harness_py_sdk/harness_connectors.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.1/src/harness_py_sdk/harness_old_connectors.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.1/src/harness_py_sdk/harness_pipelines.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.1/src/harness_py_sdk/harness_services.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.1/src/harness_py_sdk/harness_templates.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.1/LICENSE
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.1/README.md
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    34745 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/docs/harness_py_sdk.html
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/docs/index.html
+-rw-r--r--   0        0        0    96377 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/docs/search.js
+-rw-r--r--   0        0        0    34733 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/docs/harness_py_sdk/ __init__.html
+-rw-r--r--   0        0        0    37520 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/docs/harness_py_sdk/harness_base_service.html
+-rw-r--r--   0        0        0    39751 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/docs/harness_py_sdk/harness_connectors.html
+-rw-r--r--   0        0        0    38088 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/docs/harness_py_sdk/harness_old_connectors.html
+-rw-r--r--   0        0        0    39703 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/docs/harness_py_sdk/harness_pipelines.html
+-rw-r--r--   0        0        0    38057 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/docs/harness_py_sdk/harness_services.html
+-rw-r--r--   0        0        0    39334 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/docs/harness_py_sdk/harness_templates.html
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/src/harness_py_sdk/ __init__.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/src/harness_py_sdk/harness_base_service.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/src/harness_py_sdk/harness_connectors.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/src/harness_py_sdk/harness_old_connectors.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/src/harness_py_sdk/harness_pipelines.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/src/harness_py_sdk/harness_services.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/src/harness_py_sdk/harness_templates.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.2/PKG-INFO
```

### Comparing `harness_py_sdk-0.0.1/src/harness_py_sdk/harness_base_service.py` & `harness_py_sdk-0.0.2/src/harness_py_sdk/harness_base_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import requests
 from harness_pipelines import HarnessPipelines
 from harness_connectors import HarnessConnectors
 from harness_services import HarnessServices
 
 class HarnessBaseService:
     def __init__(self, api_key, account_identifier):
-        self.session = requests.Session()
-        self.session.   headers.update({
+        self._session = requests.Session()
+        self._session.   headers.update({
             'x-api-key': api_key,
             'Harness-Account': account_identifier,
             'Content-Type': 'application/json'
         })
         self._account_identifier = account_identifier
-        self.base_url = "https://app.harness.io"
+        self._base_url = "https://app.harness.io"
         self._pipelines = None  # Placeholder for the Pipelines class
         self._connectors = None  # Placeholder for the Connectors class
         self._services = None  # Placeholder for the Services class
 
     @property
     def pipelines(self):
         if self._pipelines is None:
@@ -32,23 +32,23 @@
     @property
     def connectors(self):
         if self._connectors is None:
             self._connectors = HarnessConnectors(self)  # Initialize with self to pass the session
         return self._connectors
 
     def _make_request(self, method, endpoint, **kwargs):
-        url = f"{self.base_url}{endpoint}"
-        response = self.session.request(method, url, **kwargs)
+        url = f"{self._base_url}{endpoint}"
+        response = self._session.request(method, url, **kwargs)
         if response.ok:
             return response.json()
         print(response.text)
         response.raise_for_status()
     
     # Build the url dynamically for the new beta API
-    def construct_url(self, entity, identifier=None, org_identifier=None, project_identifier=None):
+    def _construct_url(self, entity, identifier=None, org_identifier=None, project_identifier=None):
         parts = ["/v1"]
 
         if org_identifier:
             parts.extend(["orgs", org_identifier])
             if project_identifier:
                 parts.extend(["projects", project_identifier])
```

### Comparing `harness_py_sdk-0.0.1/src/harness_py_sdk/harness_old_connectors.py` & `harness_py_sdk-0.0.2/src/harness_py_sdk/harness_old_connectors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 class HarnessOldConnectors():
     def __init__(self, harness_service):
-        self.harness_service = harness_service
+        self._harness_service = harness_service
     
     def fetch_connectors_listV2(self, data, org_identifier=None, project_identifier=None):
         endpoint = "/ng/api/connectors/listV2"
         query_params = {
-            "accountIdentifier": self.harness_service._account_identifier,
+            "accountIdentifier": self._harness_service._account_identifier,
         }
 
         if org_identifier:
             query_params["orgIdentifier"] = org_identifier
         
         if project_identifier:
             query_params["projectIdentifier"] = project_identifier
 
-        return self.harness_service._make_request("POST", endpoint, params = query_params, json = data)
+        return self._harness_service._make_request("POST", endpoint, params = query_params, json = data)
     
     def update_connector(self, data, org_identifier=None, project_identifier=None):
         endpoint = "/ng/api/connectors"
         query_params = {
-            "accountIdentifier": self.harness_service._account_identifier,
+            "accountIdentifier": self._harness_service._account_identifier,
         }
 
         if org_identifier:
             query_params["orgIdentifier"] = org_identifier
         
         if project_identifier:
             query_params["projectIdentifier"] = project_identifier
 
-        return self.harness_service._make_request("PUT", endpoint, params = query_params, json = data)
+        return self._harness_service._make_request("PUT", endpoint, params = query_params, json = data)
```

### Comparing `harness_py_sdk-0.0.1/src/harness_py_sdk/harness_pipelines.py` & `harness_py_sdk-0.0.2/src/harness_py_sdk/harness_pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 class HarnessPipelines:
     def __init__(self, harness_service):
-        self.harness_service = harness_service
+        self._harness_service = harness_service
 
     def fetch_pipeline_yaml(self, org_identifier, project_identifier, pipeline_identifier):
         endpoint = f"/v1/orgs/{org_identifier}/projects/{project_identifier}/pipelines/{pipeline_identifier}"
-        return self.harness_service._make_request("GET", endpoint)
+        return self._harness_service._make_request("GET", endpoint)
     
     def create_pipeline(self, org_identifier, project_identifier, pipeline_data):
         endpoint = f"/v1/orgs/{org_identifier}/projects/{project_identifier}/pipelines"
-        return self.harness_service._make_request("POST", endpoint, json=pipeline_data)
+        return self._harness_service._make_request("POST", endpoint, json=pipeline_data)
     
     def update_pipeline(self, org_identifier, project_identifier, pipeline_data, pipeline_identifier):
         endpoint = f"/v1/orgs/{org_identifier}/projects/{project_identifier}/pipelines/{pipeline_identifier}"
-        return self.harness_service._make_request("PUT", endpoint, json=pipeline_data)
+        return self._harness_service._make_request("PUT", endpoint, json=pipeline_data)
     
     def delete_pipeline(self, org_identifier, project_identifier, pipeline_identifier):
         endpoint = f"/v1/orgs/{org_identifier}/projects/{project_identifier}/pipelines/{pipeline_identifier}"
-        return self.harness_service._make_request("DELETE", endpoint)
+        return self._harness_service._make_request("DELETE", endpoint)
```

### Comparing `harness_py_sdk-0.0.1/src/harness_py_sdk/harness_services.py` & `harness_py_sdk-0.0.2/src/harness_py_sdk/harness_services.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 class HarnessServices():
     def __init__(self, harness_service):
-        self.harness_service = harness_service
+        self._harness_service = harness_service
     
     def fetch_services(self, params = None, org_identifier=None, project_identifier=None):
-        endpoint = self.harness_service.construct_url("services", None, org_identifier, project_identifier)
-        return self.harness_service._make_request("GET", endpoint, params = params)
+        endpoint = self._harness_service._construct_url("services", None, org_identifier, project_identifier)
+        return self._harness_service._make_request("GET", endpoint, params = params)
     
     def update_service(self, identifier, data, org_identifier=None, project_identifier=None):
-        endpoint = self.harness_service.construct_url("services", identifier, org_identifier, project_identifier)
-        return self.harness_service._make_request("PUT", endpoint, json=data)
+        endpoint = self._harness_service._construct_url("services", identifier, org_identifier, project_identifier)
+        return self._harness_service._make_request("PUT", endpoint, json=data)
```

### Comparing `harness_py_sdk-0.0.1/src/harness_py_sdk/harness_templates.py` & `harness_py_sdk-0.0.2/src/harness_py_sdk/harness_templates.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from harness_base_service import HarnessService
+from harness_base_service import HarnessBaseService
 
-class HarnessTemplates(HarnessService):
+class HarnessTemplates(HarnessBaseService):
     def fetch_template_yaml(self, template_identifier, version, org_identifier=None, project_identifier=None):
-        endpoint = self.construct_url(template_identifier, "templates", org_identifier, project_identifier) + f"/versions/{version}"
+        endpoint = self._construct_url(template_identifier, "templates", org_identifier, project_identifier) + f"/versions/{version}"
         return self._make_request("GET", endpoint)
     
     def fetch_stable_template_yaml(self, template_identifier, org_identifier=None, project_identifier=None):
-        return self._make_request("GET", self.construct_url(template_identifier, "templates", org_identifier, project_identifier))
+        return self._make_request("GET", self._construct_url(template_identifier, "templates", org_identifier, project_identifier))
     
     def create_template_pipeline(self, template_data, org_identifier=None, project_identifier=None):
         return self._make_request(
             "POST", 
-            self.construct_url(entity = "templates", org_identifier = org_identifier, project_identifier = project_identifier), 
+            self._construct_url(entity = "templates", org_identifier = org_identifier, project_identifier = project_identifier), 
             json=template_data
         )
```

### Comparing `harness_py_sdk-0.0.1/LICENSE` & `harness_py_sdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.1/pyproject.toml` & `harness_py_sdk-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "harness-py-sdk"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Guilherme Zanini", email="guilherme.zanini@harness.io" },
 ]
 description = "This is a non-official package that leverages the Harness API using Python."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -18,8 +18,8 @@
 Issues = "https://github.com/guilhermezanini-harness/harness-py-sdk/issues"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/harness_py_sdk"]
+packages = ["src/harness_py_sdk"]
```

