# Comparing `tmp/ryght_platform_sdk-0.3.7.tar.gz` & `tmp/ryght_platform_sdk-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryght_platform_sdk-0.3.7.tar", max compression
+gzip compressed data, was "ryght_platform_sdk-0.3.8.tar", max compression
```

## Comparing `ryght_platform_sdk-0.3.7.tar` & `ryght_platform_sdk-0.3.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       16 2024-02-02 11:03:05.872282 ryght_platform_sdk-0.3.7/README.md
--rw-r--r--   0        0        0      645 2024-03-28 15:16:02.778966 ryght_platform_sdk-0.3.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-13 18:28:11.113560 ryght_platform_sdk-0.3.7/src/ryght/__init__.py
--rw-r--r--   0        0        0       58 2024-03-13 05:48:02.731588 ryght_platform_sdk-0.3.7/src/ryght/clients/__init__.py
--rw-r--r--   0        0        0    12935 2024-03-28 15:11:02.522805 ryght_platform_sdk-0.3.7/src/ryght/clients/api.py
--rw-r--r--   0        0        0     4655 2024-03-26 22:13:47.025119 ryght_platform_sdk-0.3.7/src/ryght/clients/user.py
--rw-r--r--   0        0        0     2011 2024-03-21 11:17:01.513468 ryght_platform_sdk-0.3.7/src/ryght/configs/__init__.py
--rw-r--r--   0        0        0     8357 2024-03-28 15:13:48.761560 ryght_platform_sdk-0.3.7/src/ryght/configs/api_config.py
--rw-r--r--   0        0        0     3182 2024-03-25 16:52:52.483525 ryght_platform_sdk-0.3.7/src/ryght/configs/api_endpoints.yaml
--rw-r--r--   0        0        0       61 2024-03-13 05:43:00.067020 ryght_platform_sdk-0.3.7/src/ryght/interface/__init__.py
--rw-r--r--   0        0        0     5340 2024-03-20 17:55:57.727098 ryght_platform_sdk-0.3.7/src/ryght/interface/api.py
--rw-r--r--   0        0        0     6379 2024-03-26 22:21:53.881553 ryght_platform_sdk-0.3.7/src/ryght/interface/client.py
--rw-r--r--   0        0        0       77 2024-02-13 18:28:11.115970 ryght_platform_sdk-0.3.7/src/ryght/managers/__init__.py
--rw-r--r--   0        0        0     1656 2024-03-26 22:18:22.520369 ryght_platform_sdk-0.3.7/src/ryght/managers/collections.py
--rw-r--r--   0        0        0     8368 2024-03-20 11:19:15.859848 ryght_platform_sdk-0.3.7/src/ryght/managers/tokens.py
--rw-r--r--   0        0        0      297 2024-03-09 12:48:07.301267 ryght_platform_sdk-0.3.7/src/ryght/models/__init__.py
--rw-r--r--   0        0        0     8970 2024-03-25 17:48:34.446053 ryght_platform_sdk-0.3.7/src/ryght/models/data_models.py
--rw-r--r--   0        0        0       49 2024-02-13 18:28:11.117875 ryght_platform_sdk-0.3.7/src/ryght/requests/__init__.py
--rw-r--r--   0        0        0     3101 2024-03-14 14:41:30.204889 ryght_platform_sdk-0.3.7/src/ryght/requests/http_requestor.py
--rw-r--r--   0        0        0     3845 2024-02-19 11:54:44.707024 ryght_platform_sdk-0.3.7/src/ryght/utils/__init__.py
--rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 ryght_platform_sdk-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-02-02 11:03:05.872282 ryght_platform_sdk-0.3.8/README.md
+-rw-r--r--   0        0        0      645 2024-03-28 19:16:30.588596 ryght_platform_sdk-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-13 18:28:11.113560 ryght_platform_sdk-0.3.8/src/ryght/__init__.py
+-rw-r--r--   0        0        0       58 2024-03-13 05:48:02.731588 ryght_platform_sdk-0.3.8/src/ryght/clients/__init__.py
+-rw-r--r--   0        0        0    12961 2024-03-28 19:14:24.776974 ryght_platform_sdk-0.3.8/src/ryght/clients/api.py
+-rw-r--r--   0        0        0     4655 2024-03-26 22:13:47.025119 ryght_platform_sdk-0.3.8/src/ryght/clients/user.py
+-rw-r--r--   0        0        0     2011 2024-03-21 11:17:01.513468 ryght_platform_sdk-0.3.8/src/ryght/configs/__init__.py
+-rw-r--r--   0        0        0     8357 2024-03-28 15:13:48.761560 ryght_platform_sdk-0.3.8/src/ryght/configs/api_config.py
+-rw-r--r--   0        0        0     3182 2024-03-25 16:52:52.483525 ryght_platform_sdk-0.3.8/src/ryght/configs/api_endpoints.yaml
+-rw-r--r--   0        0        0       61 2024-03-13 05:43:00.067020 ryght_platform_sdk-0.3.8/src/ryght/interface/__init__.py
+-rw-r--r--   0        0        0     5340 2024-03-20 17:55:57.727098 ryght_platform_sdk-0.3.8/src/ryght/interface/api.py
+-rw-r--r--   0        0        0     6379 2024-03-26 22:21:53.881553 ryght_platform_sdk-0.3.8/src/ryght/interface/client.py
+-rw-r--r--   0        0        0       77 2024-02-13 18:28:11.115970 ryght_platform_sdk-0.3.8/src/ryght/managers/__init__.py
+-rw-r--r--   0        0        0     1656 2024-03-26 22:18:22.520369 ryght_platform_sdk-0.3.8/src/ryght/managers/collections.py
+-rw-r--r--   0        0        0     8368 2024-03-20 11:19:15.859848 ryght_platform_sdk-0.3.8/src/ryght/managers/tokens.py
+-rw-r--r--   0        0        0      297 2024-03-09 12:48:07.301267 ryght_platform_sdk-0.3.8/src/ryght/models/__init__.py
+-rw-r--r--   0        0        0     8970 2024-03-25 17:48:34.446053 ryght_platform_sdk-0.3.8/src/ryght/models/data_models.py
+-rw-r--r--   0        0        0       49 2024-02-13 18:28:11.117875 ryght_platform_sdk-0.3.8/src/ryght/requests/__init__.py
+-rw-r--r--   0        0        0     3101 2024-03-14 14:41:30.204889 ryght_platform_sdk-0.3.8/src/ryght/requests/http_requestor.py
+-rw-r--r--   0        0        0     3845 2024-02-19 11:54:44.707024 ryght_platform_sdk-0.3.8/src/ryght/utils/__init__.py
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 ryght_platform_sdk-0.3.8/PKG-INFO
```

### Comparing `ryght_platform_sdk-0.3.7/src/ryght/clients/api.py` & `ryght_platform_sdk-0.3.8/src/ryght/clients/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,16 @@
         }
         headers = self.get_headers()
         headers['Content-Type'] = 'application/json'
         result = self.execute_request(
             method=RequestMethods.POST,
             url=url,
             headers=headers,
-            data=json.dumps(payload)
+            data=json.dumps(payload),
+            timeout=20.0
         )
         if result:
             return CompletionsResponse(**result)
         else:
             return CompletionsResponse().init_with_none()
 
     # Models
```

### Comparing `ryght_platform_sdk-0.3.7/src/ryght/clients/user.py` & `ryght_platform_sdk-0.3.8/src/ryght/clients/user.py`

 * *Files identical despite different names*

### Comparing `ryght_platform_sdk-0.3.7/src/ryght/configs/__init__.py` & `ryght_platform_sdk-0.3.8/src/ryght/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `ryght_platform_sdk-0.3.7/src/ryght/configs/api_config.py` & `ryght_platform_sdk-0.3.8/src/ryght/configs/api_config.py`

 * *Files identical despite different names*

### Comparing `ryght_platform_sdk-0.3.7/src/ryght/configs/api_endpoints.yaml` & `ryght_platform_sdk-0.3.8/src/ryght/configs/api_endpoints.yaml`

 * *Files identical despite different names*

### Comparing `ryght_platform_sdk-0.3.7/src/ryght/interface/api.py` & `ryght_platform_sdk-0.3.8/src/ryght/interface/api.py`

 * *Files identical despite different names*

### Comparing `ryght_platform_sdk-0.3.7/src/ryght/interface/client.py` & `ryght_platform_sdk-0.3.8/src/ryght/interface/client.py`

 * *Files identical despite different names*

### Comparing `ryght_platform_sdk-0.3.7/src/ryght/managers/collections.py` & `ryght_platform_sdk-0.3.8/src/ryght/managers/collections.py`

 * *Files identical despite different names*

### Comparing `ryght_platform_sdk-0.3.7/src/ryght/managers/tokens.py` & `ryght_platform_sdk-0.3.8/src/ryght/managers/tokens.py`

 * *Files identical despite different names*

### Comparing `ryght_platform_sdk-0.3.7/src/ryght/models/data_models.py` & `ryght_platform_sdk-0.3.8/src/ryght/models/data_models.py`

 * *Files identical despite different names*

### Comparing `ryght_platform_sdk-0.3.7/src/ryght/requests/http_requestor.py` & `ryght_platform_sdk-0.3.8/src/ryght/requests/http_requestor.py`

 * *Files identical despite different names*

### Comparing `ryght_platform_sdk-0.3.7/src/ryght/utils/__init__.py` & `ryght_platform_sdk-0.3.8/src/ryght/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ryght_platform_sdk-0.3.7/PKG-INFO` & `ryght_platform_sdk-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryght-platform-sdk
-Version: 0.3.7
+Version: 0.3.8
 Summary: A SDk to use the Ryght Platform features
 Author: sudo-ai
 Requires-Python: >=3.11.7,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
```

