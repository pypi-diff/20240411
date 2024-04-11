# Comparing `tmp/alibabacloud_alikafka20190916_py2-2.6.4.tar.gz` & `tmp/alibabacloud_alikafka20190916_py2-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alikafka20190916_py2-2.6.4.tar", last modified: Wed Apr  3 08:47:05 2024, max compression
+gzip compressed data, was "dist/alibabacloud_alikafka20190916_py2-2.6.5.tar", last modified: Thu Apr 11 17:09:45 2024, max compression
```

## Comparing `alibabacloud_alikafka20190916_py2-2.6.4.tar` & `alibabacloud_alikafka20190916_py2-2.6.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/
--rw-r--r--   0 root         (0) root         (0)     5371 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2506 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/alibabacloud_alikafka20190916/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/alibabacloud_alikafka20190916/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77337 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/alibabacloud_alikafka20190916/client.py
--rw-r--r--   0 root         (0) root         (0)   385713 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/alibabacloud_alikafka20190916/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/alibabacloud_alikafka20190916_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2506 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/alibabacloud_alikafka20190916_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/alibabacloud_alikafka20190916_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/alibabacloud_alikafka20190916_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/alibabacloud_alikafka20190916_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/alibabacloud_alikafka20190916_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2932 2024-04-03 08:47:05.000000 alibabacloud_alikafka20190916_py2-2.6.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/
+-rw-r--r--   0 root         (0) root         (0)     6217 2024-04-11 17:09:44.000000 alibabacloud_alikafka20190916_py2-2.6.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-11 17:09:44.000000 alibabacloud_alikafka20190916_py2-2.6.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-11 17:09:44.000000 alibabacloud_alikafka20190916_py2-2.6.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2506 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-04-11 17:09:44.000000 alibabacloud_alikafka20190916_py2-2.6.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-11 17:09:44.000000 alibabacloud_alikafka20190916_py2-2.6.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 17:09:44.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77934 2024-04-11 17:09:44.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916/client.py
+-rw-r--r--   0 root         (0) root         (0)   397682 2024-04-11 17:09:44.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2506 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 17:09:45.000000 alibabacloud_alikafka20190916_py2-2.6.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2932 2024-04-11 17:09:44.000000 alibabacloud_alikafka20190916_py2-2.6.5/setup.py
```

### Comparing `alibabacloud_alikafka20190916_py2-2.6.4/ChangeLog.md` & `alibabacloud_alikafka20190916_py2-2.6.5/ChangeLog.md`

 * *Files 12% similar despite different names*

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

### Comparing `alibabacloud_alikafka20190916_py2-2.6.4/LICENSE` & `alibabacloud_alikafka20190916_py2-2.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916_py2-2.6.4/PKG-INFO` & `alibabacloud_alikafka20190916_py2-2.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alikafka20190916_py2
-Version: 2.6.4
+Version: 2.6.5
 Summary: Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alikafka20190916_py2-2.6.4/README-CN.md` & `alibabacloud_alikafka20190916_py2-2.6.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916_py2-2.6.4/README.md` & `alibabacloud_alikafka20190916_py2-2.6.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916_py2-2.6.4/alibabacloud_alikafka20190916/client.py` & `alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,45 +172,53 @@
             self.call_api(params, req, runtime)
         )
 
     def create_consumer_group(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_consumer_group_with_options(request, runtime)
 
-    def create_post_pay_order_with_options(self, request, runtime):
+    def create_post_pay_order_with_options(self, tmp_req, runtime):
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

### Comparing `alibabacloud_alikafka20190916_py2-2.6.4/alibabacloud_alikafka20190916/models.py` & `alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -603,14 +603,43 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateConsumerGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreatePostPayOrderRequestServerlessConfig(TeaModel):
+    def __init__(self, reserved_publish_capacity=None, reserved_subscribe_capacity=None):
+        self.reserved_publish_capacity = reserved_publish_capacity  # type: long
+        self.reserved_subscribe_capacity = reserved_subscribe_capacity  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreatePostPayOrderRequestServerlessConfig, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ReservedPublishCapacity') is not None:
+            self.reserved_publish_capacity = m.get('ReservedPublishCapacity')
+        if m.get('ReservedSubscribeCapacity') is not None:
+            self.reserved_subscribe_capacity = m.get('ReservedSubscribeCapacity')
+        return self
+
+
 class CreatePostPayOrderRequestTag(TeaModel):
     def __init__(self, key=None, value=None):
         # The key of tag N.
         # 
         # *   Valid values of N: 1 to 20.
         # *   If this parameter is left empty, the keys of all tags are matched.
         # *   The tag key must be up to 128 characters in length. It cannot start with acs: or aliyun or contain [http:// or https://.](http://https://。)
@@ -644,15 +673,16 @@
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class CreatePostPayOrderRequest(TeaModel):
     def __init__(self, deploy_type=None, disk_size=None, disk_type=None, eip_max=None, io_max=None, io_max_spec=None,
-                 partition_num=None, region_id=None, resource_group_id=None, spec_type=None, tag=None, topic_quota=None):
+                 paid_type=None, partition_num=None, region_id=None, resource_group_id=None, serverless_config=None,
+                 spec_type=None, tag=None, topic_quota=None):
         # The deployment mode of the instance. Valid values:
         # 
         # *   **4**: deploys the instance that allows access from the Internet and a VPC.
         # *   **5**: deploys the instance that allows access only from a VPC.
         self.deploy_type = deploy_type  # type: int
         # The disk size.
         # 
@@ -674,26 +704,28 @@
         # *   For more information about the valid values, see [Billing](~~84737~~).
         self.io_max = io_max  # type: int
         # The traffic specification of the instance. We recommend that you configure this parameter.
         # 
         # *   You must specify at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you specify only the IoMaxSpec parameter.
         # *   For more information about the valid values, see [Billing](~~84737~~).
         self.io_max_spec = io_max_spec  # type: str
+        self.paid_type = paid_type  # type: int
         # The number of partitions. We recommend that you configure this parameter.
         # 
         # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
         # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
         # *   For more information about the valid values, see [Billing](~~84737~~).
         self.partition_num = partition_num  # type: int
         # The region ID of the instance.
         self.region_id = region_id  # type: str
         # The ID of the resource group.
         # 
         # If this parameter is left empty, the default resource group is used. You can view the resource group ID on the Resource Group page in the Resource Management console.
         self.resource_group_id = resource_group_id  # type: str
+        self.serverless_config = serverless_config  # type: CreatePostPayOrderRequestServerlessConfig
         # The edition of the instance. Valid values:
         # 
         # *   **normal**: Standard Edition (High Write)
         # *   **professional**: Professional Edition (High Write)
         # *   **professionalForHighRead**: Professional Edition (High Read)
         # 
         # For more information about these instance editions, see [Billing](~~84737~~).
@@ -705,14 +737,16 @@
         # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
         # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
         # *   The default value of the TopicQuota parameter varies based on the value of the IoMaxSpec parameter. If the number of topics that you consume exceeds the default value, you are charged additional fees.
         # *   For more information about the valid values, see [Billing](~~84737~~).
         self.topic_quota = topic_quota  # type: int
 
     def validate(self):
+        if self.serverless_config:
+            self.serverless_config.validate()
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super(CreatePostPayOrderRequest, self).to_map()
@@ -728,20 +762,24 @@
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
@@ -758,32 +796,221 @@
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
+    def __init__(self, key=None, value=None):
+        # The key of tag N.
+        # 
+        # *   Valid values of N: 1 to 20.
+        # *   If this parameter is left empty, the keys of all tags are matched.
+        # *   The tag key must be up to 128 characters in length. It cannot start with acs: or aliyun or contain [http:// or https://.](http://https://。)
+        self.key = key  # type: str
+        # The value of tag N.
+        # 
+        # *   Valid values of N: 1 to 20.
+        # *   If you do not specify a tag key, you cannot specify a tag value. If this parameter is not configured, all tag values are matched.
+        # *   The tag value must be 1 to 128 characters in length. It cannot start with acs: or aliyun or contain [http:// or https://.](http://https://。)
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreatePostPayOrderShrinkRequestTag, self).to_map()
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
+class CreatePostPayOrderShrinkRequest(TeaModel):
+    def __init__(self, deploy_type=None, disk_size=None, disk_type=None, eip_max=None, io_max=None, io_max_spec=None,
+                 paid_type=None, partition_num=None, region_id=None, resource_group_id=None, serverless_config_shrink=None,
+                 spec_type=None, tag=None, topic_quota=None):
+        # The deployment mode of the instance. Valid values:
+        # 
+        # *   **4**: deploys the instance that allows access from the Internet and a VPC.
+        # *   **5**: deploys the instance that allows access only from a VPC.
+        self.deploy_type = deploy_type  # type: int
+        # The disk size.
+        # 
+        # For more information about the valid values, see [Billing](~~84737~~).
+        self.disk_size = disk_size  # type: int
+        # The disk type. Valid values:
+        # 
+        # *   **0**: ultra disk
+        # *   **1**: standard SSD
+        self.disk_type = disk_type  # type: str
+        # The Internet traffic for the instance.
+        # 
+        # *   This parameter is required if the **DeployType** parameter is set to **4**.
+        # *   For more information about the valid values, see [Billing](~~84737~~).
+        self.eip_max = eip_max  # type: int
+        # The maximum traffic for the instance. We recommend that you do not configure this parameter.
+        # 
+        # *   You must specify at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you specify only the IoMaxSpec parameter.
+        # *   For more information about the valid values, see [Billing](~~84737~~).
+        self.io_max = io_max  # type: int
+        # The traffic specification of the instance. We recommend that you configure this parameter.
+        # 
+        # *   You must specify at least one of the IoMax and IoMaxSpec parameters. If you configure both parameters, the value of the IoMaxSpec parameter takes effect. We recommend that you specify only the IoMaxSpec parameter.
+        # *   For more information about the valid values, see [Billing](~~84737~~).
+        self.io_max_spec = io_max_spec  # type: str
+        self.paid_type = paid_type  # type: int
+        # The number of partitions. We recommend that you configure this parameter.
+        # 
+        # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
+        # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
+        # *   For more information about the valid values, see [Billing](~~84737~~).
+        self.partition_num = partition_num  # type: int
+        # The region ID of the instance.
+        self.region_id = region_id  # type: str
+        # The ID of the resource group.
+        # 
+        # If this parameter is left empty, the default resource group is used. You can view the resource group ID on the Resource Group page in the Resource Management console.
+        self.resource_group_id = resource_group_id  # type: str
+        self.serverless_config_shrink = serverless_config_shrink  # type: str
+        # The edition of the instance. Valid values:
+        # 
+        # *   **normal**: Standard Edition (High Write)
+        # *   **professional**: Professional Edition (High Write)
+        # *   **professionalForHighRead**: Professional Edition (High Read)
+        # 
+        # For more information about these instance editions, see [Billing](~~84737~~).
+        self.spec_type = spec_type  # type: str
+        # The tags.
+        self.tag = tag  # type: list[CreatePostPayOrderShrinkRequestTag]
+        # The number of topics. We recommend that you do not configure this parameter.
+        # 
+        # *   You must specify at least one of the PartitionNum and TopicQuota parameters. We recommend that you configure only the PartitionNum parameter.
+        # *   If you specify both parameters, the topic-based sales model is used to check whether the PartitionNum value and the TopicQuota value are the same. If they are not the same, a failure response is returned. If they are the same, the order is placed based on the PartitionNum value.
+        # *   The default value of the TopicQuota parameter varies based on the value of the IoMaxSpec parameter. If the number of topics that you consume exceeds the default value, you are charged additional fees.
+        # *   For more information about the valid values, see [Billing](~~84737~~).
+        self.topic_quota = topic_quota  # type: int
+
+    def validate(self):
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(CreatePostPayOrderShrinkRequest, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, code=None, message=None, order_id=None, request_id=None, success=None):
         # The HTTP status code returned. The HTTP status code 200 indicates that the request is successful.
         self.code = code  # type: int
         # The message returned.
         self.message = message  # type: str
         # The ID of the order.
@@ -4552,20 +4779,20 @@
             self.current_2open_source_version = m.get('Current2OpenSourceVersion')
         return self
 
 
 class GetInstanceListResponseBodyInstanceListInstanceVO(TeaModel):
     def __init__(self, all_config=None, confluent_config=None, create_time=None, deploy_type=None, disk_size=None,
                  disk_type=None, domain_endpoint=None, eip_max=None, end_point=None, expired_time=None, instance_id=None,
-                 io_max=None, io_max_spec=None, kms_key_id=None, msg_retain=None, name=None, paid_type=None, region_id=None,
-                 reserved_publish_capacity=None, reserved_subscribe_capacity=None, resource_group_id=None, sasl_domain_endpoint=None,
-                 security_group=None, service_status=None, spec_type=None, ssl_domain_endpoint=None, ssl_end_point=None,
-                 standard_zone_id=None, tags=None, topic_num_limit=None, upgrade_service_detail_info=None, used_group_count=None,
-                 used_partition_count=None, used_topic_count=None, v_switch_id=None, view_instance_status_code=None, vpc_id=None,
-                 zone_id=None):
+                 io_max=None, io_max_read=None, io_max_spec=None, io_max_write=None, kms_key_id=None, msg_retain=None,
+                 name=None, paid_type=None, region_id=None, reserved_publish_capacity=None,
+                 reserved_subscribe_capacity=None, resource_group_id=None, sasl_domain_endpoint=None, security_group=None, service_status=None,
+                 spec_type=None, ssl_domain_endpoint=None, ssl_end_point=None, standard_zone_id=None, tags=None,
+                 topic_num_limit=None, upgrade_service_detail_info=None, used_group_count=None, used_partition_count=None,
+                 used_topic_count=None, v_switch_id=None, view_instance_status_code=None, vpc_id=None, zone_id=None):
         # The configurations of the deployed ApsaraMQ for Kafka instance.
         self.all_config = all_config  # type: str
         self.confluent_config = confluent_config  # type: GetInstanceListResponseBodyInstanceListInstanceVOConfluentConfig
         # The time when the instance was created. Unit: milliseconds.
         self.create_time = create_time  # type: long
         # The type of the network in which the instance is deployed. Valid values:
         # 
@@ -4593,16 +4820,18 @@
         self.end_point = end_point  # type: str
         # The time when the instance expires. Unit: milliseconds.
         self.expired_time = expired_time  # type: long
         # The instance ID.
         self.instance_id = instance_id  # type: str
         # The peak traffic allowed for the instance.
         self.io_max = io_max  # type: int
+        self.io_max_read = io_max_read  # type: int
         # The traffic specification.
         self.io_max_spec = io_max_spec  # type: str
+        self.io_max_write = io_max_write  # type: int
         # The ID of the key that is used for disk encryption in the region where the instance is deployed.
         self.kms_key_id = kms_key_id  # type: str
         # The retention period of messages in the instance. Unit: hours.
         self.msg_retain = msg_retain  # type: int
         # The instance name.
         self.name = name  # type: str
         # The billing method of the instance. Valid values:
@@ -4713,16 +4942,20 @@
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
@@ -4794,16 +5027,20 @@
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

### Comparing `alibabacloud_alikafka20190916_py2-2.6.4/alibabacloud_alikafka20190916_py2.egg-info/PKG-INFO` & `alibabacloud_alikafka20190916_py2-2.6.5/alibabacloud_alikafka20190916_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alikafka20190916-py2
-Version: 2.6.4
+Version: 2.6.5
 Summary: Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alikafka20190916_py2-2.6.4/setup.py` & `alibabacloud_alikafka20190916_py2-2.6.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alikafka20190916_py2.
 
-Created on 03/04/2024
+Created on 11/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alikafka20190916"
 NAME = "alibabacloud_alikafka20190916_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python2"
```

