# Comparing `tmp/alibabacloud_aligenieiap_1_0-1.1.0.tar.gz` & `tmp/alibabacloud_aligenieiap_1_0-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aligenieiap_1_0-1.1.0.tar", last modified: Fri Mar 29 08:53:54 2024, max compression
+gzip compressed data, was "dist/alibabacloud_aligenieiap_1_0-1.1.1.tar", last modified: Thu Apr 11 09:59:27 2024, max compression
```

## Comparing `alibabacloud_aligenieiap_1_0-1.1.0.tar` & `alibabacloud_aligenieiap_1_0-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/
--rw-r--r--   0 root         (0) root         (0)      369 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2430 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1112 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1197 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/alibabacloud_aligenieiap_1_0/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/alibabacloud_aligenieiap_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89920 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/alibabacloud_aligenieiap_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   164423 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/alibabacloud_aligenieiap_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/alibabacloud_aligenieiap_1_0.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2430 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/alibabacloud_aligenieiap_1_0.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/alibabacloud_aligenieiap_1_0.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/alibabacloud_aligenieiap_1_0.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      194 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/alibabacloud_aligenieiap_1_0.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/alibabacloud_aligenieiap_1_0.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2680 2024-03-29 08:53:54.000000 alibabacloud_aligenieiap_1_0-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:59:27.000000 alibabacloud_aligenieiap_1_0-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)      428 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2430 2024-04-11 09:59:27.000000 alibabacloud_aligenieiap_1_0-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:59:27.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81284 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   164650 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:59:27.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2430 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-11 09:59:27.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 09:59:27.000000 alibabacloud_aligenieiap_1_0-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/setup.py
```

### Comparing `alibabacloud_aligenieiap_1_0-1.1.0/LICENSE` & `alibabacloud_aligenieiap_1_0-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0-1.1.0/PKG-INFO` & `alibabacloud_aligenieiap_1_0-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aligenieiap_1_0
-Version: 1.1.0
+Version: 1.1.1
 Summary: Alibaba Cloud AliGenie (iap_1_0) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aligenieiap_1_0-1.1.0/README-CN.md` & `alibabacloud_aligenieiap_1_0-1.1.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0-1.1.0/README.md` & `alibabacloud_aligenieiap_1_0-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0-1.1.0/alibabacloud_aligenieiap_1_0/client.py` & `alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,49 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
+from typing import Dict
 from Tea.core import TeaCore
 
-from alibabacloud_gateway_spi.client import Client as SPIClient
 from alibabacloud_tea_openapi.client import Client as OpenApiClient
 from alibabacloud_tea_openapi import models as open_api_models
-from alibabacloud_gateway_pop.client import Client as GatewayClientClient
 from alibabacloud_tea_util.client import Client as UtilClient
+from alibabacloud_endpoint_util.client import Client as EndpointUtilClient
 from alibabacloud_aligenieiap_1_0 import models as ali_genieiap__1__0_models
 from alibabacloud_tea_util import models as util_models
 from alibabacloud_openapi_util.client import Client as OpenApiUtilClient
 
 
 class Client(OpenApiClient):
     """
     *\
     """
-    _client: SPIClient = None
-
     def __init__(
         self, 
         config: open_api_models.Config,
     ):
         super().__init__(config)
-        self._product_id = 'AliGenie'
-        self._client = GatewayClientClient()
-        self._spi = self._client
         self._endpoint_rule = ''
-        if UtilClient.empty(self._endpoint):
-            self._endpoint = 'openapi.aligenie.com/v1.0/iap'
+        self.check_config(config)
+        self._endpoint = self.get_endpoint('aligenie', self._region_id, self._endpoint_rule, self._network, self._suffix, self._endpoint_map, self._endpoint)
+
+    def get_endpoint(
+        self,
+        product_id: str,
+        region_id: str,
+        endpoint_rule: str,
+        network: str,
+        suffix: str,
+        endpoint_map: Dict[str, str],
+        endpoint: str,
+    ) -> str:
+        if not UtilClient.empty(endpoint):
+            return endpoint
+        if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
+            return endpoint_map.get(region_id)
+        return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def app_use_time_report_with_options(
         self,
         tmp_req: ali_genieiap__1__0_models.AppUseTimeReportRequest,
         headers: ali_genieiap__1__0_models.AppUseTimeReportHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_genieiap__1__0_models.AppUseTimeReportResponse:
@@ -70,24 +81,18 @@
             pathname=f'/v1.0/iap/vip/use/time/report',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='formData',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.AppUseTimeReportResponse(),
-                self.call_api(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.AppUseTimeReportResponse(),
-                self.execute(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.AppUseTimeReportResponse(),
+            self.call_api(params, req, runtime)
+        )
 
     async def app_use_time_report_with_options_async(
         self,
         tmp_req: ali_genieiap__1__0_models.AppUseTimeReportRequest,
         headers: ali_genieiap__1__0_models.AppUseTimeReportHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_genieiap__1__0_models.AppUseTimeReportResponse:
@@ -125,24 +130,18 @@
             pathname=f'/v1.0/iap/vip/use/time/report',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='formData',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.AppUseTimeReportResponse(),
-                await self.call_api_async(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.AppUseTimeReportResponse(),
-                await self.execute_async(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.AppUseTimeReportResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
 
     def app_use_time_report(
         self,
         request: ali_genieiap__1__0_models.AppUseTimeReportRequest,
     ) -> ali_genieiap__1__0_models.AppUseTimeReportResponse:
         runtime = util_models.RuntimeOptions()
         headers = ali_genieiap__1__0_models.AppUseTimeReportHeaders()
@@ -196,24 +195,18 @@
             pathname=f'/v1.0/iap/reminder/create',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='formData',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.CreateReminderResponse(),
-                self.call_api(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.CreateReminderResponse(),
-                self.execute(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.CreateReminderResponse(),
+            self.call_api(params, req, runtime)
+        )
 
     async def create_reminder_with_options_async(
         self,
         tmp_req: ali_genieiap__1__0_models.CreateReminderRequest,
         headers: ali_genieiap__1__0_models.CreateReminderHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_genieiap__1__0_models.CreateReminderResponse:
@@ -251,24 +244,18 @@
             pathname=f'/v1.0/iap/reminder/create',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='formData',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.CreateReminderResponse(),
-                await self.call_api_async(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.CreateReminderResponse(),
-                await self.execute_async(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.CreateReminderResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
 
     def create_reminder(
         self,
         request: ali_genieiap__1__0_models.CreateReminderRequest,
     ) -> ali_genieiap__1__0_models.CreateReminderResponse:
         runtime = util_models.RuntimeOptions()
         headers = ali_genieiap__1__0_models.CreateReminderHeaders()
@@ -322,24 +309,18 @@
             pathname=f'/v1.0/iap/reminder/delete',
             method='DELETE',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.DeleteReminderResponse(),
-                self.call_api(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.DeleteReminderResponse(),
-                self.execute(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.DeleteReminderResponse(),
+            self.call_api(params, req, runtime)
+        )
 
     async def delete_reminder_with_options_async(
         self,
         tmp_req: ali_genieiap__1__0_models.DeleteReminderRequest,
         headers: ali_genieiap__1__0_models.DeleteReminderHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_genieiap__1__0_models.DeleteReminderResponse:
@@ -377,24 +358,18 @@
             pathname=f'/v1.0/iap/reminder/delete',
             method='DELETE',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.DeleteReminderResponse(),
-                await self.call_api_async(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.DeleteReminderResponse(),
-                await self.execute_async(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.DeleteReminderResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
 
     def delete_reminder(
         self,
         request: ali_genieiap__1__0_models.DeleteReminderRequest,
     ) -> ali_genieiap__1__0_models.DeleteReminderResponse:
         runtime = util_models.RuntimeOptions()
         headers = ali_genieiap__1__0_models.DeleteReminderHeaders()
@@ -448,24 +423,18 @@
             pathname=f'/v1.0/iap/vip/account/get',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.GetAccountForAppResponse(),
-                self.call_api(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.GetAccountForAppResponse(),
-                self.execute(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.GetAccountForAppResponse(),
+            self.call_api(params, req, runtime)
+        )
 
     async def get_account_for_app_with_options_async(
         self,
         tmp_req: ali_genieiap__1__0_models.GetAccountForAppRequest,
         headers: ali_genieiap__1__0_models.GetAccountForAppHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_genieiap__1__0_models.GetAccountForAppResponse:
@@ -503,24 +472,18 @@
             pathname=f'/v1.0/iap/vip/account/get',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.GetAccountForAppResponse(),
-                await self.call_api_async(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.GetAccountForAppResponse(),
-                await self.execute_async(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.GetAccountForAppResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
 
     def get_account_for_app(
         self,
         request: ali_genieiap__1__0_models.GetAccountForAppRequest,
     ) -> ali_genieiap__1__0_models.GetAccountForAppResponse:
         runtime = util_models.RuntimeOptions()
         headers = ali_genieiap__1__0_models.GetAccountForAppHeaders()
@@ -574,24 +537,18 @@
             pathname=f'/v1.0/iap/app/config/get',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.GetBusAppConfigResponse(),
-                self.call_api(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.GetBusAppConfigResponse(),
-                self.execute(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.GetBusAppConfigResponse(),
+            self.call_api(params, req, runtime)
+        )
 
     async def get_bus_app_config_with_options_async(
         self,
         tmp_req: ali_genieiap__1__0_models.GetBusAppConfigRequest,
         headers: ali_genieiap__1__0_models.GetBusAppConfigHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_genieiap__1__0_models.GetBusAppConfigResponse:
@@ -629,24 +586,18 @@
             pathname=f'/v1.0/iap/app/config/get',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.GetBusAppConfigResponse(),
-                await self.call_api_async(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.GetBusAppConfigResponse(),
-                await self.execute_async(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.GetBusAppConfigResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
 
     def get_bus_app_config(
         self,
         request: ali_genieiap__1__0_models.GetBusAppConfigRequest,
     ) -> ali_genieiap__1__0_models.GetBusAppConfigResponse:
         runtime = util_models.RuntimeOptions()
         headers = ali_genieiap__1__0_models.GetBusAppConfigHeaders()
@@ -696,24 +647,18 @@
             pathname=f'/v1.0/iap/profile/phoneNumber',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.GetPhoneNumberResponse(),
-                self.call_api(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.GetPhoneNumberResponse(),
-                self.execute(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.GetPhoneNumberResponse(),
+            self.call_api(params, req, runtime)
+        )
 
     async def get_phone_number_with_options_async(
         self,
         tmp_req: ali_genieiap__1__0_models.GetPhoneNumberRequest,
         headers: ali_genieiap__1__0_models.GetPhoneNumberHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_genieiap__1__0_models.GetPhoneNumberResponse:
@@ -747,24 +692,18 @@
             pathname=f'/v1.0/iap/profile/phoneNumber',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.GetPhoneNumberResponse(),
-                await self.call_api_async(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.GetPhoneNumberResponse(),
-                await self.execute_async(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.GetPhoneNumberResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
 
     def get_phone_number(
         self,
         request: ali_genieiap__1__0_models.GetPhoneNumberRequest,
     ) -> ali_genieiap__1__0_models.GetPhoneNumberResponse:
         runtime = util_models.RuntimeOptions()
         headers = ali_genieiap__1__0_models.GetPhoneNumberHeaders()
@@ -818,24 +757,18 @@
             pathname=f'/v1.0/iap/reminder/get',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.GetReminderResponse(),
-                self.call_api(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.GetReminderResponse(),
-                self.execute(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.GetReminderResponse(),
+            self.call_api(params, req, runtime)
+        )
 
     async def get_reminder_with_options_async(
         self,
         tmp_req: ali_genieiap__1__0_models.GetReminderRequest,
         headers: ali_genieiap__1__0_models.GetReminderHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_genieiap__1__0_models.GetReminderResponse:
@@ -873,24 +806,18 @@
             pathname=f'/v1.0/iap/reminder/get',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.GetReminderResponse(),
-                await self.call_api_async(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.GetReminderResponse(),
-                await self.execute_async(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.GetReminderResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
 
     def get_reminder(
         self,
         request: ali_genieiap__1__0_models.GetReminderRequest,
     ) -> ali_genieiap__1__0_models.GetReminderResponse:
         runtime = util_models.RuntimeOptions()
         headers = ali_genieiap__1__0_models.GetReminderHeaders()
@@ -944,24 +871,18 @@
             pathname=f'/v1.0/iap/reminder/list',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.ListRemindersResponse(),
-                self.call_api(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.ListRemindersResponse(),
-                self.execute(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.ListRemindersResponse(),
+            self.call_api(params, req, runtime)
+        )
 
     async def list_reminders_with_options_async(
         self,
         tmp_req: ali_genieiap__1__0_models.ListRemindersRequest,
         headers: ali_genieiap__1__0_models.ListRemindersHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_genieiap__1__0_models.ListRemindersResponse:
@@ -999,24 +920,18 @@
             pathname=f'/v1.0/iap/reminder/list',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.ListRemindersResponse(),
-                await self.call_api_async(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.ListRemindersResponse(),
-                await self.execute_async(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.ListRemindersResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
 
     def list_reminders(
         self,
         request: ali_genieiap__1__0_models.ListRemindersRequest,
     ) -> ali_genieiap__1__0_models.ListRemindersResponse:
         runtime = util_models.RuntimeOptions()
         headers = ali_genieiap__1__0_models.ListRemindersHeaders()
@@ -1070,24 +985,18 @@
             pathname=f'/v1.0/iap/pull/cashier/',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.PullCashierResponse(),
-                self.call_api(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.PullCashierResponse(),
-                self.execute(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.PullCashierResponse(),
+            self.call_api(params, req, runtime)
+        )
 
     async def pull_cashier_with_options_async(
         self,
         tmp_req: ali_genieiap__1__0_models.PullCashierRequest,
         headers: ali_genieiap__1__0_models.PullCashierHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_genieiap__1__0_models.PullCashierResponse:
@@ -1125,24 +1034,18 @@
             pathname=f'/v1.0/iap/pull/cashier/',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.PullCashierResponse(),
-                await self.call_api_async(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.PullCashierResponse(),
-                await self.execute_async(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.PullCashierResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
 
     def pull_cashier(
         self,
         request: ali_genieiap__1__0_models.PullCashierRequest,
     ) -> ali_genieiap__1__0_models.PullCashierResponse:
         runtime = util_models.RuntimeOptions()
         headers = ali_genieiap__1__0_models.PullCashierHeaders()
@@ -1192,24 +1095,18 @@
             pathname=f'/v1.0/iap/notifications',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='formData',
             body_type='none'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.PushNotificationsResponse(),
-                self.call_api(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.PushNotificationsResponse(),
-                self.execute(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.PushNotificationsResponse(),
+            self.call_api(params, req, runtime)
+        )
 
     async def push_notifications_with_options_async(
         self,
         tmp_req: ali_genieiap__1__0_models.PushNotificationsRequest,
         headers: ali_genieiap__1__0_models.PushNotificationsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_genieiap__1__0_models.PushNotificationsResponse:
@@ -1243,24 +1140,18 @@
             pathname=f'/v1.0/iap/notifications',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='formData',
             body_type='none'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.PushNotificationsResponse(),
-                await self.call_api_async(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.PushNotificationsResponse(),
-                await self.execute_async(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.PushNotificationsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
 
     def push_notifications(
         self,
         request: ali_genieiap__1__0_models.PushNotificationsRequest,
     ) -> ali_genieiap__1__0_models.PushNotificationsResponse:
         runtime = util_models.RuntimeOptions()
         headers = ali_genieiap__1__0_models.PushNotificationsHeaders()
@@ -1318,24 +1209,18 @@
             pathname=f'/v1.0/iap/general/notifications',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='formData',
             body_type='none'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.SendNotificationsResponse(),
-                self.call_api(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.SendNotificationsResponse(),
-                self.execute(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.SendNotificationsResponse(),
+            self.call_api(params, req, runtime)
+        )
 
     async def send_notifications_with_options_async(
         self,
         tmp_req: ali_genieiap__1__0_models.SendNotificationsRequest,
         headers: ali_genieiap__1__0_models.SendNotificationsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_genieiap__1__0_models.SendNotificationsResponse:
@@ -1377,24 +1262,18 @@
             pathname=f'/v1.0/iap/general/notifications',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='formData',
             body_type='none'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.SendNotificationsResponse(),
-                await self.call_api_async(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.SendNotificationsResponse(),
-                await self.execute_async(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.SendNotificationsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
 
     def send_notifications(
         self,
         request: ali_genieiap__1__0_models.SendNotificationsRequest,
     ) -> ali_genieiap__1__0_models.SendNotificationsResponse:
         runtime = util_models.RuntimeOptions()
         headers = ali_genieiap__1__0_models.SendNotificationsHeaders()
@@ -1448,24 +1327,18 @@
             pathname=f'/v1.0/iap/reminder/update',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='formData',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.UpdateReminderResponse(),
-                self.call_api(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.UpdateReminderResponse(),
-                self.execute(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.UpdateReminderResponse(),
+            self.call_api(params, req, runtime)
+        )
 
     async def update_reminder_with_options_async(
         self,
         tmp_req: ali_genieiap__1__0_models.UpdateReminderRequest,
         headers: ali_genieiap__1__0_models.UpdateReminderHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_genieiap__1__0_models.UpdateReminderResponse:
@@ -1503,24 +1376,18 @@
             pathname=f'/v1.0/iap/reminder/update',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='formData',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.UpdateReminderResponse(),
-                await self.call_api_async(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.UpdateReminderResponse(),
-                await self.execute_async(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.UpdateReminderResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
 
     def update_reminder(
         self,
         request: ali_genieiap__1__0_models.UpdateReminderRequest,
     ) -> ali_genieiap__1__0_models.UpdateReminderResponse:
         runtime = util_models.RuntimeOptions()
         headers = ali_genieiap__1__0_models.UpdateReminderHeaders()
@@ -1574,24 +1441,18 @@
             pathname=f'/v1.0/iap/vip/use/video/report',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='formData',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.VideoAppReportResponse(),
-                self.call_api(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.VideoAppReportResponse(),
-                self.execute(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.VideoAppReportResponse(),
+            self.call_api(params, req, runtime)
+        )
 
     async def video_app_report_with_options_async(
         self,
         tmp_req: ali_genieiap__1__0_models.VideoAppReportRequest,
         headers: ali_genieiap__1__0_models.VideoAppReportHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_genieiap__1__0_models.VideoAppReportResponse:
@@ -1629,24 +1490,18 @@
             pathname=f'/v1.0/iap/vip/use/video/report',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='formData',
             body_type='json'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.VideoAppReportResponse(),
-                await self.call_api_async(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.VideoAppReportResponse(),
-                await self.execute_async(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.VideoAppReportResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
 
     def video_app_report(
         self,
         request: ali_genieiap__1__0_models.VideoAppReportRequest,
     ) -> ali_genieiap__1__0_models.VideoAppReportResponse:
         runtime = util_models.RuntimeOptions()
         headers = ali_genieiap__1__0_models.VideoAppReportHeaders()
@@ -1692,24 +1547,18 @@
             pathname=f'/v1.0/iap/wakeup',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='none'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.WakeUpAppResponse(),
-                self.call_api(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.WakeUpAppResponse(),
-                self.execute(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.WakeUpAppResponse(),
+            self.call_api(params, req, runtime)
+        )
 
     async def wake_up_app_with_options_async(
         self,
         request: ali_genieiap__1__0_models.WakeUpAppRequest,
         headers: ali_genieiap__1__0_models.WakeUpAppHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_genieiap__1__0_models.WakeUpAppResponse:
@@ -1739,24 +1588,18 @@
             pathname=f'/v1.0/iap/wakeup',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='none'
         )
-        if UtilClient.is_unset(self._signature_version) or not UtilClient.equal_string(self._signature_version, 'v4'):
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.WakeUpAppResponse(),
-                await self.call_api_async(params, req, runtime)
-            )
-        else:
-            return TeaCore.from_map(
-                ali_genieiap__1__0_models.WakeUpAppResponse(),
-                await self.execute_async(params, req, runtime)
-            )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.WakeUpAppResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
 
     def wake_up_app(
         self,
         request: ali_genieiap__1__0_models.WakeUpAppRequest,
     ) -> ali_genieiap__1__0_models.WakeUpAppResponse:
         runtime = util_models.RuntimeOptions()
         headers = ali_genieiap__1__0_models.WakeUpAppHeaders()
```

### Comparing `alibabacloud_aligenieiap_1_0-1.1.0/alibabacloud_aligenieiap_1_0/models.py` & `alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1795,41 +1795,47 @@
             self.user_info_shrink = m.get('UserInfo')
         return self
 
 
 class GetBusAppConfigResponseBodyRetValue(TeaModel):
     def __init__(
         self,
+        cashier: str = None,
         shopping_bar: str = None,
         shopping_window: str = None,
         vip_label: str = None,
     ):
+        self.cashier = cashier
         self.shopping_bar = shopping_bar
         self.shopping_window = shopping_window
         self.vip_label = vip_label
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.cashier is not None:
+            result['Cashier'] = self.cashier
         if self.shopping_bar is not None:
             result['ShoppingBar'] = self.shopping_bar
         if self.shopping_window is not None:
             result['ShoppingWindow'] = self.shopping_window
         if self.vip_label is not None:
             result['VipLabel'] = self.vip_label
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('Cashier') is not None:
+            self.cashier = m.get('Cashier')
         if m.get('ShoppingBar') is not None:
             self.shopping_bar = m.get('ShoppingBar')
         if m.get('ShoppingWindow') is not None:
             self.shopping_window = m.get('ShoppingWindow')
         if m.get('VipLabel') is not None:
             self.vip_label = m.get('VipLabel')
         return self
```

### Comparing `alibabacloud_aligenieiap_1_0-1.1.0/alibabacloud_aligenieiap_1_0.egg-info/PKG-INFO` & `alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aligenieiap-1-0
-Version: 1.1.0
+Version: 1.1.1
 Summary: Alibaba Cloud AliGenie (iap_1_0) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aligenieiap_1_0-1.1.0/setup.py` & `alibabacloud_aligenieiap_1_0-1.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,32 +20,31 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aligenieiap_1_0.
 
-Created on 29/03/2024
+Created on 11/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aligenieiap_1_0"
 NAME = "alibabacloud_aligenieiap_1_0" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AliGenie (iap_1_0) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_gateway_spi>=0.0.1, <1.0.0",
-    "alibabacloud_gateway_pop>=0.0.3, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.1, <1.0.0"
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
+    "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

