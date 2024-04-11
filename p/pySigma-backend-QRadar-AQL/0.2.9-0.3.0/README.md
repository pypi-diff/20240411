# Comparing `tmp/pysigma_backend_qradar_aql-0.2.9.tar.gz` & `tmp/pysigma_backend_qradar_aql-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_qradar_aql-0.2.9.tar", max compression
+gzip compressed data, was "pysigma_backend_qradar_aql-0.3.0.tar", max compression
```

## Comparing `pysigma_backend_qradar_aql-0.2.9.tar` & `pysigma_backend_qradar_aql-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1088 2023-05-11 10:26:27.440460 pysigma_backend_qradar_aql-0.2.9/LICENSE
--rw-r--r--   0        0        0    27904 2023-11-21 14:00:20.753746 pysigma_backend_qradar_aql-0.2.9/README.md
--rw-r--r--   0        0        0      571 2024-02-01 14:15:14.679528 pysigma_backend_qradar_aql-0.2.9/pyproject.toml
--rw-r--r--   0        0        0    10869 2024-01-31 07:34:12.414638 pysigma_backend_qradar_aql-0.2.9/sigma/backends/QRadarAQL/QRadarAQL.py
--rw-r--r--   0        0        0      251 2023-06-12 15:14:20.587205 pysigma_backend_qradar_aql-0.2.9/sigma/backends/QRadarAQL/__init__.py
--rw-r--r--   0        0        0     4026 2023-11-20 13:36:41.782729 pysigma_backend_qradar_aql-0.2.9/sigma/mapping/fields.py
--rw-r--r--   0        0        0    11407 2023-09-21 07:51:28.830818 pysigma_backend_qradar_aql-0.2.9/sigma/mapping/logsources.py
--rw-r--r--   0        0        0     2323 2023-09-21 07:51:28.831225 pysigma_backend_qradar_aql-0.2.9/sigma/mapping/products.py
--rw-r--r--   0        0        0     1109 2023-09-21 07:51:28.831607 pysigma_backend_qradar_aql-0.2.9/sigma/mapping/services.py
--rw-r--r--   0        0        0     7773 2023-09-21 07:51:28.832620 pysigma_backend_qradar_aql-0.2.9/sigma/pipelines/QRadarAQL/QRadarAQL.py
--rw-r--r--   0        0        0      231 2023-09-21 07:51:28.833683 pysigma_backend_qradar_aql-0.2.9/sigma/pipelines/QRadarAQL/__init__.py
--rw-r--r--   0        0        0       53 2023-09-21 15:33:24.168146 pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/.git
--rw-r--r--   0        0        0     1088 2023-09-21 15:33:24.250672 pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/LICENSE
--rw-r--r--   0        0        0     6894 2024-02-01 12:37:06.417482 pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/QRadarBackend.py
--rw-r--r--   0        0        0     1938 2024-01-25 14:58:22.484123 pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/QRadarFieldsPipeline.py
--rw-r--r--   0        0        0     6746 2024-01-25 14:58:22.485065 pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/QRadarPayloadPipeline.py
--rw-r--r--   0        0        0     3439 2024-01-25 14:58:22.486784 pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/QRadarPipeline.py
--rw-r--r--   0        0        0      787 2023-09-21 15:33:24.251943 pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/README.md
--rw-r--r--   0        0        0     1744 2024-01-25 14:58:22.488050 pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/generate_readme_mapping.py
--rw-r--r--   0        0        0    35331 2023-09-21 15:33:24.252727 pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/poetry.lock
--rw-r--r--   0        0        0      529 2023-09-21 15:33:24.252984 pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/pyproject.toml
--rw-r--r--   0        0        0    28713 1970-01-01 00:00:00.000000 pysigma_backend_qradar_aql-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-11 10:26:27.440460 pysigma_backend_qradar_aql-0.3.0/LICENSE
+-rw-r--r--   0        0        0    27904 2023-11-21 14:00:20.753746 pysigma_backend_qradar_aql-0.3.0/README.md
+-rw-r--r--   0        0        0      571 2024-04-11 08:48:58.073386 pysigma_backend_qradar_aql-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    10869 2024-01-31 07:34:12.414638 pysigma_backend_qradar_aql-0.3.0/sigma/backends/QRadarAQL/QRadarAQL.py
+-rw-r--r--   0        0        0      251 2023-06-12 15:14:20.587205 pysigma_backend_qradar_aql-0.3.0/sigma/backends/QRadarAQL/__init__.py
+-rw-r--r--   0        0        0     4026 2023-11-20 13:36:41.782729 pysigma_backend_qradar_aql-0.3.0/sigma/mapping/fields.py
+-rw-r--r--   0        0        0    11407 2023-09-21 07:51:28.830818 pysigma_backend_qradar_aql-0.3.0/sigma/mapping/logsources.py
+-rw-r--r--   0        0        0     2323 2023-09-21 07:51:28.831225 pysigma_backend_qradar_aql-0.3.0/sigma/mapping/products.py
+-rw-r--r--   0        0        0     1109 2023-09-21 07:51:28.831607 pysigma_backend_qradar_aql-0.3.0/sigma/mapping/services.py
+-rw-r--r--   0        0        0     7773 2023-09-21 07:51:28.832620 pysigma_backend_qradar_aql-0.3.0/sigma/pipelines/QRadarAQL/QRadarAQL.py
+-rw-r--r--   0        0        0      231 2023-09-21 07:51:28.833683 pysigma_backend_qradar_aql-0.3.0/sigma/pipelines/QRadarAQL/__init__.py
+-rw-r--r--   0        0        0       53 2023-09-21 15:33:24.168146 pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/.git
+-rw-r--r--   0        0        0     1088 2023-09-21 15:33:24.250672 pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/LICENSE
+-rw-r--r--   0        0        0     6894 2024-04-11 09:05:56.016782 pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/QRadarBackend.py
+-rw-r--r--   0        0        0     1938 2024-01-25 14:58:22.484123 pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/QRadarFieldsPipeline.py
+-rw-r--r--   0        0        0     6746 2024-01-25 14:58:22.485065 pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/QRadarPayloadPipeline.py
+-rw-r--r--   0        0        0     3895 2024-04-11 09:05:56.019170 pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/QRadarPipeline.py
+-rw-r--r--   0        0        0      787 2023-09-21 15:33:24.251943 pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/README.md
+-rw-r--r--   0        0        0     1744 2024-01-25 14:58:22.488050 pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/generate_readme_mapping.py
+-rw-r--r--   0        0        0    35331 2023-09-21 15:33:24.252727 pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/poetry.lock
+-rw-r--r--   0        0        0      539 2024-04-11 09:03:42.327659 pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/pyproject.toml
+-rw-r--r--   0        0        0    28713 1970-01-01 00:00:00.000000 pysigma_backend_qradar_aql-0.3.0/PKG-INFO
```

### Comparing `pysigma_backend_qradar_aql-0.2.9/LICENSE` & `pysigma_backend_qradar_aql-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.2.9/README.md` & `pysigma_backend_qradar_aql-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.2.9/pyproject.toml` & `pysigma_backend_qradar_aql-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "pySigma-backend-QRadar-AQL"
-version = "0.2.9"
+version = "0.3.0"
 description = "pySigma QRadarAQL backend"
 authors = ["IBM <noaakless@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/IBM/pySigma-backend-QRadar-AQL"
 packages = [
     { include = "sigma" }
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pysigma = ">=0.9.8, <0.11.0"
+pysigma = ">=0.9.8, <0.12.0"
 regex = "^2023.12.25"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 coverage = "^7.2.5"
```

### Comparing `pysigma_backend_qradar_aql-0.2.9/sigma/backends/QRadarAQL/QRadarAQL.py` & `pysigma_backend_qradar_aql-0.3.0/sigma/backends/QRadarAQL/QRadarAQL.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.2.9/sigma/mapping/fields.py` & `pysigma_backend_qradar_aql-0.3.0/sigma/mapping/fields.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.2.9/sigma/mapping/logsources.py` & `pysigma_backend_qradar_aql-0.3.0/sigma/mapping/logsources.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.2.9/sigma/mapping/products.py` & `pysigma_backend_qradar_aql-0.3.0/sigma/mapping/products.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.2.9/sigma/mapping/services.py` & `pysigma_backend_qradar_aql-0.3.0/sigma/mapping/services.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.2.9/sigma/pipelines/QRadarAQL/QRadarAQL.py` & `pysigma_backend_qradar_aql-0.3.0/sigma/pipelines/QRadarAQL/QRadarAQL.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/LICENSE` & `pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/QRadarBackend.py` & `pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/QRadarBackend.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/QRadarFieldsPipeline.py` & `pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/QRadarFieldsPipeline.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/QRadarPayloadPipeline.py` & `pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/QRadarPayloadPipeline.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/QRadarPipeline.py` & `pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/QRadarPipeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Optional, Union, Iterable, List, Pattern
 
 from sigma.processing.transformations import SetStateTransformation, \
     FieldMappingTransformation
 
 # See https://sigmahq-pysigma.readthedocs.io/en/latest/Processing_Pipelines.html
 # for further documentation.
-from sigma.rule import SigmaDetection, SigmaRule
+from sigma.rule import SigmaDetection, SigmaRule, SigmaLogSource
 from sigma.types import SigmaType
 
 IPV4 = "ipv4"
 IPV6 = "ipv6"
 
 
 def is_ipv6(val):
@@ -58,43 +58,58 @@
     set the logsources values from the field devicetype in state, to use it in the
     backend's finalize query
     """
     device_type_field_name: str
     log_source_mapping: dict
 
     def device_type_mapping(
-            self, field: str, val: SigmaType
-    ) -> Optional[Union[SigmaType, Iterable[SigmaType]]]:
+            self, field: str, val: SigmaType, rule_log_source: SigmaLogSource
+    ) -> Optional[int]:
         log_sources = self.log_source_mapping
         str_value = str(val)
         if field == self.device_type_field_name:
             if str_value in log_sources:
                 return log_sources[str_value]
+            elif rule_log_source in SigmaLogSource(
+                    product='ibm_qradar_suite', service="log_insights"
+            ):
+                return int(str_value)
             warnings.warn(
                 f"'{val}' is not a supported log source type and therefore is being "
                 f"removed"
             )
             return None
 
-    def detection_log_sources(self, detection: SigmaDetection, device_types: list):
+    def detection_log_sources(
+            self, detection: SigmaDetection,
+            device_types: list,
+            rule_log_source: SigmaLogSource
+    ):
         for i, detection_item in enumerate(detection.detection_items):
             if isinstance(detection_item,
                           SigmaDetection):  # recurse into nested detection items
-                self.detection_log_sources(detection_item, device_types)
+                self.detection_log_sources(
+                    detection_item, device_types, rule_log_source
+                )
             else:
                 for value in detection_item.value:
-                    res = self.device_type_mapping(detection_item.field, value)
+                    res = self.device_type_mapping(
+                        detection_item.field, value, rule_log_source
+                    )
                     if res:
                         if isinstance(res, Iterable) and not isinstance(res, SigmaType):
                             device_types.extend(res)
                         else:
                             device_types.append(res)
                     self.processing_item_applied(detection_item)
         return device_types
 
     def apply(self, pipeline, rule: SigmaRule) -> None:
         device_types = []
         for detection in rule.detection.detections.values():
-            log_source = self.detection_log_sources(detection, device_types) or []
+            log_source = (
+                    self.detection_log_sources(detection, device_types, rule.logsource)
+                    or []
+            )
             device_types.extend(log_source)
         self.val = device_types
         super().apply(pipeline, rule)
```

### Comparing `pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/README.md` & `pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/README.md`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/generate_readme_mapping.py` & `pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/generate_readme_mapping.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/poetry.lock` & `pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/poetry.lock`

 * *Files identical despite different names*

### Comparing `pysigma_backend_qradar_aql-0.2.9/sigma/pySigma_QRadar_base/pyproject.toml` & `pysigma_backend_qradar_aql-0.3.0/sigma/pySigma_QRadar_base/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 packages = [
     { include = "sigma" }
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pysigma = "^0.9.6"
+pysigma = ">=0.9.6, <0.12.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 coverage = "^7.2.5"
 
 [build-system]
```

### Comparing `pysigma_backend_qradar_aql-0.2.9/PKG-INFO` & `pysigma_backend_qradar_aql-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pySigma-backend-QRadar-AQL
-Version: 0.2.9
+Version: 0.3.0
 Summary: pySigma QRadarAQL backend
 Home-page: https://github.com/IBM/pySigma-backend-QRadar-AQL
 License: MIT
 Author: IBM
 Author-email: noaakless@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pysigma (>=0.9.8,<0.11.0)
+Requires-Dist: pysigma (>=0.9.8,<0.12.0)
 Requires-Dist: regex (>=2023.12.25,<2024.0.0)
 Project-URL: Repository, https://github.com/IBM/pySigma-backend-QRadar-AQL
 Description-Content-Type: text/markdown
 
 # `PySigma QRadar AQL`
 This is the QRadar AQL backend for [pySigma](https://github.com/SigmaHQ/pySigma) 
 which parses and converts [Sigma](https://github.com/SigmaHQ/sigma) Rules into
```

