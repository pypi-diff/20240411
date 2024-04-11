# Comparing `tmp/alibabacloud_dcdn20180115-2.3.0.tar.gz` & `tmp/alibabacloud_dcdn20180115-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dcdn20180115-2.3.0.tar", last modified: Mon Apr  8 17:08:33 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dcdn20180115-2.4.0.tar", last modified: Thu Apr 11 17:10:51 2024, max compression
```

## Comparing `alibabacloud_dcdn20180115-2.3.0.tar` & `alibabacloud_dcdn20180115-2.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/
--rw-r--r--   0 root         (0) root         (0)     4098 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2408 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1099 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1184 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1059206 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115/client.py
--rw-r--r--   0 root         (0) root         (0)  1418866 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2408 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2616 2024-04-08 17:08:33.000000 alibabacloud_dcdn20180115-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/
+-rw-r--r--   0 root         (0) root         (0)     4531 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/alibabacloud_dcdn20180115/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/alibabacloud_dcdn20180115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1063348 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/alibabacloud_dcdn20180115/client.py
+-rw-r--r--   0 root         (0) root         (0)  1422947 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/alibabacloud_dcdn20180115/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/alibabacloud_dcdn20180115.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/alibabacloud_dcdn20180115.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/alibabacloud_dcdn20180115.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/alibabacloud_dcdn20180115.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/alibabacloud_dcdn20180115.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/alibabacloud_dcdn20180115.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2616 2024-04-11 17:10:51.000000 alibabacloud_dcdn20180115-2.4.0/setup.py
```

### Comparing `alibabacloud_dcdn20180115-2.3.0/ChangeLog.md` & `alibabacloud_dcdn20180115-2.4.0/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+2024-04-08 Version: 2.3.0
+- Support API BatchDeleteDcdnKv.
+- Support API BatchDeleteDcdnKvWithHighCapacity.
+- Support API BatchPutDcdnKvWithHighCapacity.
+- Support API PutDcdnKvWithHighCapacity.
+- Update API BatchPutDcdnKv: update param KvList.
+- Update API DescribeDcdnDomainConfigs: update param FunctionNames.
+- Update API DescribeDcdnWafGroups: update response param.
+- Update API PutDcdnKvNamespace: update param Description.
+
+
 2024-03-21 Version: 2.2.1
 - Update API DescribeDcdnKvNamespace: update response param.
 - Update API PutDcdnKvNamespace: update response param.
 
 
 2024-01-08 Version: 2.2.0
 - Generated python 2018-01-15 for dcdn.
```

### Comparing `alibabacloud_dcdn20180115-2.3.0/LICENSE` & `alibabacloud_dcdn20180115-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115-2.3.0/PKG-INFO` & `alibabacloud_dcdn20180115-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dcdn20180115
-Version: 2.3.0
+Version: 2.4.0
 Summary: Alibaba Cloud dcdn (20180115) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dcdn20180115-2.3.0/README-CN.md` & `alibabacloud_dcdn20180115-2.4.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115-2.3.0/README.md` & `alibabacloud_dcdn20180115-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115/client.py` & `alibabacloud_dcdn20180115-2.4.0/alibabacloud_dcdn20180115/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2505,18 +2505,16 @@
 
     def create_dcdn_sub_task_with_options(
         self,
         request: dcdn_20180115_models.CreateDcdnSubTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.CreateDcdnSubTaskResponse:
         """
-        *\
-        ****\
-        *\
-        *\
+        >    This operation allows you to create a custom operations report for a specific domain name. You can view the statistics about the domain name in the report.
+        > *   You can call this operation up to three times per second per account.
         
         @param request: CreateDcdnSubTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDcdnSubTaskResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -2545,18 +2543,16 @@
 
     async def create_dcdn_sub_task_with_options_async(
         self,
         request: dcdn_20180115_models.CreateDcdnSubTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.CreateDcdnSubTaskResponse:
         """
-        *\
-        ****\
-        *\
-        *\
+        >    This operation allows you to create a custom operations report for a specific domain name. You can view the statistics about the domain name in the report.
+        > *   You can call this operation up to three times per second per account.
         
         @param request: CreateDcdnSubTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDcdnSubTaskResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -2584,34 +2580,30 @@
         )
 
     def create_dcdn_sub_task(
         self,
         request: dcdn_20180115_models.CreateDcdnSubTaskRequest,
     ) -> dcdn_20180115_models.CreateDcdnSubTaskResponse:
         """
-        *\
-        ****\
-        *\
-        *\
+        >    This operation allows you to create a custom operations report for a specific domain name. You can view the statistics about the domain name in the report.
+        > *   You can call this operation up to three times per second per account.
         
         @param request: CreateDcdnSubTaskRequest
         @return: CreateDcdnSubTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_dcdn_sub_task_with_options(request, runtime)
 
     async def create_dcdn_sub_task_async(
         self,
         request: dcdn_20180115_models.CreateDcdnSubTaskRequest,
     ) -> dcdn_20180115_models.CreateDcdnSubTaskResponse:
         """
-        *\
-        ****\
-        *\
-        *\
+        >    This operation allows you to create a custom operations report for a specific domain name. You can view the statistics about the domain name in the report.
+        > *   You can call this operation up to three times per second per account.
         
         @param request: CreateDcdnSubTaskRequest
         @return: CreateDcdnSubTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_dcdn_sub_task_with_options_async(request, runtime)
 
@@ -9843,15 +9835,15 @@
 
     def describe_dcdn_domain_staging_config_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainStagingConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainStagingConfigResponse:
         """
-        The name of the accelerated domain.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDcdnDomainStagingConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainStagingConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9880,15 +9872,15 @@
 
     async def describe_dcdn_domain_staging_config_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainStagingConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnDomainStagingConfigResponse:
         """
-        The name of the accelerated domain.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDcdnDomainStagingConfigRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnDomainStagingConfigResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9916,28 +9908,28 @@
         )
 
     def describe_dcdn_domain_staging_config(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainStagingConfigRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainStagingConfigResponse:
         """
-        The name of the accelerated domain.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDcdnDomainStagingConfigRequest
         @return: DescribeDcdnDomainStagingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_staging_config_with_options(request, runtime)
 
     async def describe_dcdn_domain_staging_config_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnDomainStagingConfigRequest,
     ) -> dcdn_20180115_models.DescribeDcdnDomainStagingConfigResponse:
         """
-        The name of the accelerated domain.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: DescribeDcdnDomainStagingConfigRequest
         @return: DescribeDcdnDomainStagingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_domain_staging_config_with_options_async(request, runtime)
 
@@ -11409,15 +11401,15 @@
 
     def describe_dcdn_https_domain_list_with_options(
         self,
         request: dcdn_20180115_models.DescribeDcdnHttpsDomainListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnHttpsDomainListResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnHttpsDomainListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnHttpsDomainListResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11448,15 +11440,15 @@
 
     async def describe_dcdn_https_domain_list_with_options_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnHttpsDomainListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeDcdnHttpsDomainListResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnHttpsDomainListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDcdnHttpsDomainListResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11486,28 +11478,28 @@
         )
 
     def describe_dcdn_https_domain_list(
         self,
         request: dcdn_20180115_models.DescribeDcdnHttpsDomainListRequest,
     ) -> dcdn_20180115_models.DescribeDcdnHttpsDomainListResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnHttpsDomainListRequest
         @return: DescribeDcdnHttpsDomainListResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_https_domain_list_with_options(request, runtime)
 
     async def describe_dcdn_https_domain_list_async(
         self,
         request: dcdn_20180115_models.DescribeDcdnHttpsDomainListRequest,
     ) -> dcdn_20180115_models.DescribeDcdnHttpsDomainListResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDcdnHttpsDomainListRequest
         @return: DescribeDcdnHttpsDomainListResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dcdn_https_domain_list_with_options_async(request, runtime)
 
@@ -18776,15 +18768,15 @@
         return await self.describe_routine_spec_with_options_async(runtime)
 
     def describe_routine_user_info_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeRoutineUserInfoResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeRoutineUserInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeRoutineUserInfoResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -18804,15 +18796,15 @@
         )
 
     async def describe_routine_user_info_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.DescribeRoutineUserInfoResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeRoutineUserInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeRoutineUserInfoResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -18829,24 +18821,24 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeRoutineUserInfoResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_routine_user_info(self) -> dcdn_20180115_models.DescribeRoutineUserInfoResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @return: DescribeRoutineUserInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_routine_user_info_with_options(runtime)
 
     async def describe_routine_user_info_async(self) -> dcdn_20180115_models.DescribeRoutineUserInfoResponse:
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
         @return: DescribeRoutineUserInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_routine_user_info_with_options_async(runtime)
 
     def describe_user_dcdn_ipa_status_with_options(
@@ -20935,14 +20927,92 @@
     async def put_dcdn_kv_with_high_capacity_async(
         self,
         request: dcdn_20180115_models.PutDcdnKvWithHighCapacityRequest,
     ) -> dcdn_20180115_models.PutDcdnKvWithHighCapacityResponse:
         runtime = util_models.RuntimeOptions()
         return await self.put_dcdn_kv_with_high_capacity_with_options_async(request, runtime)
 
+    def refresh_dcdn_object_cache_by_cache_tag_with_options(
+        self,
+        request: dcdn_20180115_models.RefreshDcdnObjectCacheByCacheTagRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dcdn_20180115_models.RefreshDcdnObjectCacheByCacheTagResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.cache_tag):
+            query['CacheTag'] = request.cache_tag
+        if not UtilClient.is_unset(request.domain_name):
+            query['DomainName'] = request.domain_name
+        if not UtilClient.is_unset(request.force):
+            query['Force'] = request.force
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RefreshDcdnObjectCacheByCacheTag',
+            version='2018-01-15',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dcdn_20180115_models.RefreshDcdnObjectCacheByCacheTagResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def refresh_dcdn_object_cache_by_cache_tag_with_options_async(
+        self,
+        request: dcdn_20180115_models.RefreshDcdnObjectCacheByCacheTagRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dcdn_20180115_models.RefreshDcdnObjectCacheByCacheTagResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.cache_tag):
+            query['CacheTag'] = request.cache_tag
+        if not UtilClient.is_unset(request.domain_name):
+            query['DomainName'] = request.domain_name
+        if not UtilClient.is_unset(request.force):
+            query['Force'] = request.force
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RefreshDcdnObjectCacheByCacheTag',
+            version='2018-01-15',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dcdn_20180115_models.RefreshDcdnObjectCacheByCacheTagResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def refresh_dcdn_object_cache_by_cache_tag(
+        self,
+        request: dcdn_20180115_models.RefreshDcdnObjectCacheByCacheTagRequest,
+    ) -> dcdn_20180115_models.RefreshDcdnObjectCacheByCacheTagResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.refresh_dcdn_object_cache_by_cache_tag_with_options(request, runtime)
+
+    async def refresh_dcdn_object_cache_by_cache_tag_async(
+        self,
+        request: dcdn_20180115_models.RefreshDcdnObjectCacheByCacheTagRequest,
+    ) -> dcdn_20180115_models.RefreshDcdnObjectCacheByCacheTagResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.refresh_dcdn_object_cache_by_cache_tag_with_options_async(request, runtime)
+
     def refresh_dcdn_object_caches_with_options(
         self,
         request: dcdn_20180115_models.RefreshDcdnObjectCachesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.RefreshDcdnObjectCachesResponse:
         """
         DCDN supports POST requests in which parameters are sent as a form.
@@ -22957,15 +23027,15 @@
 
     def update_dcdn_domain_with_options(
         self,
         request: dcdn_20180115_models.UpdateDcdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.UpdateDcdnDomainResponse:
         """
-        >  You can call this operation up to 30 times per second per account.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: UpdateDcdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateDcdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -23002,15 +23072,15 @@
 
     async def update_dcdn_domain_with_options_async(
         self,
         request: dcdn_20180115_models.UpdateDcdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dcdn_20180115_models.UpdateDcdnDomainResponse:
         """
-        >  You can call this operation up to 30 times per second per account.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: UpdateDcdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateDcdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -23046,28 +23116,28 @@
         )
 
     def update_dcdn_domain(
         self,
         request: dcdn_20180115_models.UpdateDcdnDomainRequest,
     ) -> dcdn_20180115_models.UpdateDcdnDomainResponse:
         """
-        >  You can call this operation up to 30 times per second per account.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: UpdateDcdnDomainRequest
         @return: UpdateDcdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_dcdn_domain_with_options(request, runtime)
 
     async def update_dcdn_domain_async(
         self,
         request: dcdn_20180115_models.UpdateDcdnDomainRequest,
     ) -> dcdn_20180115_models.UpdateDcdnDomainResponse:
         """
-        >  You can call this operation up to 30 times per second per account.
+        > You can call this operation up to 30 times per second per account.
         
         @param request: UpdateDcdnDomainRequest
         @return: UpdateDcdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_dcdn_domain_with_options_async(request, runtime)
```

### Comparing `alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115/models.py` & `alibabacloud_dcdn20180115-2.4.0/alibabacloud_dcdn20180115/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3322,32 +3322,34 @@
 
 class CreateDcdnSubTaskRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         report_ids: str = None,
     ):
-        # [](https://workorder-intl.console.aliyun.com/?spm=5176.2020520001.aliyun_topbar.18.dbd44bd3e4f845#/ticket/createIndex)
+        # The domain names to be tracked. Separate multiple domain names with commas (,). You can specify up to 500 domain names. If you want to specify more than 500 domain names, [submit a ticket](https://workorder-intl.console.aliyun.com/?spm=5176.2020520001.aliyun_topbar.18.dbd44bd3e4f845#/ticket/createIndex).
         # 
-        # **\
-        # 
-        # ****\
+        # > If you do not specify a domain name, the tracking task is created for all domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name
-        # *   ****\
-        # *   ****\
-        # *   ****\
-        # *   ****\
-        # *   ****\
-        # *   ****\
-        # *   ****\
-        # *   ****\
-        # *   ****\
-        # *   ****\
-        # *   ****\
-        # *   ****\
+        # The IDs of the metrics that you want to include in the report. Separate multiple IDs with commas (,). Valid values:
+        # 
+        # *   **2**: Popular URLs by Request
+        # *   **4**: Popular URLs by Traffic
+        # *   **6**: Popular Referer by Request
+        # *   **8**: Popular Referer by Traffic
+        # *   **10**: Popular Back-to-origin URLs by Request
+        # *   **12**: Popular Back-to-origin URLs by Traffic
+        # *   **14**: Top Client IPs by Request
+        # *   **16**: Top Client IPs by Traffic
+        # *   **18**: Popular Domain Names by Traffic
+        # *   **20**: PV/UV
+        # *   **22**: Visit Distribution by Region
+        # *   **24**: Distribution of ISPs
+        # *   **26**: Peak IPv4/IPv6 Bandwidth
+        # *   **27**: Back-to-origin bandwidth
         self.report_ids = report_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3371,14 +3373,15 @@
 
 
 class CreateDcdnSubTaskResponseBody(TeaModel):
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
@@ -4481,15 +4484,15 @@
 
 class DeleteDcdnKvRequest(TeaModel):
     def __init__(
         self,
         key: str = None,
         namespace: str = None,
     ):
-        # The ID of the request.
+        # The name of the key that you want to delete.
         self.key = key
         # The namespace that you specify when you call the PutDcdnKvNamespace operation.
         self.namespace = namespace
 
     def validate(self):
         pass
 
@@ -4515,15 +4518,15 @@
 
 
 class DeleteDcdnKvResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The name of the key to delete.
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16761,17 +16764,17 @@
 
 class DescribeDcdnDomainStagingConfigRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         function_names: str = None,
     ):
-        # The names of the features to query. You can specify multiple features and separate them with commas (,).
+        # The accelerated domain name.
         self.domain_name = domain_name
-        # The ID of the request.
+        # The names of the features to query. You can separate multiple features with commas (,).
         self.function_names = function_names
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16796,16 +16799,17 @@
 
 class DescribeDcdnDomainStagingConfigResponseBodyDomainConfigsFunctionArgs(TeaModel):
     def __init__(
         self,
         arg_name: str = None,
         arg_value: str = None,
     ):
-        # The value of the configuration.
+        # The name of the configuration.
         self.arg_name = arg_name
+        # The value of the configuration.
         self.arg_value = arg_value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16832,21 +16836,26 @@
     def __init__(
         self,
         config_id: str = None,
         function_args: List[DescribeDcdnDomainStagingConfigResponseBodyDomainConfigsFunctionArgs] = None,
         function_name: str = None,
         status: str = None,
     ):
-        # The name of the feature.
+        # The ID of the configuration.
         self.config_id = config_id
-        # The name of the configuration.
+        # The following table describes the features.
         self.function_args = function_args
-        # The descriptions of a feature.
+        # The name of the feature.
         self.function_name = function_name
-        # The ID of the configuration.
+        # The status. Valid values:
+        # 
+        # *   success: The configuration is successful.
+        # *   testing: The configuration is under testing.
+        # *   failed: The task failed.
+        # *   configuring: The feature is being configured.
         self.status = status
 
     def validate(self):
         if self.function_args:
             for k in self.function_args:
                 if k:
                     k.validate()
@@ -16887,22 +16896,17 @@
 
 class DescribeDcdnDomainStagingConfigResponseBody(TeaModel):
     def __init__(
         self,
         domain_configs: List[DescribeDcdnDomainStagingConfigResponseBodyDomainConfigs] = None,
         request_id: str = None,
     ):
-        # The status of the feature. Valid values:
-        # 
-        # *   success
-        # *   testing
-        # *   failed
-        # *   configuring
-        self.domain_configs = domain_configs
         # The configurations of accelerated domain names returned.
+        self.domain_configs = domain_configs
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.domain_configs:
             for k in self.domain_configs:
                 if k:
                     k.validate()
@@ -20289,28 +20293,19 @@
 class DescribeDcdnHttpsDomainListRequest(TeaModel):
     def __init__(
         self,
         keyword: str = None,
         page_number: int = None,
         page_size: int = None,
     ):
-        # The status of the certificate. Valid values:
-        # 
-        # *   **ok**: The certificate is working as expected.
-        # *   **mismatch**: The certificate does not match the specified domain name.
-        # *   **expired**: The certificate has expired.
-        # *   **expire_soon**: The certificate is about to expire.
+        # The keyword that is used to search for certificates.
         self.keyword = keyword
-        # The total number of entries returned.
+        # The number of returned pages. Valid values: **1 to 100000**.
         self.page_number = page_number
-        # The type of the certificate. Valid values:
-        # 
-        # *   **free**: A free certificate.
-        # *   **cas**: A certificate that is purchased through Alibaba Cloud SSL Certificates Service.
-        # *   **upload**: A user-uploaded certificate.
+        # The number of entries to return on each page. Valid values: **1 to 500**. Default value: **20**.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20345,29 +20340,37 @@
         cert_name: str = None,
         cert_start_time: str = None,
         cert_status: str = None,
         cert_type: str = None,
         cert_update_time: str = None,
         domain_name: str = None,
     ):
-        # The certificate information about the domain name.
+        # The returned primary domain name of the certificate.
         self.cert_common_name = cert_common_name
-        # The name of the certificate.
+        # The time at which the certificate expires.
         self.cert_expire_time = cert_expire_time
-        # The accelerated domain name for which the certificate information was queried.
+        # The name of the certificate.
         self.cert_name = cert_name
-        # The time when the certificate expires.
+        # The time at which the certificate became effective.
         self.cert_start_time = cert_start_time
-        # The number of pages to return. Valid values: **1 to 100000**.
+        # The status of the certificate. Valid values:
+        # 
+        # *   **ok**: The certificate is working as expected.
+        # *   **mismatch**: The certificate does not match the specified domain name.
+        # *   **expired**: The certificate has expired.
+        # *   **expire_soon**: The certificate is about to expire.
         self.cert_status = cert_status
-        # The operation that you want to perform. Set the value to **DescribeDcdnHttpsDomainList**.
+        # The type of the certificate. Valid values:
+        # 
+        # *   **cas**: a certificate that is purchased by using Certificate Management Service
+        # *   **upload**: a custom certificate that you upload
         self.cert_type = cert_type
-        # The keyword used for search.
+        # The time at which the certificate was updated.
         self.cert_update_time = cert_update_time
-        # The time when the certificate was updated.
+        # The accelerated domain name.
         self.domain_name = domain_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20452,19 +20455,19 @@
 class DescribeDcdnHttpsDomainListResponseBody(TeaModel):
     def __init__(
         self,
         cert_infos: DescribeDcdnHttpsDomainListResponseBodyCertInfos = None,
         request_id: str = None,
         total_count: int = None,
     ):
-        # The time when the certificate became effective.
+        # The information about the certificate.
         self.cert_infos = cert_infos
-        # The returned primary domain name of the certificate.
+        # The ID of the request.
         self.request_id = request_id
-        # The number of entries to return on each page. Valid values: **1 to 500**. Default value: **20**.
+        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.cert_infos:
             self.cert_infos.validate()
 
     def to_map(self):
@@ -36217,17 +36220,17 @@
 
 class DescribeRoutineUserInfoResponseBody(TeaModel):
     def __init__(
         self,
         content: Dict[str, Any] = None,
         request_id: str = None,
     ):
-        # The ID of the request.
+        # The content returned by calling the operation.
         self.content = content
-        # The operation that you want to perform. Set the value to **DescribeRoutineUserInfo**.
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -39197,14 +39200,127 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PutDcdnKvWithHighCapacityResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RefreshDcdnObjectCacheByCacheTagRequest(TeaModel):
+    def __init__(
+        self,
+        cache_tag: str = None,
+        domain_name: str = None,
+        force: bool = None,
+    ):
+        self.cache_tag = cache_tag
+        self.domain_name = domain_name
+        self.force = force
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
+        if self.cache_tag is not None:
+            result['CacheTag'] = self.cache_tag
+        if self.domain_name is not None:
+            result['DomainName'] = self.domain_name
+        if self.force is not None:
+            result['Force'] = self.force
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CacheTag') is not None:
+            self.cache_tag = m.get('CacheTag')
+        if m.get('DomainName') is not None:
+            self.domain_name = m.get('DomainName')
+        if m.get('Force') is not None:
+            self.force = m.get('Force')
+        return self
+
+
+class RefreshDcdnObjectCacheByCacheTagResponseBody(TeaModel):
+    def __init__(
+        self,
+        refresh_task_id: str = None,
+        request_id: str = None,
+    ):
+        self.refresh_task_id = refresh_task_id
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
+        if self.refresh_task_id is not None:
+            result['RefreshTaskId'] = self.refresh_task_id
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RefreshTaskId') is not None:
+            self.refresh_task_id = m.get('RefreshTaskId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class RefreshDcdnObjectCacheByCacheTagResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: RefreshDcdnObjectCacheByCacheTagResponseBody = None,
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
+            temp_model = RefreshDcdnObjectCacheByCacheTagResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class RefreshDcdnObjectCachesRequest(TeaModel):
     def __init__(
         self,
         force: bool = None,
         object_path: str = None,
         object_type: str = None,
         owner_id: int = None,
@@ -40195,15 +40311,15 @@
 
 
 class SetDcdnDomainStagingConfigResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the region.
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -41521,23 +41637,23 @@
         domain_name: str = None,
         owner_id: int = None,
         resource_group_id: str = None,
         security_token: str = None,
         sources: str = None,
         top_level_domain: str = None,
     ):
-        # The top-level domain name.
+        # The accelerated domain name. You can specify only one domain name in each call.
         self.domain_name = domain_name
         self.owner_id = owner_id
-        # The ID of the request.
+        # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.security_token = security_token
-        # The accelerated domain name. You can specify only one domain name in each call.
+        # The information about the addresses of origin servers.
         self.sources = sources
-        # The operation that you want to perform. Set the value to **UpdateDcdnDomain**.
+        # The top-level domain.
         self.top_level_domain = top_level_domain
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -41577,15 +41693,15 @@
 
 
 class UpdateDcdnDomainResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The information about the addresses of origin servers.
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_dcdn20180115-2.3.0/alibabacloud_dcdn20180115.egg-info/PKG-INFO` & `alibabacloud_dcdn20180115-2.4.0/alibabacloud_dcdn20180115.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dcdn20180115
-Version: 2.3.0
+Version: 2.4.0
 Summary: Alibaba Cloud dcdn (20180115) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dcdn20180115-2.3.0/setup.py` & `alibabacloud_dcdn20180115-2.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dcdn20180115.
 
-Created on 08/04/2024
+Created on 11/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dcdn20180115"
 NAME = "alibabacloud_dcdn20180115" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud dcdn (20180115) SDK Library for Python"
```

