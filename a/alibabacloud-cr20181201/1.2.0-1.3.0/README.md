# Comparing `tmp/alibabacloud_cr20181201-1.2.0.tar.gz` & `tmp/alibabacloud_cr20181201-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cr20181201-1.2.0.tar", last modified: Wed Sep 27 17:12:06 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cr20181201-1.3.0.tar", last modified: Thu Apr 11 06:06:11 2024, max compression
```

## Comparing `alibabacloud_cr20181201-1.2.0.tar` & `alibabacloud_cr20181201-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/
--rw-r--r--   0 root         (0) root         (0)      599 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2322 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1019 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1104 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/alibabacloud_cr20181201/
--rw-r--r--   0 root         (0) root         (0)       21 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/alibabacloud_cr20181201/__init__.py
--rw-r--r--   0 root         (0) root         (0)   297402 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/alibabacloud_cr20181201/client.py
--rw-r--r--   0 root         (0) root         (0)   567123 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/alibabacloud_cr20181201/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/alibabacloud_cr20181201.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2322 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/alibabacloud_cr20181201.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/alibabacloud_cr20181201.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/alibabacloud_cr20181201.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/alibabacloud_cr20181201.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/alibabacloud_cr20181201.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2606 2023-09-27 17:12:06.000000 alibabacloud_cr20181201-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)      794 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   316752 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201/client.py
+-rw-r--r--   0 root         (0) root         (0)   597292 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-04-11 06:06:11.000000 alibabacloud_cr20181201-1.3.0/setup.py
```

### Comparing `alibabacloud_cr20181201-1.2.0/ChangeLog.md` & `alibabacloud_cr20181201-1.3.0/ChangeLog.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+2023-11-23 Version: 1.1.3
+- Generated python 2018-12-01 for cr.
+
+2023-11-03 Version: 1.1.2
+- Generated python 2018-12-01 for cr.
+
+2023-09-27 Version: 1.2.0
+- Generated python 2018-12-01 for cr.
+
 2023-08-22 Version: 1.1.0
 - Generated python 2018-12-01 for cr.
 
 2023-08-22 Version: 1.1.0
 - Generated python 2018-12-01 for cr.
 
 2022-12-08 Version: 1.0.11
```

### Comparing `alibabacloud_cr20181201-1.2.0/LICENSE` & `alibabacloud_cr20181201-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cr20181201-1.2.0/PKG-INFO` & `alibabacloud_cr20181201-1.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cr20181201
-Version: 1.2.0
+Version: 1.3.0
 Summary: Alibaba Cloud cr (20181201) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/cr-20181201/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_cr20181201-1.2.0/README-CN.md` & `alibabacloud_cr20181201-1.3.0/README-CN.md`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/cr-20181201/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_cr20181201-1.2.0/README.md` & `alibabacloud_cr20181201-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/cr-20181201/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_cr20181201-1.2.0/alibabacloud_cr20181201/client.py` & `alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,30 +269,37 @@
         request: cr_20181201_models.ChangeResourceGroupRequest,
     ) -> cr_20181201_models.ChangeResourceGroupResponse:
         runtime = util_models.RuntimeOptions()
         return await self.change_resource_group_with_options_async(request, runtime)
 
     def create_artifact_build_rule_with_options(
         self,
-        request: cr_20181201_models.CreateArtifactBuildRuleRequest,
+        tmp_req: cr_20181201_models.CreateArtifactBuildRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cr_20181201_models.CreateArtifactBuildRuleResponse:
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
@@ -310,30 +317,37 @@
         return TeaCore.from_map(
             cr_20181201_models.CreateArtifactBuildRuleResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def create_artifact_build_rule_with_options_async(
         self,
-        request: cr_20181201_models.CreateArtifactBuildRuleRequest,
+        tmp_req: cr_20181201_models.CreateArtifactBuildRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cr_20181201_models.CreateArtifactBuildRuleResponse:
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
@@ -354,28 +368,30 @@
         )
 
     def create_artifact_build_rule(
         self,
         request: cr_20181201_models.CreateArtifactBuildRuleRequest,
     ) -> cr_20181201_models.CreateArtifactBuildRuleResponse:
         """
-        The ID of the rule.
+        You can create building rules of accelerated images only for image repositories of Container Registry Advanced Edition instances. You cannot create building rules of accelerated images for image repositories of Container Registry Basic Edition instances. For more information, see [Specifications of different editions](https://www.alibabacloud.com/help/zh/container-registry/latest/what-is-container-registry#section-go7-lhg-qbc).
+        Accelerated images can be built in the following regions: China (Hangzhou), China (Shanghai), China (Beijing), China (Shenzhen), China (Guangzhou), China (Zhangjiakou), China (Hong Kong), US (Virginia), US (Silicon Valley), Singapore, Japan (Tokyo), and Malaysia (Kuala Lumpur).
         
         @param request: CreateArtifactBuildRuleRequest
         @return: CreateArtifactBuildRuleResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_artifact_build_rule_with_options(request, runtime)
 
     async def create_artifact_build_rule_async(
         self,
         request: cr_20181201_models.CreateArtifactBuildRuleRequest,
     ) -> cr_20181201_models.CreateArtifactBuildRuleResponse:
         """
-        The ID of the rule.
+        You can create building rules of accelerated images only for image repositories of Container Registry Advanced Edition instances. You cannot create building rules of accelerated images for image repositories of Container Registry Basic Edition instances. For more information, see [Specifications of different editions](https://www.alibabacloud.com/help/zh/container-registry/latest/what-is-container-registry#section-go7-lhg-qbc).
+        Accelerated images can be built in the following regions: China (Hangzhou), China (Shanghai), China (Beijing), China (Shenzhen), China (Guangzhou), China (Zhangjiakou), China (Hong Kong), US (Virginia), US (Silicon Valley), Singapore, Japan (Tokyo), and Malaysia (Kuala Lumpur).
         
         @param request: CreateArtifactBuildRuleRequest
         @return: CreateArtifactBuildRuleResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_artifact_build_rule_with_options_async(request, runtime)
 
@@ -885,15 +901,15 @@
 
     def create_instance_vpc_endpoint_linked_vpc_with_options(
         self,
         request: cr_20181201_models.CreateInstanceVpcEndpointLinkedVpcRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cr_20181201_models.CreateInstanceVpcEndpointLinkedVpcResponse:
         """
-        The ID of the request.
+        A maximum of three VPCs can be associated with a Container Registry instance. If you want to associate more VPCs, contact Alibaba Cloud technical support.
         
         @param request: CreateInstanceVpcEndpointLinkedVpcRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateInstanceVpcEndpointLinkedVpcResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -928,15 +944,15 @@
 
     async def create_instance_vpc_endpoint_linked_vpc_with_options_async(
         self,
         request: cr_20181201_models.CreateInstanceVpcEndpointLinkedVpcRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cr_20181201_models.CreateInstanceVpcEndpointLinkedVpcResponse:
         """
-        The ID of the request.
+        A maximum of three VPCs can be associated with a Container Registry instance. If you want to associate more VPCs, contact Alibaba Cloud technical support.
         
         @param request: CreateInstanceVpcEndpointLinkedVpcRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateInstanceVpcEndpointLinkedVpcResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -970,28 +986,28 @@
         )
 
     def create_instance_vpc_endpoint_linked_vpc(
         self,
         request: cr_20181201_models.CreateInstanceVpcEndpointLinkedVpcRequest,
     ) -> cr_20181201_models.CreateInstanceVpcEndpointLinkedVpcResponse:
         """
-        The ID of the request.
+        A maximum of three VPCs can be associated with a Container Registry instance. If you want to associate more VPCs, contact Alibaba Cloud technical support.
         
         @param request: CreateInstanceVpcEndpointLinkedVpcRequest
         @return: CreateInstanceVpcEndpointLinkedVpcResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_instance_vpc_endpoint_linked_vpc_with_options(request, runtime)
 
     async def create_instance_vpc_endpoint_linked_vpc_async(
         self,
         request: cr_20181201_models.CreateInstanceVpcEndpointLinkedVpcRequest,
     ) -> cr_20181201_models.CreateInstanceVpcEndpointLinkedVpcResponse:
         """
-        The ID of the request.
+        A maximum of three VPCs can be associated with a Container Registry instance. If you want to associate more VPCs, contact Alibaba Cloud technical support.
         
         @param request: CreateInstanceVpcEndpointLinkedVpcRequest
         @return: CreateInstanceVpcEndpointLinkedVpcResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_instance_vpc_endpoint_linked_vpc_with_options_async(request, runtime)
 
@@ -5440,14 +5456,16 @@
     ) -> cr_20181201_models.ListInstanceEndpointResponse:
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
@@ -5470,14 +5488,16 @@
     ) -> cr_20181201_models.ListInstanceEndpointResponse:
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
@@ -6449,14 +6469,232 @@
     async def list_repository_async(
         self,
         request: cr_20181201_models.ListRepositoryRequest,
     ) -> cr_20181201_models.ListRepositoryResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_repository_with_options_async(request, runtime)
 
+    def list_scan_baseline_by_task_with_options(
+        self,
+        request: cr_20181201_models.ListScanBaselineByTaskRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.ListScanBaselineByTaskResponse:
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
+    async def list_scan_baseline_by_task_with_options_async(
+        self,
+        request: cr_20181201_models.ListScanBaselineByTaskRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.ListScanBaselineByTaskResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_scan_baseline_by_task(
+        self,
+        request: cr_20181201_models.ListScanBaselineByTaskRequest,
+    ) -> cr_20181201_models.ListScanBaselineByTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_scan_baseline_by_task_with_options(request, runtime)
+
+    async def list_scan_baseline_by_task_async(
+        self,
+        request: cr_20181201_models.ListScanBaselineByTaskRequest,
+    ) -> cr_20181201_models.ListScanBaselineByTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_scan_baseline_by_task_with_options_async(request, runtime)
+
+    def list_scan_malicious_file_by_task_with_options(
+        self,
+        request: cr_20181201_models.ListScanMaliciousFileByTaskRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.ListScanMaliciousFileByTaskResponse:
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
+    async def list_scan_malicious_file_by_task_with_options_async(
+        self,
+        request: cr_20181201_models.ListScanMaliciousFileByTaskRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.ListScanMaliciousFileByTaskResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_scan_malicious_file_by_task(
+        self,
+        request: cr_20181201_models.ListScanMaliciousFileByTaskRequest,
+    ) -> cr_20181201_models.ListScanMaliciousFileByTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_scan_malicious_file_by_task_with_options(request, runtime)
+
+    async def list_scan_malicious_file_by_task_async(
+        self,
+        request: cr_20181201_models.ListScanMaliciousFileByTaskRequest,
+    ) -> cr_20181201_models.ListScanMaliciousFileByTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_scan_malicious_file_by_task_with_options_async(request, runtime)
+
+    def list_tag_resources_with_options(
+        self,
+        request: cr_20181201_models.ListTagResourcesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.ListTagResourcesResponse:
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
+    async def list_tag_resources_with_options_async(
+        self,
+        request: cr_20181201_models.ListTagResourcesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.ListTagResourcesResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_tag_resources(
+        self,
+        request: cr_20181201_models.ListTagResourcesRequest,
+    ) -> cr_20181201_models.ListTagResourcesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_tag_resources_with_options(request, runtime)
+
+    async def list_tag_resources_async(
+        self,
+        request: cr_20181201_models.ListTagResourcesRequest,
+    ) -> cr_20181201_models.ListTagResourcesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_tag_resources_with_options_async(request, runtime)
+
     def reset_login_password_with_options(
         self,
         request: cr_20181201_models.ResetLoginPasswordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cr_20181201_models.ResetLoginPasswordResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -6523,14 +6761,182 @@
     async def reset_login_password_async(
         self,
         request: cr_20181201_models.ResetLoginPasswordRequest,
     ) -> cr_20181201_models.ResetLoginPasswordResponse:
         runtime = util_models.RuntimeOptions()
         return await self.reset_login_password_with_options_async(request, runtime)
 
+    def tag_resources_with_options(
+        self,
+        request: cr_20181201_models.TagResourcesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.TagResourcesResponse:
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
+    async def tag_resources_with_options_async(
+        self,
+        request: cr_20181201_models.TagResourcesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.TagResourcesResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def tag_resources(
+        self,
+        request: cr_20181201_models.TagResourcesRequest,
+    ) -> cr_20181201_models.TagResourcesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.tag_resources_with_options(request, runtime)
+
+    async def tag_resources_async(
+        self,
+        request: cr_20181201_models.TagResourcesRequest,
+    ) -> cr_20181201_models.TagResourcesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.tag_resources_with_options_async(request, runtime)
+
+    def untag_resources_with_options(
+        self,
+        request: cr_20181201_models.UntagResourcesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.UntagResourcesResponse:
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
+    async def untag_resources_with_options_async(
+        self,
+        request: cr_20181201_models.UntagResourcesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cr_20181201_models.UntagResourcesResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def untag_resources(
+        self,
+        request: cr_20181201_models.UntagResourcesRequest,
+    ) -> cr_20181201_models.UntagResourcesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.untag_resources_with_options(request, runtime)
+
+    async def untag_resources_async(
+        self,
+        request: cr_20181201_models.UntagResourcesRequest,
+    ) -> cr_20181201_models.UntagResourcesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.untag_resources_with_options_async(request, runtime)
+
     def update_chain_with_options(
         self,
         request: cr_20181201_models.UpdateChainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cr_20181201_models.UpdateChainResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_cr20181201-1.2.0/alibabacloud_cr20181201/models.py` & `alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import Dict, List, Any
+from typing import Dict, Any, List
 
 
 class CancelArtifactBuildTaskRequest(TeaModel):
     def __init__(
         self,
         build_task_id: str = None,
         instance_id: str = None,
@@ -92,17 +92,14 @@
         body: CancelArtifactBuildTaskResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -220,17 +217,14 @@
         body: CancelRepoBuildRecordResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -259,17 +253,19 @@
 class ChangeResourceGroupRequest(TeaModel):
     def __init__(
         self,
         resource_group_id: str = None,
         resource_id: str = None,
         resource_region_id: str = None,
     ):
+        # The ID of the resource group.
         self.resource_group_id = resource_group_id
         # Id of the request
         self.resource_id = resource_id
+        # The region ID of the resource group.
         self.resource_region_id = resource_region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -297,14 +293,15 @@
 
 
 class ChangeResourceGroupResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -331,17 +328,14 @@
         body: ChangeResourceGroupResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -368,20 +362,95 @@
 
 
 class CreateArtifactBuildRuleRequest(TeaModel):
     def __init__(
         self,
         artifact_type: str = None,
         instance_id: str = None,
+        parameters: Dict[str, Any] = None,
         scope_id: str = None,
         scope_type: str = None,
     ):
+        # The type of the artifact.
+        # 
+        # *   `ACCELERATED_IMAGE`: accelerated images.
+        self.artifact_type = artifact_type
+        # The instance ID.
+        self.instance_id = instance_id
+        # Additional parameters.
+        self.parameters = parameters
+        # The ID of the effective range of the rule.
+        # 
+        # *   Set the value to the ID of the image repository.
+        self.scope_id = scope_id
+        # The effective range of the rule. Valid values:
+        # 
+        # *   `REPOSITORY`
+        self.scope_type = scope_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.artifact_type is not None:
+            result['ArtifactType'] = self.artifact_type
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.parameters is not None:
+            result['Parameters'] = self.parameters
+        if self.scope_id is not None:
+            result['ScopeId'] = self.scope_id
+        if self.scope_type is not None:
+            result['ScopeType'] = self.scope_type
+        return result
+
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        artifact_type: str = None,
+        instance_id: str = None,
+        parameters_shrink: str = None,
+        scope_id: str = None,
+        scope_type: str = None,
+    ):
+        # The type of the artifact.
+        # 
+        # *   `ACCELERATED_IMAGE`: accelerated images.
         self.artifact_type = artifact_type
+        # The instance ID.
         self.instance_id = instance_id
+        # Additional parameters.
+        self.parameters_shrink = parameters_shrink
+        # The ID of the effective range of the rule.
+        # 
+        # *   Set the value to the ID of the image repository.
         self.scope_id = scope_id
+        # The effective range of the rule. Valid values:
+        # 
+        # *   `REPOSITORY`
         self.scope_type = scope_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -389,26 +458,30 @@
             return _map
 
         result = dict()
         if self.artifact_type is not None:
             result['ArtifactType'] = self.artifact_type
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
+        if self.parameters_shrink is not None:
+            result['Parameters'] = self.parameters_shrink
         if self.scope_id is not None:
             result['ScopeId'] = self.scope_id
         if self.scope_type is not None:
             result['ScopeType'] = self.scope_type
         return result
 
     def from_map(self, m: dict = None):
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
 
 
@@ -416,17 +489,21 @@
     def __init__(
         self,
         build_rule_id: str = None,
         code: str = None,
         is_success: bool = None,
         request_id: str = None,
     ):
+        # The ID of the accelerated image building rule.
         self.build_rule_id = build_rule_id
+        # The return value.
         self.code = code
+        # Indicates whether the request is successful.
         self.is_success = is_success
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -465,17 +542,14 @@
         body: CreateArtifactBuildRuleResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -593,17 +667,14 @@
         body: CreateBuildRecordByRecordResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -728,17 +799,14 @@
         body: CreateBuildRecordByRuleResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -891,17 +959,14 @@
         body: CreateChainResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1036,17 +1101,14 @@
         body: CreateChartNamespaceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1193,17 +1255,14 @@
         body: CreateChartRepositoryResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1341,17 +1400,14 @@
         body: CreateInstanceEndpointAclPolicyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1382,18 +1438,31 @@
         self,
         enable_create_dnsrecord_in_pvzt: bool = None,
         instance_id: str = None,
         module_name: str = None,
         vpc_id: str = None,
         vswitch_id: str = None,
     ):
+        # Specifies whether to automatically create Alibaba Cloud DNS PrivateZone records. Valid values:
+        # 
+        # >  If you enable automatic creation of PrivateZone records, a PrivateZone record is automatically created when you associate a VPC with the instance.
+        # 
+        # *   `true`
+        # *   `false`
         self.enable_create_dnsrecord_in_pvzt = enable_create_dnsrecord_in_pvzt
+        # The instance ID.
         self.instance_id = instance_id
+        # The name of the module that you want to access. Valid values:
+        # 
+        # *   `Registry`: image repositories.
+        # *   `Chart`: Helm charts.
         self.module_name = module_name
+        # The VPC ID.
         self.vpc_id = vpc_id
+        # The ID of the vSwitch that is associated with the specified VPC.
         self.vswitch_id = vswitch_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1431,16 +1500,22 @@
 class CreateInstanceVpcEndpointLinkedVpcResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
         is_success: bool = None,
         request_id: str = None,
     ):
+        # The return value.
         self.code = code
+        # Indicates whether the request is successful.
+        # 
+        # *   `true`: The request is successful.
+        # *   `false`: The request fails.
         self.is_success = is_success
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1475,17 +1550,14 @@
         body: CreateInstanceVpcEndpointLinkedVpcResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1613,17 +1685,14 @@
         body: CreateNamespaceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1804,17 +1873,14 @@
         body: CreateRepoBuildRuleResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1976,17 +2042,14 @@
         body: CreateRepoSourceCodeRepoResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2158,17 +2221,14 @@
         body: CreateRepoSyncRuleResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2328,17 +2388,14 @@
         body: CreateRepoSyncTaskResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2473,17 +2530,14 @@
         body: CreateRepoSyncTaskByRuleResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2615,17 +2669,14 @@
         body: CreateRepoTagResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2763,17 +2814,14 @@
         body: CreateRepoTagScanTaskResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2930,17 +2978,14 @@
         body: CreateRepoTriggerResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3099,17 +3144,14 @@
         body: CreateRepositoryResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3220,17 +3262,14 @@
         body: DeleteChainResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3344,17 +3383,14 @@
         body: DeleteChartNamespaceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3486,17 +3522,14 @@
         body: DeleteChartReleaseResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3617,17 +3650,14 @@
         body: DeleteChartRepositoryResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3731,17 +3761,14 @@
         body: DeleteEventCenterRuleResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3872,17 +3899,14 @@
         body: DeleteInstanceEndpointAclPolicyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4013,17 +4037,14 @@
         body: DeleteInstanceVpcEndpointLinkedVpcResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4134,17 +4155,14 @@
         body: DeleteNamespaceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4262,17 +4280,14 @@
         body: DeleteRepoBuildRuleResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4383,17 +4398,14 @@
         body: DeleteRepoSyncRuleResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4511,17 +4523,14 @@
         body: DeleteRepoTagResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4642,17 +4651,14 @@
         body: DeleteRepoTriggerResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4686,15 +4692,17 @@
         repo_name: str = None,
         repo_namespace_name: str = None,
     ):
         # The ID of the instance.
         self.instance_id = instance_id
         # The ID of the image repository.
         self.repo_id = repo_id
+        # The name of the repository.
         self.repo_name = repo_name
+        # The name of the namespace to which the repository belongs.
         self.repo_namespace_name = repo_namespace_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4728,22 +4736,22 @@
 class DeleteRepositoryResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
         is_success: bool = None,
         request_id: str = None,
     ):
-        # The return value.
+        # Return values
         self.code = code
         # Indicates whether the request is successful. Valid values:
         # 
         # *   `true`: The request is successful.
         # *   `false`: The request fails.
         self.is_success = is_success
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4778,17 +4786,14 @@
         body: DeleteRepositoryResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4861,35 +4866,65 @@
         if m.get('ScopeId') is not None:
             self.scope_id = m.get('ScopeId')
         if m.get('ScopeType') is not None:
             self.scope_type = m.get('ScopeType')
         return self
 
 
+class GetArtifactBuildRuleResponseBodyParameters(TeaModel):
+    def __init__(
+        self,
+        image_index_only: bool = None,
+    ):
+        self.image_index_only = image_index_only
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.image_index_only is not None:
+            result['ImageIndexOnly'] = self.image_index_only
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ImageIndexOnly') is not None:
+            self.image_index_only = m.get('ImageIndexOnly')
+        return self
+
+
 class GetArtifactBuildRuleResponseBody(TeaModel):
     def __init__(
         self,
         artifact_type: str = None,
         build_rule_id: str = None,
         code: str = None,
         is_success: bool = None,
+        parameters: GetArtifactBuildRuleResponseBodyParameters = None,
         request_id: str = None,
         scope_id: str = None,
         scope_type: str = None,
     ):
         self.artifact_type = artifact_type
         self.build_rule_id = build_rule_id
         self.code = code
         self.is_success = is_success
+        self.parameters = parameters
         self.request_id = request_id
         self.scope_id = scope_id
         self.scope_type = scope_type
 
     def validate(self):
-        pass
+        if self.parameters:
+            self.parameters.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -4897,14 +4932,16 @@
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
@@ -4915,14 +4952,17 @@
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
@@ -4936,17 +4976,14 @@
         body: GetArtifactBuildRuleResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5209,17 +5246,14 @@
         body: GetArtifactBuildTaskResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5351,17 +5385,14 @@
         body: GetAuthorizationTokenResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5840,17 +5871,14 @@
         body: GetChainResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6021,17 +6049,14 @@
         body: GetChartNamespaceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6227,17 +6252,14 @@
         body: GetChartRepositoryResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6286,43 +6308,81 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         return self
 
 
+class GetInstanceResponseBodyTags(TeaModel):
+    def __init__(
+        self,
+        tag_key: str = None,
+        tag_value: str = None,
+    ):
+        self.tag_key = tag_key
+        self.tag_value = tag_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        if m.get('TagValue') is not None:
+            self.tag_value = m.get('TagValue')
+        return self
+
+
 class GetInstanceResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
         create_time: int = None,
         instance_id: str = None,
         instance_issue: str = None,
         instance_name: str = None,
         instance_specification: str = None,
         instance_status: str = None,
         is_success: bool = None,
         modified_time: int = None,
         request_id: str = None,
         resource_group_id: str = None,
+        tags: List[GetInstanceResponseBodyTags] = None,
     ):
         self.code = code
         self.create_time = create_time
         self.instance_id = instance_id
         self.instance_issue = instance_issue
         self.instance_name = instance_name
         self.instance_specification = instance_specification
         self.instance_status = instance_status
         self.is_success = is_success
         self.modified_time = modified_time
         self.request_id = request_id
         self.resource_group_id = resource_group_id
+        self.tags = tags
 
     def validate(self):
-        pass
+        if self.tags:
+            for k in self.tags:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -6344,14 +6404,18 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
         if m.get('CreateTime') is not None:
@@ -6370,14 +6434,19 @@
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
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -6385,17 +6454,14 @@
         body: GetInstanceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6474,17 +6540,14 @@
         body: GetInstanceCountResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6730,17 +6793,14 @@
         body: GetInstanceEndpointResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6903,17 +6963,14 @@
         body: GetInstanceUsageResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -7126,17 +7183,14 @@
         body: GetInstanceVpcEndpointResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -7305,17 +7359,14 @@
         body: GetNamespaceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -7505,17 +7556,14 @@
         body: GetRepoBuildRecordResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -7640,17 +7688,14 @@
         body: GetRepoBuildRecordStatusResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -7829,17 +7874,14 @@
         body: GetRepoSourceCodeRepoResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -8226,17 +8268,14 @@
         body: GetRepoSyncTaskResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -8405,17 +8444,14 @@
         body: GetRepoTagResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -8614,17 +8650,14 @@
         body: GetRepoTagLayersResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -9069,17 +9102,14 @@
         body: GetRepoTagManifestResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -9215,17 +9245,14 @@
         body: GetRepoTagScanStatusResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -9394,17 +9421,14 @@
         body: GetRepoTagScanSummaryResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -9628,17 +9652,14 @@
         body: GetRepositoryResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -9823,17 +9844,14 @@
         body: ListArtifactBuildTaskLogResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -10085,17 +10103,14 @@
         body: ListChainResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -10401,17 +10416,14 @@
         body: ListChainInstanceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -10657,17 +10669,14 @@
         body: ListChartNamespaceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -10912,17 +10921,14 @@
         body: ListChartReleaseResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -11198,17 +11204,14 @@
         body: ListChartRepositoryResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -11237,14 +11240,16 @@
 class ListEventCenterRecordRequest(TeaModel):
     def __init__(
         self,
         event_type: str = None,
         instance_id: str = None,
         page_no: int = None,
         page_size: int = None,
+        repo_name: str = None,
+        repo_namespace_name: str = None,
         rule_id: str = None,
     ):
         # The type of the event. Valid values:
         # 
         # *   `cr:Artifact:DeliveryChainCompleted`: The delivery chain is processed.
         # *   `cr:Artifact:SynchronizationCompleted`: The image is replicated.
         # *   `cr:Artifact:BuildCompleted`: The image is built.
@@ -11253,14 +11258,16 @@
         self.event_type = event_type
         # The ID of the instance.
         self.instance_id = instance_id
         # The number of the page to return.
         self.page_no = page_no
         # The number of entries to return on each page.
         self.page_size = page_size
+        self.repo_name = repo_name
+        self.repo_namespace_name = repo_namespace_name
         # The ID of the event notification rule.
         self.rule_id = rule_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -11273,28 +11280,36 @@
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
 
     def from_map(self, m: dict = None):
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
     def __init__(
@@ -11498,17 +11513,14 @@
         body: ListEventCenterRecordResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -11662,17 +11674,14 @@
         body: ListEventCenterRuleNameResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -11703,18 +11712,32 @@
         self,
         instance_name: str = None,
         instance_status: str = None,
         page_no: int = None,
         page_size: int = None,
         resource_group_id: str = None,
     ):
+        # The instance name.
         self.instance_name = instance_name
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
         self.instance_status = instance_status
+        # The page number.
         self.page_no = page_no
+        # The number of entries per page.
         self.page_size = page_size
+        # The ID of the resource group to which the instance belongs.
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11745,39 +11768,86 @@
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         return self
 
 
+class ListInstanceResponseBodyInstancesTags(TeaModel):
+    def __init__(
+        self,
+        tag_key: str = None,
+        tag_value: str = None,
+    ):
+        self.tag_key = tag_key
+        self.tag_value = tag_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        if m.get('TagValue') is not None:
+            self.tag_value = m.get('TagValue')
+        return self
+
+
 class ListInstanceResponseBodyInstances(TeaModel):
     def __init__(
         self,
         create_time: str = None,
         instance_id: str = None,
         instance_issue: str = None,
         instance_name: str = None,
         instance_specification: str = None,
         instance_status: str = None,
         modified_time: str = None,
         region_id: str = None,
         resource_group_id: str = None,
+        tags: List[ListInstanceResponseBodyInstancesTags] = None,
     ):
+        # The time when the instance was created.
         self.create_time = create_time
+        # The instance ID.
         self.instance_id = instance_id
+        # The issue occurs on the instance.
         self.instance_issue = instance_issue
+        # The name of the instance.
         self.instance_name = instance_name
+        # The edition of the Container Registry Enterprise Edition instance.
         self.instance_specification = instance_specification
+        # The status of the instance.
         self.instance_status = instance_status
+        # The time when the instance was last modified.
         self.modified_time = modified_time
+        # The region ID of the instance.
         self.region_id = region_id
+        # The ID of the resource group to which the instance belongs.
         self.resource_group_id = resource_group_id
+        self.tags = tags
 
     def validate(self):
-        pass
+        if self.tags:
+            for k in self.tags:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -11795,14 +11865,18 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('InstanceId') is not None:
@@ -11817,34 +11891,46 @@
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
     def __init__(
         self,
         code: str = None,
         instances: List[ListInstanceResponseBodyInstances] = None,
         is_success: bool = None,
         page_no: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The return value.
         self.code = code
+        # The queried instances.
         self.instances = instances
+        # Indicates whether the request is successful.
         self.is_success = is_success
+        # The page number. Default value: 1.
         self.page_no = page_no
+        # The number of entries per page. Default value: 30.
         self.page_size = page_size
+        # The request ID.
         self.request_id = request_id
+        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.instances:
             for k in self.instances:
                 if k:
                     k.validate()
@@ -11903,17 +11989,14 @@
         body: ListInstanceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -11940,44 +12023,50 @@
 
 
 class ListInstanceEndpointRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         module_name: str = None,
+        summary: bool = None,
     ):
         # The ID of the instance.
         self.instance_id = instance_id
         # The name of the module that you want to access. Valid values:
         # 
         # *   `Registry`: the image repository.
         # *   `Chart`: a Helm chart.
         self.module_name = module_name
+        self.summary = summary
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('ModuleName') is not None:
             self.module_name = m.get('ModuleName')
+        if m.get('Summary') is not None:
+            self.summary = m.get('Summary')
         return self
 
 
 class ListInstanceEndpointResponseBodyEndpointsAclEntries(TeaModel):
     def __init__(
         self,
         entry: str = None,
@@ -12229,17 +12318,14 @@
         body: ListInstanceEndpointResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -12396,17 +12482,14 @@
         body: ListInstanceRegionResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -12630,17 +12713,14 @@
         body: ListNamespaceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -12911,17 +12991,14 @@
         body: ListRepoBuildRecordResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -13124,17 +13201,14 @@
         body: ListRepoBuildRecordLogResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -13376,17 +13450,14 @@
         body: ListRepoBuildRuleResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -13722,17 +13793,14 @@
         body: ListRepoSyncRuleResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -14100,17 +14168,14 @@
         body: ListRepoSyncTaskResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -14341,17 +14406,14 @@
         body: ListRepoTagResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -14687,17 +14749,14 @@
         body: ListRepoTagScanResultResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -14896,17 +14955,14 @@
         body: ListRepoTriggerResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -15161,17 +15217,14 @@
         body: ListRepositoryResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -15193,14 +15246,811 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListRepositoryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListScanBaselineByTaskRequest(TeaModel):
+    def __init__(
+        self,
+        digest: str = None,
+        instance_id: str = None,
+        level: str = None,
+        page_no: int = None,
+        page_size: int = None,
+        repo_id: str = None,
+        scan_task_id: str = None,
+        tag: str = None,
+    ):
+        self.digest = digest
+        self.instance_id = instance_id
+        self.level = level
+        self.page_no = page_no
+        self.page_size = page_size
+        self.repo_id = repo_id
+        self.scan_task_id = scan_task_id
+        self.tag = tag
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        baseline_class_alias: str = None,
+        baseline_detail_advice: str = None,
+        baseline_detail_description: str = None,
+        baseline_detail_prompt: str = None,
+        baseline_item_count: int = None,
+        baseline_name_alias: str = None,
+        baseline_name_key: str = None,
+        baseline_name_level: str = None,
+        create_time: int = None,
+        first_scan_time: int = None,
+        high_risk_item_count: int = None,
+        low_risk_item_count: int = None,
+        middle_risk_item_count: int = None,
+        scan_task_id: str = None,
+        update_time: int = None,
+    ):
+        self.baseline_class_alias = baseline_class_alias
+        self.baseline_detail_advice = baseline_detail_advice
+        self.baseline_detail_description = baseline_detail_description
+        self.baseline_detail_prompt = baseline_detail_prompt
+        self.baseline_item_count = baseline_item_count
+        self.baseline_name_alias = baseline_name_alias
+        self.baseline_name_key = baseline_name_key
+        self.baseline_name_level = baseline_name_level
+        self.create_time = create_time
+        self.first_scan_time = first_scan_time
+        self.high_risk_item_count = high_risk_item_count
+        self.low_risk_item_count = low_risk_item_count
+        self.middle_risk_item_count = middle_risk_item_count
+        self.scan_task_id = scan_task_id
+        self.update_time = update_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        code: int = None,
+        is_success: bool = None,
+        page_no: int = None,
+        page_size: int = None,
+        request_id: str = None,
+        scan_baselines: List[ListScanBaselineByTaskResponseBodyScanBaselines] = None,
+        total_count: int = None,
+    ):
+        self.code = code
+        self.is_success = is_success
+        self.page_no = page_no
+        self.page_size = page_size
+        # Id of the request
+        self.request_id = request_id
+        self.scan_baselines = scan_baselines
+        self.total_count = total_count
+
+    def validate(self):
+        if self.scan_baselines:
+            for k in self.scan_baselines:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListScanBaselineByTaskResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        digest: str = None,
+        instance_id: str = None,
+        level: str = None,
+        page_no: int = None,
+        page_size: int = None,
+        repo_id: str = None,
+        scan_task_id: str = None,
+        tag: str = None,
+    ):
+        self.digest = digest
+        self.instance_id = instance_id
+        self.level = level
+        self.page_no = page_no
+        self.page_size = page_size
+        self.repo_id = repo_id
+        self.scan_task_id = scan_task_id
+        self.tag = tag
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        create_time: int = None,
+        file_path: str = None,
+        first_scan_time: int = None,
+        level: str = None,
+        malicious_md_5: str = None,
+        malicious_name: str = None,
+        scan_task_id: str = None,
+        update_time: int = None,
+    ):
+        self.create_time = create_time
+        self.file_path = file_path
+        self.first_scan_time = first_scan_time
+        self.level = level
+        self.malicious_md_5 = malicious_md_5
+        self.malicious_name = malicious_name
+        self.scan_task_id = scan_task_id
+        self.update_time = update_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        code: int = None,
+        is_success: bool = None,
+        page_no: int = None,
+        page_size: int = None,
+        request_id: str = None,
+        scan_malicious_files: List[ListScanMaliciousFileByTaskResponseBodyScanMaliciousFiles] = None,
+        total_count: int = None,
+    ):
+        self.code = code
+        self.is_success = is_success
+        self.page_no = page_no
+        self.page_size = page_size
+        self.request_id = request_id
+        self.scan_malicious_files = scan_malicious_files
+        self.total_count = total_count
+
+    def validate(self):
+        if self.scan_malicious_files:
+            for k in self.scan_malicious_files:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListScanMaliciousFileByTaskResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class ListTagResourcesRequest(TeaModel):
+    def __init__(
+        self,
+        next_token: str = None,
+        region_id: str = None,
+        resource_id: List[str] = None,
+        resource_type: str = None,
+        tag: List[ListTagResourcesRequestTag] = None,
+    ):
+        self.next_token = next_token
+        self.region_id = region_id
+        self.resource_id = resource_id
+        self.resource_type = resource_type
+        self.tag = tag
+
+    def validate(self):
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        resource_id: str = None,
+        resource_type: str = None,
+        tag_key: str = None,
+        tag_value: str = None,
+    ):
+        self.resource_id = resource_id
+        self.resource_type = resource_type
+        self.tag_key = tag_key
+        self.tag_value = tag_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        tag_resource: List[ListTagResourcesResponseBodyTagResourcesTagResource] = None,
+    ):
+        self.tag_resource = tag_resource
+
+    def validate(self):
+        if self.tag_resource:
+            for k in self.tag_resource:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        next_token: str = None,
+        request_id: str = None,
+        tag_resources: ListTagResourcesResponseBodyTagResources = None,
+    ):
+        self.next_token = next_token
+        self.request_id = request_id
+        self.tag_resources = tag_resources
+
+    def validate(self):
+        if self.tag_resources:
+            self.tag_resources.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListTagResourcesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         instance_id: str = None,
         password: str = None,
     ):
         # The ID of the instance.
@@ -15285,17 +16135,14 @@
         body: ResetLoginPasswordResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -15317,14 +16164,287 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ResetLoginPasswordResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class TagResourcesRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class TagResourcesRequest(TeaModel):
+    def __init__(
+        self,
+        region_id: str = None,
+        resource_id: List[str] = None,
+        resource_type: str = None,
+        tag: List[TagResourcesRequestTag] = None,
+    ):
+        self.region_id = region_id
+        self.resource_id = resource_id
+        self.resource_type = resource_type
+        self.tag = tag
+
+    def validate(self):
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class TagResourcesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: TagResourcesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        all: bool = None,
+        region_id: str = None,
+        resource_id: List[str] = None,
+        resource_type: str = None,
+        tag_key: List[str] = None,
+    ):
+        self.all = all
+        self.region_id = region_id
+        self.resource_id = resource_id
+        self.resource_type = resource_type
+        self.tag_key = tag_key
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UntagResourcesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UntagResourcesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         chain_config: str = None,
         chain_id: str = None,
         description: str = None,
         instance_id: str = None,
@@ -15434,17 +16554,14 @@
         body: UpdateChainResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -15578,17 +16695,14 @@
         body: UpdateChartNamespaceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -15726,17 +16840,14 @@
         body: UpdateChartRepositoryResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -16018,17 +17129,14 @@
         body: UpdateEventCenterRuleResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -16162,17 +17270,14 @@
         body: UpdateInstanceEndpointStatusResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -16300,17 +17405,14 @@
         body: UpdateNamespaceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -16498,17 +17600,14 @@
         body: UpdateRepoBuildRuleResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -16677,17 +17776,14 @@
         body: UpdateRepoSourceCodeRepoResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -16839,17 +17935,14 @@
         body: UpdateRepoTriggerResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -16991,17 +18084,14 @@
         body: UpdateRepositoryResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
```

### Comparing `alibabacloud_cr20181201-1.2.0/alibabacloud_cr20181201.egg-info/PKG-INFO` & `alibabacloud_cr20181201-1.3.0/alibabacloud_cr20181201.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cr20181201
-Version: 1.2.0
+Version: 1.3.0
 Summary: Alibaba Cloud cr (20181201) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/cr-20181201/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_cr20181201-1.2.0/setup.py` & `alibabacloud_cr20181201-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cr20181201.
 
-Created on 27/09/2023
+Created on 11/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cr20181201"
 NAME = "alibabacloud_cr20181201" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud cr (20181201) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

