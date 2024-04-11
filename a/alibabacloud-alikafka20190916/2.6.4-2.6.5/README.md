# Comparing `tmp/alibabacloud_alikafka20190916-2.6.4.tar.gz` & `tmp/alibabacloud_alikafka20190916-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alikafka20190916-2.6.4.tar", last modified: Wed Apr  3 08:48:04 2024, max compression
+gzip compressed data, was "dist/alibabacloud_alikafka20190916-2.6.5.tar", last modified: Thu Apr 11 17:10:00 2024, max compression
```

## Comparing `alibabacloud_alikafka20190916-2.6.4.tar` & `alibabacloud_alikafka20190916-2.6.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/
--rw-r--r--   0 root         (0) root         (0)     5628 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2440 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/alibabacloud_alikafka20190916/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/alibabacloud_alikafka20190916/__init__.py
--rw-r--r--   0 root         (0) root         (0)   180756 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/alibabacloud_alikafka20190916/client.py
--rw-r--r--   0 root         (0) root         (0)   384021 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/alibabacloud_alikafka20190916/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/alibabacloud_alikafka20190916.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2440 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/alibabacloud_alikafka20190916.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/alibabacloud_alikafka20190916.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/alibabacloud_alikafka20190916.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/alibabacloud_alikafka20190916.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/alibabacloud_alikafka20190916.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2640 2024-04-03 08:48:04.000000 alibabacloud_alikafka20190916-2.6.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/
+-rw-r--r--   0 root         (0) root         (0)     6474 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   181950 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916/client.py
+-rw-r--r--   0 root         (0) root         (0)   395926 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2640 2024-04-11 17:10:00.000000 alibabacloud_alikafka20190916-2.6.5/setup.py
```

### Comparing `alibabacloud_alikafka20190916-2.6.4/ChangeLog.md` & `alibabacloud_alikafka20190916-2.6.5/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+2024-04-03 Version: 2.6.4
+- Update API CreateAcl: add param AclOperationTypes.
+- Update API CreateAcl: add param AclPermissionType.
+- Update API CreateAcl: add param Host.
+- Update API CreateAcl: update param AclOperationType.
+- Update API CreateSaslUser: add param Mechanism.
+- Update API DeleteAcl: add param AclOperationTypes.
+- Update API DeleteAcl: add param AclPermissionType.
+- Update API DeleteAcl: add param Host.
+- Update API DeleteAcl: update param AclOperationType.
+- Update API DeleteSaslUser: add param Mechanism.
+- Update API DescribeAcls: add param AclOperationType.
+- Update API DescribeAcls: add param AclPermissionType.
+- Update API DescribeAcls: add param Host.
+- Update API DescribeAcls: update response param.
+- Update API DescribeSaslUsers: update response param.
+- Update API GetConsumerProgress: update response param.
+
+
 2024-03-25 Version: 2.6.2
 - Update API GetInstanceList: update response param.
 
 
 2024-03-20 Version: 2.6.1
 - Update API CreatePrePayOrder: add param Duration.
 - Update API CreatePrePayOrder: add param PaidType.
```

### Comparing `alibabacloud_alikafka20190916-2.6.4/LICENSE` & `alibabacloud_alikafka20190916-2.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916-2.6.4/PKG-INFO` & `alibabacloud_alikafka20190916-2.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alikafka20190916
-Version: 2.6.4
+Version: 2.6.5
 Summary: Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alikafka20190916-2.6.4/README-CN.md` & `alibabacloud_alikafka20190916-2.6.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916-2.6.4/README.md` & `alibabacloud_alikafka20190916-2.6.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916-2.6.4/alibabacloud_alikafka20190916/client.py` & `alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,44 +387,52 @@
         request: alikafka_20190916_models.CreateConsumerGroupRequest,
     ) -> alikafka_20190916_models.CreateConsumerGroupResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_consumer_group_with_options_async(request, runtime)
 
     def create_post_pay_order_with_options(
         self,
-        request: alikafka_20190916_models.CreatePostPayOrderRequest,
+        tmp_req: alikafka_20190916_models.CreatePostPayOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.CreatePostPayOrderResponse:
         """
         Before you call this operation, make sure that you understand the billing method and pricing of pay-as-you-go Message Queue for Apache Kafka instances. For more information, see [Billing](~~84737~~).
         
-        @param request: CreatePostPayOrderRequest
+        @param tmp_req: CreatePostPayOrderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreatePostPayOrderResponse
         """
-        UtilClient.validate_model(request)
+        UtilClient.validate_model(tmp_req)
+        request = alikafka_20190916_models.CreatePostPayOrderShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.serverless_config):
+            request.serverless_config_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.serverless_config, 'ServerlessConfig', 'json')
         query = {}
         if not UtilClient.is_unset(request.deploy_type):
             query['DeployType'] = request.deploy_type
         if not UtilClient.is_unset(request.disk_size):
             query['DiskSize'] = request.disk_size
         if not UtilClient.is_unset(request.disk_type):
             query['DiskType'] = request.disk_type
         if not UtilClient.is_unset(request.eip_max):
             query['EipMax'] = request.eip_max
         if not UtilClient.is_unset(request.io_max):
             query['IoMax'] = request.io_max
         if not UtilClient.is_unset(request.io_max_spec):
             query['IoMaxSpec'] = request.io_max_spec
+        if not UtilClient.is_unset(request.paid_type):
+            query['PaidType'] = request.paid_type
         if not UtilClient.is_unset(request.partition_num):
             query['PartitionNum'] = request.partition_num
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.serverless_config_shrink):
+            query['ServerlessConfig'] = request.serverless_config_shrink
         if not UtilClient.is_unset(request.spec_type):
             query['SpecType'] = request.spec_type
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         if not UtilClient.is_unset(request.topic_quota):
             query['TopicQuota'] = request.topic_quota
         req = open_api_models.OpenApiRequest(
@@ -444,44 +452,52 @@
         return TeaCore.from_map(
             alikafka_20190916_models.CreatePostPayOrderResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def create_post_pay_order_with_options_async(
         self,
-        request: alikafka_20190916_models.CreatePostPayOrderRequest,
+        tmp_req: alikafka_20190916_models.CreatePostPayOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.CreatePostPayOrderResponse:
         """
         Before you call this operation, make sure that you understand the billing method and pricing of pay-as-you-go Message Queue for Apache Kafka instances. For more information, see [Billing](~~84737~~).
         
-        @param request: CreatePostPayOrderRequest
+        @param tmp_req: CreatePostPayOrderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreatePostPayOrderResponse
         """
-        UtilClient.validate_model(request)
+        UtilClient.validate_model(tmp_req)
+        request = alikafka_20190916_models.CreatePostPayOrderShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.serverless_config):
+            request.serverless_config_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.serverless_config, 'ServerlessConfig', 'json')
         query = {}
         if not UtilClient.is_unset(request.deploy_type):
             query['DeployType'] = request.deploy_type
         if not UtilClient.is_unset(request.disk_size):
             query['DiskSize'] = request.disk_size
         if not UtilClient.is_unset(request.disk_type):
             query['DiskType'] = request.disk_type
         if not UtilClient.is_unset(request.eip_max):
             query['EipMax'] = request.eip_max
         if not UtilClient.is_unset(request.io_max):
             query['IoMax'] = request.io_max
         if not UtilClient.is_unset(request.io_max_spec):
             query['IoMaxSpec'] = request.io_max_spec
+        if not UtilClient.is_unset(request.paid_type):
+            query['PaidType'] = request.paid_type
         if not UtilClient.is_unset(request.partition_num):
             query['PartitionNum'] = request.partition_num
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.serverless_config_shrink):
+            query['ServerlessConfig'] = request.serverless_config_shrink
         if not UtilClient.is_unset(request.spec_type):
             query['SpecType'] = request.spec_type
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         if not UtilClient.is_unset(request.topic_quota):
             query['TopicQuota'] = request.topic_quota
         req = open_api_models.OpenApiRequest(
```

### Comparing `alibabacloud_alikafka20190916-2.6.4/alibabacloud_alikafka20190916/models.py` & `alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -681,14 +681,47 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateConsumerGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreatePostPayOrderRequestServerlessConfig(TeaModel):
+    def __init__(
+        self,
+        reserved_publish_capacity: int = None,
+        reserved_subscribe_capacity: int = None,
+    ):
+        self.reserved_publish_capacity = reserved_publish_capacity
+        self.reserved_subscribe_capacity = reserved_subscribe_capacity
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
+        if self.reserved_publish_capacity is not None:
+            result['ReservedPublishCapacity'] = self.reserved_publish_capacity
+        if self.reserved_subscribe_capacity is not None:
+            result['ReservedSubscribeCapacity'] = self.reserved_subscribe_capacity
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ReservedPublishCapacity') is not None:
+            self.reserved_publish_capacity = m.get('ReservedPublishCapacity')
+        if m.get('ReservedSubscribeCapacity') is not None:
+            self.reserved_subscribe_capacity = m.get('ReservedSubscribeCapacity')
+        return self
+
+
 class CreatePostPayOrderRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
         # The key of tag N.
@@ -733,17 +766,19 @@
         self,
         deploy_type: int = None,
         disk_size: int = None,
         disk_type: str = None,
         eip_max: int = None,
         io_max: int = None,
         io_max_spec: str = None,
+        paid_type: int = None,
         partition_num: int = None,
         region_id: str = None,
         resource_group_id: str = None,
+        serverless_config: CreatePostPayOrderRequestServerlessConfig = None,
         spec_type: str = None,
         tag: List[CreatePostPayOrderRequestTag] = None,
         topic_quota: int = None,
     ):
         # The deployment mode of the instance. Valid values:
         # 
         # *   **4**: deploys the instance that allows access from the Internet and a VPC.
@@ -769,26 +804,28 @@
         # *   For more information about the valid values, see [Billing](~~84737~~).
         self.io_max = io_max
         # The traffic specification of the instance. We recommend that you configure this parameter.
         # 
         # *   You must specify at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you specify only the IoMaxSpec parameter.
         # *   For more information about the valid values, see [Billing](~~84737~~).
         self.io_max_spec = io_max_spec
+        self.paid_type = paid_type
         # The number of partitions. We recommend that you configure this parameter.
         # 
         # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
         # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
         # *   For more information about the valid values, see [Billing](~~84737~~).
         self.partition_num = partition_num
         # The region ID of the instance.
         self.region_id = region_id
         # The ID of the resource group.
         # 
         # If this parameter is left empty, the default resource group is used. You can view the resource group ID on the Resource Group page in the Resource Management console.
         self.resource_group_id = resource_group_id
+        self.serverless_config = serverless_config
         # The edition of the instance. Valid values:
         # 
         # *   **normal**: Standard Edition (High Write)
         # *   **professional**: Professional Edition (High Write)
         # *   **professionalForHighRead**: Professional Edition (High Read)
         # 
         # For more information about these instance editions, see [Billing](~~84737~~).
@@ -800,14 +837,16 @@
         # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
         # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
         # *   The default value of the TopicQuota parameter varies based on the value of the IoMaxSpec parameter. If the number of topics that you consume exceeds the default value, you are charged additional fees.
         # *   For more information about the valid values, see [Billing](~~84737~~).
         self.topic_quota = topic_quota
 
     def validate(self):
+        if self.serverless_config:
+            self.serverless_config.validate()
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
@@ -823,20 +862,24 @@
             result['DiskType'] = self.disk_type
         if self.eip_max is not None:
             result['EipMax'] = self.eip_max
         if self.io_max is not None:
             result['IoMax'] = self.io_max
         if self.io_max_spec is not None:
             result['IoMaxSpec'] = self.io_max_spec
+        if self.paid_type is not None:
+            result['PaidType'] = self.paid_type
         if self.partition_num is not None:
             result['PartitionNum'] = self.partition_num
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
+        if self.serverless_config is not None:
+            result['ServerlessConfig'] = self.serverless_config.to_map()
         if self.spec_type is not None:
             result['SpecType'] = self.spec_type
         result['Tag'] = []
         if self.tag is not None:
             for k in self.tag:
                 result['Tag'].append(k.to_map() if k else None)
         if self.topic_quota is not None:
@@ -853,32 +896,239 @@
             self.disk_type = m.get('DiskType')
         if m.get('EipMax') is not None:
             self.eip_max = m.get('EipMax')
         if m.get('IoMax') is not None:
             self.io_max = m.get('IoMax')
         if m.get('IoMaxSpec') is not None:
             self.io_max_spec = m.get('IoMaxSpec')
+        if m.get('PaidType') is not None:
+            self.paid_type = m.get('PaidType')
         if m.get('PartitionNum') is not None:
             self.partition_num = m.get('PartitionNum')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('ServerlessConfig') is not None:
+            temp_model = CreatePostPayOrderRequestServerlessConfig()
+            self.serverless_config = temp_model.from_map(m['ServerlessConfig'])
         if m.get('SpecType') is not None:
             self.spec_type = m.get('SpecType')
         self.tag = []
         if m.get('Tag') is not None:
             for k in m.get('Tag'):
                 temp_model = CreatePostPayOrderRequestTag()
                 self.tag.append(temp_model.from_map(k))
         if m.get('TopicQuota') is not None:
             self.topic_quota = m.get('TopicQuota')
         return self
 
 
+class CreatePostPayOrderShrinkRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        # The key of tag N.
+        # 
+        # *   Valid values of N: 1 to 20.
+        # *   If this parameter is left empty, the keys of all tags are matched.
+        # *   The tag key must be up to 128 characters in length. It cannot start with acs: or aliyun or contain [http:// or https://.](http://https://。)
+        self.key = key
+        # The value of tag N.
+        # 
+        # *   Valid values of N: 1 to 20.
+        # *   If you do not specify a tag key, you cannot specify a tag value. If this parameter is not configured, all tag values are matched.
+        # *   The tag value must be 1 to 128 characters in length. It cannot start with acs: or aliyun or contain [http:// or https://.](http://https://。)
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
+class CreatePostPayOrderShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        deploy_type: int = None,
+        disk_size: int = None,
+        disk_type: str = None,
+        eip_max: int = None,
+        io_max: int = None,
+        io_max_spec: str = None,
+        paid_type: int = None,
+        partition_num: int = None,
+        region_id: str = None,
+        resource_group_id: str = None,
+        serverless_config_shrink: str = None,
+        spec_type: str = None,
+        tag: List[CreatePostPayOrderShrinkRequestTag] = None,
+        topic_quota: int = None,
+    ):
+        # The deployment mode of the instance. Valid values:
+        # 
+        # *   **4**: deploys the instance that allows access from the Internet and a VPC.
+        # *   **5**: deploys the instance that allows access only from a VPC.
+        self.deploy_type = deploy_type
+        # The disk size.
+        # 
+        # For more information about the valid values, see [Billing](~~84737~~).
+        self.disk_size = disk_size
+        # The disk type. Valid values:
+        # 
+        # *   **0**: ultra disk
+        # *   **1**: standard SSD
+        self.disk_type = disk_type
+        # The Internet traffic for the instance.
+        # 
+        # *   This parameter is required if the **DeployType** parameter is set to **4**.
+        # *   For more information about the valid values, see [Billing](~~84737~~).
+        self.eip_max = eip_max
+        # The maximum traffic for the instance. We recommend that you do not configure this parameter.
+        # 
+        # *   You must specify at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you specify only the IoMaxSpec parameter.
+        # *   For more information about the valid values, see [Billing](~~84737~~).
+        self.io_max = io_max
+        # The traffic specification of the instance. We recommend that you configure this parameter.
+        # 
+        # *   You must specify at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you specify only the IoMaxSpec parameter.
+        # *   For more information about the valid values, see [Billing](~~84737~~).
+        self.io_max_spec = io_max_spec
+        self.paid_type = paid_type
+        # The number of partitions. We recommend that you configure this parameter.
+        # 
+        # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
+        # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
+        # *   For more information about the valid values, see [Billing](~~84737~~).
+        self.partition_num = partition_num
+        # The region ID of the instance.
+        self.region_id = region_id
+        # The ID of the resource group.
+        # 
+        # If this parameter is left empty, the default resource group is used. You can view the resource group ID on the Resource Group page in the Resource Management console.
+        self.resource_group_id = resource_group_id
+        self.serverless_config_shrink = serverless_config_shrink
+        # The edition of the instance. Valid values:
+        # 
+        # *   **normal**: Standard Edition (High Write)
+        # *   **professional**: Professional Edition (High Write)
+        # *   **professionalForHighRead**: Professional Edition (High Read)
+        # 
+        # For more information about these instance editions, see [Billing](~~84737~~).
+        self.spec_type = spec_type
+        # The tags.
+        self.tag = tag
+        # The number of topics. We recommend that you do not configure this parameter.
+        # 
+        # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
+        # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
+        # *   The default value of the TopicQuota parameter varies based on the value of the IoMaxSpec parameter. If the number of topics that you consume exceeds the default value, you are charged additional fees.
+        # *   For more information about the valid values, see [Billing](~~84737~~).
+        self.topic_quota = topic_quota
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
+        if self.deploy_type is not None:
+            result['DeployType'] = self.deploy_type
+        if self.disk_size is not None:
+            result['DiskSize'] = self.disk_size
+        if self.disk_type is not None:
+            result['DiskType'] = self.disk_type
+        if self.eip_max is not None:
+            result['EipMax'] = self.eip_max
+        if self.io_max is not None:
+            result['IoMax'] = self.io_max
+        if self.io_max_spec is not None:
+            result['IoMaxSpec'] = self.io_max_spec
+        if self.paid_type is not None:
+            result['PaidType'] = self.paid_type
+        if self.partition_num is not None:
+            result['PartitionNum'] = self.partition_num
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
+        if self.serverless_config_shrink is not None:
+            result['ServerlessConfig'] = self.serverless_config_shrink
+        if self.spec_type is not None:
+            result['SpecType'] = self.spec_type
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
+        if self.topic_quota is not None:
+            result['TopicQuota'] = self.topic_quota
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DeployType') is not None:
+            self.deploy_type = m.get('DeployType')
+        if m.get('DiskSize') is not None:
+            self.disk_size = m.get('DiskSize')
+        if m.get('DiskType') is not None:
+            self.disk_type = m.get('DiskType')
+        if m.get('EipMax') is not None:
+            self.eip_max = m.get('EipMax')
+        if m.get('IoMax') is not None:
+            self.io_max = m.get('IoMax')
+        if m.get('IoMaxSpec') is not None:
+            self.io_max_spec = m.get('IoMaxSpec')
+        if m.get('PaidType') is not None:
+            self.paid_type = m.get('PaidType')
+        if m.get('PartitionNum') is not None:
+            self.partition_num = m.get('PartitionNum')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('ServerlessConfig') is not None:
+            self.serverless_config_shrink = m.get('ServerlessConfig')
+        if m.get('SpecType') is not None:
+            self.spec_type = m.get('SpecType')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = CreatePostPayOrderShrinkRequestTag()
+                self.tag.append(temp_model.from_map(k))
+        if m.get('TopicQuota') is not None:
+            self.topic_quota = m.get('TopicQuota')
+        return self
+
+
 class CreatePostPayOrderResponseBody(TeaModel):
     def __init__(
         self,
         code: int = None,
         message: str = None,
         order_id: str = None,
         request_id: str = None,
@@ -5133,15 +5383,17 @@
         disk_type: int = None,
         domain_endpoint: str = None,
         eip_max: int = None,
         end_point: str = None,
         expired_time: int = None,
         instance_id: str = None,
         io_max: int = None,
+        io_max_read: int = None,
         io_max_spec: str = None,
+        io_max_write: int = None,
         kms_key_id: str = None,
         msg_retain: int = None,
         name: str = None,
         paid_type: int = None,
         region_id: str = None,
         reserved_publish_capacity: int = None,
         reserved_subscribe_capacity: int = None,
@@ -5195,16 +5447,18 @@
         self.end_point = end_point
         # The time when the instance expires. Unit: milliseconds.
         self.expired_time = expired_time
         # The instance ID.
         self.instance_id = instance_id
         # The peak traffic allowed for the instance.
         self.io_max = io_max
+        self.io_max_read = io_max_read
         # The traffic specification.
         self.io_max_spec = io_max_spec
+        self.io_max_write = io_max_write
         # The ID of the key that is used for disk encryption in the region where the instance is deployed.
         self.kms_key_id = kms_key_id
         # The retention period of messages in the instance. Unit: hours.
         self.msg_retain = msg_retain
         # The instance name.
         self.name = name
         # The billing method of the instance. Valid values:
@@ -5315,16 +5569,20 @@
             result['EndPoint'] = self.end_point
         if self.expired_time is not None:
             result['ExpiredTime'] = self.expired_time
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.io_max is not None:
             result['IoMax'] = self.io_max
+        if self.io_max_read is not None:
+            result['IoMaxRead'] = self.io_max_read
         if self.io_max_spec is not None:
             result['IoMaxSpec'] = self.io_max_spec
+        if self.io_max_write is not None:
+            result['IoMaxWrite'] = self.io_max_write
         if self.kms_key_id is not None:
             result['KmsKeyId'] = self.kms_key_id
         if self.msg_retain is not None:
             result['MsgRetain'] = self.msg_retain
         if self.name is not None:
             result['Name'] = self.name
         if self.paid_type is not None:
@@ -5396,16 +5654,20 @@
             self.end_point = m.get('EndPoint')
         if m.get('ExpiredTime') is not None:
             self.expired_time = m.get('ExpiredTime')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('IoMax') is not None:
             self.io_max = m.get('IoMax')
+        if m.get('IoMaxRead') is not None:
+            self.io_max_read = m.get('IoMaxRead')
         if m.get('IoMaxSpec') is not None:
             self.io_max_spec = m.get('IoMaxSpec')
+        if m.get('IoMaxWrite') is not None:
+            self.io_max_write = m.get('IoMaxWrite')
         if m.get('KmsKeyId') is not None:
             self.kms_key_id = m.get('KmsKeyId')
         if m.get('MsgRetain') is not None:
             self.msg_retain = m.get('MsgRetain')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('PaidType') is not None:
```

### Comparing `alibabacloud_alikafka20190916-2.6.4/alibabacloud_alikafka20190916.egg-info/PKG-INFO` & `alibabacloud_alikafka20190916-2.6.5/alibabacloud_alikafka20190916.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alikafka20190916
-Version: 2.6.4
+Version: 2.6.5
 Summary: Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alikafka20190916-2.6.4/setup.py` & `alibabacloud_alikafka20190916-2.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alikafka20190916.
 
-Created on 03/04/2024
+Created on 11/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alikafka20190916"
 NAME = "alibabacloud_alikafka20190916" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python"
```

