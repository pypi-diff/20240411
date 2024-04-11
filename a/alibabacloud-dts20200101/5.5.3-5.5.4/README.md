# Comparing `tmp/alibabacloud_dts20200101-5.5.3.tar.gz` & `tmp/alibabacloud_dts20200101-5.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dts20200101-5.5.3.tar", last modified: Fri Mar 29 17:26:13 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dts20200101-5.5.4.tar", last modified: Thu Apr 11 17:13:09 2024, max compression
```

## Comparing `alibabacloud_dts20200101-5.5.3.tar` & `alibabacloud_dts20200101-5.5.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 17:26:13.000000 alibabacloud_dts20200101-5.5.3/
--rw-r--r--   0 root         (0) root         (0)     1302 2024-03-29 17:26:12.000000 alibabacloud_dts20200101-5.5.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-29 17:26:12.000000 alibabacloud_dts20200101-5.5.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-29 17:26:12.000000 alibabacloud_dts20200101-5.5.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2415 2024-03-29 17:26:13.000000 alibabacloud_dts20200101-5.5.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-03-29 17:26:12.000000 alibabacloud_dts20200101-5.5.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-03-29 17:26:12.000000 alibabacloud_dts20200101-5.5.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 17:26:13.000000 alibabacloud_dts20200101-5.5.3/alibabacloud_dts20200101/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-29 17:26:12.000000 alibabacloud_dts20200101-5.5.3/alibabacloud_dts20200101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   605374 2024-03-29 17:26:12.000000 alibabacloud_dts20200101-5.5.3/alibabacloud_dts20200101/client.py
--rw-r--r--   0 root         (0) root         (0)  1711295 2024-03-29 17:26:12.000000 alibabacloud_dts20200101-5.5.3/alibabacloud_dts20200101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 17:26:13.000000 alibabacloud_dts20200101-5.5.3/alibabacloud_dts20200101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2415 2024-03-29 17:26:13.000000 alibabacloud_dts20200101-5.5.3/alibabacloud_dts20200101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-03-29 17:26:13.000000 alibabacloud_dts20200101-5.5.3/alibabacloud_dts20200101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 17:26:13.000000 alibabacloud_dts20200101-5.5.3/alibabacloud_dts20200101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      316 2024-03-29 17:26:13.000000 alibabacloud_dts20200101-5.5.3/alibabacloud_dts20200101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-29 17:26:13.000000 alibabacloud_dts20200101-5.5.3/alibabacloud_dts20200101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-29 17:26:13.000000 alibabacloud_dts20200101-5.5.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2816 2024-03-29 17:26:12.000000 alibabacloud_dts20200101-5.5.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/
+-rw-r--r--   0 root         (0) root         (0)     9762 2024-04-11 17:13:08.000000 alibabacloud_dts20200101-5.5.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-11 17:13:08.000000 alibabacloud_dts20200101-5.5.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-11 17:13:08.000000 alibabacloud_dts20200101-5.5.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-11 17:13:08.000000 alibabacloud_dts20200101-5.5.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-04-11 17:13:08.000000 alibabacloud_dts20200101-5.5.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 17:13:08.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   605758 2024-04-11 17:13:08.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101/client.py
+-rw-r--r--   0 root         (0) root         (0)  1711725 2024-04-11 17:13:08.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 17:13:09.000000 alibabacloud_dts20200101-5.5.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2816 2024-04-11 17:13:08.000000 alibabacloud_dts20200101-5.5.4/setup.py
```

### Comparing `alibabacloud_dts20200101-5.5.3/LICENSE` & `alibabacloud_dts20200101-5.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dts20200101-5.5.3/PKG-INFO` & `alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_dts20200101
-Version: 5.5.3
+Name: alibabacloud-dts20200101
+Version: 5.5.4
 Summary: Alibaba Cloud Data Transmission (20200101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dts20200101-5.5.3/README-CN.md` & `alibabacloud_dts20200101-5.5.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dts20200101-5.5.3/README.md` & `alibabacloud_dts20200101-5.5.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dts20200101-5.5.3/alibabacloud_dts20200101/client.py` & `alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -12323,14 +12323,18 @@
         query = {}
         if not UtilClient.is_unset(request.buy_count):
             query['BuyCount'] = request.buy_count
         if not UtilClient.is_unset(request.charge_type):
             query['ChargeType'] = request.charge_type
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
+        if not UtilClient.is_unset(request.max_du):
+            query['MaxDu'] = request.max_du
+        if not UtilClient.is_unset(request.min_du):
+            query['MinDu'] = request.min_du
         if not UtilClient.is_unset(request.period):
             query['Period'] = request.period
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
@@ -12371,14 +12375,18 @@
         query = {}
         if not UtilClient.is_unset(request.buy_count):
             query['BuyCount'] = request.buy_count
         if not UtilClient.is_unset(request.charge_type):
             query['ChargeType'] = request.charge_type
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
+        if not UtilClient.is_unset(request.max_du):
+            query['MaxDu'] = request.max_du
+        if not UtilClient.is_unset(request.min_du):
+            query['MinDu'] = request.min_du
         if not UtilClient.is_unset(request.period):
             query['Period'] = request.period
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
```

### Comparing `alibabacloud_dts20200101-5.5.3/alibabacloud_dts20200101/models.py` & `alibabacloud_dts20200101-5.5.4/alibabacloud_dts20200101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -41390,14 +41390,16 @@
 
 class TransferPayTypeRequest(TeaModel):
     def __init__(
         self,
         buy_count: str = None,
         charge_type: str = None,
         dts_job_id: str = None,
+        max_du: int = None,
+        min_du: int = None,
         period: str = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
         # The subscription length.
         # 
         # *   If the **Period** parameter is set to **Year**, the value range is **1** to **5**.
@@ -41412,14 +41414,16 @@
         # 
         # > 
         # *   The billing method of subscription instances cannot be changed to pay-as-you-go. To prevent resource waste, determine whether you need to change the billing method of your resources.
         # *   If you do not need to change the billing method, specify the current billing method.
         self.charge_type = charge_type
         # The ID of the data synchronization or change tracking task. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
         self.dts_job_id = dts_job_id
+        self.max_du = max_du
+        self.min_du = min_du
         # The billing cycle of the subscription instance. Valid values:
         # 
         # *   **Year**\
         # *   **Month** (default value)
         # 
         # >  You must specify this parameter only if you set the **ChargeType** parameter to **PrePaid**.
         self.period = period
@@ -41438,14 +41442,18 @@
         result = dict()
         if self.buy_count is not None:
             result['BuyCount'] = self.buy_count
         if self.charge_type is not None:
             result['ChargeType'] = self.charge_type
         if self.dts_job_id is not None:
             result['DtsJobId'] = self.dts_job_id
+        if self.max_du is not None:
+            result['MaxDu'] = self.max_du
+        if self.min_du is not None:
+            result['MinDu'] = self.min_du
         if self.period is not None:
             result['Period'] = self.period
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         return result
@@ -41454,14 +41462,18 @@
         m = m or dict()
         if m.get('BuyCount') is not None:
             self.buy_count = m.get('BuyCount')
         if m.get('ChargeType') is not None:
             self.charge_type = m.get('ChargeType')
         if m.get('DtsJobId') is not None:
             self.dts_job_id = m.get('DtsJobId')
+        if m.get('MaxDu') is not None:
+            self.max_du = m.get('MaxDu')
+        if m.get('MinDu') is not None:
+            self.min_du = m.get('MinDu')
         if m.get('Period') is not None:
             self.period = m.get('Period')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         return self
```

### Comparing `alibabacloud_dts20200101-5.5.3/alibabacloud_dts20200101.egg-info/PKG-INFO` & `alibabacloud_dts20200101-5.5.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-dts20200101
-Version: 5.5.3
+Name: alibabacloud_dts20200101
+Version: 5.5.4
 Summary: Alibaba Cloud Data Transmission (20200101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dts20200101-5.5.3/setup.py` & `alibabacloud_dts20200101-5.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dts20200101.
 
-Created on 29/03/2024
+Created on 11/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dts20200101"
 NAME = "alibabacloud_dts20200101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Data Transmission (20200101) SDK Library for Python"
```

