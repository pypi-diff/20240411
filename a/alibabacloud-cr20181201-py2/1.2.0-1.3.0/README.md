# Comparing `tmp/alibabacloud_cr20181201_py2-1.2.0.tar.gz` & `tmp/alibabacloud_cr20181201_py2-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cr20181201_py2-1.2.0.tar", last modified: Wed Sep 27 17:10:25 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cr20181201_py2-1.3.0.tar", last modified: Thu Apr 11 06:07:03 2024, max compression
```

## Comparing `alibabacloud_cr20181201_py2-1.2.0.tar` & `alibabacloud_cr20181201_py2-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/
--rw-r--r--   0 root         (0) root         (0)       66 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2466 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1030 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1113 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/alibabacloud_cr20181201/
--rw-r--r--   0 root         (0) root         (0)       21 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/alibabacloud_cr20181201/__init__.py
--rw-r--r--   0 root         (0) root         (0)   123227 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/alibabacloud_cr20181201/client.py
--rw-r--r--   0 root         (0) root         (0)   569896 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/alibabacloud_cr20181201/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/alibabacloud_cr20181201_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2466 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/alibabacloud_cr20181201_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      432 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/alibabacloud_cr20181201_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/alibabacloud_cr20181201_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/alibabacloud_cr20181201_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/alibabacloud_cr20181201_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2898 2023-09-27 17:10:25.000000 alibabacloud_cr20181201_py2-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)      264 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2466 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1030 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   131418 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201/client.py
+-rw-r--r--   0 root         (0) root         (0)   600366 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2466 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      432 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-11 06:07:03.000000 alibabacloud_cr20181201_py2-1.3.0/setup.py
```

### Comparing `alibabacloud_cr20181201_py2-1.2.0/LICENSE` & `alibabacloud_cr20181201_py2-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cr20181201_py2-1.2.0/PKG-INFO` & `alibabacloud_cr20181201_py2-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cr20181201_py2
-Version: 1.2.0
+Version: 1.3.0
 Summary: Alibaba Cloud cr (20181201) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cr20181201_py2-1.2.0/README-CN.md` & `alibabacloud_cr20181201_py2-1.3.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cr20181201_py2-1.2.0/README.md` & `alibabacloud_cr20181201_py2-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cr20181201_py2-1.2.0/alibabacloud_cr20181201/client.py` & `alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,31 +120,38 @@
             self.call_api(params, req, runtime)
         )
 
     def change_resource_group(self, request):
         runtime = util_models.RuntimeOptions()
         return self.change_resource_group_with_options(request, runtime)
 
-    def create_artifact_build_rule_with_options(self, request, runtime):
+    def create_artifact_build_rule_with_options(self, tmp_req, runtime):
         """
-        The ID of the rule.
+        You can create building rules of accelerated images only for image repositories of Container Registry Advanced Edition instances. You cannot create building rules of accelerated images for image repositories of Container Registry Basic Edition instances. For more information, see [Specifications of different editions](https://www.alibabacloud.com/help/zh/container-registry/latest/what-is-container-registry#section-go7-lhg-qbc).
+        Accelerated images can be built in the following regions: China (Hangzhou), China (Shanghai), China (Beijing), China (Shenzhen), China (Guangzhou), China (Zhangjiakou), China (Hong Kong), US (Virginia), US (Silicon Valley), Singapore, Japan (Tokyo), and Malaysia (Kuala Lumpur).
         
 
-        @param request: CreateArtifactBuildRuleRequest
+        @param tmp_req: CreateArtifactBuildRuleRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateArtifactBuildRuleResponse
         """
-        UtilClient.validate_model(request)
+        UtilClient.validate_model(tmp_req)
+        request = cr_20181201_models.CreateArtifactBuildRuleShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.parameters):
+            request.parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.parameters, 'Parameters', 'json')
         query = {}
         if not UtilClient.is_unset(request.artifact_type):
             query['ArtifactType'] = request.artifact_type
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.parameters_shrink):
+            query['Parameters'] = request.parameters_shrink
         if not UtilClient.is_unset(request.scope_id):
             query['ScopeId'] = request.scope_id
         if not UtilClient.is_unset(request.scope_type):
             query['ScopeType'] = request.scope_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -162,15 +169,16 @@
         return TeaCore.from_map(
             cr_20181201_models.CreateArtifactBuildRuleResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_artifact_build_rule(self, request):
         """
-        The ID of the rule.
+        You can create building rules of accelerated images only for image repositories of Container Registry Advanced Edition instances. You cannot create building rules of accelerated images for image repositories of Container Registry Basic Edition instances. For more information, see [Specifications of different editions](https://www.alibabacloud.com/help/zh/container-registry/latest/what-is-container-registry#section-go7-lhg-qbc).
+        Accelerated images can be built in the following regions: China (Hangzhou), China (Shanghai), China (Beijing), China (Shenzhen), China (Guangzhou), China (Zhangjiakou), China (Hong Kong), US (Virginia), US (Silicon Valley), Singapore, Japan (Tokyo), and Malaysia (Kuala Lumpur).
         
 
         @param request: CreateArtifactBuildRuleRequest
 
         @return: CreateArtifactBuildRuleResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -384,15 +392,15 @@
 
     def create_instance_endpoint_acl_policy(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_instance_endpoint_acl_policy_with_options(request, runtime)
 
     def create_instance_vpc_endpoint_linked_vpc_with_options(self, request, runtime):
         """
-        The ID of the request.
+        A maximum of three VPCs can be associated with a Container Registry instance. If you want to associate more VPCs, contact Alibaba Cloud technical support.
         
 
         @param request: CreateInstanceVpcEndpointLinkedVpcRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateInstanceVpcEndpointLinkedVpcResponse
@@ -426,15 +434,15 @@
         return TeaCore.from_map(
             cr_20181201_models.CreateInstanceVpcEndpointLinkedVpcResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_instance_vpc_endpoint_linked_vpc(self, request):
         """
-        The ID of the request.
+        A maximum of three VPCs can be associated with a Container Registry instance. If you want to associate more VPCs, contact Alibaba Cloud technical support.
         
 
         @param request: CreateInstanceVpcEndpointLinkedVpcRequest
 
         @return: CreateInstanceVpcEndpointLinkedVpcResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -2313,14 +2321,16 @@
     def list_instance_endpoint_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.module_name):
             query['ModuleName'] = request.module_name
+        if not UtilClient.is_unset(request.summary):
+            query['Summary'] = request.summary
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListInstanceEndpoint',
             version='2018-12-01',
             protocol='HTTPS',
@@ -2732,14 +2742,102 @@
             self.call_api(params, req, runtime)
         )
 
     def list_repository(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_repository_with_options(request, runtime)
 
+    def list_scan_baseline_by_task_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListScanBaselineByTask',
+            version='2018-12-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cr_20181201_models.ListScanBaselineByTaskResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def list_scan_baseline_by_task(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_scan_baseline_by_task_with_options(request, runtime)
+
+    def list_scan_malicious_file_by_task_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListScanMaliciousFileByTask',
+            version='2018-12-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cr_20181201_models.ListScanMaliciousFileByTaskResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def list_scan_malicious_file_by_task(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_scan_malicious_file_by_task_with_options(request, runtime)
+
+    def list_tag_resources_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListTagResources',
+            version='2018-12-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cr_20181201_models.ListTagResourcesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def list_tag_resources(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_tag_resources_with_options(request, runtime)
+
     def reset_login_password_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.password):
             query['Password'] = request.password
@@ -2762,14 +2860,84 @@
             self.call_api(params, req, runtime)
         )
 
     def reset_login_password(self, request):
         runtime = util_models.RuntimeOptions()
         return self.reset_login_password_with_options(request, runtime)
 
+    def tag_resources_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='TagResources',
+            version='2018-12-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cr_20181201_models.TagResourcesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def tag_resources(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.tag_resources_with_options(request, runtime)
+
+    def untag_resources_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.all):
+            query['All'] = request.all
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag_key):
+            query['TagKey'] = request.tag_key
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UntagResources',
+            version='2018-12-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cr_20181201_models.UntagResourcesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def untag_resources(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.untag_resources_with_options(request, runtime)
+
     def update_chain_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.chain_config):
             query['ChainConfig'] = request.chain_config
         if not UtilClient.is_unset(request.chain_id):
             query['ChainId'] = request.chain_id
```

### Comparing `alibabacloud_cr20181201_py2-1.2.0/alibabacloud_cr20181201/models.py` & `alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,14 @@
 class CancelArtifactBuildTaskResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CancelArtifactBuildTaskResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CancelArtifactBuildTaskResponse, self).to_map()
         if _map is not None:
             return _map
@@ -190,17 +187,14 @@
 class CancelRepoBuildRecordResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CancelRepoBuildRecordResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CancelRepoBuildRecordResponse, self).to_map()
         if _map is not None:
             return _map
@@ -224,17 +218,19 @@
             temp_model = CancelRepoBuildRecordResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ChangeResourceGroupRequest(TeaModel):
     def __init__(self, resource_group_id=None, resource_id=None, resource_region_id=None):
+        # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
         # Id of the request
         self.resource_id = resource_id  # type: str
+        # The region ID of the resource group.
         self.resource_region_id = resource_region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ChangeResourceGroupRequest, self).to_map()
@@ -259,14 +255,15 @@
         if m.get('ResourceRegionId') is not None:
             self.resource_region_id = m.get('ResourceRegionId')
         return self
 
 
 class ChangeResourceGroupResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ChangeResourceGroupResponseBody, self).to_map()
@@ -288,17 +285,14 @@
 class ChangeResourceGroupResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ChangeResourceGroupResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ChangeResourceGroupResponse, self).to_map()
         if _map is not None:
             return _map
@@ -321,18 +315,30 @@
         if m.get('body') is not None:
             temp_model = ChangeResourceGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateArtifactBuildRuleRequest(TeaModel):
-    def __init__(self, artifact_type=None, instance_id=None, scope_id=None, scope_type=None):
+    def __init__(self, artifact_type=None, instance_id=None, parameters=None, scope_id=None, scope_type=None):
+        # The type of the artifact.
+        # 
+        # *   `ACCELERATED_IMAGE`: accelerated images.
         self.artifact_type = artifact_type  # type: str
+        # The instance ID.
         self.instance_id = instance_id  # type: str
+        # Additional parameters.
+        self.parameters = parameters  # type: dict[str, any]
+        # The ID of the effective range of the rule.
+        # 
+        # *   Set the value to the ID of the image repository.
         self.scope_id = scope_id  # type: str
+        # The effective range of the rule. Valid values:
+        # 
+        # *   `REPOSITORY`
         self.scope_type = scope_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateArtifactBuildRuleRequest, self).to_map()
@@ -340,38 +346,101 @@
             return _map
 
         result = dict()
         if self.artifact_type is not None:
             result['ArtifactType'] = self.artifact_type
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
+        if self.parameters is not None:
+            result['Parameters'] = self.parameters
+        if self.scope_id is not None:
+            result['ScopeId'] = self.scope_id
+        if self.scope_type is not None:
+            result['ScopeType'] = self.scope_type
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ArtifactType') is not None:
+            self.artifact_type = m.get('ArtifactType')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('Parameters') is not None:
+            self.parameters = m.get('Parameters')
+        if m.get('ScopeId') is not None:
+            self.scope_id = m.get('ScopeId')
+        if m.get('ScopeType') is not None:
+            self.scope_type = m.get('ScopeType')
+        return self
+
+
+class CreateArtifactBuildRuleShrinkRequest(TeaModel):
+    def __init__(self, artifact_type=None, instance_id=None, parameters_shrink=None, scope_id=None, scope_type=None):
+        # The type of the artifact.
+        # 
+        # *   `ACCELERATED_IMAGE`: accelerated images.
+        self.artifact_type = artifact_type  # type: str
+        # The instance ID.
+        self.instance_id = instance_id  # type: str
+        # Additional parameters.
+        self.parameters_shrink = parameters_shrink  # type: str
+        # The ID of the effective range of the rule.
+        # 
+        # *   Set the value to the ID of the image repository.
+        self.scope_id = scope_id  # type: str
+        # The effective range of the rule. Valid values:
+        # 
+        # *   `REPOSITORY`
+        self.scope_type = scope_type  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateArtifactBuildRuleShrinkRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.artifact_type is not None:
+            result['ArtifactType'] = self.artifact_type
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.parameters_shrink is not None:
+            result['Parameters'] = self.parameters_shrink
         if self.scope_id is not None:
             result['ScopeId'] = self.scope_id
         if self.scope_type is not None:
             result['ScopeType'] = self.scope_type
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ArtifactType') is not None:
             self.artifact_type = m.get('ArtifactType')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
+        if m.get('Parameters') is not None:
+            self.parameters_shrink = m.get('Parameters')
         if m.get('ScopeId') is not None:
             self.scope_id = m.get('ScopeId')
         if m.get('ScopeType') is not None:
             self.scope_type = m.get('ScopeType')
         return self
 
 
 class CreateArtifactBuildRuleResponseBody(TeaModel):
     def __init__(self, build_rule_id=None, code=None, is_success=None, request_id=None):
+        # The ID of the accelerated image building rule.
         self.build_rule_id = build_rule_id  # type: str
+        # The return value.
         self.code = code  # type: str
+        # Indicates whether the request is successful.
         self.is_success = is_success  # type: bool
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateArtifactBuildRuleResponseBody, self).to_map()
@@ -405,17 +474,14 @@
 class CreateArtifactBuildRuleResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateArtifactBuildRuleResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateArtifactBuildRuleResponse, self).to_map()
         if _map is not None:
             return _map
@@ -517,17 +583,14 @@
 class CreateBuildRecordByRecordResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateBuildRecordByRecordResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateBuildRecordByRecordResponse, self).to_map()
         if _map is not None:
             return _map
@@ -636,17 +699,14 @@
 class CreateBuildRecordByRuleResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateBuildRecordByRuleResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateBuildRecordByRuleResponse, self).to_map()
         if _map is not None:
             return _map
@@ -780,17 +840,14 @@
 class CreateChainResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateChainResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateChainResponse, self).to_map()
         if _map is not None:
             return _map
@@ -909,17 +966,14 @@
 class CreateChartNamespaceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateChartNamespaceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateChartNamespaceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1048,17 +1102,14 @@
 class CreateChartRepositoryResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateChartRepositoryResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateChartRepositoryResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1179,17 +1230,14 @@
 class CreateInstanceEndpointAclPolicyResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateInstanceEndpointAclPolicyResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateInstanceEndpointAclPolicyResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1214,18 +1262,31 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateInstanceVpcEndpointLinkedVpcRequest(TeaModel):
     def __init__(self, enable_create_dnsrecord_in_pvzt=None, instance_id=None, module_name=None, vpc_id=None,
                  vswitch_id=None):
+        # Specifies whether to automatically create Alibaba Cloud DNS PrivateZone records. Valid values:
+        # 
+        # >  If you enable automatic creation of PrivateZone records, a PrivateZone record is automatically created when you associate a VPC with the instance.
+        # 
+        # *   `true`
+        # *   `false`
         self.enable_create_dnsrecord_in_pvzt = enable_create_dnsrecord_in_pvzt  # type: bool
+        # The instance ID.
         self.instance_id = instance_id  # type: str
+        # The name of the module that you want to access. Valid values:
+        # 
+        # *   `Registry`: image repositories.
+        # *   `Chart`: Helm charts.
         self.module_name = module_name  # type: str
+        # The VPC ID.
         self.vpc_id = vpc_id  # type: str
+        # The ID of the vSwitch that is associated with the specified VPC.
         self.vswitch_id = vswitch_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateInstanceVpcEndpointLinkedVpcRequest, self).to_map()
@@ -1258,16 +1319,22 @@
         if m.get('VswitchId') is not None:
             self.vswitch_id = m.get('VswitchId')
         return self
 
 
 class CreateInstanceVpcEndpointLinkedVpcResponseBody(TeaModel):
     def __init__(self, code=None, is_success=None, request_id=None):
+        # The return value.
         self.code = code  # type: str
+        # Indicates whether the request is successful.
+        # 
+        # *   `true`: The request is successful.
+        # *   `false`: The request fails.
         self.is_success = is_success  # type: bool
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateInstanceVpcEndpointLinkedVpcResponseBody, self).to_map()
@@ -1297,17 +1364,14 @@
 class CreateInstanceVpcEndpointLinkedVpcResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateInstanceVpcEndpointLinkedVpcResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateInstanceVpcEndpointLinkedVpcResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1419,17 +1483,14 @@
 class CreateNamespaceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateNamespaceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateNamespaceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1589,17 +1650,14 @@
 class CreateRepoBuildRuleResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateRepoBuildRuleResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateRepoBuildRuleResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1742,17 +1800,14 @@
 class CreateRepoSourceCodeRepoResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateRepoSourceCodeRepoResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateRepoSourceCodeRepoResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1901,17 +1956,14 @@
 class CreateRepoSyncRuleResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateRepoSyncRuleResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateRepoSyncRuleResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2049,17 +2101,14 @@
 class CreateRepoSyncTaskResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateRepoSyncTaskResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateRepoSyncTaskResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2177,17 +2226,14 @@
 class CreateRepoSyncTaskByRuleResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateRepoSyncTaskByRuleResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateRepoSyncTaskByRuleResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2302,17 +2348,14 @@
 class CreateRepoTagResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateRepoTagResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateRepoTagResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2433,17 +2476,14 @@
 class CreateRepoTagScanTaskResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateRepoTagScanTaskResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateRepoTagScanTaskResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2582,17 +2622,14 @@
 class CreateRepoTriggerResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateRepoTriggerResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateRepoTriggerResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2732,17 +2769,14 @@
 class CreateRepositoryResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateRepositoryResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateRepositoryResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2839,17 +2873,14 @@
 class DeleteChainResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteChainResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteChainResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2949,17 +2980,14 @@
 class DeleteChartNamespaceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteChartNamespaceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteChartNamespaceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -3074,17 +3102,14 @@
 class DeleteChartReleaseResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteChartReleaseResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteChartReleaseResponse, self).to_map()
         if _map is not None:
             return _map
@@ -3190,17 +3215,14 @@
 class DeleteChartRepositoryResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteChartRepositoryResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteChartRepositoryResponse, self).to_map()
         if _map is not None:
             return _map
@@ -3291,17 +3313,14 @@
 class DeleteEventCenterRuleResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteEventCenterRuleResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteEventCenterRuleResponse, self).to_map()
         if _map is not None:
             return _map
@@ -3416,17 +3435,14 @@
 class DeleteInstanceEndpointAclPolicyResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteInstanceEndpointAclPolicyResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteInstanceEndpointAclPolicyResponse, self).to_map()
         if _map is not None:
             return _map
@@ -3541,17 +3557,14 @@
 class DeleteInstanceVpcEndpointLinkedVpcResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteInstanceVpcEndpointLinkedVpcResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteInstanceVpcEndpointLinkedVpcResponse, self).to_map()
         if _map is not None:
             return _map
@@ -3648,17 +3661,14 @@
 class DeleteNamespaceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteNamespaceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteNamespaceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -3761,17 +3771,14 @@
 class DeleteRepoBuildRuleResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteRepoBuildRuleResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteRepoBuildRuleResponse, self).to_map()
         if _map is not None:
             return _map
@@ -3868,17 +3875,14 @@
 class DeleteRepoSyncRuleResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteRepoSyncRuleResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteRepoSyncRuleResponse, self).to_map()
         if _map is not None:
             return _map
@@ -3981,17 +3985,14 @@
 class DeleteRepoTagResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteRepoTagResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteRepoTagResponse, self).to_map()
         if _map is not None:
             return _map
@@ -4097,17 +4098,14 @@
 class DeleteRepoTriggerResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteRepoTriggerResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteRepoTriggerResponse, self).to_map()
         if _map is not None:
             return _map
@@ -4135,15 +4133,17 @@
 
 class DeleteRepositoryRequest(TeaModel):
     def __init__(self, instance_id=None, repo_id=None, repo_name=None, repo_namespace_name=None):
         # The ID of the instance.
         self.instance_id = instance_id  # type: str
         # The ID of the image repository.
         self.repo_id = repo_id  # type: str
+        # The name of the repository.
         self.repo_name = repo_name  # type: str
+        # The name of the namespace to which the repository belongs.
         self.repo_namespace_name = repo_namespace_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteRepositoryRequest, self).to_map()
@@ -4172,22 +4172,22 @@
         if m.get('RepoNamespaceName') is not None:
             self.repo_namespace_name = m.get('RepoNamespaceName')
         return self
 
 
 class DeleteRepositoryResponseBody(TeaModel):
     def __init__(self, code=None, is_success=None, request_id=None):
-        # The return value.
+        # Return values
         self.code = code  # type: str
         # Indicates whether the request is successful. Valid values:
         # 
         # *   `true`: The request is successful.
         # *   `false`: The request fails.
         self.is_success = is_success  # type: bool
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteRepositoryResponseBody, self).to_map()
@@ -4217,17 +4217,14 @@
 class DeleteRepositoryResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteRepositoryResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteRepositoryResponse, self).to_map()
         if _map is not None:
             return _map
@@ -4293,27 +4290,53 @@
         if m.get('ScopeId') is not None:
             self.scope_id = m.get('ScopeId')
         if m.get('ScopeType') is not None:
             self.scope_type = m.get('ScopeType')
         return self
 
 
+class GetArtifactBuildRuleResponseBodyParameters(TeaModel):
+    def __init__(self, image_index_only=None):
+        self.image_index_only = image_index_only  # type: bool
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetArtifactBuildRuleResponseBodyParameters, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.image_index_only is not None:
+            result['ImageIndexOnly'] = self.image_index_only
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ImageIndexOnly') is not None:
+            self.image_index_only = m.get('ImageIndexOnly')
+        return self
+
+
 class GetArtifactBuildRuleResponseBody(TeaModel):
-    def __init__(self, artifact_type=None, build_rule_id=None, code=None, is_success=None, request_id=None,
-                 scope_id=None, scope_type=None):
+    def __init__(self, artifact_type=None, build_rule_id=None, code=None, is_success=None, parameters=None,
+                 request_id=None, scope_id=None, scope_type=None):
         self.artifact_type = artifact_type  # type: str
         self.build_rule_id = build_rule_id  # type: str
         self.code = code  # type: str
         self.is_success = is_success  # type: bool
+        self.parameters = parameters  # type: GetArtifactBuildRuleResponseBodyParameters
         self.request_id = request_id  # type: str
         self.scope_id = scope_id  # type: str
         self.scope_type = scope_type  # type: str
 
     def validate(self):
-        pass
+        if self.parameters:
+            self.parameters.validate()
 
     def to_map(self):
         _map = super(GetArtifactBuildRuleResponseBody, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -4321,14 +4344,16 @@
             result['ArtifactType'] = self.artifact_type
         if self.build_rule_id is not None:
             result['BuildRuleId'] = self.build_rule_id
         if self.code is not None:
             result['Code'] = self.code
         if self.is_success is not None:
             result['IsSuccess'] = self.is_success
+        if self.parameters is not None:
+            result['Parameters'] = self.parameters.to_map()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.scope_id is not None:
             result['ScopeId'] = self.scope_id
         if self.scope_type is not None:
             result['ScopeType'] = self.scope_type
         return result
@@ -4339,14 +4364,17 @@
             self.artifact_type = m.get('ArtifactType')
         if m.get('BuildRuleId') is not None:
             self.build_rule_id = m.get('BuildRuleId')
         if m.get('Code') is not None:
             self.code = m.get('Code')
         if m.get('IsSuccess') is not None:
             self.is_success = m.get('IsSuccess')
+        if m.get('Parameters') is not None:
+            temp_model = GetArtifactBuildRuleResponseBodyParameters()
+            self.parameters = temp_model.from_map(m['Parameters'])
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('ScopeId') is not None:
             self.scope_id = m.get('ScopeId')
         if m.get('ScopeType') is not None:
             self.scope_type = m.get('ScopeType')
         return self
@@ -4355,17 +4383,14 @@
 class GetArtifactBuildRuleResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetArtifactBuildRuleResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetArtifactBuildRuleResponse, self).to_map()
         if _map is not None:
             return _map
@@ -4598,17 +4623,14 @@
 class GetArtifactBuildTaskResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetArtifactBuildTaskResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetArtifactBuildTaskResponse, self).to_map()
         if _map is not None:
             return _map
@@ -4725,17 +4747,14 @@
 class GetAuthorizationTokenResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetAuthorizationTokenResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetAuthorizationTokenResponse, self).to_map()
         if _map is not None:
             return _map
@@ -5156,17 +5175,14 @@
 class GetChainResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetChainResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetChainResponse, self).to_map()
         if _map is not None:
             return _map
@@ -5317,17 +5333,14 @@
 class GetChartNamespaceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetChartNamespaceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetChartNamespaceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -5500,17 +5513,14 @@
 class GetChartRepositoryResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetChartRepositoryResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetChartRepositoryResponse, self).to_map()
         if _map is not None:
             return _map
@@ -5556,32 +5566,65 @@
     def from_map(self, m=None):
         m = m or dict()
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         return self
 
 
+class GetInstanceResponseBodyTags(TeaModel):
+    def __init__(self, tag_key=None, tag_value=None):
+        self.tag_key = tag_key  # type: str
+        self.tag_value = tag_value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetInstanceResponseBodyTags, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.tag_key is not None:
+            result['TagKey'] = self.tag_key
+        if self.tag_value is not None:
+            result['TagValue'] = self.tag_value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        if m.get('TagValue') is not None:
+            self.tag_value = m.get('TagValue')
+        return self
+
+
 class GetInstanceResponseBody(TeaModel):
     def __init__(self, code=None, create_time=None, instance_id=None, instance_issue=None, instance_name=None,
                  instance_specification=None, instance_status=None, is_success=None, modified_time=None, request_id=None,
-                 resource_group_id=None):
+                 resource_group_id=None, tags=None):
         self.code = code  # type: str
         self.create_time = create_time  # type: long
         self.instance_id = instance_id  # type: str
         self.instance_issue = instance_issue  # type: str
         self.instance_name = instance_name  # type: str
         self.instance_specification = instance_specification  # type: str
         self.instance_status = instance_status  # type: str
         self.is_success = is_success  # type: bool
         self.modified_time = modified_time  # type: long
         self.request_id = request_id  # type: str
         self.resource_group_id = resource_group_id  # type: str
+        self.tags = tags  # type: list[GetInstanceResponseBodyTags]
 
     def validate(self):
-        pass
+        if self.tags:
+            for k in self.tags:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super(GetInstanceResponseBody, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -5603,14 +5646,18 @@
             result['IsSuccess'] = self.is_success
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
+        result['Tags'] = []
+        if self.tags is not None:
+            for k in self.tags:
+                result['Tags'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
         if m.get('CreateTime') is not None:
@@ -5629,27 +5676,29 @@
             self.is_success = m.get('IsSuccess')
         if m.get('ModifiedTime') is not None:
             self.modified_time = m.get('ModifiedTime')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
+        self.tags = []
+        if m.get('Tags') is not None:
+            for k in m.get('Tags'):
+                temp_model = GetInstanceResponseBodyTags()
+                self.tags.append(temp_model.from_map(k))
         return self
 
 
 class GetInstanceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetInstanceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetInstanceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -5717,17 +5766,14 @@
 class GetInstanceCountResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetInstanceCountResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetInstanceCountResponse, self).to_map()
         if _map is not None:
             return _map
@@ -5946,17 +5992,14 @@
 class GetInstanceEndpointResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetInstanceEndpointResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetInstanceEndpointResponse, self).to_map()
         if _map is not None:
             return _map
@@ -6100,17 +6143,14 @@
 class GetInstanceUsageResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetInstanceUsageResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetInstanceUsageResponse, self).to_map()
         if _map is not None:
             return _map
@@ -6299,17 +6339,14 @@
 class GetInstanceVpcEndpointResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetInstanceVpcEndpointResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetInstanceVpcEndpointResponse, self).to_map()
         if _map is not None:
             return _map
@@ -6457,17 +6494,14 @@
 class GetNamespaceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetNamespaceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetNamespaceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -6634,17 +6668,14 @@
 class GetRepoBuildRecordResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetRepoBuildRecordResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetRepoBuildRecordResponse, self).to_map()
         if _map is not None:
             return _map
@@ -6753,17 +6784,14 @@
 class GetRepoBuildRecordStatusResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetRepoBuildRecordStatusResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetRepoBuildRecordStatusResponse, self).to_map()
         if _map is not None:
             return _map
@@ -6922,17 +6950,14 @@
 class GetRepoSourceCodeRepoResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetRepoSourceCodeRepoResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetRepoSourceCodeRepoResponse, self).to_map()
         if _map is not None:
             return _map
@@ -7274,17 +7299,14 @@
 class GetRepoSyncTaskResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetRepoSyncTaskResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetRepoSyncTaskResponse, self).to_map()
         if _map is not None:
             return _map
@@ -7432,17 +7454,14 @@
 class GetRepoTagResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetRepoTagResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetRepoTagResponse, self).to_map()
         if _map is not None:
             return _map
@@ -7617,17 +7636,14 @@
 class GetRepoTagLayersResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetRepoTagLayersResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetRepoTagLayersResponse, self).to_map()
         if _map is not None:
             return _map
@@ -8023,17 +8039,14 @@
 class GetRepoTagManifestResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetRepoTagManifestResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetRepoTagManifestResponse, self).to_map()
         if _map is not None:
             return _map
@@ -8150,17 +8163,14 @@
 class GetRepoTagScanStatusResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetRepoTagScanStatusResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetRepoTagScanStatusResponse, self).to_map()
         if _map is not None:
             return _map
@@ -8308,17 +8318,14 @@
 class GetRepoTagScanSummaryResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetRepoTagScanSummaryResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetRepoTagScanSummaryResponse, self).to_map()
         if _map is not None:
             return _map
@@ -8515,17 +8522,14 @@
 class GetRepositoryResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetRepositoryResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetRepositoryResponse, self).to_map()
         if _map is not None:
             return _map
@@ -8688,17 +8692,14 @@
 class ListArtifactBuildTaskLogResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListArtifactBuildTaskLogResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListArtifactBuildTaskLogResponse, self).to_map()
         if _map is not None:
             return _map
@@ -8920,17 +8921,14 @@
 class ListChainResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListChainResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListChainResponse, self).to_map()
         if _map is not None:
             return _map
@@ -9201,17 +9199,14 @@
 class ListChainInstanceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListChainInstanceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListChainInstanceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -9429,17 +9424,14 @@
 class ListChartNamespaceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListChartNamespaceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListChartNamespaceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -9656,17 +9648,14 @@
 class ListChartReleaseResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListChartReleaseResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListChartReleaseResponse, self).to_map()
         if _map is not None:
             return _map
@@ -9911,17 +9900,14 @@
 class ListChartRepositoryResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListChartRepositoryResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListChartRepositoryResponse, self).to_map()
         if _map is not None:
             return _map
@@ -9944,29 +9930,32 @@
         if m.get('body') is not None:
             temp_model = ListChartRepositoryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListEventCenterRecordRequest(TeaModel):
-    def __init__(self, event_type=None, instance_id=None, page_no=None, page_size=None, rule_id=None):
+    def __init__(self, event_type=None, instance_id=None, page_no=None, page_size=None, repo_name=None,
+                 repo_namespace_name=None, rule_id=None):
         # The type of the event. Valid values:
         # 
         # *   `cr:Artifact:DeliveryChainCompleted`: The delivery chain is processed.
         # *   `cr:Artifact:SynchronizationCompleted`: The image is replicated.
         # *   `cr:Artifact:BuildCompleted`: The image is built.
         # *   `cr:Artifact:ScanCompleted`: The image is scanned.
         # *   `cr:Artifact:SigningCompleted`: The image is signed.
         self.event_type = event_type  # type: str
         # The ID of the instance.
         self.instance_id = instance_id  # type: str
         # The number of the page to return.
         self.page_no = page_no  # type: int
         # The number of entries to return on each page.
         self.page_size = page_size  # type: int
+        self.repo_name = repo_name  # type: str
+        self.repo_namespace_name = repo_namespace_name  # type: str
         # The ID of the event notification rule.
         self.rule_id = rule_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -9979,28 +9968,36 @@
             result['EventType'] = self.event_type
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.page_no is not None:
             result['PageNo'] = self.page_no
         if self.page_size is not None:
             result['PageSize'] = self.page_size
+        if self.repo_name is not None:
+            result['RepoName'] = self.repo_name
+        if self.repo_namespace_name is not None:
+            result['RepoNamespaceName'] = self.repo_namespace_name
         if self.rule_id is not None:
             result['RuleId'] = self.rule_id
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('EventType') is not None:
             self.event_type = m.get('EventType')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('PageNo') is not None:
             self.page_no = m.get('PageNo')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
+        if m.get('RepoName') is not None:
+            self.repo_name = m.get('RepoName')
+        if m.get('RepoNamespaceName') is not None:
+            self.repo_namespace_name = m.get('RepoNamespaceName')
         if m.get('RuleId') is not None:
             self.rule_id = m.get('RuleId')
         return self
 
 
 class ListEventCenterRecordResponseBodyRecords(TeaModel):
     def __init__(self, create_time=None, event_channel=None, event_notify_id=None, event_notify_method=None,
@@ -10178,17 +10175,14 @@
 class ListEventCenterRecordResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListEventCenterRecordResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListEventCenterRecordResponse, self).to_map()
         if _map is not None:
             return _map
@@ -10324,17 +10318,14 @@
 class ListEventCenterRuleNameResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListEventCenterRuleNameResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListEventCenterRuleNameResponse, self).to_map()
         if _map is not None:
             return _map
@@ -10359,18 +10350,32 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListInstanceRequest(TeaModel):
     def __init__(self, instance_name=None, instance_status=None, page_no=None, page_size=None,
                  resource_group_id=None):
+        # The instance name.
         self.instance_name = instance_name  # type: str
+        # The status of the instance. Valid values:
+        # 
+        # *   `PENDING`: The instance is being initialized.
+        # *   `INIT_ERROR`: The initialization of the instance fails.
+        # *   `STARTING`: The instance is being started.
+        # *   `RUNNING`: The instance is running.
+        # *   `STOPPING`: The instance is being stopped.
+        # *   `STOPPED`: The instance is stopped.
+        # *   `DELETING`: The instance is being deleted.
+        # *   `DELETED`: The instance is deleted.
         self.instance_status = instance_status  # type: str
+        # The page number.
         self.page_no = page_no  # type: int
+        # The number of entries per page.
         self.page_size = page_size  # type: int
+        # The ID of the resource group to which the instance belongs.
         self.resource_group_id = resource_group_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListInstanceRequest, self).to_map()
@@ -10401,29 +10406,71 @@
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         return self
 
 
+class ListInstanceResponseBodyInstancesTags(TeaModel):
+    def __init__(self, tag_key=None, tag_value=None):
+        self.tag_key = tag_key  # type: str
+        self.tag_value = tag_value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListInstanceResponseBodyInstancesTags, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.tag_key is not None:
+            result['TagKey'] = self.tag_key
+        if self.tag_value is not None:
+            result['TagValue'] = self.tag_value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        if m.get('TagValue') is not None:
+            self.tag_value = m.get('TagValue')
+        return self
+
+
 class ListInstanceResponseBodyInstances(TeaModel):
     def __init__(self, create_time=None, instance_id=None, instance_issue=None, instance_name=None,
-                 instance_specification=None, instance_status=None, modified_time=None, region_id=None, resource_group_id=None):
+                 instance_specification=None, instance_status=None, modified_time=None, region_id=None, resource_group_id=None, tags=None):
+        # The time when the instance was created.
         self.create_time = create_time  # type: str
+        # The instance ID.
         self.instance_id = instance_id  # type: str
+        # The issue occurs on the instance.
         self.instance_issue = instance_issue  # type: str
+        # The name of the instance.
         self.instance_name = instance_name  # type: str
+        # The edition of the Container Registry Enterprise Edition instance.
         self.instance_specification = instance_specification  # type: str
+        # The status of the instance.
         self.instance_status = instance_status  # type: str
+        # The time when the instance was last modified.
         self.modified_time = modified_time  # type: str
+        # The region ID of the instance.
         self.region_id = region_id  # type: str
+        # The ID of the resource group to which the instance belongs.
         self.resource_group_id = resource_group_id  # type: str
+        self.tags = tags  # type: list[ListInstanceResponseBodyInstancesTags]
 
     def validate(self):
-        pass
+        if self.tags:
+            for k in self.tags:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super(ListInstanceResponseBodyInstances, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -10441,14 +10488,18 @@
             result['InstanceStatus'] = self.instance_status
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
+        result['Tags'] = []
+        if self.tags is not None:
+            for k in self.tags:
+                result['Tags'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('InstanceId') is not None:
@@ -10463,26 +10514,38 @@
             self.instance_status = m.get('InstanceStatus')
         if m.get('ModifiedTime') is not None:
             self.modified_time = m.get('ModifiedTime')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
+        self.tags = []
+        if m.get('Tags') is not None:
+            for k in m.get('Tags'):
+                temp_model = ListInstanceResponseBodyInstancesTags()
+                self.tags.append(temp_model.from_map(k))
         return self
 
 
 class ListInstanceResponseBody(TeaModel):
     def __init__(self, code=None, instances=None, is_success=None, page_no=None, page_size=None, request_id=None,
                  total_count=None):
+        # The return value.
         self.code = code  # type: str
+        # The queried instances.
         self.instances = instances  # type: list[ListInstanceResponseBodyInstances]
+        # Indicates whether the request is successful.
         self.is_success = is_success  # type: bool
+        # The page number. Default value: 1.
         self.page_no = page_no  # type: int
+        # The number of entries per page. Default value: 30.
         self.page_size = page_size  # type: int
+        # The request ID.
         self.request_id = request_id  # type: str
+        # The total number of entries returned.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.instances:
             for k in self.instances:
                 if k:
                     k.validate()
@@ -10536,17 +10599,14 @@
 class ListInstanceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListInstanceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListInstanceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -10569,44 +10629,49 @@
         if m.get('body') is not None:
             temp_model = ListInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListInstanceEndpointRequest(TeaModel):
-    def __init__(self, instance_id=None, module_name=None):
+    def __init__(self, instance_id=None, module_name=None, summary=None):
         # The ID of the instance.
         self.instance_id = instance_id  # type: str
         # The name of the module that you want to access. Valid values:
         # 
         # *   `Registry`: the image repository.
         # *   `Chart`: a Helm chart.
         self.module_name = module_name  # type: str
+        self.summary = summary  # type: bool
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListInstanceEndpointRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.module_name is not None:
             result['ModuleName'] = self.module_name
+        if self.summary is not None:
+            result['Summary'] = self.summary
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('ModuleName') is not None:
             self.module_name = m.get('ModuleName')
+        if m.get('Summary') is not None:
+            self.summary = m.get('Summary')
         return self
 
 
 class ListInstanceEndpointResponseBodyEndpointsAclEntries(TeaModel):
     def __init__(self, entry=None):
         # Details about the ACL.
         self.entry = entry  # type: str
@@ -10829,17 +10894,14 @@
 class ListInstanceEndpointResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListInstanceEndpointResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListInstanceEndpointResponse, self).to_map()
         if _map is not None:
             return _map
@@ -10978,17 +11040,14 @@
 class ListInstanceRegionResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListInstanceRegionResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListInstanceRegionResponse, self).to_map()
         if _map is not None:
             return _map
@@ -11184,17 +11243,14 @@
 class ListNamespaceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListNamespaceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListNamespaceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -11433,17 +11489,14 @@
 class ListRepoBuildRecordResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListRepoBuildRecordResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListRepoBuildRecordResponse, self).to_map()
         if _map is not None:
             return _map
@@ -11622,17 +11675,14 @@
 class ListRepoBuildRecordLogResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListRepoBuildRecordLogResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListRepoBuildRecordLogResponse, self).to_map()
         if _map is not None:
             return _map
@@ -11846,17 +11896,14 @@
 class ListRepoBuildRuleResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListRepoBuildRuleResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListRepoBuildRuleResponse, self).to_map()
         if _map is not None:
             return _map
@@ -12155,17 +12202,14 @@
 class ListRepoSyncRuleResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListRepoSyncRuleResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListRepoSyncRuleResponse, self).to_map()
         if _map is not None:
             return _map
@@ -12486,17 +12530,14 @@
 class ListRepoSyncTaskResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListRepoSyncTaskResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListRepoSyncTaskResponse, self).to_map()
         if _map is not None:
             return _map
@@ -12700,17 +12741,14 @@
 class ListRepoTagResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListRepoTagResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListRepoTagResponse, self).to_map()
         if _map is not None:
             return _map
@@ -13008,17 +13046,14 @@
 class ListRepoTagScanResultResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListRepoTagScanResultResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListRepoTagScanResultResponse, self).to_map()
         if _map is not None:
             return _map
@@ -13195,17 +13230,14 @@
 class ListRepoTriggerResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListRepoTriggerResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListRepoTriggerResponse, self).to_map()
         if _map is not None:
             return _map
@@ -13428,17 +13460,14 @@
 class ListRepositoryResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListRepositoryResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListRepositoryResponse, self).to_map()
         if _map is not None:
             return _map
@@ -13460,14 +13489,714 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListRepositoryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListScanBaselineByTaskRequest(TeaModel):
+    def __init__(self, digest=None, instance_id=None, level=None, page_no=None, page_size=None, repo_id=None,
+                 scan_task_id=None, tag=None):
+        self.digest = digest  # type: str
+        self.instance_id = instance_id  # type: str
+        self.level = level  # type: str
+        self.page_no = page_no  # type: int
+        self.page_size = page_size  # type: int
+        self.repo_id = repo_id  # type: str
+        self.scan_task_id = scan_task_id  # type: str
+        self.tag = tag  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListScanBaselineByTaskRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.digest is not None:
+            result['Digest'] = self.digest
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.level is not None:
+            result['Level'] = self.level
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.repo_id is not None:
+            result['RepoId'] = self.repo_id
+        if self.scan_task_id is not None:
+            result['ScanTaskId'] = self.scan_task_id
+        if self.tag is not None:
+            result['Tag'] = self.tag
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Digest') is not None:
+            self.digest = m.get('Digest')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('Level') is not None:
+            self.level = m.get('Level')
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RepoId') is not None:
+            self.repo_id = m.get('RepoId')
+        if m.get('ScanTaskId') is not None:
+            self.scan_task_id = m.get('ScanTaskId')
+        if m.get('Tag') is not None:
+            self.tag = m.get('Tag')
+        return self
+
+
+class ListScanBaselineByTaskResponseBodyScanBaselines(TeaModel):
+    def __init__(self, baseline_class_alias=None, baseline_detail_advice=None, baseline_detail_description=None,
+                 baseline_detail_prompt=None, baseline_item_count=None, baseline_name_alias=None, baseline_name_key=None,
+                 baseline_name_level=None, create_time=None, first_scan_time=None, high_risk_item_count=None, low_risk_item_count=None,
+                 middle_risk_item_count=None, scan_task_id=None, update_time=None):
+        self.baseline_class_alias = baseline_class_alias  # type: str
+        self.baseline_detail_advice = baseline_detail_advice  # type: str
+        self.baseline_detail_description = baseline_detail_description  # type: str
+        self.baseline_detail_prompt = baseline_detail_prompt  # type: str
+        self.baseline_item_count = baseline_item_count  # type: int
+        self.baseline_name_alias = baseline_name_alias  # type: str
+        self.baseline_name_key = baseline_name_key  # type: str
+        self.baseline_name_level = baseline_name_level  # type: str
+        self.create_time = create_time  # type: long
+        self.first_scan_time = first_scan_time  # type: long
+        self.high_risk_item_count = high_risk_item_count  # type: int
+        self.low_risk_item_count = low_risk_item_count  # type: int
+        self.middle_risk_item_count = middle_risk_item_count  # type: int
+        self.scan_task_id = scan_task_id  # type: str
+        self.update_time = update_time  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListScanBaselineByTaskResponseBodyScanBaselines, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.baseline_class_alias is not None:
+            result['BaselineClassAlias'] = self.baseline_class_alias
+        if self.baseline_detail_advice is not None:
+            result['BaselineDetailAdvice'] = self.baseline_detail_advice
+        if self.baseline_detail_description is not None:
+            result['BaselineDetailDescription'] = self.baseline_detail_description
+        if self.baseline_detail_prompt is not None:
+            result['BaselineDetailPrompt'] = self.baseline_detail_prompt
+        if self.baseline_item_count is not None:
+            result['BaselineItemCount'] = self.baseline_item_count
+        if self.baseline_name_alias is not None:
+            result['BaselineNameAlias'] = self.baseline_name_alias
+        if self.baseline_name_key is not None:
+            result['BaselineNameKey'] = self.baseline_name_key
+        if self.baseline_name_level is not None:
+            result['BaselineNameLevel'] = self.baseline_name_level
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.first_scan_time is not None:
+            result['FirstScanTime'] = self.first_scan_time
+        if self.high_risk_item_count is not None:
+            result['HighRiskItemCount'] = self.high_risk_item_count
+        if self.low_risk_item_count is not None:
+            result['LowRiskItemCount'] = self.low_risk_item_count
+        if self.middle_risk_item_count is not None:
+            result['MiddleRiskItemCount'] = self.middle_risk_item_count
+        if self.scan_task_id is not None:
+            result['ScanTaskId'] = self.scan_task_id
+        if self.update_time is not None:
+            result['UpdateTime'] = self.update_time
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('BaselineClassAlias') is not None:
+            self.baseline_class_alias = m.get('BaselineClassAlias')
+        if m.get('BaselineDetailAdvice') is not None:
+            self.baseline_detail_advice = m.get('BaselineDetailAdvice')
+        if m.get('BaselineDetailDescription') is not None:
+            self.baseline_detail_description = m.get('BaselineDetailDescription')
+        if m.get('BaselineDetailPrompt') is not None:
+            self.baseline_detail_prompt = m.get('BaselineDetailPrompt')
+        if m.get('BaselineItemCount') is not None:
+            self.baseline_item_count = m.get('BaselineItemCount')
+        if m.get('BaselineNameAlias') is not None:
+            self.baseline_name_alias = m.get('BaselineNameAlias')
+        if m.get('BaselineNameKey') is not None:
+            self.baseline_name_key = m.get('BaselineNameKey')
+        if m.get('BaselineNameLevel') is not None:
+            self.baseline_name_level = m.get('BaselineNameLevel')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('FirstScanTime') is not None:
+            self.first_scan_time = m.get('FirstScanTime')
+        if m.get('HighRiskItemCount') is not None:
+            self.high_risk_item_count = m.get('HighRiskItemCount')
+        if m.get('LowRiskItemCount') is not None:
+            self.low_risk_item_count = m.get('LowRiskItemCount')
+        if m.get('MiddleRiskItemCount') is not None:
+            self.middle_risk_item_count = m.get('MiddleRiskItemCount')
+        if m.get('ScanTaskId') is not None:
+            self.scan_task_id = m.get('ScanTaskId')
+        if m.get('UpdateTime') is not None:
+            self.update_time = m.get('UpdateTime')
+        return self
+
+
+class ListScanBaselineByTaskResponseBody(TeaModel):
+    def __init__(self, code=None, is_success=None, page_no=None, page_size=None, request_id=None,
+                 scan_baselines=None, total_count=None):
+        self.code = code  # type: int
+        self.is_success = is_success  # type: bool
+        self.page_no = page_no  # type: int
+        self.page_size = page_size  # type: int
+        # Id of the request
+        self.request_id = request_id  # type: str
+        self.scan_baselines = scan_baselines  # type: list[ListScanBaselineByTaskResponseBodyScanBaselines]
+        self.total_count = total_count  # type: int
+
+    def validate(self):
+        if self.scan_baselines:
+            for k in self.scan_baselines:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListScanBaselineByTaskResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.is_success is not None:
+            result['IsSuccess'] = self.is_success
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['ScanBaselines'] = []
+        if self.scan_baselines is not None:
+            for k in self.scan_baselines:
+                result['ScanBaselines'].append(k.to_map() if k else None)
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('IsSuccess') is not None:
+            self.is_success = m.get('IsSuccess')
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.scan_baselines = []
+        if m.get('ScanBaselines') is not None:
+            for k in m.get('ScanBaselines'):
+                temp_model = ListScanBaselineByTaskResponseBodyScanBaselines()
+                self.scan_baselines.append(temp_model.from_map(k))
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListScanBaselineByTaskResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListScanBaselineByTaskResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListScanBaselineByTaskResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListScanBaselineByTaskResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListScanMaliciousFileByTaskRequest(TeaModel):
+    def __init__(self, digest=None, instance_id=None, level=None, page_no=None, page_size=None, repo_id=None,
+                 scan_task_id=None, tag=None):
+        self.digest = digest  # type: str
+        self.instance_id = instance_id  # type: str
+        self.level = level  # type: str
+        self.page_no = page_no  # type: int
+        self.page_size = page_size  # type: int
+        self.repo_id = repo_id  # type: str
+        self.scan_task_id = scan_task_id  # type: str
+        self.tag = tag  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListScanMaliciousFileByTaskRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.digest is not None:
+            result['Digest'] = self.digest
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.level is not None:
+            result['Level'] = self.level
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.repo_id is not None:
+            result['RepoId'] = self.repo_id
+        if self.scan_task_id is not None:
+            result['ScanTaskId'] = self.scan_task_id
+        if self.tag is not None:
+            result['Tag'] = self.tag
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Digest') is not None:
+            self.digest = m.get('Digest')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('Level') is not None:
+            self.level = m.get('Level')
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RepoId') is not None:
+            self.repo_id = m.get('RepoId')
+        if m.get('ScanTaskId') is not None:
+            self.scan_task_id = m.get('ScanTaskId')
+        if m.get('Tag') is not None:
+            self.tag = m.get('Tag')
+        return self
+
+
+class ListScanMaliciousFileByTaskResponseBodyScanMaliciousFiles(TeaModel):
+    def __init__(self, create_time=None, file_path=None, first_scan_time=None, level=None, malicious_md_5=None,
+                 malicious_name=None, scan_task_id=None, update_time=None):
+        self.create_time = create_time  # type: long
+        self.file_path = file_path  # type: str
+        self.first_scan_time = first_scan_time  # type: long
+        self.level = level  # type: str
+        self.malicious_md_5 = malicious_md_5  # type: str
+        self.malicious_name = malicious_name  # type: str
+        self.scan_task_id = scan_task_id  # type: str
+        self.update_time = update_time  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListScanMaliciousFileByTaskResponseBodyScanMaliciousFiles, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.file_path is not None:
+            result['FilePath'] = self.file_path
+        if self.first_scan_time is not None:
+            result['FirstScanTime'] = self.first_scan_time
+        if self.level is not None:
+            result['Level'] = self.level
+        if self.malicious_md_5 is not None:
+            result['MaliciousMd5'] = self.malicious_md_5
+        if self.malicious_name is not None:
+            result['MaliciousName'] = self.malicious_name
+        if self.scan_task_id is not None:
+            result['ScanTaskId'] = self.scan_task_id
+        if self.update_time is not None:
+            result['UpdateTime'] = self.update_time
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('FilePath') is not None:
+            self.file_path = m.get('FilePath')
+        if m.get('FirstScanTime') is not None:
+            self.first_scan_time = m.get('FirstScanTime')
+        if m.get('Level') is not None:
+            self.level = m.get('Level')
+        if m.get('MaliciousMd5') is not None:
+            self.malicious_md_5 = m.get('MaliciousMd5')
+        if m.get('MaliciousName') is not None:
+            self.malicious_name = m.get('MaliciousName')
+        if m.get('ScanTaskId') is not None:
+            self.scan_task_id = m.get('ScanTaskId')
+        if m.get('UpdateTime') is not None:
+            self.update_time = m.get('UpdateTime')
+        return self
+
+
+class ListScanMaliciousFileByTaskResponseBody(TeaModel):
+    def __init__(self, code=None, is_success=None, page_no=None, page_size=None, request_id=None,
+                 scan_malicious_files=None, total_count=None):
+        self.code = code  # type: int
+        self.is_success = is_success  # type: bool
+        self.page_no = page_no  # type: int
+        self.page_size = page_size  # type: int
+        self.request_id = request_id  # type: str
+        self.scan_malicious_files = scan_malicious_files  # type: list[ListScanMaliciousFileByTaskResponseBodyScanMaliciousFiles]
+        self.total_count = total_count  # type: int
+
+    def validate(self):
+        if self.scan_malicious_files:
+            for k in self.scan_malicious_files:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListScanMaliciousFileByTaskResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.is_success is not None:
+            result['IsSuccess'] = self.is_success
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['ScanMaliciousFiles'] = []
+        if self.scan_malicious_files is not None:
+            for k in self.scan_malicious_files:
+                result['ScanMaliciousFiles'].append(k.to_map() if k else None)
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('IsSuccess') is not None:
+            self.is_success = m.get('IsSuccess')
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.scan_malicious_files = []
+        if m.get('ScanMaliciousFiles') is not None:
+            for k in m.get('ScanMaliciousFiles'):
+                temp_model = ListScanMaliciousFileByTaskResponseBodyScanMaliciousFiles()
+                self.scan_malicious_files.append(temp_model.from_map(k))
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListScanMaliciousFileByTaskResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListScanMaliciousFileByTaskResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListScanMaliciousFileByTaskResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListScanMaliciousFileByTaskResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListTagResourcesRequestTag(TeaModel):
+    def __init__(self, key=None, value=None):
+        self.key = key  # type: str
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListTagResourcesRequestTag, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class ListTagResourcesRequest(TeaModel):
+    def __init__(self, next_token=None, region_id=None, resource_id=None, resource_type=None, tag=None):
+        self.next_token = next_token  # type: str
+        self.region_id = region_id  # type: str
+        self.resource_id = resource_id  # type: list[str]
+        self.resource_type = resource_type  # type: str
+        self.tag = tag  # type: list[ListTagResourcesRequestTag]
+
+    def validate(self):
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListTagResourcesRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = ListTagResourcesRequestTag()
+                self.tag.append(temp_model.from_map(k))
+        return self
+
+
+class ListTagResourcesResponseBodyTagResourcesTagResource(TeaModel):
+    def __init__(self, resource_id=None, resource_type=None, tag_key=None, tag_value=None):
+        self.resource_id = resource_id  # type: str
+        self.resource_type = resource_type  # type: str
+        self.tag_key = tag_key  # type: str
+        self.tag_value = tag_value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListTagResourcesResponseBodyTagResourcesTagResource, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        if self.tag_key is not None:
+            result['TagKey'] = self.tag_key
+        if self.tag_value is not None:
+            result['TagValue'] = self.tag_value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        if m.get('TagValue') is not None:
+            self.tag_value = m.get('TagValue')
+        return self
+
+
+class ListTagResourcesResponseBodyTagResources(TeaModel):
+    def __init__(self, tag_resource=None):
+        self.tag_resource = tag_resource  # type: list[ListTagResourcesResponseBodyTagResourcesTagResource]
+
+    def validate(self):
+        if self.tag_resource:
+            for k in self.tag_resource:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListTagResourcesResponseBodyTagResources, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['TagResource'] = []
+        if self.tag_resource is not None:
+            for k in self.tag_resource:
+                result['TagResource'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.tag_resource = []
+        if m.get('TagResource') is not None:
+            for k in m.get('TagResource'):
+                temp_model = ListTagResourcesResponseBodyTagResourcesTagResource()
+                self.tag_resource.append(temp_model.from_map(k))
+        return self
+
+
+class ListTagResourcesResponseBody(TeaModel):
+    def __init__(self, next_token=None, request_id=None, tag_resources=None):
+        self.next_token = next_token  # type: str
+        self.request_id = request_id  # type: str
+        self.tag_resources = tag_resources  # type: ListTagResourcesResponseBodyTagResources
+
+    def validate(self):
+        if self.tag_resources:
+            self.tag_resources.validate()
+
+    def to_map(self):
+        _map = super(ListTagResourcesResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.tag_resources is not None:
+            result['TagResources'] = self.tag_resources.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TagResources') is not None:
+            temp_model = ListTagResourcesResponseBodyTagResources()
+            self.tag_resources = temp_model.from_map(m['TagResources'])
+        return self
+
+
+class ListTagResourcesResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListTagResourcesResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListTagResourcesResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListTagResourcesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ResetLoginPasswordRequest(TeaModel):
     def __init__(self, instance_id=None, password=None):
         # The ID of the instance.
         self.instance_id = instance_id  # type: str
         # The new password that you specify to log on to the instance. The password must be 8 to 32 bits in length, and must contain at least two of the following character types: letters, special characters, and digits.
         self.password = password  # type: str
 
@@ -13538,17 +14267,14 @@
 class ResetLoginPasswordResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ResetLoginPasswordResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ResetLoginPasswordResponse, self).to_map()
         if _map is not None:
             return _map
@@ -13570,14 +14296,254 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ResetLoginPasswordResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class TagResourcesRequestTag(TeaModel):
+    def __init__(self, key=None, value=None):
+        self.key = key  # type: str
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(TagResourcesRequestTag, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class TagResourcesRequest(TeaModel):
+    def __init__(self, region_id=None, resource_id=None, resource_type=None, tag=None):
+        self.region_id = region_id  # type: str
+        self.resource_id = resource_id  # type: list[str]
+        self.resource_type = resource_type  # type: str
+        self.tag = tag  # type: list[TagResourcesRequestTag]
+
+    def validate(self):
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(TagResourcesRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = TagResourcesRequestTag()
+                self.tag.append(temp_model.from_map(k))
+        return self
+
+
+class TagResourcesResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(TagResourcesResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class TagResourcesResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: TagResourcesResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(TagResourcesResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = TagResourcesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class UntagResourcesRequest(TeaModel):
+    def __init__(self, all=None, region_id=None, resource_id=None, resource_type=None, tag_key=None):
+        self.all = all  # type: bool
+        self.region_id = region_id  # type: str
+        self.resource_id = resource_id  # type: list[str]
+        self.resource_type = resource_type  # type: str
+        self.tag_key = tag_key  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UntagResourcesRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.all is not None:
+            result['All'] = self.all
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        if self.tag_key is not None:
+            result['TagKey'] = self.tag_key
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('All') is not None:
+            self.all = m.get('All')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        return self
+
+
+class UntagResourcesResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UntagResourcesResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UntagResourcesResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: UntagResourcesResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(UntagResourcesResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UntagResourcesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateChainRequest(TeaModel):
     def __init__(self, chain_config=None, chain_id=None, description=None, instance_id=None, name=None,
                  scope_exclude=None):
         # The configuration of the delivery chain in the JSON format.
         self.chain_config = chain_config  # type: str
         # The ID of the delivery chain.
         self.chain_id = chain_id  # type: str
@@ -13670,17 +14636,14 @@
 class UpdateChainResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: UpdateChainResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UpdateChainResponse, self).to_map()
         if _map is not None:
             return _map
@@ -13798,17 +14761,14 @@
 class UpdateChartNamespaceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: UpdateChartNamespaceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UpdateChartNamespaceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -13929,17 +14889,14 @@
 class UpdateChartRepositoryResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: UpdateChartRepositoryResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UpdateChartRepositoryResponse, self).to_map()
         if _map is not None:
             return _map
@@ -14189,17 +15146,14 @@
 class UpdateEventCenterRuleResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: UpdateEventCenterRuleResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UpdateEventCenterRuleResponse, self).to_map()
         if _map is not None:
             return _map
@@ -14317,17 +15271,14 @@
 class UpdateInstanceEndpointStatusResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: UpdateInstanceEndpointStatusResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UpdateInstanceEndpointStatusResponse, self).to_map()
         if _map is not None:
             return _map
@@ -14439,17 +15390,14 @@
 class UpdateNamespaceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: UpdateNamespaceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UpdateNamespaceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -14615,17 +15563,14 @@
 class UpdateRepoBuildRuleResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: UpdateRepoBuildRuleResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UpdateRepoBuildRuleResponse, self).to_map()
         if _map is not None:
             return _map
@@ -14774,17 +15719,14 @@
 class UpdateRepoSourceCodeRepoResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: UpdateRepoSourceCodeRepoResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UpdateRepoSourceCodeRepoResponse, self).to_map()
         if _map is not None:
             return _map
@@ -14918,17 +15860,14 @@
 class UpdateRepoTriggerResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: UpdateRepoTriggerResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UpdateRepoTriggerResponse, self).to_map()
         if _map is not None:
             return _map
@@ -15051,17 +15990,14 @@
 class UpdateRepositoryResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: UpdateRepositoryResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UpdateRepositoryResponse, self).to_map()
         if _map is not None:
             return _map
```

### Comparing `alibabacloud_cr20181201_py2-1.2.0/alibabacloud_cr20181201_py2.egg-info/PKG-INFO` & `alibabacloud_cr20181201_py2-1.3.0/alibabacloud_cr20181201_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cr20181201-py2
-Version: 1.2.0
+Version: 1.3.0
 Summary: Alibaba Cloud cr (20181201) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cr20181201_py2-1.2.0/setup.py` & `alibabacloud_cr20181201_py2-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cr20181201_py2.
 
-Created on 27/09/2023
+Created on 11/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cr20181201"
 NAME = "alibabacloud_cr20181201_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud cr (20181201) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.8, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
```

