# Comparing `tmp/okareo-0.0.8.tar.gz` & `tmp/okareo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okareo-0.0.8.tar", max compression
+gzip compressed data, was "okareo-0.0.9.tar", max compression
```

## Comparing `okareo-0.0.8.tar` & `okareo-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     2871 2023-10-09 14:57:24.077136 okareo-0.0.8/README.md
--rw-r--r--   0        0        0     2314 2023-10-09 14:57:24.077136 okareo-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       50 2023-10-09 14:57:24.077136 okareo-0.0.8/src/okareo/__init__.py
--rw-r--r--   0        0        0        0 2023-10-09 14:57:24.077136 okareo-0.0.8/src/okareo/client.py
--rw-r--r--   0        0        0        0 2023-10-09 14:57:24.077136 okareo-0.0.8/src/okareo/common.py
--rw-r--r--   0        0        0        0 2023-10-09 14:57:24.077136 okareo-0.0.8/src/okareo/core.py
--rw-r--r--   0        0        0     2193 2023-10-09 14:57:24.077136 okareo-0.0.8/src/okareo/okareo.py
--rw-r--r--   0        0        0        0 2023-10-09 14:57:24.077136 okareo-0.0.8/src/okareo/py.typed
--rw-r--r--   0        0        0       72 2023-10-09 14:57:24.077136 okareo-0.0.8/src/okareo_api_client/__init__.py
--rw-r--r--   0        0        0      887 2023-10-09 14:57:24.077136 okareo-0.0.8/src/okareo_api_client/api_config.py
--rw-r--r--   0        0        0      449 2023-10-09 14:57:24.077136 okareo-0.0.8/src/okareo_api_client/models/DatapointList.py
--rw-r--r--   0        0        0      326 2023-10-09 14:57:24.077136 okareo-0.0.8/src/okareo_api_client/models/DatapointResponse.py
--rw-r--r--   0        0        0      972 2023-10-09 14:57:24.077136 okareo-0.0.8/src/okareo_api_client/models/DatapointSchema.py
--rw-r--r--   0        0        0      787 2023-10-09 14:57:24.081136 okareo-0.0.8/src/okareo_api_client/models/DatapointSearch.py
--rw-r--r--   0        0        0      227 2023-10-09 14:57:24.081136 okareo-0.0.8/src/okareo_api_client/models/GenerationList.py
--rw-r--r--   0        0        0      303 2023-10-09 14:57:24.081136 okareo-0.0.8/src/okareo_api_client/models/GenerationPayload.py
--rw-r--r--   0        0        0      219 2023-10-09 14:57:24.081136 okareo-0.0.8/src/okareo_api_client/models/GenerationResponse.py
--rw-r--r--   0        0        0      286 2023-10-09 14:57:24.081136 okareo-0.0.8/src/okareo_api_client/models/HTTPValidationError.py
--rw-r--r--   0        0        0      315 2023-10-09 14:57:24.081136 okareo-0.0.8/src/okareo_api_client/models/ModelUnderTestResponse.py
--rw-r--r--   0        0        0      374 2023-10-09 14:57:24.081136 okareo-0.0.8/src/okareo_api_client/models/ModelUnderTestSchema.py
--rw-r--r--   0        0        0      264 2023-10-09 14:57:24.081136 okareo-0.0.8/src/okareo_api_client/models/ProjectResponse.py
--rw-r--r--   0        0        0      275 2023-10-09 14:57:24.081136 okareo-0.0.8/src/okareo_api_client/models/ProjectSchema.py
--rw-r--r--   0        0        0      264 2023-10-09 14:57:24.081136 okareo-0.0.8/src/okareo_api_client/models/ValidationError.py
--rw-r--r--   0        0        0      421 2023-10-09 14:57:24.081136 okareo-0.0.8/src/okareo_api_client/models/__init__.py
--rw-r--r--   0        0        0    13928 2023-10-09 14:57:24.081136 okareo-0.0.8/src/okareo_api_client/services/None_service.py
--rw-r--r--   0        0        0        0 2023-10-09 14:57:24.081136 okareo-0.0.8/src/okareo_api_client/services/__init__.py
--rw-r--r--   0        0        0    14227 2023-10-09 14:57:24.081136 okareo-0.0.8/src/okareo_api_client/services/async_None_service.py
--rw-r--r--   0        0        0     4027 1970-01-01 00:00:00.000000 okareo-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2871 2023-10-09 20:57:03.081800 okareo-0.0.9/README.md
+-rw-r--r--   0        0        0     2314 2023-10-09 20:57:03.085800 okareo-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo/client.py
+-rw-r--r--   0        0        0        0 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo/common.py
+-rw-r--r--   0        0        0        0 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo/core.py
+-rw-r--r--   0        0        0     2193 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo/okareo.py
+-rw-r--r--   0        0        0        0 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo/py.typed
+-rw-r--r--   0        0        0       72 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/__init__.py
+-rw-r--r--   0        0        0      887 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/api_config.py
+-rw-r--r--   0        0        0      449 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/models/DatapointList.py
+-rw-r--r--   0        0        0      326 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/models/DatapointResponse.py
+-rw-r--r--   0        0        0      972 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/models/DatapointSchema.py
+-rw-r--r--   0        0        0      787 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/models/DatapointSearch.py
+-rw-r--r--   0        0        0      227 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/models/GenerationList.py
+-rw-r--r--   0        0        0      303 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/models/GenerationPayload.py
+-rw-r--r--   0        0        0      219 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/models/GenerationResponse.py
+-rw-r--r--   0        0        0      286 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/models/HTTPValidationError.py
+-rw-r--r--   0        0        0      315 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/models/ModelUnderTestResponse.py
+-rw-r--r--   0        0        0      374 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/models/ModelUnderTestSchema.py
+-rw-r--r--   0        0        0      264 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/models/ProjectResponse.py
+-rw-r--r--   0        0        0      275 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/models/ProjectSchema.py
+-rw-r--r--   0        0        0      264 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/models/ValidationError.py
+-rw-r--r--   0        0        0      421 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/models/__init__.py
+-rw-r--r--   0        0        0    13928 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/services/None_service.py
+-rw-r--r--   0        0        0        0 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/services/__init__.py
+-rw-r--r--   0        0        0    14227 2023-10-09 20:57:03.085800 okareo-0.0.9/src/okareo_api_client/services/async_None_service.py
+-rw-r--r--   0        0        0     4027 1970-01-01 00:00:00.000000 okareo-0.0.9/PKG-INFO
```

### Comparing `okareo-0.0.8/README.md` & `okareo-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `okareo-0.0.8/pyproject.toml` & `okareo-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "okareo"
-version = "0.0.8"
+version = "0.0.9"
 description = "Python SDK for intercating with Okareo Cloud APIs"
 authors = [
     "berni <info@okareo.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `okareo-0.0.8/src/okareo/okareo.py` & `okareo-0.0.9/src/okareo/okareo.py`

 * *Files identical despite different names*

### Comparing `okareo-0.0.8/src/okareo_api_client/api_config.py` & `okareo-0.0.9/src/okareo_api_client/api_config.py`

 * *Files identical despite different names*

### Comparing `okareo-0.0.8/src/okareo_api_client/models/DatapointSchema.py` & `okareo-0.0.9/src/okareo_api_client/models/DatapointSchema.py`

 * *Files identical despite different names*

### Comparing `okareo-0.0.8/src/okareo_api_client/models/DatapointSearch.py` & `okareo-0.0.9/src/okareo_api_client/models/DatapointSearch.py`

 * *Files identical despite different names*

### Comparing `okareo-0.0.8/src/okareo_api_client/services/None_service.py` & `okareo-0.0.9/src/okareo_api_client/services/None_service.py`

 * *Files identical despite different names*

### Comparing `okareo-0.0.8/src/okareo_api_client/services/async_None_service.py` & `okareo-0.0.9/src/okareo_api_client/services/async_None_service.py`

 * *Files identical despite different names*

### Comparing `okareo-0.0.8/PKG-INFO` & `okareo-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okareo
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python SDK for intercating with Okareo Cloud APIs
 Home-page: https://okareo-ai.github.io/okareo-python-sdk
 License: MIT
 Author: berni
 Author-email: info@okareo.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

