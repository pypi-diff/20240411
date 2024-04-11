# Comparing `tmp/alibabacloud_dts20200101_py2-1.3.2.tar.gz` & `tmp/alibabacloud_dts20200101_py2-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dts20200101_py2-1.3.2.tar", last modified: Fri Mar 29 17:29:06 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dts20200101_py2-1.3.3.tar", last modified: Thu Apr 11 17:12:22 2024, max compression
```

## Comparing `alibabacloud_dts20200101_py2-1.3.2.tar` & `alibabacloud_dts20200101_py2-1.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 17:29:06.000000 alibabacloud_dts20200101_py2-1.3.2/
--rw-r--r--   0 root         (0) root         (0)      705 2024-03-29 17:29:05.000000 alibabacloud_dts20200101_py2-1.3.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-29 17:29:05.000000 alibabacloud_dts20200101_py2-1.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-29 17:29:05.000000 alibabacloud_dts20200101_py2-1.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2486 2024-03-29 17:29:06.000000 alibabacloud_dts20200101_py2-1.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2024-03-29 17:29:05.000000 alibabacloud_dts20200101_py2-1.3.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2024-03-29 17:29:05.000000 alibabacloud_dts20200101_py2-1.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 17:29:06.000000 alibabacloud_dts20200101_py2-1.3.2/alibabacloud_dts20200101/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-29 17:29:05.000000 alibabacloud_dts20200101_py2-1.3.2/alibabacloud_dts20200101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   269637 2024-03-29 17:29:05.000000 alibabacloud_dts20200101_py2-1.3.2/alibabacloud_dts20200101/client.py
--rw-r--r--   0 root         (0) root         (0)  1728005 2024-03-29 17:29:05.000000 alibabacloud_dts20200101_py2-1.3.2/alibabacloud_dts20200101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 17:29:06.000000 alibabacloud_dts20200101_py2-1.3.2/alibabacloud_dts20200101_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2486 2024-03-29 17:29:06.000000 alibabacloud_dts20200101_py2-1.3.2/alibabacloud_dts20200101_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2024-03-29 17:29:06.000000 alibabacloud_dts20200101_py2-1.3.2/alibabacloud_dts20200101_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 17:29:06.000000 alibabacloud_dts20200101_py2-1.3.2/alibabacloud_dts20200101_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      347 2024-03-29 17:29:06.000000 alibabacloud_dts20200101_py2-1.3.2/alibabacloud_dts20200101_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-29 17:29:06.000000 alibabacloud_dts20200101_py2-1.3.2/alibabacloud_dts20200101_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-29 17:29:06.000000 alibabacloud_dts20200101_py2-1.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3124 2024-03-29 17:29:05.000000 alibabacloud_dts20200101_py2-1.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/
+-rw-r--r--   0 root         (0) root         (0)     9165 2024-04-11 17:12:21.000000 alibabacloud_dts20200101_py2-1.3.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-11 17:12:21.000000 alibabacloud_dts20200101_py2-1.3.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-11 17:12:21.000000 alibabacloud_dts20200101_py2-1.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2486 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-11 17:12:21.000000 alibabacloud_dts20200101_py2-1.3.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2024-04-11 17:12:21.000000 alibabacloud_dts20200101_py2-1.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 17:12:21.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   269829 2024-04-11 17:12:21.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101/client.py
+-rw-r--r--   0 root         (0) root         (0)  1728431 2024-04-11 17:12:21.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2486 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      347 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 17:12:22.000000 alibabacloud_dts20200101_py2-1.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3124 2024-04-11 17:12:21.000000 alibabacloud_dts20200101_py2-1.3.3/setup.py
```

### Comparing `alibabacloud_dts20200101_py2-1.3.2/LICENSE` & `alibabacloud_dts20200101_py2-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dts20200101_py2-1.3.2/PKG-INFO` & `alibabacloud_dts20200101_py2-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dts20200101_py2
-Version: 1.3.2
+Version: 1.3.3
 Summary: Alibaba Cloud Data Transmission (20200101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dts20200101_py2-1.3.2/README-CN.md` & `alibabacloud_dts20200101_py2-1.3.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dts20200101_py2-1.3.2/README.md` & `alibabacloud_dts20200101_py2-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dts20200101_py2-1.3.2/alibabacloud_dts20200101/client.py` & `alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -5648,14 +5648,18 @@
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

### Comparing `alibabacloud_dts20200101_py2-1.3.2/alibabacloud_dts20200101/models.py` & `alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -36863,16 +36863,16 @@
         if m.get('body') is not None:
             temp_model = TransferInstanceClassResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class TransferPayTypeRequest(TeaModel):
-    def __init__(self, buy_count=None, charge_type=None, dts_job_id=None, period=None, region_id=None,
-                 resource_group_id=None):
+    def __init__(self, buy_count=None, charge_type=None, dts_job_id=None, max_du=None, min_du=None, period=None,
+                 region_id=None, resource_group_id=None):
         # The subscription length.
         # 
         # *   If the **Period** parameter is set to **Year**, the value range is **1** to **5**.
         # *   If the **Period** parameter is set to **Month**, the value range is **1** to **60**.
         # 
         # >  You must specify this parameter only if you set the **ChargeType** parameter to **PrePaid**.
         self.buy_count = buy_count  # type: str
@@ -36883,14 +36883,16 @@
         # 
         # > 
         # *   The billing method of subscription instances cannot be changed to pay-as-you-go. To prevent resource waste, determine whether you need to change the billing method of your resources.
         # *   If you do not need to change the billing method, specify the current billing method.
         self.charge_type = charge_type  # type: str
         # The ID of the data synchronization or change tracking task. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
         self.dts_job_id = dts_job_id  # type: str
+        self.max_du = max_du  # type: int
+        self.min_du = min_du  # type: int
         # The billing cycle of the subscription instance. Valid values:
         # 
         # *   **Year**\
         # *   **Month** (default value)
         # 
         # >  You must specify this parameter only if you set the **ChargeType** parameter to **PrePaid**.
         self.period = period  # type: str
@@ -36909,14 +36911,18 @@
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
@@ -36925,14 +36931,18 @@
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

### Comparing `alibabacloud_dts20200101_py2-1.3.2/alibabacloud_dts20200101_py2.egg-info/PKG-INFO` & `alibabacloud_dts20200101_py2-1.3.3/alibabacloud_dts20200101_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dts20200101-py2
-Version: 1.3.2
+Version: 1.3.3
 Summary: Alibaba Cloud Data Transmission (20200101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dts20200101_py2-1.3.2/setup.py` & `alibabacloud_dts20200101_py2-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dts20200101_py2.
 
-Created on 29/03/2024
+Created on 11/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dts20200101"
 NAME = "alibabacloud_dts20200101_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Data Transmission (20200101) SDK Library for Python2"
```

