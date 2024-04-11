# Comparing `tmp/alibabacloud_dcdn20180115_py2-2.3.0.tar.gz` & `tmp/alibabacloud_dcdn20180115_py2-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dcdn20180115_py2-2.3.0.tar", last modified: Mon Apr  8 17:07:44 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dcdn20180115_py2-2.4.0.tar", last modified: Thu Apr 11 17:12:36 2024, max compression
```

## Comparing `alibabacloud_dcdn20180115_py2-2.3.0.tar` & `alibabacloud_dcdn20180115_py2-2.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/
--rw-r--r--   0 root         (0) root         (0)     3915 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2478 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115/__init__.py
--rw-r--r--   0 root         (0) root         (0)   459855 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115/client.py
--rw-r--r--   0 root         (0) root         (0)  1437036 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2478 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      448 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2908 2024-04-08 17:07:44.000000 alibabacloud_dcdn20180115_py2-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:12:36.000000 alibabacloud_dcdn20180115_py2-2.4.0/
+-rw-r--r--   0 root         (0) root         (0)     4348 2024-04-11 17:12:35.000000 alibabacloud_dcdn20180115_py2-2.4.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-11 17:12:35.000000 alibabacloud_dcdn20180115_py2-2.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-11 17:12:35.000000 alibabacloud_dcdn20180115_py2-2.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-11 17:12:36.000000 alibabacloud_dcdn20180115_py2-2.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-04-11 17:12:35.000000 alibabacloud_dcdn20180115_py2-2.4.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-04-11 17:12:35.000000 alibabacloud_dcdn20180115_py2-2.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:12:36.000000 alibabacloud_dcdn20180115_py2-2.4.0/alibabacloud_dcdn20180115/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 17:12:35.000000 alibabacloud_dcdn20180115_py2-2.4.0/alibabacloud_dcdn20180115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   461566 2024-04-11 17:12:35.000000 alibabacloud_dcdn20180115_py2-2.4.0/alibabacloud_dcdn20180115/client.py
+-rw-r--r--   0 root         (0) root         (0)  1441173 2024-04-11 17:12:35.000000 alibabacloud_dcdn20180115_py2-2.4.0/alibabacloud_dcdn20180115/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 17:12:36.000000 alibabacloud_dcdn20180115_py2-2.4.0/alibabacloud_dcdn20180115_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-11 17:12:36.000000 alibabacloud_dcdn20180115_py2-2.4.0/alibabacloud_dcdn20180115_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2024-04-11 17:12:36.000000 alibabacloud_dcdn20180115_py2-2.4.0/alibabacloud_dcdn20180115_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 17:12:36.000000 alibabacloud_dcdn20180115_py2-2.4.0/alibabacloud_dcdn20180115_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-11 17:12:36.000000 alibabacloud_dcdn20180115_py2-2.4.0/alibabacloud_dcdn20180115_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-11 17:12:36.000000 alibabacloud_dcdn20180115_py2-2.4.0/alibabacloud_dcdn20180115_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 17:12:36.000000 alibabacloud_dcdn20180115_py2-2.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2908 2024-04-11 17:12:35.000000 alibabacloud_dcdn20180115_py2-2.4.0/setup.py
```

### Comparing `alibabacloud_dcdn20180115_py2-2.3.0/ChangeLog.md` & `alibabacloud_dcdn20180115_py2-2.4.0/ChangeLog.md`

 * *Files 16% similar despite different names*

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
 2024-03-21 Version: 2.2.0
 - Support API CreateDcdnCertificateSigningRequest.
 - Support API SetDcdnDomainCSRCertificate.
 - Update API DescribeDcdnKvNamespace: update response param.
 - Update API PutDcdnKvNamespace: update response param.
```

### Comparing `alibabacloud_dcdn20180115_py2-2.3.0/LICENSE` & `alibabacloud_dcdn20180115_py2-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115_py2-2.3.0/PKG-INFO` & `alibabacloud_dcdn20180115_py2-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dcdn20180115_py2
-Version: 2.3.0
+Version: 2.4.0
 Summary: Alibaba Cloud dcdn (20180115) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dcdn20180115_py2-2.3.0/README-CN.md` & `alibabacloud_dcdn20180115_py2-2.4.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115_py2-2.3.0/README.md` & `alibabacloud_dcdn20180115_py2-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115/client.py` & `alibabacloud_dcdn20180115_py2-2.4.0/alibabacloud_dcdn20180115/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1218,18 +1218,16 @@
         @return: CreateDcdnSLSRealTimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_dcdn_slsreal_time_log_delivery_with_options(request, runtime)
 
     def create_dcdn_sub_task_with_options(self, request, runtime):
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
@@ -1257,18 +1255,16 @@
         return TeaCore.from_map(
             dcdn_20180115_models.CreateDcdnSubTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_dcdn_sub_task(self, request):
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
@@ -4712,15 +4708,15 @@
         @return: DescribeDcdnDomainRegionDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_domain_region_data_with_options(request, runtime)
 
     def describe_dcdn_domain_staging_config_with_options(self, request, runtime):
         """
-        The name of the accelerated domain.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeDcdnDomainStagingConfigRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnDomainStagingConfigResponse
@@ -4748,15 +4744,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnDomainStagingConfigResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_domain_staging_config(self, request):
         """
-        The name of the accelerated domain.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: DescribeDcdnDomainStagingConfigRequest
 
         @return: DescribeDcdnDomainStagingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -5464,15 +5460,15 @@
         @return: DescribeDcdnFullDomainsBlockIPHistoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dcdn_full_domains_block_iphistory_with_options(request, runtime)
 
     def describe_dcdn_https_domain_list_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeDcdnHttpsDomainListRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDcdnHttpsDomainListResponse
@@ -5502,15 +5498,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeDcdnHttpsDomainListResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dcdn_https_domain_list(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeDcdnHttpsDomainListRequest
 
         @return: DescribeDcdnHttpsDomainListResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -8950,15 +8946,15 @@
         @return: DescribeRoutineSpecResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_routine_spec_with_options(runtime)
 
     def describe_routine_user_info_with_options(self, runtime):
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeRoutineUserInfoRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeRoutineUserInfoResponse
@@ -8978,15 +8974,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.DescribeRoutineUserInfoResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_routine_user_info(self):
         """
-        >  You can call this operation up to 100 times per second per account.
+        > You can call this operation up to 100 times per second per account.
         
 
         @return: DescribeRoutineUserInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_routine_user_info_with_options(runtime)
 
@@ -9954,14 +9950,46 @@
             self.call_api(params, req, runtime)
         )
 
     def put_dcdn_kv_with_high_capacity(self, request):
         runtime = util_models.RuntimeOptions()
         return self.put_dcdn_kv_with_high_capacity_with_options(request, runtime)
 
+    def refresh_dcdn_object_cache_by_cache_tag_with_options(self, request, runtime):
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
+    def refresh_dcdn_object_cache_by_cache_tag(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.refresh_dcdn_object_cache_by_cache_tag_with_options(request, runtime)
+
     def refresh_dcdn_object_caches_with_options(self, request, runtime):
         """
         DCDN supports POST requests in which parameters are sent as a form.
         *   You can call the [RefreshDcdnObjectCaches](~~130620~~) operation to refresh content and call the [PreloadDcdnObjectCaches](~~130636~~) operation to prefetch content.
         *   By default, each Alibaba Cloud account can refresh content from a maximum of 10,000 URLs and 100 directories per day, including subdirectories. If the daily peak bandwidth value exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to request a quota increase. DCDN evaluates your application based on your workloads.
         *   You can specify up to 1,000 URLs or 100 directories that you want to refresh in each request.
         *   You can refresh a maximum of 1,000 URLs per minute for each domain name.
@@ -10918,15 +10946,15 @@
         @return: UpdateDcdnDeliverTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_dcdn_deliver_task_with_options(request, runtime)
 
     def update_dcdn_domain_with_options(self, request, runtime):
         """
-        >  You can call this operation up to 30 times per second per account.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: UpdateDcdnDomainRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: UpdateDcdnDomainResponse
@@ -10962,15 +10990,15 @@
         return TeaCore.from_map(
             dcdn_20180115_models.UpdateDcdnDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def update_dcdn_domain(self, request):
         """
-        >  You can call this operation up to 30 times per second per account.
+        > You can call this operation up to 30 times per second per account.
         
 
         @param request: UpdateDcdnDomainRequest
 
         @return: UpdateDcdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
```

### Comparing `alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115/models.py` & `alibabacloud_dcdn20180115_py2-2.4.0/alibabacloud_dcdn20180115/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2936,32 +2936,34 @@
             temp_model = CreateDcdnSLSRealTimeLogDeliveryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateDcdnSubTaskRequest(TeaModel):
     def __init__(self, domain_name=None, report_ids=None):
-        # [](https://workorder-intl.console.aliyun.com/?spm=5176.2020520001.aliyun_topbar.18.dbd44bd3e4f845#/ticket/createIndex)
+        # The domain names to be tracked. Separate multiple domain names with commas (,). You can specify up to 500 domain names. If you want to specify more than 500 domain names, [submit a ticket](https://workorder-intl.console.aliyun.com/?spm=5176.2020520001.aliyun_topbar.18.dbd44bd3e4f845#/ticket/createIndex).
         # 
-        # **\
-        # 
-        # ****\
+        # > If you do not specify a domain name, the tracking task is created for all domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name  # type: str
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
         self.report_ids = report_ids  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateDcdnSubTaskRequest, self).to_map()
@@ -2982,14 +2984,15 @@
         if m.get('ReportIds') is not None:
             self.report_ids = m.get('ReportIds')
         return self
 
 
 class CreateDcdnSubTaskResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateDcdnSubTaskResponseBody, self).to_map()
@@ -3963,15 +3966,15 @@
             temp_model = DeleteDcdnIpaSpecificConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteDcdnKvRequest(TeaModel):
     def __init__(self, key=None, namespace=None):
-        # The ID of the request.
+        # The name of the key that you want to delete.
         self.key = key  # type: str
         # The namespace that you specify when you call the PutDcdnKvNamespace operation.
         self.namespace = namespace  # type: str
 
     def validate(self):
         pass
 
@@ -3994,15 +3997,15 @@
         if m.get('Namespace') is not None:
             self.namespace = m.get('Namespace')
         return self
 
 
 class DeleteDcdnKvResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The name of the key to delete.
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteDcdnKvResponseBody, self).to_map()
@@ -14907,17 +14910,17 @@
             temp_model = DescribeDcdnDomainRegionDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnDomainStagingConfigRequest(TeaModel):
     def __init__(self, domain_name=None, function_names=None):
-        # The names of the features to query. You can specify multiple features and separate them with commas (,).
+        # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The ID of the request.
+        # The names of the features to query. You can separate multiple features with commas (,).
         self.function_names = function_names  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainStagingConfigRequest, self).to_map()
@@ -14938,16 +14941,17 @@
         if m.get('FunctionNames') is not None:
             self.function_names = m.get('FunctionNames')
         return self
 
 
 class DescribeDcdnDomainStagingConfigResponseBodyDomainConfigsFunctionArgs(TeaModel):
     def __init__(self, arg_name=None, arg_value=None):
-        # The value of the configuration.
+        # The name of the configuration.
         self.arg_name = arg_name  # type: str
+        # The value of the configuration.
         self.arg_value = arg_value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnDomainStagingConfigResponseBodyDomainConfigsFunctionArgs, self).to_map()
@@ -14968,21 +14972,26 @@
         if m.get('ArgValue') is not None:
             self.arg_value = m.get('ArgValue')
         return self
 
 
 class DescribeDcdnDomainStagingConfigResponseBodyDomainConfigs(TeaModel):
     def __init__(self, config_id=None, function_args=None, function_name=None, status=None):
-        # The name of the feature.
+        # The ID of the configuration.
         self.config_id = config_id  # type: str
-        # The name of the configuration.
+        # The following table describes the features.
         self.function_args = function_args  # type: list[DescribeDcdnDomainStagingConfigResponseBodyDomainConfigsFunctionArgs]
-        # The descriptions of a feature.
+        # The name of the feature.
         self.function_name = function_name  # type: str
-        # The ID of the configuration.
+        # The status. Valid values:
+        # 
+        # *   success: The configuration is successful.
+        # *   testing: The configuration is under testing.
+        # *   failed: The task failed.
+        # *   configuring: The feature is being configured.
         self.status = status  # type: str
 
     def validate(self):
         if self.function_args:
             for k in self.function_args:
                 if k:
                     k.validate()
@@ -15019,22 +15028,17 @@
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
 
 
 class DescribeDcdnDomainStagingConfigResponseBody(TeaModel):
     def __init__(self, domain_configs=None, request_id=None):
-        # The status of the feature. Valid values:
-        # 
-        # *   success
-        # *   testing
-        # *   failed
-        # *   configuring
-        self.domain_configs = domain_configs  # type: list[DescribeDcdnDomainStagingConfigResponseBodyDomainConfigs]
         # The configurations of accelerated domain names returned.
+        self.domain_configs = domain_configs  # type: list[DescribeDcdnDomainStagingConfigResponseBodyDomainConfigs]
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.domain_configs:
             for k in self.domain_configs:
                 if k:
                     k.validate()
@@ -18061,28 +18065,19 @@
             temp_model = DescribeDcdnFullDomainsBlockIPHistoryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDcdnHttpsDomainListRequest(TeaModel):
     def __init__(self, keyword=None, page_number=None, page_size=None):
-        # The status of the certificate. Valid values:
-        # 
-        # *   **ok**: The certificate is working as expected.
-        # *   **mismatch**: The certificate does not match the specified domain name.
-        # *   **expired**: The certificate has expired.
-        # *   **expire_soon**: The certificate is about to expire.
+        # The keyword that is used to search for certificates.
         self.keyword = keyword  # type: str
-        # The total number of entries returned.
+        # The number of returned pages. Valid values: **1 to 100000**.
         self.page_number = page_number  # type: int
-        # The type of the certificate. Valid values:
-        # 
-        # *   **free**: A free certificate.
-        # *   **cas**: A certificate that is purchased through Alibaba Cloud SSL Certificates Service.
-        # *   **upload**: A user-uploaded certificate.
+        # The number of entries to return on each page. Valid values: **1 to 500**. Default value: **20**.
         self.page_size = page_size  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnHttpsDomainListRequest, self).to_map()
@@ -18108,29 +18103,37 @@
             self.page_size = m.get('PageSize')
         return self
 
 
 class DescribeDcdnHttpsDomainListResponseBodyCertInfosCertInfo(TeaModel):
     def __init__(self, cert_common_name=None, cert_expire_time=None, cert_name=None, cert_start_time=None,
                  cert_status=None, cert_type=None, cert_update_time=None, domain_name=None):
-        # The certificate information about the domain name.
+        # The returned primary domain name of the certificate.
         self.cert_common_name = cert_common_name  # type: str
-        # The name of the certificate.
+        # The time at which the certificate expires.
         self.cert_expire_time = cert_expire_time  # type: str
-        # The accelerated domain name for which the certificate information was queried.
+        # The name of the certificate.
         self.cert_name = cert_name  # type: str
-        # The time when the certificate expires.
+        # The time at which the certificate became effective.
         self.cert_start_time = cert_start_time  # type: str
-        # The number of pages to return. Valid values: **1 to 100000**.
+        # The status of the certificate. Valid values:
+        # 
+        # *   **ok**: The certificate is working as expected.
+        # *   **mismatch**: The certificate does not match the specified domain name.
+        # *   **expired**: The certificate has expired.
+        # *   **expire_soon**: The certificate is about to expire.
         self.cert_status = cert_status  # type: str
-        # The operation that you want to perform. Set the value to **DescribeDcdnHttpsDomainList**.
+        # The type of the certificate. Valid values:
+        # 
+        # *   **cas**: a certificate that is purchased by using Certificate Management Service
+        # *   **upload**: a custom certificate that you upload
         self.cert_type = cert_type  # type: str
-        # The keyword used for search.
+        # The time at which the certificate was updated.
         self.cert_update_time = cert_update_time  # type: str
-        # The time when the certificate was updated.
+        # The accelerated domain name.
         self.domain_name = domain_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDcdnHttpsDomainListResponseBodyCertInfosCertInfo, self).to_map()
@@ -18207,19 +18210,19 @@
                 temp_model = DescribeDcdnHttpsDomainListResponseBodyCertInfosCertInfo()
                 self.cert_info.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDcdnHttpsDomainListResponseBody(TeaModel):
     def __init__(self, cert_infos=None, request_id=None, total_count=None):
-        # The time when the certificate became effective.
+        # The information about the certificate.
         self.cert_infos = cert_infos  # type: DescribeDcdnHttpsDomainListResponseBodyCertInfos
-        # The returned primary domain name of the certificate.
+        # The ID of the request.
         self.request_id = request_id  # type: str
-        # The number of entries to return on each page. Valid values: **1 to 500**. Default value: **20**.
+        # The total number of entries returned.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.cert_infos:
             self.cert_infos.validate()
 
     def to_map(self):
@@ -32252,17 +32255,17 @@
             temp_model = DescribeRoutineSpecResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeRoutineUserInfoResponseBody(TeaModel):
     def __init__(self, content=None, request_id=None):
-        # The ID of the request.
+        # The content returned by calling the operation.
         self.content = content  # type: dict[str, any]
-        # The operation that you want to perform. Set the value to **DescribeRoutineUserInfo**.
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeRoutineUserInfoResponseBody, self).to_map()
@@ -34892,14 +34895,113 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PutDcdnKvWithHighCapacityResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RefreshDcdnObjectCacheByCacheTagRequest(TeaModel):
+    def __init__(self, cache_tag=None, domain_name=None, force=None):
+        self.cache_tag = cache_tag  # type: str
+        self.domain_name = domain_name  # type: str
+        self.force = force  # type: bool
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(RefreshDcdnObjectCacheByCacheTagRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, refresh_task_id=None, request_id=None):
+        self.refresh_task_id = refresh_task_id  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(RefreshDcdnObjectCacheByCacheTagResponseBody, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RefreshTaskId') is not None:
+            self.refresh_task_id = m.get('RefreshTaskId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class RefreshDcdnObjectCacheByCacheTagResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: RefreshDcdnObjectCacheByCacheTagResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(RefreshDcdnObjectCacheByCacheTagResponse, self).to_map()
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
+            temp_model = RefreshDcdnObjectCacheByCacheTagResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class RefreshDcdnObjectCachesRequest(TeaModel):
     def __init__(self, force=None, object_path=None, object_type=None, owner_id=None, security_token=None):
         # Specifies whether to refresh resources in a directory if the resources are different from the resources in the same directory in the origin server. Default value: false.
         # 
         # *   **true**: refresh all resources in the directory.
         # *   **false**: refresh the changed resources in the directory.
         self.force = force  # type: bool
@@ -35774,15 +35876,15 @@
         if m.get('Functions') is not None:
             self.functions = m.get('Functions')
         return self
 
 
 class SetDcdnDomainStagingConfigResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the region.
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetDcdnDomainStagingConfigResponseBody, self).to_map()
@@ -36943,23 +37045,23 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateDcdnDomainRequest(TeaModel):
     def __init__(self, domain_name=None, owner_id=None, resource_group_id=None, security_token=None, sources=None,
                  top_level_domain=None):
-        # The top-level domain name.
+        # The accelerated domain name. You can specify only one domain name in each call.
         self.domain_name = domain_name  # type: str
         self.owner_id = owner_id  # type: long
-        # The ID of the request.
+        # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
         self.security_token = security_token  # type: str
-        # The accelerated domain name. You can specify only one domain name in each call.
+        # The information about the addresses of origin servers.
         self.sources = sources  # type: str
-        # The operation that you want to perform. Set the value to **UpdateDcdnDomain**.
+        # The top-level domain.
         self.top_level_domain = top_level_domain  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateDcdnDomainRequest, self).to_map()
@@ -36996,15 +37098,15 @@
         if m.get('TopLevelDomain') is not None:
             self.top_level_domain = m.get('TopLevelDomain')
         return self
 
 
 class UpdateDcdnDomainResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The information about the addresses of origin servers.
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateDcdnDomainResponseBody, self).to_map()
```

### Comparing `alibabacloud_dcdn20180115_py2-2.3.0/alibabacloud_dcdn20180115_py2.egg-info/PKG-INFO` & `alibabacloud_dcdn20180115_py2-2.4.0/alibabacloud_dcdn20180115_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dcdn20180115-py2
-Version: 2.3.0
+Version: 2.4.0
 Summary: Alibaba Cloud dcdn (20180115) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dcdn20180115_py2-2.3.0/setup.py` & `alibabacloud_dcdn20180115_py2-2.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dcdn20180115_py2.
 
-Created on 08/04/2024
+Created on 11/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dcdn20180115"
 NAME = "alibabacloud_dcdn20180115_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud dcdn (20180115) SDK Library for Python2"
```

